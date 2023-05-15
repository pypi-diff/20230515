# Comparing `tmp/tinycta-0.2.8.tar.gz` & `tmp/tinycta-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinycta-0.2.8.tar", max compression
+gzip compressed data, was "tinycta-0.3.1.tar", max compression
```

## Comparing `tinycta-0.2.8.tar` & `tinycta-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-05-01 17:18:28.326201 tinycta-0.2.8/LICENSE
--rw-r--r--   0        0        0      241 2023-05-01 17:18:28.326201 tinycta-0.2.8/README.md
--rw-r--r--   0        0        0      416 2023-05-01 17:18:47.986483 tinycta-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 17:18:28.326201 tinycta-0.2.8/tinycta/__init__.py
--rw-r--r--   0        0        0     2439 2023-05-01 17:18:28.326201 tinycta-0.2.8/tinycta/linalg.py
--rw-r--r--   0        0        0     2635 2023-05-01 17:18:28.326201 tinycta-0.2.8/tinycta/portfolio.py
--rw-r--r--   0        0        0     1471 2023-05-01 17:18:28.326201 tinycta-0.2.8/tinycta/signal.py
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 tinycta-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-15 05:32:52.659093 tinycta-0.3.1/LICENSE
+-rw-r--r--   0        0        0      241 2023-05-15 05:32:52.659093 tinycta-0.3.1/README.md
+-rw-r--r--   0        0        0      429 2023-05-15 05:33:18.791764 tinycta-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 05:32:52.683096 tinycta-0.3.1/tinycta/__init__.py
+-rw-r--r--   0        0        0     2439 2023-05-15 05:32:52.683096 tinycta-0.3.1/tinycta/linalg.py
+-rw-r--r--   0        0        0     1414 2023-05-15 05:32:52.683096 tinycta-0.3.1/tinycta/month.py
+-rw-r--r--   0        0        0     3377 2023-05-15 05:32:52.683096 tinycta-0.3.1/tinycta/port.py
+-rw-r--r--   0        0        0     1471 2023-05-15 05:32:52.683096 tinycta-0.3.1/tinycta/signal.py
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 tinycta-0.3.1/PKG-INFO
```

### Comparing `tinycta-0.2.8/LICENSE` & `tinycta-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinycta-0.2.8/tinycta/linalg.py` & `tinycta-0.3.1/tinycta/linalg.py`

 * *Files identical despite different names*

### Comparing `tinycta-0.2.8/tinycta/signal.py` & `tinycta-0.3.1/tinycta/signal.py`

 * *Files identical despite different names*

### Comparing `tinycta-0.2.8/PKG-INFO` & `tinycta-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tinycta
-Version: 0.2.8
+Version: 0.3.1
 Summary: ...
 Home-page: https://github.com/tschm/TinyCTA
 Author: Thomas Schmelzer
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: QuantStats
+Requires-Dist: pandas
 Project-URL: Repository, https://github.com/tschm/TinyCTA
 Description-Content-Type: text/markdown
 
 # TinyCTA
 
 [![DeepSource](https://deepsource.io/gh/tschm/TinyCTA.svg/?label=active+issues&show_trend=true&token=ZC0ssHYvIZKKygElRTGFTpFW)](https://deepsource.io/gh/tschm/TinyCTA/?ref=repository-badge)
```

