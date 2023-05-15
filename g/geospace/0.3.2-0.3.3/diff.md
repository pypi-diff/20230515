# Comparing `tmp/geospace-0.3.2.tar.gz` & `tmp/geospace-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geospace-0.3.2.tar", last modified: Sun Apr  9 15:26:58 2023, max compression
+gzip compressed data, was "geospace-0.3.3.tar", last modified: Mon May 15 19:15:24 2023, max compression
```

## Comparing `geospace-0.3.2.tar` & `geospace-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 15:26:58.667079 geospace-0.3.2/
--rw-rw-rw-   0        0        0     1055 2021-03-21 14:06:09.000000 geospace-0.3.2/LICENSE
--rw-rw-rw-   0        0        0       25 2021-03-20 14:22:17.000000 geospace-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1294 2023-04-09 15:26:58.667079 geospace-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      582 2021-03-20 14:45:55.000000 geospace-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 15:26:58.662079 geospace-0.3.2/geospace/
--rw-rw-rw-   0        0        0      449 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/__init__.py
--rw-rw-rw-   0        0        0     1028 2023-03-21 08:26:55.000000 geospace-0.3.2/geospace/_const.py
--rw-rw-rw-   0        0        0     4333 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/boundary.py
--rw-rw-rw-   0        0        0     8356 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/gee_export.py
--rw-rw-rw-   0        0        0     4248 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/map_calc.py
--rw-rw-rw-   0        0        0     1557 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/projection.py
--rw-rw-rw-   0        0        0     1240 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/ras_to_shp.py
--rw-rw-rw-   0        0        0     5931 2023-04-09 15:26:08.000000 geospace-0.3.2/geospace/raster.py
--rw-rw-rw-   0        0        0     5489 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/shape.py
--rw-rw-rw-   0        0        0     6206 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/shp_to_ras.py
--rw-rw-rw-   0        0        0     6363 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/spatial_calc.py
--rw-rw-rw-   0        0        0     6405 2023-04-09 15:26:01.000000 geospace-0.3.2/geospace/utils.py
--rw-rw-rw-   0        0        0     8848 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/zonal_stats.py
-drwxrwxrwx   0        0        0        0 2023-04-09 15:26:58.666080 geospace-0.3.2/geospace.egg-info/
--rw-rw-rw-   0        0        0     1294 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 15:26:58.667079 geospace-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     3987 2023-04-09 15:26:40.000000 geospace-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:15:24.197647 geospace-0.3.3/
+-rw-rw-rw-   0        0        0     1055 2021-03-21 14:06:09.000000 geospace-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0       25 2021-03-20 14:22:17.000000 geospace-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1294 2023-05-15 19:15:24.196647 geospace-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2021-03-20 14:45:55.000000 geospace-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 19:15:24.177893 geospace-0.3.3/geospace/
+-rw-rw-rw-   0        0        0      519 2023-05-09 09:52:33.000000 geospace-0.3.3/geospace/__init__.py
+-rw-rw-rw-   0        0        0     1028 2023-03-21 08:26:55.000000 geospace-0.3.3/geospace/_const.py
+-rw-rw-rw-   0        0        0     4333 2023-03-20 09:13:43.000000 geospace-0.3.3/geospace/boundary.py
+-rw-rw-rw-   0        0        0     8864 2023-05-15 19:13:59.000000 geospace-0.3.3/geospace/gee_export.py
+-rw-rw-rw-   0        0        0     4248 2023-03-20 09:13:43.000000 geospace-0.3.3/geospace/map_calc.py
+-rw-rw-rw-   0        0        0     2498 2023-05-09 09:51:44.000000 geospace-0.3.3/geospace/mask.py
+-rw-rw-rw-   0        0        0     1557 2023-03-20 09:13:43.000000 geospace-0.3.3/geospace/projection.py
+-rw-rw-rw-   0        0        0     1240 2023-03-20 09:13:43.000000 geospace-0.3.3/geospace/ras_to_shp.py
+-rw-rw-rw-   0        0        0     5931 2023-04-09 15:26:08.000000 geospace-0.3.3/geospace/raster.py
+-rw-rw-rw-   0        0        0     5489 2023-03-20 09:13:43.000000 geospace-0.3.3/geospace/shape.py
+-rw-rw-rw-   0        0        0     6206 2023-03-20 09:13:43.000000 geospace-0.3.3/geospace/shp_to_ras.py
+-rw-rw-rw-   0        0        0     6363 2023-03-20 09:13:43.000000 geospace-0.3.3/geospace/spatial_calc.py
+-rw-rw-rw-   0        0        0     6405 2023-04-09 15:26:01.000000 geospace-0.3.3/geospace/utils.py
+-rw-rw-rw-   0        0        0     8848 2023-03-20 09:13:43.000000 geospace-0.3.3/geospace/zonal_stats.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:15:24.194649 geospace-0.3.3/geospace.egg-info/
+-rw-rw-rw-   0        0        0     1294 2023-05-15 19:15:23.000000 geospace-0.3.3/geospace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-05-15 19:15:24.000000 geospace-0.3.3/geospace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 19:15:23.000000 geospace-0.3.3/geospace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-15 19:15:23.000000 geospace-0.3.3/geospace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 19:15:23.000000 geospace-0.3.3/geospace.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 19:15:24.197647 geospace-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     3987 2023-05-15 19:14:38.000000 geospace-0.3.3/setup.py
```

### Comparing `geospace-0.3.2/LICENSE` & `geospace-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/PKG-INFO` & `geospace-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospace
-Version: 0.3.2
+Version: 0.3.3
 Summary: Geospatial processing library based on GDAL and Google Earth Engine
 Home-page: https://github.com/xiejx5/geospace
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `geospace-0.3.2/README.md` & `geospace-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/_const.py` & `geospace-0.3.3/geospace/_const.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/boundary.py` & `geospace-0.3.3/geospace/boundary.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/gee_export.py` & `geospace-0.3.3/geospace/gee_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,29 +126,33 @@
         details are in Export.image.toDrive()
     """
     params['image'] = image
     params['description'] = params.pop('description', image.bandNames().get(0).getInfo())
     params['crs'] = params.pop('crs', 'EPSG:4326')
     params['maxPixels'] = params.pop('maxPixels', 1e13)
 
-    if params.get('dimensions') == 'default':
-        params['dimensions'] = '360x180'
-
     if params.get('crsTransform') == 'ERA5_LAND':
         params['crsTransform'] = [0.1, 0, -180.05, 0, -0.1, 90.05]
 
     if params.get('region') == 'global':
         params['region'] = ee.Geometry.Rectangle([-180, -90, 180, 90],
                                                  geodesic=False, proj="EPSG:4326")
+        if params.get('dimensions') == 'default':
+            params['dimensions'] = '360x180'
+    elif params.get('region') == 'nonATA':
+        params['region'] = ee.Geometry.Rectangle([-180, -60, 180, 89],
+                                                 geodesic=False, proj="EPSG:4326")
+        if params.get('dimensions') == 'default':
+            params['dimensions'] = '360x149'
 
     ee.batch.Export.image.toDrive(**params).start()
 
 
 def gee_export_csv(fc, image, fields=['ORDER', '.*mean'],
-                   return_url=False, **kwargs):
+                   return_url=False, to_drive=None, **kwargs):
     """export a csv containing the basin average value
 
     Args:
         fc (ee.FeatureCollection): e.g. basins
         image (ee.Image): e.g. DEM
 
     Returns:
@@ -159,19 +163,23 @@
     scale = kwargs.pop('scale', image.projection().nominalScale())
 
     if image.projection().crs().getInfo() != 'EPSG:4326':
         image = image.reproject('EPSG:4326', None, scale)
 
     means = image.reduceRegions(fc, reducer=reducer, scale=scale, **kwargs)
 
-    url = means.select(fields, retainGeometry=False).getDownloadURL(filetype='csv')
-    if return_url:
-        return url
+    if to_drive is None:
+        url = means.select(fields, retainGeometry=False).getDownloadURL(filetype='csv')
+        if return_url:
+            return url
+        else:
+            return pd.read_csv(url)
     else:
-        return pd.read_csv(url)
+        ee.batch.Export.table.toDrive(means, description=to_drive,
+                                      selectors=fields).start()
 
 
 def gee_soilgrids(band):
     """download and preprocess soilgrids from google earth engine
 
     https://git.wur.nl/isric/soilgrids/soilgrids.notebooks/-/blob/master/markdown/access_on_gee.md
```

