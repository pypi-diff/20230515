# Comparing `tmp/FileInfo_Video_Audio-0.0.3.tar.gz` & `tmp/FileInfo_Video_Audio-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileInfo_Video_Audio-0.0.3.tar", last modified: Sun May 14 18:53:00 2023, max compression
+gzip compressed data, was "FileInfo_Video_Audio-0.0.4.tar", last modified: Mon May 15 07:59:53 2023, max compression
```

## Comparing `FileInfo_Video_Audio-0.0.3.tar` & `FileInfo_Video_Audio-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:53:00.211923 FileInfo_Video_Audio-0.0.3/
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:53:00.211923 FileInfo_Video_Audio-0.0.3/FileInfo_Video_Audio.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      381 2023-05-14 18:53:00.000000 FileInfo_Video_Audio-0.0.3/FileInfo_Video_Audio.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-14 18:53:00.000000 FileInfo_Video_Audio-0.0.3/FileInfo_Video_Audio.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-14 18:53:00.000000 FileInfo_Video_Audio-0.0.3/FileInfo_Video_Audio.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-14 18:53:00.000000 FileInfo_Video_Audio-0.0.3/FileInfo_Video_Audio.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-14 18:53:00.000000 FileInfo_Video_Audio-0.0.3/FileInfo_Video_Audio.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      381 2023-05-14 18:53:00.211923 FileInfo_Video_Audio-0.0.3/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       10 2023-05-14 18:23:40.000000 FileInfo_Video_Audio-0.0.3/README.md
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-14 18:53:00.211923 FileInfo_Video_Audio-0.0.3/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      816 2023-05-14 18:51:44.000000 FileInfo_Video_Audio-0.0.3/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:53:00.211923 FileInfo_Video_Audio-0.0.3/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:26:11.000000 FileInfo_Video_Audio-0.0.3/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:53:00.211923 FileInfo_Video_Audio-0.0.3/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.0.3/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.0.3/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2797 2023-05-14 18:50:04.000000 FileInfo_Video_Audio-0.0.3/source/main.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-15 07:59:53.350392 FileInfo_Video_Audio-0.0.4/
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-15 07:59:53.350392 FileInfo_Video_Audio-0.0.4/FileInfo_Video_Audio.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      381 2023-05-15 07:59:53.000000 FileInfo_Video_Audio-0.0.4/FileInfo_Video_Audio.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-15 07:59:53.000000 FileInfo_Video_Audio-0.0.4/FileInfo_Video_Audio.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-15 07:59:53.000000 FileInfo_Video_Audio-0.0.4/FileInfo_Video_Audio.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-15 07:59:53.000000 FileInfo_Video_Audio-0.0.4/FileInfo_Video_Audio.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-15 07:59:53.000000 FileInfo_Video_Audio-0.0.4/FileInfo_Video_Audio.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      381 2023-05-15 07:59:53.350392 FileInfo_Video_Audio-0.0.4/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       10 2023-05-14 18:23:40.000000 FileInfo_Video_Audio-0.0.4/README.md
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-15 07:59:53.350392 FileInfo_Video_Audio-0.0.4/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      816 2023-05-15 07:54:48.000000 FileInfo_Video_Audio-0.0.4/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-15 07:59:53.350392 FileInfo_Video_Audio-0.0.4/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:26:11.000000 FileInfo_Video_Audio-0.0.4/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-15 07:59:53.350392 FileInfo_Video_Audio-0.0.4/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.0.4/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.0.4/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3816 2023-05-15 07:49:11.000000 FileInfo_Video_Audio-0.0.4/source/main.py
```

### Comparing `FileInfo_Video_Audio-0.0.3/setup.py` & `FileInfo_Video_Audio-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = os.popen("/usr/local/bin/pipreqs main --print").read().splitlines()
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='FileInfo_Video_Audio',
-    version='0.0.3',
+    version='0.0.4',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
     description="In this tool is help to get the properties of the Audio and Video files",
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details',
     install_requires=requirements,
     long_description=long_description,
