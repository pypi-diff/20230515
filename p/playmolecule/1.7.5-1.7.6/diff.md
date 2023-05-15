# Comparing `tmp/playmolecule-1.7.5.tar.gz` & `tmp/playmolecule-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.7.5.tar", last modified: Mon May 15 09:41:13 2023, max compression
+gzip compressed data, was "playmolecule-1.7.6.tar", last modified: Mon May 15 09:43:08 2023, max compression
```

## Comparing `playmolecule-1.7.5.tar` & `playmolecule-1.7.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:41:13.551748 playmolecule-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-15 09:40:49.000000 playmolecule-1.7.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 09:40:49.000000 playmolecule-1.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-15 09:41:13.551748 playmolecule-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-15 09:40:49.000000 playmolecule-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:41:13.555748 playmolecule-1.7.5/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 09:41:13.555748 playmolecule-1.7.5/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    34314 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-15 09:40:49.000000 playmolecule-1.7.5/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:41:13.551748 playmolecule-1.7.5/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-15 09:41:13.000000 playmolecule-1.7.5/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-15 09:41:13.000000 playmolecule-1.7.5/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:41:13.000000 playmolecule-1.7.5/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:41:13.000000 playmolecule-1.7.5/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 09:41:13.000000 playmolecule-1.7.5/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 09:41:13.000000 playmolecule-1.7.5/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-15 09:40:49.000000 playmolecule-1.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:41:13.555748 playmolecule-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-15 09:40:49.000000 playmolecule-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:41:13.551748 playmolecule-1.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-15 09:40:49.000000 playmolecule-1.7.5/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-15 09:40:49.000000 playmolecule-1.7.5/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-15 09:40:49.000000 playmolecule-1.7.5/tests/test_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-15 09:40:49.000000 playmolecule-1.7.5/tests/test_func_to_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:43:08.886223 playmolecule-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-15 09:42:50.000000 playmolecule-1.7.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 09:42:50.000000 playmolecule-1.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-15 09:43:08.886223 playmolecule-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-15 09:42:50.000000 playmolecule-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:43:08.886223 playmolecule-1.7.6/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 09:43:08.886223 playmolecule-1.7.6/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34392 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-15 09:42:50.000000 playmolecule-1.7.6/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:43:08.886223 playmolecule-1.7.6/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-15 09:43:08.000000 playmolecule-1.7.6/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-15 09:43:08.000000 playmolecule-1.7.6/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:43:08.000000 playmolecule-1.7.6/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:43:08.000000 playmolecule-1.7.6/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 09:43:08.000000 playmolecule-1.7.6/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 09:43:08.000000 playmolecule-1.7.6/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-15 09:42:50.000000 playmolecule-1.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:43:08.886223 playmolecule-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-15 09:42:50.000000 playmolecule-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:43:08.886223 playmolecule-1.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-15 09:42:50.000000 playmolecule-1.7.6/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-15 09:42:50.000000 playmolecule-1.7.6/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-15 09:42:50.000000 playmolecule-1.7.6/tests/test_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-15 09:42:50.000000 playmolecule-1.7.6/tests/test_func_to_argparse.py
```

### Comparing `playmolecule-1.7.5/LICENSE.md` & `playmolecule-1.7.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/PKG-INFO` & `playmolecule-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.7.5
+Version: 1.7.6
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.7.5/playmolecule/__init__.py` & `playmolecule-1.7.6/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/_test_funcs.py` & `playmolecule-1.7.6/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/config.py` & `playmolecule-1.7.6/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/datacenter.py` & `playmolecule-1.7.6/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/devutils.py` & `playmolecule-1.7.6/playmolecule/devutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,16 +464,18 @@
 
     manifest["description"] = parser.description
     manifest["params"] = parserargs
 
     # Deprecate these once we update or get rid of the backend
     if "specs" not in manifest:
         manifest["specs"] = '{"app": "play0GPU"}'
+    if "api_version" not in manifest:
+        manifest["api_version"] = "v1"
     if "container" not in manifest:
-        manifest["container"] = f"{manifest['name']}_{manifest['version']}"
+        manifest["container"] = f"{manifest['name']}_v{manifest['version']}"
     if "periodicity" not in manifest:
         manifest["periodicity"] = 0
 
     return manifest
 
 
 def write_argparser_json(outfile, parser):
```

### Comparing `playmolecule-1.7.5/playmolecule/func2argparse.py` & `playmolecule-1.7.6/playmolecule/func2argparse.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/job.py` & `playmolecule-1.7.6/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/jsonlogger.py` & `playmolecule-1.7.6/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/local.py` & `playmolecule-1.7.6/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/playqueue.py` & `playmolecule-1.7.6/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/session.py` & `playmolecule-1.7.6/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule/utils.py` & `playmolecule-1.7.6/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.7.6/playmolecule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.7.5
+Version: 1.7.6
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.7.5/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.7.6/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/pyproject.toml` & `playmolecule-1.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/tests/test.py` & `playmolecule-1.7.6/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/tests/test_app_wrapper.py` & `playmolecule-1.7.6/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/tests/test_datacenter.py` & `playmolecule-1.7.6/tests/test_datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.5/tests/test_func_to_argparse.py` & `playmolecule-1.7.6/tests/test_func_to_argparse.py`

 * *Files identical despite different names*

