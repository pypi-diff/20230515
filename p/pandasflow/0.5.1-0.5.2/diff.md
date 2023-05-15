# Comparing `tmp/pandasflow-0.5.1.tar.gz` & `tmp/pandasflow-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.5.1.tar", last modified: Mon May 15 09:14:12 2023, max compression
+gzip compressed data, was "pandasflow-0.5.2.tar", last modified: Mon May 15 10:19:36 2023, max compression
```

## Comparing `pandasflow-0.5.1.tar` & `pandasflow-0.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.858849 pandasflow-0.5.1/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.1/LICENCE
--rw-rw-rw-   0        0        0      694 2023-05-15 09:14:12.858849 pandasflow-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.835956 pandasflow-0.5.1/pandasflow/
--rw-rw-rw-   0        0        0      391 2023-05-15 09:13:53.000000 pandasflow-0.5.1/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.839947 pandasflow-0.5.1/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.1/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.1/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.1/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.1/pandasflow/get_psql.py
--rw-rw-rw-   0        0        0      206 2023-05-09 15:33:32.000000 pandasflow-0.5.1/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.846995 pandasflow-0.5.1/pandasflow/metrics/
--rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.1/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.1/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.1/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.5.1/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.1/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.1/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.1/pandasflow/metrics/roc.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.847570 pandasflow-0.5.1/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.1/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.1/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.848561 pandasflow-0.5.1/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.1/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.849770 pandasflow-0.5.1/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.1/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3016 2023-05-04 13:48:42.000000 pandasflow-0.5.1/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3719 2023-05-04 13:48:33.000000 pandasflow-0.5.1/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.838950 pandasflow-0.5.1/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      958 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 09:14:12.000000 pandasflow-0.5.1/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 09:14:12.859834 pandasflow-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:14:12.857839 pandasflow-0.5.1/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.1/test/__init__.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.1/test/best_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.1/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.5.1/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.1/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.1/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.1/test/roc_test.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.5.1/test/split_tt_test.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.5.1/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.385079 pandasflow-0.5.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.2/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-05-15 10:19:36.385079 pandasflow-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.366124 pandasflow-0.5.2/pandasflow/
+-rw-rw-rw-   0        0        0      391 2023-05-15 10:19:19.000000 pandasflow-0.5.2/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.370119 pandasflow-0.5.2/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.2/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.2/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.2/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.2/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.5.2/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.375106 pandasflow-0.5.2/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.2/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.2/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.2/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.5.2/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.2/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.2/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.2/pandasflow/metrics/roc.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.376103 pandasflow-0.5.2/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.2/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.2/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.377100 pandasflow-0.5.2/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.2/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.378098 pandasflow-0.5.2/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.2/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.5.2/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3944 2023-05-15 10:18:04.000000 pandasflow-0.5.2/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.369121 pandasflow-0.5.2/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 10:19:36.000000 pandasflow-0.5.2/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 10:19:36.385079 pandasflow-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:19:36.384082 pandasflow-0.5.2/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.2/test/__init__.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.2/test/best_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.2/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.5.2/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.2/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.2/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.2/test/roc_test.py
+-rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.5.2/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      661 2023-05-15 10:18:38.000000 pandasflow-0.5.2/test/split_tvt_test.py
```

### Comparing `pandasflow-0.5.1/LICENCE` & `pandasflow-0.5.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/PKG-INFO` & `pandasflow-0.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.1
+Version: 0.5.2
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.1/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.5.2/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/pandasflow/metrics/best_f1.py` & `pandasflow-0.5.2/pandasflow/metrics/best_f1.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/pandasflow/metrics/conf_mat.py` & `pandasflow-0.5.2/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/pandasflow/metrics/lloss_up.py` & `pandasflow-0.5.2/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/pandasflow/metrics/precision_recall.py` & `pandasflow-0.5.2/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/pandasflow/metrics/roc.py` & `pandasflow-0.5.2/pandasflow/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/pandasflow/reset_mi.py` & `pandasflow-0.5.2/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/pandasflow/split/train_test.py` & `pandasflow-0.5.2/pandasflow/split/train_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pandasflow as pdf
 
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
 def train_test(
 	*arrays,
-	test_size=None,
 	train_size=0.8,
 	random_state=42,
 	shuffle=True,
 	stratify=None,
 	round_=None,
 	target=None
 ):
@@ -18,21 +17,14 @@
 
 	Parameters
 	----------
 	*arrays : sequence of indexables with same length / shape[0]
 		Allowed inputs are lists, numpy arrays, scipy-sparse
 		matrices or pandas dataframes.
 
