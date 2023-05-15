# Comparing `tmp/drb-topic-safe-1.1.0.tar.gz` & `tmp/drb-topic-safe-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-topic-safe-1.1.0.tar", last modified: Tue Jan  3 09:45:30 2023, max compression
+gzip compressed data, was "drb-topic-safe-1.2.0.tar", last modified: Mon May 15 13:53:50 2023, max compression
```

## Comparing `drb-topic-safe-1.1.0.tar` & `drb-topic-safe-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:45:30.763933 drb-topic-safe-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-01-03 09:31:55.000000 drb-topic-safe-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      989 2023-01-03 09:45:30.763933 drb-topic-safe-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-01-02 17:30:23.000000 drb-topic-safe-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:45:30.755932 drb-topic-safe-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:45:30.755932 drb-topic-safe-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:45:30.763933 drb-topic-safe-1.1.0/drb/topics/safe/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-01-02 17:30:23.000000 drb-topic-safe-1.1.0/drb/topics/safe/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-03 09:45:30.763933 drb-topic-safe-1.1.0/drb/topics/safe/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-01-02 17:30:23.000000 drb-topic-safe-1.1.0/drb/topics/safe/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 09:45:30.763933 drb-topic-safe-1.1.0/drb_topic_safe.egg-info/
--rw-r--r--   0 root         (0) root         (0)      989 2023-01-03 09:45:30.000000 drb-topic-safe-1.1.0/drb_topic_safe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-01-03 09:45:30.000000 drb-topic-safe-1.1.0/drb_topic_safe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 09:45:30.000000 drb-topic-safe-1.1.0/drb_topic_safe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-01-03 09:45:30.000000 drb-topic-safe-1.1.0/drb_topic_safe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-01-03 09:45:30.000000 drb-topic-safe-1.1.0/drb_topic_safe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-03 09:45:30.000000 drb-topic-safe-1.1.0/drb_topic_safe.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-01-03 09:31:55.000000 drb-topic-safe-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-01-03 09:45:30.763933 drb-topic-safe-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1060 2023-01-03 09:31:55.000000 drb-topic-safe-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2023-01-02 17:30:23.000000 drb-topic-safe-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:53:50.518031 drb-topic-safe-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 14:19:08.000000 drb-topic-safe-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-01-03 09:31:55.000000 drb-topic-safe-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-15 13:53:50.518031 drb-topic-safe-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-01-02 17:30:23.000000 drb-topic-safe-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:53:50.506030 drb-topic-safe-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:53:50.506030 drb-topic-safe-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:53:50.518031 drb-topic-safe-1.2.0/drb/topics/safe/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-01-02 17:30:23.000000 drb-topic-safe-1.2.0/drb/topics/safe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-15 13:53:50.518031 drb-topic-safe-1.2.0/drb/topics/safe/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-05-15 13:53:16.000000 drb-topic-safe-1.2.0/drb/topics/safe/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:53:50.518031 drb-topic-safe-1.2.0/drb_topic_safe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-15 13:53:50.000000 drb-topic-safe-1.2.0/drb_topic_safe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-05-15 13:53:50.000000 drb-topic-safe-1.2.0/drb_topic_safe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 13:53:50.000000 drb-topic-safe-1.2.0/drb_topic_safe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-15 13:53:50.000000 drb-topic-safe-1.2.0/drb_topic_safe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 13:53:50.000000 drb-topic-safe-1.2.0/drb_topic_safe.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-15 13:53:50.000000 drb-topic-safe-1.2.0/drb_topic_safe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-15 13:53:50.000000 drb-topic-safe-1.2.0/drb_topic_safe.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-15 13:37:00.000000 drb-topic-safe-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-11 15:23:39.000000 drb-topic-safe-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-15 13:53:50.518031 drb-topic-safe-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-15 12:59:09.000000 drb-topic-safe-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:53:50.518031 drb-topic-safe-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-05-11 15:23:39.000000 drb-topic-safe-1.2.0/tests/test_topic.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2023-01-02 17:30:23.000000 drb-topic-safe-1.2.0/versioneer.py
```

### Comparing `drb-topic-safe-1.1.0/PKG-INFO` & `drb-topic-safe-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: drb-topic-safe
-Version: 1.1.0
+Version: 1.2.0
 Summary: Safe topic for DRB Python
 Home-page: https://gitlab.com/drb-python/topics/safe
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # drb-topic-safe
 The DRB plugin `drb-topic-safe` declare topics about *Standard Archive Format 
 for Europe* ([**SAFE**](https://sentinels.copernicus.eu/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification))
 format specification.
 
 
@@ -29,9 +29,7 @@
 
 ```mermaid
 graph TB
     A([SAFE Product<br/>487b0c70-6199-46de-9e41-4914520e25d9])
     B([SAFE Manifest<br/>3289b9eb-4c8e-4d3b-8e37-8eeb843941f5])
 ```
 
-
-
```

### Comparing `drb-topic-safe-1.1.0/README.md` & `drb-topic-safe-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-topic-safe-1.1.0/drb_topic_safe.egg-info/PKG-INFO` & `drb-topic-safe-1.2.0/drb_topic_safe.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: drb-topic-safe
-Version: 1.1.0
+Version: 1.2.0
 Summary: Safe topic for DRB Python
 Home-page: https://gitlab.com/drb-python/topics/safe
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # drb-topic-safe
 The DRB plugin `drb-topic-safe` declare topics about *Standard Archive Format 
 for Europe* ([**SAFE**](https://sentinels.copernicus.eu/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification))
 format specification.
 
 
@@ -29,9 +29,7 @@
 
 ```mermaid
 graph TB
     A([SAFE Product<br/>487b0c70-6199-46de-9e41-4914520e25d9])
     B([SAFE Manifest<br/>3289b9eb-4c8e-4d3b-8e37-8eeb843941f5])
 ```
 
-
-
```

### Comparing `drb-topic-safe-1.1.0/versioneer.py` & `drb-topic-safe-1.2.0/versioneer.py`

 * *Files identical despite different names*

