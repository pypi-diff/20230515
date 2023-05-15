# Comparing `tmp/azureenergylabelercli-2.0.3.tar.gz` & `tmp/azureenergylabelercli-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureenergylabelercli-2.0.3.tar", last modified: Tue Mar 21 13:58:06 2023, max compression
+gzip compressed data, was "azureenergylabelercli-2.1.0.tar", last modified: Mon May 15 09:23:40 2023, max compression
```

## Comparing `azureenergylabelercli-2.0.3.tar` & `azureenergylabelercli-2.1.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:58:06.065608 azureenergylabelercli-2.0.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-03-21 13:58:06.065608 azureenergylabelercli-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   108909 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     8088 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/USAGE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/azure_energy_labeler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:58:06.061608 azureenergylabelercli-2.0.3/azureenergylabelercli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   108909 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     8088 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2170 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17288 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/azureenergylabelercli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/azureenergylabelercliexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:58:06.065608 azureenergylabelercli-2.0.3/azureenergylabelercli/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/conf/logging.json-example
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/azureenergylabelercli/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:58:06.065608 azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-21 13:58:06.000000 azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:58:06.065608 azureenergylabelercli-2.0.3/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6822 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9072 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-21 13:58:05.000000 azureenergylabelercli-2.0.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-03-21 13:58:06.065608 azureenergylabelercli-2.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:58:06.065608 azureenergylabelercli-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-21 13:56:33.000000 azureenergylabelercli-2.0.3/tests/test_azureenergylabelercli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:23:40.703066 azureenergylabelercli-2.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-05-15 09:23:40.703066 azureenergylabelercli-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   108010 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8103 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/USAGE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/azure_energy_labeler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:23:40.699066 azureenergylabelercli-2.1.0/azureenergylabelercli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   108010 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8103 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2170 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18592 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/azureenergylabelercli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/azureenergylabelercliexceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:23:40.699066 azureenergylabelercli-2.1.0/azureenergylabelercli/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/conf/logging.json-example
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/azureenergylabelercli/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:23:40.699066 azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:23:40.703066 azureenergylabelercli-2.1.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6822 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9072 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-15 09:23:40.000000 azureenergylabelercli-2.1.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-05-15 09:23:40.703066 azureenergylabelercli-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:23:40.703066 azureenergylabelercli-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-15 09:22:04.000000 azureenergylabelercli-2.1.0/tests/test_azureenergylabelercli.py
```

### Comparing `azureenergylabelercli-2.0.3/CONTRIBUTING.rst` & `azureenergylabelercli-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/HISTORY.rst` & `azureenergylabelercli-2.1.0/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -53,7 +53,14 @@
 * Bump template and dependencies.
 
 
 2.0.3 (21-03-2023)
 ------------------
 
 * Bumped library version which now filters subscriptions based on the tenant_id.
+
+
+2.1.0 (15-05-2023)
+------------------
+
+* Added option to disable banner and spinner
+* Improved filtering of findings
```

### Comparing `azureenergylabelercli-2.0.3/LICENSE` & `azureenergylabelercli-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/PKG-INFO` & `azureenergylabelercli-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureenergylabelercli
-Version: 2.0.3
+Version: 2.1.0
 Summary: A cli to help generate energy label for Azure tenant, subscriptions and resource groups.
 Home-page: https://github.com/schubergphilis/azureenergylabelercli
 Author: Sayantan Khanra
 Author-email: skhanra@schubergphilis.com
 License: MIT
 Keywords: azureenergylabelercli
 Classifier: Development Status :: 1 - Planning
@@ -45,15 +45,15 @@
   :header: "description", "CLI argument", "environment variable", "example value"
 
   "Tenand ID (required)", "`--tenant-id`", "`AZURE_LABELER_TENANT_ID`", "`00000000-0000-0000-0000-000000000000`"
   "Path to export the results", "`--export-path`", "`AZURE_LABELER_EXPORT_PATH`", "`/local/path` or Storage Account Url with SAS token `https://sa.blob.windows.net/container/?sas_token`"
   "Export only number of findings and energy label", "`--export-metrics`", "`AZURE_LABELER_EXPORT_METRICS`", "`false` (default)"
   "Export all findings information along with energy label", "`--export-all`", "`AZURE_LABELER_EXPORT_ALL`", "`true` (default)"
   "Regulatory frameworks to take into account", "`--frameworks`", "`AZURE_LABELER_FRAMEWORKS`", "`'Microsoft cloud security benchmark,Azure CIS 1.1.0'`"
-  "Explicit list of subscriptions to take into account", "`--allowed-subscription-ids`", "`AZURE_LABELER_TENANT_ID`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
+  "Explicit list of subscriptions to take into account", "`--allowed-subscription-ids`", "`AZURE_LABELER_ALLOWED_SUBSCRIPTION_IDS`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
   "Explicit list of subscriptions NOT to take into account", "`--denied-subscription-ids`", "`AZURE_LABELER_DENIED_SUBSCRIPTION_IDS`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
   "Level of log printing", "`--log-level`", "`AZURE_LABELER_LOG_LEVEL`", "`info`"
   "Logging configuration", "`--log-config`", "`AZURE_LABELER_LOG_CONFIG`", ""
 
 
 Supported authentication types
 ==============================
@@ -290,7 +290,14 @@
 * Bump template and dependencies.
 
 
 2.0.3 (21-03-2023)
 ------------------
 
 * Bumped library version which now filters subscriptions based on the tenant_id.
+
+
+2.1.0 (15-05-2023)
+------------------
+
+* Added option to disable banner and spinner
+* Improved filtering of findings
```

### Comparing `azureenergylabelercli-2.0.3/Pipfile` & `azureenergylabelercli-2.1.0/Pipfile`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 twine = ">=4.0,<5.0"
 coloredlogs = ">=15.0,<16.0"
 emoji = ">=2.0,<3.0"
 toml = ">=0.1,<1.0"
 
 [packages]
 coloredlogs = "~=15.0.1"
-azureenergylabelerlib = "~=3.1.1"
+azureenergylabelerlib = "~=3.2.0"
 yaspin = "~=2.3.0"
 terminaltables = "~=3.1.10"
 art = "~=5.8"
 
 [requires]
 python_version = "3.9"
```