-	test_size : float or int, default=None
-		If float, should be between 0.0 and 1.0 and represent the proportion
-		of the dataset to include in the test split. If int, represents the
-		absolute number of test samples. If None, the value is set to the
-		complement of the train size. If ``train_size`` is also None, it will
-		be set to 0.25.
-
 	train_size : float or int, default=None
 		If float, should be between 0.0 and 1.0 and represent the
 		proportion of the dataset to include in the train split. If
 		int, represents the absolute number of train samples. If None,
 		the value is automatically set to the complement of the test size.
 
 	random_state : int, RandomState instance or None, default=None
@@ -80,30 +72,37 @@
 	table.index = ['train',
 				   'test',
 				   '',
 				   'Amount',
 				   'InitData']
 	
 	if target != None:
+		target_ = []
+		if type(target) == str:
+			target_.append(target)
+		
+		elif type(target) == list:
+			target_ = target
+		
 		try:
-			if type(target) is str:
-				table[target] = [train[target].mean(),
-								 test[target].mean(),
-								 '',
-								 '',
-								 df[target].mean()]
-			
-			
-			elif type(target) is list:
-				for col in list(target):
-					table[col] = [train[col].mean(),
-								  test[col].mean(),
-								  '',
-								  '',
-								  df[col].mean()]
+			for col in list(target_):
+				train_col = train[col].mean()
+				test_col = test[col].mean()
+				df_col = df[col].mean()
+				
+				if round_ not in [None, 'n', 'N'] and round_ > 0:
+					train_col = round(train_col, round_)
+					test_col = round(test_col, round_)
+					df_col = round(df_col, round_)
+				
+				table[col] = [train_col,
+							  test_col,
+							  '',
+							  '',
+							  df_col]
 		except KeyError:
 			raise KeyError(*target)
 	
 	print(table)
 	
 	if amount_prop != 1.0 or len(arrays[0]) != amount_len:
 		print('---')
```

### Comparing `pandasflow-0.5.1/pandasflow/split/train_valid_test.py` & `pandasflow-0.5.2/pandasflow/split/train_valid_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,32 +92,41 @@
 				 amount_prop,
 				 ''],
 		
 		
 	})
 	
 	if target != None:
+		
+		target_ = []
+		if type(target) == str:
+			target_.append(target)
+		
+		elif type(target) == list:
+			target_ = target
+		
 		try:
-			if type(target) is str:
-				table[target] = [train[target].mean(),
-							  valid[target].mean(),
-							  test[target].mean(),
-							  '',
-							  '',
-							  df[target].mean()]
-			
-			
-			elif type(target) is list:
-				for col in list(target):
-					table[col] = [train[col].mean(),
-									valid[col].mean(),
-									test[col].mean(),
-									'',
-									'',
-									df[col].mean()]
+			for col in list(target_):
+				train_col = train[col].mean()
+				valid_col = valid[col].mean()
+				test_col = test[col].mean()
+				df_col = df[col].mean()
+				
+				if round_ not in [None, 'n', 'N'] and round_ > 0:
+					train_col = round(train_col, round_)
+					test_col = round(test_col, round_)
+					valid_col = round(valid_col, round_)
+					df_col = round(df_col, round_)
+				
+				table[col] = [train_col,
+								valid_col,
+								test_col,
+								'',
+								'',
+								df_col]
 		except KeyError:
 			raise KeyError(*target)
 	
 	table.index = ['train',
 				   'valid',
 				   'test',
 				   '',
```

### Comparing `pandasflow-0.5.1/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.5.2/pandasflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.1
+Version: 0.5.2
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.1/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.5.2/pandasflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/setup.py` & `pandasflow-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/test/best_f1_test.py` & `pandasflow-0.5.2/test/best_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/test/conf_mat_test.py` & `pandasflow-0.5.2/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/test/lloss_up_test.py` & `pandasflow-0.5.2/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/test/precision_recall_test.py` & `pandasflow-0.5.2/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/test/roc_test.py` & `pandasflow-0.5.2/test/roc_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.1/test/split_tvt_test.py` & `pandasflow-0.5.2/test/split_tvt_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 train, valid, test = pdf.split.train_valid_test(df, target='Exited')
 print('\n')
 
 train, valid, test = pdf.split.train_valid_test(df, target='Exited', stratify='Exited')
 print('\n')
 
-train, valid, test = pdf.split.train_valid_test(df, target=['Exited', 'HasCrCard'])
+train, valid, test = pdf.split.train_valid_test(df, target=['Exited', 'Age'])
 print('\n')
 
-train, valid, test = pdf.split.train_valid_test(df, target=['Exited', 'HasCrCard'], stratify='Exited')
+train, valid, test = pdf.split.train_valid_test(df, target=['Exited', 'Age'], stratify='Exited')
 print('\n')
 
-#
-# train, valid, test = pdf.split.train_valid_test(df, target=['Surname'])
-# print('\n')
+train, valid, test = pdf.split.train_valid_test(df, target=['Exited', 'Age'], stratify='Exited', round_=3)
+print('\n')
```

