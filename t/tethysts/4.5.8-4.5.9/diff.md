# Comparing `tmp/tethysts-4.5.8.tar.gz` & `tmp/tethysts-4.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tethysts-4.5.8.tar", last modified: Sun Nov 27 05:33:23 2022, max compression
+gzip compressed data, was "tethysts-4.5.9.tar", last modified: Sun Nov 27 08:13:01 2022, max compression
```

## Comparing `tethysts-4.5.8.tar` & `tethysts-4.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-27 05:33:23.304763 tethysts-4.5.8/
--rw-rw-rw-   0 mike      (1000) mike      (1000)    11357 2020-11-05 20:00:10.000000 tethysts-4.5.8/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      565 2022-11-27 05:33:23.304763 tethysts-4.5.8/PKG-INFO
--rw-rw-rw-   0 mike      (1000) mike      (1000)      234 2021-04-16 08:55:33.000000 tethysts-4.5.8/README.rst
--rw-rw-rw-   0 mike      (1000) mike      (1000)      104 2022-02-11 06:19:22.000000 tethysts-4.5.8/pyproject.toml
--rw-rw-rw-   0 mike      (1000) mike      (1000)       67 2022-11-27 05:33:23.308763 tethysts-4.5.8/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7336 2022-11-27 05:32:34.000000 tethysts-4.5.8/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-27 05:33:23.304763 tethysts-4.5.8/tethysts/
--rw-rw-rw-   0 mike      (1000) mike      (1000)       60 2020-12-31 21:46:07.000000 tethysts-4.5.8/tethysts/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    22155 2022-11-27 04:38:08.000000 tethysts-4.5.8/tethysts/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-27 05:33:23.304763 tethysts-4.5.8/tethysts/tests/
--rw-rw-rw-   0 mike      (1000) mike      (1000)      208 2020-11-05 20:00:10.000000 tethysts-4.5.8/tethysts/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6111 2022-11-08 06:04:34.000000 tethysts-4.5.8/tethysts/tests/test_tethysts.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    19181 2022-11-27 05:17:30.000000 tethysts-4.5.8/tethysts/tests/utest_tethysts.py
--rw-rw-rw-   0 mike      (1000) mike      (1000)     6567 2021-05-07 07:48:29.000000 tethysts-4.5.8/tethysts/tests/working.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    28955 2022-11-27 04:36:55.000000 tethysts-4.5.8/tethysts/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-27 05:33:23.304763 tethysts-4.5.8/tethysts.egg-info/
--rw-rw-rw-   0 mike      (1000) mike      (1000)      565 2022-11-27 05:33:23.000000 tethysts-4.5.8/tethysts.egg-info/PKG-INFO
--rw-rw-rw-   0 mike      (1000) mike      (1000)      385 2022-11-27 05:33:23.000000 tethysts-4.5.8/tethysts.egg-info/SOURCES.txt
--rw-rw-rw-   0 mike      (1000) mike      (1000)        1 2022-11-27 05:33:23.000000 tethysts-4.5.8/tethysts.egg-info/dependency_links.txt
--rw-rw-rw-   0 mike      (1000) mike      (1000)      115 2022-11-27 05:33:23.000000 tethysts-4.5.8/tethysts.egg-info/requires.txt
--rw-rw-rw-   0 mike      (1000) mike      (1000)        9 2022-11-27 05:33:23.000000 tethysts-4.5.8/tethysts.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-27 08:13:01.106809 tethysts-4.5.9/
+-rw-rw-rw-   0 mike      (1000) mike      (1000)    11357 2020-11-05 20:00:10.000000 tethysts-4.5.9/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      565 2022-11-27 08:13:01.106809 tethysts-4.5.9/PKG-INFO
+-rw-rw-rw-   0 mike      (1000) mike      (1000)      234 2021-04-16 08:55:33.000000 tethysts-4.5.9/README.rst
+-rw-rw-rw-   0 mike      (1000) mike      (1000)      104 2022-02-11 06:19:22.000000 tethysts-4.5.9/pyproject.toml
+-rw-rw-rw-   0 mike      (1000) mike      (1000)       67 2022-11-27 08:13:01.110809 tethysts-4.5.9/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7336 2022-11-27 08:12:22.000000 tethysts-4.5.9/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-27 08:13:01.106809 tethysts-4.5.9/tethysts/
+-rw-rw-rw-   0 mike      (1000) mike      (1000)       60 2020-12-31 21:46:07.000000 tethysts-4.5.9/tethysts/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    22155 2022-11-27 04:38:08.000000 tethysts-4.5.9/tethysts/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-27 08:13:01.106809 tethysts-4.5.9/tethysts/tests/
+-rw-rw-rw-   0 mike      (1000) mike      (1000)      208 2020-11-05 20:00:10.000000 tethysts-4.5.9/tethysts/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6111 2022-11-08 06:04:34.000000 tethysts-4.5.9/tethysts/tests/test_tethysts.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    19181 2022-11-27 05:17:30.000000 tethysts-4.5.9/tethysts/tests/utest_tethysts.py
+-rw-rw-rw-   0 mike      (1000) mike      (1000)     6567 2021-05-07 07:48:29.000000 tethysts-4.5.9/tethysts/tests/working.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    29459 2022-11-27 08:05:42.000000 tethysts-4.5.9/tethysts/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-27 08:13:01.106809 tethysts-4.5.9/tethysts.egg-info/
+-rw-rw-rw-   0 mike      (1000) mike      (1000)      565 2022-11-27 08:13:01.000000 tethysts-4.5.9/tethysts.egg-info/PKG-INFO
+-rw-rw-rw-   0 mike      (1000) mike      (1000)      385 2022-11-27 08:13:01.000000 tethysts-4.5.9/tethysts.egg-info/SOURCES.txt
+-rw-rw-rw-   0 mike      (1000) mike      (1000)        1 2022-11-27 08:13:01.000000 tethysts-4.5.9/tethysts.egg-info/dependency_links.txt
+-rw-rw-rw-   0 mike      (1000) mike      (1000)      115 2022-11-27 08:13:01.000000 tethysts-4.5.9/tethysts.egg-info/requires.txt
+-rw-rw-rw-   0 mike      (1000) mike      (1000)        9 2022-11-27 08:13:01.000000 tethysts-4.5.9/tethysts.egg-info/top_level.txt
```

### Comparing `tethysts-4.5.8/LICENSE` & `tethysts-4.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tethysts-4.5.8/PKG-INFO` & `tethysts-4.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tethysts
-Version: 4.5.8
+Version: 4.5.9
 Summary: tethys time series S3 extraction
 Home-page: https://github.com/tethys-ts/tethysts
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: tethys
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tethysts-4.5.8/setup.py` & `tethysts-4.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'tethysts'
 main_package = 'tethysts'
 datasets = 'datasets/time_series'
