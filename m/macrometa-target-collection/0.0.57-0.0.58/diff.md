# Comparing `tmp/macrometa-target-collection-0.0.57.tar.gz` & `tmp/macrometa-target-collection-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.57.tar", last modified: Fri Apr 21 12:20:09 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.58.tar", last modified: Mon May 15 07:29:00 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.57.tar` & `macrometa-target-collection-0.0.58.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:20:09.655585 macrometa-target-collection-0.0.57/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-21 12:20:09.655585 macrometa-target-collection-0.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:20:09.651584 macrometa-target-collection-0.0.57/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13919 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:20:09.655585 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 12:20:09.000000 macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-21 12:19:45.000000 macrometa-target-collection-0.0.57/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 12:20:09.655585 macrometa-target-collection-0.0.57/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:00.201777 macrometa-target-collection-0.0.58/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-15 07:28:35.000000 macrometa-target-collection-0.0.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-15 07:29:00.201777 macrometa-target-collection-0.0.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-15 07:28:35.000000 macrometa-target-collection-0.0.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:00.201777 macrometa-target-collection-0.0.58/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-15 07:28:35.000000 macrometa-target-collection-0.0.58/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14034 2023-05-15 07:28:35.000000 macrometa-target-collection-0.0.58/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:00.201777 macrometa-target-collection-0.0.58/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-15 07:29:00.000000 macrometa-target-collection-0.0.58/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 07:29:00.000000 macrometa-target-collection-0.0.58/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:29:00.000000 macrometa-target-collection-0.0.58/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 07:29:00.000000 macrometa-target-collection-0.0.58/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 07:29:00.000000 macrometa-target-collection-0.0.58/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 07:29:00.000000 macrometa-target-collection-0.0.58/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-15 07:28:35.000000 macrometa-target-collection-0.0.58/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 07:29:00.201777 macrometa-target-collection-0.0.58/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.57/LICENSE` & `macrometa-target-collection-0.0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.57/PKG-INFO` & `macrometa-target-collection-0.0.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.57
+Version: 0.0.58
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.57/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.58/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.57/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.58/macrometa_target_collection/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,19 @@
 scrape_complete_flag = Counter("scrape_complete_flag", "Flag to check if the last scrape has been completed", ['workflow'])
 
 region_label = os.getenv("GDN_FEDERATION", "NA")
 tenant_label = os.getenv("GDN_TENANT", "NA")
 fabric_label = os.getenv("GDN_FABRIC", "NA")
 workflow_label = os.getenv("WORKFLOW_UUID", "NA")
 metric_service_url = os.getenv("METRIC_SERVICE_API")
+is_metrics_enabled = os.getenv("MACROMETA_TARGET_COLLECTION_IS_METRICS_ENABLED", False)
 
 # Start the Prometheus HTTP server for exposing metrics
-start_http_server(8000)
+if is_metrics_enabled:
+    start_http_server(8000)
 
 class RecordBatch:
     """Class wrapping the record batch in order to make it thread safe."""
 
     def __init__(self, config: dict):
         self._list = list()
         self._lock = Lock()
```

### Comparing `macrometa-target-collection-0.0.57/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.58/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.57
+Version: 0.0.58
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.57/pyproject.toml` & `macrometa-target-collection-0.0.58/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.57"
+version = "0.0.58"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

