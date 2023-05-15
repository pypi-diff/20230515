# Comparing `tmp/pymodaq_femto-0.2.1.tar.gz` & `tmp/pymodaq_femto-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_femto-0.2.1.tar", last modified: Tue May  2 10:39:10 2023, max compression
+gzip compressed data, was "pymodaq_femto-0.2.2.tar", last modified: Mon May 15 15:07:48 2023, max compression
```

## Comparing `pymodaq_femto-0.2.1.tar` & `pymodaq_femto-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-02 10:39:10.980780 pymodaq_femto-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.972779 pymodaq_femto-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/pnps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/resources/load_settings.png
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/resources/save_settings.png
--rw-r--r--   0 runner    (1001) docker     (123)    95147 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto/utils/raw_scans/
--rw-r--r--   0 runner    (1001) docker     (123)  1554195 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/utils/raw_scans/example_measured_dscan_to_convert.h5
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-02 10:38:57.000000 pymodaq_femto-0.2.1/src/pymodaq_femto/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:39:10.976779 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 10:39:10.000000 pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:07:48.938170 pymodaq_femto-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-15 15:07:48.938170 pymodaq_femto-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-15 15:07:48.942170 pymodaq_femto-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:07:48.930170 pymodaq_femto-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:07:48.934170 pymodaq_femto-0.2.2/src/pymodaq_femto/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/pnps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:07:48.938170 pymodaq_femto-0.2.2/src/pymodaq_femto/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/resources/load_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/resources/save_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95146 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:07:48.938170 pymodaq_femto-0.2.2/src/pymodaq_femto/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:07:48.938170 pymodaq_femto-0.2.2/src/pymodaq_femto/utils/raw_scans/
+-rw-r--r--   0 runner    (1001) docker     (123)  1554195 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/utils/raw_scans/example_measured_dscan_to_convert.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-15 15:07:37.000000 pymodaq_femto-0.2.2/src/pymodaq_femto/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:07:48.938170 pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-15 15:07:48.000000 pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-15 15:07:48.000000 pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:07:48.000000 pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-15 15:07:48.000000 pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-15 15:07:48.000000 pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 15:07:48.000000 pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/top_level.txt
```

### Comparing `pymodaq_femto-0.2.1/LICENSE` & `pymodaq_femto-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/PKG-INFO` & `pymodaq_femto-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_femto
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyMoDAQ extension for femtosecond laser pulse characterization
 Home-page: http://pymodaq.cnrs.fr
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CeCILL-B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_femto-0.2.1/setup.cfg` & `pymodaq_femto-0.2.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,14 @@
 [options.packages.find]
 where = src
 
 [options.entry_points]
 pymodaq.extensions = 
 	femto = pymodaq_femto
 console_scripts = 
-	simulator=pymodaq_femto.simulation:main
+	simulator=pymodaq_femto.simulator:main
 	retriever=pymodaq_femto.retriever:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/__init__.py` & `pymodaq_femto-0.2.2/src/pymodaq_femto/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/graphics.py` & `pymodaq_femto-0.2.2/src/pymodaq_femto/graphics.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/materials.py` & `pymodaq_femto-0.2.2/src/pymodaq_femto/materials.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/pnps.py` & `pymodaq_femto-0.2.2/src/pymodaq_femto/pnps.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/resources/load_settings.png` & `pymodaq_femto-0.2.2/src/pymodaq_femto/resources/load_settings.png`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/resources/save_settings.png` & `pymodaq_femto-0.2.2/src/pymodaq_femto/resources/save_settings.png`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/retriever.py` & `pymodaq_femto-0.2.2/src/pymodaq_femto/retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     RetrievalResultPlot,
     MplCanvas,
     NavigationToolbar,
     MeshDataPlot,
     PulsePlot,
     PulsePropagationPlot,
 )
-from pymodaq_femto.simulation import Simulator, methods, nlprocesses, materials
+from pymodaq_femto.simulator import Simulator, methods, nlprocesses, materials
 from collections import OrderedDict
 from pypret import FourierTransform, Pulse, PNPS, lib, MeshData, random_gaussian
 from pypret.frequencies import om2wl, wl2om, convert
 import scipy
 import importlib
 from scipy.fftpack import next_fast_len
 from pymodaq.daq_utils.h5modules import H5BrowserUtil, H5Saver
```

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/simulation.py` & `pymodaq_femto-0.2.2/src/pymodaq_femto/simulator.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py` & `pymodaq_femto-0.2.2/src/pymodaq_femto/utils/convert_to_pymodaq_compatible.py`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/utils/raw_scans/example_measured_dscan_to_convert.h5` & `pymodaq_femto-0.2.2/src/pymodaq_femto/utils/raw_scans/example_measured_dscan_to_convert.h5`

 * *Files identical despite different names*

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto/viewers.py` & `pymodaq_femto-0.2.2/src/pymodaq_femto/viewers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from qtpy.QtCore import QObject
 from qtpy import QtWidgets
 import matplotlib
 matplotlib.use('Qt5Agg')
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg, NavigationToolbar2QT as NavigationToolbar
 from matplotlib.figure import Figure
-from pymodaq_femto.simulation import Simulator
+from pymodaq_femto.simulator import Simulator
 from pyqtgraph.parametertree import ParameterTree
 
 class MplCanvas(FigureCanvasQTAgg):
     def __init__(self, parent=None, width=5, height=4, dpi=100):
         fig = Figure(figsize=(width, height), dpi=dpi)
         self.axes = fig.add_subplot(111)
         super(MplCanvas, self).__init__(fig)
```

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/PKG-INFO` & `pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-femto
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyMoDAQ extension for femtosecond laser pulse characterization
 Home-page: http://pymodaq.cnrs.fr
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CeCILL-B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_femto-0.2.1/src/pymodaq_femto.egg-info/SOURCES.txt` & `pymodaq_femto-0.2.2/src/pymodaq_femto.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 setup.py
 src/pymodaq_femto/VERSION
 src/pymodaq_femto/__init__.py
 src/pymodaq_femto/graphics.py
 src/pymodaq_femto/materials.py
 src/pymodaq_femto/pnps.py
 src/pymodaq_femto/retriever.py
-src/pymodaq_femto/simulation.py
+src/pymodaq_femto/simulator.py
 src/pymodaq_femto/viewers.py
 src/pymodaq_femto.egg-info/PKG-INFO
 src/pymodaq_femto.egg-info/SOURCES.txt
 src/pymodaq_femto.egg-info/dependency_links.txt
 src/pymodaq_femto.egg-info/entry_points.txt
 src/pymodaq_femto.egg-info/requires.txt
 src/pymodaq_femto.egg-info/top_level.txt
```