### Comparing `geospace-0.3.2/geospace/map_calc.py` & `geospace-0.3.3/geospace/map_calc.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/projection.py` & `geospace-0.3.3/geospace/projection.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/ras_to_shp.py` & `geospace-0.3.3/geospace/ras_to_shp.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/raster.py` & `geospace-0.3.3/geospace/raster.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/shape.py` & `geospace-0.3.3/geospace/shape.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/shp_to_ras.py` & `geospace-0.3.3/geospace/shp_to_ras.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/spatial_calc.py` & `geospace-0.3.3/geospace/spatial_calc.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/utils.py` & `geospace-0.3.3/geospace/utils.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace/zonal_stats.py` & `geospace-0.3.3/geospace/zonal_stats.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.2/geospace.egg-info/PKG-INFO` & `geospace-0.3.3/geospace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospace
-Version: 0.3.2
+Version: 0.3.3
 Summary: Geospatial processing library based on GDAL and Google Earth Engine
 Home-page: https://github.com/xiejx5/geospace
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `geospace-0.3.2/setup.py` & `geospace-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'geospace'
 DESCRIPTION = 'Geospatial processing library based on GDAL and Google Earth Engine'
 URL = 'https://github.com/xiejx5/geospace'
 EMAIL = 'xiejx5@gmail.com'
 AUTHOR = 'Cody James'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.2'
+VERSION = '0.3.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy', 'gdal', 'tqdm'
 ]
 
 # What packages are optional?
```

