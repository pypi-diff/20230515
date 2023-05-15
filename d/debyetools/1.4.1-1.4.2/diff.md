# Comparing `tmp/debyetools-1.4.1.tar.gz` & `tmp/debyetools-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/debyetools-1.4.1.tar", last modified: Mon May  8 19:48:26 2023, max compression
+gzip compressed data, was "dist/debyetools-1.4.2.tar", last modified: Mon May 15 18:19:58 2023, max compression
```

## Comparing `debyetools-1.4.1.tar` & `debyetools-1.4.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 19:48:26.363857 debyetools-1.4.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    34521 2023-05-08 19:47:31.000000 debyetools-1.4.1/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2642 2023-05-08 19:48:26.363857 debyetools-1.4.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2023-05-08 19:47:31.000000 debyetools-1.4.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 19:48:26.359857 debyetools-1.4.1/debyetools/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11745 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/anharmonicity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6335 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/aux_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1844 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/debfunct.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8033 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/defects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3717 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/electronic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1436 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/fs_compound_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9911 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/layout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11113 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/ndeb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4926 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/pairanalysis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3496 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/poisson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   161578 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/potentials.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4698 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/potentials_2.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 19:48:26.363857 debyetools-1.4.1/debyetools/tpropsgui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11483 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/atomtools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      688 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/dialog_doscar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      268 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/dialog_warning.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34356 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13883 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/functions0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2272 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/get_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42948 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10086 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/layout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8849 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/mainwindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/plot_EV.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/plotter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/plotter_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      883 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/toolbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2460 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_dialog_doscar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16226 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_heatcapacitywindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18970 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_interatomic_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22118 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_mainwindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/ui_warning.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7951 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/window_cp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6654 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/tpropsgui/window_interatomicparams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24920 2023-05-08 19:47:31.000000 debyetools-1.4.1/debyetools/vibrational.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-08 19:48:26.359857 debyetools-1.4.1/debyetools.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2642 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1341 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-05-08 19:48:26.000000 debyetools-1.4.1/debyetools.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-05-08 19:48:26.363857 debyetools-1.4.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2023-05-08 19:47:31.000000 debyetools-1.4.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-15 18:19:58.517797 debyetools-1.4.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34521 2023-05-15 18:18:27.000000 debyetools-1.4.2/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3187 2023-05-15 18:19:58.517797 debyetools-1.4.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2402 2023-05-15 18:18:27.000000 debyetools-1.4.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-15 18:19:58.509785 debyetools-1.4.2/debyetools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11745 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/anharmonicity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6563 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/aux_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1844 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/debfunct.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8033 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/defects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3723 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/electronic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1436 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/fs_compound_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9911 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/layout.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11240 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/ndeb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4645 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/pairanalysis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3410 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/poisson.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   156709 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/potentials.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4698 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/potentials_2.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-15 18:19:58.517797 debyetools-1.4.2/debyetools/tpropsgui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11445 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/atomtools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      688 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/dialog_doscar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      268 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/dialog_warning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34356 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/events.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13883 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/functions0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2272 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/get_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42963 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/gui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10086 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/layout.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9056 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/plot_EV.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/plotter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/plotter_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      883 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/toolbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2460 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/ui_dialog_doscar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16221 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/ui_heatcapacitywindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18970 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/ui_interatomic_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22050 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/ui_mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/ui_warning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7951 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/window_cp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6654 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/tpropsgui/window_interatomicparams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24920 2023-05-15 18:18:27.000000 debyetools-1.4.2/debyetools/vibrational.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-15 18:19:58.513791 debyetools-1.4.2/debyetools.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3187 2023-05-15 18:19:58.000000 debyetools-1.4.2/debyetools.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1341 2023-05-15 18:19:58.000000 debyetools-1.4.2/debyetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-15 18:19:58.000000 debyetools-1.4.2/debyetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       35 2023-05-15 18:19:58.000000 debyetools-1.4.2/debyetools.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-05-15 18:19:58.000000 debyetools-1.4.2/debyetools.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-05-15 18:19:58.517797 debyetools-1.4.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2023-05-15 18:18:27.000000 debyetools-1.4.2/setup.py
```

### Comparing `debyetools-1.4.1/LICENSE.md` & `debyetools-1.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/PKG-INFO` & `debyetools-1.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debyetools
-Version: 1.4.1
+Version: 1.4.2
 Summary: Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.
 Home-page: https://debyetools.readthedocs.io/
 Author: Javier Jofre
 Author-email: javier.jofre@polymtl.ca
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -20,67 +20,80 @@
 # debyetools
 
 Implementation of a tool for calculating self-consistent thermodynamic properties that can take into account all kinds of contributions to the free energy inluding explicit anharmonicity. The software presented here is based in the Debye approximation within the QHA using the crystal internal energetics parametrized at ground-state to project the thermodynamics properties at high temperatures. 
 
 Made by Javier Jofre: javier.jofre@polymtl.ca
 Please cite.
 
-### Requirements:
+### Requirements for Python module:
 - numpy
 - mpmath
 - scipy
-- PySimpleGUI
-- matplotlib
 
+### Requirements for Interface:
+For the interface it will also be necesary:
+- matplotlib
+- PySide6
 
 ### Installation
 ```
 pip install --upgrade debyetools
 ```
 
 ### Get started
 
 To start getting familiar with the interface `tProps` you can download `examples input files`.
 The GUI can be launched by executing the interface script from the debyetools repository main folder:
 
 ```
-python gui.py
+python interface.py
 ```
 
 Or you can launch  inside python:
 ```
-from debyetools.tpropsgui.gui import gui
-gui()
+from debyetools.tpropsgui.gui import interface
+interface()
 ```
 
 Debye tools can also be used as a library. Example: heat capacity of Al fcc using 3rd order Birch-Murnaghan EOS
 
 ```Python
 import numpy as np
+import debyetools.potentials as potentials
 from debyetools.ndeb import nDeb
 
-nu, m = 0.32, 0.026981500000000002
-Tmelting = 933
+# EOS parametrization
+# =========================
+EOS_parameters = [-3.607736520e+05, 9.929277050e-06, 7.729289055e+10, 4.604381753e+00]
+EOS = potentials.BM()
+EOS.fitEOS([0], [0], initial_parameters=EOS_parameters, fit=False)
 
-p_EOS = [-3.617047894e+05, 9.929931142e-06, 7.618619745e+10, 4.591924487e+00]
-p_intanh = 0, 1, p_EOS[1]
+# Other Contributions parametrization
+# =========================
 p_electronic = [3.8027342892e-01, -1.8875015171e-02, 5.3071034596e-04, -7.0100707467e-06]
-p_defects = 8.46, 1.69, Tmelting, 0.1, p_EOS[2],p_EOS[1]
-p_anh = 0,0,0
-
-EOS_name = 'BM'
-
-ndeb_BM = nDeb(nu, m, p_intanh, p_EOS, p_electronic, p_defects,p_anh,EOS_name)
-
-T,V = 9.33000000000e+02,1.07790131286e-05
-                       #
-result = ndeb_BM.eval_props(T,V)['Cp']
+mass = 0.026981500000000002
+Tmelting = 933
+p_defects = 8.46, 1.69, Tmelting, 0.1
+p_anharmonicity = 0, 1
+p_XS = 0, 0, 0
+poissonsratio = 0.37
+
+# F minimization using Slater approximaiton
+# =========================
+ndeb = nDeb(poissonsratio, mass, p_anharmonicity, EOS, p_electronic, p_defects, p_XS, mode='jjsl')
+T_initial, T_final= 0.1, 1000
+T = np.arange(T_initial, T_final, 10)
+Pressure = 0
+T, V = ndeb.min_G(T, EOS_parameters[0] * .9, P=Pressure)
+
+# Evaluation of thermodynamic properties
+# =========================
+tprops_dict = ndeb.eval_props(T, V, P=Pressure)
 ```
 
 To Do's:
 
-- Add More Examples to Documentation
 - Improve error handling
 - Add 'Compatible input files formats'
 - Improve Documentation
 - Add handling of anisotropic materials
 - Prediction of explicit anharmonicity parameters
```

### Comparing `debyetools-1.4.1/debyetools/anharmonicity.py` & `debyetools-1.4.2/debyetools/anharmonicity.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/aux_functions.py` & `debyetools-1.4.2/debyetools/aux_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 import itertools as it
 import re
 import numpy as np
+from typing import Tuple
 
 class logging(object):
     def __init__(self, *files):
         self.files = files
     def write(self, obj):
         for f in self.files:
             f.write(obj)
             f.flush() # If you want the output to be visible immediately
     def flush(self) :
         for f in self.files:
             f.flush()
