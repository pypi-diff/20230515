# Comparing `tmp/pytest-logikal-1.8.3.tar.gz` & `tmp/pytest-logikal-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-logikal-1.8.3.tar", last modified: Mon May 15 19:12:39 2023, max compression
+gzip compressed data, was "pytest-logikal-1.8.4.tar", last modified: Mon May 15 20:09:18 2023, max compression
```

## Comparing `pytest-logikal-1.8.3.tar` & `pytest-logikal-1.8.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/compose.yml
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/entry_points.ini
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.586800 pytest-logikal-1.8.3/pytest_logikal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/bandit.py
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/bandit_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)    12973 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     8232 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/css.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/css_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/file_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/html.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/isort.py
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/js_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/licenses.py
--rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/package.json
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/pylint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/style.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/svg.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/pytest_logikal/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/pytest_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-15 19:12:39.000000 pytest-logikal-1.8.3/pytest_logikal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-15 19:12:15.000000 pytest-logikal-1.8.3/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-15 19:12:16.000000 pytest-logikal-1.8.3/requirements/extras/browser.txt
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-15 19:12:16.000000 pytest-logikal-1.8.3/requirements/extras/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 19:12:39.590800 pytest-logikal-1.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.226343 pytest-logikal-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/entry_points.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/pytest_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/bandit_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12973 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8232 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/css_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/file_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/isort.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/js_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/package.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/svg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/pytest_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2903 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/extras/browser.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/extras/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 20:09:18.226343 pytest-logikal-1.8.4/setup.cfg
```

### Comparing `pytest-logikal-1.8.3/LICENSE.txt` & `pytest-logikal-1.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/PKG-INFO` & `pytest-logikal-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.8.3
+Version: 1.8.4
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.8.3/entry_points.ini` & `pytest-logikal-1.8.4/entry_points.ini`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pyproject.toml` & `pytest-logikal-1.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/bandit.py` & `pytest-logikal-1.8.4/pytest_logikal/bandit.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/browser.py` & `pytest-logikal-1.8.4/pytest_logikal/browser.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/build.py` & `pytest-logikal-1.8.4/pytest_logikal/build.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/core.py` & `pytest-logikal-1.8.4/pytest_logikal/core.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/css.py` & `pytest-logikal-1.8.4/pytest_logikal/css.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/css_config.yml` & `pytest-logikal-1.8.4/pytest_logikal/css_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/django.py` & `pytest-logikal-1.8.4/pytest_logikal/django.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/docker.py` & `pytest-logikal-1.8.4/pytest_logikal/docker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/docs.py` & `pytest-logikal-1.8.4/pytest_logikal/docs.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/file_checker.py` & `pytest-logikal-1.8.4/pytest_logikal/file_checker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/html.py` & `pytest-logikal-1.8.4/pytest_logikal/html.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/isort.py` & `pytest-logikal-1.8.4/pytest_logikal/isort.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/js.py` & `pytest-logikal-1.8.4/pytest_logikal/js.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/js_config.yml` & `pytest-logikal-1.8.4/pytest_logikal/js_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/licenses.py` & `pytest-logikal-1.8.4/pytest_logikal/licenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     'html-tag-names': 'GNU General Public License v3 or later (GPLv3+)',  # djlint dependency
     'html-void-elements': 'GNU General Public License v3 or later (GPLv3+)',  # djlint dependency
     'pkg_resources': 'UNKNOWN',  # caused by an Ubuntu bug, see [1]
     'pkg-resources': 'UNKNOWN',  # caused by an Ubuntu bug, see [1]
     'Pillow': 'Historical Permission Notice and Disclaimer (HPND)',  # license is BSD-like
     'pylint': 'GNU General Public License v2 (GPLv2)',  # only used as a local tool
     'pylint-django': 'GPLv2',  # only used as a local tool plugin
-    'pylint-plugin-utils': 'GPLv2',  # only used as a local tool plugin
+    'pylint-plugin-utils': 'GNU General Public License v2 or later (GPLv2+)',  # local tool plugin
     'python-lsp-jsonrpc': 'UNKNOWN',  # license is MIT
 }
 # [1] https://bugs.launchpad.net/ubuntu/+source/python-pip/+bug/1635463
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
     group = parser.getgroup('licenses')
```

