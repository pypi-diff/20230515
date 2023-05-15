# Comparing `tmp/pyatlan-0.0.30.tar.gz` & `tmp/pyatlan-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.30.tar", last modified: Thu May 11 19:35:36 2023, max compression
+gzip compressed data, was "pyatlan-0.0.31.tar", last modified: Mon May 15 11:10:35 2023, max compression
```

## Comparing `pyatlan-0.0.30.tar` & `pyatlan-0.0.31.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.730618 pyatlan-0.0.30/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-11 19:35:25.000000 pyatlan-0.0.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 19:35:25.000000 pyatlan-0.0.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-11 19:35:25.000000 pyatlan-0.0.30/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-11 19:35:36.730618 pyatlan-0.0.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-11 19:35:25.000000 pyatlan-0.0.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.726618 pyatlan-0.0.30/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.726618 pyatlan-0.0.30/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   869422 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:35:36.730618 pyatlan-0.0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-11 19:35:25.000000 pyatlan-0.0.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.726618 pyatlan-0.0.30/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.726618 pyatlan-0.0.30/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33620 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.730618 pyatlan-0.0.30/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.751690 pyatlan-0.0.31/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-15 11:10:21.000000 pyatlan-0.0.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 11:10:21.000000 pyatlan-0.0.31/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-15 11:10:21.000000 pyatlan-0.0.31/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-15 11:10:35.751690 pyatlan-0.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-15 11:10:21.000000 pyatlan-0.0.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.739690 pyatlan-0.0.31/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.739690 pyatlan-0.0.31/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.739690 pyatlan-0.0.31/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26718 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.743690 pyatlan-0.0.31/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.743690 pyatlan-0.0.31/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.747690 pyatlan-0.0.31/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   869422 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16624 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.739690 pyatlan-0.0.31/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:10:35.751690 pyatlan-0.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-15 11:10:21.000000 pyatlan-0.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.747690 pyatlan-0.0.31/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.747690 pyatlan-0.0.31/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/role_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33620 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.747690 pyatlan-0.0.31/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.30/LICENSE` & `pyatlan-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/PKG-INFO` & `pyatlan-0.0.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.30
+Version: 0.0.31
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.30/README.md` & `pyatlan-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.31/pyatlan/cache/classification_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     cache_by_id: dict[str, ClassificationDef] = dict()
     map_id_to_name: dict[str, str] = dict()
     map_name_to_id: dict[str, str] = dict()
     deleted_ids: set[str] = set()
     deleted_names: set[str] = set()
 
     @classmethod
-    def _refresh_cache(cls) -> None:
+    def refresh_cache(cls) -> None:
         from pyatlan.client.atlan import AtlanClient
 
         client = AtlanClient.get_default_client()
         if client is None:
             client = AtlanClient()
         response = client.get_typedefs(type_category=AtlanTypeCategory.CLASSIFICATION)
         if response is not None:
@@ -37,15 +37,15 @@
     def get_id_for_name(cls, name: str) -> Optional[str]:
         """
         Translate the provided human-readable classification name to its Atlan-internal ID string.
         """
         cls_id = cls.map_name_to_id.get(name)
         if not cls_id and name not in cls.deleted_names:
             # If not found, refresh the cache and look again (could be stale)
-            cls._refresh_cache()
+            cls.refresh_cache()
             cls_id = cls.map_name_to_id.get(name)
             if not cls_id:
                 # If still not found after refresh, mark it as deleted (could be
                 # an entry in an audit log that refers to a classification that
                 # no longer exists)
                 cls.deleted_names.add(name)
         return cls_id
@@ -54,15 +54,15 @@
     def get_name_for_id(cls, idstr: str) -> Optional[str]:
         """
         Translate the provided Atlan-internal classification ID string to the human-readable classification name.
         """
         cls_name = cls.map_id_to_name.get(idstr)
         if not cls_name and idstr not in cls.deleted_ids:
             # If not found, refresh the cache and look again (could be stale)