-def c_types(atom_types):
+def c_types(atom_types: str) -> Tuple[list, list]:
     """
     returns all the pair types combinations.
 
-    :param list_of_str atom_types: the types of each atom in the primitive cell in the same order as the basis vectors.
+    :param str atom_types: the types of each atom in the primitive cell in the same order as the basis vectors.
+    :return: pair types and list wuth individual types.
+    :rtype: Tuple[list, list]
     """
     types_all = re.findall('[A-Z][^A-Z]*', atom_types)
     ptypes=list(set([s for s in types_all]))
     ptypes.sort()
     combs_types = list(it.combinations_with_replacement(ptypes, r=2))
     combs_types = [A[0]+'-'+A[1] for A in combs_types]
     return combs_types, types_all
 
 def generate_cells_coordinates(size, primitive_cell,center):
     """ generate the cell coordinates for which we are going
     to calculate the neighbor list.
 
-    :param array size: Number of times we are replicating the primitive cell
-    :param array primitive_cell: The primitive cell
-    :param array center: The position in space where the system of reference is
+    :param np.ndarray size: Number of times we are replicating the primitive cell
+    :param np.ndarray primitive_cell: The primitive cell
+    :param np.ndarray center: The position in space where the system of reference is
+    :return: cell coordinates.
+    :rtype: np.ndarray
 
     """
 
     cell_coords = np.array(list((it.product(np.arange(size[0]),
                                             np.arange(size[1]),
                                             np.arange(size[2])))))
 
     cell_coords_centered = cell_coords + center
     cell_coords_centered = np.dot(cell_coords_centered, primitive_cell)
 
     return cell_coords_centered
 
-def gen_Ts(Ti,Tf,nTs):
+def gen_Ts(Ti: float, Tf: float, nTs: int) -> np.ndarray:
     """
     Function to generate a range of temperatures.
 
     :param float Ti: Initial temperature. (Try not to use the value 0. Use 0.1 instead.)
     :param float Tf: Final temperature.
     :param int nTs: Number of values. This does not include room temperature, which is included anyways.
 
-    :retun list_of_floats: Values of temperatures between Ti and Tf, inclusive, plus room temperature.
+    :retun np.ndarray: Values of temperatures between Ti and Tf, inclusive, plus room temperature.
     """
     minF_step = (Tf - Ti)/(nTs - 1.)
     Ts = np.arange(Ti, Tf+minF_step, minF_step)
     Ts = np.r_[Ts, [298.15]]
     Ts.sort()
     return Ts
 def gen_Ps(Ti,Tf,nTs):
@@ -101,29 +106,29 @@
         ENAl = np.array(EN)
         # print(dosfile, EN)
         E.append([float(s) for s in list(ENAl[:,0])])
         N.append([float(s)/nat for s in list(ENAl[:,1])])
 
     return E,N,Ef
 
-def load_V_E(energy_dir,energy_dir_contcar, units='eV/atom'):
+def load_V_E(energy_dir_summary,energy_dir_contcar, units='eV/atom'):
     with open(energy_dir_contcar,'r') as f_poscar:
         f_poscar_lines = f_poscar.readlines()
         cell_poscar = f_poscar_lines[2:5]
 
         cell_lst = [c.split() for c in cell_poscar]
         diag_cell = [float(c[i]) for i, c in enumerate(cell_lst)]
 
         try:
             nat = sum([int(li) for li in np.fromstring(f_poscar_lines[5], dtype=int, sep=' ')])
             1/nat
         except:
             nat = sum([int(li) for li in np.fromstring(f_poscar_lines[6], dtype=int, sep=' ')])
             1/nat
-    with open(energy_dir + '/SUMMARY.fcc') as f_summary:
+    with open(energy_dir_summary) as f_summary:
         f_summary_lines = f_summary.readlines()
         f_summary_lines = list(dict.fromkeys(f_summary_lines))
         ds = []
         E = []
         for l in f_summary_lines:
             l_lst = l.split(' ')
             ds.append(float(l_lst[0]))
```

### Comparing `debyetools-1.4.1/debyetools/debfunct.py` & `debyetools-1.4.2/debyetools/debfunct.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/defects.py` & `debyetools-1.4.2/debyetools/defects.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/electronic.py` & `debyetools-1.4.2/debyetools/electronic.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,17 +88,17 @@
     NfV0 = (EfV0 - E1)*(N2 - N1)/(E2 - E1) + N1
     NfV = np.array([NfV0*np.sqrt(ef/EfV0) for ef in Ef][ixss:ixse])
     P2 = leastsq(NfV2m, p_el, args=(V[ixss:ixse], NfV),maxfev=1000)
 
     P2 = P2[0]
 
     NfVcalc = [NfV_poly_fun(Vi, P2[0], P2[1], P2[2], P2[3]) for Vi in V[ixss:ixse]]
-    print('#V NfVdata NfVcalc')
-    for Vi, Ndatai, Ncalci in zip(V[ixss:ixse], NfV, NfVcalc):
-        print('%.5e %.5e %.5e' % (Vi, Ndatai, Ncalci))
+    # print('#V NfVdata NfVcalc')
+    # for Vi, Ndatai, Ncalci in zip(V[ixss:ixse], NfV, NfVcalc):
+    #     print('%.5e %.5e %.5e' % (Vi, Ndatai, Ncalci))
     return P2
 
 def NfV_poly_fun(V, _A, _B, _C, _D):
     return _A + _B*V + _C*V**2 + _D*V**3
 
 def NfV2m(P, Vdata, NfVdata):
     NfVcalc = [NfV_poly_fun(Vi, P[0], P[1], P[2], P[3]) for Vi in Vdata]
```

### Comparing `debyetools-1.4.1/debyetools/fs_compound_db.py` & `debyetools-1.4.2/debyetools/fs_compound_db.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/layout.py` & `debyetools-1.4.2/debyetools/layout.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/ndeb.py` & `debyetools-1.4.2/debyetools/ndeb.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     :param list_of_floats EOS: Equation of state instance.
     :param list_of_floats p_electronic: Electronic contribution parameters.
     :param list_of_floats p_defects: Mono-vacancies defects contribution parameters: Evac00,Svac00,Tm,a,P2,V0.
     :param list_of_floats p_anh: Excess contribution parameters.
     :param string mode: Type of approximation of the Debye temperature (see vibrational contribution).
     """
 
-    def __init__(self, nu, m, p_intanh, EOS, p_electronic, p_defects, p_anh, *args, units='J/mol', mode='jjsl'):
+    def __init__(self, nu: float, m: float, p_intanh: np.ndarray, EOS: object, p_electronic: np.ndarray, p_defects: np.ndarray, p_anh: np.ndarray, *args: object, units: object = 'J/mol',
+                 mode: str = 'jjsl') -> None:
 
         a0, m0 = p_intanh
         q0, q1, q2, q3 = p_electronic
         Evac00, Svac00, Tm, a = p_defects
         s0, s1, s2 = p_anh
 
         self.nu, self.r, self.m = nu, 1, m
@@ -109,20 +110,20 @@
             V.append(V0i)
 
 
         newV = np.array(V)  # V[0]*np.exp(self.integrl())
         del V
 
         ixs = np.where(newV <= 1.5 * newV[0])
-        Tmax = T[-1]
+        # Tmax = T[-1]
         T, V = T[ixs], newV[ixs]
 
         return T, V
 
-    def eval_props(self, T, V, P):
+    def eval_props(self, T, V, P=None):
         """
         Evaluates the thermodynamic properties of a given compound/element at (T,V).
 
         :params float T: The temperature in Kelvin.
         :params float V: The volume in "units".
         :return dict: A dictionary with the following keys: 'T': temperature, 'V': volume, 'tD': Debye temperature, 'g': Gruneisen parameter, 'Kt': isothermal bulk modulus, 'Ktp': pressure derivative of the isothermal bulk modulus, 'Ktpp': second order pressure derivative of the isothermal bulk modulus, 'Cv': constant-volume heat capacity, 'a': thermal expansion, 'Cp': constant-pressure heat capacity, 'Ks': adiabatic bulk modulus , 'Ksp': pressure derivative of the adiabatic bulk modulus, 'G': Gibbs free energy, 'E': total internal energy, 'S': entropy, 'E0': 'cold' internal energy defined by the EOS, 'Fvib': vibrational free energy, 'Evib': vibrational internal energy, 'Svib': vibrational entropy, 'Cvvib': vibrational heat capacity, 'Pcold': 'cold' pressure, 'dPdT_V': (dP/dT)_V, 'G^2': Ktp**2-2*Kt*Ktpp, 'dSdP_T': (dS/dP)_T, 'dKtdT_P': (dKt/dT)_P, 'dadP_T': (da/dP)_T, 'dCpdP_T': (dCp/dP)_T, 'ddSdT_PdP_T': (d2S/dTdP).
         """
```

### Comparing `debyetools-1.4.1/debyetools/pairanalysis.py` & `debyetools-1.4.2/debyetools/pairanalysis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,95 +1,98 @@
 import numpy as np
 import itertools as it
 import debyetools.aux_functions as afn
+from typing import Tuple
 
-
-
-def neighbor_list(size, max_distance, center, basis_vectors, primitive_cell, ncells=True):
+def neighbor_list(size: np.ndarray, basis: np.ndarray, cell: np.ndarray, cutoff: float)->Tuple[np.ndarray,np.ndarray,np.ndarray]:
     """ calculate a list i, j, dij where i and j are a pair of atoms of
     indexes i and j, respectively, and dij is the distance between them.
 
