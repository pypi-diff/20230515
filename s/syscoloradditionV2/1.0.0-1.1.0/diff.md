# Comparing `tmp/syscoloradditionV2-1.0.0.tar.gz` & `tmp/syscoloradditionV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscoloradditionV2-1.0.0.tar", last modified: Mon May 15 11:13:26 2023, max compression
+gzip compressed data, was "syscoloradditionV2-1.1.0.tar", last modified: Mon May 15 11:15:34 2023, max compression
```

## Comparing `syscoloradditionV2-1.0.0.tar` & `syscoloradditionV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:13:26.987907 syscoloradditionV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-15 11:13:26.987907 syscoloradditionV2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 11:13:26.987907 syscoloradditionV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-15 11:13:26.000000 syscoloradditionV2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:13:26.987907 syscoloradditionV2-1.0.0/syscoloradditionV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 11:13:26.000000 syscoloradditionV2-1.0.0/syscoloradditionV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:13:26.987907 syscoloradditionV2-1.0.0/syscoloradditionV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-15 11:13:26.000000 syscoloradditionV2-1.0.0/syscoloradditionV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-15 11:13:26.000000 syscoloradditionV2-1.0.0/syscoloradditionV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 11:13:26.000000 syscoloradditionV2-1.0.0/syscoloradditionV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-15 11:13:26.000000 syscoloradditionV2-1.0.0/syscoloradditionV2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:15:34.242501 syscoloradditionV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-15 11:15:34.242501 syscoloradditionV2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 11:15:34.246501 syscoloradditionV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-15 11:15:34.000000 syscoloradditionV2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:15:34.242501 syscoloradditionV2-1.1.0/syscoloradditionV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 11:15:34.000000 syscoloradditionV2-1.1.0/syscoloradditionV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:15:34.242501 syscoloradditionV2-1.1.0/syscoloradditionV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-15 11:15:34.000000 syscoloradditionV2-1.1.0/syscoloradditionV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-15 11:15:34.000000 syscoloradditionV2-1.1.0/syscoloradditionV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 11:15:34.000000 syscoloradditionV2-1.1.0/syscoloradditionV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-15 11:15:34.000000 syscoloradditionV2-1.1.0/syscoloradditionV2.egg-info/top_level.txt
```

### Comparing `syscoloradditionV2-1.0.0/setup.py` & `syscoloradditionV2-1.1.0/setup.py`

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
     name="syscoloradditionV2",
     version=VERSION,
```

