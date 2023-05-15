# Comparing `tmp/hahomematic-2023.5.1.tar.gz` & `tmp/hahomematic-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.5.1.tar", last modified: Sat May 13 11:35:13 2023, max compression
+gzip compressed data, was "hahomematic-2023.5.2.tar", last modified: Mon May 15 13:36:19 2023, max compression
```

## Comparing `hahomematic-2023.5.1.tar` & `hahomematic-2023.5.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.251598 hahomematic-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-13 11:35:13.251598 hahomematic-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.235598 hahomematic-2023.5.1/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.239598 hahomematic-2023.5.1/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24401 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    50182 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    45773 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14403 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.239598 hahomematic-2023.5.1/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.243598 hahomematic-2023.5.1/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    33824 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.247598 hahomematic-2023.5.1/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.251598 hahomematic-2023.5.1/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.251598 hahomematic-2023.5.1/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:35:13.239598 hahomematic-2023.5.1/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-13 11:35:12.000000 hahomematic-2023.5.1/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-13 11:35:13.000000 hahomematic-2023.5.1/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:35:12.000000 hahomematic-2023.5.1/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:35:10.000000 hahomematic-2023.5.1/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-13 11:35:12.000000 hahomematic-2023.5.1/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-13 11:35:13.000000 hahomematic-2023.5.1/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-13 11:34:37.000000 hahomematic-2023.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-13 11:35:13.251598 hahomematic-2023.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.497626 hahomematic-2023.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-15 13:36:19.497626 hahomematic-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.489626 hahomematic-2023.5.2/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.489626 hahomematic-2023.5.2/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24401 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50693 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46635 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14403 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.489626 hahomematic-2023.5.2/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.493626 hahomematic-2023.5.2/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33824 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24859 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.493626 hahomematic-2023.5.2/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.493626 hahomematic-2023.5.2/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.497626 hahomematic-2023.5.2/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:19.489626 hahomematic-2023.5.2/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-15 13:36:18.000000 hahomematic-2023.5.2/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-15 13:36:19.000000 hahomematic-2023.5.2/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:36:18.000000 hahomematic-2023.5.2/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:36:17.000000 hahomematic-2023.5.2/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 13:36:19.000000 hahomematic-2023.5.2/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 13:36:19.000000 hahomematic-2023.5.2/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-15 13:35:37.000000 hahomematic-2023.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 13:36:19.497626 hahomematic-2023.5.2/setup.cfg
```

### Comparing `hahomematic-2023.5.1/LICENSE` & `hahomematic-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/PKG-INFO` & `hahomematic-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.5.1/README.md` & `hahomematic-2023.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/__init__.py` & `hahomematic-2023.5.2/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/backport.py` & `hahomematic-2023.5.2/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/caches/dynamic.py` & `hahomematic-2023.5.2/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/caches/persistent.py` & `hahomematic-2023.5.2/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/caches/visibility.py` & `hahomematic-2023.5.2/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/central_unit.py` & `hahomematic-2023.5.2/hahomematic/central_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     HH_EVENT_LIST_DEVICES,
     HH_EVENT_NEW_DEVICES,
     HM_ADDRESS,
     IF_PRIMARY,
     LOCAL_INTERFACE,
     MAX_CACHE_AGE,
     PROXY_INIT_SUCCESS,
