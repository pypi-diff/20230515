# Comparing `tmp/ImoT_tools-1.1.0.tar.gz` & `tmp/ImoT_tools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ImoT_tools-1.1.0.tar", last modified: Thu Oct 22 15:21:55 2020, max compression
+gzip compressed data, was "ImoT_tools-1.2.0.tar", last modified: Mon May 15 14:10:11 2023, max compression
```

## Comparing `ImoT_tools-1.1.0.tar` & `ImoT_tools-1.2.0.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/
--rw-r--r--   0 sep       (1000) sep       (1000)       42 2020-10-22 15:21:54.000000 ImoT_tools-1.1.0/AUTHORS
--rw-r--r--   0 sep       (1000) sep       (1000)      299 2020-10-22 15:21:54.000000 ImoT_tools-1.1.0/ChangeLog
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/ImoT_tools.egg-info/
--rw-r--r--   0 sep       (1000) sep       (1000)     1293 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/ImoT_tools.egg-info/PKG-INFO
--rw-r--r--   0 sep       (1000) sep       (1000)     2294 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/ImoT_tools.egg-info/SOURCES.txt
--rw-r--r--   0 sep       (1000) sep       (1000)        1 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/ImoT_tools.egg-info/dependency_links.txt
--rw-r--r--   0 sep       (1000) sep       (1000)        1 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/ImoT_tools.egg-info/not-zip-safe
--rw-r--r--   0 sep       (1000) sep       (1000)       47 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/ImoT_tools.egg-info/pbr.json
--rw-r--r--   0 sep       (1000) sep       (1000)       94 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/ImoT_tools.egg-info/requires.txt
--rw-r--r--   0 sep       (1000) sep       (1000)       11 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/ImoT_tools.egg-info/top_level.txt
--rw-r--r--   0 sep       (1000) sep       (1000)     1536 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/LICENSE.txt
--rw-r--r--   0 sep       (1000) sep       (1000)     1293 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/PKG-INFO
--rw-r--r--   0 sep       (1000) sep       (1000)      419 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/README.rst
--rw-r--r--   0 sep       (1000) sep       (1000)       77 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/codestyle.toml
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/doc/
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/doc/api/
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/doc/api/_img/
--rw-r--r--   0 sep       (1000) sep       (1000)    18299 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/doc/api/_img/cmap_example.png
--rw-r--r--   0 sep       (1000) sep       (1000)    21703 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/_img/colorbar_example.png
--rw-r--r--   0 sep       (1000) sep       (1000)    67060 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/_img/sph_dirichlet_example.png
--rw-r--r--   0 sep       (1000) sep       (1000)   145936 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/_img/sphericalimage_aeqd_example.png
--rw-r--r--   0 sep       (1000) sep       (1000)   132430 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/_img/sphericalimage_gnom_example.png
--rw-r--r--   0 sep       (1000) sep       (1000)   127199 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/_img/sphericalimage_lcc_example.png
--rw-r--r--   0 sep       (1000) sep       (1000)      152 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/doc/api/imot_tools.io.plot.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      163 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.io.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      286 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.io.s2image.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      221 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.func.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      219 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.linalg.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      252 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      313 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.special.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      231 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.sphere.grid.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      263 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.sphere.interpolate.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      249 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.sphere.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      294 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.sphere.transform.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      207 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.math.stat.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      228 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.phased_array.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      548 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/doc/api/imot_tools.util.argcheck.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      189 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.util.array.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      175 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/imot_tools.util.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      384 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/api/index.rst
--rw-r--r--   0 sep       (1000) sep       (1000)     3428 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/conf.py
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/doc/general/
--rw-r--r--   0 sep       (1000) sep       (1000)      300 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/general/index.rst
--rw-r--r--   0 sep       (1000) sep       (1000)     1003 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/doc/general/install.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      586 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/index.rst
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/doc/notes/
--rw-r--r--   0 sep       (1000) sep       (1000)     3077 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/notes/func_interpolation_OL_zonal.rst
--rw-r--r--   0 sep       (1000) sep       (1000)      316 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/doc/notes/index.rst
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/
--rw-r--r--   0 sep       (1000) sep       (1000)      241 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/__init__.py
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/data/
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/data/io/
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/data/io/colormap/
--rw-r--r--   0 sep       (1000) sep       (1000)     1501 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/data/io/colormap/algue.csv
--rw-r--r--   0 sep       (1000) sep       (1000)     1382 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/data/io/colormap/aqua.csv
--rw-r--r--   0 sep       (1000) sep       (1000)     1202 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/data/io/colormap/fire.csv
--rw-r--r--   0 sep       (1000) sep       (1000)     1852 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/data/io/colormap/jet_alt.csv
--rw-r--r--   0 sep       (1000) sep       (1000)     1507 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/data/io/colormap/lava.csv
--rw-r--r--   0 sep       (1000) sep       (1000)     1128 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/data/io/colormap/lightbulb.csv
--rw-r--r--   0 sep       (1000) sep       (1000)     2195 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/data/io/imot_tools.mplstyle
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/data/math/
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/data/math/special/
--rw-r--r--   0 sep       (1000) sep       (1000)    20545 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/data/math/special/ive_threshold.csv
--rw-r--r--   0 sep       (1000) sep       (1000)      258 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/data/math/special/jv_series_threshold.csv
--rw-r--r--   0 sep       (1000) sep       (1000)    22191 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/data/math/special/jv_threshold.csv
--rw-r--r--   0 sep       (1000) sep       (1000)     9847 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/data/math/special/spherical_jn_series_threshold.csv
--rw-r--r--   0 sep       (1000) sep       (1000)    22176 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/data/math/special/spherical_jn_threshold.csv
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/io/
--rw-r--r--   0 sep       (1000) sep       (1000)      269 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/io/__init__.py
--rw-r--r--   0 sep       (1000) sep       (1000)     3566 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/io/plot.py
--rw-r--r--   0 sep       (1000) sep       (1000)    26828 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/io/s2image.py
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/math/
--rw-r--r--   0 sep       (1000) sep       (1000)      270 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/math/__init__.py
--rw-r--r--   0 sep       (1000) sep       (1000)    16201 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/math/func.py
--rw-r--r--   0 sep       (1000) sep       (1000)     8130 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/math/linalg.py
--rw-r--r--   0 sep       (1000) sep       (1000)     6096 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/math/special.py
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/math/sphere/
--rw-r--r--   0 sep       (1000) sep       (1000)      278 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/math/sphere/__init__.py
--rw-r--r--   0 sep       (1000) sep       (1000)    16503 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/math/sphere/grid.py
--rw-r--r--   0 sep       (1000) sep       (1000)     9051 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/math/sphere/interpolate.py
--rw-r--r--   0 sep       (1000) sep       (1000)     6774 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/math/sphere/transform.py
--rw-r--r--   0 sep       (1000) sep       (1000)     3871 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/math/stat.py
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/phased_array/
--rw-r--r--   0 sep       (1000) sep       (1000)     1987 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/phased_array/__init__.py
-drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/imot_tools/util/
--rw-r--r--   0 sep       (1000) sep       (1000)      291 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/util/__init__.py
--rw-r--r--   0 sep       (1000) sep       (1000)    20161 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/imot_tools/util/argcheck.py
--rw-r--r--   0 sep       (1000) sep       (1000)      932 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/imot_tools/util/array.py
--rw-r--r--   0 sep       (1000) sep       (1000)      360 2020-10-22 14:04:50.000000 ImoT_tools-1.1.0/requirements.txt
--rw-r--r--   0 sep       (1000) sep       (1000)      898 2020-10-22 15:21:55.000000 ImoT_tools-1.1.0/setup.cfg
--rw-r--r--   0 sep       (1000) sep       (1000)      353 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/setup.py
--rw-r--r--   0 sep       (1000) sep       (1000)     1788 2020-10-22 12:47:20.000000 ImoT_tools-1.1.0/test.py
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.280348 ImoT_tools-1.2.0/
+-rw-r--r--   0 sep       (1000) sep       (1000)       77 2023-05-15 14:10:11.000000 ImoT_tools-1.2.0/AUTHORS
+-rw-r--r--   0 sep       (1000) sep       (1000)      536 2023-05-15 14:10:11.000000 ImoT_tools-1.2.0/ChangeLog
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.273681 ImoT_tools-1.2.0/ImoT_tools.egg-info/
+-rw-r--r--   0 sep       (1000) sep       (1000)     1182 2023-05-15 14:10:11.000000 ImoT_tools-1.2.0/ImoT_tools.egg-info/PKG-INFO
+-rw-r--r--   0 sep       (1000) sep       (1000)     2347 2023-05-15 14:10:11.000000 ImoT_tools-1.2.0/ImoT_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 sep       (1000) sep       (1000)        1 2023-05-15 14:10:11.000000 ImoT_tools-1.2.0/ImoT_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 sep       (1000) sep       (1000)        1 2020-10-23 08:01:57.000000 ImoT_tools-1.2.0/ImoT_tools.egg-info/not-zip-safe
+-rw-r--r--   0 sep       (1000) sep       (1000)       47 2023-05-15 14:10:11.000000 ImoT_tools-1.2.0/ImoT_tools.egg-info/pbr.json
+-rw-r--r--   0 sep       (1000) sep       (1000)      100 2023-05-15 14:10:11.000000 ImoT_tools-1.2.0/ImoT_tools.egg-info/requires.txt
+-rw-r--r--   0 sep       (1000) sep       (1000)       11 2023-05-15 14:10:11.000000 ImoT_tools-1.2.0/ImoT_tools.egg-info/top_level.txt
+-rw-r--r--   0 sep       (1000) sep       (1000)     1536 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/LICENSE.txt
+-rw-r--r--   0 sep       (1000) sep       (1000)     1182 2023-05-15 14:10:11.280348 ImoT_tools-1.2.0/PKG-INFO
+-rw-r--r--   0 sep       (1000) sep       (1000)      419 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/README.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)       77 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/codestyle.toml
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.273681 ImoT_tools-1.2.0/doc/
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.273681 ImoT_tools-1.2.0/doc/api/
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.277014 ImoT_tools-1.2.0/doc/api/_img/
+-rw-r--r--   0 sep       (1000) sep       (1000)    18299 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/doc/api/_img/cmap_example.png
+-rw-r--r--   0 sep       (1000) sep       (1000)    21703 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/_img/colorbar_example.png
+-rw-r--r--   0 sep       (1000) sep       (1000)    67060 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/_img/sph_dirichlet_example.png
+-rw-r--r--   0 sep       (1000) sep       (1000)   145936 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/_img/sphericalimage_aeqd_example.png
+-rw-r--r--   0 sep       (1000) sep       (1000)   132430 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/_img/sphericalimage_gnom_example.png
+-rw-r--r--   0 sep       (1000) sep       (1000)   127199 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/_img/sphericalimage_lcc_example.png
+-rw-r--r--   0 sep       (1000) sep       (1000)      180 2020-10-26 20:02:53.000000 ImoT_tools-1.2.0/doc/api/imot_tools.io.fits.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      152 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/doc/api/imot_tools.io.plot.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      186 2020-10-26 20:02:53.000000 ImoT_tools-1.2.0/doc/api/imot_tools.io.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      281 2020-10-27 05:47:54.000000 ImoT_tools-1.2.0/doc/api/imot_tools.io.s2image.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      221 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.func.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      219 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.linalg.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      252 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      313 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.special.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      231 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.sphere.grid.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      263 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.sphere.interpolate.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      249 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.sphere.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      294 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.sphere.transform.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      207 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.math.stat.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      228 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.phased_array.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      548 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/doc/api/imot_tools.util.argcheck.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      189 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.util.array.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      175 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/imot_tools.util.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      384 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/api/index.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)     3428 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/conf.py
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.277014 ImoT_tools-1.2.0/doc/general/
+-rw-r--r--   0 sep       (1000) sep       (1000)      300 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/general/index.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)     1003 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/doc/general/install.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      586 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/index.rst
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.277014 ImoT_tools-1.2.0/doc/notes/
+-rw-r--r--   0 sep       (1000) sep       (1000)     3123 2020-10-28 12:46:02.000000 ImoT_tools-1.2.0/doc/notes/func_interpolation_OL_zonal.rst
+-rw-r--r--   0 sep       (1000) sep       (1000)      316 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/doc/notes/index.rst
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.277014 ImoT_tools-1.2.0/imot_tools/
+-rw-r--r--   0 sep       (1000) sep       (1000)      241 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/__init__.py
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.267014 ImoT_tools-1.2.0/imot_tools/data/
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.277014 ImoT_tools-1.2.0/imot_tools/data/io/
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.277014 ImoT_tools-1.2.0/imot_tools/data/io/colormap/
+-rw-r--r--   0 sep       (1000) sep       (1000)     1501 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/data/io/colormap/algue.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)     1382 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/data/io/colormap/aqua.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)     1202 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/data/io/colormap/fire.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)     1852 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/data/io/colormap/jet_alt.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)     1507 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/data/io/colormap/lava.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)     1128 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/data/io/colormap/lightbulb.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)     2195 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/data/io/imot_tools.mplstyle
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.267014 ImoT_tools-1.2.0/imot_tools/data/math/
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.277014 ImoT_tools-1.2.0/imot_tools/data/math/special/
+-rw-r--r--   0 sep       (1000) sep       (1000)    20545 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/data/math/special/ive_threshold.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)      258 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/data/math/special/jv_series_threshold.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)    22191 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/data/math/special/jv_threshold.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)     9847 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/data/math/special/spherical_jn_series_threshold.csv
+-rw-r--r--   0 sep       (1000) sep       (1000)    22176 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/data/math/special/spherical_jn_threshold.csv
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.277014 ImoT_tools-1.2.0/imot_tools/io/
+-rw-r--r--   0 sep       (1000) sep       (1000)      269 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/io/__init__.py
+-rw-r--r--   0 sep       (1000) sep       (1000)     2495 2020-10-26 19:49:04.000000 ImoT_tools-1.2.0/imot_tools/io/fits.py
+-rw-r--r--   0 sep       (1000) sep       (1000)     3566 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/io/plot.py
+-rw-r--r--   0 sep       (1000) sep       (1000)    30268 2021-02-23 13:12:25.000000 ImoT_tools-1.2.0/imot_tools/io/s2image.py
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.280348 ImoT_tools-1.2.0/imot_tools/math/
+-rw-r--r--   0 sep       (1000) sep       (1000)      270 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/math/__init__.py
+-rw-r--r--   0 sep       (1000) sep       (1000)    16201 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/math/func.py
+-rw-r--r--   0 sep       (1000) sep       (1000)     8130 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/math/linalg.py
+-rw-r--r--   0 sep       (1000) sep       (1000)     6096 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/math/special.py
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.280348 ImoT_tools-1.2.0/imot_tools/math/sphere/
+-rw-r--r--   0 sep       (1000) sep       (1000)      278 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/math/sphere/__init__.py
+-rw-r--r--   0 sep       (1000) sep       (1000)    16503 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/math/sphere/grid.py
+-rw-r--r--   0 sep       (1000) sep       (1000)    11502 2020-10-28 12:46:02.000000 ImoT_tools-1.2.0/imot_tools/math/sphere/interpolate.py
+-rw-r--r--   0 sep       (1000) sep       (1000)     6774 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/math/sphere/transform.py
+-rw-r--r--   0 sep       (1000) sep       (1000)     3871 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/math/stat.py
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.280348 ImoT_tools-1.2.0/imot_tools/phased_array/
+-rw-r--r--   0 sep       (1000) sep       (1000)     1987 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/phased_array/__init__.py
+drwxr-xr-x   0 sep       (1000) sep       (1000)        0 2023-05-15 14:10:11.280348 ImoT_tools-1.2.0/imot_tools/util/
+-rw-r--r--   0 sep       (1000) sep       (1000)      291 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/util/__init__.py
+-rw-r--r--   0 sep       (1000) sep       (1000)    20161 2020-10-22 14:04:50.000000 ImoT_tools-1.2.0/imot_tools/util/argcheck.py
+-rw-r--r--   0 sep       (1000) sep       (1000)      932 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/imot_tools/util/array.py
+-rw-r--r--   0 sep       (1000) sep       (1000)      368 2023-05-15 14:08:07.000000 ImoT_tools-1.2.0/requirements.txt
+-rw-r--r--   0 sep       (1000) sep       (1000)     1042 2023-05-15 14:10:11.280348 ImoT_tools-1.2.0/setup.cfg
+-rw-r--r--   0 sep       (1000) sep       (1000)      353 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/setup.py
+-rw-r--r--   0 sep       (1000) sep       (1000)     1788 2020-10-22 12:47:20.000000 ImoT_tools-1.2.0/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ImoT_tools-1.1.0/ImoT_tools.egg-info/PKG-INFO` & `ImoT_tools-1.2.0/ImoT_tools.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: ImoT-tools
-Version: 1.1.0
+Version: 1.2.0
 Summary: Collection of useful tools common to ImagingOfThings projects.
 Home-page: https://github.com/imagingofthings/ImoT_tools
