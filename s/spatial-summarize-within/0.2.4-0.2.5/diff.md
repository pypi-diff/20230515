# Comparing `tmp/spatial_summarize_within-0.2.4.tar.gz` & `tmp/spatial_summarize_within-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-0.2.4.tar", last modified: Fri May 12 18:09:51 2023, max compression
+gzip compressed data, was "spatial_summarize_within-0.2.5.tar", last modified: Mon May 15 04:12:15 2023, max compression
```

## Comparing `spatial_summarize_within-0.2.4.tar` & `spatial_summarize_within-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 18:09:51.457204 spatial_summarize_within-0.2.4/
--rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.2.4/LICENSE
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-12 18:09:51.457085 spatial_summarize_within-0.2.4/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)     2170 2023-05-08 23:11:41.000000 spatial_summarize_within-0.2.4/README.md
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-12 18:09:51.457240 spatial_summarize_within-0.2.4/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-05-12 18:09:42.000000 spatial_summarize_within-0.2.4/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 18:09:51.456228 spatial_summarize_within-0.2.4/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2447 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/max_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2455 2023-05-12 06:16:37.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/mean_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2448 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/min_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2429 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/sum_within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 18:09:51.456930 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-15 04:12:15.191775 spatial_summarize_within-0.2.5/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.2.5/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-15 04:12:15.191663 spatial_summarize_within-0.2.5/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     2170 2023-05-08 23:11:41.000000 spatial_summarize_within-0.2.5/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-15 04:12:15.191808 spatial_summarize_within-0.2.5/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-05-15 04:12:06.000000 spatial_summarize_within-0.2.5/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-15 04:12:15.190878 spatial_summarize_within-0.2.5/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2447 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/max_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2645 2023-05-15 03:55:52.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/mean_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2448 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/min_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2429 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.5/spatial_summarize_within/sum_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-15 04:12:15.191515 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-15 04:12:15.000000 spatial_summarize_within-0.2.5/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-0.2.4/LICENSE` & `spatial_summarize_within-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.4/README.md` & `spatial_summarize_within-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.4/spatial_summarize_within/max_within.py` & `spatial_summarize_within-0.2.5/spatial_summarize_within/max_within.py`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.4/spatial_summarize_within/mean_within.py` & `spatial_summarize_within-0.2.5/spatial_summarize_within/sum_within.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
 # Function
-def mean_within(input_shapefile, input_summary_features, columns, key):
+def sum_within(input_shapefile, input_summary_features, columns, key):
     # Read input and overlay shapefiles
     input_shapefile = input_shapefile
     input_summary_features = input_summary_features
 
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
     # Create an empty geodataframe to store the results
@@ -26,22 +26,22 @@
         temp_overlay.set_crs(input_summary_features.crs, inplace=True)
         # Intersect the input geodataframe with the current overlay polygon
         temp_intersect = gpd.overlay(input_summary_features, temp_overlay, how='intersection')
         # Calculate the area of each polygon in intersect dataframe
         temp_intersect["intersect_area"] = temp_intersect.area
         # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
         temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
-        # Calculate the weighted mean
+        # Calculate the weighted sum
         columns = columns
         for column in columns:
             temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
-        # Group the results and calculate the mean
-        temp_result = temp_intersect.groupby(key).mean(numeric_only=True).reset_index()
+        # Group the results
+        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = input_shapefile.merge(result_gdf, on=key)
 
     # Remove the added area column from input geodataframe
```

### Comparing `spatial_summarize_within-0.2.4/spatial_summarize_within/min_within.py` & `spatial_summarize_within-0.2.5/spatial_summarize_within/min_within.py`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.4/spatial_summarize_within/sum_within.py` & `spatial_summarize_within-0.2.5/spatial_summarize_within/mean_within.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
 # Function
-def sum_within(input_shapefile, input_summary_features, columns, key):
+def mean_within(input_shapefile, input_summary_features, columns, key):
     # Read input and overlay shapefiles
     input_shapefile = input_shapefile
     input_summary_features = input_summary_features
 
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
     # Create an empty geodataframe to store the results
@@ -26,24 +26,27 @@
         temp_overlay.set_crs(input_summary_features.crs, inplace=True)
         # Intersect the input geodataframe with the current overlay polygon
         temp_intersect = gpd.overlay(input_summary_features, temp_overlay, how='intersection')
         # Calculate the area of each polygon in intersect dataframe
         temp_intersect["intersect_area"] = temp_intersect.area
         # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
         temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
-        # Calculate the weighted sum
+        # Calculate the weighted mean
         columns = columns
         for column in columns:
-            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
+            temp_intersect[column] = temp_intersect[column] * temp_intersect["intersect_area"]
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
-        # Group the results
-        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
+        # Group the results by key and calculate the sum of each group
+        temp_sum = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
+        # Calculate the mean by dividing the sum by the total intersect area
+        for column in columns:
+            temp_sum[column] = temp_sum[column] / temp_sum['intersect_area']
         # Append the results to the result gdf
-        result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
+        result_gdf = pd.concat([result_gdf, temp_sum], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = input_shapefile.merge(result_gdf, on=key)
 
     # Remove the added area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
```

