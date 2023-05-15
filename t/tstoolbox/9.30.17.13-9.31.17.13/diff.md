# Comparing `tmp/tstoolbox-9.30.17.13.tar.gz` & `tmp/tstoolbox-9.31.17.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tstoolbox-9.30.17.13.tar", last modified: Wed May 31 12:01:35 2017, max compression
+gzip compressed data, was "dist/tstoolbox-9.31.17.13.tar", last modified: Wed May 31 18:58:41 2017, max compression
```

## Comparing `tstoolbox-9.30.17.13.tar` & `tstoolbox-9.31.17.13.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/tstoolbox.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      482 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/tstoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      108 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/tstoolbox.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)     7268 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/tstoolbox.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2013-10-01 03:47:19.000000 tstoolbox-9.30.17.13/tstoolbox.egg-info/not-zip-safe
--rw-r--r--   0 tim       (1000) tim       (1000)       10 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/tstoolbox.egg-info/top_level.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/tstoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       56 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/tstoolbox.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     5034 2017-02-15 03:14:19.000000 tstoolbox-9.30.17.13/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     7268 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)       50 2014-12-14 07:05:08.000000 tstoolbox-9.30.17.13/AUTHORS.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)       49 2016-09-16 02:25:56.000000 tstoolbox-9.30.17.13/pip_requirements.txt
--rw-r--r--   0 tim       (1000) tim       (1000)     3166 2014-12-14 07:05:08.000000 tstoolbox-9.30.17.13/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       85 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      114 2013-10-24 02:15:58.000000 tstoolbox-9.30.17.13/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)     1486 2013-09-05 20:14:01.000000 tstoolbox-9.30.17.13/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     2023 2017-05-16 02:05:24.000000 tstoolbox-9.30.17.13/setup.py
--rw-rw-r--   0 tim       (1000) tim       (1000)       11 2017-05-31 12:00:28.000000 tstoolbox-9.30.17.13/VERSION
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-05-31 12:01:35.000000 tstoolbox-9.30.17.13/tstoolbox/
--rw-r--r--   0 tim       (1000) tim       (1000)    24307 2017-05-30 20:22:19.000000 tstoolbox-9.30.17.13/tstoolbox/tsutils.py
--rw-r--r--   0 tim       (1000) tim       (1000)       32 2016-08-26 22:31:16.000000 tstoolbox-9.30.17.13/tstoolbox/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)   108316 2017-05-31 11:59:30.000000 tstoolbox-9.30.17.13/tstoolbox/tstoolbox.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    28113 2017-03-29 01:11:03.000000 tstoolbox-9.30.17.13/tstoolbox/peakdetect.py
--rw-r--r--   0 tim       (1000) tim       (1000)     7685 2017-05-08 20:17:57.000000 tstoolbox-9.30.17.13/tstoolbox/fill_functions.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2551 2017-05-23 02:23:30.000000 tstoolbox-9.30.17.13/tstoolbox/filters.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/tstoolbox.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      482 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/tstoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      108 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/tstoolbox.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)     7268 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/tstoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2013-10-01 03:47:19.000000 tstoolbox-9.31.17.13/tstoolbox.egg-info/not-zip-safe
+-rw-r--r--   0 tim       (1000) tim       (1000)       10 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/tstoolbox.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/tstoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       56 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/tstoolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5034 2017-02-15 03:14:19.000000 tstoolbox-9.31.17.13/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     7268 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)       50 2014-12-14 07:05:08.000000 tstoolbox-9.31.17.13/AUTHORS.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)       49 2016-09-16 02:25:56.000000 tstoolbox-9.31.17.13/pip_requirements.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)     3166 2014-12-14 07:05:08.000000 tstoolbox-9.31.17.13/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       85 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      114 2013-10-24 02:15:58.000000 tstoolbox-9.31.17.13/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)     1486 2013-09-05 20:14:01.000000 tstoolbox-9.31.17.13/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2023 2017-05-16 02:05:24.000000 tstoolbox-9.31.17.13/setup.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)       11 2017-05-31 18:57:49.000000 tstoolbox-9.31.17.13/VERSION
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-05-31 18:58:41.000000 tstoolbox-9.31.17.13/tstoolbox/
+-rw-r--r--   0 tim       (1000) tim       (1000)    24316 2017-05-31 18:56:10.000000 tstoolbox-9.31.17.13/tstoolbox/tsutils.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       32 2016-08-26 22:31:16.000000 tstoolbox-9.31.17.13/tstoolbox/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)   108316 2017-05-31 11:59:30.000000 tstoolbox-9.31.17.13/tstoolbox/tstoolbox.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28113 2017-03-29 01:11:03.000000 tstoolbox-9.31.17.13/tstoolbox/peakdetect.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     7685 2017-05-08 20:17:57.000000 tstoolbox-9.31.17.13/tstoolbox/fill_functions.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2551 2017-05-23 02:23:30.000000 tstoolbox-9.31.17.13/tstoolbox/filters.py
```

### Comparing `tstoolbox-9.30.17.13/tstoolbox.egg-info/PKG-INFO` & `tstoolbox-9.31.17.13/tstoolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tstoolbox
-Version: 9.30.17.13
+Version: 9.31.17.13
 Summary: Command line script to manipulate time series files.
 Home-page: http://timcera.bitbucket.org/tstoolbox/docsrc/index.html
 Author: Tim Cera, P.E.
 Author-email: tim@cerazone.net
 License: UNKNOWN
 Description: .. image:: https://travis-ci.org/timcera/tstoolbox.svg?branch=master
             :target: https://travis-ci.org/timcera/tstoolbox
