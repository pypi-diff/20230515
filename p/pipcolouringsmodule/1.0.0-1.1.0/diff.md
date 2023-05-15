# Comparing `tmp/pipcolouringsmodule-1.0.0.tar.gz` & `tmp/pipcolouringsmodule-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcolouringsmodule-1.0.0.tar", last modified: Mon May 15 14:35:48 2023, max compression
+gzip compressed data, was "pipcolouringsmodule-1.1.0.tar", last modified: Mon May 15 14:37:53 2023, max compression
```

## Comparing `pipcolouringsmodule-1.0.0.tar` & `pipcolouringsmodule-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 14:35:48.623620 pipcolouringsmodule-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-15 14:35:48.623620 pipcolouringsmodule-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 14:35:48.623620 pipcolouringsmodule-1.0.0/pipcolouringsmodule/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 14:35:48.000000 pipcolouringsmodule-1.0.0/pipcolouringsmodule/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 14:35:48.623620 pipcolouringsmodule-1.0.0/pipcolouringsmodule.egg-info/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-15 14:35:48.000000 pipcolouringsmodule-1.0.0/pipcolouringsmodule.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-15 14:35:48.000000 pipcolouringsmodule-1.0.0/pipcolouringsmodule.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 14:35:48.000000 pipcolouringsmodule-1.0.0/pipcolouringsmodule.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-15 14:35:48.000000 pipcolouringsmodule-1.0.0/pipcolouringsmodule.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 14:35:48.623620 pipcolouringsmodule-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-15 14:35:48.000000 pipcolouringsmodule-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 14:37:53.822284 pipcolouringsmodule-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-15 14:37:53.822284 pipcolouringsmodule-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 14:37:53.822284 pipcolouringsmodule-1.1.0/pipcolouringsmodule/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 14:37:53.000000 pipcolouringsmodule-1.1.0/pipcolouringsmodule/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 14:37:53.822284 pipcolouringsmodule-1.1.0/pipcolouringsmodule.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-15 14:37:53.000000 pipcolouringsmodule-1.1.0/pipcolouringsmodule.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-15 14:37:53.000000 pipcolouringsmodule-1.1.0/pipcolouringsmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 14:37:53.000000 pipcolouringsmodule-1.1.0/pipcolouringsmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-15 14:37:53.000000 pipcolouringsmodule-1.1.0/pipcolouringsmodule.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 14:37:53.822284 pipcolouringsmodule-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-15 14:37:53.000000 pipcolouringsmodule-1.1.0/setup.py
```

### Comparing `pipcolouringsmodule-1.0.0/setup.py` & `pipcolouringsmodule-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcolouringsmodule",
     version=VERSION,
```

