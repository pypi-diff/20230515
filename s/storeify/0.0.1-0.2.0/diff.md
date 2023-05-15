# Comparing `tmp/storeify-0.0.1.tar.gz` & `tmp/storeify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storeify-0.0.1.tar", last modified: Wed Apr 19 00:25:35 2023, max compression
+gzip compressed data, was "storeify-0.2.0.tar", last modified: Mon May 15 11:51:24 2023, max compression
```

## Comparing `storeify-0.0.1.tar` & `storeify-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,15 @@
--rw-r--r--   0        0        0     3078 2023-04-19 00:25:21.256487 storeify-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-19 00:21:33.679997 storeify-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-19 00:21:38.220086 storeify-0.0.1/README.md
--rw-r--r--   0        0        0     1144 2023-04-19 00:24:37.711626 storeify-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-04-19 00:25:09.488254 storeify-0.0.1/storeify/__init__.py
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 storeify-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-15 11:51:16.623293 storeify-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3100 2023-04-20 18:30:40.068815 storeify-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-19 00:21:33.679997 storeify-0.2.0/LICENSE
+-rw-r--r--   0        0        0       73 2023-05-15 11:03:51.249023 storeify-0.2.0/README.md
+-rw-r--r--   0        0        0     1239 2023-05-15 11:03:56.125144 storeify-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-05-15 10:55:53.005648 storeify-0.2.0/storeify/__init__.py
+-rw-r--r--   0        0        0     2349 2023-05-15 10:07:32.625312 storeify-0.2.0/storeify/base.py
+-rw-r--r--   0        0        0       85 2023-05-15 10:07:32.625312 storeify-0.2.0/storeify/errors.py
+-rw-r--r--   0        0        0     1462 2023-05-15 11:01:40.369812 storeify-0.2.0/storeify/file.py
+-rw-r--r--   0        0        0      791 2023-05-15 10:56:20.738274 storeify-0.2.0/storeify/memory.py
+-rw-r--r--   0        0        0      663 2023-05-15 10:56:15.630158 storeify-0.2.0/storeify/shared.py
+-rw-r--r--   0        0        0      348 2023-05-15 10:55:19.816905 storeify-0.2.0/storeify/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:53:05.489951 storeify-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      708 2023-05-15 11:03:32.548561 storeify-0.2.0/tests/test_stores.py
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 storeify-0.2.0/PKG-INFO
```

### Comparing `storeify-0.0.1/.gitignore` & `storeify-0.2.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+.vscode/settings.json
```

### Comparing `storeify-0.0.1/LICENSE` & `storeify-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `storeify-0.0.1/pyproject.toml` & `storeify-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "storeify"
-version = "0.0.1"
-description = "Data storage made simple"
+version = "0.2.0"
+description = "Data storage made simple!"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -28,15 +28,23 @@
 requires-python = ">=3.9"
 dependencies = []
 
 [project.urls]
 Source = "https://github.com/Ben-Brady/storeify"
 
 [project.optional-dependencies]
-test = []
+redis = [
+    "redis[hiredis]~=4.5.4",
+]
+s3 = [
+    "boto3~=1.26.116",
+]
+test = [
+    "pytest~=7.3.1"
+]
 docs = []
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests",
```

