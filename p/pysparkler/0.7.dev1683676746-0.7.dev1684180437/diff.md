# Comparing `tmp/pysparkler-0.7.dev1683676746.tar.gz` & `tmp/pysparkler-0.7.dev1684180437.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.7.dev1683676746.tar", max compression
+gzip compressed data, was "pysparkler-0.7.dev1684180437.tar", max compression
```

## Comparing `pysparkler-0.7.dev1683676746.tar` & `pysparkler-0.7.dev1684180437.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    12173 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/README.md
--rw-r--r--   0        0        0     1203 2023-05-09 23:59:06.821590 pysparkler-0.7.dev1683676746/pyproject.toml
--rw-r--r--   0        0        0      807 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/__init__.py
--rw-r--r--   0        0        0     5294 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/api.py
--rw-r--r--   0        0        0     7372 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/base.py
--rw-r--r--   0        0        0     6398 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     2206 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10561 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3969 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4550 2023-05-09 23:58:59.305604 pysparkler-0.7.dev1683676746/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0    13052 1970-01-01 00:00:00.000000 pysparkler-0.7.dev1683676746/PKG-INFO
+-rw-r--r--   0        0        0    12173 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/README.md
+-rw-r--r--   0        0        0     1203 2023-05-15 19:53:58.347415 pysparkler-0.7.dev1684180437/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/__init__.py
+-rw-r--r--   0        0        0     5294 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/api.py
+-rw-r--r--   0        0        0     7372 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/base.py
+-rw-r--r--   0        0        0     6398 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2206 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10561 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4550 2023-05-15 19:53:50.871330 pysparkler-0.7.dev1684180437/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0    13052 1970-01-01 00:00:00.000000 pysparkler-0.7.dev1684180437/PKG-INFO
```

### Comparing `pysparkler-0.7.dev1683676746/README.md` & `pysparkler-0.7.dev1684180437/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pyproject.toml` & `pysparkler-0.7.dev1684180437/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.7.dev1683676746"
+version = "0.7.dev1684180437"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/__init__.py` & `pysparkler-0.7.dev1684180437/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/api.py` & `pysparkler-0.7.dev1684180437/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/base.py` & `pysparkler-0.7.dev1684180437/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/cli.py` & `pysparkler-0.7.dev1684180437/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.7.dev1684180437/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.7.dev1684180437/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.7.dev1684180437/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.7.dev1684180437/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.7.dev1684180437/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1683676746/PKG-INFO` & `pysparkler-0.7.dev1684180437/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.7.dev1683676746
+Version: 0.7.dev1684180437
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

