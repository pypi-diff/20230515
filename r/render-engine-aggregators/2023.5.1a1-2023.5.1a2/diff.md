# Comparing `tmp/render_engine_aggregators-2023.5.1a1.tar.gz` & `tmp/render_engine_aggregators-2023.5.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine_aggregators-2023.5.1a1.tar", last modified: Mon May 15 12:12:16 2023, max compression
+gzip compressed data, was "render_engine_aggregators-2023.5.1a2.tar", last modified: Mon May 15 13:28:52 2023, max compression
```

## Comparing `render_engine_aggregators-2023.5.1a1.tar` & `render_engine_aggregators-2023.5.1a2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/.github/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:12:16.552987 render_engine_aggregators-2023.5.1a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators/feed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 12:12:16.000000 render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-15 12:12:16.000000 render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:12:16.000000 render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 12:12:16.000000 render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 12:12:16.000000 render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:12:16.556987 render_engine_aggregators-2023.5.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 12:12:00.000000 render_engine_aggregators-2023.5.1a1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:28:52.323172 render_engine_aggregators-2023.5.1a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:28:52.319172 render_engine_aggregators-2023.5.1a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/.github/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:28:52.319172 render_engine_aggregators-2023.5.1a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:28:52.319172 render_engine_aggregators-2023.5.1a2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 13:28:52.323172 render_engine_aggregators-2023.5.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:28:52.323172 render_engine_aggregators-2023.5.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:28:52.319172 render_engine_aggregators-2023.5.1a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:28:52.319172 render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators/feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:28:52.323172 render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 13:28:52.000000 render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-15 13:28:52.000000 render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:28:52.000000 render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 13:28:52.000000 render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 13:28:52.000000 render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:28:52.323172 render_engine_aggregators-2023.5.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-15 13:28:31.000000 render_engine_aggregators-2023.5.1a2/tests/test.py
```

### Comparing `render_engine_aggregators-2023.5.1a1/.github/CODE_OF_CONDUCT.md` & `render_engine_aggregators-2023.5.1a2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/.github/LICENSE` & `render_engine_aggregators-2023.5.1a2/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/.github/dependabot.yml` & `render_engine_aggregators-2023.5.1a2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/.github/workflows/publish.yml` & `render_engine_aggregators-2023.5.1a2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/.gitignore` & `render_engine_aggregators-2023.5.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/.vscode/settings.json` & `render_engine_aggregators-2023.5.1a2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/pyproject.toml` & `render_engine_aggregators-2023.5.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/requirements.txt` & `render_engine_aggregators-2023.5.1a2/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/src/render_engine_aggregators.egg-info/SOURCES.txt` & `render_engine_aggregators-2023.5.1a2/src/render_engine_aggregators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a1/tests/conftest.py` & `render_engine_aggregators-2023.5.1a2/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         pages = [page2()]
 
 
     class AggregateFeed1(AggregateFeed):
         collections = [Collection1, Collection2]
 
 
-    return AggregateFeed1()
+    return AggregateFeed1
```

