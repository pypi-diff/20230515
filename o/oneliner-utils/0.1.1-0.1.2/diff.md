# Comparing `tmp/oneliner-utils-0.1.1.tar.gz` & `tmp/oneliner-utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oneliner-utils-0.1.1.tar", last modified: Tue Nov 15 22:15:04 2022, max compression
+gzip compressed data, was "dist/oneliner-utils-0.1.2.tar", last modified: Mon May 15 09:33:40 2023, max compression
```

## Comparing `oneliner-utils-0.1.1.tar` & `oneliner-utils-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/
--rw-r--r--   0 elias      (502) staff       (20)     1070 2022-09-29 12:49:19.000000 oneliner-utils-0.1.1/LICENSE
--rw-r--r--   0 elias      (502) staff       (20)      593 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/PKG-INFO
--rw-r--r--   0 elias      (502) staff       (20)       16 2022-11-15 21:17:43.000000 oneliner-utils-0.1.1/README.md
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/oneliner_utils/
--rw-r--r--   0 elias      (502) staff       (20)     2344 2022-11-15 22:14:09.000000 oneliner-utils-0.1.1/oneliner_utils/__init__.py
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/
--rw-r--r--   0 elias      (502) staff       (20)        0 2022-09-29 15:06:19.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/__init__.py
--rw-r--r--   0 elias      (502) staff       (20)      146 2022-11-14 16:42:52.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/common.py
--rw-r--r--   0 elias      (502) staff       (20)     1700 2022-11-14 17:22:31.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/csv_handler.py
--rw-r--r--   0 elias      (502) staff       (20)     2798 2022-11-15 18:56:51.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/gzip_handler.py
--rw-r--r--   0 elias      (502) staff       (20)      472 2022-11-14 17:06:45.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/json_handler.py
--rw-r--r--   0 elias      (502) staff       (20)     1187 2022-11-14 17:09:46.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/jsonl_handler.py
--rw-r--r--   0 elias      (502) staff       (20)     1368 2022-11-14 17:10:23.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/list_handler.py
--rw-r--r--   0 elias      (502) staff       (20)      454 2022-11-15 15:34:02.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/lz4_handler.py
--rw-r--r--   0 elias      (502) staff       (20)      457 2022-11-14 16:44:00.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/numpy_handler.py
--rw-r--r--   0 elias      (502) staff       (20)      236 2022-11-14 16:42:03.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/path_handler.py
--rw-r--r--   0 elias      (502) staff       (20)      424 2022-11-14 16:44:04.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/pickle_handler.py
--rw-r--r--   0 elias      (502) staff       (20)      469 2022-11-14 16:44:08.000000 oneliner-utils-0.1.1/oneliner_utils/handlers/string_handler.py
-drwxr-xr-x   0 elias      (502) staff       (20)        0 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/oneliner_utils.egg-info/
--rw-r--r--   0 elias      (502) staff       (20)      593 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/oneliner_utils.egg-info/PKG-INFO
--rw-r--r--   0 elias      (502) staff       (20)      716 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/oneliner_utils.egg-info/SOURCES.txt
--rw-r--r--   0 elias      (502) staff       (20)        1 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/oneliner_utils.egg-info/dependency_links.txt
--rw-r--r--   0 elias      (502) staff       (20)       17 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/oneliner_utils.egg-info/requires.txt
--rw-r--r--   0 elias      (502) staff       (20)       15 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/oneliner_utils.egg-info/top_level.txt
--rw-r--r--   0 elias      (502) staff       (20)       38 2022-11-15 22:15:04.000000 oneliner-utils-0.1.1/setup.cfg
--rw-r--r--   0 elias      (502) staff       (20)      856 2022-11-15 22:14:29.000000 oneliner-utils-0.1.1/setup.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/
+-rw-r--r--   0 elias      (501) staff       (20)     1070 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/LICENSE
+-rw-r--r--   0 elias      (501) staff       (20)      594 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)       16 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/README.md
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/oneliner_utils/
+-rw-r--r--   0 elias      (501) staff       (20)     2344 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/__init__.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/
+-rw-r--r--   0 elias      (501) staff       (20)        0 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)      146 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/common.py
+-rw-r--r--   0 elias      (501) staff       (20)     1700 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/csv_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     2798 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/gzip_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      572 2023-05-15 09:31:44.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/json_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     1327 2023-05-15 09:19:12.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/jsonl_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     1368 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/list_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      454 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/lz4_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      457 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/numpy_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      236 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/path_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      424 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/pickle_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      469 2023-05-15 09:15:08.000000 oneliner-utils-0.1.2/oneliner_utils/handlers/string_handler.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/oneliner_utils.egg-info/
+-rw-r--r--   0 elias      (501) staff       (20)      594 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/oneliner_utils.egg-info/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)      716 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/oneliner_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 elias      (501) staff       (20)        1 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/oneliner_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 elias      (501) staff       (20)       17 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/oneliner_utils.egg-info/requires.txt
+-rw-r--r--   0 elias      (501) staff       (20)       15 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/oneliner_utils.egg-info/top_level.txt
+-rw-r--r--   0 elias      (501) staff       (20)       38 2023-05-15 09:33:40.000000 oneliner-utils-0.1.2/setup.cfg
+-rw-r--r--   0 elias      (501) staff       (20)      857 2023-05-15 09:27:57.000000 oneliner-utils-0.1.2/setup.py
```

### Comparing `oneliner-utils-0.1.1/LICENSE` & `oneliner-utils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oneliner-utils-0.1.1/PKG-INFO` & `oneliner-utils-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: oneliner-utils
-Version: 0.1.1
-Summary: Oneline Utils for Python
+Version: 0.1.2
+Summary: One-line Utils for Python
 Home-page: https://github.com/AmenRa/oneliner-utils
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: oneliner,oneliners,utils,utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `oneliner-utils-0.1.1/oneliner_utils/__init__.py` & `oneliner-utils-0.1.2/oneliner_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `oneliner-utils-0.1.1/oneliner_utils/handlers/csv_handler.py` & `oneliner-utils-0.1.2/oneliner_utils/handlers/csv_handler.py`

 * *Files identical despite different names*

### Comparing `oneliner-utils-0.1.1/oneliner_utils/handlers/gzip_handler.py` & `oneliner-utils-0.1.2/oneliner_utils/handlers/gzip_handler.py`

 * *Files identical despite different names*

### Comparing `oneliner-utils-0.1.1/oneliner_utils/handlers/jsonl_handler.py` & `oneliner-utils-0.1.2/oneliner_utils/handlers/jsonl_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,8 +37,14 @@
     callback: Callable = None,
 ) -> None:
     path = create_path(path)
     path.parent.mkdir(parents=True, exist_ok=True)
 
     with open(path, "wb") as f:
         for y in x:
