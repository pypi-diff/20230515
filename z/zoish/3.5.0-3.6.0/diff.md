# Comparing `tmp/zoish-3.5.0.tar.gz` & `tmp/zoish-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoish-3.5.0.tar", max compression
+gzip compressed data, was "zoish-3.6.0.tar", max compression
```

## Comparing `zoish-3.5.0.tar` & `zoish-3.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1323 2023-04-20 18:05:36.346876 zoish-3.5.0/LICENSE
--rw-r--r--   0        0        0    10737 2023-04-20 18:05:36.347039 zoish-3.5.0/README.md
--rw-r--r--   0        0        0     1264 2023-04-25 22:23:05.050109 zoish-3.5.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-04-20 18:05:36.358370 zoish-3.5.0/zoish/.env
--rw-r--r--   0        0        0      925 2023-04-25 22:23:05.051109 zoish-3.5.0/zoish/__init__.py
--rw-r--r--   0        0        0     1938 2023-04-20 18:05:36.358804 zoish-3.5.0/zoish/abstracs/feature_selector_abstracts.py
--rw-r--r--   0        0        0    60046 2023-04-20 18:05:36.359334 zoish-3.5.0/zoish/base_classes/best_estimator_getters.py
--rw-r--r--   0        0        0      675 2023-04-20 18:05:36.359553 zoish-3.5.0/zoish/config.yaml
--rw-r--r--   0        0        0      375 2023-04-20 18:05:36.359847 zoish-3.5.0/zoish/decorators/decorators.py
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.360014 zoish-3.5.0/zoish/examples/__init__.py
--rw-r--r--   0        0        0    54613 2023-04-20 18:05:36.361103 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb
--rw-r--r--   0        0        0    42652 2023-04-20 18:05:36.361831 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61640 2023-04-20 18:05:36.362393 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb
--rw-r--r--   0        0        0    97297 2023-04-20 18:05:36.362969 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0   114986 2023-04-20 18:05:36.363251 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb
--rw-r--r--   0        0        0    20432 2023-04-20 18:05:36.363794 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb
--rw-r--r--   0        0        0    40581 2023-04-20 18:05:36.364116 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    63450 2023-04-20 18:05:36.364446 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb
--rw-r--r--   0        0        0    56051 2023-04-20 18:05:36.364756 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0    71923 2023-04-20 18:05:36.365059 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb
--rw-r--r--   0        0        0    22310 2023-04-20 18:05:36.365292 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb
--rw-r--r--   0        0        0    53217 2023-04-20 18:05:36.365575 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61941 2023-04-20 18:05:36.366026 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb
--rw-r--r--   0        0        0   102159 2023-04-20 18:05:36.366576 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb
--rw-r--r--   0        0        0   118140 2023-04-20 18:05:36.366880 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.367139 zoish-3.5.0/zoish/examples/shap/__init__.py
--rw-r--r--   0        0        0    21194 2023-04-20 18:05:36.369666 zoish-3.5.0/zoish/examples/shap/shap_grid_search_classification.ipynb
--rw-r--r--   0        0        0    58856 2023-04-20 18:05:36.370122 zoish-3.5.0/zoish/examples/shap/shap_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61444 2023-04-20 18:05:36.373990 zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_1.ipynb
--rw-r--r--   0        0        0   413648 2023-04-20 18:05:36.376447 zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_2.ipynb
--rw-r--r--   0        0        0   465032 2023-04-20 18:05:36.396730 zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_3.ipynb
--rw-r--r--   0        0        0    88426 2023-04-20 18:05:36.397119 zoish-3.5.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0    69117 2023-04-20 18:05:36.397585 zoish-3.5.0/zoish/examples/shap/shap_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.397811 zoish-3.5.0/zoish/examples/single_feature/__init__.py
--rw-r--r--   0        0        0    40086 2023-04-20 18:05:36.398323 zoish-3.5.0/zoish/examples/single_feature/single_grid_search_classification.ipynb
--rw-r--r--   0        0        0    45581 2023-04-20 18:05:36.398779 zoish-3.5.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    85377 2023-04-20 18:05:36.399183 zoish-3.5.0/zoish/examples/single_feature/single_random_search_classification.ipynb
--rw-r--r--   0        0        0   106211 2023-04-20 18:05:36.399543 zoish-3.5.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb
--rw-r--r--   0        0        0   122582 2023-04-20 18:05:36.399841 zoish-3.5.0/zoish/examples/single_feature/single_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.399998 zoish-3.5.0/zoish/factories/factories.py
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.400140 zoish-3.5.0/zoish/feature_selectors/__init__.py
--rw-r--r--   0        0        0    85614 2023-04-20 18:05:36.400421 zoish-3.5.0/zoish/feature_selectors/recursive_feature_addition.py
--rw-r--r--   0        0        0    85793 2023-04-20 18:05:36.402572 zoish-3.5.0/zoish/feature_selectors/recursive_feature_elimination.py
--rw-r--r--   0        0        0    85872 2023-04-20 18:05:36.403025 zoish-3.5.0/zoish/feature_selectors/select_by_shuffling.py
--rw-r--r--   0        0        0   100851 2023-04-20 18:05:36.403301 zoish-3.5.0/zoish/feature_selectors/shap_selectors.py
--rw-r--r--   0        0        0    86006 2023-04-20 18:05:36.403660 zoish-3.5.0/zoish/feature_selectors/single_feature_selectors.py
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.403823 zoish-3.5.0/zoish/logs/zoish.log
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.403960 zoish-3.5.0/zoish/mediators/mediators.py
--rw-r--r--   0        0        0       95 2023-04-20 18:05:36.404077 zoish-3.5.0/zoish/project_conf.py
--rw-r--r--   0        0        0       48 2023-04-25 22:23:05.052109 zoish-3.5.0/zoish/version.py
--rw-r--r--   0        0        0    12279 1970-01-01 00:00:00.000000 zoish-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-04-20 18:05:36.346876 zoish-3.6.0/LICENSE
+-rw-r--r--   0        0        0    10737 2023-04-20 18:05:36.347039 zoish-3.6.0/README.md
+-rw-r--r--   0        0        0     1264 2023-05-15 19:51:17.906386 zoish-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-04-20 18:05:36.358370 zoish-3.6.0/zoish/.env
+-rw-r--r--   0        0        0      925 2023-05-15 19:51:17.906386 zoish-3.6.0/zoish/__init__.py
+-rw-r--r--   0        0        0     1938 2023-04-20 18:05:36.358804 zoish-3.6.0/zoish/abstracs/feature_selector_abstracts.py
+-rw-r--r--   0        0        0    60046 2023-04-20 18:05:36.359334 zoish-3.6.0/zoish/base_classes/best_estimator_getters.py
+-rw-r--r--   0        0        0      675 2023-04-20 18:05:36.359553 zoish-3.6.0/zoish/config.yaml
+-rw-r--r--   0        0        0      375 2023-04-20 18:05:36.359847 zoish-3.6.0/zoish/decorators/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.360014 zoish-3.6.0/zoish/examples/__init__.py
+-rw-r--r--   0        0        0    54613 2023-04-20 18:05:36.361103 zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    42652 2023-04-20 18:05:36.361831 zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61640 2023-04-20 18:05:36.362393 zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb
+-rw-r--r--   0        0        0    97297 2023-04-20 18:05:36.362969 zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0   114986 2023-04-20 18:05:36.363251 zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb
+-rw-r--r--   0        0        0    20432 2023-04-20 18:05:36.363794 zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    40581 2023-04-20 18:05:36.364116 zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    63450 2023-04-20 18:05:36.364446 zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb
+-rw-r--r--   0        0        0    56051 2023-04-20 18:05:36.364756 zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0    71923 2023-04-20 18:05:36.365059 zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb
+-rw-r--r--   0        0        0    22310 2023-04-20 18:05:36.365292 zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    53217 2023-04-20 18:05:36.365575 zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61941 2023-04-20 18:05:36.366026 zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb
+-rw-r--r--   0        0        0   102159 2023-04-20 18:05:36.366576 zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb
+-rw-r--r--   0        0        0   118140 2023-04-20 18:05:36.366880 zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.367139 zoish-3.6.0/zoish/examples/shap/__init__.py
+-rw-r--r--   0        0        0    21194 2023-04-20 18:05:36.369666 zoish-3.6.0/zoish/examples/shap/shap_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    58856 2023-04-20 18:05:36.370122 zoish-3.6.0/zoish/examples/shap/shap_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61444 2023-04-20 18:05:36.373990 zoish-3.6.0/zoish/examples/shap/shap_random_search_classification_1.ipynb
+-rw-r--r--   0        0        0   413648 2023-04-20 18:05:36.376447 zoish-3.6.0/zoish/examples/shap/shap_random_search_classification_2.ipynb
+-rw-r--r--   0        0        0   465032 2023-04-20 18:05:36.396730 zoish-3.6.0/zoish/examples/shap/shap_random_search_classification_3.ipynb
+-rw-r--r--   0        0        0    88426 2023-04-20 18:05:36.397119 zoish-3.6.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0    69117 2023-04-20 18:05:36.397585 zoish-3.6.0/zoish/examples/shap/shap_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.397811 zoish-3.6.0/zoish/examples/single_feature/__init__.py
+-rw-r--r--   0        0        0    40086 2023-04-20 18:05:36.398323 zoish-3.6.0/zoish/examples/single_feature/single_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    45581 2023-04-20 18:05:36.398779 zoish-3.6.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    85377 2023-04-20 18:05:36.399183 zoish-3.6.0/zoish/examples/single_feature/single_random_search_classification.ipynb
+-rw-r--r--   0        0        0   106211 2023-04-20 18:05:36.399543 zoish-3.6.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb
+-rw-r--r--   0        0        0   122582 2023-04-20 18:05:36.399841 zoish-3.6.0/zoish/examples/single_feature/single_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.399998 zoish-3.6.0/zoish/factories/factories.py
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.400140 zoish-3.6.0/zoish/feature_selectors/__init__.py
+-rw-r--r--   0        0        0    85614 2023-04-20 18:05:36.400421 zoish-3.6.0/zoish/feature_selectors/recursive_feature_addition.py
+-rw-r--r--   0        0        0    85793 2023-04-20 18:05:36.402572 zoish-3.6.0/zoish/feature_selectors/recursive_feature_elimination.py
+-rw-r--r--   0        0        0    85872 2023-04-20 18:05:36.403025 zoish-3.6.0/zoish/feature_selectors/select_by_shuffling.py
+-rw-r--r--   0        0        0   100851 2023-04-20 18:05:36.403301 zoish-3.6.0/zoish/feature_selectors/shap_selectors.py
+-rw-r--r--   0        0        0    86006 2023-04-20 18:05:36.403660 zoish-3.6.0/zoish/feature_selectors/single_feature_selectors.py
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.403823 zoish-3.6.0/zoish/logs/zoish.log
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.403960 zoish-3.6.0/zoish/mediators/mediators.py
+-rw-r--r--   0        0        0       95 2023-04-20 18:05:36.404077 zoish-3.6.0/zoish/project_conf.py
+-rw-r--r--   0        0        0       48 2023-05-15 19:51:17.906386 zoish-3.6.0/zoish/version.py
+-rw-r--r--   0        0        0    12279 1970-01-01 00:00:00.000000 zoish-3.6.0/PKG-INFO
```

### Comparing `zoish-3.5.0/LICENSE` & `zoish-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/README.md` & `zoish-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/pyproject.toml` & `zoish-3.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zoish"
-version = "3.5.0"
+version = "3.6.0"
 description = "Zoish: Automated feature selectoion tools"
 
 authors = ["drhosseinjavedani <h.javedani@gmail.com>"]
 homepage = "https://github.com/drhosseinjavedani/zoish"
 license = "BSD 2-Clause License"
 
 readme = "README.md"
