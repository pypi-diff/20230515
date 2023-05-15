# Comparing `tmp/typer_config-0.1.3a3.tar.gz` & `tmp/typer_config-0.1.3a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.1.3a3.tar", max compression
+gzip compressed data, was "typer_config-0.1.3a5.tar", max compression
```

## Comparing `typer_config-0.1.3a3.tar` & `typer_config-0.1.3a5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/LICENSE
--rw-r--r--   0        0        0     1044 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/README.md
--rw-r--r--   0        0        0     1010 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/pyproject.toml
--rw-r--r--   0        0        0     1434 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/typer_config/__init__.py
--rw-r--r--   0        0        0     1081 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/typer_config/_typing.py
--rw-r--r--   0        0        0     3714 2023-05-15 01:37:34.135512 typer_config-0.1.3a3/typer_config/loaders.py
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 typer_config-0.1.3a3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-15 01:53:18.490990 typer_config-0.1.3a5/LICENSE
+-rw-r--r--   0        0        0     1044 2023-05-15 01:53:18.490990 typer_config-0.1.3a5/README.md
+-rw-r--r--   0        0        0     1010 2023-05-15 01:53:18.494990 typer_config-0.1.3a5/pyproject.toml
+-rw-r--r--   0        0        0     1434 2023-05-15 01:53:18.494990 typer_config-0.1.3a5/typer_config/__init__.py
+-rw-r--r--   0        0        0     1081 2023-05-15 01:53:18.494990 typer_config-0.1.3a5/typer_config/_typing.py
+-rw-r--r--   0        0        0     3714 2023-05-15 01:53:18.494990 typer_config-0.1.3a5/typer_config/loaders.py
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 typer_config-0.1.3a5/PKG-INFO
```

### Comparing `typer_config-0.1.3a3/LICENSE` & `typer_config-0.1.3a5/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.3a3/README.md` & `typer_config-0.1.3a5/README.md`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.3a3/pyproject.toml` & `typer_config-0.1.3a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.1.3a3"
+version = "0.1.3a5"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 keywords = ["typer"]
```

### Comparing `typer_config-0.1.3a3/typer_config/__init__.py` & `typer_config-0.1.3a5/typer_config/__init__.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.3a3/typer_config/_typing.py` & `typer_config-0.1.3a5/typer_config/_typing.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.3a3/typer_config/loaders.py` & `typer_config-0.1.3a5/typer_config/loaders.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.3a3/PKG-INFO` & `typer_config-0.1.3a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.1.3a3
+Version: 0.1.3a5
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://github.com/maxb2/typer-config
 License: MIT
 Keywords: typer
 Author: Matt Anderson
 Author-email: matt@manderscience.com
 Requires-Python: >=3.8,<4.0
```

