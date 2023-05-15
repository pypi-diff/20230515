# Comparing `tmp/statute_patterns-0.2.2.tar.gz` & `tmp/statute_patterns-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_patterns-0.2.2.tar", max compression
+gzip compressed data, was "statute_patterns-0.2.3.tar", max compression
```

## Comparing `statute_patterns-0.2.2.tar` & `statute_patterns-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      540 2023-01-24 05:16:45.918551 statute_patterns-0.2.2/README.md
--rw-r--r--   0        0        0     1592 2023-03-06 01:34:19.306746 statute_patterns-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      413 2023-03-06 01:37:38.494809 statute_patterns-0.2.2/statute_patterns/__init__.py
--rw-r--r--   0        0        0     2587 2023-03-06 01:38:57.132031 statute_patterns-0.2.2/statute_patterns/__main__.py
--rw-r--r--   0        0        0      347 2022-11-15 05:02:57.881610 statute_patterns-0.2.2/statute_patterns/components/__init__.py
--rw-r--r--   0        0        0     9606 2023-03-05 05:22:13.847839 statute_patterns-0.2.2/statute_patterns/components/category.py
--rw-r--r--   0        0        0     3232 2023-03-05 05:24:24.768020 statute_patterns-0.2.2/statute_patterns/components/details.py
--rw-r--r--   0        0        0     9174 2023-03-05 05:26:48.589297 statute_patterns-0.2.2/statute_patterns/components/rule.py
--rw-r--r--   0        0        0     2015 2022-12-30 06:17:42.944342 statute_patterns-0.2.2/statute_patterns/components/short.py
--rw-r--r--   0        0        0     2681 2023-03-05 05:24:31.413742 statute_patterns-0.2.2/statute_patterns/components/utils.py
--rw-r--r--   0        0        0     5369 2023-03-05 05:24:24.782830 statute_patterns-0.2.2/statute_patterns/models.py
--rw-r--r--   0        0        0     4617 2023-01-23 14:00:20.449616 statute_patterns-0.2.2/statute_patterns/names.py
--rw-r--r--   0        0        0      249 2022-11-15 04:58:03.940842 statute_patterns-0.2.2/statute_patterns/recipes/__init__.py
--rw-r--r--   0        0        0      380 2022-11-07 05:50:23.161499 statute_patterns-0.2.2/statute_patterns/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-03-05 05:24:53.354912 statute_patterns-0.2.2/statute_patterns/recipes/digits.py
--rw-r--r--   0        0        0      311 2022-11-07 05:50:23.161594 statute_patterns-0.2.2/statute_patterns/recipes/roc.py
--rw-r--r--   0        0        0      550 2022-11-07 05:50:23.161690 statute_patterns-0.2.2/statute_patterns/recipes/spain.py
--rw-r--r--   0        0        0     6553 2023-03-05 05:25:51.543676 statute_patterns-0.2.2/statute_patterns/serials.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 statute_patterns-0.2.2/setup.py
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 statute_patterns-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      540 2023-01-24 05:16:45.918551 statute_patterns-0.2.3/README.md
+-rw-r--r--   0        0        0     1597 2023-05-15 16:43:15.557380 statute_patterns-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      413 2023-05-15 16:43:31.621286 statute_patterns-0.2.3/statute_patterns/__init__.py
+-rw-r--r--   0        0        0     2587 2023-03-06 01:38:57.132031 statute_patterns-0.2.3/statute_patterns/__main__.py
+-rw-r--r--   0        0        0      347 2022-11-15 05:02:57.881610 statute_patterns-0.2.3/statute_patterns/components/__init__.py
+-rw-r--r--   0        0        0     9606 2023-03-05 05:22:13.847839 statute_patterns-0.2.3/statute_patterns/components/category.py
+-rw-r--r--   0        0        0     3232 2023-03-05 05:24:24.768020 statute_patterns-0.2.3/statute_patterns/components/details.py
+-rw-r--r--   0        0        0     9174 2023-03-05 05:26:48.589297 statute_patterns-0.2.3/statute_patterns/components/rule.py
+-rw-r--r--   0        0        0     2015 2022-12-30 06:17:42.944342 statute_patterns-0.2.3/statute_patterns/components/short.py
+-rw-r--r--   0        0        0     2681 2023-03-05 05:24:31.413742 statute_patterns-0.2.3/statute_patterns/components/utils.py
+-rw-r--r--   0        0        0     5369 2023-03-05 05:24:24.782830 statute_patterns-0.2.3/statute_patterns/models.py
+-rw-r--r--   0        0        0     4617 2023-01-23 14:00:20.449616 statute_patterns-0.2.3/statute_patterns/names.py
+-rw-r--r--   0        0        0      249 2022-11-15 04:58:03.940842 statute_patterns-0.2.3/statute_patterns/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2022-11-07 05:50:23.161499 statute_patterns-0.2.3/statute_patterns/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-03-05 05:24:53.354912 statute_patterns-0.2.3/statute_patterns/recipes/digits.py
+-rw-r--r--   0        0        0      311 2022-11-07 05:50:23.161594 statute_patterns-0.2.3/statute_patterns/recipes/roc.py
+-rw-r--r--   0        0        0      550 2022-11-07 05:50:23.161690 statute_patterns-0.2.3/statute_patterns/recipes/spain.py
+-rw-r--r--   0        0        0     6553 2023-03-05 05:25:51.543676 statute_patterns-0.2.3/statute_patterns/serials.py
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 statute_patterns-0.2.3/PKG-INFO
```

### Comparing `statute_patterns-0.2.2/README.md` & `statute_patterns-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/pyproject.toml` & `statute_patterns-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-patterns"
-version = "0.2.2"
+version = "0.2.3"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-patterns"
 documentation = "https://justmars.github.io/statute-patterns"
