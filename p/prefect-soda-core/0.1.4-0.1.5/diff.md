# Comparing `tmp/prefect-soda-core-0.1.4.tar.gz` & `tmp/prefect-soda-core-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-soda-core/prefect-soda-core/dist/.tmp-w2pkzorz/prefect-soda-core-0.1.4.tar", last modified: Sun May 14 19:14:24 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-soda-core/prefect-soda-core/dist/.tmp-nki02jkc/prefect-soda-core-0.1.5.tar", last modified: Sun May 14 19:35:58 2023, max compression
```

## Comparing `prefect-soda-core-0.1.4.tar` & `prefect-soda-core-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/soda_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/sodacl_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/tests/test_soda_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/tests/test_sodacl_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/prefect_soda_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/prefect_soda_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/prefect_soda_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/prefect_soda_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/prefect_soda_core/soda_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/prefect_soda_core/sodacl_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/prefect_soda_core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/prefect_soda_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/prefect_soda_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/prefect_soda_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/prefect_soda_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/prefect_soda_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/prefect_soda_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:35:58.000000 prefect-soda-core-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/tests/test_soda_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/tests/test_sodacl_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-14 19:34:25.000000 prefect-soda-core-0.1.5/versioneer.py
```

### Comparing `prefect-soda-core-0.1.4/LICENSE` & `prefect-soda-core-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/PKG-INFO` & `prefect-soda-core-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-soda-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: Prefect 2.0 collection for Soda Core
 Home-page: https://github.com/sodadata/prefect-soda-core
 Author: Soda Data NV.
 Author-email: vijay@soda.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -15,24 +15,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: bigquery
 Provides-Extra: redshift
-Provides-Extra: db2
-Provides-Extra: sqlserver
 Provides-Extra: athena
-Provides-Extra: spark-df
+Provides-Extra: trino
+Provides-Extra: sqlserver
 Provides-Extra: snowflake
-Provides-Extra: mysql
+Provides-Extra: spark-df
 Provides-Extra: postgres
-Provides-Extra: trino
-Provides-Extra: bigquery
+Provides-Extra: mysql
+Provides-Extra: db2
 Provides-Extra: dev
 License-File: LICENSE
 
 # prefect-soda-core
 
 ## Welcome!
```

### Comparing `prefect-soda-core-0.1.4/README.md` & `prefect-soda-core-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/prefect_soda_core/soda_configuration.py` & `prefect-soda-core-0.1.5/prefect_soda_core/soda_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     configuration_yaml_path: str
     configuration_yaml_str: Optional[str]
 
     _block_type_name: Optional[str] = "Soda Configuration"
     _logo_url: Optional[
         HttpUrl
-    ] = "https://github.com/PrefectHQ/prefect/blob/main/docs/img/collections/soda.png"  # noqa
+    ] = "https://raw.githubusercontent.com/PrefectHQ/prefect/main/docs/img/collections/soda.png"  # noqa
 
     @root_validator(pre=True)
     def check_block_configuration(cls, values):
         """
         Ensure that the configuration options are valid.
         A configuration is valid if it provides just the path to the
         YAML configuration file or if it has both the path
```

### Comparing `prefect-soda-core-0.1.4/prefect_soda_core/sodacl_check.py` & `prefect-soda-core-0.1.5/prefect_soda_core/sodacl_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     sodacl_yaml_path: str
     sodacl_yaml_str: Optional[str]
 
     _block_type_name: Optional[str] = "SodaCL Check"
     _logo_url: Optional[
         HttpUrl
-    ] = "https://github.com/PrefectHQ/prefect/blob/main/docs/img/collections/soda.png"  # noqa
+    ] = "https://raw.githubusercontent.com/PrefectHQ/prefect/main/docs/img/collections/soda.png"  # noqa
 
     @root_validator(pre=True)
     def check_block_configuration(cls, values):
         """
         Ensure that the check configuration options are valid.
         A check configuration is valid if it provides just the path to the
         YAML Soda checks file or if it has both the path
```

### Comparing `prefect-soda-core-0.1.4/prefect_soda_core/tasks.py` & `prefect-soda-core-0.1.5/prefect_soda_core/tasks.py`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/prefect_soda_core.egg-info/PKG-INFO` & `prefect-soda-core-0.1.5/prefect_soda_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-soda-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: Prefect 2.0 collection for Soda Core
 Home-page: https://github.com/sodadata/prefect-soda-core
 Author: Soda Data NV.
 Author-email: vijay@soda.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -15,24 +15,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: bigquery
 Provides-Extra: redshift
-Provides-Extra: db2
-Provides-Extra: sqlserver
 Provides-Extra: athena
-Provides-Extra: spark-df
+Provides-Extra: trino
+Provides-Extra: sqlserver
 Provides-Extra: snowflake
-Provides-Extra: mysql
+Provides-Extra: spark-df
 Provides-Extra: postgres
-Provides-Extra: trino
-Provides-Extra: bigquery
+Provides-Extra: mysql
+Provides-Extra: db2
 Provides-Extra: dev
 License-File: LICENSE
 
 # prefect-soda-core
 
 ## Welcome!
```

### Comparing `prefect-soda-core-0.1.4/prefect_soda_core.egg-info/SOURCES.txt` & `prefect-soda-core-0.1.5/prefect_soda_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/prefect_soda_core.egg-info/requires.txt` & `prefect-soda-core-0.1.5/prefect_soda_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/setup.cfg` & `prefect-soda-core-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/setup.py` & `prefect-soda-core-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/tests/test_soda_configuration.py` & `prefect-soda-core-0.1.5/tests/test_soda_configuration.py`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/tests/test_sodacl_check.py` & `prefect-soda-core-0.1.5/tests/test_sodacl_check.py`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/tests/test_tasks.py` & `prefect-soda-core-0.1.5/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.4/versioneer.py` & `prefect-soda-core-0.1.5/versioneer.py`

 * *Files identical despite different names*