### Comparing `pytest-logikal-1.8.3/pytest_logikal/package-lock.json` & `pytest-logikal-1.8.4/pytest_logikal/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/plugin.py` & `pytest-logikal-1.8.4/pytest_logikal/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/pylint.py` & `pytest-logikal-1.8.4/pytest_logikal/pylint.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/requirements.py` & `pytest-logikal-1.8.4/pytest_logikal/requirements.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/style.py` & `pytest-logikal-1.8.4/pytest_logikal/style.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/svg.py` & `pytest-logikal-1.8.4/pytest_logikal/svg.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/utils.py` & `pytest-logikal-1.8.4/pytest_logikal/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal/validator.py` & `pytest-logikal-1.8.4/pytest_logikal/validator.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal.egg-info/PKG-INFO` & `pytest-logikal-1.8.4/pytest_logikal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.8.3
+Version: 1.8.4
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.8.3/pytest_logikal.egg-info/SOURCES.txt` & `pytest-logikal-1.8.4/pytest_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal.egg-info/entry_points.txt` & `pytest-logikal-1.8.4/pytest_logikal.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/pytest_logikal.egg-info/requires.txt` & `pytest-logikal-1.8.4/pytest_logikal.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 bandit==1.7.5
 coverage[toml]==7.2.5
 isort[colors]==5.12.0
-mypy==1.2.0
+mypy==1.3.0
 pip-licenses==4.3.1
 pycodestyle==2.10.0
 pydocstyle[toml]==6.3.0
 pylint==2.17.4
 pytest==7.3.1
 pytest-cov==4.0.0
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist[psutil]==3.2.1
+pytest-xdist[psutil]==3.3.0
 Pillow~=9.4
 Pygments~=2.15
 docker~=6.1
 pyorbs~=2.0
 termcolor~=2.3
 tomli~=2.0
 
 [browser]
 selenium==4.9.1
 
 [django]
 Django~=4.2
 django-stubs~=4.2
 django-migration-linter~=4.1
-djlint==1.25.1
+djlint==1.27.2
 pylint-django==2.5.3
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
 requests~=2.28
 types-requests~=2.28
```

### Comparing `pytest-logikal-1.8.3/requirements/build.txt.lock` & `pytest-logikal-1.8.4/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.3/requirements/dev.txt.lock` & `pytest-logikal-1.8.4/requirements/dev.txt.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 2134406769d7050fa4ae6847b899158b56f34fa84fc3e5ecc4643794e28391da
+##  Requirements hash: 0e455408c9c56e0a39bdb8aacd526635799e910415fdf1a72a6ed693a7454a65
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.6.0
-astroid==2.15.4
+astroid==2.15.5
 async-generator==1.10
 attrs==23.1.0
 Babel==2.12.1
 backports.zoneinfo==0.2.1
 bandit==1.7.5
 bleach==6.0.0
 build==0.10.0
@@ -27,16 +27,16 @@
 cryptography==40.0.2
 cssbeautifier==1.14.7
 dill==0.3.6
 Django==4.2.1
 django-migration-linter==4.1.0
 django-stubs==4.2.0
 django-stubs-ext==4.2.0
-djlint==1.25.1
-docker==6.1.1
+djlint==1.27.2
+docker==6.1.2
 docutils==0.17.1
 EditorConfig==0.12.3
 exceptiongroup==1.1.1
 execnet==1.9.0
 factory-boy==3.2.1
 Faker==18.7.0
 filelock==3.12.0
@@ -52,54 +52,54 @@
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.12.0
 jaraco.classes==3.2.3
 jeepney==0.8.0
 Jinja2==3.1.2
 jsbeautifier==1.14.7
-json5==0.9.11
+json5==0.9.14
 keyring==23.13.1
 lazy-object-proxy==1.9.0
 logikal-docs==1.1.3
 markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==9.1.0
-mypy==1.2.0
+mypy==1.3.0
 mypy-extensions==1.0.0
 outcome==1.2.0
 packaging==23.1
 pathspec==0.11.1
 pbr==5.11.1
 Pillow==9.5.0
 pip==23.1.2
 pip-licenses==4.3.1
 pkginfo==1.9.6
-platformdirs==3.5.0
+platformdirs==3.5.1
 pluggy==1.0.0
 prettytable==3.7.0
 psutil==5.9.5
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
 Pygments==2.15.1
 pylint==2.17.4
 pylint-django==2.5.3
-pylint-plugin-utils==0.7
+pylint-plugin-utils==0.8.1
 pyorbs==2.0.0
 pyproject_hooks==1.0.0
 PySocks==1.7.1
 pytest==7.3.1
 pytest-cov==4.0.0
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist==3.2.1
+pytest-xdist==3.3.0
 python-dateutil==2.8.2
 pytz==2023.3
 PyYAML==6.0
 readme-renderer==37.3
 regex==2023.5.5
 requests==2.30.0
 requests-toolbelt==1.0.0