```

### Comparing `FileInfo_Video_Audio-0.0.3/source/lib/Argument.py` & `FileInfo_Video_Audio-0.0.4/source/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `FileInfo_Video_Audio-0.0.3/source/main.py` & `FileInfo_Video_Audio-0.0.4/source/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,48 +9,72 @@
 def help():
     print("<FileInfo> [Options].. ")
 
 def main():
     if Argument.hasOptionValue('-file'):
         if Argument.getoptionvalue('--type') and Argument.getoptionvalue('--option'):
             file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
-            if file_content["media"]["track"] != None:
-                for track in file_content["media"]["track"]:
-                    if(track['@type'] == Argument.getoptionvalue('--type')):
-                        d = json.dumps(track, indent=4)
-                        option = Argument.getoptionvalue('--option')
-                        for i in track.keys():
-                            if option == i:
-                                print(f"{option} ==> {track[i]}")
+            try:
+                if file_content["media"]["track"]:
+                    for track in file_content["media"]["track"]:
+                        if(track['@type'] == Argument.getoptionvalue('--type')):
+                            d = json.dumps(track, indent=4)
+                            option = Argument.getoptionvalue('--option')
+                            for i in track.keys():
+                                if option == i:
+                                    print(f"{option} ==> {track[i]}")
+                                     
+                
                 else:
-                    print("Unable to fetch the Tracks of your Source file")
+                    raise Exception("Unable to fetch the Tracks of your Source file")
+            except ValueError as e:
+                print(e)
                             
         elif Argument.hasOption(['--type']) and (Argument.hasCommands(['--help']) or Argument.hasOption(['-h'])):
             file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
-            for track in file_content["media"]["track"]:
-                tracks = track['@type']
-                if tracks =="General":
-                    print(f"{tracks}  ==> Show's the Files General properties" )
-                if tracks =="Video":
-                    print(f"{tracks}    ==> Show's the Files Video properties" )
-                if tracks =="Audio":
-                    print(f"{tracks}    ==> Show's the Files Audio properties" )
+            try:
+                if file_content["media"]["track"]:
+                    for track in file_content["media"]["track"]:
+                        tracks = track['@type']
+                        if tracks =="General":
+                            print(f"{tracks}  ==> Show's the Files General properties" )
+                        if tracks =="Video":
+                            print(f"{tracks}    ==> Show's the Files Video properties" )
+                        if tracks =="Audio":
+                            print(f"{tracks}    ==> Show's the Files Audio properties" )
+                else:
+                    raise Exception("Unable to fetch the Tracks of your Source file")
+            except ValueError as e:
+                print(e)
+                    
                     
         elif Argument.getoptionvalue('--type') and  Argument.hasOption(['--options']):
             file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
-            for track in file_content["media"]["track"]:
-                if(track['@type'] == Argument.getoptionvalue('--type')):
-                    type = Argument.getoptionvalue('--type')
-                    for i in track:
-                        print(f"{i}  ==> {i} of the Source File")
+            try:
+                if file_content["media"]["track"]:
+                    for track in file_content["media"]["track"]:
+                        if(track['@type'] == Argument.getoptionvalue('--type')):
+                            type = Argument.getoptionvalue('--type')
+                            for i in track:
+                                print(f"{i}  ==> {i} of the Source File")
+                else:
+                    raise Exception("Unable to fetch the Tracks of your Source file")
+            except ValueError as e:
+                print(e)
                         
         elif (Argument.hasOption(['--help']) or Argument.hasOption(['--help'])) and Argument.hasOptionValue('-file'):
             file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
-            for track in file_content["media"]["track"]:
-                print(f"Your Tracks are ==> {track['@type']}")
+            try:
+                if file_content["media"]["track"]:
+                    for track in file_content["media"]["track"]:
+                        print(f"Your Tracks are ==> {track['@type']}")
+                else:
+                    raise Exception("Unable to fetch the Tracks of your Source file")
+            except ValueError as e:
+                print(e)
             
     else:
         help()
         
 if __name__ == "__main__":
     main()
```

