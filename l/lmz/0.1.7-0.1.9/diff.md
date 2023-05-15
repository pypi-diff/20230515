# Comparing `tmp/lmz-0.1.7.tar.gz` & `tmp/lmz-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lmz-0.1.7.tar", last modified: Fri Apr  3 09:45:13 2020, max compression
+gzip compressed data, was "lmz-0.1.9.tar", last modified: Tue Jun  1 21:53:41 2021, max compression
```

## Comparing `lmz-0.1.7.tar` & `lmz-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2020-04-03 09:45:13.000000 lmz-0.1.7/
-drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2020-04-03 09:45:13.000000 lmz-0.1.7/lmz.egg-info/
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      158 2020-04-03 09:45:13.000000 lmz-0.1.7/lmz.egg-info/SOURCES.txt
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      258 2020-04-03 09:45:13.000000 lmz-0.1.7/lmz.egg-info/PKG-INFO
--rw-rw-r--   0 ikea      (1000) ikea      (1000)        1 2020-04-03 09:45:13.000000 lmz-0.1.7/lmz.egg-info/dependency_links.txt
--rw-rw-r--   0 ikea      (1000) ikea      (1000)        4 2020-04-03 09:45:13.000000 lmz-0.1.7/lmz.egg-info/top_level.txt
--rw-rw-r--   0 ikea      (1000) ikea      (1000)       70 2020-01-30 16:03:04.000000 lmz-0.1.7/README.md
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      258 2020-04-03 09:45:13.000000 lmz-0.1.7/PKG-INFO
--rw-rw-r--   0 ikea      (1000) ikea      (1000)     3203 2020-01-30 11:37:58.000000 lmz-0.1.7/setup.py
-drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2020-04-03 09:45:13.000000 lmz-0.1.7/lmz/
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      178 2020-04-03 09:45:13.000000 lmz-0.1.7/lmz/_version.py
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      514 2020-04-03 09:43:26.000000 lmz-0.1.7/lmz/__init__.py
--rw-rw-r--   0 ikea      (1000) ikea      (1000)       38 2020-04-03 09:45:13.000000 lmz-0.1.7/setup.cfg
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2021-06-01 21:53:41.808655 lmz-0.1.9/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      258 2021-06-01 21:53:41.808655 lmz-0.1.9/PKG-INFO
+-rw-r--r--   0 ikea      (1000) ikea      (1000)       70 2020-11-29 19:45:15.000000 lmz-0.1.9/README.md
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2021-06-01 21:53:41.805321 lmz-0.1.9/lmz/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      665 2021-06-01 21:49:36.000000 lmz-0.1.9/lmz/__init__.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      178 2021-06-01 21:53:41.000000 lmz-0.1.9/lmz/_version.py
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2021-06-01 21:53:41.808655 lmz-0.1.9/lmz.egg-info/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      258 2021-06-01 21:53:41.000000 lmz-0.1.9/lmz.egg-info/PKG-INFO
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      158 2021-06-01 21:53:41.000000 lmz-0.1.9/lmz.egg-info/SOURCES.txt
+-rw-r--r--   0 ikea      (1000) ikea      (1000)        1 2021-06-01 21:53:41.000000 lmz-0.1.9/lmz.egg-info/dependency_links.txt
+-rw-r--r--   0 ikea      (1000) ikea      (1000)        4 2021-06-01 21:53:41.000000 lmz-0.1.9/lmz.egg-info/top_level.txt
+-rw-r--r--   0 ikea      (1000) ikea      (1000)       38 2021-06-01 21:53:41.808655 lmz-0.1.9/setup.cfg
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     3203 2020-11-29 19:45:15.000000 lmz-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lmz-0.1.7/setup.py` & `lmz-0.1.9/setup.py`

 * *Files identical despite different names*

