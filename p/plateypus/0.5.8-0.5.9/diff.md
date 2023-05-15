# Comparing `tmp/plateypus-0.5.8.tar.gz` & `tmp/plateypus-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plateypus-0.5.8.tar", last modified: Thu Mar 30 00:36:34 2023, max compression
+gzip compressed data, was "plateypus-0.5.9.tar", last modified: Mon May 15 18:40:31 2023, max compression
```

## Comparing `plateypus-0.5.8.tar` & `plateypus-0.5.9.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-03-30 00:36:34.012844 plateypus-0.5.8/
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    35149 2021-05-03 18:39:06.000000 plateypus-0.5.8/LICENSE.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       61 2021-05-04 23:25:56.000000 plateypus-0.5.8/MANIFEST.in
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1400 2023-03-30 00:36:34.012543 plateypus-0.5.8/PKG-INFO
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)      782 2021-12-05 01:48:37.000000 plateypus-0.5.8/README.md
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-03-30 00:36:33.984417 plateypus-0.5.8/plateypus/
--rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-05-03 16:35:22.000000 plateypus-0.5.8/plateypus/__init__.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     7119 2022-07-03 20:24:09.000000 plateypus-0.5.8/plateypus/__main__.py
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-03-30 00:36:33.997503 plateypus-0.5.8/plateypus/dataprocessing/
--rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-05-03 16:35:42.000000 plateypus-0.5.8/plateypus/dataprocessing/__init__.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    19985 2022-08-29 16:14:11.000000 plateypus-0.5.8/plateypus/dataprocessing/cellDataProcessing.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27250 2023-01-04 13:20:28.000000 plateypus-0.5.8/plateypus/dataprocessing/cytokineDataProcessing.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     9602 2023-01-21 00:10:47.000000 plateypus-0.5.8/plateypus/dataprocessing/dataProcessingGUI.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    22334 2023-02-15 15:29:55.000000 plateypus-0.5.8/plateypus/dataprocessing/initialDataProcessing.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5235 2023-01-21 00:11:19.000000 plateypus-0.5.8/plateypus/dataprocessing/killingDataProcessing.py
--rwxr-x---   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    16813 2022-07-03 19:47:33.000000 plateypus-0.5.8/plateypus/dataprocessing/miscFunctions.py
--rwxr-x---   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    24949 2022-07-03 20:35:35.000000 plateypus-0.5.8/plateypus/dataprocessing/proliferationDataProcessing.py
--rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    22340 2022-07-21 16:25:15.000000 plateypus-0.5.8/plateypus/dataprocessing/singleCellDataProcessing.py
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)   135903 2021-05-04 04:03:03.000000 plateypus-0.5.8/plateypus/plateypusLogo.png
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-03-30 00:36:34.006045 plateypus-0.5.8/plateypus/plotting/
--rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-05-03 16:35:50.000000 plateypus-0.5.8/plateypus/plotting/__init__.py
--rwxr-x---   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5431 2021-06-08 08:39:14.000000 plateypus-0.5.8/plateypus/plotting/facetPlot1D.py
--rwxr-x---   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     3277 2021-11-17 16:25:07.000000 plateypus-0.5.8/plateypus/plotting/facetPlot2D.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     8053 2022-07-03 20:15:16.000000 plateypus-0.5.8/plateypus/plotting/facetPlot3D.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    10282 2021-05-03 17:29:09.000000 plateypus-0.5.8/plateypus/plotting/facetPlotCategorical.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27471 2022-07-03 20:46:51.000000 plateypus-0.5.8/plateypus/plotting/facetPlotLibrary.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27445 2021-05-11 22:19:52.000000 plateypus-0.5.8/plateypus/plotting/interactiveGUIElements.py
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    35603 2022-07-03 20:21:52.000000 plateypus-0.5.8/plateypus/plotting/plottingGUI.py
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-03-30 00:36:34.011737 plateypus-0.5.8/plateypus/setup/
--rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-05-03 16:35:53.000000 plateypus-0.5.8/plateypus/setup/__init__.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    55094 2022-07-03 20:41:53.000000 plateypus-0.5.8/plateypus/setup/createPlateLayout.py
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     8474 2023-03-30 00:31:43.000000 plateypus-0.5.8/plateypus/setup/createTubeLayout.py
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     7537 2022-07-03 21:13:08.000000 plateypus-0.5.8/plateypus/setup/experimentCreationGUI.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    39986 2023-03-29 18:56:37.000000 plateypus-0.5.8/plateypus/setup/experimentSetupGUI.py
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1349 2022-07-03 20:45:21.000000 plateypus-0.5.8/plateypus/setup/removeExperiment.py
-drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-03-30 00:36:33.988211 plateypus-0.5.8/plateypus.egg-info/
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1400 2023-03-30 00:36:33.000000 plateypus-0.5.8/plateypus.egg-info/PKG-INFO
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1271 2023-03-30 00:36:33.000000 plateypus-0.5.8/plateypus.egg-info/SOURCES.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        1 2023-03-30 00:36:33.000000 plateypus-0.5.8/plateypus.egg-info/dependency_links.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       54 2023-03-30 00:36:33.000000 plateypus-0.5.8/plateypus.egg-info/entry_points.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       90 2023-03-30 00:36:33.000000 plateypus-0.5.8/plateypus.egg-info/requires.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       10 2023-03-30 00:36:33.000000 plateypus-0.5.8/plateypus.egg-info/top_level.txt
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)      104 2021-05-03 19:50:38.000000 plateypus-0.5.8/pyproject.toml
--rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       38 2023-03-30 00:36:34.012960 plateypus-0.5.8/setup.cfg
--rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1341 2023-03-30 00:36:19.000000 plateypus-0.5.8/setup.py
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-05-15 18:40:31.469667 plateypus-0.5.9/
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    35149 2021-05-03 18:39:06.000000 plateypus-0.5.9/LICENSE.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       61 2021-05-04 23:25:56.000000 plateypus-0.5.9/MANIFEST.in
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1400 2023-05-15 18:40:31.469371 plateypus-0.5.9/PKG-INFO
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)      782 2021-12-05 01:48:37.000000 plateypus-0.5.9/README.md
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-05-15 18:40:31.439910 plateypus-0.5.9/plateypus/
+-rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-05-03 16:35:22.000000 plateypus-0.5.9/plateypus/__init__.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     7119 2022-07-03 20:24:09.000000 plateypus-0.5.9/plateypus/__main__.py
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-05-15 18:40:31.453564 plateypus-0.5.9/plateypus/dataprocessing/
+-rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-05-03 16:35:42.000000 plateypus-0.5.9/plateypus/dataprocessing/__init__.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    19985 2022-08-29 16:14:11.000000 plateypus-0.5.9/plateypus/dataprocessing/cellDataProcessing.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27250 2023-01-04 13:20:28.000000 plateypus-0.5.9/plateypus/dataprocessing/cytokineDataProcessing.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    10334 2023-05-10 16:04:35.000000 plateypus-0.5.9/plateypus/dataprocessing/dataProcessingGUI.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    22450 2023-05-10 17:51:52.000000 plateypus-0.5.9/plateypus/dataprocessing/initialDataProcessing.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5235 2023-01-21 00:11:19.000000 plateypus-0.5.9/plateypus/dataprocessing/killingDataProcessing.py
+-rwxr-x---   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    16813 2023-05-10 15:49:07.000000 plateypus-0.5.9/plateypus/dataprocessing/miscFunctions.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5154 2023-05-10 17:51:13.000000 plateypus-0.5.9/plateypus/dataprocessing/pcrDataProcessing.py
+-rwxr-x---   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    24949 2022-07-03 20:35:35.000000 plateypus-0.5.9/plateypus/dataprocessing/proliferationDataProcessing.py
+-rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    22340 2022-07-21 16:25:15.000000 plateypus-0.5.9/plateypus/dataprocessing/singleCellDataProcessing.py
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)   135903 2021-05-04 04:03:03.000000 plateypus-0.5.9/plateypus/plateypusLogo.png
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-05-15 18:40:31.461916 plateypus-0.5.9/plateypus/plotting/
+-rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-05-03 16:35:50.000000 plateypus-0.5.9/plateypus/plotting/__init__.py
+-rwxr-x---   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     5431 2021-06-08 08:39:14.000000 plateypus-0.5.9/plateypus/plotting/facetPlot1D.py
+-rwxr-x---   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     3277 2021-11-17 16:25:07.000000 plateypus-0.5.9/plateypus/plotting/facetPlot2D.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     8053 2022-07-03 20:15:16.000000 plateypus-0.5.9/plateypus/plotting/facetPlot3D.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    10282 2021-05-03 17:29:09.000000 plateypus-0.5.9/plateypus/plotting/facetPlotCategorical.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27471 2022-07-03 20:46:51.000000 plateypus-0.5.9/plateypus/plotting/facetPlotLibrary.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    27445 2021-05-11 22:19:52.000000 plateypus-0.5.9/plateypus/plotting/interactiveGUIElements.py
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    35750 2023-05-10 22:26:42.000000 plateypus-0.5.9/plateypus/plotting/plottingGUI.py
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-05-15 18:40:31.468575 plateypus-0.5.9/plateypus/setup/
+-rwxr--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       26 2021-05-03 16:35:53.000000 plateypus-0.5.9/plateypus/setup/__init__.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    55094 2022-07-03 20:41:53.000000 plateypus-0.5.9/plateypus/setup/createPlateLayout.py
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     8474 2023-03-30 00:31:43.000000 plateypus-0.5.9/plateypus/setup/createTubeLayout.py
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     7537 2022-07-03 21:13:08.000000 plateypus-0.5.9/plateypus/setup/experimentCreationGUI.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)    39998 2023-05-10 17:46:23.000000 plateypus-0.5.9/plateypus/setup/experimentSetupGUI.py
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1349 2022-07-03 20:45:21.000000 plateypus-0.5.9/plateypus/setup/removeExperiment.py
+drwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        0 2023-05-15 18:40:31.443691 plateypus-0.5.9/plateypus.egg-info/
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1400 2023-05-15 18:40:31.000000 plateypus-0.5.9/plateypus.egg-info/PKG-INFO
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1317 2023-05-15 18:40:31.000000 plateypus-0.5.9/plateypus.egg-info/SOURCES.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)        1 2023-05-15 18:40:31.000000 plateypus-0.5.9/plateypus.egg-info/dependency_links.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       54 2023-05-15 18:40:31.000000 plateypus-0.5.9/plateypus.egg-info/entry_points.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       90 2023-05-15 18:40:31.000000 plateypus-0.5.9/plateypus.egg-info/requires.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       10 2023-05-15 18:40:31.000000 plateypus-0.5.9/plateypus.egg-info/top_level.txt
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)      104 2021-05-03 19:50:38.000000 plateypus-0.5.9/pyproject.toml
+-rw-r--r--   0 acharsr  (1061017723) NIH\Domain Users (1360859114)       38 2023-05-15 18:40:31.469787 plateypus-0.5.9/setup.cfg
+-rwxr-xr-x   0 acharsr  (1061017723) NIH\Domain Users (1360859114)     1341 2023-05-15 18:40:19.000000 plateypus-0.5.9/setup.py
```

### Comparing `plateypus-0.5.8/LICENSE.txt` & `plateypus-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/PKG-INFO` & `plateypus-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plateypus
-Version: 0.5.8
+Version: 0.5.9
 Summary: Processes and plots high throughput cytometry experiments through a GUI
 Home-page: https://github.com/soorajachar/plateypus
 Author: Sooraj Achar
 Author-email: acharsr@nih.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