```

### Comparing `zoish-3.5.0/zoish/__init__.py` & `zoish-3.6.0/zoish/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.5.0"
+__version__ = "3.6.0"
 
 import logging
 import logging.config
 import os
 
 import yaml
 from dotenv import load_dotenv
```

### Comparing `zoish-3.5.0/zoish/abstracs/feature_selector_abstracts.py` & `zoish-3.6.0/zoish/abstracs/feature_selector_abstracts.py`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/base_classes/best_estimator_getters.py` & `zoish-3.6.0/zoish/base_classes/best_estimator_getters.py`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/config.yaml` & `zoish-3.6.0/zoish/config.yaml`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb` & `zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb` & `zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb` & `zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb` & `zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb` & `zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb` & `zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb` & `zoish-3.6.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/shap/shap_grid_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/shap/shap_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/shap/shap_optuna_search_regression.ipynb` & `zoish-3.6.0/zoish/examples/shap/shap_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_1.ipynb` & `zoish-3.6.0/zoish/examples/shap/shap_random_search_classification_1.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_2.ipynb` & `zoish-3.6.0/zoish/examples/shap/shap_random_search_classification_2.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_3.ipynb` & `zoish-3.6.0/zoish/examples/shap/shap_random_search_classification_3.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb` & `zoish-3.6.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/shap/shap_tune_search_regression.ipynb` & `zoish-3.6.0/zoish/examples/shap/shap_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/single_feature/single_grid_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/single_feature/single_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb` & `zoish-3.6.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/single_feature/single_random_search_classification.ipynb` & `zoish-3.6.0/zoish/examples/single_feature/single_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb` & `zoish-3.6.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/examples/single_feature/single_tune_search_regression.ipynb` & `zoish-3.6.0/zoish/examples/single_feature/single_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/feature_selectors/recursive_feature_addition.py` & `zoish-3.6.0/zoish/feature_selectors/recursive_feature_addition.py`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/feature_selectors/recursive_feature_elimination.py` & `zoish-3.6.0/zoish/feature_selectors/recursive_feature_elimination.py`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/feature_selectors/select_by_shuffling.py` & `zoish-3.6.0/zoish/feature_selectors/select_by_shuffling.py`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/feature_selectors/shap_selectors.py` & `zoish-3.6.0/zoish/feature_selectors/shap_selectors.py`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/zoish/feature_selectors/single_feature_selectors.py` & `zoish-3.6.0/zoish/feature_selectors/single_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `zoish-3.5.0/PKG-INFO` & `zoish-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoish
-Version: 3.5.0
+Version: 3.6.0
 Summary: Zoish: Automated feature selectoion tools
 Home-page: https://github.com/drhosseinjavedani/zoish
 License: BSD 2-Clause License
 Keywords: Auto ML,Feature Selection,Pipeline,Machine learning,shap
 Author: drhosseinjavedani
 Author-email: h.javedani@gmail.com
 Requires-Python: >=3.8,<3.11
```

