# Comparing `tmp/qcrepocleaner-1.4.tar.gz` & `tmp/qcrepocleaner-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcrepocleaner-1.4.tar", last modified: Wed Mar 22 13:07:42 2023, max compression
+gzip compressed data, was "qcrepocleaner-1.5.tar", last modified: Mon May 15 08:46:17 2023, max compression
```

## Comparing `qcrepocleaner-1.4.tar` & `qcrepocleaner-1.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-03-22 13:07:42.009527 qcrepocleaner-1.4/
--rw-r--r--   0 bvonhall   (502) staff       (20)     3807 2023-03-22 13:07:42.009182 qcrepocleaner-1.4/PKG-INFO
--rw-r--r--   0 bvonhall   (502) staff       (20)     3182 2023-03-17 13:45:20.000000 qcrepocleaner-1.4/README.md
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-03-22 13:07:41.997619 qcrepocleaner-1.4/qcrepocleaner/
--rw-r--r--   0 bvonhall   (502) staff       (20)    10133 2023-03-17 13:45:20.000000 qcrepocleaner-1.4/qcrepocleaner/Ccdb.py
--rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/__init__.py
--rw-r--r--   0 bvonhall   (502) staff       (20)      688 2023-03-22 10:52:32.000000 qcrepocleaner-1.4/qcrepocleaner/binUtils.py
--rwxr-xr-x   0 bvonhall   (502) staff       (20)    15361 2023-03-17 13:45:20.000000 qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-cleaner
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     4436 2023-03-22 10:52:32.000000 qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-delete-objects-in-runs
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     3234 2023-03-22 10:52:32.000000 qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-delete-time-interval
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     3080 2023-03-17 13:45:20.000000 qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-find-objects-not-updated
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     3368 2023-03-22 10:52:32.000000 qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-move-objects
--rw-r--r--   0 bvonhall   (502) staff       (20)     1249 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/pidfile.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1138 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/policies_utils.py
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-03-22 13:07:42.005460 qcrepocleaner-1.4/qcrepocleaner/rules/
--rw-r--r--   0 bvonhall   (502) staff       (20)     3397 2023-03-17 13:45:20.000000 qcrepocleaner-1.4/qcrepocleaner/rules/1_per_hour.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     5494 2023-03-17 13:45:20.000000 qcrepocleaner-1.4/qcrepocleaner/rules/1_per_run.py
--rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/rules/__init__.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     2739 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/rules/last_only.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     5950 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/rules/multiple_per_run.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     2282 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/rules/none_kept.py
--rw-r--r--   0 bvonhall   (502) staff       (20)      987 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/rules/plugin_template.py
--rw-r--r--   0 bvonhall   (502) staff       (20)    13102 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/rules/production.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1408 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/qcrepocleaner/rules/skip.py
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-03-22 13:07:42.001419 qcrepocleaner-1.4/qcrepocleaner.egg-info/
--rw-r--r--   0 bvonhall   (502) staff       (20)     3807 2023-03-22 13:07:41.000000 qcrepocleaner-1.4/qcrepocleaner.egg-info/PKG-INFO
--rw-r--r--   0 bvonhall   (502) staff       (20)     1044 2023-03-22 13:07:41.000000 qcrepocleaner-1.4/qcrepocleaner.egg-info/SOURCES.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)        1 2023-03-22 13:07:41.000000 qcrepocleaner-1.4/qcrepocleaner.egg-info/dependency_links.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)       55 2023-03-22 13:07:41.000000 qcrepocleaner-1.4/qcrepocleaner.egg-info/requires.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)       20 2023-03-22 13:07:41.000000 qcrepocleaner-1.4/qcrepocleaner.egg-info/top_level.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)       38 2023-03-22 13:07:42.009630 qcrepocleaner-1.4/setup.cfg
--rw-r--r--   0 bvonhall   (502) staff       (20)     1361 2023-03-22 13:02:53.000000 qcrepocleaner-1.4/setup.py
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-03-22 13:07:42.008636 qcrepocleaner-1.4/tests/
--rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/tests/__init__.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     4318 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/tests/test_1_per_hour.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     4173 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/tests/test_1_per_run.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1772 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/tests/test_Ccdb.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     8735 2023-03-22 13:02:34.000000 qcrepocleaner-1.4/tests/test_MultiplePerRun.py
--rw-r--r--   0 bvonhall   (502) staff       (20)    12389 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/tests/test_Production.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     3154 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/tests/test_last_only.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     2641 2023-03-17 13:01:58.000000 qcrepocleaner-1.4/tests/test_repoCleaner.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-05-15 08:46:17.216982 qcrepocleaner-1.5/
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3807 2023-05-15 08:46:17.215246 qcrepocleaner-1.5/PKG-INFO
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3182 2023-03-17 13:45:20.000000 qcrepocleaner-1.5/README.md
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-05-15 08:46:17.103279 qcrepocleaner-1.5/qcrepocleaner/
+-rw-r--r--   0 bvonhall   (502) staff       (20)    10002 2023-05-15 08:10:39.000000 qcrepocleaner-1.5/qcrepocleaner/Ccdb.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/__init__.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)      688 2023-05-15 08:10:36.000000 qcrepocleaner-1.5/qcrepocleaner/binUtils.py
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)    15361 2023-03-17 13:45:20.000000 qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-cleaner
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     3301 2023-05-15 08:10:36.000000 qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-delete-not-in-runs
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     4436 2023-03-22 10:52:32.000000 qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-delete-objects-in-runs
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     3234 2023-03-22 10:52:32.000000 qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-delete-time-interval
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     3080 2023-03-17 13:45:20.000000 qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-find-objects-not-updated
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     3368 2023-03-22 10:52:32.000000 qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-move-objects
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1249 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/pidfile.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1138 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/policies_utils.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-05-15 08:46:17.167446 qcrepocleaner-1.5/qcrepocleaner/rules/
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3397 2023-03-17 13:45:20.000000 qcrepocleaner-1.5/qcrepocleaner/rules/1_per_hour.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     5494 2023-03-17 13:45:20.000000 qcrepocleaner-1.5/qcrepocleaner/rules/1_per_run.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/rules/__init__.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     2739 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/rules/last_only.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     5950 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/rules/multiple_per_run.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     2282 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/rules/none_kept.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)      987 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/rules/plugin_template.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)    13102 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/rules/production.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1408 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/qcrepocleaner/rules/skip.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-05-15 08:46:17.113842 qcrepocleaner-1.5/qcrepocleaner.egg-info/
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3807 2023-05-15 08:46:16.000000 qcrepocleaner-1.5/qcrepocleaner.egg-info/PKG-INFO
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1088 2023-05-15 08:46:16.000000 qcrepocleaner-1.5/qcrepocleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)        1 2023-05-15 08:46:16.000000 qcrepocleaner-1.5/qcrepocleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)       55 2023-05-15 08:46:16.000000 qcrepocleaner-1.5/qcrepocleaner.egg-info/requires.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)       20 2023-05-15 08:46:16.000000 qcrepocleaner-1.5/qcrepocleaner.egg-info/top_level.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)       38 2023-05-15 08:46:17.217663 qcrepocleaner-1.5/setup.cfg
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1416 2023-05-15 08:45:07.000000 qcrepocleaner-1.5/setup.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-05-15 08:46:17.213225 qcrepocleaner-1.5/tests/
+-rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/tests/__init__.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     4318 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/tests/test_1_per_hour.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     4173 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/tests/test_1_per_run.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1772 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/tests/test_Ccdb.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     8735 2023-03-28 07:15:11.000000 qcrepocleaner-1.5/tests/test_MultiplePerRun.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)    12389 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/tests/test_Production.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3154 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/tests/test_last_only.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     2641 2023-03-17 13:01:58.000000 qcrepocleaner-1.5/tests/test_repoCleaner.py
```

### Comparing `qcrepocleaner-1.4/PKG-INFO` & `qcrepocleaner-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcrepocleaner
-Version: 1.4
+Version: 1.5
 Summary: Set of tools to clean up the QCDB repository.
 Home-page: https://gitlab.cern.ch/AliceO2Group/QualityControl/Framework/script/RepoCleaner
 Author: Barthelemy von Haller
 Author-email: bvonhall@cern.ch
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qcrepocleaner-1.4/README.md` & `qcrepocleaner-1.5/README.md`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/Ccdb.py` & `qcrepocleaner-1.5/qcrepocleaner/Ccdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,19 +78,16 @@
         r.raise_for_status()
         try:
             json = r.json()
         except json.decoder.JSONDecodeError as err:
             logger.error(f"JSON decode error: {err}")
             raise
         paths = []
-        logger.debug(f"json: {json}")
         for item in json['objects']:
             paths.append(item['path'])
-        logger.debug(type(json['objects']));
-        logger.debug(type(json['objects'][0]));
 
         return paths
 
     def getFullObjectsDetails(self, path: str = "") -> List[Dict]:
         '''
         Return the full json of all the objects found in the path.
         :param path:
```

