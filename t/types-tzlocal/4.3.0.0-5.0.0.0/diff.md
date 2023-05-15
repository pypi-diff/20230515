# Comparing `tmp/types-tzlocal-4.3.0.0.tar.gz` & `tmp/types-tzlocal-5.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tzlocal-4.3.0.0.tar", last modified: Sun Mar 19 09:15:11 2023, max compression
+gzip compressed data, was "types-tzlocal-5.0.0.0.tar", last modified: Mon May 15 09:15:14 2023, max compression
```

## Comparing `types-tzlocal-4.3.0.0.tar` & `types-tzlocal-5.0.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:15:11.588675 types-tzlocal-4.3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-19 09:15:10.000000 types-tzlocal-4.3.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-19 09:15:10.000000 types-tzlocal-4.3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-19 09:15:11.588675 types-tzlocal-4.3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 09:15:11.588675 types-tzlocal-4.3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-19 09:15:10.000000 types-tzlocal-4.3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:15:11.588675 types-tzlocal-4.3.0.0/types_tzlocal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-19 09:15:11.000000 types-tzlocal-4.3.0.0/types_tzlocal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-19 09:15:11.000000 types-tzlocal-4.3.0.0/types_tzlocal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 09:15:11.000000 types-tzlocal-4.3.0.0/types_tzlocal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-19 09:15:11.000000 types-tzlocal-4.3.0.0/types_tzlocal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-19 09:15:11.000000 types-tzlocal-4.3.0.0/types_tzlocal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:15:11.588675 types-tzlocal-4.3.0.0/tzlocal-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-19 09:15:10.000000 types-tzlocal-4.3.0.0/tzlocal-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-19 09:14:58.000000 types-tzlocal-4.3.0.0/tzlocal-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-19 09:14:58.000000 types-tzlocal-4.3.0.0/tzlocal-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-19 09:14:58.000000 types-tzlocal-4.3.0.0/tzlocal-stubs/windows_tz.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:15:14.703823 types-tzlocal-5.0.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-15 09:15:12.000000 types-tzlocal-5.0.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 09:15:12.000000 types-tzlocal-5.0.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-15 09:15:14.703823 types-tzlocal-5.0.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:15:14.703823 types-tzlocal-5.0.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-15 09:15:12.000000 types-tzlocal-5.0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:15:14.703823 types-tzlocal-5.0.0.0/types_tzlocal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-15 09:15:14.000000 types-tzlocal-5.0.0.0/types_tzlocal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-15 09:15:14.000000 types-tzlocal-5.0.0.0/types_tzlocal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:15:14.000000 types-tzlocal-5.0.0.0/types_tzlocal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 09:15:14.000000 types-tzlocal-5.0.0.0/types_tzlocal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 09:15:14.000000 types-tzlocal-5.0.0.0/types_tzlocal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:15:14.703823 types-tzlocal-5.0.0.0/tzlocal-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 09:15:12.000000 types-tzlocal-5.0.0.0/tzlocal-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-15 09:14:55.000000 types-tzlocal-5.0.0.0/tzlocal-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-15 09:14:55.000000 types-tzlocal-5.0.0.0/tzlocal-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 09:14:55.000000 types-tzlocal-5.0.0.0/tzlocal-stubs/windows_tz.pyi
```

### Comparing `types-tzlocal-4.3.0.0/CHANGELOG.md` & `types-tzlocal-5.0.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 5.0.0.0 (2023-05-15)
+
+Bump `tzlocal` to `5.0` (#10183)
+
 ## 4.3.0.0 (2023-03-19)
 
 [stubsabot] Bump tzlocal to 4.3 (#9903)
 
 Release: https://pypi.org/pypi/tzlocal/4.3
 Diff: https://github.com/regebro/tzlocal/compare/4.2...4.3
```

### Comparing `types-tzlocal-4.3.0.0/PKG-INFO` & `types-tzlocal-5.0.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tzlocal
-Version: 4.3.0.0
+Version: 5.0.0.0
 Summary: Typing stubs for tzlocal
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tzlocal.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tzlocal`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tzlocal. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8080e491d2fa92b1b1390c87fac23a1a38dcd919`.
+This package was generated from typeshed commit `b25a5b6aef4b18226a9fd367421ed8ebaaed9528`.
```

### Comparing `types-tzlocal-4.3.0.0/setup.py` & `types-tzlocal-5.0.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tzlocal`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tzlocal. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8080e491d2fa92b1b1390c87fac23a1a38dcd919`.
+This package was generated from typeshed commit `b25a5b6aef4b18226a9fd367421ed8ebaaed9528`.
 '''.lstrip()
 
 setup(name=name,
-      version="4.3.0.0",
+      version="5.0.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tzlocal.md",
```

### Comparing `types-tzlocal-4.3.0.0/types_tzlocal.egg-info/PKG-INFO` & `types-tzlocal-5.0.0.0/types_tzlocal.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tzlocal
-Version: 4.3.0.0
+Version: 5.0.0.0
 Summary: Typing stubs for tzlocal
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tzlocal.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tzlocal`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tzlocal. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8080e491d2fa92b1b1390c87fac23a1a38dcd919`.
+This package was generated from typeshed commit `b25a5b6aef4b18226a9fd367421ed8ebaaed9528`.
```

