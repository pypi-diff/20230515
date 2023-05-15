# Comparing `tmp/etl-entities-1.3.1.tar.gz` & `tmp/etl-entities-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl-entities-1.3.1.tar", last modified: Mon Feb 27 11:24:39 2023, max compression
+gzip compressed data, was "etl-entities-1.3.2.tar", last modified: Mon May 15 14:59:56 2023, max compression
```

## Comparing `etl-entities-1.3.1.tar` & `etl-entities-1.3.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.346750 etl-entities-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-02-27 11:24:33.000000 etl-entities-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-27 11:24:33.000000 etl-entities-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-27 11:24:39.346750 etl-entities-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-02-27 11:24:33.000000 etl-entities-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.342749 etl-entities-1.3.1/etl_entities/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.342749 etl-entities-1.3.1/etl_entities/hwm/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/column_hwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/date_hwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/datetime_hwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/file_hwm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/file_list_hwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/hwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/hwm_type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/hwm/int_hwm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.342749 etl-entities-1.3.1/etl_entities/instance/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.342749 etl-entities-1.3.1/etl_entities/instance/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/cluster/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.342749 etl-entities-1.3.1/etl_entities/instance/host/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/host/host.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.346750 etl-entities-1.3.1/etl_entities/instance/path/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/path/absolute_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/path/generic_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/path/relative_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.346750 etl-entities-1.3.1/etl_entities/instance/url/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/instance/url/generic_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.346750 etl-entities-1.3.1/etl_entities/process/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/process/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/process/process_stack_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.346750 etl-entities-1.3.1/etl_entities/source/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.346750 etl-entities-1.3.1/etl_entities/source/db/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/source/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/source/db/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/source/db/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.346750 etl-entities-1.3.1/etl_entities/source/file/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/source/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/source/file/remote_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-27 11:24:33.000000 etl-entities-1.3.1/etl_entities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 11:24:39.342749 etl-entities-1.3.1/etl_entities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-27 11:24:39.000000 etl-entities-1.3.1/etl_entities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-02-27 11:24:39.000000 etl-entities-1.3.1/etl_entities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 11:24:39.000000 etl-entities-1.3.1/etl_entities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 11:24:39.000000 etl-entities-1.3.1/etl_entities.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 11:24:39.000000 etl-entities-1.3.1/etl_entities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-27 11:24:39.000000 etl-entities-1.3.1/etl_entities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-27 11:24:33.000000 etl-entities-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-27 11:24:33.000000 etl-entities-1.3.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 11:24:33.000000 etl-entities-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-02-27 11:24:39.346750 etl-entities-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-02-27 11:24:33.000000 etl-entities-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.938330 etl-entities-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-15 14:59:52.000000 etl-entities-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 14:59:52.000000 etl-entities-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-15 14:59:56.938330 etl-entities-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-15 14:59:52.000000 etl-entities-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.934329 etl-entities-1.3.2/etl_entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.934329 etl-entities-1.3.2/etl_entities/hwm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/column_hwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/date_hwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/datetime_hwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/file_hwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/file_list_hwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/hwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/hwm_type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/hwm/int_hwm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.934329 etl-entities-1.3.2/etl_entities/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.934329 etl-entities-1.3.2/etl_entities/instance/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/cluster/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.938330 etl-entities-1.3.2/etl_entities/instance/host/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/host/host.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.938330 etl-entities-1.3.2/etl_entities/instance/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/path/absolute_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/path/generic_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/path/relative_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.938330 etl-entities-1.3.2/etl_entities/instance/url/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/instance/url/generic_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.938330 etl-entities-1.3.2/etl_entities/process/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/process/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/process/process_stack_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.938330 etl-entities-1.3.2/etl_entities/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.938330 etl-entities-1.3.2/etl_entities/source/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/source/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/source/db/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/source/db/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.938330 etl-entities-1.3.2/etl_entities/source/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/source/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/source/file/remote_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-15 14:59:52.000000 etl-entities-1.3.2/etl_entities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:59:56.934329 etl-entities-1.3.2/etl_entities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-15 14:59:56.000000 etl-entities-1.3.2/etl_entities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-15 14:59:56.000000 etl-entities-1.3.2/etl_entities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:59:56.000000 etl-entities-1.3.2/etl_entities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:59:56.000000 etl-entities-1.3.2/etl_entities.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 14:59:56.000000 etl-entities-1.3.2/etl_entities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 14:59:56.000000 etl-entities-1.3.2/etl_entities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 14:59:52.000000 etl-entities-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 14:59:52.000000 etl-entities-1.3.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 14:59:52.000000 etl-entities-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-15 14:59:56.938330 etl-entities-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-15 14:59:52.000000 etl-entities-1.3.2/setup.py
```

### Comparing `etl-entities-1.3.1/LICENSE.txt` & `etl-entities-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/PKG-INFO` & `etl-entities-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: etl-entities
-Version: 1.3.1
+Version: 1.3.2
 Summary: ETL Entities lib for onETL
 Home-page: https://github.com/MobileTeleSystems/etl-entities
 Author: ONEtools Team
 Author-email: onetools@mts.ru
 License: Apache License 2.0