+Download-URL: https://github.com/imagingofthings/ImoT_tools
 Author: Sepand KASHANI
 Author-email: kashani.sepand@gmail.com
 License: BSD
-Download-URL: https://github.com/imagingofthings/ImoT_tools
-Description: .. #############################################################################
-        .. README.rst
-        .. ==========
-        .. Author : Sepand KASHANI [kashani.sepand@gmail.com]
-        .. #############################################################################
-        
-        ##########
-        ImoT_tools
-        ##########
-        
-        *ImoT_tools* packages together useful tools common to ImagingOfThings projects.
-        
-        
-        Installation
-        ------------
-        See ``doc/general/install.rst``
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE.txt
+License-File: AUTHORS
+
+.. #############################################################################
+.. README.rst
+.. ==========
+.. Author : Sepand KASHANI [kashani.sepand@gmail.com]
+.. #############################################################################
+
+##########
+ImoT_tools
+##########
+
+*ImoT_tools* packages together useful tools common to ImagingOfThings projects.
+
+
+Installation
+------------
+See ``doc/general/install.rst``
```

### Comparing `ImoT_tools-1.1.0/ImoT_tools.egg-info/SOURCES.txt` & `ImoT_tools-1.2.0/ImoT_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ImoT_tools.egg-info/dependency_links.txt
 ImoT_tools.egg-info/not-zip-safe
 ImoT_tools.egg-info/pbr.json
 ImoT_tools.egg-info/requires.txt
 ImoT_tools.egg-info/top_level.txt
 doc/conf.py
 doc/index.rst
