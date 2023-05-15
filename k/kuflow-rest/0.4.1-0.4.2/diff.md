# Comparing `tmp/kuflow_rest-0.4.1.tar.gz` & `tmp/kuflow_rest-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_rest-0.4.1.tar", max compression
+gzip compressed data, was "kuflow_rest-0.4.2.tar", max compression
```

## Comparing `kuflow_rest-0.4.1.tar` & `kuflow_rest-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      875 2023-03-06 08:52:05.054863 kuflow_rest-0.4.1/README.md
--rw-r--r--   0        0        0        6 2023-03-06 08:52:05.054863 kuflow_rest-0.4.1/VERSION
--rw-r--r--   0        0        0     1335 2023-03-06 08:52:05.054863 kuflow_rest-0.4.1/kuflow_rest/__init__.py
--rw-r--r--   0        0        0     1907 2023-03-06 08:52:05.054863 kuflow_rest-0.4.1/kuflow_rest/_generated/__init__.py
--rw-r--r--   0        0        0     7087 2023-03-06 08:52:05.054863 kuflow_rest-0.4.1/kuflow_rest/_generated/_client.py
--rw-r--r--   0        0        0     3983 2023-03-06 08:52:05.054863 kuflow_rest-0.4.1/kuflow_rest/_generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/_patch.py
--rw-r--r--   0        0        0    77869 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/_serialization.py
--rw-r--r--   0        0        0     1874 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/_vendor.py
--rw-r--r--   0        0        0     1517 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/_version.py
--rw-r--r--   0        0        0     1854 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/__init__.py
--rw-r--r--   0        0        0     7230 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/_client.py
--rw-r--r--   0        0        0     4026 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/_patch.py
--rw-r--r--   0        0        0     2060 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     7223 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_patch.py
--rw-r--r--   0        0        0     7842 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_principal_operations.py
--rw-r--r--   0        0        0    34839 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_process_operations.py
--rw-r--r--   0        0        0    51643 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_task_operations.py
--rw-r--r--   0        0        0     5191 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/models/__init__.py
--rw-r--r--   0        0        0     3294 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/models/_enums.py
--rw-r--r--   0        0        0    71240 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/models/_patch.py
--rw-r--r--   0        0        0     2060 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/operations/__init__.py
--rw-r--r--   0        0        0     7823 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_patch.py
--rw-r--r--   0        0        0     9752 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_principal_operations.py
--rw-r--r--   0        0        0    41609 2023-03-06 08:52:05.058863 kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_process_operations.py
--rw-r--r--   0        0        0    62943 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_task_operations.py
--rw-r--r--   0        0        0       26 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/_generated/py.typed
--rw-r--r--   0        0        0     7545 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/_kuflow_rest_client.py
--rw-r--r--   0        0        0     4336 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/models/__init__.py
--rw-r--r--   0        0        0     3383 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/models/_models.py
--rw-r--r--   0        0        0     1440 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/operations/__init__.py
--rw-r--r--   0        0        0     2501 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/operations/_authentication_operations.py
--rw-r--r--   0        0        0     4073 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/operations/_principal_operations.py
--rw-r--r--   0        0        0     9685 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/operations/_process_operations.py
--rw-r--r--   0        0        0    14938 2023-03-06 08:52:05.062862 kuflow_rest-0.4.1/kuflow_rest/operations/_task_operations.py
--rw-r--r--   0        0        0      756 2023-03-06 08:53:12.921967 kuflow_rest-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 kuflow_rest-0.4.1/setup.py
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/README.md
+-rw-r--r--   0        0        0        6 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/VERSION
+-rw-r--r--   0        0        0     1335 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/__init__.py
+-rw-r--r--   0        0        0     1907 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/__init__.py
+-rw-r--r--   0        0        0     7087 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/_client.py
+-rw-r--r--   0        0        0     3983 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/_patch.py
+-rw-r--r--   0        0        0    77869 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/_serialization.py
+-rw-r--r--   0        0        0     1874 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/_vendor.py
+-rw-r--r--   0        0        0     1517 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/_version.py
+-rw-r--r--   0        0        0     1854 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/__init__.py
+-rw-r--r--   0        0        0     7230 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/_client.py
+-rw-r--r--   0        0        0     4026 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/_patch.py
+-rw-r--r--   0        0        0     2060 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0     7223 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     7842 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_principal_operations.py
+-rw-r--r--   0        0        0    34839 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_process_operations.py
+-rw-r--r--   0        0        0    51643 2023-03-22 13:32:42.991844 kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_task_operations.py
+-rw-r--r--   0        0        0     5191 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/models/__init__.py
+-rw-r--r--   0        0        0     3294 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/models/_enums.py
+-rw-r--r--   0        0        0    71240 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/models/_patch.py
+-rw-r--r--   0        0        0     2060 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/operations/__init__.py
+-rw-r--r--   0        0        0     7823 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_patch.py
+-rw-r--r--   0        0        0     9752 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_principal_operations.py
+-rw-r--r--   0        0        0    41609 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_process_operations.py
+-rw-r--r--   0        0        0    62943 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_task_operations.py
+-rw-r--r--   0        0        0       26 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_generated/py.typed
+-rw-r--r--   0        0        0     7622 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/_kuflow_rest_client.py
+-rw-r--r--   0        0        0     4336 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/models/__init__.py
+-rw-r--r--   0        0        0     3383 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/models/_models.py
+-rw-r--r--   0        0        0     1440 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/operations/__init__.py
+-rw-r--r--   0        0        0     2501 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/operations/_authentication_operations.py
+-rw-r--r--   0        0        0     4073 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/operations/_principal_operations.py
+-rw-r--r--   0        0        0     9685 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/operations/_process_operations.py
+-rw-r--r--   0        0        0    14938 2023-03-22 13:32:42.995844 kuflow_rest-0.4.2/kuflow_rest/operations/_task_operations.py
+-rw-r--r--   0        0        0      756 2023-03-22 13:33:49.711049 kuflow_rest-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 kuflow_rest-0.4.2/setup.py
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.4.2/PKG-INFO
```

### Comparing `kuflow_rest-0.4.1/README.md` & `kuflow_rest-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/__init__.py` & `kuflow_rest-0.4.2/kuflow_rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from ._kuflow_rest_client import KuFlowRestClient
 from ._generated._serialization import Deserializer, Serializer, Model
 
 __all__ = ["Deserializer", "KuFlowRestClient", "Model", "Serializer"]
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/__init__.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/_client.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/_configuration.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/_patch.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/_serialization.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/_vendor.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/_version.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
 