```

### Comparing `plateypus-0.5.8/README.md` & `plateypus-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/__main__.py` & `plateypus-0.5.9/plateypus/__main__.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/dataprocessing/cellDataProcessing.py` & `plateypus-0.5.9/plateypus/dataprocessing/cellDataProcessing.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/dataprocessing/cytokineDataProcessing.py` & `plateypus-0.5.9/plateypus/dataprocessing/cytokineDataProcessing.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/dataprocessing/dataProcessingGUI.py` & `plateypus-0.5.9/plateypus/dataprocessing/dataProcessingGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pandas as pd
 import tkinter as tk
 from plateypus.dataprocessing import initialDataProcessing as idp
 from plateypus.dataprocessing import cytokineDataProcessing as cydp
 from plateypus.dataprocessing import cellDataProcessing as cdp
 from plateypus.dataprocessing import proliferationDataProcessing as pdp
 from plateypus.dataprocessing import killingDataProcessing as kdp
+from plateypus.dataprocessing import pcrDataProcessing as pcrdp
 from plateypus.dataprocessing import singleCellDataProcessing as scdp
 #import automatedCBAProcessingGUI as autoCBA
 import os
 if os.name == 'nt':
     dirSep = '\\'
 else:
     dirSep = '/'
@@ -38,14 +39,15 @@
         
         l2 = tk.Label(mainWindow, text="""Datatype: """,padx = 20).grid(row=0,column=0,sticky=tk.W)
         l2a = tk.Label(mainWindow, text="Cytokine:",padx = 20).grid(row=1,column=0,sticky=tk.W)
         l2b = tk.Label(mainWindow,text="Cell:",padx = 20).grid(row=2,column=0,sticky=tk.W)
         l2c = tk.Label(mainWindow,text="Proliferation:",padx = 20).grid(row=3,column=0,sticky=tk.W)
         l2e = tk.Label(mainWindow,text="Killing:",padx = 20).grid(row=4,column=0,sticky=tk.W)
         l2d = tk.Label(mainWindow,text="Single Cell:",padx = 20).grid(row=5,column=0,sticky=tk.W)
