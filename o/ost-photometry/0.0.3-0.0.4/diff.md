# Comparing `tmp/ost_photometry-0.0.3.tar.gz` & `tmp/ost_photometry-0.0.4.tar.gz`

## Comparing `ost_photometry-0.0.3.tar` & `ost_photometry-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/__init__.py
--rwxr-xr-x   0        0        0    21964 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/aux.py
--rwxr-xr-x   0        0        0     6453 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/calibration_data.py
--rwxr-xr-x   0        0        0     5281 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/checks.py
--rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/style.py
--rwxr-xr-x   0        0        0     1761 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/terminal_output.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/analyze/__init__.py
--rwxr-xr-x   0        0        0   166982 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/analyze/analyze.py
--rwxr-xr-x   0        0        0    82799 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/analyze/aux.py
--rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/analyze/calib.py
--rwxr-xr-x   0        0        0    32008 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/analyze/correlate.py
--rwxr-xr-x   0        0        0    65772 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/analyze/plot.py
--rwxr-xr-x   0        0        0    60779 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/analyze/trans.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/reduce/__init__.py
--rwxr-xr-x   0        0        0    67568 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/reduce/aux.py
--rwxr-xr-x   0        0        0    10487 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/reduce/plot.py
--rwxr-xr-x   0        0        0    75654 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/src/ost_photometry/reduce/redu.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/README.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 ost_photometry-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/__init__.py
+-rwxr-xr-x   0        0        0    21964 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/aux.py
+-rwxr-xr-x   0        0        0     6453 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/calibration_data.py
+-rwxr-xr-x   0        0        0     5281 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/checks.py
+-rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/style.py
+-rwxr-xr-x   0        0        0     1761 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/terminal_output.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/analyze/__init__.py
+-rwxr-xr-x   0        0        0   166982 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/analyze/analyze.py
+-rwxr-xr-x   0        0        0    82799 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/analyze/aux.py
+-rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/analyze/calib.py
+-rwxr-xr-x   0        0        0    32008 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/analyze/correlate.py
+-rwxr-xr-x   0        0        0    65772 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/analyze/plot.py
+-rwxr-xr-x   0        0        0    60779 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/analyze/trans.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/reduce/__init__.py
+-rwxr-xr-x   0        0        0    67568 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/reduce/aux.py
+-rwxr-xr-x   0        0        0    10487 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/reduce/plot.py
+-rwxr-xr-x   0        0        0    75654 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/src/ost_photometry/reduce/redu.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/LICENSE
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/README.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 ost_photometry-0.0.4/PKG-INFO
```

### Comparing `ost_photometry-0.0.3/src/ost_photometry/aux.py` & `ost_photometry-0.0.4/src/ost_photometry/aux.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/calibration_data.py` & `ost_photometry-0.0.4/src/ost_photometry/calibration_data.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/checks.py` & `ost_photometry-0.0.4/src/ost_photometry/checks.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/terminal_output.py` & `ost_photometry-0.0.4/src/ost_photometry/terminal_output.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/analyze/analyze.py` & `ost_photometry-0.0.4/src/ost_photometry/analyze/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,15 +583,15 @@
 
         sigma_psf       : `float`
             Sigma of the objects PSF, assuming it is a Gaussian
 
         multi_start     : `float`, optional
             Multiplier for the background RMS, used to calculate the
             threshold to identify stars
-            Default is ``7``.
+            Default is ``5``.
 
         method         : `string`, optional
             Finder method DAO or IRAF
             Default is ``IRAF``.
 
         verbose         : `boolean`, optional
             If True addtional information will be printed to the terminal.
```

### Comparing `ost_photometry-0.0.3/src/ost_photometry/analyze/aux.py` & `ost_photometry-0.0.4/src/ost_photometry/analyze/aux.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/analyze/calib.py` & `ost_photometry-0.0.4/src/ost_photometry/analyze/calib.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/analyze/correlate.py` & `ost_photometry-0.0.4/src/ost_photometry/analyze/correlate.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/analyze/plot.py` & `ost_photometry-0.0.4/src/ost_photometry/analyze/plot.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/analyze/trans.py` & `ost_photometry-0.0.4/src/ost_photometry/analyze/trans.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/reduce/aux.py` & `ost_photometry-0.0.4/src/ost_photometry/reduce/aux.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/reduce/plot.py` & `ost_photometry-0.0.4/src/ost_photometry/reduce/plot.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/src/ost_photometry/reduce/redu.py` & `ost_photometry-0.0.4/src/ost_photometry/reduce/redu.py`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/LICENSE` & `ost_photometry-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ost_photometry-0.0.3/pyproject.toml` & `ost_photometry-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ost_photometry"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Rainer Hainich", email="rhainich@astro.physik.uni-potsdam.de" },
 ]
 description = "Phtometry reduction and analysis package for the OST observatory"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "Path>=16.0",
```

### Comparing `ost_photometry-0.0.3/PKG-INFO` & `ost_photometry-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ost_photometry
-Version: 0.0.3
+Version: 0.0.4
 Summary: Phtometry reduction and analysis package for the OST observatory
 Project-URL: Homepage, https://github.com/OST-Observatory/ost_photometry_package
 Project-URL: Bug Tracker, https://github.com/OST-Observatory/ost_photometry_package/issues
 Author-email: Rainer Hainich <rhainich@astro.physik.uni-potsdam.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Requires-Dist: astroalign>=2.4
 Requires-Dist: astropy>=5.0
 Requires-Dist: astroquery>=0.4
 Requires-Dist: ccdproc>=2.3
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: numpy>=1.18
 Requires-Dist: path>=16.0
```