-version = '4.5.8'
+version = '4.5.9'
 descrip = 'tethys time series S3 extraction'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

### Comparing `tethysts-4.5.8/tethysts/main.py` & `tethysts-4.5.9/tethysts/main.py`

 * *Files identical despite different names*

### Comparing `tethysts-4.5.8/tethysts/tests/test_tethysts.py` & `tethysts-4.5.9/tethysts/tests/test_tethysts.py`

 * *Files identical despite different names*

### Comparing `tethysts-4.5.8/tethysts/tests/utest_tethysts.py` & `tethysts-4.5.9/tethysts/tests/utest_tethysts.py`

 * *Files identical despite different names*

### Comparing `tethysts-4.5.8/tethysts/tests/working.py` & `tethysts-4.5.9/tethysts/tests/working.py`

 * *Files identical despite different names*

### Comparing `tethysts-4.5.8/tethysts/utils.py` & `tethysts-4.5.9/tethysts/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -852,14 +852,37 @@
                 del c1
             else:
                 raise TypeError('Dataset data should be either an ndarray or a MemoryCachedArray.')
 
     return xr3
 
 
+def filter_mod_dates(results, from_mod_date=None, to_mod_date=None):
+    """
+    Need to do this because xarray "where" is useless...
+    """
+    if ((from_mod_date is not None) or (to_mod_date is not None)) and ('modified_date' in results):
+        mod_dates = results['modified_date'].copy().load()
+
+        if (from_mod_date is not None) and (to_mod_date is not None):
+            mod_bool = (mod_dates >= pd.Timestamp(from_mod_date)) & (mod_dates <= pd.Timestamp(to_mod_date))
+        elif (from_mod_date is not None):
+            mod_bool = (mod_dates >= pd.Timestamp(from_mod_date))
+        elif (to_mod_date is not None):
+            mod_bool = (mod_dates <= pd.Timestamp(to_mod_date))
+
+        data_vars1 = [var for var in results.data_vars if 'time' in results[var].dims]
+
+        results[data_vars1] = results[data_vars1].where(mod_bool)
+
+        return results.dropna('time', how='all')
+    else:
+        return results
+
+
 def results_concat(results_list, output_path=None, from_date=None, to_date=None, from_mod_date=None, to_mod_date=None, compression='lzf'):
     """
 
     """
     if output_path is None:
         output_path = io.BytesIO()
         compression = 'zstd'
@@ -868,24 +891,15 @@
     h1 = result_filters(h1, from_date, to_date)
     h1.to_hdf5(output_path, compression=compression)
 
     xr3 = xr.open_dataset(output_path, engine='h5netcdf', cache=False)
 
     ## Deal with mod dates filters
     if ((from_mod_date is not None) or (to_mod_date is not None)) and ('modified_date' in xr3):
-        mod_dates = xr3['modified_date'].copy().load()
-
-        if (from_mod_date is not None) and (to_mod_date is not None):
-            mod_bool = (mod_dates >= pd.Timestamp(from_mod_date)) & (mod_dates <= pd.Timestamp(to_mod_date))
-        elif (from_mod_date is not None):
-            mod_bool = (mod_dates >= pd.Timestamp(from_mod_date))
-        elif (to_mod_date is not None):
-            mod_bool = (mod_dates <= pd.Timestamp(to_mod_date))
-
-        xr3 = xr3.where(mod_bool, drop=True)
+        xr3 = filter_mod_dates(xr3, from_mod_date, to_mod_date)
 
     return xr3
```

### Comparing `tethysts-4.5.8/tethysts.egg-info/PKG-INFO` & `tethysts-4.5.9/tethysts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tethysts
-Version: 4.5.8
+Version: 4.5.9
 Summary: tethys time series S3 extraction
 Home-page: https://github.com/tethys-ts/tethysts
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: tethys
 Classifier: Development Status :: 3 - Alpha
```