@@ -118,27 +118,27 @@
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sqlparse==0.4.4
-stevedore==5.0.0
+stevedore==5.1.0
 termcolor==2.3.0
 toml==0.10.2
 tomli==2.0.1
 tomlkit==0.11.8
 tqdm==4.65.0
 trio==0.22.0
 trio-websocket==0.10.2
 twine==4.0.2
 types-pytz==2023.3.0.0
 types-PyYAML==6.0.12.9
 types-requests==2.30.0.0
-types-urllib3==1.26.25.12
+types-urllib3==1.26.25.13
 typing_extensions==4.5.0
 urllib3==2.0.2
 wcwidth==0.2.6
 webencodings==0.5.1
 websocket-client==1.5.1
 wheel==0.40.0
 wrapt==1.15.0
```

### Comparing `pytest-logikal-1.8.3/requirements/docs.txt.lock` & `pytest-logikal-1.8.4/requirements/docs.txt.lock`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 0e866b1bea523e49e31423bce6ea72139b00106fcba40e86d373d7074e56c7ba
+##  Requirements hash: d7e5b7eb5d25fb787135d9a9cd3f8e57d6592a677f77275b1a41f8a7d293f5d1
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.6.0
-astroid==2.15.4
+astroid==2.15.5
 async-generator==1.10
 attrs==23.1.0
 Babel==2.12.1
 backports.zoneinfo==0.2.1
 bandit==1.7.5
 certifi==2023.5.7
 charset-normalizer==3.1.0
@@ -23,16 +23,16 @@
 coverage==7.2.5
 cssbeautifier==1.14.7
 dill==0.3.6
 Django==4.2.1
 django-migration-linter==4.1.0
 django-stubs==4.2.0
 django-stubs-ext==4.2.0
-djlint==1.25.1
-docker==6.1.1
+djlint==1.27.2
+docker==6.1.2
 docutils==0.17.1
 EditorConfig==0.12.3
 exceptiongroup==1.1.1
 execnet==1.9.0
 factory-boy==3.2.1
 Faker==18.7.0
 filelock==3.12.0
@@ -45,49 +45,49 @@
 imagesize==1.4.1
 importlib-metadata==6.6.0
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.12.0
 Jinja2==3.1.2
 jsbeautifier==1.14.7
-json5==0.9.11
+json5==0.9.14
 lazy-object-proxy==1.9.0
 logikal-docs==1.1.3
 markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 mccabe==0.7.0
 mdurl==0.1.2
-mypy==1.2.0
+mypy==1.3.0
 mypy-extensions==1.0.0
 outcome==1.2.0
 packaging==23.1
 pathspec==0.11.1
 pbr==5.11.1
 Pillow==9.5.0
 pip==23.1.2
 pip-licenses==4.3.1
-platformdirs==3.5.0
+platformdirs==3.5.1
 pluggy==1.0.0
 prettytable==3.7.0
 psutil==5.9.5
 pycodestyle==2.10.0
 pydocstyle==6.3.0
 Pygments==2.15.1
 pylint==2.17.4
 pylint-django==2.5.3
-pylint-plugin-utils==0.7
+pylint-plugin-utils==0.8.1
 pyorbs==2.0.0
 PySocks==1.7.1
 pytest==7.3.1
 pytest-cov==4.0.0
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist==3.2.1
+pytest-xdist==3.3.0
 python-dateutil==2.8.2
 pytz==2023.3
 PyYAML==6.0
 regex==2023.5.5
 requests==2.30.0
 rich==13.3.5
 selenium==4.9.1
@@ -102,26 +102,26 @@
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sqlparse==0.4.4
-stevedore==5.0.0
+stevedore==5.1.0
 termcolor==2.3.0
 toml==0.10.2
 tomli==2.0.1
 tomlkit==0.11.8
 tqdm==4.65.0
 trio==0.22.0
 trio-websocket==0.10.2
 types-pytz==2023.3.0.0
 types-PyYAML==6.0.12.9
 types-requests==2.30.0.0
-types-urllib3==1.26.25.12
+types-urllib3==1.26.25.13
 typing_extensions==4.5.0
 urllib3==2.0.2
 wcwidth==0.2.6
 websocket-client==1.5.1
 wheel==0.40.0
 wrapt==1.15.0
 wsproto==1.2.0
```

