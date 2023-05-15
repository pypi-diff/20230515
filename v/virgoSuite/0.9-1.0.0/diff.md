# Comparing `tmp/virgoSuite-0.9.tar.gz` & `tmp/virgoSuite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgoSuite-0.9.tar", last modified: Wed May 10 12:37:10 2023, max compression
+gzip compressed data, was "virgoSuite-1.0.0.tar", last modified: Mon May 15 16:48:05 2023, max compression
```

## Comparing `virgoSuite-0.9.tar` & `virgoSuite-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:37:10.848439 virgoSuite-0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 12:36:51.000000 virgoSuite-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 12:37:10.848439 virgoSuite-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 12:36:51.000000 virgoSuite-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:37:10.848439 virgoSuite-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 12:36:51.000000 virgoSuite-0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:37:10.848439 virgoSuite-0.9/virgoSuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 12:37:10.000000 virgoSuite-0.9/virgoSuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 12:37:10.000000 virgoSuite-0.9/virgoSuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:37:10.000000 virgoSuite-0.9/virgoSuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:37:10.000000 virgoSuite-0.9/virgoSuite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:48:05.254796 virgoSuite-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-15 16:48:05.254796 virgoSuite-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:48:05.254796 virgoSuite-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:48:05.250796 virgoSuite-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:48:05.250796 virgoSuite-1.0.0/src/virgoSuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/src/virgoSuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-05-15 16:47:49.000000 virgoSuite-1.0.0/src/virgoSuite/sfdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:48:05.250796 virgoSuite-1.0.0/src/virgoSuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-15 16:48:05.000000 virgoSuite-1.0.0/src/virgoSuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 16:48:05.000000 virgoSuite-1.0.0/src/virgoSuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:48:05.000000 virgoSuite-1.0.0/src/virgoSuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 16:48:05.000000 virgoSuite-1.0.0/src/virgoSuite.egg-info/top_level.txt
```

### Comparing `virgoSuite-0.9/LICENSE` & `virgoSuite-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virgoSuite-0.9/setup.py` & `virgoSuite-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,9 +26,10 @@
     long_description=long_description,
     author="Riccardo Felicetti",
     author_email="riccardo.felicetti@infn.it",
     license="MIT",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
-    packages=find_packages(include=["virgoSuie", "virgoSuite.*"]),
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
 )
```

