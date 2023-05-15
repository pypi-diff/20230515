# Comparing `tmp/cartagen4py-0.1.4.tar.gz` & `tmp/cartagen4py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartagen4py-0.1.4.tar", last modified: Fri May 12 08:51:36 2023, max compression
+gzip compressed data, was "cartagen4py-0.1.5.tar", last modified: Mon May 15 08:52:54 2023, max compression
```

## Comparing `cartagen4py-0.1.4.tar` & `cartagen4py-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,61 @@
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:51:36.133912 cartagen4py-0.1.4/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-12 08:51:36.129912 cartagen4py-0.1.4/PKG-INFO
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      229 2023-03-01 13:47:49.000000 cartagen4py-0.1.4/README.md
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:51:36.129912 cartagen4py-0.1.4/cartagen4py/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-04-21 09:00:14.000000 cartagen4py-0.1.4/cartagen4py/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:51:36.129912 cartagen4py-0.1.4/cartagen4py/algorithms/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       68 2023-04-21 08:51:33.000000 cartagen4py-0.1.4/cartagen4py/algorithms/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:51:36.129912 cartagen4py-0.1.4/cartagen4py/algorithms/buildings/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      147 2023-05-12 08:35:36.000000 cartagen4py-0.1.4/cartagen4py/algorithms/buildings/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4454 2023-03-30 13:45:12.000000 cartagen4py-0.1.4/cartagen4py/algorithms/buildings/amalgamation.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7432 2023-03-30 13:44:15.000000 cartagen4py-0.1.4/cartagen4py/algorithms/buildings/random_displacement.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7988 2023-04-21 08:51:00.000000 cartagen4py-0.1.4/cartagen4py/algorithms/buildings/simplification.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14749 2023-05-10 10:01:58.000000 cartagen4py-0.1.4/cartagen4py/algorithms/buildings/squaring.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:51:36.129912 cartagen4py-0.1.4/cartagen4py.egg-info/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-12 08:51:36.000000 cartagen4py-0.1.4/cartagen4py.egg-info/PKG-INFO
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      497 2023-05-12 08:51:36.000000 cartagen4py-0.1.4/cartagen4py.egg-info/SOURCES.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-12 08:51:36.000000 cartagen4py-0.1.4/cartagen4py.egg-info/dependency_links.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-12 08:51:36.000000 cartagen4py-0.1.4/cartagen4py.egg-info/requires.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-12 08:51:36.000000 cartagen4py-0.1.4/cartagen4py.egg-info/top_level.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-12 08:51:36.133912 cartagen4py-0.1.4/setup.cfg
--rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     1683 2023-05-12 08:51:29.000000 cartagen4py-0.1.4/setup.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      229 2023-03-01 13:47:49.000000 cartagen4py-0.1.5/README.md
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.513099 cartagen4py-0.1.5/cartagen4py/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      179 2023-05-15 08:33:30.000000 cartagen4py-0.1.5/cartagen4py/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.513099 cartagen4py-0.1.5/cartagen4py/algorithms/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      134 2023-05-15 08:34:07.000000 cartagen4py-0.1.5/cartagen4py/algorithms/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-05-15 08:34:43.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4482 2023-05-15 08:35:40.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/amalgamation.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7441 2023-05-15 08:35:18.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/random_displacement.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     8000 2023-05-15 08:35:47.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14748 2023-05-15 08:35:50.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/squaring.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/algorithms/general/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       55 2023-05-12 12:21:40.000000 cartagen4py-0.1.5/cartagen4py/algorithms/general/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    27075 2023-05-12 11:58:26.000000 cartagen4py-0.1.5/cartagen4py/algorithms/general/constraint.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/algorithms/lines/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      120 2023-05-12 12:23:23.000000 cartagen4py-0.1.5/cartagen4py/algorithms/lines/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     5310 2023-05-12 11:58:09.000000 cartagen4py-0.1.5/cartagen4py/algorithms/lines/line_simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      394 2023-03-15 09:37:20.000000 cartagen4py-0.1.5/cartagen4py/algorithms/lines/line_smoothing.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/data_enrichment/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      113 2023-05-12 12:24:09.000000 cartagen4py-0.1.5/cartagen4py/data_enrichment/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1570 2023-05-12 12:24:49.000000 cartagen4py-0.1.5/cartagen4py/data_enrichment/building_measures.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1018 2023-05-12 11:58:54.000000 cartagen4py-0.1.5/cartagen4py/data_enrichment/urban_areas.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/evaluation/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.5/cartagen4py/evaluation/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      238 2023-03-01 13:47:49.000000 cartagen4py-0.1.5/cartagen4py/evaluation/constraint_satisfaction.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/processes/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.5/cartagen4py/processes/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/utils/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      210 2023-05-15 08:50:08.000000 cartagen4py-0.1.5/cartagen4py/utils/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/utils/clustering/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       49 2023-05-15 08:52:08.000000 cartagen4py-0.1.5/cartagen4py/utils/clustering/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-30 13:41:05.000000 cartagen4py-0.1.5/cartagen4py/utils/clustering/dbscan.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/utils/geometry/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      189 2023-05-15 08:51:46.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      386 2023-03-15 09:37:20.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/angle.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1327 2023-03-21 13:10:50.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/extent.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1195 2023-03-30 13:41:05.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/line.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3167 2023-05-12 11:54:30.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/segment.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/cartagen4py/utils/math/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       91 2023-05-15 08:51:15.000000 cartagen4py-0.1.5/cartagen4py/utils/math/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4304 2023-04-21 08:51:00.000000 cartagen4py-0.1.5/cartagen4py/utils/math/morphology.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      474 2023-05-12 11:28:23.000000 cartagen4py-0.1.5/cartagen4py/utils/math/vector.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/cartagen4py/utils/partitioning/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      106 2023-05-15 08:50:53.000000 cartagen4py-0.1.5/cartagen4py/utils/partitioning/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     2183 2023-05-12 11:55:23.000000 cartagen4py-0.1.5/cartagen4py/utils/partitioning/network.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      343 2023-03-20 10:07:44.000000 cartagen4py-0.1.5/cartagen4py/utils/partitioning/quadtree.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/cartagen4py/utils/tessellation/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       59 2023-05-15 08:50:31.000000 cartagen4py-0.1.5/cartagen4py/utils/tessellation/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3747 2023-03-15 09:37:20.000000 cartagen4py-0.1.5/cartagen4py/utils/tessellation/hexagonal_tess.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.513099 cartagen4py-0.1.5/cartagen4py.egg-info/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1617 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/SOURCES.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/dependency_links.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/requires.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/top_level.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/setup.cfg
+-rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     2053 2023-05-15 08:52:53.000000 cartagen4py-0.1.5/setup.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/test/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-15 08:37:58.000000 cartagen4py-0.1.5/test/test-imports.py
```

### Comparing `cartagen4py-0.1.4/PKG-INFO` & `cartagen4py-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
 Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
 License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
