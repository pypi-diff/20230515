# Comparing `tmp/copytool-0.11.tar.gz` & `tmp/copytool-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copytool-0.11.tar", last modified: Sun May 14 21:22:35 2023, max compression
+gzip compressed data, was "copytool-0.12.tar", last modified: Mon May 15 02:26:48 2023, max compression
```

## Comparing `copytool-0.11.tar` & `copytool-0.12.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 21:22:35.357171 copytool-0.11/
--rw-rw-rw-   0        0        0     1148 2023-05-14 21:22:26.000000 copytool-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      274 2023-05-14 21:22:24.000000 copytool-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     1868 2023-05-14 21:22:35.357171 copytool-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     1270 2023-05-13 08:11:38.000000 copytool-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 21:22:35.351186 copytool-0.11/copytool/
--rw-rw-rw-   0        0        0     1270 2023-05-13 08:11:38.000000 copytool-0.11/copytool/README.md
--rw-rw-rw-   0        0        0     7946 2023-05-14 21:19:43.000000 copytool-0.11/copytool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 21:22:35.356173 copytool-0.11/copytool/buffcall/
--rw-rw-rw-   0        0        0       30 2023-05-13 08:11:38.000000 copytool-0.11/copytool/buffcall/__init__.py
--rw-rw-rw-   0        0        0    17920 2023-05-13 08:11:38.000000 copytool-0.11/copytool/buffcall/buffercalc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    17920 2023-05-13 08:11:38.000000 copytool-0.11/copytool/buffercalc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0      514 2023-05-13 08:11:38.000000 copytool-0.11/copytool/buffercalc.pyx
--rw-rw-rw-   0        0        0       69 2023-05-14 21:22:34.000000 copytool-0.11/copytool/requirements.txt
--rw-rw-rw-   0        0        0     8933 2023-05-14 21:22:34.000000 copytool-0.11/copytool/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-14 21:22:35.354179 copytool-0.11/copytool.egg-info/
--rw-rw-rw-   0        0        0     1868 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-14 21:22:35.358168 copytool-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-05-14 21:22:34.000000 copytool-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:26:48.380457 copytool-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-05-15 02:26:40.000000 copytool-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      274 2023-05-15 02:26:39.000000 copytool-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     2265 2023-05-15 02:26:48.380457 copytool-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1667 2023-05-15 02:26:10.000000 copytool-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 02:26:48.375470 copytool-0.12/copytool/
+-rw-rw-rw-   0        0        0     1667 2023-05-15 02:26:10.000000 copytool-0.12/copytool/README.md
+-rw-rw-rw-   0        0        0    13706 2023-05-15 02:25:55.000000 copytool-0.12/copytool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 02:26:48.379459 copytool-0.12/copytool/buffcall/
+-rw-rw-rw-   0        0        0       30 2023-05-13 08:11:38.000000 copytool-0.12/copytool/buffcall/__init__.py
+-rw-rw-rw-   0        0        0    18432 2023-05-14 23:19:29.000000 copytool-0.12/copytool/buffcall/buffercalc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0    18432 2023-05-14 23:19:29.000000 copytool-0.12/copytool/buffercalc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0      573 2023-05-14 23:19:18.000000 copytool-0.12/copytool/buffercalc.pyx
+-rw-rw-rw-   0        0        0       69 2023-05-15 02:26:47.000000 copytool-0.12/copytool/requirements.txt
+-rw-rw-rw-   0        0        0     8933 2023-05-15 02:26:47.000000 copytool-0.12/copytool/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-15 02:26:48.378461 copytool-0.12/copytool.egg-info/
+-rw-rw-rw-   0        0        0     2265 2023-05-15 02:26:48.000000 copytool-0.12/copytool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-05-15 02:26:48.000000 copytool-0.12/copytool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 02:26:48.000000 copytool-0.12/copytool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-15 02:26:48.000000 copytool-0.12/copytool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 02:26:48.000000 copytool-0.12/copytool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-15 02:26:48.380457 copytool-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-05-15 02:26:47.000000 copytool-0.12/setup.py
```

### Comparing `copytool-0.11/LICENSE.rst` & `copytool-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `copytool-0.11/PKG-INFO` & `copytool-0.12/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copytool
-Version: 0.11
+Version: 0.12
 Summary: copytool copies files hell-bent for leather
 Home-page: https://github.com/hansalemaos/copytool
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: copy
 Classifier: Development Status :: 4 - Beta
@@ -21,34 +21,49 @@
 ### Tested+compiled against Windows 10 / Python 3.10 / Anaconda
 
 
 TeraCopy needs 4 minutes, copytool does it 6 seconds
 ![](https://github.com/hansalemaos/copytool/blob/main/fastcopyscreenshot.png?raw=true)
 
 ## CLI
-Compiled EXE: [](https://github.com/hansalemaos/copytool/raw/main/copytool.exe)
+Compiled EXE: 
+[](https://github.com/hansalemaos/copytool/raw/main/copytool.zip)
+[](https://github.com/hansalemaos/copytool/raw/main/copytool.z01)
 
       Example: copytool --src "C:\ProgramData\anaconda3\envs" --dst "e:\envbackup" --use_tqdm 1 --copy_date 1 --copy_permission 0 --overwrite 1
       --src                     str         (source folder)
       --dst                     str         (destination folder)
       --log                     str  ""     (csv log)
       --copy_date               int  0      (copy date stats)
       --copy_permission         int  0      (copy permissions)
       --use_tqdm                int  1      (show progress bar)
       --overwrite               int  1      (overwrite existing files in dst)
+      --use_uffs                int  1      (use uffs to get a list of files)
 
 
 ## Python
 
 ```python
 # pip install copytool 
 from copytool import get_all_files_on_hdd_and_copy
 get_all_files_on_hdd_and_copy(
     src = r"C:\path",
     dst = r"e:\dest",
     log = "c:\\copylog.csv",
-    copy_date= 1,
+    copy_date= 0,
     copy_permission= 0,
     use_tqdm = 1,
     overwrite = 1,
+    use_uffs = 1
+)     
+
+get_all_files_on_hdd_and_copy(
+    src = r"C:\path",
+    dst = r"e:\dest",
+    log = "",
+    copy_date= 0,
+    copy_permission= 0,
+    use_tqdm = 1,
+    overwrite = 1,
+    use_uffs = 0 # no logging without uffs 
 )     
 ```
```

