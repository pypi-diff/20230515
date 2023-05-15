# Comparing `tmp/polymetric-0.7.0.tar.gz` & `tmp/polymetric-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/polymetric-0.7.0.tar", last modified: Mon Feb 24 17:00:36 2020, max compression
+gzip compressed data, was "polymetric-0.8.0.tar", last modified: Mon May 15 07:20:27 2023, max compression
```

## Comparing `polymetric-0.7.0.tar` & `polymetric-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2020-02-24 17:00:36.000000 polymetric-0.7.0/
--rw-r--r--   0 jesse      (501) staff       (20)      535 2020-02-24 17:00:36.000000 polymetric-0.7.0/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)      110 2018-10-17 21:19:20.000000 polymetric-0.7.0/README.md
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2020-02-24 17:00:36.000000 polymetric-0.7.0/polymetric/
--rw-r--r--   0 jesse      (501) staff       (20)       25 2018-10-14 20:00:07.000000 polymetric-0.7.0/polymetric/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2020-02-24 17:00:36.000000 polymetric-0.7.0/polymetric/exporters/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2018-11-08 06:50:27.000000 polymetric-0.7.0/polymetric/exporters/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)      688 2019-08-08 16:37:03.000000 polymetric-0.7.0/polymetric/exporters/dxf.py
--rw-r--r--   0 jesse      (501) staff       (20)     2270 2019-08-08 16:37:03.000000 polymetric-0.7.0/polymetric/exporters/gds.py
--rw-r--r--   0 jesse      (501) staff       (20)     1587 2019-08-08 08:42:15.000000 polymetric-0.7.0/polymetric/plotting.py
--rw-r--r--   0 jesse      (501) staff       (20)    20601 2019-12-01 16:04:43.000000 polymetric-0.7.0/polymetric/polymetric.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2020-02-24 17:00:36.000000 polymetric-0.7.0/polymetric.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)      535 2020-02-24 17:00:36.000000 polymetric-0.7.0/polymetric.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)      347 2020-02-24 17:00:36.000000 polymetric-0.7.0/polymetric.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2020-02-24 17:00:36.000000 polymetric-0.7.0/polymetric.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)       14 2020-02-24 17:00:36.000000 polymetric-0.7.0/polymetric.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)       11 2020-02-24 17:00:36.000000 polymetric-0.7.0/polymetric.egg-info/top_level.txt
--rw-r--r--   0 jesse      (501) staff       (20)       38 2020-02-24 17:00:36.000000 polymetric-0.7.0/setup.cfg
--rw-r--r--   0 jesse      (501) staff       (20)      639 2020-02-24 16:59:13.000000 polymetric-0.7.0/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-15 07:20:27.942922 polymetric-0.8.0/
+-rw-r--r--   0 jesse      (501) staff       (20)     1067 2018-10-14 19:58:33.000000 polymetric-0.8.0/LICENSE
+-rw-r--r--   0 jesse      (501) staff       (20)      530 2023-05-15 07:20:27.942327 polymetric-0.8.0/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)      110 2018-10-17 21:19:20.000000 polymetric-0.8.0/README.md
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-15 07:20:27.934057 polymetric-0.8.0/polymetric/
+-rw-r--r--   0 jesse      (501) staff       (20)       25 2018-10-14 20:00:07.000000 polymetric-0.8.0/polymetric/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-15 07:20:27.941228 polymetric-0.8.0/polymetric/exporters/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2018-11-08 06:50:27.000000 polymetric-0.8.0/polymetric/exporters/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)      688 2019-08-08 16:37:03.000000 polymetric-0.8.0/polymetric/exporters/dxf.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2833 2020-03-04 07:33:31.000000 polymetric-0.8.0/polymetric/exporters/gds.py
+-rw-r--r--   0 jesse      (501) staff       (20)     1674 2020-03-04 07:44:17.000000 polymetric-0.8.0/polymetric/plotting.py
+-rw-r--r--   0 jesse      (501) staff       (20)    20542 2020-11-18 13:46:26.000000 polymetric-0.8.0/polymetric/polymetric.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-15 07:20:27.939318 polymetric-0.8.0/polymetric.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)      530 2023-05-15 07:20:27.000000 polymetric-0.8.0/polymetric.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)      355 2023-05-15 07:20:27.000000 polymetric-0.8.0/polymetric.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-05-15 07:20:27.000000 polymetric-0.8.0/polymetric.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       14 2023-05-15 07:20:27.000000 polymetric-0.8.0/polymetric.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       11 2023-05-15 07:20:27.000000 polymetric-0.8.0/polymetric.egg-info/top_level.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-05-15 07:20:27.943169 polymetric-0.8.0/setup.cfg
+-rw-r--r--   0 jesse      (501) staff       (20)      639 2023-05-15 07:05:49.000000 polymetric-0.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `polymetric-0.7.0/PKG-INFO` & `polymetric-0.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: polymetric
-Version: 0.7.0
+Version: 0.8.0
 Summary: Generate complex polygon structures
 Home-page: UNKNOWN
 Author: Jesse Slim
 Author-email: jesse.j.slim@gmail.com
 License: UNKNOWN
-Description: # polymetric
-        
-        Polymetric is a Python package to define and generate **poly**gon structures para**metric**ally.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# polymetric
+
+Polymetric is a Python package to define and generate **poly**gon structures para**metric**ally.
+
```

