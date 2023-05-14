# Comparing `tmp/discminer-0.2.5.tar.gz` & `tmp/discminer-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.2.5.tar", last modified: Sun May  7 20:54:46 2023, max compression
+gzip compressed data, was "discminer-0.2.6.tar", last modified: Sun May 14 22:17:43 2023, max compression
```

## Comparing `discminer-0.2.5.tar` & `discminer-0.2.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.481751 discminer-0.2.5/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.5/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-07 20:54:46.481951 discminer-0.2.5/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.5/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.456936 discminer-0.2.5/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.5/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.5/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.5/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.5/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.5/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.5/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.5/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.5/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.5/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.5/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.5/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.5/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.468196 discminer-0.2.5/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.5/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-07 20:52:36.000000 discminer-0.2.5/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     2069 2023-05-05 17:33:30.000000 discminer-0.2.5/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.5/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.5/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.5/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.5/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.5/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.475297 discminer-0.2.5/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.5/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.5/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.5/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    31514 2023-05-07 20:50:53.000000 discminer-0.2.5/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    36007 2023-05-03 15:09:48.000000 discminer-0.2.5/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.5/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.477642 discminer-0.2.5/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.5/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.5/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.5/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.5/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.469912 discminer-0.2.5/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.5/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-07 20:54:46.482391 discminer-0.2.5/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.5/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.481042 discminer-0.2.5/template/
--rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.5/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.5/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.5/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.5/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.585278 discminer-0.2.6/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.6/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-14 22:17:43.585572 discminer-0.2.6/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.6/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.555658 discminer-0.2.6/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.6/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.6/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.6/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.6/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.6/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.6/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.6/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.6/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.6/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.6/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.6/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.6/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.569760 discminer-0.2.6/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.6/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-14 22:16:27.000000 discminer-0.2.6/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     2069 2023-05-05 17:33:30.000000 discminer-0.2.6/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.6/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.6/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.6/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.6/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.6/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.578610 discminer-0.2.6/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.6/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.6/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12955 2023-05-14 20:31:53.000000 discminer-0.2.6/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    35724 2023-05-14 22:07:59.000000 discminer-0.2.6/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    36007 2023-05-03 15:09:48.000000 discminer-0.2.6/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.6/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.580599 discminer-0.2.6/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.6/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.6/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.6/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.6/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.571711 discminer-0.2.6/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.6/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-14 22:17:43.586340 discminer-0.2.6/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.6/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.584349 discminer-0.2.6/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.6/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.6/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.6/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.6/template/prepare_data.py
```

### Comparing `discminer-0.2.5/LICENSE` & `discminer-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/PKG-INFO` & `discminer-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.5 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.6 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.5/README.md` & `discminer-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/make_channels.py` & `discminer-0.2.6/_mining/make_channels.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/make_parfile.py` & `discminer-0.2.6/_mining/make_parfile.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/make_single_moments.py` & `discminer-0.2.6/_mining/make_single_moments.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/plot_attributes_model.py` & `discminer-0.2.6/_mining/plot_attributes_model.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/plot_azimuthal_profiles.py` & `discminer-0.2.6/_mining/plot_azimuthal_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/plot_moment+offset.py` & `discminer-0.2.6/_mining/plot_moment+offset.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/plot_moment+residuals.py` & `discminer-0.2.6/_mining/plot_moment+residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/plot_peak_residuals.py` & `discminer-0.2.6/_mining/plot_peak_residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/plot_radial_profiles.py` & `discminer-0.2.6/_mining/plot_radial_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/plot_residuals+all.py` & `discminer-0.2.6/_mining/plot_residuals+all.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/plot_residuals+deproj.py` & `discminer-0.2.6/_mining/plot_residuals+deproj.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/_mining/utils.py` & `discminer-0.2.6/_mining/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/cart.py` & `discminer-0.2.6/discminer/cart.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/core.py` & `discminer-0.2.6/discminer/core.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/cube.py` & `discminer-0.2.6/discminer/cube.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/disc2d.py` & `discminer-0.2.6/discminer/disc2d.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/grid.py` & `discminer-0.2.6/discminer/grid.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/icons/button_box.png` & `discminer-0.2.6/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/icons/button_cursor.jpeg` & `discminer-0.2.6/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/icons/button_path.png` & `discminer-0.2.6/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/icons/button_return.png` & `discminer-0.2.6/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/icons/button_surface.png` & `discminer-0.2.6/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/icons/button_trash.jpg` & `discminer-0.2.6/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/pick.py` & `discminer-0.2.6/discminer/pick.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,22 +213,22 @@
         print ("accepted variance peaks on PHI:", acc_peaks_phi)
 
         var_colors_phi = np.array(['1.0']*n_phi).astype('<U9')
         var_colors_phi[acc_peaks_phi] = 'palegreen' #kde_color
         ind_variance_peak_phi = np.argmax(variance_phi_y)
         variance_nomax = np.sort(variance_phi_y)[:-len(acc_peaks_phi)]
         peak_variance_std_phi = var_std_phi #std of variances except those from accepted peaks np.std(variance_nomax)
