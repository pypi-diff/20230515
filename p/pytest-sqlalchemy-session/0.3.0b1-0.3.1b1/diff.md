# Comparing `tmp/pytest-sqlalchemy-session-0.3.0b1.tar.gz` & `tmp/pytest-sqlalchemy-session-0.3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sqlalchemy-session-0.3.0b1.tar", last modified: Fri May  5 13:18:11 2023, max compression
+gzip compressed data, was "pytest-sqlalchemy-session-0.3.1b1.tar", last modified: Mon May 15 19:54:29 2023, max compression
```

## Comparing `pytest-sqlalchemy-session-0.3.0b1.tar` & `pytest-sqlalchemy-session-0.3.1b1.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/tests/test_strict_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:54:29.826231 pytest-sqlalchemy-session-0.3.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-15 19:54:29.826231 pytest-sqlalchemy-session-0.3.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:54:29.826231 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:54:29.826231 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-15 19:54:29.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 19:54:29.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:54:29.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 19:54:29.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 19:54:29.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 19:54:29.000000 pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:54:29.826231 pytest-sqlalchemy-session-0.3.1b1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-15 19:54:29.826231 pytest-sqlalchemy-session-0.3.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:54:29.826231 pytest-sqlalchemy-session-0.3.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-15 19:54:20.000000 pytest-sqlalchemy-session-0.3.1b1/tests/test_strict_mode.py
```

### Comparing `pytest-sqlalchemy-session-0.3.0b1/LICENSE` & `pytest-sqlalchemy-session-0.3.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.0b1/PKG-INFO` & `pytest-sqlalchemy-session-0.3.1b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sqlalchemy-session
-Version: 0.3.0b1
+Version: 0.3.1b1
 Summary: A pytest plugin for preserving test isolation that use SQLAlchemy.
 Author-email: Stanislav Shkitin <stanislav.shkitin@yandex.ru>
 License: MIT
 Keywords: pytest,sqlalchemy,transaction
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-sqlalchemy-session-0.3.0b1/pyproject.toml` & `pytest-sqlalchemy-session-0.3.1b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pytest-sqlalchemy-session'
-version = "0.3.0-beta1"
+version = "0.3.1-beta1"
 authors = [
     {name = "Stanislav Shkitin", email = "stanislav.shkitin@yandex.ru"},
 ]
 license = {text = "MIT"}
 description = "A pytest plugin for preserving test isolation that use SQLAlchemy."
 keywords = ["pytest", "sqlalchemy", "transaction"]
 readme = "README.md"
@@ -34,11 +34,11 @@
 ]
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements/base.txt"]}
 
 [tool.setuptools]
-py-modules = ["pytest_sqlalchemy_session"]
+packages = ["pytest_sqlalchemy_session"]
 
 [project.entry-points.pytest11]
 pytest-sqlalchemy-session = "pytest_sqlalchemy_session.plugin"
```

### Comparing `pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/PKG-INFO` & `pytest-sqlalchemy-session-0.3.1b1/pytest_sqlalchemy_session.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sqlalchemy-session
-Version: 0.3.0b1
+Version: 0.3.1b1
 Summary: A pytest plugin for preserving test isolation that use SQLAlchemy.
 Author-email: Stanislav Shkitin <stanislav.shkitin@yandex.ru>
 License: MIT
 Keywords: pytest,sqlalchemy,transaction
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-sqlalchemy-session-0.3.0b1/setup.cfg` & `pytest-sqlalchemy-session-0.3.1b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.0b1/tests/test_configs.py` & `pytest-sqlalchemy-session-0.3.1b1/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.0b1/tests/test_strict_mode.py` & `pytest-sqlalchemy-session-0.3.1b1/tests/test_strict_mode.py`

 * *Files identical despite different names*

