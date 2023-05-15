# Comparing `tmp/pandasflow-0.5.2.tar.gz` & `tmp/pandasflow-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.5.2.tar", last modified: Mon May 15 10:19:36 2023, max compression
+gzip compressed data, was "pandasflow-0.5.3.tar", last modified: Mon May 15 11:35:53 2023, max compression
```

## Comparing `pandasflow-0.5.2.tar` & `pandasflow-0.5.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.385079 pandasflow-0.5.2/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.2/LICENCE
--rw-rw-rw-   0        0        0      694 2023-05-15 10:19:36.385079 pandasflow-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.366124 pandasflow-0.5.2/pandasflow/
--rw-rw-rw-   0        0        0      391 2023-05-15 10:19:19.000000 pandasflow-0.5.2/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.370119 pandasflow-0.5.2/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.2/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.2/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.2/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.2/pandasflow/get_psql.py
--rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.5.2/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.375106 pandasflow-0.5.2/pandasflow/metrics/
--rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.2/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.2/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.2/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.5.2/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.2/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.2/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.2/pandasflow/metrics/roc.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.376103 pandasflow-0.5.2/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.2/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.2/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.377100 pandasflow-0.5.2/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.2/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.378098 pandasflow-0.5.2/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.2/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.5.2/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3944 2023-05-15 10:18:04.000000 pandasflow-0.5.2/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.369121 pandasflow-0.5.2/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      958 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 10:19:36.385079 pandasflow-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.384082 pandasflow-0.5.2/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.2/test/__init__.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.2/test/best_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.2/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.5.2/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.2/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.2/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.2/test/roc_test.py
--rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.5.2/test/split_tt_test.py
--rw-rw-rw-   0        0        0      661 2023-05-15 10:18:38.000000 pandasflow-0.5.2/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.247340 pandasflow-0.5.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.3/LICENCE
+-rw-rw-rw-   0        0        0      869 2023-05-15 11:35:53.247340 pandasflow-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.226821 pandasflow-0.5.3/pandasflow/
+-rw-rw-rw-   0        0        0      391 2023-05-15 11:35:48.000000 pandasflow-0.5.3/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.230258 pandasflow-0.5.3/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.3/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.3/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.3/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.3/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.5.3/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.236280 pandasflow-0.5.3/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.3/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.3/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.3/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.5.3/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.3/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.3/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.3/pandasflow/metrics/roc.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.237729 pandasflow-0.5.3/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.3/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.3/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.238619 pandasflow-0.5.3/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.3/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.240002 pandasflow-0.5.3/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.3/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.5.3/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.5.3/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.229657 pandasflow-0.5.3/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      869 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 11:35:53.248337 pandasflow-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.247340 pandasflow-0.5.3/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.3/test/__init__.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.3/test/best_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.3/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.5.3/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.3/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.3/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.3/test/roc_test.py
+-rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.5.3/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.5.3/test/split_tvt_test.py
```

### Comparing `pandasflow-0.5.2/LICENCE` & `pandasflow-0.5.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.5.3/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/metrics/best_f1.py` & `pandasflow-0.5.3/pandasflow/metrics/best_f1.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/metrics/conf_mat.py` & `pandasflow-0.5.3/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/metrics/lloss_up.py` & `pandasflow-0.5.3/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/metrics/precision_recall.py` & `pandasflow-0.5.3/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/metrics/roc.py` & `pandasflow-0.5.3/pandasflow/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/reset_mi.py` & `pandasflow-0.5.3/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/split/train_test.py` & `pandasflow-0.5.3/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow/split/train_valid_test.py` & `pandasflow-0.5.3/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.5.3/pandasflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/setup.py` & `pandasflow-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/test/best_f1_test.py` & `pandasflow-0.5.3/test/best_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/test/conf_mat_test.py` & `pandasflow-0.5.3/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/test/lloss_up_test.py` & `pandasflow-0.5.3/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/test/precision_recall_test.py` & `pandasflow-0.5.3/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/test/roc_test.py` & `pandasflow-0.5.3/test/roc_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.2/test/split_tvt_test.py` & `pandasflow-0.5.3/test/split_tvt_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,7 +18,10 @@
 print('\n')
 
 train, valid, test = pdf.split.train_valid_test(df, target=['Exited', 'Age'], stratify='Exited')
 print('\n')
 
 train, valid, test = pdf.split.train_valid_test(df, target=['Exited', 'Age'], stratify='Exited', round_=3)
 print('\n')
+
+train, valid, test = pdf.split.train_valid_test(df, target=['Exited', 'Age'], stratify='Exited', round_=1)
+print('\n')
```