-            cls._refresh_cache()
+            cls.refresh_cache()
             cls_name = cls.map_id_to_name.get(idstr)
             if not cls_name:
                 # If still not found after refresh, mark it as deleted (could be
                 # an entry in an audit log that refers to a classification that
                 # no longer exists)
                 cls.deleted_ids.add(idstr)
         return cls_name
```

### Comparing `pyatlan-0.0.30/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.31/pyatlan/cache/custom_metadata_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     map_name_to_id: dict[str, str] = dict()
     map_attr_id_to_name: dict[str, dict[str, str]] = dict()
     map_attr_name_to_id: dict[str, dict[str, str]] = dict()
     archived_attr_ids: dict[str, str] = dict()
     types_by_asset: dict[str, set[type]] = dict()
 
     @classmethod
-    def _refresh_cache(cls) -> None:
+    def refresh_cache(cls) -> None:
         from pyatlan.model.core import CustomMetadata, to_snake_case
 
         client = AtlanClient.get_default_client()
         if client is None:
             client = AtlanClient()
         response = client.get_typedefs(type_category=AtlanTypeCategory.CUSTOM_METADATA)
         if response is not None:
@@ -94,46 +94,46 @@
     def get_id_for_name(cls, name: str) -> Optional[str]:
         """
         Translate the provided human-readable custom metadata set name to its Atlan-internal ID string.
         """
         if cm_id := cls.map_name_to_id.get(name):
             return cm_id
         # If not found, refresh the cache and look again (could be stale)
-        cls._refresh_cache()
+        cls.refresh_cache()
         return cls.map_name_to_id.get(name)
 
     @classmethod
     def get_name_for_id(cls, idstr: str) -> Optional[str]:
         """
         Translate the provided Atlan-internal custom metadata ID string to the human-readable custom metadata set name.
         """
         if cm_name := cls.map_id_to_name.get(idstr):
             return cm_name
         # If not found, refresh the cache and look again (could be stale)
-        cls._refresh_cache()
+        cls.refresh_cache()
         return cls.map_id_to_name.get(idstr)
 
     @classmethod
     def get_type_for_id(cls, idstr: str) -> Optional[type]:
         if cm_type := cls.map_id_to_type.get(idstr):
             return cm_type
-        cls._refresh_cache()
+        cls.refresh_cache()
         return cls.map_id_to_type.get(idstr)
 
     @classmethod
     def get_all_custom_attributes(
         cls, include_deleted: bool = False, force_refresh: bool = False
     ) -> dict[str, list[AttributeDef]]:
         """
         Retrieve all the custom metadata attributes. The map will be keyed by custom metadata set
         name, and the value will be a listing of all the attributes within that set (with all the details
         of each of those attributes).
         """
         if len(cls.cache_by_id) == 0 or force_refresh:
-            cls._refresh_cache()
+            cls.refresh_cache()
         m = {}
         for type_id, cm in cls.cache_by_id.items():
             type_name = cls.get_name_for_id(type_id)
             if not type_name:
                 raise NotFoundError(
                     f"The type_name for {type_id} could not be found.", code="fixme"
                 )
@@ -161,30 +161,30 @@
         if set_id := cls.get_id_for_name(set_name):
             if sub_map := cls.map_attr_name_to_id.get(set_id):
                 attr_id = sub_map.get(attr_name)
             if attr_id:
                 # If found, return straight away
                 return attr_id
             # Otherwise, refresh the cache and look again (could be stale)
-            cls._refresh_cache()
+            cls.refresh_cache()
             if sub_map := cls.map_attr_name_to_id.get(set_id):
                 return sub_map.get(attr_name)
         return None
 
     @classmethod
     def get_attr_name_for_id(cls, set_id: str, attr_id: str) -> Optional[str]:
         """
         Translate the provided human-readable custom metadata set and attribute names to the Atlan-internal ID string
         for the attribute.
         """
         if sub_map := cls.map_attr_id_to_name.get(set_id):
             attr_name = sub_map.get(attr_id)
             if attr_name:
                 return attr_name
