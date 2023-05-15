# Comparing `tmp/hoppysearch-0.0.7.tar.gz` & `tmp/hoppysearch-0.0.8.tar.gz`

## Comparing `hoppysearch-0.0.7.tar` & `hoppysearch-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,25 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/.swagger-codegen-ignore
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/.travis.yml
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/a.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/requirements.txt
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/setup.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/test-requirements.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/tox.ini
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/.swagger-codegen/VERSION
--rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/docs/GeneralApi.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/__init__.py
--rw-r--r--   0        0        0    25919 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/api_client.py
--rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/configuration.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/dictToClass.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/hs_api.py
--rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/rest.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/api/__init__.py
--rw-r--r--   0        0        0    21714 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/api/general_api.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/src/hoppysearch/models/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/swagger_client/__init__.py
--rw-r--r--   0        0        0    25727 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/swagger_client/api_client.py
--rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/swagger_client/configuration.py
--rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/swagger_client/rest.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/swagger_client/api/__init__.py
--rw-r--r--   0        0        0    21651 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/swagger_client/api/general_api.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/swagger_client/models/__init__.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/test/__init__.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/test/test_general_api.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/LICENSE
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 hoppysearch-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/.swagger-codegen-ignore
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/.travis.yml
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/a.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/setup.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/test-requirements.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/tox.ini
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/docs/GeneralApi.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/__init__.py
+-rw-r--r--   0        0        0    25919 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/api_client.py
+-rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/configuration.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/dictToClass.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/hs_api.py
+-rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/rest.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/api/__init__.py
+-rw-r--r--   0        0        0    21714 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/api/general_api.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/src/hoppysearch/models/__init__.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/test/__init__.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/test/test_general_api.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/LICENSE
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/README.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 hoppysearch-0.0.8/PKG-INFO
```

### Comparing `hoppysearch-0.0.7/.swagger-codegen-ignore` & `hoppysearch-0.0.8/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/a.py` & `hoppysearch-0.0.8/a.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from src.hoppysearch.hs_api import HsApi
-from swagger_client.rest import ApiException
+from src.hoppysearch.rest import ApiException
 
 index_id ="lucene-serverless"
 api_key ="hs_f3vrd6tqwzcc01oh"
 hs = HsApi(index_id, api_key )
 
 
 # # index
```

### Comparing `hoppysearch-0.0.7/setup.py` & `hoppysearch-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/docs/GeneralApi.md` & `hoppysearch-0.0.8/docs/GeneralApi.md`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/src/hoppysearch/__init__.py` & `hoppysearch-0.0.8/src/hoppysearch/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 
 # from src.hoppysearch.api.general_api import GeneralApi
 # # import ApiClient
 # from src.hoppysearch.api_client import ApiClient
 # from src.hoppysearch.configuration import Configuration
 # # import models into sdk package
 
-from .hs_api import HsApi
+from .hs_api import HsApi
+from .rest import ApiException
```

### Comparing `hoppysearch-0.0.7/src/hoppysearch/api_client.py` & `hoppysearch-0.0.8/src/hoppysearch/api_client.py`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/src/hoppysearch/configuration.py` & `hoppysearch-0.0.8/src/hoppysearch/configuration.py`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/src/hoppysearch/hs_api.py` & `hoppysearch-0.0.8/src/hoppysearch/hs_api.py`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/src/hoppysearch/rest.py` & `hoppysearch-0.0.8/src/hoppysearch/rest.py`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/src/hoppysearch/api/general_api.py` & `hoppysearch-0.0.8/src/hoppysearch/api/general_api.py`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/test/test_general_api.py` & `hoppysearch-0.0.8/test/test_general_api.py`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/.gitignore` & `hoppysearch-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/LICENSE` & `hoppysearch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/README.md` & `hoppysearch-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hoppysearch-0.0.7/pyproject.toml` & `hoppysearch-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "hoppysearch"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Pragyan Satapathy", email="pragyan@hoppysoft.com" },
 ]
 description = "Hoppysearch Search JavaScript Client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hoppysearch-0.0.7/PKG-INFO` & `hoppysearch-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppysearch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Hoppysearch Search JavaScript Client
 Project-URL: Homepage, https://github.com/Hoppysoft-pvt/hoppysearch-python-client.git
 Author-email: Pragyan Satapathy <pragyan@hoppysoft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

