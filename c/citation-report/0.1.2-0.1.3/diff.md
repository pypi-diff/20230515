# Comparing `tmp/citation_report-0.1.2.tar.gz` & `tmp/citation_report-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_report-0.1.2.tar", max compression
+gzip compressed data, was "citation_report-0.1.3.tar", max compression
```

## Comparing `citation_report-0.1.2.tar` & `citation_report-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      172 2023-02-23 08:15:49.376409 citation_report-0.1.2/citation_report/__init__.py
--rw-r--r--   0        0        0     6143 2023-01-23 14:31:25.452050 citation_report-0.1.2/citation_report/__main__.py
--rw-r--r--   0        0        0     1751 2023-01-24 04:28:16.713479 citation_report-0.1.2/citation_report/published_report.py
--rw-r--r--   0        0        0     3235 2023-01-23 14:30:33.463242 citation_report-0.1.2/citation_report/publisher.py
--rw-r--r--   0        0        0     1352 2023-02-23 08:15:00.709353 citation_report-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 citation_report-0.1.2/setup.py
--rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 citation_report-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-05-15 16:22:47.952684 citation_report-0.1.3/citation_report/__init__.py
+-rw-r--r--   0        0        0     6143 2023-01-23 14:31:25.452050 citation_report-0.1.3/citation_report/__main__.py
+-rw-r--r--   0        0        0     1751 2023-01-24 04:28:16.713479 citation_report-0.1.3/citation_report/published_report.py
+-rw-r--r--   0        0        0     3235 2023-01-23 14:30:33.463242 citation_report-0.1.3/citation_report/publisher.py
+-rw-r--r--   0        0        0     1488 2023-05-15 16:23:08.412866 citation_report-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 citation_report-0.1.3/PKG-INFO
```

### Comparing `citation_report-0.1.2/citation_report/__main__.py` & `citation_report-0.1.3/citation_report/__main__.py`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.2/citation_report/published_report.py` & `citation_report-0.1.3/citation_report/published_report.py`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.2/citation_report/publisher.py` & `citation_report-0.1.3/citation_report/publisher.py`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.2/pyproject.toml` & `citation_report-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation-report"
-version = "0.1.2"
+version = "0.1.3"
 description = "Regex formula of Philippine Supreme Court citations in report format, i.e. SCRA, PHIL, OFFG."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-report"
 documentation = "https://justmars.github.io/citation-report"
 classifiers = [
@@ -15,29 +15,32 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pydantic = "^1.10.4"
-citation-date = "^0.1.2"
+pydantic = "^1.10.7"
+citation-date = "^0.1.4"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2"
+pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
-mkdocs-material = "^9.0.13"
+mkdocs-material = "^9.1"
 
-[tool.pytest]
-minversion = "7.2"
-addopts = "-ra -q --cov=citation_report tests/"
-testpaths = ["tests"]
+[tool.pytest.ini_options]
+minversion = "7.3"
+addopts = "-ra -q --cov --doctest-modules"
+filterwarnings = [
+  "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
+]
+testpaths = ["tests", "citation_report"]
 
 [tool.ruff]
 ignore = ["F401"]
 
 [tool.black]
 line-length = 79
 include = '.pyi?$'
```

### Comparing `citation_report-0.1.2/PKG-INFO` & `citation_report-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-report
-Version: 0.1.2
+Version: 0.1.3
 Summary: Regex formula of Philippine Supreme Court citations in report format, i.e. SCRA, PHIL, OFFG.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,11 +13,11 @@
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
-Requires-Dist: citation-date (>=0.1.2,<0.2.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: citation-date (>=0.1.4,<0.2.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Project-URL: Documentation, https://justmars.github.io/citation-report
 Project-URL: Repository, https://github.com/justmars/citation-report
```