-            cls._refresh_cache()
+            cls.refresh_cache()
             if sub_map := cls.map_attr_id_to_name.get(set_id):
                 return sub_map.get(attr_id)
         return None
 
     @classmethod
     def _get_attributes_for_search_results(cls, set_id: str) -> Optional[list[str]]:
         if sub_map := cls.map_attr_name_to_id.get(set_id):
@@ -196,15 +196,15 @@
     def get_attributes_for_search_results(cls, set_name: str) -> Optional[list[str]]:
         """
         Retrieve the full set of custom attributes to include on search results.
         """
         if set_id := cls.get_id_for_name(set_name):
             if dot_names := cls._get_attributes_for_search_results(set_id):
                 return dot_names
-            cls._refresh_cache()
+            cls.refresh_cache()
             return cls._get_attributes_for_search_results(set_id)
         return None
 
     @classmethod
     def get_custom_metadata(
         cls,
         name: str,
```

### Comparing `pyatlan-0.0.30/pyatlan/cache/role_cache.py` & `pyatlan-0.0.31/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/client/atlan.py` & `pyatlan-0.0.31/pyatlan/client/atlan.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     CREATE_TYPE_DEFS,
     DELETE_ENTITY_BY_ATTRIBUTE,
     DELETE_ENTITY_BY_GUID,
     DELETE_TYPE_DEF_BY_NAME,
     GET_ALL_TYPE_DEFS,
     GET_ENTITY_BY_GUID,
     GET_ENTITY_BY_UNIQUE_ATTRIBUTE,
+    GET_LINEAGE,
     GET_ROLES,
     INDEX_SEARCH,
     PARTIAL_UPDATE_ENTITY_BY_ATTRIBUTE,
     UPDATE_ENTITY_BY_ATTRIBUTE,
 )
 from pyatlan.error import AtlanError, NotFoundError
 from pyatlan.exceptions import AtlanServiceException, InvalidRequestException
@@ -63,20 +64,22 @@
 )
 from pyatlan.model.enums import (
     AtlanConnectorType,
     AtlanDeleteType,
     AtlanTypeCategory,
     CertificateStatus,
 )
+from pyatlan.model.lineage import LineageRequest, LineageResponse
 from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.role import RoleResponse
 from pyatlan.model.search import DSL, IndexSearchRequest, Term
 from pyatlan.model.typedef import (
     ClassificationDef,
     CustomMetadataDef,
+    EnumDef,
     TypeDef,
     TypeDefResponse,
 )
 from pyatlan.utils import HTTPStatus, get_logger
 
 LOGGER = get_logger()
 T = TypeVar("T", bound=Referenceable)
@@ -468,28 +471,50 @@
                 classification_defs=[],
                 enum_defs=[],
                 struct_defs=[],
                 entity_defs=[],
                 relationship_defs=[],
                 custom_metadata_defs=[typedef],
             )
+        elif isinstance(typedef, EnumDef):
+            # Set up the request payload...
+            payload = TypeDefResponse(
+                classification_defs=[],
+                enum_defs=[typedef],
+                struct_defs=[],
+                entity_defs=[],
+                relationship_defs=[],
+                custom_metadata_defs=[],
+            )
         else:
             raise InvalidRequestException(
                 "Unable to create new type definitions of category: "
                 + typedef.category.value,
                 param="category",
             )
             # Throw an invalid request exception
         raw_json = self._call_api(
             CREATE_TYPE_DEFS, request_obj=payload, exclude_unset=False
         )
+        if isinstance(typedef, ClassificationDef):
+            from pyatlan.cache.classification_cache import ClassificationCache
+            ClassificationCache.refresh_cache()
+        if isinstance(typedef, CustomMetadataDef):
+            from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+            CustomMetadataCache.refresh_cache()
         return TypeDefResponse(**raw_json)
 
     def purge_typedef(self, internal_name: str) -> None:
         self._call_api(DELETE_TYPE_DEF_BY_NAME.format_path_with_params(internal_name))