@@ -15,19 +15,19 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-python-dotenv = "^0.21"
-pydantic = "^1.10.5"
+python-dotenv = "^1.0"
+pydantic = "^1.10.7"
 python-slugify = "^8.0"
 python-dateutil = "^2.8.2"
-email-validator = "^1.3.0"
+email-validator = "^2.0.0.post2"
 
 [tool.poetry.dev-dependencies]
 rich = "^13.3"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
```

### Comparing `statute_patterns-0.2.2/statute_patterns/__main__.py` & `statute_patterns-0.2.3/statute_patterns/__main__.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/components/category.py` & `statute_patterns-0.2.3/statute_patterns/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/components/details.py` & `statute_patterns-0.2.3/statute_patterns/components/details.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/components/rule.py` & `statute_patterns-0.2.3/statute_patterns/components/rule.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/components/short.py` & `statute_patterns-0.2.3/statute_patterns/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/components/utils.py` & `statute_patterns-0.2.3/statute_patterns/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/models.py` & `statute_patterns-0.2.3/statute_patterns/models.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/names.py` & `statute_patterns-0.2.3/statute_patterns/names.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/recipes/digits.py` & `statute_patterns-0.2.3/statute_patterns/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/recipes/spain.py` & `statute_patterns-0.2.3/statute_patterns/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/statute_patterns/serials.py` & `statute_patterns-0.2.3/statute_patterns/serials.py`

 * *Files identical despite different names*

### Comparing `statute_patterns-0.2.2/PKG-INFO` & `statute_patterns-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-patterns
-Version: 0.2.2
+Version: 0.2.3
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,18 +12,18 @@
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Dist: email-validator (>=1.3.0,<2.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: email-validator (>=2.0.0.post2,<3.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: python-dotenv (>=0.21,<0.22)
+Requires-Dist: python-dotenv (>=1.0,<2.0)
 Requires-Dist: python-slugify (>=8.0,<9.0)
 Project-URL: Documentation, https://justmars.github.io/statute-patterns
 Project-URL: Repository, https://github.com/justmars/statute-patterns
 Description-Content-Type: text/markdown
 
 # statute-patterns
```