### Comparing `copytool-0.11/README.md` & `copytool-0.12/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,49 @@
 ### Tested+compiled against Windows 10 / Python 3.10 / Anaconda
 
 
 TeraCopy needs 4 minutes, copytool does it 6 seconds
 ![](https://github.com/hansalemaos/copytool/blob/main/fastcopyscreenshot.png?raw=true)
 
 ## CLI
-Compiled EXE: [](https://github.com/hansalemaos/copytool/raw/main/copytool.exe)
+Compiled EXE: 
+[](https://github.com/hansalemaos/copytool/raw/main/copytool.zip)
+[](https://github.com/hansalemaos/copytool/raw/main/copytool.z01)
 
       Example: copytool --src "C:\ProgramData\anaconda3\envs" --dst "e:\envbackup" --use_tqdm 1 --copy_date 1 --copy_permission 0 --overwrite 1
       --src                     str         (source folder)
       --dst                     str         (destination folder)
       --log                     str  ""     (csv log)
       --copy_date               int  0      (copy date stats)
       --copy_permission         int  0      (copy permissions)
       --use_tqdm                int  1      (show progress bar)
       --overwrite               int  1      (overwrite existing files in dst)
+      --use_uffs                int  1      (use uffs to get a list of files)
 
 
 ## Python
 
 ```python
 # pip install copytool 
 from copytool import get_all_files_on_hdd_and_copy
 get_all_files_on_hdd_and_copy(
     src = r"C:\path",
     dst = r"e:\dest",
     log = "c:\\copylog.csv",
-    copy_date= 1,
+    copy_date= 0,
     copy_permission= 0,
     use_tqdm = 1,
     overwrite = 1,
+    use_uffs = 1
+)     
+
+get_all_files_on_hdd_and_copy(
+    src = r"C:\path",
+    dst = r"e:\dest",
+    log = "",
+    copy_date= 0,
+    copy_permission= 0,
+    use_tqdm = 1,
+    overwrite = 1,
+    use_uffs = 0 # no logging without uffs 
 )     
 ```
```

### Comparing `copytool-0.11/copytool/README.md` & `copytool-0.12/copytool/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,49 @@
 ### Tested+compiled against Windows 10 / Python 3.10 / Anaconda
 
 
 TeraCopy needs 4 minutes, copytool does it 6 seconds
 ![](https://github.com/hansalemaos/copytool/blob/main/fastcopyscreenshot.png?raw=true)
 
 ## CLI
-Compiled EXE: [](https://github.com/hansalemaos/copytool/raw/main/copytool.exe)
+Compiled EXE: 
+[](https://github.com/hansalemaos/copytool/raw/main/copytool.zip)
+[](https://github.com/hansalemaos/copytool/raw/main/copytool.z01)
 
       Example: copytool --src "C:\ProgramData\anaconda3\envs" --dst "e:\envbackup" --use_tqdm 1 --copy_date 1 --copy_permission 0 --overwrite 1
       --src                     str         (source folder)
       --dst                     str         (destination folder)
       --log                     str  ""     (csv log)
       --copy_date               int  0      (copy date stats)
       --copy_permission         int  0      (copy permissions)
       --use_tqdm                int  1      (show progress bar)
       --overwrite               int  1      (overwrite existing files in dst)
+      --use_uffs                int  1      (use uffs to get a list of files)
 
 
 ## Python
 
 ```python
 # pip install copytool 
 from copytool import get_all_files_on_hdd_and_copy
 get_all_files_on_hdd_and_copy(
     src = r"C:\path",
     dst = r"e:\dest",
     log = "c:\\copylog.csv",
-    copy_date= 1,
+    copy_date= 0,
     copy_permission= 0,
     use_tqdm = 1,
     overwrite = 1,
+    use_uffs = 1
+)     
+
+get_all_files_on_hdd_and_copy(
+    src = r"C:\path",
+    dst = r"e:\dest",
+    log = "",
+    copy_date= 0,
+    copy_permission= 0,
+    use_tqdm = 1,
+    overwrite = 1,
+    use_uffs = 0 # no logging without uffs 
 )     
 ```
```

### Comparing `copytool-0.11/copytool/buffercalc.pyx` & `copytool-0.12/copytool/buffercalc.pyx`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # cython: language_level=3
 import cython
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-@cython.nogil
-cpdef get_mu(buffer):
+cpdef get_mu(buffer_):
+    cdef int buffer = buffer_
     cdef int multi = 8*512
     cdef int multi2 = multi
     cdef int buffer2
 
     if buffer > 512 * multi:
         buffer2 = 512 * multi
 
-        while (buffer % buffer2 != 0) and multi > 0:
+        while (buffer % buffer2 != 0) and multi > 2:
             multi -= 2
             buffer2 = 512 * multi
 
         if multi > 0:
             buffer = buffer2
         else:
             buffer = 512*4
-
+    if buffer < 512:
+        buffer = 512
     return buffer
```

### Comparing `copytool-0.11/copytool/thirdparty.json` & `copytool-0.12/copytool/thirdparty.json`

 * *Files identical despite different names*

### Comparing `copytool-0.11/copytool.egg-info/PKG-INFO` & `copytool-0.12/copytool.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copytool
-Version: 0.11
+Version: 0.12
 Summary: copytool copies files hell-bent for leather
 Home-page: https://github.com/hansalemaos/copytool
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: copy
 Classifier: Development Status :: 4 - Beta
@@ -21,34 +21,49 @@
 ### Tested+compiled against Windows 10 / Python 3.10 / Anaconda
 
 
 TeraCopy needs 4 minutes, copytool does it 6 seconds
 ![](https://github.com/hansalemaos/copytool/blob/main/fastcopyscreenshot.png?raw=true)
 
 ## CLI
-Compiled EXE: [](https://github.com/hansalemaos/copytool/raw/main/copytool.exe)
+Compiled EXE: 
+[](https://github.com/hansalemaos/copytool/raw/main/copytool.zip)
+[](https://github.com/hansalemaos/copytool/raw/main/copytool.z01)
 
       Example: copytool --src "C:\ProgramData\anaconda3\envs" --dst "e:\envbackup" --use_tqdm 1 --copy_date 1 --copy_permission 0 --overwrite 1
       --src                     str         (source folder)
       --dst                     str         (destination folder)
       --log                     str  ""     (csv log)
       --copy_date               int  0      (copy date stats)
       --copy_permission         int  0      (copy permissions)
       --use_tqdm                int  1      (show progress bar)
       --overwrite               int  1      (overwrite existing files in dst)
+      --use_uffs                int  1      (use uffs to get a list of files)
 
 
 ## Python
 
 ```python
 # pip install copytool 
 from copytool import get_all_files_on_hdd_and_copy
 get_all_files_on_hdd_and_copy(
     src = r"C:\path",
     dst = r"e:\dest",
     log = "c:\\copylog.csv",
-    copy_date= 1,
+    copy_date= 0,
     copy_permission= 0,
     use_tqdm = 1,
     overwrite = 1,
+    use_uffs = 1
+)     
+
+get_all_files_on_hdd_and_copy(
+    src = r"C:\path",
+    dst = r"e:\dest",
+    log = "",
+    copy_date= 0,
+    copy_permission= 0,
+    use_tqdm = 1,
+    overwrite = 1,
+    use_uffs = 0 # no logging without uffs 
 )     
 ```
```

### Comparing `copytool-0.11/setup.py` & `copytool-0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''copytool copies files hell-bent for leather'''
 
 # Setting up
 setup(
     name="copytool",
     version=VERSION,
     license='MIT',
```