+        l2f = tk.Label(mainWindow,text="PCR:",padx = 20).grid(row=6,column=0,sticky=tk.W)
         
         def createDataFrame(dataType):
             dataProcessingMaster(folderName,expNum,dataType,ex_data,v3.get())#,v4.get())
         
         l3 = tk.Label(mainWindow, text="""Action: """).grid(row=0,column=1,sticky=tk.W)
         
         cytCalibrationParametersButton = tk.Button(mainWindow,text='Enter CBA bead calibration parameters',command=lambda: master.switch_frame(cydp.CalibrationParameterPage,folderName,expNum,ex_data,DataProcessingStartPage,bPage))
@@ -75,14 +77,17 @@
         cbWindow = tk.Frame(mainWindow)
         cbWindow.grid(row=5,column=1,sticky=tk.W)
         l3 = tk.Label(cbWindow,text='Use empty wells?').grid(row=0,column=0,sticky=tk.W)
         v3 = tk.BooleanVar(value=False)
         cb = tk.Checkbutton(cbWindow, variable=v3)
         cb.grid(row=0,column=1,sticky=tk.W)
         
+        killingDfButton = tk.Button(mainWindow,text='Create dataframe',command=lambda: createDataFrame('pcr'))
+        killingDfButton.grid(row=6,column=2,sticky=tk.W)
+        
         #rbWindow = tk.Frame(mainWindow)
         #rbWindow.grid(row=4,column=1,sticky=tk.W)
         #l4 = tk.Label(rbWindow,text='Well wrap:').grid(row=0,column=0,sticky=tk.W)
         #v4 = tk.StringVar(value=False)
         #cb = tk.Checkbutton(cbWindow, variable=v3)
         #cb.grid(row=0,column=1,sticky=tk.W)
 
