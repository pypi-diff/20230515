# Comparing `tmp/e2enetworks-0.0.2.tar.gz` & `tmp/e2enetworks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-0.0.2.tar", last modified: Mon May 15 07:19:06 2023, max compression
+gzip compressed data, was "e2enetworks-0.0.3.tar", last modified: Mon May 15 07:25:54 2023, max compression
```

## Comparing `e2enetworks-0.0.2.tar` & `e2enetworks-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:19:06.507419 e2enetworks-0.0.2/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.2/LICENSE.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:19:06.507510 e2enetworks-0.0.2/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.2/README.rst
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:19:06.506208 e2enetworks-0.0.2/e2enetowrks/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:16:44.000000 e2enetworks-0.0.2/e2enetowrks/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:19:06.506422 e2enetworks-0.0.2/e2enetowrks/cloud/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 06:50:17.000000 e2enetworks-0.0.2/e2enetowrks/cloud/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 06:54:08.000000 e2enetworks-0.0.2/e2enetowrks/cloud/test.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:19:06.507301 e2enetworks-0.0.2/e2enetworks.egg-info/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:19:06.000000 e2enetworks-0.0.2/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      261 2023-05-15 07:19:06.000000 e2enetworks-0.0.2/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 07:19:06.000000 e2enetworks-0.0.2/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-15 07:19:06.000000 e2enetworks-0.0.2/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 07:19:06.507775 e2enetworks-0.0.2/setup.cfg
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 07:17:19.000000 e2enetworks-0.0.2/setup.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:25:54.355497 e2enetworks-0.0.3/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.3/LICENSE.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:25:54.355583 e2enetworks-0.0.3/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.3/README.rst
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:25:54.354197 e2enetworks-0.0.3/e2enetowrks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:16:44.000000 e2enetworks-0.0.3/e2enetowrks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:25:54.354529 e2enetworks-0.0.3/e2enetowrks/cloud/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 06:50:17.000000 e2enetworks-0.0.3/e2enetowrks/cloud/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 06:54:08.000000 e2enetworks-0.0.3/e2enetowrks/cloud/test.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:25:54.355382 e2enetworks-0.0.3/e2enetworks.egg-info/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:25:54.000000 e2enetworks-0.0.3/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      261 2023-05-15 07:25:54.000000 e2enetworks-0.0.3/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 07:25:54.000000 e2enetworks-0.0.3/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-15 07:25:54.000000 e2enetworks-0.0.3/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 07:25:54.355836 e2enetworks-0.0.3/setup.cfg
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 07:25:41.000000 e2enetworks-0.0.3/setup.py
```

### Comparing `e2enetworks-0.0.2/LICENSE.txt` & `e2enetworks-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.2/PKG-INFO` & `e2enetworks-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.2
+Version: 0.0.3
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.2/README.rst` & `e2enetworks-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.2/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-0.0.3/e2enetworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.2
+Version: 0.0.3
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.2/setup.py` & `e2enetworks-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "0.0.2"
+version = "0.0.3"
 install_requires = [
 
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst")) as f:
```

