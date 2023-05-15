# Comparing `tmp/pyalarmdotcomajax-0.4.9b0.tar.gz` & `tmp/pyalarmdotcomajax-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.4.9b0.tar", last modified: Sat Jan  7 05:23:36 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.0b0.tar", last modified: Mon May 15 04:47:02 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.4.9b0.tar` & `pyalarmdotcomajax-0.5.0b0.tar`

### file list

```diff
@@ -1,45 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 05:23:36.940173 pyalarmdotcomajax-0.4.9b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-01-07 05:23:36.940173 pyalarmdotcomajax-0.4.9b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 05:23:36.932173 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    40943 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 05:23:36.936173 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23689 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 05:23:36.936173 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-01-07 05:23:36.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-07 05:23:36.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 05:23:36.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-07 05:23:36.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-07 05:23:36.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-07 05:23:36.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 05:23:36.000000 pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-01-07 05:23:36.940173 pyalarmdotcomajax-0.4.9b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 05:23:36.940173 pyalarmdotcomajax-0.4.9b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 05:23:36.940173 pyalarmdotcomajax-0.4.9b0/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/tests/test_no_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-01-07 05:23:27.000000 pyalarmdotcomajax-0.4.9b0/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:47:02.281239 pyalarmdotcomajax-0.5.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-05-15 04:47:02.281239 pyalarmdotcomajax-0.5.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:47:02.265239 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    40562 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16515 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:47:02.273239 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:47:02.273239 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:47:02.277239 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/websockets/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:47:02.269239 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-05-15 04:47:02.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-15 04:47:02.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:47:02.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 04:47:02.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 04:47:02.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 04:47:02.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:47:02.000000 pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-15 04:47:02.281239 pyalarmdotcomajax-0.5.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:47:02.281239 pyalarmdotcomajax-0.5.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:47:02.281239 pyalarmdotcomajax-0.5.0b0/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-15 04:46:51.000000 pyalarmdotcomajax-0.5.0b0/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.4.9b0/LICENSE` & `pyalarmdotcomajax-0.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.4.9b0/PKG-INFO` & `pyalarmdotcomajax-0.5.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.4.9b0
+Version: 0.5.0b0
 Summary: Python Interface for Alarm.com
-Home-page: https://github.com/uvjustin/pyalarmdotcomajax
+Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
-Maintainer: Justin Wong, Elahd Bar-Shai, Kevin David
+Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
 Keywords: Alarm.com,Security System,Home Assistant
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center"><img src="https://user-images.githubusercontent.com/466460/175575400-44ab6ed5-acb4-4a8c-b2ab-8b757675e900.png" height="200px"></p>
 <h1 align="center" border="1px solid black">pyalarmdotcomajax</h1>
 <h3 align="center">Asynchronous Python Library for Accessing Alarm.com Services</h3>
 <p align="center">This is an unofficial project that is not affiliated with Alarm.com.</p>
 <p align="center"><em>Forked from Daren Lord's pyalarmdotcom.</em></p>
 <br />
 <p align="center">
   <a href="https://github.com/uvjustin"><img src="https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue" /></a>
   <a href="https://github.com/elahd"><img src="https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue" /></a>
 </p>
 <p align="center">
-  <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a>
-  <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a>
+  <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a> -->
+  <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <a href="https://results.pre-commit.ci/latest/github/pyalarmdotcom/pyalarmdotcomajax/master"><img src="https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/master.svg" /></a>
   <a href="https://pypi.org/project/pyalarmdotcomajax/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pyalarmdotcomajax"></a>
   <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
   <a href="https://github.com/PyCQA/pylint"><img src="https://img.shields.io/badge/linting-pylint-yellowgreen" /></a>
   <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax"></a>
 </p>
 
@@ -75,14 +75,15 @@
 | Sensor       | `device_subtype`                                                                                                                                                                                                                                                                                                                                                                                                                                                          | (none)                                |                                                  |
 | Locks        | `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                                           | lock, unlock                          |                                                  |
 | Garage Door  | (none)                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | open, close                           |                                                  |
 | Gate         | `supports_remote_close`                                                                                                                                                                                                                                                                                                                                                                                                                                                   | open, close                           |                                                  |
 | Image Sensor | `images`                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | peek_in                               |                                                  |
 | Light        | `brightness`                                                                                                                                                                                                                                                                                                                                                                                                                                                              | turn_on (with brightness), turn_off   | No support for RGB/W, effects, temperature, etc. |
 | Thermostat   | `temp_average`, `temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`, `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`, `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`, `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`, `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`, `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` | set_attribute                         |                                                  |
+| Water Sensor |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | (none)                                |                                                  |
 
 ### Known Sensor deviceTypes
 
 This list identifies deviceTypes used in the alarm.com API and is incomplete. Please help by submitting missing values.
 
 | deviceType | Description                            |
 | ---------- | -------------------------------------- |
@@ -185,15 +186,15 @@
 ### Open Items
 
 #### Features
 
 1. Support additional components (lights, irrigation, etc.).
 2. Support more sensor types (see list above in this README).
 3. Add `debug_info` property to `ADCController` that returns aggregate of raw JSON from all endpoints. This will allow users to export the entity model of unsupported devices to help maintainers implement support in this library.
-4. Similar to above, proactively populate `unsupported_devices` property for `ADCBaseElement` to show users device id, device name, and device type for available but unsupported devices.
+4. Similar to above, proactively populate `unsupported_device_types` property for `ADCBaseElement` to show users device id, device name, and device type for available but unsupported devices.
 5. More granular exception handling when logging in. Should report discrete error types for authentication failures due to wrong credentials, connection issues, or other.
 
 MIT License
 
 Copyright (c) 2020 Justin Wong
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,35 +1,33 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.4.9b0 Summary: Python
-Interface for Alarm.com Home-page: https://github.com/uvjustin/
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b0 Summary: Python
+Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
-46082645+uvjustin@users.noreply.github.com Maintainer: Justin Wong, Elahd Bar-
-Shai, Kevin David Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
+46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
+Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
-System,Home Assistant Classifier: Development Status :: 4 - Beta Classifier:
-Natural Language :: English Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Home Automation Requires-
-Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English Classifier: Environment :: Web
+Environment Classifier: Intended Audience :: Developers Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Home Automation
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+LICENSE
 [https://user-images.githubusercontent.com/466460/175575400-44ab6ed5-acb4-4a8c-
                             b2ab-8b757675e900.png]
                         ****** pyalarmdotcomajax ******
     **** Asynchronous Python Library for Accessing Alarm.com Services ****
      This is an unofficial project that is not affiliated with Alarm.com.
                     Forked from Daren Lord's pyalarmdotcom.
 
   [https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue]
  [https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue]
