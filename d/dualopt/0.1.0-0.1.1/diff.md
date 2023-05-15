# Comparing `tmp/dualopt-0.1.0.tar.gz` & `tmp/dualopt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualopt-0.1.0.tar", last modified: Mon May 15 01:18:43 2023, max compression
+gzip compressed data, was "dualopt-0.1.1.tar", last modified: Mon May 15 01:30:41 2023, max compression
```

## Comparing `dualopt-0.1.0.tar` & `dualopt-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 01:18:43.647209 dualopt-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-05-15 01:05:45.000000 dualopt-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      772 2023-05-15 01:18:43.643208 dualopt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-05-15 01:16:51.000000 dualopt-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 01:18:43.579301 dualopt-0.1.0/dualopt/
--rw-rw-rw-   0        0        0       49 2023-05-15 01:14:55.000000 dualopt-0.1.0/dualopt/__init__.py
--rw-rw-rw-   0        0        0     6035 2023-05-15 01:16:17.000000 dualopt-0.1.0/dualopt/classification.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:18:43.639207 dualopt-0.1.0/dualopt.egg-info/
--rw-rw-rw-   0        0        0      772 2023-05-15 01:18:43.000000 dualopt-0.1.0/dualopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-15 01:18:43.000000 dualopt-0.1.0/dualopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 01:18:43.000000 dualopt-0.1.0/dualopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-15 01:18:43.000000 dualopt-0.1.0/dualopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 01:18:43.000000 dualopt-0.1.0/dualopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 01:18:43.647209 dualopt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-05-15 01:16:20.000000 dualopt-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:30:41.526289 dualopt-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-15 01:05:45.000000 dualopt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      772 2023-05-15 01:30:41.526289 dualopt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2023-05-15 01:16:51.000000 dualopt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 01:30:41.510660 dualopt-0.1.1/dualopt/
+-rw-rw-rw-   0        0        0       49 2023-05-15 01:14:55.000000 dualopt-0.1.1/dualopt/__init__.py
+-rw-rw-rw-   0        0        0     6035 2023-05-15 01:16:17.000000 dualopt-0.1.1/dualopt/classification.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:30:41.526289 dualopt-0.1.1/dualopt.egg-info/
+-rw-rw-rw-   0        0        0      772 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 01:30:41.000000 dualopt-0.1.1/dualopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 01:30:41.526289 dualopt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-15 01:30:02.000000 dualopt-0.1.1/setup.py
```

### Comparing `dualopt-0.1.0/LICENSE` & `dualopt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.0/PKG-INFO` & `dualopt-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.0/dualopt/classification.py` & `dualopt-0.1.1/dualopt/classification.py`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.0/dualopt.egg-info/PKG-INFO` & `dualopt-0.1.1/dualopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualopt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dual Optimizer Training
 Home-page: https://github.com/pranavphoenix/DualOpt
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,machine learning,optimizer,training,image classificationsemantic segmentation,image super-resolution
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dualopt-0.1.0/setup.py` & `dualopt-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'dualopt',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.0',
+  version = '0.1.1',
   license='MIT',
   description = 'Dual Optimizer Training',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/DualOpt',
```

