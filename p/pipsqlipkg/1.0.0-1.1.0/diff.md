# Comparing `tmp/pipsqlipkg-1.0.0.tar.gz` & `tmp/pipsqlipkg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlipkg-1.0.0.tar", last modified: Mon May 15 05:30:25 2023, max compression
+gzip compressed data, was "pipsqlipkg-1.1.0.tar", last modified: Mon May 15 05:32:30 2023, max compression
```

## Comparing `pipsqlipkg-1.0.0.tar` & `pipsqlipkg-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:30:25.733381 pipsqlipkg-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-15 05:30:25.733381 pipsqlipkg-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:30:25.733381 pipsqlipkg-1.0.0/pipsqlipkg/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 05:30:25.000000 pipsqlipkg-1.0.0/pipsqlipkg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:30:25.733381 pipsqlipkg-1.0.0/pipsqlipkg.egg-info/
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-15 05:30:25.000000 pipsqlipkg-1.0.0/pipsqlipkg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-15 05:30:25.000000 pipsqlipkg-1.0.0/pipsqlipkg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 05:30:25.000000 pipsqlipkg-1.0.0/pipsqlipkg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-15 05:30:25.000000 pipsqlipkg-1.0.0/pipsqlipkg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 05:30:25.733381 pipsqlipkg-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      556 2023-05-15 05:30:25.000000 pipsqlipkg-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:32:30.192016 pipsqlipkg-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-15 05:32:30.192016 pipsqlipkg-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:32:30.192016 pipsqlipkg-1.1.0/pipsqlipkg/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 05:32:29.000000 pipsqlipkg-1.1.0/pipsqlipkg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 05:32:30.192016 pipsqlipkg-1.1.0/pipsqlipkg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-15 05:32:30.000000 pipsqlipkg-1.1.0/pipsqlipkg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-15 05:32:30.000000 pipsqlipkg-1.1.0/pipsqlipkg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 05:32:30.000000 pipsqlipkg-1.1.0/pipsqlipkg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-15 05:32:30.000000 pipsqlipkg-1.1.0/pipsqlipkg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 05:32:30.192016 pipsqlipkg-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      556 2023-05-15 05:32:29.000000 pipsqlipkg-1.1.0/setup.py
```

### Comparing `pipsqlipkg-1.0.0/setup.py` & `pipsqlipkg-1.1.0/setup.py`

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
     name="pipsqlipkg",
     version=VERSION,
```