-    :param array size: Number of times we are replicating the primitive cel
-    :param int max_distance: Number of times we are replicating the supercell up to which we are considering for the calculation (uses pbc)
-    :param array center: The position in space where the system of reference is
-    :param array basis_vectors: atoms position within a single primitive cell
-    :param array primitive_cell: the primitive cell
+    :param np.ndarray size: Number of times we are replicating the primitive cel
+    :param np.ndarray basis: atoms position within a single primitive cell
+    :param np.ndarray cell: the primitive cell
+    :param float cutoff: cut-off distance
     :return: D, I , J
-    """
+    :rtype: Tuple[np.ndarray, np.ndarray, np.ndarray]
+    
 
-    basis_vectors = np.dot(basis_vectors,primitive_cell)
-    size_g = size + 2*max_distance  #to do: change max_distance for some other word and add a max_distance distance.
-                              # new_co= int(min(max_distance,....))
+    """
+    max_depth = np.array([2*int(m) for m in cutoff/np.linalg.norm(cell, axis=1)])
+    center = np.array([0,0,0])
+    basis = np.dot(basis, cell)
+    size_g = size + 2*max_depth
 
-    cell_coords_centered = afn.generate_cells_coordinates(size, primitive_cell, center)
-    cell_coords_centered_g = afn.generate_cells_coordinates(size_g, primitive_cell, center-max_distance)
+    cell_coords_centered = afn.generate_cells_coordinates(size, cell, center)
+    cell_coords_centered_g = afn.generate_cells_coordinates(size_g, cell, center-max_depth)
     # print(size_g)
 
     XCs = []
     Is = []
     Js = []
     CIXs = []
 
 
-    ixs = np.arange(len(basis_vectors))
-    jxs = np.arange(len(basis_vectors))
+    ixs = np.arange(len(basis))
+    jxs = np.arange(len(basis))
 
     for cell_coords_i in cell_coords_centered:
-        ix_neighbor = np.where(np.all(abs(cell_coords_centered_g-cell_coords_i)<=max_distance, axis=1))[0]
-        Xs = np.array([cell_coords_i,]*len(basis_vectors))+basis_vectors
+        ix_neighbor = np.where(np.all(abs(cell_coords_centered_g-cell_coords_i)<=cutoff, axis=1))[0]
+        Xs = np.array([cell_coords_i,]*len(basis))+basis
 
         for ixx, cell_coords_i_g in enumerate(cell_coords_centered_g[ix_neighbor]):
-            Xsg = np.array([cell_coords_i_g,]*len(basis_vectors))+basis_vectors
+            Xsg = np.array([cell_coords_i_g,]*len(basis))+basis
             for x, xg in it.product(Xs, Xsg):
                 XCs.append((x-xg)**2)
             for i, j in it.product(ixs, jxs):
                 Is.append(i)
                 Js.append(j)
                 CIXs.append(ix_neighbor[ixx])
 
 
     XCs = np.array(XCs)
     Is = np.array(Is)
     Js = np.array(Js)
     CIXs = np.array(CIXs)
 
-    CX = np.sum(XCs/max_distance**2, axis=1)
+    CX = np.sum(XCs/cutoff**2, axis=1)
 
     ix = np.where(np.all([CX<=1, CX>0], axis=0))[0]
     distances = np.sqrt(np.sum(XCs[ix], axis=1))
 
-    res = distances, Is[ix], Js[ix], cell_coords_centered_g, CIXs[ix]
+    res = distances, Is[ix], Js[ix]#, cell_coords_centered_g, CIXs[ix]
 
     return res
 
-def pair_analysis(atom_types, size, max_distance, center, basis_vectors, primitive_cell, prec=10, full=False, cutoff=None):
+def pair_analysis(atom_types, cutoff, basis, cell, prec=10, full=False):
     """
     run a pair analysis of a crystal structure of almost any type of symmetry.
 
-    :param list_of_str atom_types: the types of each atom in the primitive cell in the same order as the basis vectors.
-    :param array size: Number of times we are replicating the primitive cel
-    :param int max_distance: Number of times we are replicating the supercell up to which we are considering for the calculation (uses pbc)
-    :param array center: The position in space where the system of reference is
-    :param array basis_vectors: atoms position within a single primitive cell
-    :param array primitive_cell: the primitive cell
+    :param str atom_types: the types of each atom in the primitive cell in the same order as the basis vectors.
+    :param float cutoff: cut-off distance
+    :param np.ndarray basis: atoms position within a single primitive cell
+    :param np.ndarray cell: the primitive cell
     :return:  pair distance, pair number, pair types
+    :rtype: Tuple[np.ndarray,np.ndarray,np.ndarray]
     """
-    max_distance = np.array([int(max_distance), int(max_distance), int(max_distance)]) ##<--- fix_here
-    dAxBy, iAxBy, jAxBy, cells_cohordniates, ij_ccix  = neighbor_list(size, max_distance, center, basis_vectors, primitive_cell)
+    # dAxBy, iAxBy, jAxBy, cells_cohordniates, ij_ccix  = neighbor_list(size, max_distance, center, basis, cell)
+    size=np.array([1,1,1])
+    dAxBy, iAxBy, jAxBy  = neighbor_list(size, basis, cell, cutoff)
+    # max_distance = np.array([int(cutoff), int(cutoff), int(cutoff)]) ##<--- fix_here
     if cutoff is not None:
         maxdjx = np.where(dAxBy <= cutoff)
-        dAxBy, iAxBy, jAxBy, ij_ccix = dAxBy[maxdjx], iAxBy[maxdjx], jAxBy[maxdjx], ij_ccix[maxdjx]
+        # dAxBy, iAxBy, jAxBy, ij_ccix = dAxBy[maxdjx], iAxBy[maxdjx], jAxBy[maxdjx], ij_ccix[maxdjx]
+        dAxBy, iAxBy, jAxBy = dAxBy[maxdjx], iAxBy[maxdjx], jAxBy[maxdjx]
     dAxBy = np.array([np.round(d,prec) for d in dAxBy])
-    res_2 = dAxBy, iAxBy, jAxBy
-    nat = np.prod(size)*len(basis_vectors)
+    # res_2 = dAxBy, iAxBy, jAxBy
+    nat = np.prod(size)*len(basis)
 
     combs_types,types_all = afn.c_types(atom_types)
 
     # dAxBy = np.array([float('%0.10e'%(d)) for d in dAxBy])
-    bins_dAxBy =list(set([li for li in list(set(np.append(dAxBy, [max(max_distance)])))]))
+    bins_dAxBy =list(set([li for li in list(set(np.append(dAxBy, [cutoff])))]))
     bins_dAxBy.sort()
     distances = bins_dAxBy[:-1]
 
     ptlst = []
     for i,j,d in zip(iAxBy,jAxBy,dAxBy):
         for ii in range(len(combs_types)):
             if (types_all[i]+'-'+types_all[j] == combs_types[ii]) or (types_all[j]+'-'+types_all[i] == combs_types[ii]):
@@ -105,10 +108,11 @@
     bs = ['' for x in range(len(combs_types))]
     for i in range(len(combs_types)):
         hs[i], bs[i] = np.histogram(ds[i], bins=bins_dAxBy)
     tot_num_bonds_per_molecule = np.array(hs).T
     num_bonds_per_formula = tot_num_bonds_per_molecule/nat
 
     if full:
