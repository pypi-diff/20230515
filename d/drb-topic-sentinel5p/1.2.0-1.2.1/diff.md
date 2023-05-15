# Comparing `tmp/drb-topic-sentinel5p-1.2.0.tar.gz` & `tmp/drb-topic-sentinel5p-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-topic-sentinel5p-1.2.0.tar", last modified: Wed Mar 15 13:49:26 2023, max compression
+gzip compressed data, was "drb-topic-sentinel5p-1.2.1.tar", last modified: Mon May 15 11:56:15 2023, max compression
```

## Comparing `drb-topic-sentinel5p-1.2.0.tar` & `drb-topic-sentinel5p-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 15:37:30.000000 drb-topic-sentinel5p-1.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6053 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5522 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:49:26.946108 drb-topic-sentinel5p-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:49:26.946108 drb-topic-sentinel5p-1.2.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/auxiliary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/auxiliary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4864 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/auxiliary/cortex.yml
--rw-rw-rw-   0 root         (0) root         (0)     1279 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/level1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/level1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5155 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/level1/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/level2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/level2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5855 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/level2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6053 2023-03-15 13:49:26.000000 drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      699 2023-03-15 13:49:26.000000 drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 13:49:26.000000 drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      187 2023-03-15 13:49:26.000000 drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-15 13:49:26.000000 drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-15 13:49:26.000000 drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-01-03 11:10:29.000000 drb-topic-sentinel5p-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-03-15 13:49:26.954108 drb-topic-sentinel5p-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1528 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-01-03 11:10:29.000000 drb-topic-sentinel5p-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:56:15.157901 drb-topic-sentinel5p-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 15:37:30.000000 drb-topic-sentinel5p-1.2.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6053 2023-05-15 11:56:15.157901 drb-topic-sentinel5p-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5522 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:56:15.021898 drb-topic-sentinel5p-1.2.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:56:15.021898 drb-topic-sentinel5p-1.2.1/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:56:15.161901 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-15 11:56:15.161901 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:56:15.133900 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/auxiliary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/auxiliary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4864 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/auxiliary/cortex.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:56:15.145900 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/level1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/level1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5155 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/level1/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:56:15.153900 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/level2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/level2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5855 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/level2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 11:56:15.157901 drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6053 2023-05-15 11:56:14.000000 drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      699 2023-05-15 11:56:14.000000 drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 11:56:14.000000 drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-15 11:56:14.000000 drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-15 11:56:14.000000 drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-15 11:56:14.000000 drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-15 11:55:25.000000 drb-topic-sentinel5p-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-05-15 11:56:15.157901 drb-topic-sentinel5p-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2023-03-15 13:26:17.000000 drb-topic-sentinel5p-1.2.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-01-03 11:10:29.000000 drb-topic-sentinel5p-1.2.1/versioneer.py
```

### Comparing `drb-topic-sentinel5p-1.2.0/LICENCE.txt` & `drb-topic-sentinel5p-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel5p-1.2.0/PKG-INFO` & `drb-topic-sentinel5p-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel5p
-Version: 1.2.0
+Version: 1.2.1
 Summary: sentinel-5P topic for DRB Python
 Home-page: https://gitlab.com/drb-python/topics/sentinel5p
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-topic-sentinel5p-1.2.0/README.md` & `drb-topic-sentinel5p-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/auxiliary/cortex.yml` & `drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/auxiliary/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/cortex.yml` & `drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/level1/cortex.yml` & `drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/level1/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel5p-1.2.0/drb/topics/sentinel5p/level2/cortex.yml` & `drb-topic-sentinel5p-1.2.1/drb/topics/sentinel5p/level2/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/PKG-INFO` & `drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel5p
-Version: 1.2.0
+Version: 1.2.1
 Summary: sentinel-5P topic for DRB Python
 Home-page: https://gitlab.com/drb-python/topics/sentinel5p
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-topic-sentinel5p-1.2.0/drb_topic_sentinel5p.egg-info/SOURCES.txt` & `drb-topic-sentinel5p-1.2.1/drb_topic_sentinel5p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel5p-1.2.0/setup.py` & `drb-topic-sentinel5p-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel5p-1.2.0/versioneer.py` & `drb-topic-sentinel5p-1.2.1/versioneer.py`

 * *Files identical despite different names*

