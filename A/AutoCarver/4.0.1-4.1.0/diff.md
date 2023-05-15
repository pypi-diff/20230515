# Comparing `tmp/AutoCarver-4.0.1.tar.gz` & `tmp/AutoCarver-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoCarver-4.0.1.tar", last modified: Sun May 14 14:17:14 2023, max compression
+gzip compressed data, was "dist\AutoCarver-4.1.0.tar", last modified: Mon May 15 17:51:59 2023, max compression
```

## Comparing `AutoCarver-4.0.1.tar` & `AutoCarver-4.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver/
--rw-rw-rw-   0        0        0    22800 2023-05-14 14:15:32.000000 AutoCarver-4.0.1/AutoCarver/AutoCarver.py
--rw-rw-rw-   0        0        0    50746 2023-05-14 14:15:32.000000 AutoCarver-4.0.1/AutoCarver/Discretizers.py
--rw-rw-rw-   0        0        0    14207 2023-01-28 13:57:43.000000 AutoCarver-4.0.1/AutoCarver/FeatureSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-09 19:45:37.000000 AutoCarver-4.0.1/AutoCarver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/
--rw-rw-rw-   0        0        0     8312 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8312 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6346 2023-04-12 10:19:04.000000 AutoCarver-4.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-14 14:15:44.000000 AutoCarver-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/
+drwxrwxrwx   0        0        0        0 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/AutoCarver/
+-rw-rw-rw-   0        0        0    22860 2023-05-15 17:49:41.000000 AutoCarver-4.1.0/AutoCarver/AutoCarver.py
+-rw-rw-rw-   0        0        0    51141 2023-05-15 17:25:48.000000 AutoCarver-4.1.0/AutoCarver/Discretizers.py
+-rw-rw-rw-   0        0        0    16742 2023-05-15 07:01:19.000000 AutoCarver-4.1.0/AutoCarver/FeatureSelector.py
+-rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.1.0/AutoCarver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/AutoCarver.egg-info/
+-rw-rw-rw-   0        0        0     7119 2023-05-15 17:51:52.000000 AutoCarver-4.1.0/AutoCarver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-05-15 17:51:57.000000 AutoCarver-4.1.0/AutoCarver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 17:51:52.000000 AutoCarver-4.1.0/AutoCarver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 17:51:52.000000 AutoCarver-4.1.0/AutoCarver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7119 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 17:51:59.000000 AutoCarver-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-15 17:20:11.000000 AutoCarver-4.1.0/setup.py
```

### Comparing `AutoCarver-4.0.1/AutoCarver/AutoCarver.py` & `AutoCarver-4.1.0/AutoCarver/AutoCarver.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     pipe = Pipeline(pipe)
 
     # applying pipe to a validation set or in production
     X_val = pipe.transform(X_val)
 
     """
    
-    def __init__(self, values_orders: Dict[str, Any]={}, *, sort_by: str='tschuprowt',
+    def __init__(self, values_orders: Dict[str, Any], *, sort_by: str='tschuprowt',
                  copy: bool=False, max_n_mod: int=5, dropna: bool=True,
                  verbose: bool=True) -> None:
         
         self.features = list(values_orders.keys())
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.non_viable_features: List[str] = []  # list of features non viable features
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
@@ -493,26 +493,27 @@
     """ Computes measures of association between feature x and feature2. """
 
     # numnber of observations
     n_obs = xtab.sum().sum()
 
     # number of values taken by the features
     n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
+    min_n_mod = min(n_mod_x, n_mod_y)
 
     # Chi2 statistic
     chi2 = chi2_contingency(xtab)[0]
 
     # Cramer's V
-    cramerv = sqrt(chi2 / n_obs)
+    cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
 
     # Tschuprow's T
-    n_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
+    dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
     tschuprowt = 0
-    if n_mods > 0:
-        tschuprowt = sqrt(chi2 / n_obs / n_mods)
+    if dof_mods > 0:
+        tschuprowt = sqrt(chi2 / n_obs / dof_mods)
 
     results = {'cramerv': cramerv, 'tschuprowt': tschuprowt}
     
     return results
 
 def nan_crosstab(x: Series, y: Series):
     """ Crosstab that keeps nans as a specific value"""
```

### Comparing `AutoCarver-4.0.1/AutoCarver/Discretizers.py` & `AutoCarver-4.1.0/AutoCarver/Discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
      - [Qualitative ordinal features] user-specified order.
 
     Parameters
     ----------
     features: list
         Contains qualitative (categorical and categorical ordinal) features to be discretized.
 
-    min_freq: int, default None
+    min_freq: int
         [Qualitative features] Minimal frequency of a modality.
          - NaNs are considered a specific modality but will not be grouped.
          - [Qualitative features] Less frequent modalities are grouped in the `__OTHER__` modality.
          - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
         (smallest frequency or closest target rate), between the superior and inferior values (specified
         in the `values_orders` dictionnary).
         Recommandation: `min_freq` should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
@@ -255,15 +255,15 @@
         [Qualitative ordinal features] dict of features values and list of orders of their values.
          - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
     
-    def __init__(self, features: List[str], min_freq: float=None, 
+    def __init__(self, features: List[str], min_freq: float, *,
                  values_orders: Dict[str, Any]={}, copy: bool=False, 
                  verbose: bool=False, dropna: bool=False) -> None:
     
         self.features = features[:]
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.ordinal_features = [f for f in values_orders if f in features]
         self.non_ordinal_features = [f for f in features if f not in self.ordinal_features]
@@ -316,14 +316,15 @@
             self.pipe += [('QualitativeClosestDiscretizer', discretizer)]  # adding discretizer to pipe
 
         # [Qualitative non-ordinal features] Grouping rare values into default_value '__OTHER__'
         if len(self.non_ordinal_features) > 0:
 
             # Grouping rare modalities
             discretizer = DefaultDiscretizer(self.non_ordinal_features, min_freq=self.min_freq, 
+                                             values_orders=self.values_orders,
                                              verbose=self.verbose, dropna=self.dropna)
             discretizer.fit(Xc, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
             self.pipe += [('DefaultDiscretizer', discretizer)]  # adding discretizer to pipe
 
@@ -361,19 +362,19 @@
         cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
         Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
         cut in q=5 quantiles.
         Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
 
     """
     
