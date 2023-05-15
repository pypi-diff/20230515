# Comparing `tmp/statute_trees-0.1.4.tar.gz` & `tmp/statute_trees-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_trees-0.1.4.tar", max compression
+gzip compressed data, was "statute_trees-0.1.5.tar", max compression
```

## Comparing `statute_trees-0.1.4.tar` & `statute_trees-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      562 2023-01-24 06:30:35.804211 statute_trees-0.1.4/README.md
--rw-r--r--   0        0        0     1718 2023-03-07 13:22:24.740778 statute_trees-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      458 2023-03-07 13:24:30.171929 statute_trees-0.1.4/statute_trees/__init__.py
--rw-r--r--   0        0        0     4094 2023-01-24 06:44:56.662064 statute_trees-0.1.4/statute_trees/nodes_codification.py
--rw-r--r--   0        0        0     3306 2023-01-24 06:44:51.412762 statute_trees-0.1.4/statute_trees/nodes_document.py
--rw-r--r--   0        0        0     5309 2023-03-07 13:23:04.378740 statute_trees-0.1.4/statute_trees/nodes_statute.py
--rw-r--r--   0        0        0    15731 2023-01-24 06:58:58.569350 statute_trees-0.1.4/statute_trees/resources.py
--rw-r--r--   0        0        0      125 2022-11-08 13:44:50.046115 statute_trees-0.1.4/statute_trees/utils/__init__.py
--rw-r--r--   0        0        0      635 2022-11-07 07:36:17.339729 statute_trees-0.1.4/statute_trees/utils/get.py
--rw-r--r--   0        0        0     3853 2023-01-20 03:24:13.515358 statute_trees-0.1.4/statute_trees/utils/layer.py
--rw-r--r--   0        0        0     1339 2023-01-22 15:33:00.868666 statute_trees-0.1.4/statute_trees/utils/set.py
--rw-r--r--   0        0        0     1299 2022-12-30 06:25:58.514677 statute_trees-0.1.4/statute_trees/utils/walk.py
--rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 statute_trees-0.1.4/setup.py
--rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 statute_trees-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-15 16:56:21.397441 statute_trees-0.1.5/LICENSE
+-rw-r--r--   0        0        0      562 2023-01-24 06:30:35.804211 statute_trees-0.1.5/README.md
+-rw-r--r--   0        0        0     1741 2023-05-15 16:56:34.844039 statute_trees-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      458 2023-05-15 16:49:44.811140 statute_trees-0.1.5/statute_trees/__init__.py
+-rw-r--r--   0        0        0     4094 2023-01-24 06:44:56.662064 statute_trees-0.1.5/statute_trees/nodes_codification.py
+-rw-r--r--   0        0        0     3306 2023-01-24 06:44:51.412762 statute_trees-0.1.5/statute_trees/nodes_document.py
+-rw-r--r--   0        0        0     5309 2023-03-07 13:23:04.378740 statute_trees-0.1.5/statute_trees/nodes_statute.py
+-rw-r--r--   0        0        0    15731 2023-01-24 06:58:58.569350 statute_trees-0.1.5/statute_trees/resources.py
+-rw-r--r--   0        0        0      125 2022-11-08 13:44:50.046115 statute_trees-0.1.5/statute_trees/utils/__init__.py
+-rw-r--r--   0        0        0      635 2022-11-07 07:36:17.339729 statute_trees-0.1.5/statute_trees/utils/get.py
+-rw-r--r--   0        0        0     3853 2023-01-20 03:24:13.515358 statute_trees-0.1.5/statute_trees/utils/layer.py
+-rw-r--r--   0        0        0     1339 2023-01-22 15:33:00.868666 statute_trees-0.1.5/statute_trees/utils/set.py
+-rw-r--r--   0        0        0     1299 2022-12-30 06:25:58.514677 statute_trees-0.1.5/statute_trees/utils/walk.py
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 statute_trees-0.1.5/PKG-INFO
```

### Comparing `statute_trees-0.1.4/README.md` & `statute_trees-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/pyproject.toml` & `statute_trees-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 [tool.poetry]
 name = "statute-trees"
-version = "0.1.4"
+version = "0.1.5"
 description = "Tree-based Philippine Codifications, Statutes, and Documents, using a uniform node structure (i.e., leaves of a tree) identified by a given material path."
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
-license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-trees"
 documentation = "https://github.com/justmars/statute-trees"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Intended Audience :: Legal Industry",
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-citation-utils = "^0.2.8"
-statute-patterns = "^0.2.2"
+citation-utils = "^0.2.11"
+statute-patterns = "^0.2.5"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 types-Markdown = "^3.4.0"
 types-PyYAML = "^6.0.7"
 types-python-slugify = "^5.0.4"
 types-python-dateutil = "^2.8.19.2"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
-mkdocs-material = "^9.1.0"
-ipython = "^8.11.0"
+mkdocs-material = "^9.1"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
-filterwarnings = ['ignore::DeprecationWarning']
-addopts = "-ra -q --doctest-modules --cov=citation_utils tests/"
-testpaths = ["tests"]
+addopts = "-ra -q --doctest-modules --cov"
+filterwarnings = [
+  "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
+]
+testpaths = ["tests", "statute_trees"]
 
 [tool.ruff]
 ignore = ["F401"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
 [tool.black]
```

### Comparing `statute_trees-0.1.4/statute_trees/nodes_codification.py` & `statute_trees-0.1.5/statute_trees/nodes_codification.py`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/statute_trees/nodes_document.py` & `statute_trees-0.1.5/statute_trees/nodes_document.py`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/statute_trees/nodes_statute.py` & `statute_trees-0.1.5/statute_trees/nodes_statute.py`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/statute_trees/resources.py` & `statute_trees-0.1.5/statute_trees/resources.py`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/statute_trees/utils/get.py` & `statute_trees-0.1.5/statute_trees/utils/get.py`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/statute_trees/utils/layer.py` & `statute_trees-0.1.5/statute_trees/utils/layer.py`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/statute_trees/utils/set.py` & `statute_trees-0.1.5/statute_trees/utils/set.py`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/statute_trees/utils/walk.py` & `statute_trees-0.1.5/statute_trees/utils/walk.py`

 * *Files identical despite different names*

### Comparing `statute_trees-0.1.4/PKG-INFO` & `statute_trees-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: statute-trees
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tree-based Philippine Codifications, Statutes, and Documents, using a uniform node structure (i.e., leaves of a tree) identified by a given material path.
 Home-page: https://lawsql.com
-License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Dist: citation-utils (>=0.2.8,<0.3.0)
-Requires-Dist: statute-patterns (>=0.2.2,<0.3.0)
+Requires-Dist: citation-utils (>=0.2.11,<0.3.0)
+Requires-Dist: statute-patterns (>=0.2.5,<0.3.0)
 Project-URL: Documentation, https://github.com/justmars/statute-trees
 Project-URL: Repository, https://github.com/justmars/statute-trees
 Description-Content-Type: text/markdown
 
 # statute-trees
 
 ![Github CI](https://github.com/justmars/statute-trees/actions/workflows/main.yml/badge.svg)
```

