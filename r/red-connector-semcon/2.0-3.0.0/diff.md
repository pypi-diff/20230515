# Comparing `tmp/red-connector-semcon-2.0.tar.gz` & `tmp/red-connector-semcon-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red-connector-semcon-2.0.tar", max compression
+gzip compressed data, was "red-connector-semcon-3.0.0.tar", max compression
```

## Comparing `red-connector-semcon-2.0.tar` & `red-connector-semcon-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    34523 2022-09-23 09:23:49.004721 red-connector-semcon-2.0/LICENSE
--rw-r--r--   0        0        0      992 2022-09-30 07:20:44.335126 red-connector-semcon-2.0/README.md
--rw-r--r--   0        0        0      628 2023-02-24 09:08:14.829210 red-connector-semcon-2.0/pyproject.toml
--rw-r--r--   0        0        0       72 2022-09-23 09:25:43.448365 red-connector-semcon-2.0/red_connector_semcon/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 09:25:11.828283 red-connector-semcon-2.0/red_connector_semcon/commons/__init__.py
--rw-r--r--   0        0        0      809 2022-09-23 09:25:11.828283 red-connector-semcon-2.0/red_connector_semcon/commons/cli_modes.py
--rw-r--r--   0        0        0     4187 2023-02-23 13:13:44.999588 red-connector-semcon-2.0/red_connector_semcon/commons/helpers.py
--rw-r--r--   0        0        0      992 2023-02-23 12:25:41.927265 red-connector-semcon-2.0/red_connector_semcon/commons/schemas.py
--rw-r--r--   0        0        0        0 2022-09-23 09:25:11.828283 red-connector-semcon-2.0/red_connector_semcon/semcon/__init__.py
--rw-r--r--   0        0        0       89 2022-09-23 09:38:18.476480 red-connector-semcon-2.0/red_connector_semcon/semcon/__main__.py
--rw-r--r--   0        0        0     1261 2023-02-23 12:44:10.723844 red-connector-semcon-2.0/red_connector_semcon/semcon/main.py
--rw-r--r--   0        0        0     3427 2023-02-24 09:03:48.916276 red-connector-semcon-2.0/red_connector_semcon/semcon/send_receive_file.py
--rw-r--r--   0        0        0       16 2023-02-24 09:09:24.585790 red-connector-semcon-2.0/red_connector_semcon/version.py
--rw-r--r--   0        0        0     1972 2023-02-24 09:14:04.811402 red-connector-semcon-2.0/setup.py
--rw-r--r--   0        0        0     1817 2023-02-24 09:14:04.811694 red-connector-semcon-2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-17 10:18:01.925936 red-connector-semcon-3.0.0/LICENSE
+-rw-r--r--   0        0        0      942 2023-05-15 09:22:11.438935 red-connector-semcon-3.0.0/README.md
+-rw-r--r--   0        0        0      630 2023-05-15 09:22:11.438935 red-connector-semcon-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-04-17 10:18:01.925936 red-connector-semcon-3.0.0/red_connector_semcon/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:18:01.925936 red-connector-semcon-3.0.0/red_connector_semcon/commons/__init__.py
+-rw-r--r--   0        0        0      809 2023-04-18 08:43:41.969871 red-connector-semcon-3.0.0/red_connector_semcon/commons/cli_modes.py
+-rw-r--r--   0        0        0     4690 2023-05-15 09:22:11.438935 red-connector-semcon-3.0.0/red_connector_semcon/commons/helpers.py
+-rw-r--r--   0        0        0     1654 2023-05-15 09:22:11.438935 red-connector-semcon-3.0.0/red_connector_semcon/commons/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:18:01.925936 red-connector-semcon-3.0.0/red_connector_semcon/semcon/__init__.py
+-rw-r--r--   0        0        0       89 2023-04-17 10:18:01.925936 red-connector-semcon-3.0.0/red_connector_semcon/semcon/__main__.py
+-rw-r--r--   0        0        0     1261 2023-04-17 10:18:01.925936 red-connector-semcon-3.0.0/red_connector_semcon/semcon/main.py
+-rw-r--r--   0        0        0     5012 2023-05-15 09:22:11.438935 red-connector-semcon-3.0.0/red_connector_semcon/semcon/send_receive_file.py
+-rw-r--r--   0        0        0       18 2023-05-15 09:22:11.438935 red-connector-semcon-3.0.0/red_connector_semcon/version.py
+-rw-r--r--   0        0        0     1923 2023-05-15 09:24:02.703336 red-connector-semcon-3.0.0/setup.py
+-rw-r--r--   0        0        0     1769 2023-05-15 09:24:02.703517 red-connector-semcon-3.0.0/PKG-INFO
```

### Comparing `red-connector-semcon-2.0/LICENSE` & `red-connector-semcon-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `red-connector-semcon-2.0/pyproject.toml` & `red-connector-semcon-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "red-connector-semcon"
-version = "2.0"
+version = "3.0.0"
 authors = ["Christoph Jansen <Christoph.Jansen@htw-berlin.de>", "Bruno Schilling <Bruno.Schilling@student.htw-berlin.de>"]
 license = "AGPL-3.0"
 readme = "README.md"
 repository = "https://github.com/curious-containers/red-connector-semcon"
 homepage = "https://www.curious-containers.cc/"
 description = "RED Connector Semcon is part of the Curious Containers project."
```