```

### Comparing `cartagen4py-0.1.4/cartagen4py/algorithms/buildings/amalgamation.py` & `cartagen4py-0.1.5/cartagen4py/algorithms/buildings/amalgamation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # This file contains several algorithms to amalgamate or aggregate two or more buildings
 
-from shapely.geometry import Polygon,MultiPolygon,Point
-from cartagen4py.util import morpho_math
-from cartagen4py.util.vector2D import Vector2D
 import math
-from cartagen4py.util.segment import get_segment_list
+
+from shapely.geometry import Polygon,MultiPolygon,Point
+
+from cartagen4py.utils.math.morphology import closing_multi_polygon, opening
+from cartagen4py.utils.math.vector import Vector2D
+from cartagen4py.utils.geometry.segment import get_segment_list
 
 # This the amalgamation algorithm from Damen et al. 2008 (https://www.semanticscholar.org/paper/High-Quality-Building-Generalization-by-Extending-Damen-Kreveld/b64618584b3ae3725da7eeb5a545d1580e5f2113)
 def morphological_amalgamation(buildings, buffer_size, edge_length):
     output_collection = []
     clusters = []
     multipolygon = MultiPolygon(buildings)
 
     # make a morphological closing on the multipolygon
-    closed = morpho_math.closing_multi_polygon(multipolygon, buffer_size, cap_style=2)
-    merged = morpho_math.opening(closed, buffer_size, cap_style=2)
+    closed = closing_multi_polygon(multipolygon, buffer_size, cap_style=2)
+    merged = opening(closed, buffer_size, cap_style=2)
 
     if(merged.geom_type == 'Polygon'):
         clusters.append(merged)
     elif (merged.geom_type == 'MultiPolygon'):
         for simple in merged.geoms:
             clusters.append(simple)
```

### Comparing `cartagen4py-0.1.4/cartagen4py/algorithms/buildings/random_displacement.py` & `cartagen4py-0.1.5/cartagen4py/algorithms/buildings/random_displacement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # This is an implementation of the random building displacement algorithm
 
-import random, math, shapely
-from cartagen4py.util.partitioning.network import network_partition
+import random, math
+
+import shapely
+
+from cartagen4py.utils.partitioning.network import network_partition
 
 class BuildingDisplacementRandom:
     """
     Initialize random displacement object, with default length displacement factor and number of iterations per building
     """
     def __init__(self, max_trials=25, max_displacement=10, network_partitioning=True, verbose=False):
         self.MAX_TRIALS = max_trials
```

### Comparing `cartagen4py-0.1.4/cartagen4py/algorithms/buildings/simplification.py` & `cartagen4py-0.1.5/cartagen4py/algorithms/buildings/simplification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # this file contains building simplification algorithms
-from shapely.geometry import Polygon, Point, LinearRing
-from cartagen4py.util.segment import get_segment_list_polygon, Segment
 from math import atan2, pi, sqrt
 
+from shapely.geometry import Polygon, Point, LinearRing
+
+from cartagen4py.utils.geometry.segment import get_segment_list_polygon, Segment
+
 # Building simplification algorithm from (Ruas, 1988). Port of the CartAGen implementation of the algorithm.
 def building_simplification_ruas(building, edge_threshold, parallel_limit = 20 * pi / 180, orthogonal_limit = 20 * pi / 180):
 
     # first get all the small segments in the polygon
     small_segments = __get_small_segments(building, edge_threshold)
 
     # loop on these small segments to remove them
```

### Comparing `cartagen4py-0.1.4/cartagen4py/algorithms/buildings/squaring.py` & `cartagen4py-0.1.5/cartagen4py/algorithms/buildings/squaring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # This is an implementation of the least squares based squaring algorithm proposed by Lokhat & Touya (https://hal.science/hal-02147792)
-
 import numpy as np
 
 class Squarer:
     """Initialize squaring object, with default weights and tolerance set in the constructor
     """
     def __init__(self, max_iter=1000, norm_tol=0.05,rtol=10, ftol=0.11, hrtol=7, pfixe=5, p90=100, p0=50, p45=10, switch_new=False):
         self.SWITCH_NEW = switch_new
```

### Comparing `cartagen4py-0.1.4/cartagen4py.egg-info/PKG-INFO` & `cartagen4py-0.1.5/cartagen4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
 Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
 License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
```

