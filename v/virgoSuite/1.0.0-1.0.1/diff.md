# Comparing `tmp/virgoSuite-1.0.0.tar.gz` & `tmp/virgoSuite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgoSuite-1.0.0.tar", last modified: Mon May 15 16:48:05 2023, max compression
+gzip compressed data, was "virgoSuite-1.0.1.tar", last modified: Mon May 15 17:16:56 2023, max compression
```

## Comparing `virgoSuite-1.0.0.tar` & `virgoSuite-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:48:05.254796 virgoSuite-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-15 16:48:05.254796 virgoSuite-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:48:05.254796 virgoSuite-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:48:05.250796 virgoSuite-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:48:05.250796 virgoSuite-1.0.0/src/virgoSuite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/src/virgoSuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/src/virgoSuite/sfdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:48:05.250796 virgoSuite-1.0.0/src/virgoSuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-15 16:48:05.000000 virgoSuite-1.0.0/src/virgoSuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 16:48:05.000000 virgoSuite-1.0.0/src/virgoSuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:48:05.000000 virgoSuite-1.0.0/src/virgoSuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 16:48:05.000000 virgoSuite-1.0.0/src/virgoSuite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/src/virgoSuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/src/virgoSuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/src/virgoSuite/sfdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/src/virgoSuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/top_level.txt
```

### Comparing `virgoSuite-1.0.0/LICENSE` & `virgoSuite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `virgoSuite-1.0.0/setup.py` & `virgoSuite-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,12 +24,23 @@
     description="Toolbox used from the data analysis group of Virgo Rome",  # Optional
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Riccardo Felicetti",
     author_email="riccardo.felicetti@infn.it",
     license="MIT",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
     ],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
+    install_requires=[
+        "numpy",
+        "scipy",
+        "matplotlib",
+        "xarray",
+        "pandas",
+        "astropy",
+        "zarr",
+        "tqdm",
+        "requests",
+    ],
 )
```

### Comparing `virgoSuite-1.0.0/src/virgoSuite/sfdb.py` & `virgoSuite-1.0.1/src/virgoSuite/sfdb.py`

 * *Files identical despite different names*

