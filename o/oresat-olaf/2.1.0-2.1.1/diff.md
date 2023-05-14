# Comparing `tmp/oresat-olaf-2.1.0.tar.gz` & `tmp/oresat-olaf-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-olaf-2.1.0.tar", last modified: Sun May  7 20:22:13 2023, max compression
+gzip compressed data, was "oresat-olaf-2.1.1.tar", last modified: Sun May 14 22:52:13 2023, max compression
```

## Comparing `oresat-olaf-2.1.0.tar` & `oresat-olaf-2.1.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.791717 oresat-olaf-2.1.0/olaf/
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.791717 oresat-olaf-2.1.0/olaf/_internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.791717 oresat-olaf-2.1.0/olaf/_internals/data/
--rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/data/oresat_app.eds
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/master_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.795717 oresat-olaf-2.1.0/olaf/_internals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/file_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/fread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/fwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/os_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/power_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/store_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.795717 oresat-olaf-2.1.0/olaf/_internals/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.799717 oresat-olaf-2.1.0/olaf/_internals/rest_api/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.799717 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/fread.html
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/fwrite.html
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/od.html
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/os_command.html
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/power_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/root.html
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/system_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/updater.html
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.803717 oresat-olaf-2.1.0/olaf/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/cpufreq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/timer_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.807718 oresat-olaf-2.1.0/olaf/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2478 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/file_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/new_eds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1208 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/os_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/sdo_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3537 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.807718 oresat-olaf-2.1.0/oresat_olaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-07 20:22:13.815718 oresat-olaf-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.807718 oresat-olaf-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.807718 oresat-olaf-2.1.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/test_oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/test_oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/tests/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/tests/internals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_file_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_fread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_fwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_os_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/test_rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/tests/internals/updater/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.168002 oresat-olaf-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-14 22:52:13.168002 oresat-olaf-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.160002 oresat-olaf-2.1.1/olaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.160002 oresat-olaf-2.1.1/olaf/_internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.160002 oresat-olaf-2.1.1/olaf/_internals/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/data/oresat_app.eds
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.160002 oresat-olaf-2.1.1/olaf/_internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/power_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/store_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/resources/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.160002 oresat-olaf-2.1.1/olaf/_internals/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.160002 oresat-olaf-2.1.1/olaf/_internals/rest_api/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.164002 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/fread.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/fwrite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/od.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/os_command.html
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/power_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/root.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/system_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/updater.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/_internals/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.164002 oresat-olaf-2.1.1/olaf/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/common/cpufreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/common/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/common/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/common/oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/common/oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/common/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/common/timer_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.164002 oresat-olaf-2.1.1/olaf/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2478 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/scripts/file_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/scripts/new_eds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1208 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/scripts/os_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/scripts/sdo_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/scripts/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3537 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/olaf/scripts/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.164002 oresat-olaf-2.1.1/oresat_olaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-14 22:52:13.000000 oresat-olaf-2.1.1/oresat_olaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-14 22:52:13.000000 oresat-olaf-2.1.1/oresat_olaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:52:13.000000 oresat-olaf-2.1.1/oresat_olaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-14 22:52:13.000000 oresat-olaf-2.1.1/oresat_olaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 22:52:13.000000 oresat-olaf-2.1.1/oresat_olaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 22:52:13.000000 oresat-olaf-2.1.1/oresat_olaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-14 22:52:13.168002 oresat-olaf-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.164002 oresat-olaf-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.164002 oresat-olaf-2.1.1/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/common/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/common/test_oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/common/test_oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/common/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.164002 oresat-olaf-2.1.1/tests/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.164002 oresat-olaf-2.1.1/tests/internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/resources/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/resources/test_file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/resources/test_fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/resources/test_fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/resources/test_os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/resources/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/test_rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:13.168002 oresat-olaf-2.1.1/tests/internals/updater/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-14 22:52:00.000000 oresat-olaf-2.1.1/tests/internals/updater/test_updater.py
```

### Comparing `oresat-olaf-2.1.0/LICENSE` & `oresat-olaf-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/PKG-INFO` & `oresat-olaf-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 2.1.0
+Version: 2.1.1
 Summary: Application framework for all OreSat Linux boards
 Home-page: https://github.com/oresat/oresat-olaf
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-olaf-2.1.0/README.rst` & `oresat-olaf-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/__init__.py` & `oresat-olaf-2.1.1/olaf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .common.resource import Resource
 from .common.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
 from .common.oresat_file import OreSatFile, new_oresat_file
 from .common.oresat_file_cache import OreSatFileCache
 from .common.timer_loop import TimerLoop
 from .common.gpio import GPIO
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 def olaf_setup(eds_path: str = None, master_node: bool = False) -> Namespace:
     '''
     Parse runtime args and setup the app and REST API.
 
     Parameters
```

### Comparing `oresat-olaf-2.1.0/olaf/_internals/app.py` & `oresat-olaf-2.1.1/olaf/_internals/app.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/data/oresat_app.eds` & `oresat-olaf-2.1.1/olaf/_internals/data/oresat_app.eds`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/master_node.py` & `oresat-olaf-2.1.1/olaf/_internals/master_node.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/node.py` & `oresat-olaf-2.1.1/olaf/_internals/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,17 @@
 
         if self.first_bus_reset:
             logger.error(f'{self._bus} is down')
 
         if geteuid() == 0:  # running as root
             if self.first_bus_reset:
                 logger.info(f'trying to restart CAN bus {self._bus}')
-            cmd = f'ip link set {self._bus} down;ip link set {self._bus} up'
+            cmd = (f'ip link set {self._bus} down;'
+                   f'ip link set {self._bus} type can bitrate 1000000;'
+                   f'ip link set {self._bus} up')
             out = subprocess.run(cmd, shell=True)
             if out.returncode != 0:
                 logger.error(out)
 
         self.first_bus_reset = False
 
     def _restart_network(self):
```

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/ecss.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/file_caches.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/file_caches.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/fread.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/fread.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/fwrite.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/logs.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/logs.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/os_command.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/power_control.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/power_control.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/store_eds.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/store_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/system_info.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/resources/updater.py` & `oresat-olaf-2.1.1/olaf/_internals/resources/updater.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/__init__.py` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/static/favicon.ico` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/base.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/base.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/fread.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/fread.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/fwrite.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/fwrite.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/logs.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/logs.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/od.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/od.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/os_command.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/os_command.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/power_control.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/power_control.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/system_info.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/system_info.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/updater.html` & `oresat-olaf-2.1.1/olaf/_internals/rest_api/templates/updater.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/_internals/updater.py` & `oresat-olaf-2.1.1/olaf/_internals/updater.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/common/cpufreq.py` & `oresat-olaf-2.1.1/olaf/common/cpufreq.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/common/ecss.py` & `oresat-olaf-2.1.1/olaf/common/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/common/gpio.py` & `oresat-olaf-2.1.1/olaf/common/gpio.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/common/oresat_file.py` & `oresat-olaf-2.1.1/olaf/common/oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/common/oresat_file_cache.py` & `oresat-olaf-2.1.1/olaf/common/oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/common/resource.py` & `oresat-olaf-2.1.1/olaf/common/resource.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/common/timer_loop.py` & `oresat-olaf-2.1.1/olaf/common/timer_loop.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/scripts/file_transfer.py` & `oresat-olaf-2.1.1/olaf/scripts/file_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/scripts/new_eds.py` & `oresat-olaf-2.1.1/olaf/scripts/new_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/scripts/os_command.py` & `oresat-olaf-2.1.1/olaf/scripts/os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/scripts/sdo_transfer.py` & `oresat-olaf-2.1.1/olaf/scripts/sdo_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/olaf/scripts/system_info.py` & `oresat-olaf-2.1.1/olaf/scripts/system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/oresat_olaf.egg-info/PKG-INFO` & `oresat-olaf-2.1.1/oresat_olaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 2.1.0
+Version: 2.1.1
 Summary: Application framework for all OreSat Linux boards
 Home-page: https://github.com/oresat/oresat-olaf
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-olaf-2.1.0/oresat_olaf.egg-info/SOURCES.txt` & `oresat-olaf-2.1.1/oresat_olaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/setup.cfg` & `oresat-olaf-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/common/test_ecss.py` & `oresat-olaf-2.1.1/tests/common/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/common/test_oresat_file.py` & `oresat-olaf-2.1.1/tests/common/test_oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/common/test_oresat_file_cache.py` & `oresat-olaf-2.1.1/tests/common/test_oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/common/test_resources.py` & `oresat-olaf-2.1.1/tests/common/test_resources.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/internals/resources/__init__.py` & `oresat-olaf-2.1.1/tests/internals/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/internals/resources/test_file_caches.py` & `oresat-olaf-2.1.1/tests/internals/resources/test_file_caches.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/internals/resources/test_fread.py` & `oresat-olaf-2.1.1/tests/internals/resources/test_fread.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/internals/resources/test_fwrite.py` & `oresat-olaf-2.1.1/tests/internals/resources/test_fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/internals/resources/test_os_command.py` & `oresat-olaf-2.1.1/tests/internals/resources/test_os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/internals/resources/test_system_info.py` & `oresat-olaf-2.1.1/tests/internals/resources/test_system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/internals/test_rest_api.py` & `oresat-olaf-2.1.1/tests/internals/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.0/tests/internals/updater/test_updater.py` & `oresat-olaf-2.1.1/tests/internals/updater/test_updater.py`

 * *Files identical despite different names*