+doc/api/imot_tools.io.fits.rst
 doc/api/imot_tools.io.plot.rst
 doc/api/imot_tools.io.rst
 doc/api/imot_tools.io.s2image.rst
 doc/api/imot_tools.math.func.rst
 doc/api/imot_tools.math.linalg.rst
 doc/api/imot_tools.math.rst
 doc/api/imot_tools.math.special.rst
@@ -53,14 +54,15 @@
 imot_tools/data/io/colormap/lightbulb.csv
 imot_tools/data/math/special/ive_threshold.csv
 imot_tools/data/math/special/jv_series_threshold.csv
 imot_tools/data/math/special/jv_threshold.csv
 imot_tools/data/math/special/spherical_jn_series_threshold.csv
 imot_tools/data/math/special/spherical_jn_threshold.csv
 imot_tools/io/__init__.py
+imot_tools/io/fits.py
 imot_tools/io/plot.py
 imot_tools/io/s2image.py
 imot_tools/math/__init__.py
 imot_tools/math/func.py
 imot_tools/math/linalg.py
 imot_tools/math/special.py
 imot_tools/math/stat.py
```

### Comparing `ImoT_tools-1.1.0/LICENSE.txt` & `ImoT_tools-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/PKG-INFO` & `ImoT_tools-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: ImoT_tools
-Version: 1.1.0
+Version: 1.2.0
 Summary: Collection of useful tools common to ImagingOfThings projects.
 Home-page: https://github.com/imagingofthings/ImoT_tools
