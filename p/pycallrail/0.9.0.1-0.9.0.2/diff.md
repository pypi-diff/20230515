# Comparing `tmp/pycallrail-0.9.0.1.tar.gz` & `tmp/pycallrail-0.9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycallrail-0.9.0.1.tar", last modified: Mon May 15 07:19:38 2023, max compression
+gzip compressed data, was "pycallrail-0.9.0.2.tar", last modified: Mon May 15 17:09:09 2023, max compression
```

## Comparing `pycallrail-0.9.0.1.tar` & `pycallrail-0.9.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.863575 pycallrail-0.9.0.1/
--rw-rw-rw-   0        0        0     1100 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/LICENSE
--rw-rw-rw-   0        0        0       61 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3263 2023-05-15 07:19:38.862495 pycallrail-0.9.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.807327 pycallrail-0.9.0.1/pycallrail/
--rw-rw-rw-   0        0        0     1039 2023-05-15 07:19:22.000000 pycallrail-0.9.0.1/pycallrail/__init__.py
--rw-rw-rw-   0        0        0      251 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/base.py
--rw-rw-rw-   0        0        0    12252 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/callrail.py
--rw-rw-rw-   0        0        0      148 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/errors.py
--rw-rw-rw-   0        0        0      550 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/helpers.py
--rw-rw-rw-   0        0        0        0 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/mixins.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.841345 pycallrail-0.9.0.1/pycallrail/objects/
--rw-rw-rw-   0        0        0        0 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/__init__.py
--rw-rw-rw-   0        0        0    18844 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/accounts.py
--rw-rw-rw-   0        0        0     7114 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/calls.py
--rw-rw-rw-   0        0        0     3504 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/companies.py
--rw-rw-rw-   0        0        0     4271 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/form_submissions.py
--rw-rw-rw-   0        0        0     3487 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/tags.py
--rw-rw-rw-   0        0        0     3844 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pycallrail/objects/textmessages.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.827322 pycallrail-0.9.0.1/pycallrail.egg-info/
--rw-rw-rw-   0        0        0     3263 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      281 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 07:19:38.000000 pycallrail-0.9.0.1/pycallrail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       75 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 07:19:38.863575 pycallrail-0.9.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2667 2023-05-15 07:12:37.000000 pycallrail-0.9.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:19:38.861097 pycallrail-0.9.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-03-21 03:45:56.000000 pycallrail-0.9.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0       55 2023-05-04 01:12:26.000000 pycallrail-0.9.0.1/tests/cfg.py
--rw-rw-rw-   0        0        0    18215 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_account.py
--rw-rw-rw-   0        0        0     8894 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_apiclient.py
--rw-rw-rw-   0        0        0    18436 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_call.py
--rw-rw-rw-   0        0        0     5238 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_companies.py
--rw-rw-rw-   0        0        0    14850 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_formsubmissions.py
--rw-rw-rw-   0        0        0     2785 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_helpers.py
--rw-rw-rw-   0        0        0     3121 2023-05-04 14:18:45.000000 pycallrail-0.9.0.1/tests/test_integration.py
--rw-rw-rw-   0        0        0     4983 2023-05-04 14:18:46.000000 pycallrail-0.9.0.1/tests/test_tags.py
--rw-rw-rw-   0        0        0     8376 2023-05-04 14:18:46.000000 pycallrail-0.9.0.1/tests/test_textmessages.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:09:09.351887 pycallrail-0.9.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/LICENSE
+-rw-rw-rw-   0        0        0       61 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3263 2023-05-15 17:09:09.350887 pycallrail-0.9.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 17:09:09.040330 pycallrail-0.9.0.2/pycallrail/
+-rw-rw-rw-   0        0        0     1045 2023-05-15 17:07:51.000000 pycallrail-0.9.0.2/pycallrail/__init__.py
+-rw-rw-rw-   0        0        0      251 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/base.py
+-rw-rw-rw-   0        0        0    12252 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/callrail.py
+-rw-rw-rw-   0        0        0      148 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/errors.py
+-rw-rw-rw-   0        0        0      550 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/helpers.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/mixins.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:09:09.223086 pycallrail-0.9.0.2/pycallrail/objects/
+-rw-rw-rw-   0        0        0        0 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/objects/__init__.py
+-rw-rw-rw-   0        0        0    18844 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/objects/accounts.py
+-rw-rw-rw-   0        0        0     7114 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/objects/calls.py
+-rw-rw-rw-   0        0        0     3504 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/objects/companies.py
+-rw-rw-rw-   0        0        0     4271 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/objects/form_submissions.py
+-rw-rw-rw-   0        0        0     3487 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/objects/tags.py
+-rw-rw-rw-   0        0        0     3844 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pycallrail/objects/textmessages.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:09:09.098984 pycallrail-0.9.0.2/pycallrail.egg-info/
+-rw-rw-rw-   0        0        0     3263 2023-05-15 17:09:08.000000 pycallrail-0.9.0.2/pycallrail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-05-15 17:09:08.000000 pycallrail-0.9.0.2/pycallrail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 17:09:08.000000 pycallrail-0.9.0.2/pycallrail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      281 2023-05-15 17:09:08.000000 pycallrail-0.9.0.2/pycallrail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 17:09:08.000000 pycallrail-0.9.0.2/pycallrail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       75 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 17:09:09.351887 pycallrail-0.9.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2667 2023-05-15 07:12:37.000000 pycallrail-0.9.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:09:09.348888 pycallrail-0.9.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-21 03:45:56.000000 pycallrail-0.9.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-05-04 01:12:26.000000 pycallrail-0.9.0.2/tests/cfg.py
+-rw-rw-rw-   0        0        0    18215 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/tests/test_account.py
+-rw-rw-rw-   0        0        0     8894 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/tests/test_apiclient.py
+-rw-rw-rw-   0        0        0    18436 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/tests/test_call.py
+-rw-rw-rw-   0        0        0     5238 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/tests/test_companies.py
+-rw-rw-rw-   0        0        0    14850 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/tests/test_formsubmissions.py
+-rw-rw-rw-   0        0        0     2785 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     3121 2023-05-04 14:18:45.000000 pycallrail-0.9.0.2/tests/test_integration.py
+-rw-rw-rw-   0        0        0     4983 2023-05-04 14:18:46.000000 pycallrail-0.9.0.2/tests/test_tags.py
+-rw-rw-rw-   0        0        0     8376 2023-05-04 14:18:46.000000 pycallrail-0.9.0.2/tests/test_textmessages.py
```

### Comparing `pycallrail-0.9.0.1/LICENSE` & `pycallrail-0.9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/PKG-INFO` & `pycallrail-0.9.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycallrail
-Version: 0.9.0.1
+Version: 0.9.0.2
 Summary: An unofficial Python wrapper for the CallRail API
 Home-page: https://github.com/predictive-data-lab/pycallrail
 Author: Engineering @ Predictive Data Lab
 License: MIT
 Project-URL: Documentation, https://pycallrail.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/predictive-data-lab/pycallrail/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycallrail-0.9.0.1/README.rst` & `pycallrail-0.9.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail/__init__.py` & `pycallrail-0.9.0.2/pycallrail/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 """
 
 __title__ = 'pycallrail'
 __author__ = 'Engineering @ Predictive Data Lab'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 by Predictive Data Lab'
