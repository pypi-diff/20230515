# Comparing `tmp/pkgsettings-1.0.0.tar.gz` & `tmp/pkgsettings-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgsettings-1.0.0.tar", last modified: Wed Apr  6 12:24:52 2022, max compression
+gzip compressed data, was "pkgsettings-1.1.0.tar", last modified: Mon May 15 14:34:42 2023, max compression
```

## Comparing `pkgsettings-1.0.0.tar` & `pkgsettings-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:24:52.771464 pkgsettings-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:24:52.767464 pkgsettings-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:24:52.767464 pkgsettings-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2451 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     4475 2022-04-06 12:24:52.771464 pkgsettings-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:24:52.767464 pkgsettings-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:24:52.767464 pkgsettings-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/docs/_static/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (121)     9870 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6991 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:24:52.767464 pkgsettings-1.0.0/pkgsettings/
--rwxr-xr-x   0 runner    (1001) docker     (121)      210 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/pkgsettings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3549 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/pkgsettings/pkgsettings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 12:24:52.771464 pkgsettings-1.0.0/pkgsettings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4475 2022-04-06 12:24:52.000000 pkgsettings-1.0.0/pkgsettings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-04-06 12:24:52.000000 pkgsettings-1.0.0/pkgsettings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 12:24:52.000000 pkgsettings-1.0.0/pkgsettings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 12:24:52.000000 pkgsettings-1.0.0/pkgsettings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-06 12:24:52.000000 pkgsettings-1.0.0/pkgsettings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-06 12:24:52.000000 pkgsettings-1.0.0/pkgsettings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-04-06 12:24:52.771464 pkgsettings-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-04-06 12:24:37.000000 pkgsettings-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.726378 pkgsettings-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.726378 pkgsettings-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/_static/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9870 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/pkgsettings/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/pkgsettings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4363 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/pkgsettings/pkgsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/pkgsettings/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/pkgsettings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/tox.ini
```

### Comparing `pkgsettings-1.0.0/.editorconfig` & `pkgsettings-1.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.0.0/.gitchangelog.rc` & `pkgsettings-1.1.0/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.0.0/.github/workflows/publish.yml` & `pkgsettings-1.1.0/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     types: [published]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.10'
+        python-version: '3.11'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
```

### Comparing `pkgsettings-1.0.0/.github/workflows/tests.yml` & `pkgsettings-1.1.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 name: Unit tests
 
-on: [push, pull_request]
+on:
+  push:
+    branches:
+    - master
+  pull_request:
+    branches:
+    - master
 
 jobs:
   build:
     name: Unit tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        cache: pip
     - name: Install Tox and other dependencies
       run: pip install tox tox-docker wheel twine
     - name: Run tests with Tox
       # Run tox using the version of Python in `PATH`
       run: tox -e py
     - name: Test package build
       run: |
```

### Comparing `pkgsettings-1.0.0/.gitignore` & `pkgsettings-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.0.0/Changelog.md` & `pkgsettings-1.1.0/Changelog.md`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.0.0/Makefile` & `pkgsettings-1.1.0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # This Makefile requires the following commands to be available:
-# * python3.10
+# * python3.11
 
 SRC:=pkgsettings tests setup.py
 
 .PHONY: pyclean
 pyclean:
 	-find . -name "*.pyc" -delete
 	-rm -rf *.egg-info build
 	-rm -rf coverage*.xml .coverage
 
 .PHONY: clean
 clean: pyclean
 	-rm -rf venv
 	-rm -rf .tox
 
-venv: PYTHON?=python3.10
+venv: PYTHON?=python3.11
 venv:
 	$(PYTHON) -m venv venv
-	# FIXME: unpin when https://github.com/pypa/pip/issues/9215 is fixed
-	venv/bin/pip install -U "pip==20.2" -q
+	venv/bin/pip install -U pip -q
 	venv/bin/pip install -r requirements.txt '.[all]'
 
 ## Code style
 .PHONY: lint
 lint: lint/black lint/flake8 lint/isort lint/mypy
 
 .PHONY: lint/black
```

