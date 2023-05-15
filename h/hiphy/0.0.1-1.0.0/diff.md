# Comparing `tmp/hiphy-0.0.1-py3.9.egg` & `tmp/hiphy-1.0.0-py3.9.egg`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 6149 bytes, number of entries: 8
--rw-r--r--  2.0 unx     9634 b- defN 23-May-15 13:15 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      176 b- defN 23-May-15 13:15 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 13:15 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-15 13:15 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 13:15 EGG-INFO/zip-safe
--rwxr-xr-x  2.0 unx     3156 b- defN 23-May-15 13:15 EGG-INFO/scripts/hiphy
+Zip file size: 7389 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9491 b- defN 23-May-15 13:59 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      204 b- defN 23-May-15 13:59 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 13:59 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       74 b- defN 23-May-15 13:59 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-15 13:59 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 13:59 EGG-INFO/zip-safe
+-rwxr-xr-x  2.0 unx     3205 b- defN 23-May-15 13:59 EGG-INFO/scripts/hiphy
 -rw-r--r--  2.0 unx        0 b- defN 23-May-15 12:06 scripts/__init__.py
--rw-r--r--  2.0 unx      144 b- defN 23-May-15 13:15 scripts/__pycache__/__init__.cpython-39.pyc
-8 files, 13120 bytes uncompressed, 5141 bytes compressed:  60.8%
+-rwxr-xr-x  2.0 unx     3169 b- defN 23-May-15 13:12 scripts/hiphy
+-rw-r--r--  2.0 unx      144 b- defN 23-May-15 13:59 scripts/__pycache__/__init__.cpython-39.pyc
+10 files, 16297 bytes uncompressed, 6161 bytes compressed:  62.2%
```

## zipnote «TEMP»/diffoscope_nmzr1lqq_/tmpdsh1tm_u_.zip

```diff
@@ -3,23 +3,29 @@
 
 Filename: EGG-INFO/SOURCES.txt
 Comment: 
 
 Filename: EGG-INFO/dependency_links.txt
 Comment: 
 
+Filename: EGG-INFO/requires.txt
+Comment: 
+
 Filename: EGG-INFO/top_level.txt
 Comment: 
 
 Filename: EGG-INFO/zip-safe
 Comment: 
 
 Filename: EGG-INFO/scripts/hiphy
 Comment: 
 
 Filename: scripts/__init__.py
 Comment: 
 
+Filename: scripts/hiphy
+Comment: 
+
 Filename: scripts/__pycache__/__init__.cpython-39.pyc
 Comment: 
 
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: hiphy
-Version: 0.0.1
-Summary: A python package making videos dance
+Version: 1.0.0
+Summary: Command-line tool to make videos dance.
 Home-page: https://github.com/austinbrown34/hiphy-pip
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # How to Publish a Pip or Conda library (Companion Repo to [Earth Lab blog post](https://www.colorado.edu/earthlab/2019/01/03/publishing-your-python-code-pip-and-conda-tips-and-best-practices))
 
 For more detailed information on building and managing python libraries properly, see my [Blog Post](https://blog.willmnorris.com/2020/10/tools-for-writing-effective-and-robust.html) on Unit Testing, Continuous Integration, and Linting in python.
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
 setup.py
 hiphy.egg-info/PKG-INFO
 hiphy.egg-info/SOURCES.txt
 hiphy.egg-info/dependency_links.txt
+hiphy.egg-info/requires.txt
 hiphy.egg-info/top_level.txt
 scripts/__init__.py
 scripts/hiphy
```

## EGG-INFO/scripts/hiphy

```diff
@@ -1,8 +1,8 @@
-#!python
+#!/Users/austinbrown/miniforge3/envs/hiphy-pip/bin/python
 
 import sys
 sys.path.append('../visbeats')
 import argparse
 from hiphy import Hiphy
 from datetime import datetime
 import json
```