-[https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd]
-                [https://app.codacy.com/project/badge/Coverage/
-c58b00c68f9542aea1554d160997e5cd] [https://results.pre-commit.ci/badge/github/
-  pyalarmdotcom/pyalarmdotcomajax/master.svg] [PyPI] [https://img.shields.io/
-  badge/code%20style-black-000000.svg] [https://img.shields.io/badge/linting-
-                         pylint-yellowgreen] [GitHub]
+  [https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/
+master.svg] [PyPI] [https://img.shields.io/badge/code%20style-black-000000.svg]
+      [https://img.shields.io/badge/linting-pylint-yellowgreen] [GitHub]
 ## Installation / Usage To install use pip: ```bash pip install
 pyalarmdotcomajax ``` Or clone the repo: ```bash git clone https://github.com/
 uvjustin/pyalarmdotcomajax.git python setup.py install ``` ## Usage See
 `examples/basic_sensor_data.py` for a basic usage example. ## Device Support
 (Core Functions) Pyalarmdotcomajax supports core features (monitoring and using
 actions) of the device types listed below. - As of v0.2, multiples of all
 devices are supported. - All devices include the attributes: `name`, `id_`,
@@ -51,87 +49,88 @@
 temperature, etc. | | Thermostat | `temp_average`, `temp_at_tstat`,
 `step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
 `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`,
 `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`,
 `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`,
 `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`,
 `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` |
-set_attribute | | ### Known Sensor deviceTypes This list identifies deviceTypes
-used in the alarm.com API and is incomplete. Please help by submitting missing
-values. | deviceType | Description | | ---------- | ---------------------------
------------ | | 1 | Contact Sensor | | 2 | Motion Sensor | | 5 | Smoke Detector
-| | 6 | CO Detector | | 8 | Freeze Sensor | | 9 | Panic Button | | 10 | Fixed
-Panic Button | | 14 | Siren | | 19 | Glass Break Detector | | 52 | Vibration
-Contact Sensor | | 68 | Panel Image Sensor | | 69 | Mobile Phone (for Bluetooth
-Disarming) | | 83 | Panel Glass Break Sensor | | 89 | Panel Motion Sensor | ##
-Device Support (Configuration) Pyalarmdotcomajax supports changing
-configuration options for the devices listed below. ### Skybell HD ####
-Doorbell Camera | Configuration Option | Slug | Supported Values | Notes | | --
------------------------ | -------------------- | ------------------------------
------- | -------------------------- | | Indoor Chime | `indoor-chime` | `on`,
-`off` | | | Outdoor Chime | `outdoor-chime` | `off`, `low`, `medium`, `high` |
-| | LED Brightness | `led-brightness` | 0-100 | | | LED Color | `led-color` |
-`#000000` - `#FFFFFF` | Must include `#` at start. | | Motion Sensor
-Sensitivity | `motion-sensitivity` | `low`, `medium`, `high`, `very_high` | |
-## Command Line Interface The CLI is available by running `adc` from anywhere
-in your terminal. Use `adc --help`, `adc get --help`, and `adc set --help` for
-more information. ```bash usage: adc [-h] [-d] [-ver] [-v] -u USERNAME -
-p PASSWORD [-n DEVICE_NAME] [-c COOKIE | -o ONE_TIME_PASSWORD] {get,set} ...
-basic command line debug interface for alarm.com via pyalarmdotcomajax. shows
-device states in various formats. options: -h, --help show this help message
-and exit -d, --debug show pyalarmdotcomajax's debug output. -ver, --version
-show program's version number and exit -v, --verbose show verbose output. -vv
-returns base64 image data for image sensor images. -u USERNAME, --username
-USERNAME alarm.com username -p PASSWORD, --password PASSWORD alarm.com password
--n DEVICE_NAME, --device-name DEVICE_NAME registers a device with this name on
-alarm.com and requests the two-factor authentication cookie for the device. -
-c COOKIE, --cookie COOKIE two-factor authentication cookie. cannot be used with
---one-time-password! -o ONE_TIME_PASSWORD, --one-time-password
-ONE_TIME_PASSWORD provide otp code for accounts that have two-factor
-authentication enabled. if not provided here, adc will prompt user for otp.
-cannot be used with --cookie! actions: {get,set} get get data from alarm.com.
-use 'adc get --help' for parameters. set set device configuration option. use
-'adc set --help' for parameters get options: -h, --help show this help message
-and exit -x, --include-unsupported return basic data for all known unsupported
-devices. always outputs in verbose format. set options: -h, --help show this
-help message and exit -i DEVICE_ID, --device-id DEVICE_ID Numeric Alarm.com
-device identifier. -s SETTING_SLUG, --setting-slug SETTING_SLUG Identifier for
-setting. Appears in parenthesis after setting name in adc set human readable
-output. -k NEW_VALUE, --new-value NEW_VALUE New value for setting. ``` ###
-Examples 1. Get human-readable status (and device IDs) for all devices: `adc -
-u "your_username" -p "your_password" get` 2. Get raw JSON output from Alarm.com
-for all devices: `adc -v -u "your_username" -p "your_password" get` 3. Turn off
-Skybell HD indoor chime (assume Skybell device ID is 283431032-1520): `adc -
-u "your_username" -p "your_password" set -i "283431032-1520" -s "indoor-chime"
--k "off"` ## Development ### VS Code Support Structures This repository
-includes a full development environment for VS Code: 1. VS Code [dev container]
-(https://code.visualstudio.com/docs/remote/create-dev-container). Automatically
-installs extensions and Python dependencies and registers Git pre-commit
-scripts. 2. Configuration files for type checking ([mypy](http://mypy-lang.org/
-)), linting ([flake8](https://flake8.pycqa.org/en/latest/), [isort](https://
-github.com/PyCQA/isort), and [black](https://github.com/psf/black)), code
-security ([Bandit](https://bandit.readthedocs.io/en/latest/)), etc. 3. Pre-
-commit checks run all of the above when committing to Git and on demand via VS
-Code [tasks](https://code.visualstudio.com/docs/editor/tasks). ### References
-1. Some API definitions are available in the [node-alarm-dot-com repository]
-(https://github.com/node-alarm-dot-com/node-alarm-dot-com/tree/master/src/
-_models). ### Open Items #### Features 1. Support additional components
-(lights, irrigation, etc.). 2. Support more sensor types (see list above in
-this README). 3. Add `debug_info` property to `ADCController` that returns
-aggregate of raw JSON from all endpoints. This will allow users to export the
-entity model of unsupported devices to help maintainers implement support in
-this library. 4. Similar to above, proactively populate `unsupported_devices`
-property for `ADCBaseElement` to show users device id, device name, and device
-type for available but unsupported devices. 5. More granular exception handling
-when logging in. Should report discrete error types for authentication failures
-due to wrong credentials, connection issues, or other. MIT License Copyright
-(c) 2020 Justin Wong Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated documentation files
-(the "Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish, distribute,
+set_attribute | | | Water Sensor | | (none) | | ### Known Sensor deviceTypes
+This list identifies deviceTypes used in the alarm.com API and is incomplete.
+Please help by submitting missing values. | deviceType | Description | | ------
+---- | -------------------------------------- | | 1 | Contact Sensor | | 2 |
+Motion Sensor | | 5 | Smoke Detector | | 6 | CO Detector | | 8 | Freeze Sensor
+| | 9 | Panic Button | | 10 | Fixed Panic Button | | 14 | Siren | | 19 | Glass
+Break Detector | | 52 | Vibration Contact Sensor | | 68 | Panel Image Sensor |
+| 69 | Mobile Phone (for Bluetooth Disarming) | | 83 | Panel Glass Break Sensor
+| | 89 | Panel Motion Sensor | ## Device Support (Configuration)
+Pyalarmdotcomajax supports changing configuration options for the devices
+listed below. ### Skybell HD #### Doorbell Camera | Configuration Option | Slug
+| Supported Values | Notes | | ------------------------- | -------------------
+- | ------------------------------------ | -------------------------- | |
+Indoor Chime | `indoor-chime` | `on`, `off` | | | Outdoor Chime | `outdoor-
+chime` | `off`, `low`, `medium`, `high` | | | LED Brightness | `led-brightness`
+| 0-100 | | | LED Color | `led-color` | `#000000` - `#FFFFFF` | Must include
+`#` at start. | | Motion Sensor Sensitivity | `motion-sensitivity` | `low`,
+`medium`, `high`, `very_high` | | ## Command Line Interface The CLI is
+available by running `adc` from anywhere in your terminal. Use `adc --help`,
+`adc get --help`, and `adc set --help` for more information. ```bash usage: adc
+[-h] [-d] [-ver] [-v] -u USERNAME -p PASSWORD [-n DEVICE_NAME] [-c COOKIE | -
+o ONE_TIME_PASSWORD] {get,set} ... basic command line debug interface for
+alarm.com via pyalarmdotcomajax. shows device states in various formats.
+options: -h, --help show this help message and exit -d, --debug show
+pyalarmdotcomajax's debug output. -ver, --version show program's version number
+and exit -v, --verbose show verbose output. -vv returns base64 image data for
+image sensor images. -u USERNAME, --username USERNAME alarm.com username -
+p PASSWORD, --password PASSWORD alarm.com password -n DEVICE_NAME, --device-
+name DEVICE_NAME registers a device with this name on alarm.com and requests
+the two-factor authentication cookie for the device. -c COOKIE, --cookie COOKIE
+two-factor authentication cookie. cannot be used with --one-time-password! -
+o ONE_TIME_PASSWORD, --one-time-password ONE_TIME_PASSWORD provide otp code for
+accounts that have two-factor authentication enabled. if not provided here, adc
+will prompt user for otp. cannot be used with --cookie! actions: {get,set} get
+get data from alarm.com. use 'adc get --help' for parameters. set set device
+configuration option. use 'adc set --help' for parameters get options: -h, --
+help show this help message and exit -x, --include-unsupported return basic
+data for all known unsupported devices. always outputs in verbose format. set
+options: -h, --help show this help message and exit -i DEVICE_ID, --device-id
+DEVICE_ID Numeric Alarm.com device identifier. -s SETTING_SLUG, --setting-slug
+SETTING_SLUG Identifier for setting. Appears in parenthesis after setting name
+in adc set human readable output. -k NEW_VALUE, --new-value NEW_VALUE New value
+for setting. ``` ### Examples 1. Get human-readable status (and device IDs) for
+all devices: `adc -u "your_username" -p "your_password" get` 2. Get raw JSON
+output from Alarm.com for all devices: `adc -v -u "your_username" -
+p "your_password" get` 3. Turn off Skybell HD indoor chime (assume Skybell
+device ID is 283431032-1520): `adc -u "your_username" -p "your_password" set -
+i "283431032-1520" -s "indoor-chime" -k "off"` ## Development ### VS Code
+Support Structures This repository includes a full development environment for
+VS Code: 1. VS Code [dev container](https://code.visualstudio.com/docs/remote/
+create-dev-container). Automatically installs extensions and Python
+dependencies and registers Git pre-commit scripts. 2. Configuration files for
+type checking ([mypy](http://mypy-lang.org/)), linting ([flake8](https://
+flake8.pycqa.org/en/latest/), [isort](https://github.com/PyCQA/isort), and
+[black](https://github.com/psf/black)), code security ([Bandit](https://
+bandit.readthedocs.io/en/latest/)), etc. 3. Pre-commit checks run all of the
+above when committing to Git and on demand via VS Code [tasks](https://
+code.visualstudio.com/docs/editor/tasks). ### References 1. Some API
+definitions are available in the [node-alarm-dot-com repository](https://
+github.com/node-alarm-dot-com/node-alarm-dot-com/tree/master/src/_models). ###
+Open Items #### Features 1. Support additional components (lights, irrigation,
+etc.). 2. Support more sensor types (see list above in this README). 3. Add
+`debug_info` property to `ADCController` that returns aggregate of raw JSON
+from all endpoints. This will allow users to export the entity model of
+unsupported devices to help maintainers implement support in this library. 4.
+Similar to above, proactively populate `unsupported_device_types` property for
+`ADCBaseElement` to show users device id, device name, and device type for
+available but unsupported devices. 5. More granular exception handling when
+logging in. Should report discrete error types for authentication failures due
+to wrong credentials, connection issues, or other. MIT License Copyright (c)
+2020 Justin Wong Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including without
+limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
 above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
 IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
```

### Comparing `pyalarmdotcomajax-0.4.9b0/README.md` & `pyalarmdotcomajax-0.5.0b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 <p align="center"><em>Forked from Daren Lord's pyalarmdotcom.</em></p>
 <br />
 <p align="center">
   <a href="https://github.com/uvjustin"><img src="https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue" /></a>
   <a href="https://github.com/elahd"><img src="https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue" /></a>
 </p>
 <p align="center">
-  <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a>
-  <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a>
+  <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a> -->
+  <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <a href="https://results.pre-commit.ci/latest/github/pyalarmdotcom/pyalarmdotcomajax/master"><img src="https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/master.svg" /></a>
   <a href="https://pypi.org/project/pyalarmdotcomajax/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pyalarmdotcomajax"></a>
   <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
   <a href="https://github.com/PyCQA/pylint"><img src="https://img.shields.io/badge/linting-pylint-yellowgreen" /></a>
   <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax"></a>
 </p>
 
@@ -51,14 +51,15 @@
 | Sensor       | `device_subtype`                                                                                                                                                                                                                                                                                                                                                                                                                                                          | (none)                                |                                                  |
 | Locks        | `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                                           | lock, unlock                          |                                                  |
 | Garage Door  | (none)                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | open, close                           |                                                  |
 | Gate         | `supports_remote_close`                                                                                                                                                                                                                                                                                                                                                                                                                                                   | open, close                           |                                                  |
 | Image Sensor | `images`                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | peek_in                               |                                                  |
 | Light        | `brightness`                                                                                                                                                                                                                                                                                                                                                                                                                                                              | turn_on (with brightness), turn_off   | No support for RGB/W, effects, temperature, etc. |
 | Thermostat   | `temp_average`, `temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`, `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`, `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`, `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`, `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`, `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` | set_attribute                         |                                                  |
+| Water Sensor |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | (none)                                |                                                  |
 
 ### Known Sensor deviceTypes
 
 This list identifies deviceTypes used in the alarm.com API and is incomplete. Please help by submitting missing values.
 
 | deviceType | Description                            |
 | ---------- | -------------------------------------- |
@@ -161,9 +162,9 @@
 ### Open Items
 
 #### Features
 
 1. Support additional components (lights, irrigation, etc.).
 2. Support more sensor types (see list above in this README).
 3. Add `debug_info` property to `ADCController` that returns aggregate of raw JSON from all endpoints. This will allow users to export the entity model of unsupported devices to help maintainers implement support in this library.
-4. Similar to above, proactively populate `unsupported_devices` property for `ADCBaseElement` to show users device id, device name, and device type for available but unsupported devices.
+4. Similar to above, proactively populate `unsupported_device_types` property for `ADCBaseElement` to show users device id, device name, and device type for available but unsupported devices.
 5. More granular exception handling when logging in. Should report discrete error types for authentication failures due to wrong credentials, connection issues, or other.
```

#### html2text {}

```diff
@@ -3,20 +3,17 @@
                         ****** pyalarmdotcomajax ******
     **** Asynchronous Python Library for Accessing Alarm.com Services ****
      This is an unofficial project that is not affiliated with Alarm.com.
                     Forked from Daren Lord's pyalarmdotcom.
 
   [https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue]
  [https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue]
-[https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd]
-                [https://app.codacy.com/project/badge/Coverage/
-c58b00c68f9542aea1554d160997e5cd] [https://results.pre-commit.ci/badge/github/
-  pyalarmdotcom/pyalarmdotcomajax/master.svg] [PyPI] [https://img.shields.io/
-  badge/code%20style-black-000000.svg] [https://img.shields.io/badge/linting-
-                         pylint-yellowgreen] [GitHub]
+  [https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/
+master.svg] [PyPI] [https://img.shields.io/badge/code%20style-black-000000.svg]
+      [https://img.shields.io/badge/linting-pylint-yellowgreen] [GitHub]
 ## Installation / Usage To install use pip: ```bash pip install
 pyalarmdotcomajax ``` Or clone the repo: ```bash git clone https://github.com/
 uvjustin/pyalarmdotcomajax.git python setup.py install ``` ## Usage See
 `examples/basic_sensor_data.py` for a basic usage example. ## Device Support
 (Core Functions) Pyalarmdotcomajax supports core features (monitoring and using
 actions) of the device types listed below. - As of v0.2, multiples of all
 devices are supported. - All devices include the attributes: `name`, `id_`,
@@ -38,76 +35,77 @@
 temperature, etc. | | Thermostat | `temp_average`, `temp_at_tstat`,
 `step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
 `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`,
 `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`,
 `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`,
 `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`,
 `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` |
-set_attribute | | ### Known Sensor deviceTypes This list identifies deviceTypes
-used in the alarm.com API and is incomplete. Please help by submitting missing
-values. | deviceType | Description | | ---------- | ---------------------------
------------ | | 1 | Contact Sensor | | 2 | Motion Sensor | | 5 | Smoke Detector
-| | 6 | CO Detector | | 8 | Freeze Sensor | | 9 | Panic Button | | 10 | Fixed
-Panic Button | | 14 | Siren | | 19 | Glass Break Detector | | 52 | Vibration
-Contact Sensor | | 68 | Panel Image Sensor | | 69 | Mobile Phone (for Bluetooth
-Disarming) | | 83 | Panel Glass Break Sensor | | 89 | Panel Motion Sensor | ##
-Device Support (Configuration) Pyalarmdotcomajax supports changing
-configuration options for the devices listed below. ### Skybell HD ####
-Doorbell Camera | Configuration Option | Slug | Supported Values | Notes | | --
------------------------ | -------------------- | ------------------------------
------- | -------------------------- | | Indoor Chime | `indoor-chime` | `on`,
-`off` | | | Outdoor Chime | `outdoor-chime` | `off`, `low`, `medium`, `high` |
-| | LED Brightness | `led-brightness` | 0-100 | | | LED Color | `led-color` |
-`#000000` - `#FFFFFF` | Must include `#` at start. | | Motion Sensor
-Sensitivity | `motion-sensitivity` | `low`, `medium`, `high`, `very_high` | |
-## Command Line Interface The CLI is available by running `adc` from anywhere
-in your terminal. Use `adc --help`, `adc get --help`, and `adc set --help` for
-more information. ```bash usage: adc [-h] [-d] [-ver] [-v] -u USERNAME -
-p PASSWORD [-n DEVICE_NAME] [-c COOKIE | -o ONE_TIME_PASSWORD] {get,set} ...
-basic command line debug interface for alarm.com via pyalarmdotcomajax. shows
-device states in various formats. options: -h, --help show this help message
-and exit -d, --debug show pyalarmdotcomajax's debug output. -ver, --version
-show program's version number and exit -v, --verbose show verbose output. -vv
-returns base64 image data for image sensor images. -u USERNAME, --username
-USERNAME alarm.com username -p PASSWORD, --password PASSWORD alarm.com password
--n DEVICE_NAME, --device-name DEVICE_NAME registers a device with this name on
-alarm.com and requests the two-factor authentication cookie for the device. -
-c COOKIE, --cookie COOKIE two-factor authentication cookie. cannot be used with
---one-time-password! -o ONE_TIME_PASSWORD, --one-time-password
-ONE_TIME_PASSWORD provide otp code for accounts that have two-factor
-authentication enabled. if not provided here, adc will prompt user for otp.
-cannot be used with --cookie! actions: {get,set} get get data from alarm.com.
-use 'adc get --help' for parameters. set set device configuration option. use
-'adc set --help' for parameters get options: -h, --help show this help message
-and exit -x, --include-unsupported return basic data for all known unsupported
-devices. always outputs in verbose format. set options: -h, --help show this
-help message and exit -i DEVICE_ID, --device-id DEVICE_ID Numeric Alarm.com
-device identifier. -s SETTING_SLUG, --setting-slug SETTING_SLUG Identifier for
-setting. Appears in parenthesis after setting name in adc set human readable
-output. -k NEW_VALUE, --new-value NEW_VALUE New value for setting. ``` ###
-Examples 1. Get human-readable status (and device IDs) for all devices: `adc -
-u "your_username" -p "your_password" get` 2. Get raw JSON output from Alarm.com
-for all devices: `adc -v -u "your_username" -p "your_password" get` 3. Turn off
-Skybell HD indoor chime (assume Skybell device ID is 283431032-1520): `adc -
-u "your_username" -p "your_password" set -i "283431032-1520" -s "indoor-chime"
--k "off"` ## Development ### VS Code Support Structures This repository
-includes a full development environment for VS Code: 1. VS Code [dev container]
-(https://code.visualstudio.com/docs/remote/create-dev-container). Automatically
-installs extensions and Python dependencies and registers Git pre-commit
-scripts. 2. Configuration files for type checking ([mypy](http://mypy-lang.org/
-)), linting ([flake8](https://flake8.pycqa.org/en/latest/), [isort](https://
-github.com/PyCQA/isort), and [black](https://github.com/psf/black)), code
-security ([Bandit](https://bandit.readthedocs.io/en/latest/)), etc. 3. Pre-
-commit checks run all of the above when committing to Git and on demand via VS
-Code [tasks](https://code.visualstudio.com/docs/editor/tasks). ### References
-1. Some API definitions are available in the [node-alarm-dot-com repository]
-(https://github.com/node-alarm-dot-com/node-alarm-dot-com/tree/master/src/
-_models). ### Open Items #### Features 1. Support additional components
-(lights, irrigation, etc.). 2. Support more sensor types (see list above in
-this README). 3. Add `debug_info` property to `ADCController` that returns
-aggregate of raw JSON from all endpoints. This will allow users to export the
-entity model of unsupported devices to help maintainers implement support in
-this library. 4. Similar to above, proactively populate `unsupported_devices`
-property for `ADCBaseElement` to show users device id, device name, and device
-type for available but unsupported devices. 5. More granular exception handling
-when logging in. Should report discrete error types for authentication failures
-due to wrong credentials, connection issues, or other.
+set_attribute | | | Water Sensor | | (none) | | ### Known Sensor deviceTypes
+This list identifies deviceTypes used in the alarm.com API and is incomplete.
+Please help by submitting missing values. | deviceType | Description | | ------
+---- | -------------------------------------- | | 1 | Contact Sensor | | 2 |
+Motion Sensor | | 5 | Smoke Detector | | 6 | CO Detector | | 8 | Freeze Sensor
+| | 9 | Panic Button | | 10 | Fixed Panic Button | | 14 | Siren | | 19 | Glass
+Break Detector | | 52 | Vibration Contact Sensor | | 68 | Panel Image Sensor |
+| 69 | Mobile Phone (for Bluetooth Disarming) | | 83 | Panel Glass Break Sensor
+| | 89 | Panel Motion Sensor | ## Device Support (Configuration)
+Pyalarmdotcomajax supports changing configuration options for the devices
+listed below. ### Skybell HD #### Doorbell Camera | Configuration Option | Slug
+| Supported Values | Notes | | ------------------------- | -------------------
+- | ------------------------------------ | -------------------------- | |
+Indoor Chime | `indoor-chime` | `on`, `off` | | | Outdoor Chime | `outdoor-
+chime` | `off`, `low`, `medium`, `high` | | | LED Brightness | `led-brightness`
+| 0-100 | | | LED Color | `led-color` | `#000000` - `#FFFFFF` | Must include
+`#` at start. | | Motion Sensor Sensitivity | `motion-sensitivity` | `low`,
+`medium`, `high`, `very_high` | | ## Command Line Interface The CLI is
+available by running `adc` from anywhere in your terminal. Use `adc --help`,
+`adc get --help`, and `adc set --help` for more information. ```bash usage: adc
+[-h] [-d] [-ver] [-v] -u USERNAME -p PASSWORD [-n DEVICE_NAME] [-c COOKIE | -
+o ONE_TIME_PASSWORD] {get,set} ... basic command line debug interface for
+alarm.com via pyalarmdotcomajax. shows device states in various formats.
+options: -h, --help show this help message and exit -d, --debug show
+pyalarmdotcomajax's debug output. -ver, --version show program's version number
+and exit -v, --verbose show verbose output. -vv returns base64 image data for
+image sensor images. -u USERNAME, --username USERNAME alarm.com username -
+p PASSWORD, --password PASSWORD alarm.com password -n DEVICE_NAME, --device-
+name DEVICE_NAME registers a device with this name on alarm.com and requests
+the two-factor authentication cookie for the device. -c COOKIE, --cookie COOKIE
+two-factor authentication cookie. cannot be used with --one-time-password! -
+o ONE_TIME_PASSWORD, --one-time-password ONE_TIME_PASSWORD provide otp code for
+accounts that have two-factor authentication enabled. if not provided here, adc
+will prompt user for otp. cannot be used with --cookie! actions: {get,set} get
+get data from alarm.com. use 'adc get --help' for parameters. set set device
+configuration option. use 'adc set --help' for parameters get options: -h, --
+help show this help message and exit -x, --include-unsupported return basic
+data for all known unsupported devices. always outputs in verbose format. set
+options: -h, --help show this help message and exit -i DEVICE_ID, --device-id
+DEVICE_ID Numeric Alarm.com device identifier. -s SETTING_SLUG, --setting-slug
+SETTING_SLUG Identifier for setting. Appears in parenthesis after setting name
+in adc set human readable output. -k NEW_VALUE, --new-value NEW_VALUE New value
+for setting. ``` ### Examples 1. Get human-readable status (and device IDs) for
+all devices: `adc -u "your_username" -p "your_password" get` 2. Get raw JSON
+output from Alarm.com for all devices: `adc -v -u "your_username" -
+p "your_password" get` 3. Turn off Skybell HD indoor chime (assume Skybell
+device ID is 283431032-1520): `adc -u "your_username" -p "your_password" set -
+i "283431032-1520" -s "indoor-chime" -k "off"` ## Development ### VS Code
+Support Structures This repository includes a full development environment for
+VS Code: 1. VS Code [dev container](https://code.visualstudio.com/docs/remote/
+create-dev-container). Automatically installs extensions and Python
+dependencies and registers Git pre-commit scripts. 2. Configuration files for
+type checking ([mypy](http://mypy-lang.org/)), linting ([flake8](https://
+flake8.pycqa.org/en/latest/), [isort](https://github.com/PyCQA/isort), and
+[black](https://github.com/psf/black)), code security ([Bandit](https://
+bandit.readthedocs.io/en/latest/)), etc. 3. Pre-commit checks run all of the
+above when committing to Git and on demand via VS Code [tasks](https://
+code.visualstudio.com/docs/editor/tasks). ### References 1. Some API
+definitions are available in the [node-alarm-dot-com repository](https://
+github.com/node-alarm-dot-com/node-alarm-dot-com/tree/master/src/_models). ###
+Open Items #### Features 1. Support additional components (lights, irrigation,
+etc.). 2. Support more sensor types (see list above in this README). 3. Add
+`debug_info` property to `ADCController` that returns aggregate of raw JSON
+from all endpoints. This will allow users to export the entity model of
+unsupported devices to help maintainers implement support in this library. 4.
+Similar to above, proactively populate `unsupported_device_types` property for
+`ADCBaseElement` to show users device id, device name, and device type for
+available but unsupported devices. 5. More granular exception handling when
+logging in. Should report discrete error types for authentication failures due
+to wrong credentials, connection issues, or other.
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,72 @@
 """Alarmdotcom API Controller."""
 from __future__ import annotations
 
 import asyncio
-from enum import Enum
+import contextlib
 import json
 import logging
 import re
+from collections.abc import Awaitable
+from datetime import datetime
+from enum import Enum
+from typing import TypedDict
 
 import aiohttp
-from aiohttp.client_exceptions import ContentTypeError
 from bs4 import BeautifulSoup
 
-from pyalarmdotcomajax.helpers import slug_to_title
+from pyalarmdotcomajax.devices.partition import Partition
+from pyalarmdotcomajax.devices.registry import AllDevices_t
+from pyalarmdotcomajax.websockets.client import WebSocketClient
 
 from . import const as c
 from .devices import (
-    DEVICE_URLS,
     BaseDevice,
-    DeviceType,
-    ElementSpecificData,
+    DeviceTypeSpecificData,
     TroubleCondition,
 )
-from .devices.camera import Camera
-from .devices.garage_door import GarageDoor
-from .devices.gate import Gate
-from .devices.image_sensor import ImageSensor
-from .devices.light import Light
-from .devices.lock import Lock
-from .devices.partition import Partition
-from .devices.sensor import Sensor
-from .devices.system import System
-from .devices.thermostat import Thermostat
+from .devices.registry import AttributeRegistry, DeviceRegistry, DeviceType
 from .errors import (
     AuthenticationFailed,
-    BadAccount,
     DataFetchFailed,
     NagScreen,
+    TryAgain,
     UnexpectedDataStructure,
     UnsupportedDevice,
 )
 from .extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOption,
+    ControllerExtensions_t,
     ExtendedProperties,
 )
 
-__version__ = "0.4.9-beta"
+# TODO: Use error handler and exception handlers in _async_get_system_devices on other request functions.
+# TODO: Fix get raw server response function.
 
-log = logging.getLogger(__name__)
+__version__ = "0.5.0-beta"
 
-# Map DeviceType enum to device class.
-DEVICE_CLASSES: dict = {
-    DeviceType.CAMERA: Camera,
-    DeviceType.GARAGE_DOOR: GarageDoor,
-    DeviceType.GATE: Gate,
-    DeviceType.IMAGE_SENSOR: ImageSensor,
-    DeviceType.LIGHT: Light,
-    DeviceType.LOCK: Lock,
-    DeviceType.PARTITION: Partition,
-    DeviceType.SENSOR: Sensor,
-    DeviceType.SYSTEM: System,
-    DeviceType.THERMOSTAT: Thermostat,
-}
+log = logging.getLogger(__name__)
 
 
 class AuthResult(Enum):
     """Standard for reporting results of login attempt."""
 
     SUCCESS = "success"
     OTP_REQUIRED = "otp_required"
     ENABLE_TWO_FACTOR = "enable_two_factor"
 
 
+class ExtensionResults(TypedDict):
+    """Results of multi-device extension calls."""
+
+    settings: dict[str, ConfigurationOption]
+    controller: ControllerExtensions_t
+
+
 class OtpType(Enum):
     """Alarm.com two factor authentication type."""
 
     # https://www.alarm.com/web/system/assets/customer-ember/enums/TwoFactorAuthenticationType.js
 
     DISABLED = 0
     APP = 1
@@ -87,28 +78,38 @@
     """Base class for communicating with Alarm.com via API."""
 
     AJAX_HEADERS_TEMPLATE = {
         "Accept": "application/vnd.api+json",
         "ajaxrequestuniquekey": None,
     }
 
+    ALL_DEVICES_URL_TEMPLATE = (  # Substitute with base url and system ID.
+        "{}web/api/settings/manageDevices/deviceCatalogs/{}"
+    )
+    ALL_SYSTEMS_URL_TEMPLATE = "{}web/api/systems/availableSystemItems?searchString="
+    ALL_RECENT_IMAGES_TEMPLATE = "{}web/api/imageSensor/imageSensorImages/getRecentImages"
+
     # LOGIN & SESSION: BEGIN
     LOGIN_TWO_FACTOR_COOKIE_NAME = "twoFactorAuthenticationId"
     LOGIN_USERNAME_FIELD = "ctl00$ContentPlaceHolder1$loginform$txtUserName"
-    LOGIN_PASSWORD_FIELD = "txtPassword"  # nosec
+    LOGIN_PASSWORD_FIELD = "txtPassword"  # noqa: S105
 
     LOGIN_URL = "https://www.alarm.com/login"
     LOGIN_POST_URL = "https://www.alarm.com/web/Default.aspx"
-    LOGIN_2FA_POST_URL_TEMPLATE = "{}web/api/twoFactorAuthentication/twoFactorAuthentications/{}/verifyTwoFactorCode"
-    LOGIN_2FA_DETAIL_URL_TEMPLATE = (
-        "{}web/api/twoFactorAuthentication/twoFactorAuthentications/{}"
+    LOGIN_2FA_POST_URL_TEMPLATE = (
+        "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/verifyTwoFactorCode"
     )
-    LOGIN_2FA_TRUST_URL_TEMPLATE = "{}web/api/twoFactorAuthentication/twoFactorAuthentications/{}/trustTwoFactorDevice"
-    LOGIN_2FA_REQUEST_OTP_SMS_URL_TEMPLATE = "{}web/api/twoFactorAuthentication/twoFactorAuthentications/{}/sendTwoFactorAuthenticationCode"
-    LOGIN_2FA_REQUEST_OTP_EMAIL_URL_TEMPLATE = "{}web/api/twoFactorAuthentication/twoFactorAuthentications/{}/sendTwoFactorAuthenticationCodeViaEmail"
+    LOGIN_2FA_DETAIL_URL_TEMPLATE = "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}"
+    LOGIN_2FA_TRUST_URL_TEMPLATE = (
+        "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/trustTwoFactorDevice"
+    )
+    LOGIN_2FA_REQUEST_OTP_SMS_URL_TEMPLATE = (
+        "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/sendTwoFactorAuthenticationCode"
+    )
+    LOGIN_2FA_REQUEST_OTP_EMAIL_URL_TEMPLATE = "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/sendTwoFactorAuthenticationCodeViaEmail"
 
     VIEWSTATE_FIELD = "__VIEWSTATE"
     VIEWSTATEGENERATOR_FIELD = "__VIEWSTATEGENERATOR"
     EVENTVALIDATION_FIELD = "__EVENTVALIDATION"
     PREVIOUSPAGE_FIELD = "__PREVIOUSPAGE"
 
     KEEP_ALIVE_CHECK_URL_TEMPLATE = "{}web/KeepAlive.aspx?timestamp={}"
@@ -118,52 +119,57 @@
 
     def __init__(
         self,
         username: str,
         password: str,
         websession: aiohttp.ClientSession,
         twofactorcookie: str | None = None,
+        notify_on_update_callback: Awaitable | None = None,
     ):
         """Manage access to Alarm.com API and builds devices."""
 
         #
         # SET
         #
         self._username: str = username
         self._password: str = password
         self._websession: aiohttp.ClientSession = websession
-        self._two_factor_cookie: dict = (
-            {"twoFactorAuthenticationId": twofactorcookie} if twofactorcookie else {}
-        )
+        self._two_factor_cookie: dict = {"twoFactorAuthenticationId": twofactorcookie} if twofactorcookie else {}
 
         #
         # INITIALIZE
         #
+
         self._factor_type_id: int | None = None
         self._two_factor_method: OtpType | None = None
         self._provider_name: str | None = None
         self._user_id: str | None = None
         self._user_email: str | None = None
+        self._active_system_id: str | None = None
         self._ajax_headers: dict = self.AJAX_HEADERS_TEMPLATE
+        self.notify_on_update_callback: Awaitable | None = notify_on_update_callback
 
-        # Individual devices don't list their associated partitions. This map is used to retrieve partition id when each device is created.
-        self._partition_map: dict = {}
+        self._partition_map: dict = (
+            {}
+        )  # Individual devices don't list their associated partitions. This map is used to retrieve partition id when each device is created.
+
+        self._installed_device_types: set[DeviceType] = (
+            set()
+        )  # List of device types that are present in a user's environment. We'll use this to cut down on the number of API calls made.
 
         self._trouble_conditions: dict = {}
 
-        self.systems: list[System] = []
-        self.partitions: list[Partition] = []
-        self.sensors: list[Sensor] = []
-        self.locks: list[Lock] = []
-        self.garage_doors: list[GarageDoor] = []
-        self.gates: list[Gate] = []
-        self.image_sensors: list[ImageSensor] = []
-        self.lights: list[Light] = []
-        self.cameras: list[Camera] = []
-        self.thermostats: list[Thermostat] = []
+        self.devices: DeviceRegistry = DeviceRegistry()
+
+        #
+        # CLI ATTRIBUTES
+        #
+        self.raw_catalog: dict = {}
+        self.raw_image_sensors: dict = {}
+        self.raw_recent_images: dict = {}
 
     #
     #
     ##############
     # PROPERTIES #
     ##############
     #
@@ -186,17 +192,15 @@
 
     @property
     def two_factor_cookie(self) -> str | None:
         """Return two factor cookie."""
         return (
             cookie
             if isinstance(self._two_factor_cookie, dict)
-            and (
-                cookie := self._two_factor_cookie.get(self.LOGIN_TWO_FACTOR_COOKIE_NAME)
-            )
+            and (cookie := self._two_factor_cookie.get(self.LOGIN_TWO_FACTOR_COOKIE_NAME))
             else None
         )
 
     #
     #
     ####################
     # PUBLIC FUNCTIONS #
@@ -204,14 +208,16 @@
     #
     #
 
     async def async_login(self, request_otp: bool = True) -> AuthResult:
         """Login to Alarm.com."""
         log.debug("Attempting to log in to Alarm.com")
 
+        # TODO: Prevent login from making a ton of saved devices in ADC.
+
         try:
             await self._async_login_and_get_key()
             await self._async_get_identity_info()
 
             if not self._two_factor_cookie and await self._async_requires_2fa():
                 log.debug("Two factor authentication code or cookie required.")
 
@@ -253,19 +259,16 @@
 
         except (asyncio.TimeoutError, aiohttp.ClientError) as err:
             log.error("Can not load 2FA submission page from Alarm.com")
             raise DataFetchFailed from err
 
         return None
 
-    async def async_submit_otp(
-        self, code: str, device_name: str | None = None
-    ) -> str | None:
-        """
-        Submit two factor authentication code.
+    async def async_submit_otp(self, code: str, device_name: str | None = None) -> str | None:
+        """Submit two factor authentication code.
 
         Register device and return 2FA code if device_name is not None.
         """
 
         # Submit code
         try:
             log.debug("Submitting OTP code...")
@@ -302,502 +305,531 @@
 
         # Submit device name for "remember me" function.
         if json_rsp.get("value", {}).get("deviceName"):
             try:
                 log.debug("Registering device...")
 
                 async with self._websession.post(
-                    url=self.LOGIN_2FA_TRUST_URL_TEMPLATE.format(
-                        c.URL_BASE, self._user_id
-                    ),
+                    url=self.LOGIN_2FA_TRUST_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
                     headers=self._ajax_headers,
                     json={"deviceName": device_name},
                 ) as resp:
                     json_rsp = await resp.json()
             except (asyncio.TimeoutError, aiohttp.ClientError) as err:
                 log.error("Can not load device trust page from Alarm.com")
                 raise DataFetchFailed from err
 
             log.debug("Registered device.")
 
         # Save 2FA cookie value.
         for cookie in self._websession.cookie_jar:
             if cookie.key == self.LOGIN_TWO_FACTOR_COOKIE_NAME:
                 log.debug("Found two-factor authentication cookie: %s", cookie.value)
-                self._two_factor_cookie = (
-                    {"twoFactorAuthenticationId": cookie.value} if cookie.value else {}
-                )
+                self._two_factor_cookie = {"twoFactorAuthenticationId": cookie.value} if cookie.value else {}
                 return str(cookie.value)
 
         log.error("Failed to find two-factor authentication cookie.")
         return None
 
-    async def async_update(self, device_type: DeviceType | None = None) -> None:
+    async def async_update(self) -> None:  # noqa: C901
         """Fetch latest device data."""
 
         log.debug("Calling update on Alarm.com")
 
-        try:
+        has_image_sensors: bool = False
+
+        if not self._active_system_id:
+            self._active_system_id = await self._async_get_active_system()
+            has_image_sensors = await self._async_has_image_sensors(self._active_system_id)
+
+        with contextlib.suppress(DataFetchFailed, UnexpectedDataStructure):
             await self._async_get_trouble_conditions()
 
-            device_types: list[DeviceType] = (
-                [DeviceType.SYSTEM, device_type]
-                if device_type
-                else list(DEVICE_URLS["supported"].keys())
+        #
+        # GET CORE DEVICE ATTRIBUTES
+        #
+
+        device_instances: dict[str, AllDevices_t] = {}
+        raw_devices: list[dict] = await self._async_get_system_devices(self._active_system_id)
+
+        #
+        # QUERY MULTI-DEVICE EXTENSIONS
+        #
+
+        extension_results = await self._async_update__query_multi_device_extensions(raw_devices)
+
+        #
+        # QUERY IMAGE SENSORS
+        #
+        # Detailed image sensors data is not included in the main device catalog. It must be queried separately.
+        #
+        # TODO: Convert image sensors images to device extension. Merge entity_specific_data and settings; eliminate "additional endpoints" concept. Maybe push processing/placement into specific device class.
+
+        device_type_specific_data = {}
+
+        if has_image_sensors:
+            # Get detailed image sensor data and add to raw device list.
+            image_sensors = await self._async_get_devices_by_device_type(DeviceType.IMAGE_SENSOR)
+            raw_devices.extend(image_sensors)
+
+            # Get recent images
+            device_type_specific_data = await self._async_get_recent_images()
+
+        #
+        # BUILD PARTITIONS
+        #
+        # Ensures that partition map is built before devices are built.
+
+        for device in [
+            device
+            for device in raw_devices
+            if device["type"] == AttributeRegistry.get_relationship_id_from_devicetype(DeviceType.PARTITION)
+        ]:
+            partition_instance: AllDevices_t = await self._async_update__build_device(
+                device, device_type_specific_data, extension_results
             )
 
-            await self._async_get_and_build_devices(device_types)
+            for child, _ in partition_instance.children:
+                self._partition_map[child] = partition_instance.id_
 
-        except (PermissionError, UnexpectedDataStructure) as err:
-            raise err
+            device_instances.update({partition_instance.id_: partition_instance})
+
+            raw_devices.remove(device)
+
+            #
+            # BUILD ALL DEVICES IN PARTITION
+            #
+            # This ensures that partition map is built before devices are built.
+
+            for device in raw_devices:
+                try:
+                    device_instance: AllDevices_t = await self._async_update__build_device(
+                        device, device_type_specific_data, extension_results
+                    )
+
+                    device_instances.update({device_instance.id_: device_instance})
+
+                except UnsupportedDevice:
+                    continue
+
+        self.devices.update(device_instances, purge=True)
+
+    async def _async_update__build_device(
+        self,
+        raw_device: dict,
+        device_type_specific_data: dict[str, DeviceTypeSpecificData],
+        extension_results: dict[str, ExtensionResults],
+    ) -> AllDevices_t:
+        """Build device instance."""
+
+        #
+        # DETERMINE DEVICE'S PYALARMDOTCOMAJAX PYTHON CLASS & DEVICETYPE
+        #
+        device_type: DeviceType = AttributeRegistry.get_devicetype_from_relationship_id(raw_device["type"])
+        device_class: type[AllDevices_t] = AttributeRegistry.get_class(device_type)
+
+        #
+        # SKIP UNSUPPORTED DEVICE TYPES
+        #
+        # There is a hack here for cameras. We don't really support cameras (no images / streaming), we only support settings for the Skybell HD.
+        if not AttributeRegistry.is_supported(device_type) or (
+            (device_type == DeviceType.CAMERA)
+            and (raw_device.get("attributes", {}).get("deviceModel") != "SKYBELLHD")
+        ):
+            raise UnsupportedDevice(f"Unsupported device type: {device_type}")
+
+        children: list[tuple[str, DeviceType]] = []
+
+        # Get child elements for partitions and systems if function called using a device_type.
+        if device_type in [DeviceType.PARTITION, DeviceType.SYSTEM]:
+            for family_name, family_data in raw_device["relationships"].items():
+                if DeviceType.has_value(family_name):
+                    for sub_device in family_data["data"]:
+                        children.append((sub_device["id"], DeviceType(family_name)))
+
+        #
+        # BUILD DEVICE INSTANCE
+        #
+
+        device_extension_results: ExtensionResults | dict = extension_results.get(
+            entity_id := raw_device["id"], {}
+        )
+
+        device_instance = device_class(
+            id_=entity_id,
+            raw_device_data=raw_device,
+            children=children,
+            device_type_specific_data=device_type_specific_data.get(entity_id),
+            send_action_callback=self.async_send_command,
+            config_change_callback=(
+                extension_controller.submit_change
+                if (extension_controller := device_extension_results.get("controller"))
+                else None
+            ),
+            trouble_conditions=self._trouble_conditions.get(entity_id),
+            partition_id=self._partition_map.get(entity_id),
+            settings=device_extension_results.get("settings"),
+        )
+
+        return device_instance
+
+    async def _async_update__query_multi_device_extensions(
+        self, raw_devices: list[dict]
+    ) -> dict[str, ExtensionResults]:
+        """Query device extensions that request data for multiple devices at once.
+
+        Args:
+            raw_devices: A list of devices to query.
+
+        Returns:
+            A dict containing a dictionary with the device id, device extensions, and a
+            ControllerExtensions_t object.
+
+        """
+
+        required_extensions: list[type[ControllerExtensions_t]] = []
+        name_id_map: dict[str, str] = {}
+
+        #
+        # Check whether any devices have extensions.
+        #
+
+        for raw_device in raw_devices:
+            device_type: DeviceType = AttributeRegistry.get_devicetype_from_relationship_id(raw_device["type"])
+
+            #
+            # Camera Skybell HD Extension
+            # Skybell HD extension pulls data for all cameras at once.
+            #
+            if device_type == DeviceType.CAMERA:
+                if raw_device.get("attributes", {}).get("deviceModel") == "SKYBELLHD":
+                    required_extensions.append(CameraSkybellControllerExtension)
+                    # Stop searching at the first hit since once we have a Skybell, we know that we need to query the extension.
+                    break
+
+        if not required_extensions:
+            return {}
+
+        #
+        # Build map of device names -> device ids.
+        #
+
+        for raw_device in raw_devices:
+            if name := raw_device.get("attributes", {}).get("description"):
+                name_id_map[name] = raw_device["id"]
+
+        #
+        # Retrieve data for extensions
+        #
+
+        results: dict[str, ExtensionResults] = {}
+
+        for extension_t in required_extensions:
+            extension_controller = extension_t(
+                websession=self._websession,
+                headers=self._ajax_headers,
+            )
+
+            try:
+                # Fetch from Alarm.com
+                extended_properties_by_device: list[ExtendedProperties] = await extension_controller.fetch()
+            except UnexpectedDataStructure:
+                continue
+
+            # Match extended properties to devices by name, then add to storage.
+
+            for device_properties in extended_properties_by_device:
+                if (device_name := device_properties.device_name) in name_id_map:
+                    device_id = name_id_map[device_name]
+                    results[device_id] = {
+                        "settings": device_properties.settings,
+                        "controller": extension_controller,
+                    }
+
+        return results
 
     async def async_send_command(
         self,
         device_type: DeviceType,
-        event: Lock.Command
-        | Partition.Command
-        | GarageDoor.Command
-        | Gate.Command
-        | Light.Command
-        | ImageSensor.Command
-        | Thermostat.Command,
+        event: BaseDevice.Command,
         device_id: str | None = None,  # ID corresponds to device_type
-        msg_body: dict | None = None,  # Body of request. No abstractions here.
+        msg_body: dict = {},  # Body of request. No abstractions here.
         retry_on_failure: bool = True,  # Set to prevent infinite loops when function calls itself
     ) -> bool:
         """Send commands to Alarm.com."""
-        log.debug("Sending %s to Alarm.com.", event)
-
-        if not msg_body:
-            msg_body = {}
+        log.info("Sending %s to Alarm.com.", event)
 
         msg_body["statePollOnly"] = False
 
-        url = (
-            f"{DEVICE_URLS['supported'][device_type]['endpoint'].format(c.URL_BASE, device_id)}/{event.value}"
-        )
+        try:
+            url = (
+                f"{AttributeRegistry.get_endpoints(device_type)['primary'].format(c.URL_BASE, device_id)}/{event.value}"
+            )
+        except KeyError as err:
+            raise UnsupportedDevice from err
+
         log.debug("Url %s", url)
 
-        async with self._websession.post(
-            url=url, json=msg_body, headers=self._ajax_headers
-        ) as resp:
+        async with self._websession.post(url=url, json=msg_body, headers=self._ajax_headers) as resp:
             log.debug("Response from Alarm.com %s", resp.status)
-            if resp.status == 200:
-                # Update alarm.com status after calling state change.
-                await self.async_update(device_type)
-                return True
-            if resp.status == 423:
-                # User has read-only permission to the entity.
-                err_msg = (
-                    f"{__name__}: User {self.user_email} has read-only access to"
-                    f" {device_type.name.lower()} {device_id}."
-                )
-                raise PermissionError(err_msg)
-            if (
-                (resp.status == 422)
-                and isinstance(event, Partition.Command)
-                and (msg_body.get("forceBypass") is True)
-            ):
-                # 422 sometimes occurs when forceBypass is True but there's nothing to bypass.
-                log.debug(
-                    "Error executing %s, trying again without force bypass...",
-                    event.value,
-                )
 
-                # Not changing retry_on_failure. Changing forcebypass means that we won't re-enter this block.
+            match str(resp.status):
+                case "200":
+                    # Update entities after calling state change.
+                    # TODO: Confirm that we can remove this call because of webhook support.
+                    # await self.async_update()
+                    return True
+
+                case "423":
+                    # User has read-only permission to the entity.
+                    err_msg = (
+                        f"{__name__}: User {self.user_email} has read-only access to"
+                        f" {device_type.name.lower()} {device_id}."
+                    )
+                    raise PermissionError(err_msg)
 
-                msg_body["forceBypass"] = False
+                case "422":
+                    if isinstance(event, Partition.Command) and (msg_body.get("forceBypass") is True):
+                        # 422 sometimes occurs when forceBypass is True but there's nothing to bypass.
+                        log.debug(
+                            "Error executing %s, trying again without force bypass...",
+                            event.value,
+                        )
 
-                return await self.async_send_command(
-                    device_type=device_type,
-                    event=event,
-                    device_id=device_id,
-                    msg_body=msg_body,
-                )
-            if resp.status == 403:
-                # May have been logged out, try again
-                log.warning(
-                    "Error executing %s, logging in and trying again...", event.value
-                )
-                if retry_on_failure:
-                    await self.async_login()
-                    return await self.async_send_command(
-                        device_type,
-                        event,
-                        device_id,
-                        msg_body,
-                        False,
+                        # Not changing retry_on_failure. Changing forcebypass means that we won't re-enter this block.
+
+                        msg_body["forceBypass"] = False
+
+                        return await self.async_send_command(
+                            device_type=device_type,
+                            event=event,
+                            device_id=device_id,
+                            msg_body=msg_body,
+                        )
+
+                case "403":
+                    # May have been logged out, try again
+                    log.warning(
+                        "Error executing %s, logging in and trying again...",
+                        event.value,
                     )
+                    if retry_on_failure:
+                        await self.async_login()
+                        return await self.async_send_command(
+                            device_type,
+                            event,
+                            device_id,
+                            msg_body,
+                            False,
+                        )
 
-        log.error("%s failed with HTTP code %s", event.value, resp.status)
         log.error(
-            """URL: %s
-            JSON: %s
-            Headers: %s""",
-            url,
-            msg_body,
-            self._ajax_headers,
+            f"{event.value} failed with HTTP code {resp.status}. URL: {url}\nJSON: {msg_body}\nHeaders:"
+            f" {self._ajax_headers}"
         )
         raise ConnectionError
 
-    async def async_get_raw_server_responses(
-        self,
-        device_types: list[type[BaseDevice]],
-        include_image_sensor_b64: bool = False,
-    ) -> dict:
-        """Get raw responses from Alarm.com device endpoints."""
-
-        return_data: dict = {}
-
-        endpoints = []
-
-        for device_type, device_data in (
-            DEVICE_URLS["supported"] | DEVICE_URLS["unsupported"]
-        ).items():
-            if device_type in device_types:
-                endpoints.append(
-                    (slug_to_title(device_type.name), device_data["endpoint"])
-                )
+    def get_websocket_client(self) -> WebSocketClient:
+        """Construct and return a websocket client."""
+
+        return WebSocketClient(self._websession, self._ajax_headers, self.devices)
+
+    #
+    #
+    #####################
+    # PRIVATE FUNCTIONS #
+    #####################
+    #
+    # Communicate directly with the ADC API
+
+    async def _is_logged_in(self) -> bool:
+        """Check if we are logged in."""
+
+        async with self._websession.get(
+            url=self.KEEP_ALIVE_CHECK_URL_TEMPLATE.format(c.URL_BASE, int(round(datetime.now().timestamp()))),
+            headers=self._ajax_headers,
+        ) as resp:
+            text_rsp = await resp.text()
+
+        return bool(text_rsp == self.KEEP_ALIVE_CHECK_RESPONSE)
 
-        if ImageSensor in device_types:
-            endpoints.append(("Image Sensor Data", c.IMAGE_SENSOR_DATA_URL_TEMPLATE))
+    async def _async_get_active_system(self) -> str:
+        """Get active system for user account."""
+
+        try:
+            log.info("Getting active system.")
 
-        for name, url_template in endpoints:
             async with self._websession.get(
-                url=url_template.format(c.URL_BASE, ""),
+                url=self.ALL_SYSTEMS_URL_TEMPLATE.format(c.URL_BASE),
                 headers=self._ajax_headers,
+                raise_for_status=True,
             ) as resp:
-                try:
-                    json_rsp = await resp.json()
+                json_rsp = await resp.json()
 
-                    if name == "Image Sensor Data" and not include_image_sensor_b64:
-                        for image in json_rsp["data"]:
-                            del image["attributes"]["image"]
-
-                    rsp_errors = json_rsp.get("errors", [])
-
-                    if len(rsp_errors) != 0:
-                        error_msg = (
-                            "async_get_raw_server_responses(): Failed to get data."
-                            f" Response: {rsp_errors}"
-                        )
-                        log.debug(error_msg)
+                return str(
+                    [system["id"] for system in json_rsp.get("data", []) if system["attributes"]["isSelected"]][0]
+                )
 
-                        if rsp_errors[0].get("status") in ["403"]:
-                            raise PermissionError(error_msg)
+        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
+            log.error("Failed to get available systems.")
+            raise DataFetchFailed from err
 
-                        if (
-                            rsp_errors[0].get("status") == "409"
-                            and rsp_errors[0].get("detail")
-                            == "TwoFactorAuthenticationRequired"
-                        ):
-                            raise AuthenticationFailed(error_msg)
-
-                        if not (rsp_errors[0].get("status") in ["423"]):
-                            # We'll get here if user doesn't have permission to access a specific device type.
-                            pass
+    async def _async_get_recent_images(self) -> dict[str, DeviceTypeSpecificData]:
+        """Get recent images."""
 
-                    return_data[slug_to_title(name)] = (
-                        "\n" + json.dumps(json_rsp) + "\n"
-                    )
+        try:
+            log.info("Getting recent images.")
 
-                except ContentTypeError:
-                    if resp.status == 404:
-                        return_data[slug_to_title(name)] = "Endpoint not found."
-                    else:
-                        return_data[
-                            slug_to_title(name)
-                        ] = f"\nUnprocessable output:\n{resp.text}\n"
-
-        return return_data
-
-    def get_device_by_id(self, device_id: str) -> BaseDevice | None:
-        """Find device by its id."""
-
-        device: BaseDevice
-        for device in (
-            *self.systems,
-            *self.partitions,
-            *self.sensors,
-            *self.locks,
-            *self.garage_doors,
-            *self.gates,
-            *self.image_sensors,
-            *self.lights,
-            *self.cameras,
-            *self.thermostats,
-        ):
-            if device.id_ == device_id:
-                return device
+            async with self._websession.get(
+                url=self.ALL_RECENT_IMAGES_TEMPLATE.format(c.URL_BASE),
+                headers=self._ajax_headers,
+            ) as resp:
+                json_rsp = await resp.json()
 
-        return None
+            # Used by adc CLI.
+            self.raw_recent_images = json_rsp
 
-    #
-    #
-    #####################
-    # PRIVATE FUNCTIONS #
-    #####################
-    #
-    # Help process data returned by the API
+            if resp.status >= 400 or not isinstance(json_rsp, dict) or not len(json_rsp.get("data", [])):
+                return {}
 
-    async def _async_get_and_build_devices(
-        self,
-        device_types: list[DeviceType],
-    ) -> None:
-        """Get data for the specified device types and build objects."""
+            device_type_specific_data: dict[str, DeviceTypeSpecificData] = {}
 
-        for device_type in device_types:
-            #
-            # DETERMINE DEVICE'S PYALARMDOTCOMAJAX PYTHON CLASS
-            #
-            try:
-                device_class: (type[BaseDevice]) = DEVICE_CLASSES[device_type]
+            for image in json_rsp["data"]:
+                device_type_specific_data.setdefault(
+                    str(image["relationships"]["imageSensor"]["data"]["id"]), {}
+                ).setdefault("raw_recent_images", []).append(image)
 
-            except KeyError as err:
-                raise UnsupportedDevice from err
+            return device_type_specific_data
 
-            #############################
-            # FETCH DATA FROM ALARM.COM #
-            #############################
+        except (asyncio.TimeoutError, aiohttp.ClientError, KeyError) as err:
+            log.error("Failed to get available systems.")
+            raise DataFetchFailed from err
 
-            #
-            # GET ALL DEVICES WITHIN SPECIFIED CLASS
-            #
-            devices = []
-            try:
-                devices = await self._async_get_items_and_subordinates(
-                    device_type=device_type
-                )
+    async def _async_has_image_sensors(self, system_id: str, retry_on_failure: bool = True) -> bool:
+        """Check whether image sensors are present in system.
 
-            except BadAccount as err:
-                # Indicates fatal account error.
-                raise PermissionError from err
+        Check is required because image sensors are not shown in the device catalog endpoint.
+        """
 
-            except DataFetchFailed:
-                log.error(
-                    (
-                        "Encountered data error while fetching %ss. Skipping this"
-                        " device type."
-                    ),
-                    device_type.name,
-                )
+        try:
+            log.info(f"Checking system {system_id} for image sensors.")
 
-            if len(devices) == 0:
-                continue
+            # Find image sensors.
 
-            #
-            # PURGE UNSUPPORTED CAMERAS
-            #
-            # This is a hack. We don't really support cameras (no images / streaming), we only support settings for the Skybell HD.
-            if device_type == DeviceType.CAMERA:
-                skybells: list = []
-                for device_json, _ in devices:
-                    if (
-                        device_json.get("attributes", {}).get("deviceModel")
-                        == "SKYBELLHD"
-                    ):
-                        skybells.append((device_json, None))
+            async with self._websession.get(
+                url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, system_id),
+                headers=self._ajax_headers,
+                raise_for_status=True,
+            ) as resp:
+                json_rsp = await resp.json()
 
-                if not (devices := skybells):
-                    pass
+                await self._async_handle_server_errors(json_rsp, "image sensors", retry_on_failure)
 
-            #
-            # MAKE ADDITIONAL CALLS IF REQUIRED FOR DEVICE TYPE
-            #
-            additional_endpoint_raw_results: dict = {}
+                return len(json_rsp["data"].get("relationships", {}).get("imageSensors", {}).get("data", [])) > 0
 
-            try:
-                additional_endpoints: dict = DEVICE_URLS["supported"][device_type][
-                    "additional_endpoints"
-                ]
+        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
+            log.error("Failed to get image sensors.")
+            raise DataFetchFailed from err
 
-                for name, url in additional_endpoints.items():
-                    additional_endpoint_raw_results[
-                        name
-                    ] = await self._async_get_items_and_subordinates(url=url)
-
-            except KeyError:
-                pass
-
-            ####################
-            # QUERY EXTENSIONS #
-            ####################
+    async def _async_get_system_devices(self, system_id: str, retry_on_failure: bool = True) -> list[dict]:
+        """Get all devices present in system."""
 
-            #
-            # Check whether any devices have extensions.
-            #
+        try:
+            log.info(f"Getting all devices in {system_id}.")
 
-            required_extensions: list[type[CameraSkybellControllerExtension]] = []
-            device_settings: dict[
-                str, dict[str, ConfigurationOption]
-            ] = {}  # device_id {slug: ConfigurationOption}
-            name_id_map: dict[str, str] = {}
+            async with self._websession.get(
+                url=self.ALL_DEVICES_URL_TEMPLATE.format(c.URL_BASE, system_id),
+                headers=self._ajax_headers,
+                raise_for_status=True,
+            ) as resp:
+                json_rsp = await resp.json()
 
-            #
-            # Camera Skybell HD Extension
-            # Skybell HD extension pulls data for all cameras at once. We can stop searching at the first hit since we only care if we have at least one.
-            if device_type == DeviceType.CAMERA:
-                for device_json, _ in devices:
-                    if (
-                        device_json.get("attributes", {}).get("deviceModel")
-                        == "SKYBELLHD"
-                    ):
-                        required_extensions.append(CameraSkybellControllerExtension)
-                        break
+                # Used by adc CLI.
+                self.raw_catalog = json_rsp
 
-            #
-            # Build map of device names -> device ids.
-            #
+                await self._async_handle_server_errors(json_rsp, "system devices", retry_on_failure)
 
-            for device_json, subordinates in devices:
-                if name := device_json.get("attributes", {}).get("description"):
-                    name_id_map[name] = device_json["id"]
+                return [
+                    device
+                    for device in json_rsp["included"]
+                    if device.get("type") in AttributeRegistry.all_relationship_ids
+                ]
 
-            #
-            # Retrieve data for extensions
-            #
+        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
+            log.error("Failed to get system devices.")
+            raise DataFetchFailed from err
+        except TryAgain:
+            return await self._async_get_system_devices(system_id=system_id, retry_on_failure=False)
 
-            extension_controller: CameraSkybellControllerExtension | None = None
+    async def _async_get_devices_by_device_type(
+        self, device_type: DeviceType, retry_on_failure: bool = True
+    ) -> list[dict]:
+        """Get all devices of the specified type."""
 
-            for extension_class in required_extensions:
-                extension_controller = extension_class(
-                    websession=self._websession,
-                    headers=self._ajax_headers,
-                )
-
-                try:
-                    # Fetch from Alarm.com
-                    extended_properties_list: list[
-                        ExtendedProperties
-                    ] = await extension_controller.fetch()
-                except UnexpectedDataStructure:
-                    continue
+        try:
+            log.info(f"Getting all {device_type.value}.")
 
-                # Match extended properties to devices by name, then add to device_settings storage.
-                for extended_property in extended_properties_list:
-                    if (device_name := extended_property.device_name) in name_id_map:
-                        device_id = name_id_map[device_name]
-                        device_settings[device_id] = extended_property.settings
-
-            ##############################
-            # PREPROCESS ADDITIONAL DATA #
-            ##############################
+            async with self._websession.get(
+                url=AttributeRegistry.get_endpoints(device_type)["primary"].format(c.URL_BASE, ""),
+                headers=self._ajax_headers,
+                raise_for_status=True,
+            ) as resp:
+                json_rsp = await resp.json()
 
-            #
-            # PREPROCESSING FOR IMAGE SENSORS
-            #
-            # Extract recent images from image sensors
+                # Used by adc CLI.
+                if device_type == DeviceType.IMAGE_SENSOR:
+                    self.raw_image_sensors = json_rsp
 
-            element_specific_data: dict[str, ElementSpecificData] = {}
+                await self._async_handle_server_errors(json_rsp, f"get all {device_type.value}", retry_on_failure)
 
-            if device_class is ImageSensor:
-                for image in additional_endpoint_raw_results["recent_images"]:
-                    if isinstance(image, dict) and (
-                        image_sensor_id := str(
-                            image.get("relationships", {})
-                            .get("imageSensor", {})
-                            .get("data", {})
-                            .get("id")
-                        )
-                    ):
-                        element_specific_data.setdefault(
-                            image_sensor_id, {}
-                        ).setdefault("raw_recent_images", set()).add(image)
-
-            ###################
-            # BASE PROCESSING #
-            ###################
-
-            temp_device_storage: list = []
-
-            for device_raw_attribs, subordinates in devices:
-                entity_id = device_raw_attribs["id"]
-
-                entity_obj = device_class(
-                    id_=entity_id,
-                    raw_device_data=device_raw_attribs,
-                    subordinates=subordinates,
-                    element_specific_data=element_specific_data.get(entity_id),
-                    send_action_callback=self.async_send_command,
-                    config_change_callback=extension_controller.submit_change
-                    if extension_controller
-                    else None,
-                    trouble_conditions=self._trouble_conditions.get(entity_id),
-                    partition_id=self._partition_map.get(entity_id),
-                    settings=device_settings.get(entity_id),
-                )
+                return list(json_rsp["data"])
 
-                temp_device_storage.append(entity_obj)
+        except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
+            log.error(f"Failed to get {device_type.value}.")
+            raise DataFetchFailed from err
+        except TryAgain:
+            return await self._async_get_devices_by_device_type(device_type=device_type, retry_on_failure=False)
 
-            if device_class is System:
-                self.systems[:] = temp_device_storage
-            elif device_class is Partition:
-                self.partitions[:] = temp_device_storage
-            elif device_class is Sensor:
-                self.sensors[:] = temp_device_storage
-            elif device_class is GarageDoor:
-                self.garage_doors[:] = temp_device_storage
-            elif device_class is Gate:
-                self.gates[:] = temp_device_storage
-            elif device_class is Lock:
-                self.locks[:] = temp_device_storage
-            elif device_class is Light:
-                self.lights[:] = temp_device_storage
-            elif device_class is ImageSensor:
-                self.image_sensors[:] = temp_device_storage
-            elif device_class is Camera:
-                self.cameras[:] = temp_device_storage
-            elif device_class is Thermostat:
-                self.thermostats[:] = temp_device_storage
+    async def _async_unmask_otp(self, enabled_otp_types: int) -> OtpType:
+        """Extract single OTP type from enabledTwoFactorTypes bitmask."""
 
-    #
-    #
-    #################
-    # API FUNCTIONS #
-    #################
-    #
-    # Communicate directly with the ADC API
+        if bool(enabled_otp_types & OtpType.APP.value):
+            return OtpType.APP
+        elif bool(enabled_otp_types & OtpType.SMS.value):
+            return OtpType.SMS
+        elif bool(enabled_otp_types & OtpType.EMAIL.value):
+            return OtpType.EMAIL
+        else:
+            raise ValueError(f"Unknown OTP type: {enabled_otp_types}")
 
     async def _async_requires_2fa(self) -> bool | None:
         """Check whether two factor authentication is enabled on the account."""
         async with self._websession.get(
-            url=DEVICE_URLS["supported"][DeviceType.SYSTEM]["endpoint"].format(
-                c.URL_BASE, ""
-            ),
+            url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, ""),
             headers=self._ajax_headers,
         ) as resp:
             json_rsp = await resp.json()
 
         if (errors := json_rsp.get("errors")) and len(errors) > 0:
             for error in errors:
-                if (
-                    error.get("status") == "409"
-                    and error.get("detail") == "TwoFactorAuthenticationRequired"
-                ):
+                if error.get("status") == "409" and error.get("detail") == "TwoFactorAuthenticationRequired":
+                    log.debug("Two factor authentication is required. Getting details...")
                     # Get 2FA type ID
                     async with self._websession.get(
-                        url=self.LOGIN_2FA_DETAIL_URL_TEMPLATE.format(
-                            c.URL_BASE, self._user_id
-                        ),
+                        url=self.LOGIN_2FA_DETAIL_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
                         headers=self._ajax_headers,
                     ) as resp:
                         json_rsp = await resp.json()
 
-                        if isinstance(
-                            factor_id := json_rsp.get("data", {}).get("id"), int
-                        ):
+                        if isinstance(factor_id := json_rsp.get("data", {}).get("id"), int):
                             self._factor_type_id = factor_id
-                            self._two_factor_method = OtpType(
-                                json_rsp.get("data", {})
-                                .get("attributes", {})
-                                .get("twoFactorType")
-                            )
-                            log.debug(
-                                "Requires 2FA. Using method %s", self._two_factor_method
+                            self._two_factor_method = await self._async_unmask_otp(
+                                json_rsp.get("data", {}).get("attributes", {}).get("enabledTwoFactorTypes")
                             )
+                            log.info("Requires 2FA. Using method %s", self._two_factor_method)
                             return True
 
         log.debug("Does not require 2FA.")
         return False
 
     async def _async_get_identity_info(self) -> None:
         """Get user id, email address, provider name, etc."""
@@ -805,266 +837,161 @@
             async with self._websession.get(
                 url=c.IDENTITIES_URL_TEMPLATE.format(c.URL_BASE, ""),
                 headers=self._ajax_headers,
                 cookies=self._two_factor_cookie,
             ) as resp:
                 json_rsp = await resp.json()
 
-                # This is a verbose response. Uncommend when needed.
-                # log.debug("Got identity info:\n%s", json.dumps(json_rsp))
-
                 self._user_id = json_rsp["data"][0]["id"]
                 self._provider_name = json_rsp["data"][0]["attributes"]["logoName"]
 
                 for inclusion in json_rsp["included"]:
-                    if (
-                        inclusion["id"] == self._user_id
-                        and inclusion["type"] == "profile/profile"
-                    ):
+                    if inclusion["id"] == self._user_id and inclusion["type"] == "profile/profile":
                         self._user_email = inclusion["attributes"]["loginEmailAddress"]
 
             if self._user_email is None:
                 raise AuthenticationFailed("Could not find user email address.")
 
-            log.debug(
-                "Got Provider: %s, User ID: %s", self._provider_name, self._user_id
-            )
+            log.debug("Got Provider: %s, User ID: %s", self._provider_name, self._user_id)
 
         except KeyError as err:
-            log.debug(json_rsp)
+            log.error(f"{__name__} _async_get_identity_info: Failed to get user's identity info.")
+            log.debug(f"{__name__} _async_get_identity_info: Server Response:\n{json.dumps(json_rsp, indent=4)}")
             raise AuthenticationFailed from err
 
     async def _async_get_trouble_conditions(self) -> None:
         """Get trouble conditions for all devices."""
+
+        # TODO: Trouble condition dict should be flagged, not None, when library encounters an error retrieving trouble conditions.
+
         try:
             async with self._websession.get(
                 url=c.TROUBLECONDITIONS_URL_TEMPLATE.format(c.URL_BASE, ""),
                 headers=self._ajax_headers,
             ) as resp:
                 json_rsp = await resp.json()
 
                 log.debug("Trouble condition response:\n%s", json_rsp)
 
                 trouble_all_devices: dict = {}
                 for condition in json_rsp.get("data", []):
+                    device_id = condition.get("attributes", {}).get("emberDeviceId")
                     new_trouble: TroubleCondition = {
                         "message_id": condition.get("id"),
                         "title": condition.get("attributes", {}).get("description"),
-                        "body": condition.get("attributes", {})
-                        .get("extraData", {})
-                        .get("description"),
-                        "device_id": (
-                            device_id := condition.get("attributes", {}).get(
-                                "emberDeviceId"
-                            )
-                        ),
+                        "body": condition.get("attributes", {}).get("extraData", {}).get("description"),
+                        "device_id": device_id,
                     }
 
                     trouble_single_device: list = trouble_all_devices.get(device_id, [])
                     trouble_single_device.append(new_trouble)
                     trouble_all_devices[device_id] = trouble_single_device
 
                 self._trouble_conditions = trouble_all_devices
 
         except aiohttp.ContentTypeError as err:
+            self._trouble_conditions = {}
             log.error(
-                (
-                    "Server returned wrong content type. Response: %s\n\nResponse"
-                    " Text:\n\n%s\n\n"
-                ),
+                "Server returned wrong content type. Response: %s\n\nResponse Text:\n\n%s\n\n",
                 resp,
                 resp.text(),
             )
             raise DataFetchFailed from err
 
         except (asyncio.TimeoutError, aiohttp.ClientError) as err:
+            self._trouble_conditions = {}
             log.error("Connection error while fetching trouble conditions.")
             raise DataFetchFailed from err
 
         except KeyError as err:
+            self._trouble_conditions = {}
             log.error("Failed processing trouble conditions.")
             raise UnexpectedDataStructure from err
 
-    # Takes EITHER url (without base) or device_type.
-    async def _async_get_items_and_subordinates(
-        self,
-        device_type: DeviceType | None = None,
-        url: str | None = None,
-        retry_on_failure: bool = True,
-    ) -> list:
-        """Get attributes, metadata, and child devices for an ADC device class."""
-
-        #
-        # Determine URL
-        #
-        if (not device_type and not url) or (device_type and url):
-            raise ValueError
+    async def _async_handle_server_errors(
+        self, json_rsp: dict, request_name: str, retry_on_failure: bool = False
+    ) -> None:
+        """Handle errors returned by the server."""
 
-        full_path = (
-            DEVICE_URLS["supported"][device_type]["endpoint"] if device_type else url
+        log.debug(
+            f"\n==============================\nServer Response:\n{json_rsp}\n=============================="
         )
 
-        #
-        # Request data for device type
-        #
-        try:
-            async with self._websession.get(
-                url=full_path.format(c.URL_BASE, ""),
-                headers=self._ajax_headers,
-            ) as resp:
-                json_rsp = await resp.json()
-        except (ContentTypeError, json.JSONDecodeError) as err:
-            error_msg = (
-                "Could not fetch data for"
-                f" {device_type.name if device_type is not None else url}. Server"
-                f" responded with status {resp.status}."
-            )
-            log.warning(error_msg)
-            raise DataFetchFailed(error_msg) from err
+        if not len(rsp_errors := json_rsp.get("errors", [])):
+            return
 
-        return_items = []
-
-        #
-        # Handle Errors
-        #
-
-        rsp_errors = json_rsp.get("errors", [])
-        if len(rsp_errors) != 0:
-            error_msg = (
-                "_async_get_items_and_subordinates(): Failed to get data for device"
-                f" type {device_type}. Response: {rsp_errors}. Errors: {json_rsp}."
-            )
-            log.debug(error_msg)
+        log.debug(
+            error_msg := f"{__name__}: Request error. Status: {rsp_errors[0].get('status')}. Response: {json_rsp}"
+        )
 
-            if rsp_errors[0].get("status") == "423":
-                log.debug(
-                    (
-                        "Error fetching data from Alarm.com. This account either"
-                        " doesn't have permission to %s, is on a plan that does not"
-                        " support %s, or is part of a system with %s turned off."
-                    ),
-                    device_type,
-                    device_type,
-                    device_type,
+        match rsp_errors[0].get("status"):
+            case "423":  # Processing Error
+                log.error(
+                    f"Got a processing error when trying to request {request_name}. This may be caused by missing"
+                    " permissions, being on an Alarm.com plan without support for a particular device type, or"
+                    " having a device type disabled for this system."
                 )
-                # Carry on. We'll still try to load all other devices to which a user has access.
-                return []
+                log.debug(error_msg := f"{request_name} failed.\nResponse:\n{json_rsp}.")
+                raise PermissionError
 
-            if rsp_errors[0].get("status") == "403":
-                # User likely has an account without access to this class of device.
-                # I.e. Surety's "Surety Home" plan is alarm only; no cameras, lights, etc.
-                # All requests for those device types will return 403.
-                #
-                # On some providers, 403 may mean that the user has been logged out.
-                # Try logging in again, then give up by pretending that we couldn't find any devices of this type.
-
-                log.error("Error fetching data from Alarm.com.")
+            case "403":  # Invalid Anti-Forgery Token
+                # 403 means that either the user doesn't have access to this class of device or that the user has logged out.
+                # Unsupported device types should be stripped out in async_update(), so assume logged out.
+                # If logged out, try logging in again, then give up by pretending that we couldn't find any devices of this type.
 
                 if not retry_on_failure:
-                    log.debug(
-                        (
-                            "Got 403 status when fetching data for device type %s."
-                            " Logging in again didn't help."
-                        ),
-                        device_type,
+                    log.error(
+                        "Error fetching data from Alarm.com. Got 403 status when"
+                        f" fetching {request_name}. Logging in"
+                        " again didn't help. Giving up on device type."
                     )
+                    raise DataFetchFailed(error_msg)
 
-                    return list([])
-
-                log.error("Trying to refresh auth tokens by logging in again.")
+                if not self._is_logged_in():
+                    log.debug(
+                        "Error fetching data from Alarm.com. Got 403 status"
+                        f" when requesting {request_name}. Trying to"
+                        " refresh auth tokens by logging in again."
+                    )
 
-                await self.async_login()
+                    await self.async_login()
 
-                return await self._async_get_items_and_subordinates(
-                    device_type=device_type,
-                    retry_on_failure=False,
-                )
+                    raise TryAgain
 
-            if (
-                rsp_errors[0].get("status") == "409"
-                and rsp_errors[0].get("detail") == "TwoFactorAuthenticationRequired"
-            ):
+            case "409":
                 log.error(
-                    "Failed while fetching items and subordinates. Two factor"
-                    " authentication cookie is incorrect."
-                )
-                raise AuthenticationFailed(
-                    "Failed while fetching items and subordinates. Two factor"
-                    " authentication cookie is incorrect."
+                    error_msg := f"Failed to request {request_name}. Two factor authentication cookie is incorrect."
                 )
+                log.debug(error_msg := f"{request_name} failed.\nResponse:\n{json_rsp}.")
+                raise AuthenticationFailed(error_msg)
 
-            error_msg = (
-                f"{__name__}: Showing first error only. Status:"
-                f" {rsp_errors[0].get('status')}. Response: {json_rsp}"
-            )
-            log.debug(error_msg)
-            raise DataFetchFailed(error_msg)
-
-        #
-        # Get child elements for partitions and systems if function called using device_type parameter.
-        # If only url parameter used, we're probably just here to fetch additional endpoints.
-        #
-
-        if device_type and json_rsp.get("data"):
-            try:
-                for device in json_rsp["data"]:
-                    # Get list of downstream devices. Add to list for reference
-                    subordinates = []
-                    if device_type in [
-                        DeviceType.PARTITION,
-                        DeviceType.SYSTEM,
-                    ]:
-                        for family_name, family_data in device["relationships"].items():
-                            # TODO: Get list of unsupported devices to notify user of what has not been collected. Currently only collects known unknowns.
-                            if DeviceType.has_value(family_name):
-                                for sub_device in family_data["data"]:
-                                    subordinates.append(
-                                        (sub_device["id"], sub_device["type"])
-                                    )
-
-                                    if device_type == DeviceType.PARTITION:
-                                        self._partition_map[sub_device["id"]] = device[
-                                            "id"
-                                        ]
-
-                    return_items.append((device, subordinates))
-            except KeyError as err:
-                raise UnexpectedDataStructure(
-                    f"Failed while processing {device_type}"
-                ) from err
-
-        return return_items
+            case _:
+                log.error(f"Unknown error while requesting {request_name}.")
+                log.debug(error_msg := f"{request_name} failed.\nResponse:\n{json_rsp}.")
+                raise DataFetchFailed(error_msg)
 
     async def _async_login_and_get_key(self) -> None:
         """Load hidden fields from login page."""
         try:
             # load login page once and grab VIEWSTATE/cookies
-            async with self._websession.get(
-                url=self.LOGIN_URL, cookies=self._two_factor_cookie
-            ) as resp:
+            async with self._websession.get(url=self.LOGIN_URL, cookies=self._two_factor_cookie) as resp:
                 text = await resp.text()
                 log.debug("Response status from Alarm.com: %s", resp.status)
                 tree = BeautifulSoup(text, "html.parser")
                 login_info = {
-                    self.VIEWSTATE_FIELD: tree.select(f"#{self.VIEWSTATE_FIELD}")[
-                        0
-                    ].attrs.get("value"),
-                    self.VIEWSTATEGENERATOR_FIELD: tree.select(
-                        f"#{self.VIEWSTATEGENERATOR_FIELD}"
-                    )[0].attrs.get("value"),
-                    self.EVENTVALIDATION_FIELD: tree.select(
-                        f"#{self.EVENTVALIDATION_FIELD}"
-                    )[0].attrs.get("value"),
-                    self.PREVIOUSPAGE_FIELD: tree.select(f"#{self.PREVIOUSPAGE_FIELD}")[
-                        0
-                    ].attrs.get("value"),
+                    self.VIEWSTATE_FIELD: tree.select(f"#{self.VIEWSTATE_FIELD}")[0].attrs.get("value"),
+                    self.VIEWSTATEGENERATOR_FIELD: tree.select(f"#{self.VIEWSTATEGENERATOR_FIELD}")[0].attrs.get(
+                        "value"
+                    ),
+                    self.EVENTVALIDATION_FIELD: tree.select(f"#{self.EVENTVALIDATION_FIELD}")[0].attrs.get(
+                        "value"
+                    ),
+                    self.PREVIOUSPAGE_FIELD: tree.select(f"#{self.PREVIOUSPAGE_FIELD}")[0].attrs.get("value"),
                 }
 
-                log.debug(login_info)
-
         except (
             asyncio.TimeoutError,
             aiohttp.ClientError,
             asyncio.exceptions.CancelledError,
         ) as err:
             log.error("Can not load login page from Alarm.com")
 
@@ -1076,38 +1003,32 @@
             # login and grab ajax key
             async with self._websession.post(
                 url=self.LOGIN_POST_URL,
                 data={
                     self.LOGIN_USERNAME_FIELD: self._username,
                     self.LOGIN_PASSWORD_FIELD: self._password,
                     self.VIEWSTATE_FIELD: login_info[self.VIEWSTATE_FIELD],
-                    self.VIEWSTATEGENERATOR_FIELD: login_info[
-                        self.VIEWSTATEGENERATOR_FIELD
-                    ],
+                    self.VIEWSTATEGENERATOR_FIELD: login_info[self.VIEWSTATEGENERATOR_FIELD],
                     self.EVENTVALIDATION_FIELD: login_info[self.EVENTVALIDATION_FIELD],
                     self.PREVIOUSPAGE_FIELD: login_info[self.PREVIOUSPAGE_FIELD],
                     "IsFromNewSite": "1",
                 },
                 cookies=self._two_factor_cookie,
             ) as resp:
                 if re.search("m=login_fail", str(resp.url)) is not None:
                     log.error("Login failed.")
                     log.error("\nResponse URL:\n%s\n", str(resp.url))
-                    log.error(
-                        "\nRequest Headers:\n%s\n", str(resp.request_info.headers)
-                    )
+                    log.error("\nRequest Headers:\n%s\n", str(resp.request_info.headers))
                     raise AuthenticationFailed("Invalid username and password.")
 
                 # If Alarm.com is warning us that we'll have to set up two factor authentication soon, alert caller.
-                if (
-                    re.search("concurrent-two-factor-authentication", str(resp.url))
-                    is not None
-                ):
+                if re.search("concurrent-two-factor-authentication", str(resp.url)) is not None:
                     raise NagScreen("Encountered 2FA nag screen.")
 
+                # Update anti-forgery cookie
                 self._ajax_headers["ajaxrequestuniquekey"] = resp.cookies["afg"].value
 
         except (asyncio.TimeoutError, aiohttp.ClientError) as err:
             log.error("Can not login to Alarm.com")
             raise DataFetchFailed from err
         except KeyError as err:
             log.error("Unable to extract ajax key from Alarm.com. Response:\n%s", resp)
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-"""
-pyalarmdotcomajax CLI.
+"""pyalarmdotcomajax CLI.
 
 Based on https://github.com/uvjustin/pyalarmdotcomajax/pull/16 by Kevin David (@kevin-david)
 """
+
+# ruff: noqa: T201
+
 from __future__ import annotations
 
 import argparse
 import asyncio
-from dataclasses import asdict
-from enum import Enum
 import logging
 import platform
 import sys
+from dataclasses import asdict
+from enum import Enum
 from typing import Any
 
 import aiohttp
 from termcolor import colored, cprint
 
 import pyalarmdotcomajax
+from pyalarmdotcomajax.devices.registry import AllDevices_t, AttributeRegistry
 
 from . import AlarmController, AuthResult
-from .devices import DEVICE_URLS, BaseDevice, DeviceType
+from .devices import BaseDevice, DeviceType
 from .devices.light import Light
 from .devices.sensor import Sensor
 from .devices.system import System
 from .errors import (
-    AuthenticationFailed,
-    DataFetchFailed,
     InvalidConfigurationOption,
     NagScreen,
     UnexpectedDataStructure,
 )
 from .extensions import ConfigurationOption
 from .helpers import ExtendedEnumMixin, slug_to_title
 
@@ -39,16 +40,16 @@
 
 async def cli() -> None:
     """Support CLI development and testing. Not used in normal library operation."""
 
     parser = argparse.ArgumentParser(
         prog="adc",
         description=(
-            "basic command line debug interface for alarm.com via pyalarmdotcomajax."
-            " shows device states in various formats."
+            "basic command line debug interface for alarm.com via pyalarmdotcomajax. shows device states in"
+            " various formats."
         ),
     )
 
     ##################
     # BASE ARGUMENTS #
     ##################
 
@@ -66,35 +67,28 @@
         dest="version",
         action="version",
         version=f"%(prog)s {pyalarmdotcomajax.__version__}",
     )
     parser.add_argument(
         "-v",
         "--verbose",
-        help=(
-            "show verbose output. -vv returns base64 image data for image sensor"
-            " images."
-        ),
+        help="show verbose output. -vv returns base64 image data for image sensor images.",
         action="count",
         default=0,
         required=False,
     )
-    parser.add_argument(
-        "-u", "--username", dest="username", help="alarm.com username", required=True
-    )
-    parser.add_argument(
-        "-p", "--password", dest="password", help="alarm.com password", required=True
-    )
+    parser.add_argument("-u", "--username", dest="username", help="alarm.com username", required=True)
+    parser.add_argument("-p", "--password", dest="password", help="alarm.com password", required=True)
 
     parser.add_argument(
         "-n",
         "--device-name",
         help=(
-            "registers a device with this name on alarm.com and requests the two-factor"
-            " authentication cookie for the device."
+            "registers a device with this name on alarm.com and requests the two-factor authentication cookie for"
+            " the device."
         ),
         required=False,
     )
 
     ##########
     # GROUPS #
     ##########
@@ -104,17 +98,15 @@
     #
 
     otp_group = parser.add_mutually_exclusive_group()
 
     otp_group.add_argument(
         "-c",
         "--cookie",
-        help=(
-            "two-factor authentication cookie. cannot be used with --one-time-password!"
-        ),
+        help="two-factor authentication cookie. cannot be used with --one-time-password!",
         required=False,
     )
     otp_group.add_argument(
         "-o",
         "--one-time-password",
         help=(
             "provide otp code for accounts that have two-factor authentication enabled."
@@ -139,69 +131,71 @@
         description="get data from alarm.com",
         help="get data from alarm.com. use '%(prog)s get --help' for parameters.",
     )
 
     get_subparser.add_argument(
         "-x",
         "--include-unsupported",
-        help=(
-            "return basic data for all known unsupported devices. always outputs in"
-            " verbose format."
-        ),
+        help="return basic data for all known unsupported devices. always outputs in verbose format.",
         action="store_true",
         required=False,
     )
 
     #
     # Setting Subparser
     #
 
     set_subparser = subparsers.add_parser(
         "set",
         description="set device configuration option",
-        help=(
-            "set device configuration option. use '%(prog)s set --help' for parameters"
-        ),
+        help="set device configuration option. use '%(prog)s set --help' for parameters",
     )
 
-    set_subparser.add_argument(
-        "-i", "--device-id", help="Numeric Alarm.com device identifier.", required=True
-    )
+    set_subparser.add_argument("-i", "--device-id", help="Numeric Alarm.com device identifier.", required=True)
     set_subparser.add_argument(
         "-s",
         "--setting-slug",
         help=(
-            "Identifier for setting. Appears in parenthesis after setting name in"
-            " %(prog)s human readable output."
+            "Identifier for setting. Appears in parenthesis after setting name in %(prog)s human readable output."
         ),
     )
     set_subparser.add_argument(
         "-k",
         "--new-value",
         help="New value for setting.",
     )
 
+    #
+    # WebSocket / Watch Subparser
+    #
+
+    get_subparser = subparsers.add_parser(
+        "watch",
+        description="monitor alarm.com for real time updates",
+        help="monitor alarm.com for real time updates over WebSockets. hit Ctrl + C to exit.",
+    )
+
     ##########
     # SET UP #
     ##########
 
     args = vars(parser.parse_args())
 
     if args.get("debug", 0) > 0:
         logging.basicConfig(level=logging.DEBUG)
+    elif args.get("action") == "watch":
+        logging.basicConfig(level=logging.INFO)
     else:
         logging.basicConfig(level=logging.ERROR)
 
     ##########
     # LOG IN #
     ##########
 
-    cprint(
-        f"Logging in as {args.get('username')}.", "grey", "on_yellow", attrs=["bold"]
-    )
+    cprint(f"Logging in as {args.get('username')}.", "grey", "on_yellow", attrs=["bold"])
 
     if args.get("cookie") is not None:
         cprint(
             f"Using 2FA cookie {args.get('cookie')}.",
             "grey",
             "on_yellow",
             attrs=["bold"],
@@ -217,108 +211,88 @@
 
         generated_2fa_cookie = None
 
         try:
             login_result = await alarm.async_login()
         except NagScreen:
             cprint(
-                (
-                    "Unable to log in. Please set up two-factor authentication for this"
-                    " account."
-                ),
+                "Unable to log in. Please set up two-factor authentication for this account.",
                 "red",
             )
             sys.exit()
 
         if login_result == AuthResult.OTP_REQUIRED:
             code: str | None
             if not (code := args.get("one_time_password")):
                 cprint(
                     "Two factor authentication is enabled for this user.",
                     attrs=["bold"],
                 )
                 code = input("Enter One-Time Password: ")
 
             if code:
-                generated_2fa_cookie = await alarm.async_submit_otp(
-                    code=code, device_name=args.get("device_name")
-                )
+                generated_2fa_cookie = await alarm.async_submit_otp(code=code, device_name=args.get("device_name"))
             else:
                 cprint(
-                    (
-                        "Not enough information provided to make a decision regarding"
-                        " two-factor authentication."
-                    ),
+                    "Not enough information provided to make a decision regarding two-factor authentication.",
                     "red",
                 )
                 sys.exit()
 
         if login_result == AuthResult.ENABLE_TWO_FACTOR:
             cprint(
-                (
-                    "Unable to log in. Please set up two-factor authentication for this"
-                    " account."
-                ),
+                "Unable to log in. Please set up two-factor authentication for this account.",
                 "red",
             )
             sys.exit()
 
-        ######################
-        # UPDATE DEVICE DATA #
-        ######################
+        #######################
+        # REFRESH DEVICE DATA #
+        #######################
 
         await alarm.async_update()
 
         device_type_output: dict = {}
 
-        ############################
-        # GET DEVICE DATA WORKFLOW #
-        ############################
+        ###################
+        # GET DEVICE DATA #
+        ###################
 
         if args.get("action") == "get":
-            # Built List of Device Types
+            # Process MACHINE output
 
-            supported_device_types = []
-            for device_type in DEVICE_URLS["supported"]:
-                supported_device_types.append(device_type)
-
-            unsupported_device_types = []
-            if include_unsupported := args.get("include_unsupported", False):
-                for device_type in DEVICE_URLS["unsupported"]:
-                    unsupported_device_types.append(device_type)
-
-            # Get & Add Machine Output
-
-            if (verbose := args.get("verbose", 0)) > 0 or include_unsupported:
-                device_type_output.update(
-                    await _async_machine_output(
-                        alarm=alarm,
-                        include_image_sensor_b64=(verbose > 1),
-                        device_types=supported_device_types + unsupported_device_types
-                        if verbose > 0
-                        else unsupported_device_types,
-                    )
+            device_type_output = {
+                slug_to_title(device_type.name): [
+                    device
+                    for device in alarm.raw_catalog.get("included", [])
+                    if device.get("type") == AttributeRegistry.get_relationship_id_from_devicetype(device_type)
+                ] or "\n(none found)\n"
+                for device_type in DeviceType
+                if (
+                    device_type in AttributeRegistry.supported_device_types
+                    or args.get("include_unsupported", False)
                 )
+            }
+
+            # TODO: Include Image Sensor Image Data
 
             # Get & Add Human Output
 
-            if verbose == 0:
+            if (args.get("verbose", 0)) == 0:
                 device_type_output.update(_human_output(alarm))
 
             # Print Account Info
 
             print(f"\nProvider: {alarm.provider_name}")
             print(f"Logged in as: {alarm.user_email} ({alarm.user_id})")
             print("")
 
-            # Print Device Types
+            # Print Devices By Type
 
-            for device_type_name, device_type_body in sorted(
-                device_type_output.items()
-            ):
+            for device_type_name, device_type_body in sorted(device_type_output.items()):
                 cprint(
                     f"====[ {device_type_name} ]====",
                     "grey",
                     "on_yellow",
                     attrs=["bold"],
                 )
                 print(device_type_body)
@@ -335,36 +309,32 @@
             try:
                 device_id: str = args["device_id"]
                 setting_slug: str = args["setting_slug"]
                 new_value: Any = args["new_value"]
             except AttributeError:
                 cprint("Missing set parameter.", "red")
 
-            if not (device := alarm.get_device_by_id(device_id)):
+            if not (device := alarm.devices.get(device_id)):
                 cprint(f"Unable to find a device with ID {device_id}.", "red")
                 sys.exit(0)
 
             try:
                 config_option: ConfigurationOption = device.settings[setting_slug]
             except KeyError:
                 cprint(
-                    (
-                        f"{device.name} ({device_id}) does not have the setting"
-                        f" {setting_slug}."
-                    ),
+                    f"{device.name} ({device_id}) does not have the setting {setting_slug}.",
                     "red",
                 )
                 sys.exit(0)
 
             #
             # Convert user input into proper type
             #
-            config_option_type = config_option.value_type
 
-            if config_option_type in [bool, str, int]:
+            if (config_option_type := config_option.value_type) in [bool, str, int]:
                 try:
                     typed_new_value = config_option_type(new_value)
                 except ValueError:
                     cprint(
                         f"Setting {setting_slug} must be {config_option_type.__name__}",
                         "red",
                     )
@@ -385,133 +355,99 @@
 
             else:
                 cprint("Unexpected value type. This is a bug.")
                 sys.exit(0)
 
             # Submit new value.
             try:
-                await device.async_change_setting(
-                    slug=setting_slug, new_value=typed_new_value
-                )
+                await device.async_change_setting(slug=setting_slug, new_value=typed_new_value)
             except asyncio.TimeoutError:
                 cprint("Timed out while connecting to Alarm.com.")
             except (
                 aiohttp.ClientError,
                 asyncio.exceptions.CancelledError,
             ):
                 cprint("Failed to connect to Alarm.com.")
             except UnexpectedDataStructure:
                 cprint("Couldn't find settings on device configuration page.")
             except InvalidConfigurationOption:
-                cprint(
-                    "Couldn't load pyalarmdotcomajax configuration extension for"
-                    f" {setting_slug}."
-                )
+                cprint(f"Couldn't load pyalarmdotcomajax configuration extension for {setting_slug}.")
             except TypeError as err:
                 cprint(str(err), "red")
                 sys.exit(0)
 
             # Check success
             if issubclass(device.settings.get(setting_slug, {}).value_type, Enum):
-                reported_value = str(
-                    device.settings.get(setting_slug, {}).current_value.name
-                ).upper()
+                reported_value = str(device.settings.get(setting_slug, {}).current_value.name).upper()
             else:
-                reported_value = device.settings.get(setting_slug, {}).get(
-                    "current_value"
-                )
+                reported_value = device.settings.get(setting_slug, {}).get("current_value")
 
             if str(reported_value).upper() == str(new_value).upper():
                 cprint(
-                    (
-                        f"{config_option.name} was successfully changed to"
-                        f" {new_value} for {device.name}."
-                    ),
+                    f"{config_option.name} was successfully changed to {new_value} for {device.name}.",
                     "green",
                 )
             else:
                 cprint(
                     f"Error changing {config_option.name} for {device.name}.",
                     "red",
                 )
 
+        ###########################
+        # WATCH REAL TIME UPDATES #
+        ###########################
+
+        if args.get("action") == "watch":
+            cprint(
+                "Watching for real-time updates...",
+                "grey",
+                "on_yellow",
+                attrs=["bold"],
+            )
+            await _async_watch_realtime(alarm)
+
 
 #############
 # FUNCTIONS #
 #############
 
 
-async def _async_machine_output(
-    alarm: AlarmController,
-    device_types: list,
-    include_image_sensor_b64: bool = False,
-) -> dict:
-    """Output raw server responses."""
-
-    try:
-        responses = await alarm.async_get_raw_server_responses(
-            include_image_sensor_b64=include_image_sensor_b64, device_types=device_types
-        )
-    except PermissionError:
-        cprint("Permission error. Check that your credentials are correct.", "red")
-    except DataFetchFailed:
-        cprint("Connection error.", "red")
-    except AuthenticationFailed:
-        cprint(
-            (
-                "Authentication error. Check that your two factor authentication cookie"
-                " is correct."
-            ),
-            "red",
-        )
+async def _async_watch_realtime(alarm: AlarmController) -> None:
+    """Watch for real-time updates via WebSockets."""
 
-    return responses
+    ws_client = alarm.get_websocket_client()
+    await ws_client.async_connect()
 
 
 def _human_output(alarm: AlarmController) -> dict:
     """Output user-friendly list of devices and statuses."""
 
     output = {}
 
-    type_to_var: list[tuple[DeviceType, list]] = [
-        (DeviceType.SYSTEM, alarm.systems),
-        (DeviceType.PARTITION, alarm.partitions),
-        (DeviceType.SENSOR, alarm.sensors),
-        (DeviceType.LOCK, alarm.locks),
-        (DeviceType.GARAGE_DOOR, alarm.garage_doors),
-        (DeviceType.IMAGE_SENSOR, alarm.image_sensors),
-        (DeviceType.LIGHT, alarm.lights),
-        (DeviceType.CAMERA, alarm.cameras),
-        (DeviceType.THERMOSTAT, alarm.thermostats),
-    ]
-
-    device_type: DeviceType
-    devices: list
-    for device_type, devices in type_to_var:
+    for device_type in AttributeRegistry.supported_device_types:
+        devices: dict[str, AllDevices_t] = getattr(alarm.devices, AttributeRegistry.get_storage_name(device_type))
         device_type_output: str = ""
         if len(devices) == 0:
             device_type_output += "\n(none found)\n"
         else:
-            for device in sorted(devices, key=lambda device: str(device.name)):
+            for device in sorted(devices.values(), key=lambda device: str(device.name)):
                 device_type_output += _print_element_tearsheet(device)
 
         output[slug_to_title(device_type.name)] = device_type_output
 
     return output
 
 
 def _print_element_tearsheet(
     element: BaseDevice,
 ) -> str:
     output_str: str = ""
 
     # DEVICE NAME
-    output_str += colored(
-        f"\n{element.name} ({element.id_})", attrs=["bold", "underline"]
-    )
+    output_str += colored(f"\n{element.name} ({element.id_})", attrs=["bold", "underline"])
 
     if element.malfunction:
         output_str += colored(" (MALFUNCTION)", "red", attrs=["bold"])
 
     output_str += "\n"
 
     # BATTERY
@@ -587,13 +523,11 @@
     return output_str
 
 
 def main() -> None:
     """Run primary CLI function via asyncio. Main entrypoint for command line tool."""
 
     # Below is necessary to prevent asyncio "Event loop is closed" error in Windows.
-    if platform.system() == "Windows" and hasattr(
-        asyncio, "WindowsSelectorEventLoopPolicy"
-    ):
+    if platform.system() == "Windows" and hasattr(asyncio, "WindowsSelectorEventLoopPolicy"):
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
     asyncio.run(cli())
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/garage_door.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/garage_door.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Alarm.com garage door."""
 from __future__ import annotations
 
-from enum import Enum
 import logging
+from enum import Enum
+
+from pyalarmdotcomajax.devices import DeviceType
 
-from . import BaseDevice, DesiredStateMixin, DeviceType
+from . import BaseDevice, DesiredStateMixin
 
 log = logging.getLogger(__name__)
 
 
 class GarageDoor(DesiredStateMixin, BaseDevice):
     """Represent Alarm.com garage door element."""
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/gate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Alarm.com gate."""
 from __future__ import annotations
 
+import logging
 from dataclasses import dataclass
 from enum import Enum
-import logging
 
-from . import BaseDevice, DesiredStateMixin, DeviceType
+from pyalarmdotcomajax.devices import DeviceType
+
+from . import BaseDevice, DesiredStateMixin
 
 log = logging.getLogger(__name__)
 
 
 class Gate(DesiredStateMixin, BaseDevice):
     """Represent Alarm.com gate element."""
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Alarm.com image sensor."""
 from __future__ import annotations
 
+import logging
 from datetime import datetime
 from enum import Enum
-import logging
 from typing import TypedDict
 
 from dateutil import parser
 
-from . import BaseDevice, DeviceType
+from pyalarmdotcomajax.devices import DeviceType
+
+from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
 class ImageSensorImage(TypedDict):
     """Holds metadata for image sensor images."""
 
@@ -29,31 +31,24 @@
     class Command(Enum):
         """Commands for ADC image sensors."""
 
         PEEK_IN = "doPeekInNow"
 
     _recent_images: list[ImageSensorImage] = []
 
-    def process_element_specific_data(self) -> None:
+    def process_device_type_specific_data(self) -> None:
         """Process recent images."""
 
-        if not (
-            raw_recent_images := self._element_specific_data.get("raw_recent_images")
-        ):
+        if not (raw_recent_images := self._device_type_specific_data.get("raw_recent_images")):
             return
 
         for image in raw_recent_images:
             if (
                 isinstance(image, dict)
-                and str(
-                    image.get("relationships", {})
-                    .get("imageSensor", {})
-                    .get("data", {})
-                    .get("id")
-                )
+                and str(image.get("relationships", {}).get("imageSensor", {}).get("data", {}).get("id"))
                 == self.id_
             ):
                 image_data: ImageSensorImage = {
                     "id_": image["id"],
                     "image_b64": image["attributes"]["image"],
                     "image_src": image["attributes"]["imageSrc"],
                     "description": image["attributes"]["description"],
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/light.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Alarm.com light."""
 from __future__ import annotations
 
-from enum import Enum
 import logging
+from enum import Enum
 
-from . import BaseDevice, DesiredStateMixin, DeviceType
+from pyalarmdotcomajax.devices import BaseDevice, DesiredStateMixin, DeviceType
 
 log = logging.getLogger(__name__)
 
 
+# WebSocket Handler: https://www.alarm.com/web/system/assets/customer-ember/websockets/handlers/lights.ts
 class Light(DesiredStateMixin, BaseDevice):
     """Represent Alarm.com light element."""
 
+    ATTRIB_LIGHT_LEVEL = "lightLevel"
+
     class DeviceState(Enum):
         """Enum of light states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/LightStatus.js
 
         OFFLINE = 0
         NOSTATE = 1
@@ -32,25 +35,24 @@
     @property
     def available(self) -> bool:
         """Return whether the light can be manipulated."""
         return (
             self._attribs_raw.get("canReceiveCommands", False)
             and self._attribs_raw.get("remoteCommandsEnabled", False)
             and self._attribs_raw.get("hasPermissionToChangeState", False)
-            and self.state
-            in [self.DeviceState.ON, self.DeviceState.OFF, self.DeviceState.LEVELCHANGE]
+            and self.state in [self.DeviceState.ON, self.DeviceState.OFF, self.DeviceState.LEVELCHANGE]
         )
 
     @property
     def brightness(self) -> int | None:
         """Return light's brightness."""
         if not self._attribs_raw.get("isDimmer", False):
             return None
 
-        if isinstance(level := self._attribs_raw.get("lightLevel", 0), int):
+        if isinstance(level := self._attribs_raw.get(self.ATTRIB_LIGHT_LEVEL, 0), int):
             return level
 
         return None
 
     @property
     def supports_state_tracking(self) -> bool | None:
         """Return whether the light reports its current state."""
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/lock.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/lock.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Alarm.com lock."""
 from __future__ import annotations
 
-from enum import Enum
 import logging
+from enum import Enum
+
+from pyalarmdotcomajax.devices import DeviceType
 
-from . import BaseDevice, DesiredStateMixin, DeviceType
+from . import BaseDevice, DesiredStateMixin
 
 log = logging.getLogger(__name__)
 
 
 class Lock(DesiredStateMixin, BaseDevice):
     """Represent Alarm.com sensor element."""
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/partition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 """Alarm.com partition."""
 from __future__ import annotations
 
+import logging
 from dataclasses import dataclass
 from enum import Enum
-import logging
 
-from . import BaseDevice, DesiredStateMixin, DeviceType
+from pyalarmdotcomajax.devices import DeviceType
+
+from . import BaseDevice, DesiredStateMixin
 
 log = logging.getLogger(__name__)
 
 
 class Partition(DesiredStateMixin, BaseDevice):
     """Represent Alarm.com partition element."""
 
-    @dataclass
-    class ExtendedArmingMapping:
-        """Map of which extended arming states apply to which arming types."""
-
-        disarmed: list[Partition.ExtendedArmingOption] | None
-        armed_stay: list[Partition.ExtendedArmingOption] | None
-        armed_away: list[Partition.ExtendedArmingOption] | None
-        armed_night: list[Partition.ExtendedArmingOption] | None
-
-    @dataclass
-    class PartitionAttributes(BaseDevice.DeviceAttributes):
-        """Partition attributes."""
-
-        extended_arming_options: Partition.ExtendedArmingMapping | None  # List of extended arming options
-
     class ExtendedArmingOption(Enum):
         """Enum of extended arming options."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/ArmingOption.js
 
         BYPASS_SENSORS = 0
         NO_ENTRY_DELAY = 1
         SILENT_ARMING = 2
         NIGHT_ARMING = 3
         SELECTIVE_BYPASS = 4
 
+    @dataclass
+    class ExtendedArmingMapping:
+        """Map of which extended arming states apply to which arming types."""
+
+        disarm: list[Partition.ExtendedArmingOption | None]
+        arm_stay: list[Partition.ExtendedArmingOption | None]
+        arm_away: list[Partition.ExtendedArmingOption | None]
+        arm_night: list[Partition.ExtendedArmingOption | None]
+
+    @dataclass
+    class PartitionAttributes(BaseDevice.DeviceAttributes):
+        """Partition attributes."""
+
+        extended_arming_options: Partition.ExtendedArmingMapping  # List of extended arming options
+
     class DeviceState(Enum):
         """Enum of arming states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/ArmingState.js
 
         UNKNOWN = 0
         DISARMED = 1
@@ -56,100 +58,113 @@
         DISARM = "disarm"
         ARM_STAY = "armStay"
         ARM_AWAY = "armAway"
 
     @property
     def uncleared_issues(self) -> bool | None:
         """Return whether user needs to clear device state on alarm.com."""
-        if isinstance(
-            issues := self._attribs_raw.get("needsClearIssuesPrompt", None), bool
-        ):
+        if isinstance(issues := self._attribs_raw.get("needsClearIssuesPrompt", None), bool):
             return issues
 
         return None
 
     async def _async_arm(
         self,
         arm_type: Command,
-        force_bypass: bool = False,
-        no_entry_delay: bool = False,
-        silent_arming: bool = False,
-        night_arming: bool = False,
+        extended_arming_options: list[Partition.ExtendedArmingOption | None],
+        force_bypass: bool | None = None,
+        no_entry_delay: bool | None = None,
+        silent_arming: bool | None = None,
+        night_arming: bool | None = None,
     ) -> None:
         """Arm alarm system."""
 
         if arm_type == self.Command.DISARM:
             log.error("Invalid arm type.")
             return
 
-        msg_body = {
-            "forceBypass": force_bypass,
-            "noEntryDelay": no_entry_delay,
-            "silentArming": silent_arming,
-        }
+        msg_body = {}
+
+        if force_bypass and Partition.ExtendedArmingOption.BYPASS_SENSORS in extended_arming_options:
+            msg_body.update({"forceBypass": force_bypass})
 
-        # Sending nightArming when false causes trouble.
-        if night_arming:
+        if no_entry_delay and Partition.ExtendedArmingOption.NO_ENTRY_DELAY in extended_arming_options:
+            msg_body.update({"noEntryDelay": no_entry_delay})
+
+        if silent_arming and Partition.ExtendedArmingOption.SILENT_ARMING in extended_arming_options:
+            msg_body.update({"silentArming": silent_arming})
+
+        if night_arming and Partition.ExtendedArmingOption.NIGHT_ARMING in extended_arming_options:
             msg_body.update({"nightArming": night_arming})
 
         await self._send_action_callback(
             device_type=DeviceType.PARTITION,
             event=arm_type,
             device_id=self.id_,
             msg_body=msg_body,
         )
 
+    @property
+    def supports_night_arming(self) -> bool | None:
+        """Return whether night arming is supported."""
+
+        if Partition.ExtendedArmingOption.NIGHT_ARMING in self.attributes.extended_arming_options.arm_night:
+            return True
+
+        return False
+
     async def async_arm_stay(
         self,
-        force_bypass: bool = False,
-        no_entry_delay: bool = False,
-        silent_arming: bool = False,
+        force_bypass: bool | None = None,
+        no_entry_delay: bool | None = None,
+        silent_arming: bool | None = None,
     ) -> None:
         """Arm stay alarm."""
 
         log.debug("Calling arm stay.")
 
         await self._async_arm(
             arm_type=self.Command.ARM_STAY,
+            extended_arming_options=self.attributes.extended_arming_options.arm_stay,
             force_bypass=force_bypass,
             no_entry_delay=no_entry_delay,
             silent_arming=silent_arming,
-            night_arming=False,
         )
 
     async def async_arm_away(
         self,
-        force_bypass: bool = False,
-        no_entry_delay: bool = False,
-        silent_arming: bool = False,
+        force_bypass: bool | None = None,
+        no_entry_delay: bool | None = None,
+        silent_arming: bool | None = None,
     ) -> None:
         """Arm stay alarm."""
 
         log.debug("Calling arm away.")
 
         await self._async_arm(
             arm_type=self.Command.ARM_AWAY,
+            extended_arming_options=self.attributes.extended_arming_options.arm_away,
             force_bypass=force_bypass,
             no_entry_delay=no_entry_delay,
             silent_arming=silent_arming,
-            night_arming=False,
         )
 
     async def async_arm_night(
         self,
-        force_bypass: bool = False,
-        no_entry_delay: bool = False,
-        silent_arming: bool = False,
+        force_bypass: bool | None = None,
+        no_entry_delay: bool | None = None,
+        silent_arming: bool | None = None,
     ) -> None:
         """Arm stay alarm."""
 
         log.debug("Calling arm night.")
 
         await self._async_arm(
             arm_type=self.Command.ARM_STAY,
+            extended_arming_options=self.attributes.extended_arming_options.arm_night,
             force_bypass=force_bypass,
             no_entry_delay=no_entry_delay,
             silent_arming=silent_arming,
             night_arming=True,
         )
 
     async def async_disarm(
@@ -161,38 +176,26 @@
 
         await self._send_action_callback(
             device_type=DeviceType.PARTITION,
             event=self.Command.DISARM,
             device_id=self.id_,
         )
 
-    def _get_extended_arming_options(
-        self, options_list: list
-    ) -> list[Partition.ExtendedArmingOption]:
+    def _get_extended_arming_options(self, options_list: list) -> list[Partition.ExtendedArmingOption | None]:
         """Convert raw extended arming options to ExtendedArmingOption."""
 
         return [self.ExtendedArmingOption(option) for option in options_list]
 
     @property
-    def attributes(self) -> PartitionAttributes | None:
+    def attributes(self) -> PartitionAttributes:
         """Return partition attributes."""
 
-        extended_arming_options = dict(
-            self._attribs_raw.get("extendedArmingOptions", {})
-        )
+        extended_arming_options = dict(self._attribs_raw.get("extendedArmingOptions", {}))
 
         return self.PartitionAttributes(
             extended_arming_options=self.ExtendedArmingMapping(
-                disarmed=self._get_extended_arming_options(
-                    extended_arming_options.get("Disarmed", [])
-                ),
-                armed_stay=self._get_extended_arming_options(
-                    extended_arming_options.get("ArmedStay", [])
-                ),
-                armed_away=self._get_extended_arming_options(
-                    extended_arming_options.get("ArmedAway", [])
-                ),
-                armed_night=self._get_extended_arming_options(
-                    extended_arming_options.get("ArmedNight", [])
-                ),
+                disarm=self._get_extended_arming_options(extended_arming_options.get("Disarmed", [])),
+                arm_stay=self._get_extended_arming_options(extended_arming_options.get("ArmedStay", [])),
+                arm_away=self._get_extended_arming_options(extended_arming_options.get("ArmedAway", [])),
+                arm_night=self._get_extended_arming_options(extended_arming_options.get("ArmedNight", [])),
             )
         )
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/sensor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """Alarm.com sensor."""
 from __future__ import annotations
 
-from enum import Enum, IntEnum
 import logging
+from enum import Enum, IntEnum
 
 from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
 class Sensor(BaseDevice):
-    """Represent Alarm.com system element."""
+    """Represent Alarm.com sensor element."""
 
     class DeviceState(Enum):
         """Enum of sensor states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/SensorStatus.js
 
         UNKNOWN = 0
         CLOSED = 1
         OPEN = 2
         IDLE = 3
         ACTIVE = 4
-        DRY = 5
-        WET = 6
+
+        # Supported in WaterSensor class.
+        # DRY = 5
+        # WET = 6
 
         # Below not currently supported.
         # FULL = 7
         # LOW = 8
         # OPENED_CLOSED = 9
         # ISSUE = 10
         # OK = 11
@@ -45,12 +47,7 @@
         SIREN = 14
         GLASS_BREAK_DETECTOR = 19
         CONTACT_SHOCK_SENSOR = 52
         PANEL_MOTION_SENSOR = 89
         PANEL_GLASS_BREAK_DETECTOR = 83
         PANEL_IMAGE_SENSOR = 68
         MOBILE_PHONE = 69
-
-    @property
-    def read_only(self) -> None:
-        """Non-actionable object."""
-        return
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/system.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/system.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/devices/thermostat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,37 @@
 """Alarm.com thermostat."""
 from __future__ import annotations
 
+import logging
 from dataclasses import dataclass
 from enum import Enum
-import logging
 
+from pyalarmdotcomajax.devices import DeviceType
 from pyalarmdotcomajax.errors import UnexpectedDataStructure
 
-from . import BaseDevice, DesiredStateMixin, DeviceType
+from . import BaseDevice, DesiredStateMixin
 
 log = logging.getLogger(__name__)
 
 
 class Thermostat(DesiredStateMixin, BaseDevice):
     """Represent Alarm.com thermostat element."""
 
     # Fan duration of 0 is indefinite. otherwise value == hours.
     # TODO: desiredRts (remote temp sensor), desiredLocalDisplayLockingMode. Need user with remote sensors.
     # In identity info, check localizeTempUnitsToCelsius.
 
-    @dataclass
-    class ThermostatAttributes(BaseDevice.DeviceAttributes):
-        """Thermostat attributes."""
-
-        # Base
-        temp_average: float | None  # Temperature from thermostat and all remote sensors, averaged.
-        temp_at_tstat: float | None  # Temperature at thermostat only.
-        setpoint_offset: float | None
-        inferred_mode: Thermostat.DeviceState | None  # Indicates what thermostat is actually doing (cooling vs heating) if mode = auto.
-        # Fan
-        supports_fan_mode: bool | None
-        supports_fan_indefinite: bool | None
-        supports_fan_circulate_when_off: bool | None
-        supported_fan_durations: list[int] | None
-        fan_mode: Thermostat.FanMode | None
-        # fan_duration: int | None # Fan duration is not updated in server response, even when fan is turned on for specific amount of time.
-        # Temp
-        supports_heat: bool | None
-        supports_heat_aux: bool | None
-        supports_cool: bool | None
-        supports_auto: bool | None
-        supports_setpoints: bool | None
-        min_heat_setpoint: float | None
-        max_heat_setpoint: float | None
-        min_cool_setpoint: float | None
-        max_cool_setpoint: float | None
-        heat_setpoint: float | None
-        cool_setpoint: float | None
-        setpoint_buffer: float | None
-        # Humidity
-        supports_humidity: bool | None
-        humidity: int | None
-        # Schedules
-        supports_schedules: bool | None
-        supports_schedules_smart: bool | None
-        schedule_mode: Thermostat.ScheduleMode | None
-
-    class DeviceState(Enum):
-        """Enum of thermostat states."""
-
-        # https://www.alarm.com/web/system/assets/customer-ember/enums/ThermostatStatus.js
-
-        UNKNOWN = 0
-        OFF = 1
-        HEAT = 2
-        COOL = 3
-        AUTO = 4
-        AUX_HEAT = 5
+    ATTRIB_SETPOINT_OFFSET = "setpointOffset"
+    ATTRIB_AMBIENT_TEMP = "ambientTemp"
+    ATTRIB_FAN_MODE = "fanMode"
+    ATTRIB_DESIRED_FAN_MODE = "desiredFanMode"
+    ATTRIB_HEAT_SETPOINT = "heatSetpoint"
+    ATTRIB_DESIRED_HEAT_SETPOINT = "desiredHeatSetpoint"
+    ATTRIB_COOL_SETPOINT = "coolSetpoint"
+    ATTRIB_DESIRED_COOL_SETPOINT = "desiredCoolSetpoint"
 
     class FanMode(Enum):
         """Enum of thermostat fan modes."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/ThermostatFanMode.js
 
         AUTO = 0
@@ -80,14 +41,26 @@
         # AUTO_HIGH = 2
         # ON_HIGH = 3
         # AUTO_MEDIUM = 4
         # ON_MEDIUM = 5
         # CIRCULATE = 6
         # HUMIDITY = 7
 
+    class DeviceState(Enum):
+        """Enum of thermostat states."""
+
+        # https://www.alarm.com/web/system/assets/customer-ember/enums/ThermostatStatus.js
+
+        UNKNOWN = 0
+        OFF = 1
+        HEAT = 2
+        COOL = 3
+        AUTO = 4
+        AUX_HEAT = 5
+
     class LockMode(Enum):
         """Enum of thermostat lock modes."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/ThermostatLock.js
 
         DISABLED = 0
         ENABLED = 1
@@ -111,15 +84,52 @@
         SLEEP = 3
 
     class Command(Enum):
         """Commands for ADC lights."""
 
         SET_STATE = "setState"
 
-    DEVICE_MODELS = {
+    @dataclass
+    class ThermostatAttributes(BaseDevice.DeviceAttributes):
+        """Thermostat attributes."""
+
+        # Base
+        temp_average: float | None  # Temperature from thermostat and all remote sensors, averaged.
+        temp_at_tstat: float | None  # Temperature at thermostat only.
+        setpoint_offset: float | None
+        inferred_mode: Thermostat.DeviceState | None  # Indicates what thermostat is actually doing (cooling vs heating) if mode = auto.
+        # Fan
+        supports_fan_mode: bool | None
+        supports_fan_indefinite: bool | None
+        supports_fan_circulate_when_off: bool | None
+        supported_fan_durations: list[int] | None
+        fan_mode: Thermostat.FanMode | None
+        # fan_duration: int | None # Fan duration is not updated in server response, even when fan is turned on for specific amount of time.
+        # Temp
+        supports_heat: bool | None
+        supports_heat_aux: bool | None
+        supports_cool: bool | None
+        supports_auto: bool | None
+        supports_setpoints: bool | None
+        min_heat_setpoint: float | None
+        max_heat_setpoint: float | None
+        min_cool_setpoint: float | None
+        max_cool_setpoint: float | None
+        heat_setpoint: float | None
+        cool_setpoint: float | None
+        setpoint_buffer: float | None
+        # Humidity
+        supports_humidity: bool | None
+        humidity: int | None
+        # Schedules
+        supports_schedules: bool | None
+        supports_schedules_smart: bool | None
+        schedule_mode: Thermostat.ScheduleMode | None
+
+    _DEVICE_MODELS = {
         4293: {"manufacturer": "Honeywell", "model": "T6 Pro"},
         10023: {"manufacturer": "ecobee", "model": "ecobee3 lite"},
     }
 
     @property
     def available(self) -> bool:
         """Return whether the light can be manipulated."""
@@ -127,41 +137,39 @@
             self._attribs_raw.get("canReceiveCommands", False)
             and self._attribs_raw.get("remoteCommandsEnabled", False)
             and self._attribs_raw.get("hasPermissionToChangeState", False)
             and self.state is not self.DeviceState.UNKNOWN
         )
 
     @property
-    def attributes(self) -> ThermostatAttributes | None:
+    def attributes(self) -> ThermostatAttributes:
         """Return thermostat attributes."""
 
         return self.ThermostatAttributes(
             temp_average=self._get_float("forwardingAmbientTemp"),
-            temp_at_tstat=self._get_float("ambientTemp"),
+            temp_at_tstat=self._get_float(self.ATTRIB_AMBIENT_TEMP),
             inferred_mode=self._get_special("inferredMode", self.DeviceState),
-            setpoint_offset=self._get_float("setpointOffset"),
+            setpoint_offset=self._get_float(self.ATTRIB_SETPOINT_OFFSET),
             supports_fan_mode=self._get_bool("supportsFanMode"),
             supports_fan_indefinite=self._get_bool("supportsIndefiniteFanOn"),
-            supports_fan_circulate_when_off=self._get_bool(
-                "supportsCirculateFanModeWhenOff"
-            ),
+            supports_fan_circulate_when_off=self._get_bool("supportsCirculateFanModeWhenOff"),
             supported_fan_durations=self._get_list("supportedFanDurations", int),
-            fan_mode=self._get_special("fanMode", self.FanMode),
+            fan_mode=self._get_special(self.ATTRIB_FAN_MODE, self.FanMode),
             supports_heat=self._get_bool("supportsHeatMode"),
             supports_heat_aux=self._get_bool("supportsAuxHeatMode"),
             supports_cool=self._get_bool("supportsCoolMode"),
             supports_auto=self._get_bool("supportsAutoMode"),
             supports_setpoints=self._get_bool("supportsSetpoints"),
             setpoint_buffer=self._get_float("autoSetpointBuffer"),
             min_heat_setpoint=self._get_float("minHeatSetpoint"),
             min_cool_setpoint=self._get_float("minCoolSetpoint"),
             max_heat_setpoint=self._get_float("maxHeatSetpoint"),
             max_cool_setpoint=self._get_float("maxCoolSetpoint"),
-            heat_setpoint=self._get_float("heatSetpoint"),
-            cool_setpoint=self._get_float("coolSetpoint"),
+            heat_setpoint=self._get_float(self.ATTRIB_HEAT_SETPOINT),
+            cool_setpoint=self._get_float(self.ATTRIB_COOL_SETPOINT),
             supports_humidity=self._get_bool("supportsHumidity"),
             humidity=self._get_int("humidityLevel"),
             supports_schedules=self._get_bool("supportsSchedules"),
             supports_schedules_smart=self._get_bool("supportsSmartSchedules"),
             schedule_mode=self._get_special("scheduleMode", self.ScheduleMode),
         )
 
@@ -174,33 +182,31 @@
         schedule_mode: ScheduleMode | None = None,
     ) -> None:
         """Send turn on command with optional brightness."""
 
         msg_body: dict[str, float | int] = {}
 
         # Make sure we're only being asked to set one attribute at a time.
-        if (
-            attrib_list := [state, fan, cool_setpoint, heat_setpoint, schedule_mode]
-        ).count(None) < len(attrib_list) - 1:
+        if (attrib_list := [state, fan, cool_setpoint, heat_setpoint, schedule_mode]).count(None) < len(
+            attrib_list
+        ) - 1:
             raise UnexpectedDataStructure
 
         # Build the request body.
         if state:
-            msg_body = {"desiredState": state.value}
+            msg_body = {self._ATTRIB_STATE: state.value}
         elif fan:
             msg_body = {
-                "desiredFanMode": self.FanMode(fan[0]).value,
-                "desiredFanDuration": 0
-                if self.FanMode(fan[0]) == self.FanMode.AUTO
-                else fan[1],
+                self.ATTRIB_DESIRED_FAN_MODE: self.FanMode(fan[0]).value,
+                "desiredFanDuration": 0 if self.FanMode(fan[0]) == self.FanMode.AUTO else fan[1],
             }
         elif cool_setpoint:
-            msg_body = {"desiredCoolSetpoint": cool_setpoint}
+            msg_body = {self.ATTRIB_DESIRED_COOL_SETPOINT: cool_setpoint}
         elif heat_setpoint:
-            msg_body = {"desiredHeatSetpoint": heat_setpoint}
+            msg_body = {self.ATTRIB_DESIRED_HEAT_SETPOINT: heat_setpoint}
         elif schedule_mode:
             msg_body = {"desiredScheduleMode": schedule_mode.value}
 
         # Send
         await self._send_action_callback(
             device_type=DeviceType.THERMOSTAT,
             event=self.Command.SET_STATE,
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/errors.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from __future__ import annotations
 
 
 class UnsupportedDevice(Exception):
     """pyalarmdotcomajax encountered a device not currently supported by the package."""
 
 
+class UnkonwnDevice(Exception):
+    """pyalarmdotcomajax did not recognize the device ID."""
+
+
 class AuthenticationFailed(Exception):
     """Alarm.com authentication failure."""
 
 
 class TwoFactorAuthEnabled(Exception):
     """User has two factor authentication enabled."""
 
@@ -36,7 +40,11 @@
 
 class InvalidConfigurationOption(Exception):
     """Configuration option is not valid."""
 
 
 class UnsupportedAction(Exception):
     """Device does not support requested action."""
+
+
+class TryAgain(Exception):
+    """Request that caller tries again after session has been fixed."""
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Configuration option extensions."""
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
 import asyncio
-from dataclasses import dataclass
-from enum import Enum, auto
 import logging
 import re
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
+from enum import Enum, auto
 from typing import Any
 
 import aiohttp
 from bs4 import BeautifulSoup, Tag
 
 from pyalarmdotcomajax import const as c
 from pyalarmdotcomajax.errors import UnexpectedDataStructure
@@ -263,28 +263,24 @@
 
         #
         # Initialize request variables and get data for first camera.
         #
         try:
             additional_camera_config_ids: list[str] = []
 
-            async with self._websession.get(
-                url=self.ENDPOINT, headers=self._headers
-            ) as resp:
+            async with self._websession.get(url=self.ENDPOINT, headers=self._headers) as resp:
                 text = await resp.text()
                 log.debug("Response status from Alarm.com: %s", resp.status)
                 # log.debug("Response text from Alarm.com: %s", text)
                 tree = BeautifulSoup(text, "html.parser")
 
                 # Build list of cameras (everything or selection from camera_names)
 
                 child: Tag
-                for child in tree.select_one(
-                    "#ctl00_phBody_CamSelector_ddlCams"
-                ).findChildren():
+                for child in tree.select_one("#ctl00_phBody_CamSelector_ddlCams").findChildren():
                     camera_config_id: str = child.attrs.get("value")
                     if child.attrs.get("selected") == "selected":
                         # Retrieve data for camera on current page.
                         current_form_data = self._extract_fields(camera_config_id, tree)
 
                         if not camera_names or child.text in camera_names:
                             # Store data for current camera.
@@ -298,28 +294,25 @@
             aiohttp.ClientError,
             asyncio.exceptions.CancelledError,
         ) as err:
             log.error("Can not load settings page from Alarm.com")
             raise err
         except (AttributeError, IndexError) as err:
             log.error("Unable to extract page info from Alarm.com.")
-            log.debug(
-                "====== HTTP DUMP BEGIN ======\n%s\n====== HTTP DUMP END ======", text
-            )
+            log.debug("====== HTTP DUMP BEGIN ======\n%s\n====== HTTP DUMP END ======", text)
             raise UnexpectedDataStructure from err
 
         #
         # Get data for additional cameras.
         #
         try:
             for config_id in additional_camera_config_ids:
                 # Build payload to request config page for next camera
-                postback_form_data = current_form_data.raw_attribs
 
-                if not postback_form_data:
+                if not (postback_form_data := current_form_data.raw_attribs):
                     raise UnexpectedDataStructure
 
                 postback_form_data["__EVENTTARGET"] = "ctl00$phBody$CamSelector$ddlCams"
                 postback_form_data["ctl00$phBody$CamSelector$ddlCams"] = config_id
 
                 async with self._websession.post(
                     url=self.ENDPOINT,
@@ -327,17 +320,15 @@
                     headers=self._headers,
                 ) as resp:
                     text = await resp.text()
                     log.debug("Response status from Alarm.com: %s", resp.status)
                     tree = BeautifulSoup(text, "html.parser")
 
                     # Pull data for camera on current page
-                    camera_return_data.append(
-                        current_form_data := self._extract_fields(config_id, tree)
-                    )
+                    camera_return_data.append(current_form_data := self._extract_fields(config_id, tree))
         except (
             asyncio.TimeoutError,
             aiohttp.ClientError,
             asyncio.exceptions.CancelledError,
         ) as err:
             log.error("Can not load settings page for additional camera from Alarm.com")
 
@@ -356,18 +347,15 @@
     ) -> ConfigurationOption:
         """Change a setting."""
 
         # For non-volume adjustable chimes (indoor), value is "on" when checkbox is checked. Field is removed from POST payload when off.
         # For volume adjustable chimes (outdoor),  When on, either 1 for low, 2 for medium, 3 for high, or 0 for off.
 
         log.debug(
-            (
-                "CameraSkybellControllerExtension -> submit_change(): Requested change"
-                " for %s: %s to %s."
-            ),
+            "CameraSkybellControllerExtension -> submit_change(): Requested change for %s: %s to %s.",
             camera_name,
             slug,
             new_value,
         )
 
         #
         # Get field name for submitted value.
@@ -383,17 +371,15 @@
                     field_name = config_option_field_name
                     field_value_type = config_option.value_type
                     field_config_options = config_option
 
         except KeyError as err:
             raise UnexpectedDataStructure("Slug not found.") from err
 
-        log.debug(
-            "CameraSkybellControllerExtension -> submit_change(): Validating input."
-        )
+        log.debug("CameraSkybellControllerExtension -> submit_change(): Validating input.")
 
         #
         # VALIDATE INPUT
         #
 
         # Check that submitted value is correct type.
         # Currently only supports enums. In the future, should be expanded to also support native types.
@@ -401,56 +387,44 @@
         if field_value_type and not isinstance(new_value, field_value_type):
             raise TypeError(f"New value {new_value} is not of type {field_value_type}")
 
         # Validation for ints
 
         if field_value_type == int:
             if (
-                (
-                    (value_max := field_config_options.value_max)
-                    and new_value > value_max
-                )
-                or (
-                    (value_min := field_config_options.value_min)
-                    and new_value < value_min
-                )
+                ((value_max := field_config_options.value_max) and new_value > value_max)
+                or ((value_min := field_config_options.value_min) and new_value < value_min)
                 or not (isinstance(new_value, int))
             ):
                 raise ValueError
 
         # Validation for strings
 
         if field_value_type == str:
             if (
-                (value_regex := field_config_options.value_regex)
-                and not re.search(value_regex, new_value)
+                (value_regex := field_config_options.value_regex) and not re.search(value_regex, new_value)
             ) or not isinstance(new_value, str):
                 raise ValueError
 
-        log.debug(
-            "CameraSkybellControllerExtension -> submit_change(): Refreshing settings."
-        )
+        log.debug("CameraSkybellControllerExtension -> submit_change(): Refreshing settings.")
 
         #
         # Refresh settings data to prime submission payload.
         #
 
         results = await self.fetch(
             camera_names=[camera_name],
         )
 
         if not (payload := results[0].raw_attribs) or not (
             (config_id := results[0].config_id) or not isinstance(payload, dict)
         ):
             raise UnexpectedDataStructure("Failed to refresh settings data for device.")
 
-        log.debug(
-            "CameraSkybellControllerExtension -> submit_change(): Creating response"
-            " payload."
-        )
+        log.debug("CameraSkybellControllerExtension -> submit_change(): Creating response payload.")
 
         #
         # Process into response payload.
         #
 
         # Special processing for ChimeAdjustableVolume (currently only outdoor chime).
         # When volume is set, automatically change on/off setting.
@@ -511,18 +485,15 @@
         # Add static fields.
         #
 
         debug_payload = processed_payload.copy()
         debug_payload.pop("__VIEWSTATE")
 
         log.debug(
-            (
-                "======= POST PAYLOAD - BEGIN =======\n\n%s\n\n======= POST"
-                " PAYLOAD - END ======="
-            ),
+            "======= POST PAYLOAD - BEGIN =======\n\n%s\n\n======= POST PAYLOAD - END =======",
             debug_payload,
         )
 
         #
         # Submit payload and refresh data.
         #
 
@@ -554,34 +525,30 @@
         """Build POST for new setting submission or for getting other camera data."""
 
         # Pre-populate static fields.
         static_form_data: dict = {
             "__SCROLLPOSITIONX": "0",
             "__SCROLLPOSITIONY": "0",
             "ctl00$phBody$CamSelector$ddlPage": "CameraInfo",
-            "ctl00$phBody$AutomaticClipDonationSettings$ShowClipDonationLegalAgreement": (
-                "1"
-            ),
+            "ctl00$phBody$AutomaticClipDonationSettings$ShowClipDonationLegalAgreement": "1",
             "ctl00$phBody$tfSave": "Save",
             "ctl00$phBody$bridgeInfo$wirelessSettings$rblEncryption": "MakeASelection",
             "ctl00$phBody$bridgeInfo$wirelessSettings$rblAlgoritm": "MakeASelection",
             "ctl00$phBody$fwUpgradeModalTailTextBox": (
-                "Firmware upgrade is complete. You can check the video device status"
-                " after closing this dialog box."
+                "Firmware upgrade is complete. You can check the video device status after closing this dialog"
+                " box."
             ),
         }
 
         # Merge in dynamic fields with changed values.
         static_form_data.update(response_data)
 
         return static_form_data
 
-    def _extract_fields(
-        self, config_id: str, tree: BeautifulSoup
-    ) -> ExtendedProperties:
+    def _extract_fields(self, config_id: str, tree: BeautifulSoup) -> ExtendedProperties:
         """Extract data from camera config page."""
 
         # To prevent a single Skybell error from throwing an exception, missing fields will have values set to empty strings.
 
         raw_attribs: dict = {}
         properties = ExtendedProperties(
             config_id=config_id,
@@ -698,7 +665,10 @@
         except (KeyError, ValueError, UnexpectedDataStructure) as err:
             log.error("Unable to extract field. Failed on field %s.", field_name)
             raise UnexpectedDataStructure from err
 
         properties.raw_attribs = raw_attribs
 
         return properties
+
+
+ControllerExtensions_t = CameraSkybellControllerExtension
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.4.9b0
+Version: 0.5.0b0
 Summary: Python Interface for Alarm.com
-Home-page: https://github.com/uvjustin/pyalarmdotcomajax
+Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
-Maintainer: Justin Wong, Elahd Bar-Shai, Kevin David
+Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
 Keywords: Alarm.com,Security System,Home Assistant
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center"><img src="https://user-images.githubusercontent.com/466460/175575400-44ab6ed5-acb4-4a8c-b2ab-8b757675e900.png" height="200px"></p>
 <h1 align="center" border="1px solid black">pyalarmdotcomajax</h1>
 <h3 align="center">Asynchronous Python Library for Accessing Alarm.com Services</h3>
 <p align="center">This is an unofficial project that is not affiliated with Alarm.com.</p>
 <p align="center"><em>Forked from Daren Lord's pyalarmdotcom.</em></p>
 <br />
 <p align="center">
   <a href="https://github.com/uvjustin"><img src="https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue" /></a>
   <a href="https://github.com/elahd"><img src="https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue" /></a>
 </p>
 <p align="center">
-  <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a>
-  <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a>
+  <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd"/></a> -->
+  <!-- <a href="https://www.codacy.com/gh/pyalarmdotcom/pyalarmdotcomajax/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pyalarmdotcom/pyalarmdotcomajax&amp;utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/c58b00c68f9542aea1554d160997e5cd"/></a> -->
   <a href="https://results.pre-commit.ci/latest/github/pyalarmdotcom/pyalarmdotcomajax/master"><img src="https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/master.svg" /></a>
   <a href="https://pypi.org/project/pyalarmdotcomajax/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pyalarmdotcomajax"></a>
   <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
   <a href="https://github.com/PyCQA/pylint"><img src="https://img.shields.io/badge/linting-pylint-yellowgreen" /></a>
   <a href="https://github.com/pyalarmdotcom/pyalarmdotcomajax/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/pyalarmdotcom/pyalarmdotcomajax"></a>
 </p>
 
@@ -75,14 +75,15 @@
 | Sensor       | `device_subtype`                                                                                                                                                                                                                                                                                                                                                                                                                                                          | (none)                                |                                                  |
 | Locks        | `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                                           | lock, unlock                          |                                                  |
 | Garage Door  | (none)                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | open, close                           |                                                  |
 | Gate         | `supports_remote_close`                                                                                                                                                                                                                                                                                                                                                                                                                                                   | open, close                           |                                                  |
 | Image Sensor | `images`                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | peek_in                               |                                                  |
 | Light        | `brightness`                                                                                                                                                                                                                                                                                                                                                                                                                                                              | turn_on (with brightness), turn_off   | No support for RGB/W, effects, temperature, etc. |
 | Thermostat   | `temp_average`, `temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`, `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`, `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`, `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`, `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`, `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` | set_attribute                         |                                                  |
+| Water Sensor |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | (none)                                |                                                  |
 
 ### Known Sensor deviceTypes
 
 This list identifies deviceTypes used in the alarm.com API and is incomplete. Please help by submitting missing values.
 
 | deviceType | Description                            |
 | ---------- | -------------------------------------- |
@@ -185,15 +186,15 @@
 ### Open Items
 
 #### Features
 
 1. Support additional components (lights, irrigation, etc.).
 2. Support more sensor types (see list above in this README).
 3. Add `debug_info` property to `ADCController` that returns aggregate of raw JSON from all endpoints. This will allow users to export the entity model of unsupported devices to help maintainers implement support in this library.
-4. Similar to above, proactively populate `unsupported_devices` property for `ADCBaseElement` to show users device id, device name, and device type for available but unsupported devices.
+4. Similar to above, proactively populate `unsupported_device_types` property for `ADCBaseElement` to show users device id, device name, and device type for available but unsupported devices.
 5. More granular exception handling when logging in. Should report discrete error types for authentication failures due to wrong credentials, connection issues, or other.
 
 MIT License
 
 Copyright (c) 2020 Justin Wong
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,35 +1,33 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.4.9b0 Summary: Python
-Interface for Alarm.com Home-page: https://github.com/uvjustin/
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b0 Summary: Python
+Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
-46082645+uvjustin@users.noreply.github.com Maintainer: Justin Wong, Elahd Bar-
-Shai, Kevin David Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
+46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
+Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
-System,Home Assistant Classifier: Development Status :: 4 - Beta Classifier:
-Natural Language :: English Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Home Automation Requires-
-Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English Classifier: Environment :: Web
+Environment Classifier: Intended Audience :: Developers Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Home Automation
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+LICENSE
 [https://user-images.githubusercontent.com/466460/175575400-44ab6ed5-acb4-4a8c-
                             b2ab-8b757675e900.png]
                         ****** pyalarmdotcomajax ******
     **** Asynchronous Python Library for Accessing Alarm.com Services ****
      This is an unofficial project that is not affiliated with Alarm.com.
                     Forked from Daren Lord's pyalarmdotcom.
 
   [https://img.shields.io/badge/Creator-Justin%20Wong%20(%40uvjustin)-blue]
  [https://img.shields.io/badge/Maintainer-Elahd%20Bar--Shai%20(%40elahd)-blue]
-[https://app.codacy.com/project/badge/Grade/c58b00c68f9542aea1554d160997e5cd]
-                [https://app.codacy.com/project/badge/Coverage/
-c58b00c68f9542aea1554d160997e5cd] [https://results.pre-commit.ci/badge/github/
-  pyalarmdotcom/pyalarmdotcomajax/master.svg] [PyPI] [https://img.shields.io/
-  badge/code%20style-black-000000.svg] [https://img.shields.io/badge/linting-
-                         pylint-yellowgreen] [GitHub]
+  [https://results.pre-commit.ci/badge/github/pyalarmdotcom/pyalarmdotcomajax/
+master.svg] [PyPI] [https://img.shields.io/badge/code%20style-black-000000.svg]
+      [https://img.shields.io/badge/linting-pylint-yellowgreen] [GitHub]
 ## Installation / Usage To install use pip: ```bash pip install
 pyalarmdotcomajax ``` Or clone the repo: ```bash git clone https://github.com/
 uvjustin/pyalarmdotcomajax.git python setup.py install ``` ## Usage See
 `examples/basic_sensor_data.py` for a basic usage example. ## Device Support
 (Core Functions) Pyalarmdotcomajax supports core features (monitoring and using
 actions) of the device types listed below. - As of v0.2, multiples of all
 devices are supported. - All devices include the attributes: `name`, `id_`,
@@ -51,87 +49,88 @@
 temperature, etc. | | Thermostat | `temp_average`, `temp_at_tstat`,
 `step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
 `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`,
 `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`,
 `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`,
 `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`,
 `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` |
-set_attribute | | ### Known Sensor deviceTypes This list identifies deviceTypes
-used in the alarm.com API and is incomplete. Please help by submitting missing
-values. | deviceType | Description | | ---------- | ---------------------------
------------ | | 1 | Contact Sensor | | 2 | Motion Sensor | | 5 | Smoke Detector
-| | 6 | CO Detector | | 8 | Freeze Sensor | | 9 | Panic Button | | 10 | Fixed
-Panic Button | | 14 | Siren | | 19 | Glass Break Detector | | 52 | Vibration
-Contact Sensor | | 68 | Panel Image Sensor | | 69 | Mobile Phone (for Bluetooth
-Disarming) | | 83 | Panel Glass Break Sensor | | 89 | Panel Motion Sensor | ##
-Device Support (Configuration) Pyalarmdotcomajax supports changing
-configuration options for the devices listed below. ### Skybell HD ####
-Doorbell Camera | Configuration Option | Slug | Supported Values | Notes | | --
------------------------ | -------------------- | ------------------------------
------- | -------------------------- | | Indoor Chime | `indoor-chime` | `on`,
-`off` | | | Outdoor Chime | `outdoor-chime` | `off`, `low`, `medium`, `high` |
-| | LED Brightness | `led-brightness` | 0-100 | | | LED Color | `led-color` |
-`#000000` - `#FFFFFF` | Must include `#` at start. | | Motion Sensor
-Sensitivity | `motion-sensitivity` | `low`, `medium`, `high`, `very_high` | |
-## Command Line Interface The CLI is available by running `adc` from anywhere
-in your terminal. Use `adc --help`, `adc get --help`, and `adc set --help` for
-more information. ```bash usage: adc [-h] [-d] [-ver] [-v] -u USERNAME -
-p PASSWORD [-n DEVICE_NAME] [-c COOKIE | -o ONE_TIME_PASSWORD] {get,set} ...
-basic command line debug interface for alarm.com via pyalarmdotcomajax. shows
-device states in various formats. options: -h, --help show this help message
-and exit -d, --debug show pyalarmdotcomajax's debug output. -ver, --version
-show program's version number and exit -v, --verbose show verbose output. -vv
-returns base64 image data for image sensor images. -u USERNAME, --username
-USERNAME alarm.com username -p PASSWORD, --password PASSWORD alarm.com password
--n DEVICE_NAME, --device-name DEVICE_NAME registers a device with this name on
-alarm.com and requests the two-factor authentication cookie for the device. -
-c COOKIE, --cookie COOKIE two-factor authentication cookie. cannot be used with
---one-time-password! -o ONE_TIME_PASSWORD, --one-time-password
-ONE_TIME_PASSWORD provide otp code for accounts that have two-factor
-authentication enabled. if not provided here, adc will prompt user for otp.
-cannot be used with --cookie! actions: {get,set} get get data from alarm.com.
-use 'adc get --help' for parameters. set set device configuration option. use
-'adc set --help' for parameters get options: -h, --help show this help message
-and exit -x, --include-unsupported return basic data for all known unsupported
-devices. always outputs in verbose format. set options: -h, --help show this
-help message and exit -i DEVICE_ID, --device-id DEVICE_ID Numeric Alarm.com
-device identifier. -s SETTING_SLUG, --setting-slug SETTING_SLUG Identifier for
-setting. Appears in parenthesis after setting name in adc set human readable
-output. -k NEW_VALUE, --new-value NEW_VALUE New value for setting. ``` ###
-Examples 1. Get human-readable status (and device IDs) for all devices: `adc -
-u "your_username" -p "your_password" get` 2. Get raw JSON output from Alarm.com
-for all devices: `adc -v -u "your_username" -p "your_password" get` 3. Turn off
-Skybell HD indoor chime (assume Skybell device ID is 283431032-1520): `adc -
-u "your_username" -p "your_password" set -i "283431032-1520" -s "indoor-chime"
--k "off"` ## Development ### VS Code Support Structures This repository
-includes a full development environment for VS Code: 1. VS Code [dev container]
-(https://code.visualstudio.com/docs/remote/create-dev-container). Automatically
-installs extensions and Python dependencies and registers Git pre-commit
-scripts. 2. Configuration files for type checking ([mypy](http://mypy-lang.org/
-)), linting ([flake8](https://flake8.pycqa.org/en/latest/), [isort](https://
-github.com/PyCQA/isort), and [black](https://github.com/psf/black)), code
-security ([Bandit](https://bandit.readthedocs.io/en/latest/)), etc. 3. Pre-
-commit checks run all of the above when committing to Git and on demand via VS
-Code [tasks](https://code.visualstudio.com/docs/editor/tasks). ### References
-1. Some API definitions are available in the [node-alarm-dot-com repository]
-(https://github.com/node-alarm-dot-com/node-alarm-dot-com/tree/master/src/
-_models). ### Open Items #### Features 1. Support additional components
-(lights, irrigation, etc.). 2. Support more sensor types (see list above in
-this README). 3. Add `debug_info` property to `ADCController` that returns
-aggregate of raw JSON from all endpoints. This will allow users to export the
-entity model of unsupported devices to help maintainers implement support in
-this library. 4. Similar to above, proactively populate `unsupported_devices`
-property for `ADCBaseElement` to show users device id, device name, and device
-type for available but unsupported devices. 5. More granular exception handling
-when logging in. Should report discrete error types for authentication failures
-due to wrong credentials, connection issues, or other. MIT License Copyright
-(c) 2020 Justin Wong Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated documentation files
-(the "Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish, distribute,
+set_attribute | | | Water Sensor | | (none) | | ### Known Sensor deviceTypes
+This list identifies deviceTypes used in the alarm.com API and is incomplete.
+Please help by submitting missing values. | deviceType | Description | | ------
+---- | -------------------------------------- | | 1 | Contact Sensor | | 2 |
+Motion Sensor | | 5 | Smoke Detector | | 6 | CO Detector | | 8 | Freeze Sensor
+| | 9 | Panic Button | | 10 | Fixed Panic Button | | 14 | Siren | | 19 | Glass
+Break Detector | | 52 | Vibration Contact Sensor | | 68 | Panel Image Sensor |
+| 69 | Mobile Phone (for Bluetooth Disarming) | | 83 | Panel Glass Break Sensor
+| | 89 | Panel Motion Sensor | ## Device Support (Configuration)
+Pyalarmdotcomajax supports changing configuration options for the devices
+listed below. ### Skybell HD #### Doorbell Camera | Configuration Option | Slug
+| Supported Values | Notes | | ------------------------- | -------------------
+- | ------------------------------------ | -------------------------- | |
+Indoor Chime | `indoor-chime` | `on`, `off` | | | Outdoor Chime | `outdoor-
+chime` | `off`, `low`, `medium`, `high` | | | LED Brightness | `led-brightness`
+| 0-100 | | | LED Color | `led-color` | `#000000` - `#FFFFFF` | Must include
+`#` at start. | | Motion Sensor Sensitivity | `motion-sensitivity` | `low`,
+`medium`, `high`, `very_high` | | ## Command Line Interface The CLI is
+available by running `adc` from anywhere in your terminal. Use `adc --help`,
+`adc get --help`, and `adc set --help` for more information. ```bash usage: adc
+[-h] [-d] [-ver] [-v] -u USERNAME -p PASSWORD [-n DEVICE_NAME] [-c COOKIE | -
+o ONE_TIME_PASSWORD] {get,set} ... basic command line debug interface for
+alarm.com via pyalarmdotcomajax. shows device states in various formats.
+options: -h, --help show this help message and exit -d, --debug show
+pyalarmdotcomajax's debug output. -ver, --version show program's version number
+and exit -v, --verbose show verbose output. -vv returns base64 image data for
+image sensor images. -u USERNAME, --username USERNAME alarm.com username -
+p PASSWORD, --password PASSWORD alarm.com password -n DEVICE_NAME, --device-
+name DEVICE_NAME registers a device with this name on alarm.com and requests
+the two-factor authentication cookie for the device. -c COOKIE, --cookie COOKIE
+two-factor authentication cookie. cannot be used with --one-time-password! -
+o ONE_TIME_PASSWORD, --one-time-password ONE_TIME_PASSWORD provide otp code for
+accounts that have two-factor authentication enabled. if not provided here, adc
+will prompt user for otp. cannot be used with --cookie! actions: {get,set} get
+get data from alarm.com. use 'adc get --help' for parameters. set set device
+configuration option. use 'adc set --help' for parameters get options: -h, --
+help show this help message and exit -x, --include-unsupported return basic
+data for all known unsupported devices. always outputs in verbose format. set
+options: -h, --help show this help message and exit -i DEVICE_ID, --device-id
+DEVICE_ID Numeric Alarm.com device identifier. -s SETTING_SLUG, --setting-slug
+SETTING_SLUG Identifier for setting. Appears in parenthesis after setting name
+in adc set human readable output. -k NEW_VALUE, --new-value NEW_VALUE New value
+for setting. ``` ### Examples 1. Get human-readable status (and device IDs) for
+all devices: `adc -u "your_username" -p "your_password" get` 2. Get raw JSON
+output from Alarm.com for all devices: `adc -v -u "your_username" -
+p "your_password" get` 3. Turn off Skybell HD indoor chime (assume Skybell
+device ID is 283431032-1520): `adc -u "your_username" -p "your_password" set -
+i "283431032-1520" -s "indoor-chime" -k "off"` ## Development ### VS Code
+Support Structures This repository includes a full development environment for
+VS Code: 1. VS Code [dev container](https://code.visualstudio.com/docs/remote/
+create-dev-container). Automatically installs extensions and Python
+dependencies and registers Git pre-commit scripts. 2. Configuration files for
+type checking ([mypy](http://mypy-lang.org/)), linting ([flake8](https://
+flake8.pycqa.org/en/latest/), [isort](https://github.com/PyCQA/isort), and
+[black](https://github.com/psf/black)), code security ([Bandit](https://
+bandit.readthedocs.io/en/latest/)), etc. 3. Pre-commit checks run all of the
+above when committing to Git and on demand via VS Code [tasks](https://
+code.visualstudio.com/docs/editor/tasks). ### References 1. Some API
+definitions are available in the [node-alarm-dot-com repository](https://
+github.com/node-alarm-dot-com/node-alarm-dot-com/tree/master/src/_models). ###
+Open Items #### Features 1. Support additional components (lights, irrigation,
+etc.). 2. Support more sensor types (see list above in this README). 3. Add
+`debug_info` property to `ADCController` that returns aggregate of raw JSON
+from all endpoints. This will allow users to export the entity model of
+unsupported devices to help maintainers implement support in this library. 4.
+Similar to above, proactively populate `unsupported_device_types` property for
+`ADCBaseElement` to show users device id, device name, and device type for
+available but unsupported devices. 5. More granular exception handling when
+logging in. Should report discrete error types for authentication failures due
+to wrong credentials, connection issues, or other. MIT License Copyright (c)
+2020 Justin Wong Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including without
+limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
 above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
 IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
```

### Comparing `pyalarmdotcomajax-0.4.9b0/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.0b0/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
-setup.py
 pyalarmdotcomajax/__init__.py
 pyalarmdotcomajax/__main__.py
 pyalarmdotcomajax/cli.py
 pyalarmdotcomajax/const.py
 pyalarmdotcomajax/errors.py
 pyalarmdotcomajax/extensions.py
 pyalarmdotcomajax/helpers.py
+pyalarmdotcomajax/ws.py
 pyalarmdotcomajax.egg-info/PKG-INFO
 pyalarmdotcomajax.egg-info/SOURCES.txt
 pyalarmdotcomajax.egg-info/dependency_links.txt
 pyalarmdotcomajax.egg-info/entry_points.txt
 pyalarmdotcomajax.egg-info/requires.txt
 pyalarmdotcomajax.egg-info/top_level.txt
 pyalarmdotcomajax.egg-info/zip-safe
@@ -21,18 +21,33 @@
 pyalarmdotcomajax/devices/camera.py
 pyalarmdotcomajax/devices/garage_door.py
 pyalarmdotcomajax/devices/gate.py
 pyalarmdotcomajax/devices/image_sensor.py
 pyalarmdotcomajax/devices/light.py
 pyalarmdotcomajax/devices/lock.py
 pyalarmdotcomajax/devices/partition.py
+pyalarmdotcomajax/devices/registry.py
 pyalarmdotcomajax/devices/sensor.py
 pyalarmdotcomajax/devices/system.py
 pyalarmdotcomajax/devices/thermostat.py
+pyalarmdotcomajax/devices/water_sensor.py
+pyalarmdotcomajax/websockets/__init__.py
+pyalarmdotcomajax/websockets/client.py
+pyalarmdotcomajax/websockets/const.py
+pyalarmdotcomajax/websockets/messages.py
+pyalarmdotcomajax/websockets/handler/__init__.py
+pyalarmdotcomajax/websockets/handler/garage_door.py
+pyalarmdotcomajax/websockets/handler/gate.py
+pyalarmdotcomajax/websockets/handler/light.py
+pyalarmdotcomajax/websockets/handler/lock.py
+pyalarmdotcomajax/websockets/handler/partition.py
+pyalarmdotcomajax/websockets/handler/sensor.py
+pyalarmdotcomajax/websockets/handler/thermostat.py
+pyalarmdotcomajax/websockets/handler/water_sensor.py
 tests/__init__.py
 tests/conftest.py
 tests/test_controller.py
 tests/test_device_extensions.py
-tests/test_no_permissions.py
 tests/test_partition.py
+tests/test_sensors.py
 tests/test_thermostat.py
 tests/responses/__init__.py
```

### Comparing `pyalarmdotcomajax-0.4.9b0/setup.cfg` & `pyalarmdotcomajax-0.5.0b0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [metadata]
 name = pyalarmdotcomajax
 description = Python Interface for Alarm.com
 author = Justin Wong
 author_email = 46082645+uvjustin@users.noreply.github.com
-maintainer = Justin Wong, Elahd Bar-Shai, Kevin David
+maintainer = Elahd Bar-Shai
 maintainer_email = 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 version = attr: pyalarmdotcomajax.__version__
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
-url = https://github.com/uvjustin/pyalarmdotcomajax
+url = https://github.com/pyalarmdotcom/pyalarmdotcomajax
 keywords = Alarm.com, Security System, Home Assistant
 license = MIT
 license_files = LICENSE
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Natural Language :: English
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Home Automation
 
 [options]
 zip_safe = True
 include_package_data = True
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 install_requires = 
 	beautifulsoup4 >= 4.10.0
 	aiohttp >= 3.8.1
 	python-dateutil >= 2.8.2
 	termcolor >= 2.1.1
 
 [options.entry_points]
```

### Comparing `pyalarmdotcomajax-0.4.9b0/tests/__init__.py` & `pyalarmdotcomajax-0.5.0b0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tests for pyalarmdotcomajax"""
+"""Tests for pyalarmdotcomajax."""
 
 #
 # TESTING RESOURCES
 #
 # Test Creation References
 #
 # https://github.com/JohnPaton/airbase/tree/9fe0fcd837d26b0d9f842a193d8bdd2a59d9f32a/tests
```

### Comparing `pyalarmdotcomajax-0.4.9b0/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.0b0/tests/test_device_extensions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,162 +1,138 @@
 """Test device extensions."""
 
+
 import aiohttp
 import pytest
+from aioresponses import aioresponses
 
 from pyalarmdotcomajax import AlarmController
+from pyalarmdotcomajax import const as c
 from pyalarmdotcomajax.cli import _print_element_tearsheet
 from pyalarmdotcomajax.devices.camera import Camera
 from pyalarmdotcomajax.extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOptionType,
     ExtendedProperties,
 )
 
 from .responses import get_http_body_html
 
 
-@pytest.mark.asyncio  # type: ignore
+@pytest.mark.asyncio
 async def test__extension_camera_skybellhd__fetch(
-    all_base_ok_responses: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
     """Ensures that ExtendedProperties objects are created from server response data."""
 
     async with aiohttp.ClientSession() as websession:
-        extension = CameraSkybellControllerExtension(
-            websession=websession, headers={"foo": "bar"}
-        )
+        extension = CameraSkybellControllerExtension(websession=websession, headers={"foo": "bar"})
         configs: list[ExtendedProperties] = await extension.fetch()
 
     assert configs[0].device_name == "Front Doorbell"
     assert configs[0].config_id == "2048"
-    assert (
-        configs[0].settings["indoor-chime"].current_value
-        is CameraSkybellControllerExtension.ChimeOnOff.ON
-    )
+    assert configs[0].settings["indoor-chime"].current_value is CameraSkybellControllerExtension.ChimeOnOff.ON
     assert (
         configs[0].settings["outdoor-chime"].current_value
         is CameraSkybellControllerExtension.ChimeAdjustableVolume.MEDIUM
     )
     assert configs[0].raw_attribs
 
 
-@pytest.mark.asyncio  # type: ignore
+@pytest.mark.asyncio
 async def test__extension_camera_skybellhd__via_alarm_controller(
-    all_base_ok_responses: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
-    """Test whether pyalarmdotcomajax camera objects are properly built when encountering Skybell HD cameras.
-    """
+    """Test whether pyalarmdotcomajax camera objects are properly built when encountering Skybell HD cameras."""
 
     await adc_client.async_update()
 
-    assert adc_client.cameras[0]
+    assert adc_client.devices.cameras["id-camera-skybell"]
 
-    skybell = adc_client.cameras[0]
+    skybell = adc_client.devices.cameras["id-camera-skybell"]
 
     assert skybell.name == "Front Doorbell"
-    assert (
-        skybell.settings["indoor-chime"].current_value
-        is CameraSkybellControllerExtension.ChimeOnOff.ON
-    )
+    assert skybell.settings["indoor-chime"].current_value is CameraSkybellControllerExtension.ChimeOnOff.ON
     assert (
         skybell.settings["outdoor-chime"].current_value
         is CameraSkybellControllerExtension.ChimeAdjustableVolume.MEDIUM
     )
-    assert (
-        skybell.settings["indoor-chime"].option_type
-        is ConfigurationOptionType.BINARY_CHIME
-    )
+    assert skybell.settings["indoor-chime"].option_type is ConfigurationOptionType.BINARY_CHIME
 
 
-@pytest.mark.asyncio  # type: ignore
+@pytest.mark.asyncio
 async def test__extension_camera_skybellhd__cli_tearsheet(
-    all_base_ok_responses: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
     """_print_element_tearsheet will throw exception on failure."""
 
     await adc_client.async_update()
 
-    assert adc_client.cameras[0]
+    assert adc_client.devices.cameras["id-camera-skybell"]
 
-    _print_element_tearsheet(adc_client.cameras[0])
+    _print_element_tearsheet(adc_client.devices.cameras["id-camera-skybell"])
 
 
-# @pytest.mark.asyncio  # type: ignore
+# @pytest.mark.asyncio # type: ignore
 # async def test__extension_camera_skybellhd__change_indoor_chime(
-#     all_base_ok_responses: pytest.fixture,
-#     all_extension_ok_responses: pytest.fixture,
+#     all_base_ok_responses: str,
+#
 #     adc_client: AlarmController,
 # ) -> None:
 #     """_print_element_tearsheet will throw exception on failure."""
 
 
-@pytest.mark.asyncio  # type: ignore
+@pytest.mark.asyncio
 async def test__extension_camera_skybellhd__submit_change(
-    all_base_ok_responses: pytest.fixture,
-    response_mocker: pytest.fixture,
+    all_base_ok_responses: str,
+    response_mocker: aioresponses,
     adc_client: AlarmController,
 ) -> None:
     """Test changing configuration option."""
 
     response_mocker.get(
-        url=CameraSkybellControllerExtension.ENDPOINT,
+        url=CameraSkybellControllerExtension.ENDPOINT.format(c.URL_BASE),
         status=200,
         body=get_http_body_html("camera_settings_skybell"),
         repeat=True,
     )
 
     response_mocker.post(
-        url=CameraSkybellControllerExtension.ENDPOINT,
+        url=CameraSkybellControllerExtension.ENDPOINT.format(c.URL_BASE),
         status=200,
         body=get_http_body_html("camera_settings_skybell_changed"),
     )
 
     await adc_client.async_update()
 
-    camera: Camera = adc_client.cameras[0]
+    camera: Camera = adc_client.devices.cameras["id-camera-skybell"]
 
-    await camera.async_change_setting(
-        "indoor-chime", CameraSkybellControllerExtension.ChimeOnOff.OFF
-    )
+    assert camera.settings["indoor-chime"].current_value == CameraSkybellControllerExtension.ChimeOnOff.ON
 
-    assert (
-        camera.settings["indoor-chime"].current_value
-        is CameraSkybellControllerExtension.ChimeOnOff.OFF
-    )
+    await camera.async_change_setting("indoor-chime", CameraSkybellControllerExtension.ChimeOnOff.OFF)
 
+    assert camera.settings["indoor-chime"].current_value == CameraSkybellControllerExtension.ChimeOnOff.OFF
 
-@pytest.mark.asyncio  # type: ignore
+
+@pytest.mark.asyncio
 async def test__extension_camera_skybellhd__missing_field(
-    all_base_ok_responses: pytest.fixture,
-    skybell_missing_video_quality_field: pytest.fixture,
-    response_mocker: pytest.fixture,
+    skybell_missing_video_quality_field: str,
     adc_client: AlarmController,
 ) -> None:
-    """Ensures that pyalarmdotcomajax skips loading data from Skybell HD if Skybell HD config page has unexpected structure.
-    """
+    """Ensures that pyalarmdotcomajax skips loading data from Skybell HD if Skybell HD config page has unexpected structure."""
 
     await adc_client.async_update()
 
-    assert adc_client.cameras[0]
+    assert adc_client.devices.cameras is not None
 
-    skybell = adc_client.cameras[0]
+    skybell = adc_client.devices.cameras["id-camera-skybell"]
 
     assert skybell.name == "Front Doorbell"
-    assert (
-        skybell.settings["indoor-chime"].current_value
-        is CameraSkybellControllerExtension.ChimeOnOff.ON
-    )
+    assert skybell.settings["indoor-chime"].current_value is CameraSkybellControllerExtension.ChimeOnOff.ON
     assert (
         skybell.settings["outdoor-chime"].current_value
         is CameraSkybellControllerExtension.ChimeAdjustableVolume.MEDIUM
     )
-    assert (
-        skybell.settings["indoor-chime"].option_type
-        is ConfigurationOptionType.BINARY_CHIME
-    )
+    assert skybell.settings["indoor-chime"].option_type is ConfigurationOptionType.BINARY_CHIME
```

### Comparing `pyalarmdotcomajax-0.4.9b0/tests/test_no_permissions.py` & `pyalarmdotcomajax-0.5.0b0/tests/test_controller.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,74 @@
 """Tests for main controller."""
 
 # pylint: disable=protected-access
 
+
+import aiohttp
 import pytest
 
 from pyalarmdotcomajax import AlarmController
-from pyalarmdotcomajax.devices import DeviceType
+from pyalarmdotcomajax.errors import DataFetchFailed
 
 
-@pytest.mark.asyncio  # type: ignore
-async def test__async_get_items_and_subordinates__cameras(
-    camera_no_permissions: pytest.fixture,
-    all_base_ok_responses: pytest.fixture,
+def test_property__initial_state(adc_client: AlarmController) -> None:
+    """Ensure that login data is ingested correctly."""
+    assert adc_client._password == "hunter2"  # noqa: S105
+    assert adc_client._username == "test-username"
+    assert adc_client.two_factor_cookie == "test-cookie"
+    assert isinstance(adc_client._websession, aiohttp.ClientSession)
+
+    assert adc_client.provider_name is None
+    assert adc_client.user_id is None
+
+    assert not adc_client.devices.systems.values()
+    assert not adc_client.devices.partitions.values()
+    assert not adc_client.devices.sensors.values()
+    assert not adc_client.devices.locks.values()
+    assert not adc_client.devices.garage_doors.values()
+    assert not adc_client.devices.image_sensors.values()
+    assert not adc_client.devices.lights.values()
+    assert not adc_client.devices.thermostats.values()
+    assert not adc_client.devices.cameras.values()
+    assert not adc_client.devices.water_sensors.values()
+
+
+@pytest.mark.asyncio
+async def test__device_storage(
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
     """Test for function that fetches item metadata from Alarm.com API."""
 
-    items = await adc_client._async_get_items_and_subordinates(DeviceType.CAMERA)
-
-    assert items == []
-
-
-@pytest.mark.asyncio  # type: ignore
-async def test___async_get_and_build_devices__cameras(
-    camera_no_permissions: pytest.fixture,
-    all_base_ok_responses: pytest.fixture,
-    adc_client: AlarmController,
-) -> None:
-    """Test _async_get_and_build_devices for account without camera service."""
-
-    await adc_client._async_get_and_build_devices([DeviceType.CAMERA])
+    await adc_client.async_update()
 
-    assert adc_client.cameras == []
+    assert adc_client.devices.systems.values()
+    assert adc_client.devices.partitions.values()
+    assert adc_client.devices.sensors.values()
+    assert adc_client.devices.locks.values()
+    assert adc_client.devices.garage_doors.values()
+    assert adc_client.devices.image_sensors.values()
+    assert adc_client.devices.lights.values()
+    assert adc_client.devices.thermostats.values()
+    assert adc_client.devices.water_sensors.values()
 
 
-@pytest.mark.asyncio  # type: ignore
-async def test___async_update__no_permissions(
-    all_base_ok_camera_403: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
+@pytest.mark.asyncio
+async def test___async_update__refresh_failure(
+    device_catalog_no_permissions: str,
     adc_client: AlarmController,
 ) -> None:
-    """Test that 403 for one device type doesn't impede downstream device types from loading.
-    """
+    """Test for when devices initialize but fail to refresh. Ensure that devices are wiped on update failure."""
 
-    await adc_client.async_update()
+    with pytest.raises(DataFetchFailed):
+        await adc_client.async_update()
 
-    assert adc_client.systems
-    assert adc_client.partitions
-    assert adc_client.sensors
-    assert adc_client.locks
-    assert adc_client.garage_doors
-    assert adc_client.image_sensors
-    assert adc_client.lights
-    assert adc_client.thermostats
-    assert not adc_client.cameras
 
-
-@pytest.mark.asyncio  # type: ignore
-async def test___async_update__invalid_endpoint(
-    all_base_ok_camera_404: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
+@pytest.mark.asyncio
+async def test__async_has_image_sensors(
+    image_sensors_no_permission: str,
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
-    """Test that 403 for one device type doesn't impede downstream device types from loading.
-    """
+    """Test for function that fetches image sensor images."""
 
     await adc_client.async_update()
-
-    assert adc_client.systems
-    assert adc_client.partitions
-    assert adc_client.sensors
-    assert adc_client.locks
-    assert adc_client.garage_doors
-    assert adc_client.image_sensors
-    assert adc_client.lights
-    assert adc_client.thermostats
-    assert not adc_client.cameras
```

### Comparing `pyalarmdotcomajax-0.4.9b0/tests/test_partition.py` & `pyalarmdotcomajax-0.5.0b0/tests/test_partition.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,52 +5,78 @@
 import pytest
 
 from pyalarmdotcomajax import AlarmController
 from pyalarmdotcomajax.cli import _print_element_tearsheet
 from pyalarmdotcomajax.devices.partition import Partition
 
 
-@pytest.mark.asyncio  # type: ignore
-async def test__device_partition__ok(
-    all_base_ok_responses: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
-    response_mocker: pytest.fixture,
+@pytest.mark.asyncio
+async def test__device_partition__house__ok(
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
     """Ensures that partitions load correctly."""
 
     await adc_client.async_update()
 
-    assert adc_client.partitions[0]
+    assert adc_client.devices.partitions["id-partition-house"]
 
-    partition = adc_client.partitions[0]
+    partition = adc_client.devices.partitions["id-partition-house"]
 
     assert partition is not None
-    assert partition.name == "Alarm"
+    assert partition.name == "House"
 
     assert partition.attributes is not None
 
     if partition.attributes.extended_arming_options is not None:
         # Counter allows for comparing lists while ignoring order.
-        assert Counter(
-            partition.attributes.extended_arming_options.armed_away
-        ) == Counter(
+        assert Counter(partition.attributes.extended_arming_options.arm_away) == Counter(
             [
                 Partition.ExtendedArmingOption.NO_ENTRY_DELAY,
                 Partition.ExtendedArmingOption.SILENT_ARMING,
+                Partition.ExtendedArmingOption.BYPASS_SENSORS,
+                Partition.ExtendedArmingOption.SELECTIVE_BYPASS,
             ]
         )
 
 
-@pytest.mark.asyncio  # type: ignore
+@pytest.mark.asyncio
+async def test__device_partition__garage__ok(
+    all_base_ok_responses: str,
+    response_mocker: str,
+    adc_client: AlarmController,
+) -> None:
+    """Ensures that partitions load correctly."""
+
+    await adc_client.async_update()
+
+    assert adc_client.devices.partitions["id-partition-detached_garage"]
+
+    partition = adc_client.devices.partitions["id-partition-detached_garage"]
+
+    assert partition is not None
+    assert partition.name == "Detached Garage"
+
+    assert partition.attributes is not None
+
+    if partition.attributes.extended_arming_options is not None:
+        # Counter allows for comparing lists while ignoring order.
+        assert Counter(partition.attributes.extended_arming_options.arm_away) == Counter(
+            [
+                Partition.ExtendedArmingOption.NO_ENTRY_DELAY,
+                Partition.ExtendedArmingOption.SILENT_ARMING,
+            ]
+        )
+
+
+@pytest.mark.asyncio
 async def test__device_partition__cli_tearsheet(
-    all_base_ok_responses: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
     """_print_element_tearsheet will throw exception on failure."""
 
     await adc_client.async_update()
 
-    assert adc_client.partitions[0]
+    assert len(adc_client.devices.partitions) == 2
 
-    _print_element_tearsheet(adc_client.partitions[0])
+    _print_element_tearsheet(adc_client.devices.partitions["id-partition-house"])
```

### Comparing `pyalarmdotcomajax-0.4.9b0/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.0b0/tests/test_thermostat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Test thermostat device."""
 
+
 import pytest
 
 from pyalarmdotcomajax import AlarmController
 from pyalarmdotcomajax.cli import _print_element_tearsheet
 from pyalarmdotcomajax.devices.thermostat import Thermostat
 
 
-@pytest.mark.asyncio  # type: ignore
+@pytest.mark.asyncio
 async def test__device_thermostat__ok(
-    all_base_ok_responses: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
-    response_mocker: pytest.fixture,
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
     """Ensures that thermostats load correctly."""
 
     await adc_client.async_update()
 
-    assert adc_client.thermostats[0]
+    assert adc_client.devices.thermostats["id-tstat-upstairs"]
 
-    thermostat = adc_client.thermostats[0]
+    thermostat = adc_client.devices.thermostats["id-tstat-upstairs"]
 
     assert thermostat is not None
     assert thermostat.name == "Upstairs"
 
     assert thermostat.attributes is not None
     assert thermostat.attributes.temp_at_tstat == 72
     assert thermostat.attributes.temp_average == 72
@@ -48,20 +47,19 @@
     assert thermostat.attributes.supports_humidity is False
     assert thermostat.attributes.humidity == 69
     assert thermostat.attributes.supports_schedules is True
     assert thermostat.attributes.supports_schedules_smart is False
     assert thermostat.attributes.schedule_mode == Thermostat.ScheduleMode.SCHEDULED
 
 
-@pytest.mark.asyncio  # type: ignore
+@pytest.mark.asyncio
 async def test__device_thermostat__cli_tearsheet(
-    all_base_ok_responses: pytest.fixture,
-    all_extension_ok_responses: pytest.fixture,
+    all_base_ok_responses: str,
     adc_client: AlarmController,
 ) -> None:
     """_print_element_tearsheet will throw exception on failure."""
 
     await adc_client.async_update()
 
-    assert adc_client.thermostats[0]
+    assert adc_client.devices.thermostats["id-tstat-upstairs"]
 
-    _print_element_tearsheet(adc_client.thermostats[0])
+    _print_element_tearsheet(adc_client.devices.thermostats["id-tstat-upstairs"])
```

