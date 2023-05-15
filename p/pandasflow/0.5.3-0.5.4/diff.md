# Comparing `tmp/pandasflow-0.5.3.tar.gz` & `tmp/pandasflow-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.5.3.tar", last modified: Mon May 15 11:35:53 2023, max compression
+gzip compressed data, was "pandasflow-0.5.4.tar", last modified: Mon May 15 12:04:24 2023, max compression
```

## Comparing `pandasflow-0.5.3.tar` & `pandasflow-0.5.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.247340 pandasflow-0.5.3/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.3/LICENCE
--rw-rw-rw-   0        0        0      869 2023-05-15 11:35:53.247340 pandasflow-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.226821 pandasflow-0.5.3/pandasflow/
--rw-rw-rw-   0        0        0      391 2023-05-15 11:35:48.000000 pandasflow-0.5.3/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.230258 pandasflow-0.5.3/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.3/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.3/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.3/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.3/pandasflow/get_psql.py
--rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.5.3/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.236280 pandasflow-0.5.3/pandasflow/metrics/
--rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.3/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.3/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.3/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.5.3/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.3/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.3/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.3/pandasflow/metrics/roc.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.237729 pandasflow-0.5.3/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.3/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.3/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.238619 pandasflow-0.5.3/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.3/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.240002 pandasflow-0.5.3/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.3/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.5.3/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.5.3/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.229657 pandasflow-0.5.3/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      869 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      958 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 11:35:53.000000 pandasflow-0.5.3/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 11:35:53.248337 pandasflow-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:35:53.247340 pandasflow-0.5.3/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.3/test/__init__.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.3/test/best_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.3/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.5.3/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.3/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.3/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.3/test/roc_test.py
--rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.5.3/test/split_tt_test.py
--rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.5.3/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.168489 pandasflow-0.5.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.4/LICENCE
+-rw-rw-rw-   0        0        0      869 2023-05-15 12:04:24.168489 pandasflow-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.151139 pandasflow-0.5.4/pandasflow/
+-rw-rw-rw-   0        0        0      391 2023-05-15 12:04:20.000000 pandasflow-0.5.4/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.153133 pandasflow-0.5.4/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.4/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.4/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.4/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.5.4/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.5.4/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.158120 pandasflow-0.5.4/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.4/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.4/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.4/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.5.4/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.4/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.4/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.4/pandasflow/metrics/roc.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.159029 pandasflow-0.5.4/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.4/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.4/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.160268 pandasflow-0.5.4/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.4/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.161659 pandasflow-0.5.4/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.4/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.5.4/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.5.4/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.153133 pandasflow-0.5.4/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      869 2023-05-15 12:04:24.000000 pandasflow-0.5.4/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2023-05-15 12:04:24.000000 pandasflow-0.5.4/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 12:04:24.000000 pandasflow-0.5.4/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-15 12:04:24.000000 pandasflow-0.5.4/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 12:04:24.000000 pandasflow-0.5.4/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 12:04:24.168489 pandasflow-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:04:24.167398 pandasflow-0.5.4/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.4/test/__init__.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.4/test/best_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.4/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.5.4/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.4/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.4/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.4/test/roc_test.py
+-rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.5.4/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.5.4/test/split_tvt_test.py
```

### Comparing `pandasflow-0.5.3/LICENCE` & `pandasflow-0.5.4/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/PKG-INFO` & `pandasflow-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.3
+Version: 0.5.4
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.3/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.5.4/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/pandasflow/metrics/best_f1.py` & `pandasflow-0.5.4/pandasflow/metrics/best_f1.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/pandasflow/metrics/conf_mat.py` & `pandasflow-0.5.4/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/pandasflow/metrics/lloss_up.py` & `pandasflow-0.5.4/pandasflow/metrics/lloss_up.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,63 +5,60 @@
 # Для задач классификации с таргетом 0-1
 # Сравнение человеческого baseline с машинным предиктом
 # Возвращает две метрики:
 # log_loss - чем меньше, тем лучше
 # uplift - чем больше, тем лучше
 
 
-def def_baseline(df, target):
-	base = df[target].sum()
-	base_pct = df[target].sum() / len(df)
+def def_baseline(target):
+	base = target.sum()
+	base_pct = base / len(target)
 	
 	return base, base_pct
 
 
-def _uplift(df, target, sort_score, pct, baseline=None):
-	base, base_pct = def_baseline(df, target)
+def _uplift(target, sort_score, pct, baseline=None):
+	base, base_pct = def_baseline(target)
 	if baseline != None:
 		print('baseline is not None, but unknown')
 	
-	_df = df.sort_values(sort_score, ascending=False)
-	pct_len = round(len(df) * pct)
-	base_found = _df.head(pct_len)[target].sum()
+	_df = sort_score.sort_values(ascending=False)
+	pct_len = round(len(target) * pct)
+	base_found = _df.head(pct_len).sum()
 
 	return base_pct, ((base_found / base) / pct)
 
 
-def lloss_up(df, target, score, pct=0.2, baseline=None):
+def lloss_up(target, score, pct=0.2, baseline=None):
 	'''Для задач классификации с таргетом 0-1
 	Сравнение человеческого baseline с машинным предиктом
 	Возвращает две метрики:
 	
 	log_loss - чем меньше, тем лучше
 	uplift - чем больше, тем лучше
 	
 	Parameters
 	----------
-	df : pd.DataFrame
-		Таблица данных
-	
-	target : str
+	target : pd.Series
 		Название колонки с искомым значением
 	
-	score : str
+	score : pd.Series
 		Название колонки с предиктом машинного обучение
 		Результат работы, который и сравниваем
 	
 	pct : float, default = 0.2
 		Процент колонки предикта, из которого и считаем uplift
 	
 	baseline : None, def, int, float. default = None
 		Худший вариант предсказания, базово - среднееарифметическое
 		Лучше не трогать и оно посчитается от target
 	'''
 
-	lloss = log_loss(df[target], df[score])
-	base, up = _uplift(df, target, score, pct, baseline=baseline)
+	lloss = log_loss(target, score)
+	base, up = _uplift(target, score, pct, baseline=baseline)
 	
 	table = pd.DataFrame()
 	table.index = ['baseline', 'log_loss', 'uplift']
 	table[' '] = [base, lloss, up]
 	
 	print(table)
 	print()
```

### Comparing `pandasflow-0.5.3/pandasflow/metrics/precision_recall.py` & `pandasflow-0.5.4/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/pandasflow/metrics/roc.py` & `pandasflow-0.5.4/pandasflow/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/pandasflow/reset_mi.py` & `pandasflow-0.5.4/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/pandasflow/split/train_test.py` & `pandasflow-0.5.4/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/pandasflow/split/train_valid_test.py` & `pandasflow-0.5.4/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.5.4/pandasflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.5.3
+Version: 0.5.4
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.5.3/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.5.4/pandasflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/setup.py` & `pandasflow-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/test/best_f1_test.py` & `pandasflow-0.5.4/test/best_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/test/conf_mat_test.py` & `pandasflow-0.5.4/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/test/precision_recall_test.py` & `pandasflow-0.5.4/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/test/roc_test.py` & `pandasflow-0.5.4/test/roc_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.5.3/test/split_tvt_test.py` & `pandasflow-0.5.4/test/split_tvt_test.py`

 * *Files identical despite different names*

