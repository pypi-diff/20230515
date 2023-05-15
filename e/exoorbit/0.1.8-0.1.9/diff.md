# Comparing `tmp/exoorbit-0.1.8.tar.gz` & `tmp/exoorbit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoorbit-0.1.8.tar", last modified: Tue Dec 14 14:20:45 2021, max compression
+gzip compressed data, was "exoorbit-0.1.9.tar", last modified: Tue Dec 14 14:22:35 2021, max compression
```

## Comparing `exoorbit-0.1.8.tar` & `exoorbit-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 14:20:45.876772 exoorbit-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-12-14 14:20:13.000000 exoorbit-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-12-14 14:20:45.876772 exoorbit-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-12-14 14:20:13.000000 exoorbit-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 14:20:45.880772 exoorbit-0.1.8/exoorbit/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-12-14 14:20:13.000000 exoorbit-0.1.8/exoorbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-12-14 14:20:45.880772 exoorbit-0.1.8/exoorbit/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6966 2021-12-14 14:20:13.000000 exoorbit-0.1.8/exoorbit/bodies.py
--rw-r--r--   0 runner    (1001) docker     (121)    20642 2021-12-14 14:20:13.000000 exoorbit-0.1.8/exoorbit/dataclasses_quantity.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2021-12-14 14:20:13.000000 exoorbit-0.1.8/exoorbit/library.py
--rw-r--r--   0 runner    (1001) docker     (121)    14218 2021-12-14 14:20:13.000000 exoorbit-0.1.8/exoorbit/orbit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3247 2021-12-14 14:20:13.000000 exoorbit-0.1.8/exoorbit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 14:20:45.876772 exoorbit-0.1.8/exoorbit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-12-14 14:20:45.000000 exoorbit-0.1.8/exoorbit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      350 2021-12-14 14:20:45.000000 exoorbit-0.1.8/exoorbit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 14:20:45.000000 exoorbit-0.1.8/exoorbit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-14 14:20:45.000000 exoorbit-0.1.8/exoorbit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-12-14 14:20:45.880772 exoorbit-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      508 2021-12-14 14:20:13.000000 exoorbit-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 14:20:45.876772 exoorbit-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2021-12-14 14:20:13.000000 exoorbit-0.1.8/test/test_orbit.py
--rw-r--r--   0 runner    (1001) docker     (121)    70144 2021-12-14 14:20:13.000000 exoorbit-0.1.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 14:22:35.270913 exoorbit-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2021-12-14 14:21:57.000000 exoorbit-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-12-14 14:22:35.270913 exoorbit-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2021-12-14 14:21:57.000000 exoorbit-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 14:22:35.270913 exoorbit-0.1.9/exoorbit/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-12-14 14:21:57.000000 exoorbit-0.1.9/exoorbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-12-14 14:22:35.270913 exoorbit-0.1.9/exoorbit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6974 2021-12-14 14:21:57.000000 exoorbit-0.1.9/exoorbit/bodies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20642 2021-12-14 14:21:57.000000 exoorbit-0.1.9/exoorbit/dataclasses_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2021-12-14 14:21:57.000000 exoorbit-0.1.9/exoorbit/library.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14218 2021-12-14 14:21:57.000000 exoorbit-0.1.9/exoorbit/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3247 2021-12-14 14:21:57.000000 exoorbit-0.1.9/exoorbit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 14:22:35.270913 exoorbit-0.1.9/exoorbit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-12-14 14:22:35.000000 exoorbit-0.1.9/exoorbit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2021-12-14 14:22:35.000000 exoorbit-0.1.9/exoorbit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 14:22:35.000000 exoorbit-0.1.9/exoorbit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-14 14:22:35.000000 exoorbit-0.1.9/exoorbit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2021-12-14 14:22:35.270913 exoorbit-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2021-12-14 14:21:57.000000 exoorbit-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 14:22:35.270913 exoorbit-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     4366 2021-12-14 14:21:57.000000 exoorbit-0.1.9/test/test_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    70144 2021-12-14 14:21:57.000000 exoorbit-0.1.9/versioneer.py
```

### Comparing `exoorbit-0.1.8/PKG-INFO` & `exoorbit-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exoorbit
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/AWehrhahn/ExoOrbits
 Author: Ansgar Wehrhahn
 Author-email: ansgar.wehrhahn@physics.uu.se
 License: UNKNOWN
 Description: ![Python application](https://github.com/AWehrhahn/ExoOrbits/workflows/Python%20application/badge.svg)
```

### Comparing `exoorbit-0.1.8/exoorbit/bodies.py` & `exoorbit-0.1.9/exoorbit/bodies.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     @u.quantity_input
     def circumference(self) -> Quantity[u.km]:
         """Quantity(km): circumference of the disk"""
         return 2 * pi * self.radius
 
     @property
     @u.quantity_input
-    def gravity_value(self) -> Quantity[u.m**3/u.s**2]:
+    def gravity_value(self) -> Quantity[u.m ** 3 / u.s ** 2]:
         """Quantity(): specific gravity parameter for this object"""
         return G * self.mass
 
     @property
     @u.quantity_input
     def volume(self) -> Quantity[u.km ** 3]:
         """Quantity(km**3): volume of this object"""
@@ -177,15 +177,15 @@
             effective temperature of the star
 
         Returns
         -------
         equi_temp: u.K
             equilibrium temperature of the planet
         """
-        teff = ((pi * self.radius ** 2) / self.a ** 2) ** 0.25 * stellar_teff
+        teff = ((pi * self.radius ** 2) / self.sma ** 2) ** 0.25 * stellar_teff
         return teff
 
     @u.quantity_input
     def atm_scale_height(self, surface_temp: u.K) -> u.km:
         """
         Calculate the scale height of the atmosphere, based on the surface
         temperature of the planet. The surface temperature can for example
```

### Comparing `exoorbit-0.1.8/exoorbit/dataclasses_quantity.py` & `exoorbit-0.1.9/exoorbit/dataclasses_quantity.py`

 * *Files identical despite different names*

### Comparing `exoorbit-0.1.8/exoorbit/library.py` & `exoorbit-0.1.9/exoorbit/library.py`

 * *Files identical despite different names*

### Comparing `exoorbit-0.1.8/exoorbit/orbit.py` & `exoorbit-0.1.9/exoorbit/orbit.py`

 * *Files identical despite different names*

### Comparing `exoorbit-0.1.8/exoorbit/util.py` & `exoorbit-0.1.9/exoorbit/util.py`

 * *Files identical despite different names*

### Comparing `exoorbit-0.1.8/exoorbit.egg-info/PKG-INFO` & `exoorbit-0.1.9/exoorbit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exoorbit
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/AWehrhahn/ExoOrbits
 Author: Ansgar Wehrhahn
 Author-email: ansgar.wehrhahn@physics.uu.se
 License: UNKNOWN
 Description: ![Python application](https://github.com/AWehrhahn/ExoOrbits/workflows/Python%20application/badge.svg)
```

### Comparing `exoorbit-0.1.8/test/test_orbit.py` & `exoorbit-0.1.9/test/test_orbit.py`

 * *Files identical despite different names*

### Comparing `exoorbit-0.1.8/versioneer.py` & `exoorbit-0.1.9/versioneer.py`

 * *Files identical despite different names*

