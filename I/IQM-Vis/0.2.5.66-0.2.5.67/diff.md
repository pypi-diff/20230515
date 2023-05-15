# Comparing `tmp/IQM-Vis-0.2.5.66.tar.gz` & `tmp/IQM-Vis-0.2.5.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IQM-Vis-0.2.5.66.tar", last modified: Fri May 12 16:28:01 2023, max compression
+gzip compressed data, was "IQM-Vis-0.2.5.67.tar", last modified: Mon May 15 15:29:12 2023, max compression
```

## Comparing `IQM-Vis-0.2.5.66.tar` & `IQM-Vis-0.2.5.67.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.770582 IQM-Vis-0.2.5.66/IQM_Vis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.774582 IQM-Vis-0.2.5.66/IQM_Vis/UI/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/custom_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24876 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/experiment_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/style-dark.css
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/style-light.css
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24364 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/UI/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.774582 IQM-Vis-0.2.5.66/IQM_Vis/data_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/data_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/data_handlers/data_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/data_handlers/data_api_abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/IQM_Vis/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/IQM_Vis/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/images/HIQM.csv
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/images/waves1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/images/waves2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/images/waves3.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/examples/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/IQM_Vis/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/metrics/IQMs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/IQM_Vis/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/transformations/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/ui_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/IQM_Vis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/utils/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/utils/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/IQM_Vis/utils/save_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.770582 IQM-Vis-0.2.5.66/IQM_Vis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-12 16:28:01.000000 IQM-Vis-0.2.5.66/IQM_Vis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-12 16:28:01.000000 IQM-Vis-0.2.5.66/IQM_Vis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:28:01.000000 IQM-Vis-0.2.5.66/IQM_Vis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 16:28:01.000000 IQM-Vis-0.2.5.66/IQM_Vis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 16:28:01.000000 IQM-Vis-0.2.5.66/IQM_Vis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:28:01.778582 IQM-Vis-0.2.5.66/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 16:27:46.000000 IQM-Vis-0.2.5.66/tests/test_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.391760 IQM-Vis-0.2.5.67/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.379760 IQM-Vis-0.2.5.67/IQM_Vis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.383760 IQM-Vis-0.2.5.67/IQM_Vis/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/custom_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24876 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/experiment_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/style-dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/style-light.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24364 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/UI/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.387760 IQM-Vis-0.2.5.67/IQM_Vis/data_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/data_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/data_handlers/data_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/data_handlers/data_api_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.387760 IQM-Vis-0.2.5.67/IQM_Vis/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.387760 IQM-Vis-0.2.5.67/IQM_Vis/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/images/HIQM.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/images/waves1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/images/waves2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/images/waves3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/examples/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.387760 IQM-Vis-0.2.5.67/IQM_Vis/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    16346 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/metrics/IQMs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.387760 IQM-Vis-0.2.5.67/IQM_Vis/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/transformations/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/ui_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.391760 IQM-Vis-0.2.5.67/IQM_Vis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/utils/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/utils/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/IQM_Vis/utils/save_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.383760 IQM-Vis-0.2.5.67/IQM_Vis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-15 15:29:12.000000 IQM-Vis-0.2.5.67/IQM_Vis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-15 15:29:12.000000 IQM-Vis-0.2.5.67/IQM_Vis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:29:12.000000 IQM-Vis-0.2.5.67/IQM_Vis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 15:29:12.000000 IQM-Vis-0.2.5.67/IQM_Vis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 15:29:12.000000 IQM-Vis-0.2.5.67/IQM_Vis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-15 15:29:12.391760 IQM-Vis-0.2.5.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:29:12.391760 IQM-Vis-0.2.5.67/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:29:12.391760 IQM-Vis-0.2.5.67/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-15 15:28:55.000000 IQM-Vis-0.2.5.67/tests/test_inputs.py
```

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/UI/custom_widgets.py` & `IQM-Vis-0.2.5.67/IQM_Vis/UI/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/UI/experiment_mode.py` & `IQM-Vis-0.2.5.67/IQM_Vis/UI/experiment_mode.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/UI/images.py` & `IQM-Vis-0.2.5.67/IQM_Vis/UI/images.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/UI/layout.py` & `IQM-Vis-0.2.5.67/IQM_Vis/UI/layout.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/UI/main.py` & `IQM-Vis-0.2.5.67/IQM_Vis/UI/main.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/UI/threads.py` & `IQM-Vis-0.2.5.67/IQM_Vis/UI/threads.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/UI/widgets.py` & `IQM-Vis-0.2.5.67/IQM_Vis/UI/widgets.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/data_handlers/data_api.py` & `IQM-Vis-0.2.5.67/IQM_Vis/data_handlers/data_api.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/data_handlers/data_api_abstract.py` & `IQM-Vis-0.2.5.67/IQM_Vis/data_handlers/data_api_abstract.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/all.py` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/all.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/dataset.py` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/dataset.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/dists.py` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/dists.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/experiment.py` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/experiment.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/images/waves1.jpeg` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/images/waves1.jpeg`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/images/waves2.jpeg` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/images/waves2.jpeg`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/images/waves3.jpeg` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/images/waves3.jpeg`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/multiple.py` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/multiple.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/examples/simple.py` & `IQM-Vis-0.2.5.67/IQM_Vis/examples/simple.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/metrics/IQMs.py` & `IQM-Vis-0.2.5.67/IQM_Vis/metrics/IQMs.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import torch
 import torch.nn as nn
 import numpy as np
 import warnings
 
 from torchmetrics import StructuralSimilarityIndexMeasure as ssim_torch
 from torchmetrics import MultiScaleStructuralSimilarityIndexMeasure as Mssim_torch
