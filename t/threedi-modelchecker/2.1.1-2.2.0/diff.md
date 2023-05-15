# Comparing `tmp/threedi-modelchecker-2.1.1.tar.gz` & `tmp/threedi-modelchecker-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-modelchecker-2.1.1.tar", last modified: Mon May  8 13:57:24 2023, max compression
+gzip compressed data, was "threedi-modelchecker-2.2.0.tar", last modified: Mon May 15 16:01:49 2023, max compression
```

## Comparing `threedi-modelchecker-2.1.1.tar` & `threedi-modelchecker-2.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.678184 threedi-modelchecker-2.1.1/threedi_modelchecker/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.682184 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/geo_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    29978 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/checks/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    90598 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.682184 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface_gdal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface_rasterio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/model_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.686184 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/data/empty_v4.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_other.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-08 13:57:21.000000 threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_model_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:24.682184 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 13:57:24.000000 threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:49.556542 threedi-modelchecker-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-15 16:01:49.556542 threedi-modelchecker-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-15 16:01:49.556542 threedi-modelchecker-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:49.552542 threedi-modelchecker-2.2.0/threedi_modelchecker/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:49.556542 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/geo_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32989 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/checks/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94471 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:49.556542 threedi-modelchecker-2.2.0/threedi_modelchecker/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/interfaces/raster_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/interfaces/raster_interface_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/interfaces/raster_interface_rasterio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:49.556542 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:49.556542 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/data/empty_v4.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-15 16:01:43.000000 threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_model_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:01:49.552542 threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-15 16:01:49.000000 threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-15 16:01:49.000000 threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:01:49.000000 threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 16:01:49.000000 threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:01:49.000000 threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-15 16:01:49.000000 threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 16:01:49.000000 threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/top_level.txt
```

### Comparing `threedi-modelchecker-2.1.1/CHANGES.rst` & `threedi-modelchecker-2.2.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,52 @@
 Changelog of threedi-modelchecker
 =================================
 
 
+2.2.0 (2023-05-15)
+------------------
+
+- Added check 98: cross-section diameters must not be smaller than 0.1 m.
+
+- Changed check 324 to 1151, to keep the aggregation settings checks grouped together.
+
+- Clarified error message for check 206 and Use0DFlowCheck.
+
+- Added --ignore-checks option on the modelchecker check command to ignore all checks matching a regex pattern.
+
+- Added check 614 to make sure that no more than 50 surfaces are linked to a connection node.
+
+- Added check 1152 to ensure all aggregation setting timesteps are the same.
+
+- Added check 1153 to ensure all aggregation setting timesteps are less than the global settings timestep.
+
+- Added check 1154 to ensure aggregation settings are present with all the aggregation_method-flow_variable pairs listed in the docs.
+
+- Added checks 45 and 360 to ensure that channel, pipe and culvert dist_calc_points and global_settings dist_calc_points, respectively, are at least 5 metres.
+
+
 2.1.1 (2023-05-08)
 ------------------
 
 - Vegetation_drag column names have changed. Update column names in code.
 
 - Bump threedi-schema version to 0.217.0.
 
+- Raster checks 10001-10004 have been renamed to 1401-1404 to stay within 4 digits.
+
+- Added check 1227: if v2_control.control_id references an id, the table it references must contain that id.
+
+- Added check 56: the cross-sections on a channel must either all be open or all be closed.
+
+- Added check 63: pumpstation capacity and storage at the end node must be set so the water level doesn't rise more than 1 m/s.
+
+- Added check 613: the combined surface area linked to a connection node must not be more than 10000 m2.
+
+- Added check 8: all of the ids in the database must be a positive signed 32-bit integer.
+
 
 2.1.0 (2023-03-27)
 ------------------
 
 - Add support for designating beta features in threedi-schema. If a user puts a
   non-null value in a column marked as beta in threedi-schema, a BetaFeaturesCheck
   error 1300 will be raised by the modelchecker. The allow-beta flag has been added
```

### Comparing `threedi-modelchecker-2.1.1/LICENSE` & `threedi-modelchecker-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/PKG-INFO` & `threedi-modelchecker-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.1.1
+Version: 2.2.0
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.1.1/README.rst` & `threedi-modelchecker-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/setup.py` & `threedi-modelchecker-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/base.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/checks/base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/cross_section_definitions.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/checks/cross_section_definitions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from sqlalchemy.orm import Query
-from threedi_schema import models
+from threedi_schema import constants, models
 
 from .base import BaseCheck
 
 
 class CrossSectionBaseCheck(BaseCheck):
     """Base class for all cross section definition checks."""
 
@@ -315,7 +315,90 @@
             ):
                 invalids.append(record)
 
         return invalids
 
     def description(self):
         return f"{self.column_name} should be monotonically increasing for open YZ profiles. Perhaps this is actually a closed profile?"
