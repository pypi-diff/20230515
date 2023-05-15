# Comparing `tmp/pythoncolouringspackagesV1-1.0.0.tar.gz` & `tmp/pythoncolouringspackagesV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncolouringspackagesV1-1.0.0.tar", last modified: Mon May 15 16:23:31 2023, max compression
+gzip compressed data, was "pythoncolouringspackagesV1-1.1.0.tar", last modified: Mon May 15 16:25:37 2023, max compression
```

## Comparing `pythoncolouringspackagesV1-1.0.0.tar` & `pythoncolouringspackagesV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:23:31.948858 pythoncolouringspackagesV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      359 2023-05-15 16:23:31.948858 pythoncolouringspackagesV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:23:31.948858 pythoncolouringspackagesV1-1.0.0/pythoncolouringspackagesV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 16:23:31.000000 pythoncolouringspackagesV1-1.0.0/pythoncolouringspackagesV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:23:31.948858 pythoncolouringspackagesV1-1.0.0/pythoncolouringspackagesV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      359 2023-05-15 16:23:31.000000 pythoncolouringspackagesV1-1.0.0/pythoncolouringspackagesV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-15 16:23:31.000000 pythoncolouringspackagesV1-1.0.0/pythoncolouringspackagesV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 16:23:31.000000 pythoncolouringspackagesV1-1.0.0/pythoncolouringspackagesV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-15 16:23:31.000000 pythoncolouringspackagesV1-1.0.0/pythoncolouringspackagesV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 16:23:31.948858 pythoncolouringspackagesV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-15 16:23:31.000000 pythoncolouringspackagesV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:25:37.007470 pythoncolouringspackagesV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-05-15 16:25:37.007470 pythoncolouringspackagesV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:25:37.003470 pythoncolouringspackagesV1-1.1.0/pythoncolouringspackagesV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 16:25:36.000000 pythoncolouringspackagesV1-1.1.0/pythoncolouringspackagesV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:25:37.007470 pythoncolouringspackagesV1-1.1.0/pythoncolouringspackagesV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-05-15 16:25:36.000000 pythoncolouringspackagesV1-1.1.0/pythoncolouringspackagesV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-15 16:25:36.000000 pythoncolouringspackagesV1-1.1.0/pythoncolouringspackagesV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 16:25:36.000000 pythoncolouringspackagesV1-1.1.0/pythoncolouringspackagesV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-15 16:25:36.000000 pythoncolouringspackagesV1-1.1.0/pythoncolouringspackagesV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 16:25:37.007470 pythoncolouringspackagesV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      572 2023-05-15 16:25:36.000000 pythoncolouringspackagesV1-1.1.0/setup.py
```

### Comparing `pythoncolouringspackagesV1-1.0.0/setup.py` & `pythoncolouringspackagesV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncolouringspackagesV1",
     version=VERSION,
```

