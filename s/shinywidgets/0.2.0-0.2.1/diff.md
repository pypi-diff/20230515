# Comparing `tmp/shinywidgets-0.2.0.tar.gz` & `tmp/shinywidgets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinywidgets-0.2.0.tar", last modified: Thu Apr 13 19:45:06 2023, max compression
+gzip compressed data, was "shinywidgets-0.2.1.tar", last modified: Mon May 15 15:38:46 2023, max compression
```

## Comparing `shinywidgets-0.2.0.tar` & `shinywidgets-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:45:06.750275 shinywidgets-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-13 19:45:06.750275 shinywidgets-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 19:45:06.750275 shinywidgets-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:45:06.742275 shinywidgets-0.2.0/shinywidgets/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_as_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_shinywidgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:45:06.746275 shinywidgets-0.2.0/shinywidgets/static/
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff
--rw-r--r--   0 runner    (1001) docker     (123)  3866031 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/libembed-amd.js
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js
--rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/output.js
--rw-r--r--   0 runner    (1001) docker     (123)  1006878 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:45:06.742275 shinywidgets-0.2.0/shinywidgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:38:46.683843 shinywidgets-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-15 15:38:46.683843 shinywidgets-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-15 15:38:46.683843 shinywidgets-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:38:46.675843 shinywidgets-0.2.1/shinywidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/_as_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/_shinywidgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:38:46.683843 shinywidgets-0.2.1/shinywidgets/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff
+-rw-r--r--   0 runner    (1001) docker     (123)  3866031 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/libembed-amd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/output.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1006878 2023-05-15 15:38:22.000000 shinywidgets-0.2.1/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:38:46.675843 shinywidgets-0.2.1/shinywidgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-15 15:38:46.000000 shinywidgets-0.2.1/shinywidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-15 15:38:46.000000 shinywidgets-0.2.1/shinywidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:38:46.000000 shinywidgets-0.2.1/shinywidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:38:46.000000 shinywidgets-0.2.1/shinywidgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 15:38:46.000000 shinywidgets-0.2.1/shinywidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 15:38:46.000000 shinywidgets-0.2.1/shinywidgets.egg-info/top_level.txt
```

### Comparing `shinywidgets-0.2.0/LICENSE` & `shinywidgets-0.2.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 RStudio, PBC
+Copyright (c) 2023 Posit Software, PBC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `shinywidgets-0.2.0/PKG-INFO` & `shinywidgets-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinywidgets
-Version: 0.2.0
+Version: 0.2.1
 Summary: Render ipywidgets in Shiny applications
 Home-page: https://github.com/rstudio/py-shinywidgets
 Author: Carson Sievert
 Author-email: carson@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shinywidgets/issues
 Project-URL: Documentation, https://github.com/rstudio/py-shinywidgets/
```

### Comparing `shinywidgets-0.2.0/README.md` & `shinywidgets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/setup.cfg` & `shinywidgets-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/_as_widget.py` & `shinywidgets-0.2.1/shinywidgets/_as_widget.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/_comm.py` & `shinywidgets-0.2.1/shinywidgets/_comm.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/_dependencies.py` & `shinywidgets-0.2.1/shinywidgets/_dependencies.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/_serialization.py` & `shinywidgets-0.2.1/shinywidgets/_serialization.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/_shinywidgets.py` & `shinywidgets-0.2.1/shinywidgets/_shinywidgets.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf` & `shinywidgets-0.2.1/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2` & `shinywidgets-0.2.1/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot` & `shinywidgets-0.2.1/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg` & `shinywidgets-0.2.1/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff` & `shinywidgets-0.2.1/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/libembed-amd.js` & `shinywidgets-0.2.1/shinywidgets/static/libembed-amd.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js` & `shinywidgets-0.2.1/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/output.js` & `shinywidgets-0.2.1/shinywidgets/static/output.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js` & `shinywidgets-0.2.1/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.2.0/shinywidgets.egg-info/PKG-INFO` & `shinywidgets-0.2.1/shinywidgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinywidgets
-Version: 0.2.0
+Version: 0.2.1
 Summary: Render ipywidgets in Shiny applications
 Home-page: https://github.com/rstudio/py-shinywidgets
 Author: Carson Sievert
 Author-email: carson@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shinywidgets/issues
 Project-URL: Documentation, https://github.com/rstudio/py-shinywidgets/
```

### Comparing `shinywidgets-0.2.0/shinywidgets.egg-info/SOURCES.txt` & `shinywidgets-0.2.1/shinywidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

