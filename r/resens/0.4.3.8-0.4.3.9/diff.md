# Comparing `tmp/resens-0.4.3.8.tar.gz` & `tmp/resens-0.4.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resens-0.4.3.8.tar", last modified: Fri Oct 21 13:14:56 2022, max compression
+gzip compressed data, was "resens-0.4.3.9.tar", last modified: Tue Oct 25 13:10:44 2022, max compression
```

## Comparing `resens-0.4.3.8.tar` & `resens-0.4.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nikos     (1000) nikos     (1000)        0 2022-10-21 13:14:56.537347 resens-0.4.3.8/
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)     1085 2022-08-08 20:33:21.000000 resens-0.4.3.8/LICENSE.rst
--rw-r--r--   0 nikos     (1000) nikos     (1000)      466 2022-10-21 13:14:56.537347 resens-0.4.3.8/PKG-INFO
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)      119 2022-02-26 13:45:49.000000 resens-0.4.3.8/README.md
-drwxr-xr-x   0 nikos     (1000) nikos     (1000)        0 2022-10-21 13:14:56.536347 resens-0.4.3.8/resens/
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)      121 2022-10-21 13:13:22.000000 resens-0.4.3.8/resens/__init__.py
--rw-r--r--   0 nikos     (1000) nikos     (1000)       24 2022-10-21 13:11:12.000000 resens-0.4.3.8/resens/__version__.py
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)     8752 2022-09-09 10:12:40.000000 resens-0.4.3.8/resens/analysis.py
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)     7160 2022-09-12 09:21:21.000000 resens-0.4.3.8/resens/io.py
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)     9038 2022-09-14 13:51:31.000000 resens-0.4.3.8/resens/processing.py
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)      430 2022-09-08 14:19:22.000000 resens-0.4.3.8/resens/rasteroptions.py
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)     5401 2022-10-21 13:09:31.000000 resens-0.4.3.8/resens/utils.py
-drwxr-xr-x   0 nikos     (1000) nikos     (1000)        0 2022-10-21 13:14:56.537347 resens-0.4.3.8/resens.egg-info/
--rw-r--r--   0 nikos     (1000) nikos     (1000)      466 2022-10-21 13:14:56.000000 resens-0.4.3.8/resens.egg-info/PKG-INFO
--rw-r--r--   0 nikos     (1000) nikos     (1000)      352 2022-10-21 13:14:56.000000 resens-0.4.3.8/resens.egg-info/SOURCES.txt
--rw-r--r--   0 nikos     (1000) nikos     (1000)        1 2022-10-21 13:14:56.000000 resens-0.4.3.8/resens.egg-info/dependency_links.txt
--rw-r--r--   0 nikos     (1000) nikos     (1000)        1 2022-10-21 13:12:01.000000 resens-0.4.3.8/resens.egg-info/not-zip-safe
--rw-r--r--   0 nikos     (1000) nikos     (1000)       30 2022-10-21 13:14:56.000000 resens-0.4.3.8/resens.egg-info/requires.txt
--rw-r--r--   0 nikos     (1000) nikos     (1000)        7 2022-10-21 13:14:56.000000 resens-0.4.3.8/resens.egg-info/top_level.txt
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)      107 2022-10-21 13:14:56.537347 resens-0.4.3.8/setup.cfg
--rwxrwxrwx   0 nikos     (1000) nikos     (1000)      719 2022-10-21 13:11:11.000000 resens-0.4.3.8/setup.py
+drwxr-xr-x   0 nikos     (1000) nikos     (1000)        0 2022-10-25 13:10:44.012177 resens-0.4.3.9/
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)     1085 2022-08-08 20:33:21.000000 resens-0.4.3.9/LICENSE.rst
+-rw-r--r--   0 nikos     (1000) nikos     (1000)      466 2022-10-25 13:10:44.012177 resens-0.4.3.9/PKG-INFO
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)      119 2022-02-26 13:45:49.000000 resens-0.4.3.9/README.md
+drwxr-xr-x   0 nikos     (1000) nikos     (1000)        0 2022-10-25 13:10:44.011177 resens-0.4.3.9/resens/
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)      121 2022-10-21 13:13:22.000000 resens-0.4.3.9/resens/__init__.py
+-rw-r--r--   0 nikos     (1000) nikos     (1000)       24 2022-10-25 13:10:04.000000 resens-0.4.3.9/resens/__version__.py
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)     8752 2022-09-09 10:12:40.000000 resens-0.4.3.9/resens/analysis.py
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)     7160 2022-09-12 09:21:21.000000 resens-0.4.3.9/resens/io.py
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)     9038 2022-09-14 13:51:31.000000 resens-0.4.3.9/resens/processing.py
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)      430 2022-09-08 14:19:22.000000 resens-0.4.3.9/resens/rasteroptions.py
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)     5428 2022-10-25 13:09:15.000000 resens-0.4.3.9/resens/utils.py
+drwxr-xr-x   0 nikos     (1000) nikos     (1000)        0 2022-10-25 13:10:44.012177 resens-0.4.3.9/resens.egg-info/
+-rw-r--r--   0 nikos     (1000) nikos     (1000)      466 2022-10-25 13:10:43.000000 resens-0.4.3.9/resens.egg-info/PKG-INFO
+-rw-r--r--   0 nikos     (1000) nikos     (1000)      352 2022-10-25 13:10:43.000000 resens-0.4.3.9/resens.egg-info/SOURCES.txt
+-rw-r--r--   0 nikos     (1000) nikos     (1000)        1 2022-10-25 13:10:43.000000 resens-0.4.3.9/resens.egg-info/dependency_links.txt
+-rw-r--r--   0 nikos     (1000) nikos     (1000)        1 2022-10-21 13:12:01.000000 resens-0.4.3.9/resens.egg-info/not-zip-safe
+-rw-r--r--   0 nikos     (1000) nikos     (1000)       30 2022-10-25 13:10:43.000000 resens-0.4.3.9/resens.egg-info/requires.txt
+-rw-r--r--   0 nikos     (1000) nikos     (1000)        7 2022-10-25 13:10:43.000000 resens-0.4.3.9/resens.egg-info/top_level.txt
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)      107 2022-10-25 13:10:44.012177 resens-0.4.3.9/setup.cfg
+-rwxrwxrwx   0 nikos     (1000) nikos     (1000)      719 2022-10-25 13:10:12.000000 resens-0.4.3.9/setup.py
```

### Comparing `resens-0.4.3.8/LICENSE.rst` & `resens-0.4.3.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `resens-0.4.3.8/resens/analysis.py` & `resens-0.4.3.9/resens/analysis.py`

 * *Files identical despite different names*

