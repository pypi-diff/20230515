# Comparing `tmp/visbeats-0.0.2-py3.9.egg` & `tmp/visbeats-0.0.3-py3.9.egg`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6090 bytes, number of entries: 8
--rw-r--r--  2.0 unx     9640 b- defN 23-May-15 12:16 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx     1399 b- defN 23-May-15 12:16 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 12:16 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-15 12:16 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 12:16 EGG-INFO/zip-safe
--rwxr-xr-x  2.0 unx     1495 b- defN 23-May-15 12:12 EGG-INFO/scripts/visbeats
+Zip file size: 6122 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     9640 b- defN 23-May-15 17:29 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx     1399 b- defN 23-May-15 17:29 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 17:29 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-15 17:29 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 17:29 EGG-INFO/zip-safe
+-rwxr-xr-x  2.0 unx     1547 b- defN 23-May-15 17:29 EGG-INFO/scripts/visbeats
 -rw-r--r--  2.0 unx        0 b- defN 23-May-15 12:06 scripts/__init__.py
--rw-r--r--  2.0 unx      144 b- defN 23-May-15 12:16 scripts/__pycache__/__init__.cpython-39.pyc
-8 files, 12688 bytes uncompressed, 5076 bytes compressed:  60.0%
+-rw-r--r--  2.0 unx      144 b- defN 23-May-15 17:29 scripts/__pycache__/__init__.cpython-39.pyc
+8 files, 12740 bytes uncompressed, 5108 bytes compressed:  59.9%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visbeats
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package making videos dance
 Home-page: https://github.com/austinbrown34/visbeats-pip
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

## EGG-INFO/scripts/visbeats

```diff
@@ -1,8 +1,8 @@
-#!python
+#!/Users/austinbrown/miniforge3/envs/visbeats-pip/bin/python
 
 import sys
 import argparse
 import matplotlib
 matplotlib.use('PS')
 sys.path.append('../visbeats')
 import visbeats
```