### Comparing `red-connector-semcon-2.0/red_connector_semcon/commons/cli_modes.py` & `red-connector-semcon-3.0.0/red_connector_semcon/commons/cli_modes.py`

 * *Files identical despite different names*

### Comparing `red-connector-semcon-2.0/red_connector_semcon/commons/helpers.py` & `red-connector-semcon-3.0.0/red_connector_semcon/commons/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import json
 import os
 import sys
 import jsonschema
 from functools import wraps
+from urllib.parse import urljoin
 
 import requests
-from requests.auth import HTTPBasicAuth, HTTPDigestAuth
 
 
 CONNECT_TIMEOUT = 12.05
 READ_TIMEOUT = 1000
 DEFAULT_TIMEOUT = (CONNECT_TIMEOUT, READ_TIMEOUT)
 
+OAUTH_ENDPOINT = '/oauth/token'
+OAUTH_GRANTTYPE = 'client_credentials'
+
 
 class ListingError(Exception):
     pass
 
 
 def graceful_error(func):
     @wraps(func)
@@ -47,72 +50,92 @@
         return requests.put
     if http_method == 'post':
         return requests.post
 
     raise Exception('Invalid HTTP method: {}'.format(http_method))
 
 
-def auth_method_obj(access):
+def oauth_token(access, verify, default_scope='read'):
     if not access.get('auth'):
         return None
-
+    
+    url = urljoin(access['url'], OAUTH_ENDPOINT)
     auth = access['auth']
-    auth_method = auth.get('method', 'basic').lower()
-
-    if auth_method == 'basic':
-        return HTTPBasicAuth(
-            auth['username'],
-            auth['password']
-        )
-    if auth_method == 'digest':
-        return HTTPDigestAuth(
-            auth['username'],
-            auth['password']
-        )
+    
+    client_id = auth['username']
+    client_secret = auth['password']
+    scope = auth.get('scope', default_scope)
+    
+    data = {
+        "client_id": client_id,
+        "client_secret": client_secret,
+        "grant_type": OAUTH_GRANTTYPE,
+        "scope": scope
+    }
+    
+    r = requests.post(
+        url,
+        json=data,
+        verify=verify,
+        stream=True,
+        timeout=(CONNECT_TIMEOUT, READ_TIMEOUT)
+    )
+    r.raise_for_status()
+    
+    access_token = r.json().get('access_token')
+    return access_token
 
