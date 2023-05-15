# Comparing `tmp/apache-airflow-providers-sktvane-0.0.9.tar.gz` & `tmp/apache-airflow-providers-sktvane-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.0.9.tar", last modified: Thu Mar  9 02:26:42 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-0.1.0.tar", last modified: Mon May 15 08:28:13 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.0.9.tar` & `apache-airflow-providers-sktvane-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.943633 apache-airflow-providers-sktvane-0.0.9/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.943633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.943633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-09 02:26:42.000000 apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-09 02:26:42.947633 apache-airflow-providers-sktvane-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-09 02:26:39.000000 apache-airflow-providers-sktvane-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.969227 apache-airflow-providers-sktvane-0.1.0/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.969227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.969227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 08:28:13.977227 apache-airflow-providers-sktvane-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.0.9/PKG-INFO` & `apache-airflow-providers-sktvane-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.0.9
+Version: 0.1.0
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
-Home-page: UNKNOWN
-Author: lapetus
-Author-email: lapetus@sktai.io
+Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
+Author: aidp
+Author-email: aidp@sktai.io
 License: MIT
-Project-URL: Homepage, https://github.com/sktaiflow/apache-airflow-providers-sktvane
-Project-URL: Source Code, https://github.com/sktaiflow/apache-airflow-providers-sktvane
+Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # apache-airflow-providers-sktvane
 
 ###
 
 ```shell
```

### Comparing `apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/gcp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 
 from google.cloud import bigquery
 from google.oauth2 import service_account
-from sktvane.providers.vault.macros.vault import get_secrets
+
+from ..macros.vault import get_secrets
 
 
 def _get_credentials():
     key = get_secrets("gcp/skt-datahub/dataflow")["config"]
     json_acct_info = json.loads(key)
     credentials = service_account.Credentials.from_service_account_info(json_acct_info)
     scoped_credentials = credentials.with_scopes(
```

### Comparing `apache-airflow-providers-sktvane-0.0.9/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/sensors/gcp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from airflow.sensors.base import BaseSensorOperator
-from sktvane.providers.gcp.macros.gcp import bigquery_client
+
+from ..macros.gcp import bigquery_client
 
 
 class BigqueryPartitionSensor(BaseSensorOperator):
-    template_fields = ("project_id", "dataset_id", "table_id", "partition")
+    template_fields = ("dataset_id", "table_id", "partition")
 
     def __init__(
         self,
-        project_id,
         dataset_id,
         table_id,
         partition,
         timeout=(60 * 60) * 24 * 2,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
-        self.project_id = project_id
+        self.project_id = "skt-datahub"
         self.dataset_id = dataset_id
         self.table_id = table_id
         self.partition = partition
         self.mode = "reschedule"
         self.poke_interval = 300  # 5 min
         self.timeout = timeout
```

### Comparing `apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/PKG-INFO` & `apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.0.9
+Version: 0.1.0
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
-Home-page: UNKNOWN
-Author: lapetus
-Author-email: lapetus@sktai.io
+Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
+Author: aidp
+Author-email: aidp@sktai.io
 License: MIT
-Project-URL: Homepage, https://github.com/sktaiflow/apache-airflow-providers-sktvane
-Project-URL: Source Code, https://github.com/sktaiflow/apache-airflow-providers-sktvane
+Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # apache-airflow-providers-sktvane
 
 ###
 
 ```shell
```

### Comparing `apache-airflow-providers-sktvane-0.0.9/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 README.md
 setup.cfg
 setup.py
 airflow/providers/sktvane/__init__.py
 airflow/providers/sktvane/macros/__init__.py
+airflow/providers/sktvane/macros/date.py
 airflow/providers/sktvane/macros/gcp.py
+airflow/providers/sktvane/macros/slack.py
 airflow/providers/sktvane/macros/vault.py
 airflow/providers/sktvane/operators/__init__.py
 airflow/providers/sktvane/operators/nes.py
 airflow/providers/sktvane/sensors/__init__.py
 airflow/providers/sktvane/sensors/gcp.py
+airflow/providers/sktvane/tests/__init__.py
+airflow/providers/sktvane/tests/test.py
 apache_airflow_providers_sktvane.egg-info/PKG-INFO
 apache_airflow_providers_sktvane.egg-info/SOURCES.txt
 apache_airflow_providers_sktvane.egg-info/dependency_links.txt
 apache_airflow_providers_sktvane.egg-info/requires.txt
 apache_airflow_providers_sktvane.egg-info/top_level.txt
```

