# Comparing `tmp/postodon-0.0.2.tar.gz` & `tmp/postodon-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postodon-0.0.2.tar", last modified: Mon Feb 13 15:39:37 2023, max compression
+gzip compressed data, was "postodon-0.0.3.tar", max compression
```

## Comparing `postodon-0.0.2.tar` & `postodon-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:39:37.400351 postodon-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-02-13 15:39:23.000000 postodon-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-02-13 15:39:37.400351 postodon-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-02-13 15:39:23.000000 postodon-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:39:37.396351 postodon-0.0.2/postodon/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-13 15:39:23.000000 postodon-0.0.2/postodon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-13 15:39:23.000000 postodon-0.0.2/postodon/append_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-02-13 15:39:23.000000 postodon-0.0.2/postodon/select_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-13 15:39:23.000000 postodon-0.0.2/postodon/submit_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-13 15:39:23.000000 postodon-0.0.2/postodon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:39:37.400351 postodon-0.0.2/postodon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-02-13 15:39:37.000000 postodon-0.0.2/postodon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-13 15:39:37.000000 postodon-0.0.2/postodon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 15:39:37.000000 postodon-0.0.2/postodon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-13 15:39:37.000000 postodon-0.0.2/postodon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-13 15:39:37.000000 postodon-0.0.2/postodon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-13 15:39:37.000000 postodon-0.0.2/postodon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-13 15:39:23.000000 postodon-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 15:39:37.400351 postodon-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:39:37.400351 postodon-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-13 15:39:23.000000 postodon-0.0.2/tests/test_postodon.py
+-rw-r--r--   0        0        0    11339 2023-05-15 11:12:33.601442 postodon-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2193 2023-05-15 11:12:33.601442 postodon-0.0.3/README.md
+-rw-r--r--   0        0        0     1057 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/__init__.py
+-rw-r--r--   0        0        0      294 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/append_post.py
+-rw-r--r--   0        0        0     1611 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/select_post.py
+-rw-r--r--   0        0        0      520 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/submit_post.py
+-rw-r--r--   0        0        0      345 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/utils.py
+-rw-r--r--   0        0        0     1019 2023-05-15 11:12:33.601442 postodon-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 postodon-0.0.3/PKG-INFO
```

### Comparing `postodon-0.0.2/LICENSE` & `postodon-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postodon-0.0.2/PKG-INFO` & `postodon-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: postodon
-Version: 0.0.2
+Version: 0.0.3
 Summary: Post to Mastodon
-Author-email: msleigh <msleigh@users.noreply.github.com>
-Project-URL: Homepage, https://github.com/msleigh/postodon
-Project-URL: Bug Tracker, https://github.com/msleigh/postodon/issues
-Project-URL: CI, https://github.com/msleigh/postodon/actions
-Project-URL: Changelog, https://github.com/msleigh/postodon/releases
+Home-page: https://github.com/msleigh/postodon
+License: Apache-2.0
+Author: msleigh
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: sphinx (>=7.0.1,<8.0.0)
+Project-URL: Bug Tracker, https://github.com/msleigh/postodon/issues
+Project-URL: CI, https://github.com/msleigh/postodon/actions
+Project-URL: Changelog, https://github.com/msleigh/postodon/releases
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: tests
-License-File: LICENSE
 
 # postodon
 
 [![PyPI](https://img.shields.io/pypi/v/postodon.svg)](https://pypi.org/project/postodon/)
 [![Changelog](https://img.shields.io/github/v/release/msleigh/postodon?include_prereleases&label=changelog)](https://github.com/msleigh/postodon/releases)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/msleigh/postodon/blob/main/LICENSE)
 
@@ -84,7 +88,8 @@
 Now install the dependencies and test dependencies:
 
     pip install -e '.[dev,tests]'
 
 To run the tests:
 
     pytest
+
```

### Comparing `postodon-0.0.2/README.md` & `postodon-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 
 Now install the dependencies and test dependencies:
 
     pip install -e '.[dev,tests]'
 
 To run the tests:
 
-    pytest
+    pytest
```

### Comparing `postodon-0.0.2/postodon/__init__.py` & `postodon-0.0.3/postodon/__init__.py`

 * *Files identical despite different names*

### Comparing `postodon-0.0.2/postodon/select_post.py` & `postodon-0.0.3/postodon/select_post.py`

 * *Files identical despite different names*

### Comparing `postodon-0.0.2/postodon/submit_post.py` & `postodon-0.0.3/postodon/submit_post.py`

 * *Files identical despite different names*

### Comparing `postodon-0.0.2/pyproject.toml` & `postodon-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[project]
+[tool.poetry]
 name = "postodon"
-version = "0.0.2"
-authors = [
-  { name="msleigh", email="msleigh@users.noreply.github.com" },
-]
+version = "0.0.3"
 description = "Post to Mastodon"
+authors = ["msleigh"]
 readme = "README.md"
-requires-python = ">=3.7"
+packages = [{include = "postodon"}]
+license = "Apache-2.0"
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
-dependencies = [
-    "requests",
-]
+"homepage" = "https://github.com/msleigh/postodon"
 
-[project.optional-dependencies]
-dev = [
-  "black",
-]
-docs = [
-  "sphinx",
-]
-tests = [
-  "pytest",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/msleigh/postodon"
+[tool.poetry.urls]
 "Bug Tracker" = "https://github.com/msleigh/postodon/issues"
 "CI" = "https://github.com/msleigh/postodon/actions"
 "Changelog" = "https://github.com/msleigh/postodon/releases"
 
-[project.scripts]
+[tool.poetry.dependencies]
+python = "^3.8"
+requests = "^2.30.0"
+sphinx = "^7.0.1"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs-material = "^9.1.12"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.1"
+
+[tool.project.scripts]
 postodon = "postodon:main"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