-        return np.array(distances), num_bonds_per_formula, combs_types, res_2[0], res_2[1], res_2[2], cells_cohordniates, ij_ccix
+        # return np.array(distances), num_bonds_per_formula, combs_types, res_2[0], res_2[1], res_2[2], cells_cohordniates, ij_ccix
+        return np.array(distances), num_bonds_per_formula, combs_types
     else:
         return np.array(distances), num_bonds_per_formula, combs_types
```

### Comparing `debyetools-1.4.1/debyetools/poisson.py` & `debyetools-1.4.2/debyetools/poisson.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,31 +5,31 @@
     :param list_of_lists_of_floats EM: Elastic moduli matrix.
 
     :return float: Poisson's ratio.
     """
     if quiet:
         return quiet_pa(EM)
 
-    C11, C12, C13 = EM[0,0]*1e-1, EM[0,1]*1e-1, EM[0,2]*1e-1
-    C22, C23 = EM[1,1]*1e-1, EM[1,2]*1e-1
-    C33 = EM[2,2]*1e-1
-    C44 = EM[3,3]*1e-1
-    C55 = EM[4,4]*1e-1
-    C66 = EM[5,5]*1e-1
-
-    if EM[0,4]**2*1e-1>0:
-        C15 = EM[0,4]*1e-1
-        C25 = EM[1,4]*1e-1
-        C35 = EM[2,4]*1e-1
-        C46 = EM[3,5]*1e-1
+    C11, C12, C13 = EM[0,0], EM[0,1], EM[0,2]
+    C22, C23 = EM[1,1], EM[1,2]
+    C33 = EM[2,2]
+    C44 = EM[3,3]
+    C55 = EM[4,4]
+    C66 = EM[5,5]
+
+    if EM[0,4]**2>0:
+        C15 = EM[0,4]
+        C25 = EM[1,4]
+        C35 = EM[2,4]
+        C46 = EM[3,5]
     else:
-        C15 = EM[0,5]*1e-1
-        C25 = EM[1,5]*1e-1
-        C35 = EM[2,5]*1e-1
-        C46 = EM[3,4]*1e-1
+        C15 = EM[0,5]
+        C25 = EM[1,5]
+        C35 = EM[2,5]
+        C46 = EM[3,4]
 
     f = C11*(C22*C55-C25**2)-C12*(C12*C55-C15*C25)+C15*(C12*C25-C15*C22)+C25*(C23*C35-C25*C33)
     g = C11*C22*C33-C11*C23**2-C22*C13**2-C33*C12**2+2*C12*C13*C23
     Omega=2*(C15*C25*(C33*C12-C13*C23)+C15*C35*(C22*C13-C12*C23)+C25*C35*(C11*C23-C12*C13)) -(C15**2*(C22*C33-C23**2)+C25**2*(C11*C33-C13**2)+C35**2*(C11*C22-C12**2))+g*C55
     GV = 1/15*(C11+C22+C33+3*(C44+C55+C66)-(C12+C13+C23))
     GR = 15*(4*((C33*C55-C35**2)*(C11+C22+C12) + (C23*C55-C25*C35)*(C11-C12-C23) + (C13*C35-C15*C33)*(C15+C25) + (C13*C55-C15*C35)*(C22-C12-C23-C13) + (C13*C25-C15*C23)*(C15-C25) + f)/Omega+3*(g/Omega+(C44+C66)/(C44*C66-C46**2)))**(-1)
     BV = (C11+C22+C33+2*(C12+C13+C23))/9
@@ -40,16 +40,16 @@
     Sr=GR
     Sv=GV
     B = (BR+BV)/2
     S = (GR+GV)/2
     Y = (9.*B*S)/(3.*B+S)
     nu = (3.*B-Y)/(6.*B)
     AU = 5*Sv/Sr+Bv/Br-6
-    print('Sv/Sr',Sv/Sr, 'Bv/Br', Bv/Br)
-    print('C11, C12, C13, C15, C22, C23, C25, C33, C35, C44, C46, C55, C66, B, Y, S, AU, nu','\n',C11, C12, C13, C15, C22, C23, C25, C33, C35, C44, C46, C55, C66, B, Y, S, AU, nu)
+    # print('Sv/Sr',Sv/Sr, 'Bv/Br', Bv/Br)
+    # print('C11, C12, C13, C15, C22, C23, C25, C33, C35, C44, C46, C55, C66, B, Y, S, AU, nu','\n',C11, C12, C13, C15, C22, C23, C25, C33, C35, C44, C46, C55, C66, B, Y, S, AU, nu)
 
     return nu
 
 def quiet_pa(EM):
     C11, C12, C13 = EM[0,0]*1e-1, EM[0,1]*1e-1, EM[0,2]*1e-1
     C22, C23 = EM[1,1]*1e-1, EM[1,2]*1e-1
     C33 = EM[2,2]*1e-1
```

### Comparing `debyetools-1.4.1/debyetools/potentials.py` & `debyetools-1.4.2/debyetools/potentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,35 +30,24 @@
         :type initial_parameters: list.
         :param bool fit: True to run the fitting. False to just use the input parameters.
 
         :return: Optimal parameters.
         :rtype: list
         """
         if fit:
-            # print(verb, 0)
             pEOS = initial_parameters[:4]
-            # print(verb, 1)
-            # for x in [self.error2min, pEOS,Vdata, Edata]:
-            #     print(type(x))
             popt = least_squares(self.error2min, pEOS, args=(Vdata, Edata))['x']
-            # print(verb, 2)
             self.pEOS = popt
-            # print(verb, 3)
         if not fit:
             self.pEOS = initial_parameters[:4]
 
-        # bounds = [(min(Vdata) * .99, max(Vdata) * 1.01)]
-        # mV = minimize(self.E0, [np.mean(Vdata)], bounds=bounds, tol=1e-10)
-        # print(verb, 4)
         mV = minimize(self.E0, [np.mean(Vdata)], bounds=[(min(Vdata), max(Vdata))], tol=1e-10)
-        # print(verb, 5)
         self.V0 = mV['x'][0]
-        # print(verb, 6)
 
-        return self.pEOS
+        # return self.pEOS
 
     def E04min(self, V, pEOS):
         E0, V0, B0, Bp0 = pEOS
         if B0<0:
             return 1
         P0, P1, P2, P3 = EVBBp_to_BMparams(pEOS)
         return P0 + P1 / V ** (2 / 3) + P2 / V ** (4 / 3) + P3 * V ** (-6 / 3)
@@ -529,23 +518,20 @@
 
     :param list args: formula, primitive_cell, basis_vectors, cutoff, number_of_neighbor_levels.
     :param list_of_floats parameters: Morse potential parameters.
     """
 
     def __init__(self, *args, units='J/mol', parameters='', prec=10):
         formula, primitive_cell, basis_vectors, cutoff, number_of_neighbor_levels = args
-        # formula,    primitive_cell,    basis_vectors    = pair_analysis.ReadPOSCAR(ins_atoms_positions_filename)
         self.formula, self.primitive_cell, self.basis_vectors = formula, primitive_cell, basis_vectors
 
         size = np.array([1, 1, 1])
-        center = np.array([0, 0, 0])
         atom_types = formula * np.prod(size)
         neigbor_distances_at_Vstar, number_of_pairs_per_distance, comb_types = pairanalysis.pair_analysis(atom_types,
-                                                                                                          size, cutoff,
-                                                                                                          center,
+                                                                                                          cutoff,
                                                                                                           basis_vectors,
                                                                                                           primitive_cell,
                                                                                                           prec=prec)
 
         neigbor_distances_at_Vstar, number_of_pairs_per_distance = neigbor_distances_at_Vstar[
                                                                    :number_of_neighbor_levels], number_of_pairs_per_distance[
                                                                                                 :number_of_neighbor_levels,
@@ -586,18 +572,15 @@
             lstsq_sol = least_squares(self.error2min, pEOS, args=(Vdata, Edata), bounds=(0, np.inf))
             popt = lstsq_sol['x']
             self.pEOS = popt
             self.eos_residuals = lstsq_sol['fun']
         if not fit:
             self.pEOS = initial_parameters
 
-            #        for i in range(-20, 21):
-            #            print(Vdata[0]*(1+i/100) , self.E0(Vdata[0]*(1+i/100)))
         mV = minimize(self.E0, [np.mean(Vdata)], bounds=[(min(Vdata) * .9, max(Vdata) * 1.1)], tol=1e-10)
-        # mV2 = self.minimize_bruteforce(self.E0, [np.mean(Vdata)], bounds=[(min(Vdata)*.9, max(Vdata)*1.1)], tol=1e-10)
         self.V0 = mV['x'][0]
 
         return self.pEOS
 
     def E04min(self, V, pEOS):
         if type(V) == np.ndarray:
             return np.array([self.E04min(Vi, pEOS) for Vi in V])
@@ -619,16 +602,15 @@
         V = V / self.mult_V
         pEOS = self.pEOS
         pEOS = pEOS.reshape((int(len(pEOS) / 3)), 3)
         Ds, alphas, r0s = pEOS.T[:]
         ms = []
         for njs, Dj, alphaj, r0j in zip(self.npair.T, Ds, alphas, r0s):
             for rstari, nij in zip(self.ndist, njs):
-                ms.append(
-                    nij / 2 * Dj * ((1 - np.exp(-alphaj * (rstari * (V / self.Vstar) ** (1 / 3) - r0j))) ** 2 - 1))
+                ms.append(nij / 2 * Dj * ((1 - np.exp(-alphaj * (rstari * (V / self.Vstar) ** (1 / 3) - r0j))) ** 2 - 1))
         return np.sum(ms) * (self.mult_E)
 
     def dE0dV_T(self, V):
         """
         (dE0/dV)_T
 
         :param float V: Volume.