-# from torchmetrics import PeakSignalNoiseRatio as PSNRs
+from torchmetrics import PeakSignalNoiseRatio as PSNRs
 # from torchmetrics import UniversalImageQualityIndex as UIQI
 # from torchmetrics.functional import universal_image_quality_index as UIQI
 # from torchmetrics import SpectralDistortionIndex as SDI
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity as lpips_torch
 from DISTS_pytorch import DISTS as dists_original
 from .NLPD_torch.pyramids import LaplacianPyramid
 
@@ -177,14 +177,65 @@
             ssim_full_im = torch.clip(ssim_full_im, 0, 1)
             _score = ssim_full_im.cpu().detach().numpy()
         else:
             _score = _metric(im_ref, im_comp).cpu().detach().numpy()
         _score = 1 - _score
         _metric.reset()
         return _score
+    
+
+class one_over_PSNR:
+    '''Peak signal to noise ratio - https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio
+    The score given is normalised between 0, 1 by taking 1/PSNR 
+
+    Args:
+        return_image (bool): Whether to return the image (Defaults to False which
+                             will return a scalar value)
+    '''
+
+    def __init__(self):
+        self.metric = PSNRs
+        self.device = torch.device(
+            "cuda" if torch.cuda.is_available() else "cpu")
+        self.preproccess_function = _numpy_to_torch_image
+        self.initialised = False
+
+    def __call__(self, im_ref, im_comp, **kwargs):
+        '''When an instance is called
+
+        Args:
+            im_ref (np.array): Reference image
+            im_comp (np.array): Comparison image
+            **kwargs: Arbitrary keyword arguments
+
+        Returns:
+            score (np.array): PSNR between the images
+        '''
+        _check_shapes(im_ref, im_comp)
+        se = np.square(im_ref - im_comp)
+        mse = se.mean()
+        if mse == 0:
+            return 0
+        psnr = 10 * np.log10(1/(mse))
+        return 1/psnr
+
+        # im_ref = self.preproccess_function(im_ref).to(
+        #     device=self.device, dtype=torch.float)
+        # im_comp = self.preproccess_function(im_comp).to(
+        #     device=self.device, dtype=torch.float)
+        # # set up metric
+        # if self.initialised == False:
+        #     with warnings.catch_warnings():    # we don't care about the warnings these give
+        #         warnings.simplefilter("ignore")
+        #         self._metric = self.metric()
+        #         self._metric.to(self.device)
+        # _score = self._metric(im_ref*255, im_comp*255).cpu().detach().numpy()
+        # _score = 1 - _score
+        # self._metric.reset()
+        # return _score/255
 
 class LPIPS:
     '''Learned Perceptual Image Patch Similarity between two images.
        Images must have the same dimensions.
 
     Args:
         network (str): Pretrained network to use. Choose between ‘alex’, ‘vgg’
```

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/metrics/__init__.py` & `IQM-Vis-0.2.5.67/IQM_Vis/metrics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-from .IQMs import MAE, MSE, SSIM, MS_SSIM, LPIPS, DISTS, NLPD
+from .IQMs import (MAE, 
+                   MSE, 
+                   SSIM, 
+                   MS_SSIM, 
+                   LPIPS, 
+                   DISTS, 
+                   NLPD,
+                   one_over_PSNR)
 
 def get_all_metrics():
     ''' Get all available IQMs provided by IQM_Vis '''
     all_metrics = {
         'MSE': MSE(),
-        'SSIM': SSIM(),
-        'MS_SSIM': MS_SSIM(),
+        '1-SSIM': SSIM(),
+        '1-MS_SSIM': MS_SSIM(),
+        '1/PSNR': one_over_PSNR(),
         'DISTS': DISTS(),
-        'SSIM': SSIM(),
         'LPIPS': LPIPS(),
         'NLPD': NLPD(),
         'MAE': MAE(),
     }
     return all_metrics
 
 def get_all_metric_images():
```

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/ui_wrapper.py` & `IQM-Vis-0.2.5.67/IQM_Vis/ui_wrapper.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/utils/gui_utils.py` & `IQM-Vis-0.2.5.67/IQM_Vis/utils/gui_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/utils/image_utils.py` & `IQM-Vis-0.2.5.67/IQM_Vis/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/utils/plot_utils.py` & `IQM-Vis-0.2.5.67/IQM_Vis/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis/utils/save_utils.py` & `IQM-Vis-0.2.5.67/IQM_Vis/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis.egg-info/PKG-INFO` & `IQM-Vis-0.2.5.67/IQM_Vis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IQM-Vis
-Version: 0.2.5.66
+Version: 0.2.5.67
 Summary: Extendable user interface for the assessment of transformations on image metrics.
 Author: Matt Clifford
 Author-email: matt.clifford@bristol.ac.uk
 Description-Content-Type: text/markdown
 
 | | |
 |-|-|
```

### Comparing `IQM-Vis-0.2.5.66/IQM_Vis.egg-info/SOURCES.txt` & `IQM-Vis-0.2.5.67/IQM_Vis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/PKG-INFO` & `IQM-Vis-0.2.5.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IQM-Vis
-Version: 0.2.5.66
+Version: 0.2.5.67
 Summary: Extendable user interface for the assessment of transformations on image metrics.
 Author: Matt Clifford
 Author-email: matt.clifford@bristol.ac.uk
 Description-Content-Type: text/markdown
 
 | | |
 |-|-|
```

### Comparing `IQM-Vis-0.2.5.66/README.md` & `IQM-Vis-0.2.5.67/README.md`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/setup.py` & `IQM-Vis-0.2.5.67/setup.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.66/tests/test_inputs.py` & `IQM-Vis-0.2.5.67/tests/test_inputs.py`

 * *Files identical despite different names*