-VERSION = "0.4.1"
+VERSION = "0.4.2"
```

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/__init__.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/_client.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/_configuration.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/_patch.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/__init__.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_authentication_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_patch.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_principal_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_process_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/aio/operations/_task_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/aio/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/models/__init__.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/models/_enums.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/models/_enums.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/models/_models.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/models/_patch.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/operations/__init__.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_authentication_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_patch.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_principal_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_process_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_generated/operations/_task_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/_generated/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/_kuflow_rest_client.py` & `kuflow_rest-0.4.2/kuflow_rest/_kuflow_rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,18 +150,21 @@
     :paramtype allow_insecure_connection: bool
     """
 
     def __init__(
         self,
         client_id: str,
         client_secret: str,
-        endpoint: str = "https://api.kuflow.com/v2022-10-08",
-        allow_insecure_connection: bool = False,
+        endpoint: Optional[str] = None,
+        allow_insecure_connection: Optional[bool] = None,
         **kwargs: Any,
     ) -> None:
+        if endpoint is None:
+            endpoint = "https://api.kuflow.com/v2022-10-08"
+
         per_call_policies = []
         if allow_insecure_connection:
             per_call_policies.append(AllowHttpPolicy())
 
         if not endpoint.endswith("/" + KuFlowRestClient.API_VERSION):
             endpoint = endpoint + "/" + KuFlowRestClient.API_VERSION
```

### Comparing `kuflow_rest-0.4.1/kuflow_rest/models/__init__.py` & `kuflow_rest-0.4.2/kuflow_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/models/_models.py` & `kuflow_rest-0.4.2/kuflow_rest/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/operations/__init__.py` & `kuflow_rest-0.4.2/kuflow_rest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/operations/_authentication_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/operations/_principal_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/operations/_process_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/kuflow_rest/operations/_task_operations.py` & `kuflow_rest-0.4.2/kuflow_rest/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.1/pyproject.toml` & `kuflow_rest-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-rest"
-version = "0.4.1"
+version = "0.4.2"
 description = "Client for KuFlow Rest Api"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
```

### Comparing `kuflow_rest-0.4.1/setup.py` & `kuflow_rest-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['azure-core>=1.26.3,<2.0.0', 'isodate>=0.6.1,<0.7.0']
 
 setup_kwargs = {
     'name': 'kuflow-rest',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Client for KuFlow Rest Api',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n\n# KuFlow Rest\n\nThis is a client for the KuFlow API Rest that allows you to interact with our API in a comfortable way in the creation of your workers and tools.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_rest-0.4.1/PKG-INFO` & `kuflow_rest-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuflow-rest
-Version: 0.4.1
+Version: 0.4.2
 Summary: Client for KuFlow Rest Api
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

