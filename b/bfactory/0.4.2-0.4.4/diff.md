# Comparing `tmp/bfactory-0.4.2.tar.gz` & `tmp/bfactory-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfactory-0.4.2.tar", last modified: Sun May 14 03:15:27 2023, max compression
+gzip compressed data, was "bfactory-0.4.4.tar", last modified: Mon May 15 01:04:41 2023, max compression
```

## Comparing `bfactory-0.4.2.tar` & `bfactory-0.4.4.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/
--rw-r--r--   0 blackbox  (1000) users      (985)     1063 2022-10-03 23:46:43.000000 bfactory-0.4.2/LICENSE
--rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-05-14 03:15:27.875584 bfactory-0.4.2/PKG-INFO
--rw-r--r--   0 blackbox  (1000) users      (985)     1929 2023-05-14 03:12:02.000000 bfactory-0.4.2/README.md
--rw-r--r--   0 blackbox  (1000) users      (985)       87 2022-10-03 23:46:43.000000 bfactory-0.4.2/pyproject.toml
--rw-r--r--   0 blackbox  (1000) users      (985)      856 2023-05-14 03:15:27.875584 bfactory-0.4.2/setup.cfg
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-04 00:29:45.000000 bfactory-0.4.2/src/bfactory/__init__.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory/cli/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/cli/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)      744 2023-05-13 21:38:11.000000 bfactory-0.4.2/src/bfactory/cli/django_cli.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory/config/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/config/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1253 2023-05-14 03:12:52.000000 bfactory-0.4.2/src/bfactory/config/settings.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory/core/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/core/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     3777 2023-05-13 21:38:24.000000 bfactory-0.4.2/src/bfactory/core/engine.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2127 2023-05-13 20:14:24.000000 bfactory-0.4.2/src/bfactory/core/tasks.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/core/templates/
--rw-r--r--   0 blackbox  (1000) users      (985)       85 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/core/templates/READ.ME
--rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-10-04 00:02:46.000000 bfactory-0.4.2/src/bfactory/core/templates/admin.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/core/templates/helpers/
--rw-r--r--   0 blackbox  (1000) users      (985)     1463 2023-05-14 03:07:12.000000 bfactory-0.4.2/src/bfactory/core/templates/helpers/field.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1262 2023-05-14 01:53:53.000000 bfactory-0.4.2/src/bfactory/core/templates/helpers/field_serializer.py
--rw-r--r--   0 blackbox  (1000) users      (985)      416 2023-05-14 01:52:12.000000 bfactory-0.4.2/src/bfactory/core/templates/helpers/field_type_linting.py
--rw-r--r--   0 blackbox  (1000) users      (985)      624 2022-11-06 04:00:22.000000 bfactory-0.4.2/src/bfactory/core/templates/models.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2759 2022-10-04 00:02:40.000000 bfactory-0.4.2/src/bfactory/core/templates/myconf.py
--rw-r--r--   0 blackbox  (1000) users      (985)      599 2023-04-29 00:34:58.000000 bfactory-0.4.2/src/bfactory/core/templates/selectors.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1621 2022-11-29 20:30:05.000000 bfactory-0.4.2/src/bfactory/core/templates/services.py
--rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-11-05 23:27:19.000000 bfactory-0.4.2/src/bfactory/core/templates/urls.py
--rw-r--r--   0 blackbox  (1000) users      (985)     4388 2022-11-10 03:54:52.000000 bfactory-0.4.2/src/bfactory/core/templates/views.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/inputs/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/inputs/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1986 2023-05-13 21:39:17.000000 bfactory-0.4.2/src/bfactory/inputs/arguments.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2534 2022-11-10 03:35:04.000000 bfactory-0.4.2/src/bfactory/inputs/manifest.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2698 2022-10-30 07:02:48.000000 bfactory-0.4.2/src/bfactory/inputs/manifest.schema.json
--rw-r--r--   0 blackbox  (1000) users      (985)      887 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/inputs/parse_manifest.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1363 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/inputs/validators.py
--rwxr-xr-x   0 blackbox  (1000) users      (985)     1421 2023-05-13 21:38:47.000000 bfactory-0.4.2/src/bfactory/main.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/tests/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/tests/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)      698 2023-05-13 21:38:08.000000 bfactory-0.4.2/src/bfactory/tests/engine_tests.py
--rw-r--r--   0 blackbox  (1000) users      (985)      992 2023-05-14 01:43:35.000000 bfactory-0.4.2/src/bfactory/tests/manifest_test.json
--rw-r--r--   0 blackbox  (1000) users      (985)      673 2023-05-13 20:14:43.000000 bfactory-0.4.2/src/bfactory/tests/manifest_test.py
--rw-r--r--   0 blackbox  (1000) users      (985)      932 2022-10-04 00:31:46.000000 bfactory-0.4.2/src/bfactory/tests/run_tests.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/utils/
--rw-r--r--   0 blackbox  (1000) users      (985)      900 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/utils/crypto.py
--rw-r--r--   0 blackbox  (1000) users      (985)      450 2022-10-04 00:26:40.000000 bfactory-0.4.2/src/bfactory/utils/render.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2830 2023-05-13 21:38:35.000000 bfactory-0.4.2/src/bfactory/utils/state.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory.egg-info/
--rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/PKG-INFO
--rw-r--r--   0 blackbox  (1000) users      (985)     1461 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/SOURCES.txt
--rw-r--r--   0 blackbox  (1000) users      (985)        1 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/dependency_links.txt
--rw-r--r--   0 blackbox  (1000) users      (985)       48 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/entry_points.txt
--rw-r--r--   0 blackbox  (1000) users      (985)       91 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/requires.txt
--rw-r--r--   0 blackbox  (1000) users      (985)        9 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/top_level.txt
--rwxr-xr-x   0 blackbox  (1000) users      (985)      197 2022-11-29 20:30:05.000000 bfactory-0.4.2/src/bfactory.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/
+-rw-r--r--   0 blackbox  (1000) users      (985)     1063 2022-10-03 23:46:43.000000 bfactory-0.4.4/LICENSE
+-rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-05-15 01:04:41.728956 bfactory-0.4.4/PKG-INFO
+-rw-r--r--   0 blackbox  (1000) users      (985)     1929 2023-05-14 03:12:02.000000 bfactory-0.4.4/README.md
+-rw-r--r--   0 blackbox  (1000) users      (985)       87 2022-10-03 23:46:43.000000 bfactory-0.4.4/pyproject.toml
+-rw-r--r--   0 blackbox  (1000) users      (985)      856 2023-05-15 01:04:41.728956 bfactory-0.4.4/setup.cfg
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.725623 bfactory-0.4.4/src/
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.725623 bfactory-0.4.4/src/bfactory/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-04 00:29:45.000000 bfactory-0.4.4/src/bfactory/__init__.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/src/bfactory/cli/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.4/src/bfactory/cli/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      744 2023-05-13 21:38:11.000000 bfactory-0.4.4/src/bfactory/cli/django_cli.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/src/bfactory/config/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.4/src/bfactory/config/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1253 2023-05-15 00:55:46.000000 bfactory-0.4.4/src/bfactory/config/settings.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/src/bfactory/core/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.4/src/bfactory/core/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     3777 2023-05-13 21:38:24.000000 bfactory-0.4.4/src/bfactory/core/engine.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2127 2023-05-13 20:14:24.000000 bfactory-0.4.4/src/bfactory/core/tasks.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/src/bfactory/core/templates/
+-rw-r--r--   0 blackbox  (1000) users      (985)       85 2022-10-03 23:46:43.000000 bfactory-0.4.4/src/bfactory/core/templates/READ.ME
+-rw-r--r--   0 blackbox  (1000) users      (985)      570 2023-05-14 23:10:00.000000 bfactory-0.4.4/src/bfactory/core/templates/admin.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/src/bfactory/core/templates/helpers/
+-rw-r--r--   0 blackbox  (1000) users      (985)     1673 2023-05-14 23:13:44.000000 bfactory-0.4.4/src/bfactory/core/templates/helpers/field.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1334 2023-05-14 22:42:39.000000 bfactory-0.4.4/src/bfactory/core/templates/helpers/field_serializer.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      463 2023-05-14 22:42:14.000000 bfactory-0.4.4/src/bfactory/core/templates/helpers/field_type_linting.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      630 2023-05-14 23:07:31.000000 bfactory-0.4.4/src/bfactory/core/templates/models.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2759 2022-10-04 00:02:40.000000 bfactory-0.4.4/src/bfactory/core/templates/myconf.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      599 2023-04-29 00:34:58.000000 bfactory-0.4.4/src/bfactory/core/templates/selectors.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1627 2023-05-14 23:07:44.000000 bfactory-0.4.4/src/bfactory/core/templates/services.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-11-05 23:27:19.000000 bfactory-0.4.4/src/bfactory/core/templates/urls.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     4759 2023-05-15 00:42:17.000000 bfactory-0.4.4/src/bfactory/core/templates/views.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/src/bfactory/inputs/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.4/src/bfactory/inputs/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1934 2023-05-14 23:12:12.000000 bfactory-0.4.4/src/bfactory/inputs/arguments.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2534 2022-11-10 03:35:04.000000 bfactory-0.4.4/src/bfactory/inputs/manifest.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     4073 2023-05-14 22:51:52.000000 bfactory-0.4.4/src/bfactory/inputs/manifest.schema.json
+-rw-r--r--   0 blackbox  (1000) users      (985)      887 2022-10-03 23:46:43.000000 bfactory-0.4.4/src/bfactory/inputs/parse_manifest.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2171 2023-05-15 00:51:35.000000 bfactory-0.4.4/src/bfactory/inputs/validators.py
+-rwxr-xr-x   0 blackbox  (1000) users      (985)     1416 2023-05-14 22:54:34.000000 bfactory-0.4.4/src/bfactory/main.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/src/bfactory/tests/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.4/src/bfactory/tests/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      698 2023-05-13 21:38:08.000000 bfactory-0.4.4/src/bfactory/tests/engine_tests.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      688 2023-05-14 23:12:27.000000 bfactory-0.4.4/src/bfactory/tests/jsonschema_test.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2026 2023-05-15 00:58:07.000000 bfactory-0.4.4/src/bfactory/tests/manifest_test.json
+-rw-r--r--   0 blackbox  (1000) users      (985)      771 2023-05-15 00:52:57.000000 bfactory-0.4.4/src/bfactory/tests/manifest_test.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1017 2023-05-15 00:51:42.000000 bfactory-0.4.4/src/bfactory/tests/run_tests.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.728956 bfactory-0.4.4/src/bfactory/utils/
+-rw-r--r--   0 blackbox  (1000) users      (985)      900 2022-10-03 23:46:43.000000 bfactory-0.4.4/src/bfactory/utils/crypto.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      450 2022-10-04 00:26:40.000000 bfactory-0.4.4/src/bfactory/utils/render.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2830 2023-05-13 21:38:35.000000 bfactory-0.4.4/src/bfactory/utils/state.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-15 01:04:41.725623 bfactory-0.4.4/src/bfactory.egg-info/
+-rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-05-15 01:04:41.000000 bfactory-0.4.4/src/bfactory.egg-info/PKG-INFO
+-rw-r--r--   0 blackbox  (1000) users      (985)     1499 2023-05-15 01:04:41.000000 bfactory-0.4.4/src/bfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)        1 2023-05-15 01:04:41.000000 bfactory-0.4.4/src/bfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)       48 2023-05-15 01:04:41.000000 bfactory-0.4.4/src/bfactory.egg-info/entry_points.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)       91 2023-05-15 01:04:41.000000 bfactory-0.4.4/src/bfactory.egg-info/requires.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)        9 2023-05-15 01:04:41.000000 bfactory-0.4.4/src/bfactory.egg-info/top_level.txt
+-rwxr-xr-x   0 blackbox  (1000) users      (985)      197 2022-11-29 20:30:05.000000 bfactory-0.4.4/src/bfactory.py
```

### Comparing `bfactory-0.4.2/LICENSE` & `bfactory-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/PKG-INFO` & `bfactory-0.4.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfactory
-Version: 0.4.2
+Version: 0.4.4
 Summary: Build an API from a manifest file
 Home-page: https://github.com/forkear/bfactory
 Author: Forkear
 Author-email: forkear@no-spam.org
 Project-URL: Documentation, https://github.com/forkear/bfactory/blob/main/README.md
 Project-URL: Source, https://github.com/forkear/bfactory
 Project-URL: Tracker, https://github.com/forkear/bfactory/issues