@@ -638,18 +620,15 @@
         V = V / self.mult_V
         pEOS = self.pEOS
         pEOS = pEOS.reshape((int(len(pEOS) / 3)), 3)
         Ds, alphas, r0s = pEOS.T[:]
         ms = []
         for njs, Dj, alphaj, r0j in zip(self.npair.T, Ds, alphas, r0s):
             for rstari, nij in zip(self.ndist, njs):
-                ms.append(-nij * Dj * (-1 + np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                            2 / 3)) / self.Vstar)) * alphaj * rstari * np.exp(
-                    alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) / (
-                                      3 * self.Vstar ** (1 / 3) * V ** (2 / 3)))
+                ms.append(-nij * Dj * (-1 + np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar)) * alphaj * rstari * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) / (3 * self.Vstar ** (1 / 3) * V ** (2 / 3)))
         return np.sum(ms) * (self.mult_E) / (self.mult_V)
 
     def d2E0dV2_T(self, V):
         """
         (d2E0/dV2)_T
 
         :param float V: Volume.
@@ -659,21 +638,15 @@
         V = V / self.mult_V
         pEOS = self.pEOS
         pEOS = pEOS.reshape((int(len(pEOS) / 3)), 3)
         Ds, alphas, r0s = pEOS.T[:]
         ms = []
         for njs, Dj, alphaj, r0j in zip(self.npair.T, Ds, alphas, r0s):
             for rstari, nij in zip(self.ndist, njs):
-                ms.append(2 * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                            2 / 3)) / self.Vstar) * nij * alphaj * rstari * Dj * (
-                                      (alphaj * rstari * V ** (1 / 3) * self.Vstar ** (2 / 3) + self.Vstar) * np.exp(
-                                  alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                              2 / 3)) / self.Vstar) - (1 / 2) * alphaj * rstari * V ** (
-                                                  1 / 3) * self.Vstar ** (2 / 3) - self.Vstar) / (
-                                      9 * V ** (5 / 3) * self.Vstar ** (4 / 3)))
+                ms.append(2*np.exp(alphaj*(r0j*self.Vstar-rstari*V**(1/3)*self.Vstar**(2/3))/self.Vstar)*nij*alphaj*rstari*Dj*((alphaj*rstari*V**(1/3)*self.Vstar**(2/3)+self.Vstar)*np.exp(alphaj*(r0j*self.Vstar-rstari*V**(1/3)*self.Vstar**(2/3))/self.Vstar)-(1/2)*alphaj*rstari*V**(1/3)*self.Vstar**(2/3)-self.Vstar)/(9*V**(5/3)*self.Vstar**(4/3)))
         return np.sum(ms) * (self.mult_E) / (self.mult_V) ** 2
 
     def d3E0dV3_T(self, V):
         """
         (d3E0/dV3)_T
 
         :param float V: Volume.
@@ -683,27 +656,15 @@
         V = V / self.mult_V
         pEOS = self.pEOS
         pEOS = pEOS.reshape((int(len(pEOS) / 3)), 3)
         Ds, alphas, r0s = pEOS.T[:]
         ms = []
         for njs, Dj, alphaj, r0j in zip(self.npair.T, Ds, alphas, r0s):
             for rstari, nij in zip(self.ndist, njs):
-                ms.append(-nij * Dj * alphaj * rstari * np.exp(
-                    alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) * (
-                                      4 * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                          2 / 3)) / self.Vstar) * alphaj ** 2 * rstari ** 2 * V ** (
-                                                  2 / 3) * self.Vstar ** (1 / 3) - alphaj ** 2 * rstari ** 2 * V ** (
-                                                  2 / 3) * self.Vstar ** (1 / 3) + 12 * alphaj * rstari * np.exp(
-                                  alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                              2 / 3)) / self.Vstar) * V ** (1 / 3) * self.Vstar ** (
-                                                  2 / 3) - 6 * alphaj * rstari * V ** (1 / 3) * self.Vstar ** (
-                                                  2 / 3) + 10 * self.Vstar * np.exp(alphaj * (
-                                          r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                              2 / 3)) / self.Vstar) - 10 * self.Vstar) / (
-                                      27 * self.Vstar ** (4 / 3) * V ** (8 / 3)))
+                ms.append(-nij*Dj*alphaj*rstari*np.exp(alphaj*(r0j*self.Vstar-rstari*V**(1/3)*self.Vstar**(2/3))/self.Vstar)*(4*np.exp(alphaj*(r0j*self.Vstar-rstari*V**(1/3)*self.Vstar**(2 / 3)) / self.Vstar) * alphaj ** 2 * rstari ** 2 * V ** (2 / 3) * self.Vstar ** (1 / 3) - alphaj ** 2 * rstari ** 2 * V ** (2 / 3) * self.Vstar ** (1 / 3) + 12 * alphaj * rstari * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) * V ** (1 / 3) * self.Vstar ** (2 / 3) - 6 * alphaj * rstari * V ** (1 / 3) * self.Vstar ** (2 / 3) + 10 * self.Vstar * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) - 10 * self.Vstar) / (27 * self.Vstar ** (4 / 3) * V ** (8 / 3)))
         return np.sum(ms) * (self.mult_E) / (self.mult_V) ** 3
 
     def d4E0dV4_T(self, V):
         """
         (d4E0/dV4)_T
 
         :param float V: Volume.
@@ -713,30 +674,15 @@
         V = V / self.mult_V
         pEOS = self.pEOS
         pEOS = pEOS.reshape((int(len(pEOS) / 3)), 3)
         Ds, alphas, r0s = pEOS.T[:]
         ms = []
         for njs, Dj, alphaj, r0j in zip(self.npair.T, Ds, alphas, r0s):
             for rstari, nij in zip(self.ndist, njs):
-                ms.append(8 * nij * alphaj * np.exp(
-                    alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) * ((
-                                                                                                                                                                      V * alphaj ** 3 * rstari ** 3 + 6 * alphaj ** 2 * rstari ** 2 * V ** (
-                                                                                                                                                                      2 / 3) * self.Vstar ** (
-                                                                                                                                         1 / 3) + 13 * alphaj * rstari * V ** (
-                                                                                                                                         1 / 3) * self.Vstar ** (
-                                                                                                                                         2 / 3) + 10 * self.Vstar) * np.exp(
-                    alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) - (
-                                                                                                                             1 / 8) * V * alphaj ** 3 * rstari ** 3 - 3 * alphaj ** 2 * rstari ** 2 * V ** (
-                                                                                                                             2 / 3) * self.Vstar ** (
-                                                                                                                             1 / 3) * (
-                                                                                                                             1 / 2) - 13 * alphaj * rstari * V ** (
-                                                                                                                             1 / 3) * self.Vstar ** (
-                                                                                                                             2 / 3) * (
-                                                                                                                             1 / 2) - 10 * self.Vstar) * rstari * Dj / (
-                                      81 * self.Vstar ** (4 / 3) * V ** (11 / 3)))
+                ms.append(8*nij*alphaj*np.exp(alphaj*(r0j*self.Vstar-rstari*V**(1/3)*self.Vstar**(2/3))/self.Vstar)*((V*alphaj**3*rstari**3+6*alphaj**2*rstari**2*V**(2/3)*self.Vstar**(1/3)+13*alphaj*rstari*V**(1/3)*self.Vstar**(2/3)+10*self.Vstar)*np.exp(alphaj*(r0j*self.Vstar-rstari*V**(1/3)*self.Vstar**(2/3))/self.Vstar)-(1/8)*V*alphaj**3*rstari**3-3*alphaj**2*rstari**2*V**(2/3)*self.Vstar**(1/3)*(1/2)-13*alphaj*rstari*V**(1/3)*self.Vstar**(2/3)*(1/2)-10*self.Vstar)*rstari*Dj/(81*self.Vstar**(4/3)*V**(11/3)))
         return np.sum(ms) * (self.mult_E) / (self.mult_V) ** 4
 
     def d5E0dV5_T(self, V):
         """
         (d5E0/dV5)_T
 
         :param float V: Volume.