-Project-URL: Documentation, https://etl-entities.readthedocs.io/en/stable/
+Project-URL: Documentation, https://etl-entities.readthedocs.io/
 Project-URL: Source, https://github.com/MobileTeleSystems/etl-entities
 Project-URL: CI/CD, https://github.com/MobileTeleSystems/etl-entities/actions
 Project-URL: Tracker, https://github.com/MobileTeleSystems/etl-entities/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -26,27 +26,25 @@
 
 ETL Entities lib
 ================
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/etl-entities
 .. |PyPI| image:: https://img.shields.io/pypi/v/etl-entities
     :target: https://pypi.org/project/etl-entities/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/etl-entities.svg
     :target: https://github.com/MobileTeleSystems/etl-entities/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/etl-entities.svg
     :target: https://badge.fury.io/py/etl-entities
-.. |ReadTheDocs| image:: https://img.shields.io/readthedocs/etl-entities.svg
-    :target: https://etl-entities.readthedocs.io
 .. |Build Status| image:: https://github.com/MobileTeleSystems/etl-entities/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/etl-entities/actions
 .. |Documentation| image:: https://readthedocs.org/projects/etl-entities/badge/?version=stable
-    :target: https://etl-entities.readthedocs.io/en/latest/?badge=stable
+    :target: https://etl-entities.readthedocs.io/
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/etl-entities/branch/develop/graph/badge.svg?token=RIO8URKNZJ
     :target: https://codecov.io/gh/MobileTeleSystems/etl-entities
 
 What is ETL Entities?
 -----------------------
 
 Collection of classes used for handling High Water Mark (HWM) and gathering Lineage graph.
```

### Comparing `etl-entities-1.3.1/README.rst` & `etl-entities-1.3.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 
 ETL Entities lib
 ================
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/etl-entities
 .. |PyPI| image:: https://img.shields.io/pypi/v/etl-entities
     :target: https://pypi.org/project/etl-entities/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/etl-entities.svg
     :target: https://github.com/MobileTeleSystems/etl-entities/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/etl-entities.svg
     :target: https://badge.fury.io/py/etl-entities
-.. |ReadTheDocs| image:: https://img.shields.io/readthedocs/etl-entities.svg
-    :target: https://etl-entities.readthedocs.io
 .. |Build Status| image:: https://github.com/MobileTeleSystems/etl-entities/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/etl-entities/actions
 .. |Documentation| image:: https://readthedocs.org/projects/etl-entities/badge/?version=stable
-    :target: https://etl-entities.readthedocs.io/en/latest/?badge=stable
+    :target: https://etl-entities.readthedocs.io/
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/etl-entities/branch/develop/graph/badge.svg?token=RIO8URKNZJ
     :target: https://codecov.io/gh/MobileTeleSystems/etl-entities
 
 What is ETL Entities?
 -----------------------
 
 Collection of classes used for handling High Water Mark (HWM) and gathering Lineage graph.