-        peak_variance_angle = kcenters_phi[:,0][ind_variance_peak_phi]
+        self.peak_variance_phi = kcenters_phi[:,0][ind_variance_peak_phi]
 
         kc_indsort_phi = np.argsort(kcenters_phi[:,0])
         kcent_sort_phi = kcenters_phi[:,0][kc_indsort_phi]
         kcent_sort_vel_phi = kcenters_phi[:,1][kc_indsort_phi]
         var_y_sort_phi = variance_phi_y[kc_indsort_phi]*var_scale
-        var_nopeaks_phi = np.delete(var_y_sort_phi, acc_peaks_phi)
-        peak_variance_mean_phi = np.mean(var_nopeaks_phi)/var_scale #mean of variances excluding those from accepted peaks
+        self.var_nopeaks_phi = np.delete(var_y_sort_phi, acc_peaks_phi)
+        peak_variance_mean_phi = np.mean(self.var_nopeaks_phi)/var_scale #mean of variances excluding those from accepted peaks
 
         #peak_variance_sigmas = (self.variance_y[ind_variance_peak]-peak_variance_mean)/peak_variance_std #Considering only peak accepted variance
         self.peak_variance_sigmas_phi = (np.mean(var_y_sort_phi[acc_peaks_phi])/var_scale-peak_variance_mean_phi)/peak_variance_std_phi #Considering mean std of all accepted peaks
 
         #***************************
         #FIND PEAK RADIAL CLUSTER VARIANCES
         #***************************
@@ -236,22 +236,22 @@
         print ("accepted variance peaks on R:", acc_peaks_R)
 
         var_colors_R = np.array(['1.0']*n_R).astype('<U9')
         var_colors_R[acc_peaks_R] = 'palegreen' #kde_color
         ind_variance_peak_R = np.argmax(variance_R_y)
         variance_nomax = np.sort(variance_R_y)[:-len(acc_peaks_R)]
         peak_variance_std_R = var_std_R #std of variances except those from accepted peaks np.std(variance_nomax)
-        peak_variance_angle = kcenters_R[:,0][ind_variance_peak_R]
+        self.peak_variance_R = kcenters_R[:,0][ind_variance_peak_R]
 
         kc_indsort_R = np.argsort(kcenters_R[:,0])
         kcent_sort_R = kcenters_R[:,0][kc_indsort_R]
         kcent_sort_vel_R = kcenters_R[:,1][kc_indsort_R]
         var_y_sort_R = variance_R_y[kc_indsort_R]*var_scale
-        var_nopeaks_R = np.delete(var_y_sort_R, acc_peaks_R)
-        peak_variance_mean_R = np.mean(var_nopeaks_R)/var_scale #mean of variances excluding those from accepted peaks
+        self.var_nopeaks_R = np.delete(var_y_sort_R, acc_peaks_R)
+        peak_variance_mean_R = np.mean(self.var_nopeaks_R)/var_scale #mean of variances excluding those from accepted peaks
 
         #peak_variance_sigmas = (self.variance_y[ind_variance_peak]-peak_variance_mean)/peak_variance_std #Considering only peak accepted variance
         self.peak_variance_sigmas_R = (np.mean(var_y_sort_R[acc_peaks_R])/var_scale-peak_variance_mean_R)/peak_variance_std_R #Considering mean std of all accepted peaks
 
         #**************************
         self.kcent_sort_phi = kcent_sort_phi
         self.var_y_sort_phi = var_y_sort_phi
