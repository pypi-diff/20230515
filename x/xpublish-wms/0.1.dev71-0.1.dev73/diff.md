# Comparing `tmp/xpublish_wms-0.1.dev71.tar.gz` & `tmp/xpublish_wms-0.1.dev73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpublish_wms-0.1.dev71.tar", last modified: Mon May 15 15:29:26 2023, max compression
+gzip compressed data, was "xpublish_wms-0.1.dev73.tar", last modified: Mon May 15 17:11:08 2023, max compression
```

## Comparing `xpublish_wms-0.1.dev71.tar` & `xpublish_wms-0.1.dev73.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 15:29:26.232672 xpublish_wms-0.1.dev71/
--rw-r--r--   0 akerney    (502) staff       (20)       34 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev71/.gitattributes
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 15:29:26.223089 xpublish_wms-0.1.dev71/.github/
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 15:29:26.228290 xpublish_wms-0.1.dev71/.github/workflows/
--rw-r--r--   0 akerney    (502) staff       (20)      956 2023-05-15 13:28:23.000000 xpublish_wms-0.1.dev71/.github/workflows/tests.yml
--rw-r--r--   0 akerney    (502) staff       (20)     1432 2023-05-15 13:37:44.000000 xpublish_wms-0.1.dev71/.pre-commit-config.yaml
--rw-r--r--   0 akerney    (502) staff       (20)     1472 2023-05-15 12:15:12.000000 xpublish_wms-0.1.dev71/LICENSE.txt
--rw-r--r--   0 akerney    (502) staff       (20)      220 2023-05-15 12:15:12.000000 xpublish_wms-0.1.dev71/MANIFEST.in
--rw-r--r--   0 akerney    (502) staff       (20)     3838 2023-05-15 15:29:26.232979 xpublish_wms-0.1.dev71/PKG-INFO
--rw-r--r--   0 akerney    (502) staff       (20)     1296 2023-05-15 13:25:06.000000 xpublish_wms-0.1.dev71/README.md
--rw-r--r--   0 akerney    (502) staff       (20)     1757 2023-05-15 15:29:14.000000 xpublish_wms-0.1.dev71/pyproject.toml
--rw-r--r--   0 akerney    (502) staff       (20)      256 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev71/requirements-dev.txt
--rw-r--r--   0 akerney    (502) staff       (20)       85 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev71/requirements.txt
--rw-r--r--   0 akerney    (502) staff       (20)      201 2023-05-15 15:29:26.233716 xpublish_wms-0.1.dev71/setup.cfg
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 15:29:26.231952 xpublish_wms-0.1.dev71/xpublish_wms/
--rw-r--r--   0 akerney    (502) staff       (20)      235 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev71/xpublish_wms/__init__.py
--rw-r--r--   0 akerney    (502) staff       (20)      170 2023-05-15 15:29:26.000000 xpublish_wms-0.1.dev71/xpublish_wms/_version.py
--rw-r--r--   0 akerney    (502) staff       (20)    16205 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev71/xpublish_wms/cf_wms.py
--rw-r--r--   0 akerney    (502) staff       (20)    11193 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev71/xpublish_wms/getmap.py
--rw-r--r--   0 akerney    (502) staff       (20)      987 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev71/xpublish_wms/plugin.py
--rw-r--r--   0 akerney    (502) staff       (20)     1726 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev71/xpublish_wms/utils.py
-drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 15:29:26.232330 xpublish_wms-0.1.dev71/xpublish_wms.egg-info/
--rw-r--r--   0 akerney    (502) staff       (20)      304 2023-05-15 15:29:26.000000 xpublish_wms-0.1.dev71/xpublish_wms.egg-info/SOURCES.txt
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.650133 xpublish_wms-0.1.dev73/
+-rw-r--r--   0 akerney    (502) staff       (20)       34 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev73/.gitattributes
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.639731 xpublish_wms-0.1.dev73/.github/
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.645990 xpublish_wms-0.1.dev73/.github/workflows/
+-rw-r--r--   0 akerney    (502) staff       (20)     1766 2023-05-15 15:28:34.000000 xpublish_wms-0.1.dev73/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 akerney    (502) staff       (20)      956 2023-05-15 13:28:23.000000 xpublish_wms-0.1.dev73/.github/workflows/tests.yml
+-rw-r--r--   0 akerney    (502) staff       (20)     1432 2023-05-15 13:37:44.000000 xpublish_wms-0.1.dev73/.pre-commit-config.yaml
+-rw-r--r--   0 akerney    (502) staff       (20)     1472 2023-05-15 12:15:12.000000 xpublish_wms-0.1.dev73/LICENSE.txt
+-rw-r--r--   0 akerney    (502) staff       (20)      220 2023-05-15 12:15:12.000000 xpublish_wms-0.1.dev73/MANIFEST.in
+-rw-r--r--   0 akerney    (502) staff       (20)     3995 2023-05-15 17:11:08.650659 xpublish_wms-0.1.dev73/PKG-INFO
+-rw-r--r--   0 akerney    (502) staff       (20)     1451 2023-05-15 15:33:21.000000 xpublish_wms-0.1.dev73/README.md
+-rw-r--r--   0 akerney    (502) staff       (20)     1759 2023-05-15 17:10:52.000000 xpublish_wms-0.1.dev73/pyproject.toml
+-rw-r--r--   0 akerney    (502) staff       (20)      256 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev73/requirements-dev.txt
+-rw-r--r--   0 akerney    (502) staff       (20)       85 2023-05-15 13:25:07.000000 xpublish_wms-0.1.dev73/requirements.txt
+-rw-r--r--   0 akerney    (502) staff       (20)      201 2023-05-15 17:11:08.651527 xpublish_wms-0.1.dev73/setup.cfg
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.649518 xpublish_wms-0.1.dev73/xpublish_wms/
+-rw-r--r--   0 akerney    (502) staff       (20)      235 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/__init__.py
+-rw-r--r--   0 akerney    (502) staff       (20)      170 2023-05-15 17:11:08.000000 xpublish_wms-0.1.dev73/xpublish_wms/_version.py
+-rw-r--r--   0 akerney    (502) staff       (20)    16205 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/cf_wms.py
+-rw-r--r--   0 akerney    (502) staff       (20)    11193 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/getmap.py
+-rw-r--r--   0 akerney    (502) staff       (20)      987 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/plugin.py
+-rw-r--r--   0 akerney    (502) staff       (20)     1726 2023-05-15 13:34:24.000000 xpublish_wms-0.1.dev73/xpublish_wms/utils.py
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-15 17:11:08.649896 xpublish_wms-0.1.dev73/xpublish_wms.egg-info/
+-rw-r--r--   0 akerney    (502) staff       (20)      342 2023-05-15 17:11:08.000000 xpublish_wms-0.1.dev73/xpublish_wms.egg-info/SOURCES.txt
```

### Comparing `xpublish_wms-0.1.dev71/.github/workflows/tests.yml` & `xpublish_wms-0.1.dev73/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.1.dev71/.pre-commit-config.yaml` & `xpublish_wms-0.1.dev73/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.1.dev71/LICENSE.txt` & `xpublish_wms-0.1.dev73/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.1.dev71/pyproject.toml` & `xpublish_wms-0.1.dev73/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xpublish_wms"
 authors = [{ name = "Matthew Iannucci", email = "matt.iannucci@rpsgroup.com" }]
 description = "WMS plugin for xpublish"
 readme = "README.md"
