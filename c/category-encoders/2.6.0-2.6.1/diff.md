# Comparing `tmp/category_encoders-2.6.0.tar.gz` & `tmp/category_encoders-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/category_encoders-2.6.0.tar", last modified: Sat Jan 14 21:22:02 2023, max compression
+gzip compressed data, was "dist/category_encoders-2.6.1.tar", last modified: Mon May 15 21:29:54 2023, max compression
```

## Comparing `category_encoders-2.6.0.tar` & `category_encoders-2.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 21:22:02.000000 category_encoders-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-14 21:21:27.000000 category_encoders-2.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-14 21:21:27.000000 category_encoders-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-01-14 21:22:02.000000 category_encoders-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-01-14 21:21:27.000000 category_encoders-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders/
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/backward_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/base_contrast_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/basen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/cat_boost.py
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/datasets/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/datasets/data/compass.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/datasets/data/postcode_dataset_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/glmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/gray.py
--rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/helmert.py
--rw-r--r--   0 runner    (1001) docker     (123)    20859 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/james_stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/leave_one_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/m_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/ordinal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/quantile_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/rankhot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/sum_coding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18358 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/woe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-01-14 21:21:27.000000 category_encoders-2.6.0/category_encoders/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-14 21:22:02.000000 category_encoders-2.6.0/category_encoders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-14 21:21:27.000000 category_encoders-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-14 21:22:02.000000 category_encoders-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-01-14 21:21:27.000000 category_encoders-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:29:54.000000 category_encoders-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-15 21:29:22.000000 category_encoders-2.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-15 21:29:22.000000 category_encoders-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-05-15 21:29:54.000000 category_encoders-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-05-15 21:29:22.000000 category_encoders-2.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/backward_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/base_contrast_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/basen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/cat_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/datasets/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/datasets/data/compass.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/datasets/data/postcode_dataset_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/glmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/gray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/helmert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20859 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/james_stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/leave_one_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/m_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/ordinal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/quantile_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/rankhot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/sum_coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19023 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/woe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-05-15 21:29:22.000000 category_encoders-2.6.1/category_encoders/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 21:29:54.000000 category_encoders-2.6.1/category_encoders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 21:29:22.000000 category_encoders-2.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-15 21:29:54.000000 category_encoders-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-15 21:29:22.000000 category_encoders-2.6.1/setup.py
```

### Comparing `category_encoders-2.6.0/LICENSE.md` & `category_encoders-2.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/PKG-INFO` & `category_encoders-2.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: category_encoders
-Version: 2.6.0
+Version: 2.6.1
 Summary: A collection of sklearn transformers to encode categorical variables as numeric
 Home-page: https://github.com/scikit-learn-contrib/category_encoders
 Author: Will McGinnis
 Author-email: will@pedalwrencher.com
 License: BSD