+Download-URL: https://github.com/imagingofthings/ImoT_tools
 Author: Sepand KASHANI
 Author-email: kashani.sepand@gmail.com
 License: BSD
-Download-URL: https://github.com/imagingofthings/ImoT_tools
-Description: .. #############################################################################
-        .. README.rst
-        .. ==========
-        .. Author : Sepand KASHANI [kashani.sepand@gmail.com]
-        .. #############################################################################
-        
-        ##########
-        ImoT_tools
-        ##########
-        
-        *ImoT_tools* packages together useful tools common to ImagingOfThings projects.
-        
-        
-        Installation
-        ------------
-        See ``doc/general/install.rst``
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE.txt
+License-File: AUTHORS
+
+.. #############################################################################
+.. README.rst
+.. ==========
+.. Author : Sepand KASHANI [kashani.sepand@gmail.com]
+.. #############################################################################
+
+##########
+ImoT_tools
+##########
+
+*ImoT_tools* packages together useful tools common to ImagingOfThings projects.
+
+
+Installation
+------------
+See ``doc/general/install.rst``
```

### Comparing `ImoT_tools-1.1.0/doc/api/_img/cmap_example.png` & `ImoT_tools-1.2.0/doc/api/_img/cmap_example.png`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/api/_img/colorbar_example.png` & `ImoT_tools-1.2.0/doc/api/_img/colorbar_example.png`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/api/_img/sph_dirichlet_example.png` & `ImoT_tools-1.2.0/doc/api/_img/sph_dirichlet_example.png`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/api/_img/sphericalimage_aeqd_example.png` & `ImoT_tools-1.2.0/doc/api/_img/sphericalimage_aeqd_example.png`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/api/_img/sphericalimage_gnom_example.png` & `ImoT_tools-1.2.0/doc/api/_img/sphericalimage_gnom_example.png`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/api/_img/sphericalimage_lcc_example.png` & `ImoT_tools-1.2.0/doc/api/_img/sphericalimage_lcc_example.png`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/api/imot_tools.util.argcheck.rst` & `ImoT_tools-1.2.0/doc/api/imot_tools.util.argcheck.rst`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/conf.py` & `ImoT_tools-1.2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/general/install.rst` & `ImoT_tools-1.2.0/doc/general/install.rst`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/index.rst` & `ImoT_tools-1.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/doc/notes/func_interpolation_OL_zonal.rst` & `ImoT_tools-1.2.0/doc/notes/func_interpolation_OL_zonal.rst`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,17 @@
 
    \beta_{q l} & = \frac{2 \pi}{(N + 1)^{2}} \sin\theta_{q} \sum_{a = 0}^{N} \frac{\sin[(2 a + 1) \theta_{q}]}{2 a + 1}.
 
 
 Implementation Notes
 ********************
 
-* :py:func:`~imot_tools.math.sphere.grid.ea_sample`,
-  :py:func:`~imot_tools.math.sphere.grid.fibonacci_sample` and
+* :py:func:`~imot_tools.math.sphere.grid.equal_angle`,
+  :py:func:`~imot_tools.math.sphere.grid.fibonacci`,
+  :py:func:`~imot_tools.math.sphere.grid.healpix` and
   :py:class:`~imot_tools.math.sphere.interpolate.Interpolator` can be used to sample order-limited
   zonal functions and evaluate them at arbitrary :math:`r \in \mathbb{S}^{2}`.
 
 * When :math:`N` is large, precise values of :math:`K_{N}(x)` can only be achieved using the
   recurrence relation on Legendre polynomials.  If minor errors can be tolerated, it is
   computationally advantageous to use function interpolation to approximate :math:`K_{N}(x)`.  Both
   exact and approximate values of :math:`K_{N}(x)` can be obtained using
```