### Comparing `polymetric-0.7.0/polymetric/exporters/dxf.py` & `polymetric-0.8.0/polymetric/exporters/dxf.py`

 * *Files identical despite different names*

### Comparing `polymetric-0.7.0/polymetric/exporters/gds.py` & `polymetric-0.8.0/polymetric/exporters/gds.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import gdspy
 from importlib import reload
+from .. import polymetric as pm
 
 
-# should we reload the gdspy module every time something is saved?
+# should we reload the gdspy module every time something is saved/loaded?
+# GDSPY keeps some global library of stuff in memory that might need to be wiped
 DO_RELOAD = True
 
 # maximum number of vertices per polygon. Absolute limit set by GDS file format is 8191
 # can be adjusted by user
 MAX_VERTICES = 8000
 
 
@@ -20,16 +22,15 @@
             "Polygon contains interiors, which can not be represented"
             " in the GDS file format. To ignore, call with ignore_interiors=True")
 
     vertex_lists = shape.get_exterior_vertex_lists()
 
     for vl in vertex_lists:
         if len(vl) > MAX_VERTICES:
-            raise ValueError("Polygon contains {} vertices, more than"
-                " the limit of {} vertices".format(len(vl), MAX_VERTICES))
+            raise ValueError(f"Polygon contains {len(vl)} vertices, more than the limit of {MAX_VERTICES} vertices")
 
         # shapely always duplicates the first vertex as the last vertex, get rid of that
         gds_poly = gdspy.Polygon(vl[:-1], datatype=datatype)
         poly_cell.add(gds_poly)
 
     gdspy.write_gds(filename, **kw)
 
@@ -55,7 +56,26 @@
             if layers is not None:
                 layer = layers[i]
             # shapely always duplicates the first vertex as the last vertex, get rid of that
             gds_poly = gdspy.Polygon(vl[:-1], datatype=datatype, layer=layer)
             poly_cell.add(gds_poly)
 
     gdspy.write_gds(filename, **kw)
+
+
+def load(filename):
+    if DO_RELOAD:
+        reload(gdspy)
+
+    gdslib = gdspy.GdsLibrary(infile=filename)
+
+    polys_per_layer = {}
+
+    for _, cell in gdslib.cell_dict.items():
+        for p1 in cell.polygons:
+            for (layer, poly) in zip(p1.layers, p1.polygons):
+                if layer not in polys_per_layer:
+                    polys_per_layer[layer] = []
+
+                polys_per_layer[layer].append(pm.Polygon(shell=poly))
+
+    return polys_per_layer
```

### Comparing `polymetric-0.7.0/polymetric/plotting.py` & `polymetric-0.8.0/polymetric/plotting.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 import shapely as sp
 import shapely.geometry
 
