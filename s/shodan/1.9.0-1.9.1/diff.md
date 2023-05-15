# Comparing `tmp/shodan-1.9.0.tar.gz` & `tmp/shodan-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shodan-1.9.0.tar", last modified: Wed Aug  1 06:26:35 2018, max compression
+gzip compressed data, was "dist/shodan-1.9.1.tar", last modified: Sat Aug 18 01:22:47 2018, max compression
```

## Comparing `shodan-1.9.0.tar` & `shodan-1.9.1.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-01 06:26:35.000000 shodan-1.9.0/
-drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-01 06:26:35.000000 shodan-1.9.0/shodan.egg-info/
--rw-rw-r--   0 achillean  (1000) achillean  (1000)        1 2018-08-01 06:26:34.000000 shodan-1.9.0/shodan.egg-info/dependency_links.txt
--rw-rw-r--   0 achillean  (1000) achillean  (1000)       56 2018-08-01 06:26:34.000000 shodan-1.9.0/shodan.egg-info/requires.txt
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     3499 2018-08-01 06:26:34.000000 shodan-1.9.0/shodan.egg-info/PKG-INFO
--rw-r--r--   0 achillean  (1000) achillean  (1000)       49 2018-08-01 06:26:34.000000 shodan-1.9.0/shodan.egg-info/entry_points.txt
--rw-rw-r--   0 achillean  (1000) achillean  (1000)      968 2018-08-01 06:26:34.000000 shodan-1.9.0/shodan.egg-info/SOURCES.txt
--rw-rw-r--   0 achillean  (1000) achillean  (1000)        7 2018-08-01 06:26:34.000000 shodan-1.9.0/shodan.egg-info/top_level.txt
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     1930 2018-06-01 02:35:05.000000 shodan-1.9.0/README.rst
-drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-01 06:26:35.000000 shodan-1.9.0/tests/
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     4359 2015-11-20 00:41:53.000000 shodan-1.9.0/tests/test_shodan.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)        0 2014-10-04 23:45:40.000000 shodan-1.9.0/tests/__init__.py
--rw-r--r--   0 achillean  (1000) achillean  (1000)     3499 2018-08-01 06:26:35.000000 shodan-1.9.0/PKG-INFO
--rw-rw-r--   0 achillean  (1000) achillean  (1000)       52 2014-10-04 23:45:40.000000 shodan-1.9.0/AUTHORS
--rw-rw-r--   0 achillean  (1000) achillean  (1000)       95 2017-07-05 21:17:17.000000 shodan-1.9.0/.gitignore
--rw-r--r--   0 achillean  (1000) achillean  (1000)       59 2018-08-01 06:26:35.000000 shodan-1.9.0/setup.cfg
--rw-rw-r--   0 achillean  (1000) achillean  (1000)       55 2017-06-16 21:52:10.000000 shodan-1.9.0/requirements.txt
--rwxr-xr-x   0 achillean  (1000) achillean  (1000)     1459 2018-08-01 06:08:43.000000 shodan-1.9.0/setup.py
-drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-01 06:26:35.000000 shodan-1.9.0/shodan/
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     7088 2017-05-17 17:08:42.000000 shodan-1.9.0/shodan/api.py
-drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-01 06:26:35.000000 shodan-1.9.0/shodan/cli/
--rwxr-xr-x   0 achillean  (1000) achillean  (1000)     9095 2018-02-24 21:29:40.000000 shodan-1.9.0/shodan/cli/worldmap.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)        0 2014-11-29 20:45:10.000000 shodan-1.9.0/shodan/cli/__init__.py
--rw-r--r--   0 achillean  (1000) achillean  (1000)      674 2018-02-24 19:28:32.000000 shodan-1.9.0/shodan/cli/helpers.py
-drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-01 06:26:35.000000 shodan-1.9.0/shodan/cli/converter/
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     2280 2016-02-18 06:38:38.000000 shodan-1.9.0/shodan/cli/converter/csvc.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)      168 2017-06-20 22:17:07.000000 shodan-1.9.0/shodan/cli/converter/__init__.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     3808 2017-06-17 00:33:56.000000 shodan-1.9.0/shodan/cli/converter/excel.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)      121 2016-02-18 05:00:23.000000 shodan-1.9.0/shodan/cli/converter/base.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     1825 2017-06-20 23:01:02.000000 shodan-1.9.0/shodan/cli/converter/images.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     4487 2016-02-18 05:02:06.000000 shodan-1.9.0/shodan/cli/converter/kml.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     1431 2016-12-19 02:29:03.000000 shodan-1.9.0/shodan/cli/converter/geojson.py
--rw-r--r--   0 achillean  (1000) achillean  (1000)      189 2016-12-16 21:10:32.000000 shodan-1.9.0/shodan/cli/settings.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)    18256 2018-08-01 06:07:51.000000 shodan-1.9.0/shodan/client.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)      225 2015-11-20 00:41:53.000000 shodan-1.9.0/shodan/alert.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     4785 2018-08-01 06:07:51.000000 shodan-1.9.0/shodan/stream.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)      101 2015-03-01 05:14:58.000000 shodan-1.9.0/shodan/__init__.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     4986 2018-08-01 06:07:51.000000 shodan-1.9.0/shodan/helpers.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)      420 2015-11-20 00:41:53.000000 shodan-1.9.0/shodan/exception.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     2152 2018-08-01 06:07:51.000000 shodan-1.9.0/shodan/threatnet.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)    49347 2018-08-01 06:07:51.000000 shodan-1.9.0/shodan/__main__.py
-drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-01 06:26:35.000000 shodan-1.9.0/docs/
-drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-01 06:26:35.000000 shodan-1.9.0/docs/examples/
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     3791 2016-01-17 03:32:15.000000 shodan-1.9.0/docs/examples/gifcreator.rst
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     1640 2018-03-16 21:33:58.000000 shodan-1.9.0/docs/examples/cert-stream.rst
--rw-r--r--   0 achillean  (1000) achillean  (1000)     3338 2017-12-03 05:42:17.000000 shodan-1.9.0/docs/examples/query-summary.rst
--rw-rw-r--   0 achillean  (1000) achillean  (1000)      730 2016-01-17 02:37:54.000000 shodan-1.9.0/docs/examples/basic-search.rst
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     6715 2014-10-04 23:45:40.000000 shodan-1.9.0/docs/make.bat
--rw-rw-r--   0 achillean  (1000) achillean  (1000)      289 2014-10-04 23:45:40.000000 shodan-1.9.0/docs/api.rst
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     1123 2018-03-16 21:35:43.000000 shodan-1.9.0/docs/index.rst
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     6790 2014-10-04 23:45:40.000000 shodan-1.9.0/docs/Makefile
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     8264 2014-10-04 23:45:40.000000 shodan-1.9.0/docs/conf.py
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     3154 2018-03-16 21:31:41.000000 shodan-1.9.0/docs/tutorial.rst
--rw-r--r--   0 achillean  (1000) achillean  (1000)       98 2017-07-05 21:14:10.000000 shodan-1.9.0/MANIFEST.in
--rw-rw-r--   0 achillean  (1000) achillean  (1000)     1299 2018-05-31 21:52:28.000000 shodan-1.9.0/LICENSE
+drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-18 01:22:47.000000 shodan-1.9.1/
+drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan.egg-info/
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)        1 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan.egg-info/dependency_links.txt
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)       56 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan.egg-info/requires.txt
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     3736 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan.egg-info/PKG-INFO
+-rw-r--r--   0 achillean  (1000) achillean  (1000)       49 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan.egg-info/entry_points.txt
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     1000 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan.egg-info/SOURCES.txt
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)        7 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan.egg-info/top_level.txt
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     2119 2018-08-17 21:19:34.000000 shodan-1.9.1/README.rst
+drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-18 01:22:47.000000 shodan-1.9.1/tests/
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     4359 2015-11-20 00:41:53.000000 shodan-1.9.1/tests/test_shodan.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)        0 2014-10-04 23:45:40.000000 shodan-1.9.1/tests/__init__.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     1722 2018-08-18 01:22:21.000000 shodan-1.9.1/CHANGELOG.md
+-rw-r--r--   0 achillean  (1000) achillean  (1000)     3736 2018-08-18 01:22:47.000000 shodan-1.9.1/PKG-INFO
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)       52 2014-10-04 23:45:40.000000 shodan-1.9.1/AUTHORS
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)       95 2017-07-05 21:17:17.000000 shodan-1.9.1/.gitignore
+-rw-r--r--   0 achillean  (1000) achillean  (1000)       59 2018-08-18 01:22:47.000000 shodan-1.9.1/setup.cfg
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)       55 2017-06-16 21:52:10.000000 shodan-1.9.1/requirements.txt
+-rwxr-xr-x   0 achillean  (1000) achillean  (1000)     1459 2018-08-18 01:18:58.000000 shodan-1.9.1/setup.py
+drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan/
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     7088 2017-05-17 17:08:42.000000 shodan-1.9.1/shodan/api.py
+drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan/cli/
+-rwxr-xr-x   0 achillean  (1000) achillean  (1000)     9243 2018-08-17 22:45:21.000000 shodan-1.9.1/shodan/cli/worldmap.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)        0 2014-11-29 20:45:10.000000 shodan-1.9.1/shodan/cli/__init__.py
+-rw-r--r--   0 achillean  (1000) achillean  (1000)      674 2018-02-24 19:28:32.000000 shodan-1.9.1/shodan/cli/helpers.py
+drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-18 01:22:47.000000 shodan-1.9.1/shodan/cli/converter/
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     2280 2016-02-18 06:38:38.000000 shodan-1.9.1/shodan/cli/converter/csvc.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)      168 2017-06-20 22:17:07.000000 shodan-1.9.1/shodan/cli/converter/__init__.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     3808 2017-06-17 00:33:56.000000 shodan-1.9.1/shodan/cli/converter/excel.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)      121 2016-02-18 05:00:23.000000 shodan-1.9.1/shodan/cli/converter/base.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     1825 2017-06-20 23:01:02.000000 shodan-1.9.1/shodan/cli/converter/images.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     4487 2016-02-18 05:02:06.000000 shodan-1.9.1/shodan/cli/converter/kml.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     1431 2016-12-19 02:29:03.000000 shodan-1.9.1/shodan/cli/converter/geojson.py
+-rw-r--r--   0 achillean  (1000) achillean  (1000)      189 2016-12-16 21:10:32.000000 shodan-1.9.1/shodan/cli/settings.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     4984 2018-08-17 20:44:48.000000 shodan-1.9.1/shodan/cli/host.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)    18687 2018-08-18 00:59:43.000000 shodan-1.9.1/shodan/client.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)      225 2015-11-20 00:41:53.000000 shodan-1.9.1/shodan/alert.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     4785 2018-08-01 06:07:51.000000 shodan-1.9.1/shodan/stream.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)      101 2015-03-01 05:14:58.000000 shodan-1.9.1/shodan/__init__.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     4986 2018-08-01 06:07:51.000000 shodan-1.9.1/shodan/helpers.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)      420 2015-11-20 00:41:53.000000 shodan-1.9.1/shodan/exception.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     2152 2018-08-01 06:07:51.000000 shodan-1.9.1/shodan/threatnet.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)    45425 2018-08-17 23:36:48.000000 shodan-1.9.1/shodan/__main__.py
+drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-18 01:22:47.000000 shodan-1.9.1/docs/
+drwxr-xr-x   0 achillean  (1000) achillean  (1000)        0 2018-08-18 01:22:47.000000 shodan-1.9.1/docs/examples/
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     3791 2016-01-17 03:32:15.000000 shodan-1.9.1/docs/examples/gifcreator.rst
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     1640 2018-03-16 21:33:58.000000 shodan-1.9.1/docs/examples/cert-stream.rst
+-rw-r--r--   0 achillean  (1000) achillean  (1000)     3338 2017-12-03 05:42:17.000000 shodan-1.9.1/docs/examples/query-summary.rst
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)      730 2016-01-17 02:37:54.000000 shodan-1.9.1/docs/examples/basic-search.rst
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     6715 2014-10-04 23:45:40.000000 shodan-1.9.1/docs/make.bat
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)      289 2014-10-04 23:45:40.000000 shodan-1.9.1/docs/api.rst
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     1123 2018-03-16 21:35:43.000000 shodan-1.9.1/docs/index.rst
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     6790 2014-10-04 23:45:40.000000 shodan-1.9.1/docs/Makefile
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     8264 2014-10-04 23:45:40.000000 shodan-1.9.1/docs/conf.py
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     3154 2018-03-16 21:31:41.000000 shodan-1.9.1/docs/tutorial.rst
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)      119 2018-08-17 19:14:48.000000 shodan-1.9.1/MANIFEST.in
+-rw-rw-r--   0 achillean  (1000) achillean  (1000)     1299 2018-05-31 21:52:28.000000 shodan-1.9.1/LICENSE
```

### Comparing `shodan-1.9.0/shodan.egg-info/PKG-INFO` & `shodan-1.9.1/shodan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: shodan
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python library and command-line utility for Shodan (https://developer.shodan.io)
 Home-page: http://github.com/achillean/shodan-python/tree/master
 Author: John Matherly
 Author-email: jmath@shodan.io
 License: UNKNOWN
-Description: shodan: The official Python library for accessing Shodan
-        ========================================================
+Description: shodan: The official Python library and CLI for Shodan
+        ======================================================
         
         .. image:: https://img.shields.io/pypi/v/shodan.svg
             :target: https://pypi.org/project/shodan/
         
         .. image:: https://img.shields.io/github/contributors/achillean/shodan-python.svg
             :target: https://github.com/achillean/shodan-python/graphs/contributors
         
@@ -24,14 +24,20 @@
         
         - Search Shodan
         - `Fast/ bulk IP lookups <https://help.shodan.io/developer-fundamentals/looking-up-ip-info>`_
         - Streaming API support for real-time consumption of Shodan firehose
         - `Network alerts (aka private firehose) <https://help.shodan.io/guides/how-to-monitor-network>`_
         - Exploit search API fully implemented
         - Bulk data downloads
+        - `Command-line interface <https://cli.shodan.io>`_
+        
+        .. image:: https://cli.shodan.io/img/shodan-cli-preview.png
+            :target: https://asciinema.org/~Shodan
+            :width: 400px
+            :align: center
         
         
         Quick Start
         -----------
         
         .. code-block:: python
```

### Comparing `shodan-1.9.0/shodan.egg-info/SOURCES.txt` & `shodan-1.9.1/shodan.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 AUTHORS
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 docs/Makefile
 docs/api.rst
@@ -28,14 +29,15 @@
 shodan.egg-info/SOURCES.txt
 shodan.egg-info/dependency_links.txt
 shodan.egg-info/entry_points.txt
 shodan.egg-info/requires.txt
 shodan.egg-info/top_level.txt
 shodan/cli/__init__.py
 shodan/cli/helpers.py
+shodan/cli/host.py
 shodan/cli/settings.py
 shodan/cli/worldmap.py
 shodan/cli/converter/__init__.py
 shodan/cli/converter/base.py
 shodan/cli/converter/csvc.py
 shodan/cli/converter/excel.py
 shodan/cli/converter/geojson.py
```

### Comparing `shodan-1.9.0/README.rst` & `shodan-1.9.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-shodan: The official Python library for accessing Shodan
-========================================================
+shodan: The official Python library and CLI for Shodan
+======================================================
 
 .. image:: https://img.shields.io/pypi/v/shodan.svg
     :target: https://pypi.org/project/shodan/
 
 .. image:: https://img.shields.io/github/contributors/achillean/shodan-python.svg
     :target: https://github.com/achillean/shodan-python/graphs/contributors
 
@@ -16,14 +16,20 @@
 
 - Search Shodan
 - `Fast/ bulk IP lookups <https://help.shodan.io/developer-fundamentals/looking-up-ip-info>`_
 - Streaming API support for real-time consumption of Shodan firehose
 - `Network alerts (aka private firehose) <https://help.shodan.io/guides/how-to-monitor-network>`_
 - Exploit search API fully implemented
 - Bulk data downloads
+- `Command-line interface <https://cli.shodan.io>`_
+
+.. image:: https://cli.shodan.io/img/shodan-cli-preview.png
+    :target: https://asciinema.org/~Shodan
+    :width: 400px
+    :align: center
 
 
 Quick Start
 -----------
 
 .. code-block:: python
```

### Comparing `shodan-1.9.0/tests/test_shodan.py` & `shodan-1.9.1/tests/test_shodan.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/PKG-INFO` & `shodan-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: shodan
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python library and command-line utility for Shodan (https://developer.shodan.io)
 Home-page: http://github.com/achillean/shodan-python/tree/master
 Author: John Matherly
 Author-email: jmath@shodan.io
 License: UNKNOWN
-Description: shodan: The official Python library for accessing Shodan
-        ========================================================
+Description: shodan: The official Python library and CLI for Shodan
+        ======================================================
         
         .. image:: https://img.shields.io/pypi/v/shodan.svg
             :target: https://pypi.org/project/shodan/
         
         .. image:: https://img.shields.io/github/contributors/achillean/shodan-python.svg
             :target: https://github.com/achillean/shodan-python/graphs/contributors
         
@@ -24,14 +24,20 @@
         
         - Search Shodan
         - `Fast/ bulk IP lookups <https://help.shodan.io/developer-fundamentals/looking-up-ip-info>`_
         - Streaming API support for real-time consumption of Shodan firehose
         - `Network alerts (aka private firehose) <https://help.shodan.io/guides/how-to-monitor-network>`_
         - Exploit search API fully implemented
         - Bulk data downloads
+        - `Command-line interface <https://cli.shodan.io>`_
+        
+        .. image:: https://cli.shodan.io/img/shodan-cli-preview.png
+            :target: https://asciinema.org/~Shodan
+            :width: 400px
+            :align: center
         
         
         Quick Start
         -----------
         
         .. code-block:: python
```

### Comparing `shodan-1.9.0/setup.py` & `shodan-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 DEPENDENCIES = open('requirements.txt', 'r').read().split('\n')
 README = open('README.rst', 'r').read()
 
 setup(
     name = 'shodan',
-    version = '1.9.0',
+    version = '1.9.1',
     description = 'Python library and command-line utility for Shodan (https://developer.shodan.io)',
     long_description = README,
     long_description_content_type = 'text/x-rst',
     author = 'John Matherly',
     author_email = 'jmath@shodan.io',
     url = 'http://github.com/achillean/shodan-python/tree/master',
     packages = ['shodan', 'shodan.cli', 'shodan.cli.converter'],
```

### Comparing `shodan-1.9.0/shodan/api.py` & `shodan-1.9.1/shodan/api.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/cli/worldmap.py` & `shodan-1.9.1/shodan/cli/worldmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 '''
 import curses
 import locale
 import random
 import time
 
+from shodan.exception import APIError
 from shodan.helpers import get_ip
 
 
 MAPS = {
     'world': {
         # offset (as (y, x) for curses...)
         'corners': (1, 4, 23, 73),
@@ -205,27 +206,30 @@
                 for banner in self.api.stream.banners():
                     if 'location' in banner and banner['location']['latitude']:
                         banners.append(banner)
                     if len(banners) >= 20:
                         break
                 self.data = banners
                 self.last_fetch = epoch_now
-            except StandardError:
+            except APIError:
                 raise
         return refresh
 
     def run(self, scr):
         """ Initialize and run the application """
         m = AsciiMap()
         curses.halfdelay(self.sleep)
         while True:
             now = int(time.time())
             refresh = self.fetch_data(now)
             m.set_data(self.data)
-            m.draw(scr)
+            try:
+                m.draw(scr)
+            except curses.error:
+                raise Exception('Terminal window too small')
             scr.addstr(0, 1, 'Shodan Radar', curses.A_BOLD)
             scr.addstr(0, 40, time.strftime("%c UTC", time.gmtime(now)).rjust(37), curses.A_BOLD)
 
             # Key Input
             # q     - Quit
             event = scr.getch()
             if event == ord('q'):
```

### Comparing `shodan-1.9.0/shodan/cli/helpers.py` & `shodan-1.9.1/shodan/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/cli/converter/csvc.py` & `shodan-1.9.1/shodan/cli/converter/csvc.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/cli/converter/excel.py` & `shodan-1.9.1/shodan/cli/converter/excel.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/cli/converter/images.py` & `shodan-1.9.1/shodan/cli/converter/images.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/cli/converter/kml.py` & `shodan-1.9.1/shodan/cli/converter/kml.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/cli/converter/geojson.py` & `shodan-1.9.1/shodan/cli/converter/geojson.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/client.py` & `shodan-1.9.1/shodan/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,17 +186,25 @@
 
         # Check that the API key wasn't rejected
         if data.status_code == 401:
             try:
                 # Return the actual error message if the API returned valid JSON
                 error = data.json()['error']
             except Exception as e:
-                error = 'Invalid API key'
+                # If the response looks like HTML then it's probably the 401 page that nginx returns
+                # for 401 responses by default
+                if data.text.startswith('<'):
+                    error = 'Invalid API key'
+                else:
+                    # Otherwise lets raise the error message
+                    error = u'{}'.format(e)
 
             raise APIError(error)
+        elif data.status_code == 403:
+            raise APIError('Access denied (403 Forbidden)')
 
         # Parse the text into JSON
         try:
             data = data.json()
         except:
             raise APIError('Unable to parse JSON response')
```

### Comparing `shodan-1.9.0/shodan/stream.py` & `shodan-1.9.1/shodan/stream.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/helpers.py` & `shodan-1.9.1/shodan/helpers.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/threatnet.py` & `shodan-1.9.1/shodan/threatnet.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/shodan/__main__.py` & `shodan-1.9.1/shodan/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 from shodan.cli.converter import CsvConverter, KmlConverter, GeoJsonConverter, ExcelConverter, ImagesConverter
 
 # Constants
 from shodan.cli.settings import SHODAN_CONFIG_DIR, COLORIZE_FIELDS
 
 # Helper methods
 from shodan.cli.helpers import get_api_key
+from shodan.cli.host import HOST_PRINT
 
 # Allow 3rd-parties to develop custom commands
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
 
 # Make "-h" work like "--help"
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
@@ -181,15 +182,15 @@
 
     # Make sure it's a valid API key
     key = key.strip()
     try:
         api = shodan.Shodan(key)
         test = api.info()
     except shodan.APIError as e:
-        raise click.ClickException('Invalid API key')
+        raise click.ClickException(e.value)
 
     # Store the API key in the user's directory
     keyfile = shodan_dir + '/api_key'
     with open(keyfile, 'w') as fout:
         fout.write(key.strip())
         click.echo(click.style('Successfully initialized', fg='green'))
 
@@ -208,15 +209,15 @@
     key = get_api_key()
 
     # Get the list
     api = shodan.Shodan(key)
     try:
         alerts = api.alerts()
         for alert in alerts:
-            click.echo('Removing {} ({})'.format(alert['name'], alert['id']))
+            click.echo(u'Removing {} ({})'.format(alert['name'], alert['id']))
             api.delete_alert(alert['id'])
     except shodan.APIError as e:
         raise click.ClickException(e.value)
     click.echo("Alerts deleted")
 
 @alert.command(name='create')
 @click.argument('name', metavar='<name>')
@@ -245,19 +246,19 @@
     api = shodan.Shodan(key)
     try:
         results = api.alerts(include_expired=expired)
     except shodan.APIError as e:
         raise click.ClickException(e.value)
 
     if len(results) > 0:
-        click.echo('# {:14} {:<21} {:<15s}'.format('Alert ID', 'Name', 'IP/ Network'))
+        click.echo(u'# {:14} {:<21} {:<15s}'.format('Alert ID', 'Name', 'IP/ Network'))
         # click.echo('#' * 65)
         for alert in results:
             click.echo(
-                '{:16} {:<30} {:<35} '.format(
+                u'{:16} {:<30} {:<35} '.format(
                     click.style(alert['id'],  fg='yellow'),
                     click.style(alert['name'], fg='cyan'),
                     click.style(', '.join(alert['filters']['ip']), fg='white')
                 ),
                 nl=False
             )
 
@@ -322,15 +323,15 @@
     api = shodan.Shodan(key)
 
     if dataset:
         # Show the files within this dataset
         files = api.data.list_files(dataset)
 
         for file in files:
-            click.echo(click.style('{:20s}'.format(file['name']), fg='cyan'), nl=False)
+            click.echo(click.style(u'{:20s}'.format(file['name']), fg='cyan'), nl=False)
             click.echo(click.style('{:10s}'.format(helpers.humanize_bytes(file['size'])), fg='yellow'), nl=False)
             click.echo('{}'.format(file['url']))
     else:
         # If no dataset was provided then show a list of all datasets
         datasets = api.data.list_datasets()
 
         for ds in datasets:
@@ -453,119 +454,29 @@
         # Let the user know we're done
         if count < limit:
             click.echo(click.style('Notice: fewer results were saved than requested', 'yellow'))
         click.echo(click.style('Saved %s results into file %s' % (count, filename), 'green'))
 
 
 @main.command()
-@click.option('--format', help='The output format for the host information. Possible values are: pretty, csv, tsv. (placeholder)', default='pretty', type=str)
+@click.option('--format', help='The output format for the host information. Possible values are: pretty, tsv.', default='pretty', type=click.Choice(['pretty', 'tsv']))
 @click.option('--history', help='Show the complete history of the host.', default=False, is_flag=True)
 @click.option('--filename', '-O', help='Save the host information in the given file (append if file exists).', default=None)
 @click.option('--save', '-S', help='Save the host information in the a file named after the IP (append if file exists).', default=False, is_flag=True)
 @click.argument('ip', metavar='<ip address>')
 def host(format, history, filename, save, ip):
     """View all available information for an IP address"""
     key = get_api_key()
     api = shodan.Shodan(key)
 
     try:
         host = api.host(ip, history=history)
 
-        # General info
-        click.echo(click.style(ip, fg='green'))
-        if len(host['hostnames']) > 0:
-            click.echo('{:25s}{}'.format('Hostnames:', ';'.join(host['hostnames'])))
-
-        if 'city' in host and host['city']:
-            click.echo('{:25s}{}'.format('City:', host['city']))
-
-        if 'country_name' in host and host['country_name']:
-            click.echo('{:25s}{}'.format('Country:', host['country_name']))
-
-        if 'os' in host and host['os']:
-            click.echo('{:25s}{}'.format('Operating System:', host['os']))
-
-        if 'org' in host and host['org']:
-            click.echo('{:25s}{}'.format('Organization:', host['org']))
-
-        if 'last_update' in host and host['last_update']:
-            click.echo('{:25s}{}'.format('Updated:', host['last_update']))
-
-        click.echo('{:25s}{}'.format('Number of open ports:', len(host['ports'])))
-
-        # Output the vulnerabilities the host has
-        if 'vulns' in host and len(host['vulns']) > 0:
-            vulns = []
-            for vuln in host['vulns']:
-                if vuln.startswith('!'):
-                    continue
-                if vuln.upper() == 'CVE-2014-0160':
-                    vulns.append(click.style('Heartbleed', fg='red'))
-                else:
-                    vulns.append(click.style(vuln, fg='red'))
-
-            if len(vulns) > 0:
-                click.echo('{:25s}'.format('Vulnerabilities:'), nl=False)
-
-                for vuln in vulns:
-                    click.echo(vuln + '\t', nl=False)
-
-                click.echo('')
-
-        click.echo('')
-
-        # If the user doesn't have access to SSL/ Telnet results then we need
-        # to pad the host['data'] property with empty banners so they still see
-        # the port listed as open. (#63)
-        if len(host['ports']) != len(host['data']):
-            # Find the ports the user can't see the data for
-            ports = host['ports']
-            for banner in host['data']:
-                if banner['port'] in ports:
-                    ports.remove(banner['port'])
-
-            # Add the placeholder banners
-            for port in ports:
-                banner = {
-                    'port': port,
-                    'transport': 'tcp', # All the filtered services use TCP
-                    'timestamp': host['data'][-1]['timestamp'], # Use the timestamp of the oldest banner
-                    'placeholder': True, # Don't store this banner when the file is saved
-                }
-                host['data'].append(banner)
-
-        click.echo('Ports:')
-        for banner in sorted(host['data'], key=lambda k: k['port']):
-            product = ''
-            version = ''
-            if 'product' in banner and banner['product']:
-                product = banner['product']
-            if 'version' in banner and banner['version']:
-                version = '({})'.format(banner['version'])
-
-            click.echo(click.style('{:>7d}'.format(banner['port']), fg='cyan'), nl=False)
-            click.echo('/', nl=False)
-            click.echo(click.style('{} '.format(banner['transport']), fg='yellow'), nl=False)
-            click.echo('{} {}'.format(product, version), nl=False)
-
-            if history:
-                # Format the timestamp to only show the year-month-day
-                date = banner['timestamp'][:10]
-                click.echo(click.style('\t\t({})'.format(date), fg='white', dim=True), nl=False)
-            click.echo('')
-
-            # Show optional ssl info
-            if 'ssl' in banner:
-                if 'versions' in banner['ssl'] and banner['ssl']['versions']:
-                    click.echo('\t|-- SSL Versions: {}'.format(', '.join([version for version in sorted(banner['ssl']['versions']) if not version.startswith('-')])))
-                if 'dhparams' in banner['ssl'] and banner['ssl']['dhparams']:
-                    click.echo('\t|-- Diffie-Hellman Parameters:')
-                    click.echo('\t\t{:15s}{}\n\t\t{:15s}{}'.format('Bits:', banner['ssl']['dhparams']['bits'], 'Generator:', banner['ssl']['dhparams']['generator']))
-                    if 'fingerprint' in banner['ssl']['dhparams']:
-                        click.echo('\t\t{:15s}{}'.format('Fingerprint:', banner['ssl']['dhparams']['fingerprint']))
+        # Print the host information to the terminal using the user-specified format
+        HOST_PRINT[format](host, history=history)
 
         # Store the results
         if filename or save:
             if save:
                 filename = '{}.json.gz'.format(ip)
 
             # Add the appropriate extension if it's not there atm
@@ -1324,15 +1235,21 @@
 @main.command()
 def radar():
     """Real-Time Map of some results as Shodan finds them."""
     key = get_api_key()
     api = shodan.Shodan(key)
 
     from shodan.cli.worldmap import launch_map
-    launch_map(api)
+
+    try:
+        launch_map(api)
+    except shodan.APIError as e:
+        raise click.ClickException(e.value)
+    except Exception as e:
+        raise click.ClickException(u'{}'.format(e))
 
 def async_spinner(finished):
     spinner = itertools.cycle(['-', '/', '|', '\\'])
     while not finished.is_set():
         sys.stdout.write('\b{}'.format(next(spinner)))
         sys.stdout.flush()
         finished.wait(0.2)
```

### Comparing `shodan-1.9.0/docs/examples/gifcreator.rst` & `shodan-1.9.1/docs/examples/gifcreator.rst`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/docs/examples/cert-stream.rst` & `shodan-1.9.1/docs/examples/cert-stream.rst`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/docs/examples/query-summary.rst` & `shodan-1.9.1/docs/examples/query-summary.rst`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/docs/examples/basic-search.rst` & `shodan-1.9.1/docs/examples/basic-search.rst`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/docs/make.bat` & `shodan-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/docs/index.rst` & `shodan-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/docs/Makefile` & `shodan-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/docs/conf.py` & `shodan-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/docs/tutorial.rst` & `shodan-1.9.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `shodan-1.9.0/LICENSE` & `shodan-1.9.1/LICENSE`

 * *Files identical despite different names*