-    raise Exception('Invalid auth method: {}'.format(auth_method))
+def bearer_auth_header(access_token):
+    if access_token is None:
+        return None
+    
+    headers = {
+        'Authorization': f"Bearer {access_token}"
+    }
+    return headers
 
 
-def fetch_file(file_path, url, http_method, auth_method, verify=True, data_key=None):
+def fetch_file(file_path, url, http_method, headers, params, verify=True, data_key=None):
     """
     Fetches the given file. Assumes that the directory in which this file is stored is already present in the local
     filesystem.
 
     :param file_path: The path where the file content should be stored
     :param url: The url from where to fetch the file
     :param http_method: An function object, which returns a requests result,
-    if called with (url, auth=auth_method, verify=verify, stream=True)
-    :param auth_method: An auth_method, which can be used as parameter for requests.http_method
+    if called with (url, headers=headers, params=params, verify=verify, stream=True)
+    :param headers: The request headers, which will be send with the http request.
+    :param params: The parameters, which will be send with the http request.
     :param verify: A boolean indicating if SSL Certification should be used.
     :param data_key: The key to index the json data. If None no key will be used.
 
     :raise requests.exceptions.HTTPError: If the HTTP requests could not be resolved correctly.
     """
 
     r = http_method(
         url,
-        auth=auth_method,
+        headers=headers,
+        params=params,
         verify=verify,
         stream=True,
         timeout=(CONNECT_TIMEOUT, READ_TIMEOUT)
     )
     r.raise_for_status()
-
-    data = r.json().get('data')
-    if data is None:
-        raise InvalidDataException('No data key in response.')
-    if len(data) < 1:
-        raise InvalidDataException('Empty data object.')
-    data = data[-1]  # always take last entry
-    if 'content' not in data:
-        raise InvalidDataException('No content key in data.')
-    data = data['content']
-
+    
+    data = r.json()
+    
     if data_key is not None:
-        data = data[data_key]
+        if 'data' in data:
+            data = data['data']
+        if 'content' in data:
+            data = data['content']
+        if isinstance(data, dict):
+            data = data[data_key]
+        else:
+            raise InvalidDataException('Data key can only be fetched from a dictonary.')
 
     with open(file_path, 'w') as f:
         if isinstance(data, str) and not file_path.endswith('.json'):  # dump strings as plain files. Not as json.
             f.write(data)
         else:
             json.dump(data, f)
```

### Comparing `red-connector-semcon-2.0/red_connector_semcon/commons/schemas.py` & `red-connector-semcon-3.0.0/red_connector_semcon/commons/schemas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,54 @@
 from copy import deepcopy
 
 
 _HTTP_METHODS = ['Get', 'Put', 'Post']
 _HTTP_METHODS_ENUMS = deepcopy(_HTTP_METHODS) + [m.lower() for m in _HTTP_METHODS] + [m.upper() for m in _HTTP_METHODS]
 
-_AUTH_METHODS = ['Basic', 'Digest']
-_AUTH_METHODS_ENUMS = deepcopy(_AUTH_METHODS) + [m.lower() for m in _AUTH_METHODS] + [m.upper() for m in _AUTH_METHODS]
+_RESOURCE_TYPE_ENUMS = ['id', 'dri', 'schema_dri', 'table']
+_OUTPUT_FORMAT_ENUMS = ['plain', 'full', 'meta', 'validation']
 
