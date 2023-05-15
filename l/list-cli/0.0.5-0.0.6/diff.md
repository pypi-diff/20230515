# Comparing `tmp/list-cli-0.0.5.tar.gz` & `tmp/list-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/list-cli-0.0.5.tar", last modified: Sat Nov  9 01:00:32 2019, max compression
+gzip compressed data, was "list-cli-0.0.6.tar", last modified: Sun Jun 13 13:21:50 2021, max compression
```

## Comparing `list-cli-0.0.5.tar` & `list-cli-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 jzaleski (1116128489) admin       (80)        0 2019-11-09 01:00:32.000000 list-cli-0.0.5/
--rw-r--r--   0 jzaleski (1116128489) admin       (80)      848 2019-11-09 01:00:32.000000 list-cli-0.0.5/PKG-INFO
--rw-r--r--   0 jzaleski (1116128489) admin       (80)     2569 2019-10-30 15:42:48.000000 list-cli-0.0.5/README.md
-drwxr-xr-x   0 jzaleski (1116128489) admin       (80)        0 2019-11-09 01:00:32.000000 list-cli-0.0.5/bin/
--rwxr-xr-x   0 jzaleski (1116128489) admin       (80)      195 2019-10-29 14:51:11.000000 list-cli-0.0.5/bin/reset
--rwxr-xr-x   0 jzaleski (1116128489) admin       (80)      213 2019-10-29 17:07:27.000000 list-cli-0.0.5/bin/run
--rwxr-xr-x   0 jzaleski (1116128489) admin       (80)      162 2019-10-29 14:51:40.000000 list-cli-0.0.5/bin/setup
-drwxr-xr-x   0 jzaleski (1116128489) admin       (80)        0 2019-11-09 01:00:32.000000 list-cli-0.0.5/list/
--rw-r--r--   0 jzaleski (1116128489) admin       (80)        0 2019-10-30 15:49:12.000000 list-cli-0.0.5/list/__init__.py
--rw-r--r--   0 jzaleski (1116128489) admin       (80)      228 2019-11-09 00:40:34.000000 list-cli-0.0.5/list/__main__.py
--rw-r--r--   0 jzaleski (1116128489) admin       (80)    10226 2019-11-09 00:59:36.000000 list-cli-0.0.5/list/cli.py
-drwxr-xr-x   0 jzaleski (1116128489) admin       (80)        0 2019-11-09 01:00:32.000000 list-cli-0.0.5/list_cli.egg-info/
--rw-r--r--   0 jzaleski (1116128489) admin       (80)      848 2019-11-09 01:00:32.000000 list-cli-0.0.5/list_cli.egg-info/PKG-INFO
--rw-r--r--   0 jzaleski (1116128489) admin       (80)      265 2019-11-09 01:00:32.000000 list-cli-0.0.5/list_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jzaleski (1116128489) admin       (80)        1 2019-11-09 01:00:32.000000 list-cli-0.0.5/list_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jzaleski (1116128489) admin       (80)       49 2019-11-09 01:00:32.000000 list-cli-0.0.5/list_cli.egg-info/entry_points.txt
--rw-r--r--   0 jzaleski (1116128489) admin       (80)        5 2019-11-09 01:00:32.000000 list-cli-0.0.5/list_cli.egg-info/top_level.txt
--rw-r--r--   0 jzaleski (1116128489) admin       (80)       79 2019-11-09 01:00:32.000000 list-cli-0.0.5/setup.cfg
--rw-r--r--   0 jzaleski (1116128489) admin       (80)     1446 2019-11-09 00:58:53.000000 list-cli-0.0.5/setup.py
+drwxr-xr-x   0 jzaleski (1116128489) 701497816        0 2021-06-13 13:21:50.837094 list-cli-0.0.6/
+-rw-r--r--   0 jzaleski (1116128489) 701497816     1076 2021-06-13 12:52:30.000000 list-cli-0.0.6/LICENSE
+-rw-r--r--   0 jzaleski (1116128489) 701497816      898 2021-06-13 13:21:50.837284 list-cli-0.0.6/PKG-INFO
+-rw-r--r--   0 jzaleski (1116128489) 701497816     2569 2021-06-13 12:52:30.000000 list-cli-0.0.6/README.md
+drwxr-xr-x   0 jzaleski (1116128489) 701497816        0 2021-06-13 13:21:50.834988 list-cli-0.0.6/list/
+-rw-r--r--   0 jzaleski (1116128489) 701497816        0 2021-06-13 12:52:30.000000 list-cli-0.0.6/list/__init__.py
+-rw-r--r--   0 jzaleski (1116128489) 701497816      228 2021-06-13 12:52:30.000000 list-cli-0.0.6/list/__main__.py
+-rw-r--r--   0 jzaleski (1116128489) 701497816    10226 2021-06-13 13:02:29.000000 list-cli-0.0.6/list/cli.py
+drwxr-xr-x   0 jzaleski (1116128489) 701497816        0 2021-06-13 13:21:50.836714 list-cli-0.0.6/list_cli.egg-info/
+-rw-r--r--   0 jzaleski (1116128489) 701497816      898 2021-06-13 13:21:50.000000 list-cli-0.0.6/list_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jzaleski (1116128489) 701497816      245 2021-06-13 13:21:50.000000 list-cli-0.0.6/list_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jzaleski (1116128489) 701497816        1 2021-06-13 13:21:50.000000 list-cli-0.0.6/list_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jzaleski (1116128489) 701497816       49 2021-06-13 13:21:50.000000 list-cli-0.0.6/list_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jzaleski (1116128489) 701497816        5 2021-06-13 13:21:50.000000 list-cli-0.0.6/list_cli.egg-info/top_level.txt
+-rw-r--r--   0 jzaleski (1116128489) 701497816       79 2021-06-13 13:21:50.837743 list-cli-0.0.6/setup.cfg
+-rw-r--r--   0 jzaleski (1116128489) 701497816     1478 2021-06-13 13:02:01.000000 list-cli-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `list-cli-0.0.5/PKG-INFO` & `list-cli-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: list-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Description: List Management Application (CLI)
 Keywords: list,list-cli,tasktodo
@@ -15,8 +15,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
```

