# Comparing `tmp/trex2champ-2.1.0.tar.gz` & `tmp/trex2champ-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex2champ-2.1.0.tar", last modified: Mon May 15 09:18:11 2023, max compression
+gzip compressed data, was "trex2champ-2.1.5.tar", last modified: Mon May 15 09:15:12 2023, max compression
```

## Comparing `trex2champ-2.1.0.tar` & `trex2champ-2.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-15 09:18:11.713273 trex2champ-2.1.0/
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)     1830 2023-05-15 09:18:11.713273 trex2champ-2.1.0/PKG-INFO
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)      837 2023-05-15 08:49:39.000000 trex2champ-2.1.0/README.md
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-15 09:18:11.713273 trex2champ-2.1.0/setup.cfg
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)     1407 2023-05-15 09:17:14.000000 trex2champ-2.1.0/setup.py
-drwxrwxr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-15 09:18:11.713273 trex2champ-2.1.0/trex2champ.egg-info/
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)     1830 2023-05-15 09:18:11.000000 trex2champ-2.1.0/trex2champ.egg-info/PKG-INFO
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)      224 2023-05-15 09:18:11.000000 trex2champ-2.1.0/trex2champ.egg-info/SOURCES.txt
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-15 09:18:11.000000 trex2champ-2.1.0/trex2champ.egg-info/dependency_links.txt
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)       47 2023-05-15 09:18:11.000000 trex2champ-2.1.0/trex2champ.egg-info/entry_points.txt
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)       31 2023-05-15 09:18:11.000000 trex2champ-2.1.0/trex2champ.egg-info/requires.txt
--rw-rw-r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-15 09:18:11.000000 trex2champ-2.1.0/trex2champ.egg-info/top_level.txt
+drwxrwxr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-15 09:15:12.605771 trex2champ-2.1.5/
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)     1830 2023-05-15 09:15:12.605771 trex2champ-2.1.5/PKG-INFO
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)      837 2023-05-15 08:49:39.000000 trex2champ-2.1.5/README.md
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-15 09:15:12.605771 trex2champ-2.1.5/setup.cfg
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)     1407 2023-05-15 09:14:48.000000 trex2champ-2.1.5/setup.py
+drwxrwxr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-15 09:15:12.605771 trex2champ-2.1.5/trex2champ.egg-info/
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)     1830 2023-05-15 09:15:12.000000 trex2champ-2.1.5/trex2champ.egg-info/PKG-INFO
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)      224 2023-05-15 09:15:12.000000 trex2champ-2.1.5/trex2champ.egg-info/SOURCES.txt
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-15 09:15:12.000000 trex2champ-2.1.5/trex2champ.egg-info/dependency_links.txt
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)       47 2023-05-15 09:15:12.000000 trex2champ-2.1.5/trex2champ.egg-info/entry_points.txt
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)       31 2023-05-15 09:15:12.000000 trex2champ-2.1.5/trex2champ.egg-info/requires.txt
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-15 09:15:12.000000 trex2champ-2.1.5/trex2champ.egg-info/top_level.txt
```

### Comparing `trex2champ-2.1.0/PKG-INFO` & `trex2champ-2.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex2champ
-Version: 2.1.0
+Version: 2.1.5
 Summary: A package to convert trexio files into various text input files for CHAMP code.
 Home-page: https://github.com/neelravi/trex2champ
 Author: Ravindra Shinde
 Author-email: r.l.shinde@utwente.nl
 Keywords: trexio quantum monte carlo champ converter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `trex2champ-2.1.0/README.md` & `trex2champ-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `trex2champ-2.1.0/setup.py` & `trex2champ-2.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='trex2champ',
-    version='2.1.0',
+    version='2.1.5',
     packages=['./'],
     install_requires=[
         'trexio>=1.3.2',
         'resultsFile>=2.4',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `trex2champ-2.1.0/trex2champ.egg-info/PKG-INFO` & `trex2champ-2.1.5/trex2champ.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex2champ
-Version: 2.1.0
+Version: 2.1.5
 Summary: A package to convert trexio files into various text input files for CHAMP code.
 Home-page: https://github.com/neelravi/trex2champ
 Author: Ravindra Shinde
 Author-email: r.l.shinde@utwente.nl
 Keywords: trexio quantum monte carlo champ converter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

