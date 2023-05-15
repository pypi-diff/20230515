# Comparing `tmp/sect-6.1.0.tar.gz` & `tmp/sect-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sect-6.1.0.tar", last modified: Thu Apr 21 06:47:18 2022, max compression
+gzip compressed data, was "sect-7.0.0.tar", last modified: Mon May 15 00:36:00 2023, max compression
```

## Comparing `sect-6.1.0.tar` & `sect-7.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:18.175149 sect-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-04-21 06:47:01.000000 sect-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-04-21 06:47:01.000000 sect-6.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6394 2022-04-21 06:47:18.171149 sect-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5561 2022-04-21 06:47:01.000000 sect-6.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-04-21 06:47:01.000000 sect-6.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:18.171149 sect-6.1.0/sect/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-04-21 06:47:01.000000 sect-6.1.0/sect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:18.171149 sect-6.1.0/sect/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:18.171149 sect-6.1.0/sect/core/delaunay/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/delaunay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/delaunay/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     7892 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/delaunay/events_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/delaunay/hints.py
--rw-r--r--   0 runner    (1001) docker     (121)     5539 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/delaunay/quad_edge.py
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/delaunay/sweep_line.py
--rw-r--r--   0 runner    (1001) docker     (121)    19276 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/delaunay/triangulation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5295 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/delaunay/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:18.171149 sect-6.1.0/sect/core/trapezoidal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/edge.py
--rw-r--r--   0 runner    (1001) docker     (121)    16340 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/hints.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/leaf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/trapezoid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/x_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/trapezoidal/y_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-04-21 06:47:01.000000 sect-6.1.0/sect/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-04-21 06:47:01.000000 sect-6.1.0/sect/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-04-21 06:47:01.000000 sect-6.1.0/sect/triangulation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 06:47:18.171149 sect-6.1.0/sect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6394 2022-04-21 06:47:17.000000 sect-6.1.0/sect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-04-21 06:47:18.000000 sect-6.1.0/sect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 06:47:17.000000 sect-6.1.0/sect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-04-21 06:47:17.000000 sect-6.1.0/sect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-21 06:47:18.000000 sect-6.1.0/sect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-21 06:47:18.175149 sect-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-04-21 06:47:01.000000 sect-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.302933 sect-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 00:35:47.000000 sect-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 00:35:47.000000 sect-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-15 00:36:00.298933 sect-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-15 00:35:47.000000 sect-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-15 00:35:47.000000 sect-7.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 00:35:47.000000 sect-7.0.0/sect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect/core/delaunay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/events_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/quad_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/sweep_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19304 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/delaunay/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect/core/trapezoidal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/trapezoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/x_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/trapezoidal/y_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 00:35:47.000000 sect-7.0.0/sect/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 00:35:47.000000 sect-7.0.0/sect/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 00:35:47.000000 sect-7.0.0/sect/triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:36:00.298933 sect-7.0.0/sect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 00:36:00.000000 sect-7.0.0/sect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 00:36:00.302933 sect-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 00:35:47.000000 sect-7.0.0/setup.py
```

### Comparing `sect-6.1.0/LICENSE` & `sect-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/PKG-INFO` & `sect-7.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,18 @@
-Metadata-Version: 2.1
-Name: sect
-Version: 6.1.0
-Summary: Geometric objects partitioning.
-Home-page: https://github.com/lycantropos/sect/
-Download-URL: https://github.com/lycantropos/sect/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
-License: MIT License
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 sect
 ====
 
 [![](https://github.com/lycantropos/sect/workflows/CI/badge.svg)](https://github.com/lycantropos/sect/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/sect/badge/?version=latest)](https://sect.readthedocs.io/en/latest "Documentation")
 [![](https://codecov.io/gh/lycantropos/sect/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/sect "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/sect.svg)](https://github.com/lycantropos/sect/blob/master/LICENSE "License")
 [![](https://badge.fury.io/py/sect.svg)](https://badge.fury.io/py/sect "PyPI")
 
-In what follows `python` is an alias for `python3.6` or `pypy3.6`
-or any later version (`python3.7`, `pypy3.7` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.8`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
@@ -88,29 +66,32 @@
 ...                         context=context).triangles()
 ...  == [Contour([Point(0, 1), Point(1, 0), Point(1, 1)]),
 ...      Contour([Point(0, 0), Point(1, 0), Point(0, 1)])])
 True
 >>> Polygon = context.polygon_cls
 >>> (Triangulation.constrained_delaunay(
 ...      Polygon(Contour([Point(0, 0), Point(1, 0), Point(0, 1)]), []),
-...      context=context).triangles()
+...      context=context
+...  ).triangles()
 ...  == [Contour([Point(0, 0), Point(1, 0), Point(0, 1)])])
 True
 >>> (Triangulation.constrained_delaunay(
 ...      Polygon(Contour([Point(0, 0), Point(3, 0), Point(1, 1), Point(0, 3)]),
 ...              []),
-...      context=context).triangles()
+...      context=context
+...  ).triangles()
 ...  == [Contour([Point(0, 0), Point(3, 0), Point(1, 1)]),
 ...      Contour([Point(0, 0), Point(1, 1), Point(0, 3)])])
 True
 >>> (Triangulation.constrained_delaunay(
 ...      Polygon(Contour([Point(0, 0), Point(4, 0), Point(0, 4)]),
 ...              [Contour([Point(0, 0), Point(1, 2),
 ...                        Point(2, 1)])]),
-...      context=context).triangles()
+...      context=context
+...  ).triangles()
 ...  == [Contour([Point(0, 0), Point(4, 0), Point(2, 1)]),
 ...      Contour([Point(1, 2), Point(2, 1), Point(4, 0)]),
 ...      Contour([Point(0, 4), Point(1, 2), Point(4, 0)]),
 ...      Contour([Point(0, 0), Point(1, 2), Point(0, 4)])])
 True
 >>> from sect.decomposition import Graph
 >>> graph = Graph.from_polygon(Polygon(Contour([Point(0, 0), Point(6, 0),
@@ -228,9 +209,7 @@
   ```powershell
   .\run-tests.ps1 cpython
   ```
 - with `PyPy`
   ```powershell
   .\run-tests.ps1 pypy
   ```
-
-
```

### Comparing `sect-6.1.0/sect/core/delaunay/event.py` & `sect-7.0.0/sect/core/delaunay/event.py`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/sect/core/delaunay/events_queue.py` & `sect-7.0.0/sect/core/delaunay/events_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,20 +93,22 @@
                                  'should not overlap.')
             starts_equal = below_event.start == event.start
             ends_equal = below_event.end == event.end
             start_min, start_max = (
                 (event, below_event)
                 if starts_equal or (self._queue.key(event)
                                     < self._queue.key(below_event))
-                else (below_event, event))
+                else (below_event, event)
+            )
             end_min, end_max = (
                 (event.right, below_event.right)
                 if ends_equal or (self._queue.key(event.right)
                                   < self._queue.key(below_event.right))
-                else (below_event.right, event.right))
+                else (below_event.right, event.right)
+            )
             if starts_equal:
                 # both line segments are equal or share the left endpoint
                 event.is_overlap = below_event.is_overlap = True
                 if not ends_equal:
                     self.divide_segment(end_max.left, end_min.start)
                 return True
             elif ends_equal:
@@ -131,26 +133,28 @@
 
     def register_edge(self,
                       edge: QuadEdge,
                       *,
                       from_first: bool,
                       is_counterclockwise_contour: bool) -> None:
         start_event = LeftEvent.from_segment_endpoints(
-                to_endpoints(edge), from_first, is_counterclockwise_contour)
+                to_endpoints(edge), from_first, is_counterclockwise_contour
+        )
         start_event.edge = edge
         self.push(start_event)
         self.push(start_event.right)
 
     def register_segment(self,
                          endpoints: SegmentEndpoints,
                          *,
                          from_first: bool,
                          is_counterclockwise_contour: bool) -> None:
         start_event = LeftEvent.from_segment_endpoints(
-                endpoints, from_first, is_counterclockwise_contour)
+                endpoints, from_first, is_counterclockwise_contour
+        )
         self.push(start_event)
         self.push(start_event.right)
 
     def sweep(self) -> Iterable[LeftEvent]:
         sweep_line = SweepLine(self.context)
         queue = self._queue
         while queue:
```

### Comparing `sect-6.1.0/sect/core/delaunay/quad_edge.py` & `sect-7.0.0/sect/core/delaunay/quad_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,35 +40,35 @@
         return result
 
     @property
     def context(self) -> Context:
         return self._context
 
     @property
-    def left_from_start(self) -> 'QuadEdge':
-        """
-        aka "Onext" in L. Guibas and J. Stolfi notation.
-        """
-        return self._left_from_start
-
-    @property
     def end(self) -> Point:
         """
         aka "Dest" in L. Guibas and J. Stolfi notation.
         """
         return self.opposite.start
 
     @property
     def left_from_end(self) -> 'QuadEdge':
         """
         aka "Lnext" in L. Guibas and J. Stolfi notation.
         """
         return self.rotated.opposite.left_from_start.rotated
 
     @property
+    def left_from_start(self) -> 'QuadEdge':
+        """
+        aka "Onext" in L. Guibas and J. Stolfi notation.
+        """
+        return self._left_from_start
+
+    @property
     def opposite(self) -> 'QuadEdge':
         """
         aka "Sym" in L. Guibas and J. Stolfi notation.
         """
         return self.rotated.rotated
 
     @property
@@ -130,17 +130,19 @@
         return self.context.angle_orientation(self.start, self.end, point)
 
     def splice(self, other: 'QuadEdge') -> None:
         """Splices the edge with the other."""
         alpha = self.left_from_start.rotated
         beta = other.left_from_start.rotated
         self._left_from_start, other._left_from_start = (
-            other.left_from_start, self.left_from_start)
+            other.left_from_start, self.left_from_start
+        )
         alpha._left_from_start, beta._left_from_start = (
-            beta.left_from_start, alpha.left_from_start)
+            beta.left_from_start, alpha.left_from_start
+        )
 
     def swap(self) -> None:
         """
         Swaps diagonal in a quadrilateral formed by triangles
         in both clockwise and counterclockwise order around the start.
         """
         side = self.right_from_start
