# Comparing `tmp/pythoncolourlibrary-1.0.0.tar.gz` & `tmp/pythoncolourlibrary-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncolourlibrary-1.0.0.tar", last modified: Mon May 15 15:53:29 2023, max compression
+gzip compressed data, was "pythoncolourlibrary-1.1.0.tar", last modified: Mon May 15 15:55:35 2023, max compression
```

## Comparing `pythoncolourlibrary-1.0.0.tar` & `pythoncolourlibrary-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:53:29.461998 pythoncolourlibrary-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-15 15:53:29.461998 pythoncolourlibrary-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:53:29.461998 pythoncolourlibrary-1.0.0/pythoncolourlibrary/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 15:53:29.000000 pythoncolourlibrary-1.0.0/pythoncolourlibrary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:53:29.461998 pythoncolourlibrary-1.0.0/pythoncolourlibrary.egg-info/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-15 15:53:29.000000 pythoncolourlibrary-1.0.0/pythoncolourlibrary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-15 15:53:29.000000 pythoncolourlibrary-1.0.0/pythoncolourlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 15:53:29.000000 pythoncolourlibrary-1.0.0/pythoncolourlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-15 15:53:29.000000 pythoncolourlibrary-1.0.0/pythoncolourlibrary.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 15:53:29.461998 pythoncolourlibrary-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-15 15:53:29.000000 pythoncolourlibrary-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:55:35.504326 pythoncolourlibrary-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-15 15:55:35.504326 pythoncolourlibrary-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:55:35.504326 pythoncolourlibrary-1.1.0/pythoncolourlibrary/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 15:55:35.000000 pythoncolourlibrary-1.1.0/pythoncolourlibrary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:55:35.504326 pythoncolourlibrary-1.1.0/pythoncolourlibrary.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-15 15:55:35.000000 pythoncolourlibrary-1.1.0/pythoncolourlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-15 15:55:35.000000 pythoncolourlibrary-1.1.0/pythoncolourlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 15:55:35.000000 pythoncolourlibrary-1.1.0/pythoncolourlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-15 15:55:35.000000 pythoncolourlibrary-1.1.0/pythoncolourlibrary.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 15:55:35.504326 pythoncolourlibrary-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-15 15:55:35.000000 pythoncolourlibrary-1.1.0/setup.py
```

### Comparing `pythoncolourlibrary-1.0.0/setup.py` & `pythoncolourlibrary-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncolourlibrary",
     version=VERSION,
```

