# Comparing `tmp/lifx_cli-2.4.1.tar.gz` & `tmp/lifx_cli-2.4.3.tar.gz`

## Comparing `lifx_cli-2.4.1.tar` & `lifx_cli-2.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/requirements.txt
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/src/lifx/__init__.py
--rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1762 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/src/lifx/colors.py
--rwxr-xr-x   0        0        0    10650 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     4407 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/src/lifx/lights.py
--rwxr-xr-x   0        0        0     1002 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/src/lifx/scenes.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/LICENSE
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/requirements.txt
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/src/lifx/__init__.py
+-rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/src/lifx/colors.py
+-rwxr-xr-x   0        0        0    10650 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     4407 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1002 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/src/lifx/scenes.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/LICENSE
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.4.3/PKG-INFO
```

### Comparing `lifx_cli-2.4.1/.github/workflows/pylint.yml` & `lifx_cli-2.4.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.1/.github/workflows/python-publish.yml` & `lifx_cli-2.4.3/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # separate terms of service, privacy policy, and support
 # documentation.
 
 name: Upload Python Package
 
 on:
   push:
-    branches:
-      - main
+    tags:
+      - v*.*
 
 permissions:
   contents: read
 
 jobs:
   deploy:
```

### Comparing `lifx_cli-2.4.1/src/lifx/auth.py` & `lifx_cli-2.4.3/src/lifx/auth.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.1/src/lifx/colors.py` & `lifx_cli-2.4.3/src/lifx/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,7 +40,8 @@
         saturation = response['saturation'] or 'None'
         brightness = response['brightness'] or 'None'
         kelvin = response['kelvin'] or 'None'
 
         validated_colors = [[hue, saturation, brightness, kelvin]]
 
         print(tabulate(validated_colors, headers=["Hue", "Saturation", "Brightness", "Kelvin"]))
+
```

### Comparing `lifx_cli-2.4.1/src/lifx/lifx.py` & `lifx_cli-2.4.3/src/lifx/lifx.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.1/src/lifx/lights.py` & `lifx_cli-2.4.3/src/lifx/lights.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.1/src/lifx/scenes.py` & `lifx_cli-2.4.3/src/lifx/scenes.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.1/.gitignore` & `lifx_cli-2.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.1/LICENSE` & `lifx_cli-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.1/README.md` & `lifx_cli-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.1/pyproject.toml` & `lifx_cli-2.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifx-cli"
-version = "2.4.1"
+version = "2.4.3"
 authors = [{name="Wes Henderson", email="info@necrux.com"}]
 description = "The Unofficial LIFX CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'requests',
   'tabulate',
```

### Comparing `lifx_cli-2.4.1/PKG-INFO` & `lifx_cli-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-cli
-Version: 2.4.1
+Version: 2.4.3
 Summary: The Unofficial LIFX CLI
 Project-URL: Homepage, https://github.com/necrux/lifx-cli
 Project-URL: Bug Tracker, https://github.com/necrux/lifx-cli/issues
 Author-email: Wes Henderson <info@necrux.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