```

### Comparing `sect-6.1.0/sect/core/delaunay/sweep_line.py` & `sect-7.0.0/sect/core/delaunay/sweep_line.py`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/sect/core/delaunay/triangulation.py` & `sect-7.0.0/sect/core/delaunay/triangulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
                     Optional,
                     Sequence,
                     Set,
                     Type)
 
 from decision.partition import coin_change
 from ground.base import (Context,
-                         Location, Orientation,
+                         Location,
+                         Orientation,
                          Relation)
 from ground.hints import (Contour,
                           Point,
                           Polygon,
                           Segment)
 from reprit.base import generate_repr
 
@@ -94,30 +95,32 @@
         :returns:
             triangulation of the border, holes & extra points
             considering constraints.
         """
         border, holes = polygon.border, polygon.holes
         if extra_points:
             border, holes, extra_points = complete_vertices(
-                    border, holes, extra_points, context)
+                    border, holes, extra_points, context
+            )
         result = cls.delaunay(list(chain(border.vertices,
                                          flatten(hole.vertices
                                                  for hole in holes),
                                          extra_points)),
                               context=context)
         border_edges = context.contour_segments(border)
         constrain(result, chain(border_edges,
                                 flatten(map(context.contour_segments, holes)),
                                 extra_constraints))
         bound(result, border_edges)
         cut(result, holes)
         result._triangular_holes_vertices.update(
                 frozenset(hole.vertices)
                 for hole in holes
-                if len(hole.vertices) == 3)
+                if len(hole.vertices) == 3
+        )
         return result
 
     @classmethod
     def delaunay(cls,
                  points: Sequence[Point],
                  *,
                  context: Context) -> 'Triangulation':
@@ -135,16 +138,15 @@
 
         :param points: 3 or more points to triangulate.
         :param context: geometric context.
         :returns: triangulation of the points.
         """
         points = sorted(to_distinct(points))
         lengths = coin_change(len(points), base_cases)
-        result = [cls._initialize_triangulation(points[start:stop],
-                                                context)
+        result = [cls._initialize_triangulation(points[start:stop], context)
                   for start, stop in pairwise(accumulate((0,) + lengths))]
         for _ in repeat(None, ceil_log2(len(result))):
             parts_to_merge_count = len(result) // 2 * 2
             result = ([merge(result[offset], result[offset + 1])
                        for offset in range(0, parts_to_merge_count, 2)]
                       + result[parts_to_merge_count:])
         return result[0]
@@ -174,15 +176,16 @@
         """Returns triangles of the triangulation."""
         vertices_sets = to_distinct(
                 frozenset((edge.start, edge.end, edge.left_from_start.end))
                 for edge in to_edges(self)
                 if (edge.left_from_start.end
                     == edge.opposite.right_from_start.end
                     and (edge.orientation_of(edge.left_from_start.end)
-                         is Orientation.COUNTERCLOCKWISE)))
+                         is Orientation.COUNTERCLOCKWISE))
+        )
         contour_cls, orienteer = (self.context.contour_cls,
                                   self.context.angle_orientation)
         return [contour_cls(normalize_contour_vertices(list(vertices),
                                                        orienteer))
                 for vertices in vertices_sets
                 if vertices not in self._triangular_holes_vertices]
 
@@ -209,43 +212,45 @@
 
 
 def connect(base_edge: QuadEdge,
             point_in_circle_locator: PointInCircleLocator) -> None:
     while True:
         left_candidate, right_candidate = (
             to_left_candidate(base_edge, point_in_circle_locator),
-            to_right_candidate(base_edge, point_in_circle_locator))
+            to_right_candidate(base_edge, point_in_circle_locator)
+        )
         if left_candidate is right_candidate is None:
             break
         base_edge = (
             right_candidate.connect(base_edge.opposite)
             if (left_candidate is None
                 or right_candidate is not None
                 and (point_in_circle_locator(right_candidate.end,
                                              left_candidate.end, base_edge.end,
                                              base_edge.start)
                      is Location.INTERIOR))
-            else base_edge.opposite.connect(left_candidate.opposite))
+            else base_edge.opposite.connect(left_candidate.opposite)
+        )
 
 
 def constrain(triangulation: Triangulation,
               constraints: Iterable[Segment]) -> None:
     endpoints = {to_endpoints(edge) for edge in to_edges(triangulation)}
     inner_edges = to_unique_inner_edges(triangulation)
     point_in_circle_locator, segments_relater = (
         triangulation.context.locate_point_in_point_point_point_circle,
-        triangulation.context.segments_relation)
+        triangulation.context.segments_relation
+    )
     for constraint in constraints:
         constraint_endpoints = to_endpoints(constraint)
         if constraint_endpoints in endpoints:
             continue
         crossings = detect_crossings(inner_edges, constraint, segments_relater)
         inner_edges.difference_update(crossings)
-        endpoints.difference_update(to_endpoints(edge)
-                                    for edge in crossings)
+        endpoints.difference_update(to_endpoints(edge) for edge in crossings)
         new_edges = resolve_crossings(crossings, constraint, segments_relater)
         set_criterion({edge
                        for edge in new_edges
                        if to_endpoints(edge) != constraint_endpoints},
                       point_in_circle_locator)
         endpoints.update(to_endpoints(edge) for edge in new_edges)
         inner_edges.update(new_edges)
@@ -260,15 +265,16 @@
                                    from_first=True,
                                    is_counterclockwise_contour=True)
     orienteer = triangulation.context.angle_orientation
     for hole in holes:
         for endpoints in contour_to_oriented_edges_endpoints(
                 hole,
                 clockwise=True,
-                orienteer=orienteer):
+                orienteer=orienteer
+        ):
             events_queue.register_segment(endpoints,
                                           from_first=False,
                                           is_counterclockwise_contour=False)
     for event in events_queue.sweep():
         if event.from_first and event.inside:
             triangulation.delete(event.edge)
 
@@ -291,46 +297,48 @@
                  is Location.INTERIOR
                  or (point_in_circle_locator(edge.left_from_start.end,
                                              edge.end, edge.start,
                                              edge.right_from_start.end)
                      is Location.INTERIOR)))
 
 
-def find_base_edge(left: Triangulation, right: Triangulation) -> QuadEdge:
+def find_base_edge(first: Triangulation, second: Triangulation) -> QuadEdge:
     while True:
-        if (left.right_side.orientation_of(right.left_side.start)
+        if (first.right_side.orientation_of(second.left_side.start)
                 is Orientation.COUNTERCLOCKWISE):
-            left.right_side = left.right_side.left_from_end
-        elif (right.left_side.orientation_of(left.right_side.start)
+            first.right_side = first.right_side.left_from_end
+        elif (second.left_side.orientation_of(first.right_side.start)
               is Orientation.CLOCKWISE):
-            right.left_side = right.left_side.right_from_end
+            second.left_side = second.left_side.right_from_end
         else:
             break
-    base_edge = right.left_side.opposite.connect(left.right_side)
-    if left.right_side.start == left.left_side.start:
-        left.left_side = base_edge.opposite
-    if right.left_side.start == right.right_side.start:
-        right.right_side = base_edge
+    base_edge = second.left_side.opposite.connect(first.right_side)
+    if first.right_side.start == first.left_side.start:
+        first.left_side = base_edge.opposite
+    if second.left_side.start == second.right_side.start:
+        second.right_side = base_edge
     return base_edge
 
 
 def is_convex_quadrilateral_diagonal(edge: QuadEdge) -> bool:
     return (edge.right_from_start.orientation_of(edge.end)
             is Orientation.COUNTERCLOCKWISE
             is edge.right_from_end.opposite.orientation_of(
-                    edge.left_from_start.end)
+                    edge.left_from_start.end
+            )
             is edge.left_from_end.orientation_of(edge.start)
             is edge.left_from_start.opposite.orientation_of(
-                    edge.right_from_start.end))
+                    edge.right_from_start.end
+            ))
 
 
-def merge(left: Triangulation, right: Triangulation) -> Triangulation:
-    connect(find_base_edge(left, right),
-            left.context.locate_point_in_point_point_point_circle)
-    return type(left)(left.left_side, right.right_side, left.context)
+def merge(first: Triangulation, second: Triangulation) -> Triangulation:
+    connect(find_base_edge(first, second),
+            first.context.locate_point_in_point_point_point_circle)
+    return type(first)(first.left_side, second.right_side, first.context)
 
 
 def resolve_crossings(crossings: List[QuadEdge],
                       constraint: Segment,
                       segments_relater: SegmentsRelater) -> List[QuadEdge]:
     result = []
     crossings = deque(crossings,
@@ -347,18 +355,19 @@
             crossings.append(edge)
     return result
 
 
 def set_criterion(target_edges: Set[QuadEdge],
                   point_in_circle_locator: PointInCircleLocator) -> None:
     while True:
-        edges_to_swap = {edge
-                         for edge in target_edges
-                         if
-                         edge_should_be_swapped(edge, point_in_circle_locator)}
+        edges_to_swap = {
+            edge
+            for edge in target_edges
+            if edge_should_be_swapped(edge, point_in_circle_locator)
+        }
         if not edges_to_swap:
             break
         for edge in edges_to_swap:
             edge.swap()
         target_edges.difference_update(edges_to_swap)
```