-SCHEMA = {
+_BASE_SCHEMA = {
     'type': 'object',
     'properties': {
         'url': {'type': 'string'},
         'method': {'enum': _HTTP_METHODS_ENUMS},
         'auth': {
             'type': 'object',
             'properties': {
                 'username': {'type': 'string'},
                 'password': {'type': 'string'},
-                'method': {'enum': _AUTH_METHODS_ENUMS}
+                'scope': {'type': 'string'}
             },
             'additionalProperties': False,
             'required': ['username', 'password']
         },
-        'key': {'type': 'string'},
         'disableSSLVerification': {'type': 'boolean'}
     },
     'additionalProperties': False,
-    'required': ['url', 'key']
+    'required': ['url']
+}
+
+RECEIVE_FILE_SCHEMA = deepcopy(_BASE_SCHEMA)
+RECEIVE_FILE_SCHEMA['properties']['resource'] = {
+    'type': 'object',
+    'properties': {
+        'resourceType': {'enum': _RESOURCE_TYPE_ENUMS},
+        'resourceValue': {'type': 'string'},
+        'key': {'type': 'string'},
+        'format': {'enum': _OUTPUT_FORMAT_ENUMS}
+    },
+    'additionalProperties': False,
+    'required': ['resourceType', 'resourceValue']
+}
+
+SEND_FILE_SCHEMA = deepcopy(_BASE_SCHEMA)
+SEND_FILE_SCHEMA['properties']['resource'] = {
+    'type': 'object',
+    'properties': {
+        'dri': {'type': 'string'},
+        'schemaDri': {'type': 'string'},
+        'tableName': {'type': 'string'},
+        'key': {'type': 'string'}
+    },
+    'additionalProperties': False
 }
```

### Comparing `red-connector-semcon-2.0/red_connector_semcon/semcon/main.py` & `red-connector-semcon-3.0.0/red_connector_semcon/semcon/main.py`

 * *Files identical despite different names*

### Comparing `red-connector-semcon-2.0/setup.py` & `red-connector-semcon-3.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 entry_points = \
 {'console_scripts': ['red-connector-semcon = '
                      'red_connector_semcon.semcon.main:main']}
 
 setup_kwargs = {
     'name': 'red-connector-semcon',
-    'version': '2.0',
+    'version': '3.0.0',
     'description': 'RED Connector Semcon is part of the Curious Containers project.',
-    'long_description': '# RED Connector Semcon\n\nRED Connector Semcon is part of the Curious Containers project.\n\nThis connector is designed to read data from a [semantic container](https://www.ownyourdata.eu/en/semcon/).\n\nFor more information please refer to the Curious Containers [documentation](https://www.curious-containers.cc/).\n\n## Limitations / Future Work\n- No O-Auth authentification used by Semantic Container. This may be implemented in the future.\n- Only handles json data from Semantic Container. No other format or binary data is supported.\n\n## Acknowledgements\n\nThe Curious Containers software is developed at [CBMI](https://cbmi.htw-berlin.de/) (HTW Berlin - University of Applied Sciences). The work is supported by the German Federal Ministry of Economic Affairs and Energy (ZIM project BeCRF, grant number KF3470401BZ4), the German Federal Ministry of Education and Research (project deep.TEACHING, grant number 01IS17056 and project deep.HEALTH, grant number 13FH770IX6) and HTW Berlin Booster.\n',
+    'long_description': '# RED Connector Semcon\n\nRED Connector Semcon is part of the Curious Containers project.\n\nThis connector is designed to read data from a [semantic container](https://www.ownyourdata.eu/en/semcon/).\n\nFor more information please refer to the Curious Containers [documentation](https://www.curious-containers.cc/).\n\n## Limitations / Future Work\n- Selections within the content of a data entry are partially supported in json format. For any other format this is currently not possible.\n\n## Acknowledgements\n\nThe Curious Containers software is developed at [CBMI](https://cbmi.htw-berlin.de/) (HTW Berlin - University of Applied Sciences). The work is supported by the German Federal Ministry of Economic Affairs and Energy (ZIM project BeCRF, grant number KF3470401BZ4), the German Federal Ministry of Education and Research (project deep.TEACHING, grant number 01IS17056 and project deep.HEALTH, grant number 13FH770IX6) and HTW Berlin Booster.\n',
     'author': 'Christoph Jansen',
     'author_email': 'Christoph.Jansen@htw-berlin.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.curious-containers.cc/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `red-connector-semcon-2.0/PKG-INFO` & `red-connector-semcon-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-connector-semcon
-Version: 2.0
+Version: 3.0.0
 Summary: RED Connector Semcon is part of the Curious Containers project.
 Home-page: https://www.curious-containers.cc/
 License: AGPL-3.0
 Author: Christoph Jansen
 Author-email: Christoph.Jansen@htw-berlin.de
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -23,14 +23,13 @@
 RED Connector Semcon is part of the Curious Containers project.
 
 This connector is designed to read data from a [semantic container](https://www.ownyourdata.eu/en/semcon/).
 
 For more information please refer to the Curious Containers [documentation](https://www.curious-containers.cc/).
 
 ## Limitations / Future Work
-- No O-Auth authentification used by Semantic Container. This may be implemented in the future.
-- Only handles json data from Semantic Container. No other format or binary data is supported.
+- Selections within the content of a data entry are partially supported in json format. For any other format this is currently not possible.
 
 ## Acknowledgements
 
 The Curious Containers software is developed at [CBMI](https://cbmi.htw-berlin.de/) (HTW Berlin - University of Applied Sciences). The work is supported by the German Federal Ministry of Economic Affairs and Energy (ZIM project BeCRF, grant number KF3470401BZ4), the German Federal Ministry of Education and Research (project deep.TEACHING, grant number 01IS17056 and project deep.HEALTH, grant number 13FH770IX6) and HTW Berlin Booster.
```