+
+
+class CrossSectionMinimumDiameterCheck(CrossSectionBaseCheck):
+    """Check if cross section widths and heights are large enough"""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(column=models.CrossSectionDefinition.id, *args, **kwargs)
+
+    def get_invalid(self, session):
+        invalids = []
+        for record in self.to_check(session).filter(
+            (models.CrossSectionDefinition.width != None)
+            & (models.CrossSectionDefinition.width != "")
+        ):
+            try:
+                widths = [float(x) for x in record.width.split(" ")]
+                heights = (
+                    [float(x) for x in record.height.split(" ")]
+                    if record.height not in [None, ""]
+                    else []
+                )
+            except ValueError:
+                continue  # other check catches this
+
+            if record.shape.value == constants.CrossSectionShape.CLOSED_RECTANGLE.value:
+                max_height = max(heights)
+                max_width = max(widths)
+                configuration = "closed"
+            elif record.shape.value == constants.CrossSectionShape.RECTANGLE.value:
+                max_width = max(widths)
+                configuration = "open"
+            elif record.shape.value == constants.CrossSectionShape.CIRCLE.value:
+                # any value filled in for heights will be overwritten by the widths value, also in the simulation
+                max_height = max_width = max(widths)
+                configuration = "closed"
+            elif record.shape.value in [
+                constants.CrossSectionShape.EGG.value,
+                constants.CrossSectionShape.INVERTED_EGG.value,
+            ]:
+                # any value filled in for heights will be overwritten by 1.5 times the widths value, also in the simulation
+                max_width = max(widths)
+                max_height = 1.5 * max_width
+                configuration = "closed"
+            elif record.shape.value in [
+                constants.CrossSectionShape.TABULATED_RECTANGLE.value,
+                constants.CrossSectionShape.TABULATED_TRAPEZIUM.value,
+            ]:
+                last_width = widths[-1]
+                max_height = max(heights)
+                max_width = max(widths)
+                if last_width == 0:
+                    configuration = "closed"
+                elif last_width > 0:
+                    configuration = "open"
+                else:
+                    continue
+            elif record.shape.value == constants.CrossSectionShape.TABULATED_YZ.value:
+                # without the rounding, floating-point errors occur
+                max_width = round((max(widths) - min(widths)), 9)
+                max_height = round((max(heights) - min(heights)), 9)
+                first_width = widths[0]
+                last_width = widths[-1]
+                first_height = heights[0]
+                last_height = heights[-1]
+                if (first_width, first_height) == (last_width, last_height):
+                    configuration = "closed"
+                else:
+                    configuration = "open"
+
+            # See nens/threedi-modelchecker#251
+            minimum_diameter = 0.1
+            if configuration == "closed":
+                if (max_height < minimum_diameter) or (max_width < minimum_diameter):
+                    invalids.append(record)
+            # the profile height does not need checking on an open cross-section
+            elif configuration == "open":
+                if max_width < minimum_diameter:
+                    invalids.append(record)
+
+        return invalids
+
+    def description(self):
+        return "v2_cross_section_definition.width and/or height should probably be at least 0.1m"
```

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/factories.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/checks/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/geo_query.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/checks/geo_query.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/other.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/checks/other.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,52 @@
     .order_by(models.GlobalSetting.id)
     .limit(1)
     .scalar_subquery()
 )
 first_setting_filter = models.GlobalSetting.id == first_setting
 
 
+class CorrectAggregationSettingsExist(BaseCheck):
+    """Check if aggregation settings are correctly filled with aggregation_method and flow_variable as required"""
+
+    def __init__(
+        self,
+        aggregation_method: constants.AggregationMethod,
+        flow_variable: constants.FlowVariable,
+        *args,
+        **kwargs,
+    ):
+        super().__init__(column=models.GlobalSetting.id, *args, **kwargs)
+        self.aggregation_method = aggregation_method.value
+        self.flow_variable = flow_variable.value
+
+    def get_invalid(self, session: Session) -> List[NamedTuple]:
+        global_settings = self.to_check(session).filter(first_setting_filter)
+        correctly_defined = session.execute(
+            select(models.AggregationSettings)
+            .filter(
+                models.AggregationSettings.aggregation_method
+                == self.aggregation_method,
+                models.AggregationSettings.flow_variable == self.flow_variable,
+            )
+            .filter(
+                models.AggregationSettings.global_settings_id
+                == global_settings.subquery().c.id
+            )
+        ).all()
+
+        return global_settings.all() if len(correctly_defined) == 0 else []
+
+    def description(self) -> str:
+        return (
+            "To use the water balance tool, v2_aggregation_settings should have a row where "
+            f"aggregation_method is {self.aggregation_method} and flow_variable is {self.flow_variable}."
+        )
+
+
 class CrossSectionLocationCheck(BaseCheck):
     """Check if cross section locations are within {max_distance} of their channel."""
 
     def __init__(self, max_distance, *args, **kwargs):
         super().__init__(column=models.CrossSectionLocation.the_geom, *args, **kwargs)
         self.max_distance = max_distance
 
@@ -231,16 +269,16 @@
                 invalid_rows.append(row)
             else:
                 continue
         return invalid_rows
 
     def description(self):
         return (
-            "When %s is used, there should exist at least one "
-            "(impervious) surface." % self.column
+            f"When {self.column_name} is used, there should exist at least one "
+            "(impervious) surface."
         )
 
 
 class ConnectionNodes(BaseCheck):
     """Check that all connection nodes are connected to at least one of the
     following objects:
     - Culvert
@@ -260,25 +298,34 @@
 
 class ConnectionNodesLength(BaseCheck):
     """Check that the distance between `start_node` and `end_node` is at least
     `min_distance`. The coords will be transformed into (the first entry) of
     GlobalSettings.epsg_code.
     """
 
-    def __init__(self, start_node, end_node, min_distance: float, *args, **kwargs):
+    def __init__(
+        self,
+        start_node,
+        end_node,
+        min_distance: float,
+        recommended_distance: float = 1.0,
+        *args,
+        **kwargs,
+    ):
         """
 
         :param start_node: column name of the start node
         :param end_node: column name of the end node
         :param min_distance: minimum required distance between start and end node
         """
         super().__init__(*args, **kwargs)
         self.start_node = start_node
         self.end_node = end_node
         self.min_distance = min_distance
+        self.recommended_distance = recommended_distance
 
     def get_invalid(self, session):
         start_node = aliased(models.ConnectionNode)
         end_node = aliased(models.ConnectionNode)
         q = (
             Query(self.column.class_)
             .join(start_node, self.start_node)
@@ -288,15 +335,15 @@
             )
         )
         return list(q.with_session(session).all())
 
     def description(self) -> str:
         return (
             f"The length of {self.table} is "
-            f"very short (< {self.min_distance}). A length of at least 1.0 m is recommended."
+            f"very short (< {self.min_distance}). A length of at least {self.recommended_distance} m is recommended to avoid timestep reduction."
         )
 
 
 class ConnectionNodesDistance(BaseCheck):
     """Check that the distance between connection nodes is above a certain
     threshold
     """
@@ -762,14 +809,53 @@
             .all()
         )
 
     def description(self) -> str:
         return f"{self.column_name} has a an associated inflow area larger than 10000 m2; this might be an error."
 
 
+class NodeSurfaceConnectionsCheck(BaseCheck):
+    """Check that no more than 50 surfaces are mapped to a connection node"""
+
+    def __init__(
+        self,
+        check_type: Literal["impervious", "pervious"] = "impervious",
+        *args,
+        **kwargs,
+    ):
+        super().__init__(column=models.ConnectionNode.id, *args, **kwargs)
+
+        self.surface_column = None
+        if check_type == "impervious":
+            self.surface_column = models.ImperviousSurfaceMap
+        elif check_type == "pervious":
+            self.surface_column = models.SurfaceMap
+
+    def get_invalid(self, session: Session) -> List[NamedTuple]:
+        if self.surface_column is None:
+            return []
+
+        overloaded_connections = (
+            select(self.surface_column.connection_node_id)
+            .group_by(self.surface_column.connection_node_id)
+            .having(func.count(self.surface_column.connection_node_id) > 50)
+        ).subquery()
+
+        return (
+            session.query(models.ConnectionNode)
+            .filter(
+                models.ConnectionNode.id == overloaded_connections.c.connection_node_id
+            )
+            .all()
+        )
+
+    def description(self) -> str:
+        return f"{self.column_name} has more than 50 surface areas mapped to it; this might be an error."
+
+
 class BetaColumnsCheck(BaseCheck):
     """Check that no beta columns were used in the database"""
 
     def get_invalid(self, session: Session) -> List[NamedTuple]:
         return session.query(self.table).filter(self.column.isnot(None)).all()
 
     def description(self) -> str:
```

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/raster.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/checks/raster.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/checks/timeseries.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/checks/timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/config.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     CrossSectionExpectEmptyCheck,
     CrossSectionFirstElementNonZeroCheck,
     CrossSectionFirstElementZeroCheck,
     CrossSectionFloatCheck,
     CrossSectionFloatListCheck,
     CrossSectionGreaterZeroCheck,
     CrossSectionIncreasingCheck,
