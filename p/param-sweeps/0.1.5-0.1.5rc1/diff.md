# Comparing `tmp/param_sweeps-0.1.5.tar.gz` & `tmp/param-sweeps-0.1.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "param_sweeps-0.1.5.tar", max compression
+gzip compressed data, was "param-sweeps-0.1.5rc1.tar", max compression
```

## Comparing `param_sweeps-0.1.5.tar` & `param-sweeps-0.1.5rc1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1093 2022-10-12 15:56:34.681986 param_sweeps-0.1.5/LICENSE
--rw-r--r--   0        0        0      262 2023-05-15 16:42:31.376587 param_sweeps-0.1.5/param_sweeps/__init__.py
--rw-r--r--   0        0        0      492 2023-01-27 16:59:23.340009 param_sweeps-0.1.5/param_sweeps/constants.py
--rw-r--r--   0        0        0     7981 2023-05-15 16:42:31.378141 param_sweeps-0.1.5/param_sweeps/driver.py
--rw-r--r--   0        0        0     3255 2023-05-15 16:42:31.379951 param_sweeps-0.1.5/param_sweeps/generate.py
--rw-r--r--   0        0        0      967 2023-05-15 16:42:31.380061 param_sweeps-0.1.5/param_sweeps/sample_driver.py
--rw-r--r--   0        0        0     1705 2023-05-15 16:42:31.385010 param_sweeps-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1153 2022-11-10 19:09:10.043391 param_sweeps-0.1.5/README.md
--rw-r--r--   0        0        0     2311 1970-01-01 00:00:00.000000 param_sweeps-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1093 2022-10-12 15:56:34.681986 param-sweeps-0.1.5rc1/LICENSE
+-rw-r--r--   0        0        0      267 2023-03-27 18:46:26.351129 param-sweeps-0.1.5rc1/param_sweeps/__init__.py
+-rw-r--r--   0        0        0      492 2023-01-27 16:59:23.340009 param-sweeps-0.1.5rc1/param_sweeps/constants.py
+-rw-r--r--   0        0        0     7981 2023-03-27 18:46:26.352129 param-sweeps-0.1.5rc1/param_sweeps/driver.py
+-rw-r--r--   0        0        0     3255 2023-03-27 18:46:26.352750 param-sweeps-0.1.5rc1/param_sweeps/generate.py
+-rw-r--r--   0        0        0      967 2023-03-27 18:46:26.352750 param-sweeps-0.1.5rc1/param_sweeps/sample_driver.py
+-rw-r--r--   0        0        0     1710 2023-03-27 18:46:26.354142 param-sweeps-0.1.5rc1/pyproject.toml
+-rw-r--r--   0        0        0     1153 2022-11-10 19:09:10.043391 param-sweeps-0.1.5rc1/README.md
+-rw-r--r--   0        0        0     1852 2023-03-27 18:47:08.834733 param-sweeps-0.1.5rc1/setup.py
+-rw-r--r--   0        0        0     2314 2023-03-27 18:47:08.834733 param-sweeps-0.1.5rc1/PKG-INFO
```

### Comparing `param_sweeps-0.1.5/LICENSE` & `param-sweeps-0.1.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.5/param_sweeps/driver.py` & `param-sweeps-0.1.5rc1/param_sweeps/driver.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.5/param_sweeps/generate.py` & `param-sweeps-0.1.5rc1/param_sweeps/generate.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.5/param_sweeps/sample_driver.py` & `param-sweeps-0.1.5rc1/param_sweeps/sample_driver.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.5/pyproject.toml` & `param-sweeps-0.1.5rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "param-sweeps"
-version = "0.1.5"
+version = "0.1.5-rc.1"
 description = "Parameter sweeper for ui.json powered applications"
 authors = ["Mira Geoscience <benjamink@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/param-sweeps"
 homepage = "https://mirageoscience.com"
 readme = "README.md"
 keywords = ["geology", "geophysics", "earth sciences"]
 classifiers = [
```

### Comparing `param_sweeps-0.1.5/README.md` & `param-sweeps-0.1.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.5/PKG-INFO` & `param-sweeps-0.1.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: param-sweeps
-Version: 0.1.5
+Version: 0.1.5rc1
 Summary: Parameter sweeper for ui.json powered applications
 Home-page: https://mirageoscience.com
 Keywords: geology,geophysics,earth sciences
 Author: Mira Geoscience
 Author-email: benjamink@mirageoscience.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -12,17 +12,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: geoh5py (>=0.6.0)
 Requires-Dist: numpy (>=1.21.5,<2.0.0)
 Project-URL: Repository, https://github.com/MiraGeoscience/param-sweeps
 Description-Content-Type: text/markdown
```

