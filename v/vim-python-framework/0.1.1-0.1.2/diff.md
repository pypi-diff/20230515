# Comparing `tmp/vim-python-framework-0.1.1.tar.gz` & `tmp/vim-python-framework-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vim-python-framework-0.1.1.tar", last modified: Mon May 15 20:34:19 2023, max compression
+gzip compressed data, was "vim-python-framework-0.1.2.tar", last modified: Mon May 15 20:57:37 2023, max compression
```

## Comparing `vim-python-framework-0.1.1.tar` & `vim-python-framework-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 20:34:19.891761 vim-python-framework-0.1.1/
--rw-r--r--   0 david     (1000) david     (1000)      199 2023-05-15 20:34:19.891761 vim-python-framework-0.1.1/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-05-15 20:34:19.891761 vim-python-framework-0.1.1/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      467 2023-05-15 20:29:03.000000 vim-python-framework-0.1.1/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 20:34:19.890761 vim-python-framework-0.1.1/vim_python_framework/
--rw-r--r--   0 david     (1000) david     (1000)      132 2023-04-25 22:53:56.000000 vim-python-framework-0.1.1/vim_python_framework/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 20:34:19.891761 vim-python-framework-0.1.1/vim_python_framework.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      199 2023-05-15 20:34:19.000000 vim-python-framework-0.1.1/vim_python_framework.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      307 2023-05-15 20:34:19.000000 vim-python-framework-0.1.1/vim_python_framework.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-15 20:34:19.000000 vim-python-framework-0.1.1/vim_python_framework.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       64 2023-05-15 20:34:19.000000 vim-python-framework-0.1.1/vim_python_framework.egg-info/entry_points.txt
--rw-r--r--   0 david     (1000) david     (1000)       75 2023-05-15 20:34:19.000000 vim-python-framework-0.1.1/vim_python_framework.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       21 2023-05-15 20:34:19.000000 vim-python-framework-0.1.1/vim_python_framework.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 20:57:37.787994 vim-python-framework-0.1.2/
+-rw-r--r--   0 david     (1000) david     (1000)      199 2023-05-15 20:57:37.787994 vim-python-framework-0.1.2/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-05-15 20:57:37.787994 vim-python-framework-0.1.2/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)      445 2023-05-15 20:55:39.000000 vim-python-framework-0.1.2/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 20:57:37.786994 vim-python-framework-0.1.2/vim_python_framework/
+-rw-r--r--   0 david     (1000) david     (1000)      132 2023-04-25 22:53:56.000000 vim-python-framework-0.1.2/vim_python_framework/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 20:57:37.787994 vim-python-framework-0.1.2/vim_python_framework/include/
+-rw-r--r--   0 david     (1000) david     (1000)       16 2023-04-10 02:22:52.000000 vim-python-framework-0.1.2/vim_python_framework/include/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      324 2023-05-08 22:33:37.000000 vim-python-framework-0.1.2/vim_python_framework/include/mymodule.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 20:57:37.787994 vim-python-framework-0.1.2/vim_python_framework/src/
+-rw-r--r--   0 david     (1000) david     (1000)       18 2023-04-10 02:45:09.000000 vim-python-framework-0.1.2/vim_python_framework/src/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)       42 2023-04-10 02:38:31.000000 vim-python-framework-0.1.2/vim_python_framework/src/calculator.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 20:57:37.786994 vim-python-framework-0.1.2/vim_python_framework.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      199 2023-05-15 20:57:37.000000 vim-python-framework-0.1.2/vim_python_framework.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      422 2023-05-15 20:57:37.000000 vim-python-framework-0.1.2/vim_python_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-15 20:57:37.000000 vim-python-framework-0.1.2/vim_python_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       64 2023-05-15 20:57:37.000000 vim-python-framework-0.1.2/vim_python_framework.egg-info/entry_points.txt
+-rw-r--r--   0 david     (1000) david     (1000)       21 2023-05-15 20:57:37.000000 vim-python-framework-0.1.2/vim_python_framework.egg-info/top_level.txt
```