+    CrossSectionMinimumDiameterCheck,
     CrossSectionNullCheck,
     CrossSectionYZCoordinateCountCheck,
     CrossSectionYZHeightCheck,
     CrossSectionYZIncreasingWidthIfOpenCheck,
 )
 from .checks.factories import (
     generate_enum_checks,
@@ -42,18 +43,20 @@
 from .checks.other import (
     BetaColumnsCheck,
     BetaValuesCheck,
     BoundaryCondition1DObjectNumberCheck,
     ChannelManholeLevelCheck,
     ConnectionNodesDistance,
     ConnectionNodesLength,
+    CorrectAggregationSettingsExist,
     CrossSectionLocationCheck,
     CrossSectionSameConfigurationCheck,
     ImperviousNodeInflowAreaCheck,
     LinestringLocationCheck,
+    NodeSurfaceConnectionsCheck,
     OpenChannelsWithNestedNewton,
     PerviousNodeInflowAreaCheck,
     PotentialBreachInterdistanceCheck,
     PotentialBreachStartEndCheck,
     PumpStorageTimestepCheck,
     SpatialIndexCheck,
     Use0DFlowCheck,
@@ -289,14 +292,25 @@
         column=models.ConnectionNode.storage_area,
         invalid=Query(models.ConnectionNode)
         .join(models.Manhole)
         .filter(models.ConnectionNode.storage_area < 0),
         message="v2_connection_nodes.storage_area is not greater than or equal to 0",
     ),
 ]