@@ -135,23 +140,27 @@
         idp.saveFinalDataFrames(folderName,secondPath,expNum,dataType,celldf,ex_data) 
     elif(dataType == 'prolif'):
         prolifdf = pdp.generateBulkProliferationStatistics(folderName,expNum)
         idp.saveFinalDataFrames(folderName,secondPath,expNum,dataType,prolifdf,ex_data) 
     elif(dataType == 'killing'):
         killingdf = kdp.generateBulkKillingStatistics(experimentParameters,folderName,expNum,dataType,experimentLevelLayoutDict)
         idp.saveFinalDataFrames(folderName,secondPath,expNum,dataType,killingdf,ex_data) 
+    elif(dataType == 'pcr'):
+        pcrdp.convertPCRinput(experimentParameters,folderName,expNum,dataType,experimentLevelLayoutDict)
+        pcrdf = idp.createBaseDataFrame(experimentParameters,folderName,expNum,dataType,experimentLevelLayoutDict).droplevel(['CellType','Marker']).rename({'MFI':'Cp'})
+        idp.saveFinalDataFrames(folderName,secondPath,expNum,dataType,pcrdf,ex_data) 
         
         #Re-add parsed time values back into experiment parameter file
         #levelLabelDict = experimentParameters['levelLabelDict']
         #levelLabelDict['Time'] = list(killingDf.columns) 
         #experimentParameters['levelLabelDict'] = levelLabelDict
         #with open('misc/experimentParameters-'+folderName+'-'+dataType+'.json', 'w') as fp:
         #    json.dump(experimentParameters, fp)
 
     elif(dataType == 'singlecell'):
         dataType = 'singlecell'
         if experimentFormat == 'plate':
             scdp.createPlateSingleCellDataFrame(folderName,experimentParameters,experimentLevelLayoutDict,useBlankWells)
         else:
             scdf = scdp.createTubeSingleCellDataFrame(folderName,experimentParameters,experimentLevelLayoutDict)
