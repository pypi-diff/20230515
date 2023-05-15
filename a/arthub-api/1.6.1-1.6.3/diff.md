# Comparing `tmp/arthub_api-1.6.1.tar.gz` & `tmp/arthub_api-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.6.1.tar", last modified: Fri May 12 03:07:27 2023, max compression
+gzip compressed data, was "arthub_api-1.6.3.tar", last modified: Mon May 15 09:23:52 2023, max compression
```

## Comparing `arthub_api-1.6.1.tar` & `arthub_api-1.6.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 03:07:27.645915 arthub_api-1.6.1/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.1/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-05-12 03:07:27.644918 arthub_api-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 03:07:27.625466 arthub_api-1.6.1/arthub_api/
--rw-rw-rw-   0        0        0      607 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     2316 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      233 2023-05-12 03:06:06.000000 arthub_api-1.6.1/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.1/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.1/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    37291 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0    22945 2023-05-11 11:42:27.000000 arthub_api-1.6.1/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.1/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.1/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.1/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.1/arthub_api/models.py
--rw-rw-rw-   0        0        0    41051 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.1/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 03:07:27.634757 arthub_api-1.6.1/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      814 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.1/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 03:07:27.645915 arthub_api-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     2908 2023-05-11 11:42:27.000000 arthub_api-1.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 03:07:27.643921 arthub_api-1.6.1/tests/
--rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.1/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.1/tests/_utils.py
--rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.1/tests/conftest.py
--rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.1/tests/test_open_api.py
--rw-rw-rw-   0        0        0    15230 2023-05-11 09:00:19.000000 arthub_api-1.6.1/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.1/tests/test_storage.py
--rw-rw-rw-   0        0        0     3691 2023-05-11 11:42:27.000000 arthub_api-1.6.1/tests/test_storage_blade.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:23:52.454767 arthub_api-1.6.3/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-05-15 09:23:52.453767 arthub_api-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 09:23:52.383916 arthub_api-1.6.3/arthub_api/
+-rw-rw-rw-   0        0        0      666 2023-05-15 09:23:22.000000 arthub_api-1.6.3/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     2316 2023-05-12 03:05:16.000000 arthub_api-1.6.3/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-05-15 09:23:22.000000 arthub_api-1.6.3/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.3/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.3/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.3/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    37291 2023-05-12 03:05:16.000000 arthub_api-1.6.3/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     1032 2023-05-15 09:23:22.000000 arthub_api-1.6.3/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    22945 2023-05-11 11:42:27.000000 arthub_api-1.6.3/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.3/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.3/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.3/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.3/arthub_api/models.py
+-rw-rw-rw-   0        0        0    41857 2023-05-15 09:23:22.000000 arthub_api-1.6.3/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.3/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.3/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:23:52.411904 arthub_api-1.6.3/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.3/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       65 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 09:23:52.454767 arthub_api-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     2908 2023-05-11 11:42:27.000000 arthub_api-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:23:52.451737 arthub_api-1.6.3/tests/
+-rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.3/tests/_utils.py
+-rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.3/tests/conftest.py
+-rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.3/tests/test_open_api.py
+-rw-rw-rw-   0        0        0    16594 2023-05-15 09:23:22.000000 arthub_api-1.6.3/tests/test_open_api_blade.py
+-rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.3/tests/test_storage.py
+-rw-rw-rw-   0        0        0     3691 2023-05-11 11:42:27.000000 arthub_api-1.6.3/tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.1/LICENSE` & `arthub_api-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/PKG-INFO` & `arthub_api-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.6.1
+Version: 1.6.3
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.1/README.md` & `arthub_api-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/__init__.py` & `arthub_api-1.6.3/arthub_api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     APIResponse
 )
 
 from .blade_api import (
     BladeAPI
 )
 
+from .blade_api_instance import (
+    BladeInstance
+)
+
 from .blade_storage import (
     Client,
     BladeCOSApi
 )
 
 from .storage import (
     Storage,
```

### Comparing `arthub_api-1.6.1/arthub_api/__main__.py` & `arthub_api-1.6.3/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/_internal_utils.py` & `arthub_api-1.6.3/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/asset_matrix.py` & `arthub_api-1.6.3/arthub_api/asset_matrix.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/blade_api.py` & `arthub_api-1.6.3/arthub_api/blade_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/blade_storage.py` & `arthub_api-1.6.3/arthub_api/blade_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/config.py` & `arthub_api-1.6.3/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/exception.py` & `arthub_api-1.6.3/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/models.py` & `arthub_api-1.6.3/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/open_api.py` & `arthub_api-1.6.3/arthub_api/open_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,38 @@
             "updated_date",
             "description",
             "total_leaf_count"
         ]
     return metas
 
 
+class APIError(Exception):
+    pass
+
+
+class NotLoginError(Exception):
+    pass
+
+
+class NoPermissionError(Exception):
+    pass
+
+
 class APIResponse(object):
     def __init__(self, http_response, network_connection_failed=False):
         self._http_response = http_response
         self._network_connection_failed = network_connection_failed
         self._direct_result = None
 
         self.api_result_code = -9999
         self.api_item_result_code = -9999
         self.api_error_message = "Unknown"
         self.results = {}
         self.errors = {}