+        # TODO: if we know which kind of typedef is being purged, we only need
+        #  to refresh that particular cache
+        from pyatlan.cache.classification_cache import ClassificationCache
+        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+        ClassificationCache.refresh_cache()
+        CustomMetadataCache.refresh_cache()
 
     @validate_arguments()
     def add_classifications(
         self,
         asset_type: Type[A],
         qualified_name: str,
         classification_names: list[str],
@@ -709,22 +734,30 @@
         return asset
 
     @validate_arguments()
     def find_connections_by_name(
         self,
         name: str,
         connector_type: AtlanConnectorType,
-        attributes: list[str] = None,
+        attributes: Optional[list[str]] = None,
     ) -> list[Connection]:
+        if attributes is None:
+            attributes = []
         query = (
             Term.with_state("ACTIVE")
             + Term.with_type_name("CONNECTION")
             + Term.with_name(name)
             + Term(field="connectorName", value=connector_type.value)
         )
         dsl = DSL(query=query)
         search_request = IndexSearchRequest(
             dsl=dsl,
             attributes=attributes,
         )
         results = self.search(search_request)
         return [asset for asset in results if isinstance(asset, Connection)]
+
+    def get_lineage(self, lineage_request: LineageRequest) -> LineageResponse:
+        raw_json = self._call_api(
+            GET_LINEAGE, None, lineage_request, exclude_unset=False
+        )
+        return LineageResponse(**raw_json)
```

### Comparing `pyatlan-0.0.30/pyatlan/client/constants.py` & `pyatlan-0.0.31/pyatlan/client/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 ADMIN_API = f"{BASE_URI}admin/"
 ENTITY_PURGE_API = f"{ADMIN_API}purge/"
 ENTITY_BULK_API = f"{ENTITY_API}bulk/"
 BULK_SET_CLASSIFICATIONS = "bulk/setClassifications"
 BULK_HEADERS = "bulk/headers"
 
 BULK_UPDATE = API(ENTITY_BULK_API, HTTPMethod.POST, HTTPStatus.OK)
+# Lineage APIs
+GET_LINEAGE = API(f"{BASE_URI}lineage/getlineage", HTTPMethod.POST, HTTPStatus.OK)
 # Entity APIs
 GET_ENTITY_BY_GUID = API(f"{ENTITY_API}guid", HTTPMethod.GET, HTTPStatus.OK)
 GET_ENTITY_BY_UNIQUE_ATTRIBUTE = API(
     f"{ENTITY_API}uniqueAttribute/type", HTTPMethod.GET, HTTPStatus.OK
 )
 GET_ENTITIES_BY_GUIDS = API(ENTITY_BULK_API, HTTPMethod.GET, HTTPStatus.OK)
 GET_ENTITIES_BY_UNIQUE_ATTRIBUTE = API(
```

### Comparing `pyatlan-0.0.30/pyatlan/error.py` & `pyatlan-0.0.31/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/exceptions.py` & `pyatlan-0.0.31/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.31/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/model/assets.py` & `pyatlan-0.0.31/pyatlan/model/assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/model/core.py` & `pyatlan-0.0.31/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/model/enums.py` & `pyatlan-0.0.31/pyatlan/model/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,7 +252,13 @@
     SAPHANA = ("sap-hana", AtlanConnectionCategory.WAREHOUSE)
     EMPTY = ("empty", None)
 
 
 class SortOrder(str, Enum):
     ASCENDING = "asc"
     DESCENDING = "desc"
+
+
+class LineageDirection(str, Enum):
+    UPSTREAM = "INPUT"
+    DOWNSTREAM = "OUTPUT"
+    BOTH = "BOTH"
```

### Comparing `pyatlan-0.0.30/pyatlan/model/response.py` & `pyatlan-0.0.31/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/model/role.py` & `pyatlan-0.0.31/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/model/search.py` & `pyatlan-0.0.31/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/model/structs.py` & `pyatlan-0.0.31/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan/model/typedef.py` & `pyatlan-0.0.31/pyatlan/model/typedef.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         custom_type: Optional[str] = Field(
             None,
             description="Used for Atlan-specific types like `users`, `groups`, `url`, and `SQL`.\n",
         )
         is_archived: Optional[bool] = Field(
             None,
             description="Whether the attribute has been deleted (true) or is still active (false).\n",
-            example=True
+            example=True,
         )
         archived_at: Optional[int] = Field(
             None, description="When the attribute was deleted.\n"
         )
         archived_by: Optional[str] = Field(
             None, description="User who deleted the attribute.\n"
         )
@@ -144,15 +144,15 @@
         primitive_type: Optional[str] = Field(
             None, description="The type of the option"
         )
 
     is_new: Optional[bool] = Field(
         True,
         description="Whether the attribute is being newly created (true) or not (false).",
-        example=True
+        example=True,
     )
     cardinality: Optional[Cardinality] = Field(
         "SINGLE",
         description="Whether the attribute allows a single or multiple values. In the case of multiple values, "
         "`LIST` indicates they are ordered and duplicates are allowed, while `SET` indicates "
         "they are unique and unordered.\n",
         example="SINGLE",
```

### Comparing `pyatlan-0.0.30/pyatlan/utils.py` & `pyatlan-0.0.31/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.31/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.30
+Version: 0.0.31
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.30/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.31/pyatlan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 pyatlan/generator/generate_from_typdefs.py
 pyatlan/generator/templates/__init__.py
 pyatlan/model/__init__.py
 pyatlan/model/assets.py
 pyatlan/model/core.py
 pyatlan/model/enums.py
 pyatlan/model/internal.py
+pyatlan/model/lineage.py
 pyatlan/model/response.py
 pyatlan/model/role.py
 pyatlan/model/search.py
 pyatlan/model/structs.py
 pyatlan/model/typedef.py
 tests/__init__.py
 tests/integration/__init__.py
@@ -42,11 +43,12 @@
 tests/integration/test_client.py
 tests/integration/test_entity_model.py
 tests/integration/test_index_search.py
 tests/unit/__init__.py
 tests/unit/test_classification_name.py
 tests/unit/test_client.py
 tests/unit/test_glossary_term.py
+tests/unit/test_lineage.py
 tests/unit/test_model.py
 tests/unit/test_search_model.py
 tests/unit/test_typedef_model.py
 tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.30/setup.py` & `pyatlan-0.0.31/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/integration/classification_test.py` & `pyatlan-0.0.31/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.31/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/integration/role_test.py` & `pyatlan-0.0.31/tests/integration/role_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/integration/test_client.py` & `pyatlan-0.0.31/tests/integration/test_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Callable, Generator
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryTerm, Connection, Database
 from pyatlan.model.enums import AtlanConnectorType
+from pyatlan.model.lineage import LineageRequest
 
 iter_count = count(1)
 
 
 @pytest.fixture(scope="module")
 def client() -> AtlanClient:
     return AtlanClient()
@@ -226,7 +227,15 @@
     connections = client.find_connections_by_name(
         name="Test Connection",
         connector_type=AtlanConnectorType.SNOWFLAKE,
         attributes=["connectorName"],
     )
     assert len(connections) == 1
     assert connections[0].connector_name == AtlanConnectorType.SNOWFLAKE.value
+
+
+def test_get_lineage(client: AtlanClient):
+    response = client.get_lineage(
+        LineageRequest(guid="75474eab-3105-4ef9-9f84-709e386a7d3e")
+    )
+    for guid, asset in response.guid_entity_map.items():
+        assert guid == asset.guid
```

### Comparing `pyatlan-0.0.30/tests/integration/test_entity_model.py` & `pyatlan-0.0.31/tests/integration/test_entity_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/integration/test_index_search.py` & `pyatlan-0.0.31/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/unit/test_classification_name.py` & `pyatlan-0.0.31/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/unit/test_client.py` & `pyatlan-0.0.31/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/unit/test_glossary_term.py` & `pyatlan-0.0.31/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/unit/test_model.py` & `pyatlan-0.0.31/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/unit/test_search_model.py` & `pyatlan-0.0.31/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.30/tests/unit/test_typedef_model.py` & `pyatlan-0.0.31/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

