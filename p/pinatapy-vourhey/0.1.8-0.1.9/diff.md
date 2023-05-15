# Comparing `tmp/pinatapy-vourhey-0.1.8.tar.gz` & `tmp/pinatapy-vourhey-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinatapy-vourhey-0.1.8.tar", last modified: Wed Nov  9 18:50:47 2022, max compression
+gzip compressed data, was "pinatapy-vourhey-0.1.9.tar", last modified: Mon May 15 10:18:18 2023, max compression
```

## Comparing `pinatapy-vourhey-0.1.8.tar` & `pinatapy-vourhey-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 18:50:47.526154 pinatapy-vourhey-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-11-09 18:50:32.000000 pinatapy-vourhey-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-11-09 18:50:47.526154 pinatapy-vourhey-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-11-09 18:50:32.000000 pinatapy-vourhey-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 18:50:47.522154 pinatapy-vourhey-0.1.8/pinatapy/
--rw-r--r--   0 runner    (1001) docker     (121)     9527 2022-11-09 18:50:32.000000 pinatapy-vourhey-0.1.8/pinatapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 18:50:47.522154 pinatapy-vourhey-0.1.8/pinatapy_vourhey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-11-09 18:50:47.000000 pinatapy-vourhey-0.1.8/pinatapy_vourhey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-09 18:50:47.000000 pinatapy-vourhey-0.1.8/pinatapy_vourhey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 18:50:47.000000 pinatapy-vourhey-0.1.8/pinatapy_vourhey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-09 18:50:47.000000 pinatapy-vourhey-0.1.8/pinatapy_vourhey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-09 18:50:47.000000 pinatapy-vourhey-0.1.8/pinatapy_vourhey.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 18:50:47.526154 pinatapy-vourhey-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-11-09 18:50:32.000000 pinatapy-vourhey-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 18:50:47.526154 pinatapy-vourhey-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-09 18:50:32.000000 pinatapy-vourhey-0.1.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-11-09 18:50:32.000000 pinatapy-vourhey-0.1.8/test/test_pinatapy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:18:18.323295 pinatapy-vourhey-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-15 10:17:59.000000 pinatapy-vourhey-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-15 10:18:18.323295 pinatapy-vourhey-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 10:17:59.000000 pinatapy-vourhey-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:18:18.319295 pinatapy-vourhey-0.1.9/pinatapy/
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-05-15 10:17:59.000000 pinatapy-vourhey-0.1.9/pinatapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:18:18.323295 pinatapy-vourhey-0.1.9/pinatapy_vourhey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-15 10:18:18.000000 pinatapy-vourhey-0.1.9/pinatapy_vourhey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 10:18:18.000000 pinatapy-vourhey-0.1.9/pinatapy_vourhey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:18:18.000000 pinatapy-vourhey-0.1.9/pinatapy_vourhey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 10:18:18.000000 pinatapy-vourhey-0.1.9/pinatapy_vourhey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 10:18:18.000000 pinatapy-vourhey-0.1.9/pinatapy_vourhey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 10:18:18.323295 pinatapy-vourhey-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-15 10:17:59.000000 pinatapy-vourhey-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:18:18.323295 pinatapy-vourhey-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 10:17:59.000000 pinatapy-vourhey-0.1.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-15 10:17:59.000000 pinatapy-vourhey-0.1.9/test/test_pinatapy.py
```

### Comparing `pinatapy-vourhey-0.1.8/LICENSE` & `pinatapy-vourhey-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pinatapy-vourhey-0.1.8/PKG-INFO` & `pinatapy-vourhey-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinatapy-vourhey
-Version: 0.1.8
+Version: 0.1.9
 Summary: Non-official Pinata.cloud library
 Home-page: https://github.com/vourhey/pinatapy
 Author: Vadim Manaenko
 Author-email: vadim.razorq@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pinatapy-vourhey-0.1.8/README.md` & `pinatapy-vourhey-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pinatapy-vourhey-0.1.8/pinatapy/__init__.py` & `pinatapy-vourhey-0.1.9/pinatapy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,14 +35,25 @@
         Validates the IPFS destination folder name is valid by removing 
         blankspaces and adding '/' to the end of the path
         """
         path = path.replace(" ", "")
         if not path.endswith("/"):
             path = path + "/"
         return path
+    
+    @staticmethod
+    def _validate_path_to_file(path: str) -> str:
+        """
+        Validates the path to file is valid by removing '/' at the end 
+        of the path.
+        """
+        path = path.replace(" ", "")
+        if path.endswith("/"):
+            path = path[:-1]
+        return path
 
     def pin_file_to_ipfs(
             self,
             path_to_file: str,
             ipfs_destination_path: str = "/",
             save_absolute_paths: bool = True,
             options: tp.Optional[OptionsDict] = None,
@@ -74,40 +85,43 @@
         headers: Headers = {k: self._auth_headers[k] for k in ["pinata_api_key", "pinata_secret_api_key"]}
         payload: OptionsDict = {}
         dest_folder_name = (
             ipfs_destination_path
             if ipfs_destination_path == "/"
             else self._validate_destination_folder_name(ipfs_destination_path)
         )
-
+        
         def get_all_files(directory: str) -> tp.List[str]:
             """get a list of absolute paths to every file located in the directory"""
             paths: tp.List[str] = []
             for root, dirs, files_ in os.walk(os.path.abspath(directory)):
                 for file in files_:
                     paths.append(os.path.join(root, file))
             return paths
 
-        def get_mutated_filepath(filepath: str, dest_folder_name: str, save_absolute_paths: bool):
+        def get_mutated_filepath(filepath: str, dest_folder_name: str, save_absolute_paths: bool, path_to_file: str, is_directory: bool = False):
             """transform filepath with dest_folder_name and absolute path saving rules"""
             if save_absolute_paths:
                 return dest_folder_name + (filepath[:1].replace("/", "") + filepath[1:])  # remove first '/' if exists
             else:
-                return dest_folder_name + filepath.split("/")[-1]
-
+                # can't pin directory into root and save directory's hierarchy
+                if is_directory and dest_folder_name == "/":
+                    dest_folder_name =  self._validate_path_to_file(path_to_file).split("/")[-1]
+                return dest_folder_name + filepath.split(dest_folder_name)[-1]
+        
         files: tp.List[str, tp.Any]
 
         # If path_to_file is a directory
         if os.path.isdir(path_to_file):
             all_files: tp.List[str] = get_all_files(path_to_file)
-            files = [("file", (get_mutated_filepath(file, dest_folder_name, save_absolute_paths), open(file, "rb"))) for
+            files = [("file", (get_mutated_filepath(file, dest_folder_name, save_absolute_paths, path_to_file, is_directory=True), open(file, "rb"))) for
                      file in all_files]  # type: ignore
         # If path_to_file is a single file
         else:
-            files = [("file", (get_mutated_filepath(path_to_file, dest_folder_name, save_absolute_paths),
+            files = [("file", (get_mutated_filepath(path_to_file, dest_folder_name, save_absolute_paths, path_to_file),
                                open(path_to_file, "rb")))]  # type: ignore
 
         if options is not None:
             if "pinataMetadata" in options:
                 pinataMetadata = options["pinataMetadata"]
                 payload["pinataMetadata"] = pinataMetadata if type(pinataMetadata) == str else json.dumps(pinataMetadata)
             if "pinataOptions" in options:
```

### Comparing `pinatapy-vourhey-0.1.8/pinatapy_vourhey.egg-info/PKG-INFO` & `pinatapy-vourhey-0.1.9/pinatapy_vourhey.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinatapy-vourhey
-Version: 0.1.8
+Version: 0.1.9
 Summary: Non-official Pinata.cloud library
 Home-page: https://github.com/vourhey/pinatapy
 Author: Vadim Manaenko
 Author-email: vadim.razorq@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pinatapy-vourhey-0.1.8/setup.py` & `pinatapy-vourhey-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pinatapy-vourhey",
-    version="0.1.8",
+    version="0.1.9",
     author="Vadim Manaenko",
     author_email="vadim.razorq@gmail.com",
     description="Non-official Pinata.cloud library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vourhey/pinatapy",
     packages=setuptools.find_packages(),
```

### Comparing `pinatapy-vourhey-0.1.8/test/test_pinatapy.py` & `pinatapy-vourhey-0.1.9/test/test_pinatapy.py`

 * *Files identical despite different names*

