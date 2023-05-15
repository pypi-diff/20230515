# Comparing `tmp/prophecy-libs-1.5.0.tar.gz` & `tmp/prophecy-libs-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.5.0.tar", last modified: Wed Apr 19 07:55:26 2023, max compression
+gzip compressed data, was "prophecy-libs-1.5.1.tar", last modified: Mon May 15 15:31:21 2023, max compression
```

## Comparing `prophecy-libs-1.5.0.tar` & `prophecy-libs-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:26.001192 prophecy-libs-1.5.0/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-04-19 07:55:26.001192 prophecy-libs-1.5.0/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:25.997192 prophecy-libs-1.5.0/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:25.997192 prophecy-libs-1.5.0/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2858 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:25.997192 prophecy-libs-1.5.0/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      619 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:25.997192 prophecy-libs-1.5.0/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:25.997192 prophecy-libs-1.5.0/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:25.997192 prophecy-libs-1.5.0/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      638 2023-04-12 12:00:52.000000 prophecy-libs-1.5.0/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.0/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:25.997192 prophecy-libs-1.5.0/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      985 2023-03-12 14:51:36.000000 prophecy-libs-1.5.0/prophecy/udfs/scala_udf_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     8981 2023-04-12 12:00:52.000000 prophecy-libs-1.5.0/prophecy/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:55:26.001192 prophecy-libs-1.5.0/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-04-19 07:55:25.000000 prophecy-libs-1.5.0/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)      773 2023-04-19 07:55:25.000000 prophecy-libs-1.5.0/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-04-19 07:55:25.000000 prophecy-libs-1.5.0/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.0/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-04-19 07:55:25.000000 prophecy-libs-1.5.0/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-04-19 07:55:25.000000 prophecy-libs-1.5.0/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-04-19 07:55:26.001192 prophecy-libs-1.5.0/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-04-19 07:55:24.000000 prophecy-libs-1.5.0/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.947171 prophecy-libs-1.5.1/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-15 15:31:21.947171 prophecy-libs-1.5.1/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.943171 prophecy-libs-1.5.1/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.943171 prophecy-libs-1.5.1/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2858 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.943171 prophecy-libs-1.5.1/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      619 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.947171 prophecy-libs-1.5.1/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.947171 prophecy-libs-1.5.1/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.947171 prophecy-libs-1.5.1/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.1/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.1/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.947171 prophecy-libs-1.5.1/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      985 2023-03-12 14:51:36.000000 prophecy-libs-1.5.1/prophecy/udfs/scala_udf_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     8981 2023-04-12 12:00:52.000000 prophecy-libs-1.5.1/prophecy/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-15 15:31:21.947171 prophecy-libs-1.5.1/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-15 15:31:21.000000 prophecy-libs-1.5.1/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      773 2023-05-15 15:31:21.000000 prophecy-libs-1.5.1/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-05-15 15:31:21.000000 prophecy-libs-1.5.1/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.1/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-05-15 15:31:21.000000 prophecy-libs-1.5.1/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-05-15 15:31:21.000000 prophecy-libs-1.5.1/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-05-15 15:31:21.947171 prophecy-libs-1.5.1/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-05-15 15:31:20.000000 prophecy-libs-1.5.1/setup.py
```

### Comparing `prophecy-libs-1.5.0/prophecy/config/config_base.py` & `prophecy-libs-1.5.1/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/config/utils.py` & `prophecy-libs-1.5.1/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/libs/utils.py` & `prophecy-libs-1.5.1/prophecy/libs/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.5.1/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/random_data_creator.py` & `prophecy-libs-1.5.1/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.5.1/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/test/utils.py` & `prophecy-libs-1.5.1/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.5.1/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.5.1/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy/utils.py` & `prophecy-libs-1.5.1/prophecy/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.0/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.5.1/prophecy_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

