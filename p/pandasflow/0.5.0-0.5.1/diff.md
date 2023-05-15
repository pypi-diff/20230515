# Comparing `tmp/pandasflow-0.5.0.tar.gz` & `tmp/pandasflow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.5.0.tar", last modified: Tue May  9 15:34:30 2023, max compression
+gzip compressed data, was "pandasflow-0.5.1.tar", last modified: Mon May 15 09:14:12 2023, max compression
```

## Comparing `pandasflow-0.5.0.tar` & `pandasflow-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.021614 pandasflow-0.5.0/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.0/LICENCE
--rw-rw-rw-   0        0        0      694 2023-05-09 15:34:30.021614 pandasflow-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.002664 pandasflow-0.5.0/pandasflow/
--rw-rw-rw-   0        0        0      346 2023-05-09 15:34:20.000000 pandasflow-0.5.0/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.006654 pandasflow-0.5.0/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.0/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.0/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.0/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      206 2023-05-09 15:33:32.000000 pandasflow-0.5.0/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.011641 pandasflow-0.5.0/pandasflow/metrics/
--rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.0/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.0/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.0/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.5.0/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.0/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.0/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.0/pandasflow/metrics/roc.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.012637 pandasflow-0.5.0/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.0/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.0/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.012637 pandasflow-0.5.0/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.0/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.014632 pandasflow-0.5.0/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.0/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3016 2023-05-04 13:48:42.000000 pandasflow-0.5.0/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3719 2023-05-04 13:48:33.000000 pandasflow-0.5.0/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.005655 pandasflow-0.5.0/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      935 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 15:34:30.021614 pandasflow-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.020620 pandasflow-0.5.0/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.0/test/__init__.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.0/test/best_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.0/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.5.0/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.0/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.0/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.0/test/roc_test.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.5.0/test/split_tt_test.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.5.0/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.858849 pandasflow-0.5.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.1/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-05-15 09:14:12.858849 pandasflow-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.835956 pandasflow-0.5.1/pandasflow/
+-rw-rw-rw-   0        0        0      391 2023-05-15 09:13:53.000000 pandasflow-0.5.1/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.839947 pandasflow-0.5.1/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.1/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.1/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.1/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.1/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      206 2023-05-09 15:33:32.000000 pandasflow-0.5.1/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.846995 pandasflow-0.5.1/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.1/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.1/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.1/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.5.1/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.1/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.1/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.1/pandasflow/metrics/roc.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.847570 pandasflow-0.5.1/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.1/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.1/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.848561 pandasflow-0.5.1/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.1/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.849770 pandasflow-0.5.1/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.1/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3016 2023-05-04 13:48:42.000000 pandasflow-0.5.1/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3719 2023-05-04 13:48:33.000000 pandasflow-0.5.1/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.838950 pandasflow-0.5.1/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 09:14:12.859834 pandasflow-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.857839 pandasflow-0.5.1/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.1/test/__init__.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.1/test/best_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.1/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.5.1/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.1/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.1/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.1/test/roc_test.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.5.1/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.5.1/test/split_tvt_test.py
```

### Comparing `pandasflow-0.5.0/LICENCE` & `pandasflow-0.5.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/PKG-INFO` & `pandasflow-0.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.0
+Version: 0.5.1
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.0/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.5.1/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow/metrics/best_f1.py` & `pandasflow-0.5.1/pandasflow/metrics/best_f1.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow/metrics/conf_mat.py` & `pandasflow-0.5.1/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow/metrics/lloss_up.py` & `pandasflow-0.5.1/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow/metrics/precision_recall.py` & `pandasflow-0.5.1/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow/metrics/roc.py` & `pandasflow-0.5.1/pandasflow/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow/reset_mi.py` & `pandasflow-0.5.1/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow/split/train_test.py` & `pandasflow-0.5.1/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow/split/train_valid_test.py` & `pandasflow-0.5.1/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.5.1/pandasflow.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.0
+Version: 0.5.1
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.0/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.5.1/pandasflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENCE
 README.md
 setup.cfg
 setup.py
 pandasflow/__init__.py
 pandasflow/get_import.py
+pandasflow/get_psql.py
 pandasflow/get_sqlt.py
 pandasflow/reset_mi.py
 pandasflow.egg-info/PKG-INFO
 pandasflow.egg-info/SOURCES.txt
 pandasflow.egg-info/dependency_links.txt
 pandasflow.egg-info/requires.txt
 pandasflow.egg-info/top_level.txt
```

### Comparing `pandasflow-0.5.0/setup.py` & `pandasflow-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/test/best_f1_test.py` & `pandasflow-0.5.1/test/best_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/test/conf_mat_test.py` & `pandasflow-0.5.1/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/test/lloss_up_test.py` & `pandasflow-0.5.1/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/test/precision_recall_test.py` & `pandasflow-0.5.1/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/test/roc_test.py` & `pandasflow-0.5.1/test/roc_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.0/test/split_tvt_test.py` & `pandasflow-0.5.1/test/split_tvt_test.py`

 * *Files identical despite different names*

