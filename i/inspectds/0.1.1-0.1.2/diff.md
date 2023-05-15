# Comparing `tmp/inspectds-0.1.1.tar.gz` & `tmp/inspectds-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspectds-0.1.1.tar", max compression
+gzip compressed data, was "inspectds-0.1.2.tar", max compression
```

## Comparing `inspectds-0.1.1.tar` & `inspectds-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0        0 2022-01-12 14:50:49.718152 inspectds-0.1.1/inspectds/__init__.py
--rw-r--r--   0        0        0     5948 2023-04-26 06:36:14.421631 inspectds-0.1.1/inspectds/cli.py
--rw-r--r--   0        0        0     1991 2023-04-26 06:37:40.314098 inspectds-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 inspectds-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-26 07:05:35.386016 inspectds-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2557 2023-04-26 07:05:35.386016 inspectds-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2022-01-12 14:50:49.718152 inspectds-0.1.2/inspectds/__init__.py
+-rw-r--r--   0        0        0     5948 2023-04-26 06:51:41.603165 inspectds-0.1.2/inspectds/cli.py
+-rw-r--r--   0        0        0     2461 2023-04-26 07:05:43.749138 inspectds-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 inspectds-0.1.2/PKG-INFO
```

### Comparing `inspectds-0.1.1/inspectds/cli.py` & `inspectds-0.1.2/inspectds/cli.py`

 * *Files identical despite different names*

### Comparing `inspectds-0.1.1/pyproject.toml` & `inspectds-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 [tool.poetry]
 name = "inspectds"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Panos Mavrogiorgos <pmav99@gmail.com>"]
+license = "Unlicense"
+readme = "README.md"
+repository = "https://github.com/pmav99/inspectds.git"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: The Unlicense (Unlicense)",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Utilities",
+]
 
 [tool.poetry.scripts]
 inspectds = "inspectds.cli:app"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 xarray = "*"
```

