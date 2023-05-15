# Comparing `tmp/torqueclient-0.4.0.tar.gz` & `tmp/torqueclient-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torqueclient-0.4.0.tar", last modified: Tue Mar 28 11:50:49 2023, max compression
+gzip compressed data, was "torqueclient-0.4.2.tar", last modified: Mon May 15 17:35:52 2023, max compression
```

## Comparing `torqueclient-0.4.0.tar` & `torqueclient-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:50:49.294648 torqueclient-0.4.0/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    34523 2023-02-19 01:57:21.000000 torqueclient-0.4.0/LICENSE
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      976 2023-03-28 11:50:49.294648 torqueclient-0.4.0/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      502 2023-02-19 01:57:21.000000 torqueclient-0.4.0/README.md
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      107 2023-02-19 01:57:21.000000 torqueclient-0.4.0/pyproject.toml
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2023-03-28 11:50:49.294648 torqueclient-0.4.0/setup.cfg
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      973 2023-02-19 01:57:21.000000 torqueclient-0.4.0/setup.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:50:49.294648 torqueclient-0.4.0/torqueclient/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       36 2023-02-19 01:57:21.000000 torqueclient-0.4.0/torqueclient/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    14055 2023-02-19 01:57:21.000000 torqueclient-0.4.0/torqueclient/api.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6710 2023-02-19 01:57:21.000000 torqueclient-0.4.0/torqueclient/cache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       22 2023-03-28 11:47:12.000000 torqueclient-0.4.0/torqueclient/version.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:50:49.294648 torqueclient-0.4.0/torqueclient.egg-info/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      976 2023-03-28 11:50:49.000000 torqueclient-0.4.0/torqueclient.egg-info/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      319 2023-03-28 11:50:49.000000 torqueclient-0.4.0/torqueclient.egg-info/SOURCES.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2023-03-28 11:50:49.000000 torqueclient-0.4.0/torqueclient.egg-info/dependency_links.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       25 2023-03-28 11:50:49.000000 torqueclient-0.4.0/torqueclient.egg-info/requires.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       13 2023-03-28 11:50:49.000000 torqueclient-0.4.0/torqueclient.egg-info/top_level.txt
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-05-15 17:35:52.454375 torqueclient-0.4.2/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    34523 2023-02-19 01:57:21.000000 torqueclient-0.4.2/LICENSE
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      976 2023-05-15 17:35:52.454375 torqueclient-0.4.2/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      502 2023-02-19 01:57:21.000000 torqueclient-0.4.2/README.md
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      107 2023-02-19 01:57:21.000000 torqueclient-0.4.2/pyproject.toml
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2023-05-15 17:35:52.454375 torqueclient-0.4.2/setup.cfg
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      973 2023-02-19 01:57:21.000000 torqueclient-0.4.2/setup.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-05-15 17:35:52.450375 torqueclient-0.4.2/torqueclient/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       36 2023-02-19 01:57:21.000000 torqueclient-0.4.2/torqueclient/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    14055 2023-02-19 01:57:21.000000 torqueclient-0.4.2/torqueclient/api.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6710 2023-02-19 01:57:21.000000 torqueclient-0.4.2/torqueclient/cache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       22 2023-05-15 17:34:09.000000 torqueclient-0.4.2/torqueclient/version.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-05-15 17:35:52.454375 torqueclient-0.4.2/torqueclient.egg-info/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      976 2023-05-15 17:35:52.000000 torqueclient-0.4.2/torqueclient.egg-info/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      319 2023-05-15 17:35:52.000000 torqueclient-0.4.2/torqueclient.egg-info/SOURCES.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2023-05-15 17:35:52.000000 torqueclient-0.4.2/torqueclient.egg-info/dependency_links.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       25 2023-05-15 17:35:52.000000 torqueclient-0.4.2/torqueclient.egg-info/requires.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       13 2023-05-15 17:35:52.000000 torqueclient-0.4.2/torqueclient.egg-info/top_level.txt
```

### Comparing `torqueclient-0.4.0/LICENSE` & `torqueclient-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torqueclient-0.4.0/PKG-INFO` & `torqueclient-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torqueclient
-Version: 0.4.0
+Version: 0.4.2
 Summary: Python client for mediawiki/torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `torqueclient-0.4.0/setup.py` & `torqueclient-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `torqueclient-0.4.0/torqueclient/api.py` & `torqueclient-0.4.2/torqueclient/api.py`

 * *Files identical despite different names*

### Comparing `torqueclient-0.4.0/torqueclient/cache.py` & `torqueclient-0.4.2/torqueclient/cache.py`

 * *Files identical despite different names*

### Comparing `torqueclient-0.4.0/torqueclient.egg-info/PKG-INFO` & `torqueclient-0.4.2/torqueclient.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torqueclient
-Version: 0.4.0
+Version: 0.4.2
 Summary: Python client for mediawiki/torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

