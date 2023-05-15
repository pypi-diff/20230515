# Comparing `tmp/deepBreaks-1.0.1.tar.gz` & `tmp/deepBreaks-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepBreaks-1.0.1.tar", last modified: Tue Jan 31 16:38:14 2023, max compression
+gzip compressed data, was "deepBreaks-1.0.2.tar", last modified: Mon May 15 20:20:24 2023, max compression
```

## Comparing `deepBreaks-1.0.1.tar` & `deepBreaks-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-01-31 16:38:14.566669 deepBreaks-1.0.1/
--rw-r--r--   0 root         (0) staff       (20)     1084 2022-05-16 04:21:29.000000 deepBreaks-1.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) staff       (20)       58 2023-01-24 00:28:00.000000 deepBreaks-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)    22478 2023-01-31 16:38:14.566269 deepBreaks-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    21601 2023-01-24 00:27:15.000000 deepBreaks-1.0.1/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-01-31 16:38:14.560936 deepBreaks-1.0.1/deepBreaks/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-05-16 04:21:29.000000 deepBreaks-1.0.1/deepBreaks/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9980 2023-01-25 20:33:40.000000 deepBreaks-1.0.1/deepBreaks/deepBreaks.py
--rw-r--r--   0 root         (0) staff       (20)    11621 2023-01-17 18:58:04.000000 deepBreaks-1.0.1/deepBreaks/models.py
--rw-r--r--   0 root         (0) staff       (20)    17472 2023-01-17 20:27:51.000000 deepBreaks-1.0.1/deepBreaks/preprocessing.py
--rw-r--r--   0 root         (0) staff       (20)    18237 2023-01-17 18:58:04.000000 deepBreaks-1.0.1/deepBreaks/visualization.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-01-31 16:38:14.565979 deepBreaks-1.0.1/deepBreaks.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    22478 2023-01-31 16:38:14.000000 deepBreaks-1.0.1/deepBreaks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      423 2023-01-31 16:38:14.000000 deepBreaks-1.0.1/deepBreaks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-01-31 16:38:14.000000 deepBreaks-1.0.1/deepBreaks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       58 2023-01-31 16:38:14.000000 deepBreaks-1.0.1/deepBreaks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-01-25 20:19:53.000000 deepBreaks-1.0.1/deepBreaks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)      145 2023-01-31 16:38:14.000000 deepBreaks-1.0.1/deepBreaks.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       11 2023-01-31 16:38:14.000000 deepBreaks-1.0.1/deepBreaks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      144 2023-01-17 18:58:04.000000 deepBreaks-1.0.1/requirements.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-01-31 16:38:14.566846 deepBreaks-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     3001 2023-01-24 00:22:47.000000 deepBreaks-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 20:20:24.051900 deepBreaks-1.0.2/
+-rw-r--r--   0 root         (0) staff       (20)     1084 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/LICENSE.txt
+-rw-r--r--   0 root         (0) staff       (20)    22640 2023-05-15 20:20:24.051665 deepBreaks-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    21765 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 20:20:24.049931 deepBreaks-1.0.2/deepBreaks/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9980 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/deepBreaks.py
+-rw-r--r--   0 root         (0) staff       (20)    11921 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/models.py
+-rw-r--r--   0 root         (0) staff       (20)    17472 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/preprocessing.py
+-rw-r--r--   0 root         (0) staff       (20)    18237 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/visualization.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 20:20:24.051392 deepBreaks-1.0.2/deepBreaks.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    22640 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      394 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       58 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)      145 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       11 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-15 20:20:24.051972 deepBreaks-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     3001 2023-05-15 20:18:53.000000 deepBreaks-1.0.2/setup.py
```

### Comparing `deepBreaks-1.0.1/LICENSE.txt` & `deepBreaks-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deepBreaks-1.0.1/PKG-INFO` & `deepBreaks-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepBreaks
-Version: 1.0.1
+Version: 1.0.2
 Summary: deepBreaks: a machine learning tool for identifying and prioritizing genotype-phenotype associations
 Home-page: http://github.com/omicsEye/deepBreaks
 Author: Mahdi Baghbanzadeh
 Author-email: mbagh@gwu.edu
 License: MIT
 Keywords: machine learning,genomics,sequencing data
 Platform: Linux
