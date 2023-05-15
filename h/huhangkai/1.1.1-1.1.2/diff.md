# Comparing `tmp/huhangkai-1.1.1.tar.gz` & `tmp/huhangkai-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.1.1.tar", last modified: Mon May  8 07:22:44 2023, max compression
+gzip compressed data, was "huhangkai-1.1.2.tar", last modified: Mon May 15 01:36:51 2023, max compression
```

## Comparing `huhangkai-1.1.1.tar` & `huhangkai-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:22:44.585038 huhangkai-1.1.1/
--rw-rw-rw-   0        0        0      228 2023-05-08 07:22:44.584042 huhangkai-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 07:22:44.570076 huhangkai-1.1.1/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.1/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-04-23 09:30:51.000000 huhangkai-1.1.1/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-04-23 09:30:51.000000 huhangkai-1.1.1/commen/unit_dict.py
--rw-rw-rw-   0        0        0    20401 2023-05-08 07:22:18.000000 huhangkai-1.1.1/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-04-23 09:30:51.000000 huhangkai-1.1.1/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-04-23 09:30:51.000000 huhangkai-1.1.1/commen/unit_request.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:22:44.582047 huhangkai-1.1.1/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-05-08 07:22:44.000000 huhangkai-1.1.1/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-05-08 07:22:44.000000 huhangkai-1.1.1/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:22:44.000000 huhangkai-1.1.1/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-08 07:22:44.000000 huhangkai-1.1.1/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 07:22:44.000000 huhangkai-1.1.1/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 07:22:44.586038 huhangkai-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-05-08 07:22:40.000000 huhangkai-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:36:51.946654 huhangkai-1.1.2/
+-rw-rw-rw-   0        0        0      228 2023-05-15 01:36:51.945656 huhangkai-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-15 01:36:51.929700 huhangkai-1.1.2/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.2/commen/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-05-08 06:03:41.000000 huhangkai-1.1.2/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-08 06:03:41.000000 huhangkai-1.1.2/commen/unit_dict.py
+-rw-rw-rw-   0        0        0    20401 2023-05-08 07:11:26.000000 huhangkai-1.1.2/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-08 06:03:41.000000 huhangkai-1.1.2/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     6122 2023-05-08 06:03:41.000000 huhangkai-1.1.2/commen/unit_request.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:36:51.943663 huhangkai-1.1.2/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-05-15 01:36:51.000000 huhangkai-1.1.2/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-05-15 01:36:51.000000 huhangkai-1.1.2/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 01:36:51.000000 huhangkai-1.1.2/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-15 01:36:51.000000 huhangkai-1.1.2/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 01:36:51.000000 huhangkai-1.1.2/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 01:36:51.946654 huhangkai-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-05-15 01:36:43.000000 huhangkai-1.1.2/setup.py
```

### Comparing `huhangkai-1.1.1/commen/__init__.py` & `huhangkai-1.1.2/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.1/commen/init_project.py` & `huhangkai-1.1.2/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.1/commen/unit_dict.py` & `huhangkai-1.1.2/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.1/commen/unit_fun.py` & `huhangkai-1.1.2/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.1/commen/unit_logger.py` & `huhangkai-1.1.2/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.1/commen/unit_request.py` & `huhangkai-1.1.2/commen/unit_request.py`

 * *Files identical despite different names*