### Comparing `qcrepocleaner-1.4/qcrepocleaner/binUtils.py` & `qcrepocleaner-1.5/qcrepocleaner/binUtils.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-cleaner` & `qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-cleaner`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-delete-objects-in-runs` & `qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-delete-objects-in-runs`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-delete-time-interval` & `qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-delete-time-interval`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-find-objects-not-updated` & `qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-find-objects-not-updated`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/o2-qc-repo-move-objects` & `qcrepocleaner-1.5/qcrepocleaner/o2-qc-repo-move-objects`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/pidfile.py` & `qcrepocleaner-1.5/qcrepocleaner/pidfile.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/policies_utils.py` & `qcrepocleaner-1.5/qcrepocleaner/policies_utils.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/rules/1_per_hour.py` & `qcrepocleaner-1.5/qcrepocleaner/rules/1_per_hour.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/rules/1_per_run.py` & `qcrepocleaner-1.5/qcrepocleaner/rules/1_per_run.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/rules/last_only.py` & `qcrepocleaner-1.5/qcrepocleaner/rules/last_only.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/rules/multiple_per_run.py` & `qcrepocleaner-1.5/qcrepocleaner/rules/multiple_per_run.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/rules/none_kept.py` & `qcrepocleaner-1.5/qcrepocleaner/rules/none_kept.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/rules/plugin_template.py` & `qcrepocleaner-1.5/qcrepocleaner/rules/plugin_template.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/rules/production.py` & `qcrepocleaner-1.5/qcrepocleaner/rules/production.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner/rules/skip.py` & `qcrepocleaner-1.5/qcrepocleaner/rules/skip.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/qcrepocleaner.egg-info/PKG-INFO` & `qcrepocleaner-1.5/qcrepocleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcrepocleaner
-Version: 1.4
+Version: 1.5
 Summary: Set of tools to clean up the QCDB repository.
 Home-page: https://gitlab.cern.ch/AliceO2Group/QualityControl/Framework/script/RepoCleaner
 Author: Barthelemy von Haller
 Author-email: bvonhall@cern.ch
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qcrepocleaner-1.4/qcrepocleaner.egg-info/SOURCES.txt` & `qcrepocleaner-1.5/qcrepocleaner.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 qcrepocleaner/Ccdb.py
 qcrepocleaner/__init__.py
 qcrepocleaner/binUtils.py
 qcrepocleaner/o2-qc-repo-cleaner
