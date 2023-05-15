# Comparing `tmp/ladybug-display-0.8.0.tar.gz` & `tmp/ladybug-display-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-display-0.8.0.tar", last modified: Thu Dec 15 23:12:58 2022, max compression
+gzip compressed data, was "dist/ladybug-display-0.9.0.tar", last modified: Tue Jan 10 01:12:30 2023, max compression
```

## Comparing `ladybug-display-0.8.0.tar` & `ladybug-display-0.9.0.tar`

### file list

```diff
@@ -1,107 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/_extend_ladybug.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/altnumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/dictutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display/extension/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/extension/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/extension/hourlyplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/extension/monthlychart.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/extension/psychchart.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/extension/sunpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/extension/windprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/extension/windrose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry2d/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/cone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/polyface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/geometry3d/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    64826 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/ladybug_display/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/ladybug_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:12:58.000000 ladybug-display-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/arc2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/arc3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/cone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/cylinder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/face3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/line2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/line3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/mesh2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/mesh3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/plane_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/point2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/point3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/polyface3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/polygon2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/polyline2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/polyline3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/ray2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/ray3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/sphere_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/vector2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/vector3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2022-12-15 23:11:50.000000 ladybug-display-0.8.0/tests/visualization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/_extend_ladybug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/altnumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/dictutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/hourlyplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/monthlychart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/psychchart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/raddome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/radrose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/skydome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/sunpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/windprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/windrose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/polyface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64826 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/arc2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/arc3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/cone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/cylinder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/face3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/line2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/line3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/mesh2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/mesh3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/plane_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/point2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/point3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/polyface3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/polygon2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/polyline2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/polyline3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/ray2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/ray3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/sphere_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/vector2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/vector3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/visualization_test.py
```

### Comparing `ladybug-display-0.8.0/.github/workflows/ci.yaml` & `ladybug-display-0.9.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/LICENSE` & `ladybug-display-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/PKG-INFO` & `ladybug-display-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-display
-Version: 0.8.0
+Version: 0.9.0
 Summary: A library that assigns basic display attributes to ladybug-geometry objects (color, line weight, line type, etc).
 Home-page: https://github.com/ladybug-tools/ladybug-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `ladybug-display-0.8.0/README.md` & `ladybug-display-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/dev-requirements.txt` & `ladybug-display-0.9.0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/docs/_static/custom.css` & `ladybug-display-0.9.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/docs/_templates/layout.html` & `ladybug-display-0.9.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/docs/conf.py` & `ladybug-display-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/_base.py` & `ladybug-display-0.9.0/ladybug_display/_base.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/altnumber.py` & `ladybug-display-0.9.0/ladybug_display/altnumber.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/dictutil.py` & `ladybug-display-0.9.0/ladybug_display/dictutil.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/extension/compass.py` & `ladybug-display-0.9.0/ladybug_display/extension/compass.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,24 +90,24 @@
     # generate the labels and tick marks for the altitudes
     if projection is not None:
         if projection.title() == 'Orthographic':
             for circle in compass.orthographic_altitude_circles:
                 arc_geo = Arc3D.from_arc2d(circle, z)
                 result.append(DisplayArc3D(arc_geo, line_width=1, line_type='Dotted'))
             for txt, pt in zip(compass.ALTITUDES, compass.orthographic_altitude_points):
-                txt_pln = Plane(o=Point3D(pt.x, pt.y, z), x=xaxis)
+                txt_pln = Plane(o=Point3D(pt.x, pt.y, z + 0.01), x=xaxis)
                 d_txt = DisplayText3D(
                     str(txt), txt_pln, min_txt, None, font, 'Center', 'Top')
                 result.append(d_txt)
         elif projection.title() == 'Stereographic':
             for circle in compass.stereographic_altitude_circles:
                 arc_geo = Arc3D.from_arc2d(circle, z)
                 result.append(DisplayArc3D(arc_geo, line_width=1, line_type='Dotted'))
             for txt, pt in zip(compass.ALTITUDES, compass.stereographic_altitude_points):
-                txt_pln = Plane(o=Point3D(pt.x, pt.y, z), x=xaxis)
+                txt_pln = Plane(o=Point3D(pt.x, pt.y, z + 0.01), x=xaxis)
                 d_txt = DisplayText3D(
                     str(txt), txt_pln, min_txt, None, font, 'Center', 'Top')
                 result.append(d_txt)
 
     # assemble everything into a ContextGeometry and VisualizationSet
     con_geo = ContextGeometry('Compass', result)
     return VisualizationSet('Compass', [con_geo])