### Comparing `sect-6.1.0/sect/core/delaunay/utils.py` & `sect-7.0.0/sect/core/delaunay/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,26 @@
                       holes: Sequence[Contour],
                       candidates: Sequence[Point],
                       context: Context
                       ) -> Tuple[Contour, Sequence[Contour], Sequence[Point]]:
     candidates = sorted(to_distinct(candidates))
     contour_cls, segment_cls, segment_point_relater = (
         context.contour_cls, context.segment_cls,
-        context.segment_contains_point)
+        context.segment_contains_point
+    )
     border, candidates = _complete_contour_vertices(
             border, candidates, contour_cls, segment_cls,
-            segment_point_relater)
+            segment_point_relater
+    )
     completed_holes = []
     for hole in holes:
         hole, candidates = _complete_contour_vertices(
                 hole, candidates, contour_cls, segment_cls,
-                segment_point_relater)
+                segment_point_relater
+        )
         completed_holes.append(hole)
     return border, completed_holes, candidates
 
 
 def contour_to_oriented_edges_endpoints(contour: Contour,
                                         *,
                                         clockwise: bool,
@@ -89,15 +92,16 @@
                                   bisect(candidates, end))
         if start_index > end_index:
             start_index, end_index = end_index, start_index
         extra_vertices_indices = [
             candidate_index
             for candidate_index in range(start_index, end_index)
             if _is_inner_segment_point(start, end, candidates[candidate_index],
-                                       segment_cls, containment_checker)]
+                                       segment_cls, containment_checker)
+        ]
         if extra_vertices_indices:
             extra_vertices[index] = [candidates[index]
                                      for index in extra_vertices_indices]
             extra_vertices_indices = frozenset(extra_vertices_indices)
             candidates = [point
                           for index, point in enumerate(candidates)
                           if index not in extra_vertices_indices]