```

### Comparing `etl-entities-1.3.1/etl_entities/__init__.py` & `etl-entities-1.3.2/etl_entities/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/entity.py` & `etl-entities-1.3.2/etl_entities/entity.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/__init__.py` & `etl-entities-1.3.2/etl_entities/hwm/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/column_hwm.py` & `etl-entities-1.3.2/etl_entities/hwm/column_hwm.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/date_hwm.py` & `etl-entities-1.3.2/etl_entities/hwm/date_hwm.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/datetime_hwm.py` & `etl-entities-1.3.2/etl_entities/hwm/datetime_hwm.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/file_hwm.py` & `etl-entities-1.3.2/etl_entities/hwm/file_hwm.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/file_list_hwm.py` & `etl-entities-1.3.2/etl_entities/hwm/file_list_hwm.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/hwm.py` & `etl-entities-1.3.2/etl_entities/hwm/hwm.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/hwm_type_registry.py` & `etl-entities-1.3.2/etl_entities/hwm/hwm_type_registry.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/hwm/int_hwm.py` & `etl-entities-1.3.2/etl_entities/hwm/int_hwm.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/__init__.py` & `etl-entities-1.3.2/etl_entities/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/cluster/__init__.py` & `etl-entities-1.3.2/etl_entities/instance/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/cluster/cluster.py` & `etl-entities-1.3.2/etl_entities/instance/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/host/__init__.py` & `etl-entities-1.3.2/etl_entities/instance/host/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/host/host.py` & `etl-entities-1.3.2/etl_entities/instance/host/host.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/path/__init__.py` & `etl-entities-1.3.2/etl_entities/instance/path/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/path/absolute_path.py` & `etl-entities-1.3.2/etl_entities/instance/path/absolute_path.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/path/generic_path.py` & `etl-entities-1.3.2/etl_entities/instance/path/generic_path.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/path/relative_path.py` & `etl-entities-1.3.2/etl_entities/instance/path/relative_path.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/url/__init__.py` & `etl-entities-1.3.2/etl_entities/instance/url/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/instance/url/generic_url.py` & `etl-entities-1.3.2/etl_entities/instance/url/generic_url.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/process/__init__.py` & `etl-entities-1.3.2/etl_entities/process/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/process/process.py` & `etl-entities-1.3.2/etl_entities/process/process.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/process/process_stack_manager.py` & `etl-entities-1.3.2/etl_entities/process/process_stack_manager.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/source/__init__.py` & `etl-entities-1.3.2/etl_entities/source/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/source/db/__init__.py` & `etl-entities-1.3.2/etl_entities/source/db/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/source/db/column.py` & `etl-entities-1.3.2/etl_entities/source/db/column.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/source/db/table.py` & `etl-entities-1.3.2/etl_entities/source/db/table.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/source/file/__init__.py` & `etl-entities-1.3.2/etl_entities/source/file/__init__.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/source/file/remote_folder.py` & `etl-entities-1.3.2/etl_entities/source/file/remote_folder.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities/version.py` & `etl-entities-1.3.2/etl_entities/version.py`

 * *Files identical despite different names*

### Comparing `etl-entities-1.3.1/etl_entities.egg-info/PKG-INFO` & `etl-entities-1.3.2/etl_entities.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: etl-entities
-Version: 1.3.1
+Version: 1.3.2
 Summary: ETL Entities lib for onETL
 Home-page: https://github.com/MobileTeleSystems/etl-entities
 Author: ONEtools Team
 Author-email: onetools@mts.ru
 License: Apache License 2.0
