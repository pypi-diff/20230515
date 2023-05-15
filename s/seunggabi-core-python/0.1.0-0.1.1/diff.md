# Comparing `tmp/seunggabi_core_python-0.1.0.tar.gz` & `tmp/seunggabi_core_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seunggabi_core_python-0.1.0.tar", last modified: Mon May 15 13:15:40 2023, max compression
+gzip compressed data, was "seunggabi_core_python-0.1.1.tar", last modified: Mon May 15 14:36:17 2023, max compression
```

## Comparing `seunggabi_core_python-0.1.0.tar` & `seunggabi_core_python-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 13:15:40.400399 seunggabi_core_python-0.1.0/
--rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.1.0/LICENSE
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-15 13:15:40.400266 seunggabi_core_python-0.1.0/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      441 2023-05-13 15:56:24.000000 seunggabi_core_python-0.1.0/README.md
--rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-05-15 13:15:40.400433 seunggabi_core_python-0.1.0/setup.cfg
--rw-r--r--   0 seunggabi   (501) staff       (20)      690 2023-05-15 13:15:08.000000 seunggabi_core_python-0.1.0/setup.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 13:15:40.398971 seunggabi_core_python-0.1.0/seunggabi_core_python/
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-15 13:15:08.000000 seunggabi_core_python-0.1.0/seunggabi_core_python/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.1.0/seunggabi_core_python/const.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 13:15:40.399644 seunggabi_core_python-0.1.0/seunggabi_core_python/exception/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.1.0/seunggabi_core_python/exception/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       95 2023-05-15 12:54:12.000000 seunggabi_core_python-0.1.0/seunggabi_core_python/exception/bad_request.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 13:15:40.400084 seunggabi_core_python-0.1.0/seunggabi_core_python/util/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.1.0/seunggabi_core_python/util/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      926 2023-05-15 13:10:45.000000 seunggabi_core_python-0.1.0/seunggabi_core_python/util/config_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      142 2023-05-13 14:44:24.000000 seunggabi_core_python-0.1.0/seunggabi_core_python/util/json_util.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 13:15:40.399422 seunggabi_core_python-0.1.0/seunggabi_core_python.egg-info/
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-15 13:15:40.000000 seunggabi_core_python-0.1.0/seunggabi_core_python.egg-info/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      483 2023-05-15 13:15:40.000000 seunggabi_core_python-0.1.0/seunggabi_core_python.egg-info/SOURCES.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-05-15 13:15:40.000000 seunggabi_core_python-0.1.0/seunggabi_core_python.egg-info/dependency_links.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-15 13:15:40.000000 seunggabi_core_python-0.1.0/seunggabi_core_python.egg-info/top_level.txt
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 14:36:17.864845 seunggabi_core_python-0.1.1/
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.1.1/LICENSE
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-15 14:36:17.864740 seunggabi_core_python-0.1.1/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      332 2023-05-15 13:55:58.000000 seunggabi_core_python-0.1.1/README.md
+-rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-05-15 14:36:17.864873 seunggabi_core_python-0.1.1/setup.cfg
+-rw-r--r--   0 seunggabi   (501) staff       (20)      746 2023-05-15 13:20:26.000000 seunggabi_core_python-0.1.1/setup.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 14:36:17.863474 seunggabi_core_python-0.1.1/seunggabi_core_python/
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-15 14:36:14.000000 seunggabi_core_python-0.1.1/seunggabi_core_python/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.1.1/seunggabi_core_python/const.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 14:36:17.864133 seunggabi_core_python-0.1.1/seunggabi_core_python/exception/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.1.1/seunggabi_core_python/exception/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       95 2023-05-15 12:54:12.000000 seunggabi_core_python-0.1.1/seunggabi_core_python/exception/bad_request.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 14:36:17.864572 seunggabi_core_python-0.1.1/seunggabi_core_python/util/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.1.1/seunggabi_core_python/util/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      926 2023-05-15 13:10:45.000000 seunggabi_core_python-0.1.1/seunggabi_core_python/util/config_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      142 2023-05-13 14:44:24.000000 seunggabi_core_python-0.1.1/seunggabi_core_python/util/json_util.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 14:36:17.863930 seunggabi_core_python-0.1.1/seunggabi_core_python.egg-info/
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-15 14:36:17.000000 seunggabi_core_python-0.1.1/seunggabi_core_python.egg-info/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      483 2023-05-15 14:36:17.000000 seunggabi_core_python-0.1.1/seunggabi_core_python.egg-info/SOURCES.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-05-15 14:36:17.000000 seunggabi_core_python-0.1.1/seunggabi_core_python.egg-info/dependency_links.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-15 14:36:17.000000 seunggabi_core_python-0.1.1/seunggabi_core_python.egg-info/top_level.txt
```

### Comparing `seunggabi_core_python-0.1.0/LICENSE` & `seunggabi_core_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.1.0/PKG-INFO` & `seunggabi_core_python-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seunggabi_core_python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.1.0/seunggabi_core_python/util/config_util.py` & `seunggabi_core_python-0.1.1/seunggabi_core_python/util/config_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.1.0/seunggabi_core_python.egg-info/PKG-INFO` & `seunggabi_core_python-0.1.1/seunggabi_core_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seunggabi-core-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

