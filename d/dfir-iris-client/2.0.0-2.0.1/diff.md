# Comparing `tmp/dfir_iris_client-2.0.0.tar.gz` & `tmp/dfir-iris-client-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfir_iris_client-2.0.0.tar", last modified: Sun Mar 26 08:48:54 2023, max compression
+gzip compressed data, was "dfir-iris-client-2.0.1.tar", last modified: Mon May 15 14:22:15 2023, max compression
```

## Comparing `dfir_iris_client-2.0.0.tar` & `dfir-iris-client-2.0.1.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-03-26 08:48:54.170659 dfir_iris_client-2.0.0/
--rw-r--r--   0 blue       (501) staff       (20)     7652 2022-02-02 11:18:01.000000 dfir_iris_client-2.0.0/LICENSE.txt
--rw-r--r--   0 blue       (501) staff       (20)     1488 2023-03-26 08:48:54.170520 dfir_iris_client-2.0.0/PKG-INFO
--rw-r--r--   0 blue       (501) staff       (20)      999 2023-03-26 08:47:38.000000 dfir_iris_client-2.0.0/README.md
-drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-03-26 08:48:54.156501 dfir_iris_client-2.0.0/dfir_iris_client/
--rw-r--r--   0 blue       (501) staff       (20)        1 2023-03-26 08:40:56.000000 dfir_iris_client-2.0.0/dfir_iris_client/__init__.py
--rw-r--r--   0 blue       (501) staff       (20)    29499 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/admin.py
--rw-r--r--   0 blue       (501) staff       (20)    90888 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/case.py
--rw-r--r--   0 blue       (501) staff       (20)     2510 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/customer.py
--rw-r--r--   0 blue       (501) staff       (20)     2281 2023-03-26 08:40:56.000000 dfir_iris_client-2.0.0/dfir_iris_client/global_search.py
-drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-03-26 08:48:54.160053 dfir_iris_client-2.0.0/dfir_iris_client/helper/
--rw-r--r--   0 blue       (501) staff       (20)        0 2023-03-26 08:40:56.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/__init__.py
--rw-r--r--   0 blue       (501) staff       (20)     2199 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/analysis_status.py
--rw-r--r--   0 blue       (501) staff       (20)     2608 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/assets_type.py
--rw-r--r--   0 blue       (501) staff       (20)      993 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/authorization.py
--rw-r--r--   0 blue       (501) staff       (20)     2321 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/case_classifications.py
--rw-r--r--   0 blue       (501) staff       (20)     1110 2023-03-26 08:40:56.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/colors.py
--rw-r--r--   0 blue       (501) staff       (20)     1805 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/compromise_status.py
--rw-r--r--   0 blue       (501) staff       (20)      927 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/doc_tracer.py
--rw-r--r--   0 blue       (501) staff       (20)     1777 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/docker_helper.py
--rw-r--r--   0 blue       (501) staff       (20)     4144 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/errors.py
--rw-r--r--   0 blue       (501) staff       (20)     2209 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/events_categories.py
--rw-r--r--   0 blue       (501) staff       (20)     2100 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/ioc_types.py
--rw-r--r--   0 blue       (501) staff       (20)    13960 2023-03-26 08:40:56.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/iris_object.py
--rw-r--r--   0 blue       (501) staff       (20)     3147 2023-03-26 08:40:56.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/objects_def.py
--rw-r--r--   0 blue       (501) staff       (20)     1555 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/outcome_status.py
--rw-r--r--   0 blue       (501) staff       (20)     1680 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/report_template_types.py
--rw-r--r--   0 blue       (501) staff       (20)     2163 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/task_status.py
--rw-r--r--   0 blue       (501) staff       (20)     2039 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/tlps.py
--rw-r--r--   0 blue       (501) staff       (20)     8564 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/helper/utils.py
--rw-r--r--   0 blue       (501) staff       (20)    11963 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/session.py
-drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-03-26 08:48:54.170213 dfir_iris_client-2.0.0/dfir_iris_client/tests/
--rw-r--r--   0 blue       (501) staff       (20)        0 2023-03-26 08:40:56.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/__init__.py
--rw-r--r--   0 blue       (501) staff       (20)     3795 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/conftest.py
--rw-r--r--   0 blue       (501) staff       (20)    12081 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_admin.py
--rw-r--r--   0 blue       (501) staff       (20)     2340 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_analysis_status.py
--rw-r--r--   0 blue       (501) staff       (20)     2080 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_asset_type.py
--rw-r--r--   0 blue       (501) staff       (20)    19023 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_authorization.py
--rw-r--r--   0 blue       (501) staff       (20)    76050 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_case.py
--rw-r--r--   0 blue       (501) staff       (20)     2790 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_case_classifications.py
--rw-r--r--   0 blue       (501) staff       (20)     2072 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_compromise_status.py
--rw-r--r--   0 blue       (501) staff       (20)     2273 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_customer.py
--rw-r--r--   0 blue       (501) staff       (20)     2293 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_event_categories.py
--rw-r--r--   0 blue       (501) staff       (20)     1977 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_global_search.py
--rw-r--r--   0 blue       (501) staff       (20)     2372 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_ioc_types.py
--rw-r--r--   0 blue       (501) staff       (20)     2600 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_task_status.py
--rw-r--r--   0 blue       (501) staff       (20)     2388 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/test_tlps.py
--rw-r--r--   0 blue       (501) staff       (20)     5768 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/tests/tests_helper.py
--rw-r--r--   0 blue       (501) staff       (20)     3108 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/dfir_iris_client/users.py
-drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-03-26 08:48:54.157225 dfir_iris_client-2.0.0/dfir_iris_client.egg-info/
--rw-r--r--   0 blue       (501) staff       (20)     1488 2023-03-26 08:48:54.000000 dfir_iris_client-2.0.0/dfir_iris_client.egg-info/PKG-INFO
--rw-r--r--   0 blue       (501) staff       (20)     1865 2023-03-26 08:48:54.000000 dfir_iris_client-2.0.0/dfir_iris_client.egg-info/SOURCES.txt
--rw-r--r--   0 blue       (501) staff       (20)        1 2023-03-26 08:48:54.000000 dfir_iris_client-2.0.0/dfir_iris_client.egg-info/dependency_links.txt
--rw-r--r--   0 blue       (501) staff       (20)       30 2023-03-26 08:48:54.000000 dfir_iris_client-2.0.0/dfir_iris_client.egg-info/requires.txt
--rw-r--r--   0 blue       (501) staff       (20)       17 2023-03-26 08:48:54.000000 dfir_iris_client-2.0.0/dfir_iris_client.egg-info/top_level.txt
--rw-r--r--   0 blue       (501) staff       (20)      225 2023-03-26 08:41:32.000000 dfir_iris_client-2.0.0/pyproject.toml
--rw-r--r--   0 blue       (501) staff       (20)       38 2023-03-26 08:48:54.170709 dfir_iris_client-2.0.0/setup.cfg
--rw-r--r--   0 blue       (501) staff       (20)     1746 2023-03-26 08:47:20.000000 dfir_iris_client-2.0.0/setup.py
+drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-05-15 14:22:15.937433 dfir-iris-client-2.0.1/
+-rw-r--r--   0 blue       (501) staff       (20)     7652 2022-02-02 11:18:01.000000 dfir-iris-client-2.0.1/LICENSE.txt
+-rw-r--r--   0 blue       (501) staff       (20)     1463 2023-05-15 14:22:15.937321 dfir-iris-client-2.0.1/PKG-INFO
+-rw-r--r--   0 blue       (501) staff       (20)      999 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/README.md
+drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-05-15 14:22:15.930597 dfir-iris-client-2.0.1/dfir_iris_client/
+-rw-r--r--   0 blue       (501) staff       (20)        1 2023-03-26 08:40:56.000000 dfir-iris-client-2.0.1/dfir_iris_client/__init__.py
+-rw-r--r--   0 blue       (501) staff       (20)    30130 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/dfir_iris_client/admin.py
+-rw-r--r--   0 blue       (501) staff       (20)     8582 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/dfir_iris_client/alert.py
+-rw-r--r--   0 blue       (501) staff       (20)    90888 2023-03-28 06:30:13.000000 dfir-iris-client-2.0.1/dfir_iris_client/case.py
+-rw-r--r--   0 blue       (501) staff       (20)     2510 2023-04-28 09:37:09.000000 dfir-iris-client-2.0.1/dfir_iris_client/customer.py
+-rw-r--r--   0 blue       (501) staff       (20)     2281 2023-03-26 08:40:56.000000 dfir-iris-client-2.0.1/dfir_iris_client/global_search.py
+drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-05-15 14:22:15.934205 dfir-iris-client-2.0.1/dfir_iris_client/helper/
+-rw-r--r--   0 blue       (501) staff       (20)        0 2023-03-26 08:40:56.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/__init__.py
+-rw-r--r--   0 blue       (501) staff       (20)     2146 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/alert_status.py
+-rw-r--r--   0 blue       (501) staff       (20)     2199 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/analysis_status.py
+-rw-r--r--   0 blue       (501) staff       (20)     2608 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/assets_type.py
+-rw-r--r--   0 blue       (501) staff       (20)      993 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/authorization.py
+-rw-r--r--   0 blue       (501) staff       (20)     2321 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/case_classifications.py
+-rw-r--r--   0 blue       (501) staff       (20)     1110 2023-03-26 08:40:56.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/colors.py
+-rw-r--r--   0 blue       (501) staff       (20)     1805 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/compromise_status.py
+-rw-r--r--   0 blue       (501) staff       (20)      927 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/doc_tracer.py
+-rw-r--r--   0 blue       (501) staff       (20)     1777 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/docker_helper.py
+-rw-r--r--   0 blue       (501) staff       (20)     4144 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/errors.py
+-rw-r--r--   0 blue       (501) staff       (20)     2209 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/events_categories.py
+-rw-r--r--   0 blue       (501) staff       (20)     2100 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/ioc_types.py
+-rw-r--r--   0 blue       (501) staff       (20)    13960 2023-03-26 08:40:56.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/iris_object.py
+-rw-r--r--   0 blue       (501) staff       (20)     3147 2023-03-26 08:40:56.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/objects_def.py
+-rw-r--r--   0 blue       (501) staff       (20)     1555 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/outcome_status.py
+-rw-r--r--   0 blue       (501) staff       (20)     1680 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/report_template_types.py
+-rw-r--r--   0 blue       (501) staff       (20)     2163 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/task_status.py
+-rw-r--r--   0 blue       (501) staff       (20)     2039 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/tlps.py
+-rw-r--r--   0 blue       (501) staff       (20)    10118 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/dfir_iris_client/helper/utils.py
+-rw-r--r--   0 blue       (501) staff       (20)    11964 2023-05-15 14:17:03.000000 dfir-iris-client-2.0.1/dfir_iris_client/session.py
+drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-05-15 14:22:15.937140 dfir-iris-client-2.0.1/dfir_iris_client/tests/
+-rw-r--r--   0 blue       (501) staff       (20)        0 2023-03-26 08:40:56.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/__init__.py
+-rw-r--r--   0 blue       (501) staff       (20)     3795 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/conftest.py
+-rw-r--r--   0 blue       (501) staff       (20)    12115 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_admin.py
+-rw-r--r--   0 blue       (501) staff       (20)    18891 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_alert.py
+-rw-r--r--   0 blue       (501) staff       (20)     2355 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_alert_status.py
+-rw-r--r--   0 blue       (501) staff       (20)     2340 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_analysis_status.py
+-rw-r--r--   0 blue       (501) staff       (20)     2080 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_asset_type.py
+-rw-r--r--   0 blue       (501) staff       (20)    19023 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_authorization.py
+-rw-r--r--   0 blue       (501) staff       (20)    76050 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_case.py
+-rw-r--r--   0 blue       (501) staff       (20)     2790 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_case_classifications.py
+-rw-r--r--   0 blue       (501) staff       (20)     2072 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_compromise_status.py
+-rw-r--r--   0 blue       (501) staff       (20)     2273 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_customer.py
+-rw-r--r--   0 blue       (501) staff       (20)     2293 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_event_categories.py
+-rw-r--r--   0 blue       (501) staff       (20)     1977 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_global_search.py
+-rw-r--r--   0 blue       (501) staff       (20)     2372 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_ioc_types.py
+-rw-r--r--   0 blue       (501) staff       (20)     2600 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_task_status.py
+-rw-r--r--   0 blue       (501) staff       (20)     2388 2023-04-28 09:37:09.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/test_tlps.py
+-rw-r--r--   0 blue       (501) staff       (20)     5768 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/tests/tests_helper.py
+-rw-r--r--   0 blue       (501) staff       (20)     3108 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/dfir_iris_client/users.py
+drwxr-xr-x   0 blue       (501) staff       (20)        0 2023-05-15 14:22:15.931259 dfir-iris-client-2.0.1/dfir_iris_client.egg-info/
+-rw-r--r--   0 blue       (501) staff       (20)     1463 2023-05-15 14:22:15.000000 dfir-iris-client-2.0.1/dfir_iris_client.egg-info/PKG-INFO
+-rw-r--r--   0 blue       (501) staff       (20)     2012 2023-05-15 14:22:15.000000 dfir-iris-client-2.0.1/dfir_iris_client.egg-info/SOURCES.txt
+-rw-r--r--   0 blue       (501) staff       (20)        1 2023-05-15 14:22:15.000000 dfir-iris-client-2.0.1/dfir_iris_client.egg-info/dependency_links.txt
+-rw-r--r--   0 blue       (501) staff       (20)       30 2023-05-15 14:22:15.000000 dfir-iris-client-2.0.1/dfir_iris_client.egg-info/requires.txt
+-rw-r--r--   0 blue       (501) staff       (20)       17 2023-05-15 14:22:15.000000 dfir-iris-client-2.0.1/dfir_iris_client.egg-info/top_level.txt
+-rw-r--r--   0 blue       (501) staff       (20)      225 2023-03-26 08:41:32.000000 dfir-iris-client-2.0.1/pyproject.toml
+-rw-r--r--   0 blue       (501) staff       (20)       38 2023-05-15 14:22:15.937468 dfir-iris-client-2.0.1/setup.cfg
+-rw-r--r--   0 blue       (501) staff       (20)     1746 2023-05-15 14:16:31.000000 dfir-iris-client-2.0.1/setup.py
```

### Comparing `dfir_iris_client-2.0.0/LICENSE.txt` & `dfir-iris-client-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/PKG-INFO` & `dfir-iris-client-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
-Name: dfir_iris_client
-Version: 2.0.0
+Name: dfir-iris-client
+Version: 2.0.1
 Summary: Client for DFIR-IRIS API
 Home-page: https://github.com/dfir-iris/dfir-iris-client
 Author: DFIR-IRIS