### Comparing `ImoT_tools-1.1.0/imot_tools/data/io/colormap/algue.csv` & `ImoT_tools-1.2.0/imot_tools/data/io/colormap/algue.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/io/colormap/aqua.csv` & `ImoT_tools-1.2.0/imot_tools/data/io/colormap/aqua.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/io/colormap/fire.csv` & `ImoT_tools-1.2.0/imot_tools/data/io/colormap/fire.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/io/colormap/jet_alt.csv` & `ImoT_tools-1.2.0/imot_tools/data/io/colormap/jet_alt.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/io/colormap/lava.csv` & `ImoT_tools-1.2.0/imot_tools/data/io/colormap/lava.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/io/colormap/lightbulb.csv` & `ImoT_tools-1.2.0/imot_tools/data/io/colormap/lightbulb.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/io/imot_tools.mplstyle` & `ImoT_tools-1.2.0/imot_tools/data/io/imot_tools.mplstyle`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/math/special/ive_threshold.csv` & `ImoT_tools-1.2.0/imot_tools/data/math/special/ive_threshold.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/math/special/jv_threshold.csv` & `ImoT_tools-1.2.0/imot_tools/data/math/special/jv_threshold.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/math/special/spherical_jn_series_threshold.csv` & `ImoT_tools-1.2.0/imot_tools/data/math/special/spherical_jn_series_threshold.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/data/math/special/spherical_jn_threshold.csv` & `ImoT_tools-1.2.0/imot_tools/data/math/special/spherical_jn_threshold.csv`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/io/plot.py` & `ImoT_tools-1.2.0/imot_tools/io/plot.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/io/s2image.py` & `ImoT_tools-1.2.0/imot_tools/io/s2image.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 r"""
 Visualization and storage of images on :math:`\mathbb{S}^{2}`.
 """
 
 import astropy.coordinates as coord
 import astropy.io.fits as fits
 import astropy.units as u
+import astropy.wcs as wcs
 import matplotlib.axes as axes
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import matplotlib.tri as tri
 import numpy as np
 import pyproj
 import scipy.linalg as linalg
 
+import imot_tools.io.fits as ifits
 import imot_tools.io.plot as plot
 import imot_tools.math.sphere.transform as transform
 import imot_tools.util.argcheck as chk
 
 
 def from_fits(file_name):
     """