```

### Comparing `ladybug-display-0.8.0/ladybug_display/extension/hourlyplot.py` & `ladybug-display-0.9.0/ladybug_display/extension/hourlyplot.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/extension/monthlychart.py` & `ladybug-display-0.9.0/ladybug_display/extension/monthlychart.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/extension/psychchart.py` & `ladybug-display-0.9.0/ladybug_display/extension/psychchart.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/extension/sunpath.py` & `ladybug-display-0.9.0/ladybug_display/extension/sunpath.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/extension/windprofile.py` & `ladybug-display-0.9.0/ladybug_display/extension/windprofile.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/extension/windrose.py` & `ladybug-display-0.9.0/ladybug_display/extension/windrose.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/_base.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/_base.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/arc.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/arc.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/line.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/line.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/mesh.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/mesh.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/point.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/point.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/polygon.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/polygon.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/polyline.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/polyline.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/ray.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/ray.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry2d/vector.py` & `ladybug-display-0.9.0/ladybug_display/geometry2d/vector.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/__init__.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/_base.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/_base.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/arc.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/arc.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/cone.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/cone.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/cylinder.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/cylinder.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/face.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/face.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/line.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/line.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/mesh.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/mesh.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/plane.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/plane.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/point.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/point.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/polyface.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/polyface.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/polyline.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/polyline.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/ray.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/ray.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/sphere.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/sphere.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/text.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/text.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/geometry3d/vector.py` & `ladybug-display-0.9.0/ladybug_display/geometry3d/vector.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/typing.py` & `ladybug-display-0.9.0/ladybug_display/typing.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display/visualization.py` & `ladybug-display-0.9.0/ladybug_display/visualization.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/ladybug_display.egg-info/PKG-INFO` & `ladybug-display-0.9.0/ladybug_display.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-display
-Version: 0.8.0
+Version: 0.9.0
 Summary: A library that assigns basic display attributes to ladybug-geometry objects (color, line weight, line type, etc).
 Home-page: https://github.com/ladybug-tools/ladybug-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `ladybug-display-0.8.0/ladybug_display.egg-info/SOURCES.txt` & `ladybug-display-0.9.0/ladybug_display.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 ladybug_display.egg-info/requires.txt
 ladybug_display.egg-info/top_level.txt
 ladybug_display/extension/__init__.py
 ladybug_display/extension/compass.py
 ladybug_display/extension/hourlyplot.py
 ladybug_display/extension/monthlychart.py
 ladybug_display/extension/psychchart.py
+ladybug_display/extension/raddome.py
+ladybug_display/extension/radrose.py
+ladybug_display/extension/skydome.py
 ladybug_display/extension/sunpath.py
 ladybug_display/extension/windprofile.py
 ladybug_display/extension/windrose.py
 ladybug_display/geometry2d/__init__.py
 ladybug_display/geometry2d/_base.py
 ladybug_display/geometry2d/arc.py
 ladybug_display/geometry2d/line.py
```

### Comparing `ladybug-display-0.8.0/setup.py` & `ladybug-display-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/arc2d_test.py` & `ladybug-display-0.9.0/tests/arc2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/arc3d_test.py` & `ladybug-display-0.9.0/tests/arc3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/cone_test.py` & `ladybug-display-0.9.0/tests/cone_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/cylinder_test.py` & `ladybug-display-0.9.0/tests/cylinder_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/face3d_test.py` & `ladybug-display-0.9.0/tests/face3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/line2d_test.py` & `ladybug-display-0.9.0/tests/line2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/line3d_test.py` & `ladybug-display-0.9.0/tests/line3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/mesh2d_test.py` & `ladybug-display-0.9.0/tests/mesh2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/mesh3d_test.py` & `ladybug-display-0.9.0/tests/mesh3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/plane_test.py` & `ladybug-display-0.9.0/tests/plane_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/point2d_test.py` & `ladybug-display-0.9.0/tests/point2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/point3d_test.py` & `ladybug-display-0.9.0/tests/point3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/polyface3d_test.py` & `ladybug-display-0.9.0/tests/polyface3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/polygon2d_test.py` & `ladybug-display-0.9.0/tests/polygon2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/polyline2d_test.py` & `ladybug-display-0.9.0/tests/polyline2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/polyline3d_test.py` & `ladybug-display-0.9.0/tests/polyline3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/ray2d_test.py` & `ladybug-display-0.9.0/tests/ray2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/ray3d_test.py` & `ladybug-display-0.9.0/tests/ray3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/sphere_test.py` & `ladybug-display-0.9.0/tests/sphere_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/vector2d_test.py` & `ladybug-display-0.9.0/tests/vector2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/vector3d_test.py` & `ladybug-display-0.9.0/tests/vector3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.8.0/tests/visualization_test.py` & `ladybug-display-0.9.0/tests/visualization_test.py`

 * *Files identical despite different names*

