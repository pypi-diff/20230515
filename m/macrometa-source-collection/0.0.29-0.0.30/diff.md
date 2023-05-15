# Comparing `tmp/macrometa-source-collection-0.0.29.tar.gz` & `tmp/macrometa-source-collection-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.29.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.30.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.29.tar` & `macrometa-source-collection-0.0.30.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8346 2023-05-15 07:28:54.788062 macrometa-source-collection-0.0.29/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     8411 2023-05-15 07:28:54.788062 macrometa-source-collection-0.0.29/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-05-15 07:28:55.032064 macrometa-source-collection-0.0.29/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.29/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.29/PKG-INFO
+-rw-r--r--   0        0        0     8346 2023-05-15 08:26:35.052074 macrometa-source-collection-0.0.30/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     8499 2023-05-15 08:26:35.052074 macrometa-source-collection-0.0.30/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-05-15 08:26:35.312074 macrometa-source-collection-0.0.30/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.30/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.30/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.29/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.30/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.29/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.30/macrometa_source_collection/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 LOGGER = singer.get_logger('macrometa_source_collection')
 
 region_label = os.getenv("GDN_FEDERATION", "NA")
 tenant_label = os.getenv("GDN_TENANT", "NA")
 fabric_label = os.getenv("GDN_FABRIC", "NA")
 workflow_label = os.getenv("WORKFLOW_UUID", "NA")
 metric_service_url = os.getenv("METRIC_SERVICE_API")
-is_metrics_enabled = os.getenv("MACROMETA_SOURCE_COLLECTION_IS_METRICS_ENABLED", False)
+is_metrics_enabled = os.getenv("MACROMETA_SOURCE_COLLECTION_IS_METRICS_ENABLED", 'False')
 
 class GDNCollectionClient:
     """Client for handling GDN collection streams."""
 
     def __init__(self, config) -> None:
         """Init new GDN Collection Client."""
         self._host = config.get("region")
@@ -46,16 +46,17 @@
         self._c8_client.update_collection_properties(self._collection, has_stream=True)
 
         self.exported_bytes = Counter("exported_bytes", "Total number of bytes exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
         self.exported_documents = Counter("exported_documents", "Total number of documents exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
         self.export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
         self.export_lag = Histogram("export_lag", "The average time from when the data changes in GDN collections are reflected in external data sources", ['region', 'tenant', 'fabric', 'workflow'])
         
-        # Start the Prometheus HTTP server for exposing metri
-        if is_metrics_enabled:
+        # Start the Prometheus HTTP server for exposing metrics
+        if is_metrics_enabled.lower() == 'true':
+            LOGGER.info("Source is starting the metrics server.")
             start_http_server(8000)
 
     def sync(self, stream):
         """Return documents in target GDN collection as records."""
         if self._c8_client.has_collection(self._collection):
             self.send_schema_message(stream)
             columns = list(stream.schema.properties.keys())
```

### Comparing `macrometa-source-collection-0.0.29/pyproject.toml` & `macrometa-source-collection-0.0.30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.29'
+version='0.0.30'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.29/setup.py` & `macrometa-source-collection-0.0.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.29',
+    'version': '0.0.30',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.29/PKG-INFO` & `macrometa-source-collection-0.0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.29
+Version: 0.0.30
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