-Download-URL: https://github.com/scikit-learn-contrib/category_encoders/tarball/2.6.0
+Download-URL: https://github.com/scikit-learn-contrib/category_encoders/tarball/2.6.1
 Description: Categorical Encoding Methods
         ============================
         
         [![Downloads](https://pepy.tech/badge/category-encoders)](https://pepy.tech/project/category-encoders)
         [![Downloads](https://pepy.tech/badge/category-encoders/month)](https://pepy.tech/project/category-encoders)
         ![Test Suite and Linting](https://github.com/scikit-learn-contrib/category_encoders/workflows/Test%20Suite%20and%20Linting/badge.svg)
         [![DOI](https://zenodo.org/badge/47077067.svg)](https://zenodo.org/badge/latestdoi/47077067)
@@ -153,17 +153,18 @@
          6. BaseN Encoding and Grid Search in categorical variables. From http://www.willmcginnis.com/2016/12/18/basen-encoding-grid-search-category_encoders/
          7. Daniele Miccii-Barreca (2001). A Preprocessing Scheme for High-Cardinality Categorical Attributes in Classification and Prediction Problems. SIGKDD Explor. Newsl. 3, 1. From http://dx.doi.org/10.1145/507533.507538
          8. Weight of Evidence (WOE) and Information Value Explained. From https://www.listendata.com/2015/03/weight-of-evidence-woe-and-information.html
          9. Empirical Bayes for multiple sample sizes. From http://chris-said.io/2017/05/03/empirical-bayes-for-multiple-sample-sizes/
          10. Simple Count or Frequency Encoding. From https://www.datacamp.com/community/tutorials/encoding-methodologies
          11. Transforming categorical features to numerical features. From https://tech.yandex.com/catboost/doc/dg/concepts/algorithm-main-stages_cat-to-numberic-docpage/
          12. Andrew Gelman and Jennifer Hill (2006). Data Analysis Using Regression and Multilevel/Hierarchical Models. From https://faculty.psau.edu.sa/filedownload/doc-12-pdf-a1997d0d31f84d13c1cdc44ac39a8f2c-original.pdf
-         13. Carlos Mougan, David Masip, Jordi Nin and Oriol Pujol (2021). Quantile Encoder: Tackling High Cardinality Categorical Features in Regression Problems. https://link.springer.com/chapter/10.1007%2F978-3-030-85529-1_14
+         13. Carlos Mougan, David Masip, Jordi Nin and Oriol Pujol (2021). Quantile Encoder: Tackling High Cardinality Categorical Features in Regression Problems. Modeling Decisions for Artificial Intelligence, 2021. Springer International Publishing https://link.springer.com/chapter/10.1007%2F978-3-030-85529-1_14
          14. Gray Encoding. From https://en.wikipedia.org/wiki/Gray_code 
          15. Jacob Buckman, Aurko Roy, Colin Raffel, Ian Goodfellow: Thermometer Encoding: One Hot Way To Resist Adversarial Examples. From https://openreview.net/forum?id=S18Su--CW
+         16. Fairness implications of encoding protected categorical attributes. Carlos Mougan, Jose Alvarez, Salvatore Ruggieri, and Steffen Staab.  In Proceedings of the 2023 AAAI/ACM Conference on AI, Ethics, and Society, AIES ’21, https://arxiv.org/abs/2201.11358
         
 Keywords: python data science machine learning pandas sklearn
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `category_encoders-2.6.0/README.md` & `category_encoders-2.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -144,10 +144,11 @@
  6. BaseN Encoding and Grid Search in categorical variables. From http://www.willmcginnis.com/2016/12/18/basen-encoding-grid-search-category_encoders/
  7. Daniele Miccii-Barreca (2001). A Preprocessing Scheme for High-Cardinality Categorical Attributes in Classification and Prediction Problems. SIGKDD Explor. Newsl. 3, 1. From http://dx.doi.org/10.1145/507533.507538
  8. Weight of Evidence (WOE) and Information Value Explained. From https://www.listendata.com/2015/03/weight-of-evidence-woe-and-information.html
  9. Empirical Bayes for multiple sample sizes. From http://chris-said.io/2017/05/03/empirical-bayes-for-multiple-sample-sizes/
  10. Simple Count or Frequency Encoding. From https://www.datacamp.com/community/tutorials/encoding-methodologies
  11. Transforming categorical features to numerical features. From https://tech.yandex.com/catboost/doc/dg/concepts/algorithm-main-stages_cat-to-numberic-docpage/
  12. Andrew Gelman and Jennifer Hill (2006). Data Analysis Using Regression and Multilevel/Hierarchical Models. From https://faculty.psau.edu.sa/filedownload/doc-12-pdf-a1997d0d31f84d13c1cdc44ac39a8f2c-original.pdf
- 13. Carlos Mougan, David Masip, Jordi Nin and Oriol Pujol (2021). Quantile Encoder: Tackling High Cardinality Categorical Features in Regression Problems. https://link.springer.com/chapter/10.1007%2F978-3-030-85529-1_14
+ 13. Carlos Mougan, David Masip, Jordi Nin and Oriol Pujol (2021). Quantile Encoder: Tackling High Cardinality Categorical Features in Regression Problems. Modeling Decisions for Artificial Intelligence, 2021. Springer International Publishing https://link.springer.com/chapter/10.1007%2F978-3-030-85529-1_14
  14. Gray Encoding. From https://en.wikipedia.org/wiki/Gray_code 
  15. Jacob Buckman, Aurko Roy, Colin Raffel, Ian Goodfellow: Thermometer Encoding: One Hot Way To Resist Adversarial Examples. From https://openreview.net/forum?id=S18Su--CW
+ 16. Fairness implications of encoding protected categorical attributes. Carlos Mougan, Jose Alvarez, Salvatore Ruggieri, and Steffen Staab.  In Proceedings of the 2023 AAAI/ACM Conference on AI, Ethics, and Society, AIES ’21, https://arxiv.org/abs/2201.11358
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `category_encoders-2.6.0/category_encoders/__init__.py` & `category_encoders-2.6.1/category_encoders/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from category_encoders.m_estimate import MEstimateEncoder
 from category_encoders.james_stein import JamesSteinEncoder
 from category_encoders.cat_boost import CatBoostEncoder
 from category_encoders.rankhot import RankHotEncoder
 from category_encoders.glmm import GLMMEncoder
 from category_encoders.quantile_encoder import QuantileEncoder, SummaryEncoder
 
-__version__ = '2.6.0'
+
+__version__ = '2.6.1'
 
 __author__ = "willmcginnis", "cmougan", "paulwestenthanner"
 
 __all__ = [
     "BackwardDifferenceEncoder",
     "BinaryEncoder",
     "GrayEncoder",
```

### Comparing `category_encoders-2.6.0/category_encoders/backward_difference.py` & `category_encoders-2.6.1/category_encoders/backward_difference.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/base_contrast_encoder.py` & `category_encoders-2.6.1/category_encoders/base_contrast_encoder.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/basen.py` & `category_encoders-2.6.1/category_encoders/basen.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/binary.py` & `category_encoders-2.6.1/category_encoders/binary.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/cat_boost.py` & `category_encoders-2.6.1/category_encoders/cat_boost.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/count.py` & `category_encoders-2.6.1/category_encoders/count.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/datasets/_base.py` & `category_encoders-2.6.1/category_encoders/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/datasets/data/postcode_dataset_100.csv` & `category_encoders-2.6.1/category_encoders/datasets/data/postcode_dataset_100.csv`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/glmm.py` & `category_encoders-2.6.1/category_encoders/glmm.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/gray.py` & `category_encoders-2.6.1/category_encoders/gray.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/hashing.py` & `category_encoders-2.6.1/category_encoders/hashing.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/helmert.py` & `category_encoders-2.6.1/category_encoders/helmert.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/james_stein.py` & `category_encoders-2.6.1/category_encoders/james_stein.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/leave_one_out.py` & `category_encoders-2.6.1/category_encoders/leave_one_out.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/m_estimate.py` & `category_encoders-2.6.1/category_encoders/m_estimate.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/one_hot.py` & `category_encoders-2.6.1/category_encoders/one_hot.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         options are 'error', 'return_nan', 'value', and 'indicator'. The default is 'value'.
 
         'error' will raise a `ValueError` if missings are encountered.
         'return_nan' will encode a missing value as `np.nan` in every dummy column.
         'value' will encode a missing value as 0 in every dummy column.
         'indicator' will treat missingness as its own category, adding an additional dummy column
         (whether there are missing values in the training set or not).
+        'ignore' will encode missing values as 0 in every dummy column, NOT adding an additional category.
+        
 
     Example
     -------
     >>> from category_encoders import *
     >>> import pandas as pd
     >>> from sklearn.datasets import fetch_openml
     >>> bunch = fetch_openml(name="house_prices", as_frame=True)
@@ -96,22 +98,23 @@
                          handle_unknown=handle_unknown, handle_missing=handle_missing)
         self.mapping = None
         self.ordinal_encoder = None
         self.use_cat_names = use_cat_names
 
     @property
     def category_mapping(self):
-        return self.ordinal_encoder.category_mapping
+        return self.mapping
 
     def _fit(self, X, y=None, **kwargs):
         oe_missing_strat = {
             'error': 'error',
             'return_nan': 'return_nan',
             'value': 'value',
             'indicator': 'return_nan',
+            'ignore': 'return_nan'
         }[self.handle_missing]
         self.ordinal_encoder = OrdinalEncoder(
             verbose=self.verbose,
             cols=self.cols,
             handle_unknown='value',
             handle_missing=oe_missing_strat,
         )
@@ -133,15 +136,15 @@
                 continue
 
             index = []
             new_columns = []
 
             append_nan_to_index = False
             for cat_name, class_ in values.items():
-                if pd.isna(cat_name) and self.handle_missing == 'return_nan':
+                if pd.isna(cat_name) and self.handle_missing in ['return_nan', 'ignore']:
                     # we don't want a mapping column if return_nan
                     # but do add the index to the end
                     append_nan_to_index = class_
                     continue
                 if self.use_cat_names:
                     n_col_name = f"{col}_{cat_name}"
                     found_count = found_column_counts.get(n_col_name, 0)
@@ -171,15 +174,15 @@
             if self.handle_unknown == 'value':
                 base_df.loc[-1] = 0
             elif self.handle_unknown == 'return_nan':
                 base_df.loc[-1] = np.nan
 
             if self.handle_missing == 'return_nan':
                 base_df.loc[-2] = np.nan
-            elif self.handle_missing == 'value':
+            elif self.handle_missing in ['value','ignore']:
                 base_df.loc[-2] = 0
 
             mapping.append({'col': col, 'mapping': base_df})
 
         return mapping
 
     def _transform(self, X):
```

### Comparing `category_encoders-2.6.0/category_encoders/ordinal.py` & `category_encoders-2.6.1/category_encoders/ordinal.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,19 +216,25 @@
                 if handle_missing == 'return_nan':
                     X[column] = X[column].map(return_nan_series).where(X[column] == -2, X[column])
 
         else:
             mapping_out = []
             for col in cols:
                 nan_identity = np.nan
-                categories = list(X[col].unique())
+                categories = X[col].unique()
+                # make nan last category
+                if pd.isna(categories).any():
+                    categories = [c for c in categories if not pd.isna(c)] + [nan_identity]
+                else:
+                    categories = categories.tolist()
                 if util.is_category(X[col].dtype):
                     # Avoid using pandas category dtype meta-data if possible, see #235, #238.
                     if X[col].dtype.ordered:
-                        categories = [c for c in X[col].dtype.categories if c in categories]
+                        category_set = set(categories)  # convert to set for faster membership checks c.f. #407
+                        categories = [c for c in X[col].dtype.categories if c in category_set]
                     if X[col].isna().any():
                         categories += [np.nan]
 
                 index = pd.Series(categories).fillna(nan_identity).unique()
 
                 data = pd.Series(index=index, data=range(1, len(index) + 1))
```

### Comparing `category_encoders-2.6.0/category_encoders/polynomial.py` & `category_encoders-2.6.1/category_encoders/polynomial.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/quantile_encoder.py` & `category_encoders-2.6.1/category_encoders/quantile_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -249,15 +249,14 @@
         self.cols = cols
         self.use_default_cols = cols is None  # if True, even a repeated call of fit() will select string columns from X
         self.ordinal_encoder = None
         self._dim = None
         self.mapping = None
         self.handle_unknown = handle_unknown
         self.handle_missing = handle_missing
-        self.feature_names_out_ = None
         self.quantiles = quantiles
         self.m = m
         self.encoder_list = None
 
     def fit(self, X, y):
         """Fits the encoder according to X and y by fitting the individual encoders.
 
@@ -274,14 +273,16 @@
         -------
 
         self : encoder
             Returns self.
 
         """
         X, y = util.convert_inputs(X, y)
+        self.feature_names_in_ = X.columns.tolist()
+        self.n_features_in_ = len(self.feature_names_in_)
 
         if self.use_default_cols:
             self.cols = util.get_obj_cols(X)
         else:
             self.cols = util.convert_cols_to_list(self.cols)
 
         rounded_percentiles = [round(quantile * 100) for quantile in self.quantiles]
@@ -339,36 +340,44 @@
             return transformed_df.values
 
     def get_feature_names(self) -> List[str]:
         warnings.warn("`get_feature_names` is deprecated in all of sklearn. Use `get_feature_names_out` instead.",
                       category=FutureWarning)
         return self.get_feature_names_out()
 
-    def get_feature_names_out(self):
+    def get_feature_names_out(self, input_features=None) -> np.ndarray:
         """
         Returns the names of all transformed / added columns.
+
+        Note that in sklearn the get_feature_names_out function takes the feature_names_in as an argument
+        and determines the output feature names using the input. A fit is usually not necessary and if so a
+        NotFittedError is raised.
+        We just require a fit all the time and return the fitted output columns.
+
         Returns
         -------
-        feature_names: list
+        feature_names: np.ndarray
             A list with all feature names transformed or added.
-            Note: potentially dropped features are not included!
-        """
+            Note: potentially dropped features (because the feature is constant/invariant) are not included!
 
-        if not isinstance(self.feature_names_out_, list):
-            raise NotFittedError("Must fit data first. Affected feature names are not known before.")
+        """
+        out_feats = getattr(self, "feature_names_out_", None)
+        if not isinstance(out_feats, list):
+            raise NotFittedError("Estimator has to be fitted to return feature names.")
         else:
-            return self.feature_names_out_
+            return np.array(out_feats, dtype=object)
 
     def get_feature_names_in(self) -> List[str]:
         """
         Returns the names of all input columns present when fitting.
         These columns are necessary for the transform step.
-       """
-        if not isinstance(self.cols, list):
+        """
+        in_feats = getattr(self, "feature_names_in_", None)
+        if not isinstance(in_feats, list):
             raise NotFittedError("Estimator has to be fitted to return feature names.")
         else:
-            return self.cols
+            return in_feats
 
     @staticmethod
     def _get_col_name(col: str, quantile: float) -> str:
         percentile = round(quantile * 100)
         return f"{col}_{percentile}"
```

### Comparing `category_encoders-2.6.0/category_encoders/rankhot.py` & `category_encoders-2.6.1/category_encoders/rankhot.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 
             if len(values) == 0:
                 continue
 
             index = []
             new_columns = []
 
-            for cat_name, class_ in values.iteritems():
+            for cat_name, class_ in values.items():
                 if self.use_cat_names:
                     n_col_name = f"{col}_{cat_name}"
                     found_count = found_column_counts.get(n_col_name, 0)
                     found_column_counts[n_col_name] = found_count + 1
                     n_col_name += "#" * found_count
                 else:
                     n_col_name = f"{col}_{class_}"
```

### Comparing `category_encoders-2.6.0/category_encoders/sum_coding.py` & `category_encoders-2.6.1/category_encoders/sum_coding.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/target_encoder.py` & `category_encoders-2.6.1/category_encoders/target_encoder.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/utils.py` & `category_encoders-2.6.1/category_encoders/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,17 @@
     X_alt_index = y.index if isinstance(y, pd.Series) else index
     X = convert_input(X, columns=columns, deep=deep, index=X_alt_index)
     if y is not None:
         y = convert_input_vector(y, index=X.index)
         # N.B.: If either was already pandas, it keeps its index.
 
         if any(X.index != y.index):
-            raise ValueError("`X` and `y` both have indexes, but they do not match.")
+            msg = "`X` and `y` both have indexes, but they do not match. If you are shuffling your input data on " \
+                  "purpose (e.g. via permutation_test_score) use np arrays instead of data frames / series"
+            raise ValueError(msg)
         if X.shape[0] != y.shape[0]:
             raise ValueError("The length of X is " + str(X.shape[0]) + " but length of y is " + str(y.shape[0]) + ".")
     return X, y
 
 
 def convert_input(X, columns=None, deep=False, index=None):
     """
@@ -220,15 +222,14 @@
     cols: List[str]
     use_default_cols: bool
     handle_missing: str
     handle_unknown: str
     verbose: int
     drop_invariant: bool
     invariant_cols: List[str] = []
-    feature_names_out_: Union[None, List[str]] = None
     return_df: bool
     supervised: bool
     encoding_relation: EncodingRelation
 
     INVARIANCE_THRESHOLD = 10e-5  # columns with variance less than this will be considered constant / invariant
 
     def __init__(self, verbose=0, cols=None, drop_invariant=False, return_df=True,
@@ -260,16 +261,15 @@
             additional encoder specific parameters like regularisation.
         """
         self.return_df = return_df
         self.drop_invariant = drop_invariant
         self.invariant_cols = []
         self.verbose = verbose
         self.use_default_cols = cols is None  # if True, even a repeated call of fit() will select string columns from X
-        self.cols = cols  # This cannot be called `feature_names_in_` since it is a parameter. This does not feel right
-        self.feature_names_out_ = None
+        self.cols = cols  # note that cols are only the columns to be encoded, feature_names_in_ are all columns
         self.mapping = None
         self.handle_unknown = handle_unknown
         self.handle_missing = handle_missing
         self._dim = None
 
     def fit(self, X, y=None, **kwargs):
         """Fits the encoder according to X and y.
@@ -288,14 +288,16 @@
 
         self : encoder
             Returns self.
 
         """
         self._check_fit_inputs(X, y)
         X, y = convert_inputs(X, y)
+        self.feature_names_in_ = X.columns.tolist()
+        self.n_features_in_ = len(self.feature_names_in_)
 
         self._dim = X.shape[1]
         self._determine_fit_columns(X)
 
         if not set(self.cols).issubset(X.columns):
             raise ValueError('X does not contain the columns listed in cols')
 
@@ -357,39 +359,46 @@
             self.cols = convert_cols_to_list(self.cols)
 
     def get_feature_names(self) -> List[str]:
         warnings.warn("`get_feature_names` is deprecated in all of sklearn. Use `get_feature_names_out` instead.",
                       category=FutureWarning)
         return self.get_feature_names_out()
 
-    def get_feature_names_out(self) -> List[str]:
+    def get_feature_names_out(self, input_features=None) -> np.ndarray:
         """
         Returns the names of all transformed / added columns.
 
+        Note that in sklearn the get_feature_names_out function takes the feature_names_in as an argument
+        and determines the output feature names using the input. A fit is usually not necessary and if so a
+        NotFittedError is raised.
+        We just require a fit all the time and return the fitted output columns.
+
         Returns
         -------
-        feature_names: list
-            A list with all feature names transformed or added.
+        feature_names: np.ndarray
+            A numpy array with all feature names transformed or added.
             Note: potentially dropped features (because the feature is constant/invariant) are not included!
 
         """
-        if not isinstance(self.feature_names_out_, list):
+        out_feats = getattr(self, "feature_names_out_", None)
+        if not isinstance(out_feats, list):
             raise NotFittedError("Estimator has to be fitted to return feature names.")
         else:
-            return self.feature_names_out_
+            return np.array(out_feats, dtype=object)
 
     def get_feature_names_in(self) -> List[str]:
         """
         Returns the names of all input columns present when fitting.
         These columns are necessary for the transform step.
-       """
-        if not isinstance(self.cols, list):
+        """
+        in_feats = getattr(self, "feature_names_in_", None)
+        if not isinstance(in_feats, list):
             raise NotFittedError("Estimator has to be fitted to return feature names.")
         else:
-            return self.cols
+            return in_feats
 
     @abstractmethod
     def _fit(self, X: pd.DataFrame, y: Optional[pd.Series], **kwargs):
         ...
 
 
 class SupervisedTransformerMixin(sklearn.base.TransformerMixin):
```

### Comparing `category_encoders-2.6.0/category_encoders/woe.py` & `category_encoders-2.6.1/category_encoders/woe.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders/wrapper.py` & `category_encoders-2.6.1/category_encoders/wrapper.py`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/category_encoders.egg-info/PKG-INFO` & `category_encoders-2.6.1/category_encoders.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: category-encoders
-Version: 2.6.0
+Version: 2.6.1
 Summary: A collection of sklearn transformers to encode categorical variables as numeric
 Home-page: https://github.com/scikit-learn-contrib/category_encoders
 Author: Will McGinnis
 Author-email: will@pedalwrencher.com
 License: BSD
-Download-URL: https://github.com/scikit-learn-contrib/category_encoders/tarball/2.6.0
+Download-URL: https://github.com/scikit-learn-contrib/category_encoders/tarball/2.6.1
 Description: Categorical Encoding Methods
         ============================
         
         [![Downloads](https://pepy.tech/badge/category-encoders)](https://pepy.tech/project/category-encoders)
         [![Downloads](https://pepy.tech/badge/category-encoders/month)](https://pepy.tech/project/category-encoders)
         ![Test Suite and Linting](https://github.com/scikit-learn-contrib/category_encoders/workflows/Test%20Suite%20and%20Linting/badge.svg)
         [![DOI](https://zenodo.org/badge/47077067.svg)](https://zenodo.org/badge/latestdoi/47077067)
@@ -153,17 +153,18 @@
          6. BaseN Encoding and Grid Search in categorical variables. From http://www.willmcginnis.com/2016/12/18/basen-encoding-grid-search-category_encoders/
          7. Daniele Miccii-Barreca (2001). A Preprocessing Scheme for High-Cardinality Categorical Attributes in Classification and Prediction Problems. SIGKDD Explor. Newsl. 3, 1. From http://dx.doi.org/10.1145/507533.507538
          8. Weight of Evidence (WOE) and Information Value Explained. From https://www.listendata.com/2015/03/weight-of-evidence-woe-and-information.html
          9. Empirical Bayes for multiple sample sizes. From http://chris-said.io/2017/05/03/empirical-bayes-for-multiple-sample-sizes/
          10. Simple Count or Frequency Encoding. From https://www.datacamp.com/community/tutorials/encoding-methodologies
          11. Transforming categorical features to numerical features. From https://tech.yandex.com/catboost/doc/dg/concepts/algorithm-main-stages_cat-to-numberic-docpage/
          12. Andrew Gelman and Jennifer Hill (2006). Data Analysis Using Regression and Multilevel/Hierarchical Models. From https://faculty.psau.edu.sa/filedownload/doc-12-pdf-a1997d0d31f84d13c1cdc44ac39a8f2c-original.pdf
-         13. Carlos Mougan, David Masip, Jordi Nin and Oriol Pujol (2021). Quantile Encoder: Tackling High Cardinality Categorical Features in Regression Problems. https://link.springer.com/chapter/10.1007%2F978-3-030-85529-1_14
+         13. Carlos Mougan, David Masip, Jordi Nin and Oriol Pujol (2021). Quantile Encoder: Tackling High Cardinality Categorical Features in Regression Problems. Modeling Decisions for Artificial Intelligence, 2021. Springer International Publishing https://link.springer.com/chapter/10.1007%2F978-3-030-85529-1_14
          14. Gray Encoding. From https://en.wikipedia.org/wiki/Gray_code 
          15. Jacob Buckman, Aurko Roy, Colin Raffel, Ian Goodfellow: Thermometer Encoding: One Hot Way To Resist Adversarial Examples. From https://openreview.net/forum?id=S18Su--CW
+         16. Fairness implications of encoding protected categorical attributes. Carlos Mougan, Jose Alvarez, Salvatore Ruggieri, and Steffen Staab.  In Proceedings of the 2023 AAAI/ACM Conference on AI, Ethics, and Society, AIES ’21, https://arxiv.org/abs/2201.11358
         
 Keywords: python data science machine learning pandas sklearn
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `category_encoders-2.6.0/category_encoders.egg-info/SOURCES.txt` & `category_encoders-2.6.1/category_encoders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `category_encoders-2.6.0/setup.py` & `category_encoders-2.6.1/setup.py`

 * *Files identical despite different names*