### Comparing `resens-0.4.3.8/resens/io.py` & `resens-0.4.3.9/resens/io.py`

 * *Files identical despite different names*

### Comparing `resens-0.4.3.8/resens/processing.py` & `resens-0.4.3.9/resens/processing.py`

 * *Files identical despite different names*

### Comparing `resens-0.4.3.8/resens/utils.py` & `resens-0.4.3.9/resens/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     if "s3" in polygon_shp:
         gdf = gpd.read_file(polygon_shp)
 
         # Write temporary file
         polygon_shp = tempfile.NamedTemporaryFile().name
         gdf.to_file(polygon_shp)
         remove_files.append(polygon_shp)
-    elif not polygon_shp.exists():
+    elif not Path(polygon_shp).exists():
         raise FileNotFoundError(f"Polygon shapefile does not exist at {polygon_shp.as_posix()}.")
     
     polygon_shp = Path(polygon_shp)
 
     # Make sure the shapefile and image are using the same CRS
     gdf = gpd.read_file(polygon_shp)
     out_epsg = gdf.crs.from_wkt(projection).to_epsg()
@@ -132,14 +132,15 @@
 
     # Load shapefile layers
     shp_ds = ogr.Open(polygon_shp.as_posix())
     shp_lyr = shp_ds.GetLayer()
 
     # Rasterization
     gdal.RasterizeLayer(target_ds, [1], shp_lyr, burn_values=[burn_value])
+    target_ds = None
 
     # Load the mask array
     mask_arr, transf, proj, _ = io.load_image(mask_outpath.as_posix())
 
     # Dilate the mask
     if dilation:
         if dilation_iters:
```

### Comparing `resens-0.4.3.8/setup.py` & `resens-0.4.3.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="resens",
-    version="0.4.3.8",
+    version="0.4.3.9",
     description="Raster Processing package for Remote Sensing and Earth Observation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.nargyrop.com",
     author="Nikos Argyropoulos",
     author_email="n.argiropgeo@gmail.com",
     license="MIT",
```