+qcrepocleaner/o2-qc-repo-delete-not-in-runs
 qcrepocleaner/o2-qc-repo-delete-objects-in-runs
 qcrepocleaner/o2-qc-repo-delete-time-interval
 qcrepocleaner/o2-qc-repo-find-objects-not-updated
 qcrepocleaner/o2-qc-repo-move-objects
 qcrepocleaner/pidfile.py
 qcrepocleaner/policies_utils.py
 qcrepocleaner.egg-info/PKG-INFO
```

### Comparing `qcrepocleaner-1.4/setup.py` & `qcrepocleaner-1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='qcrepocleaner',
-    version='1.4',
+    version='1.5',
     author='Barthelemy von Haller',
     author_email='bvonhall@cern.ch',
     url='https://gitlab.cern.ch/AliceO2Group/QualityControl/Framework/script/RepoCleaner',
     license='GPLv3',
     description='Set of tools to clean up the QCDB repository.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -23,14 +23,15 @@
         'Development Status :: 5 - Production/Stable'
     ],
     python_requires='>=3.6',
     install_requires=['requests', 'dryable', 'responses', 'PyYAML', 'python-consul', 'psutil'],
     scripts=[
         'qcrepocleaner/o2-qc-repo-cleaner',
         'qcrepocleaner/o2-qc-repo-delete-objects-in-runs',
+        'qcrepocleaner/o2-qc-repo-delete-not-in-runs',
         'qcrepocleaner/o2-qc-repo-delete-time-interval',
         'qcrepocleaner/o2-qc-repo-find-objects-not-updated',
         'qcrepocleaner/o2-qc-repo-move-objects'],
     include_package_data=True,
     package_data={
         'qcrepocleaner': ['qcrepocleaner/config.yaml']
     }
```

### Comparing `qcrepocleaner-1.4/tests/test_1_per_hour.py` & `qcrepocleaner-1.5/tests/test_1_per_hour.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/tests/test_1_per_run.py` & `qcrepocleaner-1.5/tests/test_1_per_run.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/tests/test_Ccdb.py` & `qcrepocleaner-1.5/tests/test_Ccdb.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/tests/test_MultiplePerRun.py` & `qcrepocleaner-1.5/tests/test_MultiplePerRun.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/tests/test_Production.py` & `qcrepocleaner-1.5/tests/test_Production.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/tests/test_last_only.py` & `qcrepocleaner-1.5/tests/test_last_only.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.4/tests/test_repoCleaner.py` & `qcrepocleaner-1.5/tests/test_repoCleaner.py`

 * *Files identical despite different names*

