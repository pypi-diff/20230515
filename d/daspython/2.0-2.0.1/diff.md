# Comparing `tmp/daspython-2.0.tar.gz` & `tmp/daspython-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daspython-2.0.tar", last modified: Fri May 12 15:45:30 2023, max compression
+gzip compressed data, was "daspython-2.0.1.tar", last modified: Mon May 15 10:30:17 2023, max compression
```

## Comparing `daspython-2.0.tar` & `daspython-2.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.687981 daspython-2.0/
--rw-rw-rw-   0        0        0    35821 2023-03-29 09:37:21.000000 daspython-2.0/LICENSE
--rw-rw-rw-   0        0        0     2183 2023-05-12 15:45:30.686990 daspython-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1659 2023-03-29 15:15:01.000000 daspython-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.565903 daspython-2.0/daspython/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.632070 daspython-2.0/daspython/auth/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/auth/__init__.py
--rw-rw-rw-   0        0        0     1969 2023-05-11 16:36:35.000000 daspython-2.0/daspython/auth/authenticate.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.636084 daspython-2.0/daspython/client/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:25:32.000000 daspython-2.0/daspython/client/__init__.py
--rw-rw-rw-   0        0        0     1001 2023-04-06 09:00:06.000000 daspython-2.0/daspython/client/client.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.640517 daspython-2.0/daspython/common/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/common/__init__.py
--rw-rw-rw-   0        0        0     5566 2023-05-11 16:05:46.000000 daspython-2.0/daspython/common/api.py
--rw-rw-rw-   0        0        0      110 2023-03-29 09:37:21.000000 daspython-2.0/daspython/common/response.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.646054 daspython-2.0/daspython/dastypes/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:20:32.000000 daspython-2.0/daspython/dastypes/__init__.py
--rw-rw-rw-   0        0        0       30 2023-04-06 08:46:36.000000 daspython-2.0/daspython/dastypes/entry.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.648052 daspython-2.0/daspython/services/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.651060 daspython-2.0/daspython/services/alcs/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/alcs/__init__.py
--rw-rw-rw-   0        0        0      500 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/alcs/aclservice.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.654205 daspython-2.0/daspython/services/attributes/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/attributes/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/attributes/attributeservice.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.656468 daspython-2.0/daspython/services/digitalobjects/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/digitalobjects/__init__.py
--rw-rw-rw-   0        0        0    11310 2023-05-12 15:33:43.000000 daspython-2.0/daspython/services/digitalobjects/digitalobjectservice.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.660480 daspython-2.0/daspython/services/entries/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/entries/__init__.py
--rw-rw-rw-   0        0        0    17184 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/entries/entryservice.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.666015 daspython-2.0/daspython/services/entryfields/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/entryfields/__init__.py
--rw-rw-rw-   0        0        0      722 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/entryfields/entryfieldservice.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.669013 daspython-2.0/daspython/services/searches/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/searches/__init__.py
--rw-rw-rw-   0        0        0     1960 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/searches/searchservice.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.629565 daspython-2.0/daspython.egg-info/
--rw-rw-rw-   0        0        0     2183 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      841 2023-05-12 15:40:43.000000 daspython-2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 15:45:30.688981 daspython-2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.684970 daspython-2.0/tests/
--rw-rw-rw-   0        0        0     1033 2023-05-11 16:51:54.000000 daspython-2.0/tests/test_aclservice.py
--rw-rw-rw-   0        0        0     1187 2023-05-11 16:47:49.000000 daspython-2.0/tests/test_attributeservice.py
--rw-rw-rw-   0        0        0      526 2023-05-11 16:47:21.000000 daspython-2.0/tests/test_authenticate.py
--rw-rw-rw-   0        0        0      700 2023-04-06 09:25:24.000000 daspython-2.0/tests/test_dasclient.py
--rw-rw-rw-   0        0        0     2489 2023-05-12 15:34:51.000000 daspython-2.0/tests/test_digital_object_service.py
--rw-rw-rw-   0        0        0      861 2023-05-11 16:47:43.000000 daspython-2.0/tests/test_entry_field_service.py
--rw-rw-rw-   0        0        0     7078 2023-05-11 16:47:47.000000 daspython-2.0/tests/test_entry_service.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.616558 daspython-2.0.1/
+-rw-rw-rw-   0        0        0    35821 2023-03-29 09:37:21.000000 daspython-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2185 2023-05-15 10:30:17.615558 daspython-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1659 2023-03-29 15:15:01.000000 daspython-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.500448 daspython-2.0.1/daspython/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.557777 daspython-2.0.1/daspython/auth/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/auth/__init__.py
+-rw-rw-rw-   0        0        0     1971 2023-05-15 10:28:47.000000 daspython-2.0.1/daspython/auth/authenticate.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.562299 daspython-2.0.1/daspython/client/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:25:32.000000 daspython-2.0.1/daspython/client/__init__.py
+-rw-rw-rw-   0        0        0     1001 2023-04-06 09:00:06.000000 daspython-2.0.1/daspython/client/client.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.570299 daspython-2.0.1/daspython/common/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/common/__init__.py
+-rw-rw-rw-   0        0        0     5566 2023-05-11 16:05:46.000000 daspython-2.0.1/daspython/common/api.py
+-rw-rw-rw-   0        0        0      110 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/common/response.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.575601 daspython-2.0.1/daspython/dastypes/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:20:32.000000 daspython-2.0.1/daspython/dastypes/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-04-06 08:46:36.000000 daspython-2.0.1/daspython/dastypes/entry.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.577577 daspython-2.0.1/daspython/services/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.580578 daspython-2.0.1/daspython/services/alcs/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/alcs/__init__.py
+-rw-rw-rw-   0        0        0      500 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/alcs/aclservice.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.583976 daspython-2.0.1/daspython/services/attributes/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/attributes/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/attributes/attributeservice.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.587975 daspython-2.0.1/daspython/services/digitalobjects/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/digitalobjects/__init__.py
+-rw-rw-rw-   0        0        0    11310 2023-05-12 15:33:43.000000 daspython-2.0.1/daspython/services/digitalobjects/digitalobjectservice.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.590488 daspython-2.0.1/daspython/services/entries/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/entries/__init__.py
+-rw-rw-rw-   0        0        0    17184 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/entries/entryservice.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.593500 daspython-2.0.1/daspython/services/entryfields/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/entryfields/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/entryfields/entryfieldservice.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.597504 daspython-2.0.1/daspython/services/searches/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/searches/__init__.py
+-rw-rw-rw-   0        0        0     1960 2023-03-29 09:37:21.000000 daspython-2.0.1/daspython/services/searches/searchservice.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.552775 daspython-2.0.1/daspython.egg-info/
+-rw-rw-rw-   0        0        0     2185 2023-05-15 10:30:17.000000 daspython-2.0.1/daspython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2023-05-15 10:30:17.000000 daspython-2.0.1/daspython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 10:30:17.000000 daspython-2.0.1/daspython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-05-15 10:30:17.000000 daspython-2.0.1/daspython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 10:30:17.000000 daspython-2.0.1/daspython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      844 2023-05-15 10:26:26.000000 daspython-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 10:30:17.616558 daspython-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 10:30:17.613559 daspython-2.0.1/tests/
+-rw-rw-rw-   0        0        0     1033 2023-05-11 16:51:54.000000 daspython-2.0.1/tests/test_aclservice.py
+-rw-rw-rw-   0        0        0     1187 2023-05-11 16:47:49.000000 daspython-2.0.1/tests/test_attributeservice.py
+-rw-rw-rw-   0        0        0      526 2023-05-11 16:47:21.000000 daspython-2.0.1/tests/test_authenticate.py
+-rw-rw-rw-   0        0        0      700 2023-04-06 09:25:24.000000 daspython-2.0.1/tests/test_dasclient.py
+-rw-rw-rw-   0        0        0     2489 2023-05-12 15:34:51.000000 daspython-2.0.1/tests/test_digital_object_service.py
+-rw-rw-rw-   0        0        0      861 2023-05-11 16:47:43.000000 daspython-2.0.1/tests/test_entry_field_service.py
+-rw-rw-rw-   0        0        0     7078 2023-05-11 16:47:47.000000 daspython-2.0.1/tests/test_entry_service.py
```

### Comparing `daspython-2.0/LICENSE` & `daspython-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daspython-2.0/PKG-INFO` & `daspython-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daspython
-Version: 2.0
+Version: 2.0.1
 Summary: DAS api client.
 Author: Royal Netherlands Institute for Sea Research
 Project-URL: Homepage, https://git.nioz.nl/ict-projects/das-python
 Project-URL: Bug Tracker, https://git.nioz.nl/ict-projects/das-python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `daspython-2.0/README.md` & `daspython-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `daspython-2.0/daspython/auth/authenticate.py` & `daspython-2.0.1/daspython/auth/authenticate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import json
 import requests