-Author-email: contact@dfir-iris.org
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: DFIR-IRIS <contact@dfir-iris.org>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python client
 
 `dfir_iris_client` offers a Python interface to communicate with IRIS.
 
 It relies exclusively on the API, which means output of the methods are the same as specified in the API reference.
 
 ## Versions
-The Python client version follows the API versions (until the patch level). Meaning for API v2.0.0, one need to install `dfir_iris_client-2.0.0`. 
+The Python client version follows the API versions (until the patch level). Meaning for API v2.0.1, one need to install `dfir_iris_client-2.0.1`. 
 Please refer to the [documentation](https://dfir-iris.github.io/operations/api/#references) to check which version applies to your IRIS instance. 
 
 ## Install 
 IRIS Client is now part of PyPI. You can simply install it with : 
 ```
 pip3 install dfir-iris-client
 ```
@@ -38,9 +36,7 @@
 
 
 ## Examples
 Some examples are available [here](https://github.com/dfir-iris/iris-client/tree/master/examples).
 
 ## Documentation 
 The documentation is available in the [IRIS documentation](https://docs.dfir-iris.org/python_client/).
-
-
```

### Comparing `dfir_iris_client-2.0.0/README.md` & `dfir-iris-client-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Python client
 
 `dfir_iris_client` offers a Python interface to communicate with IRIS.
 
 It relies exclusively on the API, which means output of the methods are the same as specified in the API reference.
 
 ## Versions
-The Python client version follows the API versions (until the patch level). Meaning for API v2.0.0, one need to install `dfir_iris_client-2.0.0`. 
+The Python client version follows the API versions (until the patch level). Meaning for API v2.0.1, one need to install `dfir_iris_client-2.0.1`. 
 Please refer to the [documentation](https://dfir-iris.github.io/operations/api/#references) to check which version applies to your IRIS instance. 
 
 ## Install 
 IRIS Client is now part of PyPI. You can simply install it with : 
 ```
 pip3 install dfir-iris-client
 ```
```

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/admin.py` & `dfir-iris-client-2.0.1/dfir_iris_client/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,39 +94,42 @@
             if ret.is_error():
                 return ret
             data = get_data_from_resp(ret)
             user = parse_api_data(data, 'user_id')
 
         return self._s.pi_get(f'manage/users/{user}')
 
-    def add_user(self, login: str, name: str, password: str, email: str, **kwargs) -> ApiResponse:
+    def add_user(self, login: str, name: str, password: str, email: str, is_service_account: bool = False,
+                 **kwargs) -> ApiResponse:
         """
         Adds a new user. A new user can be successfully added if
         
         - login is unique
         - email is unique
         - password meets the requirements of IRIS
         
         !!! tip "Requires server administrator rights"
 
         Args:
           login: Username (login name) of the user to add
           name: Full name of the user
           password: Password of the user
           email: Email of the user
+          is_service_account: True if the user is a service account
 
         Returns:
           ApiResponse
 
         """
         body = {
             "user_login": login,
             "user_name": name,
             "user_password": password,
             "user_email": email,
+            "user_is_service_account": is_service_account,
             "cid": 1
         }
 
         if kwargs.get('is_admin') is not None:
             warnings.warn("\'is_admin argument\' is deprecated, use set_group_permissions method instead",
                           DeprecationWarning)
 
@@ -558,29 +561,36 @@
         body = {
             "asset_name": name if name else ioc.get('asset_name'),
             "asset_description": description if description else ioc.get('asset_description'),
             "cid": 1
         }
         return self._s.pi_post(f'manage/asset-type/update/{asset_type_id}', data=body)
 
-    def add_customer(self, customer_name: str):
+    def add_customer(self, customer_name: str, customer_description: str = None,
+                     customer_sla: str = None, custom_attributes: dict = {}) -> ApiResponse:
         """
         Creates a new customer. A new customer can be added if:
         
         - customer_name is unique
 
         Args:
-          customer_name: Name of the customer to add.
+            customer_name: Name of the customer to add.
+            customer_description: Description of the customer
+            customer_sla: SLA of the customer
+            custom_attributes: Custom attributes of the customer
 
         Returns:
           ApiResponse object
 
         """
         body = {
-            "customer_name": customer_name.lower()
+            "customer_name": customer_name.lower(),
+            "customer_description": customer_description,
+            "customer_sla": customer_sla,
+            "custom_attributes": custom_attributes
         }
         resp = self._s.pi_post('manage/customers/add',
                                data=body)
         return resp
 
     def update_customer(self, customer_id: int, customer_name: str):
         """
```

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/case.py` & `dfir-iris-client-2.0.1/dfir_iris_client/case.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/customer.py` & `dfir-iris-client-2.0.1/dfir_iris_client/customer.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/global_search.py` & `dfir-iris-client-2.0.1/dfir_iris_client/global_search.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/analysis_status.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/analysis_status.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/assets_type.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/assets_type.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/authorization.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/authorization.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/case_classifications.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/case_classifications.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/colors.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/colors.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/compromise_status.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/compromise_status.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/doc_tracer.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/doc_tracer.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/docker_helper.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/docker_helper.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/errors.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/errors.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/events_categories.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/events_categories.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/ioc_types.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/ioc_types.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/iris_object.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/iris_object.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/objects_def.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/objects_def.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/outcome_status.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/outcome_status.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/report_template_types.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/report_template_types.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/task_status.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/task_status.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/tlps.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/tlps.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/helper/utils.py` & `dfir-iris-client-2.0.1/dfir_iris_client/helper/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, write to the Free Software Foundation,
 #  Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-from typing import Union
+from typing import Union, List
 
 import logging as log
 import json
 
 from types import SimpleNamespace
 
 from dfir_iris_client.helper.errors import ApiRequestFailure, InvalidApiResponse, OperationSuccess, IrisStatus, \
@@ -138,14 +138,43 @@
     def get_data(self):
         """ """
         if not hasattr(self, "_response"):
             return None
 
         return self._response.get('data')
 
+    def get_data_field(self, field: Union[List[str], str], index: int = None):
+        """
+        Return the value of a field in the data section of the response
+
+        Args:
+            field: Field to return
+            index: Index of the data section to return (Default value = None). Allows to iterate over a list of data
+
+        Returns:
+            Value of the field
+        """
+        if not hasattr(self, "_response"):
+            return None
+
+        if index is not None:
+            if isinstance(field, str):
+                return self._response.get('data')[index].get(field)
+
+            if isinstance(field, list):
+                return reduce(lambda d, key: d.get(key) if d else None, field, self._response.get('data')[index])
+
+        if isinstance(field, str):
+            return self._response.get('data').get(field)
+
+        if isinstance(field, list):
+            return reduce(lambda d, key: d.get(key) if d else None, field, self._response.get('data'))
+
+        return None
+
     def get_msg(self):
         """ """
         if not hasattr(self, "_response"):
             return None
 
         return self._response.get('message')
 
@@ -237,14 +266,30 @@
             raise IrisClientException(InvalidApiResponse(message=f'Object {path} not found in API response {data}'))
         else:
             return None
 
     return fdata
 
 
+def get_data(api_response: ApiResponse, path: Union[list, str], strict=True) -> any:
+    """Parses the data field of an API response. Path describes a path to fetch a specific value in data.
+    If strict is set, an exception is raised, otherwise None is returned.
+
+    Args:
+      api_response: ApiResponse:
+      path: Value to get from within data
+      strict: Set to true to fails if path is not found in data (default)
+
+    Returns:
+      ApiResponse
+
+    """
+    return parse_api_data(get_data_from_resp(api_response), path, strict)
+
+
 def ClientApiError(error=None, msg=None):
     """
 
     Args:
       error:  (Default value = None)
       msg:  (Default value = None)
```

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/session.py` & `dfir-iris-client-2.0.1/dfir_iris_client/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 log = logger.getLogger(__name__)
 
 """API_VERSION
 The API version is not directly correlated with Iris version. 
 Server has an endpoint /api/versions which should returns the API compatible versions 
 it can handles. 
 """
-API_VERSION = "2.0.0"
+API_VERSION = "2.0.1"
+
 
 """client_session
 Defines a global session, accessible by all classes. client_session is of type ClientSession.
 """
 client_session = None
```

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/conftest.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_admin.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         assert ret.get_data().get('name') == ['Case classification name already exists']
 
         self.adm.delete_case_classification(fid)
         self.adm.delete_case_classification(fod)
 
     def test_add_customer_valid(self):
         """ """
-        ret = self.adm.add_customer('dummy customer')
+        ret = self.adm.add_customer('dummy customer', 'dummy description', 'dummy sla')
 
         if parse_api_data(ret.get_data(), 'customer_name') == ['Customer already exists']:
             ret = self.adm.delete_customer('dummy customer')
             assert assert_api_resp(ret, soft_fail=False)
 
             ret = self.adm.add_customer('dummy customer')
```

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_analysis_status.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_analysis_status.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_asset_type.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_asset_type.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_authorization.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_case.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_case_classifications.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_case_classifications.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_compromise_status.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_compromise_status.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_customer.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_customer.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_event_categories.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_event_categories.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_global_search.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_global_search.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_ioc_types.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_ioc_types.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_task_status.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_task_status.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/test_tlps.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/test_tlps.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/tests/tests_helper.py` & `dfir-iris-client-2.0.1/dfir_iris_client/tests/tests_helper.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client/users.py` & `dfir-iris-client-2.0.1/dfir_iris_client/users.py`

 * *Files identical despite different names*

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client.egg-info/PKG-INFO` & `dfir-iris-client-2.0.1/dfir_iris_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: dfir-iris-client
-Version: 2.0.0
+Version: 2.0.1
 Summary: Client for DFIR-IRIS API
 Home-page: https://github.com/dfir-iris/dfir-iris-client
 Author: DFIR-IRIS
-Author-email: contact@dfir-iris.org
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: DFIR-IRIS <contact@dfir-iris.org>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python client
 
 `dfir_iris_client` offers a Python interface to communicate with IRIS.
 
 It relies exclusively on the API, which means output of the methods are the same as specified in the API reference.
 
 ## Versions
-The Python client version follows the API versions (until the patch level). Meaning for API v2.0.0, one need to install `dfir_iris_client-2.0.0`. 
+The Python client version follows the API versions (until the patch level). Meaning for API v2.0.1, one need to install `dfir_iris_client-2.0.1`. 
 Please refer to the [documentation](https://dfir-iris.github.io/operations/api/#references) to check which version applies to your IRIS instance. 
 
 ## Install 
 IRIS Client is now part of PyPI. You can simply install it with : 
 ```
 pip3 install dfir-iris-client
 ```
@@ -38,9 +36,7 @@
 
 
 ## Examples
 Some examples are available [here](https://github.com/dfir-iris/iris-client/tree/master/examples).
 
 ## Documentation 
 The documentation is available in the [IRIS documentation](https://docs.dfir-iris.org/python_client/).
-
-
```

### Comparing `dfir_iris_client-2.0.0/dfir_iris_client.egg-info/SOURCES.txt` & `dfir-iris-client-2.0.1/dfir_iris_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 dfir_iris_client/__init__.py
 dfir_iris_client/admin.py
+dfir_iris_client/alert.py
 dfir_iris_client/case.py
 dfir_iris_client/customer.py
 dfir_iris_client/global_search.py
 dfir_iris_client/session.py
 dfir_iris_client/users.py
 dfir_iris_client.egg-info/PKG-INFO
 dfir_iris_client.egg-info/SOURCES.txt
 dfir_iris_client.egg-info/dependency_links.txt
 dfir_iris_client.egg-info/requires.txt
 dfir_iris_client.egg-info/top_level.txt
 dfir_iris_client/helper/__init__.py
+dfir_iris_client/helper/alert_status.py
 dfir_iris_client/helper/analysis_status.py
 dfir_iris_client/helper/assets_type.py
 dfir_iris_client/helper/authorization.py
 dfir_iris_client/helper/case_classifications.py
 dfir_iris_client/helper/colors.py
 dfir_iris_client/helper/compromise_status.py
 dfir_iris_client/helper/doc_tracer.py
@@ -32,14 +34,16 @@
 dfir_iris_client/helper/report_template_types.py
 dfir_iris_client/helper/task_status.py
 dfir_iris_client/helper/tlps.py
 dfir_iris_client/helper/utils.py
 dfir_iris_client/tests/__init__.py
 dfir_iris_client/tests/conftest.py
 dfir_iris_client/tests/test_admin.py
+dfir_iris_client/tests/test_alert.py
+dfir_iris_client/tests/test_alert_status.py
 dfir_iris_client/tests/test_analysis_status.py
 dfir_iris_client/tests/test_asset_type.py
 dfir_iris_client/tests/test_authorization.py
 dfir_iris_client/tests/test_case.py
 dfir_iris_client/tests/test_case_classifications.py
 dfir_iris_client/tests/test_compromise_status.py
 dfir_iris_client/tests/test_customer.py
```

### Comparing `dfir_iris_client-2.0.0/setup.py` & `dfir-iris-client-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 CURR_DIR = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (CURR_DIR / "README.md").read_text()
 
 setuptools.setup(
      name='dfir_iris_client',
-     version='2.0.0',
+     version='2.0.1',
      packages=['dfir_iris_client', 'dfir_iris_client.helper', 'dfir_iris_client.tests'],
      author="DFIR-IRIS",
      author_email="contact@dfir-iris.org",
      description="Client for DFIR-IRIS API",
      long_description=README,
      long_description_content_type="text/markdown",
      url="https://github.com/dfir-iris/dfir-iris-client",
```