@@ -107,15 +111,16 @@
     if extra_vertices:
         contour = contour_cls(
                 list(flatten((extra_vertices[index]
                               if vertices[index - 1] < vertex
                               else extra_vertices[index][::-1]) + [vertex]
                              if index in extra_vertices
                              else [vertex]
-                             for index, vertex in enumerate(vertices))))
+                             for index, vertex in enumerate(vertices)))
+        )
     return contour, candidates
 
 
 def _is_inner_segment_point(start: Point,
                             end: Point,
                             point: Point,
                             segment_cls: Type[Segment],
```

### Comparing `sect-6.1.0/sect/core/trapezoidal/edge.py` & `sect-7.0.0/sect/core/trapezoidal/edge.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     def __init__(self,
                  left: Point,
                  right: Point,
                  interior_to_left: bool,
                  context: Context) -> None:
         assert left < right, 'Incorrect endpoints order'
         self.context, self.interior_to_left, self.left, self.right = (
-            context, interior_to_left, left, right)
+            context, interior_to_left, left, right
+        )
 
     def __lt__(self, other: 'Edge') -> bool:
         """Checks if the edge is lower than the other."""
         other_left_orientation = self.orientation_of(other.left)
         other_right_orientation = self.orientation_of(other.right)
         if other_left_orientation is other_right_orientation:
             return other_left_orientation is Orientation.COUNTERCLOCKWISE
