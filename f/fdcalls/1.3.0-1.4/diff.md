# Comparing `tmp/fdcalls-1.3.0-py3-none-any.whl.zip` & `tmp/fdcalls-1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4899 bytes, number of entries: 7
+Zip file size: 5115 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 23-May-08 12:39 fdcalls/__init__.py
--rw-r--r--  2.0 unx    16413 b- defN 23-May-11 09:19 fdcalls/fdcalls.py
--rw-r--r--  2.0 unx      276 b- defN 23-May-11 10:07 fdcalls-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 10:07 fdcalls-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-May-11 10:07 fdcalls-1.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-11 10:07 fdcalls-1.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      540 b- defN 23-May-11 10:07 fdcalls-1.3.0.dist-info/RECORD
-7 files, 17379 bytes uncompressed, 3935 bytes compressed:  77.4%
+-rw-r--r--  2.0 unx    15747 b- defN 23-May-13 06:16 fdcalls/fdcalls.py
+-rw-r--r--  2.0 unx      274 b- defN 23-May-15 13:44 fdcalls-1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 13:44 fdcalls-1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-May-15 13:44 fdcalls-1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-15 13:44 fdcalls-1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      530 b- defN 23-May-15 13:44 fdcalls-1.4.dist-info/RECORD
+7 files, 16701 bytes uncompressed, 4171 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: fdcalls/__init__.py
 Comment: 
 
 Filename: fdcalls/fdcalls.py
 Comment: 
 
-Filename: fdcalls-1.3.0.dist-info/METADATA
+Filename: fdcalls-1.4.dist-info/METADATA
 Comment: 
 
-Filename: fdcalls-1.3.0.dist-info/WHEEL
+Filename: fdcalls-1.4.dist-info/WHEEL
 Comment: 
 
-Filename: fdcalls-1.3.0.dist-info/entry_points.txt
+Filename: fdcalls-1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: fdcalls-1.3.0.dist-info/top_level.txt
+Filename: fdcalls-1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: fdcalls-1.3.0.dist-info/RECORD
+Filename: fdcalls-1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fdcalls/fdcalls.py

