# Comparing `tmp/pytest-logikal-1.8.2.tar.gz` & `tmp/pytest-logikal-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-logikal-1.8.2.tar", last modified: Sun May 14 19:55:04 2023, max compression
+gzip compressed data, was "pytest-logikal-1.8.3.tar", last modified: Mon May 15 19:12:39 2023, max compression
```

## Comparing `pytest-logikal-1.8.2.tar` & `pytest-logikal-1.8.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 19:55:04.473800 pytest-logikal-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-14 19:55:04.473800 pytest-logikal-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/compose.yml
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/entry_points.ini
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 19:55:04.473800 pytest-logikal-1.8.2/pytest_logikal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/bandit.py
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/bandit_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)    12973 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     8232 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/css.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/css_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/file_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/html.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/isort.py
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/js_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/licenses.py
--rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/package.json
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/pylint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/style.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/svg.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/pytest_logikal/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 19:55:04.473800 pytest-logikal-1.8.2/pytest_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-14 19:55:04.000000 pytest-logikal-1.8.2/pytest_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-14 19:55:04.000000 pytest-logikal-1.8.2/pytest_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 19:55:04.000000 pytest-logikal-1.8.2/pytest_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-14 19:55:04.000000 pytest-logikal-1.8.2/pytest_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-14 19:55:04.000000 pytest-logikal-1.8.2/pytest_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-14 19:55:04.000000 pytest-logikal-1.8.2/pytest_logikal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 19:55:04.473800 pytest-logikal-1.8.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 19:55:04.473800 pytest-logikal-1.8.2/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/extras/browser.txt
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-14 19:54:40.000000 pytest-logikal-1.8.2/requirements/extras/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-14 19:55:04.473800 pytest-logikal-1.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/entry_points.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.586800 pytest-logikal-1.8.3/pytest_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/bandit_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12973 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8232 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/css_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/file_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/isort.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/js_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/package.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/svg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/pytest_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-15 19:12:16.000000 pytest-logikal-1.8.3/requirements/extras/browser.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-15 19:12:16.000000 pytest-logikal-1.8.3/requirements/extras/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/setup.cfg
```

### Comparing `pytest-logikal-1.8.2/LICENSE.txt` & `pytest-logikal-1.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/PKG-INFO` & `pytest-logikal-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.8.2
+Version: 1.8.3
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.8.2/entry_points.ini` & `pytest-logikal-1.8.3/entry_points.ini`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pyproject.toml` & `pytest-logikal-1.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/bandit.py` & `pytest-logikal-1.8.3/pytest_logikal/bandit.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/browser.py` & `pytest-logikal-1.8.3/pytest_logikal/browser.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/build.py` & `pytest-logikal-1.8.3/pytest_logikal/build.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/core.py` & `pytest-logikal-1.8.3/pytest_logikal/core.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/css.py` & `pytest-logikal-1.8.3/pytest_logikal/css.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/css_config.yml` & `pytest-logikal-1.8.3/pytest_logikal/css_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/django.py` & `pytest-logikal-1.8.3/pytest_logikal/django.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/docker.py` & `pytest-logikal-1.8.3/pytest_logikal/docker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/docs.py` & `pytest-logikal-1.8.3/pytest_logikal/docs.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/file_checker.py` & `pytest-logikal-1.8.3/pytest_logikal/file_checker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/html.py` & `pytest-logikal-1.8.3/pytest_logikal/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         #     errors = process.stdout.strip().replace('@@\n\n', '@@\n')
         #     errors = '\n'.join(self._color_diff(line) for line in errors.splitlines()[2:-2])
         #     messages.append(errors or process.stderr.strip())
 
         # Lint
         ignore = [
             'H023',  # we allow some entity references (e.g. quotes, special spaces, dashes)
+            'H031',  # meta keywords are not that useful anymore
             'J004', 'J018',  # we have our own functions for Jinja environments
             'T002',  # we always use single quotes
             'T003',  # we don't mandate named end blocks
         ]
         command = ['djlint', '--lint', '--ignore', ','.join(ignore), *common_args]
         process = subprocess.run(command, capture_output=True, text=True, check=False)  # nosec
         if process.returncode:
```

### Comparing `pytest-logikal-1.8.2/pytest_logikal/isort.py` & `pytest-logikal-1.8.3/pytest_logikal/isort.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/js.py` & `pytest-logikal-1.8.3/pytest_logikal/js.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/js_config.yml` & `pytest-logikal-1.8.3/pytest_logikal/js_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/licenses.py` & `pytest-logikal-1.8.3/pytest_logikal/licenses.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/package-lock.json` & `pytest-logikal-1.8.3/pytest_logikal/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/plugin.py` & `pytest-logikal-1.8.3/pytest_logikal/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/pylint.py` & `pytest-logikal-1.8.3/pytest_logikal/pylint.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/requirements.py` & `pytest-logikal-1.8.3/pytest_logikal/requirements.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/style.py` & `pytest-logikal-1.8.3/pytest_logikal/style.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/svg.py` & `pytest-logikal-1.8.3/pytest_logikal/svg.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/utils.py` & `pytest-logikal-1.8.3/pytest_logikal/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal/validator.py` & `pytest-logikal-1.8.3/pytest_logikal/validator.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal.egg-info/PKG-INFO` & `pytest-logikal-1.8.3/pytest_logikal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.8.2
+Version: 1.8.3
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.8.2/pytest_logikal.egg-info/SOURCES.txt` & `pytest-logikal-1.8.3/pytest_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal.egg-info/entry_points.txt` & `pytest-logikal-1.8.3/pytest_logikal.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/pytest_logikal.egg-info/requires.txt` & `pytest-logikal-1.8.3/pytest_logikal.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/requirements/build.txt.lock` & `pytest-logikal-1.8.3/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/requirements/dev.txt.lock` & `pytest-logikal-1.8.3/requirements/dev.txt.lock`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.2/requirements/docs.txt.lock` & `pytest-logikal-1.8.3/requirements/docs.txt.lock`

 * *Files identical despite different names*

