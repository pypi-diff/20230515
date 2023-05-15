# Comparing `tmp/autogluon-0.7.1b20230514.tar.gz` & `tmp/autogluon-0.7.1b20230515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.7.1b20230514.tar", last modified: Sun May 14 09:04:17 2023, max compression
+gzip compressed data, was "autogluon-0.7.1b20230515.tar", last modified: Mon May 15 09:04:37 2023, max compression
```

## Comparing `autogluon-0.7.1b20230514.tar` & `autogluon-0.7.1b20230515.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:04:17.415749 autogluon-0.7.1b20230514/
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-14 09:04:17.415749 autogluon-0.7.1b20230514/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 09:04:17.419749 autogluon-0.7.1b20230514/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-14 09:03:30.000000 autogluon-0.7.1b20230514/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:04:17.415749 autogluon-0.7.1b20230514/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:04:17.415749 autogluon-0.7.1b20230514/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-14 09:03:30.000000 autogluon-0.7.1b20230514/src/autogluon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-14 09:04:17.000000 autogluon-0.7.1b20230514/src/autogluon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:04:17.415749 autogluon-0.7.1b20230514/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-14 09:04:17.000000 autogluon-0.7.1b20230514/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-14 09:04:17.000000 autogluon-0.7.1b20230514/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:04:17.000000 autogluon-0.7.1b20230514/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 09:04:17.000000 autogluon-0.7.1b20230514/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-14 09:04:17.000000 autogluon-0.7.1b20230514/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 09:04:17.000000 autogluon-0.7.1b20230514/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:04:17.000000 autogluon-0.7.1b20230514/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:37.462293 autogluon-0.7.1b20230515/
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-15 09:04:37.462293 autogluon-0.7.1b20230515/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:04:37.462293 autogluon-0.7.1b20230515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-15 09:03:46.000000 autogluon-0.7.1b20230515/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:37.458293 autogluon-0.7.1b20230515/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:37.462293 autogluon-0.7.1b20230515/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 09:03:46.000000 autogluon-0.7.1b20230515/src/autogluon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 09:04:37.000000 autogluon-0.7.1b20230515/src/autogluon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:37.462293 autogluon-0.7.1b20230515/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-15 09:04:37.000000 autogluon-0.7.1b20230515/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 09:04:37.000000 autogluon-0.7.1b20230515/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:04:37.000000 autogluon-0.7.1b20230515/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 09:04:37.000000 autogluon-0.7.1b20230515/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-15 09:04:37.000000 autogluon-0.7.1b20230515/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 09:04:37.000000 autogluon-0.7.1b20230515/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:04:37.000000 autogluon-0.7.1b20230515/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.7.1b20230514/PKG-INFO` & `autogluon-0.7.1b20230515/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230514
+Version: 0.7.1b20230515
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.7.1b20230514/setup.py` & `autogluon-0.7.1b20230515/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.7.1b20230514/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.7.1b20230515/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230514
+Version: 0.7.1b20230515
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

