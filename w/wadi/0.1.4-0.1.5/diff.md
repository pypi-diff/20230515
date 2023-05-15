# Comparing `tmp/wadi-0.1.4.tar.gz` & `tmp/wadi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wadi-0.1.4.tar", last modified: Fri May 12 10:54:46 2023, max compression
+gzip compressed data, was "wadi-0.1.5.tar", last modified: Mon May 15 07:44:34 2023, max compression
```

## Comparing `wadi-0.1.4.tar` & `wadi-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:54:46.936150 wadi-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 10:54:32.000000 wadi-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-12 10:54:46.936150 wadi-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-12 10:54:32.000000 wadi-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:54:46.936150 wadi-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-12 10:54:32.000000 wadi-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:54:46.928150 wadi-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-12 10:54:32.000000 wadi-0.1.4/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:54:46.932150 wadi-0.1.4/wadi/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/documentation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/filereader.py
--rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/harmonizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/infotable.py
--rw-r--r--   0 runner    (1001) docker     (123)    29684 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-12 10:54:32.000000 wadi-0.1.4/wadi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:54:46.936150 wadi-0.1.4/wadi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 10:54:46.000000 wadi-0.1.4/wadi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:34.013752 wadi-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 07:44:22.000000 wadi-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-15 07:44:34.013752 wadi-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-15 07:44:22.000000 wadi-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:44:34.013752 wadi-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 07:44:22.000000 wadi-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:34.013752 wadi-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-15 07:44:22.000000 wadi-0.1.5/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:34.013752 wadi-0.1.5/wadi/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/documentation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/harmonizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/infotable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29684 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-15 07:44:22.000000 wadi-0.1.5/wadi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:34.013752 wadi-0.1.5/wadi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-15 07:44:34.000000 wadi-0.1.5/wadi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 07:44:34.000000 wadi-0.1.5/wadi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:44:34.000000 wadi-0.1.5/wadi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-15 07:44:34.000000 wadi-0.1.5/wadi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 07:44:34.000000 wadi-0.1.5/wadi.egg-info/top_level.txt
```

### Comparing `wadi-0.1.4/LICENSE` & `wadi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/PKG-INFO` & `wadi-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wadi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generic importer for water quality data of the (Dutch) water laboratory
 Home-page: https://github.com/KWR-Water/wadi
 Author: KWR Water Research Institute
 Author-email: martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl
 License: MIT
 Project-URL: Source, https://github.com/KWR-Water/wadi
 Project-URL: Documentation, http://wadi.readthedocs.io/en/latest/
```

### Comparing `wadi-0.1.4/README.md` & `wadi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/setup.py` & `wadi-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import glob
 import os
 from setuptools import setup, find_packages
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 setup(
     name='wadi',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(exclude=['tests*']),
+    data_files=glob.glob('mapping_data/**'),
     license='MIT',
     description='Generic importer for water quality data of the (Dutch) water laboratory',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
```

### Comparing `wadi-0.1.4/wadi/api_utils.py` & `wadi-0.1.5/wadi/api_utils.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/base.py` & `wadi-0.1.5/wadi/base.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/dataobject.py` & `wadi-0.1.5/wadi/dataobject.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/documentation_helpers.py` & `wadi-0.1.5/wadi/documentation_helpers.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/filereader.py` & `wadi-0.1.5/wadi/filereader.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/harmonizer.py` & `wadi-0.1.5/wadi/harmonizer.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/infotable.py` & `wadi-0.1.5/wadi/infotable.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/mapper.py` & `wadi-0.1.5/wadi/mapper.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/unitconverter.py` & `wadi-0.1.5/wadi/unitconverter.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi/utils.py` & `wadi-0.1.5/wadi/utils.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.4/wadi.egg-info/PKG-INFO` & `wadi-0.1.5/wadi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wadi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generic importer for water quality data of the (Dutch) water laboratory
 Home-page: https://github.com/KWR-Water/wadi
 Author: KWR Water Research Institute
 Author-email: martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl
 License: MIT
 Project-URL: Source, https://github.com/KWR-Water/wadi
 Project-URL: Documentation, http://wadi.readthedocs.io/en/latest/
```

