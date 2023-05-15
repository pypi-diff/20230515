# Comparing `tmp/python-schema-registry-client-2.4.2.tar.gz` & `tmp/python-schema-registry-client-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-schema-registry-client-2.4.2.tar", last modified: Tue Apr 18 15:04:03 2023, max compression
+gzip compressed data, was "python-schema-registry-client-2.4.3.tar", last modified: Wed Apr 19 13:45:02 2023, max compression
```

## Comparing `python-schema-registry-client-2.4.2.tar` & `python-schema-registry-client-2.4.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 15:04:03.000000 python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/schema_registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/schema_registry/client/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    55077 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/schema_registry/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/serializers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/serializers/faust.py
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/schema_registry/serializers/message_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.897464 python-schema-registry-client-2.4.2/tests/client/async_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4850 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_http_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1258 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/tests/client/sync_client/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_http_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3497 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/client/test_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:04:03.901463 python-schema-registry-client-2.4.2/tests/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8284 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/test_async_message_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/test_faust_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/test_faust_serializer_clean_payload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7624 2023-04-18 15:03:53.000000 python-schema-registry-client-2.4.2/tests/serializer/test_message_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/schema_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/schema_registry/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55077 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/schema_registry/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/serializers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/serializers/faust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/serializers/message_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-19 13:45:02.480533 python-schema-registry-client-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/client/async_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4850 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_http_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1258 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/client/sync_client/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_http_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3497 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8284 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/test_async_message_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/test_faust_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/test_faust_serializer_clean_payload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7624 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/test_message_serializer.py
```

### Comparing `python-schema-registry-client-2.4.2/LICENSE` & `python-schema-registry-client-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/PKG-INFO` & `python-schema-registry-client-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-schema-registry-client
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python Rest Client to interact against Schema Registry Confluent Server to manage Avro Schemas
 Home-page: https://github.com/marcosschroh/python-schema-registry-client
 Author: Marcos Schroh
 Author-email: schrohm@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/python-schema-registry-client/#files
 Keywords: Schema Registry,Python,Avro,Apache,Apache Avro,JSON,JSON Schema
```

### Comparing `python-schema-registry-client-2.4.2/README.md` & `python-schema-registry-client-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/PKG-INFO` & `python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-schema-registry-client
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python Rest Client to interact against Schema Registry Confluent Server to manage Avro Schemas
 Home-page: https://github.com/marcosschroh/python-schema-registry-client
 Author: Marcos Schroh
 Author-email: schrohm@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/python-schema-registry-client/#files
 Keywords: Schema Registry,Python,Avro,Apache,Apache Avro,JSON,JSON Schema
```

### Comparing `python-schema-registry-client-2.4.2/python_schema_registry_client.egg-info/SOURCES.txt` & `python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 python_schema_registry_client.egg-info/PKG-INFO
 python_schema_registry_client.egg-info/SOURCES.txt
 python_schema_registry_client.egg-info/dependency_links.txt
 python_schema_registry_client.egg-info/requires.txt
 python_schema_registry_client.egg-info/top_level.txt
 schema_registry/__init__.py
+schema_registry/py.typed
 schema_registry/client/__init__.py
 schema_registry/client/auth_utils.py
 schema_registry/client/client.py
 schema_registry/client/errors.py
 schema_registry/client/paths.py
 schema_registry/client/schema.py
 schema_registry/client/status.py
```

### Comparing `python-schema-registry-client-2.4.2/schema_registry/client/client.py` & `python-schema-registry-client-2.4.3/schema_registry/client/client.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/schema_registry/client/paths.py` & `python-schema-registry-client-2.4.3/schema_registry/client/paths.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/schema_registry/client/schema.py` & `python-schema-registry-client-2.4.3/schema_registry/client/schema.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/schema_registry/client/status.py` & `python-schema-registry-client-2.4.3/schema_registry/client/status.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/schema_registry/client/urls.py` & `python-schema-registry-client-2.4.3/schema_registry/client/urls.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/schema_registry/client/utils.py` & `python-schema-registry-client-2.4.3/schema_registry/client/utils.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/schema_registry/serializers/__init__.py` & `python-schema-registry-client-2.4.3/schema_registry/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/schema_registry/serializers/faust.py` & `python-schema-registry-client-2.4.3/schema_registry/serializers/faust.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/schema_registry/serializers/message_serializer.py` & `python-schema-registry-client-2.4.3/schema_registry/serializers/message_serializer.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/setup.py` & `python-schema-registry-client-2.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """ setup.py for python-schema-registry-client."""
 
 from setuptools import find_packages, setup
 
-__version__ = "2.4.2"
+__version__ = "2.4.3"
 
 with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 
 requires = [
     "fastavro>=1.4.4",
@@ -24,14 +24,15 @@
     name="python-schema-registry-client",
     version=__version__,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Marcos Schroh",
     author_email="schrohm@gmail.com",
+    package_data={"schema_registry":["py.typed"]},
     install_requires=requires,
     extras_require={
         "faust": [
             "faust-streaming",
         ],
         "docs": [
             "mkdocs",
```

### Comparing `python-schema-registry-client-2.4.2/tests/client/async_client/test_http_client.py` & `python-schema-registry-client-2.4.3/tests/client/async_client/test_http_client.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema.py` & `python-schema-registry-client-2.4.3/tests/client/async_client/test_schema.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_compatibility.py` & `python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_compatibility.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_delete.py` & `python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_delete.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_getters.py` & `python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_getters.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_registration.py` & `python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_registration.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/async_client/test_schema_version.py` & `python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_version.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/sync_client/test_http_client.py` & `python-schema-registry-client-2.4.3/tests/client/sync_client/test_http_client.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema.py` & `python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_compatibility.py` & `python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_compatibility.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_delete.py` & `python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_delete.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_getters.py` & `python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_getters.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_registration.py` & `python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_registration.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/sync_client/test_schema_version.py` & `python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_version.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/client/test_urls.py` & `python-schema-registry-client-2.4.3/tests/client/test_urls.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/serializer/test_async_message_serializer.py` & `python-schema-registry-client-2.4.3/tests/serializer/test_async_message_serializer.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/serializer/test_faust_serializer.py` & `python-schema-registry-client-2.4.3/tests/serializer/test_faust_serializer.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/serializer/test_faust_serializer_clean_payload.py` & `python-schema-registry-client-2.4.3/tests/serializer/test_faust_serializer_clean_payload.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.2/tests/serializer/test_message_serializer.py` & `python-schema-registry-client-2.4.3/tests/serializer/test_message_serializer.py`

 * *Files identical despite different names*

