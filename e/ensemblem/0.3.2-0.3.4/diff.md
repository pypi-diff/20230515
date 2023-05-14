# Comparing `tmp/ensemblem-0.3.2.tar.gz` & `tmp/ensemblem-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemblem-0.3.2.tar", last modified: Fri Oct 28 16:15:47 2022, max compression
+gzip compressed data, was "ensemblem-0.3.4.tar", last modified: Sun Oct 30 11:15:11 2022, max compression
```

## Comparing `ensemblem-0.3.2.tar` & `ensemblem-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2022-10-28 16:15:47.136671 ensemblem-0.3.2/
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     1070 2022-10-14 16:36:09.000000 ensemblem-0.3.2/LICENSE
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3647 2022-10-28 16:15:47.136470 ensemblem-0.3.2/PKG-INFO
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3087 2022-10-27 21:19:54.000000 ensemblem-0.3.2/README.md
--rw-r--r--   0 ivanvigorito   (501) staff       (20)       38 2022-10-28 16:15:47.136743 ensemblem-0.3.2/setup.cfg
--rw-r--r--   0 ivanvigorito   (501) staff       (20)      886 2022-10-28 12:25:06.000000 ensemblem-0.3.2/setup.py
-drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2022-10-28 16:15:47.133513 ensemblem-0.3.2/src/
-drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2022-10-28 16:15:47.135488 ensemblem-0.3.2/src/ensemblem/
--rw-r--r--   0 ivanvigorito   (501) staff       (20)        0 2022-10-14 16:36:09.000000 ensemblem-0.3.2/src/ensemblem/__init__.py
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     2998 2022-10-22 09:47:17.000000 ensemblem-0.3.2/src/ensemblem/metrics.py
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3600 2022-10-28 07:32:01.000000 ensemblem-0.3.2/src/ensemblem/model.py
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     1410 2022-10-22 09:31:26.000000 ensemblem-0.3.2/src/ensemblem/utils.py
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     2131 2022-10-22 09:31:26.000000 ensemblem-0.3.2/src/ensemblem/weights_functions.py
-drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2022-10-28 16:15:47.136229 ensemblem-0.3.2/src/ensemblem.egg-info/
--rw-r--r--   0 ivanvigorito   (501) staff       (20)     3647 2022-10-28 16:15:47.000000 ensemblem-0.3.2/src/ensemblem.egg-info/PKG-INFO
--rw-r--r--   0 ivanvigorito   (501) staff       (20)      306 2022-10-28 16:15:47.000000 ensemblem-0.3.2/src/ensemblem.egg-info/SOURCES.txt
--rw-r--r--   0 ivanvigorito   (501) staff       (20)        1 2022-10-28 16:15:47.000000 ensemblem-0.3.2/src/ensemblem.egg-info/dependency_links.txt
--rw-r--r--   0 ivanvigorito   (501) staff       (20)       10 2022-10-28 16:15:47.000000 ensemblem-0.3.2/src/ensemblem.egg-info/top_level.txt
+drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2022-10-30 11:15:11.022621 ensemblem-0.3.4/
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     1070 2022-10-14 16:36:09.000000 ensemblem-0.3.4/LICENSE
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3795 2022-10-30 11:15:11.022410 ensemblem-0.3.4/PKG-INFO
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3235 2022-10-30 10:41:56.000000 ensemblem-0.3.4/README.md
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)       38 2022-10-30 11:15:11.022690 ensemblem-0.3.4/setup.cfg
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)      886 2022-10-30 11:14:30.000000 ensemblem-0.3.4/setup.py
+drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2022-10-30 11:15:11.019576 ensemblem-0.3.4/src/
+drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2022-10-30 11:15:11.021359 ensemblem-0.3.4/src/ensemblem/
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)        0 2022-10-14 16:36:09.000000 ensemblem-0.3.4/src/ensemblem/__init__.py
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     2998 2022-10-22 09:47:17.000000 ensemblem-0.3.4/src/ensemblem/metrics.py
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3715 2022-10-30 11:04:47.000000 ensemblem-0.3.4/src/ensemblem/model.py
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     1410 2022-10-30 10:38:43.000000 ensemblem-0.3.4/src/ensemblem/utils.py
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     2131 2022-10-22 09:31:26.000000 ensemblem-0.3.4/src/ensemblem/weights_functions.py
+drwxr-xr-x   0 ivanvigorito   (501) staff       (20)        0 2022-10-30 11:15:11.022147 ensemblem-0.3.4/src/ensemblem.egg-info/
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)     3795 2022-10-30 11:15:10.000000 ensemblem-0.3.4/src/ensemblem.egg-info/PKG-INFO
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)      306 2022-10-30 11:15:10.000000 ensemblem-0.3.4/src/ensemblem.egg-info/SOURCES.txt
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)        1 2022-10-30 11:15:10.000000 ensemblem-0.3.4/src/ensemblem.egg-info/dependency_links.txt
+-rw-r--r--   0 ivanvigorito   (501) staff       (20)       10 2022-10-30 11:15:10.000000 ensemblem-0.3.4/src/ensemblem.egg-info/top_level.txt
```

### Comparing `ensemblem-0.3.2/LICENSE` & `ensemblem-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ensemblem-0.3.2/PKG-INFO` & `ensemblem-0.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensemblem
-Version: 0.3.2
+Version: 0.3.4
 Summary: Dynamic Weighted Ensemble - Local Fusion
 Home-page: https://github.com/IvanVigor/Dynamic-Weighted-Ensemble
 Author: Ivan Vigorito
 Author-email: ivanvigorit@gmail.com
 Project-URL: Bug Tracker, https://github.com/IvanVigor/Local-Fusion-Dynamic-Weighted-Ensemble/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,15 @@
 
 ```
 
 [Docs - ReadTheDocs](https://local-fusion-dynamic-weighted-ensemble.readthedocs.io/en/latest/) (UnderReview)
 
 ## Usage
 
-First of all, you need to define the KWEnsembler class. Next, it's required to provide the search-space (it could be the validation set) in which the ensembler will find the nearest elements to the generic test sample.
+First of all, you need to define the KWEnsembler class. Next, it's required to provide the search-space (it could be the validation set / neighbours-set) in which the ensembler will find the nearest elements to the generic test sample.
 
 ```{r setup, include=FALSE}
 	from ensemblem.model import KWEnsembler
 	ensemble = KWEnsembler(5)
 	ensemble.fit(X_validation, y_validation)
 ```
 
@@ -47,27 +47,28 @@
 
 ```{r setup, include=FALSE}
 	ensemble.predict(X_test,
                     features_space,
                     other_model_prediction_columns)
 ```
 
-The class returns predictions in the same order in which they are provided. The class supports one or multiple samples to forecasts.
+The class returns predictions in the same order in which they are provided. 
+It supports one or multiple samples to forecasts. In this library, we refers to the neighbours-set as the space in which the ensembler will find the nearest elements to the generic test sample.
 
 
 
 ## Example of using the KWEnsembler class
 
 
 1. Load data
-2. Split data into train, validation and test sets
+2. Split data into train, neighbours-set and test sets
 3. Train multiple expert models on the train data
 4. Generate predictions for the test data
-5. Train the ensembler on validation data
-6. Generate predictions for the test dataset coming from the ensembler
+5. Train the ensembler on neighbours-set
+6. Generate predictions for the test dataset using ensembler
 7. Compare the predictions from the ensembler with the predictions from the expert models
 
 
 ## Results & Benchmarks
 
 |    | Model   |     MAPE |      MAE |      RMSE |    RMSLE |
 |---:|:--------|---------:|---------:|----------:|---------:|
```