-__version__ = '0.9.0.1'
+__version__ = '0.9.0.2'
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple, Literal
 
-from callrail import *
-from base import *
-from errors import *
-from helpers import *
-from mixins import *
-from objects import *
+from .callrail import *
+from .base import *
+from .errors import *
+from .helpers import *
+from .mixins import *
+from .objects import *
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     revision: int
     build: int
     release: Literal['alpha', 'beta', 'rc', 'final']
```

### Comparing `pycallrail-0.9.0.1/pycallrail/callrail.py` & `pycallrail-0.9.0.2/pycallrail/callrail.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail/helpers.py` & `pycallrail-0.9.0.2/pycallrail/helpers.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail/objects/accounts.py` & `pycallrail-0.9.0.2/pycallrail/objects/accounts.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail/objects/calls.py` & `pycallrail-0.9.0.2/pycallrail/objects/calls.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail/objects/companies.py` & `pycallrail-0.9.0.2/pycallrail/objects/companies.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail/objects/form_submissions.py` & `pycallrail-0.9.0.2/pycallrail/objects/form_submissions.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail/objects/tags.py` & `pycallrail-0.9.0.2/pycallrail/objects/tags.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail/objects/textmessages.py` & `pycallrail-0.9.0.2/pycallrail/objects/textmessages.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/pycallrail.egg-info/PKG-INFO` & `pycallrail-0.9.0.2/pycallrail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycallrail
-Version: 0.9.0.1
+Version: 0.9.0.2
 Summary: An unofficial Python wrapper for the CallRail API
 Home-page: https://github.com/predictive-data-lab/pycallrail
 Author: Engineering @ Predictive Data Lab
 License: MIT
 Project-URL: Documentation, https://pycallrail.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/predictive-data-lab/pycallrail/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycallrail-0.9.0.1/pycallrail.egg-info/SOURCES.txt` & `pycallrail-0.9.0.2/pycallrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/setup.py` & `pycallrail-0.9.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_account.py` & `pycallrail-0.9.0.2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_apiclient.py` & `pycallrail-0.9.0.2/tests/test_apiclient.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_call.py` & `pycallrail-0.9.0.2/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_companies.py` & `pycallrail-0.9.0.2/tests/test_companies.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_formsubmissions.py` & `pycallrail-0.9.0.2/tests/test_formsubmissions.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_helpers.py` & `pycallrail-0.9.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_integration.py` & `pycallrail-0.9.0.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_tags.py` & `pycallrail-0.9.0.2/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.9.0.1/tests/test_textmessages.py` & `pycallrail-0.9.0.2/tests/test_textmessages.py`

 * *Files identical despite different names*