### Comparing `azureenergylabelercli-2.0.3/Pipfile.lock` & `azureenergylabelercli-2.1.0/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9742595533373665%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'9ebe67dc8190e1681e4c386e9b6648d3934e593c5b5a41a3af6565836c604dc0'}}",*

 * * "'default'": "{'azure-cli-core': {'hashes': "*

 * *              "['sha256:d70ebe7a59bcb91ab1fdeb5d931a74a04c3def6320bbfdfd506eec18a0de0c3b', "*

 * *              "'sha256:e9300ca40c4f7cb1c95ac29814045d7faa632f5245a9dae99c7545a743893105'], "*

 * *              "'version': '==2.48.1'}, 'azure-core': {'hashes': "*

 * *              "['sha256:075fe06b74c3007950dd93d49440c2f3430fd9b4a5a2756ec8c79454afc989c6', "*

 * *  […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "50da340a6da160f22a0eeb14f84737bd57f4f730e5519636221b1b457ac78dcf"
+            "sha256": "9ebe67dc8190e1681e4c386e9b6648d3934e593c5b5a41a3af6565836c604dc0"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -44,19 +44,19 @@
                 "sha256:9b02463468fc51c77200dadee970cf02c9576008c4f3b99d7ed02371ec037bd1"
             ],
             "index": "pypi",
             "version": "==5.9"
         },
         "azure-cli-core": {
             "hashes": [
-                "sha256:77442f3ee782e43aa46f6a6b0d455a981d085d9d5debe6baac1e2158d10258bd",
-                "sha256:a865351c723a5eb37f51ade24aadcc0c065ce83a422dbe0c02d30b2088c935fa"
+                "sha256:d70ebe7a59bcb91ab1fdeb5d931a74a04c3def6320bbfdfd506eec18a0de0c3b",
+                "sha256:e9300ca40c4f7cb1c95ac29814045d7faa632f5245a9dae99c7545a743893105"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==2.46.0"
+            "version": "==2.48.1"
         },
         "azure-cli-telemetry": {
             "hashes": [
                 "sha256:502cbd90723a16603822909befd096ca0b1707de1e70cf730e7b4700ddd7a456",
                 "sha256:ca996d162ab689c865f6b60be23b9757c26c3d97928e3319858eea83462df08d"
             ],
             "version": "==1.0.8"
@@ -66,75 +66,75 @@
                 "sha256:4ac0cd3214e36b6a1b6a442686722a5d8cc449603aa833f3f0f40bda836704a3",
                 "sha256:5c12d3dcf4ec20599ca6b0d3e09e86e146353d443e7fcc050c9a19c1f9df20ad"
             ],
             "version": "==1.1.28"
         },
         "azure-core": {
             "hashes": [
-                "sha256:acbd0daa9675ce88623da35c80d819cdafa91731dee6b2695c64d7ca9da82db4",
-                "sha256:f7bad0a7b4d800d6e73733ea7e13a616016221ac111ff9a344fe4cba41e51bbe"
+                "sha256:075fe06b74c3007950dd93d49440c2f3430fd9b4a5a2756ec8c79454afc989c6",
+                "sha256:d9664b4bc2675d72fba461a285ac43ae33abb2967014a955bf136d9703a2ab3c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.3"
+            "version": "==1.26.4"
         },
         "azure-identity": {
             "hashes": [
-                "sha256:2a58ce4a209a013e37eaccfd5937570ab99e9118b3e1acf875eed3a85d541b92",
-                "sha256:7f9b1ae7d97ea7af3f38dd09305e19ab81a1e16ab66ea186b6579d85c1ca2347"
+                "sha256:bd700cebb80cd9862098587c29d8677e819beca33c62568ced6d5a8e5e332b82",
+                "sha256:c931c27301ffa86b07b4dcf574e29da73e3deba9ab5d1fe4f445bb6a3117e260"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.12.0"
+            "version": "==1.13.0"
         },
         "azure-mgmt-core": {
             "hashes": [
-                "sha256:07f4afe823a55d704b048d61edfdc1318c051ed59f244032126350be95e9d501",
-                "sha256:fd829f67086e5cf6f7eb016c9e80bb0fb293cbbbd4d8738dc90af9aa1055fb7b"
+                "sha256:81071675f186a585555ef01816f2774d49c1c9024cb76e5720c3c0f6b337bb7d",
+                "sha256:d195208340094f98e5a6661b781cde6f6a051e79ce317caabd8ff97030a9b3ae"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.3.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.4.0"
         },
         "azure-mgmt-resource": {
             "hashes": [
-                "sha256:5c9712aacb230c7dde59cd7b43a734ed88a326140042ae02746d095fe779ae20",
-                "sha256:feb5d979e18b52f2cfd023b4a0a33e54a6f76cc6a252dc8cd75ece2c63298e94"
+                "sha256:b556803a3b8699dbcd1f4c33c8229830225c8c61ba058323d5bae7dc7785d65e",
+                "sha256:e6137abc3244efdecc730feed05b17542ccdaf8735a66b9141ad0a378d872922"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==22.0.0"
+            "version": "==23.0.0"
         },
         "azure-mgmt-resourcegraph": {
             "hashes": [
                 "sha256:0cf55f7ea82dc03e69d0fae0f1606e09b08b80b6ae23bd597d8b62b1ed938ace",
                 "sha256:d25f01dae3897780fb3ddca16d1625b6347c32f1b581c767fba5ef3b24443f11"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.0.0"
         },
         "azure-mgmt-security": {
             "hashes": [
-                "sha256:09d3b822a22fa0252ee2d95f238a889cbdf4afcef1b663826c313897f504e6a6",
-                "sha256:551102127f2b798c1a373003e8877fbe78e58c5d3e04e875805b06d6facea8e7"
+                "sha256:38b03efe82c2344cea203fda95e6d00b7ac22782fa1c0b585cd0ea2c8ff3e702",
+                "sha256:73a74ce8f6ffb1b345ce101c8abdd42238f161f0988d168d23918feda0089654"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.0.0"
+            "version": "==5.0.0"
         },
         "azure-storage-blob": {
             "hashes": [
-                "sha256:08d8807c577c63a436740627927c1a03a97c963efc29af5c818aed906590e1cf",
-                "sha256:f8b8d582492740ab16744455408342fb8e4c8897b64a8a3fc31743844722c2f2"
+                "sha256:43b45f19a518a5c6895632f263b3825ebc23574f25cc84b66e1630a6160e466f",
+                "sha256:91bb192b2a97939c4259c72373bac0f41e30810bbc853d5184f0f45904eacafd"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==12.15.0"
+            "version": "==12.16.0"
         },
         "azureenergylabelerlib": {
             "hashes": [
-                "sha256:0c16a9fdd91d761299ab4e6d30aeede7cfb5004b70e7dee7b4fea0b6b5869afe",
-                "sha256:6606e8494c77576338ca4c8eb50888b06179d2d655ffc257d73b787982a5a25e"
+                "sha256:d7197b14424bd3745def7fabb60338891c49f210b79e1a425b912d393f51c389",
+                "sha256:df0fcec873b7978da6bb55af83017ddb40d0d99842f77ac337687fd3338cad13"
             ],
             "index": "pypi",
-            "version": "==3.1.1"
+            "version": "==3.2.0"
         },
         "bcrypt": {
             "hashes": [
                 "sha256:089098effa1bc35dc055366740a067a2fc76987e8ec75349eb9484061c54f535",
                 "sha256:08d2947c490093a11416df18043c27abe3921558d2c03e2076ccb28a116cb6d0",
                 "sha256:0eaa47d4661c326bfc9d08d16debbc4edf78778e6aaba29c1bc7ce67214d4410",
                 "sha256:27d375903ac8261cfe4047f6709d16f7d18d39b1ec92aaf72af989552a650ebd",
@@ -165,19 +165,19 @@
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
             "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -339,40 +339,36 @@
                 "sha256:ab1e2bfe1d01d968e1b7e8d9023bc51ef3509bba217bb730cee3827e1ee82869"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==21.6.0"
         },
         "cryptography": {
             "hashes": [
-                "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1",
-                "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7",
-                "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06",
-                "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84",
-                "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915",
-                "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074",
-                "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5",
-                "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3",
-                "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9",
-                "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3",
-                "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011",
-                "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536",
-                "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a",
-                "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f",
-                "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480",
-                "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac",
-                "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0",
-                "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108",
-                "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828",
-                "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354",
-                "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612",
-                "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3",
-                "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.2"
+            "version": "==40.0.2"
         },
         "distro": {
             "hashes": [
                 "sha256:02e111d1dc6a50abb8eed6bf31c3e48ed8b0830d1ea2a1b78c61765c2513fdd8",
                 "sha256:99522ca3e365cac527b44bde033f64c6945d90eb9f769703caaec52b09bbd3ff"
             ],
             "markers": "sys_platform == 'linux'",
@@ -454,27 +450,27 @@
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.2.2"
         },
         "opnieuw": {
             "hashes": [
-                "sha256:2db9230af2146129194af549f7f7c5fb692caa681caf12fe9a81518e2a66d5cf",
-                "sha256:c2784d342af982f3197637207001d7b3025ca0129101fd1c5014cdcfaf10edf4"
+                "sha256:97aa118848261ca58b4375d8b197d975990888715a33cb28e47ca4ccab80da60",
+                "sha256:b864fc258da6722a47ae037ef15e438b165909c2b90b697dee3fb04b2c7c13d7"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.2.0"
+            "version": "==2.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "paramiko": {
             "hashes": [
                 "sha256:6950faca6819acd3219d4ae694a23c7a87ee38d084f70c1724b0c0dbb8b75769",
                 "sha256:f0caa660e797d9cd10db6fc6ae81e2c9b2767af75c3180fcd0e46158cd368d7f"
             ],
             "markers": "python_version >= '3.6'",
@@ -494,54 +490,54 @@
                 "sha256:a07c5b4f3985c3cf4798369631fb7011adb498e2a46d8440efc75a8f29a0f983"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==2.7.0"
         },
         "psutil": {
             "hashes": [
-                "sha256:149555f59a69b33f056ba1c4eb22bb7bf24332ce631c44a319cec09f876aaeff",
-                "sha256:16653106f3b59386ffe10e0bad3bb6299e169d5327d3f187614b1cb8f24cf2e1",
-                "sha256:3d7f9739eb435d4b1338944abe23f49584bde5395f27487d2ee25ad9a8774a62",
-                "sha256:3ff89f9b835100a825b14c2808a106b6fdcc4b15483141482a12c725e7f78549",
-                "sha256:54c0d3d8e0078b7666984e11b12b88af2db11d11249a8ac8920dd5ef68a66e08",
-                "sha256:54d5b184728298f2ca8567bf83c422b706200bcbbfafdc06718264f9393cfeb7",
-                "sha256:6001c809253a29599bc0dfd5179d9f8a5779f9dffea1da0f13c53ee568115e1e",
-                "sha256:68908971daf802203f3d37e78d3f8831b6d1014864d7a85937941bb35f09aefe",
-                "sha256:6b92c532979bafc2df23ddc785ed116fced1f492ad90a6830cf24f4d1ea27d24",
-                "sha256:852dd5d9f8a47169fe62fd4a971aa07859476c2ba22c2254d4a1baa4e10b95ad",
-                "sha256:9120cd39dca5c5e1c54b59a41d205023d436799b1c8c4d3ff71af18535728e94",
-                "sha256:c1ca331af862803a42677c120aff8a814a804e09832f166f226bfd22b56feee8",
-                "sha256:efeae04f9516907be44904cc7ce08defb6b665128992a56957abc9b61dca94b7",
-                "sha256:fd8522436a6ada7b4aad6638662966de0d61d241cb821239b2ae7013d41a43d4"
+                "sha256:104a5cc0e31baa2bcf67900be36acde157756b9c44017b86b2c049f11957887d",
+                "sha256:3c6f686f4225553615612f6d9bc21f1c0e305f75d7d8454f9b46e901778e7217",
+                "sha256:4aef137f3345082a3d3232187aeb4ac4ef959ba3d7c10c33dd73763fbc063da4",
+                "sha256:5410638e4df39c54d957fc51ce03048acd8e6d60abc0f5107af51e5fb566eb3c",
+                "sha256:5b9b8cb93f507e8dbaf22af6a2fd0ccbe8244bf30b1baad6b3954e935157ae3f",
+                "sha256:7a7dd9997128a0d928ed4fb2c2d57e5102bb6089027939f3b722f3a210f9a8da",
+                "sha256:89518112647f1276b03ca97b65cc7f64ca587b1eb0278383017c2a0dcc26cbe4",
+                "sha256:8c5f7c5a052d1d567db4ddd231a9d27a74e8e4a9c3f44b1032762bd7b9fdcd42",
+                "sha256:ab8ed1a1d77c95453db1ae00a3f9c50227ebd955437bcf2a574ba8adbf6a74d5",
+                "sha256:acf2aef9391710afded549ff602b5887d7a2349831ae4c26be7c807c0a39fac4",
+                "sha256:b258c0c1c9d145a1d5ceffab1134441c4c5113b2417fafff7315a917a026c3c9",
+                "sha256:be8929ce4313f9f8146caad4272f6abb8bf99fc6cf59344a3167ecd74f4f203f",
+                "sha256:c607bb3b57dc779d55e1554846352b4e358c10fff3abf3514a7a6601beebdb30",
+                "sha256:ea8518d152174e1249c4f2a1c89e3e6065941df2fa13a1ab45327716a23c2b48"
             ],
             "markers": "sys_platform != 'cygwin'",
-            "version": "==5.9.4"
+            "version": "==5.9.5"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pyjwt": {
             "hashes": [
-                "sha256:69285c7e31fc44f68a1feb309e948e0df53259d579295e6cfe2b1792329f05fd",
-                "sha256:d83c3d892a77bbb74d3e1a2cfa90afaadb60945205d1095d9221f04466f64c14"
+                "sha256:ba2b425b15ad5ef12f200dc67dd56af4e26de2331f965c5439994dad075876e1",
+                "sha256:bd6ca4a3c4285c1a2d4349e5a035fdf8fb94e04ccd0fcbe6ba289dae9cc3e074"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.0"
+            "version": "==2.7.0"
         },
         "pynacl": {
             "hashes": [
                 "sha256:06b8f6fa7f5de8d5d2f7573fe8c863c051225a27b61e6860fd047b1775807858",
                 "sha256:0c84947a22519e013607c9be43706dd42513f9e6ae5d39d3613ca1e142fba44d",
                 "sha256:20f42270d27e1b6a29f54032090b972d97f0a1b0948cc52392041ef7831fee93",
                 "sha256:401002a4aaa07c9414132aaed7f6836ff98f59277a234704ff66878c2ee4a0d1",
@@ -553,19 +549,19 @@
                 "sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.5.0"
         },
         "pyopenssl": {
             "hashes": [
-                "sha256:c1cc5f86bcacefc84dada7d31175cae1b1518d5f60d3d0bb595a67822a868a6f",
-                "sha256:df5fc28af899e74e19fccb5510df423581047e10ab6f1f4ba1763ff5fde844c0"
+                "sha256:841498b9bec61623b1b6c47ebbc02367c07d60e0e195f19790817f10cc8db0b7",
+                "sha256:9e0c526404a210df9d2b18cd33364beadb0dc858a739b885677bc65e105d4a4c"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==23.0.0"
+            "version": "==23.1.1"
         },
         "pysocks": {
             "hashes": [
                 "sha256:08e69f092cc6dbe92a0fdd16eeb9b9ffbc13cadfe5ca4c7bd92ffb078b293299",
                 "sha256:2725bd0a9925919b9b51739eea5f9e2bae91e83288108a9ad338b2e3a4435ee5",
                 "sha256:3f8804571ebe159c380ac6de37643bb4685970655d3bba243530d6558b799aa0"
             ],
@@ -626,19 +622,19 @@
             "version": "==6.0"
         },
         "requests": {
             "extras": [
                 "socks"
             ],
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.30.0"
         },
         "requests-oauthlib": {
             "hashes": [
                 "sha256:2577c501a2fb8d05a304c09d090d6e47c306fef15809d102b327cf8364bddab5",
                 "sha256:75beac4a47881eeb94d5ea5d6ad31ef88856affe2332b9aafb52c6452ccf0d7a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -665,19 +661,19 @@
                 "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.9.0"
         },
         "termcolor": {
             "hashes": [
-                "sha256:91ddd848e7251200eac969846cbae2dacd7d71c2871e92733289e7e3666f48e7",
-                "sha256:dfc8ac3f350788f23b2947b3e6cfa5a53b630b612e6cd8965a015a776020b99a"
+                "sha256:3afb05607b89aed0ffe25202399ee0867ad4d3cb4180d98aaf8eefa6a5f7d475",
+                "sha256:b5b08f68937f138fe92f6c089b99f1e2da0ae56c52b78bf7075fd95420fd9a5a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "version": "==2.3.0"
         },
         "terminaltables": {
             "hashes": [
                 "sha256:ba6eca5cb5ba02bba4c9f4f985af80c54ec3dccf94cfcd190154386255e47543",
                 "sha256:e4fdc4179c9e4aab5f674d80f09d76fa436b96fdc698a8505e0a36bf0804a874"
             ],
             "index": "pypi",
@@ -689,19 +685,19 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "yaspin": {
             "hashes": [
                 "sha256:17b5548479b3d5b30adec7a87ffcdcddb403d14a2bb86fbcee97f37951e13427",
                 "sha256:547afd1a9700ac3a29a9f5591c70343bef186ed5dfb5e545a9bb0c77e561a1c9"
             ],
             "index": "pypi",
@@ -715,19 +711,19 @@
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:525f126d5dc1b8b0b6ee398b33159105615d92dc4a17f2cd064125d57f6186fa",
-                "sha256:e3e4d0ffc2d15d954065579689c36aac57a339a4679a679579af6401db4d3fdb"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.0"
+            "version": "==2.15.5"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -763,19 +759,19 @@
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
             "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -945,97 +941,93 @@
                 "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
             "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
-                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
-                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
-                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
-                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
-                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
-                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
-                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
-                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
-                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
-                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
-                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
-                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
-                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
-                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
-                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
-                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
-                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
-                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
-                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
-                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
-                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
-                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
-                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
-                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
-                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
-                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
-                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
-                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
-                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
-                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
-                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
-                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
-                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
-                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
-                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
-                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
-                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
-                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
-                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
-                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
-                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
-                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
-                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
-                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
-                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
-                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
-                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
-                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
-                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
-                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
+                "sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3",
+                "sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a",
+                "sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813",
+                "sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0",
+                "sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a",
+                "sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd",
+                "sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139",
+                "sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b",
+                "sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252",
+                "sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790",
+                "sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045",
+                "sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce",
+                "sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200",
+                "sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718",
+                "sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b",
+                "sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f",
+                "sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5",
+                "sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade",
+                "sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5",
+                "sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a",
+                "sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8",
+                "sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33",
+                "sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e",
+                "sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c",
+                "sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3",
+                "sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969",
+                "sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068",
+                "sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2",
+                "sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771",
+                "sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed",
+                "sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212",
+                "sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614",
+                "sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88",
+                "sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3",
+                "sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c",
+                "sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84",
+                "sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11",
+                "sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1",
+                "sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1",
+                "sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e",
+                "sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1",
+                "sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd",
+                "sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47",
+                "sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a",
+                "sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c",
+                "sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31",
+                "sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5",
+                "sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6",
+                "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
+                "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
+                "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
             ],
             "index": "pypi",
-            "version": "==7.2.2"
+            "version": "==7.2.5"
         },
         "cryptography": {
             "hashes": [
-                "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1",
-                "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7",
-                "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06",
-                "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84",
-                "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915",
-                "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074",
-                "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5",
-                "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3",
-                "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9",
-                "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3",
-                "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011",
-                "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536",
-                "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a",
-                "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f",
-                "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480",
-                "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac",
-                "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0",
-                "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108",
-                "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828",
-                "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354",
-                "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612",
-                "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3",
-                "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.2"
+            "version": "==40.0.2"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
@@ -1068,19 +1060,19 @@
                 "sha256:a2986c21e4aba6b9870df40ef487a17be863cb7778dcf1c01e25917b7cd210bb"
             ],
             "index": "pypi",
             "version": "==2.2.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:3199fd0d3faea8b911be52b663dfccceb84c95949dd13179aa21436d1a79c4ce",
-                "sha256:e90b34656470756edf8b19656785c5fea73afa1953f3e1b0d645cef11cab3182"
+                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
+                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.0"
+            "version": "==3.12.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
                 "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -1139,19 +1131,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20",
-                "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==6.1.0"
+            "version": "==6.6.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
             "markers": "python_full_version >= '3.8.0'",
@@ -1334,19 +1326,19 @@
                 "sha256:ab2d0dca21aa5a7ae280c6fb869882260b825d9ced368b557b9124cf51ffb119"
             ],
             "index": "pypi",
             "version": "==0.6.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pep8-naming": {
             "hashes": [
                 "sha256:5d9f1056cb9427ce344e98d1a7f5665710e2f20f748438e308995852cfa24164",
                 "sha256:f3b4a5f9dd72b991bf7d8e2a341d2e1aa3a884a769b5aaac4f56825c1763bf3a"
             ],
             "version": "==0.10.0"
@@ -1357,19 +1349,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa",
-                "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.1"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -1420,27 +1412,27 @@
                 "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.5.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pylint": {
             "hashes": [
-                "sha256:1460829b6397cb5eb0cdb0b4fc4b556348e515cdca32115f74a1eb7c20b896b4",
-                "sha256:e097d8325f8c88e14ad12844e3fe2d963d3de871ea9a8f8ad25ab1c109889ddc"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.17.0"
+            "version": "==2.17.4"
         },
         "pylint-celery": {
             "hashes": [
                 "sha256:41e32094e7408d15c044178ea828dd524beedbdbe6f83f712c5e35bde1de4beb"
             ],
             "version": "==0.3"
         },
@@ -1528,27 +1520,27 @@
             "version": "==37.3"
         },
         "requests": {
             "extras": [
                 "socks"
             ],
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.30.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "requirements-detector": {
             "hashes": [
                 "sha256:246bd23867c12061eadb346a6fe2e616f0b64e681936154a76c494a27cda3ea8",
                 "sha256:9af62db621c95e0176fed029079924e648de22cd0bb4189c441b9376942faab1"
             ],
             "markers": "python_version >= '3.7' and python_version < '4.0'",
@@ -1560,19 +1552,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:91954fe80cfb7985727a467ca98a7618e5dd15178cc2da10f553b36a93859001",
-                "sha256:a104f37270bf677148d8acb07d33be1569eeee87e2d1beb286a4e9113caf6f2f"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.2"
+            "version": "==13.3.5"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
@@ -1622,19 +1614,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2",
-                "sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc"
+                "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b",
+                "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
             "index": "pypi",
-            "version": "==6.1.3"
+            "version": "==6.2.1"
         },
         "sphinx-rtd-theme": {
             "hashes": [
                 "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
                 "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
             ],
             "index": "pypi",
@@ -1710,19 +1702,19 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.8"
         },
         "tox": {
             "hashes": [
                 "sha256:17643b0e29c41f784c9c266a13302dc0604884b9ceff6686fbb31bada4a7aa3a",
                 "sha256:e6adcebddfec5e456e5d2884f82b9468e38c4ec6439ec97f7f1fb85d5b1bf846"
             ],
             "index": "pypi",
@@ -1742,27 +1734,27 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
-                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.21.0"
+            "version": "==20.23.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `azureenergylabelercli-2.0.3/README.rst` & `azureenergylabelercli-2.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   :header: "description", "CLI argument", "environment variable", "example value"
 
   "Tenand ID (required)", "`--tenant-id`", "`AZURE_LABELER_TENANT_ID`", "`00000000-0000-0000-0000-000000000000`"
   "Path to export the results", "`--export-path`", "`AZURE_LABELER_EXPORT_PATH`", "`/local/path` or Storage Account Url with SAS token `https://sa.blob.windows.net/container/?sas_token`"
   "Export only number of findings and energy label", "`--export-metrics`", "`AZURE_LABELER_EXPORT_METRICS`", "`false` (default)"
   "Export all findings information along with energy label", "`--export-all`", "`AZURE_LABELER_EXPORT_ALL`", "`true` (default)"
   "Regulatory frameworks to take into account", "`--frameworks`", "`AZURE_LABELER_FRAMEWORKS`", "`'Microsoft cloud security benchmark,Azure CIS 1.1.0'`"
-  "Explicit list of subscriptions to take into account", "`--allowed-subscription-ids`", "`AZURE_LABELER_TENANT_ID`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
+  "Explicit list of subscriptions to take into account", "`--allowed-subscription-ids`", "`AZURE_LABELER_ALLOWED_SUBSCRIPTION_IDS`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
   "Explicit list of subscriptions NOT to take into account", "`--denied-subscription-ids`", "`AZURE_LABELER_DENIED_SUBSCRIPTION_IDS`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
   "Level of log printing", "`--log-level`", "`AZURE_LABELER_LOG_LEVEL`", "`info`"
   "Logging configuration", "`--log-config`", "`AZURE_LABELER_LOG_CONFIG`", ""
 
 
 Supported authentication types
 ==============================
```

### Comparing `azureenergylabelercli-2.0.3/USAGE.rst` & `azureenergylabelercli-2.1.0/USAGE.rst`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azure_energy_labeler_cli.py` & `azureenergylabelercli-2.1.0/azure_energy_labeler_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 LOGGER.addHandler(logging.NullHandler())
 
 
 def _get_reporting_arguments(args):
     method_arguments = {'export_all_data_flag': args.export_all,
                         'tenant_id': args.tenant_id,
                         'frameworks': args.frameworks,
-                        'log_level': args.log_level}
+                        'log_level': args.log_level,
+                        'disable_spinner': args.disable_spinner}
     if args.single_subscription_id:
         get_reporting_data = get_subscription_reporting_data
         method_arguments.update({'subscription_id': args.single_subscription_id})
     else:
         get_reporting_data = get_tenant_reporting_data
         method_arguments.update({'allowed_subscription_ids': args.allowed_subscription_ids,
                                  'denied_subscription_ids': args.denied_subscription_ids})
@@ -87,15 +88,16 @@
 
 def main():
     """Main method."""
     args = get_arguments()
     setup_logging(args.log_level, args.logger_config)
     logging.getLogger('botocore').setLevel(logging.ERROR)
     try:
-        print(text2art("Azure Energy Labeler"))
+        if not args.disable_banner:
+            print(text2art("Azure Energy Labeler"))
         report_data, exporter_arguments = _get_reporting_arguments(args)
         if args.export_path:
             LOGGER.info(f'Trying to export data to the requested path : {args.export_path}')
             exporter = DataExporter(**exporter_arguments)
             exporter.export(args.export_path)
         report(report_data, args.to_json)
     except Exception as msg:
```

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/CONTRIBUTING.rst` & `azureenergylabelercli-2.1.0/azureenergylabelercli/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/HISTORY.rst` & `azureenergylabelercli-2.1.0/azureenergylabelercli/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -53,7 +53,14 @@
 * Bump template and dependencies.
 
 
 2.0.3 (21-03-2023)
 ------------------
 
 * Bumped library version which now filters subscriptions based on the tenant_id.
+
+
+2.1.0 (15-05-2023)
+------------------
+
+* Added option to disable banner and spinner
+* Improved filtering of findings
```

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/LICENSE` & `azureenergylabelercli-2.1.0/azureenergylabelercli/LICENSE`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/Pipfile` & `azureenergylabelercli-2.1.0/azureenergylabelercli/Pipfile`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 twine = ">=4.0,<5.0"
 coloredlogs = ">=15.0,<16.0"
 emoji = ">=2.0,<3.0"
 toml = ">=0.1,<1.0"
 
 [packages]
 coloredlogs = "~=15.0.1"
-azureenergylabelerlib = "~=3.1.1"
+azureenergylabelerlib = "~=3.2.0"
 yaspin = "~=2.3.0"
 terminaltables = "~=3.1.10"
 art = "~=5.8"
 
 [requires]
 python_version = "3.9"
```

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/Pipfile.lock` & `azureenergylabelercli-2.1.0/azureenergylabelercli/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9742595533373665%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'9ebe67dc8190e1681e4c386e9b6648d3934e593c5b5a41a3af6565836c604dc0'}}",*

 * * "'default'": "{'azure-cli-core': {'hashes': "*

 * *              "['sha256:d70ebe7a59bcb91ab1fdeb5d931a74a04c3def6320bbfdfd506eec18a0de0c3b', "*

 * *              "'sha256:e9300ca40c4f7cb1c95ac29814045d7faa632f5245a9dae99c7545a743893105'], "*

 * *              "'version': '==2.48.1'}, 'azure-core': {'hashes': "*

 * *              "['sha256:075fe06b74c3007950dd93d49440c2f3430fd9b4a5a2756ec8c79454afc989c6', "*

 * *  […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "50da340a6da160f22a0eeb14f84737bd57f4f730e5519636221b1b457ac78dcf"
+            "sha256": "9ebe67dc8190e1681e4c386e9b6648d3934e593c5b5a41a3af6565836c604dc0"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -44,19 +44,19 @@
                 "sha256:9b02463468fc51c77200dadee970cf02c9576008c4f3b99d7ed02371ec037bd1"
             ],
             "index": "pypi",
             "version": "==5.9"
         },
         "azure-cli-core": {
             "hashes": [
-                "sha256:77442f3ee782e43aa46f6a6b0d455a981d085d9d5debe6baac1e2158d10258bd",
-                "sha256:a865351c723a5eb37f51ade24aadcc0c065ce83a422dbe0c02d30b2088c935fa"
+                "sha256:d70ebe7a59bcb91ab1fdeb5d931a74a04c3def6320bbfdfd506eec18a0de0c3b",
+                "sha256:e9300ca40c4f7cb1c95ac29814045d7faa632f5245a9dae99c7545a743893105"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==2.46.0"
+            "version": "==2.48.1"
         },
         "azure-cli-telemetry": {
             "hashes": [
                 "sha256:502cbd90723a16603822909befd096ca0b1707de1e70cf730e7b4700ddd7a456",
                 "sha256:ca996d162ab689c865f6b60be23b9757c26c3d97928e3319858eea83462df08d"
             ],
             "version": "==1.0.8"
@@ -66,75 +66,75 @@
                 "sha256:4ac0cd3214e36b6a1b6a442686722a5d8cc449603aa833f3f0f40bda836704a3",
                 "sha256:5c12d3dcf4ec20599ca6b0d3e09e86e146353d443e7fcc050c9a19c1f9df20ad"
             ],
             "version": "==1.1.28"
         },
         "azure-core": {
             "hashes": [
-                "sha256:acbd0daa9675ce88623da35c80d819cdafa91731dee6b2695c64d7ca9da82db4",
-                "sha256:f7bad0a7b4d800d6e73733ea7e13a616016221ac111ff9a344fe4cba41e51bbe"
+                "sha256:075fe06b74c3007950dd93d49440c2f3430fd9b4a5a2756ec8c79454afc989c6",
+                "sha256:d9664b4bc2675d72fba461a285ac43ae33abb2967014a955bf136d9703a2ab3c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.3"
+            "version": "==1.26.4"
         },
         "azure-identity": {
             "hashes": [
-                "sha256:2a58ce4a209a013e37eaccfd5937570ab99e9118b3e1acf875eed3a85d541b92",
-                "sha256:7f9b1ae7d97ea7af3f38dd09305e19ab81a1e16ab66ea186b6579d85c1ca2347"
+                "sha256:bd700cebb80cd9862098587c29d8677e819beca33c62568ced6d5a8e5e332b82",
+                "sha256:c931c27301ffa86b07b4dcf574e29da73e3deba9ab5d1fe4f445bb6a3117e260"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.12.0"
+            "version": "==1.13.0"
         },
         "azure-mgmt-core": {
             "hashes": [
-                "sha256:07f4afe823a55d704b048d61edfdc1318c051ed59f244032126350be95e9d501",
-                "sha256:fd829f67086e5cf6f7eb016c9e80bb0fb293cbbbd4d8738dc90af9aa1055fb7b"
+                "sha256:81071675f186a585555ef01816f2774d49c1c9024cb76e5720c3c0f6b337bb7d",
+                "sha256:d195208340094f98e5a6661b781cde6f6a051e79ce317caabd8ff97030a9b3ae"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.3.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.4.0"
         },
         "azure-mgmt-resource": {
             "hashes": [
-                "sha256:5c9712aacb230c7dde59cd7b43a734ed88a326140042ae02746d095fe779ae20",
-                "sha256:feb5d979e18b52f2cfd023b4a0a33e54a6f76cc6a252dc8cd75ece2c63298e94"
+                "sha256:b556803a3b8699dbcd1f4c33c8229830225c8c61ba058323d5bae7dc7785d65e",
+                "sha256:e6137abc3244efdecc730feed05b17542ccdaf8735a66b9141ad0a378d872922"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==22.0.0"
+            "version": "==23.0.0"
         },
         "azure-mgmt-resourcegraph": {
             "hashes": [
                 "sha256:0cf55f7ea82dc03e69d0fae0f1606e09b08b80b6ae23bd597d8b62b1ed938ace",
                 "sha256:d25f01dae3897780fb3ddca16d1625b6347c32f1b581c767fba5ef3b24443f11"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.0.0"
         },
         "azure-mgmt-security": {
             "hashes": [
-                "sha256:09d3b822a22fa0252ee2d95f238a889cbdf4afcef1b663826c313897f504e6a6",
-                "sha256:551102127f2b798c1a373003e8877fbe78e58c5d3e04e875805b06d6facea8e7"
+                "sha256:38b03efe82c2344cea203fda95e6d00b7ac22782fa1c0b585cd0ea2c8ff3e702",
+                "sha256:73a74ce8f6ffb1b345ce101c8abdd42238f161f0988d168d23918feda0089654"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.0.0"
+            "version": "==5.0.0"
         },
         "azure-storage-blob": {
             "hashes": [
-                "sha256:08d8807c577c63a436740627927c1a03a97c963efc29af5c818aed906590e1cf",
-                "sha256:f8b8d582492740ab16744455408342fb8e4c8897b64a8a3fc31743844722c2f2"
+                "sha256:43b45f19a518a5c6895632f263b3825ebc23574f25cc84b66e1630a6160e466f",
+                "sha256:91bb192b2a97939c4259c72373bac0f41e30810bbc853d5184f0f45904eacafd"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==12.15.0"
+            "version": "==12.16.0"
         },
         "azureenergylabelerlib": {
             "hashes": [
-                "sha256:0c16a9fdd91d761299ab4e6d30aeede7cfb5004b70e7dee7b4fea0b6b5869afe",
-                "sha256:6606e8494c77576338ca4c8eb50888b06179d2d655ffc257d73b787982a5a25e"
+                "sha256:d7197b14424bd3745def7fabb60338891c49f210b79e1a425b912d393f51c389",
+                "sha256:df0fcec873b7978da6bb55af83017ddb40d0d99842f77ac337687fd3338cad13"
             ],
             "index": "pypi",
-            "version": "==3.1.1"
+            "version": "==3.2.0"
         },
         "bcrypt": {
             "hashes": [
                 "sha256:089098effa1bc35dc055366740a067a2fc76987e8ec75349eb9484061c54f535",
                 "sha256:08d2947c490093a11416df18043c27abe3921558d2c03e2076ccb28a116cb6d0",
                 "sha256:0eaa47d4661c326bfc9d08d16debbc4edf78778e6aaba29c1bc7ce67214d4410",
                 "sha256:27d375903ac8261cfe4047f6709d16f7d18d39b1ec92aaf72af989552a650ebd",
@@ -165,19 +165,19 @@
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
             "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -339,40 +339,36 @@
                 "sha256:ab1e2bfe1d01d968e1b7e8d9023bc51ef3509bba217bb730cee3827e1ee82869"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==21.6.0"
         },
         "cryptography": {
             "hashes": [
-                "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1",
-                "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7",
-                "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06",
-                "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84",
-                "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915",
-                "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074",
-                "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5",
-                "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3",
-                "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9",
-                "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3",
-                "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011",
-                "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536",
-                "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a",
-                "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f",
-                "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480",
-                "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac",
-                "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0",
-                "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108",
-                "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828",
-                "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354",
-                "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612",
-                "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3",
-                "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.2"
+            "version": "==40.0.2"
         },
         "distro": {
             "hashes": [
                 "sha256:02e111d1dc6a50abb8eed6bf31c3e48ed8b0830d1ea2a1b78c61765c2513fdd8",
                 "sha256:99522ca3e365cac527b44bde033f64c6945d90eb9f769703caaec52b09bbd3ff"
             ],
             "markers": "sys_platform == 'linux'",
@@ -454,27 +450,27 @@
                 "sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.2.2"
         },
         "opnieuw": {
             "hashes": [
-                "sha256:2db9230af2146129194af549f7f7c5fb692caa681caf12fe9a81518e2a66d5cf",
-                "sha256:c2784d342af982f3197637207001d7b3025ca0129101fd1c5014cdcfaf10edf4"
+                "sha256:97aa118848261ca58b4375d8b197d975990888715a33cb28e47ca4ccab80da60",
+                "sha256:b864fc258da6722a47ae037ef15e438b165909c2b90b697dee3fb04b2c7c13d7"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.2.0"
+            "version": "==2.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "paramiko": {
             "hashes": [
                 "sha256:6950faca6819acd3219d4ae694a23c7a87ee38d084f70c1724b0c0dbb8b75769",
                 "sha256:f0caa660e797d9cd10db6fc6ae81e2c9b2767af75c3180fcd0e46158cd368d7f"
             ],
             "markers": "python_version >= '3.6'",
@@ -494,54 +490,54 @@
                 "sha256:a07c5b4f3985c3cf4798369631fb7011adb498e2a46d8440efc75a8f29a0f983"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==2.7.0"
         },
         "psutil": {
             "hashes": [
-                "sha256:149555f59a69b33f056ba1c4eb22bb7bf24332ce631c44a319cec09f876aaeff",
-                "sha256:16653106f3b59386ffe10e0bad3bb6299e169d5327d3f187614b1cb8f24cf2e1",
-                "sha256:3d7f9739eb435d4b1338944abe23f49584bde5395f27487d2ee25ad9a8774a62",
-                "sha256:3ff89f9b835100a825b14c2808a106b6fdcc4b15483141482a12c725e7f78549",
-                "sha256:54c0d3d8e0078b7666984e11b12b88af2db11d11249a8ac8920dd5ef68a66e08",
-                "sha256:54d5b184728298f2ca8567bf83c422b706200bcbbfafdc06718264f9393cfeb7",
-                "sha256:6001c809253a29599bc0dfd5179d9f8a5779f9dffea1da0f13c53ee568115e1e",
-                "sha256:68908971daf802203f3d37e78d3f8831b6d1014864d7a85937941bb35f09aefe",
-                "sha256:6b92c532979bafc2df23ddc785ed116fced1f492ad90a6830cf24f4d1ea27d24",
-                "sha256:852dd5d9f8a47169fe62fd4a971aa07859476c2ba22c2254d4a1baa4e10b95ad",
-                "sha256:9120cd39dca5c5e1c54b59a41d205023d436799b1c8c4d3ff71af18535728e94",
-                "sha256:c1ca331af862803a42677c120aff8a814a804e09832f166f226bfd22b56feee8",
-                "sha256:efeae04f9516907be44904cc7ce08defb6b665128992a56957abc9b61dca94b7",
-                "sha256:fd8522436a6ada7b4aad6638662966de0d61d241cb821239b2ae7013d41a43d4"
+                "sha256:104a5cc0e31baa2bcf67900be36acde157756b9c44017b86b2c049f11957887d",
+                "sha256:3c6f686f4225553615612f6d9bc21f1c0e305f75d7d8454f9b46e901778e7217",
+                "sha256:4aef137f3345082a3d3232187aeb4ac4ef959ba3d7c10c33dd73763fbc063da4",
+                "sha256:5410638e4df39c54d957fc51ce03048acd8e6d60abc0f5107af51e5fb566eb3c",
+                "sha256:5b9b8cb93f507e8dbaf22af6a2fd0ccbe8244bf30b1baad6b3954e935157ae3f",
+                "sha256:7a7dd9997128a0d928ed4fb2c2d57e5102bb6089027939f3b722f3a210f9a8da",
+                "sha256:89518112647f1276b03ca97b65cc7f64ca587b1eb0278383017c2a0dcc26cbe4",
+                "sha256:8c5f7c5a052d1d567db4ddd231a9d27a74e8e4a9c3f44b1032762bd7b9fdcd42",
+                "sha256:ab8ed1a1d77c95453db1ae00a3f9c50227ebd955437bcf2a574ba8adbf6a74d5",
+                "sha256:acf2aef9391710afded549ff602b5887d7a2349831ae4c26be7c807c0a39fac4",
+                "sha256:b258c0c1c9d145a1d5ceffab1134441c4c5113b2417fafff7315a917a026c3c9",
+                "sha256:be8929ce4313f9f8146caad4272f6abb8bf99fc6cf59344a3167ecd74f4f203f",
+                "sha256:c607bb3b57dc779d55e1554846352b4e358c10fff3abf3514a7a6601beebdb30",
+                "sha256:ea8518d152174e1249c4f2a1c89e3e6065941df2fa13a1ab45327716a23c2b48"
             ],
             "markers": "sys_platform != 'cygwin'",
-            "version": "==5.9.4"
+            "version": "==5.9.5"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pyjwt": {
             "hashes": [
-                "sha256:69285c7e31fc44f68a1feb309e948e0df53259d579295e6cfe2b1792329f05fd",
-                "sha256:d83c3d892a77bbb74d3e1a2cfa90afaadb60945205d1095d9221f04466f64c14"
+                "sha256:ba2b425b15ad5ef12f200dc67dd56af4e26de2331f965c5439994dad075876e1",
+                "sha256:bd6ca4a3c4285c1a2d4349e5a035fdf8fb94e04ccd0fcbe6ba289dae9cc3e074"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.0"
+            "version": "==2.7.0"
         },
         "pynacl": {
             "hashes": [
                 "sha256:06b8f6fa7f5de8d5d2f7573fe8c863c051225a27b61e6860fd047b1775807858",
                 "sha256:0c84947a22519e013607c9be43706dd42513f9e6ae5d39d3613ca1e142fba44d",
                 "sha256:20f42270d27e1b6a29f54032090b972d97f0a1b0948cc52392041ef7831fee93",
                 "sha256:401002a4aaa07c9414132aaed7f6836ff98f59277a234704ff66878c2ee4a0d1",
@@ -553,19 +549,19 @@
                 "sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.5.0"
         },
         "pyopenssl": {
             "hashes": [
-                "sha256:c1cc5f86bcacefc84dada7d31175cae1b1518d5f60d3d0bb595a67822a868a6f",
-                "sha256:df5fc28af899e74e19fccb5510df423581047e10ab6f1f4ba1763ff5fde844c0"
+                "sha256:841498b9bec61623b1b6c47ebbc02367c07d60e0e195f19790817f10cc8db0b7",
+                "sha256:9e0c526404a210df9d2b18cd33364beadb0dc858a739b885677bc65e105d4a4c"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==23.0.0"
+            "version": "==23.1.1"
         },
         "pysocks": {
             "hashes": [
                 "sha256:08e69f092cc6dbe92a0fdd16eeb9b9ffbc13cadfe5ca4c7bd92ffb078b293299",
                 "sha256:2725bd0a9925919b9b51739eea5f9e2bae91e83288108a9ad338b2e3a4435ee5",
                 "sha256:3f8804571ebe159c380ac6de37643bb4685970655d3bba243530d6558b799aa0"
             ],
@@ -626,19 +622,19 @@
             "version": "==6.0"
         },
         "requests": {
             "extras": [
                 "socks"
             ],
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.30.0"
         },
         "requests-oauthlib": {
             "hashes": [
                 "sha256:2577c501a2fb8d05a304c09d090d6e47c306fef15809d102b327cf8364bddab5",
                 "sha256:75beac4a47881eeb94d5ea5d6ad31ef88856affe2332b9aafb52c6452ccf0d7a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -665,19 +661,19 @@
                 "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.9.0"
         },
         "termcolor": {
             "hashes": [
-                "sha256:91ddd848e7251200eac969846cbae2dacd7d71c2871e92733289e7e3666f48e7",
-                "sha256:dfc8ac3f350788f23b2947b3e6cfa5a53b630b612e6cd8965a015a776020b99a"
+                "sha256:3afb05607b89aed0ffe25202399ee0867ad4d3cb4180d98aaf8eefa6a5f7d475",
+                "sha256:b5b08f68937f138fe92f6c089b99f1e2da0ae56c52b78bf7075fd95420fd9a5a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "version": "==2.3.0"
         },
         "terminaltables": {
             "hashes": [
                 "sha256:ba6eca5cb5ba02bba4c9f4f985af80c54ec3dccf94cfcd190154386255e47543",
                 "sha256:e4fdc4179c9e4aab5f674d80f09d76fa436b96fdc698a8505e0a36bf0804a874"
             ],
             "index": "pypi",
@@ -689,19 +685,19 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "yaspin": {
             "hashes": [
                 "sha256:17b5548479b3d5b30adec7a87ffcdcddb403d14a2bb86fbcee97f37951e13427",
                 "sha256:547afd1a9700ac3a29a9f5591c70343bef186ed5dfb5e545a9bb0c77e561a1c9"
             ],
             "index": "pypi",
@@ -715,19 +711,19 @@
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:525f126d5dc1b8b0b6ee398b33159105615d92dc4a17f2cd064125d57f6186fa",
-                "sha256:e3e4d0ffc2d15d954065579689c36aac57a339a4679a679579af6401db4d3fdb"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.0"
+            "version": "==2.15.5"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -763,19 +759,19 @@
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
             "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -945,97 +941,93 @@
                 "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
             "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
-                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
-                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
-                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
-                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
-                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
-                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
-                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
-                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
-                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
-                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
-                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
-                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
-                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
-                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
-                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
-                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
-                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
-                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
-                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
-                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
-                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
-                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
-                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
-                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
-                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
-                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
-                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
-                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
-                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
-                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
-                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
-                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
-                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
-                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
-                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
-                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
-                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
-                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
-                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
-                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
-                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
-                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
-                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
-                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
-                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
-                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
-                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
-                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
-                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
-                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
+                "sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3",
+                "sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a",
+                "sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813",
+                "sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0",
+                "sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a",
+                "sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd",
+                "sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139",
+                "sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b",
+                "sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252",
+                "sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790",
+                "sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045",
+                "sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce",
+                "sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200",
+                "sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718",
+                "sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b",
+                "sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f",
+                "sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5",
+                "sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade",
+                "sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5",
+                "sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a",
+                "sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8",
+                "sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33",
+                "sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e",
+                "sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c",
+                "sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3",
+                "sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969",
+                "sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068",
+                "sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2",
+                "sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771",
+                "sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed",
+                "sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212",
+                "sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614",
+                "sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88",
+                "sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3",
+                "sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c",
+                "sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84",
+                "sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11",
+                "sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1",
+                "sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1",
+                "sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e",
+                "sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1",
+                "sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd",
+                "sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47",
+                "sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a",
+                "sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c",
+                "sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31",
+                "sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5",
+                "sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6",
+                "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
+                "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
+                "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
             ],
             "index": "pypi",
-            "version": "==7.2.2"
+            "version": "==7.2.5"
         },
         "cryptography": {
             "hashes": [
-                "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1",
-                "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7",
-                "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06",
-                "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84",
-                "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915",
-                "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074",
-                "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5",
-                "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3",
-                "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9",
-                "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3",
-                "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011",
-                "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536",
-                "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a",
-                "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f",
-                "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480",
-                "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac",
-                "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0",
-                "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108",
-                "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828",
-                "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354",
-                "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612",
-                "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3",
-                "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.2"
+            "version": "==40.0.2"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
@@ -1068,19 +1060,19 @@
                 "sha256:a2986c21e4aba6b9870df40ef487a17be863cb7778dcf1c01e25917b7cd210bb"
             ],
             "index": "pypi",
             "version": "==2.2.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:3199fd0d3faea8b911be52b663dfccceb84c95949dd13179aa21436d1a79c4ce",
-                "sha256:e90b34656470756edf8b19656785c5fea73afa1953f3e1b0d645cef11cab3182"
+                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
+                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.0"
+            "version": "==3.12.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
                 "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -1139,19 +1131,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20",
-                "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==6.1.0"
+            "version": "==6.6.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
             "markers": "python_full_version >= '3.8.0'",
@@ -1334,19 +1326,19 @@
                 "sha256:ab2d0dca21aa5a7ae280c6fb869882260b825d9ced368b557b9124cf51ffb119"
             ],
             "index": "pypi",
             "version": "==0.6.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pep8-naming": {
             "hashes": [
                 "sha256:5d9f1056cb9427ce344e98d1a7f5665710e2f20f748438e308995852cfa24164",
                 "sha256:f3b4a5f9dd72b991bf7d8e2a341d2e1aa3a884a769b5aaac4f56825c1763bf3a"
             ],
             "version": "==0.10.0"
@@ -1357,19 +1349,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa",
-                "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.1"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -1420,27 +1412,27 @@
                 "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.5.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pylint": {
             "hashes": [
-                "sha256:1460829b6397cb5eb0cdb0b4fc4b556348e515cdca32115f74a1eb7c20b896b4",
-                "sha256:e097d8325f8c88e14ad12844e3fe2d963d3de871ea9a8f8ad25ab1c109889ddc"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.17.0"
+            "version": "==2.17.4"
         },
         "pylint-celery": {
             "hashes": [
                 "sha256:41e32094e7408d15c044178ea828dd524beedbdbe6f83f712c5e35bde1de4beb"
             ],
             "version": "==0.3"
         },
@@ -1528,27 +1520,27 @@
             "version": "==37.3"
         },
         "requests": {
             "extras": [
                 "socks"
             ],
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.30.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "requirements-detector": {
             "hashes": [
                 "sha256:246bd23867c12061eadb346a6fe2e616f0b64e681936154a76c494a27cda3ea8",
                 "sha256:9af62db621c95e0176fed029079924e648de22cd0bb4189c441b9376942faab1"
             ],
             "markers": "python_version >= '3.7' and python_version < '4.0'",
@@ -1560,19 +1552,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:91954fe80cfb7985727a467ca98a7618e5dd15178cc2da10f553b36a93859001",
-                "sha256:a104f37270bf677148d8acb07d33be1569eeee87e2d1beb286a4e9113caf6f2f"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.2"
+            "version": "==13.3.5"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
@@ -1622,19 +1614,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2",
-                "sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc"
+                "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b",
+                "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
             "index": "pypi",
-            "version": "==6.1.3"
+            "version": "==6.2.1"
         },
         "sphinx-rtd-theme": {
             "hashes": [
                 "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
                 "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
             ],
             "index": "pypi",
@@ -1710,19 +1702,19 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.8"
         },
         "tox": {
             "hashes": [
                 "sha256:17643b0e29c41f784c9c266a13302dc0604884b9ceff6686fbb31bada4a7aa3a",
                 "sha256:e6adcebddfec5e456e5d2884f82b9468e38c4ec6439ec97f7f1fb85d5b1bf846"
             ],
             "index": "pypi",
@@ -1742,27 +1734,27 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
-                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.21.0"
+            "version": "==20.23.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/README.rst` & `azureenergylabelercli-2.1.0/azureenergylabelercli/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   :header: "description", "CLI argument", "environment variable", "example value"
 
   "Tenand ID (required)", "`--tenant-id`", "`AZURE_LABELER_TENANT_ID`", "`00000000-0000-0000-0000-000000000000`"
   "Path to export the results", "`--export-path`", "`AZURE_LABELER_EXPORT_PATH`", "`/local/path` or Storage Account Url with SAS token `https://sa.blob.windows.net/container/?sas_token`"
   "Export only number of findings and energy label", "`--export-metrics`", "`AZURE_LABELER_EXPORT_METRICS`", "`false` (default)"
   "Export all findings information along with energy label", "`--export-all`", "`AZURE_LABELER_EXPORT_ALL`", "`true` (default)"
   "Regulatory frameworks to take into account", "`--frameworks`", "`AZURE_LABELER_FRAMEWORKS`", "`'Microsoft cloud security benchmark,Azure CIS 1.1.0'`"
-  "Explicit list of subscriptions to take into account", "`--allowed-subscription-ids`", "`AZURE_LABELER_TENANT_ID`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
+  "Explicit list of subscriptions to take into account", "`--allowed-subscription-ids`", "`AZURE_LABELER_ALLOWED_SUBSCRIPTION_IDS`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
   "Explicit list of subscriptions NOT to take into account", "`--denied-subscription-ids`", "`AZURE_LABELER_DENIED_SUBSCRIPTION_IDS`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
   "Level of log printing", "`--log-level`", "`AZURE_LABELER_LOG_LEVEL`", "`info`"
   "Logging configuration", "`--log-config`", "`AZURE_LABELER_LOG_CONFIG`", ""
 
 
 Supported authentication types
 ==============================
```

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/USAGE.rst` & `azureenergylabelercli-2.1.0/azureenergylabelercli/USAGE.rst`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/__init__.py` & `azureenergylabelercli-2.1.0/azureenergylabelercli/__init__.py`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/_version.py` & `azureenergylabelercli-2.1.0/azureenergylabelercli/_version.py`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/azureenergylabelercli.py` & `azureenergylabelercli-2.1.0/azureenergylabelercli/azureenergylabelercli.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,14 +171,24 @@
     parser.add_argument('--to-json',
                         '-j',
                         dest='to_json',
                         action='store_true',
                         required=False,
                         default=os.environ.get('AZURE_LABELER_TO_JSON', False),
                         help='Return the report in json format.')
+    parser.add_argument('--disable-spinner',
+                        '-ds',
+                        action='store_true',
+                        default=os.environ.get('AZURE_LABELER_DISABLE_SPINNER', False),
+                        help='If set spinner will be disabled on the CLI.')
+    parser.add_argument('--disable-banner',
+                        '-db',
+                        action='store_true',
+                        default=os.environ.get('AZURE_LABELER_DISABLE_BANNER', False),
+                        help='If set banner will be disabled on the CLI.')
     parser.set_defaults(export_all=True)
     args = parser.parse_args()
     args.allowed_subscription_ids, args.denied_subscription_ids = get_mutually_exclusive_args(
         args.allowed_subscription_ids,
         args.denied_subscription_ids,
         msg="conflicting arguments: --denied-subscription-ids, --allowed-subscription-ids")
     args.tenant_id, _ = get_mutually_exclusive_args(
@@ -219,28 +229,29 @@
         except ValueError:
             print(f'File "{config_file}" is not valid json, cannot continue.')
             raise SystemExit(1) from None
     else:
         coloredlogs.install(level=level.upper())
 
 
-def wait_for_findings(method_name, method_argument, log_level):
+def wait_for_findings(method_name, method_argument, log_level, disable_spinner=False):
     """If log level is not debug shows a spinner while the callable provided gets security hub findings.
 
     Args:
         method_name: The method to execute while waiting.
         method_argument: The argument to pass to the method.
         log_level: The log level as set by the user.
+        disable_spinner: The spinner will be disabled while retrieving the findings.
 
     Returns:
         findings: A list of defender for cloud findings as retrieved by the callable.
 
     """
     try:
-        if not log_level == 'debug':
+        if all([log_level != 'debug', not disable_spinner]):
             with yaspin(text="Please wait while retrieving Defender For Cloud findings...", color="yellow") as spinner:
                 findings = method_name(method_argument)
             spinner.ok("✅")
         else:
             findings = method_name(method_argument)
     except Exception as msg:
         LOGGER.error(msg)
@@ -249,86 +260,96 @@
 
 
 def get_tenant_reporting_data(tenant_id,  # pylint: disable=too-many-arguments
                               allowed_subscription_ids,
                               denied_subscription_ids,
                               export_all_data_flag,
                               frameworks,
-                              log_level):
+                              log_level,
+                              disable_spinner):
     """Gets the reporting data for a landing zone.
 
     Args:
         tenant_id: Tenant Id of the tenant
         allowed_subscription_ids: The allowed subscription ids for tenant inclusion if any.
         denied_subscription_ids: The denied subscription ids for tenant zone exclusion if any.
         export_all_data_flag: If set all data is going to be exported, else only basic reporting.
         frameworks: The frameworks to include in scoring.
         log_level: The log level set.
+        disable_spinner: The spinner will be disabled while retrieving the findings.
+
 
     Returns:
         report_data, exporter_arguments
 
     """
     labeler = AzureEnergyLabeler(tenant_id=tenant_id,
                                  tenant_thresholds=TENANT_THRESHOLDS,
                                  resource_group_thresholds=RESOURCE_GROUP_THRESHOLDS,
                                  subscription_thresholds=SUBSCRIPTION_THRESHOLDS,
                                  frameworks=frameworks,
                                  allowed_subscription_ids=allowed_subscription_ids,
                                  denied_subscription_ids=denied_subscription_ids)
-    wait_for_findings(AzureEnergyLabeler.defender_for_cloud_findings.fget, labeler, log_level)
+    wait_for_findings(AzureEnergyLabeler.filtered_defender_for_cloud_findings.fget,
+                      labeler, log_level, disable_spinner=disable_spinner)
     report_data = [['Tenant ID:', tenant_id],
                    ['Tenant Security Score:', labeler.tenant_energy_label.label],
                    ['Tenant Percentage Coverage:', labeler.tenant_energy_label.coverage],
                    ['Labeled Subscriptions Measured:',
                     labeler.labeled_subscriptions_energy_label.subscriptions_measured]]
     if labeler.tenant_energy_label.best_label != labeler.tenant_energy_label.worst_label:
         report_data.extend([['Best Subscription Security Score:', labeler.tenant_energy_label.best_label],
                             ['Worst Subscription Security Score:', labeler.tenant_energy_label.worst_label]])
     export_types = ALL_TENANT_EXPORT_TYPES if export_all_data_flag else TENANT_METRIC_EXPORT_TYPES
     exporter_arguments = {'export_types': export_types,
                           'id': tenant_id,
                           'energy_label': labeler.tenant_energy_label.label,
-                          'defender_for_cloud_findings': labeler.defender_for_cloud_findings,
+                          'defender_for_cloud_findings': labeler.filtered_defender_for_cloud_findings,
                           'labeled_subscriptions': labeler.tenant_labeled_subscriptions,
                           'credentials': labeler.tenant_credentials}
     return report_data, exporter_arguments
 
 
-def get_subscription_reporting_data(
+def get_subscription_reporting_data(  # pylint: disable=too-many-arguments,too-many-locals
         tenant_id,
         subscription_id,
         export_all_data_flag,
         frameworks,
-        log_level):
+        log_level,
+        disable_spinner):
     """Gets the reporting data for a single account.
 
     Args:
         tenant_id: Tenant Id of the tenant
         subscription_id: The ID of the subscription to get reporting on.
         export_all_data_flag: If set all data is going to be exported, else only basic reporting.
         frameworks: The frameworks to include in scoring.
         log_level: The log level set.
+        disable_spinner: The spinner will be disabled while retrieving the findings.
+
 
     Returns:
         report_data, exporter_arguments
 
     """
     _allowed_subscription_ids = []
     _allowed_subscription_ids.append(subscription_id)
     labeler = AzureEnergyLabeler(tenant_id=tenant_id,
                                  tenant_thresholds=TENANT_THRESHOLDS,
                                  resource_group_thresholds=RESOURCE_GROUP_THRESHOLDS,
                                  subscription_thresholds=SUBSCRIPTION_THRESHOLDS,
                                  frameworks=frameworks,
                                  allowed_subscription_ids=_allowed_subscription_ids)
     tenant = labeler.tenant
-    defender_for_cloud_findings = wait_for_findings(AzureEnergyLabeler.defender_for_cloud_findings.fget,
+    defender_for_cloud_findings = wait_for_findings(AzureEnergyLabeler.filtered_defender_for_cloud_findings.fget,
                                                     labeler,
-                                                    log_level)
+                                                    log_level,
+                                                    disable_spinner=disable_spinner)
+    filtered_findings = [finding for finding in defender_for_cloud_findings
+                         if finding.subscription_id == subscription_id]
     subscription = next(
         subscription for subscription in tenant.subscriptions if subscription.subscription_id == subscription_id)
     energy_label = subscription.get_energy_label(defender_for_cloud_findings)
     report_data = [['Subscription ID:', subscription.subscription_id],
                    ['Subscription Security Score:', energy_label.label],
                    ['Number Of High Findings:', energy_label.number_of_high_findings],
                    ['Number Of Medium Findings:', energy_label.number_of_medium_findings],
@@ -336,11 +357,11 @@
                    ['Max Days Open:', energy_label.max_days_open]]
     if subscription.display_name:
         report_data.insert(0, ['Subscription Display Name:', subscription.display_name])
     export_types = ALL_SUBSCRIPTION_EXPORT_DATA if export_all_data_flag else SUBSCRIPTION_METRIC_EXPORT_TYPES
     exporter_arguments = {'export_types': export_types,
                           'id': subscription.subscription_id,
                           'energy_label': energy_label.label,
-                          'defender_for_cloud_findings': defender_for_cloud_findings,
-                          'labeled_subscriptions': subscription,
+                          'defender_for_cloud_findings': filtered_findings,
+                          'labeled_subscriptions': [subscription],
                           'credentials': labeler.tenant_credentials}
     return report_data, exporter_arguments
```

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/azureenergylabelercliexceptions.py` & `azureenergylabelercli-2.1.0/azureenergylabelercli/azureenergylabelercliexceptions.py`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/conf/logging.json-example` & `azureenergylabelercli-2.1.0/azureenergylabelercli/conf/logging.json-example`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/dev-requirements.txt` & `azureenergylabelercli-2.1.0/azureenergylabelercli/dev-requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # by pipenv through Pipfile and Pipfile.lock .
 #
 # This file is created and managed automatically by the template and it is left
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
-sphinx>=6.1.3
+sphinx>=6.2.1
 sphinx-rtd-theme>=1.2.0
 prospector>=1.9.0
-coverage>=7.2.2
+coverage>=7.2.5
 nose>=1.3.7
 nose-htmloutput>=0.6.0
 tox==4.0.0
 betamax>=0.8.1
 betamax-serializers~=0.2.1
 semver>=2.13.0
 gitwrapperlib>=1.0.0
```

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli/validators.py` & `azureenergylabelercli-2.1.0/azureenergylabelercli/validators.py`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/PKG-INFO` & `azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureenergylabelercli
-Version: 2.0.3
+Version: 2.1.0
 Summary: A cli to help generate energy label for Azure tenant, subscriptions and resource groups.
 Home-page: https://github.com/schubergphilis/azureenergylabelercli
 Author: Sayantan Khanra
 Author-email: skhanra@schubergphilis.com
 License: MIT
 Keywords: azureenergylabelercli
 Classifier: Development Status :: 1 - Planning
@@ -45,15 +45,15 @@
   :header: "description", "CLI argument", "environment variable", "example value"
 
   "Tenand ID (required)", "`--tenant-id`", "`AZURE_LABELER_TENANT_ID`", "`00000000-0000-0000-0000-000000000000`"
   "Path to export the results", "`--export-path`", "`AZURE_LABELER_EXPORT_PATH`", "`/local/path` or Storage Account Url with SAS token `https://sa.blob.windows.net/container/?sas_token`"
   "Export only number of findings and energy label", "`--export-metrics`", "`AZURE_LABELER_EXPORT_METRICS`", "`false` (default)"
   "Export all findings information along with energy label", "`--export-all`", "`AZURE_LABELER_EXPORT_ALL`", "`true` (default)"
   "Regulatory frameworks to take into account", "`--frameworks`", "`AZURE_LABELER_FRAMEWORKS`", "`'Microsoft cloud security benchmark,Azure CIS 1.1.0'`"
-  "Explicit list of subscriptions to take into account", "`--allowed-subscription-ids`", "`AZURE_LABELER_TENANT_ID`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
+  "Explicit list of subscriptions to take into account", "`--allowed-subscription-ids`", "`AZURE_LABELER_ALLOWED_SUBSCRIPTION_IDS`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
   "Explicit list of subscriptions NOT to take into account", "`--denied-subscription-ids`", "`AZURE_LABELER_DENIED_SUBSCRIPTION_IDS`", "`'00000000-0000-0000-0000-000000000000,00000000-0000-0000-0000-000000000001'`"
   "Level of log printing", "`--log-level`", "`AZURE_LABELER_LOG_LEVEL`", "`info`"
   "Logging configuration", "`--log-config`", "`AZURE_LABELER_LOG_CONFIG`", ""
 
 
 Supported authentication types
 ==============================
@@ -290,7 +290,14 @@
 * Bump template and dependencies.
 
 
 2.0.3 (21-03-2023)
 ------------------
 
 * Bumped library version which now filters subscriptions based on the tenant_id.
+
+
+2.1.0 (15-05-2023)
+------------------
+
+* Added option to disable banner and spinner
+* Improved filtering of findings
```

### Comparing `azureenergylabelercli-2.0.3/azureenergylabelercli.egg-info/SOURCES.txt` & `azureenergylabelercli-2.1.0/azureenergylabelercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/dev-requirements.txt` & `azureenergylabelercli-2.1.0/dev-requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # by pipenv through Pipfile and Pipfile.lock .
 #
 # This file is created and managed automatically by the template and it is left
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
-sphinx>=6.1.3
+sphinx>=6.2.1
 sphinx-rtd-theme>=1.2.0
 prospector>=1.9.0
-coverage>=7.2.2
+coverage>=7.2.5
 nose>=1.3.7
 nose-htmloutput>=0.6.0
 tox==4.0.0
 betamax>=0.8.1
 betamax-serializers~=0.2.1
 semver>=2.13.0
 gitwrapperlib>=1.0.0
```

### Comparing `azureenergylabelercli-2.0.3/docs/Makefile` & `azureenergylabelercli-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/docs/conf.py` & `azureenergylabelercli-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/docs/index.rst` & `azureenergylabelercli-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/setup.py` & `azureenergylabelercli-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `azureenergylabelercli-2.0.3/tests/test_azureenergylabelercli.py` & `azureenergylabelercli-2.1.0/tests/test_azureenergylabelercli.py`

 * *Files identical despite different names*

