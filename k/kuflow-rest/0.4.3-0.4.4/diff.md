# Comparing `tmp/kuflow_rest-0.4.3.tar.gz` & `tmp/kuflow_rest-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_rest-0.4.3.tar", max compression
+gzip compressed data, was "kuflow_rest-0.4.4.tar", max compression
```

## Comparing `kuflow_rest-0.4.3.tar` & `kuflow_rest-0.4.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      875 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/README.md
--rw-r--r--   0        0        0        6 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/VERSION
--rw-r--r--   0        0        0     1335 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/__init__.py
--rw-r--r--   0        0        0     1907 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/__init__.py
--rw-r--r--   0        0        0     7087 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/_client.py
--rw-r--r--   0        0        0     3983 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/_patch.py
--rw-r--r--   0        0        0    77869 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/_serialization.py
--rw-r--r--   0        0        0     1874 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/_vendor.py
--rw-r--r--   0        0        0     1517 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/_version.py
--rw-r--r--   0        0        0     1854 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/__init__.py
--rw-r--r--   0        0        0     7230 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/_client.py
--rw-r--r--   0        0        0     4026 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/_patch.py
--rw-r--r--   0        0        0     2060 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     7223 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_patch.py
--rw-r--r--   0        0        0     7842 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_principal_operations.py
--rw-r--r--   0        0        0    34839 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_process_operations.py
--rw-r--r--   0        0        0    51643 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_task_operations.py
--rw-r--r--   0        0        0     5191 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/models/__init__.py
--rw-r--r--   0        0        0     3294 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/models/_enums.py
--rw-r--r--   0        0        0    71240 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/models/_patch.py
--rw-r--r--   0        0        0     2060 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/operations/__init__.py
--rw-r--r--   0        0        0     7823 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_patch.py
--rw-r--r--   0        0        0     9752 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_principal_operations.py
--rw-r--r--   0        0        0    41609 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_process_operations.py
--rw-r--r--   0        0        0    62943 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_task_operations.py
--rw-r--r--   0        0        0       26 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_generated/py.typed
--rw-r--r--   0        0        0     7622 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/_kuflow_rest_client.py
--rw-r--r--   0        0        0     4336 2023-05-15 10:43:31.532858 kuflow_rest-0.4.3/kuflow_rest/models/__init__.py
--rw-r--r--   0        0        0     3383 2023-05-15 10:43:31.536858 kuflow_rest-0.4.3/kuflow_rest/models/_models.py
--rw-r--r--   0        0        0     1440 2023-05-15 10:43:31.536858 kuflow_rest-0.4.3/kuflow_rest/operations/__init__.py
--rw-r--r--   0        0        0     2501 2023-05-15 10:43:31.536858 kuflow_rest-0.4.3/kuflow_rest/operations/_authentication_operations.py
--rw-r--r--   0        0        0     4073 2023-05-15 10:43:31.536858 kuflow_rest-0.4.3/kuflow_rest/operations/_principal_operations.py
--rw-r--r--   0        0        0     9685 2023-05-15 10:43:31.536858 kuflow_rest-0.4.3/kuflow_rest/operations/_process_operations.py
--rw-r--r--   0        0        0    14938 2023-05-15 10:43:31.536858 kuflow_rest-0.4.3/kuflow_rest/operations/_task_operations.py
--rw-r--r--   0        0        0      756 2023-05-15 10:44:33.762183 kuflow_rest-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 kuflow_rest-0.4.3/setup.py
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-05-15 11:28:31.329286 kuflow_rest-0.4.4/README.md
+-rw-r--r--   0        0        0        6 2023-05-15 11:28:31.329286 kuflow_rest-0.4.4/VERSION
+-rw-r--r--   0        0        0     1335 2023-05-15 11:28:31.329286 kuflow_rest-0.4.4/kuflow_rest/__init__.py
+-rw-r--r--   0        0        0     1907 2023-05-15 11:28:31.329286 kuflow_rest-0.4.4/kuflow_rest/_generated/__init__.py
+-rw-r--r--   0        0        0     7087 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/_client.py
+-rw-r--r--   0        0        0     3983 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/_patch.py
+-rw-r--r--   0        0        0    77869 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/_serialization.py
+-rw-r--r--   0        0        0     1874 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/_vendor.py
+-rw-r--r--   0        0        0     1517 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/_version.py
+-rw-r--r--   0        0        0     1854 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/__init__.py
+-rw-r--r--   0        0        0     7230 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/_client.py
+-rw-r--r--   0        0        0     4026 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/_patch.py
+-rw-r--r--   0        0        0     2060 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0     7223 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     7842 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_principal_operations.py
+-rw-r--r--   0        0        0    34839 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_process_operations.py
+-rw-r--r--   0        0        0    51643 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_task_operations.py
+-rw-r--r--   0        0        0     5191 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/models/__init__.py
+-rw-r--r--   0        0        0     3294 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/models/_enums.py
+-rw-r--r--   0        0        0    71240 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/models/_patch.py
+-rw-r--r--   0        0        0     2060 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/operations/__init__.py
+-rw-r--r--   0        0        0     7823 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_patch.py
+-rw-r--r--   0        0        0     9752 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_principal_operations.py
+-rw-r--r--   0        0        0    41609 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_process_operations.py
+-rw-r--r--   0        0        0    62943 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_task_operations.py
+-rw-r--r--   0        0        0       26 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_generated/py.typed
+-rw-r--r--   0        0        0     7622 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/_kuflow_rest_client.py
+-rw-r--r--   0        0        0     4336 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/models/__init__.py
+-rw-r--r--   0        0        0     3383 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/models/_models.py
+-rw-r--r--   0        0        0     1440 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/operations/__init__.py
+-rw-r--r--   0        0        0     2501 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/operations/_authentication_operations.py
+-rw-r--r--   0        0        0     4073 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/operations/_principal_operations.py
+-rw-r--r--   0        0        0     9685 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/operations/_process_operations.py
+-rw-r--r--   0        0        0    14938 2023-05-15 11:28:31.333286 kuflow_rest-0.4.4/kuflow_rest/operations/_task_operations.py
+-rw-r--r--   0        0        0      756 2023-05-15 11:30:00.784991 kuflow_rest-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 kuflow_rest-0.4.4/setup.py
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.4.4/PKG-INFO
```

### Comparing `kuflow_rest-0.4.3/README.md` & `kuflow_rest-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/__init__.py` & `kuflow_rest-0.4.4/kuflow_rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from ._kuflow_rest_client import KuFlowRestClient
 from ._generated._serialization import Deserializer, Serializer, Model
 
 __all__ = ["Deserializer", "KuFlowRestClient", "Model", "Serializer"]
