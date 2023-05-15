# Comparing `tmp/thoughtspot_rest_api_v1-1.4.1.tar.gz` & `tmp/thoughtspot_rest_api_v1-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtspot_rest_api_v1-1.4.1.tar", last modified: Thu Mar 23 14:49:31 2023, max compression
+gzip compressed data, was "thoughtspot_rest_api_v1-1.5.0.tar", last modified: Mon May 15 15:24:49 2023, max compression
```

## Comparing `thoughtspot_rest_api_v1-1.4.1.tar` & `thoughtspot_rest_api_v1-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-03-23 14:49:31.338209 thoughtspot_rest_api_v1-1.4.1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.4.1/LICENSE
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-03-23 14:49:31.338297 thoughtspot_rest_api_v1-1.4.1/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365    28536 2023-03-17 18:28:57.000000 thoughtspot_rest_api_v1-1.4.1/README.md
--rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.4.1/pyproject.toml
--rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2023-03-23 14:49:31.338640 thoughtspot_rest_api_v1-1.4.1/setup.cfg
--rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.4.1/setup.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-03-23 14:49:31.333860 thoughtspot_rest_api_v1-1.4.1/src/
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-03-23 14:49:31.337062 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/__init__.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-03-17 18:44:02.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/_version.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/details_objects.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    74795 2023-03-15 16:11:57.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    21142 2023-03-17 18:42:45.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-03-23 14:49:31.338081 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1.egg-info/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-03-23 14:49:31.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2023-03-23 14:49:31.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2023-03-23 14:49:31.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-03-23 14:49:31.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1.egg-info/requires.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2023-03-23 14:49:31.000000 thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-15 15:24:49.005890 thoughtspot_rest_api_v1-1.5.0/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.5.0/LICENSE
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-05-15 15:24:49.005969 thoughtspot_rest_api_v1-1.5.0/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28536 2023-03-17 18:28:57.000000 thoughtspot_rest_api_v1-1.5.0/README.md
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.0/pyproject.toml
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2023-05-15 15:24:49.006297 thoughtspot_rest_api_v1-1.5.0/setup.cfg
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.0/setup.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-15 15:24:49.001789 thoughtspot_rest_api_v1-1.5.0/src/
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-15 15:24:49.004596 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/__init__.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-05-15 15:24:30.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/_version.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/details_objects.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    75771 2023-05-15 15:24:30.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/tsrestapiv1.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    21142 2023-03-17 18:42:45.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/tsrestapiv2.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-15 15:24:49.005761 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/requires.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
```

### Comparing `thoughtspot_rest_api_v1-1.4.1/LICENSE` & `thoughtspot_rest_api_v1-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.4.1/PKG-INFO` & `thoughtspot_rest_api_v1-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_rest_api_v1
-Version: 1.4.1
+Version: 1.5.0
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
```

### Comparing `thoughtspot_rest_api_v1-1.4.1/README.md` & `thoughtspot_rest_api_v1-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.4.1/setup.cfg` & `thoughtspot_rest_api_v1-1.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = thoughtspot_rest_api_v1
-version = 1.4.1
+version = 1.5.0
 description = Library implementing the ThoughtSpot V1 REST API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 author = Bryant Howell
 author_email = bryant.howell@thoughtspot.com
 license = MIT
```

### Comparing `thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/details_objects.py` & `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/details_objects.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py` & `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/tsrestapiv1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1383,16 +1383,17 @@
             post_params['autocreate'] = str(auto_create_user).lower()
 
         if groups is not None:
             post_params['groups'] = json.dumps(groups)
 
         url = self.base_url + endpoint
 
-        response = self.requests_session.post(url=url, data=post_params)
-        return response
+        response = self.requests_session.post(url=url, data=post_params, headers={"Accept": "text/plain"})
+        response.raise_for_status()
+        return response.content.decode()
 
     # session/login/token is typically only used within the browser and handled by the Visual Embed SDK,
     # provided here for testing
     def session_login_token_post(self, username: str, auth_token: str, redirect_url: str):
         endpoint = 'session/login/token'
 
         post_params = {
@@ -1401,14 +1402,15 @@
              'redirect_url': redirect_url,  # need to url encode
 
         }
 
         url = self.base_url + endpoint
 
         response = self.requests_session.post(url=url, data=post_params)