```

### Comparing `tstoolbox-9.30.17.13/README.rst` & `tstoolbox-9.31.17.13/README.rst`

 * *Files identical despite different names*

### Comparing `tstoolbox-9.30.17.13/PKG-INFO` & `tstoolbox-9.31.17.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tstoolbox
-Version: 9.30.17.13
+Version: 9.31.17.13
 Summary: Command line script to manipulate time series files.
 Home-page: http://timcera.bitbucket.org/tstoolbox/docsrc/index.html
 Author: Tim Cera, P.E.
 Author-email: tim@cerazone.net
 License: UNKNOWN
 Description: .. image:: https://travis-ci.org/timcera/tstoolbox.svg?branch=master
             :target: https://travis-ci.org/timcera/tstoolbox
```

### Comparing `tstoolbox-9.30.17.13/CONTRIBUTING.rst` & `tstoolbox-9.31.17.13/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tstoolbox-9.30.17.13/LICENSE.txt` & `tstoolbox-9.31.17.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tstoolbox-9.30.17.13/setup.py` & `tstoolbox-9.31.17.13/setup.py`

 * *Files identical despite different names*

### Comparing `tstoolbox-9.30.17.13/tstoolbox/tsutils.py` & `tstoolbox-9.31.17.13/tstoolbox/tsutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 
 
 def broadcast_equation(equation_str,
                        input_ts,
                        broadcast):
     # "broadcast" should be a dictionary that has keys for each variable
     # in the "equation_str".
+    pass
 
 def required_cols(input_tsd,
                   req_cols):
     """Collected all required columns."""
     collected_cols = []
     for rc in req_cols:
         try:
```

### Comparing `tstoolbox-9.30.17.13/tstoolbox/tstoolbox.py` & `tstoolbox-9.31.17.13/tstoolbox/tstoolbox.py`

 * *Files identical despite different names*

### Comparing `tstoolbox-9.30.17.13/tstoolbox/peakdetect.py` & `tstoolbox-9.31.17.13/tstoolbox/peakdetect.py`

 * *Files identical despite different names*

### Comparing `tstoolbox-9.30.17.13/tstoolbox/fill_functions.py` & `tstoolbox-9.31.17.13/tstoolbox/fill_functions.py`

 * *Files identical despite different names*

### Comparing `tstoolbox-9.30.17.13/tstoolbox/filters.py` & `tstoolbox-9.31.17.13/tstoolbox/filters.py`

 * *Files identical despite different names*

