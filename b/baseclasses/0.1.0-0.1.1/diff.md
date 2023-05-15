# Comparing `tmp/baseclasses-0.1.0.tar.gz` & `tmp/baseclasses-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseclasses-0.1.0.tar", last modified: Thu Jan  5 21:46:14 2023, max compression
+gzip compressed data, was "baseclasses-0.1.1.tar", last modified: Sun May 14 23:59:23 2023, max compression
```

## Comparing `baseclasses-0.1.0.tar` & `baseclasses-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:46:14.802157 baseclasses-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:46:14.798157 baseclasses-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:46:14.802157 baseclasses-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-01-05 21:45:58.000000 baseclasses-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-01-05 21:45:58.000000 baseclasses-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-05 21:45:58.000000 baseclasses-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-05 21:45:58.000000 baseclasses-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-01-05 21:46:14.806157 baseclasses-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-01-05 21:45:58.000000 baseclasses-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:46:14.802157 baseclasses-0.1.0/baseclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-05 21:45:58.000000 baseclasses-0.1.0/baseclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-01-05 21:45:58.000000 baseclasses-0.1.0/baseclasses/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 21:45:58.000000 baseclasses-0.1.0/baseclasses/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:46:14.802157 baseclasses-0.1.0/baseclasses/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 21:45:58.000000 baseclasses-0.1.0/baseclasses/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-01-05 21:45:58.000000 baseclasses-0.1.0/baseclasses/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-01-05 21:45:58.000000 baseclasses-0.1.0/baseclasses/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-05 21:46:14.000000 baseclasses-0.1.0/baseclasses/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:46:14.802157 baseclasses-0.1.0/baseclasses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-01-05 21:46:14.000000 baseclasses-0.1.0/baseclasses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-01-05 21:46:14.000000 baseclasses-0.1.0/baseclasses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 21:46:14.000000 baseclasses-0.1.0/baseclasses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-05 21:46:14.000000 baseclasses-0.1.0/baseclasses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-05 21:46:14.000000 baseclasses-0.1.0/baseclasses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-01-05 21:45:58.000000 baseclasses-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-05 21:45:58.000000 baseclasses-0.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-01-05 21:46:14.806157 baseclasses-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:59:23.614187 baseclasses-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:59:23.610186 baseclasses-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:59:23.610186 baseclasses-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-14 23:59:00.000000 baseclasses-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-14 23:59:00.000000 baseclasses-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-14 23:59:00.000000 baseclasses-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 23:59:00.000000 baseclasses-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-14 23:59:23.614187 baseclasses-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-14 23:59:00.000000 baseclasses-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:59:23.614187 baseclasses-0.1.1/baseclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-14 23:59:00.000000 baseclasses-0.1.1/baseclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-05-14 23:59:00.000000 baseclasses-0.1.1/baseclasses/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:59:00.000000 baseclasses-0.1.1/baseclasses/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:59:23.614187 baseclasses-0.1.1/baseclasses/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:59:00.000000 baseclasses-0.1.1/baseclasses/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-14 23:59:00.000000 baseclasses-0.1.1/baseclasses/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-14 23:59:00.000000 baseclasses-0.1.1/baseclasses/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 23:59:23.000000 baseclasses-0.1.1/baseclasses/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:59:23.614187 baseclasses-0.1.1/baseclasses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-14 23:59:23.000000 baseclasses-0.1.1/baseclasses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-14 23:59:23.000000 baseclasses-0.1.1/baseclasses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:59:23.000000 baseclasses-0.1.1/baseclasses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 23:59:23.000000 baseclasses-0.1.1/baseclasses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 23:59:23.000000 baseclasses-0.1.1/baseclasses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-14 23:59:00.000000 baseclasses-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 23:59:00.000000 baseclasses-0.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-14 23:59:23.614187 baseclasses-0.1.1/setup.cfg
```

### Comparing `baseclasses-0.1.0/.github/workflows/publish.yml` & `baseclasses-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/.github/workflows/test.yml` & `baseclasses-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/.gitignore` & `baseclasses-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/LICENSE` & `baseclasses-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/PKG-INFO` & `baseclasses-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseclasses
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dataclasses alternative
 Home-page: https://github.com/yanovs/baseclasses
 License: Apache License 2.0
 Project-URL: Packaging, https://pypi.org/project/baseclasses/
 Project-URL: Source, https://github.com/yanovs/baseclasses
 Project-URL: Tracker, https://github.com/yanovs/baseclasses/issues
 Keywords: dataclasses
```

### Comparing `baseclasses-0.1.0/README.md` & `baseclasses-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/baseclasses/core.py` & `baseclasses-0.1.1/baseclasses/core.py`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/baseclasses/tests/test_compare.py` & `baseclasses-0.1.1/baseclasses/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/baseclasses/tests/test_core.py` & `baseclasses-0.1.1/baseclasses/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/baseclasses.egg-info/PKG-INFO` & `baseclasses-0.1.1/baseclasses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseclasses
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dataclasses alternative
 Home-page: https://github.com/yanovs/baseclasses
 License: Apache License 2.0
 Project-URL: Packaging, https://pypi.org/project/baseclasses/
 Project-URL: Source, https://github.com/yanovs/baseclasses
 Project-URL: Tracker, https://github.com/yanovs/baseclasses/issues
 Keywords: dataclasses
```

### Comparing `baseclasses-0.1.0/pyproject.toml` & `baseclasses-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `baseclasses-0.1.0/setup.cfg` & `baseclasses-0.1.1/setup.cfg`

 * *Files identical despite different names*