-    niceDatatypeNameDict = {'cyt':'Cytokine','cell':'Bulk cell','prolif':'Proliferation','singlecell':'Single cell','killing':'Killing'}
+    niceDatatypeNameDict = {'cyt':'Cytokine','cell':'Bulk cell','prolif':'Proliferation','singlecell':'Single cell','killing':'Killing','pcr':'PCR'}
     tk.messagebox.showinfo("Dataframe Created", niceDatatypeNameDict[dataType]+" dataframe created!")
```

### Comparing `plateypus-0.5.8/plateypus/dataprocessing/initialDataProcessing.py` & `plateypus-0.5.9/plateypus/dataprocessing/initialDataProcessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     dirSep = '\\'
 else:
     dirSep = '/'
 from plateypus.dataprocessing.miscFunctions import cleanUpFlowjoCSV,reorderDfByInputOrder
 from plateypus.dataprocessing import cytokineDataProcessing,singleCellDataProcessing,cellDataProcessing
 
 dataTypeLevelNames = {'cyt':['Cytokine'],'cell':['CellType','Marker','Statistic'],'prolif':['Statistic'],'singlecell':['CellType']}
-dataTypeDataFrameFileNames = {'cyt':'cytokineConcentrationPickleFile','cell':'cellStatisticPickleFile','prolif':'proliferationStatisticPickleFile','singlecell':'initialSingleCellPickleFile','killing':'killingIndexPickleFile'}
+dataTypeDataFrameFileNames = {'cyt':'cytokineConcentrationPickleFile','cell':'cellStatisticPickleFile','prolif':'proliferationStatisticPickleFile','singlecell':'initialSingleCellPickleFile','killing':'killingIndexPickleFile','pcr':'pcrStatisticPickleFile'}
 plateRowLetters = list(string.ascii_uppercase)[:16]
 plateColumnNumbers = list(range(1,25))
 
 def returnMultiIndex(sortedData,sortedFiles,dataType,folderName):
     if(dataType == 'cyt'):
         newMultiIndex = cytokineDataProcessing.parseCytokineCSVHeaders(pd.read_csv('inputData'+dirSep+'bulkCSVFiles'+dirSep+'A1_'+dataType+'.csv').columns)
-    elif(dataType == 'cell'):
+    elif(dataType == 'cell' or dataType == 'pcr'):
         if 'antibodyPanel-'+folderName+'.csv' in os.listdir('misc'):
             panelData = pd.read_csv('misc'+dirSep+'antibodyPanel-'+folderName+'.csv',)
             newMultiIndex = cellDataProcessing.parseCellCSVHeaders(pd.read_csv('inputData'+dirSep+'bulkCSVFiles'+dirSep+'A1_'+dataType+'.csv').columns,panelData=panelData)
         else:
             newMultiIndex = cellDataProcessing.parseCellCSVHeaders(pd.read_csv('inputData'+dirSep+'bulkCSVFiles'+dirSep+'A1_'+dataType+'.csv').columns)
     elif(dataType == 'cytcorr'):
         newMultiIndex = []
@@ -261,14 +261,16 @@
                         print(name)
                 partialExperimentDf = pd.concat(timeDataList,keys=times,names=[list(levelLabelDict.keys())[-1]]).unstack(list(levelLabelDict.keys())[-1])
                 dfList.append(partialExperimentDf)
 
         fullExperimentDf = pd.concat(dfList)
     else:
         realDataType = dataType
+        if realDataType == 'pcr':
+            dataType = 'cell'
         
         #Reverse order; first decode 96 well barcoded plates, then repack the unbarcoded 96 well plates to a 384 well plate 
         if experimentParameters['overallPlateDimensions'][0] == 16 and 'unpackingDict' in list(experimentParameters.keys()):
             reverse = True
         #Normal order; first decode 384 well barcoded plates, then unpack the unbarcoded 384 well plates to 96 well plates
         else:
             reverse = False
