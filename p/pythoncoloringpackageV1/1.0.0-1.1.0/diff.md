# Comparing `tmp/pythoncoloringpackageV1-1.0.0.tar.gz` & `tmp/pythoncoloringpackageV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoloringpackageV1-1.0.0.tar", last modified: Sun May 14 23:40:24 2023, max compression
+gzip compressed data, was "pythoncoloringpackageV1-1.1.0.tar", last modified: Sun May 14 23:42:29 2023, max compression
```

## Comparing `pythoncoloringpackageV1-1.0.0.tar` & `pythoncoloringpackageV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:40:24.077583 pythoncoloringpackageV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      356 2023-05-14 23:40:24.077583 pythoncoloringpackageV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:40:24.077583 pythoncoloringpackageV1-1.0.0/pythoncoloringpackageV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 23:40:23.000000 pythoncoloringpackageV1-1.0.0/pythoncoloringpackageV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:40:24.077583 pythoncoloringpackageV1-1.0.0/pythoncoloringpackageV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      356 2023-05-14 23:40:24.000000 pythoncoloringpackageV1-1.0.0/pythoncoloringpackageV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-05-14 23:40:24.000000 pythoncoloringpackageV1-1.0.0/pythoncoloringpackageV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 23:40:24.000000 pythoncoloringpackageV1-1.0.0/pythoncoloringpackageV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-14 23:40:24.000000 pythoncoloringpackageV1-1.0.0/pythoncoloringpackageV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 23:40:24.077583 pythoncoloringpackageV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      569 2023-05-14 23:40:23.000000 pythoncoloringpackageV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:42:29.352212 pythoncoloringpackageV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      356 2023-05-14 23:42:29.352212 pythoncoloringpackageV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:42:29.352212 pythoncoloringpackageV1-1.1.0/pythoncoloringpackageV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-14 23:42:29.000000 pythoncoloringpackageV1-1.1.0/pythoncoloringpackageV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:42:29.352212 pythoncoloringpackageV1-1.1.0/pythoncoloringpackageV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      356 2023-05-14 23:42:29.000000 pythoncoloringpackageV1-1.1.0/pythoncoloringpackageV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2023-05-14 23:42:29.000000 pythoncoloringpackageV1-1.1.0/pythoncoloringpackageV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 23:42:29.000000 pythoncoloringpackageV1-1.1.0/pythoncoloringpackageV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-14 23:42:29.000000 pythoncoloringpackageV1-1.1.0/pythoncoloringpackageV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 23:42:29.352212 pythoncoloringpackageV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      569 2023-05-14 23:42:29.000000 pythoncoloringpackageV1-1.1.0/setup.py
```

### Comparing `pythoncoloringpackageV1-1.0.0/setup.py` & `pythoncoloringpackageV1-1.1.0/setup.py`

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
     name="pythoncoloringpackageV1",
     version=VERSION,
```

