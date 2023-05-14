# Comparing `tmp/ensemblem-0.3.5.tar.gz` & `tmp/ensemblem-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemblem-0.3.5.tar", last modified: Sun May 14 22:03:14 2023, max compression
+gzip compressed data, was "ensemblem-0.4.tar", last modified: Sun May 14 22:17:16 2023, max compression
```

## Comparing `ensemblem-0.3.5.tar` & `ensemblem-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2023-05-14 22:03:14.839913 ensemblem-0.3.5/
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     1070 2023-02-17 20:16:36.000000 ensemblem-0.3.5/LICENSE
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3894 2023-05-14 22:03:14.839727 ensemblem-0.3.5/PKG-INFO
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3297 2023-02-17 20:16:36.000000 ensemblem-0.3.5/README.md
--rw-r--r--   0 ivanvigorito   (501) staff       (20)       38 2023-05-14 22:03:14.839982 ensemblem-0.3.5/setup.cfg
--rw-r--r--   0 ivanvigorito   (501) staff       (20)      860 2023-05-14 22:03:11.000000 ensemblem-0.3.5/setup.py
-drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2023-05-14 22:03:14.836241 ensemblem-0.3.5/src/
-drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2023-05-14 22:03:14.838433 ensemblem-0.3.5/src/ensemblem/
--rw-r--r--   0 ivanvigorito   (501) staff       (20)        0 2023-02-17 20:16:36.000000 ensemblem-0.3.5/src/ensemblem/__init__.py
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3037 2023-02-17 20:18:30.000000 ensemblem-0.3.5/src/ensemblem/metrics.py
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3794 2023-05-14 16:57:12.000000 ensemblem-0.3.5/src/ensemblem/model.py
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     1439 2023-03-09 23:53:00.000000 ensemblem-0.3.5/src/ensemblem/utils.py
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     2146 2023-02-17 20:18:30.000000 ensemblem-0.3.5/src/ensemblem/weights_functions.py
-drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2023-05-14 22:03:14.839479 ensemblem-0.3.5/src/ensemblem.egg-info/
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3894 2023-05-14 22:03:14.000000 ensemblem-0.3.5/src/ensemblem.egg-info/PKG-INFO
--rw-r--r--   0 ivanvigorito   (501) staff       (20)      306 2023-05-14 22:03:14.000000 ensemblem-0.3.5/src/ensemblem.egg-info/SOURCES.txt
--rw-r--r--   0 ivanvigorito   (501) staff       (20)        1 2023-05-14 22:03:14.000000 ensemblem-0.3.5/src/ensemblem.egg-info/dependency_links.txt
--rw-r--r--   0 ivanvigorito   (501) staff       (20)       10 2023-05-14 22:03:14.000000 ensemblem-0.3.5/src/ensemblem.egg-info/top_level.txt
+drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2023-05-14 22:17:16.171973 ensemblem-0.4/
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     1070 2023-02-17 20:16:36.000000 ensemblem-0.4/LICENSE
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3892 2023-05-14 22:17:16.171794 ensemblem-0.4/PKG-INFO
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3297 2023-02-17 20:16:36.000000 ensemblem-0.4/README.md
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)       38 2023-05-14 22:17:16.172033 ensemblem-0.4/setup.cfg
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)      858 2023-05-14 22:15:22.000000 ensemblem-0.4/setup.py
+drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2023-05-14 22:17:16.169205 ensemblem-0.4/src/
+drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2023-05-14 22:17:16.170911 ensemblem-0.4/src/ensemblem/
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)        0 2023-02-17 20:16:36.000000 ensemblem-0.4/src/ensemblem/__init__.py
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3037 2023-02-17 20:18:30.000000 ensemblem-0.4/src/ensemblem/metrics.py
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3796 2023-05-14 22:15:20.000000 ensemblem-0.4/src/ensemblem/model.py
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     1439 2023-03-09 23:53:00.000000 ensemblem-0.4/src/ensemblem/utils.py
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     2146 2023-02-17 20:18:30.000000 ensemblem-0.4/src/ensemblem/weights_functions.py
+drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2023-05-14 22:17:16.171556 ensemblem-0.4/src/ensemblem.egg-info/
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3892 2023-05-14 22:17:16.000000 ensemblem-0.4/src/ensemblem.egg-info/PKG-INFO
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)      306 2023-05-14 22:17:16.000000 ensemblem-0.4/src/ensemblem.egg-info/SOURCES.txt
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)        1 2023-05-14 22:17:16.000000 ensemblem-0.4/src/ensemblem.egg-info/dependency_links.txt
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)       10 2023-05-14 22:17:16.000000 ensemblem-0.4/src/ensemblem.egg-info/top_level.txt
```

### Comparing `ensemblem-0.3.5/LICENSE` & `ensemblem-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ensemblem-0.3.5/PKG-INFO` & `ensemblem-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensemblem
-Version: 0.3.5
+Version: 0.4
 Summary: Dynamic Weighted Ensemble - Local Fusion
 Home-page: https://github.com/IvanVigor/Dynamic-Weighted-Ensemble
 Author: Ivan Vigorito
 Author-email: ivanvigorit@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/IvanVigor/Local-Fusion-Dynamic-Weighted-Ensemble/issues
 Platform: UNKNOWN
```

### Comparing `ensemblem-0.3.5/README.md` & `ensemblem-0.4/README.md`

 * *Files identical despite different names*

### Comparing `ensemblem-0.3.5/setup.py` & `ensemblem-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ensemblem",
-    version="0.3.5",
+    version="0.4",
     author="Ivan Vigorito",
     author_email="ivanvigorit@gmail.com",
     description="Dynamic Weighted Ensemble - Local Fusion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IvanVigor/Dynamic-Weighted-Ensemble",
     project_urls={
```

### Comparing `ensemblem-0.3.5/src/ensemblem/metrics.py` & `ensemblem-0.4/src/ensemblem/metrics.py`

 * *Files identical despite different names*

### Comparing `ensemblem-0.3.5/src/ensemblem/model.py` & `ensemblem-0.4/src/ensemblem/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pandas
-from weights_functions import *
-from metrics import *
+from .weights_functions import *
+from .metrics import *
 from sklearn.preprocessing import MinMaxScaler
 from typing import List
 
 
 class KWEnsembler:
     """
     KWEnsembler class
```

### Comparing `ensemblem-0.3.5/src/ensemblem/utils.py` & `ensemblem-0.4/src/ensemblem/utils.py`

 * *Files identical despite different names*

### Comparing `ensemblem-0.3.5/src/ensemblem/weights_functions.py` & `ensemblem-0.4/src/ensemblem/weights_functions.py`

 * *Files identical despite different names*

### Comparing `ensemblem-0.3.5/src/ensemblem.egg-info/PKG-INFO` & `ensemblem-0.4/src/ensemblem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensemblem
-Version: 0.3.5
+Version: 0.4
 Summary: Dynamic Weighted Ensemble - Local Fusion
 Home-page: https://github.com/IvanVigor/Dynamic-Weighted-Ensemble
 Author: Ivan Vigorito
 Author-email: ivanvigorit@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/IvanVigor/Local-Fusion-Dynamic-Weighted-Ensemble/issues
 Platform: UNKNOWN
```