@@ -303,15 +305,15 @@
         plateDimensions = experimentParameters['overallPlateDimensions'] 
         levels = list(levelLabelDict.keys())
         conditionLevels = list(levelLabelDict.keys())[:-1]
         conditionLevelValues = levelLabelDict.copy()
         del conditionLevelValues[list(levelLabelDict.keys())[-1]]
         allLevelValues = experimentParameters['levelLabelDict']
         
-        sortedData,sortedFiles = cleanUpFlowjoCSV(plateNames,folderName,dataType,experimentParameters)
+        sortedData,sortedFiles = cleanUpFlowjoCSV(plateNames,folderName,realDataType,experimentParameters)
         allRawData,newLevelList = returnMultiIndex(sortedData,sortedFiles,realDataType,folderName)
 
         #print(allRawData)
         dfList = []
         for rawData,plateID in zip(allRawData,plateNames):
             fullTupleList = []
             index = 0
@@ -339,15 +341,15 @@
                 columnSeries = pd.Series(rawData.values[:,column+1],index=mi)
                 columnSeriesList.append(columnSeries)
                 columnTupleList.append(tuple(columnTuple))
             #print(columnTupleList)
             #print(columnSeriesList)
             #print(rawData)
             #print(newLevelList)
-            platedf = pd.concat(columnSeriesList,axis=0,keys=columnTupleList,names=dataTypeLevelNames[realDataType])
+            platedf = pd.concat(columnSeriesList,axis=0,keys=columnTupleList,names=dataTypeLevelNames[dataType])
             dfList.append(platedf)
 
         idx=pd.IndexSlice 
         fullExperimentDf = pd.concat(dfList)
         #dfl = [fullExperimentDf.xs([12.0],level=['Time']),fullExperimentDf.xs([60.0],level=['Time']),fullExperimentDf.xs([96.0],level=['Time']),fullExperimentDf.xs([156.0],level=['Time'])]
         tempdf = fullExperimentDf.to_frame('temp')
         temp = []
```

### Comparing `plateypus-0.5.8/plateypus/dataprocessing/killingDataProcessing.py` & `plateypus-0.5.9/plateypus/dataprocessing/killingDataProcessing.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/dataprocessing/miscFunctions.py` & `plateypus-0.5.9/plateypus/dataprocessing/miscFunctions.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/dataprocessing/proliferationDataProcessing.py` & `plateypus-0.5.9/plateypus/dataprocessing/proliferationDataProcessing.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/dataprocessing/singleCellDataProcessing.py` & `plateypus-0.5.9/plateypus/dataprocessing/singleCellDataProcessing.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/plateypusLogo.png` & `plateypus-0.5.9/plateypus/plateypusLogo.png`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/plotting/facetPlot1D.py` & `plateypus-0.5.9/plateypus/plotting/facetPlot1D.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/plotting/facetPlot2D.py` & `plateypus-0.5.9/plateypus/plotting/facetPlot2D.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/plotting/facetPlot3D.py` & `plateypus-0.5.9/plateypus/plotting/facetPlot3D.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/plotting/facetPlotCategorical.py` & `plateypus-0.5.9/plateypus/plotting/facetPlotCategorical.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/plotting/facetPlotLibrary.py` & `plateypus-0.5.9/plateypus/plotting/facetPlotLibrary.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/plotting/interactiveGUIElements.py` & `plateypus-0.5.9/plateypus/plotting/interactiveGUIElements.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/plotting/plottingGUI.py` & `plateypus-0.5.9/plateypus/plotting/plottingGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     dirSep = '/'
 import plateypus.dataprocessing.initialDataProcessing as idp
 import plateypus.dataprocessing.miscFunctions as mf
 import plateypus.plotting.facetPlotLibrary as fpl 
 import plateypus.plotting.interactiveGUIElements as ipe
 
-expParamDict = {'cyt':'cyt','cell':'cell','prolif':'cell','singlecell':'cell','killing':'killing'}
+expParamDict = {'cyt':'cyt','cell':'cell','prolif':'cell','singlecell':'cell','killing':'killing','pcr':'pcr'}
 
 #Get level names and values into an easily accessible dictionary
 def createLabelDict(df):
     fulldf = df.stack()
     labelDict = {}
     for i in range(fulldf.index.nlevels):
         levelName = fulldf.index.levels[i].name
@@ -80,21 +80,23 @@
         l2 = tk.Label(mainWindow, text="""Datatype: """)
         v2 = tk.StringVar(value='cyt')
         rb2a = tk.Radiobutton(mainWindow, text="Cytokine",padx = 20, variable=v2, value='cyt')
         rb2b = tk.Radiobutton(mainWindow,text="Cell",padx = 20, variable=v2, value='cell')
         rb2c = tk.Radiobutton(mainWindow,text="Proliferation",padx = 20, variable=v2, value='prolif')
         rb2d = tk.Radiobutton(mainWindow,text="Single Cell",padx = 20, variable=v2, value='singlecell')
         rb2e = tk.Radiobutton(mainWindow,text="Killing",padx = 20, variable=v2, value='killing')
+        rb2f = tk.Radiobutton(mainWindow,text="PCR",padx = 20, variable=v2, value='pcr')
         
         l2.grid(row=0,column=0)
         rb2a.grid(row=1,column=0,sticky=tk.W)
         rb2b.grid(row=2,column=0,sticky=tk.W)
         rb2c.grid(row=3,column=0,sticky=tk.W)
         rb2d.grid(row=4,column=0,sticky=tk.W)
         rb2e.grid(row=5,column=0,sticky=tk.W)
+        rb2f.grid(row=6,column=0,sticky=tk.W)
         
         def collectInputs():
             global useModifiedDf
             modified = False 
             useModifiedDf = modified
             if modified:
                 modifiedString = '-modified'
```

