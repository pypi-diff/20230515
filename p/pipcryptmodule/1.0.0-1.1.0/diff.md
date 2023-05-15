# Comparing `tmp/pipcryptmodule-1.0.0.tar.gz` & `tmp/pipcryptmodule-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptmodule-1.0.0.tar", last modified: Mon May 15 02:03:02 2023, max compression
+gzip compressed data, was "pipcryptmodule-1.1.0.tar", last modified: Mon May 15 02:05:08 2023, max compression
```

## Comparing `pipcryptmodule-1.0.0.tar` & `pipcryptmodule-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:03:02.670962 pipcryptmodule-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-15 02:03:02.670962 pipcryptmodule-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:03:02.670962 pipcryptmodule-1.0.0/pipcryptmodule/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 02:03:02.000000 pipcryptmodule-1.0.0/pipcryptmodule/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:03:02.670962 pipcryptmodule-1.0.0/pipcryptmodule.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-15 02:03:02.000000 pipcryptmodule-1.0.0/pipcryptmodule.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-15 02:03:02.000000 pipcryptmodule-1.0.0/pipcryptmodule.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:03:02.000000 pipcryptmodule-1.0.0/pipcryptmodule.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-15 02:03:02.000000 pipcryptmodule-1.0.0/pipcryptmodule.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 02:03:02.670962 pipcryptmodule-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-15 02:03:02.000000 pipcryptmodule-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:05:08.853553 pipcryptmodule-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-15 02:05:08.853553 pipcryptmodule-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:05:08.853553 pipcryptmodule-1.1.0/pipcryptmodule/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 02:05:08.000000 pipcryptmodule-1.1.0/pipcryptmodule/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 02:05:08.853553 pipcryptmodule-1.1.0/pipcryptmodule.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-15 02:05:08.000000 pipcryptmodule-1.1.0/pipcryptmodule.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-15 02:05:08.000000 pipcryptmodule-1.1.0/pipcryptmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 02:05:08.000000 pipcryptmodule-1.1.0/pipcryptmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-15 02:05:08.000000 pipcryptmodule-1.1.0/pipcryptmodule.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 02:05:08.853553 pipcryptmodule-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-15 02:05:08.000000 pipcryptmodule-1.1.0/setup.py
```

### Comparing `pipcryptmodule-1.0.0/setup.py` & `pipcryptmodule-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcryptmodule",
     version=VERSION,
```