```

### Comparing `sect-6.1.0/sect/core/trapezoidal/graph.py` & `sect-7.0.0/sect/core/trapezoidal/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
         >>> context = get_context()
         >>> Multisegment, Point, Segment = (context.multisegment_cls,
         ...                                 context.point_cls,
         ...                                 context.segment_cls)
         >>> graph = Graph.from_multisegment(
         ...     Multisegment([Segment(Point(0, 0), Point(1, 0)),
         ...                   Segment(Point(0, 0), Point(0, 1))]),
-        ...     context=context)
+        ...     context=context
+        ... )
         >>> Point(1, 0) in graph
         True
         >>> Point(0, 1) in graph
         True
         >>> Point(1, 1) in graph
         False
         >>> graph.locate(Point(1, 0)) is Location.BOUNDARY
@@ -131,15 +132,16 @@
         >>> Contour, Point, Polygon = (context.contour_cls, context.point_cls,
         ...                            context.polygon_cls)
         >>> graph = Graph.from_polygon(
         ...     Polygon(Contour([Point(0, 0), Point(6, 0), Point(6, 6),
         ...                      Point(0, 6)]),
         ...             [Contour([Point(2, 2), Point(2, 4), Point(4, 4),
         ...                       Point(4, 2)])]),
-        ...     context=context)
+        ...     context=context
+        ... )
         >>> Point(1, 1) in graph
         True
         >>> Point(2, 2) in graph
         True
         >>> Point(3, 3) in graph
         False
         >>> graph.locate(Point(1, 1)) is Location.INTERIOR
