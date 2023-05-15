# Comparing `tmp/syssqlite2extensions-1.0.0.tar.gz` & `tmp/syssqlite2extensions-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlite2extensions-1.0.0.tar", last modified: Mon May 15 01:10:28 2023, max compression
+gzip compressed data, was "syssqlite2extensions-1.1.0.tar", last modified: Mon May 15 01:12:35 2023, max compression
```

## Comparing `syssqlite2extensions-1.0.0.tar` & `syssqlite2extensions-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:10:28.486418 syssqlite2extensions-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 01:10:28.486418 syssqlite2extensions-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 01:10:28.486418 syssqlite2extensions-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-15 01:10:28.000000 syssqlite2extensions-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:10:28.482418 syssqlite2extensions-1.0.0/syssqlite2extensions/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 01:10:28.000000 syssqlite2extensions-1.0.0/syssqlite2extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:10:28.486418 syssqlite2extensions-1.0.0/syssqlite2extensions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 01:10:28.000000 syssqlite2extensions-1.0.0/syssqlite2extensions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-05-15 01:10:28.000000 syssqlite2extensions-1.0.0/syssqlite2extensions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 01:10:28.000000 syssqlite2extensions-1.0.0/syssqlite2extensions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 01:10:28.000000 syssqlite2extensions-1.0.0/syssqlite2extensions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:12:35.388990 syssqlite2extensions-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 01:12:35.388990 syssqlite2extensions-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 01:12:35.388990 syssqlite2extensions-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-15 01:12:35.000000 syssqlite2extensions-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:12:35.388990 syssqlite2extensions-1.1.0/syssqlite2extensions/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 01:12:35.000000 syssqlite2extensions-1.1.0/syssqlite2extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 01:12:35.388990 syssqlite2extensions-1.1.0/syssqlite2extensions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 01:12:35.000000 syssqlite2extensions-1.1.0/syssqlite2extensions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-05-15 01:12:35.000000 syssqlite2extensions-1.1.0/syssqlite2extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 01:12:35.000000 syssqlite2extensions-1.1.0/syssqlite2extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 01:12:35.000000 syssqlite2extensions-1.1.0/syssqlite2extensions.egg-info/top_level.txt
```

### Comparing `syssqlite2extensions-1.0.0/setup.py` & `syssqlite2extensions-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syssqlite2extensions",
     version=VERSION,
```

