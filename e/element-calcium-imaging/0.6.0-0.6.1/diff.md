# Comparing `tmp/element-calcium-imaging-0.6.0.tar.gz` & `tmp/element-calcium-imaging-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-calcium-imaging-0.6.0.tar", last modified: Sun May 14 01:01:57 2023, max compression
+gzip compressed data, was "element-calcium-imaging-0.6.1.tar", last modified: Mon May 15 16:51:37 2023, max compression
```

## Comparing `element-calcium-imaging-0.6.0.tar` & `element-calcium-imaging-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:57.619209 element-calcium-imaging-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-14 01:01:57.619209 element-calcium-imaging-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:57.615209 element-calcium-imaging-0.6.0/element_calcium_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66658 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    74194 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:57.615209 element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/cell_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    26752 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:57.615209 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:01:57.619209 element-calcium-imaging-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:51:37.617578 element-calcium-imaging-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-15 16:51:37.617578 element-calcium-imaging-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:51:37.617578 element-calcium-imaging-0.6.1/element_calcium_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66658 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/imaging_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74194 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/imaging_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/imaging_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:51:37.617578 element-calcium-imaging-0.6.1/element_calcium_imaging/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/plotting/cell_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26752 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/element_calcium_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:51:37.617578 element-calcium-imaging-0.6.1/element_calcium_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-15 16:51:37.000000 element-calcium-imaging-0.6.1/element_calcium_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-15 16:51:37.000000 element-calcium-imaging-0.6.1/element_calcium_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:51:37.000000 element-calcium-imaging-0.6.1/element_calcium_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 16:51:37.000000 element-calcium-imaging-0.6.1/element_calcium_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 16:51:37.000000 element-calcium-imaging-0.6.1/element_calcium_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:51:37.617578 element-calcium-imaging-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-15 16:51:34.000000 element-calcium-imaging-0.6.1/setup.py
```

### Comparing `element-calcium-imaging-0.6.0/LICENSE` & `element-calcium-imaging-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/PKG-INFO` & `element-calcium-imaging-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.6.0
+Version: 0.6.1
 Summary: Calcium Imaging DataJoint element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
@@ -30,14 +30,16 @@
 
 ![flowchart](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/flowchart.svg)
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
++ We have designed three variations of the pipeline to handle different use cases. Displayed above is the default `imaging` schema.  Details on all of the `imaging` schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) documentation page.
+
 ## Getting Started
 
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
      ```
```

### Comparing `element-calcium-imaging-0.6.0/README.md` & `element-calcium-imaging-0.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 ![flowchart](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/flowchart.svg)
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
++ We have designed three variations of the pipeline to handle different use cases. Displayed above is the default `imaging` schema.  Details on all of the `imaging` schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) documentation page.
+
 ## Getting Started
 
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
      ```
```

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging/imaging.py` & `element-calcium-imaging-0.6.1/element_calcium_imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_no_curation.py` & `element-calcium-imaging-0.6.1/element_calcium_imaging/imaging_no_curation.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_preprocess.py` & `element-calcium-imaging-0.6.1/element_calcium_imaging/imaging_preprocess.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_report.py` & `element-calcium-imaging-0.6.1/element_calcium_imaging/imaging_report.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/cell_plot.py` & `element-calcium-imaging-0.6.1/element_calcium_imaging/plotting/cell_plot.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/widget.py` & `element-calcium-imaging-0.6.1/element_calcium_imaging/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging/scan.py` & `element-calcium-imaging-0.6.1/element_calcium_imaging/scan.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/PKG-INFO` & `element-calcium-imaging-0.6.1/element_calcium_imaging.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.6.0
+Version: 0.6.1
 Summary: Calcium Imaging DataJoint element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
@@ -30,14 +30,16 @@
 
 ![flowchart](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/flowchart.svg)
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
++ We have designed three variations of the pipeline to handle different use cases. Displayed above is the default `imaging` schema.  Details on all of the `imaging` schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) documentation page.
+
 ## Getting Started
 
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
      ```
```

### Comparing `element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/SOURCES.txt` & `element-calcium-imaging-0.6.1/element_calcium_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.0/setup.py` & `element-calcium-imaging-0.6.1/setup.py`

 * *Files identical despite different names*

