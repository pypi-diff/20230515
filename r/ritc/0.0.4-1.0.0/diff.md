# Comparing `tmp/ritc-0.0.4.tar.gz` & `tmp/ritc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ritc-0.0.4.tar", last modified: Sun Mar 12 20:47:19 2023, max compression
+gzip compressed data, was "ritc-1.0.0.tar", last modified: Mon May 15 18:14:25 2023, max compression
```

## Comparing `ritc-0.0.4.tar` & `ritc-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 juhok     (1000) juhok     (1001)        0 2023-03-12 20:47:19.446615 ritc-0.0.4/
--rw-r--r--   0 juhok     (1000) juhok     (1001)     1065 2023-02-16 02:30:22.000000 ritc-0.0.4/LICENSE
--rw-r--r--   0 juhok     (1000) juhok     (1001)     2571 2023-03-12 20:47:19.443282 ritc-0.0.4/PKG-INFO
--rw-r--r--   0 juhok     (1000) juhok     (1001)     1232 2023-02-14 03:56:22.000000 ritc-0.0.4/README.rst
-drwxr-xr-x   0 juhok     (1000) juhok     (1001)        0 2023-03-12 20:47:19.443282 ritc-0.0.4/ritc/
--rw-r--r--   0 juhok     (1000) juhok     (1001)    33709 2023-03-12 20:40:19.000000 ritc-0.0.4/ritc/__init__.py
--rw-r--r--   0 juhok     (1000) juhok     (1001)        0 2023-02-14 03:56:22.000000 ritc-0.0.4/ritc/py.typed
-drwxr-xr-x   0 juhok     (1000) juhok     (1001)        0 2023-03-12 20:47:19.443282 ritc-0.0.4/ritc.egg-info/
--rw-r--r--   0 juhok     (1000) juhok     (1001)     2571 2023-03-12 20:47:19.000000 ritc-0.0.4/ritc.egg-info/PKG-INFO
--rw-r--r--   0 juhok     (1000) juhok     (1001)      197 2023-03-12 20:47:19.000000 ritc-0.0.4/ritc.egg-info/SOURCES.txt
--rw-r--r--   0 juhok     (1000) juhok     (1001)        1 2023-03-12 20:47:19.000000 ritc-0.0.4/ritc.egg-info/dependency_links.txt
--rw-r--r--   0 juhok     (1000) juhok     (1001)       17 2023-03-12 20:47:19.000000 ritc-0.0.4/ritc.egg-info/requires.txt
--rw-r--r--   0 juhok     (1000) juhok     (1001)        5 2023-03-12 20:47:19.000000 ritc-0.0.4/ritc.egg-info/top_level.txt
--rw-r--r--   0 juhok     (1000) juhok     (1001)       38 2023-03-12 20:47:19.446615 ritc-0.0.4/setup.cfg
--rw-r--r--   0 juhok     (1000) juhok     (1001)     1669 2023-03-12 20:40:36.000000 ritc-0.0.4/setup.py
+drwxr-xr-x   0 juhok     (1000) juhok     (1001)        0 2023-05-15 18:14:25.539558 ritc-1.0.0/
+-rw-r--r--   0 juhok     (1000) juhok     (1001)     1065 2023-04-19 20:23:59.000000 ritc-1.0.0/LICENSE
+-rw-r--r--   0 juhok     (1000) juhok     (1001)     2571 2023-05-15 18:14:25.539558 ritc-1.0.0/PKG-INFO
+-rw-r--r--   0 juhok     (1000) juhok     (1001)     1232 2023-04-19 20:23:59.000000 ritc-1.0.0/README.rst
+drwxr-xr-x   0 juhok     (1000) juhok     (1001)        0 2023-05-15 18:14:25.536224 ritc-1.0.0/ritc/
+-rw-r--r--   0 juhok     (1000) juhok     (1001)    33709 2023-04-19 20:23:59.000000 ritc-1.0.0/ritc/__init__.py
+-rw-r--r--   0 juhok     (1000) juhok     (1001)        0 2023-04-19 20:23:59.000000 ritc-1.0.0/ritc/py.typed
+drwxr-xr-x   0 juhok     (1000) juhok     (1001)        0 2023-05-15 18:14:25.539558 ritc-1.0.0/ritc.egg-info/
+-rw-r--r--   0 juhok     (1000) juhok     (1001)     2571 2023-05-15 18:14:25.000000 ritc-1.0.0/ritc.egg-info/PKG-INFO
+-rw-r--r--   0 juhok     (1000) juhok     (1001)      197 2023-05-15 18:14:25.000000 ritc-1.0.0/ritc.egg-info/SOURCES.txt
+-rw-r--r--   0 juhok     (1000) juhok     (1001)        1 2023-05-15 18:14:25.000000 ritc-1.0.0/ritc.egg-info/dependency_links.txt
+-rw-r--r--   0 juhok     (1000) juhok     (1001)       17 2023-05-15 18:14:25.000000 ritc-1.0.0/ritc.egg-info/requires.txt
+-rw-r--r--   0 juhok     (1000) juhok     (1001)        5 2023-05-15 18:14:25.000000 ritc-1.0.0/ritc.egg-info/top_level.txt
+-rw-r--r--   0 juhok     (1000) juhok     (1001)       38 2023-05-15 18:14:25.539558 ritc-1.0.0/setup.cfg
+-rw-r--r--   0 juhok     (1000) juhok     (1001)     1669 2023-05-15 18:08:32.000000 ritc-1.0.0/setup.py
```

### Comparing `ritc-0.0.4/LICENSE` & `ritc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ritc-0.0.4/PKG-INFO` & `ritc-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritc
-Version: 0.0.4
+Version: 1.0.0
 Summary: A Python library for interactions with Rotman Interactive Trader Market Simulator Client Application via REST exchange API
 Home-page: https://github.com/AussieSeaweed/ritc
 Author: Juho Kim
 Author-email: juho-kim@outlook.com
 License: MIT
 Project-URL: Documentation, https://ritc.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AussieSeaweed/ritc
```

### Comparing `ritc-0.0.4/README.rst` & `ritc-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `ritc-0.0.4/ritc/__init__.py` & `ritc-1.0.0/ritc/__init__.py`

 * *Files identical despite different names*

### Comparing `ritc-0.0.4/ritc.egg-info/PKG-INFO` & `ritc-1.0.0/ritc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritc
-Version: 0.0.4
+Version: 1.0.0
 Summary: A Python library for interactions with Rotman Interactive Trader Market Simulator Client Application via REST exchange API
 Home-page: https://github.com/AussieSeaweed/ritc
 Author: Juho Kim
 Author-email: juho-kim@outlook.com
 License: MIT
 Project-URL: Documentation, https://ritc.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AussieSeaweed/ritc
```

### Comparing `ritc-0.0.4/setup.py` & `ritc-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from distutils.core import setup
 
 setup(
     name='ritc',
-    version='0.0.4',
+    version='1.0.0',
     description='A Python library for interactions with Rotman Interactive '
                 'Trader Market Simulator Client Application via REST exchange '
                 'API',
     long_description=open('README.rst', 'r').read(),
     long_description_content_type='text/x-rst',
     author='Juho Kim',
     author_email='juho-kim@outlook.com',
```