-            f.write(orjson.dumps(apply_callback(y, callback)) + "\n".encode())
+            f.write(
+                orjson.dumps(
+                    apply_callback(y, callback),
+                    option=orjson.OPT_SERIALIZE_NUMPY,
+                )
+                + "\n".encode()
+            )
```

### Comparing `oneliner-utils-0.1.1/oneliner_utils/handlers/list_handler.py` & `oneliner-utils-0.1.2/oneliner_utils/handlers/list_handler.py`

 * *Files identical despite different names*

### Comparing `oneliner-utils-0.1.1/oneliner_utils.egg-info/PKG-INFO` & `oneliner-utils-0.1.2/oneliner_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: oneliner-utils
-Version: 0.1.1
-Summary: Oneline Utils for Python
+Version: 0.1.2
+Summary: One-line Utils for Python
 Home-page: https://github.com/AmenRa/oneliner-utils
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: oneliner,oneliners,utils,utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `oneliner-utils-0.1.1/oneliner_utils.egg-info/SOURCES.txt` & `oneliner-utils-0.1.2/oneliner_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneliner-utils-0.1.1/setup.py` & `oneliner-utils-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="oneliner-utils",
-    version="0.1.1",
+    version="0.1.2",
     author="Elias Bassani",
     author_email="elias.bssn@gmail.com",
-    description="Oneline Utils for Python",
+    description="One-line Utils for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AmenRa/oneliner-utils",
     packages=setuptools.find_packages(),
     install_requires=["numpy", "orjson", "lz4"],
     classifiers=[
         "Programming Language :: Python :: 3",
```

