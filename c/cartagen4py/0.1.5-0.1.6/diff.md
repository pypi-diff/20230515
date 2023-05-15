# Comparing `tmp/cartagen4py-0.1.5.tar.gz` & `tmp/cartagen4py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartagen4py-0.1.5.tar", last modified: Mon May 15 08:52:54 2023, max compression
+gzip compressed data, was "cartagen4py-0.1.6.tar", last modified: Mon May 15 09:06:42 2023, max compression
```

## Comparing `cartagen4py-0.1.5.tar` & `cartagen4py-0.1.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/PKG-INFO
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      229 2023-03-01 13:47:49.000000 cartagen4py-0.1.5/README.md
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.513099 cartagen4py-0.1.5/cartagen4py/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      179 2023-05-15 08:33:30.000000 cartagen4py-0.1.5/cartagen4py/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.513099 cartagen4py-0.1.5/cartagen4py/algorithms/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      134 2023-05-15 08:34:07.000000 cartagen4py-0.1.5/cartagen4py/algorithms/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-05-15 08:34:43.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4482 2023-05-15 08:35:40.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/amalgamation.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7441 2023-05-15 08:35:18.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/random_displacement.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     8000 2023-05-15 08:35:47.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/simplification.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14748 2023-05-15 08:35:50.000000 cartagen4py-0.1.5/cartagen4py/algorithms/buildings/squaring.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/algorithms/general/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       55 2023-05-12 12:21:40.000000 cartagen4py-0.1.5/cartagen4py/algorithms/general/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)    27075 2023-05-12 11:58:26.000000 cartagen4py-0.1.5/cartagen4py/algorithms/general/constraint.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/algorithms/lines/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      120 2023-05-12 12:23:23.000000 cartagen4py-0.1.5/cartagen4py/algorithms/lines/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     5310 2023-05-12 11:58:09.000000 cartagen4py-0.1.5/cartagen4py/algorithms/lines/line_simplification.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      394 2023-03-15 09:37:20.000000 cartagen4py-0.1.5/cartagen4py/algorithms/lines/line_smoothing.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/data_enrichment/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      113 2023-05-12 12:24:09.000000 cartagen4py-0.1.5/cartagen4py/data_enrichment/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1570 2023-05-12 12:24:49.000000 cartagen4py-0.1.5/cartagen4py/data_enrichment/building_measures.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1018 2023-05-12 11:58:54.000000 cartagen4py-0.1.5/cartagen4py/data_enrichment/urban_areas.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/evaluation/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.5/cartagen4py/evaluation/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      238 2023-03-01 13:47:49.000000 cartagen4py-0.1.5/cartagen4py/evaluation/constraint_satisfaction.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/processes/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.5/cartagen4py/processes/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/utils/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      210 2023-05-15 08:50:08.000000 cartagen4py-0.1.5/cartagen4py/utils/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/utils/clustering/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       49 2023-05-15 08:52:08.000000 cartagen4py-0.1.5/cartagen4py/utils/clustering/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-30 13:41:05.000000 cartagen4py-0.1.5/cartagen4py/utils/clustering/dbscan.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.517099 cartagen4py-0.1.5/cartagen4py/utils/geometry/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      189 2023-05-15 08:51:46.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      386 2023-03-15 09:37:20.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/angle.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1327 2023-03-21 13:10:50.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/extent.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1195 2023-03-30 13:41:05.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/line.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3167 2023-05-12 11:54:30.000000 cartagen4py-0.1.5/cartagen4py/utils/geometry/segment.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/cartagen4py/utils/math/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       91 2023-05-15 08:51:15.000000 cartagen4py-0.1.5/cartagen4py/utils/math/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4304 2023-04-21 08:51:00.000000 cartagen4py-0.1.5/cartagen4py/utils/math/morphology.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      474 2023-05-12 11:28:23.000000 cartagen4py-0.1.5/cartagen4py/utils/math/vector.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/cartagen4py/utils/partitioning/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      106 2023-05-15 08:50:53.000000 cartagen4py-0.1.5/cartagen4py/utils/partitioning/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     2183 2023-05-12 11:55:23.000000 cartagen4py-0.1.5/cartagen4py/utils/partitioning/network.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      343 2023-03-20 10:07:44.000000 cartagen4py-0.1.5/cartagen4py/utils/partitioning/quadtree.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/cartagen4py/utils/tessellation/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       59 2023-05-15 08:50:31.000000 cartagen4py-0.1.5/cartagen4py/utils/tessellation/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3747 2023-03-15 09:37:20.000000 cartagen4py-0.1.5/cartagen4py/utils/tessellation/hexagonal_tess.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.513099 cartagen4py-0.1.5/cartagen4py.egg-info/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/PKG-INFO
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1617 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/SOURCES.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/dependency_links.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/requires.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-15 08:52:54.000000 cartagen4py-0.1.5/cartagen4py.egg-info/top_level.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/setup.cfg
--rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     2053 2023-05-15 08:52:53.000000 cartagen4py-0.1.5/setup.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:52:54.521099 cartagen4py-0.1.5/test/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-15 08:37:58.000000 cartagen4py-0.1.5/test/test-imports.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      229 2023-03-01 13:47:49.000000 cartagen4py-0.1.6/README.md
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      179 2023-05-15 08:33:30.000000 cartagen4py-0.1.6/cartagen4py/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/algorithms/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      134 2023-05-15 08:34:07.000000 cartagen4py-0.1.6/cartagen4py/algorithms/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-05-15 08:34:43.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4482 2023-05-15 08:35:40.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/amalgamation.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7441 2023-05-15 08:35:18.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/random_displacement.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     8000 2023-05-15 08:35:47.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14748 2023-05-15 08:35:50.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/squaring.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/algorithms/general/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       55 2023-05-12 12:21:40.000000 cartagen4py-0.1.6/cartagen4py/algorithms/general/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    27075 2023-05-12 11:58:26.000000 cartagen4py-0.1.6/cartagen4py/algorithms/general/constraint.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/algorithms/lines/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      120 2023-05-12 12:23:23.000000 cartagen4py-0.1.6/cartagen4py/algorithms/lines/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     5310 2023-05-12 11:58:09.000000 cartagen4py-0.1.6/cartagen4py/algorithms/lines/line_simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      394 2023-03-15 09:37:20.000000 cartagen4py-0.1.6/cartagen4py/algorithms/lines/line_smoothing.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/data_enrichment/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      113 2023-05-12 12:24:09.000000 cartagen4py-0.1.6/cartagen4py/data_enrichment/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1570 2023-05-12 12:24:49.000000 cartagen4py-0.1.6/cartagen4py/data_enrichment/building_measures.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1018 2023-05-12 11:58:54.000000 cartagen4py-0.1.6/cartagen4py/data_enrichment/urban_areas.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/evaluation/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.6/cartagen4py/evaluation/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      238 2023-03-01 13:47:49.000000 cartagen4py-0.1.6/cartagen4py/evaluation/constraint_satisfaction.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/processes/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.6/cartagen4py/processes/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      210 2023-05-15 08:50:08.000000 cartagen4py-0.1.6/cartagen4py/utils/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/clustering/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       49 2023-05-15 08:52:08.000000 cartagen4py-0.1.6/cartagen4py/utils/clustering/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-30 13:41:05.000000 cartagen4py-0.1.6/cartagen4py/utils/clustering/dbscan.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/geometry/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      189 2023-05-15 08:51:46.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      386 2023-03-15 09:37:20.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/angle.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1327 2023-03-21 13:10:50.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/extent.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1195 2023-03-30 13:41:05.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/line.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3167 2023-05-12 11:54:30.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/segment.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/math/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       91 2023-05-15 08:51:15.000000 cartagen4py-0.1.6/cartagen4py/utils/math/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4304 2023-04-21 08:51:00.000000 cartagen4py-0.1.6/cartagen4py/utils/math/morphology.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      474 2023-05-12 11:28:23.000000 cartagen4py-0.1.6/cartagen4py/utils/math/vector.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/partitioning/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      106 2023-05-15 08:50:53.000000 cartagen4py-0.1.6/cartagen4py/utils/partitioning/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     2183 2023-05-12 11:55:23.000000 cartagen4py-0.1.6/cartagen4py/utils/partitioning/network.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      334 2023-05-15 09:06:20.000000 cartagen4py-0.1.6/cartagen4py/utils/partitioning/quadtree.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/tessellation/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       59 2023-05-15 08:50:31.000000 cartagen4py-0.1.6/cartagen4py/utils/tessellation/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3747 2023-03-15 09:37:20.000000 cartagen4py-0.1.6/cartagen4py/utils/tessellation/hexagonal_tess.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py.egg-info/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1617 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/SOURCES.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/dependency_links.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/requires.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/top_level.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/setup.cfg
+-rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     2053 2023-05-15 09:06:40.000000 cartagen4py-0.1.6/setup.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/test/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:55:39.000000 cartagen4py-0.1.6/test/test-imports.py
```

### Comparing `cartagen4py-0.1.5/PKG-INFO` & `cartagen4py-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
 Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
 License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
