# Comparing `tmp/cone.fileupload-0.7.tar.gz` & `tmp/cone.fileupload-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cone.fileupload-0.7.tar", last modified: Wed Jan 19 06:57:18 2022, max compression
+gzip compressed data, was "cone.fileupload-1.0a1.tar", last modified: Mon May 15 12:06:33 2023, max compression
```

## Comparing `cone.fileupload-0.7.tar` & `cone.fileupload-1.0a1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1373 2021-07-06 05:14:15.000000 cone.fileupload-0.7/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1360 2022-01-19 06:56:45.000000 cone.fileupload-0.7/setup.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1348 2022-01-19 06:56:39.000000 cone.fileupload-0.7/CHANGES.rst
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       97 2015-12-13 18:41:51.000000 cone.fileupload-0.7/MANIFEST.in
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       56 2015-12-13 18:41:50.000000 cone.fileupload-0.7/src/cone/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/fileupload/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1289 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/fileupload/browser/
--rw-rw-r--   0 rnix      (1000) rnix      (1000)      100 2015-12-13 18:41:50.000000 cone.fileupload-0.7/src/cone/fileupload/browser/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1041 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/toolbar.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5510 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/fileupload.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2829 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/actions.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      403 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3703 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload-validate.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5266 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload-process.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/vendor/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23520 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/vendor/jquery.ui.widget.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1030 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/vendor/tmpl.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    56631 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    24036 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload-ui.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      655 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8926 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.iframe-transport.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1279 2021-12-21 05:58:41.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2155 2021-12-21 05:58:40.000000 cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3706 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/templates.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1901 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/browser/fileupload.pt
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/fileupload/locale/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2314 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/locale/cone.fileupload.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/fileupload/locale/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone/fileupload/locale/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2549 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1152 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6844 2021-12-13 12:52:55.000000 cone.fileupload-0.7/src/cone/fileupload/tests.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone.fileupload.egg-info/
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     1576 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone.fileupload.egg-info/SOURCES.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)        5 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone.fileupload.egg-info/namespace_packages.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)        1 2015-12-13 18:41:51.000000 cone.fileupload-0.7/src/cone.fileupload.egg-info/not-zip-safe
--rw-rw-r--   0 rnix      (1000) rnix      (1000)        1 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone.fileupload.egg-info/dependency_links.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       51 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone.fileupload.egg-info/requires.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)        5 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone.fileupload.egg-info/top_level.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     9524 2022-01-19 06:57:18.000000 cone.fileupload-0.7/src/cone.fileupload.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4312 2021-12-13 12:52:55.000000 cone.fileupload-0.7/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2022-01-19 06:57:18.000000 cone.fileupload-0.7/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9524 2022-01-19 06:57:18.000000 cone.fileupload-0.7/PKG-INFO
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1539 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7704 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4307 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1362 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      483 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/browser/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3322 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2829 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/actions.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1901 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/fileupload.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5510 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/fileupload.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/fileupload/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      403 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/fileupload/cone.fileupload.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2155 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/fileupload/cone.fileupload.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1279 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/fileupload/cone.fileupload.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5266 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-process.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    24036 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-ui.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3703 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-validate.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      655 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    56631 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8926 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.iframe-transport.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/vendor/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23520 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/vendor/jquery.ui.widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1030 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/vendor/tmpl.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3706 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/templates.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1041 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/browser/toolbar.pt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/locale/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2314 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/locale/cone.fileupload.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/locale/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone/fileupload/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1152 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2549 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10873 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone/fileupload/tests.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:06:33.009538 cone.fileupload-1.0a1/src/cone.fileupload.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7704 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone.fileupload.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1690 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone.fileupload.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone.fileupload.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone.fileupload.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone.fileupload.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       51 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone.fileupload.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2023-05-15 12:06:32.000000 cone.fileupload-1.0a1/src/cone.fileupload.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cone.fileupload-0.7/LICENSE.rst` & `cone.fileupload-1.0a1/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 License
 =======
 
 Copyright (c) 2013-2021, BlueDynamics Alliance, Austria
-Copyright (c) 2021, Cone Contributors
+Copyright (c) 2021-2022, Cone Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `cone.fileupload-0.7/setup.py` & `cone.fileupload-1.0a1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '0.7'
+version = '1.0a1'
 shortdesc = 'jQuery File Upload integration for cone.app'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `cone.fileupload-0.7/CHANGES.rst` & `cone.fileupload-1.0a1/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 =======
 