@@ -45,22 +47,21 @@
         image_hdu = hdulist["IMAGE"]
         klass = globals()[primary_hdu.header["IMG_TYPE"]]
 
         I = klass._from_fits(primary_hdu, image_hdu)
         return I
 
 
-# TODO: image re-interpolation for DS9-compatibility.
 class Image:
     r"""
     Container for storing real-valued images defined on :math:`\mathbb{S}^{2}`.
 
     Main features:
 
-    * import/export spherical maps to FITS format;
+    * import/export spherical maps to (non-standard) FITS format;
     * advanced 2D plotting based on `Matplotlib <https://matplotlib.org/>`_;
 
     Examples
     --------
     .. doctest::
 
        import numpy as np
@@ -124,15 +125,16 @@
 
        kwargs = dict(cmap='jet')
        I.draw(index=1, projection='LCC', data_kwargs=kwargs)
 
     .. image:: _img/sphericalimage_lcc_example.png
     """
 
-    @chk.check(dict(data=chk.has_reals, grid=chk.has_reals))
+    @chk.check(dict(data=chk.has_reals,
+                    grid=chk.has_reals))
     def __init__(self, data, grid):
         """
         Parameters
         ----------
         data : :py:class:`~numpy.ndarray`
             multi-level (float) data-cube.
 
@@ -221,16 +223,16 @@
           file.  The user-provided `grid` is assumed in ICRS.  If this is not the case, rotate the
           grid accordingly before calling :py:meth:`~imot_tools.io.s2image.Image.to_fits`.
 
         * Data cubes are stored in a secondary IMAGE frame and can be viewed with DS9 using::
 
               $ ds9 <FITS_file>.fits[IMAGE]
 
-          Only gridded maps are successfully visualized with DS9.  Moreover WCS information only
-          available in select subclasses.
+          Only FITS-compliant maps are successfully visualized with DS9.
+          Moreover WCS information only available in select subclasses.
         """
         primary_hdu = self._PrimaryHDU()
         image_hdu = self._ImageHDU()
 
         hdulist = fits.HDUList([primary_hdu, image_hdu])
         hdulist.writeto(file_name, overwrite=True)
 
@@ -262,15 +264,17 @@
         hdu : :py:class:`~astropy.io.fits.ImageHDU`
         """
         hdu = fits.ImageHDU(data=self._data, name="IMAGE")
         return hdu
 
     @classmethod
     @chk.check(
-        dict(primary_hdu=chk.is_instance(fits.PrimaryHDU), image_hdu=chk.is_instance(fits.ImageHDU))
+        dict(primary_hdu=chk.is_instance(fits.PrimaryHDU),
+             image_hdu=chk.is_instance(fits.ImageHDU),
+        )
     )
     def _from_fits(cls, primary_hdu, image_hdu):
         """
         Load image from Header Descriptor Units.
 
         Parameters
         ----------
@@ -716,15 +720,16 @@
                 catalog_kwargs = dict()
 
             plot_style = dict(s=400, facecolors="none", edgecolors="w")
             plot_style.update(catalog_kwargs)
 
             ax.scatter(c_x, c_y, **plot_style)
 
-    @chk.check(dict(projection=chk.is_instance(pyproj.Proj), ax=chk.is_instance(axes.Axes)))
+    @chk.check(dict(projection=chk.is_instance(pyproj.Proj),
+                    ax=chk.is_instance(axes.Axes)))
     def _draw_beautify(self, projection, ax):
         """
         Format plot.
 
         Parameters
         ----------
         projection : :py:class:`pyproj.Proj`
@@ -775,7 +780,121 @@
         y : :py:class:`~numpy.ndarray`
         """
         lat_d, lon_d = cls._wrapped_rad2deg(lat_r, lon_r)
         x, y = projection(lon_d, lat_d, errcheck=False)
         x[np.isclose(x, 1e30)] = np.nan
         y[np.isclose(y, 1e30)] = np.nan
         return x, y