+        response.raise_for_status()
         return response
     #
     # USER Methods
     #
 
     def user_get(self, user_id: Optional[str] = None, name: Optional[str] = None) -> Union[Dict, List]:
         endpoint = 'user/'
@@ -1824,45 +1826,61 @@
         if tagname is not None:
             url_params['tagname'] = json.dumps(tagname)
 
         response = self.requests_session.get(url=url, params=url_params)
         response.raise_for_status()
         return response.json()
 
-    def connection_fetch_connection(self, connection_guid, config_json_string, include_columns=False, authentication_type='SERVICE_ACCOUNT'):
+    def connection_fetch_connection(self, connection_guid: str, include_columns=False,
+                                    authentication_type='SERVICE_ACCOUNT', config_json_string: Optional[str] = None,
+                                    use_internal_endpoint=False):
         endpoint = 'connection/fetchConnection'
 
-        url = self.non_public_base_url + endpoint
+        if use_internal_endpoint is True:
+            url = self.non_public_base_url + endpoint
+            if config_json_string is None:
+                raise Exception('The config_json_string (a JSON object converted to string using json.dumps() ) is required')
+        else:
+            url = self.base_url + endpoint
+
         # Example of a config_json, which may vary per connection
         #
         # config_json_string_example = '''
         #       {  "password": "",
         #          "role": "SE_ROLE",
         #          "warehouse": "SE_DEMO_WH",
         #          "accountName": "thoughtspot_partner",
         #          "user": "se_demo"
         #       }
         # '''
         #
         post_data = {'id': connection_guid,
-                     'config': config_json_string,
                      'includeColumns': str(include_columns).lower(),
                      'authentication_type': authentication_type
                      }
 
+        if config_json_string is not None:
+            post_data['config'] = config_json_string
+
         response = self.requests_session.post(url=url, data=post_data)
         response.raise_for_status()
         return response.json()
 
-    def connection_fetch_live_columns(self, connection_guid, config_json_string, database_name: str,
+    def connection_fetch_live_columns(self, connection_guid, database_name: str,
                                       schema_name: str, table_name: str,
-                                      authentication_type='SERVICE_ACCOUNT'):
+                                      authentication_type='SERVICE_ACCOUNT', config_json_string: Optional[str] = None,
+                                      use_internal_endpoint=False):
         endpoint = 'connection/fetchLiveColumns'
 
-        url = self.non_public_base_url + endpoint
+        if use_internal_endpoint is True:
+            url = self.non_public_base_url + endpoint
+            if config_json_string is None:
+                raise Exception('The config_json_string (a JSON object converted to string using json.dumps() ) is required')
+        else:
+            url = self.base_url + endpoint
         tables = [{"databaseName": database_name,
                   "schemaName": schema_name,
                   "tableName": table_name
                   }]
         # Example of a config_json, which may vary per connection
         #
         # config_json_string_example = '''
@@ -1871,18 +1889,19 @@
         #          "warehouse": "SE_DEMO_WH",
         #          "accountName": "thoughtspot_partner",
         #          "user": "se_demo"
         #       }
         # '''
         #
         post_data = {'connection_id': connection_guid,
-                     'config': config_json_string,
                      'tables': json.dumps(tables),
                      'authentication_type': authentication_type
                      }
+        if config_json_string is not None:
+            post_data['config'] = config_json_string
 
         response = self.requests_session.post(url=url, data=post_data)
         response.raise_for_status()
         return response.json()
 
     #
     # connection processing to generate create / update input
```

### Comparing `thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py` & `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/tsrestapiv2.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO` & `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot-rest-api-v1
-Version: 1.4.1
+Version: 1.5.0
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
```

### Comparing `thoughtspot_rest_api_v1-1.4.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt` & `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

