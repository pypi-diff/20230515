# Comparing `tmp/e2enetworks-0.0.3.tar.gz` & `tmp/e2enetworks-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-0.0.3.tar", last modified: Mon May 15 07:25:54 2023, max compression
+gzip compressed data, was "e2enetworks-0.0.4.tar", last modified: Mon May 15 07:42:20 2023, max compression
```

## Comparing `e2enetworks-0.0.3.tar` & `e2enetworks-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:25:54.355497 e2enetworks-0.0.3/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.3/LICENSE.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:25:54.355583 e2enetworks-0.0.3/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.3/README.rst
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:25:54.354197 e2enetworks-0.0.3/e2enetowrks/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:16:44.000000 e2enetworks-0.0.3/e2enetowrks/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:25:54.354529 e2enetworks-0.0.3/e2enetowrks/cloud/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 06:50:17.000000 e2enetworks-0.0.3/e2enetowrks/cloud/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 06:54:08.000000 e2enetworks-0.0.3/e2enetowrks/cloud/test.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:25:54.355382 e2enetworks-0.0.3/e2enetworks.egg-info/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:25:54.000000 e2enetworks-0.0.3/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      261 2023-05-15 07:25:54.000000 e2enetworks-0.0.3/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 07:25:54.000000 e2enetworks-0.0.3/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-15 07:25:54.000000 e2enetworks-0.0.3/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 07:25:54.355836 e2enetworks-0.0.3/setup.cfg
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 07:25:41.000000 e2enetworks-0.0.3/setup.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:42:20.290674 e2enetworks-0.0.4/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.4/LICENSE.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:42:20.290742 e2enetworks-0.0.4/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.4/README.rst
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:42:20.289860 e2enetworks-0.0.4/e2enetworks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.4/e2enetworks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:42:20.290427 e2enetworks-0.0.4/e2enetworks/cloud/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.4/e2enetworks/cloud/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 07:31:42.000000 e2enetworks-0.0.4/e2enetworks/cloud/test.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:42:20.290258 e2enetworks-0.0.4/e2enetworks.egg-info/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:42:20.000000 e2enetworks-0.0.4/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      261 2023-05-15 07:42:20.000000 e2enetworks-0.0.4/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 07:42:20.000000 e2enetworks-0.0.4/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-15 07:42:20.000000 e2enetworks-0.0.4/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 07:42:20.290945 e2enetworks-0.0.4/setup.cfg
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 07:38:52.000000 e2enetworks-0.0.4/setup.py
```

### Comparing `e2enetworks-0.0.3/LICENSE.txt` & `e2enetworks-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.3/PKG-INFO` & `e2enetworks-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.3
+Version: 0.0.4
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.3/README.rst` & `e2enetworks-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.3/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-0.0.4/e2enetworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.3
+Version: 0.0.4
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.3/setup.py` & `e2enetworks-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "0.0.3"
+version = "0.0.4"
 install_requires = [
 
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst")) as f:
```