### Comparing `pkgsettings-1.0.0/PKG-INFO` & `pkgsettings-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 Metadata-Version: 2.1
 Name: pkgsettings
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python package to ease the configuration of packages
 Home-page: https://github.com/kpn/py-pkgsettings
 Author: KPN DE Platform
 Author-email: de-platform@kpn.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: elasticsearch
 License-File: LICENSE
 
 # pkgsettings
 
 [![image](https://github.com/kpn/py-pkgsettings/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/kpn/py-pkgsettings/actions/workflows/tests.yml)
-
 [![image](https://img.shields.io/codecov/c/github/kpn-digital/py-pkgsettings/master.svg)](https://codecov.io/github/kpn-digital/py-pkgsettings?branch=master)
-
 [![image](https://img.shields.io/pypi/v/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://img.shields.io/pypi/pyversions/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://readthedocs.org/projects/py-pkgsettings/badge/?version=latest)](https://py-pkgsettings.readthedocs.org/en/latest/?badge=latest)
-
 [![image](https://img.shields.io/pypi/l/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/kpn/py-pkgsettings)
 
 ## Goal
 
 The goal of this package is to offer an easy, generic and extendable way
 of configuring a package.
 
@@ -143,9 +133,7 @@
 foo_settings = PrefixedSettings(settings, 'FOO_')
 
 foo_settings.a # This will print: a
 foo_settings.b # This will print: b
 
 foo_settings.c # This will raise an AttributeError
 ```
-
-
```

### Comparing `pkgsettings-1.0.0/README.md` & `pkgsettings-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 # pkgsettings
 
 [![image](https://github.com/kpn/py-pkgsettings/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/kpn/py-pkgsettings/actions/workflows/tests.yml)
-
 [![image](https://img.shields.io/codecov/c/github/kpn-digital/py-pkgsettings/master.svg)](https://codecov.io/github/kpn-digital/py-pkgsettings?branch=master)
-
 [![image](https://img.shields.io/pypi/v/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://img.shields.io/pypi/pyversions/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://readthedocs.org/projects/py-pkgsettings/badge/?version=latest)](https://py-pkgsettings.readthedocs.org/en/latest/?badge=latest)
-
 [![image](https://img.shields.io/pypi/l/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/kpn/py-pkgsettings)
 
 ## Goal
 
 The goal of this package is to offer an easy, generic and extendable way
 of configuring a package.
```

### Comparing `pkgsettings-1.0.0/docs/Makefile` & `pkgsettings-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.0.0/docs/conf.py` & `pkgsettings-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.0.0/docs/make.bat` & `pkgsettings-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.0.0/pkgsettings/pkgsettings.py` & `pkgsettings-1.1.0/pkgsettings/pkgsettings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,88 @@
+from __future__ import annotations
+
 import functools
 import warnings
+from typing import Any, Callable, Dict, Generator, Optional, TypeVar, overload
+
+from typing_extensions import Self
+
+_F = TypeVar("_F", bound=Callable[..., Any])
 
 
 class DuplicateConfigureWarning(UserWarning):
     pass
 
 
-class SimpleSettings(object):
-    def as_dict(self):
+class SimpleSettings:
+    """
+    A single layer of settings.
+
+    Layers get stacked on each other in `Settings`, so allowing to override specific options.
+    """
+
+    def as_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
-class Settings(object):
-    def __init__(self):
+class Settings:
+    def __init__(self) -> None:
         self._chain = [SimpleSettings()]
-        self._override_settings = {}
+        self._override_settings: Dict[str, Any] = {}
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Any:
         for item in self._chain:
             try:
                 return getattr(item, attr)
             except AttributeError:
                 pass
         raise AttributeError(attr)
 
-    def as_dict(self):
-        result = dict()
+    def as_dict(self) -> Dict[str, Any]:
+        result = {}
         for item in reversed(self._chain):
             result.update(item.as_dict())
         return result
 
-    def children(self):
+    def children(self) -> Generator[SimpleSettings, None, None]:
         """
         Tries to return a generator of all settings objects in the chain, recursively.
         This might not yield all settings objects, if they include
-        other settings objects not by using the children() call.
+        other settings objects not by using the `children()` call.
+
         :return: generator of settings objects.
         """
         for child in self._chain:
             yield child
             children = getattr(child, "children", None)
             if callable(children):
                 for settings in children():
                     yield settings
 
-    def _has_duplicates(self):
+    def _has_duplicates(self) -> bool:
         """
         Check if there are duplicates in the chained settings objects.
+
         :return: True if there are duplicate, False otherwise.
         """
         children = set()
         for settings in self.children():
             if settings in children:
                 return True
 
             children.add(settings)
 
         return False
 
-    def configure(self, obj=None, **kwargs):
+    def configure(self, obj: Optional[Any] = None, **kwargs) -> None:
         """
         Settings that will be used by the time_execution decorator
 
-        Attributes:
-            obj (Optional[object]): Class or object with the settings as attributes
-            backends (list): List of backends
-            hooks (list): List of hooks
-            duration_field (string): Name of the field to store the duration value
+        Args:
+            obj: class or object with the settings as attributes
         """
         if not obj:
             obj = SimpleSettings()
             for key, new_value in kwargs.items():
                 setattr(obj, key, new_value)
 
         if obj is self:
@@ -78,47 +90,68 @@
             return
 
         self._chain.insert(0, obj)
 
         if self._has_duplicates():
             warnings.warn("One setting was added multiple times, maybe a loop?", DuplicateConfigureWarning)
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         self._override_enable()
+        return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
         self._override_disable()
 
-    def __call__(self, func=None, *args, **kwargs):
+    @overload
+    def __call__(self, func: _F) -> _F:
+        ...
+
+    @overload
+    def __call__(self, **override_settings: Any) -> Self:
+        ...
+
+    def __call__(self, func=None, **override_settings: Any):
+        """
+        Override settings for a decorated function.
+
+        Example:
+             >>> settings = Settings()
+             >>>
+             >>> @settings(option=42)
+             >>> def foo():
+             >>>     assert settings.option == 42
+        """
+
         if func:
 
             @functools.wraps(func)
             def inner(*args, **kwargs):
                 with self:
                     return func(*args, **kwargs)
 
             return inner
-        elif kwargs:
-            self._override_settings = kwargs
+
+        elif override_settings:
+            self._override_settings = override_settings
             return self
 
-    def _override_enable(self):
+    def _override_enable(self) -> None:
         obj = SimpleSettings()
         for key, new_value in self._override_settings.items():
             setattr(obj, key, new_value)
 
         self._chain.insert(0, obj)
 
-    def _override_disable(self):
+    def _override_disable(self) -> None:
         self._chain.pop(0)
         self._override_settings = {}
 
 
-class PrefixedSettings(object):
-    def __init__(self, settings, prefix=None):
+class PrefixedSettings:
+    def __init__(self, settings: Any, prefix: Optional[str] = None) -> None:
         self.settings = settings
         self.prefix = prefix
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Any:
         if self.prefix:
             attr = self.prefix + attr
         return getattr(self.settings, attr)
```

### Comparing `pkgsettings-1.0.0/pkgsettings.egg-info/PKG-INFO` & `pkgsettings-1.1.0/pkgsettings.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 Metadata-Version: 2.1
 Name: pkgsettings
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python package to ease the configuration of packages
 Home-page: https://github.com/kpn/py-pkgsettings
 Author: KPN DE Platform
 Author-email: de-platform@kpn.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: elasticsearch
 License-File: LICENSE
 
 # pkgsettings
 
 [![image](https://github.com/kpn/py-pkgsettings/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/kpn/py-pkgsettings/actions/workflows/tests.yml)
-
 [![image](https://img.shields.io/codecov/c/github/kpn-digital/py-pkgsettings/master.svg)](https://codecov.io/github/kpn-digital/py-pkgsettings?branch=master)
-
 [![image](https://img.shields.io/pypi/v/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://img.shields.io/pypi/pyversions/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://readthedocs.org/projects/py-pkgsettings/badge/?version=latest)](https://py-pkgsettings.readthedocs.org/en/latest/?badge=latest)
-
 [![image](https://img.shields.io/pypi/l/pkgsettings.svg)](https://pypi.org/project/pkgsettings)
-
 [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/kpn/py-pkgsettings)
 
 ## Goal
 
 The goal of this package is to offer an easy, generic and extendable way
 of configuring a package.
 
@@ -143,9 +133,7 @@
 foo_settings = PrefixedSettings(settings, 'FOO_')
 
 foo_settings.a # This will print: a
 foo_settings.b # This will print: b
 
 foo_settings.c # This will raise an AttributeError
 ```
-
-
```

### Comparing `pkgsettings-1.0.0/pkgsettings.egg-info/SOURCES.txt` & `pkgsettings-1.1.0/pkgsettings.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.github/CODEOWNERS
 .github/workflows/lint.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/license.rst
 docs/make.bat
 docs/usage.rst
 docs/_static/.gitignore
 pkgsettings/__init__.py
 pkgsettings/pkgsettings.py
+pkgsettings/py.typed
 pkgsettings.egg-info/PKG-INFO
 pkgsettings.egg-info/SOURCES.txt
 pkgsettings.egg-info/dependency_links.txt
 pkgsettings.egg-info/not-zip-safe
 pkgsettings.egg-info/requires.txt
 pkgsettings.egg-info/top_level.txt
```

### Comparing `pkgsettings-1.0.0/pyproject.toml` & `pkgsettings-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.black]
 line-length = 120
-target_version = ["py37", "py38", "py39", "py310"]
+target_version = ["py37", "py38", "py39", "py310", "py311"]
 
 [tool.isort]
 combine_as_imports = true
 default_section = "THIRDPARTY"
 known_first_party = ["pkgsettings", "tests"]
 from_first = false
 include_trailing_comma = true
@@ -24,10 +24,9 @@
 omit = ["tests/*"]
 
 [tool.setuptools_scm]
 
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm[toml]>=3.4"]
 
-[[tool.mypy.overrides]]
-module = ["setuptools"]
-ignore_missing_imports = true
+[tool.mypy]
+check_untyped_defs = true
```

### Comparing `pkgsettings-1.0.0/setup.py` & `pkgsettings-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 #!/usr/bin/env python
-# setuptools doesn't support type hints for now:
-# https://github.com/pypa/setuptools/issues/2345
-# so we ignoring mypy checks on this package
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
@@ -14,19 +11,17 @@
     setup_requires=["setuptools_scm"],
     description="Python package to ease the configuration of packages",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="KPN DE Platform",
     author_email="de-platform@kpn.com",
     url="https://github.com/kpn/py-pkgsettings",
-    install_requires=[],
-    extras_require={
-        "all": ["elasticsearch>=5.0.0,<7.0.0"],
-        "elasticsearch": ["elasticsearch>=5.0.0,<7.0.0"],
-    },
+    install_requires=[
+        "typing-extensions>=4.5.0,<5.0.0",
+    ],
     packages=find_packages(exclude=["tests*"]),
     tests_require=["tox"],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

