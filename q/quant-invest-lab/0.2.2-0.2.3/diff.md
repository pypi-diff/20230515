# Comparing `tmp/quant_invest_lab-0.2.2.tar.gz` & `tmp/quant_invest_lab-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_lab-0.2.2.tar", max compression
+gzip compressed data, was "quant_invest_lab-0.2.3.tar", max compression
```

## Comparing `quant_invest_lab-0.2.2.tar` & `quant_invest_lab-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4427 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/README.md
--rw-r--r--   0        0        0      978 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    18277 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0    17110 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    26301 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0     8038 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0     7659 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/optimization.py
--rw-r--r--   0        0        0    20461 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     8477 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0     1107 2023-05-15 19:25:29.703098 quant_invest_lab-0.2.2/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4427 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/README.md
+-rw-r--r--   0        0        0      978 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    18277 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0    17110 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    26301 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0     8038 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0     7659 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/optimization.py
+-rw-r--r--   0        0        0    20461 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     8477 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0     1107 2023-05-15 19:47:15.605004 quant_invest_lab-0.2.3/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.3/PKG-INFO
```

### Comparing `quant_invest_lab-0.2.2/README.md` & `quant_invest_lab-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/backtest.py` & `quant_invest_lab-0.2.3/quant_invest_lab/backtest.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/data_provider.py` & `quant_invest_lab-0.2.3/quant_invest_lab/data_provider.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/indicators.py` & `quant_invest_lab-0.2.3/quant_invest_lab/indicators.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/metrics.py` & `quant_invest_lab-0.2.3/quant_invest_lab/metrics.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/optimization.py` & `quant_invest_lab-0.2.3/quant_invest_lab/optimization.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/portfolio.py` & `quant_invest_lab-0.2.3/quant_invest_lab/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/screener.py` & `quant_invest_lab-0.2.3/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/simulation.py` & `quant_invest_lab-0.2.3/quant_invest_lab/simulation.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/quant_invest_lab/utils.py` & `quant_invest_lab-0.2.3/quant_invest_lab/utils.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.2/PKG-INFO` & `quant_invest_lab-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant-invest-lab
-Version: 0.2.2
+Version: 0.2.3
 Summary: Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project.
 Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.2 Summary: Quant
+Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.3 Summary: Quant
 Invest Lab is a python package to help you to do some quantitative experiments,
 while trying to learn or build quantitative investment solutions. This project
 was initially my own set of functionnalities but I decided to build a package
 for that and sharing it as open source project. Author: BaptisteZloch Author-
 email: bzloch@hotmail.fr Requires-Python: >=3.8,<3.12 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