```

### Comparing `bfactory-0.4.2/README.md` & `bfactory-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/setup.cfg` & `bfactory-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/cli/django_cli.py` & `bfactory-0.4.4/src/bfactory/cli/django_cli.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/config/settings.py` & `bfactory-0.4.4/src/bfactory/config/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.4.2'
+__version__ = '0.4.4'
 
 TITLE_BANNER='''\
 
 ██████╗ ███████╗ █████╗  ██████╗████████╗ ██████╗ ██████╗ ██╗   ██╗
 ██╔══██╗██╔════╝██╔══██╗██╔════╝╚══██╔══╝██╔═══██╗██╔══██╗╚██╗ ██╔╝
 ██████╔╝█████╗  ███████║██║        ██║   ██║   ██║██████╔╝ ╚████╔╝ 
 ██╔══██╗██╔══╝  ██╔══██║██║        ██║   ██║   ██║██╔══██╗  ╚██╔╝
```

### Comparing `bfactory-0.4.2/src/bfactory/core/engine.py` & `bfactory-0.4.4/src/bfactory/core/engine.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/core/tasks.py` & `bfactory-0.4.4/src/bfactory/core/tasks.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/admin.py` & `bfactory-0.4.4/src/bfactory/core/templates/admin.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/helpers/field.py` & `bfactory-0.4.4/src/bfactory/core/templates/helpers/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,9 +19,12 @@
 {%- if field.type == 'pint' -%}
     models.PositiveIntegerField({% if not field.req %}null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'fk' -%}
     models.ForeignKey("{{field.fk}}", related_name="{{model.name|lower}}_{{field.name|lower}}_{{field.fk|lower}}", on_delete=models.CASCADE{% if not field.req %},null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'datetime' -%}
-    models.DateTimeField({% if field.default == 'now' %}auto_now=True{% endif %}{% if not field.req %}, null=True, blank=True {% endif %})
+    models.DateTimeField({% if field.auto_now %}auto_now=True{% else %}auto_now=False{% endif %}{% if not field.req %}, null=True, blank=True {% endif %})
 {% endif %}
+{%- if field.type == 'date' -%}
+    models.DateField({% if field.auto_now %}auto_now=True{% else %}auto_now=False{% endif %}{% if not field.req %}, null=True, blank=True {% endif %})
+{% endif %}
```

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/helpers/field_serializer.py` & `bfactory-0.4.4/src/bfactory/core/templates/helpers/field_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,13 +15,16 @@
 {% endif %}
 {%- if field.type == 'fk' -%}
     serializers.PrimaryKeyRelatedField(many=False, queryset={{field.fk}}.objects.all(), required={{field.req}} {% if not field.req %}, allow_null=True {% endif %})
 {% endif %}
 {%- if field.type == 'datetime' -%}
     serializers.DateTimeField()
 {% endif %}
+{%- if field.type == 'date' -%}
+    serializers.DateField()
+{% endif %}
 {%- if field.type == 'decimal' -%}
     serializers.DecimalField(max_digits=10, decimal_places=2)
 {% endif %}
 {%- if field.type == 'user' or field.type == 'owner' -%}
     serializers.PrimaryKeyRelatedField(many=False, queryset=User.objects.all(), required={{field.req}} {% if not field.req %}, allow_null=True {% endif %})
 {% endif %}
```

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/models.py` & `bfactory-0.4.4/src/bfactory/core/templates/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 from django.db import models
 from django.contrib.auth.models import User
-from datetime import datetime
+from datetime import datetime, date
 
 {% for model in models %}
 class {{model.name}}(models.Model):
 
 {% for field in model.fields -%}
 {{ '    ' }}{{field.name}} = {% include "helpers/field.py" %}
 {%- endfor %}
```

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/myconf.py` & `bfactory-0.4.4/src/bfactory/core/templates/myconf.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/selectors.py` & `bfactory-0.4.4/src/bfactory/core/templates/selectors.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/services.py` & `bfactory-0.4.4/src/bfactory/core/templates/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 
 from django.db import models
 from django.contrib.auth.models import User
 from django.db import transaction
-from datetime import datetime
+from datetime import datetime, date
 
 {% for model in models %}from .models import {{model.name}}
 {% endfor %}
 
 {% for model in models %}
 class {{model.name}}Service:
```

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/urls.py` & `bfactory-0.4.4/src/bfactory/core/templates/urls.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/core/templates/views.py` & `bfactory-0.4.4/src/bfactory/core/templates/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,123 +27,113 @@
 
 {% for model in models %}
 
 class {{model.name}}ListAPIView(ListAPIView):
     
 
     class OutputSerializer(serializers.Serializer):
-        
         pk = serializers.CharField()
 {% for field in model.fields -%}
 {{ '    ' }}{{ '    ' }}{{field.name}} = {% include "helpers/field_serializer.py" %}
 {%- endfor %}
 
 
     class InputSerializer(serializers.Serializer):
 {% for field in model.fields if field.editable -%}
+{%- if field.type != 'owner' -%}
 {{ '    ' }}{{ '    ' }}{{field.name}} = {% include "helpers/field_serializer.py" %}
+{%- endif -%}
 {%- endfor %}
         
-
     queryset = {{model.name|lower}}_list(fetched_by=None)
     serializer_class = InputSerializer
 
     def get(self, request):
 
         {{model.name|lower}}s = {{model.name|lower}}_list(fetched_by=self.request.user)
         data = self.OutputSerializer({{model.name|lower}}s, many=True).data
         return Response(data)
     
 
     def post(self, request):
 
         serializer = self.InputSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
-        
         service = {{model.name}}Service(user=self.request.user)
-
         {{model.name|lower}} = service.create(
-            {% for field in model.fields if field.editable -%}
-            {% if field.type == 'owner' %}{{field.name}}=self.request.user,
-            {% else %}
+            {%- for field in model.fields if field.editable -%}
+            {%- if field.type == 'owner' -%}{{field.name}}=self.request.user,
+            {%- else -%}
+            {%- if field.req -%}
             {{field.name}} = serializer.validated_data['{{field.name}}'],
-            {% endif %}
+            {%- else -%}
+            {{field.name}} = serializer.validated_data.get('{{field.name}}',None),
+            {%- endif -%}
+            {%- endif -%}
             {%- endfor %}
         )
-
         data = self.OutputSerializer({{model.name|lower}}, many=False).data
-
         return Response(data, status=status.HTTP_201_CREATED)
 
-
-
         
 
 class {{model.name}}APIView(APIView):
     
 
     class OutputSerializer(serializers.Serializer):
-        
         pk = serializers.CharField()
 {% for field in model.fields -%}
 {{ '    ' }}{{ '    ' }}{{field.name}} = {% include "helpers/field_serializer.py" %}
 {%- endfor %}
 
 
     class InputSerializer(serializers.Serializer):
 {% for field in model.fields if field.editable -%}
+{%- if field.type != 'owner' -%}
 {{ '    ' }}{{ '    ' }}{{field.name}} = {% include "helpers/field_serializer.py" %}
+{%- endif -%}
 {%- endfor %}
         
-
     serializer_class = InputSerializer
 
     def get_queryset(self):
         return {{model.name|lower}}_list(fetched_by=self.request.user)
         
-
-
     def get(self, request, id:int):
 
         {{model.name|lower}} = {{model.name|lower}}_get(fetched_by=self.request.user,id=id)
         data = self.OutputSerializer({{model.name|lower}}, many=False).data
         return Response(data)
 
     def put(self, request, id:int):
 
         {{model.name|lower}} = {{model.name|lower}}_get(fetched_by=self.request.user,id=id)
 
         serializer = self.InputSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
-        
         service = {{model.name}}Service(user=self.request.user)
-
         {{model.name|lower}} = service.update(
             {{model.name|lower}}={{model.name|lower}},
             {% for field in model.fields if field.editable -%}
-            {% if field.type == 'owner' %}{{field.name}}=self.request.user,
-            {% else %}
+            {%- if field.type == 'owner' -%}{{field.name}}=self.request.user,
+            {%- else -%}
+            {%- if field.req -%}
             {{field.name}} = serializer.validated_data['{{field.name}}'],
-            {% endif %}
+            {%- else -%}
+            {{field.name}} = serializer.validated_data.get('{{field.name}}',None),
+            {%- endif -%}
+            {%- endif -%}
             {%- endfor %}
         )
 
         data = self.OutputSerializer({{model.name|lower}}, many=False).data
-
         return Response(data, status=status.HTTP_201_CREATED)
 
 
     def delete(self, request, id:int):
 
         {{model.name|lower}} = {{model.name|lower}}_get(fetched_by=self.request.user,id=id)
-        
         service = {{model.name}}Service(user=self.request.user)
-        
         service.delete({{model.name|lower}}={{model.name|lower}})
-
         return Response(status=status.HTTP_200_OK)
 
-
-
-
-
 {% endfor %}
```

### Comparing `bfactory-0.4.2/src/bfactory/inputs/arguments.py` & `bfactory-0.4.4/src/bfactory/inputs/arguments.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 )
 
 
 parser.add_argument(
     '--force',
     '-f',
     nargs='*',
-    type=pathlib.Path,
     help='Si existe Path destino lo borra',
     required=False
 )
 
 parser.add_argument(
     '--update',
     '-u',
@@ -87,12 +86,11 @@
 )
 
 
 parser.add_argument(
     '--createadmin',
     '-a',
     nargs='*',
-    type=ManifestFileType(),
     help='Crea el usuario admin',
     required=False
 )
```

### Comparing `bfactory-0.4.2/src/bfactory/inputs/manifest.py` & `bfactory-0.4.4/src/bfactory/inputs/manifest.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/inputs/manifest.schema.json` & `bfactory-0.4.4/src/bfactory/inputs/manifest.schema.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9814307486133658%*

 * *Differences: {"'properties'": "{'database': {'anyOf': {0: {'properties': {'type': {'const': 'sqlite'}}, "*

 * *                 "'required': {delete: [4, 3, 2, 1]}}, 1: {'properties': {'type': {'const': "*

 * *                 "'postgres'}}, 'required': {insert: [(1, 'username'), (2, 'password'), (3, "*

 * *                 "'host'), (4, 'port')]}}}}, 'schema': {'items': {'properties': {'attrs': "*

 * *                 "{'items': {'properties': {'type': {'enum': {insert: [(4, 'user'), (5, 'owner'), "*

 * *                 "(6, 'int'), (7, 'pint […]*

```diff
@@ -11,33 +11,33 @@
             ]
         },
         "database": {
             "anyOf": [
                 {
                     "properties": {
                         "type": {
-                            "const": "postgres"
+                            "const": "sqlite"
                         }
                     },
                     "required": [
-                        "name",
-                        "username",
-                        "password",
-                        "host",
-                        "port"
+                        "name"
                     ]
                 },
                 {
                     "properties": {
                         "type": {
-                            "const": "sqlite"
+                            "const": "postgres"
                         }
                     },
                     "required": [
-                        "name"
+                        "name",
+                        "username",
+                        "password",
+                        "host",
+                        "port"
                     ]
                 }
             ],
             "properties": {
                 "host": {
                     "type": "string"
                 },
@@ -71,59 +71,122 @@
         "schema": {
             "description": "The model",
             "items": {
                 "properties": {
                     "attrs": {
                         "description": "The model attributes",
                         "items": {
+                            "allOf": [
+                                {
+                                    "if": {
+                                        "properties": {
+                                            "type": {
+                                                "const": "fk"
+                                            }
+                                        }
+                                    },
+                                    "then": {
+                                        "required": [
+                                            "fk"
+                                        ]
+                                    }
+                                },
+                                {
+                                    "if": {
+                                        "properties": {
+                                            "type": {
+                                                "const": "date"
+                                            }
+                                        }
+                                    },
+                                    "then": {
+                                        "required": [
+                                            "auto_now"
+                                        ]
+                                    }
+                                },
+                                {
+                                    "if": {
+                                        "properties": {
+                                            "type": {
+                                                "const": "datetime"
+                                            }
+                                        }
+                                    },
+                                    "then": {
+                                        "required": [
+                                            "auto_now"
+                                        ]
+                                    }
+                                }
+                            ],
                             "properties": {
+                                "auto_now": {
+                                    "type": "boolean"
+                                },
                                 "default": {
                                     "type": [
                                         "string",
                                         "boolean"
                                     ]
                                 },
+                                "fk": {
+                                    "type": "string"
+                                },
                                 "name": {
                                     "type": "string"
                                 },
                                 "req": {
                                     "type": "boolean"
                                 },
                                 "type": {
                                     "enum": [
                                         "str",
                                         "bool",
                                         "User",
-                                        "fk"
+                                        "fk",
+                                        "user",
+                                        "owner",
+                                        "int",
+                                        "pint",
+                                        "decimal",
+                                        "datetime",
+                                        "date"
                                     ]
                                 }
                             },
                             "required": [
                                 "name",
-                                "type"
+                                "type",
+                                "req"
                             ],
                             "type": "object"
                         },
                         "type": "array"
                     },
                     "name": {
                         "description": "The model name",
                         "type": "string"
                     }
                 },
+                "required": [
+                    "name",
+                    "attrs"
+                ],
                 "type": "object"
             },
             "type": "array"
         },
         "version": {
             "description": "The version of your backend",
             "type": "string"
         }
     },
     "required": [
         "name",
         "version",
-        "auth"
+        "auth",
+        "database"
     ],
     "title": "bfactory Manifest",
     "type": "object"
 }
```

### Comparing `bfactory-0.4.2/src/bfactory/inputs/parse_manifest.py` & `bfactory-0.4.4/src/bfactory/inputs/parse_manifest.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/inputs/validators.py` & `bfactory-0.4.4/src/bfactory/inputs/validators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 #!/usr/bin/env python
 
 import os
 from typing import List
 import json 
 import argparse
+from jsonschema import Draft202012Validator, ErrorTree, SchemaError, ValidationError, validate
+
+from bfactory.utils.state import State
+
 
 V_ENTORNO = [
     "BFACTORY_BUILD_PATH",
 ]
 
 
 def validar_variables_de_entorno() -> bool:
@@ -29,32 +33,56 @@
         Verifica:
             - si existe el archivo
             - si es un json valido
 
         TODO:
             - validar la estructura del manifiesto
     """
+    state = State()
+    manifest = {}
+    schema = {}
+    jsonschema_path = state.abspath('inputs/manifest.schema.json')
+
 
     #verifico si existe el archivo:
     if not os.path.exists(file_name):
         print("El archivo de manifiesto no existe")
         return False 
 
     try:
         with open(file_name) as f:
-            json.load(f)
+            manifest = json.load(f)
         f.close()
     except Exception as e:
         
         print("[ E ] >> El archivo de manifiesto no es un JSON valido")
         return False 
 
-    return True     
+    try:
+        
+        with open(jsonschema_path) as sf:
+            schema = json.load(sf)
+        sf.close()
+        validator = Draft202012Validator(schema=schema)
+        errors = list(validator.iter_errors(manifest))
+        if not errors:
+            return True 
+        
+        print("[ E ] >> El manifiesto no es valido")
+        for error in errors:
+            print(error.message)
+
+        return False    
+    
+    except ValidationError as ve:
+        print("[ E ] >> El archivo de manifiesto valido")
+        return False
 
 
 class ManifestFileType(argparse.FileType):
 
     def __call__(self, filename):
+        
         resp = super(ManifestFileType, self).__call__(filename)
-        if not validar_manifiesto(filename):
+        if not validar_manifiesto(file_name=filename):
             raise argparse.ArgumentTypeError('No es un manifiesto valido')
         return resp
```

### Comparing `bfactory-0.4.2/src/bfactory/main.py` & `bfactory-0.4.4/src/bfactory/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,17 +17,16 @@
     state = State()    
     state.to_path = getattr(args, 'path', None)
     state.update = getattr(args, 'update', None) != None 
     state.force = getattr(args, 'force', None) != None
     state.run_api = getattr(args, 'run', None) != None
     state.template = getattr(args, 'template', None)
     state.create_admin = getattr(args, 'createadmin', None) != None
-
     manifest = getattr(args, 'manifest', None)
-    
+
     if not manifest or not state.to_path:
         parser.print_help()
         return False
 
     if not state.check_path():
         return False
```

### Comparing `bfactory-0.4.2/src/bfactory/tests/engine_tests.py` & `bfactory-0.4.4/src/bfactory/tests/engine_tests.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/tests/manifest_test.py` & `bfactory-0.4.4/src/bfactory/tests/manifest_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,19 +12,20 @@
         self.manifest_path = state.abspath('tests/manifest_test.json')
         self.manifest = Manifest(file_path_manifest=self.manifest_path)
 
     def test_version(self):
         self.assertEqual(self.manifest.app_version, "1")
     
     def test_model(self):
-
         schema = self.manifest.get_shema()
         models = self.manifest.get_models()
-        self.assertEqual(1, len(models))
-        self.assertEqual("Tarea", models[0].name)
+        self.assertEqual(3, len(models))
+        self.assertEqual("Author", models[0].name)
+        self.assertEqual("Book", models[1].name)
+        self.assertEqual("Todo", models[2].name)
```

### Comparing `bfactory-0.4.2/src/bfactory/tests/run_tests.py` & `bfactory-0.4.4/src/bfactory/tests/run_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 import unittest
 
+from bfactory.tests.jsonschema_test import JsonSchemaTest
 from bfactory.tests.manifest_test import ManifestTest
 from bfactory.tests.engine_tests import EngineTest
 
 
 def create_suite(classes, unit_tests_to_run):
     
     suite = unittest.TestSuite()
@@ -16,17 +17,20 @@
             if function_name.lower().startswith( "test" ):
                 if unit_tests_to_run_count > 0 \
                         and function_name not in unit_tests_to_run:
                     continue
                 suite.addTest( _class( function_name ) )
     return suite
 
+
+
 def run_tests() -> bool:
     runner = unittest.TextTestRunner()
     classes =  [
+        JsonSchemaTest, 
         ManifestTest,
         EngineTest,
     ]
 
     unit_tests_to_run =  [ ]
     result = runner.run( create_suite( classes, unit_tests_to_run ) )
     return result.wasSuccessful()
```

### Comparing `bfactory-0.4.2/src/bfactory/utils/crypto.py` & `bfactory-0.4.4/src/bfactory/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory/utils/state.py` & `bfactory-0.4.4/src/bfactory/utils/state.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.2/src/bfactory.egg-info/PKG-INFO` & `bfactory-0.4.4/src/bfactory.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfactory
-Version: 0.4.2
+Version: 0.4.4
 Summary: Build an API from a manifest file
 Home-page: https://github.com/forkear/bfactory
 Author: Forkear
 Author-email: forkear@no-spam.org
 Project-URL: Documentation, https://github.com/forkear/bfactory/blob/main/README.md
 Project-URL: Source, https://github.com/forkear/bfactory
 Project-URL: Tracker, https://github.com/forkear/bfactory/issues
```

### Comparing `bfactory-0.4.2/src/bfactory.egg-info/SOURCES.txt` & `bfactory-0.4.4/src/bfactory.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,13 +33,14 @@
 src/bfactory/inputs/arguments.py
 src/bfactory/inputs/manifest.py
 src/bfactory/inputs/manifest.schema.json
 src/bfactory/inputs/parse_manifest.py
 src/bfactory/inputs/validators.py
 src/bfactory/tests/__init__.py
 src/bfactory/tests/engine_tests.py
+src/bfactory/tests/jsonschema_test.py
 src/bfactory/tests/manifest_test.json
 src/bfactory/tests/manifest_test.py
 src/bfactory/tests/run_tests.py
 src/bfactory/utils/crypto.py
 src/bfactory/utils/render.py
 src/bfactory/utils/state.py
```