+CHECKS += [
+    RangeCheck(
+        error_code=45,
+        level=CheckLevel.WARNING,
+        column=table.dist_calc_points,
+        min_value=5,
+        left_inclusive=True,
+        message=f"{table.__tablename__}.dist_calc_points should preferably be at least 5.0 metres to prevent simulation timestep reduction.",
+    )
+    for table in [models.Channel, models.Pipe, models.Culvert]
+]
 
 
 ## 005x: CROSS SECTIONS
 
 CHECKS += [
     CrossSectionLocationCheck(
         level=CheckLevel.WARNING, max_distance=TOLERANCE_M, error_code=52
@@ -551,14 +565,18 @@
         error_code=96,
         shapes=(constants.CrossSectionShape.TABULATED_YZ,),
     ),
     CrossSectionYZIncreasingWidthIfOpenCheck(
         error_code=97,
         shapes=(constants.CrossSectionShape.TABULATED_YZ,),
     ),
+    CrossSectionMinimumDiameterCheck(
+        error_code=98,
+        level=CheckLevel.WARNING,
+    ),
 ]
 
 
 ## 01xx: LEVEL CHECKS
 
 CHECKS += [
     QueryCheck(
@@ -692,53 +710,55 @@
 
 CHECKS += [ConnectionNodesDistance(error_code=201, minimum_distance=0.001)]
 CHECKS += [
     QueryCheck(
         error_code=202,
         level=CheckLevel.WARNING,
         column=table.id,
-        invalid=Query(table).filter(geo_query.length(table.the_geom) < 0.05),
-        message=f"Length of a {table} is very short (< 0.05 m). A length of at least 1.0 m is recommended.",
+        invalid=Query(table).filter(geo_query.length(table.the_geom) < 5),
+        message=f"The length of {table.__tablename__} is very short (< 5 m). A length of at least 5.0 m is recommended to avoid timestep reduction.",
     )
     for table in [models.Channel, models.Culvert]
 ]
 CHECKS += [
     ConnectionNodesLength(
         error_code=203,
         level=CheckLevel.WARNING,
         column=models.Pipe.id,
         start_node=models.Pipe.connection_node_start,
         end_node=models.Pipe.connection_node_end,
-        min_distance=0.05,
+        min_distance=5.0,
+        recommended_distance=5.0,
     )
 ]
 CHECKS += [
     ConnectionNodesLength(
         error_code=204,
         level=CheckLevel.WARNING,
         column=table.id,
         filters=table.crest_type == constants.CrestType.BROAD_CRESTED,
         start_node=table.connection_node_start,
         end_node=table.connection_node_end,
-        min_distance=0.05,
+        min_distance=5.0,
+        recommended_distance=5.0,
     )
     for table in [models.Orifice, models.Weir]
 ]
 CHECKS += [
     LinestringLocationCheck(error_code=205, column=table.the_geom, max_distance=1)
     for table in [models.Channel, models.Culvert]
 ]
 CHECKS += [
     QueryCheck(
         error_code=206,
         column=models.ConnectionNode.the_geom_linestring,
         invalid=Query(models.ConnectionNode).filter(
             models.ConnectionNode.the_geom_linestring != None
         ),
-        message="The 'the_geom_linestring' column of v2_connection_nodes must be NULL",
+        message=f"{models.ConnectionNode.the_geom_linestring} must be NULL",
     )
 ]
 CHECKS += [
     SpatialIndexCheck(
         error_code=207, column=models.ConnectionNode.the_geom, level=CheckLevel.WARNING
     )
 ]
@@ -1198,22 +1218,14 @@
         invalid=Query(models.GlobalSetting).filter(
             first_setting_filter,
             models.GlobalSetting.maximum_table_step_size
             < models.GlobalSetting.table_step_size,
         ),
         message="v2_global_settings.maximum_table_step_size should be greater than v2_global_settings.table_step_size.",
     ),
-    UniqueCheck(
-        error_code=324,
-        level=CheckLevel.WARNING,
-        columns=(
-            models.AggregationSettings.flow_variable,
-            models.AggregationSettings.aggregation_method,
-        ),
-    ),
     QueryCheck(
         error_code=325,
         level=CheckLevel.WARNING,
         column=models.GlobalSetting.interception_global,
         invalid=Query(models.GlobalSetting).filter(
             first_setting_filter,
             ~is_none_or_empty(models.GlobalSetting.interception_file),
@@ -1272,14 +1284,25 @@
             models.GlobalSetting.interflow_settings_id,
             models.GlobalSetting.simple_infiltration_settings_id,
             models.GlobalSetting.groundwater_settings_id,
             models.GlobalSetting.vegetation_drag_settings_id,
         ]
     )
 ]
