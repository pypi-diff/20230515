# Comparing `tmp/netunicorn-base-0.3.2.tar.gz` & `tmp/netunicorn-base-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-base-0.3.2.tar", last modified: Wed May 10 10:25:27 2023, max compression
+gzip compressed data, was "netunicorn-base-0.3.3.tar", last modified: Sun May 14 23:15:39 2023, max compression
```

## Comparing `netunicorn-base-0.3.2.tar` & `netunicorn-base-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.703419 netunicorn-base-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-10 10:25:27.703419 netunicorn-base-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 10:25:27.703419 netunicorn-base-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.699419 netunicorn-base-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.699419 netunicorn-base-0.3.2/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.703419 netunicorn-base-0.3.2/src/netunicorn/base/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/environment_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.699419 netunicorn-base-0.3.2/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.703419 netunicorn-base-0.3.2/src/netunicorn/director/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/director/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.703419 netunicorn-base-0.3.2/src/netunicorn/director/base/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/director/base/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/director/base/connectors/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/director/base/connectors/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/director/base/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/director/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/director/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:16.000000 netunicorn-base-0.3.2/src/netunicorn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:25:27.703419 netunicorn-base-0.3.2/src/netunicorn_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-10 10:25:27.000000 netunicorn-base-0.3.2/src/netunicorn_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-10 10:25:27.000000 netunicorn-base-0.3.2/src/netunicorn_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:25:27.000000 netunicorn-base-0.3.2/src/netunicorn_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 10:25:27.000000 netunicorn-base-0.3.2/src/netunicorn_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 10:25:27.000000 netunicorn-base-0.3.2/src/netunicorn_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.916385 netunicorn-base-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-14 23:15:39.916385 netunicorn-base-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 23:15:39.916385 netunicorn-base-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/environment_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/director/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.916385 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/top_level.txt
```

### Comparing `netunicorn-base-0.3.2/pyproject.toml` & `netunicorn-base-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-base"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn base module"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/__init__.py` & `netunicorn-base-0.3.3/src/netunicorn/base/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/deployment.py` & `netunicorn-base-0.3.3/src/netunicorn/base/deployment.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/environment_definitions.py` & `netunicorn-base-0.3.3/src/netunicorn/base/environment_definitions.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/experiment.py` & `netunicorn-base-0.3.3/src/netunicorn/base/experiment.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/nodes.py` & `netunicorn-base-0.3.3/src/netunicorn/base/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         )
 
     def __repr__(self) -> str:
         return str(self)
 
     def __next__(self) -> Node:
         node = deepcopy(next(self._nodes))
-        node.name += str(uuid4())
+        node.name += uuid4().hex
         return node
 
     def __getitem__(self, key: int) -> Node:
         return self._node_template[key]
 
     def __setitem__(self, key: int, value: Node) -> None:
         self._node_template[key] = value
```

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/pipeline.py` & `netunicorn-base-0.3.3/src/netunicorn/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/task.py` & `netunicorn-base-0.3.3/src/netunicorn/base/task.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/types.py` & `netunicorn-base-0.3.3/src/netunicorn/base/types.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/base/utils.py` & `netunicorn-base-0.3.3/src/netunicorn/base/utils.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/director/base/connectors/protocol.py` & `netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/protocol.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn/director/base/resources.py` & `netunicorn-base-0.3.3/src/netunicorn/director/base/resources.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.2/src/netunicorn_base.egg-info/SOURCES.txt` & `netunicorn-base-0.3.3/src/netunicorn_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