+1.0a1 (2023-05-15)
+------------------
+
+- Use ``webresource`` for resource registration.
+  [rnix]
+
+- Replace deprecated use of ``allow_non_node_children`` by ``child_constraints``.
+  [rnix]
+
+
 0.7 (2022-01-19)
 ----------------
 
 - Modernize JavaScript setup.
 
 - Add ``i18n_messages_src``, ``upload_template_src`` and
   ``download_template_src`` attributes to ``FileUploadTile``.
```

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/toolbar.pt` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/toolbar.pt`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/fileupload.py` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/fileupload.py`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/actions.py` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/actions.py`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload-validate.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-validate.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload-process.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-process.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/vendor/jquery.ui.widget.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/vendor/jquery.ui.widget.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/vendor/tmpl.min.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/vendor/tmpl.min.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload-ui.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-ui.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.fileupload.css` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload.css`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload/jquery.iframe-transport.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/jquery-fileupload/jquery.iframe-transport.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload.min.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/fileupload/cone.fileupload.min.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/static/fileupload.js` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/static/fileupload/cone.fileupload.js`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/templates.py` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/templates.py`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/browser/fileupload.pt` & `cone.fileupload-1.0a1/src/cone/fileupload/browser/fileupload.pt`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/locale/cone.fileupload.pot` & `cone.fileupload-1.0a1/src/cone/fileupload/locale/cone.fileupload.pot`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.po` & `cone.fileupload-1.0a1/src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.po`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.mo` & `cone.fileupload-1.0a1/src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.mo`

 * *Files identical despite different names*

### Comparing `cone.fileupload-0.7/src/cone.fileupload.egg-info/SOURCES.txt` & `cone.fileupload-1.0a1/src/cone.fileupload.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 src/cone/__init__.py
 src/cone.fileupload.egg-info/PKG-INFO
 src/cone.fileupload.egg-info/SOURCES.txt
 src/cone.fileupload.egg-info/dependency_links.txt
 src/cone.fileupload.egg-info/namespace_packages.txt
 src/cone.fileupload.egg-info/not-zip-safe
@@ -15,21 +16,21 @@
 src/cone/fileupload/tests.py
 src/cone/fileupload/browser/__init__.py
 src/cone/fileupload/browser/actions.py
 src/cone/fileupload/browser/fileupload.pt
 src/cone/fileupload/browser/fileupload.py
 src/cone/fileupload/browser/templates.py
 src/cone/fileupload/browser/toolbar.pt
-src/cone/fileupload/browser/static/fileupload.css
-src/cone/fileupload/browser/static/fileupload.js
-src/cone/fileupload/browser/static/fileupload.min.js
-src/cone/fileupload/browser/static/fileupload/jquery.fileupload-process.js
-src/cone/fileupload/browser/static/fileupload/jquery.fileupload-ui.js
-src/cone/fileupload/browser/static/fileupload/jquery.fileupload-validate.js
-src/cone/fileupload/browser/static/fileupload/jquery.fileupload.css
-src/cone/fileupload/browser/static/fileupload/jquery.fileupload.js
-src/cone/fileupload/browser/static/fileupload/jquery.iframe-transport.js
-src/cone/fileupload/browser/static/fileupload/vendor/jquery.ui.widget.js
-src/cone/fileupload/browser/static/fileupload/vendor/tmpl.min.js
+src/cone/fileupload/browser/static/fileupload/cone.fileupload.css
+src/cone/fileupload/browser/static/fileupload/cone.fileupload.js
+src/cone/fileupload/browser/static/fileupload/cone.fileupload.min.js
+src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-process.js
+src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-ui.js
+src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload-validate.js
+src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload.css
+src/cone/fileupload/browser/static/jquery-fileupload/jquery.fileupload.js
+src/cone/fileupload/browser/static/jquery-fileupload/jquery.iframe-transport.js
+src/cone/fileupload/browser/static/jquery-fileupload/vendor/jquery.ui.widget.js
+src/cone/fileupload/browser/static/jquery-fileupload/vendor/tmpl.min.js
 src/cone/fileupload/locale/cone.fileupload.pot
 src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.mo
 src/cone/fileupload/locale/de/LC_MESSAGES/cone.fileupload.po
```

### Comparing `cone.fileupload-0.7/src/cone.fileupload.egg-info/PKG-INFO` & `cone.fileupload-1.0a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,277 @@
 Metadata-Version: 2.1
 Name: cone.fileupload
-Version: 0.7
+Version: 1.0a1
 Summary: jQuery File Upload integration for cone.app
 Home-page: http://github.com/conestack/cone.fileuplaod
 Author: Cone Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
