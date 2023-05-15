# Comparing `tmp/citation_date-0.1.2.tar.gz` & `tmp/citation_date-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_date-0.1.2.tar", max compression
+gzip compressed data, was "citation_date-0.1.3.tar", max compression
```

## Comparing `citation_date-0.1.2.tar` & `citation_date-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      518 2023-01-21 09:13:56.225420 citation_date-0.1.2/README.md
--rw-r--r--   0        0        0      142 2023-02-23 08:10:49.840811 citation_date-0.1.2/citation_date/__init__.py
--rw-r--r--   0        0        0      164 2023-02-23 08:10:46.211794 citation_date-0.1.2/citation_date/base/__init__.py
--rw-r--r--   0        0        0      292 2022-10-13 00:31:37.797284 citation_date-0.1.2/citation_date/base/day.py
--rw-r--r--   0        0        0      338 2022-10-13 00:31:37.797429 citation_date-0.1.2/citation_date/base/month.py
--rw-r--r--   0        0        0     1568 2023-01-24 03:37:55.769600 citation_date-0.1.2/citation_date/base/report.py
--rw-r--r--   0        0        0     1249 2023-01-24 03:41:18.844828 citation_date-0.1.2/citation_date/base/us_uk.py
--rw-r--r--   0        0        0      475 2022-10-13 00:31:37.797893 citation_date-0.1.2/citation_date/base/year.py
--rw-r--r--   0        0        0     2995 2023-01-24 03:32:20.303154 citation_date-0.1.2/citation_date/decoder.py
--rw-r--r--   0        0        0     1427 2023-02-23 08:11:16.941344 citation_date-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 citation_date-0.1.2/setup.py
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 citation_date-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      519 2023-05-15 16:15:08.545130 citation_date-0.1.3/README.md
+-rw-r--r--   0        0        0      142 2023-05-15 16:16:57.243244 citation_date-0.1.3/citation_date/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-23 08:10:46.211794 citation_date-0.1.3/citation_date/base/__init__.py
+-rw-r--r--   0        0        0      292 2022-10-13 00:31:37.797284 citation_date-0.1.3/citation_date/base/day.py
+-rw-r--r--   0        0        0      338 2022-10-13 00:31:37.797429 citation_date-0.1.3/citation_date/base/month.py
+-rw-r--r--   0        0        0     1568 2023-01-24 03:37:55.769600 citation_date-0.1.3/citation_date/base/report.py
+-rw-r--r--   0        0        0     1249 2023-01-24 03:41:18.844828 citation_date-0.1.3/citation_date/base/us_uk.py
+-rw-r--r--   0        0        0      475 2022-10-13 00:31:37.797893 citation_date-0.1.3/citation_date/base/year.py
+-rw-r--r--   0        0        0     2995 2023-01-24 03:32:20.303154 citation_date-0.1.3/citation_date/decoder.py
+-rw-r--r--   0        0        0     1667 2023-05-15 16:14:50.465481 citation_date-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 citation_date-0.1.3/PKG-INFO
```

### Comparing `citation_date-0.1.2/README.md` & `citation_date-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Development
 
 Checkout code, create a new virtual environment:
 
 ```sh
 poetry add citation-date # python -m pip install citation-date
-poetry update # install dependencies
+poetry install # install dependencies
 poetry shell
 ```
 
 Run tests:
 
 ```sh
 pytest
```

### Comparing `citation_date-0.1.2/citation_date/base/report.py` & `citation_date-0.1.3/citation_date/base/report.py`

 * *Files identical despite different names*

### Comparing `citation_date-0.1.2/citation_date/base/us_uk.py` & `citation_date-0.1.3/citation_date/base/us_uk.py`

 * *Files identical despite different names*

### Comparing `citation_date-0.1.2/citation_date/decoder.py` & `citation_date-0.1.3/citation_date/decoder.py`

 * *Files identical despite different names*

### Comparing `citation_date-0.1.2/pyproject.toml` & `citation_date-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation-date"
-version = "0.1.2"
+version = "0.1.3"
 description = "Regex date formula and decoder - Philippine Supreme Court Decisions"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-date"
 documentation = "https://justmars.github.io/citation-date"
@@ -26,14 +26,22 @@
 pytest = "^7.2"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.0.13"
 
+[tool.pytest.ini_options]
+minversion = "7.3"
+addopts = "-ra -q --cov --doctest-modules"
+filterwarnings = [
+  "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
+]
+testpaths = ["tests", "ciation_date"]
+
 [tool.pytest]
 minversion = "7.2"
 addopts = "-ra -q --cov=citation_date tests/"
 testpaths = ["tests"]
 
 [tool.ruff]
 ignore = ["F401"]
```

### Comparing `citation_date-0.1.2/PKG-INFO` & `citation_date-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-date
-Version: 0.1.2
+Version: 0.1.3
 Summary: Regex date formula and decoder - Philippine Supreme Court Decisions
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -34,15 +34,15 @@
 
 ## Development
 
 Checkout code, create a new virtual environment:
 
 ```sh
 poetry add citation-date # python -m pip install citation-date
-poetry update # install dependencies
+poetry install # install dependencies
 poetry shell
 ```
 
 Run tests:
 
 ```sh
 pytest
```

