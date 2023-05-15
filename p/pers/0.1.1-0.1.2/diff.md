# Comparing `tmp/pers-0.1.1.tar.gz` & `tmp/pers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pers-0.1.1.tar", last modified: Mon May 15 19:48:59 2023, max compression
+gzip compressed data, was "pers-0.1.2.tar", last modified: Mon May 15 19:49:46 2023, max compression
```

## Comparing `pers-0.1.1.tar` & `pers-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:48:59.649227 pers-0.1.1/
--rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-05-02 13:14:10.000000 pers-0.1.1/LICENSE
--rw-r--r--   0 ok        (1000) ok        (1000)     3465 2023-05-15 19:48:59.649227 pers-0.1.1/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)     2983 2023-05-15 19:47:59.000000 pers-0.1.1/README.md
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:48:59.648227 pers-0.1.1/pers/
--rw-r--r--   0 ok        (1000) ok        (1000)       19 2023-05-02 13:13:28.000000 pers-0.1.1/pers/__init__.py
--rw-r--r--   0 ok        (1000) ok        (1000)     3580 2023-05-15 19:41:34.000000 pers-0.1.1/pers/pers.py
--rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-05-15 19:48:09.000000 pers-0.1.1/pers/version.py
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:48:59.649227 pers-0.1.1/pers.egg-info/
--rw-r--r--   0 ok        (1000) ok        (1000)     3465 2023-05-15 19:48:59.000000 pers-0.1.1/pers.egg-info/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)      217 2023-05-15 19:48:59.000000 pers-0.1.1/pers.egg-info/SOURCES.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-15 19:48:59.000000 pers-0.1.1/pers.egg-info/dependency_links.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       12 2023-05-15 19:48:59.000000 pers-0.1.1/pers.egg-info/requires.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        5 2023-05-15 19:48:59.000000 pers-0.1.1/pers.egg-info/top_level.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-15 19:48:59.649227 pers-0.1.1/setup.cfg
--rw-r--r--   0 ok        (1000) ok        (1000)     1103 2023-05-15 19:45:08.000000 pers-0.1.1/setup.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:49:46.703617 pers-0.1.2/
+-rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-05-02 13:14:10.000000 pers-0.1.2/LICENSE
+-rw-r--r--   0 ok        (1000) ok        (1000)     3495 2023-05-15 19:49:46.703617 pers-0.1.2/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)     2983 2023-05-15 19:47:59.000000 pers-0.1.2/README.md
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:49:46.701617 pers-0.1.2/pers/
+-rw-r--r--   0 ok        (1000) ok        (1000)       19 2023-05-02 13:13:28.000000 pers-0.1.2/pers/__init__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)     3580 2023-05-15 19:41:34.000000 pers-0.1.2/pers/pers.py
+-rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-05-15 19:49:33.000000 pers-0.1.2/pers/version.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-15 19:49:46.702617 pers-0.1.2/pers.egg-info/
+-rw-r--r--   0 ok        (1000) ok        (1000)     3495 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      217 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/SOURCES.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/dependency_links.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       12 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/requires.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        5 2023-05-15 19:49:46.000000 pers-0.1.2/pers.egg-info/top_level.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-15 19:49:46.703617 pers-0.1.2/setup.cfg
+-rw-r--r--   0 ok        (1000) ok        (1000)     1133 2023-05-15 19:49:22.000000 pers-0.1.2/setup.py
```

### Comparing `pers-0.1.1/LICENSE` & `pers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pers-0.1.1/PKG-INFO` & `pers-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pers
-Version: 0.1.1
+Version: 0.1.2
 Summary: Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
-Home-page: 
+Home-page: https://github.com/rsusik/pers
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
```

### Comparing `pers-0.1.1/README.md` & `pers-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pers-0.1.1/pers/pers.py` & `pers-0.1.2/pers/pers.py`

 * *Files identical despite different names*

### Comparing `pers-0.1.1/pers.egg-info/PKG-INFO` & `pers-0.1.2/pers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pers
-Version: 0.1.1
+Version: 0.1.2
 Summary: Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
-Home-page: 
+Home-page: https://github.com/rsusik/pers
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
```

### Comparing `pers-0.1.1/setup.py` & `pers-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     ),
     long_description=io.open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     python_requires='>=3.8',
     install_requires=get_requirements(),
     package_dir={'': '.'},
     packages=find_packages(where='.'),
-    url='',
+    url='https://github.com/rsusik/pers',
     classifiers=[
         'Topic :: Utilities',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
     ],
 )
```