```

### Comparing `cartagen4py-0.1.5/cartagen4py/algorithms/buildings/amalgamation.py` & `cartagen4py-0.1.6/cartagen4py/algorithms/buildings/amalgamation.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/algorithms/buildings/random_displacement.py` & `cartagen4py-0.1.6/cartagen4py/algorithms/buildings/random_displacement.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/algorithms/buildings/simplification.py` & `cartagen4py-0.1.6/cartagen4py/algorithms/buildings/simplification.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/algorithms/buildings/squaring.py` & `cartagen4py-0.1.6/cartagen4py/algorithms/buildings/squaring.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/algorithms/general/constraint.py` & `cartagen4py-0.1.6/cartagen4py/algorithms/general/constraint.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/algorithms/lines/line_simplification.py` & `cartagen4py-0.1.6/cartagen4py/algorithms/lines/line_simplification.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/data_enrichment/building_measures.py` & `cartagen4py-0.1.6/cartagen4py/data_enrichment/building_measures.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/data_enrichment/urban_areas.py` & `cartagen4py-0.1.6/cartagen4py/data_enrichment/urban_areas.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/utils/geometry/extent.py` & `cartagen4py-0.1.6/cartagen4py/utils/geometry/extent.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/utils/geometry/line.py` & `cartagen4py-0.1.6/cartagen4py/utils/geometry/line.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/utils/geometry/segment.py` & `cartagen4py-0.1.6/cartagen4py/utils/geometry/segment.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/utils/math/morphology.py` & `cartagen4py-0.1.6/cartagen4py/utils/math/morphology.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/utils/partitioning/network.py` & `cartagen4py-0.1.6/cartagen4py/utils/partitioning/network.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py/utils/tessellation/hexagonal_tess.py` & `cartagen4py-0.1.6/cartagen4py/utils/tessellation/hexagonal_tess.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/cartagen4py.egg-info/PKG-INFO` & `cartagen4py-0.1.6/cartagen4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
 Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
 License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
```

### Comparing `cartagen4py-0.1.5/cartagen4py.egg-info/SOURCES.txt` & `cartagen4py-0.1.6/cartagen4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.5/setup.py` & `cartagen4py-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if sys.version_info[:2] < (3, 8):
     error = ('cartagen4py requires Python 3.8 or later (%d.%d detected).' % sys.version_info[:2])
     sys.stderr.write(error + "\n")
     sys.exit(1)
 
 # General informations
 name = 'cartagen4py'
-version = '0.1.5'
+version = '0.1.6'
 description = 'Python package to generalise geographic objects for cartographic purposes'
 url = 'https://github.com/LostInZoom/cartagen4py'
 author = 'Guillaume Touya, Justin Berli'
 author_email = 'guillaume.touya@ign.fr'
 lic = 'CeCILL-C'
 packages = [
     'cartagen4py',
```