+CHECKS += [
+    RangeCheck(
+        error_code=360,
+        level=CheckLevel.WARNING,
+        column=models.GlobalSetting.dist_calc_points,
+        filters=first_setting_filter,
+        min_value=5.0,
+        left_inclusive=True,  # 0 itself is not allowed
+        message="v2_global_settings.dist_calc_points should preferably be at least 5.0 metres to prevent simulation timestep reduction.",
+    )
+]
 
 ## 04xx: Groundwater, Interflow & Infiltration
 CHECKS += [
     RangeCheck(
         error_code=401,
         column=models.Interflow.porosity,
         filters=interflow_filter,
@@ -1856,14 +1879,26 @@
     ImperviousNodeInflowAreaCheck(
         error_code=613, level=CheckLevel.WARNING, filters=CONDITIONS["0d_imp"].exists()
     ),
     PerviousNodeInflowAreaCheck(
         error_code=613, level=CheckLevel.WARNING, filters=CONDITIONS["0d_surf"].exists()
     ),
 ]
+CHECKS += [
+    NodeSurfaceConnectionsCheck(
+        check_type=check_type,
+        error_code=614,
+        level=CheckLevel.WARNING,
+        filters=CONDITIONS[filter_key].exists(),
+    )
+    for check_type, filter_key in [
+        ("pervious", "0d_surf"),
+        ("impervious", "0d_imp"),
+    ]
+]
 
 
 CHECKS += [
     RangeCheck(
         error_code=606,
         column=models.SurfaceParameter.outflow_delay,
         min_value=0,
@@ -2368,14 +2403,82 @@
             & (
                 models.AggregationSettings.flow_variable.notin_(
                     ("volume", "interception")
                 )
             )
         ),
         message="v2_aggregation_settings.aggregation_method can only be 'current' for 'volume' or 'interception' flow_variables.",
+    ),
+    UniqueCheck(
+        error_code=1151,
+        level=CheckLevel.WARNING,
+        columns=(
+            models.AggregationSettings.flow_variable,
+            models.AggregationSettings.aggregation_method,
+        ),
+    ),
+    AllEqualCheck(
+        error_code=1152,
+        level=CheckLevel.WARNING,
+        column=models.AggregationSettings.timestep,
+    ),
+    QueryCheck(
+        error_code=1153,
+        level=CheckLevel.WARNING,
+        column=models.AggregationSettings.timestep,
+        invalid=Query(models.AggregationSettings)
+        .join(
+            models.GlobalSetting,
+            models.AggregationSettings.global_settings_id == models.GlobalSetting.id,
+        )
+        .filter(first_setting_filter)
+        .filter(
+            models.AggregationSettings.timestep < models.GlobalSetting.output_time_step
+        ),
+        message="v2_aggregation_settings.timestep is smaller than v2_global_settings.output_time_step",
+    ),
+]
+CHECKS += [
+    CorrectAggregationSettingsExist(
+        error_code=1154,
+        level=CheckLevel.WARNING,
+        aggregation_method=aggregation_method,
+        flow_variable=flow_variable,
+    )
+    for (aggregation_method, flow_variable) in (
+        (constants.AggregationMethod.CUMULATIVE, constants.FlowVariable.PUMP_DISCHARGE),
+        (
+            constants.AggregationMethod.CUMULATIVE,
+            constants.FlowVariable.LATERAL_DISCHARGE,
+        ),
+        (
+            constants.AggregationMethod.CUMULATIVE,
+            constants.FlowVariable.SIMPLE_INFILTRATION,
+        ),
+        (constants.AggregationMethod.CUMULATIVE, constants.FlowVariable.RAIN),
+        (constants.AggregationMethod.CUMULATIVE, constants.FlowVariable.LEAKAGE),
+        (constants.AggregationMethod.CURRENT, constants.FlowVariable.INTERCEPTION),
+        (constants.AggregationMethod.CUMULATIVE, constants.FlowVariable.DISCHARGE),
+        (
+            constants.AggregationMethod.CUMULATIVE_NEGATIVE,
+            constants.FlowVariable.DISCHARGE,
+        ),
+        (
+            constants.AggregationMethod.CUMULATIVE_POSITIVE,
+            constants.FlowVariable.DISCHARGE,
+        ),
+        (constants.AggregationMethod.CURRENT, constants.FlowVariable.VOLUM),
+        (
+            constants.AggregationMethod.CUMULATIVE_NEGATIVE,
+            constants.FlowVariable.SURFACE_SOURCE_SINK_DISCHARGE,
+        ),
+        (
+            constants.AggregationMethod.CUMULATIVE_POSITIVE,
+            constants.FlowVariable.SURFACE_SOURCE_SINK_DISCHARGE,
+        ),
     )
 ]
 
 ## 12xx  SIMULATION, timeseries
 CHECKS += [
     TimeseriesRowCheck(col, error_code=1200)
     for col in [
@@ -2596,13 +2699,17 @@
                 )
             ]
 
         self.checks += CHECKS
         if not self.allow_beta_features:
             self.checks += beta_features_check
 