+import copy
 
-def plot_polys(polys, cycle_colours=False, **kw):
+
+def plot_polys(polys, cycle_colours=False, interior_ls='--', **kw):
     single_color = None
     for i, outer_poly in enumerate(polys):
         if isinstance(outer_poly, (sp.geometry.MultiPolygon)):
             inner_poly = outer_poly.geoms
         else:
             inner_poly = [outer_poly]
         
         for poly in inner_poly:
             xs, ys = poly.exterior.xy
-            plot_params = dict(kw)
+            plot_params = copy.deepcopy(kw)
 
             if cycle_colours:
-                plot_params["color"] = "C%d" % (i % 10)
+                plot_params.setdefault("color", "C%d" % (i % 10))
             elif single_color is not None:
-                plot_params["color"] = single_color
+                plot_params.setdefault("color", single_color)
 
             l = plt.plot(xs, ys, **plot_params)
             if single_color is None:
                 single_color = l[0].get_color()
-                plot_params["color"] = single_color
+                plot_params.setdefault("color", single_color)
 
             # plot interiors with a different line style
-            plot_params["linestyle"] = "--"
+            plot_params.setdefault("linestyle", interior_ls)
             for interior in poly.interiors:
                 xs, ys = interior.xy
                 plt.plot(xs, ys, **plot_params)
 
 
 def plot_shapes(shapes, *more_shapes, **kw):
     if not isinstance(shapes, (list, tuple)):
```

### Comparing `polymetric-0.7.0/polymetric/polymetric.py` & `polymetric-0.8.0/polymetric/polymetric.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
         # (caching polygonizations would be the obvious solution,
         # but not trivial to get right as children might change for example)
         own_poly = self.apply(Flattened).polygonize()[0]
 
         return own_poly.bounds
 
     def __repr__(self):
-        child_reps = [repr(child) for child in self.children]
         class_name = type(self).__name__
 
         # # we prepend the list with an empty string, to make sure that the param string, if there are any params,
         # # starts with a ', '. This way we can immediately insert it after the other constructor arguments
         # params_as_arguments = ['']
         # for k, v in self._params.items():
         #     if k in self._params_excluded_from_repr:
@@ -135,15 +134,15 @@
 
         param_string = ", ".join(
             # we prepend the list with an empty string, to make sure that the param string, if there are any params,
             # starts with a ', '. This way we can immediately insert it after the other constructor arguments
             [''] + [f"{k}={repr(v)}" for k, v in self._params.items() if k not in self._params_excluded_from_repr]
         )
 
-        full_repr = f"{class_name}(children={repr(child_reps)}, name={repr(self.name)}{param_string})"
+        full_repr = f"{class_name}(children={repr(self.children)}, name={repr(self.name)}{param_string})"
         return full_repr
 
 
 class EmptyShape(Shape):
     def _polygonize(self):
         return [shapely.geometry.Polygon()]
```

### Comparing `polymetric-0.7.0/polymetric.egg-info/PKG-INFO` & `polymetric-0.8.0/polymetric.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: polymetric
-Version: 0.7.0
+Version: 0.8.0
 Summary: Generate complex polygon structures
 Home-page: UNKNOWN
 Author: Jesse Slim
 Author-email: jesse.j.slim@gmail.com
 License: UNKNOWN
-Description: # polymetric
-        
-        Polymetric is a Python package to define and generate **poly**gon structures para**metric**ally.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# polymetric
+
+Polymetric is a Python package to define and generate **poly**gon structures para**metric**ally.
+
```

### Comparing `polymetric-0.7.0/setup.py` & `polymetric-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="polymetric",
-    version="0.7.0",
+    version="0.8.0",
     author="Jesse Slim",
     author_email="jesse.j.slim@gmail.com",
     description="Generate complex polygon structures",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

