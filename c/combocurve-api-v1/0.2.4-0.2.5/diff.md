# Comparing `tmp/combocurve-api-v1-0.2.4.tar.gz` & `tmp/combocurve-api-v1-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/combocurve-client-python/combocurve-client-python/dist/tmpal54yy9c/combocurve-api-v1-0.2.4.tar", last modified: Thu Apr 14 21:27:29 2022, max compression
+gzip compressed data, was "combocurve-api-v1-0.2.5.tar", last modified: Mon May 15 18:50:04 2023, max compression
```

## Comparing `combocurve-api-v1-0.2.4.tar` & `combocurve-api-v1-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3251 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/combocurve_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/service_account.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/token_refresher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/pagination/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-04-14 21:26:56.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1/pagination/link.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-04-14 21:27:28.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-14 21:27:28.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-04-14 21:27:28.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-14 21:27:29.000000 combocurve-api-v1-0.2.4/src/combocurve_api_v1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:50:04.764745 combocurve-api-v1-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-15 18:50:04.764745 combocurve-api-v1-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-15 18:50:04.764745 combocurve-api-v1-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:50:04.760745 combocurve-api-v1-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:50:04.764745 combocurve-api-v1-0.2.5/src/combocurve_api_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:50:04.764745 combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/combocurve_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/token_refresher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:50:04.764745 combocurve-api-v1-0.2.5/src/combocurve_api_v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 18:49:22.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1/pagination/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:50:04.764745 combocurve-api-v1-0.2.5/src/combocurve_api_v1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-15 18:50:04.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 18:50:04.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:50:04.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-15 18:50:04.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 18:50:04.000000 combocurve-api-v1-0.2.5/src/combocurve_api_v1.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `combocurve-api-v1-0.2.4/PKG-INFO` & `combocurve-api-v1-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 Metadata-Version: 2.1
 Name: combocurve-api-v1
-Version: 0.2.4
+Version: 0.2.5
 Summary: Client library for the ComboCurve REST API
 Author: ComboCurve Inc
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
 
 # ComboCurve client for Python
 
 ## Authorization
 
 `combocurve_api` requires the API key and service account provided by ComboCurve, as shown in the example below:
@@ -105,9 +97,7 @@
     response = requests.get(url, headers=headers)
 
     # Process response
 
     url = get_next_page_url(response.headers)
     has_more = url is not None
 ```
-
-
```

### Comparing `combocurve-api-v1-0.2.4/README.md` & `combocurve-api-v1-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/combocurve_auth.py` & `combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/combocurve_auth.py`

 * *Files identical despite different names*

### Comparing `combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/jwt_handler.py` & `combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/jwt_handler.py`

 * *Files identical despite different names*

### Comparing `combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/service_account.py` & `combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/service_account.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
-
 from dataclasses import dataclass, fields
 
 
 @dataclass
 class ServiceAccount:
     client_email: str
     client_id: str
     private_key: str
     private_key_id: str
 
     @staticmethod
     def from_file(path: str) -> 'ServiceAccount':
+
         def filter_fields(d: dict):
             field_names = {f.name for f in fields(ServiceAccount)}
             return {k: d[k] for k in d if k in field_names}
 
         with open(path, 'r') as f:
             return json.load(f, object_hook=lambda d: ServiceAccount(**filter_fields(d)))
```

### Comparing `combocurve-api-v1-0.2.4/src/combocurve_api_v1/auth/token_refresher.py` & `combocurve-api-v1-0.2.5/src/combocurve_api_v1/auth/token_refresher.py`

 * *Files identical despite different names*

### Comparing `combocurve-api-v1-0.2.4/src/combocurve_api_v1.egg-info/PKG-INFO` & `combocurve-api-v1-0.2.5/src/combocurve_api_v1.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 Metadata-Version: 2.1
 Name: combocurve-api-v1
-Version: 0.2.4
+Version: 0.2.5
 Summary: Client library for the ComboCurve REST API
 Author: ComboCurve Inc
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
 
 # ComboCurve client for Python
 
 ## Authorization
 
 `combocurve_api` requires the API key and service account provided by ComboCurve, as shown in the example below:
@@ -105,9 +97,7 @@
     response = requests.get(url, headers=headers)
 
     # Process response
 
     url = get_next_page_url(response.headers)
     has_more = url is not None
 ```
-
-
```

### Comparing `combocurve-api-v1-0.2.4/src/combocurve_api_v1.egg-info/SOURCES.txt` & `combocurve-api-v1-0.2.5/src/combocurve_api_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