### Comparing `ensemblem-0.3.2/README.md` & `ensemblem-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ```
 
 [Docs - ReadTheDocs](https://local-fusion-dynamic-weighted-ensemble.readthedocs.io/en/latest/) (UnderReview)
 
 ## Usage
 
-First of all, you need to define the KWEnsembler class. Next, it's required to provide the search-space (it could be the validation set) in which the ensembler will find the nearest elements to the generic test sample.
+First of all, you need to define the KWEnsembler class. Next, it's required to provide the search-space (it could be the validation set / neighbours-set) in which the ensembler will find the nearest elements to the generic test sample.
 
 ```{r setup, include=FALSE}
 	from ensemblem.model import KWEnsembler
 	ensemble = KWEnsembler(5)
 	ensemble.fit(X_validation, y_validation)
 ```
 
@@ -32,27 +32,28 @@
 
 ```{r setup, include=FALSE}
 	ensemble.predict(X_test,
                     features_space,
                     other_model_prediction_columns)
 ```
 
-The class returns predictions in the same order in which they are provided. The class supports one or multiple samples to forecasts.
+The class returns predictions in the same order in which they are provided. 
+It supports one or multiple samples to forecasts. In this library, we refers to the neighbours-set as the space in which the ensembler will find the nearest elements to the generic test sample.
 
 
 
 ## Example of using the KWEnsembler class
 
 
 1. Load data
-2. Split data into train, validation and test sets
+2. Split data into train, neighbours-set and test sets
 3. Train multiple expert models on the train data
 4. Generate predictions for the test data
-5. Train the ensembler on validation data
-6. Generate predictions for the test dataset coming from the ensembler
+5. Train the ensembler on neighbours-set
+6. Generate predictions for the test dataset using ensembler
 7. Compare the predictions from the ensembler with the predictions from the expert models
 
 
 ## Results & Benchmarks
 
 |    | Model   |     MAPE |      MAE |      RMSE |    RMSLE |
 |---:|:--------|---------:|---------:|----------:|---------:|
```

### Comparing `ensemblem-0.3.2/setup.py` & `ensemblem-0.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "ensemblem",
-    version = "0.3.2",
+    version = "0.3.4",
     author = "Ivan Vigorito",
     author_email = "ivanvigorit@gmail.com",
     description = "Dynamic Weighted Ensemble - Local Fusion",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/IvanVigor/Dynamic-Weighted-Ensemble",
     project_urls = {
```

### Comparing `ensemblem-0.3.2/src/ensemblem/metrics.py` & `ensemblem-0.3.4/src/ensemblem/metrics.py`

 * *Files identical despite different names*

### Comparing `ensemblem-0.3.2/src/ensemblem/utils.py` & `ensemblem-0.3.4/src/ensemblem/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Split the data into train, validation and test sets with target and features
 
     Parameters
     ----------
 
     :param df: pandas.DataFrame to be divided
     :param train_size: float, size of the train set
-    :param val_size: float, size of the validation set
+    :param val_size: float, size of the neighbours-set
     :param test_size: float, size of the test set
 
     :return: train, validation and test sets with target and features
 
     """
     train, val, test = divide_sets(df, train_size, val_size, test_size)
     return train.drop(columns=[target]), \
@@ -27,15 +27,15 @@
     """
     Divide the data into train, validation and test sets
 
     Parameters
     ----------
     :param df: pandas.DataFrame to be divided
     :param train_size: float, size of the train set
-    :param val_size: float, size of the validation set
+    :param val_size: float, size of the neighbours-set
     :param test_size: float, size of the test set
 
     :return: train, validation and test sets
     """
     train_size = int(train_size * len(df))
     val_size = int(val_size * len(df))
     test_size = int(test_size * len(df))
```

### Comparing `ensemblem-0.3.2/src/ensemblem/weights_functions.py` & `ensemblem-0.3.4/src/ensemblem/weights_functions.py`

 * *Files identical despite different names*

### Comparing `ensemblem-0.3.2/src/ensemblem.egg-info/PKG-INFO` & `ensemblem-0.3.4/src/ensemblem.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensemblem
-Version: 0.3.2
+Version: 0.3.4
 Summary: Dynamic Weighted Ensemble - Local Fusion
 Home-page: https://github.com/IvanVigor/Dynamic-Weighted-Ensemble
 Author: Ivan Vigorito
 Author-email: ivanvigorit@gmail.com
 Project-URL: Bug Tracker, https://github.com/IvanVigor/Local-Fusion-Dynamic-Weighted-Ensemble/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,15 @@
 
 ```
 
 [Docs - ReadTheDocs](https://local-fusion-dynamic-weighted-ensemble.readthedocs.io/en/latest/) (UnderReview)
 
 ## Usage
 
-First of all, you need to define the KWEnsembler class. Next, it's required to provide the search-space (it could be the validation set) in which the ensembler will find the nearest elements to the generic test sample.
+First of all, you need to define the KWEnsembler class. Next, it's required to provide the search-space (it could be the validation set / neighbours-set) in which the ensembler will find the nearest elements to the generic test sample.
 
 ```{r setup, include=FALSE}
 	from ensemblem.model import KWEnsembler
 	ensemble = KWEnsembler(5)
 	ensemble.fit(X_validation, y_validation)
 ```
 
@@ -47,27 +47,28 @@
 
 ```{r setup, include=FALSE}
 	ensemble.predict(X_test,
                     features_space,
                     other_model_prediction_columns)
 ```
 
-The class returns predictions in the same order in which they are provided. The class supports one or multiple samples to forecasts.
+The class returns predictions in the same order in which they are provided. 
+It supports one or multiple samples to forecasts. In this library, we refers to the neighbours-set as the space in which the ensembler will find the nearest elements to the generic test sample.
 
 
 
 ## Example of using the KWEnsembler class
 
 
 1. Load data
-2. Split data into train, validation and test sets
+2. Split data into train, neighbours-set and test sets
 3. Train multiple expert models on the train data
 4. Generate predictions for the test data
-5. Train the ensembler on validation data
-6. Generate predictions for the test dataset coming from the ensembler
+5. Train the ensembler on neighbours-set
+6. Generate predictions for the test dataset using ensembler
 7. Compare the predictions from the ensembler with the predictions from the expert models
 
 
 ## Results & Benchmarks
 
 |    | Model   |     MAPE |      MAE |      RMSE |    RMSLE |
 |---:|:--------|---------:|---------:|----------:|---------:|
```