```diff
@@ -74,23 +74,14 @@
 def get_path_by_filename(filename, file_system_path):
     output = subprocess.check_output(['find', file_system_path, '-name', filename]).decode('utf-8')
     for line in output.split('\n'):
         return line
 
 # Obtain relevant dynamic link library names
 def get_dynamic_libraries(r2fd, file_system_path):
-    '''
-    output = subprocess.check_output(['readelf', '-d', target_file_path]).decode('utf-8')
-    libraries = []
-    for line in output.split('\n'):
-        if 'Shared library' in line:
-            library = line.split('[')[-1].split(']')[0]
-            library = get_path_by_filename(library, file_system_path)
-            libraries.append(library)
-    '''
     libraries = []
     libs = r2fd.cmdj('ilj')
     for lib in libs:
         library = get_path_by_filename(lib, file_system_path)
         libraries.append(library)
 
     return libraries
@@ -124,97 +115,104 @@
     return r2fd
 
 # get architecture of binary
 def get_architecture(r2fd):
     info = json.loads(r2fd.cmd('iIj'))
     return info["arch"]
 
+# get endian of binary
+def get_endian(r2fd):
+    info = json.loads(r2fd.cmd('iIj'))
+    return info["endian"]
+
+# get the function in .got
+def get_function_name_by_objdump(start, end, filepath, arch, endian):
+    if arch == 'arm':
+        obj = 'arm-linux-gnueabi-objdump'
+    elif arch == 'mips':
+        if endian == 'little':
+            obj = 'mipsel-linux-gnu-objdump'
+        else:
+            obj = 'mips-linux-gnu-objdump'
+    else:
+        return ''
+    output = subprocess.check_output([obj, '-d', filepath, f'--start-address={start}', f'--stop-address={end}']).decode('utf-8')
+    for line in output.split('\n'):
+        if '@plt>:' in line:
+            fun = line[line.find('<')+1:line.find('@plt>:')]
+            return fun
+    return ''
+
+# get addr from disasm
+'''
+for example:
+    0x00001a10      f0f6bce5       ldr pc, [ip, 0x6f0]!
+    -> 0x00001a10
+'''
+def get_local_addr(line_str):
+    addr = line_str[line_str.find('0x'):line_str.find('0x')+10]
+    return addr
+
 # Obtain the function called internally from the function
 '''
 for example:
     int FunA(){
         system(...);
         printf(...);
     }
     we will get:
     function_called_functions[A] = ['system', 'printf']
 
     differnet arch may be a little difference while coding
 '''
-def get_functions_called(r2fd, filename, arch):
+def get_functions_called(r2fd, filename, arch, endian):
 
     function_called_functions = {}
     functions = []
     function_name = ''
     length = 0
     
-    if arch == 'arm':
-        for fun in functions_self_defined[filename]:
-            # print(fun)
-            functions = []
-            disassembly = r2fd.cmd(f'pdf @ {fun} 2>/dev/null')
-            for line in disassembly.split('\n'):
-                function_name = ''
-                if 'sym' in line:
-                    # print(line)
-                    line1 = line[line.rfind('sym'):]
-                    if line1.find(' ') != -1:
-                        length = line1.find(' ')
-                    else:
-                        length = len(line1)
-                    # print(length)
-                    # print(line[line.find('sym'):line.find('sym')+length])
-                    function_name = line[line.find('sym'):line.find('sym')+length]
-                elif 'fcn' in line:
-                    # print(line)
-                    line1 = line[line.find('fcn'):]
-                    if line1.find(' ') != -1:
-                        length = line1.find(' ')
-                    else:
-                        length = len(line1)
-                    # print(length)
-                    # print(line[line.find('fcn'):line.find('fcn')+length])
-                    function_name = line[line.find('fcn'):line.find('fcn')+length]
-                if function_name != '' and function_name!=fun and function_name not in functions:
-                    functions.append(function_name)
-            function_called_functions[fun] = functions
-            # print(function_called_functions[fun])
-        # print(function_called_functions)
-    if arch == 'mips':
-        for fun in functions_self_defined[filename]:
-            # print(fun)
-            functions = []
-            disassembly = r2fd.cmd(f'pdf @ {fun} 2>/dev/null')
-            for line in disassembly.split('\n'):
-                function_name = ''
-                if 'sym' in line and 'XREF' not in line:
-                    # print(line)
-                    line1 = line[line.rfind('sym'):]
-                    if line1.find(' ') != -1:
-                        length = line1.find(' ')
-                    else:
-                        length = len(line1)
-                    # print(length)
-                    # print(line[line.find('sym'):line.find('sym')+length])
-                    function_name = line[line.find('sym'):line.find('sym')+length]
-                elif 'fcn' in line and 'XREF' not in line:
-                    # print(line)
-                    line1 = line[line.find('fcn'):]
-                    if line1.find(' ') != -1:
-                        length = line1.find(' ')
-                    else:
-                        length = len(line1)
-                    # print(length)
-                    # print(line[line.find('fcn'):line.find('fcn')+length])
-                    function_name = line[line.find('fcn'):line.find('fcn')+length]
-                if function_name != '' and function_name!=fun and function_name not in functions:
-                    functions.append(function_name)
-            function_called_functions[fun] = functions
-            # print(function_called_functions[fun])
-        # print(function_called_functions)
+    for fun in functions_self_defined[filename]:
+        # print(fun)
+        functions = []
+        disassembly = r2fd.cmd(f'pdf @ {fun} 2>/dev/null')
+        for line in disassembly.split('\n'):
+            function_name = ''
+            end = start = 0
+            if 'sym' in line and 'XREF' not in line:
+                # print(line)
+                line1 = line[line.rfind('sym'):]
+                if line1.find(' ') != -1:
+                    length = line1.find(' ')
+                else:
+                    length = len(line1)
+                # print(length)
+                # print(line[line.find('sym'):line.find('sym')+length])
+                function_name = line[line.find('sym'):line.find('sym')+length]
+            elif 'fcn' in line and 'XREF' not in line:
+                # print(line)
+                line1 = line[line.find('fcn'):]
+                if line1.find(' ') != -1:
+                    length = line1.find(' ')
+                else:
+                    length = len(line1)
+                # print(length)
+                # print(line[line.find('fcn'):line.find('fcn')+length])
+                function_name = line[line.find('fcn'):line.find('fcn')+length]
+            elif 'ldr pc, [ip, ' in line:
+                end = int(get_local_addr(line), 16)
+                start = end - 0x8
+                output = get_function_name_by_objdump(start, end+4, filename, arch, endian)
+                if output !='':
+                    function_name = 'sym.' + output
+            if function_name != '' and function_name!=fun and function_name not in functions:
+                functions.append(function_name)
+        function_called_functions[fun] = functions
+        # print(function_called_functions[fun])
+    # print(function_called_functions)
     return function_called_functions
 
 # Obtaining a dangerous function call chain
 '''
 for example:
     int FunA(){
         FunB();
@@ -298,28 +296,28 @@
         if 'sym.imp' in fun:
             fun = fun.replace('sym.imp', 'sym')
             if fun in function_to_library.keys():
             	print('[' + add_colour(function_to_library[fun], 'cyan') + '] ' + add_colour(fun, 'yellow'))
 
 def main():
     parser = argparse.ArgumentParser(description="fdcalls to help analysis")
-    parser.version = "1.3"
+    parser.version = "1.4"
 
     parser.add_argument('-b', '--target_binary_path', type=str, default='', help='path to target binary')
     parser.add_argument('-d', '--file_system_directory_path', type=str, default='', help='path to firmware file system directory')
     parser.add_argument('-l', '--level', type=int, default=0, help='level of analysis')
     parser.add_argument('-v', action='version', help='print the version and exit')
     args = parser.parse_args()
 
     target_filepath = args.target_binary_path
     file_system_path = args.file_system_directory_path
     level = args.level
     
     if target_filepath == '':
-        print('./dcalls.py -b [path/to/target_binary] -d [path/to/file_system_dir] -a [arch] -l [level=0]')
+        print('fdcalls -b [path/to/target_binary] -d [path/to/file_system_dir] -a [arch] -l [level=0]')
         exit(0)
     
     init()
 
     print("[*] Collecting and analysing binaries ...")
     r2_fd[target_filepath] = r2_start_analysis(target_filepath)
     dynamic_libraries[target_filepath] = get_dynamic_libraries(r2_fd[target_filepath], file_system_path)
@@ -337,14 +335,15 @@
         if f not in dynamic_libraries.keys():
             r2_fd[f] = r2_start_analysis(f)
             dynamic_libraries[f] = get_dynamic_libraries(r2_fd[f], file_system_path)
             # print(f + "=> ", end = '')
             # print(get_dynamic_libraries(r2_fd[f], file_system_path))
     # print(all_used_dynamic_libraries)
     architecture = get_architecture(r2_fd[target_filepath])
+    endian = get_endian(r2_fd[target_filepath])
     print("[+] Collect and analyse success")
 
     print("[*] Identifying functions in elf and libraries ...")
     functions_other_defined[target_filepath] = get_function_names(r2_fd[target_filepath], 0)
     for f in all_used_dynamic_libraries:
         functions_other_defined[f] = get_function_names(r2_fd[f], 0)
     # print(functions_other_defined)
@@ -357,17 +356,17 @@
     # print(functions_self_defined['./bin/pucfu'])
     # print(functions_self_defined)
     # print(function_to_library)
     print("[+] Identifying functions success")
     
     print("[*] Enumerateing call paths in libraries ...")
     for lib in all_used_dynamic_libraries:
-        libraries_called_functions[lib] = get_functions_called(r2_fd[lib] ,lib, architecture)
+        libraries_called_functions[lib] = get_functions_called(r2_fd[lib] ,lib, architecture, endian)
         # print(lib)
-        # print(get_functions_called(r2_fd[lib] ,lib, architecture))
+        # print(get_functions_called(r2_fd[lib] ,lib, architecture, endian))
     # print(libraries_called_functions)
     print("[+] Enumerateing call paths in libraries success")
 
     # Search dangerous functions and add them to dangerous_functions
     print("[*] Searching for dangerous functions in libraries ...")
     dangerous_functions_now_len = len(dangerous_functions)
     dangerous_functions_old_len = 0
```