-from common.api import Token
+from ..common.api import Token
 
 class DasAuth(Token):
     '''This object represents the authenticator to the DAS API and keeps your token.'''
 
     def __init__(self, base_url, username, password):
         '''
         Parameters
```

### Comparing `daspython-2.0/daspython/client/client.py` & `daspython-2.0.1/daspython/client/client.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/daspython/common/api.py` & `daspython-2.0.1/daspython/common/api.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/daspython/services/attributes/attributeservice.py` & `daspython-2.0.1/daspython/services/attributes/attributeservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/daspython/services/digitalobjects/digitalobjectservice.py` & `daspython-2.0.1/daspython/services/digitalobjects/digitalobjectservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/daspython/services/entries/entryservice.py` & `daspython-2.0.1/daspython/services/entries/entryservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/daspython/services/entryfields/entryfieldservice.py` & `daspython-2.0.1/daspython/services/entryfields/entryfieldservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/daspython/services/searches/searchservice.py` & `daspython-2.0.1/daspython/services/searches/searchservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/daspython.egg-info/PKG-INFO` & `daspython-2.0.1/daspython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daspython
-Version: 2.0
+Version: 2.0.1
 Summary: DAS api client.
 Author: Royal Netherlands Institute for Sea Research
 Project-URL: Homepage, https://git.nioz.nl/ict-projects/das-python
 Project-URL: Bug Tracker, https://git.nioz.nl/ict-projects/das-python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `daspython-2.0/daspython.egg-info/SOURCES.txt` & `daspython-2.0.1/daspython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daspython-2.0/pyproject.toml` & `daspython-2.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "daspython"
-version = "2.0"
+version = "2.0.01"
 authors = [
   { name="Royal Netherlands Institute for Sea Research" },
 ]
 description = "DAS api client."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `daspython-2.0/tests/test_aclservice.py` & `daspython-2.0.1/tests/test_aclservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/tests/test_attributeservice.py` & `daspython-2.0.1/tests/test_attributeservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/tests/test_authenticate.py` & `daspython-2.0.1/tests/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/tests/test_dasclient.py` & `daspython-2.0.1/tests/test_dasclient.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/tests/test_digital_object_service.py` & `daspython-2.0.1/tests/test_digital_object_service.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/tests/test_entry_field_service.py` & `daspython-2.0.1/tests/test_entry_field_service.py`

 * *Files identical despite different names*

### Comparing `daspython-2.0/tests/test_entry_service.py` & `daspython-2.0.1/tests/test_entry_service.py`

 * *Files identical despite different names*

