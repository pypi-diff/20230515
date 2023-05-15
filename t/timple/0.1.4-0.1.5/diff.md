# Comparing `tmp/timple-0.1.4.tar.gz` & `tmp/timple-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timple-0.1.4.tar", last modified: Mon Aug 16 21:21:00 2021, max compression
+gzip compressed data, was "timple-0.1.5.tar", last modified: Thu Nov 18 17:41:37 2021, max compression
```

## Comparing `timple-0.1.4.tar` & `timple-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 21:21:00.343760 timple-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-08-16 21:20:50.000000 timple-0.1.4/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2021-08-16 21:21:00.343760 timple-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2021-08-16 21:20:50.000000 timple-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-08-16 21:21:00.343760 timple-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-16 21:20:50.000000 timple-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 21:21:00.339760 timple-0.1.4/timple/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-08-16 21:20:50.000000 timple-0.1.4/timple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7083 2021-08-16 21:20:50.000000 timple-0.1.4/timple/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     4500 2021-08-16 21:20:50.000000 timple-0.1.4/timple/patches.py
--rw-r--r--   0 runner    (1001) docker     (121)    42368 2021-08-16 21:20:50.000000 timple-0.1.4/timple/timedelta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 21:21:00.343760 timple-0.1.4/timple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2021-08-16 21:21:00.000000 timple-0.1.4/timple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-08-16 21:21:00.000000 timple-0.1.4/timple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-16 21:21:00.000000 timple-0.1.4/timple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-16 21:21:00.000000 timple-0.1.4/timple.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-16 21:21:00.000000 timple-0.1.4/timple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-08-16 21:21:00.000000 timple-0.1.4/timple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 17:41:37.659070 timple-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-11-18 17:41:25.000000 timple-0.1.5/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2501 2021-11-18 17:41:37.659070 timple-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1685 2021-11-18 17:41:25.000000 timple-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2021-11-18 17:41:37.659070 timple-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 17:41:25.000000 timple-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 17:41:37.659070 timple-0.1.5/timple/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-11-18 17:41:25.000000 timple-0.1.5/timple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7083 2021-11-18 17:41:25.000000 timple-0.1.5/timple/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4500 2021-11-18 17:41:25.000000 timple-0.1.5/timple/patches.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42372 2021-11-18 17:41:25.000000 timple-0.1.5/timple/timedelta.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 17:41:37.659070 timple-0.1.5/timple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2501 2021-11-18 17:41:37.000000 timple-0.1.5/timple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-11-18 17:41:37.000000 timple-0.1.5/timple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 17:41:37.000000 timple-0.1.5/timple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 17:41:37.000000 timple-0.1.5/timple.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-18 17:41:37.000000 timple-0.1.5/timple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-18 17:41:37.000000 timple-0.1.5/timple.egg-info/top_level.txt
```

### Comparing `timple-0.1.4/LICENSE.rst` & `timple-0.1.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `timple-0.1.4/PKG-INFO` & `timple-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timple
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extended functionality for plotting timedelta-like values with Matplotlib
 Home-page: https://github.com/theOehrly/Timple
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: # Timple
```

### Comparing `timple-0.1.4/README.md` & `timple-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `timple-0.1.4/setup.cfg` & `timple-0.1.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = timple
-version = 0.1.4
+version = 0.1.5
 license = MIT
 license_files = LICENSE.rst
 author = Oehrly
 author_email = oehrly@mailbox.org
 home-page = https://github.com/theOehrly/Timple
 description = Extended functionality for plotting timedelta-like values with Matplotlib
 long-description = file: README.md
@@ -17,16 +17,16 @@
 install_requires = 
 	numpy
 	matplotlib
 
 [build_sphinx]
 project = Timple
 copyright = 2021, theOehrly
-version = 0.1.5-alpha
-release = 0.1.5-alpha
+version = 0.1.5
+release = 0.1.5
 source-dir = ./docs
 build-dir = ./docs/_build
 
 [flake8]
 max-line-length = 79
 
 [egg_info]
```

### Comparing `timple-0.1.4/timple/core.py` & `timple-0.1.5/timple/core.py`

 * *Files identical despite different names*

### Comparing `timple-0.1.4/timple/patches.py` & `timple-0.1.5/timple/patches.py`

 * *Files identical despite different names*

### Comparing `timple-0.1.4/timple/timedelta.py` & `timple-0.1.5/timple/timedelta.py`

 * *Files 1% similar despite different names*

```diff
@@ -865,16 +865,16 @@
         """
         factor = self.base_factors[base]
 
         locator = ticker.MultipleLocator(base=interval/factor)
         locator.set_axis(self.axis)
 
         if self.axis is not None:
-            locator.set_view_interval(*self.axis.get_view_interval())
-            locator.set_data_interval(*self.axis.get_data_interval())
+            self.axis.set_view_interval(*self.axis.get_view_interval())
+            self.axis.set_data_interval(*self.axis.get_data_interval())
 
         return locator
 
     def _get_unit(self):
         """
         Return how many days a unit of the locator is; used for
         intelligent autoscaling.
```

### Comparing `timple-0.1.4/timple.egg-info/PKG-INFO` & `timple-0.1.5/timple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timple
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extended functionality for plotting timedelta-like values with Matplotlib
 Home-page: https://github.com/theOehrly/Timple
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: # Timple
```