-    def __init__(self, features: List[str], q: int=None, copy: bool=False, 
+    def __init__(self, features: List[str], q: int, *, values_orders: Dict[str, Any]={}, copy: bool=False, 
                  verbose: bool=False, dropna: bool=False) -> None:
         
         self.features = features[:]
-        self.values_orders: Dict[str, GroupedList] = {}
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.q = q
         self.pipe: List[BaseEstimator] = []
         self.copy = copy
         self.verbose = verbose
     
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """ Checking data for bucketization"""
@@ -393,17 +394,17 @@
         return Xc
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """ Learning TRAIN distribution"""
         
         # checking data before bucketization
         Xc = self.prepare_data(X, y)
-        
+
         # [Quantitative features] Grouping values into quantiles
-        discretizer = QuantileDiscretizer(self.features, q=self.q, verbose=self.verbose)
+        discretizer = QuantileDiscretizer(self.features, q=self.q, values_orders=self.values_orders, verbose=self.verbose)
         Xc = discretizer.fit_transform(Xc, y)
 
         # storing results
         self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
         self.pipe += [('QuantileDiscretizer', discretizer)]  # adding discretizer to pipe
 
         # [Quantitative features] Grouping rare quantiles into closest common one
@@ -483,15 +484,15 @@
         [Qualitative ordinal features] dict of features values and list of orders of their values.
          - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
 
-    def __init__(self, quanti_features: List[str], quali_features: List[str], q: int=None, min_freq: float=None, 
+    def __init__(self, quanti_features: List[str], quali_features: List[str], q: int, min_freq: float, *, 
                  values_orders: Dict[str, Any]={}, copy: bool=False, verbose: bool=False, dropna: bool=False) -> None:
 
         self.features = quanti_features[:] + quali_features[:]
         self.quanti_features = quanti_features[:]
         self.quali_features = quali_features[:]
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.min_freq = min_freq
@@ -527,15 +528,16 @@
 
             # verbose if requested
             if self.verbose:
                 print("\n---\n[Discretizer] Fit Quantitative Features")
 
             # grouping quantitative features
             discretizer = QuantitativeDiscretizer(
-                self.quanti_features, q=self.q, copy=self.copy,
+                self.quanti_features, q=self.q,
+                values_orders=self.values_orders, copy=self.copy,
                 verbose=self.verbose, dropna=self.dropna
             )
             discretizer.fit(X, y)
 
             # storing results
             self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
             self.pipe += discretizer.pipe  # adding discretizer to pipe
@@ -561,15 +563,15 @@
 
 
 class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
     
     def __init__(self, values_orders: Dict[str, Any], *, copy: bool=False, output: type= float, verbose: bool=False) -> None:
         
         self.features = list(values_orders.keys())
-        self.values_orders = {feature: GroupedList(order) for feature, order in values_orders.items()}
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.copy = copy
         self.output = output
         self.verbose = verbose
         
     def fit(self, X, y=None) -> None:
         """ Does nothing, info is found in values_orders"""
 
@@ -662,20 +664,22 @@
         super().__init__(self.values_orders, copy=self.copy, output=str)
         super().fit(X, y)
             
         return self
 
 class QuantileDiscretizer(BaseEstimator, TransformerMixin):
     
-    def __init__(self, features: List[str], q: int, copy: bool=False, verbose: bool=False) -> None:
+    def __init__(self, features: List[str], q: int, *, 
+    	         values_orders: Dict[str, Any]={},
+                 copy: bool=False, verbose: bool=False) -> None:
         """ Discretizes quantitative features into groups of q quantiles"""
         
         self.features = features[:]
         self.q = q
-        self.values_orders: Dict[str, any] = {}
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.quantiles: Dict[str, Any] = {}
         self.copy = copy
         self.verbose = verbose
 
     def fit(self, X: DataFrame, y: Series=None) -> None:
         
         # computing quantiles for the feature
@@ -760,15 +764,15 @@
         # grouping rare modalities for each feature
         common_modalities = X[self.features].apply(
             lambda u: find_common_modalities(u, y, self.min_freq, self.values_orders.get(u.name)), 
             axis=0, result_type='expand'
         ).T.to_dict()
 
         # updating the order per feature
-        self.values_orders = {f: common_modalities.get('order').get(f) for f in self.features}
+        self.values_orders.update({f: common_modalities.get('order').get(f) for f in self.features})
 
         # defining the default value based on the strategy
         self.default_values = {f: common_modalities.get(self.default).get(f) for f in self.features}
 
         return self
     
     def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
@@ -776,15 +780,18 @@
         # copying dataset if requested
         Xc = X
         if self.copy:
             Xc = X.copy()
 
         # iterating over each feature
         for n, feature in enumerate(self.features):
-            if self.verbose: print(f" - [ClosestDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
+
+            # printing verbose if requested
+            if self.verbose:
+                print(f" - [ClosestDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
 
             # accessing feature's modalities' order
             order = self.values_orders.get(feature)
 
             # imputation des valeurs inconnues le cas échéant
             unknowns = [value for value in Xc[feature].unique() if not any(is_equal(value, known) for known in order.values())]
             unknowns = [value for value in unknowns if notna(value)]  # suppression des NaNs
@@ -844,36 +851,37 @@
     
     return n
 
 class DefaultDiscretizer(BaseEstimator, TransformerMixin):
     
     def __init__(
         self, features: List[str], min_freq: float, *, 
+        values_orders: Dict[str, Any]={},
         default_value: str='__OTHER__', dropna: bool=False, 
         copy: bool=False, verbose: bool=False) -> None:
         """ Groups a qualitative features' values less frequent than min_freq into a default_value"""
         
         self.features = features[:]
         self.min_freq = min_freq
-        self.values_orders: Dict[str, Any] = {}
+        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.default_value = default_value[:]
         self.copy = copy
         self.verbose = verbose
         self.dropna = dropna
 
     def fit(self, X: DataFrame, y: Series) -> None:
 
         # computing frequencies of each modality
         frequencies = X[self.features].apply(value_counts, dropna=False, normalize=True, axis=0)
 
         # computing ordered target rate per modality for ordering
         target_rates = X[self.features].apply(target_rate, y=y, dropna=True, ascending=True, axis=0)
 
         # attributing orders to each feature
-        self.values_orders = {feature: GroupedList(list(target_rates[feature])) for feature in self.features}
+        self.values_orders.update({feature: GroupedList(list(target_rates[feature])) for feature in self.features})
         
         #number of unique modality perf feature
         nuniques = X[self.features].apply(nunique, dropna=self.dropna, axis=0)
             
         # identifying modalities which are the most common
         kept_nan = [nan] * (~self.dropna)  # whether or not to keep nans whatever there frequency
         self.to_keep = {
@@ -881,40 +889,42 @@
                 value for value, frequency in frequencies[feature].items()
                     if ((frequency >= self.min_freq) & notna(value)) | (nuniques[feature] <= 2)
             ] for feature in self.features
         }
         
         # grouping rare modalities 
         for n, feature in enumerate(self.features):
+
+        	# printing verbose
             if self.verbose:
                 print(f" - [DefaultDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
             
                 
-                # identifying values to discard (rare modalities)
-                to_discard = [value for value in self.values_orders[feature] if value not in self.to_keep[feature]]
+            # identifying values to discard (rare modalities)
+            to_discard = [value for value in self.values_orders[feature] if value not in self.to_keep[feature]]
 
-                # discarding rare modalities
-                if len(to_discard) > 0:
+            # discarding rare modalities
+            if len(to_discard) > 0:
 
-                    # adding default_value to possible values
-                    order = self.values_orders[feature]
-                    order.append(self.default_value)
-
-                    # grouping rare modalities into default_value
-                    order.group_list(to_discard, self.default_value)
-
-                    # computing target rate for default value and reordering values according to feature's target rate
-                    default_target_rate = y.loc[X[feature].isin(order.get(self.default_value))].mean()  # computing target rate for default value
-                    order_target_rate = [target_rates.get(feature).get(value) for value in order if value != self.default_value]
-                    default_position = next(n for n, trate in enumerate(order_target_rate + [inf]) if trate > default_target_rate)
-
-                    # updating the modalities' order                
-                    new_order = order[:-1][:default_position] + [self.default_value] + order[:-1][default_position:]  # getting rid of default value already in order
-                    order = order.sort_by(new_order)
-                    self.values_orders.update({feature: order})
+                # adding default_value to possible values
+                order = self.values_orders[feature]
+                order.append(self.default_value)
+
+                # grouping rare modalities into default_value
+                order.group_list(to_discard, self.default_value)
+
+                # computing target rate for default value and reordering values according to feature's target rate
+                default_target_rate = y.loc[X[feature].isin(order.get(self.default_value))].mean()  # computing target rate for default value
+                order_target_rate = [target_rates.get(feature).get(value) for value in order if value != self.default_value]
+                default_position = next(n for n, trate in enumerate(order_target_rate + [inf]) if trate > default_target_rate)
+
+                # updating the modalities' order                
+                new_order = order[:-1][:default_position] + [self.default_value] + order[:-1][default_position:]  # getting rid of default value already in order
+                order = order.sort_by(new_order)
+                self.values_orders.update({feature: order})
 
         return self
 
     def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
 
         # copying dataset if requested
         Xc = X
```

### Comparing `AutoCarver-4.0.1/AutoCarver/FeatureSelector.py` & `AutoCarver-4.1.0/AutoCarver/FeatureSelector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,186 +1,224 @@
 from IPython.display import display_html
 from math import sqrt
 from numpy import triu, ones, nan, inf
 from pandas import DataFrame, Series, notna
 from scipy.stats import kruskal
+from sklearn.base import BaseEstimator, TransformerMixin
 from statsmodels.formula.api import ols
 from statsmodels.stats.outliers_influence import variance_inflation_factor
+from typing import List, Dict, Any, Callable
 
 
-class FeatureSelector():
-    """ A pipeline of measures to perform EDA and feature pre-selection"""
-    
-    def __init__(self, measures: list=[], filters: list=[]):
+class FeatureSelector(BaseEstimator, TransformerMixin):
+    """ A pipeline of measures to perform EDA and feature pre-selection
         
-        self.measures = [dtype_measure, nans_measure, mode_measure] + measures[:]
+    Parameters
+    ----------
+    features: List[str]
+        Features on which to compute association.
+    n_best, int:
+        Number of features to be selected
+    measures, List[Callable]: default list().
+        List of association measures to be used.
+        Implemented measures are:
+            - For association evaluation: `kruskal_measure`, `R_measure`
+            - For outlier detection: `zscore_measure`, `iqr_measure`
+        Ranks features based on last measure of the list.
+    filters, List[Callable]: default list().
+        List of filters to be used.
+        Implemented filters are:
+          - For linear correlation: `spearman_filter`, `pearson_filter`
+          - For multicoloinearity: `vif_filter`
+
+    params examples
+    ---------------
+    thresh_nan, float: default 1.
+        Maximum percentage of NaNs in a feature
+    thresh_mode, float: default 1.
+        Maximum percentage of the mode of a feature
+    thresh_outlier, float: default 1.
+        Maximum percentage of Outliers in a feature
+    thresh_corr, float: default 1.
+        Maximum association between features
+    thresh_vif, float: default inf
+        Maximum VIF between features
+    ascending, bool: default False
+        Ascending of Descending sort by sort_measure
+    """
+    
+    def __init__(self, features: List[str], n_best: int, measures: List[Callable]=list(), filters: List[Callable]=list(),
+                 copy: bool=True, verbose: bool=True, **params) -> None:
+        
+        self.features = features[:]
+        self.n_best = n_best
+        assert n_best <= len(features), "Must set n_best <= len(features)"
+
+        self.measures = [dtype_measure, nans_measure, mode_measure, zscore_measure] + measures[:]
         self.filters = [thresh_filter] + filters[:]
-        
-        self.associations = []
-        self.filtered_associations = []
+        self.sort_measures = [measure.__name__ for measure in measures[-1::]]
+
+        self.copy = copy
+        self.verbose = verbose
+        self.params = params
     
-    def measure(self, x: Series, y: Series, **params):
-        """ Measures association between x and y
-        
-        Parameters
-        ----------
-        thresh_nan, float: default 1.
-          Maximum percentage of NaNs in a feature
-        thresh_mode, float: default 1.
-          Maximum percentage of the mode of a feature
-        thresh_outlier, float: default 1.
-          Maximum percentage of Outliers in a feature
-        """
+    def measure(self, x: Series, y: Series) -> Dict[str, Any]:
+        """ Measures association between x and y """
         
-        passed = True
+        passed = True  # measures keep going only if previous basic tests are passed
         association = {}
+
+        # iterating over each measure
         for measure in self.measures:
-            passed, association = measure(passed, association, x, y, **params)
+            passed, association = measure(passed, association, x, y, **self.params)
             
         return association
     
-    def measure_apply(self, X: DataFrame, y: Series, **params):
+    def measure_apply(self, X: DataFrame, y: Series) -> None:
         """ Measures association between columns of X and y
-        
-        Parameters
-        ----------
-        thresh_nan, float: default 1.
-          Maximum percentage of NaNs in a feature
-        thresh_mode, float: default 1.
-          Maximum percentage of the mode of a feature
-        thresh_outlier, float: default 1.
-          Maximum percentage of Outliers in a feature
-        """
+
+    Parameters
+    ----------
+    ascending, bool: default False
+      Ascending of Descending sort by sort_measure
+    """
         
         # applying association measure to each column
-        self.associations = X.apply(self.measure, y=y, **params, result_type='expand', axis=0).T
-        
-        return self.associations
+        self.associations = X[self.features].apply(self.measure, y=y, result_type='expand', axis=0).T
+        self.associations = self.associations.sort_values(self.sort_measures[0], ascending=self.params.get('ascending', False))
     
-    def filter_apply(self, X: DataFrame, sort_measure: str, **params):
-        """ Filters out to correlated features that are less relevant
-        
-        Parameters
-        ----------
-        thresh_corr, float: default 1.
-          Maximum association between features
-        thresh_vif, float: default inf
-          Maximum VIF between features
-        ascending, bool: default False
-          Ascending of Descending sort by sort_measure
-        """
+    def filter_apply(self, X: DataFrame, sort_measure: str) -> DataFrame:
+        """ Filters out too correlated features (least relevant first)
+
+    Parameters
+    ----------
+    ascending, bool: default False
+      Ascending of Descending sort by sort_measure
+    """
         
         # ordering features by sort_by
-        self.filtered_associations = self.associations.sort_values(sort_measure, ascending=params.get('ascending', False))
+        self.filtered_associations = self.associations.sort_values(sort_measure, ascending=self.params.get('ascending', False))
 
         # applying successive filters
         for filtering in self.filters:
 
             # ordered filtering
-            self.filtered_associations = filtering(X, self.filtered_associations, **params)
-        
-        return self.filtered_associations
+            self.filtered_associations = filtering(X, self.filtered_associations, **self.params)
     
-    def display_stats(self, X: DataFrame, y: Series, sort_measure: str=None):
-        """ Computes statistics for EDA with default params"""
-        
-        # initial computation of all association measures
-        self.measure_apply(X, y)
+    def display_stats(self, association: DataFrame, caption: str) -> None:
+        """ EDA of fitted associations"""
         
-        # filtering
-        if not sort_measure:  # by default, last measure passed
-            sort_measure = self.measures[-1].__name__
-        association = self.filter_apply(X, sort_measure)
-            
         # appllying style 
         subset = [c for c in association if 'pct_' in c or '_measure' in c]
-        association = association.style.background_gradient(cmap='coolwarm', subset=subset)
-        display_html(association.set_table_attributes("style='display:inline'")._repr_html_(), raw=True)
+        style = association.style.background_gradient(cmap='coolwarm', subset=subset)
+        style = style.set_table_attributes("style='display:inline'")
+        style = style.set_caption(caption)
+        display_html(style._repr_html_(), raw=True)
         
     
-    def select_features(self, X: DataFrame, y: Series, n_best: int, sort_measures: list, **params):
-        """ Selects the n_best features
-        
-        Parameters
-        ----------
-        thresh_nan, float: default 1.
-          Maximum percentage of NaNs in a feature
-        thresh_mode, float: default 1.
-          Maximum percentage of the mode of a feature
-        thresh_outlier, float: default 1.
-          Maximum percentage of Outliers in a feature
-        thresh_corr, float: default 1.
-          Maximum association between features
-        thresh_vif, float: default inf
-          Maximum VIF between features
-        ascending, bool: default False
-          Ascending of Descending sort by sort_measure
-        """
+    def fit(self, X: DataFrame, y: Series) -> None:
+        """ Selects the n_best features"""
         
         # initial computation of all association measures
-#         if len(self.associations) == 0:
-        self.measure_apply(X, y, **params)
+        self.measure_apply(X, y)
+
+        # displaying association measure
+        if self.verbose:
+            self.display_stats(self.associations, 'Raw association')
         
-        # iterating over each sort_measures
+        # iterating over each sort_measures 
+        # useful when measures hints to specific associations
         ranks = []
-        for sort_measure in sort_measures:
+        for n, sort_measure in enumerate(self.sort_measures):
             
             # filtering by sort_measure
-            rank = list(self.filter_apply(X, sort_measure, **params).index)
-            ranks += [rank]
-        
+            self.filter_apply(X, sort_measure)
+            ranks += [list(self.filtered_associations.index)]
+
+            # displaying filtered out association measure
+            if n == 0 and self.verbose:
+                self.display_stats(self.filtered_associations, 'Filtered association')
+
         # retrieving the n_best features per ranking
-        best_features = [feature for rank in ranks for feature in rank[:n_best]]
-        best_features = list(set(best_features))  # deduplicating
-        
-        return best_features
+        self.best_features = [feature for rank in ranks for feature in rank[:self.n_best]]
+        self.best_features = list(set(self.best_features))  # deduplicating
+
+        # displaying filtered out association measure
+        # if n == 0 and self.verbose:
+        #     self.display_stats(self.associations.reindex(self.best_features), 'Filtered association')
+
+        return self
+
+    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+
+        # copying dataset
+        Xc = X
+        if self.copy:
+            Xc.copy()
+
+        # filtering out unwanted features
+        Xc = X.drop([c for c in self.features if c not in self.best_features], axis=1)
+
+        return Xc
+
 
-    
 # MEASURES
-def nans_measure(active: bool, association: dict, x: Series, y: Series=None, **params):
-    """ Measure of the percentage of NaNs"""
+def nans_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Measure of the percentage of NaNs
+
+    Parameters
+    ----------
+    thresh_nan, float: default 1.
+      Maximum percentage of NaNs in a feature
+    """
     
     passed = True  # whether or not tests where passed
     
     nans = x.isnull()  # ckecking for nans
     pct_nan = nans.mean()   # Computing percentage of nans
     
     # updating association
     association.update({'pct_nan': pct_nan})
     
     # Excluding feature that have to many NaNs
     passed = pct_nan < params.get('thresh_nan', 1.)
     
     return passed, association
 
-def dtype_measure(active: bool, association: dict, x: Series, y: Series=None, **params):
+def dtype_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
     """ Gets dtype"""
     
     # updating association
     association.update({'dtype': x.dtype})
         
     return active, association
 
-def mode_measure(active: bool, association: dict, x: Series, y: Series=None, **params):
-    """ Measure of the percentage of the Mode"""
+def mode_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Measure of the percentage of the Mode
+
+    Parameters
+    ----------
+    thresh_mode, float: default 1.
+      Maximum percentage of the mode of a feature
+    """
     
     passed = True  # whether or not tests where passed
     
     mode = x.mode(dropna=True).values[0]  # computing mode
     pct_mode = (x == mode).mean()  # Computing percentage of the mode
     
     # updating association
     association.update({'pct_mode': pct_mode, 'mode': mode})
     
     # Excluding feature with too frequent modes
     passed = pct_mode < params.get('thresh_mode', 1.)
     
     return passed, association
 
-def kruskal_measure(active: bool, association: dict, x: Series, y: Series, **params):
+def kruskal_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
     """ Kruskal-Wallis statistic between x (quantitative) and y (binary)"""
     
     # check that previous steps where passed
     if active:
     
         nans = x.isnull()  # ckecking for nans
         
@@ -189,15 +227,15 @@
         
         # updating association
         if kw:
             association.update({'kruskal_measure': kw[0]})
         
     return active, association
 
-def R_measure(active: bool, association: dict, x: Series, y: Series, **params):
+def R_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
     """ R of the linear regression of x (quantitative) by y (binary)"""
     
     # check that previous steps where passed
     if active:
     
         nans = x.isnull()  # ckecking for nans
 
@@ -210,16 +248,22 @@
         # updating association
         if regression.rsquared:
             association.update({'R_measure': sqrt(regression.rsquared)})
         
     return active, association
 
 
-def zscore_measure(active: bool, association: dict, x: Series, y: Series=None, **params):
-    """ Computes outliers based on the z-score"""
+def zscore_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Computes outliers based on the z-score
+
+    Parameters
+    ----------
+    thresh_outlier, float: default 1.
+      Maximum percentage of Outliers in a feature
+    """
     
     # check that previous steps where passed for computational optimization
     if active:
         
         mean = x.mean()  # mean of the feature
         std = x.std()  # standard deviation of the feature
         zscore = (x-mean) / std  # zscore per observation
@@ -238,16 +282,22 @@
         })
 
         # Excluding feature with too frequent modes
         passed = pct_zscore < params.get('thresh_outlier', 1.)
         
     return active, association
 
-def iqr_measure(active: bool, association: dict, x: Series, y: Series=None, **params):
-    """ Computes outliers based on the inter-quartile range"""
+def iqr_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
+    """ Computes outliers based on the inter-quartile range
+
+    Parameters
+    ----------
+    thresh_outlier, float: default 1.
+      Maximum percentage of Outliers in a feature
+    """
     
     # check that previous steps where passed for computational optimization
     if active:
         
         q3 = x.quantile(0.75)  # 3rd quartile
         q1 = x.quantile(0.25)  # 1st quartile
         iqr = q3 - q1  # inter quartile range
@@ -268,26 +318,32 @@
         # Excluding feature with too frequent modes
         passed = pct_iqr < params.get('thresh_outlier', 1.)
         
     return active, association
 
     
 # FILTERS        
-def thresh_filter(X: DataFrame, ranks: DataFrame, **params):
+def thresh_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
     """ Filters out missing association measure (did not pass a threshold)"""
     
     # drops rows with nans
     associations = ranks.dropna(axis=0)
     
     return associations
 
-def quantitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: str, **params):
+def quantitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: str, **params) -> Dict[str, Any]:
     """ Computes max association between X and X (quantitative) excluding features 
     that are correlated to a feature more associated with the target 
-    (defined by the prefered_order)."""
+    (defined by the prefered_order).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+      Maximum association between features
+    """
     
     # accessing the prefered order
     prefered_order = ranks.index
 
     # computing correlation between features
     X_corr = X[prefered_order].corr(corr_measure).abs()
     X_corr = X_corr.where(triu(ones(X_corr.shape), k=1).astype(bool))
@@ -321,36 +377,54 @@
             
     # applying filter on association
     associations = ranks.join(associations, how='right')
     
     return associations 
 
 
-def spearman_filter(X: DataFrame, ranks: DataFrame, **params):
+def spearman_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
     """ Computes max Spearman between X and X (quantitative) excluding features 
     that are correlated to a feature more associated with the target 