-__version__ = "0.4.3"
+__version__ = "0.4.4"
```

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/__init__.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/_client.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/_configuration.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/_patch.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/_serialization.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/_vendor.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/_version.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
 
-VERSION = "0.4.3"
+VERSION = "0.4.4"
```

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/__init__.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/_client.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/_configuration.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/_patch.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/__init__.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_authentication_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_patch.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_principal_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_process_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/aio/operations/_task_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/aio/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/models/__init__.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/models/_enums.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/models/_enums.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/models/_models.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/models/_patch.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/operations/__init__.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_authentication_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_patch.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_principal_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_process_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_generated/operations/_task_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/_generated/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/_kuflow_rest_client.py` & `kuflow_rest-0.4.4/kuflow_rest/_kuflow_rest_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/models/__init__.py` & `kuflow_rest-0.4.4/kuflow_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/models/_models.py` & `kuflow_rest-0.4.4/kuflow_rest/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/operations/__init__.py` & `kuflow_rest-0.4.4/kuflow_rest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/operations/_authentication_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/operations/_principal_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/operations/_process_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/kuflow_rest/operations/_task_operations.py` & `kuflow_rest-0.4.4/kuflow_rest/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.4.3/pyproject.toml` & `kuflow_rest-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-rest"
-version = "0.4.3"
+version = "0.4.4"
 description = "Client for KuFlow Rest Api"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
```

### Comparing `kuflow_rest-0.4.3/setup.py` & `kuflow_rest-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['azure-core>=1.26.3,<2.0.0', 'isodate>=0.6.1,<0.7.0']
 
 setup_kwargs = {
     'name': 'kuflow-rest',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'Client for KuFlow Rest Api',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n\n# KuFlow Rest\n\nThis is a client for the KuFlow API Rest that allows you to interact with our API in a comfortable way in the creation of your workers and tools.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_rest-0.4.3/PKG-INFO` & `kuflow_rest-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuflow-rest
-Version: 0.4.3
+Version: 0.4.4
 Summary: Client for KuFlow Rest Api
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

