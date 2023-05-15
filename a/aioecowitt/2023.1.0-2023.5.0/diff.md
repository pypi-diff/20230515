# Comparing `tmp/aioecowitt-2023.1.0.tar.gz` & `tmp/aioecowitt-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioecowitt-2023.1.0.tar", last modified: Sun Jan 22 17:35:19 2023, max compression
+gzip compressed data, was "aioecowitt-2023.5.0.tar", last modified: Mon May 15 10:25:54 2023, max compression
```

## Comparing `aioecowitt-2023.1.0.tar` & `aioecowitt-2023.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:35:19.000918 aioecowitt-2023.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-22 17:35:19.000918 aioecowitt-2023.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:35:19.000918 aioecowitt-2023.1.0/aioecowitt/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/aioecowitt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/aioecowitt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/aioecowitt/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/aioecowitt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/aioecowitt/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/aioecowitt/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/aioecowitt/station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:35:19.000918 aioecowitt-2023.1.0/aioecowitt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-22 17:35:18.000000 aioecowitt-2023.1.0/aioecowitt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-22 17:35:18.000000 aioecowitt-2023.1.0/aioecowitt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 17:35:18.000000 aioecowitt-2023.1.0/aioecowitt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-22 17:35:18.000000 aioecowitt-2023.1.0/aioecowitt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 17:35:18.000000 aioecowitt-2023.1.0/aioecowitt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-22 17:35:18.000000 aioecowitt-2023.1.0/aioecowitt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-22 17:35:18.000000 aioecowitt-2023.1.0/aioecowitt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-01-22 17:35:19.000918 aioecowitt-2023.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-22 17:35:08.000000 aioecowitt-2023.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:25:54.909840 aioecowitt-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-15 10:25:54.909840 aioecowitt-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:25:54.909840 aioecowitt-2023.5.0/aioecowitt/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/aioecowitt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/aioecowitt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/aioecowitt/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/aioecowitt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/aioecowitt/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/aioecowitt/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/aioecowitt/station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:25:54.909840 aioecowitt-2023.5.0/aioecowitt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-15 10:25:54.000000 aioecowitt-2023.5.0/aioecowitt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-15 10:25:54.000000 aioecowitt-2023.5.0/aioecowitt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:25:54.000000 aioecowitt-2023.5.0/aioecowitt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 10:25:54.000000 aioecowitt-2023.5.0/aioecowitt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:25:54.000000 aioecowitt-2023.5.0/aioecowitt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 10:25:54.000000 aioecowitt-2023.5.0/aioecowitt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 10:25:54.000000 aioecowitt-2023.5.0/aioecowitt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-15 10:25:54.913840 aioecowitt-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-15 10:25:37.000000 aioecowitt-2023.5.0/setup.py
```

### Comparing `aioecowitt-2023.1.0/LICENSE` & `aioecowitt-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioecowitt-2023.1.0/PKG-INFO` & `aioecowitt-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioecowitt
-Version: 2023.1.0
+Version: 2023.5.0
 Summary: Python wrapper for EcoWitt Protocol
 Home-page: https://github.com/home-assistant-libs/aioecowitt
 Download-URL: https://github.com/home-assistant-libs/aioecowitt
 Author: Home Assistant Team
 Author-email: hello@home-assistant.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `aioecowitt-2023.1.0/aioecowitt/__main__.py` & `aioecowitt-2023.5.0/aioecowitt/__main__.py`

 * *Files identical despite different names*

### Comparing `aioecowitt-2023.1.0/aioecowitt/calc.py` & `aioecowitt-2023.5.0/aioecowitt/calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,24 +40,26 @@
         data["uv"] = int(data["uv"])
     if "solarradiation" in data:
         data["solarradiation"] = float(data["solarradiation"])
         data["solarradiation_lux"] = round(data["solarradiation"] / wm_lux, 1)
 
     # lightning
     if "lightning_time" in data:
-        if data["lightning_time"] is not None and data["lightning_time"] != "":
+        if data["lightning_time"]:
             data["lightning_time"] = _timestamp_to_datetime(int(data["lightning_time"]))
         else:
             data["lightning_time"] = None
     if "lightning_num" in data:
         data["lightning_num"] = int(data["lightning_num"])
     if "lightning" in data:
-        if data["lightning"] is not None and data["lightning"] != "":
+        if data["lightning"]:
             data["lightning"] = int(data["lightning"])
             data["lightning_mi"] = int(round(data["lightning"] * km_mi))
+        else:
+            data["lightning"] = None
 
     # temperatures
     if "tempf" in data:
         data["tempf"] = float(data["tempf"])
         data["tempc"] = _ftoc(data["tempf"])
     if "tempinf" in data:
         data["tempinf"] = float(data["tempinf"])
```

### Comparing `aioecowitt-2023.1.0/aioecowitt/sensor.py` & `aioecowitt-2023.5.0/aioecowitt/sensor.py`

 * *Files identical despite different names*

### Comparing `aioecowitt-2023.1.0/aioecowitt/server.py` & `aioecowitt-2023.5.0/aioecowitt/server.py`

 * *Files identical despite different names*

### Comparing `aioecowitt-2023.1.0/aioecowitt/station.py` & `aioecowitt-2023.5.0/aioecowitt/station.py`

 * *Files identical despite different names*

### Comparing `aioecowitt-2023.1.0/aioecowitt.egg-info/PKG-INFO` & `aioecowitt-2023.5.0/aioecowitt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioecowitt
-Version: 2023.1.0
+Version: 2023.5.0
 Summary: Python wrapper for EcoWitt Protocol
 Home-page: https://github.com/home-assistant-libs/aioecowitt
 Download-URL: https://github.com/home-assistant-libs/aioecowitt
 Author: Home Assistant Team
 Author-email: hello@home-assistant.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `aioecowitt-2023.1.0/setup.cfg` & `aioecowitt-2023.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aioecowitt-2023.1.0/setup.py` & `aioecowitt-2023.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for EcoWitt."""
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2023.01.0"
+VERSION = "2023.5.0"
 
 
 setup(
     name="aioecowitt",
     version=VERSION,
     url="https://github.com/home-assistant-libs/aioecowitt",
     download_url="https://github.com/home-assistant-libs/aioecowitt",
```

