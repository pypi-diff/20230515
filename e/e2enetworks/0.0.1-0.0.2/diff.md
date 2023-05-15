# Comparing `tmp/e2enetworks-0.0.1.tar.gz` & `tmp/e2enetworks-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-0.0.1.tar", last modified: Mon May 15 07:02:28 2023, max compression
+gzip compressed data, was "e2enetworks-0.0.2.tar", last modified: Mon May 15 07:19:06 2023, max compression
```

## Comparing `e2enetworks-0.0.1.tar` & `e2enetworks-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:02:28.124961 e2enetworks-0.0.1/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.1/LICENSE.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5948 2023-05-15 07:02:28.125030 e2enetworks-0.0.1/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.1/README.rst
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:02:28.124262 e2enetworks-0.0.1/cloud/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 06:50:17.000000 e2enetworks-0.0.1/cloud/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 06:54:08.000000 e2enetworks-0.0.1/cloud/test.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:02:28.124851 e2enetworks-0.0.1/e2enetworks.egg-info/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5948 2023-05-15 07:02:28.000000 e2enetworks-0.0.1/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      213 2023-05-15 07:02:28.000000 e2enetworks-0.0.1/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 07:02:28.000000 e2enetworks-0.0.1/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        6 2023-05-15 07:02:28.000000 e2enetworks-0.0.1/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 07:02:28.125248 e2enetworks-0.0.1/setup.cfg
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 06:50:03.000000 e2enetworks-0.0.1/setup.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:19:06.507419 e2enetworks-0.0.2/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.2/LICENSE.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:19:06.507510 e2enetworks-0.0.2/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.2/README.rst
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:19:06.506208 e2enetworks-0.0.2/e2enetowrks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:16:44.000000 e2enetworks-0.0.2/e2enetowrks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:19:06.506422 e2enetworks-0.0.2/e2enetowrks/cloud/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 06:50:17.000000 e2enetworks-0.0.2/e2enetowrks/cloud/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 06:54:08.000000 e2enetworks-0.0.2/e2enetowrks/cloud/test.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:19:06.507301 e2enetworks-0.0.2/e2enetworks.egg-info/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:19:06.000000 e2enetworks-0.0.2/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      261 2023-05-15 07:19:06.000000 e2enetworks-0.0.2/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 07:19:06.000000 e2enetworks-0.0.2/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-15 07:19:06.000000 e2enetworks-0.0.2/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 07:19:06.507775 e2enetworks-0.0.2/setup.cfg
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 07:17:19.000000 e2enetworks-0.0.2/setup.py
```

### Comparing `e2enetworks-0.0.1/LICENSE.txt` & `e2enetworks-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.1/PKG-INFO` & `e2enetworks-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.1
+Version: 0.0.2
 Summary: E2E Networks Plugins
-Home-page: UNKNOWN
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `e2enetworks-0.0.1/README.rst` & `e2enetworks-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.1/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-0.0.2/e2enetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.1
+Version: 0.0.2
 Summary: E2E Networks Plugins
-Home-page: UNKNOWN
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `e2enetworks-0.0.1/setup.py` & `e2enetworks-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "0.0.1"
+version = "0.0.2"
 install_requires = [
 
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst")) as f:
```

