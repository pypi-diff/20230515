# Comparing `tmp/astro-elk-0.1.tar.gz` & `tmp/astro-elk-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-elk-0.1.tar", last modified: Mon May  8 21:38:29 2023, max compression
+gzip compressed data, was "astro-elk-0.2.tar", last modified: Mon May 15 21:43:20 2023, max compression
```

## Comparing `astro-elk-0.1.tar` & `astro-elk-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:29.339759 astro-elk-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 21:38:29.339759 astro-elk-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-08 21:38:15.000000 astro-elk-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:29.339759 astro-elk-0.1/astro_elk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:29.339759 astro-elk-0.1/elk/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 21:38:29.339759 astro-elk-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 21:38:16.000000 astro-elk-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:43:20.001366 astro-elk-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 21:43:20.001366 astro-elk-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-15 21:43:08.000000 astro-elk-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:43:20.001366 astro-elk-0.2/astro_elk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 21:43:19.000000 astro-elk-0.2/astro_elk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 21:43:19.000000 astro-elk-0.2/astro_elk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:43:19.000000 astro-elk-0.2/astro_elk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 21:43:19.000000 astro-elk-0.2/astro_elk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 21:43:19.000000 astro-elk-0.2/astro_elk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:43:20.001366 astro-elk-0.2/elk/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 21:43:08.000000 astro-elk-0.2/elk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 21:43:08.000000 astro-elk-0.2/elk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-05-15 21:43:08.000000 astro-elk-0.2/elk/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-15 21:43:08.000000 astro-elk-0.2/elk/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-15 21:43:08.000000 astro-elk-0.2/elk/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-15 21:43:08.000000 astro-elk-0.2/elk/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-15 21:43:08.000000 astro-elk-0.2/elk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 21:43:20.005365 astro-elk-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 21:43:08.000000 astro-elk-0.2/setup.py
```

### Comparing `astro-elk-0.1/PKG-INFO` & `astro-elk-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-elk
-Version: 0.1
+Version: 0.2
 Summary: This python package computes, and corrects ensemble light curves for TESS pixels within a specified aperature, from TESS FFI data.
 Home-page: https://github.com/tobin-wainer/TESS_Cluster_Project/
 Author: Tobin Wainer, Tom Wagg
 Author-email: tobinw@uw.edu
 License: MIT
 Platform: UNKNOWN
 Provides: elk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astro-elk Version: 0.1 Summary: This python package
+Metadata-Version: 2.1 Name: astro-elk Version: 0.2 Summary: This python package
 computes, and corrects ensemble light curves for TESS pixels within a specified
 aperature, from TESS FFI data. Home-page: https://github.com/tobin-wainer/
 TESS_Cluster_Project/ Author: Tobin Wainer, Tom Wagg Author-email:
 tobinw@uw.edu License: MIT Platform: UNKNOWN Provides: elk Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Provides-Extra: test Provides-
 Extra: docs
    src="https://raw.githubusercontent.com/tobin-wainer/elk/main/docs/_static/
```

### Comparing `astro-elk-0.1/README.md` & `astro-elk-0.2/README.md`

 * *Files identical despite different names*

### Comparing `astro-elk-0.1/astro_elk.egg-info/PKG-INFO` & `astro-elk-0.2/astro_elk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-elk
-Version: 0.1
+Version: 0.2
 Summary: This python package computes, and corrects ensemble light curves for TESS pixels within a specified aperature, from TESS FFI data.
 Home-page: https://github.com/tobin-wainer/TESS_Cluster_Project/
 Author: Tobin Wainer, Tom Wagg
 Author-email: tobinw@uw.edu
 License: MIT
 Platform: UNKNOWN
 Provides: elk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astro-elk Version: 0.1 Summary: This python package
+Metadata-Version: 2.1 Name: astro-elk Version: 0.2 Summary: This python package
 computes, and corrects ensemble light curves for TESS pixels within a specified
 aperature, from TESS FFI data. Home-page: https://github.com/tobin-wainer/
 TESS_Cluster_Project/ Author: Tobin Wainer, Tom Wagg Author-email:
 tobinw@uw.edu License: MIT Platform: UNKNOWN Provides: elk Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Provides-Extra: test Provides-
 Extra: docs
    src="https://raw.githubusercontent.com/tobin-wainer/elk/main/docs/_static/
```

### Comparing `astro-elk-0.1/elk/ensemble.py` & `astro-elk-0.2/elk/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
         Returns
         -------
         output_table : :class:`~astropy.table.Table`
             The full lightcurves output table that was saved
         """
         # if data is available and the lightcurves have not yet been calculated
-        if self.has_tess_data() and self.lcs == []:
+        if self.lcs == [] and self.has_tess_data():
             # download and correct lightcurves
             self.get_lcs()
 
         # ensure only unique sectors in scattered light list
         self.scattered_light_sectors = list(set(self.scattered_light_sectors))
 
         # write out the full file
```

### Comparing `astro-elk-0.1/elk/lightcurve.py` & `astro-elk-0.2/elk/lightcurve.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.1/elk/plot.py` & `astro-elk-0.2/elk/plot.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.1/elk/stats.py` & `astro-elk-0.2/elk/stats.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.1/elk/utils.py` & `astro-elk-0.2/elk/utils.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.1/setup.cfg` & `astro-elk-0.2/setup.cfg`

 * *Files identical despite different names*