-    def iter_checks(self, level=CheckLevel.ERROR):
+    def iter_checks(self, level=CheckLevel.ERROR, ignore_checks=None):
         """Iterate over checks with at least 'level'"""
         level = CheckLevel.get(level)  # normalize
         for check in self.checks:
             if check.level >= level:
-                yield check
+                if ignore_checks:
+                    if not ignore_checks.match(str(check.error_code).zfill(4)):
+                        yield check
+                else:
+                    yield check
```

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/exporters.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/interfaces/raster_interface.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface_gdal.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/interfaces/raster_interface_gdal.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/interfaces/raster_interface_rasterio.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/interfaces/raster_interface_rasterio.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/model_checks.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/model_checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,34 +42,36 @@
             raise ValueError(f"Unknown context_type '{context_type}'")
 
     @property
     def models(self):
         """Returns a list of declared models"""
         return self.schema.declared_models
 
-    def errors(self, level=CheckLevel.ERROR) -> Iterator[Tuple[BaseCheck, NamedTuple]]:
+    def errors(
+        self, level=CheckLevel.ERROR, ignore_checks=None
+    ) -> Iterator[Tuple[BaseCheck, NamedTuple]]:
         """Iterates and applies checks, returning any failing rows.
 
         By default, checks of WARNING and INFO level are ignored.
 
         :return: Tuple of the applied check and the failing row.
         """
         session = self.db.get_session()
         session.model_checker_context = self.context
-        for check in self.checks(level=level):
+        for check in self.checks(level=level, ignore_checks=ignore_checks):
             model_errors = check.get_invalid(session)
             for error_row in model_errors:
                 yield check, error_row
 
-    def checks(self, level=CheckLevel.ERROR) -> Iterator[BaseCheck]:
+    def checks(self, level=CheckLevel.ERROR, ignore_checks=None) -> Iterator[BaseCheck]:
         """Iterates over all configured checks
 
         :return: implementations of BaseChecks
         """
-        for check in self.config.iter_checks(level=level):
+        for check in self.config.iter_checks(level=level, ignore_checks=ignore_checks):
             yield check
 
     def check_table(self, table):
         pass
 
     def check_column(self, column):
         pass
```

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/scripts.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/scripts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 import click
 from threedi_schema import ThreediDatabase
 from threedi_schema.domain.models import DECLARED_MODELS
 
 from threedi_modelchecker import exporters
 from threedi_modelchecker.checks.base import CheckLevel
 from threedi_modelchecker.config import Config
@@ -31,31 +33,39 @@
 )
 @click.option(
     "--allow-beta",
     is_flag=True,
     default=False,
     help="Don't check whether beta features were used in the database.",
 )
-def check(sqlite, file, level, allow_beta):
+@click.option(
+    "--ignore-checks",
+    type=str,
+    help="Regex pattern; check codes matching this pattern are ignored.",
+    default=None,
+)
+def check(sqlite, file, level, allow_beta, ignore_checks):
     """Checks the threedi-model for errors / warnings / info messages"""
     db = ThreediDatabase(sqlite, echo=False)
     """Checks the threedi model schematisation for errors."""
     level = level.upper()
     if level == "ERROR":
         msg = "errors"
     elif level == "WARNING":
         msg = "errors or warnings"
     else:
         msg = "errors, warnings or info messages"
     click.echo("Parsing schematisation for any %s" % msg)
     if file:
         click.echo("Model errors will be written to %s" % file)
+    if ignore_checks:
+        ignore_checks = re.compile(ignore_checks)
 
     mc = ThreediModelChecker(threedi_db=db, allow_beta_features=allow_beta)
-    model_errors = mc.errors(level=level)
+    model_errors = mc.errors(level=level, ignore_checks=ignore_checks)
 
     if file:
         exporters.export_to_file(model_errors, file)
     else:
         exporters.print_errors(model_errors)
 
     click.echo("Finished processing model")
