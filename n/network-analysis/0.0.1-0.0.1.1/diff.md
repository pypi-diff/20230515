# Comparing `tmp/network-analysis-0.0.1.tar.gz` & `tmp/network-analysis-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-analysis-0.0.1.tar", last modified: Sun Feb 26 01:57:37 2023, max compression
+gzip compressed data, was "network-analysis-0.0.1.1.tar", last modified: Mon May 15 01:23:44 2023, max compression
```

## Comparing `network-analysis-0.0.1.tar` & `network-analysis-0.0.1.1.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 01:57:37.120206 network-analysis-0.0.1/
--rw-rw-rw-   0        0        0    35149 2023-02-26 01:40:30.000000 network-analysis-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      530 2023-02-26 01:57:37.117516 network-analysis-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-26 01:51:41.000000 network-analysis-0.0.1/README.md
--rw-rw-rw-   0        0        0      617 2023-02-26 01:55:36.000000 network-analysis-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-26 01:57:37.120206 network-analysis-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-26 01:57:37.073860 network-analysis-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-02-26 01:57:37.086197 network-analysis-0.0.1/src/network-analysis/
--rw-rw-rw-   0        0        0        0 2023-02-26 01:36:46.000000 network-analysis-0.0.1/src/network-analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-26 01:57:37.116509 network-analysis-0.0.1/src/network_analysis.egg-info/
--rw-rw-rw-   0        0        0      530 2023-02-26 01:57:36.000000 network-analysis-0.0.1/src/network_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-02-26 01:57:37.000000 network-analysis-0.0.1/src/network_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 01:57:36.000000 network-analysis-0.0.1/src/network_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-02-26 01:57:36.000000 network-analysis-0.0.1/src/network_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/src/network_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 01:23:44.000000 network-analysis-0.0.1.1/src/network_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-15 01:23:44.000000 network-analysis-0.0.1.1/src/network_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:23:44.000000 network-analysis-0.0.1.1/src/network_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 01:23:44.000000 network-analysis-0.0.1.1/src/network_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/src/networkanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/src/networkanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/src/networkanalysis/ergm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/src/networkanalysis/ergm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/src/networkanalysis/ergm/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/src/networkanalysis/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/tests/test_statistics.py
```

### Comparing `network-analysis-0.0.1/LICENCE` & `network-analysis-0.0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `network-analysis-0.0.1/pyproject.toml` & `network-analysis-0.0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "network-analysis"
-version = "0.0.1"
+version = "0.0.1.1"
 authors = [
   { name="Gabriel Fortin-Leblanc", email="gabriel.fortin-leblanc@umontreal.ca" },
 ]
 description = "Work in progress..."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/gabriel-fortin-leblanc/network-analysis"
-"Bug Tracker" = "https://github.com/gabriel-fortin-leblanc/network-analysis/issues"
+"Bug Tracker" = "https://github.com/gabriel-fortin-leblanc/network-analysis/issues"
```