-Description: .. image:: https://img.shields.io/pypi/v/cone.fileupload.svg
-            :target: https://pypi.python.org/pypi/cone.fileupload
-            :alt: Latest PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/cone.fileupload.svg
-            :target: https://pypi.python.org/pypi/cone.fileupload
-            :alt: Number of PyPI downloads
-        
-        .. image:: https://travis-ci.org/bluedynamics/cone.fileupload.svg?branch=master
-            :target: https://travis-ci.org/bluedynamics/cone.fileupload
-        
-        .. image:: https://coveralls.io/repos/github/bluedynamics/cone.fileupload/badge.svg?branch=master
-            :target: https://coveralls.io/github/bluedynamics/cone.fileupload?branch=master
-        
-        This package integrates
-        `jQueryFileUpload <https://github.com/blueimp/jQuery-File-Upload>`_ in cone.
-        
-        Currently, version 10.32.0 is included.
-        
-        Included files of jQuery File Upload:
-        
-        * jquery.iframe-transport.js
-        * jquery.fileupload.js
-        * jquery.fileupload-process.js
-        * jquery.fileupload-ui.js
-        * jquery.fileupload-validate.js
-        
-        Additionally, v3.20.0 of
-        `Javascript-Templates <https://github.com/blueimp/JavaScript-Templates>`_
-        is included.
-        
-        
-        Usage
-        -----
-        
-        Since ``cone.app`` not knows about the underlying data, ``cone.fileupload``
-        only provides an abstract server implementation.
-        
-        So first we need to provide a model.
-        
-        .. code-block:: python
-        
-            from cone.app.model import BaseNode
-            from pyramid.security import ALL_PERMISSIONS
-            from pyramid.security import Allow
-            from pyramid.security import Deny
-            from pyramid.security import Everyone
-        
-            ACL = [
-                (Allow, 'role:manager', ['add', 'delete']),
-                (Allow, Everyone, ['login']),
-                (Deny, Everyone, ALL_PERMISSIONS),
-            ]
-        
-            class Container(BaseNode):
-                __acl__ = ACL
-        
-                def __call__(self):
-                    """Persistence happens here.
-                    """
-        
-            class File(BaseNode):
-                __acl__ = ACL
-                # allow setting any value types
-                allow_non_node_children = True
-        
-        Now we need to provide a concrete ``FileUploadHandle`` implementation for
-        our model.
-        
-        .. code-block:: python
-        
-            from cone.fileupload.browser.fileupload import FileUploadHandle
-            from pyramid.view import view_config
-        
-            @view_config(
-                name='fileupload_handle',
-                context=Container, # <- here the view gets bound to our model
-                accept='application/json',
-                renderer='json',
-                permission='add')
-            class ContainerFileUploadHandle(FileUploadHandle):
-        
-                def create_file(self, stream, filename, mimetype):
-                    # this function gets called for persisting uploaded files
-                    file = self.model[filename] = File()
-                    file['body'] = stream.read()
-                    return {
-                        'name': filename,
-                        'size': len(file['body']),
-                        'view_url': '/{0}'.format(file.name),
-                        'download_url': '/{0}/download'.format(file.name),
-                        'delete_url': '/{0}/filedelete_handle'.format(file.name),
-                        'delete_type': 'GET',
-                    }
-        
-                def read_existing(self):
-                    # this function gets called for initial reading of existing files
-                    files = list()
-                    for node in self.model.values():
-                        files.append({
-                            'name': node.name,
-                            'size': len(node['body']),
-                            'view_url': '/{0}'.format(node.name),
-                            'download_url': '/{0}/download'.format(node.name),
-                            'delete_url': '/{0}/filedelete_handle'.format(node.name),
-                            'delete_type': 'GET',
-                        })
-                    return files
-        
-        Optionally we might want to provide a custom fileupload tile for our model.
-        
-        .. code-block:: python
-        
-            from cone.tile import tile
-            from cone.fileupload.browser.fileupload import FileUploadTile
-        
-            @tile(
-                name='fileupload',
-                path='cone.fileupload:browser/fileupload.pt',
-                interface=Container,
-                permission='add')
-            class ContainerFileUploadTile(FileUploadTile):
-                accept_file_types = r'/(\.|\/)(gif|jpg)$/i'
-        
-        The file upload actions are either rendered as dedicated tile by name
-        ``fileupload_toolbar`` or integrated into the context menu. If it's desired to
-        display the action in the context menu, ``fileupload_contextmenu_actions``
-        flag must be set on model ``properties``.
-        
-        
-        Contributors
-        ============
-        
-        - Robert Niederreiter
-        
-        
-        Changes
-        =======
-        
-        0.7 (2022-01-19)
-        ----------------
-        
-        - Modernize JavaScript setup.
-        
-        - Add ``i18n_messages_src``, ``upload_template_src`` and
-          ``download_template_src`` attributes to ``FileUploadTile``.
-        
-        - Add optional ``download_url`` to file data dict.
-        
-        - Remove ``thumbnailUrl`` from file data dict.
-        
-        **Breaking Changes**
-        
-        - Rename ``url`` to ``view_url`` in file data dict.
-        
-        - Rename ``deleteUrl`` to ``delete_url`` in file data dict.
-        
-        - Rename ``deleteType`` to ``delete_type`` in file data dict.
-        
-        
-        0.6 (2021-11-21)
-        ----------------
-        
-        - Fileupload actions optionally work from contextmenu.
-          [rnix]
-        
-        - Move button toolbar into dedicated tile for customization.
-          [rnix]
-        
-        - Reduce included files and plugins of jquery fileupload to required ones.
-          [rnix]
-        
-        - Update jquery fileupload to version 10.32.0.
-          [rnix]
-        
-        
-        0.5 (2021-11-08)
-        ----------------
-        
-        - Rename deprecated ``allow_non_node_childs`` to ``allow_non_node_children``
-          in tests and documentation.
-          [rnix]
-        
-        
-        0.4 (2020-05-30)
-        ----------------
-        
-        - Initial pypi release
-          [rnix]
-        
-        
-        0.3
-        ---
-        
-        - Python 3 compatibility.
-          [rnix]
-        
-        - Convert doctests to unittests.
-          [rnix]
-        
-        - Use ``cone.app.main_hook`` decorator.
-          [rnix]
-        
-        - Move resource registration to main hook.
-          [rnix]
-        
-        - Upgrade to ``cone.app`` 1.0b1.
-          [rnix]
-        
-        
-        0.2
-        ---
-        
-        - Code organization.
-          [rnix]
-        
-        
-        0.1
-        ---
-        
-        - Make it work
-          [rnix]
-        
-        
-        License
-        =======
-        
-        Copyright (c) 2013-2021, BlueDynamics Alliance, Austria
-        Copyright (c) 2021, Cone Contributors
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice, this
-          list of conditions and the following disclaimer in the documentation and/or
-          other materials provided with the distribution.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-        ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-        (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-        SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
 Keywords: node pyramid cone web
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Provides-Extra: test
+License-File: LICENSE.rst
+
+.. image:: https://img.shields.io/pypi/v/cone.fileupload.svg
+    :target: https://pypi.python.org/pypi/cone.fileupload
+    :alt: Latest PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/cone.fileupload.svg
+    :target: https://pypi.python.org/pypi/cone.fileupload
+    :alt: Number of PyPI downloads
+
+.. image:: https://travis-ci.org/bluedynamics/cone.fileupload.svg?branch=master
+    :target: https://travis-ci.org/bluedynamics/cone.fileupload
+
+.. image:: https://coveralls.io/repos/github/bluedynamics/cone.fileupload/badge.svg?branch=master
+    :target: https://coveralls.io/github/bluedynamics/cone.fileupload?branch=master
+
+This package integrates
+`jQueryFileUpload <https://github.com/blueimp/jQuery-File-Upload>`_ in cone.
+
+Currently, version 10.32.0 is included.
+
+Included files of jQuery File Upload:
+
+* jquery.iframe-transport.js
+* jquery.fileupload.js
+* jquery.fileupload-process.js
+* jquery.fileupload-ui.js
+* jquery.fileupload-validate.js
+
+Additionally, v3.20.0 of
+`Javascript-Templates <https://github.com/blueimp/JavaScript-Templates>`_
+is included.
+
+
+Usage
+-----
+
+Since ``cone.app`` not knows about the underlying data, ``cone.fileupload``
+only provides an abstract server implementation.
+
+So first we need to provide a model.
+
+.. code-block:: python
+
+    from cone.app.model import BaseNode
+    from pyramid.security import ALL_PERMISSIONS
+    from pyramid.security import Allow
+    from pyramid.security import Deny
+    from pyramid.security import Everyone
+
+    ACL = [
+        (Allow, 'role:manager', ['add', 'delete']),
+        (Allow, Everyone, ['login']),
+        (Deny, Everyone, ALL_PERMISSIONS),
+    ]
+
+    class Container(BaseNode):
+        __acl__ = ACL
+
+        def __call__(self):
+            """Persistence happens here.
+            """
+
+    class File(BaseNode):
+        __acl__ = ACL
+
+        # allow setting any value types
+        child_constraints = None
+
+Now we need to provide a concrete ``FileUploadHandle`` implementation for
+our model.
+
+.. code-block:: python
+
+    from cone.fileupload.browser.fileupload import FileUploadHandle
+    from pyramid.view import view_config
+
+    @view_config(
+        name='fileupload_handle',
+        context=Container, # <- here the view gets bound to our model
+        accept='application/json',
+        renderer='json',
+        permission='add')
+    class ContainerFileUploadHandle(FileUploadHandle):
+
+        def create_file(self, stream, filename, mimetype):
+            # this function gets called for persisting uploaded files
+            file = self.model[filename] = File()
+            file['body'] = stream.read()
+            return {
+                'name': filename,
+                'size': len(file['body']),
+                'view_url': '/{0}'.format(file.name),
+                'download_url': '/{0}/download'.format(file.name),
+                'delete_url': '/{0}/filedelete_handle'.format(file.name),
+                'delete_type': 'GET',
+            }
+
+        def read_existing(self):
+            # this function gets called for initial reading of existing files
+            files = list()
+            for node in self.model.values():
+                files.append({
+                    'name': node.name,
+                    'size': len(node['body']),
+                    'view_url': '/{0}'.format(node.name),
+                    'download_url': '/{0}/download'.format(node.name),
+                    'delete_url': '/{0}/filedelete_handle'.format(node.name),
+                    'delete_type': 'GET',
+                })
+            return files
+
+Optionally we might want to provide a custom fileupload tile for our model.
+
+.. code-block:: python
+
+    from cone.tile import tile
+    from cone.fileupload.browser.fileupload import FileUploadTile
+
+    @tile(
+        name='fileupload',
+        path='cone.fileupload:browser/fileupload.pt',
+        interface=Container,
+        permission='add')
+    class ContainerFileUploadTile(FileUploadTile):
+        accept_file_types = r'/(\.|\/)(gif|jpg)$/i'
+
+The file upload actions are either rendered as dedicated tile by name
+``fileupload_toolbar`` or integrated into the context menu. If it's desired to
+display the action in the context menu, ``fileupload_contextmenu_actions``
+flag must be set on model ``properties``.
+
+
+Contributors
+============
+
+- Robert Niederreiter
+
+
+Changes
+=======
+
+1.0a1 (2023-05-15)
+------------------
+
+- Use ``webresource`` for resource registration.
+  [rnix]
+
+- Replace deprecated use of ``allow_non_node_children`` by ``child_constraints``.
+  [rnix]
+
+
+0.7 (2022-01-19)
+----------------
+
+- Modernize JavaScript setup.
+
+- Add ``i18n_messages_src``, ``upload_template_src`` and
+  ``download_template_src`` attributes to ``FileUploadTile``.
+
+- Add optional ``download_url`` to file data dict.
+
+- Remove ``thumbnailUrl`` from file data dict.
+
+**Breaking Changes**
+
+- Rename ``url`` to ``view_url`` in file data dict.
+
+- Rename ``deleteUrl`` to ``delete_url`` in file data dict.
+
+- Rename ``deleteType`` to ``delete_type`` in file data dict.
+
+
+0.6 (2021-11-21)
+----------------
+
+- Fileupload actions optionally work from contextmenu.
+  [rnix]
+
+- Move button toolbar into dedicated tile for customization.
+  [rnix]
+
+- Reduce included files and plugins of jquery fileupload to required ones.
+  [rnix]
+
+- Update jquery fileupload to version 10.32.0.
+  [rnix]
+
+
+0.5 (2021-11-08)
+----------------
+
+- Rename deprecated ``allow_non_node_childs`` to ``allow_non_node_children``
+  in tests and documentation.
+  [rnix]
+
+
+0.4 (2020-05-30)
+----------------
+
+- Initial pypi release
+  [rnix]
+
+
+0.3
+---
+
+- Python 3 compatibility.
+  [rnix]
+
+- Convert doctests to unittests.
+  [rnix]
+
+- Use ``cone.app.main_hook`` decorator.
+  [rnix]
+
+- Move resource registration to main hook.
+  [rnix]
+
+- Upgrade to ``cone.app`` 1.0b1.
+  [rnix]
+
+
+0.2
+---
+
+- Code organization.
+  [rnix]
+
+
+0.1
+---
+
+- Make it work
+  [rnix]
+
+
+License
+=======
+
+Copyright (c) 2013-2021, BlueDynamics Alliance, Austria
+Copyright (c) 2021-2022, Cone Contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `cone.fileupload-0.7/README.rst` & `cone.fileupload-1.0a1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 
         def __call__(self):
             """Persistence happens here.
             """
 
     class File(BaseNode):
         __acl__ = ACL
+
         # allow setting any value types
-        allow_non_node_children = True
+        child_constraints = None
 
 Now we need to provide a concrete ``FileUploadHandle`` implementation for
 our model.
 
 .. code-block:: python
 
     from cone.fileupload.browser.fileupload import FileUploadHandle
```

### Comparing `cone.fileupload-0.7/PKG-INFO` & `cone.fileupload-1.0a1/src/cone.fileupload.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,277 @@
 Metadata-Version: 2.1
 Name: cone.fileupload
-Version: 0.7
+Version: 1.0a1
 Summary: jQuery File Upload integration for cone.app
 Home-page: http://github.com/conestack/cone.fileuplaod
 Author: Cone Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
-Description: .. image:: https://img.shields.io/pypi/v/cone.fileupload.svg
-            :target: https://pypi.python.org/pypi/cone.fileupload
-            :alt: Latest PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/cone.fileupload.svg
-            :target: https://pypi.python.org/pypi/cone.fileupload
-            :alt: Number of PyPI downloads
-        
-        .. image:: https://travis-ci.org/bluedynamics/cone.fileupload.svg?branch=master
-            :target: https://travis-ci.org/bluedynamics/cone.fileupload
-        
-        .. image:: https://coveralls.io/repos/github/bluedynamics/cone.fileupload/badge.svg?branch=master
-            :target: https://coveralls.io/github/bluedynamics/cone.fileupload?branch=master
-        
-        This package integrates
-        `jQueryFileUpload <https://github.com/blueimp/jQuery-File-Upload>`_ in cone.
-        
-        Currently, version 10.32.0 is included.
-        
-        Included files of jQuery File Upload:
-        
-        * jquery.iframe-transport.js
-        * jquery.fileupload.js
-        * jquery.fileupload-process.js
-        * jquery.fileupload-ui.js
-        * jquery.fileupload-validate.js
-        
-        Additionally, v3.20.0 of
-        `Javascript-Templates <https://github.com/blueimp/JavaScript-Templates>`_
-        is included.
-        
-        
-        Usage
-        -----
-        
-        Since ``cone.app`` not knows about the underlying data, ``cone.fileupload``
-        only provides an abstract server implementation.
-        
-        So first we need to provide a model.
-        
-        .. code-block:: python
-        
-            from cone.app.model import BaseNode
-            from pyramid.security import ALL_PERMISSIONS
-            from pyramid.security import Allow
-            from pyramid.security import Deny
-            from pyramid.security import Everyone
-        
-            ACL = [
-                (Allow, 'role:manager', ['add', 'delete']),
-                (Allow, Everyone, ['login']),
-                (Deny, Everyone, ALL_PERMISSIONS),
-            ]
-        
-            class Container(BaseNode):
-                __acl__ = ACL
-        
-                def __call__(self):
-                    """Persistence happens here.
-                    """
-        
-            class File(BaseNode):
-                __acl__ = ACL
-                # allow setting any value types
-                allow_non_node_children = True
-        
-        Now we need to provide a concrete ``FileUploadHandle`` implementation for
-        our model.
-        
-        .. code-block:: python
-        
-            from cone.fileupload.browser.fileupload import FileUploadHandle
-            from pyramid.view import view_config
-        
-            @view_config(
-                name='fileupload_handle',
-                context=Container, # <- here the view gets bound to our model
-                accept='application/json',
-                renderer='json',
-                permission='add')
-            class ContainerFileUploadHandle(FileUploadHandle):
-        
-                def create_file(self, stream, filename, mimetype):
-                    # this function gets called for persisting uploaded files
-                    file = self.model[filename] = File()
-                    file['body'] = stream.read()
-                    return {
-                        'name': filename,
-                        'size': len(file['body']),
-                        'view_url': '/{0}'.format(file.name),
-                        'download_url': '/{0}/download'.format(file.name),
-                        'delete_url': '/{0}/filedelete_handle'.format(file.name),
-                        'delete_type': 'GET',
-                    }
-        
-                def read_existing(self):
-                    # this function gets called for initial reading of existing files
-                    files = list()
-                    for node in self.model.values():
-                        files.append({
-                            'name': node.name,
-                            'size': len(node['body']),
-                            'view_url': '/{0}'.format(node.name),
-                            'download_url': '/{0}/download'.format(node.name),
-                            'delete_url': '/{0}/filedelete_handle'.format(node.name),
-                            'delete_type': 'GET',
-                        })
-                    return files
-        
-        Optionally we might want to provide a custom fileupload tile for our model.
-        
-        .. code-block:: python
-        
-            from cone.tile import tile
-            from cone.fileupload.browser.fileupload import FileUploadTile
-        
-            @tile(
-                name='fileupload',
-                path='cone.fileupload:browser/fileupload.pt',
-                interface=Container,
-                permission='add')
-            class ContainerFileUploadTile(FileUploadTile):
-                accept_file_types = r'/(\.|\/)(gif|jpg)$/i'
-        
-        The file upload actions are either rendered as dedicated tile by name
-        ``fileupload_toolbar`` or integrated into the context menu. If it's desired to
-        display the action in the context menu, ``fileupload_contextmenu_actions``
-        flag must be set on model ``properties``.
-        
-        
-        Contributors
-        ============
-        
-        - Robert Niederreiter
-        
-        
-        Changes
-        =======
-        
-        0.7 (2022-01-19)
-        ----------------
-        
-        - Modernize JavaScript setup.
-        
-        - Add ``i18n_messages_src``, ``upload_template_src`` and
-          ``download_template_src`` attributes to ``FileUploadTile``.
-        
-        - Add optional ``download_url`` to file data dict.
-        
-        - Remove ``thumbnailUrl`` from file data dict.
-        
-        **Breaking Changes**
-        
-        - Rename ``url`` to ``view_url`` in file data dict.
-        
-        - Rename ``deleteUrl`` to ``delete_url`` in file data dict.
-        
-        - Rename ``deleteType`` to ``delete_type`` in file data dict.
-        
-        
-        0.6 (2021-11-21)
-        ----------------
-        
-        - Fileupload actions optionally work from contextmenu.
-          [rnix]
-        
-        - Move button toolbar into dedicated tile for customization.
-          [rnix]
-        
-        - Reduce included files and plugins of jquery fileupload to required ones.
-          [rnix]
-        
-        - Update jquery fileupload to version 10.32.0.
-          [rnix]
-        
-        
-        0.5 (2021-11-08)
-        ----------------
-        
-        - Rename deprecated ``allow_non_node_childs`` to ``allow_non_node_children``
-          in tests and documentation.
-          [rnix]
-        
-        
-        0.4 (2020-05-30)
-        ----------------
-        
-        - Initial pypi release
-          [rnix]
-        
-        
-        0.3
-        ---
-        
-        - Python 3 compatibility.
-          [rnix]
-        
-        - Convert doctests to unittests.
-          [rnix]
-        
-        - Use ``cone.app.main_hook`` decorator.
-          [rnix]
-        
-        - Move resource registration to main hook.
-          [rnix]
-        
-        - Upgrade to ``cone.app`` 1.0b1.
-          [rnix]
-        
-        
-        0.2
-        ---
-        
-        - Code organization.
-          [rnix]
-        
-        
-        0.1
-        ---
-        
-        - Make it work
-          [rnix]
-        
-        
-        License
-        =======
-        
-        Copyright (c) 2013-2021, BlueDynamics Alliance, Austria
-        Copyright (c) 2021, Cone Contributors
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice, this
-          list of conditions and the following disclaimer in the documentation and/or
-          other materials provided with the distribution.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-        ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-        (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-        SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
 Keywords: node pyramid cone web
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Provides-Extra: test
+License-File: LICENSE.rst
+
+.. image:: https://img.shields.io/pypi/v/cone.fileupload.svg
+    :target: https://pypi.python.org/pypi/cone.fileupload
+    :alt: Latest PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/cone.fileupload.svg
+    :target: https://pypi.python.org/pypi/cone.fileupload
+    :alt: Number of PyPI downloads
+
+.. image:: https://travis-ci.org/bluedynamics/cone.fileupload.svg?branch=master
+    :target: https://travis-ci.org/bluedynamics/cone.fileupload
+
+.. image:: https://coveralls.io/repos/github/bluedynamics/cone.fileupload/badge.svg?branch=master
+    :target: https://coveralls.io/github/bluedynamics/cone.fileupload?branch=master
+
+This package integrates
+`jQueryFileUpload <https://github.com/blueimp/jQuery-File-Upload>`_ in cone.
+
+Currently, version 10.32.0 is included.
+
+Included files of jQuery File Upload:
+
+* jquery.iframe-transport.js
+* jquery.fileupload.js
+* jquery.fileupload-process.js
+* jquery.fileupload-ui.js
+* jquery.fileupload-validate.js
+
+Additionally, v3.20.0 of
+`Javascript-Templates <https://github.com/blueimp/JavaScript-Templates>`_
+is included.
+
+
+Usage
+-----
+
+Since ``cone.app`` not knows about the underlying data, ``cone.fileupload``
+only provides an abstract server implementation.
+
+So first we need to provide a model.
+
+.. code-block:: python
+
+    from cone.app.model import BaseNode
+    from pyramid.security import ALL_PERMISSIONS
+    from pyramid.security import Allow
+    from pyramid.security import Deny
+    from pyramid.security import Everyone
+
+    ACL = [
+        (Allow, 'role:manager', ['add', 'delete']),
+        (Allow, Everyone, ['login']),
+        (Deny, Everyone, ALL_PERMISSIONS),
+    ]
+
+    class Container(BaseNode):
+        __acl__ = ACL
+
+        def __call__(self):
+            """Persistence happens here.
+            """
+
+    class File(BaseNode):
+        __acl__ = ACL
+
+        # allow setting any value types
+        child_constraints = None
+
+Now we need to provide a concrete ``FileUploadHandle`` implementation for
+our model.
+
+.. code-block:: python
+
+    from cone.fileupload.browser.fileupload import FileUploadHandle
+    from pyramid.view import view_config
+
+    @view_config(
+        name='fileupload_handle',
+        context=Container, # <- here the view gets bound to our model
+        accept='application/json',
+        renderer='json',
+        permission='add')
+    class ContainerFileUploadHandle(FileUploadHandle):
+
+        def create_file(self, stream, filename, mimetype):
+            # this function gets called for persisting uploaded files
+            file = self.model[filename] = File()
+            file['body'] = stream.read()
+            return {
+                'name': filename,
+                'size': len(file['body']),
+                'view_url': '/{0}'.format(file.name),
+                'download_url': '/{0}/download'.format(file.name),
+                'delete_url': '/{0}/filedelete_handle'.format(file.name),
+                'delete_type': 'GET',
+            }
+
+        def read_existing(self):
+            # this function gets called for initial reading of existing files
+            files = list()
+            for node in self.model.values():
+                files.append({
+                    'name': node.name,
+                    'size': len(node['body']),
+                    'view_url': '/{0}'.format(node.name),
+                    'download_url': '/{0}/download'.format(node.name),
+                    'delete_url': '/{0}/filedelete_handle'.format(node.name),
+                    'delete_type': 'GET',
+                })
+            return files
+
+Optionally we might want to provide a custom fileupload tile for our model.
+
+.. code-block:: python
+
+    from cone.tile import tile
+    from cone.fileupload.browser.fileupload import FileUploadTile
+
+    @tile(
+        name='fileupload',
+        path='cone.fileupload:browser/fileupload.pt',
+        interface=Container,
+        permission='add')
+    class ContainerFileUploadTile(FileUploadTile):
+        accept_file_types = r'/(\.|\/)(gif|jpg)$/i'
+
+The file upload actions are either rendered as dedicated tile by name
+``fileupload_toolbar`` or integrated into the context menu. If it's desired to
+display the action in the context menu, ``fileupload_contextmenu_actions``
+flag must be set on model ``properties``.
+
+
+Contributors
+============
+
+- Robert Niederreiter
+
+
+Changes
+=======
+
+1.0a1 (2023-05-15)
+------------------
+
+- Use ``webresource`` for resource registration.
+  [rnix]
+
+- Replace deprecated use of ``allow_non_node_children`` by ``child_constraints``.
+  [rnix]
+
+
+0.7 (2022-01-19)
+----------------
+
+- Modernize JavaScript setup.
+
+- Add ``i18n_messages_src``, ``upload_template_src`` and
+  ``download_template_src`` attributes to ``FileUploadTile``.
+
+- Add optional ``download_url`` to file data dict.
+
+- Remove ``thumbnailUrl`` from file data dict.
+
+**Breaking Changes**
+
+- Rename ``url`` to ``view_url`` in file data dict.
+
+- Rename ``deleteUrl`` to ``delete_url`` in file data dict.
+
+- Rename ``deleteType`` to ``delete_type`` in file data dict.
+
+
+0.6 (2021-11-21)
+----------------
+
+- Fileupload actions optionally work from contextmenu.
+  [rnix]
+
+- Move button toolbar into dedicated tile for customization.
+  [rnix]
+
+- Reduce included files and plugins of jquery fileupload to required ones.
+  [rnix]
+
+- Update jquery fileupload to version 10.32.0.
+  [rnix]
+
+
+0.5 (2021-11-08)
+----------------
+
+- Rename deprecated ``allow_non_node_childs`` to ``allow_non_node_children``
+  in tests and documentation.
+  [rnix]
+
+
+0.4 (2020-05-30)
+----------------
+
+- Initial pypi release
+  [rnix]
+
+
+0.3
+---
+
+- Python 3 compatibility.
+  [rnix]
+
+- Convert doctests to unittests.
+  [rnix]
+
+- Use ``cone.app.main_hook`` decorator.
+  [rnix]
+
+- Move resource registration to main hook.
+  [rnix]
+
+- Upgrade to ``cone.app`` 1.0b1.
+  [rnix]
+
+
+0.2
+---
+
+- Code organization.
+  [rnix]
+
+
+0.1
+---
+
+- Make it work
+  [rnix]
+
+
+License
+=======
+
+Copyright (c) 2013-2021, BlueDynamics Alliance, Austria
+Copyright (c) 2021-2022, Cone Contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