### Comparing `plateypus-0.5.8/plateypus/setup/createPlateLayout.py` & `plateypus-0.5.9/plateypus/setup/createPlateLayout.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/setup/createTubeLayout.py` & `plateypus-0.5.9/plateypus/setup/createTubeLayout.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/setup/experimentCreationGUI.py` & `plateypus-0.5.9/plateypus/setup/experimentCreationGUI.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus/setup/experimentSetupGUI.py` & `plateypus-0.5.9/plateypus/setup/experimentSetupGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 if os.name == 'nt':
     dirSep = '\\'
 else:
     dirSep = '/'
 
 experimentParameters = {}
-dataTypeDict = {'Cytokine':'cyt','Bulk/Single cell':'cell','Killing':'killing'}
+dataTypeDict = {'Cytokine':'cyt','Bulk/Single cell':'cell','Killing':'killing','PCR':'pcr'}
 
 class ExperimentSetupStartPage(tk.Frame):
     def __init__(self, master,fName,bPage):
         global folderName,backPage
         folderName = fName
         backPage = bPage
         tk.Frame.__init__(self, master)
```

### Comparing `plateypus-0.5.8/plateypus/setup/removeExperiment.py` & `plateypus-0.5.9/plateypus/setup/removeExperiment.py`

 * *Files identical despite different names*

### Comparing `plateypus-0.5.8/plateypus.egg-info/PKG-INFO` & `plateypus-0.5.9/plateypus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plateypus
-Version: 0.5.8
+Version: 0.5.9
 Summary: Processes and plots high throughput cytometry experiments through a GUI
 Home-page: https://github.com/soorajachar/plateypus
 Author: Sooraj Achar
 Author-email: acharsr@nih.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
```

### Comparing `plateypus-0.5.8/plateypus.egg-info/SOURCES.txt` & `plateypus-0.5.9/plateypus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 plateypus/dataprocessing/__init__.py
 plateypus/dataprocessing/cellDataProcessing.py
 plateypus/dataprocessing/cytokineDataProcessing.py
 plateypus/dataprocessing/dataProcessingGUI.py
 plateypus/dataprocessing/initialDataProcessing.py
 plateypus/dataprocessing/killingDataProcessing.py
 plateypus/dataprocessing/miscFunctions.py
+plateypus/dataprocessing/pcrDataProcessing.py
 plateypus/dataprocessing/proliferationDataProcessing.py
 plateypus/dataprocessing/singleCellDataProcessing.py
 plateypus/plotting/__init__.py
 plateypus/plotting/facetPlot1D.py
 plateypus/plotting/facetPlot2D.py
 plateypus/plotting/facetPlot3D.py
 plateypus/plotting/facetPlotCategorical.py
```

### Comparing `plateypus-0.5.8/setup.py` & `plateypus-0.5.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="plateypus",
-    version="0.5.8",
+    version="0.5.9",
     author = "Sooraj Achar",
     author_email = "acharsr@nih.gov",
     description = "Processes and plots high throughput cytometry experiments through a GUI",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/soorajachar/plateypus",
     classifiers = classifiers,
```