@@ -161,25 +163,27 @@
             else Edge.from_endpoints(end, start,
                                      not is_border_positively_oriented,
                                      context)
             for start, end in contour_to_edges_endpoints(border)]
         for hole in polygon.holes:
             is_hole_negatively_oriented = (
                     to_contour_orientation(hole, orienteer)
-                    is Orientation.CLOCKWISE)
+                    is Orientation.CLOCKWISE
+            )
             edges.extend(
                     Edge.from_endpoints(start, end,
                                         is_hole_negatively_oriented,
                                         context)
                     if start < end
                     else
                     Edge.from_endpoints(end, start,
                                         not is_hole_negatively_oriented,
                                         context)
-                    for start, end in contour_to_edges_endpoints(hole))
+                    for start, end in contour_to_edges_endpoints(hole)
+            )
         shuffler(edges)
         result = cls(box_to_node(context.contour_box(border), context))
         for edge in edges:
             add_edge(result, edge)
         return result
 
     @property
@@ -311,21 +315,23 @@
                 above.upper_right = trapezoid.upper_right
             # connect to new trapezoids replacing old
             if below is not prev_below:
                 below.upper_left = prev_below
                 below.lower_left = (
                     prev_below
                     if trapezoid.lower_left is prev_trapezoid
-                    else trapezoid.lower_left)
+                    else trapezoid.lower_left
+                )
             if above is not prev_above:
                 above.lower_left = prev_above
                 above.upper_left = (
                     prev_above
                     if trapezoid.upper_left is prev_trapezoid
-                    else trapezoid.upper_left)
+                    else trapezoid.upper_left
+                )
         else:
             # middle trapezoid,
             # old trapezoid is neither the first
             # nor last of the 3+ trapezoids
             # that the segment intersects
             if prev_below.below is trapezoid.below:
                 below = prev_below
