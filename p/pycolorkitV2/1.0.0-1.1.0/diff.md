# Comparing `tmp/pycolorkitV2-1.0.0.tar.gz` & `tmp/pycolorkitV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolorkitV2-1.0.0.tar", last modified: Mon May 15 17:15:08 2023, max compression
+gzip compressed data, was "pycolorkitV2-1.1.0.tar", last modified: Mon May 15 17:17:14 2023, max compression
```

## Comparing `pycolorkitV2-1.0.0.tar` & `pycolorkitV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:15:08.699411 pycolorkitV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-15 17:15:08.699411 pycolorkitV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:15:08.699411 pycolorkitV2-1.0.0/pycolorkitV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 17:15:08.000000 pycolorkitV2-1.0.0/pycolorkitV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:15:08.699411 pycolorkitV2-1.0.0/pycolorkitV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-15 17:15:08.000000 pycolorkitV2-1.0.0/pycolorkitV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-15 17:15:08.000000 pycolorkitV2-1.0.0/pycolorkitV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 17:15:08.000000 pycolorkitV2-1.0.0/pycolorkitV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 17:15:08.000000 pycolorkitV2-1.0.0/pycolorkitV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 17:15:08.699411 pycolorkitV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-15 17:15:08.000000 pycolorkitV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:17:14.309998 pycolorkitV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-15 17:17:14.309998 pycolorkitV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:17:14.305998 pycolorkitV2-1.1.0/pycolorkitV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 17:17:14.000000 pycolorkitV2-1.1.0/pycolorkitV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:17:14.309998 pycolorkitV2-1.1.0/pycolorkitV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-15 17:17:14.000000 pycolorkitV2-1.1.0/pycolorkitV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-15 17:17:14.000000 pycolorkitV2-1.1.0/pycolorkitV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 17:17:14.000000 pycolorkitV2-1.1.0/pycolorkitV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-15 17:17:14.000000 pycolorkitV2-1.1.0/pycolorkitV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 17:17:14.309998 pycolorkitV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-15 17:17:14.000000 pycolorkitV2-1.1.0/setup.py
```

### Comparing `pycolorkitV2-1.0.0/setup.py` & `pycolorkitV2-1.1.0/setup.py`

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
     name="pycolorkitV2",
     version=VERSION,
```

