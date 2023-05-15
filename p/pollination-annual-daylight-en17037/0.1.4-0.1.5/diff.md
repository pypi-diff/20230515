# Comparing `tmp/pollination-annual-daylight-en17037-0.1.4.tar.gz` & `tmp/pollination-annual-daylight-en17037-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-annual-daylight-en17037-0.1.4.tar", last modified: Wed Oct 26 13:04:11 2022, max compression
+gzip compressed data, was "dist/pollination-annual-daylight-en17037-0.1.5.tar", last modified: Mon May 15 14:43:20 2023, max compression
```

## Comparing `pollination-annual-daylight-en17037-0.1.4.tar` & `pollination-annual-daylight-en17037-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     5271 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/pollination/annual_daylight_en17037/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/pollination/annual_daylight_en17037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5450 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/pollination/annual_daylight_en17037/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-10-26 13:04:10.000000 pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 13:04:10.000000 pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 13:03:20.000000 pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-26 13:04:10.000000 pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-26 13:04:10.000000 pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:04:11.000000 pollination-annual-daylight-en17037-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-10-26 13:02:53.000000 pollination-annual-daylight-en17037-0.1.4/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/pollination/annual_daylight_en17037/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/pollination/annual_daylight_en17037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/pollination/annual_daylight_en17037/_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/pollination/annual_daylight_en17037/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:42:33.000000 pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:43:20.000000 pollination-annual-daylight-en17037-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-15 14:42:05.000000 pollination-annual-daylight-en17037-0.1.5/tests/validation_test.py
```

### Comparing `pollination-annual-daylight-en17037-0.1.4/.github/workflows/ci.yaml` & `pollination-annual-daylight-en17037-0.1.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.4/.github/workflows/tests.yaml` & `pollination-annual-daylight-en17037-0.1.5/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.4/LICENSE` & `pollination-annual-daylight-en17037-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.4/PKG-INFO` & `pollination-annual-daylight-en17037-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-en17037
-Version: 0.1.4
+Version: 0.1.5
 Summary: Annual daylight EN17037 recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-en17037
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_components/honeybee/png/annualrecipe.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
-Description: # annual-daylight-en17037
-        Annual daylight EN17037 simulation for European daylight standard EN17037
-        
 Keywords: honeybee,radiance,ladybug-tools,daylight,annual-daylight-en17037
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: viz
+License-File: LICENSE
+
+# annual-daylight-en17037
+Annual daylight EN17037 simulation for European daylight standard EN17037
```

### Comparing `pollination-annual-daylight-en17037-0.1.4/pollination/annual_daylight_en17037/entry.py` & `pollination-annual-daylight-en17037-0.1.5/pollination/annual_daylight_en17037/entry.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from pollination.alias.inputs.north import north_input
 from pollination.alias.inputs.radiancepar import rad_par_annual_input, \
     daylight_thresholds_input
 from pollination.alias.inputs.grid import grid_filter_input, \
     min_sensor_count_input, cpu_count
 from pollination.alias.outputs.daylight import annual_daylight_results
 
+from ._postprocess import AnnualDaylightEN17037PostProcess
+
 
 @dataclass
 class AnnualDaylightEN17037EntryPoint(DAG):
     """Annual daylight EN17037 entry point."""
 
     # inputs
     north = Inputs.float(
@@ -119,30 +121,41 @@
             self, north=north, cpu_count=cpu_count, min_sensor_count=min_sensor_count,
             radiance_parameters=radiance_parameters, grid_filter=grid_filter,
             model=model, wea=create_wea._outputs.wea
     ):
         pass
 
     @task(
-        template=AnnualDaylightEN17037Metrics,
+        template=AnnualDaylightEN17037PostProcess,
         needs=[create_daylight_hours, run_two_phase_daylight_coefficient]
     )
-    def calculate_annual_metrics_en17037(
-        self, folder='results',
-        schedule=create_daylight_hours._outputs.daylight_hours
+    def annual_metrics_en17037_postprocess(
+        self, results='results',
+        schedule=create_daylight_hours._outputs.daylight_hours,
+        thresholds=thresholds
     ):
         return [
             {
-                'from': AnnualDaylightEN17037Metrics()._outputs.annual_en17037_metrics,
+                'from': AnnualDaylightEN17037PostProcess()._outputs.en17037,
+                'to': 'en17037'
+            },
+            {
+                'from': AnnualDaylightEN17037PostProcess()._outputs.metrics,
                 'to': 'metrics'
             }
         ]
 
     results = Outputs.folder(
         source='results', description='Folder with raw result files (.ill) that '
         'contain illuminance matrices for each sensor at each timestep of the analysis.',
         alias=annual_daylight_results
     )
 
+    en17037 = Outputs.folder(
+        source='en17037', description='Annual daylight EN17037 metrics folder.'
+    )
+
     metrics = Outputs.folder(
-        source='metrics', description='Annual EN 173037 metrics folder.'
+        source='metrics', description='Annual daylight metrics folder. These '
+        'metrics are the usual annual daylight metrics with the daylight '
+        'hours occupancy schedule.'
     )
```

### Comparing `pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/PKG-INFO` & `pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-en17037
-Version: 0.1.4
+Version: 0.1.5
 Summary: Annual daylight EN17037 recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-en17037
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_components/honeybee/png/annualrecipe.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
-Description: # annual-daylight-en17037
-        Annual daylight EN17037 simulation for European daylight standard EN17037
-        
 Keywords: honeybee,radiance,ladybug-tools,daylight,annual-daylight-en17037
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: viz
+License-File: LICENSE
+
+# annual-daylight-en17037
+Annual daylight EN17037 simulation for European daylight standard EN17037
```

### Comparing `pollination-annual-daylight-en17037-0.1.4/pollination_annual_daylight_en17037.egg-info/SOURCES.txt` & `pollination-annual-daylight-en17037-0.1.5/pollination_annual_daylight_en17037.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 requirements.txt
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/tests.yaml
 pollination/annual_daylight_en17037/__init__.py
+pollination/annual_daylight_en17037/_postprocess.py
 pollination/annual_daylight_en17037/entry.py
 pollination_annual_daylight_en17037.egg-info/PKG-INFO
 pollination_annual_daylight_en17037.egg-info/SOURCES.txt
 pollination_annual_daylight_en17037.egg-info/dependency_links.txt
 pollination_annual_daylight_en17037.egg-info/not-zip-safe
 pollination_annual_daylight_en17037.egg-info/requires.txt
 pollination_annual_daylight_en17037.egg-info/top_level.txt
```

### Comparing `pollination-annual-daylight-en17037-0.1.4/setup.py` & `pollination-annual-daylight-en17037-0.1.5/setup.py`

 * *Files identical despite different names*

