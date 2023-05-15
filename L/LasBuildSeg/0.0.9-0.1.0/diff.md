# Comparing `tmp/LasBuildSeg-0.0.9.tar.gz` & `tmp/LasBuildSeg-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.0.9.tar", last modified: Wed May 10 09:50:16 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.0.tar", last modified: Sun May 14 18:43:43 2023, max compression
```

## Comparing `LasBuildSeg-0.0.9.tar` & `LasBuildSeg-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 09:50:16.559576 LasBuildSeg-0.0.9/
--rw-rw-rw-   0        0        0      107 2023-05-10 09:49:42.000000 LasBuildSeg-0.0.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.9/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 09:50:16.495789 LasBuildSeg-0.0.9/LasBuildSeg/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.0.9/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      375 2023-05-10 08:51:25.000000 LasBuildSeg-0.0.9/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 09:50:16.552600 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     2057 2023-05-10 09:50:14.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-10 09:50:15.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 09:50:14.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-05-10 09:50:14.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 09:50:14.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2057 2023-05-10 09:50:16.556602 LasBuildSeg-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1126 2023-05-10 09:49:28.000000 LasBuildSeg-0.0.9/README.md
--rw-rw-rw-   0        0        0     1495 2023-05-10 09:49:45.000000 LasBuildSeg-0.0.9/Setup.py
--rw-rw-rw-   0        0        0      106 2023-05-10 07:11:46.000000 LasBuildSeg-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 09:50:16.560580 LasBuildSeg-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 18:43:43.039480 LasBuildSeg-0.1.0/
+-rw-rw-rw-   0        0        0      107 2023-05-14 18:43:04.000000 LasBuildSeg-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.0/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 18:43:43.019157 LasBuildSeg-0.1.0/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-14 18:43:43.036473 LasBuildSeg-0.1.0/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.0/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    14494 2023-05-14 18:22:59.000000 LasBuildSeg-0.1.0/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      472 2023-05-14 18:36:38.000000 LasBuildSeg-0.1.0/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 18:43:43.035478 LasBuildSeg-0.1.0/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     2133 2023-05-14 18:43:42.000000 LasBuildSeg-0.1.0/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-14 18:43:42.000000 LasBuildSeg-0.1.0/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 18:43:42.000000 LasBuildSeg-0.1.0/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-14 18:43:42.000000 LasBuildSeg-0.1.0/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-14 18:43:42.000000 LasBuildSeg-0.1.0/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2133 2023-05-14 18:43:43.038478 LasBuildSeg-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1202 2023-05-14 18:43:07.000000 LasBuildSeg-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1495 2023-05-14 18:43:15.000000 LasBuildSeg-0.1.0/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-14 18:30:49.000000 LasBuildSeg-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 18:43:43.039480 LasBuildSeg-0.1.0/setup.cfg
```

### Comparing `LasBuildSeg-0.0.9/LICENSE.txt` & `LasBuildSeg-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.9/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.0/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.9/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.0/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.9
+Version: 0.1.0
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,28 +23,32 @@
 This Python package is BUilding Footprint Extractor Test
 
 This of example of an how you can run your code
 
 ```python
 import LasBuildSeg as Lasb
 import numpy as np
- 
-Lasb.generate_dsm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
-Lasb.generate_dtm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
+
+Lasb.generate_dsm('YourLazfile', EPSG CODE, 1)
+Lasb.generate_dtm('YourLazfile', EPSG CODE, 1)
 Lasb.generate_ndhm('dtm.tif', 'dsm.tif')
+
 img, profile = Lasb.read_geotiff('ndhm.tif')
+dem, _ = Lasb.read_geotiff('dsm3857.tif')
 img_8bit = Lasb.to_8bit(img)
-constant = 4.6
+constant = 3.6
 block_size = 51
 img_thresh = Lasb.threshold(img_8bit, block_size, constant)
 kernel_size = 3
 img_open = Lasb.morphopen(img_thresh, kernel_size)
 min_size=35
 max_size=5000
-building_mask = Lasb.filter_contours(img_open, profile, min_size, max_size)
+tri_threshold=3
+building_mask = Lasb.filter_contours(img_open, dem, profile, min_size, max_size, tri_threshold=tri_threshold)
 kernel_size = 3
 CloseKernel_size=15
 building_mask_closed = Lasb.close(building_mask, CloseKernel_size)
 # Invert the building mask to make buildings appear as white ground pixels
 inverted_building_mask = np.ones_like(building_mask, dtype=np.uint8) - building_mask_closed
-Las.write_geotiff('buildings.tif', inverted_building_mask, profile)
+Lasb.write_geotiff('buildings.tif', building_mask_closed, profile)
+Lasb.building_footprints_to_geojson('buildings.tif', 'building.geojson')
 print('All of our steps are done.')
```

### Comparing `LasBuildSeg-0.0.9/PKG-INFO` & `LasBuildSeg-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.9
+Version: 0.1.0
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,28 +23,32 @@
 This Python package is BUilding Footprint Extractor Test
 
 This of example of an how you can run your code
 
 ```python
 import LasBuildSeg as Lasb
 import numpy as np
- 
-Lasb.generate_dsm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
-Lasb.generate_dtm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
+
+Lasb.generate_dsm('YourLazfile', EPSG CODE, 1)
+Lasb.generate_dtm('YourLazfile', EPSG CODE, 1)
 Lasb.generate_ndhm('dtm.tif', 'dsm.tif')
+
 img, profile = Lasb.read_geotiff('ndhm.tif')
+dem, _ = Lasb.read_geotiff('dsm3857.tif')
 img_8bit = Lasb.to_8bit(img)
-constant = 4.6
+constant = 3.6
 block_size = 51
 img_thresh = Lasb.threshold(img_8bit, block_size, constant)
 kernel_size = 3
 img_open = Lasb.morphopen(img_thresh, kernel_size)
 min_size=35
 max_size=5000
-building_mask = Lasb.filter_contours(img_open, profile, min_size, max_size)
+tri_threshold=3
+building_mask = Lasb.filter_contours(img_open, dem, profile, min_size, max_size, tri_threshold=tri_threshold)
 kernel_size = 3
 CloseKernel_size=15
 building_mask_closed = Lasb.close(building_mask, CloseKernel_size)
 # Invert the building mask to make buildings appear as white ground pixels
 inverted_building_mask = np.ones_like(building_mask, dtype=np.uint8) - building_mask_closed
-Las.write_geotiff('buildings.tif', inverted_building_mask, profile)
+Lasb.write_geotiff('buildings.tif', building_mask_closed, profile)
+Lasb.building_footprints_to_geojson('buildings.tif', 'building.geojson')
 print('All of our steps are done.')
```

### Comparing `LasBuildSeg-0.0.9/Setup.py` & `LasBuildSeg-0.1.0/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.0.9',
+  version='0.1.0',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

