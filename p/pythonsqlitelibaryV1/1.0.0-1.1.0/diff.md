# Comparing `tmp/pythonsqlitelibaryV1-1.0.0.tar.gz` & `tmp/pythonsqlitelibaryV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqlitelibaryV1-1.0.0.tar", last modified: Mon May 15 00:22:56 2023, max compression
+gzip compressed data, was "pythonsqlitelibaryV1-1.1.0.tar", last modified: Mon May 15 00:25:01 2023, max compression
```

## Comparing `pythonsqlitelibaryV1-1.0.0.tar` & `pythonsqlitelibaryV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 00:22:56.037474 pythonsqlitelibaryV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 00:22:56.037474 pythonsqlitelibaryV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 00:22:56.037474 pythonsqlitelibaryV1-1.0.0/pythonsqlitelibaryV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 00:22:55.000000 pythonsqlitelibaryV1-1.0.0/pythonsqlitelibaryV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 00:22:56.037474 pythonsqlitelibaryV1-1.0.0/pythonsqlitelibaryV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 00:22:55.000000 pythonsqlitelibaryV1-1.0.0/pythonsqlitelibaryV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-05-15 00:22:56.000000 pythonsqlitelibaryV1-1.0.0/pythonsqlitelibaryV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 00:22:55.000000 pythonsqlitelibaryV1-1.0.0/pythonsqlitelibaryV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 00:22:55.000000 pythonsqlitelibaryV1-1.0.0/pythonsqlitelibaryV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 00:22:56.037474 pythonsqlitelibaryV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-15 00:22:55.000000 pythonsqlitelibaryV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 00:25:01.204097 pythonsqlitelibaryV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 00:25:01.204097 pythonsqlitelibaryV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 00:25:01.204097 pythonsqlitelibaryV1-1.1.0/pythonsqlitelibaryV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 00:25:00.000000 pythonsqlitelibaryV1-1.1.0/pythonsqlitelibaryV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 00:25:01.204097 pythonsqlitelibaryV1-1.1.0/pythonsqlitelibaryV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 00:25:01.000000 pythonsqlitelibaryV1-1.1.0/pythonsqlitelibaryV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-05-15 00:25:01.000000 pythonsqlitelibaryV1-1.1.0/pythonsqlitelibaryV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 00:25:01.000000 pythonsqlitelibaryV1-1.1.0/pythonsqlitelibaryV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 00:25:01.000000 pythonsqlitelibaryV1-1.1.0/pythonsqlitelibaryV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 00:25:01.204097 pythonsqlitelibaryV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-15 00:25:00.000000 pythonsqlitelibaryV1-1.1.0/setup.py
```

### Comparing `pythonsqlitelibaryV1-1.0.0/setup.py` & `pythonsqlitelibaryV1-1.1.0/setup.py`

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
     name="pythonsqlitelibaryV1",
     version=VERSION,
```

