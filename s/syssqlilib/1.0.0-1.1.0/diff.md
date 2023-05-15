# Comparing `tmp/syssqlilib-1.0.0.tar.gz` & `tmp/syssqlilib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlilib-1.0.0.tar", last modified: Mon May 15 16:52:36 2023, max compression
+gzip compressed data, was "syssqlilib-1.1.0.tar", last modified: Mon May 15 16:54:41 2023, max compression
```

## Comparing `syssqlilib-1.0.0.tar` & `syssqlilib-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:52:36.982786 syssqlilib-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-15 16:52:36.982786 syssqlilib-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 16:52:36.982786 syssqlilib-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      556 2023-05-15 16:52:36.000000 syssqlilib-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:52:36.978786 syssqlilib-1.0.0/syssqlilib/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 16:52:36.000000 syssqlilib-1.0.0/syssqlilib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:52:36.982786 syssqlilib-1.0.0/syssqlilib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-15 16:52:36.000000 syssqlilib-1.0.0/syssqlilib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-15 16:52:36.000000 syssqlilib-1.0.0/syssqlilib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 16:52:36.000000 syssqlilib-1.0.0/syssqlilib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-15 16:52:36.000000 syssqlilib-1.0.0/syssqlilib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:54:41.857451 syssqlilib-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-15 16:54:41.857451 syssqlilib-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 16:54:41.857451 syssqlilib-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      556 2023-05-15 16:54:41.000000 syssqlilib-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:54:41.857451 syssqlilib-1.1.0/syssqlilib/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-15 16:54:41.000000 syssqlilib-1.1.0/syssqlilib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 16:54:41.857451 syssqlilib-1.1.0/syssqlilib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-15 16:54:41.000000 syssqlilib-1.1.0/syssqlilib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-15 16:54:41.000000 syssqlilib-1.1.0/syssqlilib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 16:54:41.000000 syssqlilib-1.1.0/syssqlilib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-15 16:54:41.000000 syssqlilib-1.1.0/syssqlilib.egg-info/top_level.txt
```

