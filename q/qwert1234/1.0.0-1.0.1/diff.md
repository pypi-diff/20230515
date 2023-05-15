# Comparing `tmp/qwert1234-1.0.0.tar.gz` & `tmp/qwert1234-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwert1234-1.0.0.tar", last modified: Mon May 15 11:21:34 2023, max compression
+gzip compressed data, was "qwert1234-1.0.1.tar", last modified: Mon May 15 11:34:40 2023, max compression
```

## Comparing `qwert1234-1.0.0.tar` & `qwert1234-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:21:34.587917 qwert1234-1.0.0/
--rw-rw-rw-   0        0        0      825 2023-05-15 11:21:34.587422 qwert1234-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-05-15 11:05:22.000000 qwert1234-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:21:34.586925 qwert1234-1.0.0/qwert1234.egg-info/
--rw-rw-rw-   0        0        0      825 2023-05-15 11:21:34.000000 qwert1234-1.0.0/qwert1234.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-05-15 11:21:34.000000 qwert1234-1.0.0/qwert1234.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:21:34.000000 qwert1234-1.0.0/qwert1234.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-15 11:21:34.000000 qwert1234-1.0.0/qwert1234.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 11:21:34.587917 qwert1234-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-05-15 11:21:26.000000 qwert1234-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:34:40.897348 qwert1234-1.0.1/
+-rw-rw-rw-   0        0        0      825 2023-05-15 11:34:40.897348 qwert1234-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-05-15 11:05:22.000000 qwert1234-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 11:34:40.896356 qwert1234-1.0.1/qwert1234.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-05-15 11:34:40.000000 qwert1234-1.0.1/qwert1234.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2023-05-15 11:34:40.000000 qwert1234-1.0.1/qwert1234.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:34:40.000000 qwert1234-1.0.1/qwert1234.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 11:34:40.000000 qwert1234-1.0.1/qwert1234.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 11:34:40.897348 qwert1234-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-05-15 11:32:27.000000 qwert1234-1.0.1/setup.py
```

### Comparing `qwert1234-1.0.0/PKG-INFO` & `qwert1234-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwert1234
-Version: 1.0.0
+Version: 1.0.1
 Summary: A description of your library
 Home-page: 
 Author: Evolt
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qwert1234-1.0.0/qwert1234.egg-info/PKG-INFO` & `qwert1234-1.0.1/qwert1234.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwert1234
-Version: 1.0.0
+Version: 1.0.1
 Summary: A description of your library
 Home-page: 
 Author: Evolt
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qwert1234-1.0.0/setup.py` & `qwert1234-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 import os
 setup(
     name='qwert1234',
-    version='1.0.0',
+    version='1.0.1',
     author='Evolt',
     author_email='',
     description='A description of your library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='',
-    packages=['src'],
+    packages=["qwert1234"],
     install_requires="",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

