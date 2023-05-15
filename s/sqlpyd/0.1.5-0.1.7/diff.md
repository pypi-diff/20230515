# Comparing `tmp/sqlpyd-0.1.5.tar.gz` & `tmp/sqlpyd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlpyd-0.1.5.tar", max compression
+gzip compressed data, was "sqlpyd-0.1.7.tar", max compression
```

## Comparing `sqlpyd-0.1.5.tar` & `sqlpyd-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      500 2023-01-24 07:21:05.281224 sqlpyd-0.1.5/README.md
--rw-r--r--   0        0        0     1374 2023-02-23 07:55:32.035880 sqlpyd-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      136 2023-02-23 07:56:17.807680 sqlpyd-0.1.5/sqlpyd/__init__.py
--rw-r--r--   0        0        0     4757 2023-01-07 03:27:21.527893 sqlpyd-0.1.5/sqlpyd/conn.py
--rw-r--r--   0        0        0     1612 2023-01-22 09:35:52.383955 sqlpyd-0.1.5/sqlpyd/name.py
--rw-r--r--   0        0        0     6993 2023-01-24 07:17:42.620631 sqlpyd-0.1.5/sqlpyd/tableconfig.py
--rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 sqlpyd-0.1.5/setup.py
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 sqlpyd-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-05-15 15:27:47.838319 sqlpyd-0.1.7/README.md
+-rw-r--r--   0        0        0     1622 2023-05-15 15:27:10.205792 sqlpyd-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      136 2023-05-15 15:28:04.251002 sqlpyd-0.1.7/sqlpyd/__init__.py
+-rw-r--r--   0        0        0     4757 2023-01-07 03:27:21.527893 sqlpyd-0.1.7/sqlpyd/conn.py
+-rw-r--r--   0        0        0     1612 2023-01-22 09:35:52.383955 sqlpyd-0.1.7/sqlpyd/name.py
+-rw-r--r--   0        0        0     6993 2023-01-24 07:17:42.620631 sqlpyd-0.1.7/sqlpyd/tableconfig.py
+-rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 sqlpyd-0.1.7/PKG-INFO
```

### Comparing `sqlpyd-0.1.5/sqlpyd/conn.py` & `sqlpyd-0.1.7/sqlpyd/conn.py`

 * *Files identical despite different names*

### Comparing `sqlpyd-0.1.5/sqlpyd/name.py` & `sqlpyd-0.1.7/sqlpyd/name.py`

 * *Files identical despite different names*

### Comparing `sqlpyd-0.1.5/sqlpyd/tableconfig.py` & `sqlpyd-0.1.7/sqlpyd/tableconfig.py`

 * *Files identical despite different names*

### Comparing `sqlpyd-0.1.5/PKG-INFO` & `sqlpyd-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlpyd
-Version: 0.1.5
+Version: 0.1.7
 Summary: Validate raw content with pydantic for consumption by sqlite-utils.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,17 +14,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: python-dotenv (>=0.21,<0.22)
-Requires-Dist: sqlite-utils (>=3.30,<4.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0,<2.0)
+Requires-Dist: sqlite-utils (>=3.31,<4.0)
 Project-URL: Documentation, https://github.com/justmars/sqlpyd
 Project-URL: Repository, https://github.com/justmars/sqlpyd
 Description-Content-Type: text/markdown
 
 # sqlpyd
 
 ![Github CI](https://github.com/justmars/sqlpyd/actions/workflows/main.yml/badge.svg)
@@ -37,15 +37,15 @@
 
 ## Development
 
 Checkout code, create a new virtual environment:
 
 ```sh
 poetry add sqlpyd # python -m pip install sqlpyd
-poetry update # install dependencies
+poetry install # install dependencies
 poetry shell
 ```
 
 Run tests:
 
 ```sh
 pytest
```