@@ -342,22 +348,24 @@
             # connect to new trapezoids replacing prev_trapezoid
             if below is not prev_below:
                 # below is new
                 below.upper_left = prev_below
                 below.lower_left = (
                     prev_below
                     if trapezoid.lower_left is prev_trapezoid
-                    else trapezoid.lower_left)
+                    else trapezoid.lower_left
+                )
             if above is not prev_above:
                 # above is new
                 above.lower_left = prev_above
                 above.upper_left = (
                     prev_above
                     if trapezoid.upper_left is prev_trapezoid
-                    else trapezoid.upper_left)
+                    else trapezoid.upper_left
+                )
             below.lower_right = trapezoid.lower_right
             above.upper_right = trapezoid.upper_right
         candidate = YNode(edge,
                           below.node
                           if below is prev_below
                           else Leaf(below),
                           above.node
@@ -380,22 +388,23 @@
     min_x, min_y, max_x, max_y = box.min_x, box.min_y, box.max_x, box.max_y
     delta_x, delta_y = max_x - min_x, max_y - min_y
     # handle horizontal/vertical cases
     delta_x, delta_y = delta_x or 1, delta_y or 1
     min_x, min_y, max_x, max_y = (min_x - delta_x, min_y - delta_y,
                                   max_x + delta_x, max_y + delta_y)
     point_cls = context.point_cls
-    return Leaf(Trapezoid(
-            point_cls(min_x, min_y), point_cls(max_x, min_y),
-            Edge.from_endpoints(point_cls(min_x, min_y),
-                                point_cls(max_x, min_y), False,
-                                context),
-            Edge.from_endpoints(point_cls(min_x, max_y),
-                                point_cls(max_x, max_y), True,
-                                context)))
+    return Leaf(
+            Trapezoid(point_cls(min_x, min_y), point_cls(max_x, min_y),
+                      Edge.from_endpoints(point_cls(min_x, min_y),
+                                          point_cls(max_x, min_y), False,
+                                          context),
+                      Edge.from_endpoints(point_cls(min_x, max_y),
+                                          point_cls(max_x, max_y), True,
+                                          context))
+    )
 
 
 def find_intersecting_trapezoids(graph: Graph, edge: Edge) -> List[Trapezoid]:
     trapezoid = graph.root.search_edge(edge)
     result = [trapezoid]
     right = edge.right
     while trapezoid.right < right:
```

### Comparing `sect-6.1.0/sect/core/trapezoidal/leaf.py` & `sect-7.0.0/sect/core/trapezoidal/leaf.py`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/sect/core/trapezoidal/node.py` & `sect-7.0.0/sect/core/trapezoidal/node.py`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/sect/core/trapezoidal/trapezoid.py` & `sect-7.0.0/sect/core/trapezoidal/trapezoid.py`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/sect/core/trapezoidal/x_node.py` & `sect-7.0.0/sect/core/trapezoidal/x_node.py`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/sect/core/trapezoidal/y_node.py` & `sect-7.0.0/sect/core/trapezoidal/y_node.py`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/sect/core/utils.py` & `sect-7.0.0/sect/core/utils.py`

 * *Files identical despite different names*

### Comparing `sect-6.1.0/sect.egg-info/SOURCES.txt` & `sect-7.0.0/sect.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.py
 sect/__init__.py
 sect/decomposition.py
 sect/triangulation.py
 sect.egg-info/PKG-INFO
 sect.egg-info/SOURCES.txt
 sect.egg-info/dependency_links.txt
```

