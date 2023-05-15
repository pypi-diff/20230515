# Comparing `tmp/aiorobonect-0.1.0.tar.gz` & `tmp/aiorobonect-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.1.0.tar", last modified: Mon May 15 20:06:21 2023, max compression
+gzip compressed data, was "aiorobonect-0.1.2.tar", last modified: Mon May 15 20:29:22 2023, max compression
```

## Comparing `aiorobonect-0.1.0.tar` & `aiorobonect-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:21.701377 aiorobonect-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 20:06:12.000000 aiorobonect-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 20:06:21.701377 aiorobonect-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 20:06:12.000000 aiorobonect-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:21.701377 aiorobonect-0.1.0/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:06:12.000000 aiorobonect-0.1.0/aiorobonect/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-15 20:06:12.000000 aiorobonect-0.1.0/aiorobonect/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 20:06:12.000000 aiorobonect-0.1.0/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-15 20:06:12.000000 aiorobonect-0.1.0/aiorobonect/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 20:06:12.000000 aiorobonect-0.1.0/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:21.701377 aiorobonect-0.1.0/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 20:06:21.000000 aiorobonect-0.1.0/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 20:06:21.000000 aiorobonect-0.1.0/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:06:21.000000 aiorobonect-0.1.0/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 20:06:21.000000 aiorobonect-0.1.0/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 20:06:21.000000 aiorobonect-0.1.0/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:06:21.701377 aiorobonect-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 20:06:12.000000 aiorobonect-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 20:29:06.000000 aiorobonect-0.1.2/setup.py
```

### Comparing `aiorobonect-0.1.0/LICENSE` & `aiorobonect-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.0/PKG-INFO` & `aiorobonect-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.0
+Version: 0.1.2
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.0/README.md` & `aiorobonect-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.0/aiorobonect/cli.py` & `aiorobonect-0.1.2/aiorobonect/cli.py`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.0/aiorobonect/rest.py` & `aiorobonect-0.1.2/aiorobonect/rest.py`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.0/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.1.2/aiorobonect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.0
+Version: 0.1.2
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.0/setup.py` & `aiorobonect-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.1.0",
+    version="v0.1.2",
 )
```