```

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/conftest.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/factories.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_base.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_cross_section_definitions.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_cross_section_definitions.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     CrossSectionEqualElementsCheck,
     CrossSectionExpectEmptyCheck,
     CrossSectionFirstElementNonZeroCheck,
     CrossSectionFloatCheck,
     CrossSectionFloatListCheck,
     CrossSectionGreaterZeroCheck,
     CrossSectionIncreasingCheck,
+    CrossSectionMinimumDiameterCheck,
     CrossSectionNullCheck,
     CrossSectionYZCoordinateCountCheck,
     CrossSectionYZHeightCheck,
     CrossSectionYZIncreasingWidthIfOpenCheck,
 )
 
 from . import factories
@@ -298,7 +299,162 @@
         width=width,
         height=height,
     )
     factories.CrossSectionLocationFactory(definition=definition)
     check = CrossSectionYZIncreasingWidthIfOpenCheck()
     invalid_rows = check.get_invalid(session)
     assert len(invalid_rows) == 0
+
+
+@pytest.mark.parametrize(
+    "shape,width,height,expected_result",
+    [
+        (0, "0.1", "0.2", 0),  # closed rectangle, sufficient width and height, pass
+        (0, "0.05", "0.2", 1),  # closed rectangle, insufficient width, fail
+        (0, "0.1", "0.03", 1),  # closed rectangle, insufficient height, fail
+        (1, "0.1", None, 0),  # open rectangle, sufficient width, no height, pass
+        (
+            1,
+            "0.1",
+            "0.03",
+            0,
+        ),  # open rectangle, sufficient width, insufficient height should be ignored, pass
+        (1, "0.05", "0.2", 1),  # open rectangle, insufficient width, fail
+        (
+            2,
+            "0.2",
+            "0.05",
+            0,
+        ),  # circle, insufficient height should be overwritten by width, pass
+        (2, "0.05", "0.2", 1),  # circle, insufficient width, fail
+        (
+            3,
+            "0.1",
+            "0.03",
+            0,
+        ),  # egg, insufficient height should be overwritten by 1.5 * width, pass
+        (3, "0.05", "0.2", 1),  # egg, insufficient width, fail
+        (
+            8,
+            "0.1",
+            "0.03",
+            0,
+        ),  # inverted egg, insufficient height should be overwritten by 1.5 * width, pass
+        (8, "0.05", "0.2", 1),  # inverted egg, insufficient width, fail
+        (
+            5,
+            "0.04 0.1",
+            "0.06 0.2",
+            0,
+        ),  # open tabulated rectangle, sufficient width and height, pass
+        (
+            5,
+            "0.04 0.05",
+            "0.06 0.2",
+            1,
+        ),  # open tabulated rectangle, insufficient width, fail
+        (
+            5,
+            "0.04 0.1",
+            "0.06 0.03",
+            0,
+        ),  # open tabulated rectangle, insufficient height, should be ignored, pass
+        (
+            5,
+            "0.04 0.1 0",
+            "0.06 0.2",
+            0,
+        ),  # closed tabulated rectangle, sufficient width and height, pass
+        (
+            5,
+            "0.04 0.05 0",
+            "0.06 0.2",
+            1,
+        ),  # closed tabulated rectangle, insufficient width, fail
+        (
+            5,
+            "0.04 0.1 0",
+            "0.06 0.03",
+            1,
+        ),  # closed tabulated rectangle, insufficient height, fail
+        (
+            6,
+            "0.04 0.1",
+            "0.06 0.2",
+            0,
+        ),  # open tabulated trapezium, sufficient width and height, pass
+        (
+            6,
+            "0.04 0.05",
+            "0.06 0.2",
+            1,
+        ),  # open tabulated trapezium, insufficient width, fail
+        (
+            6,
+            "0.04 0.1",
+            "0.06 0.03",
+            0,
+        ),  # open tabulated trapezium, insufficient height, should be ignored, pass
+        (
+            6,
+            "0.04 0.1 0",
+            "0.06 0.2",
+            0,
+        ),  # closed tabulated trapezium, sufficient width and height, pass
+        (
+            6,
+            "0.04 0.05 0",
+            "0.06 0.2",
+            1,
+        ),  # closed tabulated trapezium, insufficient width, fail
+        (
+            6,
+            "0.04 0.1 0",
+            "0.06 0.03",
+            1,
+        ),  # closed tabulated trapezium, insufficient height, fail
+        (
+            7,
+            "0.01 0.11",
+            "0.11 0.21",
+            0,
+        ),  # open tabulated yz, sufficient width and height, pass
+        (7, "0.01 0.10", "0.11 0.21", 1),  # open tabulated yz, insufficient width, fail
+        (
+            7,
+            "0.01 0.11",
+            "0.11 0.20",
+            0,
+        ),  # open tabulated yz, insufficient height, should be ignored, pass
+        (
+            7,
+            "0.01 0.11 0.01",
+            "0.11 0.21 0.11",
+            0,
+        ),  # closed tabulated yz, sufficient width and height, pass
+        (
+            7,
+            "0.01 0.10 0.01",
+            "0.11 0.21 0.11",
+            1,
+        ),  # closed tabulated yz, insufficient width, fail
+        (
+            7,
+            "0.01 0.11 0.01",
+            "0.11 0.20 0.11",
+            1,
+        ),  # closed tabulated yz, insufficient height, fail
+        (0, "foo", "", 0),  # bad data, pass
+    ],
+)
+def test_check_cross_section_minimum_diameter(
+    session, shape, width, height, expected_result
+):
+    definition = factories.CrossSectionDefinitionFactory(
+        shape=shape,
+        width=width,
+        height=height,
+    )
+    factories.CrossSectionLocationFactory(definition=definition)
+    check = CrossSectionMinimumDiameterCheck()
+    invalid_rows = check.get_invalid(session)
+    assert len(invalid_rows) == expected_result
```

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_factories.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_other.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_other.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,63 @@
 
 from threedi_modelchecker.checks.other import (
     BetaColumnsCheck,
     BetaValuesCheck,
     ChannelManholeLevelCheck,
     ConnectionNodesDistance,
     ConnectionNodesLength,
+    CorrectAggregationSettingsExist,
     CrossSectionLocationCheck,
     CrossSectionSameConfigurationCheck,
     ImperviousNodeInflowAreaCheck,
     LinestringLocationCheck,
+    NodeSurfaceConnectionsCheck,
     OpenChannelsWithNestedNewton,
     PerviousNodeInflowAreaCheck,
     PotentialBreachInterdistanceCheck,
     PotentialBreachStartEndCheck,
     PumpStorageTimestepCheck,
     SpatialIndexCheck,
 )
 from threedi_modelchecker.model_checks import ThreediModelChecker
 
 from . import factories
 
 