-requires-python = ">=3.89"
+requires-python = ">=3.9"
 keywords = ["xarray", "xpublish", "wms"]
 license = { file = "LICENSE.txt" }
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
 dynamic = ["version", "dependencies"]
 
 [project.urls]
-"Homepage" = "https://github.com/asascience-open/xpublish-wms"
+"Homepage" = "https://github.com/xpublish-community/xpublish-wms"
 
 [project.entry-points."xpublish.plugin"]
 cf_wms = "xpublish_wms.plugin:CfWmsPlugin"
 
 [tool.setuptools]
 packages = ["xpublish_wms"]
```

### Comparing `xpublish_wms-0.1.dev71/xpublish_wms/cf_wms.py` & `xpublish_wms-0.1.dev73/xpublish_wms/cf_wms.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.1.dev71/xpublish_wms/getmap.py` & `xpublish_wms-0.1.dev73/xpublish_wms/getmap.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.1.dev71/xpublish_wms/plugin.py` & `xpublish_wms-0.1.dev73/xpublish_wms/plugin.py`

 * *Files identical despite different names*

### Comparing `xpublish_wms-0.1.dev71/xpublish_wms/utils.py` & `xpublish_wms-0.1.dev73/xpublish_wms/utils.py`

 * *Files identical despite different names*

