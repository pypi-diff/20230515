# Comparing `tmp/devcycle-python-server-sdk-1.1.0.tar.gz` & `tmp/devcycle-python-server-sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcycle-python-server-sdk-1.1.0.tar", last modified: Wed Jun 22 19:00:03 2022, max compression
+gzip compressed data, was "devcycle-python-server-sdk-1.1.1.tar", last modified: Mon Nov 14 13:59:18 2022, max compression
```

## Comparing `devcycle-python-server-sdk-1.1.0.tar` & `devcycle-python-server-sdk-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 emma       (501) staff       (20)        0 2022-06-22 19:00:03.571552 devcycle-python-server-sdk-1.1.0/
--rw-r--r--   0 emma       (501) staff       (20)     1071 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/LICENSE
--rw-r--r--   0 emma       (501) staff       (20)      455 2022-06-22 19:00:03.571679 devcycle-python-server-sdk-1.1.0/PKG-INFO
--rw-r--r--   0 emma       (501) staff       (20)     1412 2022-06-22 16:59:07.000000 devcycle-python-server-sdk-1.1.0/README.md
-drwxr-xr-x   0 emma       (501) staff       (20)        0 2022-06-22 19:00:03.563339 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/
--rw-r--r--   0 emma       (501) staff       (20)        5 2022-06-22 16:59:07.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/VERSION.txt
--rw-r--r--   0 emma       (501) staff       (20)     1103 2022-06-21 14:24:12.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 emma       (501) staff       (20)        0 2022-06-22 19:00:03.563944 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/api/
--rw-r--r--   0 emma       (501) staff       (20)      144 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 emma       (501) staff       (20)    18116 2022-06-22 16:59:07.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/api/dvc_client.py
--rw-r--r--   0 emma       (501) staff       (20)    24815 2022-06-15 16:43:09.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/api_client.py
--rw-r--r--   0 emma       (501) staff       (20)     8289 2022-06-22 18:59:54.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/configuration.py
--rw-r--r--   0 emma       (501) staff       (20)       97 2022-06-21 14:24:12.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/dvc_options.py
-drwxr-xr-x   0 emma       (501) staff       (20)        0 2022-06-22 19:00:03.566916 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/
--rw-r--r--   0 emma       (501) staff       (20)      833 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 emma       (501) staff       (20)     4015 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 emma       (501) staff       (20)     6173 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/event.py
--rw-r--r--   0 emma       (501) staff       (20)     8501 2022-06-17 21:06:33.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 emma       (501) staff       (20)     3137 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/inline_response201.py
--rw-r--r--   0 emma       (501) staff       (20)    15928 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/user_data.py
--rw-r--r--   0 emma       (501) staff       (20)     3801 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/user_data_and_events_body.py
--rw-r--r--   0 emma       (501) staff       (20)     6525 2022-06-07 14:11:44.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/variable.py
--rw-r--r--   0 emma       (501) staff       (20)    13219 2022-06-15 16:42:59.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/rest.py
-drwxr-xr-x   0 emma       (501) staff       (20)        0 2022-06-22 19:00:03.568508 devcycle-python-server-sdk-1.1.0/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 emma       (501) staff       (20)      455 2022-06-22 19:00:02.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 emma       (501) staff       (20)     1145 2022-06-22 19:00:03.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 emma       (501) staff       (20)        1 2022-06-22 19:00:02.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 emma       (501) staff       (20)       48 2022-06-22 19:00:03.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 emma       (501) staff       (20)       33 2022-06-22 19:00:03.000000 devcycle-python-server-sdk-1.1.0/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 emma       (501) staff       (20)        0 2022-06-22 19:00:03.568927 devcycle-python-server-sdk-1.1.0/example/
--rw-r--r--   0 emma       (501) staff       (20)        0 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/example/__init__.py
--rw-r--r--   0 emma       (501) staff       (20)     2206 2022-06-22 18:59:54.000000 devcycle-python-server-sdk-1.1.0/example/example.py
--rw-r--r--   0 emma       (501) staff       (20)       79 2022-06-22 19:00:03.572112 devcycle-python-server-sdk-1.1.0/setup.cfg
--rw-r--r--   0 emma       (501) staff       (20)     1320 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/setup.py
-drwxr-xr-x   0 emma       (501) staff       (20)        0 2022-06-22 19:00:03.571145 devcycle-python-server-sdk-1.1.0/test/
--rw-r--r--   0 emma       (501) staff       (20)        0 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/test/__init__.py
--rw-r--r--   0 emma       (501) staff       (20)     1376 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/test/test_devcycle_api.py
--rw-r--r--   0 emma       (501) staff       (20)      965 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/test/test_error_response.py
--rw-r--r--   0 emma       (501) staff       (20)      915 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/test/test_feature.py
--rw-r--r--   0 emma       (501) staff       (20)      997 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/test/test_inline_response200.py
--rw-r--r--   0 emma       (501) staff       (20)      925 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/test/test_user_data.py
--rw-r--r--   0 emma       (501) staff       (20)     1027 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/test/test_user_data_and_event_body.py
--rw-r--r--   0 emma       (501) staff       (20)      923 2022-06-06 19:02:31.000000 devcycle-python-server-sdk-1.1.0/test/test_variable.py
+drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.536111 devcycle-python-server-sdk-1.1.1/
+-rw-r--r--   0 adamwootton   (501) staff       (20)     1071 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/LICENSE
+-rw-r--r--   0 adamwootton   (501) staff       (20)      455 2022-11-14 13:59:18.536162 devcycle-python-server-sdk-1.1.1/PKG-INFO
+-rw-r--r--   0 adamwootton   (501) staff       (20)     1412 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/README.md
+drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.532458 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/
+-rw-r--r--   0 adamwootton   (501) staff       (20)        5 2022-11-14 13:59:08.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/VERSION.txt
+-rw-r--r--   0 adamwootton   (501) staff       (20)     1103 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.532802 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api/
+-rw-r--r--   0 adamwootton   (501) staff       (20)      144 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)    18116 2022-11-14 13:58:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api/dvc_client.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)    24815 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api_client.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     8288 2022-11-14 13:58:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/configuration.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)       97 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/dvc_options.py
+drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.534107 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/
+-rw-r--r--   0 adamwootton   (501) staff       (20)      833 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     4015 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     6173 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     8501 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     3137 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/inline_response201.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)    15928 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/user_data.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     3801 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/user_data_and_events_body.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     6525 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/variable.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)    13219 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/rest.py
+drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.534622 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 adamwootton   (501) staff       (20)      455 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 adamwootton   (501) staff       (20)     1145 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 adamwootton   (501) staff       (20)        1 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 adamwootton   (501) staff       (20)       48 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 adamwootton   (501) staff       (20)       33 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.534781 devcycle-python-server-sdk-1.1.1/example/
+-rw-r--r--   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/example/__init__.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     2206 2022-11-14 13:58:44.000000 devcycle-python-server-sdk-1.1.1/example/example.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)       79 2022-11-14 13:59:18.536339 devcycle-python-server-sdk-1.1.1/setup.cfg
+-rw-r--r--   0 adamwootton   (501) staff       (20)     1320 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/setup.py
+drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.535978 devcycle-python-server-sdk-1.1.1/test/
+-rw-r--r--   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/__init__.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     1376 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_devcycle_api.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)      965 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_error_response.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)      915 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_feature.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)      997 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_inline_response200.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)      925 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_user_data.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)     1027 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_user_data_and_event_body.py
+-rw-r--r--   0 adamwootton   (501) staff       (20)      923 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_variable.py
```

### Comparing `devcycle-python-server-sdk-1.1.0/LICENSE` & `devcycle-python-server-sdk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/README.md` & `devcycle-python-server-sdk-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/__init__.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/api/dvc_client.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api/dvc_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/api_client.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/configuration.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
         # Default Base url
-        self.host = "https://bucketing-api.devcycle.com/"
+        self.host = "https://bucketing-api.devcycle.com"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
```

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/__init__.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/error_response.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/error_response.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/feature.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/inline_response201.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/inline_response201.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/user_data.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/user_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/user_data_and_events_body.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/user_data_and_events_body.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_sdk/rest.py` & `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/example/example.py` & `devcycle-python-server-sdk-1.1.1/example/example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/setup.py` & `devcycle-python-server-sdk-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/test/test_devcycle_api.py` & `devcycle-python-server-sdk-1.1.1/test/test_devcycle_api.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/test/test_error_response.py` & `devcycle-python-server-sdk-1.1.1/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/test/test_feature.py` & `devcycle-python-server-sdk-1.1.1/test/test_feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/test/test_inline_response200.py` & `devcycle-python-server-sdk-1.1.1/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/test/test_user_data.py` & `devcycle-python-server-sdk-1.1.1/test/test_user_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/test/test_user_data_and_event_body.py` & `devcycle-python-server-sdk-1.1.1/test/test_user_data_and_event_body.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.0/test/test_variable.py` & `devcycle-python-server-sdk-1.1.1/test/test_variable.py`

 * *Files identical despite different names*