-Project-URL: Documentation, https://etl-entities.readthedocs.io/en/stable/
+Project-URL: Documentation, https://etl-entities.readthedocs.io/
 Project-URL: Source, https://github.com/MobileTeleSystems/etl-entities
 Project-URL: CI/CD, https://github.com/MobileTeleSystems/etl-entities/actions
 Project-URL: Tracker, https://github.com/MobileTeleSystems/etl-entities/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -26,27 +26,25 @@
 
 ETL Entities lib
 ================
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/etl-entities
 .. |PyPI| image:: https://img.shields.io/pypi/v/etl-entities
     :target: https://pypi.org/project/etl-entities/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/etl-entities.svg
     :target: https://github.com/MobileTeleSystems/etl-entities/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/etl-entities.svg
     :target: https://badge.fury.io/py/etl-entities
-.. |ReadTheDocs| image:: https://img.shields.io/readthedocs/etl-entities.svg
-    :target: https://etl-entities.readthedocs.io
 .. |Build Status| image:: https://github.com/MobileTeleSystems/etl-entities/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/etl-entities/actions
 .. |Documentation| image:: https://readthedocs.org/projects/etl-entities/badge/?version=stable
-    :target: https://etl-entities.readthedocs.io/en/latest/?badge=stable
+    :target: https://etl-entities.readthedocs.io/
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/etl-entities/branch/develop/graph/badge.svg?token=RIO8URKNZJ
     :target: https://codecov.io/gh/MobileTeleSystems/etl-entities
 
 What is ETL Entities?
 -----------------------
 
 Collection of classes used for handling High Water Mark (HWM) and gathering Lineage graph.
```

### Comparing `etl-entities-1.3.1/etl_entities.egg-info/SOURCES.txt` & `etl-entities-1.3.2/etl_entities.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements-test.txt
 requirements.txt
 setup.cfg
 setup.py
 etl_entities/VERSION
 etl_entities/__init__.py
 etl_entities/entity.py
+etl_entities/py.typed
 etl_entities/version.py
 etl_entities.egg-info/PKG-INFO
 etl_entities.egg-info/SOURCES.txt
 etl_entities.egg-info/dependency_links.txt
 etl_entities.egg-info/not-zip-safe
 etl_entities.egg-info/requires.txt
 etl_entities.egg-info/top_level.txt
```

### Comparing `etl-entities-1.3.1/setup.cfg` & `etl-entities-1.3.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 max-string-usages = 15
 max-try-body-length = 15
 max-asserts = 15
 max-access-level = 6
 max-attributes = 20
 max-line-length = 120
 max-doc-length = 120
-inline-quotes = "
+inline-quotes = double
+multiline-quotes = double
+docstring-quotes = double
 show-source = True
 count = True
 statistics = True
 exclude = 
 	.tox,
 	migrations,
 	dist,
@@ -44,16 +46,14 @@
 	hadoop_archive_plugin,
 	virtualenv,
 	venv,
 	venv36,
 	ve,
 	.venv,
 	tox.ini,
-	docker,
-	Jenkinsfile,
 	dags,
 	setup.py,
 	docs,
 rst-directives = 
 	autosummary,data,currentmodule,deprecated,
 	glossary,moduleauthor,plot,testcode,
 	versionadded,versionchanged,
@@ -128,24 +128,15 @@
 	WPS210,
 	WPS228,
 	conftest.py:
 	E800,
 	S105,
 	WPS442,
 	WPS420,
-	WPS432,
-	file_downloader.py:
-	WPS232,
-	*connection.py:
-	WPS437,
-	*processing*:
-	WPS220,
-	WPS231,
-	*writer*:
-	E800,
+	WPS432
 
 [darglint]
 docstring_style = sphinx
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `etl-entities-1.3.1/setup.py` & `etl-entities-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
     project_urls={
-        "Documentation": "https://etl-entities.readthedocs.io/en/stable/",
+        "Documentation": "https://etl-entities.readthedocs.io/",
         "Source": "https://github.com/MobileTeleSystems/etl-entities",
         "CI/CD": "https://github.com/MobileTeleSystems/etl-entities/actions",
         "Tracker": "https://github.com/MobileTeleSystems/etl-entities/issues",
     },
     python_requires=">=3.7",
     install_requires=requirements,
     include_package_data=True,
```