```

### Comparing `discminer-0.2.5/discminer/plottools.py` & `discminer-0.2.6/discminer/plottools.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 ===========
 """
 import os
 import copy
 import matplotlib
 import numpy as np
 from math import ceil
+import scipy.stats as st
 import astropy.units as u
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
+from matplotlib.colors import ListedColormap
 from collections.abc import Iterable
 
 from .tools.utils import weighted_std, InputError
 from .tools.fit_kernel import _gauss
 from .grid import GridTools
 
 SMALL_SIZE = 10
@@ -477,20 +479,23 @@
 
 #*********************
 #MAKE DEPROJECTED MAPS
 #*********************
 def make_round_map(
         map2d, levels, X, Y, Rout,
         z_func=None, z_pars=None, incl=None, PA=None, xc=0, yc=0, #Optional, make N-sky axis
-        fig=None, ax=None,
+        fig=None, ax=None, make_cbar=True,
         rwidth=0.06, cmap=get_discminer_cmap('velocity'), clabel='km/s', fmt='%5.2f', quadrant=None, #cbar kwargs
         gaps=[], rings=[], kinks=[],
-        mask_wedge=None, mask_inner=None
+        mask_wedge=None, mask_inner=None, kwargs_mask={}
 ):
 
+    kw_mask = dict(facecolor='0.5', edgecolor='k', lw=1.0, alpha=0.6)
+    kw_mask.update(kwargs_mask)
+    
     #SOME DEFINITIONS
     if fig is None:
         fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
 
     X = np.nan_to_num(X.to('au').value)
     Y = np.nan_to_num(Y.to('au').value)
     Rout = Rout.to('au').value
@@ -532,27 +537,27 @@
     if quadrant is None: #Guess best quadrant based on Nsky position
         if xni is None:
             quadrant = 2
         elif (yni>0 and xni<0) or (yni<0 and xni>0):
             quadrant = 3
         else:
             quadrant = 2
-            
-    make_round_cbar(ax, Rout, levels, cmap=cmap_c, clabel=clabel, fmt=fmt, quadrant=quadrant)
+
+    if make_cbar:
+        make_round_cbar(ax, Rout, levels, cmap=cmap_c, clabel=clabel, fmt=fmt, quadrant=quadrant)
 
     sq = {1: -1,
           2: 1,
           3: 1,
           4: -1,
     }[quadrant]
         
     ax.plot([sq*Rout, sq*Rout], [0, -xlim_rec], color='0.0', lw=1.0, dash_capstyle='round', dashes=(1.5, 2.5)) #Rout projected onto Cartesian xaxis
 
     #MASK
-    kw_mask = dict(facecolor='0.5', edgecolor='k', lw=1.0, alpha=0.6)
     if mask_wedge is not None:
 
         for wedge in mask_wedge:
 
             if np.isscalar(wedge.value): #single wedge
                 w = patches.Wedge((0,0), Rout, *mask_wedge.to('deg').value, **kw_mask)
                 ax.add_artist(w)
@@ -649,15 +654,15 @@
 
     #DECORATIONS
     ax.axvline(-90, ls=':', lw=2.5, color='0.3', dash_capstyle='round')
     ax.axvline(90, ls=':', lw=2.5, color='0.3', dash_capstyle='round')
     ax.axvline(0, ls=':', lw=2.5, color='0.3', dash_capstyle='round')
 
     make_up_ax(ax, labelbottom=True, labeltop=False, labelsize=SMALL_SIZE+1,
-               xlims=(-180.1, 180.1), ylims=(1.1*Rin, 0.95*Rout))
+               xlims=(-180.1, 180.1), ylims=(1.02*Rin, 0.98*Rout))
     ax.set_xticks(np.linspace(-180, 180, 13))
     ax.set_xlabel('Azimuth [deg]', fontsize=MEDIUM_SIZE)
     ax.set_ylabel('Radius [au]', fontsize=MEDIUM_SIZE)
     mod_major_ticks(ax, axis='y', nbins=10)
                        
     cax = add_cbar_ax(fig, ax, **kwargs_cb)
     cbar = plt.colorbar(im, cax=cax, format=fmt, orientation='vertical', ticks=np.linspace(levels.min(), levels.max(), 5))
@@ -817,7 +822,106 @@
         if values_stdi < ax1_ylims[-1] and i>0:
             ax[-1].text(gauss_values_stdi+0.2*max_y, values_stdi, r'%d$\sigma$'%i, 
                         fontsize=14, ha='center', va='center', rotation=-90)
 
     for axi in ax:
         axi.set_ylim(*ax1_ylims)
 
+    return ax[-1]
+
+
+def make_clusters_1d(pick, which='phi', fig=None, ax=None, color='#FFB000', percentiles=[5, 67], var_scale=1e3):
+
+    if fig is None:
+        fig, ax = plt.subplots(ncols=2, nrows=1, figsize=(12,5))
+
+    kde_cmap = get_cmap_from_color(color, lev=len(percentiles))        
+    variance_x, variance_y = [], []
+
+    if which=='phi':
+        peak_both = np.array([pick.peak_angle, pick.peak_resid]).T        
+        klabels = pick.klabels_phi
+        xmax = 90*1.05
+        xmin = -xmax
+        kcent_x = pick.kcent_sort_phi
+        kcent_y = pick.kcent_sort_vel_phi
+        kcent_var = pick.var_y_sort_phi        
+        peak_variance = pick.peak_variance_phi
+        var_nopeaks = pick.var_nopeaks_phi        
+        color_var = pick.var_colors_phi
+        for axi in ax:
+            axi.set_xlim(-95,95)
+            axi.set_xticks(np.arange(-90,90+1,30))
+        ax[0].set_xlabel(r'Azimuth [deg]')    
+        ax[1].set_xlabel(r'Azimuth [deg]')
+            
+    elif which=='r':
+        peak_both = np.array([pick.lev_list, pick.peak_resid]).T                
+        klabels = pick.klabels_R
+        xmax = np.nanmax(pick.lev_list)
+        xmin = np.nanmin(pick.lev_list)        
+        kcent_x = pick.kcent_sort_R
+        kcent_y = pick.kcent_sort_vel_R
+        kcent_var = pick.var_y_sort_R
+        peak_variance = pick.peak_variance_R
+        var_nopeaks = pick.var_nopeaks_R
+        color_var = pick.var_colors_R
+        ax[0].set_xlabel(r'Radius [au]')    
+        ax[1].set_xlabel(r'Radius [au]')
+
+    n_clusters = len(kcent_x)
+
+    ymin, ymax = -0.1*pick.peak_global_val, 1.2*pick.peak_global_val 
+    xx, yy = np.mgrid[xmin:xmax:200j, ymin:ymax:200j]
+
+    #MAKE GAUSSIAN KDE per CLUSTER
+    for i in range(n_clusters):
+        x = peak_both[:,0][klabels == i]
+        y = peak_both[:,1][klabels == i]
+        positions = np.vstack([xx.ravel(), yy.ravel()])
+        values = np.vstack([x, y]) #shape (2, ndata)    
+        try: 
+            kernel = st.gaussian_kde(values)#, weights=pick.peak_weight[klabels==i])
+            perr = np.sqrt(np.diag(kernel.covariance))
+            variance_x.append((kernel.covariance[0,0]**0.5/kernel.factor)**2) #True variance: std**2
+            variance_y.append(kernel.covariance[1,1])
+        except ValueError: #when too few points in cluster
+            variance_x.append(0)
+            variance_y.append(0)
+            continue
+
+        f = np.reshape(kernel(positions).T, xx.shape)
+        levels = [st.scoreatpercentile(kernel(kernel.resample(1000)), per) for per in percentiles]
+        levels.append(np.amax(f))
+        try: 
+            ax[0].contourf(xx, yy, f, levels, cmap=kde_cmap)
+            ax[0].contour(xx, yy, f, levels, colors='k', linewidths=[0.5, 1.0, 1.5], alpha=0.6)
+        except ValueError:
+            continue 
+
+    #PLOT CLUSTER CENTRES
+    for j in range(n_clusters):   
+        ax[0].scatter(kcent_x[j], kcent_y[j], facecolors='1.0', edgecolors='k', linewidths=1.5, marker='X', s=200, zorder=10)
+        ax[1].scatter(kcent_x[j], kcent_var[j], facecolors=color_var[j], alpha=1,  
+                      edgecolors='k', linewidths=1.5, marker='X', s=200, zorder=10)
+
+    ax[1].plot(kcent_x, kcent_var, lw=2., ls='-', color='k', zorder=9)
+    ax_std = append_sigma_panel(fig, ax[1], var_nopeaks, hist=True)
+
+    #DECORATIONS
+    for axi in ax: 
+        axi.tick_params(labelbottom=True, top=True, right=True, which='both', direction='in')
+        mod_major_ticks(axi, nbins=8)
+        mod_minor_ticks(axi)
+
+    ax[0].set_ylim(ymin, 1.05*ymax)
+    ax[1].axvline(peak_variance, lw=3, c=color, label='variance peak')
+    ax[1].legend(frameon=False, fontsize=MEDIUM_SIZE-2, handlelength=1.0) #, loc='lower left', bbox_to_anchor=(-0.04, 0.98))    
+    ax[1].tick_params(labelleft=False, labelright=True)
+
+    ax[0].set_title('K-means clusters')
+    ax[0].set_ylabel('Peak residual [km/s]')
+    ax[1].set_title('Velocity variance from KDE cov.')
+    ax_std.set_ylabel(r'Variance [$\times 10^{-%d}$ km$^2$/s$^2$]'%int(np.log10(var_scale)))
+    
+    return fig, ax
+
```

### Comparing `discminer-0.2.5/discminer/rail.py` & `discminer-0.2.6/discminer/rail.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/testyapf.py` & `discminer-0.2.6/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/tools/discminer.mplstyle` & `discminer-0.2.6/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/tools/fit_kernel.py` & `discminer-0.2.6/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer/tools/utils.py` & `discminer-0.2.6/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/discminer.egg-info/PKG-INFO` & `discminer-0.2.6/discminer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.5 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.6 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.5/discminer.egg-info/SOURCES.txt` & `discminer-0.2.6/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/setup.py` & `discminer-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/template/README.rst` & `discminer-0.2.6/template/README.rst`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/template/download_MAPS.sh` & `discminer-0.2.6/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.2.6/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.5/template/prepare_data.py` & `discminer-0.2.6/template/prepare_data.py`

 * *Files identical despite different names*