@@ -746,35 +692,15 @@
         V = V / self.mult_V
         pEOS = self.pEOS
         pEOS = pEOS.reshape((int(len(pEOS) / 3)), 3)
         Ds, alphas, r0s = pEOS.T[:]
         ms = []
         for njs, Dj, alphaj, r0j in zip(self.npair.T, Ds, alphas, r0s):
             for rstari, nij in zip(self.ndist, njs):
-                ms.append(-nij * Dj * alphaj * rstari * np.exp(
-                    alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) * (
-                        16 * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                          2 / 3)) / self.Vstar) * V ** (
-                                                  4 / 3) * alphaj ** 4 * rstari ** 4 * self.Vstar ** (2 / 3) - V ** (
-                                                  4 / 3) * alphaj ** 4 * rstari ** 4 * self.Vstar ** (
-                                2 / 3) + 160 * np.exp(alphaj * (
-                                          r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                              2 / 3)) / self.Vstar) * V * self.Vstar * alphaj ** 3 * rstari ** 3 - 20 * V * self.Vstar * alphaj ** 3 * rstari ** 3 + 640 * np.exp(
-                                  alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                              2 / 3)) / self.Vstar) * alphaj ** 2 * rstari ** 2 * V ** (
-                                                  2 / 3) * self.Vstar ** (
-                                                  4 / 3) - 160 * alphaj ** 2 * rstari ** 2 * V ** (
-                                                  2 / 3) * self.Vstar ** (4 / 3) + 1200 * np.exp(alphaj * (
-                                          r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                              2 / 3)) / self.Vstar) * self.Vstar ** (5 / 3) * alphaj * rstari * V ** (
-                                                  1 / 3) - 600 * self.Vstar ** (5 / 3) * alphaj * rstari * V ** (
-                                1 / 3) + 880 * np.exp(alphaj * (
-                        r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (
-                                              2 / 3)) / self.Vstar) * self.Vstar ** 2 - 880 * self.Vstar ** 2) / (
-                                      243 * V ** (14 / 3) * self.Vstar ** (7 / 3)))
+                ms.append(-nij * Dj * alphaj * rstari * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (2 / 3)) / self.Vstar) * (16 * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (  2 / 3)) / self.Vstar) * V ** (  4 / 3) * alphaj ** 4 * rstari ** 4 * self.Vstar ** (2 / 3) - V ** (  4 / 3) * alphaj ** 4 * rstari ** 4 * self.Vstar ** (2 / 3) + 160 * np.exp(alphaj * (  r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (  2 / 3)) / self.Vstar) * V * self.Vstar * alphaj ** 3 * rstari ** 3 - 20 * V * self.Vstar * alphaj ** 3 * rstari ** 3 + 640 * np.exp(  alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (  2 / 3)) / self.Vstar) * alphaj ** 2 * rstari ** 2 * V ** (  2 / 3) * self.Vstar ** (  4 / 3) - 160 * alphaj ** 2 * rstari ** 2 * V ** (  2 / 3) * self.Vstar ** (4 / 3) + 1200 * np.exp(alphaj * (  r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (  2 / 3)) / self.Vstar) * self.Vstar ** (5 / 3) * alphaj * rstari * V ** (  1 / 3) - 600 * self.Vstar ** (5 / 3) * alphaj * rstari * V ** (1 / 3) + 880 * np.exp(alphaj * (r0j * self.Vstar - rstari * V ** (1 / 3) * self.Vstar ** (  2 / 3)) / self.Vstar) * self.Vstar ** 2 - 880 * self.Vstar ** 2) / (  243 * V ** (14 / 3) * self.Vstar ** (7 / 3)))
         return np.sum(ms) * (self.mult_E) / (self.mult_V) ** 5
 
     def d6E0dV6_T(self, V):
         """
         (d6E0/dV6)_T
 
         :param float V: Volume.
@@ -2471,20 +2397,17 @@
         #
         # self.stat = 0
         self.nats = len(basis_vectors)
         formula_ABCD = ''.join([Chr_fix[i] for i in range(len(re.findall('[A-Z][**A-Z]*', formula)))])
         self.formula_ABCD = formula_ABCD
         # # ## pr0nt(formula_ABCD)
         #
-        size = np.array([1, 1, 1])
-        center = np.array([0, 0, 0])
-        atom_types = self.formula_ABCD * np.prod(size)
+        atom_types = self.formula_ABCD
         neigbor_distances_at_Vstar, number_of_pairs_per_distance, comb_types = pairanalysis.pair_analysis(atom_types,
-                                                                                                          size, cutoff,
-                                                                                                          center,
+                                                                                                          cutoff,
                                                                                                           basis_vectors,
                                                                                                           primitive_cell)
         neigbor_distances_at_Vstar, number_of_pairs_per_distance = neigbor_distances_at_Vstar[
                                                                    :number_of_neighbor_levels], number_of_pairs_per_distance[
                                                                                                 :number_of_neighbor_levels,
                                                                                                 :]
         #
```

### Comparing `debyetools-1.4.1/debyetools/potentials_2.py` & `debyetools-1.4.2/debyetools/potentials_2.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/atomtools.py` & `debyetools-1.4.2/debyetools/tpropsgui/atomtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,8 +472,8 @@
 
     def update_fomula(self, types):
         self.types = types
         self.formula = ''.join([s for s in types])
 
     def run_pa(self, cutoff):
         self.cutoff = cutoff
-        self.distances, self.num_bonds_per_formula, self.combs_types = dt_pa_calc.pair_analysis(self.formula, np.array([1,1,1]), self.cutoff, np.array([0,0,0]), self.basis, self.cell)
+        self.distances, self.num_bonds_per_formula, self.combs_types = dt_pa_calc.pair_analysis(self.formula, self.cutoff, self.basis, self.cell)
```

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/dialog_doscar.py` & `debyetools-1.4.2/debyetools/tpropsgui/dialog_doscar.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/elements.py` & `debyetools-1.4.2/debyetools/tpropsgui/elements.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/events.py` & `debyetools-1.4.2/debyetools/tpropsgui/events.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/functions0.py` & `debyetools-1.4.2/debyetools/tpropsgui/functions0.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/get_functions.py` & `debyetools-1.4.2/debyetools/tpropsgui/get_functions.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/gui.py` & `debyetools-1.4.2/debyetools/tpropsgui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                 window['||B_plotter_fsprop2plt'].update(disabled=True)
                 window['||B_eval_tprops'].update(disabled=True)
                 window['||B_run_fs_params'].update(disabled=True)
 
                 window['--IC_prop2plt'].update('')
                 # print(verb,'02')
 
-                V_DFT, E_DFT = load_V_E(str_folderbrowser, str_folderbrowser+'/CONTCAR.5', units='J/mol')
+                V_DFT, E_DFT = load_V_E(str_folderbrowser+'/SUMMARY.fcc', str_folderbrowser+'/CONTCAR.5', units='J/mol')
                 # print(verb,'3')
 
                 for k in opened_EOS_dict:
                     if opened_EOS_dict[k]:
                         if k in ['MP','EAM']:
                             # print(verb,'4')
```

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/layout.py` & `debyetools-1.4.2/debyetools/tpropsgui/layout.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/mainwindow.py` & `debyetools-1.4.2/debyetools/tpropsgui/mainwindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
         self.check_el.stateChanged.connect(self.on_check_el)
         self.check_def.stateChanged.connect(self.on_check_def)
         self.check_anh.stateChanged.connect(self.on_check_anh)
         self.check_xs.stateChanged.connect(self.on_check_xs)
 
         self.ui.progress.setGeometry(450, 525, 80, 5)
+        self.ui.progress_2.setGeometry(260, 165, 80, 5)
 
         self.ipotparamsdialog = windowInteratormic(self)
         self.ipotparamsdialog.args = (None,)
         self.ipotparamsdialog.external_params_lineText = self.ui.lineEdit_2
 
         self.plotwindow = windowPlot(self)
         self.ui.actionEV.triggered.connect(self.plotEV)
@@ -80,14 +81,15 @@
         self.plotwindow.ax.set_ylim((min(Ydata)-spanY, max(Ydata)+spanY))
         self.plotwindow.ax.legend(loc=9)
         self.plotwindow.ax.set_xlabel(r'$10^{-5}m^3/mol$-$at$')
         self.plotwindow.ax.set_ylabel(r'$kJ/mol$-$at$')
         self.plotwindow.show()
 
     def selectionchange(self, i):
+        self.ui.progress_2.setValue(0)
         dict_eos = {'Birch-Murnaghan':'BM', 'Rose-Vinet':'RV', 'Mie-Gruneisen':'MG', 'TB-SMA':'TB',
                     'Murnaghan':'MU', 'Poirier-Tarantola':'PT', 'Morse int. potential':'MP', 'EAM int. potential':'EAM'}
         self.eos_str = dict_eos[self.ui.comboBox.itemText(i)]
 
         self.ipotparamsdialog.args = (None,)
         self.ui.lineEdit_2.setText('-3e5, 1e-5, 7e10, 4')
         if self.eos_str in ['MP', 'EAM']:
@@ -147,24 +149,28 @@
         self.ui.lineEdit_anh.setEnabled(self.state_anh)
 
     def on_check_xs(self):
         self.state_xs = self.check_xs.isChecked()
         self.ui.lineEdit_xs.setEnabled(self.state_xs)
 
     def on_pushButton_fitEOS(self):
+        self.ui.progress_2.setValue(33)
         self.eos = getattr(dt_potentials, self.eos_str)(*self.ipotparamsdialog.args)
 
         Vdata, Edata = self.get_EvV()
         self.Vdata = Vdata
         self.Edata = Edata
 
         initial_guess = self.get_EOS_params()
+        # print(Vdata, Edata)
         self.eos.fitEOS(Vdata, Edata, initial_parameters = initial_guess, fit=True)
 
         self.ui.lineEdit_2.setText(', '.join(['%.9e' % (p) for p in self.eos.pEOS]))
+        self.ui.progress_2.setValue(100)
+
 
     def on_pushButton_calc_nu(self):
         C = self.get_C()
         BR, BV, B, GR, GV, S, AU, nu = dt_poisson_ratio(C, quiet=True)
         self.ui.lineEdit_3.setText('%.3f'%(nu))
         self.ui.lineEdit_4.setText('%.1f'%(BR*10))
         self.ui.lineEdit_5.setText('%.1f'%(BV*10))
```

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/plot_EV.py` & `debyetools-1.4.2/debyetools/tpropsgui/plot_EV.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/plotter.py` & `debyetools-1.4.2/debyetools/tpropsgui/plotter.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/plotter_class.py` & `debyetools-1.4.2/debyetools/tpropsgui/plotter_class.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/toolbox.py` & `debyetools-1.4.2/debyetools/tpropsgui/toolbox.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/ui_dialog_doscar.py` & `debyetools-1.4.2/debyetools/tpropsgui/ui_dialog_doscar.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/ui_heatcapacitywindow.py` & `debyetools-1.4.2/debyetools/tpropsgui/ui_heatcapacitywindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
         self.retranslateUi(MainWindow)
 
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
 
     def retranslateUi(self, MainWindow):
-        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"debyetools GUI (lite) - Heat Capacity", None))
+        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"debyetools GUI - property viewer", None))
         self.label_3.setText(QCoreApplication.translate("MainWindow", u"GPa", None))
         self.lineEdit_2.setText(QCoreApplication.translate("MainWindow", u"0 30 10", None))
         self.label.setText(QCoreApplication.translate("MainWindow", u"Temperature range:", None))
         self.label_2.setText(QCoreApplication.translate("MainWindow", u"Pressure:", None))
         self.label_9.setText(QCoreApplication.translate("MainWindow", u"to:", None))
         ___qtablewidgetitem = self.tableWidget.horizontalHeaderItem(0)
         ___qtablewidgetitem.setText(QCoreApplication.translate("MainWindow", u"Values", None));
```

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/ui_interatomic_params.py` & `debyetools-1.4.2/debyetools/tpropsgui/ui_interatomic_params.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/ui_mainwindow.py` & `debyetools-1.4.2/debyetools/tpropsgui/ui_mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,23 @@
         self.frame_4 = QFrame(self.centralwidget)
         self.frame_4.setObjectName(u"frame_4")
         self.frame_4.setGeometry(QRect(10, 390, 521, 101))
         self.frame_4.setFrameShape(QFrame.Box)
         self.frame_4.setFrameShadow(QFrame.Raised)
         self.pushButton = QPushButton(self.centralwidget)
         self.pushButton.setObjectName(u"pushButton")
-        self.pushButton.setGeometry(QRect(260, 150, 80, 24))
+        self.pushButton.setGeometry(QRect(260, 140, 80, 24))
         self.label_5 = QLabel(self.centralwidget)
         self.label_5.setObjectName(u"label_5")
-        self.label_5.setGeometry(QRect(20, 150, 71, 21))
+        self.label_5.setGeometry(QRect(20, 140, 71, 21))
         self.frame_3 = QFrame(self.centralwidget)
         self.frame_3.setObjectName(u"frame_3")
         self.frame_3.setGeometry(QRect(10, 340, 521, 41))
         self.frame_3.setFrameShape(QFrame.Box)
         self.frame_3.setFrameShadow(QFrame.Raised)
-        self.radioButton_2 = QRadioButton(self.centralwidget)
-        self.radioButton_2.setObjectName(u"radioButton_2")
-        self.radioButton_2.setEnabled(False)
-        self.radioButton_2.setGeometry(QRect(360, 150, 191, 22))
-        self.radioButton_2.setChecked(True)
         self.label_2 = QLabel(self.centralwidget)
         self.label_2.setObjectName(u"label_2")
         self.label_2.setGeometry(QRect(20, 50, 31, 16))
         self.label_7 = QLabel(self.centralwidget)
         self.label_7.setObjectName(u"label_7")
         self.label_7.setGeometry(QRect(20, 200, 121, 16))
         self.lineEdit_anh = QLineEdit(self.centralwidget)
@@ -80,15 +75,15 @@
         self.lineEdit_anh.setFrame(True)
         self.pushButton_5 = QPushButton(self.centralwidget)
         self.pushButton_5.setObjectName(u"pushButton_5")
         self.pushButton_5.setEnabled(True)
         self.pushButton_5.setGeometry(QRect(450, 500, 80, 24))
         self.lineEdit_2 = QLineEdit(self.centralwidget)
         self.lineEdit_2.setObjectName(u"lineEdit_2")
-        self.lineEdit_2.setGeometry(QRect(90, 150, 161, 24))
+        self.lineEdit_2.setGeometry(QRect(90, 140, 161, 24))
         self.frame_2 = QFrame(self.centralwidget)
         self.frame_2.setObjectName(u"frame_2")
         self.frame_2.setGeometry(QRect(10, 190, 521, 141))
         self.frame_2.setFrameShape(QFrame.Box)
         self.frame_2.setFrameShadow(QFrame.Raised)
         self.pushButton_2 = QPushButton(self.frame_2)
         self.pushButton_2.setObjectName(u"pushButton_2")
@@ -211,15 +206,15 @@
         self.comboBox.addItem("")
         self.comboBox.addItem("")
         self.comboBox.addItem("")
         self.comboBox.addItem("")
         self.comboBox.addItem("")
         self.comboBox.addItem("")
         self.comboBox.setObjectName(u"comboBox")
-        self.comboBox.setGeometry(QRect(350, 150, 131, 24))
+        self.comboBox.setGeometry(QRect(350, 140, 131, 24))
         self.pushButton_3 = QPushButton(self.centralwidget)
         self.pushButton_3.setObjectName(u"pushButton_3")
         self.pushButton_3.setGeometry(QRect(330, 350, 61, 24))
         self.loaddata = QPushButton(self.centralwidget)
         self.loaddata.setObjectName(u"loaddata")
         self.loaddata.setGeometry(QRect(400, 350, 81, 24))
         self.checkBox_2 = QCheckBox(self.centralwidget)
@@ -237,25 +232,30 @@
         self.checkBox.setChecked(True)
         self.progress = QProgressBar(self.centralwidget)
         self.progress.setObjectName(u"progress")
         self.progress.setGeometry(QRect(450, 530, 81, 16))
         self.progress.setValue(0)
         self.progress.setTextVisible(False)
         self.progress.setInvertedAppearance(False)
+        self.progress_2 = QProgressBar(self.centralwidget)
+        self.progress_2.setObjectName(u"progress_2")
+        self.progress_2.setGeometry(QRect(260, 160, 81, 16))
+        self.progress_2.setValue(0)
+        self.progress_2.setTextVisible(False)
+        self.progress_2.setInvertedAppearance(False)
         MainWindow.setCentralWidget(self.centralwidget)
         self.frame_3.raise_()
         self.frame_4.raise_()
         self.frame_2.raise_()
         self.frame.raise_()
         self.lineEdit.raise_()
         self.lineEdit_xs.raise_()
         self.lineEdit_el.raise_()
         self.pushButton.raise_()
         self.label_5.raise_()
-        self.radioButton_2.raise_()
         self.label_2.raise_()
         self.label_7.raise_()
         self.lineEdit_anh.raise_()
         self.pushButton_5.raise_()
         self.lineEdit_2.raise_()
         self.label_3.raise_()
         self.label_4.raise_()
@@ -265,14 +265,15 @@
         self.pushButton_3.raise_()
         self.loaddata.raise_()
         self.checkBox_2.raise_()
         self.checkBox_3.raise_()
         self.checkBox_4.raise_()
         self.checkBox.raise_()
         self.progress.raise_()
+        self.progress_2.raise_()
         self.menubar = QMenuBar(MainWindow)
         self.menubar.setObjectName(u"menubar")
         self.menubar.setGeometry(QRect(0, 0, 536, 21))
         self.menuplot = QMenu(self.menubar)
         self.menuplot.setObjectName(u"menuplot")
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QStatusBar(MainWindow)
@@ -284,24 +285,23 @@
 
         self.retranslateUi(MainWindow)
 
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
 
     def retranslateUi(self, MainWindow):
-        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"debyetools GUI (lite)", None))
+        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"debyetools GUI", None))
         self.actionE_V.setText(QCoreApplication.translate("MainWindow", u"Exxx", None))
         self.actionasasas.setText(QCoreApplication.translate("MainWindow", u"asasas", None))
         self.actionEV.setText(QCoreApplication.translate("MainWindow", u"E(V)", None))
         self.lineEdit.setText(QCoreApplication.translate("MainWindow", u"0.02698", None))
         self.lineEdit_xs.setText(QCoreApplication.translate("MainWindow", u"0, 0, 0", None))
         self.lineEdit_el.setText(QCoreApplication.translate("MainWindow", u"0, 0, 0, 0", None))
         self.pushButton.setText(QCoreApplication.translate("MainWindow", u"fit", None))
         self.label_5.setText(QCoreApplication.translate("MainWindow", u"EOS params:", None))
-        self.radioButton_2.setText(QCoreApplication.translate("MainWindow", u"BM3", None))
         self.label_2.setText(QCoreApplication.translate("MainWindow", u"E(V):", None))
         self.label_7.setText(QCoreApplication.translate("MainWindow", u"Stiffness Tensor (GPa)", None))
         self.lineEdit_anh.setText(QCoreApplication.translate("MainWindow", u"0, 1", None))
         self.pushButton_5.setText(QCoreApplication.translate("MainWindow", u"calculate", None))
         self.lineEdit_2.setText(QCoreApplication.translate("MainWindow", u"-3e5, 1e-5, 7e10, 4", None))
         self.pushButton_2.setText(QCoreApplication.translate("MainWindow", u"re-calculate Poisson's ratio", None))
         self.label_9.setText(QCoreApplication.translate("MainWindow", u"B (Voigt):", None))
```

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/ui_warning.py` & `debyetools-1.4.2/debyetools/tpropsgui/ui_warning.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/window_cp.py` & `debyetools-1.4.2/debyetools/tpropsgui/window_cp.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/tpropsgui/window_interatomicparams.py` & `debyetools-1.4.2/debyetools/tpropsgui/window_interatomicparams.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools/vibrational.py` & `debyetools-1.4.2/debyetools/vibrational.py`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/debyetools.egg-info/PKG-INFO` & `debyetools-1.4.2/debyetools.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debyetools
-Version: 1.4.1
+Version: 1.4.2
 Summary: Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.
 Home-page: https://debyetools.readthedocs.io/
 Author: Javier Jofre
 Author-email: javier.jofre@polymtl.ca
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -20,67 +20,80 @@
 # debyetools
 
 Implementation of a tool for calculating self-consistent thermodynamic properties that can take into account all kinds of contributions to the free energy inluding explicit anharmonicity. The software presented here is based in the Debye approximation within the QHA using the crystal internal energetics parametrized at ground-state to project the thermodynamics properties at high temperatures. 
 
 Made by Javier Jofre: javier.jofre@polymtl.ca
 Please cite.
 
-### Requirements:
+### Requirements for Python module:
 - numpy
 - mpmath
 - scipy
-- PySimpleGUI
-- matplotlib
 
+### Requirements for Interface:
+For the interface it will also be necesary:
+- matplotlib
+- PySide6
 
 ### Installation
 ```
 pip install --upgrade debyetools
 ```
 
 ### Get started
 
 To start getting familiar with the interface `tProps` you can download `examples input files`.
 The GUI can be launched by executing the interface script from the debyetools repository main folder:
 
 ```
-python gui.py
+python interface.py
 ```
 
 Or you can launch  inside python:
 ```
-from debyetools.tpropsgui.gui import gui
-gui()
+from debyetools.tpropsgui.gui import interface
+interface()
 ```
 
 Debye tools can also be used as a library. Example: heat capacity of Al fcc using 3rd order Birch-Murnaghan EOS
 
 ```Python
 import numpy as np
+import debyetools.potentials as potentials
 from debyetools.ndeb import nDeb
 
-nu, m = 0.32, 0.026981500000000002
-Tmelting = 933
+# EOS parametrization
+# =========================
+EOS_parameters = [-3.607736520e+05, 9.929277050e-06, 7.729289055e+10, 4.604381753e+00]
+EOS = potentials.BM()
+EOS.fitEOS([0], [0], initial_parameters=EOS_parameters, fit=False)
 
-p_EOS = [-3.617047894e+05, 9.929931142e-06, 7.618619745e+10, 4.591924487e+00]
-p_intanh = 0, 1, p_EOS[1]
+# Other Contributions parametrization
+# =========================
 p_electronic = [3.8027342892e-01, -1.8875015171e-02, 5.3071034596e-04, -7.0100707467e-06]
-p_defects = 8.46, 1.69, Tmelting, 0.1, p_EOS[2],p_EOS[1]
-p_anh = 0,0,0
-
-EOS_name = 'BM'
-
-ndeb_BM = nDeb(nu, m, p_intanh, p_EOS, p_electronic, p_defects,p_anh,EOS_name)
-
-T,V = 9.33000000000e+02,1.07790131286e-05
-                       #
-result = ndeb_BM.eval_props(T,V)['Cp']
+mass = 0.026981500000000002
+Tmelting = 933
+p_defects = 8.46, 1.69, Tmelting, 0.1
+p_anharmonicity = 0, 1
+p_XS = 0, 0, 0
+poissonsratio = 0.37
+
+# F minimization using Slater approximaiton
+# =========================
+ndeb = nDeb(poissonsratio, mass, p_anharmonicity, EOS, p_electronic, p_defects, p_XS, mode='jjsl')
+T_initial, T_final= 0.1, 1000
+T = np.arange(T_initial, T_final, 10)
+Pressure = 0
+T, V = ndeb.min_G(T, EOS_parameters[0] * .9, P=Pressure)
+
+# Evaluation of thermodynamic properties
+# =========================
+tprops_dict = ndeb.eval_props(T, V, P=Pressure)
 ```
 
 To Do's:
 
-- Add More Examples to Documentation
 - Improve error handling
 - Add 'Compatible input files formats'
 - Improve Documentation
 - Add handling of anisotropic materials
 - Prediction of explicit anharmonicity parameters
```

### Comparing `debyetools-1.4.1/debyetools.egg-info/SOURCES.txt` & `debyetools-1.4.2/debyetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debyetools-1.4.1/setup.py` & `debyetools-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="debyetools",
-    version="1.4.1",
+    version="1.4.2",
     description="Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://debyetools.readthedocs.io/",
     author="Javier Jofre",
     author_email="javier.jofre@polymtl.ca",
     license="GPLv3",
```