+@pytest.mark.parametrize(
+    "aggregation_method,flow_variable,expected_result",
+    [
+        (
+            constants.AggregationMethod.CUMULATIVE,
+            constants.FlowVariable.PUMP_DISCHARGE,
+            0,
+        ),  # entries in aggregation settings, valid
+        (
+            constants.AggregationMethod.CUMULATIVE,
+            constants.FlowVariable.DISCHARGE,
+            1,
+        ),  # entries not in aggregation settings, invalid
+    ],
+)
+def test_aggregation_settings(
+    session, aggregation_method, flow_variable, expected_result
+):
+    factories.GlobalSettingsFactory(id=1)
+    factories.AggregationSettingsFactory(
+        global_settings_id=1,
+        aggregation_method=constants.AggregationMethod.CUMULATIVE,
+        flow_variable=constants.FlowVariable.PUMP_DISCHARGE,
+    )
+    check = CorrectAggregationSettingsExist(
+        aggregation_method=aggregation_method, flow_variable=flow_variable
+    )
+    invalid = check.get_invalid(session)
+    assert len(invalid) == expected_result
+
+
 def test_connection_nodes_length(session):
     factories.GlobalSettingsFactory(epsg_code=28992)
     factories.WeirFactory(
         connection_node_start=factories.ConnectionNodeFactory(
             the_geom="SRID=4326;POINT(-0.38222995634060702 -0.13872239147499893)"
         ),
         connection_node_end=factories.ConnectionNodeFactory(
@@ -527,14 +560,42 @@
     factories.SurfaceMapFactory(surface_id=2, connection_node_id=1)
     check = PerviousNodeInflowAreaCheck()
     invalid = check.get_invalid(session)
     assert len(invalid) == expected_result
 
 
 @pytest.mark.parametrize(
+    "surface_type",
+    [("impervious"), ("pervious")],
+)
+@pytest.mark.parametrize(
+    "connected_surfaces_count,expected_result",
+    [
+        (50, 0),
+        (51, 1),
+    ],
+)
+def test_connection_node_mapped_surfaces(
+    session, surface_type, connected_surfaces_count, expected_result
+):
+    factories.ConnectionNodeFactory(id=1)
+    if surface_type == "pervious":
+        for i in range(connected_surfaces_count):
+            factories.SurfaceMapFactory(connection_node_id=1, surface_id=i + 1)
+    elif surface_type == "impervious":
+        for i in range(connected_surfaces_count):
+            factories.ImperviousSurfaceMapFactory(
+                connection_node_id=1, impervious_surface_id=i + 1
+            )
+    check = NodeSurfaceConnectionsCheck(check_type=surface_type)
+    invalid = check.get_invalid(session)
+    assert len(invalid) == expected_result
+
+
+@pytest.mark.parametrize(
     "value,expected_result",
     [
         (None, 0),  # column not set, valid result
         (5, 1),  # column set, invalid result
     ],
 )
 def test_beta_columns(session, value, expected_result):
```

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_raster.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_raster.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_checks_timeseries.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_checks_timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_exporters.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker/tests/test_model_checks.py` & `threedi-modelchecker-2.2.0/threedi_modelchecker/tests/test_model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/PKG-INFO` & `threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.1.1
+Version: 2.2.0
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.1.1/threedi_modelchecker.egg-info/SOURCES.txt` & `threedi-modelchecker-2.2.0/threedi_modelchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