+    HmDeviceFirmwareState,
     HmEntityUsage,
     HmEventType,
     HmInterfaceEventType,
     HmPlatform,
 )
 from hahomematic.decorators import (
     async_callback_system_event,
@@ -281,14 +282,25 @@
             device.refresh_firmware_data()
         else:
             for client in self._clients.values():
                 await self._refresh_device_descriptions(client=client)
             for device in self._devices.values():
                 device.refresh_firmware_data()
 
+    async def refresh_firmware_data_by_state(
+        self, device_firmware_states: tuple[HmDeviceFirmwareState, ...]
+    ) -> None:
+        """Refresh device firmware data for processing devices."""
+        for device in [
+            device_in_state
+            for device_in_state in self._devices.values()
+            if device_in_state.firmware_update_state in device_firmware_states
+        ]:
+            await self.refresh_firmware_data(device_address=device.device_address)
+
     async def _refresh_device_descriptions(
         self, client: hmcl.Client, device_address: str | None = None
     ) -> None:
         """Refresh device descriptions."""
         if (
             device_descriptions := await client.get_device_descriptions(
                 device_address=device_address
```

### Comparing `hahomematic-2023.5.1/hahomematic/client.py` & `hahomematic-2023.5.2/hahomematic/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,20 +586,41 @@
                 )
             )
         return all_paramsets
 
     async def update_device_firmware(self, device_address: str) -> bool:
         """Update the firmware of a homematic device."""
         if device := self.central.get_device(device_address=device_address):
-            return bool(
-                await self._proxy.installFirmware(device_address)
-                if device.product_group in (HmProductGroup.HMIPW, HmProductGroup.HMIP)
-                else await self._proxy.updateFirmware(device_address)
+            _LOGGER.info(
+                "UPDATE_DEVICE_FIRMWARE: Trying firmware update for %s",
+                device_address,
             )
-
+            try:
+                update_result = (
+                    await self._proxy.installFirmware(device_address)
+                    if device.product_group in (HmProductGroup.HMIPW, HmProductGroup.HMIP)
+                    else await self._proxy.updateFirmware(device_address)
+                )
+                result = (
+                    bool(update_result)
+                    if isinstance(update_result, bool)
+                    else bool(update_result[0])
+                )
+                _LOGGER.info(
+                    "UPDATE_DEVICE_FIRMWARE: Executed firmware update for %s with result '%s'",
+                    device_address,
+                    "success" if result else "failed",
+                )
+                return result
+            except BaseHomematicException as bex:
+                _LOGGER.warning(
+                    "UPDATE_DEVICE_FIRMWARE failed: %s [%s]",
+                    bex.name,
+                    bex.args,
+                )
         return False
 
     async def update_paramset_descriptions(self, device_address: str) -> None:
         """Update paramsets descriptions for provided device_address."""
         if not self.central.device_descriptions.get_device_descriptions(
             interface_id=self.interface_id
         ):
```

### Comparing `hahomematic-2023.5.1/hahomematic/const.py` & `hahomematic-2023.5.2/hahomematic/const.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -346,22 +346,22 @@
     EVENT: Final = "event"
 
 
 class HmDeviceFirmwareState(StrEnum):
     """Enum with homematic device firmware states."""
 
     UP_TO_DATE: Final = "UP_TO_DATE"
+    LIVE_UP_TO_DATE: Final = "LIVE_UP_TO_DATE"
     NEW_FIRMWARE_AVAILABLE: Final = "NEW_FIRMWARE_AVAILABLE"
+    LIVE_NEW_FIRMWARE_AVAILABLE: Final = "LIVE_NEW_FIRMWARE_AVAILABLE"
     DELIVER_FIRMWARE_IMAGE: Final = "DELIVER_FIRMWARE_IMAGE"
+    LIVE_DELIVER_FIRMWARE_IMAGE: Final = "LIVE_DELIVER_FIRMWARE_IMAGE"
     READY_FOR_UPDATE: Final = "READY_FOR_UPDATE"
     DO_UPDATE_PENDING: Final = "DO_UPDATE_PENDING"
     PERFORMING_UPDATE: Final = "PERFORMING_UPDATE"
-    LIVE_UP_TO_DATE: Final = "LIVE_UP_TO_DATE"
-    LIVE_NEW_FIRMWARE_AVAILABLE: Final = "LIVE_NEW_FIRMWARE_AVAILABLE"
-    LIVE_DELIVER_FIRMWARE_IMAGE: Final = "LIVE_DELIVER_FIRMWARE_IMAGE"
 
 
 class HmPlatform(StrEnum):
     """Enum with platforms relevant for Home Assistant."""
 
     ACTION: Final = "action"
     BINARY_SENSOR: Final = "binary_sensor"
```

### Comparing `hahomematic-2023.5.1/hahomematic/decorators.py` & `hahomematic-2023.5.2/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/exceptions.py` & `hahomematic-2023.5.2/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/exporter.py` & `hahomematic-2023.5.2/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/hmcli.py` & `hahomematic-2023.5.2/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/json_rpc_client.py` & `hahomematic-2023.5.2/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/__init__.py` & `hahomematic-2023.5.2/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/const.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/light.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/support.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.5.2/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/device.py` & `hahomematic-2023.5.2/hahomematic/platforms/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -390,17 +390,29 @@
             or old_firmware != self._attr_firmware
             or old_firmware_update_state != self._attr_firmware_update_state
             or old_firmware_updatable != self._attr_firmware_updatable
         ):
             for _firmware_callback in self._firmware_update_callbacks:
                 _firmware_callback()
 
-    async def update_firmware(self) -> bool:
+    async def update_firmware(self, refresh_after_update_intervals: tuple[int, ...]) -> bool:
         """Update the firmware of the homematic device."""
-        return await self.client.update_device_firmware(device_address=self._attr_device_address)
+        update_result = await self.client.update_device_firmware(
+            device_address=self._attr_device_address
+        )
+
+        async def refresh_data() -> None:
+            for refresh_interval in refresh_after_update_intervals:
+                await asyncio.sleep(refresh_interval)
+                await self.central.refresh_firmware_data(device_address=self._attr_device_address)
+
+        if refresh_after_update_intervals:
+            self.central.create_task(target=refresh_data(), name="refresh_firmware_data")
+
+        return update_result
 
     async def load_value_cache(self) -> None:
         """Init the parameter cache."""
         if len(self.generic_entities) > 0:
             await self.value_cache.init_base_entities()
         if len(self.events) > 0:
             await self.value_cache.init_readable_events()
```

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/entity.py` & `hahomematic-2023.5.2/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/event.py` & `hahomematic-2023.5.2/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/action.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/button.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/number.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/select.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.5.2/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.5.2/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.5.2/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/hub/button.py` & `hahomematic-2023.5.2/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.5.2/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/hub/number.py` & `hahomematic-2023.5.2/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/hub/select.py` & `hahomematic-2023.5.2/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.5.2/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/hub/text.py` & `hahomematic-2023.5.2/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/support.py` & `hahomematic-2023.5.2/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/platforms/update.py` & `hahomematic-2023.5.2/hahomematic/platforms/update.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         """Register update callback."""
         self.device.register_firmware_update_callback(update_callback)
 
     def unregister_update_callback(self, update_callback: Callable) -> None:
         """Unregister update callback."""
         self.device.unregister_firmware_update_callback(update_callback)
 
-    async def update_firmware(self) -> None:
+    async def update_firmware(self, refresh_after_update_intervals: tuple[int, ...]) -> bool:
         """Turn the update on."""
-        await self.device.update_firmware()
+        return await self.device.update_firmware(
+            refresh_after_update_intervals=refresh_after_update_intervals
+        )
 
     async def refresh_firmware_data(self) -> None:
         """Refresh device firmware data."""
         await self.device.central.refresh_firmware_data(device_address=self.device.device_address)
```

### Comparing `hahomematic-2023.5.1/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.5.2/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.5.2/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.5.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/support.py` & `hahomematic-2023.5.2/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.5.2/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic/xml_rpc_server.py` & `hahomematic-2023.5.2/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.5.2/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.5.1/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.5.2/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.5.1/pyproject.toml` & `hahomematic-2023.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.5.1"
+version     = "2023.5.2"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