+
+
+class WCSImage(Image):
+    """
+    Spherical image container for WCS-described maps.
+
+    Main features:
+
+    * import/export to FITS-compliant format;
+    * View images using DS9/AstroPy. (see :py:meth:`~imot_tools.io.s2image.Image.to_fits`)
+    """
+    @chk.check('WCS', chk.is_instance(wcs.WCS))
+    def __init__(self, data, WCS):
+        """
+        Parameters
+        ----------
+        data : :py:class:`~numpy.ndarray`
+            multi-level (float) data-cube.
+
+            Possible shapes are:
+
+            * (N_height, N_width);
+            * (N_image, N_height, N_width);
+
+        WCS : :py:class:`~astropy.wcs.WCS`
+            (N_width, N_height) World Coordinate System with spatial axes.
+
+        Notes
+        -----
+        Caution: the FITS standard uses FORTRAN conventions for index/array
+        ordering. `WCS` dimensions/information (FORTRAN-ordered) must therefore
+        be reversed compared to `data` (assumed C-ordered).
+        """
+        if WCS.naxis != 2:
+            raise ValueError('Parameter[WCS] is ambiguous.')
+
+        N_width, N_height = WCS.array_shape
+        if data.shape[-2:] != (N_height, N_width):
+            raise ValueError('Parameters[grid, data] are inconsistent.')
+
+        grid = ifits.pix_grid(WCS)  # (3, N_height, N_width)
+        super().__init__(data, grid)
+
+        self._WCS = WCS.sub([1, 2, 0])  # 0 = insert new axis.
+        self._WCS.wcs.cname[2] = 'LAYER'
+        self._WCS.wcs.ctype[2] = ''
+
+    @property
+    def WCS(self):
+        """
+        Returns
+        -------
+        WCS : :py:class:`~astropy.wcs.WCS`
+            World Coordinate System (WCS), augmented with extra axes for
+            multi-layer images.
+        """
+        return self._WCS
+
+    def _PrimaryHDU(self):
+        """
+        Generate primary Header Descriptor Unit (HDU) for FITS export.
+
+        Returns
+        -------
+        hdu : :py:class:`~astropy.io.fits.PrimaryHDU`
+        """
+        metadata = dict(IMG_TYPE=(self.__class__.__name__, "Image subclass"))
+
+        hdu = fits.PrimaryHDU()
+        for k, v in metadata.items():
+            hdu.header[k] = v
+        return hdu
+
+    def _ImageHDU(self):
+        """
+        Generate image Header Descriptor Unit (HDU) for FITS export.
+
+        Returns
+        -------
+        hdu : :py:class:`~astropy.io.fits.ImageHDU`
+        """
+        hdu = fits.ImageHDU(data=self._data,
+                            header=self._WCS.to_header(),
+                            name="IMAGE")
+        return hdu
+
+    @classmethod
+    @chk.check(
+        dict(primary_hdu=chk.is_instance(fits.PrimaryHDU),
+             image_hdu=chk.is_instance(fits.ImageHDU),
+        )
+    )
+    def _from_fits(cls, primary_hdu, image_hdu):
+        """
+        Load image from Header Descriptor Units.
+
+        Parameters
+        ----------
+        primary_hdu : :py:class:`~astropy.io.fits.PrimaryHDU`
+        image_hdu : :py:class:`~astropy.io.fits.ImageHDU`
+
+        Returns
+        -------
+        I : :py:class:`~imot_tools.io.s2image.Image`
+        """
+        # PrimaryHDU: nothing for WCSImage.
+
+        # ImageHDU: extract data cube.
+        data = image_hdu.data
+        WCS = wcs.WCS(image_hdu).celestial  # Must drop LAYER-dimension to
+                                            # avoid ambiguity in constructor.
+
+        I = cls(data=data, WCS=WCS)
+        return I
```

### Comparing `ImoT_tools-1.1.0/imot_tools/math/func.py` & `ImoT_tools-1.2.0/imot_tools/math/func.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/math/linalg.py` & `ImoT_tools-1.2.0/imot_tools/math/linalg.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/math/special.py` & `ImoT_tools-1.2.0/imot_tools/math/special.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/math/sphere/grid.py` & `ImoT_tools-1.2.0/imot_tools/math/sphere/grid.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/math/sphere/interpolate.py` & `ImoT_tools-1.2.0/imot_tools/math/sphere/interpolate.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 """
 Interpolation algorithms.
 """
 
 import numpy as np
 import scipy.sparse as sp
+import tqdm
 
 import imot_tools.math.func as func
 import imot_tools.math.sphere.grid as grid
 import imot_tools.math.sphere.transform as transform
 import imot_tools.util.argcheck as chk
 
 
@@ -45,18 +46,16 @@
     @chk.check(
         dict(
             weight=chk.has_reals,
             support=chk.has_reals,
             f=chk.accept_any(chk.has_reals, chk.has_complex),
             r=chk.has_reals,
             sparsity_mask=chk.allow_None(
-                chk.require_all(
-                    chk.is_instance(sp.spmatrix), lambda _: np.issubdtype(_.dtype, np.bool_)
-                )
-            ),
+                chk.require_all(chk.is_instance(sp.spmatrix),
+                                lambda _: np.issubdtype(_.dtype, np.bool_))),
         )
     )
     def __call__(self, weight, support, f, r, sparsity_mask=None):
         """
         Interpolate function samples at order `N`.
 
         Parameters
@@ -97,16 +96,24 @@
                 raise ValueError("Parameter[sparsity_mask] must have shape (N_s, N_px).")
 
         if sparsity_mask is None:  # Dense evaluation
             kernel = self._kernel_func(support.T @ r)
             beta = f * weight
             f_interp = beta @ kernel
         else:  # Sparse evaluation
-            raise NotImplementedError
+            # Evaluate kernel
+            row = sparsity_mask.row
+            col = sparsity_mask.col
+            dist = np.sum(support[:, row] * r[:, col], axis=0)
+            ker = self._kernel_func(np.clip(dist, 0, 1))
+            kernel = sp.coo_matrix((ker, (row, col)), shape=sparsity_mask.shape)
 
+            kernel_T = kernel.T.tocsr()
+            beta = f * weight
+            f_interp = (kernel_T @ beta.T).T
         return f_interp
 
 
 class EqualAngleInterpolator(Interpolator):
     r"""
     Interpolate order-limited zonal function from Equal-Angle samples.
 
