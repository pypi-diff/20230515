# Comparing `tmp/calculemus-0.0.1.tar.gz` & `tmp/calculemus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculemus-0.0.1.tar", last modified: Mon May 15 12:52:04 2023, max compression
+gzip compressed data, was "calculemus-0.0.2.tar", last modified: Mon May 15 13:23:44 2023, max compression
```

## Comparing `calculemus-0.0.1.tar` & `calculemus-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 12:52:04.332261 calculemus-0.0.1/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1077 2023-05-15 11:44:36.000000 calculemus-0.0.1/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      643 2023-05-15 12:52:04.332261 calculemus-0.0.1/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       65 2023-05-15 11:44:36.000000 calculemus-0.0.1/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      659 2023-05-15 12:50:40.000000 calculemus-0.0.1/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-05-15 12:52:04.332261 calculemus-0.0.1/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 12:52:04.332261 calculemus-0.0.1/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 12:52:04.332261 calculemus-0.0.1/src/calculemus/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      106 2023-05-15 11:53:16.000000 calculemus-0.0.1/src/calculemus/__init__.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 12:52:04.332261 calculemus-0.0.1/src/calculemus/core/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-05-15 11:56:47.000000 calculemus-0.0.1/src/calculemus/core/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       34 2023-05-15 11:54:06.000000 calculemus-0.0.1/src/calculemus/version.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 12:52:04.332261 calculemus-0.0.1/src/calculemus.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      643 2023-05-15 12:52:04.000000 calculemus-0.0.1/src/calculemus.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      269 2023-05-15 12:52:04.000000 calculemus-0.0.1/src/calculemus.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-05-15 12:52:04.000000 calculemus-0.0.1/src/calculemus.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-05-15 12:52:04.000000 calculemus-0.0.1/src/calculemus.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 13:23:44.367228 calculemus-0.0.2/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1077 2023-05-15 11:44:36.000000 calculemus-0.0.2/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      658 2023-05-15 13:23:44.367228 calculemus-0.0.2/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       80 2023-05-15 13:21:02.000000 calculemus-0.0.2/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      659 2023-05-15 13:17:29.000000 calculemus-0.0.2/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-05-15 13:23:44.367228 calculemus-0.0.2/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 13:23:44.367228 calculemus-0.0.2/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 13:23:44.367228 calculemus-0.0.2/src/calculemus/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      106 2023-05-15 11:53:16.000000 calculemus-0.0.2/src/calculemus/__init__.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 13:23:44.367228 calculemus-0.0.2/src/calculemus/core/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-05-15 11:56:47.000000 calculemus-0.0.2/src/calculemus/core/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       34 2023-05-15 11:54:06.000000 calculemus-0.0.2/src/calculemus/version.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-05-15 13:23:44.367228 calculemus-0.0.2/src/calculemus.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      658 2023-05-15 13:23:44.000000 calculemus-0.0.2/src/calculemus.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      269 2023-05-15 13:23:44.000000 calculemus-0.0.2/src/calculemus.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-05-15 13:23:44.000000 calculemus-0.0.2/src/calculemus.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-05-15 13:23:44.000000 calculemus-0.0.2/src/calculemus.egg-info/top_level.txt
```

### Comparing `calculemus-0.0.1/LICENSE` & `calculemus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calculemus-0.0.1/PKG-INFO` & `calculemus-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: calculemus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Logical verification of probabilistic/language model 'intuitions'.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/machina-ratiocinatrix/calculemus
 Project-URL: Bug Tracker, https://github.com/machina-ratiocinatrix/calculemus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# calculemus
-Logical verification of probabilistic 'intuitions'.
+# Calculemus
+Logical verification of probabilistic/language model 'intuitions'.
```

### Comparing `calculemus-0.0.1/pyproject.toml` & `calculemus-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "calculemus"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Logical verification of probabilistic/language model 'intuitions'."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `calculemus-0.0.1/src/calculemus.egg-info/PKG-INFO` & `calculemus-0.0.2/src/calculemus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: calculemus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Logical verification of probabilistic/language model 'intuitions'.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/machina-ratiocinatrix/calculemus
 Project-URL: Bug Tracker, https://github.com/machina-ratiocinatrix/calculemus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# calculemus
-Logical verification of probabilistic 'intuitions'.
+# Calculemus
+Logical verification of probabilistic/language model 'intuitions'.
```