+        self.exception = None
 
         self._preprocess()
 
     def _preprocess(self):
         if self._network_connection_failed:
             return
         if self._http_response is None:
@@ -73,15 +86,16 @@
             # parse error
             self.parse_items(_data.get("error"), self.errors)
             # parse error message
             self._parse_error()
             if type(self.results) == dict:
                 self._direct_result = list(self.results.values())
 
-        except Exception:
+        except Exception as e:
+            self.exception = e
             logging.error("[API] parsing response exception, \"%s\"" % self._http_response.text)
 
     def _parse_error(self):
         if not self.errors:
             return
         e = self.errors.get(next(iter(self.errors)))
         if e is None:
@@ -229,14 +243,26 @@
         if self.is_no_permission():
             return "no permission"
         if self.is_node_not_exist():
             return "node not exist"
 
         return self.api_error_message
 
+    def raise_for_err(res):
+        if res.exception is not None:
+            raise res.exception
+        if not res._http_response.ok:
+            raise APIError("http request failed, code: %d" % res._http_response.status_code)
+        if not res.is_succeeded():
+            if res.is_api_authentication_failed():
+                raise NotLoginError("authentication failed")
+            if res.is_no_permission():
+                raise NoPermissionError("no permission")
+            raise APIError("err from api {0}".format(res.api_error_message))
+
 
 class OpenAPI(object):
     def __init__(self, config, get_token_from_cache=True):
         r"""Used to call ArtHub openapi.
         for detailed interface doc: "https://arthub.qq.com/user_manual/index.html"
 
         :param config: from arthub_api.config.
@@ -392,14 +418,15 @@
 
         # send request
         try:
             res = requests.request(method=method, url=url, headers=headers, json=data, cookies=self._cookies)
         except Exception as e:
             logging.error("[API] send request \"%s\" exception: %s" % (url, e))
             response = APIResponse(None, True)
+            response.exception = e
             return response
 
         response = APIResponse(res)
         if response.is_api_authentication_failed() and try_login_on_expired:
             # Try to log in again due to authentication failure
             if self._try_auto_login():
                 response = self._make_api_request(url, data, method, content_type, try_login_on_expired=False)
```

### Comparing `arthub_api-1.6.1/arthub_api/storage.py` & `arthub_api-1.6.3/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api/utils.py` & `arthub_api-1.6.3/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.6.3/arthub_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.6.1
+Version: 1.6.3
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.1/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.6.3/arthub_api.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 arthub_api/__init__.py
 arthub_api/__main__.py
 arthub_api/__version__.py
 arthub_api/_internal_utils.py
 arthub_api/arthub_api_config.py
 arthub_api/asset_matrix.py
 arthub_api/blade_api.py
+arthub_api/blade_api_instance.py
 arthub_api/blade_storage.py
 arthub_api/cli.py
 arthub_api/config.py
 arthub_api/exception.py
 arthub_api/models.py
 arthub_api/open_api.py
 arthub_api/storage.py
```

### Comparing `arthub_api-1.6.1/setup.py` & `arthub_api-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/tests/test_open_api.py` & `arthub_api-1.6.3/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/tests/test_open_api_blade.py` & `arthub_api-1.6.3/tests/test_open_api_blade.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,515 +1,546 @@
-import arthub_api
-import pytest
-import logging
-from arthub_api import arthub_api_config
-from . import _utils
-from arthub_api import (
-    BladeAPI,
-)
-
-
-def on_api_failed(res):
-    logging.error("[TEST][API][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
-
-
-def init_api(env, login=True):
-    api = BladeAPI(_utils.get_config(env), False)
-    if login:
-        res = api.login(arthub_api_config.account_email, arthub_api_config.password)
-        assert res.is_succeeded()
-    return api
-
-
-def get_current_role_id(env):
-    blade_api = init_api(env)
-    res = blade_api.get_account_detail()
-    assert res.is_succeeded()
-    return res.result["id"]
-
-
-def get_account_role_id(env, account_name):
-    blade_api = init_api(env)
-    res = blade_api.get_account_detail([account_name])
-    assert res.is_succeeded()
-    return res.result["id"]
-
-
-def get_root_id(env):
-    blade_api = init_api(env)
-    res = blade_api.blade_get_root_id()
-    assert res.is_succeeded()
-    return res.result
-
-
-def get_node(env, node_id, parent_id):
-    blade_api = init_api(env)
-    res = blade_api.blade_get_node_brief_by_id([{"id": node_id, "parent_id": parent_id}])
-    assert res.is_succeeded()
-    return res.first_result()
-
-
-def delete_node(env, node_id, parent_id):
-    blade_api = init_api(env)
-    res = blade_api.blade_delete_node_brief_by_id([{"id": node_id, "parent_id": parent_id}])
-    assert res.is_succeeded()
-    return res.first_result()
-
-
-def test_blade_type_option_info(env):
-    blade_api = init_api(env)
-    res = blade_api.blade_get_type_option_info()
-    if not res.is_succeeded() or type(res.result) != list:
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, current types length: %d" % (res.url, len(res.result)))
-
-
-def test_blade_toolbox(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    # create
-    toolbox_payload = {
-        "parent_id": root_id,
-        "name": "sdk_test_name",
-        "description": "toolbox for sdk test",
-        "short_name": "sdk_test_short_name",
-    }
-    res = blade_api.blade_create_toolbox(toolbox_payload)
-    assert res.is_succeeded()
-    toolbox_id = res.result
-
-    # get
-    node_brief = get_node(env, toolbox_id, root_id)
-    assert toolbox_payload["name"] == node_brief["name"]
-
-    # update
-    update_payload = {
-        "id": toolbox_id,
-        "name": "sdk_test_name",
-        "description": "toolbox for sdk test",
-        "short_name": "sdk_test_short_name",
-    }
-    res = blade_api.blade_update_toolbox(update_payload)
-    assert res.is_succeeded()
-
-    # get
-    node_brief = get_node(env, toolbox_id, root_id)
-    assert update_payload["name"] == node_brief["name"]
-    assert update_payload["description"] == node_brief["description"]
-    assert update_payload["short_name"] == node_brief["short_name"]
-
-    # delete
-    delete_node(env, toolbox_id, root_id)
-
-
-def test_blade_tool(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    # create first toolbox
-    toolbox_payload = {
-        "parent_id": root_id,
-        "name": "test_dir",
-        "short_name": "sdk_test_short_name",
-    }
-    res = blade_api.blade_create_toolbox(toolbox_payload)
-    assert res.is_succeeded()
-    toolbox_id_1 = res.result
-
-    # create tool
-    tool_payload = {
-        "parent_id": toolbox_id_1,
-        "name": "sdk_test_name",
-        "flag_color": "red",
-        "flag_content": "2020",
-    }
-    res = blade_api.blade_create_tool(tool_payload)
-    assert res.is_succeeded()
-    tool_id = res.result
-
-    # get
-    node_brief = get_node(env, tool_id, toolbox_id_1)
-    assert tool_payload["name"] == node_brief["name"]
-    assert node_brief["is_hard_link"]
-
-    # update
-    update_payload = {
-        "id": tool_id,
-        "name": "sdk_test_name_2",
-        "description": "tool for sdk test 2",
-        "command": "test command 2",
-        "command_type": "cmd",
-        "type_option": 2,
-        "flag_color": "blue",
-        "flag_content": "2022",
-    }
-    res = blade_api.blade_update_tool(update_payload)
-    assert res.is_succeeded()
-
-    # get
-    node_brief = get_node(env, tool_id, toolbox_id_1)
-    assert update_payload["name"] == node_brief["name"]
-    assert update_payload["description"] == node_brief["description"]
-    assert update_payload["command"] == node_brief["command"]
-    assert update_payload["command_type"] == node_brief["command_type"]
-    assert update_payload["type_option"] == node_brief["type_option"]
-    assert update_payload["flag_color"] == node_brief["flag_color"]
-    assert update_payload["flag_content"] == node_brief["flag_content"]
-
-    # test share
-    # create second toolbox
-    res = blade_api.blade_create_toolbox({"parent_id": root_id, "name": "dir_to_move"})
-    assert res.is_succeeded()
-    toolbox_id_2 = res.result
-    # share
-    res = blade_api.blade_share_tool([tool_id], toolbox_id_1, toolbox_id_2)
-    assert res.is_succeeded()
-
-    # test get child
-    res = blade_api.blade_get_child_node_count(toolbox_id_2)
-    assert res.is_succeeded()
-    assert res.result == 1
-    res = blade_api.blade_get_child_node_brief_in_range(toolbox_id_2)
-    assert res.is_succeeded()
-    assert res.result[0]["is_hard_link"] is False
-
-    # delete toolbox
-    delete_node(env, toolbox_id_1, root_id)
-    delete_node(env, toolbox_id_2, root_id)
-
-
-def test_edit_user(env):
-    blade_api = init_api(env)
-    qywx_alias = "bytian"
-
-    # create origin
-    account_id = get_account_role_id(env, qywx_alias)
-    # delete
-    res = blade_api.blade_delete_user_by_id(account_id)
-    assert res.is_succeeded()
-
-    # create
-    res = blade_api.blade_create_user({
-        "qywxalias": qywx_alias,
-        "email": "12345@qq.com",
-        "fullname": "tian",
-        "position": "dev",
-    })
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-    user_id = res.result
-
-    # update
-    res = blade_api.blade_update_user_by_id({
-        "id": user_id,
-        "email": "6789@qq.com",
-        "fullname": "tian2",
-        "position": "art",
-    })
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_user_by_id(user_id)
-    assert res.is_succeeded()
-    user_info = res.result
-    res = blade_api.blade_get_user_by_qywx_alias(qywx_alias)
-    assert res.is_succeeded()
-    assert user_info == res.result
-    assert user_info["email"] == "6789@qq.com"
-    logging.info("[TEST][API] get user success: %s" % user_info)
-
-    # delete
-    res = blade_api.blade_delete_user_by_id(user_id)
-    assert res.is_succeeded()
-
-
-def test_edit_config(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-    role_id = get_current_role_id(env)
-
-    name = "test_sdk"
-    config = {"env": 1}
-    # create
-    res = blade_api.blade_create_config(name, root_id, "node", config)
-    assert res.is_succeeded()
-
-    # update
-    config_new = {"env_new": 2}
-    res = blade_api.blade_update_config(name, root_id, "node", config_new)
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_config(name, root_id, "node")
-    assert res.is_succeeded()
-    result_config = res.result["config"]
-    logging.info("[TEST][API] get config success: %s" % result_config)
-    assert result_config == config_new
-
-    # create on role
-    config_role = {"env_role": 3}
-    res = blade_api.blade_create_config(name, role_id, "role", config_role)
-    assert res.is_succeeded()
-    res = blade_api.blade_batch_get_config([name], [root_id])
-    logging.info("[TEST][API] batch get config success: %s" % res.result)
-
-    # delete
-    res = blade_api.blade_delete_config(name, root_id, "node")
-    assert res.is_succeeded()
-    res = blade_api.blade_delete_config(name, role_id, "role")
-    assert res.is_succeeded()
-
-
-def test_edit_plugin(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-    role_id = get_current_role_id(env)
-
-    name = "test_sdk"
-    plugin = {
-        "runnable": True,
-        "shellable": False,
-        "short_help": "start test",
-        "packages": [
-            "pkg_1",
-            "pkg_2"
-        ]
-    }
-    # create
-    res = blade_api.blade_create_plugin(name, root_id, "node", plugin)
-    assert res.is_succeeded()
-
-    # update
-    res = blade_api.blade_update_plugin(name, root_id, "node", {
-        "is_packages_change": True,
-        "packages": ["pkg_3"]
-    })
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_plugin(name, root_id, "node")
-    assert res.is_succeeded()
-    logging.info("[TEST][API] get plugin success: %s" % res.result)
-    assert res.result["short_help"] == plugin["short_help"]
-    assert res.result["packages"] == ["pkg_3"]
-
-    # create on role
-    plugin_role = {
-        "runnable": False,
-        "shellable": True,
-        "short_help": "start test on role",
-        "packages": [
-            "pkg_role"
-        ]
-    }
-    res = blade_api.blade_create_plugin(name, role_id, "role", plugin_role)
-    assert res.is_succeeded()
-    res = blade_api.blade_batch_get_plugin([name], [root_id])
-    logging.info("[TEST][API] batch get plugin success: %s" % res.result)
-
-    # delete
-    res = blade_api.blade_delete_config(name, root_id, "node")
-    res = blade_api.blade_delete_config(name, role_id, "role")
-    assert res.is_succeeded()
-
-
-def test_edit_public_token(env):
-    blade_api = init_api(env)
-    # create
-    res = blade_api.blade_create_public_token("sdk_test_token", 10)
-    assert res.is_succeeded()
-    token_id = res.result["id"]
-    token_str = res.result["name"]
-
-    # update
-    res = blade_api.blade_update_public_token_by_id({
-        "id": token_id,
-        "fullname": "sdk_test_token_new",
-        "duration": 100,
-    })
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_public_token_by_id(token_id)
-    assert res.is_succeeded()
-    token_info = res.result
-    res = blade_api.blade_get_public_token_by_name(token_str)
-    assert res.is_succeeded()
-    assert token_info == res.result
-    assert token_info["duration"] == 100
-    logging.info("[TEST][API] get token success: %s" % token_info)
-
-    # delete
-    res = blade_api.blade_delete_public_token_by_id(token_id)
-    assert res.is_succeeded()
-
-
-def test_permission_on_toolbox(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    res = blade_api.blade_create_public_token("sdk_test_token", 100)
-    assert res.is_succeeded()
-    token_id = res.result["id"]
-    token_str = res.result["name"]
-
-    # set public token to toolbox permission
-    # create toolbox
-    res = blade_api.blade_create_toolbox({"parent_id": root_id, "name": "test_perm_dir"})
-    assert res.is_succeeded()
-    toolbox_id = res.result
-
-    # add
-    perm_item = {"account_name": token_str, "type": "public_token"}
-    res = blade_api.blade_add_permission_on_toolbox_by_account_name(toolbox_id, "developer", [perm_item])
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_permission_on_toolbox(toolbox_id)
-    assert res.is_succeeded()
-    assert res.result["developer"][0] == perm_item
-
-    # delete
-    res = blade_api.blade_delete_permission_on_toolbox_by_account_name(toolbox_id, [perm_item])
-    assert res.is_succeeded()
-
-    # delete toolbox
-    delete_node(env, toolbox_id, root_id)
-
-
-def test_permission_on_config(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    res = blade_api.blade_create_public_token("sdk_test_token_config", 100)
-    assert res.is_succeeded()
-    token_str = res.result["name"]
-
-    # set public token to config permission
-    # add
-    perm_item = {"account_name": token_str, "type": "public_token"}
-    res = blade_api.blade_add_permission_on_config_by_account_name("developer", [perm_item])
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_permission_on_config()
-    assert res.is_succeeded()
-    assert res.result["developer"][0] == perm_item
-
-    # public token permission test
-    blade_api_token = init_api(env, False)
-    blade_api_token.set_blade_public_token(token_str)
-    res = blade_api_token.blade_list_user()
-    assert res.is_succeeded()
-    res = blade_api_token.blade_create_config("token_test", root_id, "node", {"hello": "world"})
-    assert res.is_succeeded()
-    res = blade_api_token.blade_delete_config("token_test", root_id, "node")
-    assert res.is_succeeded()
-
-    # delete
-    res = blade_api.blade_delete_permission_on_config_by_account_name([perm_item])
-    assert res.is_succeeded()
-
-def test_convert_context_string(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    res = blade_api.blade_convert_context_string("globals:globals", "lightbox_config")
-    assert res.is_succeeded()
-    out = res.first_result()
-    context_id = out.get("context_id")
-    context_type = out.get("context_type")
-    assert root_id==context_id
-    assert "node"==context_type
-
-    res = blade_api.blade_convert_context_string("etc", "thm_plugins")
-    assert res.is_succeeded()
-    out = res.first_result()
-    context_id = out.get("context_id")
-    context_type = out.get("context_type")
-    assert root_id==context_id
-    assert "node"==context_type
-    
-def test_edit_package(env):
-    blade_api = init_api(env)
-    # create
-    pkg_info={
-        "authors": [
-            "Guido van Rossum"
-        ],
-        "category": "ext",
-        "description": "The Python programming language.",
-        "homepage": "https://www.python.org/",
-        "name": "arthub_test_pkg",
-        "requires": [],
-        "tools": [
-            "python"
-        ],
-        "variants": [
-            [
-            "platform-windows",
-            "python_embedded"
-            ],
-            [
-            "platform-windows",
-            "!python_embedded"
-            ]
-        ],
-        "version": "0.0.1"
-    }
-    
-    # upload
-    res = blade_api.blade_upload_package([{"name":pkg_info.get("name"), "version":pkg_info.get("version")}], force=True)
-    assert res.is_succeeded()
-    
-    # create
-    res = blade_api.blade_create_package(pkg_info, upsert=True)
-    assert res.is_succeeded()
-    
-    # create failed
-    res = blade_api.blade_create_package(pkg_info, upsert=False)
-    assert not res.is_succeeded()
-    
-    # get 1
-    res = blade_api.blade_get_package(name="arthub_test_pkg", version="0.0.1")
-    assert res.is_succeeded()
-    pkg_info_1 = res.result
-    del pkg_info_1["api_modified"]
-
-    # update
-    res = blade_api.blade_update_package(**{
-        "name": "arthub_test_pkg",
-        "version": "0.0.1",
-        "tools": [
-            "no-tools"
-        ],
-        "requires": ["python"]
-    })
-    assert res.is_succeeded()
-    pkg_info_1.update({
-        "tools": [
-            "no-tools"
-        ],
-        "requires": ["python"],
-    })    
-    
-    # get 2
-    res = blade_api.blade_get_package(name="arthub_test_pkg", version="0.0.1")
-    assert res.is_succeeded()
-    pkg_info_2 = res.result
-    del pkg_info_2["api_modified"]
-    
-    # cmp
-    assert pkg_info_1 == pkg_info_2
-    assert pkg_info_2.get("tools") == ["no-tools"]
-    logging.info("[TEST][API] edit package success: %s" % pkg_info)
-
-    # download
-    res = blade_api.blade_download_package([{"name":pkg_info.get("name"), "version":pkg_info.get("version")}])
-    assert res.is_succeeded()
-    
-    # no-delete-method
-    
+from requests import JSONDecodeError
+
+import arthub_api
+import pytest
+import logging
+
+from arthub_api.open_api import NotLoginError
+from . import _utils
+from arthub_api import (
+    arthub_api_config,
+    BladeAPI,
+)
+from arthub_api.blade_api_instance import BladeInstance
+
+
+def on_api_failed(res):
+    logging.error("[TEST][API][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
+
+
+def init_api(env, login=True):
+    api = BladeAPI(_utils.get_config(env), False)
+    if login:
+        res = api.login(arthub_api_config.account_email, arthub_api_config.password)
+        assert res.is_succeeded()
+    return api
+
+
+def get_current_role_id(env):
+    blade_api = init_api(env)
+    res = blade_api.get_account_detail()
+    assert res.is_succeeded()
+    return res.result["id"]
+
+
+def get_account_role_id(env, account_name):
+    blade_api = init_api(env)
+    res = blade_api.get_account_detail([account_name])
+    assert res.is_succeeded()
+    return res.result["id"]
+
+
+def get_root_id(env):
+    blade_api = init_api(env)
+    res = blade_api.blade_get_root_id()
+    assert res.is_succeeded()
+    return res.result
+
+
+def get_node(env, node_id, parent_id):
+    blade_api = init_api(env)
+    res = blade_api.blade_get_node_brief_by_id([{"id": node_id, "parent_id": parent_id}])
+    assert res.is_succeeded()
+    return res.first_result()
+
+
+def delete_node(env, node_id, parent_id):
+    blade_api = init_api(env)
+    res = blade_api.blade_delete_node_brief_by_id([{"id": node_id, "parent_id": parent_id}])
+    assert res.is_succeeded()
+    return res.first_result()
+
+
+def test_blade_type_option_info(env):
+    blade_api = init_api(env)
+    res = blade_api.blade_get_type_option_info()
+    if not res.is_succeeded() or type(res.result) != list:
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, current types length: %d" % (res.url, len(res.result)))
+
+
+def test_blade_toolbox(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    # create
+    toolbox_payload = {
+        "parent_id": root_id,
+        "name": "sdk_test_name",
+        "description": "toolbox for sdk test",
+        "short_name": "sdk_test_short_name",
+    }
+    res = blade_api.blade_create_toolbox(toolbox_payload)
+    assert res.is_succeeded()
+    toolbox_id = res.result
+
+    # get
+    node_brief = get_node(env, toolbox_id, root_id)
+    assert toolbox_payload["name"] == node_brief["name"]
+
+    # update
+    update_payload = {
+        "id": toolbox_id,
+        "name": "sdk_test_name",
+        "description": "toolbox for sdk test",
+        "short_name": "sdk_test_short_name",
+    }
+    res = blade_api.blade_update_toolbox(update_payload)
+    assert res.is_succeeded()
+
+    # get
+    node_brief = get_node(env, toolbox_id, root_id)
+    assert update_payload["name"] == node_brief["name"]
+    assert update_payload["description"] == node_brief["description"]
+    assert update_payload["short_name"] == node_brief["short_name"]
+
+    # delete
+    delete_node(env, toolbox_id, root_id)
+
+
+def test_blade_tool(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    # create first toolbox
+    toolbox_payload = {
+        "parent_id": root_id,
+        "name": "test_dir",
+        "short_name": "sdk_test_short_name",
+    }
+    res = blade_api.blade_create_toolbox(toolbox_payload)
+    assert res.is_succeeded()
+    toolbox_id_1 = res.result
+
+    # create tool
+    tool_payload = {
+        "parent_id": toolbox_id_1,
+        "name": "sdk_test_name",
+        "flag_color": "red",
+        "flag_content": "2020",
+    }
+    res = blade_api.blade_create_tool(tool_payload)
+    assert res.is_succeeded()
+    tool_id = res.result
+
+    # get
+    node_brief = get_node(env, tool_id, toolbox_id_1)
+    assert tool_payload["name"] == node_brief["name"]
+    assert node_brief["is_hard_link"]
+
+    # update
+    update_payload = {
+        "id": tool_id,
+        "name": "sdk_test_name_2",
+        "description": "tool for sdk test 2",
+        "command": "test command 2",
+        "command_type": "cmd",
+        "type_option": 2,
+        "flag_color": "blue",
+        "flag_content": "2022",
+    }
+    res = blade_api.blade_update_tool(update_payload)
+    assert res.is_succeeded()
+
+    # get
+    node_brief = get_node(env, tool_id, toolbox_id_1)
+    assert update_payload["name"] == node_brief["name"]
+    assert update_payload["description"] == node_brief["description"]
+    assert update_payload["command"] == node_brief["command"]
+    assert update_payload["command_type"] == node_brief["command_type"]
+    assert update_payload["type_option"] == node_brief["type_option"]
+    assert update_payload["flag_color"] == node_brief["flag_color"]
+    assert update_payload["flag_content"] == node_brief["flag_content"]
+
+    # test share
+    # create second toolbox
+    res = blade_api.blade_create_toolbox({"parent_id": root_id, "name": "dir_to_move"})
+    assert res.is_succeeded()
+    toolbox_id_2 = res.result
+    # share
+    res = blade_api.blade_share_tool([tool_id], toolbox_id_1, toolbox_id_2)
+    assert res.is_succeeded()
+
+    # test get child
+    res = blade_api.blade_get_child_node_count(toolbox_id_2)
+    assert res.is_succeeded()
+    assert res.result == 1
+    res = blade_api.blade_get_child_node_brief_in_range(toolbox_id_2)
+    assert res.is_succeeded()
+    assert res.result[0]["is_hard_link"] is False
+
+    # delete toolbox
+    delete_node(env, toolbox_id_1, root_id)
+    delete_node(env, toolbox_id_2, root_id)
+
+
+def test_edit_user(env):
+    blade_api = init_api(env)
+    qywx_alias = "bytian"
+
+    # create origin
+    account_id = get_account_role_id(env, qywx_alias)
+    # delete
+    res = blade_api.blade_delete_user_by_id(account_id)
+    assert res.is_succeeded()
+
+    # create
+    res = blade_api.blade_create_user({
+        "qywxalias": qywx_alias,
+        "email": "12345@qq.com",
+        "fullname": "tian",
+        "position": "dev",
+    })
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+    user_id = res.result
+
+    # update
+    res = blade_api.blade_update_user_by_id({
+        "id": user_id,
+        "email": "6789@qq.com",
+        "fullname": "tian2",
+        "position": "art",
+    })
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_user_by_id(user_id)
+    assert res.is_succeeded()
+    user_info = res.result
+    res = blade_api.blade_get_user_by_qywx_alias(qywx_alias)
+    assert res.is_succeeded()
+    assert user_info == res.result
+    assert user_info["email"] == "6789@qq.com"
+    logging.info("[TEST][API] get user success: %s" % user_info)
+
+    # delete
+    res = blade_api.blade_delete_user_by_id(user_id)
+    assert res.is_succeeded()
+
+
+def test_edit_config(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+    role_id = get_current_role_id(env)
+
+    name = "test_sdk"
+    config = {"env": 1}
+    # create
+    res = blade_api.blade_create_config(name, root_id, "node", config)
+    assert res.is_succeeded()
+
+    # update
+    config_new = {"env_new": 2}
+    res = blade_api.blade_update_config(name, root_id, "node", config_new)
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_config(name, root_id, "node")
+    assert res.is_succeeded()
+    result_config = res.result["config"]
+    logging.info("[TEST][API] get config success: %s" % result_config)
+    assert result_config == config_new
+
+    # create on role
+    config_role = {"env_role": 3}
+    res = blade_api.blade_create_config(name, role_id, "role", config_role)
+    assert res.is_succeeded()
+    res = blade_api.blade_batch_get_config([name], [root_id])
+    logging.info("[TEST][API] batch get config success: %s" % res.result)
+
+    # delete
+    res = blade_api.blade_delete_config(name, root_id, "node")
+    assert res.is_succeeded()
+    res = blade_api.blade_delete_config(name, role_id, "role")
+    assert res.is_succeeded()
+
+
+def test_edit_plugin(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+    role_id = get_current_role_id(env)
+
+    name = "test_sdk"
+    plugin = {
+        "runnable": True,
+        "shellable": False,
+        "short_help": "start test",
+        "packages": [
+            "pkg_1",
+            "pkg_2"
+        ]
+    }
+    # create
+    res = blade_api.blade_create_plugin(name, root_id, "node", plugin)
+    assert res.is_succeeded()
+
+    # update
+    res = blade_api.blade_update_plugin(name, root_id, "node", {
+        "is_packages_change": True,
+        "packages": ["pkg_3"]
+    })
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_plugin(name, root_id, "node")
+    assert res.is_succeeded()
+    logging.info("[TEST][API] get plugin success: %s" % res.result)
+    assert res.result["short_help"] == plugin["short_help"]
+    assert res.result["packages"] == ["pkg_3"]
+
+    # create on role
+    plugin_role = {
+        "runnable": False,
+        "shellable": True,
+        "short_help": "start test on role",
+        "packages": [
+            "pkg_role"
+        ]
+    }
+    res = blade_api.blade_create_plugin(name, role_id, "role", plugin_role)
+    assert res.is_succeeded()
+    res = blade_api.blade_batch_get_plugin([name], [root_id])
+    logging.info("[TEST][API] batch get plugin success: %s" % res.result)
+
+    # delete
+    res = blade_api.blade_delete_config(name, root_id, "node")
+    res = blade_api.blade_delete_config(name, role_id, "role")
+    assert res.is_succeeded()
+
+
+def test_edit_public_token(env):
+    blade_api = init_api(env)
+    # create
+    res = blade_api.blade_create_public_token("sdk_test_token", 10)
+    assert res.is_succeeded()
+    token_id = res.result["id"]
+    token_str = res.result["name"]
+
+    # update
+    res = blade_api.blade_update_public_token_by_id({
+        "id": token_id,
+        "fullname": "sdk_test_token_new",
+        "duration": 100,
+    })
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_public_token_by_id(token_id)
+    assert res.is_succeeded()
+    token_info = res.result
+    res = blade_api.blade_get_public_token_by_name(token_str)
+    assert res.is_succeeded()
+    assert token_info == res.result
+    assert token_info["duration"] == 100
+    logging.info("[TEST][API] get token success: %s" % token_info)
+
+    # delete
+    res = blade_api.blade_delete_public_token_by_id(token_id)
+    assert res.is_succeeded()
+
+
+def test_permission_on_toolbox(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    res = blade_api.blade_create_public_token("sdk_test_token", 100)
+    assert res.is_succeeded()
+    token_id = res.result["id"]
+    token_str = res.result["name"]
+
+    # set public token to toolbox permission
+    # create toolbox
+    res = blade_api.blade_create_toolbox({"parent_id": root_id, "name": "test_perm_dir"})
+    assert res.is_succeeded()
+    toolbox_id = res.result
+
+    # add
+    perm_item = {"account_name": token_str, "type": "public_token"}
+    res = blade_api.blade_add_permission_on_toolbox_by_account_name(toolbox_id, "developer", [perm_item])
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_permission_on_toolbox(toolbox_id)
+    assert res.is_succeeded()
+    assert res.result["developer"][0] == perm_item
+
+    # delete
+    res = blade_api.blade_delete_permission_on_toolbox_by_account_name(toolbox_id, [perm_item])
+    assert res.is_succeeded()
+
+    # delete toolbox
+    delete_node(env, toolbox_id, root_id)
+
+
+def test_permission_on_config(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    res = blade_api.blade_create_public_token("sdk_test_token_config", 100)
+    assert res.is_succeeded()
+    token_str = res.result["name"]
+
+    # set public token to config permission
+    # add
+    perm_item = {"account_name": token_str, "type": "public_token"}
+    res = blade_api.blade_add_permission_on_config_by_account_name("developer", [perm_item])
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_permission_on_config()
+    assert res.is_succeeded()
+    assert res.result["developer"][0] == perm_item
+
+    # public token permission test
+    blade_api_token = init_api(env, False)
+    blade_api_token.set_blade_public_token(token_str)
+    res = blade_api_token.blade_list_user()
+    assert res.is_succeeded()
+    res = blade_api_token.blade_create_config("token_test", root_id, "node", {"hello": "world"})
+    assert res.is_succeeded()
+    res = blade_api_token.blade_delete_config("token_test", root_id, "node")
+    assert res.is_succeeded()
+
+    # delete
+    res = blade_api.blade_delete_permission_on_config_by_account_name([perm_item])
+    assert res.is_succeeded()
+
+def test_convert_context_string(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    res = blade_api.blade_convert_context_string("globals:globals", "lightbox_config")
+    assert res.is_succeeded()
+    out = res.first_result()
+    context_id = out.get("context_id")
+    context_type = out.get("context_type")
+    assert root_id==context_id
+    assert "node"==context_type
+
+    res = blade_api.blade_convert_context_string("etc", "thm_plugins")
+    assert res.is_succeeded()
+    out = res.first_result()
+    context_id = out.get("context_id")
+    context_type = out.get("context_type")
+    assert root_id==context_id
+    assert "node"==context_type
+    
+def test_edit_package(env):
+    blade_api = init_api(env)
+    # create
+    pkg_info={
+        "authors": [
+            "Guido van Rossum"
+        ],
+        "category": "ext",
+        "description": "The Python programming language.",
+        "homepage": "https://www.python.org/",
+        "name": "arthub_test_pkg",
+        "requires": [],
+        "tools": [
+            "python"
+        ],
+        "variants": [
+            [
+            "platform-windows",
+            "python_embedded"
+            ],
+            [
+            "platform-windows",
+            "!python_embedded"
+            ]
+        ],
+        "version": "0.0.1"
+    }
+    
+    # upload
+    res = blade_api.blade_upload_package([{"name":pkg_info.get("name"), "version":pkg_info.get("version")}], force=True)
+    assert res.is_succeeded()
+    
+    # create
+    res = blade_api.blade_create_package(pkg_info, upsert=True)
+    assert res.is_succeeded()
+    
+    # create failed
+    res = blade_api.blade_create_package(pkg_info, upsert=False)
+    assert not res.is_succeeded()
+    
+    # get 1
+    res = blade_api.blade_get_package(name="arthub_test_pkg", version="0.0.1")
+    assert res.is_succeeded()
+    pkg_info_1 = res.result
+    del pkg_info_1["api_modified"]
+
+    # update
+    res = blade_api.blade_update_package(**{
+        "name": "arthub_test_pkg",
+        "version": "0.0.1",
+        "tools": [
+            "no-tools"
+        ],
+        "requires": ["python"]
+    })
+    assert res.is_succeeded()
+    pkg_info_1.update({
+        "tools": [
+            "no-tools"
+        ],
+        "requires": ["python"],
+    })    
+    
+    # get 2
+    res = blade_api.blade_get_package(name="arthub_test_pkg", version="0.0.1")
+    assert res.is_succeeded()
+    pkg_info_2 = res.result
+    del pkg_info_2["api_modified"]
+    
+    # cmp
+    assert pkg_info_1 == pkg_info_2
+    assert pkg_info_2.get("tools") == ["no-tools"]
+    logging.info("[TEST][API] edit package success: %s" % pkg_info)
+
+    # download
+    res = blade_api.blade_download_package([{"name":pkg_info.get("name"), "version":pkg_info.get("version")}])
+    assert res.is_succeeded()
+    
+    # no-delete-method
+
+    def test_raise_err(env):
+        blade_api = init_api(env)
+        res = blade_api.blade_get_package({}, [])
+        assert isinstance(res.exception, JSONDecodeError)
+        try:
+            res.raise_for_err()
+        except JSONDecodeError:
+            return
+        assert False
+
+def test_raise_err2(env):
+    blade_api = init_api(env, False)
+    res = blade_api.blade_get_root_id()
+    assert res.exception is None
+    try:
+        res.raise_for_err()
+    except NotLoginError:
+        return
+    assert False
+
+
+def test_global_instance(env):
+    backend=BladeInstance.backend()
+    assert isinstance(backend, BladeAPI)
+    backend2=BladeInstance.backend()
+    assert backend2 == backend
```

### Comparing `arthub_api-1.6.1/tests/test_storage.py` & `arthub_api-1.6.3/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.1/tests/test_storage_blade.py` & `arthub_api-1.6.3/tests/test_storage_blade.py`

 * *Files identical despite different names*