-    (defined by the prefered_order)."""
+    (defined by the prefered_order).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+      Maximum association between features
+    """
             
     # applying quantitative filter with spearman correlation
     associations = quantitative_filter(X, ranks, 'spearman', **params)
     
     return associations
 
-def pearson_filter(X: DataFrame, ranks: DataFrame, **params):
+def pearson_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
     """ Computes max Pearson between X and X (quantitative) excluding features 
     that are correlated to a feature more associated with the target 
-    (defined by the prefered_order)."""
+    (defined by the prefered_order).
+
+    Parameters
+    ----------
+    thresh_corr, float: default 1.
+      Maximum association between features
+    """
             
     # applying quantitative filter with spearman correlation
     associations = quantitative_filter(X, ranks, 'pearson', **params)
     
     return associations
 
-def vif_filter(X: DataFrame, ranks: DataFrame, **params):
-    """ Computes Variance Inflation Factor (multicolinearity)"""
+def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Computes Variance Inflation Factor (multicolinearity)
+
+    Parameters
+    ----------
+    thresh_vif, float: default inf
+      Maximum VIF between features
+    """
     
     # accessing the prefered order
     prefered_order = ranks.index
     
     # initiating list association per feature
     associations = []
```

### Comparing `AutoCarver-4.0.1/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-4.1.0/AutoCarver.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,168 +1,168 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.0.1
+Version: 4.1.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
-Description: </p>
-        <p align="center">
-            <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
-            <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
-            <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
-        </p>
-        
-        
-        # AutoCarver
-        
-        **AutoCarver** is an approach for maximising a qualitative feature's association with a binary target feature while reducing it's number of distinct modalities.
-        Can also be used to discretize quantitative features, that are prealably cut in quantiles.
-        
-         Modalities/values of features are carved/regrouped according to a computed specific order defined based on their types:
-          - *Qualitative features* grouped based on target rate per modality.
-          - *Qualitative ordinal features* grouped based on specified modality order.
-          - *Quantitative features* grouped based on the order of their values.
-         
-        Uses Tschurpow's T or Cramer's V to find the optimal carving (regrouping) of modalities/values of features.
-        
-        `AutoCarver` is an `sklearn` transformer.
-        
-        Only implementend for binary classification problems.
-        
-        ## Install
-        
-        AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
-        
-        <pre>
-        pip install --upgrade autocarver
-        </pre>
-        
-        ## Complete Example
-        
-        #### Setting up Samples
-        
-        `AutoCarver` tests the robustness of carvings on a specific sample. For this purpose, the use of an out of time sample is recommended. 
-        
-        ```python
-        # defining training and testing sets
-        X_train, y_train = ...
-        X_test, y_test = ...
-        X_val, y_val = ...
-        ```
-        
-        #### Formatting features to be carved
-        
-        All features need to be discretized via a `Discretizer` so `AutoCarver` can group their modalities. Following parameters must be set for `Discretizer`:
-        
-        - `min_freq`, should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
-          - *For qualitative features:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality.
-          - *For qualitative ordinal features:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
-        
-        - `q`, should be set from 10 (faster) to 20 (preciser).
-          - *For quantitative features:* Number of quantiles to initialy cut the feature. Values more frequent than `1/q` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
-        
-        - `values_orders`
-          - *For qualitative ordinal features:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
-        
-        At this step, all `numpy.nan` are kept as their own modality.
-        
-        For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
-        
-        By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
-        
-        ```python
-        from AutoCarver.Discretizers import Discretizer
-        
-        # specifying features to be carved
-        quantitatives = ['amount', 'distance', 'length', 'height']
-        qualitatives = ['age', 'type', 'grade', 'city']
-        
-        # specifying orders of categorical ordinal features
-        values_orders = {
-            'age': ['0-18', '18-30', '30-50', '50+'],
-            'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
-        }
-        
-        # pre-processing of features into categorical ordinal features
-        discretizer = Discretizer(quantitatives, qualitatives, min_freq=0.02, q=20, values_orders=values_orders)
-        discretizer.fit_transform(X_train, y_train)
-        discretizer.transform(X_test)
-        
-        # updating features' values orders (at this step every features are qualitative ordinal)
-        values_orders = discretizer.values_orders
-        ```
-        
-        #### Automatic Carving of features
-        
-        All specified features can now automatically be carved in an association maximising grouping of their modalities while reducing their number. Following parameters must be set for `AutoCarver`:
-        
-        - `sort_by`, association measure used to find the optimal group modality combination.
-          - Use `sort_by='cramerv'` for more modalities, less robust.
-          - Use `sort_by='tschuprowt'` for more robust modalities.
-          - **Tip:** a combination of features carved with `sort_by='cramerv'` and `sort_by='tschuprowt'` can sometime prove to be better than only one of those.
-        
-        - `max_n_mod`, maximum number of modalities for the carved features (excluding `numpy.nan`). All possible combinations of less than `max_n_mod` groups of modalities will be tested. Should be set from 4 (faster) to 6 (preciser).
-        
-        At this step, all `numpy.nan` are grouped to the best non-NaN value (after they were grouped). Use `keep_nans=True` if you want `numpy.nan` to remain as a specific modality.
-        
-        
-        ```python
-        from AutoCarver.AutoCarver import AutoCarver
-        
-        # intiating AutoCarver
-        auto_carver = AutoCarver(values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
-        
-        # fitting on training sample 
-        # a test sample can be specified to evaluate carving robustness
-        auto_carver.fit_transform(X_train, y_train, X_test, y_test)
-        
-        # applying transformation on test sample
-        auto_carver.transform(X_test)
-        ```
-        <p align="left">
-          <img width="500" src="/docs/auto_carver_fit.PNG" />
-        </p>
-        
-        #### Storing, reusing an AutoCarver
-        
-        The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
-        
-        ```python
-        from pickle import dump
-        from sklearn.pipeline import Pipeline
-        
-        # storing Discretizer
-        pipe = [('Discretizer', discretizer)]
-        
-        # storing fitted AutoCarver in a Pipeline
-        pipe += [('AutoCarver', auto_carver)]
-        pipe = Pipeline(pipe)
-        
-        # storing as pickle file
-        dump(pipe, open('my_pipe.pkl', 'wb'))
-        ```
-        
-        The stored `Pipeline`, can then be used to transform new datasets.
-        
-        ```python
-        from pickle import load
-        
-        # restoring the pipeline
-        pipe = load(open('my_pipe.pkl', 'rb'))
-        
-        # applying pipe to a validation set or in production
-        X_val = pipe.transform(X_val)
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+</p>
+<p align="center">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
+    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
+    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+</p>
+
+
+# AutoCarver
+
+**AutoCarver** is an approach for maximising a qualitative feature's association with a binary target feature while reducing it's number of distinct modalities.
+Can also be used to discretize quantitative features, that are prealably cut in quantiles.
+
+ Modalities/values of features are carved/regrouped according to a computed specific order defined based on their types:
+  - *Qualitative features* grouped based on target rate per modality.
+  - *Qualitative ordinal features* grouped based on specified modality order.
+  - *Quantitative features* grouped based on the order of their values.
+ 
+Uses Tschurpow's T or Cramer's V to find the optimal carving (regrouping) of modalities/values of features.
+
+`AutoCarver` is an `sklearn` transformer.
+
+Only implementend for binary classification problems.
+
+## Install
+
+AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
+
+<pre>
+pip install --upgrade autocarver
+</pre>
+
+## Complete Example
+
+#### Setting up Samples
+
+`AutoCarver` tests the robustness of carvings on a specific sample. For this purpose, the use of an out of time sample is recommended. 
+
+```python
+# defining training and testing sets
+X_train, y_train = ...
+X_test, y_test = ...
+X_val, y_val = ...
+```
+
+#### Formatting features to be carved
+
+All features need to be discretized via a `Discretizer` so `AutoCarver` can group their modalities. Following parameters must be set for `Discretizer`:
+
+- `min_freq`, should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
+  - *For qualitative features:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality.
+  - *For qualitative ordinal features:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
+
+- `q`, should be set from 10 (faster) to 20 (preciser).
+  - *For quantitative features:* Number of quantiles to initialy cut the feature. Values more frequent than `1/q` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
+
+- `values_orders`
+  - *For qualitative ordinal features:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
+
+At this step, all `numpy.nan` are kept as their own modality.
+
+For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
+
+By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
+
+```python
+from AutoCarver.Discretizers import Discretizer
+
+# specifying features to be carved
+quantitatives = ['amount', 'distance', 'length', 'height']
+qualitatives = ['age', 'type', 'grade', 'city']
+
+# specifying orders of categorical ordinal features
+values_orders = {
+    'age': ['0-18', '18-30', '30-50', '50+'],
+    'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
+}
+
+# pre-processing of features into categorical ordinal features
+discretizer = Discretizer(quantitatives, qualitatives, min_freq=0.02, q=20, values_orders=values_orders)
+discretizer.fit_transform(X_train, y_train)
+discretizer.transform(X_test)
+
+# updating features' values orders (at this step every features are qualitative ordinal)
+values_orders = discretizer.values_orders
+```
+
+#### Automatic Carving of features
+
+All specified features can now automatically be carved in an association maximising grouping of their modalities while reducing their number. Following parameters must be set for `AutoCarver`:
+
+- `sort_by`, association measure used to find the optimal group modality combination.
+  - Use `sort_by='cramerv'` for more modalities, less robust.
+  - Use `sort_by='tschuprowt'` for more robust modalities.
+  - **Tip:** a combination of features carved with `sort_by='cramerv'` and `sort_by='tschuprowt'` can sometime prove to be better than only one of those.
+
+- `max_n_mod`, maximum number of modalities for the carved features (excluding `numpy.nan`). All possible combinations of less than `max_n_mod` groups of modalities will be tested. Should be set from 4 (faster) to 6 (preciser).
+
+At this step, all `numpy.nan` are grouped to the best non-NaN value (after they were grouped). Use `keep_nans=True` if you want `numpy.nan` to remain as a specific modality.
+
+
+```python
+from AutoCarver.AutoCarver import AutoCarver
+
+# intiating AutoCarver
+auto_carver = AutoCarver(values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
+
+# fitting on training sample 
+# a test sample can be specified to evaluate carving robustness
+auto_carver.fit_transform(X_train, y_train, X_test, y_test)
+
+# applying transformation on test sample
+auto_carver.transform(X_test)
+```
+<p align="left">
+  <img width="500" src="/docs/auto_carver_fit.PNG" />
+</p>
+
+#### Storing, reusing an AutoCarver
+
+The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
+
+```python
+from pickle import dump
+from sklearn.pipeline import Pipeline
+
+# storing Discretizer
+pipe = [('Discretizer', discretizer)]
+
+# storing fitted AutoCarver in a Pipeline
+pipe += [('AutoCarver', auto_carver)]
+pipe = Pipeline(pipe)
+
+# storing as pickle file
+dump(pipe, open('my_pipe.pkl', 'wb'))
+```
+
+The stored `Pipeline`, can then be used to transform new datasets.
+
+```python
+from pickle import load
+
+# restoring the pipeline
+pipe = load(open('my_pipe.pkl', 'rb'))
+
+# applying pipe to a validation set or in production
+X_val = pipe.transform(X_val)
+```
```

### Comparing `AutoCarver-4.0.1/PKG-INFO` & `AutoCarver-4.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,168 +1,168 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.0.1
+Version: 4.1.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
-Description: </p>
-        <p align="center">
-            <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
-            <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
-            <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
-        </p>
-        
-        
-        # AutoCarver
-        
-        **AutoCarver** is an approach for maximising a qualitative feature's association with a binary target feature while reducing it's number of distinct modalities.
-        Can also be used to discretize quantitative features, that are prealably cut in quantiles.
-        
-         Modalities/values of features are carved/regrouped according to a computed specific order defined based on their types:
-          - *Qualitative features* grouped based on target rate per modality.
-          - *Qualitative ordinal features* grouped based on specified modality order.
-          - *Quantitative features* grouped based on the order of their values.
-         
-        Uses Tschurpow's T or Cramer's V to find the optimal carving (regrouping) of modalities/values of features.
-        
-        `AutoCarver` is an `sklearn` transformer.
-        
-        Only implementend for binary classification problems.
-        
-        ## Install
-        
-        AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
-        
-        <pre>
-        pip install --upgrade autocarver
-        </pre>
-        
-        ## Complete Example
-        
-        #### Setting up Samples
-        
-        `AutoCarver` tests the robustness of carvings on a specific sample. For this purpose, the use of an out of time sample is recommended. 
-        
-        ```python
-        # defining training and testing sets
-        X_train, y_train = ...
-        X_test, y_test = ...
-        X_val, y_val = ...
-        ```
-        
-        #### Formatting features to be carved
-        
-        All features need to be discretized via a `Discretizer` so `AutoCarver` can group their modalities. Following parameters must be set for `Discretizer`:
-        
-        - `min_freq`, should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
-          - *For qualitative features:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality.
-          - *For qualitative ordinal features:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
-        
-        - `q`, should be set from 10 (faster) to 20 (preciser).
-          - *For quantitative features:* Number of quantiles to initialy cut the feature. Values more frequent than `1/q` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
-        
-        - `values_orders`
-          - *For qualitative ordinal features:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
-        
-        At this step, all `numpy.nan` are kept as their own modality.
-        
-        For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
-        
-        By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
-        
-        ```python
-        from AutoCarver.Discretizers import Discretizer
-        
-        # specifying features to be carved
-        quantitatives = ['amount', 'distance', 'length', 'height']
-        qualitatives = ['age', 'type', 'grade', 'city']
-        
-        # specifying orders of categorical ordinal features
-        values_orders = {
-            'age': ['0-18', '18-30', '30-50', '50+'],
-            'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
-        }
-        
-        # pre-processing of features into categorical ordinal features
-        discretizer = Discretizer(quantitatives, qualitatives, min_freq=0.02, q=20, values_orders=values_orders)
-        discretizer.fit_transform(X_train, y_train)
-        discretizer.transform(X_test)
-        
-        # updating features' values orders (at this step every features are qualitative ordinal)
-        values_orders = discretizer.values_orders
-        ```
-        
-        #### Automatic Carving of features
-        
-        All specified features can now automatically be carved in an association maximising grouping of their modalities while reducing their number. Following parameters must be set for `AutoCarver`:
-        
-        - `sort_by`, association measure used to find the optimal group modality combination.
-          - Use `sort_by='cramerv'` for more modalities, less robust.
-          - Use `sort_by='tschuprowt'` for more robust modalities.
-          - **Tip:** a combination of features carved with `sort_by='cramerv'` and `sort_by='tschuprowt'` can sometime prove to be better than only one of those.
-        
-        - `max_n_mod`, maximum number of modalities for the carved features (excluding `numpy.nan`). All possible combinations of less than `max_n_mod` groups of modalities will be tested. Should be set from 4 (faster) to 6 (preciser).
-        
-        At this step, all `numpy.nan` are grouped to the best non-NaN value (after they were grouped). Use `keep_nans=True` if you want `numpy.nan` to remain as a specific modality.
-        
-        
-        ```python
-        from AutoCarver.AutoCarver import AutoCarver
-        
-        # intiating AutoCarver
-        auto_carver = AutoCarver(values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
-        
-        # fitting on training sample 
-        # a test sample can be specified to evaluate carving robustness
-        auto_carver.fit_transform(X_train, y_train, X_test, y_test)
-        
-        # applying transformation on test sample
-        auto_carver.transform(X_test)
-        ```
-        <p align="left">
-          <img width="500" src="/docs/auto_carver_fit.PNG" />
-        </p>
-        
-        #### Storing, reusing an AutoCarver
-        
-        The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
-        
-        ```python
-        from pickle import dump
-        from sklearn.pipeline import Pipeline
-        
-        # storing Discretizer
-        pipe = [('Discretizer', discretizer)]
-        
-        # storing fitted AutoCarver in a Pipeline
-        pipe += [('AutoCarver', auto_carver)]
-        pipe = Pipeline(pipe)
-        
-        # storing as pickle file
-        dump(pipe, open('my_pipe.pkl', 'wb'))
-        ```
-        
-        The stored `Pipeline`, can then be used to transform new datasets.
-        
-        ```python
-        from pickle import load
-        
-        # restoring the pipeline
-        pipe = load(open('my_pipe.pkl', 'rb'))
-        
-        # applying pipe to a validation set or in production
-        X_val = pipe.transform(X_val)
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+</p>
+<p align="center">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
+    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
+    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+</p>
+
+
+# AutoCarver
+
+**AutoCarver** is an approach for maximising a qualitative feature's association with a binary target feature while reducing it's number of distinct modalities.
+Can also be used to discretize quantitative features, that are prealably cut in quantiles.
+
+ Modalities/values of features are carved/regrouped according to a computed specific order defined based on their types:
+  - *Qualitative features* grouped based on target rate per modality.
+  - *Qualitative ordinal features* grouped based on specified modality order.
+  - *Quantitative features* grouped based on the order of their values.
+ 
+Uses Tschurpow's T or Cramer's V to find the optimal carving (regrouping) of modalities/values of features.
+
+`AutoCarver` is an `sklearn` transformer.
+
+Only implementend for binary classification problems.
+
+## Install
+
+AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
+
+<pre>
+pip install --upgrade autocarver
+</pre>
+
+## Complete Example
+
+#### Setting up Samples
+
+`AutoCarver` tests the robustness of carvings on a specific sample. For this purpose, the use of an out of time sample is recommended. 
+
+```python
+# defining training and testing sets
+X_train, y_train = ...
+X_test, y_test = ...
+X_val, y_val = ...
+```
+
+#### Formatting features to be carved
+
+All features need to be discretized via a `Discretizer` so `AutoCarver` can group their modalities. Following parameters must be set for `Discretizer`:
+
+- `min_freq`, should be set from 0.01 (preciser) to 0.05 (faster, increased stability).
+  - *For qualitative features:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality.
+  - *For qualitative ordinal features:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
+
+- `q`, should be set from 10 (faster) to 20 (preciser).
+  - *For quantitative features:* Number of quantiles to initialy cut the feature. Values more frequent than `1/q` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
+
+- `values_orders`
+  - *For qualitative ordinal features:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
+
+At this step, all `numpy.nan` are kept as their own modality.
+
+For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
+
+By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
+
+```python
+from AutoCarver.Discretizers import Discretizer
+
+# specifying features to be carved
+quantitatives = ['amount', 'distance', 'length', 'height']
+qualitatives = ['age', 'type', 'grade', 'city']
+
+# specifying orders of categorical ordinal features
+values_orders = {
+    'age': ['0-18', '18-30', '30-50', '50+'],
+    'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
+}
+
+# pre-processing of features into categorical ordinal features
+discretizer = Discretizer(quantitatives, qualitatives, min_freq=0.02, q=20, values_orders=values_orders)
+discretizer.fit_transform(X_train, y_train)
+discretizer.transform(X_test)
+
+# updating features' values orders (at this step every features are qualitative ordinal)
+values_orders = discretizer.values_orders
+```
+
+#### Automatic Carving of features
+
+All specified features can now automatically be carved in an association maximising grouping of their modalities while reducing their number. Following parameters must be set for `AutoCarver`:
+
+- `sort_by`, association measure used to find the optimal group modality combination.
+  - Use `sort_by='cramerv'` for more modalities, less robust.
+  - Use `sort_by='tschuprowt'` for more robust modalities.
+  - **Tip:** a combination of features carved with `sort_by='cramerv'` and `sort_by='tschuprowt'` can sometime prove to be better than only one of those.
+
+- `max_n_mod`, maximum number of modalities for the carved features (excluding `numpy.nan`). All possible combinations of less than `max_n_mod` groups of modalities will be tested. Should be set from 4 (faster) to 6 (preciser).
+
+At this step, all `numpy.nan` are grouped to the best non-NaN value (after they were grouped). Use `keep_nans=True` if you want `numpy.nan` to remain as a specific modality.
+
+
+```python
+from AutoCarver.AutoCarver import AutoCarver
+
+# intiating AutoCarver
+auto_carver = AutoCarver(values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
+
+# fitting on training sample 
+# a test sample can be specified to evaluate carving robustness
+auto_carver.fit_transform(X_train, y_train, X_test, y_test)
+
+# applying transformation on test sample
+auto_carver.transform(X_test)
+```
+<p align="left">
+  <img width="500" src="/docs/auto_carver_fit.PNG" />
+</p>
+
+#### Storing, reusing an AutoCarver
+
+The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
+
+```python
+from pickle import dump
+from sklearn.pipeline import Pipeline
+
+# storing Discretizer
+pipe = [('Discretizer', discretizer)]
+
+# storing fitted AutoCarver in a Pipeline
+pipe += [('AutoCarver', auto_carver)]
+pipe = Pipeline(pipe)
+
+# storing as pickle file
+dump(pipe, open('my_pipe.pkl', 'wb'))
+```
+
+The stored `Pipeline`, can then be used to transform new datasets.
+
+```python
+from pickle import load
+
+# restoring the pipeline
+pipe = load(open('my_pipe.pkl', 'rb'))
+
+# applying pipe to a validation set or in production
+X_val = pipe.transform(X_val)
+```
```

### Comparing `AutoCarver-4.0.1/README.md` & `AutoCarver-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.0.1/setup.py` & `AutoCarver-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='AutoCarver',
-    version='4.0.1',
+    version='4.1.0',
     author='Mario DEFRANCE',
     author_email='defrancemario@gmail.com',
     description='Automatic Bucketizing of Features with Optimal Association',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mdefrance/AutoCarver',
     project_urls = {
```

