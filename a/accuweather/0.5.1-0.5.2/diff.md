# Comparing `tmp/accuweather-0.5.1.tar.gz` & `tmp/accuweather-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accuweather-0.5.1.tar", last modified: Fri Apr 14 07:26:32 2023, max compression
+gzip compressed data, was "accuweather-0.5.2.tar", last modified: Mon May 15 20:45:59 2023, max compression
```

## Comparing `accuweather-0.5.1.tar` & `accuweather-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:26:32.193588 accuweather-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-14 07:26:16.000000 accuweather-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 07:26:16.000000 accuweather-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 07:26:32.193588 accuweather-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-14 07:26:16.000000 accuweather-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:26:32.193588 accuweather-0.5.1/accuweather/
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-14 07:26:16.000000 accuweather-0.5.1/accuweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-14 07:26:16.000000 accuweather-0.5.1/accuweather/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 07:26:16.000000 accuweather-0.5.1/accuweather/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:26:16.000000 accuweather-0.5.1/accuweather/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:26:32.193588 accuweather-0.5.1/accuweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-14 07:26:16.000000 accuweather-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 07:26:16.000000 accuweather-0.5.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 07:26:16.000000 accuweather-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:26:32.193588 accuweather-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-14 07:26:16.000000 accuweather-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:45:59.142764 accuweather-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-15 20:45:48.000000 accuweather-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 20:45:48.000000 accuweather-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-15 20:45:59.142764 accuweather-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-15 20:45:48.000000 accuweather-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:45:59.142764 accuweather-0.5.2/accuweather/
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-15 20:45:48.000000 accuweather-0.5.2/accuweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-15 20:45:48.000000 accuweather-0.5.2/accuweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 20:45:48.000000 accuweather-0.5.2/accuweather/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:45:48.000000 accuweather-0.5.2/accuweather/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:45:59.142764 accuweather-0.5.2/accuweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-15 20:45:48.000000 accuweather-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 20:45:48.000000 accuweather-0.5.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 20:45:48.000000 accuweather-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:45:59.142764 accuweather-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-15 20:45:48.000000 accuweather-0.5.2/setup.py
```

### Comparing `accuweather-0.5.1/LICENSE` & `accuweather-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.1/PKG-INFO` & `accuweather-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accuweather
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python wrapper for getting weather data from AccuWeather servers.
 Home-page: https://github.com/bieniu/accuweather
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `accuweather-0.5.1/README.md` & `accuweather-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.1/accuweather/__init__.py` & `accuweather-0.5.2/accuweather/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,17 @@
             day["Ozone"].setdefault("Value")
             day["Ozone"].setdefault("Category")
 
             for item in day["AirAndPollen"]:
                 if item["Name"] == "AirQuality":
                     day[item["Type"]] = item
                 day[item["Name"]] = item
-                day[item["Name"]]["Category"] = day[item["Name"]]["Category"].lower()
+                day[item["Name"]]["Category"] = (
+                    day[item["Name"]]["Category"].split(" ")[0].lower()
+                )
                 day[item["Name"]].pop("Name")
             day.pop("AirAndPollen")
 
             for temp in TEMPERATURES:
                 day[f"{temp}Min"] = day[temp]["Minimum"]
                 day[f"{temp}Max"] = day[temp]["Maximum"]
                 day.pop(temp)
```

### Comparing `accuweather-0.5.1/accuweather/const.py` & `accuweather-0.5.2/accuweather/const.py`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.1/accuweather/exceptions.py` & `accuweather-0.5.2/accuweather/exceptions.py`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.1/accuweather.egg-info/PKG-INFO` & `accuweather-0.5.2/accuweather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accuweather
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python wrapper for getting weather data from AccuWeather servers.
 Home-page: https://github.com/bieniu/accuweather
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `accuweather-0.5.1/pyproject.toml` & `accuweather-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.1/setup.py` & `accuweather-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for accuweather."""
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.5.1"
+VERSION = "0.5.2"
 
 with open("requirements.txt", encoding="utf-8") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="accuweather",
     version=VERSION,
```