@@ -46,15 +46,15 @@
 real-world applications.
 
 ---
 **Citation:**
 
 Mahdi Baghbanzadeh, Tyson Dawson, Bahar Sayoldin, Todd H. Oakley, Keith A. Crandall, Ali Rahnavard (2023).
 **_deepBreaks_: a machine learning tool for identifying and prioritizing genotype-phenotype associations**
-, https://github.com/omicsEye/deeBreaks/.
+, https://github.com/omicsEye/deepBreaks/.
 
 ---
 
 # deepBreaks user manual #
 
 ## Contents ##
 
@@ -488,10 +488,9 @@
 nucleotide sequences of the V3 loop of subtypes B and C. 
 This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype_HIV.ipynb) 
 illustrates the steps.
 
 # Support #
 
 * Please submit your questions or issues with the software at
-[Issues tracker](https://github.com/omicsEye/deepBreaks/issues).
-
-
+[Issues tracker](https://github.com/omicsEye/deepBreaks/issues).  
+* For community discussions, questions, and issue reporting, please visit our forum [here](https://forum.omicseye.org/c/omics-downstream-analysis/deepbreaks/12)
```

### Comparing `deepBreaks-1.0.1/README.md` & `deepBreaks-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 real-world applications.
 
 ---
 **Citation:**
 
 Mahdi Baghbanzadeh, Tyson Dawson, Bahar Sayoldin, Todd H. Oakley, Keith A. Crandall, Ali Rahnavard (2023).
 **_deepBreaks_: a machine learning tool for identifying and prioritizing genotype-phenotype associations**
-, https://github.com/omicsEye/deeBreaks/.
+, https://github.com/omicsEye/deepBreaks/.
 
 ---
 
 # deepBreaks user manual #
 
 ## Contents ##
 
@@ -464,8 +464,9 @@
 nucleotide sequences of the V3 loop of subtypes B and C. 
 This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype_HIV.ipynb) 
 illustrates the steps.
 
 # Support #
 
 * Please submit your questions or issues with the software at
-[Issues tracker](https://github.com/omicsEye/deepBreaks/issues).
+[Issues tracker](https://github.com/omicsEye/deepBreaks/issues).  
+* For community discussions, questions, and issue reporting, please visit our forum [here](https://forum.omicseye.org/c/omics-downstream-analysis/deepbreaks/12)
```

### Comparing `deepBreaks-1.0.1/deepBreaks/deepBreaks.py` & `deepBreaks-1.0.2/deepBreaks/deepBreaks.py`

 * *Files identical despite different names*

### Comparing `deepBreaks-1.0.1/deepBreaks/models.py` & `deepBreaks-1.0.2/deepBreaks/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 import re
 from sklearn import preprocessing
 from sklearn.model_selection import cross_validate
 from sklearn.model_selection import ParameterGrid
-
+from sklearn.model_selection import KFold
 
 def str_clean(x):
     x = str(x).split('(')[0]
     x = re.sub(r"([a-z0-9])([A-Z])", r"\1 \2", x)
     return x
 
 
@@ -59,15 +59,17 @@
 def _model_report(summary, scores, sort_by):
     tm = {}
     for key in summary.keys():
         tm[key] = [str_clean(summary[key]['model'])] + summary[key]['metrics']
     tm = pd.DataFrame.from_dict(tm, orient='index',
                                 columns=['Model'] + list(scores.keys()))
     tm.sort_values(by=sort_by, ascending=False, inplace=True)
-    tm.iloc[:, 1:] = tm.iloc[:, 1:].abs()
+    for cl in tm.columns:
+        if cl != 'Model' and cl != 'R2':
+            tm.loc[:, cl] = tm.loc[:, cl].abs()
     return tm
 
 
 def _get_models(ana_type):
 
     if ana_type == 'reg':
         from sklearn.ensemble import RandomForestRegressor, AdaBoostRegressor
@@ -160,15 +162,16 @@
 
 def model_compare(X_train, y_train, ana_type,
                   cv=10, select_top=5,
                   models=None, scores=None,
                   params=None, sort_by=None,
                   n_positions=None,
                   grouped_features=None,
-                  report_dir='.'):
+                  report_dir='.',
+                  random_state = 123):
     """
     Fits multiple models to the data and compare them based on the cross-validation score. Then returns the top models,
     their feature importance, and also calculates the `mean` of feature importance for all the features across the
     top models.
     Parameters
     ----------
     X_train : pandas.DataFrame
@@ -256,16 +259,20 @@
     if ana_type == 'reg':
         if sort_by is None:
             sort_by = 'MAE'
     else:
         if sort_by is None:
             sort_by = 'F1'
 
-    le = preprocessing.LabelEncoder()
-    y_train = le.fit_transform(y_train)
+    if ana_type == 'cl':
+        le = preprocessing.LabelEncoder()
+        y_train = le.fit_transform(y_train)
+
+    # create the KFold object with shuffling
+    cv = KFold(n_splits=cv, shuffle=True, random_state=random_state)
 
     summary = {}
     for model in models.keys():
         if model in params:
             tune_params = ['default']
             tune_params.extend(ParameterGrid(params[model]))
         else:
```

### Comparing `deepBreaks-1.0.1/deepBreaks/preprocessing.py` & `deepBreaks-1.0.2/deepBreaks/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deepBreaks-1.0.1/deepBreaks/visualization.py` & `deepBreaks-1.0.2/deepBreaks/visualization.py`

 * *Files identical despite different names*

### Comparing `deepBreaks-1.0.1/deepBreaks.egg-info/PKG-INFO` & `deepBreaks-1.0.2/deepBreaks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepBreaks
-Version: 1.0.1
+Version: 1.0.2
 Summary: deepBreaks: a machine learning tool for identifying and prioritizing genotype-phenotype associations
 Home-page: http://github.com/omicsEye/deepBreaks
 Author: Mahdi Baghbanzadeh
 Author-email: mbagh@gwu.edu
 License: MIT
 Keywords: machine learning,genomics,sequencing data
 Platform: Linux
@@ -46,15 +46,15 @@
 real-world applications.
 
 ---
 **Citation:**
 
 Mahdi Baghbanzadeh, Tyson Dawson, Bahar Sayoldin, Todd H. Oakley, Keith A. Crandall, Ali Rahnavard (2023).
 **_deepBreaks_: a machine learning tool for identifying and prioritizing genotype-phenotype associations**
-, https://github.com/omicsEye/deeBreaks/.
+, https://github.com/omicsEye/deepBreaks/.
 
 ---
 
 # deepBreaks user manual #
 
 ## Contents ##
 
@@ -488,10 +488,9 @@
 nucleotide sequences of the V3 loop of subtypes B and C. 
 This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype_HIV.ipynb) 
 illustrates the steps.
 
 # Support #
 
 * Please submit your questions or issues with the software at
-[Issues tracker](https://github.com/omicsEye/deepBreaks/issues).
-
-
+[Issues tracker](https://github.com/omicsEye/deepBreaks/issues).  
+* For community discussions, questions, and issue reporting, please visit our forum [here](https://forum.omicseye.org/c/omics-downstream-analysis/deepbreaks/12)
```

### Comparing `deepBreaks-1.0.1/setup.py` & `deepBreaks-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering :: Bio-Informatics"
     ]
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 AUTHOR = "Mahdi Baghbanzadeh"
 AUTHOR_EMAIL = "mbagh@gwu.edu"
 MAINTAINER = "Mahdi Baghbanzadeh"
 MAINTAINER_EMAIL = "mbagh@gwu.edu"
 
 # try to download the bitbucket counter file to count downloads
 # this has been added since PyPI has turned off the download stats
```