### Comparing `list-cli-0.0.5/README.md` & `list-cli-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `list-cli-0.0.5/list/cli.py` & `list-cli-0.0.6/list/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import getpass
 import re
 import time
 import uuid
 
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 
 class Processor():
     ADDED_BUCKET = 'a'
     ADD_OPERATIONS = {'a', 'add'}
     BUCKET_PATTERN = r'^(a|added|d|done|h|handed_off|m|moved|r|removed)$'
     DEFAULT_PARENT_ID = uuid.UUID('00000000-0000-0000-0000-000000000000')
```

### Comparing `list-cli-0.0.5/list_cli.egg-info/PKG-INFO` & `list-cli-0.0.6/list_cli.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: list-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Description: List Management Application (CLI)
 Keywords: list,list-cli,tasktodo
@@ -15,8 +15,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
```

### Comparing `list-cli-0.0.5/setup.py` & `list-cli-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 
 PKG_NAME = 'list-cli'
 PKG_DESCRIPTION = 'List Management Application (CLI)'
 
 _version_re = re_compile(r'__version__\s+=\s+(.*)')
-with open('list/cli.py'.format(PKG_NAME), 'rb') as f:
+with open('list/cli.py', 'rb') as f:
     PKG_VERSION = str(ast_literal_eval(_version_re.search(
         f.read().decode('utf-8')).group(1)))
 
 setup(
     name=PKG_NAME,
     version=PKG_VERSION,
     url='https://github.com/jzaleski/list-cli',
@@ -30,14 +30,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Software Development',
     ],
     keywords=[
         'list',
         'list-cli',
         'task'
         'todo',
```