@@ -176,37 +183,42 @@
         N : int
             Order of the reconstructed zonal function.
         approximate_kernel : bool
             If :py:obj:`True`, pass the `approx` option to :py:class:`~imot_tools.math.func.SphericalDirichlet`.
         """
         super().__init__(N, approximate_kernel)
 
-    # TODO: Allow sparse evaluation.
     @chk.check(
         dict(
             colat_idx=chk.has_integers,
             lon_idx=chk.has_integers,
             f=chk.accept_any(chk.has_reals, chk.has_complex),
             r=chk.has_reals,
+            sparsity_mask=chk.allow_None(
+                chk.require_all(chk.is_instance(sp.spmatrix),
+                                lambda _: np.issubdtype(_.dtype, np.bool_))),
         )
     )
-    def __call__(self, colat_idx, lon_idx, f, r):
+    def __call__(self, colat_idx, lon_idx, f, r, sparsity_mask=None):
         """
         Interpolate function samples at order `N`.
 
         Parameters
         ----------
         colat_idx : :py:class:`~numpy.ndarray`
             (N_colat,) polar support indices from :py:func:`~imot_tools.math.sphere.grid.equal_angle`.
         lon_idx : :py:class:`~numpy.ndarray`
             (N_lon,) azimuthal support indices from :py:func:`~imot_tools.math.sphere.grid.equal_angle`.
         f : :py:class:`~numpy.ndarray`
             (L, N_colat, N_lon) zonal function values at support points. (float or complex)
         r : :py:class:`~numpy.ndarray`
             (3, N_px) evaluation points.
+        sparsity_mask : :py:class:`~scipy.sparse.spmatrix`
+            (N_s, N_px) sparsity mask (bool) to perform localized kernel evaluation.
+            The 0-th dimension has size N_s = N_colat * N_lon.
 
         Returns
         -------
         f_interp : :py:class:`~numpy.ndarray`
             (L, N_px) function values at specified coordinates.
         """
         N_colat = colat_idx.size
@@ -235,10 +247,65 @@
         fw = f * weight.reshape((1, N_colat, 1))  # (L, N_colat, N_lon)
 
         f_interp = super().__call__(
             weight=np.broadcast_to([1], (N_colat * N_lon,)),
             support=transform.pol2cart(1, colat[colat_idx, :], lon[:, lon_idx]).reshape((3, -1)),
             f=fw.reshape((L, -1)),
             r=r,
-            sparsity_mask=None,
+            sparsity_mask=sparsity_mask,
         )
         return f_interp
+
+
+@chk.check(dict(N=chk.is_integer,
+                R1=chk.require_all(chk.has_ndim(2), chk.has_reals),
+                R2=chk.require_all(chk.has_ndim(2), chk.has_reals)))
+def sparsity_mask(N, R1, R2):
+    r"""
+    Generate sparsity mask for fast kernel evaluation in
+    :py:class:`~imot_tools.math.sphere.Interpolator` instances.
+
+    Parameters
+    ----------
+    N : int
+        Interpolation order.
+    R1 : :py:class:`~numpy.ndarray`
+        (3, N_1) Cartesian coordinates.
+    R2 : :py:class:`~numpy.ndarray`
+        (3, N_2) Cartesian coordinates.
+
+    Returns
+    -------
+    S : :py:class:`~scipy.sparse.coo_matrix` (bool)
+        (N_1, N_2) boolean mask where kernel must be evaluated.
+
+    Notes
+    -----
+    Dense equivalent:
+
+        S = (R1.T @ R2) >= threshold(N)
+    """
+    N_1 = R1.shape[1]
+    if R1.shape != (3, N_1):
+        raise ValueError('Parameter[R1] must be a (3, N_1) array.')
+    N_2 = R2.shape[1]
+    if R2.shape != (3, N_2):
+        raise ValueError('Parameter[R2] must be a (3, N_2) array.')
+
+    if N_1 < N_2:
+        S = sparsity_mask(N, R2, R1).T
+        return S
+    else:
+        # Compute cut-off threshold
+        f = func.SphericalDirichlet(N, approx=True)
+        x = np.linspace(-1, 1, 10**6)
+        threshold = x[np.cumsum( (f(x) / f(1)) ** 2 ).nonzero()].min()
+
+        S = sp.dok_matrix((N_1, N_2), dtype=bool)
+        L = np.zeros((N_2,), dtype=float)  # Temporary buffer
+        idx = np.zeros((N_2,), dtype=bool)  # Temporary buffer
+        for i in tqdm.tqdm(np.arange(N_1)):
+            np.dot(R1[:, i], R2, out=L)
+            np.greater_equal(L, threshold, out=idx)
+            S[i, idx] = True
+        S = sp.coo_matrix(S)
+        return S
```

### Comparing `ImoT_tools-1.1.0/imot_tools/math/sphere/transform.py` & `ImoT_tools-1.2.0/imot_tools/math/sphere/transform.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/math/stat.py` & `ImoT_tools-1.2.0/imot_tools/math/stat.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/phased_array/__init__.py` & `ImoT_tools-1.2.0/imot_tools/phased_array/__init__.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/util/argcheck.py` & `ImoT_tools-1.2.0/imot_tools/util/argcheck.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/imot_tools/util/array.py` & `ImoT_tools-1.2.0/imot_tools/util/array.py`

 * *Files identical despite different names*

### Comparing `ImoT_tools-1.1.0/test.py` & `ImoT_tools-1.2.0/test.py`

 * *Files identical despite different names*

