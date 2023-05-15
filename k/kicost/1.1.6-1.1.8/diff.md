# Comparing `tmp/kicost-1.1.6.tar.gz` & `tmp/kicost-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kicost-1.1.6.tar", last modified: Tue Oct 12 18:26:24 2021, max compression
+gzip compressed data, was "dist/kicost-1.1.8.tar", last modified: Mon May  9 17:01:35 2022, max compression
```

## Comparing `kicost-1.1.6.tar` & `kicost-1.1.8.tar`

### file list

```diff
@@ -1,78 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 18:26:24.000000 kicost-1.1.6/
--rw-rw-r--   0 root         (0) root         (0)     3257 2021-10-12 18:25:12.000000 kicost-1.1.6/CONTRIBUTING.rst
--rw-rw-r--   0 root         (0) root         (0)     1104 2021-10-12 18:25:12.000000 kicost-1.1.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      379 2021-10-12 18:25:12.000000 kicost-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5071 2021-10-12 18:26:24.000000 kicost-1.1.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2259 2021-10-12 18:25:12.000000 kicost-1.1.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 18:26:24.000000 kicost-1.1.6/docs/
--rw-rw-r--   0 root         (0) root         (0)     6939 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/Makefile
--rw-rw-r--   0 root         (0) root         (0)       36 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/authors.rst
--rw-rw-r--   0 root         (0) root         (0)   117291 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/block_diag.png
--rw-rw-r--   0 root         (0) root         (0)     8714 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/conf.py
--rw-rw-r--   0 root         (0) root         (0)       34 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/contributing.rst
--rw-rw-r--   0 root         (0) root         (0)    54286 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/gui.png
--rw-rw-r--   0 root         (0) root         (0)       36 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/history.rst
--rw-rw-r--   0 root         (0) root         (0)      510 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/index.rst
--rw-rw-r--   0 root         (0) root         (0)     2436 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/installation.rst
--rw-rw-r--   0 root         (0) root         (0)     1087 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/kicost.currency_converter.rst
--rw-rw-r--   0 root         (0) root         (0)     1183 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/kicost.distributors.rst
--rw-rw-r--   0 root         (0) root         (0)      791 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/kicost.edas.rst
--rw-rw-r--   0 root         (0) root         (0)     1958 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/kicost.rst
--rw-rw-r--   0 root         (0) root         (0)     6701 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/make.bat
--rw-rw-r--   0 root         (0) root         (0)       55 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/modules.rst
--rw-rw-r--   0 root         (0) root         (0)       28 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/readme.rst
--rw-rw-r--   0 root         (0) root         (0)    21371 2021-10-12 18:25:12.000000 kicost-1.1.6/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost/
--rw-rw-r--   0 root         (0) root         (0)      786 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/AUTHORS.rst
--rw-rw-r--   0 root         (0) root         (0)    17649 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/HISTORY.rst
--rw-rw-r--   0 root         (0) root         (0)     2073 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    19623 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/ansi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost/currency_converter/
--rw-rw-r--   0 root         (0) root         (0)       89 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/currency_converter/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3165 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/currency_converter/currency_converter.py
--rw-rw-r--   0 root         (0) root         (0)     2609 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/currency_converter/currency_tables.py
--rw-rw-r--   0 root         (0) root         (0)     1152 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/currency_converter/default_rates.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/currency_converter/download_rates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost/distributors/
--rw-rw-r--   0 root         (0) root         (0)     3348 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/distributors/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    21913 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/distributors/api_octopart.py
--rw-rw-r--   0 root         (0) root         (0)    17527 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/distributors/api_partinfo_kitspace.py
--rw-rw-r--   0 root         (0) root         (0)     7394 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/distributors/dist_local_template.py
--rw-rw-r--   0 root         (0) root         (0)     6956 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/distributors/distributor.py
--rw-rw-r--   0 root         (0) root         (0)     6605 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/distributors/distributors_info.py
--rw-rw-r--   0 root         (0) root         (0)     2112 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/distributors/global_vars.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost/edas/
--rw-rw-r--   0 root         (0) root         (0)     2388 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/edas/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11750 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/edas/eda.py
--rw-rw-r--   0 root         (0) root         (0)     6964 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/edas/eda_altium.py
--rw-rw-r--   0 root         (0) root         (0)     6958 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/edas/eda_kicad.py
--rw-rw-r--   0 root         (0) root         (0)    10028 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/edas/generic_csv.py
--rw-rw-r--   0 root         (0) root         (0)    43248 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/edas/tools.py
--rw-rw-r--   0 root         (0) root         (0)     3827 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/global_vars.py
--rw-rw-r--   0 root         (0) root         (0)    11777 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/kicad_config.py
--rw-rw-r--   0 root         (0) root         (0)    67646 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/kicost.ico
--rw-rw-r--   0 root         (0) root         (0)    15733 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/kicost.py
--rw-rw-r--   0 root         (0) root         (0)    14436 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/kicost_config.py
--rw-rw-r--   0 root         (0) root         (0)    62977 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/kicost_gui.py
--rw-rw-r--   0 root         (0) root         (0)     3614 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/kicost_kicadplugin.py
--rw-rw-r--   0 root         (0) root         (0)    18928 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/kitspace.png
--rw-rw-r--   0 root         (0) root         (0)     6778 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/log.py
--rw-rw-r--   0 root         (0) root         (0)     6036 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/os_windows.py
--rw-rw-r--   0 root         (0) root         (0)    18726 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/sexpdata.py
--rw-rw-r--   0 root         (0) root         (0)    68887 2021-10-12 18:25:12.000000 kicost-1.1.6/kicost/spreadsheet.py
--rw-rw-r--   0 root         (0) root         (0)       44 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5071 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1644 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      126 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-10-12 18:26:24.000000 kicost-1.1.6/kicost.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      133 2021-10-12 18:26:24.000000 kicost-1.1.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     6528 2021-10-12 18:25:12.000000 kicost-1.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 18:26:24.000000 kicost-1.1.6/tests/
--rw-rw-r--   0 root         (0) root         (0)       25 2021-10-12 18:25:12.000000 kicost-1.1.6/tests/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     6555 2021-10-12 18:25:12.000000 kicost-1.1.6/tests/dummy-web-server.py
--rw-rw-r--   0 root         (0) root         (0)    23972 2021-10-12 18:25:12.000000 kicost-1.1.6/tests/test_kicost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 17:01:35.000000 kicost-1.1.8/
+-rw-rw-r--   0 root         (0) root         (0)     3257 2022-05-09 17:00:50.000000 kicost-1.1.8/CONTRIBUTING.rst
+-rw-rw-r--   0 root         (0) root         (0)     1104 2022-05-09 17:00:50.000000 kicost-1.1.8/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      405 2022-05-09 17:00:50.000000 kicost-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4996 2022-05-09 17:01:35.000000 kicost-1.1.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2259 2022-05-09 17:00:50.000000 kicost-1.1.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 17:01:35.000000 kicost-1.1.8/docs/
+-rw-rw-r--   0 root         (0) root         (0)     6939 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/Makefile
+-rw-rw-r--   0 root         (0) root         (0)       36 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/authors.rst
+-rw-rw-r--   0 root         (0) root         (0)   117291 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/block_diag.png
+-rw-rw-r--   0 root         (0) root         (0)     8714 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/conf.py
+-rw-rw-r--   0 root         (0) root         (0)     4023 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/configuration.rst
+-rw-rw-r--   0 root         (0) root         (0)       34 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/contributing.rst
+-rw-rw-r--   0 root         (0) root         (0)    54286 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/gui.png
+-rw-rw-r--   0 root         (0) root         (0)       36 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/history.rst
+-rw-rw-r--   0 root         (0) root         (0)      527 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/index.rst
+-rw-rw-r--   0 root         (0) root         (0)     2436 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/installation.rst
+-rw-rw-r--   0 root         (0) root         (0)     1087 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/kicost.currency_converter.rst
+-rw-rw-r--   0 root         (0) root         (0)     1183 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/kicost.distributors.rst
+-rw-rw-r--   0 root         (0) root         (0)      791 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/kicost.edas.rst
+-rw-rw-r--   0 root         (0) root         (0)     2215 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/kicost.rst
+-rw-rw-r--   0 root         (0) root         (0)     6701 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/make.bat
+-rw-rw-r--   0 root         (0) root         (0)       55 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/modules.rst
+-rw-rw-r--   0 root         (0) root         (0)       28 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/readme.rst
+-rw-rw-r--   0 root         (0) root         (0)    21371 2022-05-09 17:00:50.000000 kicost-1.1.8/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost/
+-rw-rw-r--   0 root         (0) root         (0)      786 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/AUTHORS.rst
+-rw-rw-r--   0 root         (0) root         (0)    17848 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/HISTORY.rst
+-rw-rw-r--   0 root         (0) root         (0)     1457 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22319 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)     2428 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/ansi.py
+-rw-rw-r--   0 root         (0) root         (0)     6509 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost/currency_converter/
+-rw-rw-r--   0 root         (0) root         (0)       89 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/currency_converter/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3165 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/currency_converter/currency_converter.py
+-rw-rw-r--   0 root         (0) root         (0)     2533 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/currency_converter/currency_tables.py
+-rw-rw-r--   0 root         (0) root         (0)     1118 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/currency_converter/default_rates.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/currency_converter/download_rates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost/distributors/
+-rw-rw-r--   0 root         (0) root         (0)     4047 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9945 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/api_digikey.py
+-rw-rw-r--   0 root         (0) root         (0)    19172 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/api_element14.py
+-rw-rw-r--   0 root         (0) root         (0)    13417 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/api_mouser.py
+-rw-rw-r--   0 root         (0) root         (0)    23601 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/api_octopart.py
+-rw-rw-r--   0 root         (0) root         (0)    19747 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/api_partinfo_kitspace.py
+-rw-rw-r--   0 root         (0) root         (0)    19493 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/api_tme.py
+-rw-rw-r--   0 root         (0) root         (0)     7844 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/dist_local_template.py
+-rw-rw-r--   0 root         (0) root         (0)    10982 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/distributor.py
+-rw-rw-r--   0 root         (0) root         (0)     6605 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/distributors_info.py
+-rw-rw-r--   0 root         (0) root         (0)     2112 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/global_vars.py
+-rw-rw-r--   0 root         (0) root         (0)     1875 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/distributors/log__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost/edas/
+-rw-rw-r--   0 root         (0) root         (0)     2388 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/edas/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11781 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/edas/eda.py
+-rw-rw-r--   0 root         (0) root         (0)     6881 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/edas/eda_altium.py
+-rw-rw-r--   0 root         (0) root         (0)     6855 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/edas/eda_kicad.py
+-rw-rw-r--   0 root         (0) root         (0)     9897 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/edas/generic_csv.py
+-rw-rw-r--   0 root         (0) root         (0)     1803 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/edas/log__.py
+-rw-rw-r--   0 root         (0) root         (0)    42461 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/edas/tools.py
+-rw-rw-r--   0 root         (0) root         (0)     5407 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/global_vars.py
+-rw-rw-r--   0 root         (0) root         (0)    11790 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/kicad_config.py
+-rw-rw-r--   0 root         (0) root         (0)    67646 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/kicost.ico
+-rw-rw-r--   0 root         (0) root         (0)    16584 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/kicost.py
+-rw-rw-r--   0 root         (0) root         (0)    14148 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/kicost_config.py
+-rw-rw-r--   0 root         (0) root         (0)    62818 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/kicost_gui.py
+-rw-rw-r--   0 root         (0) root         (0)     3614 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/kicost_kicadplugin.py
+-rw-rw-r--   0 root         (0) root         (0)    18928 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/kitspace.png
+-rw-rw-r--   0 root         (0) root         (0)     7719 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/log.py
+-rw-rw-r--   0 root         (0) root         (0)     2614 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/log__.py
+-rw-rw-r--   0 root         (0) root         (0)     5984 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/os_windows.py
+-rw-rw-r--   0 root         (0) root         (0)    18726 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/sexpdata.py
+-rw-rw-r--   0 root         (0) root         (0)    68975 2022-05-09 17:00:50.000000 kicost-1.1.8/kicost/spreadsheet.py
+-rw-rw-r--   0 root         (0) root         (0)       44 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4996 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1904 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      155 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-05-09 17:01:35.000000 kicost-1.1.8/kicost.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      471 2022-05-09 17:00:50.000000 kicost-1.1.8/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      133 2022-05-09 17:01:35.000000 kicost-1.1.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     6544 2022-05-09 17:00:50.000000 kicost-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-09 17:01:35.000000 kicost-1.1.8/tests/
+-rw-rw-r--   0 root         (0) root         (0)       25 2022-05-09 17:00:50.000000 kicost-1.1.8/tests/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     6555 2022-05-09 17:00:50.000000 kicost-1.1.8/tests/dummy-web-server.py
+-rw-rw-r--   0 root         (0) root         (0)    25531 2022-05-09 17:00:50.000000 kicost-1.1.8/tests/test_kicost.py
```

### Comparing `kicost-1.1.6/CONTRIBUTING.rst` & `kicost-1.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/LICENSE` & `kicost-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/PKG-INFO` & `kicost-1.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kicost
-Version: 1.1.6
+Version: 1.1.8
 Summary: Build cost spreadsheet for a KiCad project.
 Home-page: https://hildogjr.github.io/KiCost
 Author: XESS Corporation
 Author-email: info@xess.com
 License: MIT
 Project-URL: Doc, https://hildogjr.github.io/KiCost
 Project-URL: Git, https://github.com/hildogjr/KiCost
@@ -51,15 +51,24 @@
         .. image:: https://raw.githubusercontent.com/hildogjr/KiCost/master/docs/block_diag.png
         .. image:: https://raw.githubusercontent.com/hildogjr/KiCost/master/docs/gui.png
         
         
         Latest updates
         --------------
         
-        1.1.5 (2021-05-??)
+        1.1.8 (2022-05-09)
+        ______________________
+        * Add Digi-Key API
+        * Add Mouser API
+        * Add Farnell/Newark API (Element14)
+        * Add TME API
+        * Add cache for all APIs (including KitSpace and Octopart)
+        
+        
+        1.1.6 (2021-10-14)
         ______________________
         * Fix the Farnell import code order
         * Fix LCSC link and add BOM import links of all
         * Fix reference sorting and crashes
         * Add the user custom field capability to order quote
         * Add cell size adjust algorithm (use --max_column_width 0 to disable it)
         * Add ``pricing`` processing for subparts.
@@ -70,28 +79,21 @@
         
         
         1.1.4 (2020-03-24)
         ______________________
         * Add TME and Arrow to Kitspace API.
         * Others cosmetic and internal changes.
         
-        
-        1.1.3 (2019-12-31)
-        ______________________
-        * Fix the Digikey using Digi-Reel information.
-        * Added LCSC as distributor into the Kitspace API (the list can be used to JLCPCB).
-        * Parinfo kitspace API now just return the asked distributors (before was given all the avaliable distributors).
-        
-        Access https://github.com/hildogjr/KiCost/blob/master/HISTORY.rst for full development history.
+        Access https://github.com/hildogjr/KiCost/blob/master/kicost/HISTORY.rst for full development history.
 Keywords: KiCAD,BOM,electronics
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `kicost-1.1.6/README.rst` & `kicost-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/Makefile` & `kicost-1.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/block_diag.png` & `kicost-1.1.8/docs/block_diag.png`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/conf.py` & `kicost-1.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/gui.png` & `kicost-1.1.8/docs/gui.png`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/installation.rst` & `kicost-1.1.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/kicost.currency_converter.rst` & `kicost-1.1.8/docs/kicost.currency_converter.rst`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/kicost.distributors.rst` & `kicost-1.1.8/docs/kicost.distributors.rst`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/kicost.edas.rst` & `kicost-1.1.8/docs/kicost.edas.rst`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/kicost.rst` & `kicost-1.1.8/docs/kicost.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 ------------------
 
 .. automodule:: kicost.ansi
    :members:
    :undoc-members:
    :show-inheritance:
 
+kicost.config module
+--------------------
+
+.. automodule:: kicost.config
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 kicost.global\_vars module
 --------------------------
 
 .. automodule:: kicost.global_vars
    :members:
    :undoc-members:
    :show-inheritance:
@@ -74,14 +82,22 @@
 -----------------
 
 .. automodule:: kicost.log
    :members:
    :undoc-members:
    :show-inheritance:
 
+kicost.log\_\_ module
+---------------------
+
+.. automodule:: kicost.log__
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 kicost.os\_windows module
 -------------------------
 
 .. automodule:: kicost.os_windows
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `kicost-1.1.6/docs/make.bat` & `kicost-1.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/docs/usage.rst` & `kicost-1.1.8/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/AUTHORS.rst` & `kicost-1.1.8/kicost/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/HISTORY.rst` & `kicost-1.1.8/kicost/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 .. :changelog:
 
 History
 -------
 
-1.1.5 (2021-05-??)
+1.1.8 (2022-05-09)
+______________________
+* Add Digi-Key API
+* Add Mouser API
+* Add Farnell/Newark API (Element14)
+* Add TME API
+* Add cache for all APIs (including KitSpace and Octopart)
+
+
+1.1.6 (2021-10-14)
 ______________________
 * Fix the Farnell import code order
 * Fix LCSC link and add BOM import links of all
 * Fix reference sorting and crashes
 * Add the user custom field capability to order quote
 * Add cell size adjust algorithm (use --max_column_width 0 to disable it)
 * Add ``pricing`` processing for subparts.
```

### Comparing `kicost-1.1.6/kicost/__main__.py` & `kicost-1.1.8/kicost/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,34 +28,38 @@
 import sys
 import platform
 import time
 import tqdm
 import logging
 import subprocess
 # Debug, language and default configurations.
-from .global_vars import wxPythonNotPresent, DEBUG_OBSESSIVE, DEF_MAX_COLUMN_W, set_logger, KiCostError
-# Import log first to set the domain and assign it to the global logger
-from . import log
-log.set_domain('kicost')
-logger = log.init()
-set_logger(logger)
-
+from .global_vars import wxPythonNotPresent, DEF_MAX_COLUMN_W, W_CMDLINE
+# Sub systems can be imported before logger
+from .edas import get_registered_eda_names, set_edas_logger  # noqa: E402
+from .distributors import (get_distributors_list, set_distributors_logger, set_distributors_progress, is_valid_api,
+                           init_distributor_dict, configure_from_environment, configure_apis)
 # KiCost definitions and modules/packages functions.
-from .kicost import kicost, output_filename, kicost_gui_notdependences  # kicost core functions. # noqa: E402
+from .kicost import output_filename, kicost_gui_notdependences, kicost  # kicost core functions.
 try:
     from .kicost_gui import kicost_gui
     GUI_ENABLED = True
 except wxPythonNotPresent:
     # If the wxPython dependences are not installed and the user just want the KiCost CLI.
     GUI_ENABLED = False
-from .edas import get_registered_eda_names, set_edas_logger  # noqa: E402
-from .distributors import (get_distributors_list, set_distributors_logger, set_distributors_progress, set_api_options, set_api_status,  # noqa: E402
-                           get_api_status)  # noqa: E402
-from .spreadsheet import Spreadsheet  # noqa: E402
-from . import __version__, __build__  # Version control by @xesscorp and collaborator.  # noqa: E402
+from .spreadsheet import Spreadsheet
+from .config import load_config, config_force_ttl, config_force_path
+from . import __version__, __build__, debug_obsessive, debug_detailed, error, warning, info, get_logger, set_logger, KiCostError
+from . import log
+
+
+def init_all_loggers(main_logger, dist_logger, edas_logger):
+    set_logger(main_logger)
+    set_distributors_logger(dist_logger)
+    set_edas_logger(edas_logger)
+
 
 # Python 2.7 compatibility
 try:
     FileNotFoundError
 except NameError:
     FileNotFoundError = IOError
 
@@ -124,14 +128,59 @@
 
     def close(self):
         self.progress.close()
         self.logger.removeHandler(self.logTqdmHandler)
         self.logger.propagate = True
 
 
+def command_line_api_options(api_options, args):
+    """ Applies the command line options that overrides the APIs config """
+    # Force API options from the command line
+    if args.cache_ttl is not None:
+        config_force_ttl(args.cache_ttl)
+    if args.cache_path is not None:
+        config_force_path(args.cache_path)
+    if args.octopart_key is not None:
+        api_options['Octopart']['key'] = args.octopart_key
+    if args.octopart_level is not None:
+        level = args.octopart_level
+        extended = False
+        if level[-1] == 'p':
+            extended = True
+            level = level[:-1]
+        api_options['Octopart']['level'] = level
+        api_options['Octopart']['extended'] = extended
+    for api in args.disable_api:
+        debug_obsessive('Disabling API ' + api)
+        if is_valid_api(api):
+            api_options[api]['enable'] = False
+        else:
+            warning(W_CMDLINE, 'Unknown API `{}`'.format(api))
+    for api in args.enable_api:
+        debug_obsessive('Enabling API ' + api)
+        if is_valid_api(api):
+            api_options[api]['enable'] = True
+        else:
+            warning(W_CMDLINE, 'Unknown API `{}`'.format(api))
+    debug_detailed('Final API options {}'.format(api_options))
+
+
+def configure_kicost_apis(config_file, overwrite, apply_user_opts, data):
+    # Configuration file
+    api_options = load_config(config_file)
+    # Environment, overwrite only if the config file wasn't specified in the command line
+    configure_from_environment(api_options, overwrite)
+    # Apply command line options
+    apply_user_opts(api_options, data)
+    # Configure the APIs
+    configure_apis(api_options)
+    # Start with a clean list of available distributors
+    init_distributor_dict()
+
+
 ###############################################################################
 # Command-line interface.
 ###############################################################################
 
 
 def main_real():
 
@@ -268,38 +317,68 @@
                         help='Undo the KiCost integration.')
     parser.add_argument('--octopart_key',
                         nargs='?', type=str, metavar='APIKEY',
                         help='Enable Octopart using the provided key. Use None to disable it.')
     parser.add_argument('--octopart_level',
                         nargs='?', type=str, metavar='APILEVEL', choices=['3', '3p', '4', '4p'],
                         help='Use Octopart API level. Can be 3 or 4 for basic API and 3p or 4p for PRO plans. Default: 4')
+    parser.add_argument('--disable_api',
+                        nargs='+', type=str, default=[],
+                        metavar='API',
+                        help='Disable the listed APIs.')
+    parser.add_argument('--enable_api',
+                        nargs='+', type=str, default=[],
+                        metavar='API',
+                        help='Enable the listed APIs.')
+    parser.add_argument('-c', '--config',
+                        nargs='?', type=str,
+                        metavar='CONFIG.YAML',
+                        help='Configuration file.')
+    parser.add_argument('--cache_ttl',
+                        nargs='?', type=float,
+                        metavar='DAYS',
+                        help='Force the Time To Live for the APIs caches.')
+    parser.add_argument('--cache_path',
+                        nargs='?', type=str,
+                        metavar='BASE_PATH',
+                        help='Force the base path for the APIs caches.')
 
     args = parser.parse_args()
 
+    # Set up logging verbosity
+    log.set_domain('kicost')
+    init_all_loggers(log.init(), log.get_logger('kicost.distributors'), log.get_logger('kicost.edas'))
+    log.set_verbosity(get_logger(), args.debug, args.quiet)
+    set_distributors_progress(ProgressConsole)
+
+    # Now we can print errors, inform if YAML is missing
+    try:
+        import yaml  # noqa F401
+    except ImportError:
+        error('No yaml module for Python, install it (i.e. python3-yaml)')
+
+    # APIs Configuration
+    configure_kicost_apis(args.config, args.config is None, command_line_api_options, args)
+
     # Setup and unsetup KiCost integration.
     if args.setup:
         from .kicost_config import kicost_setup
         kicost_setup()
         return
     if args.unsetup:
         from .kicost_config import kicost_unsetup
         kicost_unsetup()
         return
 
-    # Set up logging.
-    log.set_verbosity(logger, args.debug, args.quiet)
-    set_distributors_logger(log.get_logger('kicost.distributors'))
-    set_distributors_progress(ProgressConsole)
-    set_edas_logger(log.get_logger('kicost.edas'))
-
+    # Simple commands
     if args.show_dist_list:
-        logger.info('Distributor list: ' + ' '.join(sorted(get_distributors_list())))
+        info('Distributor list: ' + ' '.join(sorted(get_distributors_list())))
         sys.exit(0)
     if args.show_eda_list:
-        logger.info('EDA supported list: ' + ' '.join(sorted(get_registered_eda_names())))
+        info('EDA supported list: ' + ' '.join(sorted(get_registered_eda_names())))
         sys.exit(0)
 
     # Set up spreadsheet output file.
     if args.output is None:
         # If no output file is given...
         if args.input is not None:
             # Send output to spreadsheet with name of input file.
@@ -308,36 +387,27 @@
         else:
             # Send output to spreadsheet with name of this application.
             args.output = os.path.splitext(sys.argv[0])[0] + '.xlsx'
     else:
         # Output file was given. Make sure it has spreadsheet extension.
         args.output = os.path.splitext(args.output)[0] + '.xlsx'
 
-    # Configure the Octopart API
-    set_api_options('Octopart', key=args.octopart_key, level=args.octopart_level)
-    if get_api_status('Octopart'):
-        # Disable KitSpace if Octopart is enabled.
-        # Mixing both could sound useful, but KitSpace uses Octopart, so any difference is most probably an error.
-        # Keeping them separated will help to solve the errors.
-        # Additionally: people with an Octopart key can help to offload KitSpace.
-        set_api_status('KitSpace', False)
-
     # SET: This is half implemented. Not currently working.
     #     # Call the KiCost interface to alredy run KiCost, this is just to use the
     #     # saved user configurations of the graphical interface.
     #     if args.user:
     #         if not GUI_ENABLED:
     #             kicost_gui_notdependences()
     #         kicost_gui_runterminal(args)
     #         sys.exit(0)
 
     # Handle case where output is going into an existing spreadsheet file.
     if os.path.isfile(args.output):
         if not args.overwrite:
-            logger.error('Output file {} already exists!\nUse the --overwrite option to replace it.'.format(args.output))
+            error('Output file {} already exists!\nUse the --overwrite option to replace it.'.format(args.output))
             sys.exit(2)
 
     if args.gui:
         if not GUI_ENABLED:
             kicost_gui_notdependences()
         kicost_gui(args.force_en_us, [os.path.abspath(fileName) for fileName in args.gui])
         sys.exit(0)
@@ -349,29 +419,29 @@
         sys.exit(0)
     else:
         # Match the EDA tool formats with the input files.
         if len(args.eda) == 1:
             # Expand a single EDA format to cover all input files.
             args.eda = args.eda[0:1] * len(args.input)
         if len(args.input) != len(args.eda):
-            logger.error('The number of input files must match the number of EDA tool formats.')
+            error('The number of input files must match the number of EDA tool formats.')
             sys.exit(2)
 
         # Match the variants with the input files.
         if len(args.variant) == 1:
             args.variant = args.variant[0:1] * len(args.input)
         if len(args.input) != len(args.variant):
-            logger.error('The number of input files must match the number of variants.')
+            error('The number of input files must match the number of variants.')
             sys.exit(2)
 
         # Match the board quantities with the input files.
         if len(args.board_qty) == 1:
             args.board_qty = args.board_qty[0:1] * len(args.input)
         if len(args.input) != len(args.board_qty):
-            logger.error('The number of input files must match the number of board quantities.')
+            error('The number of input files must match the number of board quantities.')
             sys.exit(2)
 
         # Otherwise get XML from the given file.
         for i in range(len(args.input)):
             # Set '.xml' as the default file extension, treating this exception
             # allow other files extension and formats.
             try:
@@ -382,15 +452,15 @@
             except IndexError:
                 pass
 
     # List of distributors to scrape
     available = get_distributors_list()
     for d in args.include + args.exclude:
         if d not in available:
-            logger.error('Unknown distributor requested: `{}`'.format(d))
+            error('Unknown distributor requested: `{}`'.format(d))
             sys.exit(2)
     if args.no_price:
         # None
         dist_list = []
     else:
         if not args.include:
             # All by default
@@ -398,32 +468,32 @@
         else:
             # Requested to be included
             dist_list = args.include
         # Requested to be excluded
         for d in args.exclude:
             dist_list.remove(d)
 
-    logger.log(DEBUG_OBSESSIVE, 'Started ' + kicost_version_info())
+    debug_obsessive('Started ' + kicost_version_info())
 
     kicost(in_file=args.input, eda_name=args.eda,
            out_filename=args.output, collapse_refs=not args.no_collapse, suppress_cat_url=not args.show_cat_url,
            user_fields=args.fields, ignore_fields=args.ignore_fields,
            group_fields=args.group_fields, translate_fields=args.translate_fields,
            variant=args.variant, dist_list=dist_list, currency=args.currency, max_column_width=args.max_column_width,
            split_extra_fields=args.split_extra_fields, board_qty=args.board_qty)
 
 
 def main():
     try:
         main_real()
     except KiCostError as e:
-        logger.error(e.msg)
+        error(e.msg)
         sys.exit(e.id)
 
 
 ###############################################################################
 # Main entrypoint.
 ###############################################################################
 if __name__ == '__main__':
     start_time = time.time()
     main()
-    logger.log(DEBUG_OBSESSIVE, 'Elapsed time: %f seconds', time.time() - start_time)
+    debug_obsessive('Elapsed time: %f seconds', time.time() - start_time)
```

### Comparing `kicost-1.1.6/kicost/ansi.py` & `kicost-1.1.8/kicost/ansi.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/currency_converter/currency_converter.py` & `kicost-1.1.8/kicost/currency_converter/currency_converter.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/currency_converter/currency_tables.py` & `kicost-1.1.8/kicost/currency_converter/currency_tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
                     'MXN': 'MX$',
                     'MYR': 'MYR',
                     'NOK': 'NOK',
                     'NZD': 'NZ$',
                     'PHP': 'PHP',
                     'PLN': 'PLN',
                     'RON': 'RON',
-                    'RUB': 'RUB',
                     'SEK': 'SEK',
                     'SGD': 'SGD',
                     'THB': 'THB',
                     'TRY': 'TRY',
                     'USD': '$',
                     'ZAR': 'ZAR',
                     }
@@ -56,15 +55,14 @@
                   'MXN': 'Mexican Peso',
                   'MYR': 'Malaysian Ringgit',
                   'NOK': 'Norwegian Krone',
                   'NZD': 'New Zealand Dollar',
                   'PHP': 'Philippine Piso',
                   'PLN': 'Polish Zloty',
                   'RON': 'Romanian Leu',
-                  'RUB': 'Russian Ruble',
                   'SEK': 'Swedish Krona',
                   'SGD': 'Singapore Dollar',
                   'THB': 'Thai Baht',
                   'TRY': 'Turkish Lira',
                   'USD': 'US Dollar',
                   'ZAR': 'South African Rand',
                   }
```

### Comparing `kicost-1.1.6/kicost/currency_converter/download_rates.py` & `kicost-1.1.8/kicost/currency_converter/download_rates.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/distributors/__init__.py` & `kicost-1.1.8/kicost/distributors/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,21 +29,25 @@
 # Export the ORDER_COL_USERFIELDS content
 from .distributors_info import ORDER_COL_USERFIELDS  # noqa: F401
 
 # Import and register here the API / local / scrape modules.
 from .dist_local_template import dist_local_template  # noqa: F401
 from .api_octopart import api_octopart  # noqa: F401
 from .api_partinfo_kitspace import api_partinfo_kitspace  # noqa: F401
+from .api_digikey import api_digikey  # noqa: F401
+from .api_mouser import api_mouser  # noqa: F401
+from .api_element14 import api_element14  # noqa: F401
+from .api_tme import api_tme  # noqa: F401
 
 
 #
 # Some wrappers
 #
 def init_distributor_dict():
-    distributor_class.init_dist_dict()
+    distributor_class.main_init_dist_dict()
 
 
 def get_dist_parts_info(parts, dist_list, currency):
     distributor_class.get_dist_parts_info(parts, dist_list, currency)
 
 
 def get_registered_apis():
@@ -77,24 +81,39 @@
 
 
 def set_distributors_progress(cls):
     ''' Configures the class used to indicate progress '''
     distributor_class.progress = cls
 
 
-def set_api_options(api, **kwargs):
-    ''' Configure an API (by name) '''
-    distributor_class.set_api_options(api, **kwargs)
+def configure_apis(options):
+    ''' Configure all APIs. options is a dict API -> api_options '''
+    distributor_class.configure_apis(options)
 
 
 def set_api_status(api, enabled):
     ''' Enable/Disable a particular API '''
     distributor_class.set_api_status(api, enabled)
 
 
 def get_api_status(api):
     ''' Find if an API is enabled '''
     return distributor_class.get_api_status(api)
 
 
-# Init distributor dict during import.
-init_distributor_dict()
+def is_valid_api(api):
+    ''' Determines if this API is registered '''
+    return distributor_class._get_api(api) is not None
+
+
+def get_api_list():
+    ''' Returns a list of registered APIs '''
+    return [api.name for api in distributor_class.registered]
+
+
+def get_api_valid_options():
+    ''' Returns the vali options for each API '''
+    return {api.name: api.config_options for api in distributor_class.registered}
+
+
+def configure_from_environment(options, overwrite):
+    distributor_class.configure_from_environment(options, overwrite)
```

### Comparing `kicost-1.1.6/kicost/distributors/api_octopart.py` & `kicost-1.1.8/kicost/distributors/api_octopart.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,76 +31,91 @@
 from collections import Counter
 if sys.version_info[0] < 3:
     from urllib import quote_plus
 else:
     from urllib.parse import quote_plus
 
 # KiCost definitions.
-from ..global_vars import DEBUG_OVERVIEW, DEBUG_OBSESSIVE, ERR_SCRAPE, KiCostError, W_ASSQTY, W_AMBIPN
-from .. import DistData
+from .. import KiCostError, DistData, ERR_SCRAPE, W_ASSQTY, W_AMBIPN, W_APIFAIL
 # Distributors definitions.
-from .distributor import distributor_class
+from .distributor import distributor_class, QueryCache
+from .log__ import debug_overview, debug_obsessive, warning
 
 # Author information.
 __author__ = 'XESS Corporation'
 __webpage__ = 'info@xess.com'
 
 OCTOPART_MAX_PARTBYQUERY = 20  # Maximum part list length to one single query.
 
 __all__ = ['api_octopart']
 
 
+class QueryStruct(object):
+    def __init__(self, id, kind, code, part):
+        self.id = str(id)  # ID number for this query
+        self.kind = kind   # mpn/sku
+        self.code = code   # manf_code/sku
+        self.part = part   # Pointer to the part.
+        self.result = None
+        self.loaded = False
+
+
 class api_octopart(distributor_class):
     name = 'Octopart'
     type = 'api'
     enabled = False
     url = 'https://octopart.com/'  # Web site API information.
+    # Options supported by this API
+    config_options = {'key': str, 'level': int, 'extended': bool}
     api_level = 4
     # Include specs and datasheets. Only in the Pro plan.
     extended = False
+    cache = None
 
     API_KEY = None
-    API_DISTRIBUTORS = ['arrow', 'digikey', 'farnell', 'lcsc', 'mouser', 'newark', 'rs', 'tme']
+    api_distributors = ['arrow', 'digikey', 'farnell', 'lcsc', 'mouser', 'newark', 'rs', 'tme']
     DIST_TRANSLATION = {  # Distributor translation. Just a few supported.
                         'Arrow Electronics': 'arrow',
                         'Digi-Key': 'digikey',
                         'Farnell': 'farnell',
                         'Mouser': 'mouser',
                         'Newark': 'newark',
                         'RS Components': 'rs',
                         'TME': 'tme',
                         'LCSC': 'lcsc',
                        }
     # Dict to translate KiCost field names into Octopart distributor names
     KICOST2OCTOPART_DIST = {v: k for k, v in DIST_TRANSLATION.items()}
 
     @staticmethod
-    def init_dist_dict():
-        if api_octopart.enabled:
-            distributor_class.add_distributors(api_octopart.API_DISTRIBUTORS)
-
-    @staticmethod
-    def set_options(key, level):
-        if key:
-            if key.lower() == 'none':
-                api_octopart.enabled = False
-            else:
-                api_octopart.API_KEY = key
-                api_octopart.enabled = True
-                # Register our distributors
-                api_octopart.init_dist_dict()
-        if level:
-            if level[-1] == 'p':
-                api_octopart.extended = True
-                level = level[:-1]
-            else:
-                api_octopart.extended = False
-            api_octopart.api_level = int(level)
-        distributor_class.logger.log(DEBUG_OBSESSIVE, 'Octopart API configured to enabled {} key {} level {} extended {}'.
-                                     format(api_octopart.enabled, api_octopart.API_KEY, api_octopart.api_level, api_octopart.extended))
+    def configure(ops):
+        cache_ttl = 7
+        cache_path = None
+        for k, v in ops.items():
+            if k == 'key':
+                api_octopart.API_KEY = v
+                if 'enable' not in ops:
+                    # If not explicitly disabled then enable it
+                    api_octopart.enabled = True
+            elif k == 'enable':
+                api_octopart.enabled = v
+            elif k == 'extended':
+                api_octopart.extended = v
+            elif k == 'level':
+                api_octopart.api_level = v
+            elif k == 'cache_ttl':
+                cache_ttl = v
+            elif k == 'cache_path':
+                cache_path = v
+        api_octopart.cache = QueryCache(cache_path, cache_ttl)
+        if api_octopart.enabled and api_octopart.API_KEY is None:
+            warning(W_APIFAIL, "Can't enable Octopart without a `key`")
+            api_octopart.enabled = False
+        debug_obsessive('Octopart API configured to enabled {} key {} level {} extended {}'.
+                        format(api_octopart.enabled, api_octopart.API_KEY, api_octopart.api_level, api_octopart.extended))
 
     @staticmethod
     def query(query):
         """Send query to Octopart and return results."""
         # url = 'http://octopart.com/api/v3/parts/match'
         # payload = {'queries': json.dumps(query), 'include\[\]': 'specs', 'apikey': token}
         # response = requests.get(url, params=payload)
@@ -183,41 +198,52 @@
                 continue
 
             # Assign the most common manf. part number to this part.
             mpn_cnts = Counter(mpns)
             part.fields['manf#'] = mpn_cnts.most_common(1)[0][0]
 
     @staticmethod
-    def get_part_info(query, parts, distributors, currency='USD'):
-        """Query Octopart for quantity/price info and place it into the parts list."""
+    def get_part_info(queries):
+        """Query Octopart for quantity/price info."""
+        only_query = ['{"reference": "'+q.id+'", "'+q.kind+'": "'+quote_plus(q.code)+'"}' for q in queries]
+        results = api_octopart.query(only_query)
+        # Copy the results to the queries
+        q_hash = {q.id: q for q in queries}
+        for r in results:
+            query = q_hash[r['reference']]
+            query.result = r
+            api_octopart.cache.save_results(query.kind, query.code, r)
+
+    @staticmethod
+    def fill_part_info(queries, distributors, solved, currency='USD'):
+        ''' Place the results into the parts list. '''
         # Translate from Octopart distributor names to the names used internally by kicost.
         dist_xlate = api_octopart.DIST_TRANSLATION
         # List of desired distributors in native format
         native_dists = set((api_octopart.KICOST2OCTOPART_DIST[d] for d in distributors))
         # Currency priority: 1: User specified, 2: USD, 3: EUR
         currency_prio = [currency]
         if currency != 'USD':
             currency_prio.append('USD')
         if currency != 'EUR':
             currency_prio.append('EUR')
-        results = api_octopart.query(query)
         # Loop through the response to the query and enter info into the parts list.
-        for result in results:
-            i = int(result['reference'])  # Get the index into the part dict.
-            part = parts[i]
+        for query in queries:
+            result = query.result
+            part = query.part
             # Each result can match one or more components from different manufacturers
             # Take only the items with useful offers
             useful_items = []
             for item in result['items']:
                 for offer in item['offers']:
                     if offer['seller']['name'] in native_dists:
                         useful_items.append(item)
                         break
-            # distributor_class.logger.log(DEBUG_OBSESSIVE, str(result))
-            # distributor_class.logger.log(DEBUG_OBSESSIVE, str(useful_items))
+            # debug_obsessive(str(result))
+            # debug_obsessive(str(useful_items))
             # If more than one select the right one
             if len(useful_items) > 1:
                 # List of possible manufacturers
                 # TODO: Can we get more than one hit for the same manf?
                 manufacturers = {it['manufacturer']['name'].lower(): it for it in useful_items}
                 # Is the manf included?
                 manf = part.fields.get('manf', 'none').lower()
@@ -225,17 +251,17 @@
                 if not item:
                     if manf == 'none':
                         item = useful_items[0]
                     else:
                         best_match = difflib.get_close_matches(manf, manufacturers.keys())[0]
                         item = manufacturers[best_match]
                     mpn = item['mpn']
-                    distributor_class.logger.warning(W_AMBIPN+'Using "{}" for manf#="{}"'.format(item['manufacturer']['name'], mpn))
-                    distributor_class.logger.warning(W_AMBIPN+'Ambiguous manf#="{}" please use manf to select the right one, choices: {}'.format(
-                                                      mpn, list(manufacturers.keys())))
+                    warning(W_AMBIPN, 'Using "{}" for manf#="{}"'.format(item['manufacturer']['name'], mpn))
+                    warning(W_AMBIPN, 'Ambiguous manf#="{}" please use manf to select the right one, choices: {}'.format(
+                            mpn, list(manufacturers.keys())))
             else:
                 if len(useful_items):
                     item = useful_items[0]
                 else:
                     # No hits, skip
                     continue
             if api_octopart.extended:
@@ -343,97 +369,116 @@
                         # Save the link, stock code, ... of the page for minimum purchase.
                         dd.moq = moq_offer  # Minimum order qty.
                         dd.part_num = dist_part_num
                         dd.url = offer.get('product_url')
                         dd.qty_increment = part_qty_increment
                 # Update the DistData for this distributor
                 part.dd[dist] = dd
+                # We have data for this distributor
+                solved.add(dist)
 
     @staticmethod
     def query_part_info(parts, distributors, currency):
         """Fill-in the parts with price/qty/etc info from Octopart."""
-        distributor_class.logger.log(DEBUG_OVERVIEW, '# Getting part data from Octopart...')
-
-        # Setup progress bar to track progress of Octopart queries.
-        progress = distributor_class.progress(len(parts), distributor_class.logger)
+        debug_overview('# Getting part data from Octopart...')
 
         # Get the valid distributors names used by them part catalog
         # that may be index by Octopart. This is used to remove the
         # local distributors and future not implemented in the Octopart
         # definition.
         # Note: The user can use --exclude and define it with fields.
         distributors_octopart = [d for d in distributors if distributor_class.get_distributor_info(d).is_web()
-                                 and d in api_octopart.API_DISTRIBUTORS]
+                                 and d in api_octopart.api_distributors]
 
-        # Break list of parts into smaller pieces and get price/quantities from Octopart.
-        octopart_query = []
-        prev_i = 0  # Used to record index where parts query occurs.
+        # Collect all the queries
+        queries = []
         for i, part in enumerate(parts):
-
-            # Create an Octopart query using the manufacturer's part number or
-            # distributor SKU.
+            # Create an Octopart query using the manufacturer's part number or distributor SKU.
             manf_code = part.fields.get('manf#')
             if manf_code:
-                part_query = '{"reference": "'+str(i)+'", "mpn": "'+quote_plus(manf_code)+'"}'
+                query = QueryStruct(i, "mpn", manf_code, part)
             else:
                 # No MPN, so use the first distributor SKU that's found.
                 for octopart_dist_sku in distributors_octopart:
                     sku = part.fields.get(octopart_dist_sku + '#', '')
                     if sku:
                         break
                 if not sku:
                     # No MPN or SKU, so skip this part.
                     continue
                 # Create the part query using SKU matching.
-                part_query = '{"reference": "'+str(i)+'", "sku": "'+quote_plus(sku)+'"}'
+                query = QueryStruct(i, "sku", sku, part)
 
                 # Because was used the distributor (enrolled at Octopart list)
                 # despite the normal 'manf#' code, take the sub quantity as
                 # general sub quantity of the current part.
                 try:
                     part.fields['manf#_qty'] = part.fields[octopart_dist_sku + '#_qty']
-                    distributor_class.logger.warning(W_ASSQTY+"Associated {q} quantity to '{r}' due \"{f}#={q}:{c}\".".format(
+                    warning(W_ASSQTY, "Associated {q} quantity to '{r}' due \"{f}#={q}:{c}\".".format(
                             q=part.fields[octopart_dist_sku + '#_qty'], r=part.refs,
                             f=octopart_dist_sku, c=part.fields[octopart_dist_sku+'#']))
                 except KeyError:
                     pass
-
             # Add query for this part to the list of part queries.
-            octopart_query.append(part_query)
+            queries.append(query)
+
+        n_queries = len(queries)
+        debug_overview('Queries {}'.format(n_queries))
+        if not n_queries:
+            return
+
+        # Try to solve the queries from the cache
+        unsolved = []
+        for query in queries:
+            # Look in the cache
+            query.result, query.loaded = api_octopart.cache.load_results(query.kind, query.code)
+            if not query.loaded:
+                unsolved.append(query)
+
+        # Solve the rest from the site
+        n_unsolved = len(unsolved)
+        debug_overview('Cached entries {}'.format(n_queries-n_unsolved))
+        if n_unsolved:
+            # Setup progress bar to track progress of server queries.
+            progress = distributor_class.progress(n_unsolved, distributor_class.logger)
+
+            # Slice the queries into batches of the largest allowed size and gather
+            # the part data for each batch.
+            for i in range(0, n_unsolved, OCTOPART_MAX_PARTBYQUERY):
+                slc = slice(i, i+OCTOPART_MAX_PARTBYQUERY)
+                api_octopart.get_part_info(unsolved[slc])
+                progress.update(len(unsolved[slc]))
+
+            # Done with the scraping progress bar so delete it or else we get an
+            # error when the program terminates.
+            progress.close()
+
+        # Transfer the results
+        solved_dist = set()
+        api_octopart.fill_part_info(queries, distributors_octopart, solved_dist, currency)
+        return solved_dist
+
+    @staticmethod
+    def from_environment(options, overwrite):
+        ''' Configuration from the environment. '''
+        # Configure the module from the environment
+        # The command line will overwrite it using set_options()
+        key = os.getenv('KICOST_OCTOPART_KEY_V3')
+        if key:
+            api_octopart._set_from_env('key', key, options, overwrite)
+            api_octopart._set_from_env('enable', True, options, overwrite)
+            api_octopart._set_from_env('level', 3, options, overwrite)
+        else:
+            key = os.getenv('KICOST_OCTOPART_KEY_V4')
+            if key:
+                api_octopart._set_from_env('key', key, options, overwrite)
+                api_octopart._set_from_env('enable', True, options, overwrite)
+                api_octopart._set_from_env('level', 4, options, overwrite)
+            elif os.environ.get('KICOST_OCTOPART'):
+                # Currently this isn't useful, you can't do anything without a key.
+                # This is just in case we get a proxy running.
+                api_octopart._set_from_env('enable', True, options, overwrite)
+        if os.environ.get('KICOST_OCTOPART_EXTENDED'):
+            api_octopart._set_from_env('extended', True, options, overwrite)
+
 
-            # Once there are enough (but not too many) part queries, make a query request to Octopart.
-            if len(octopart_query) == OCTOPART_MAX_PARTBYQUERY:
-                api_octopart.get_part_info(octopart_query, parts, distributors_octopart, currency)
-                progress.update(i - prev_i)  # Update progress bar.
-                prev_i = i
-                octopart_query = []  # Get ready for next batch.
-
-        # Query Octopart for the last batch of parts.
-        if octopart_query:
-            api_octopart.get_part_info(octopart_query, parts, distributors_octopart, currency)
-            progress.update(len(parts)-prev_i)  # This will indicate final progress of 100%.
-
-        # Done with the scraping progress bar so delete it or else we get an
-        # error when the program terminates.
-        progress.close()
-
-
-# Configure the module from the environment
-# The command line will overwrite it using set_options()
-key = os.environ.get('KICOST_OCTOPART_KEY_V3')
-if key:
-    api_octopart.API_KEY = key
-    api_octopart.enabled = True
-    api_octopart.api_level = 3
-else:
-    key = os.environ.get('KICOST_OCTOPART_KEY_V4')
-    if key:
-        api_octopart.API_KEY = key
-        api_octopart.enabled = True
-        api_octopart.api_level = 4
-    elif os.environ.get('KICOST_OCTOPART'):
-        # Currently this isn't useful, you can't do anything without a key.
-        # This is just in case we get a proxy running.
-        api_octopart.enabled = True
-if os.environ.get('KICOST_OCTOPART_EXTENDED'):
-    api_octopart.extended = True
 distributor_class.register(api_octopart, 60)
```

### Comparing `kicost-1.1.6/kicost/distributors/api_partinfo_kitspace.py` & `kicost-1.1.8/kicost/distributors/api_partinfo_kitspace.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 # Libraries.
 import json
 import requests
 import re
 import sys
 import os
 import copy
+import pprint
 from collections import OrderedDict
 if sys.version_info[0] < 3:
     from urllib import quote_plus
 else:
     from urllib.parse import quote_plus
 
 # KiCost definitions.
-from ..global_vars import DEFAULT_CURRENCY, DEBUG_OVERVIEW, ERR_SCRAPE, KiCostError, W_NOINFO, NO_PRICE
-from .. import DistData
+from .. import KiCostError, DistData, DEFAULT_CURRENCY, ERR_SCRAPE, W_NOINFO, NO_PRICE
 # Distributors definitions.
-from .distributor import distributor_class
+from .distributor import distributor_class, QueryCache
+from .log__ import debug_overview, debug_obsessive, warning
 
 
 # Uncomment for debug
 # Use `debug('x + 1')` for instance.
 # def debug(expression):
 #     frame = sys._getframe(1)
 #     distributor_class.logger.info(expression, '=', repr(eval(expression, frame.f_globals, frame.f_locals)))
@@ -79,38 +80,57 @@
 QUERY_MATCH = 'query ($input: [MpnOrSku]!){ match(parts: $input) {' + QUERY_ANSWER + '} }'
 QUERY_SEARCH = 'query ($input: String!){ search(term: $input) {' + QUERY_ANSWER + '} }'
 QUERY_URL = 'https://dev-partinfo.kitspace.org/graphql'
 
 __all__ = ['api_partinfo_kitspace']
 
 
+class QueryStruct(object):
+    def __init__(self, query, part, for_dists):
+        self.query = query  # Each part reference query.
+        self.part = part    # Pointer to the part.
+        self.for_dists = for_dists  # Used the stock code mention for disambiguation, it is used `None` for the "manf#".
+        self.result = None
+        self.loaded = False
+
+
 class api_partinfo_kitspace(distributor_class):
     name = 'KitSpace'
     type = 'api'
     enabled = True
     url = 'https://kitspace.org/'  # Web site API information.
 
-    API_DISTRIBUTORS = ['digikey', 'farnell', 'mouser', 'newark', 'rs', 'arrow', 'tme', 'lcsc']
+    api_distributors = ['digikey', 'farnell', 'mouser', 'newark', 'rs', 'arrow', 'tme', 'lcsc']
     DIST_TRANSLATION = {  # Distributor translation.
                         'Digikey': 'digikey',
                         'Farnell': 'farnell',
                         'Mouser': 'mouser',
                         'Newark': 'newark',
                         'RS': 'rs',
                         'TME': 'tme',
                         'Arrow Electronics': 'arrow',
                         'LCSC': 'lcsc',
                        }
     # Dict to translate KiCost field names into KitSpace distributor names
     KICOST2KITSPACE_DIST = {v: k for k, v in DIST_TRANSLATION.items()}
+    cache = None
 
     @staticmethod
-    def init_dist_dict():
-        if api_partinfo_kitspace.enabled:
-            distributor_class.add_distributors(api_partinfo_kitspace.API_DISTRIBUTORS)
+    def configure(ops):
+        cache_ttl = 7
+        cache_path = None
+        for k, v in ops.items():
+            if k == 'enable':
+                api_partinfo_kitspace.enabled = v
+            elif k == 'cache_ttl':
+                cache_ttl = v
+            elif k == 'cache_path':
+                cache_path = v
+        api_partinfo_kitspace.cache = QueryCache(cache_path, cache_ttl)
+        debug_obsessive('KitSpace API configured to enabled {}'.format(api_partinfo_kitspace.enabled))
 
     @staticmethod
     def query(query_parts, distributors, query_type=QUERY_MATCH):
         '''Send query to server and return results.'''
 
         distributors = [api_partinfo_kitspace.KICOST2KITSPACE_DIST[d] for d in distributors]
         # Allow changing the URL for debug purposes
@@ -140,50 +160,78 @@
             raise KiCostError('Kitspace server not found check your internet connection.', ERR_SCRAPE)
         elif response.status_code == requests.codes['request_timeout']:  # 408
             raise KiCostError('KitSpace is not responding.', ERR_SCRAPE)
         elif response.status_code == requests.codes['bad_request']:  # 400
             raise KiCostError('Bad request to Kitspace server probably due to an incorrect string '
                               'format check your `manf#` codes and contact the suport team.', ERR_SCRAPE)
         elif response.status_code == requests.codes['gateway_timeout']:  # 504
-            raise KiCostError('One of the internal Kitspace services may experiencing problems. Contact the Kitspace support.', ERR_SCRAPE)
+            raise KiCostError('One of the internal Kitspace services may experiencing problems.'
+                              ' Most probably is saturated, please consider using other API.', ERR_SCRAPE)
         else:
             raise KiCostError('Kitspace error: ' + str(response.status_code), ERR_SCRAPE)
 
     @staticmethod
     def get_spec(data, item, default=None):
         '''Get the value of `value` field of a dictionary if the `name` field identifier.
         Used to get information from the JSON response.'''
         for d in data['specs']:
             if d['key'] == item:
                 value = d['value']
                 return value if value is not None else default
         return default
 
     @staticmethod
-    def get_part_info(query, parts, distributors, currency, distributors_wanted):
-        '''Query PartInfo for quantity/price info and place it into the parts list.
-           `distributors_wanted` is the list of distributors we want for each query.
-           `distributors` is the list of all distributors we want, in general.
-           This difference is because some queries are for an specific distributor.
-        '''
+    def query2name(query):
+        ''' Finds the prefix and name for a query '''
+        q = json.loads(query)
+        mpn = q.get('mpn', None)
+        if mpn is not None:
+            prefix = 'mpn'
+            name = mpn['part']
+        else:
+            sku = q.get('sku', None)
+            if sku is not None:
+                prefix = 'sku'
+                name = sku['vendor'] + '_' + sku['part']
+        return prefix, name
+
+    @staticmethod
+    def get_part_info(queries, distributors):
+        '''Query PartInfo for quantity/price info.
+           `distributors` is the list of all distributors we want, in general. '''
+        only_query = [q.query for q in queries]
+        results = api_partinfo_kitspace.query(only_query, distributors)
+        for i, r in enumerate(results['data']['match']):
+            queries[i].result = r
+            # Solve the prefix and name
+            prefix, name = api_partinfo_kitspace.query2name(queries[i].query)
+            api_partinfo_kitspace.cache.save_results(prefix, name, r)
+
+    @staticmethod
+    def fill_part_info(queries, distributors, currency, solved):
+        ''' Place the results into the parts list. '''
         # Translate from PartInfo distributor names to the names used internally by kicost.
         dist_xlate = api_partinfo_kitspace.DIST_TRANSLATION
 
-        results = api_partinfo_kitspace.query(query, distributors)
-
         # Loop through the response to the query and enter info into the parts list.
-        for part_query, part, dist_want, result in zip(query, parts, distributors_wanted, results['data']['match']):
+        for q in queries:
+            # Unpack the structure
+            part_query = q.query
+            part = q.part
+            dist_want = q.for_dists
+            result = q.result
+            # Process it
             if not result:
-                distributor_class.logger.warning(W_NOINFO+'No information found for parts \'{}\' query `{}`'.format(part.refs, str(part_query)))
+                warning(W_NOINFO, 'No information found for parts \'{}\' query `{}`'.format(part.refs, str(part_query)))
                 continue
             # Get the information of the part.
             part.datasheet = result.get('datasheet')
             part.lifecycle = api_partinfo_kitspace.get_spec(result, 'lifecycle_status', 'active').lower()
             # Misc data collected, currently not used inside KiCost
-            part.update_specs({sp['key']: (sp['key'], sp['value']) for sp in result['specs']})
+            part.update_specs({sp['key']: (sp['key'], sp['value']) for sp in result['specs'] if sp['value']})
             # Loop through the offers from various dists for this particular part.
             for offer in result['offers']:
                 # Get the distributor who made the offer and add their
                 # price/qty info to the parts list if its one of the accepted distributors.
                 dist = dist_xlate.get(offer['sku']['vendor'], '')
                 if dist not in dist_want:
                     # Not interested in this distributor
@@ -194,16 +242,15 @@
                 # As a stop-gap measure, just assign infinity to the part increment.
                 # A better alternative may be to examine the packaging field of the offer.
                 part_qty_increment = float("inf")
                 # Get pricing information from this distributor.
                 dist_currency = {cur: pri for cur, pri in offer['prices'].items() if pri}
                 if not dist_currency:
                     # Some times the API returns minimum purchase 0 and a not valid `price_tiers`.
-                    distributor_class.logger.warning(NO_PRICE+'No price information found for parts \'{}\' query `{}`'.
-                                                     format(part.refs, str(part_query)))
+                    warning(NO_PRICE, 'No price information found for parts \'{}\' query `{}`'.format(part.refs, str(part_query)))
                 else:
                     prices = None
                     # Get the price tiers prioritizing:
                     # 1) The asked currency by KiCost user;
                     # 2) The default currency given by `DEFAULT_CURRENCY` in root `global_vars.py`;
                     # 3) The first not null tiers
                     if currency in dist_currency:
@@ -254,32 +301,32 @@
                     # Save the link, stock code, ... of the page for minimum purchase.
                     dd.moq = moq  # Minimum order qty.
                     dd.url = offer.get('product_url', '')  # Page to purchase the minimum quantity.
                     dd.part_num = dist_part_num
                     dd.qty_increment = part_qty_increment
                 # Update the DistData for this distributor
                 part.dd[dist] = dd
+                # We have data for this distributor
+                solved.add(dist)
 
     @staticmethod
     def query_part_info(parts, distributors, currency):
         '''Fill-in the parts with price/qty/etc info from KitSpace.'''
-        distributor_class.logger.log(DEBUG_OVERVIEW, '# Getting part data from KitSpace...')
+        debug_overview('# Getting part data from KitSpace...')
 
         # Use just the distributors avaliable in this API.
         # Note: The user can use --exclude and define it with fields.
         distributors = [d for d in distributors if distributor_class.get_distributor_info(d).is_web()
-                        and d in api_partinfo_kitspace.API_DISTRIBUTORS]
+                        and d in api_partinfo_kitspace.api_distributors]
         FIELDS_CAT = sorted([d + '#' for d in distributors])
 
         # Create queries to get part price/quantities from PartInfo.
-        queries = []  # Each part reference query.
-        query_parts = []  # Pointer to the part.
-        query_part_stock_code = []  # Used the stock code mention for disambiguation, it is used `None` for the "manf#".
+        queries = []
         # Translate from PartInfo distributor names to the names used internally by kicost.
-        available_distributors = set(api_partinfo_kitspace.API_DISTRIBUTORS)
+        available_distributors = set(api_partinfo_kitspace.api_distributors)
         for part in parts:
             # Create a PartInfo query using the manufacturer's part number or the distributor's SKU.
             part_dist_use_manfpn = copy.copy(distributors)
 
             # Create queries using the distributor SKU
             # Check if that part have stock code that is accepted to use by this module (API).
             # KiCost will prioritize these codes under "manf#" that will be used for get
@@ -288,43 +335,64 @@
             found_codes_for_all_dists = True
             for d in FIELDS_CAT:
                 part_stock = part.fields.get(d)
                 if part_stock:
                     part_catalogue_code_dist = d[:-1]
                     if part_catalogue_code_dist in available_distributors:
                         part_code_dist = api_partinfo_kitspace.KICOST2KITSPACE_DIST[part_catalogue_code_dist]
-                        queries.append('{"sku":{"vendor":"' + part_code_dist + '","part":"' + part_stock + '"}}')
-                        query_parts.append(part)
-                        query_part_stock_code.append([part_catalogue_code_dist])
+                        query_text = '{"sku":{"vendor":"' + part_code_dist + '","part":"' + part_stock + '"}}'
+                        queries.append(QueryStruct(query_text, part, [part_catalogue_code_dist]))
                         part_dist_use_manfpn.remove(part_catalogue_code_dist)
                 else:
                     found_codes_for_all_dists = False
 
             # Create a query using the manufacturer P/N
             part_manf = part.fields.get('manf', '')
             part_code = part.fields.get('manf#')
             if part_code and not found_codes_for_all_dists:
                 # Not all distributors has code, add a query for the manufaturer P/N
-                queries.append('{"mpn":{"manufacturer":"' + part_manf + '","part":"' + part_code + '"}}')
-                query_parts.append(part)
+                query_text = '{"mpn":{"manufacturer":"' + part_manf + '","part":"' + part_code + '"}}'
                 # List of distributors without an specific part number
-                query_part_stock_code.append(part_dist_use_manfpn)
+                queries.append(QueryStruct(query_text, part, part_dist_use_manfpn))
 
-        n_queries = len(query_parts)
+        n_queries = len(queries)
+        debug_overview('Queries {}'.format(n_queries))
         if not n_queries:
             return
-        # Setup progress bar to track progress of server queries.
-        progress = distributor_class.progress(n_queries, distributor_class.logger)
 
-        # Slice the queries into batches of the largest allowed size and gather
-        # the part data for each batch.
-        for i in range(0, len(queries), MAX_PARTS_PER_QUERY):
-            slc = slice(i, i+MAX_PARTS_PER_QUERY)
-            api_partinfo_kitspace.get_part_info(queries[slc], query_parts[slc], distributors, currency, query_part_stock_code[slc])
-            progress.update(len(queries[slc]))
-
-        # Done with the scraping progress bar so delete it or else we get an
-        # error when the program terminates.
-        progress.close()
+        # Try to solve the queries from the cache
+        unsolved = []
+        for query in queries:
+            # Solve the prefix and name
+            prefix, name = api_partinfo_kitspace.query2name(query.query)
+            # Look in the cache
+            query.result, query.loaded = api_partinfo_kitspace.cache.load_results(prefix, name)
+            if not query.loaded:
+                unsolved.append(query)
+            else:
+                debug_obsessive('Data from cache: '+pprint.pformat(query.result))
+
+        # Solve the rest from the site
+        n_unsolved = len(unsolved)
+        debug_overview('Cached entries {} (of {})'.format(n_queries-n_unsolved, n_queries))
+        if n_unsolved:
+            # Setup progress bar to track progress of server queries.
+            progress = distributor_class.progress(n_unsolved, distributor_class.logger)
+
+            # Slice the queries into batches of the largest allowed size and gather
+            # the part data for each batch.
+            for i in range(0, n_unsolved, MAX_PARTS_PER_QUERY):
+                slc = slice(i, i+MAX_PARTS_PER_QUERY)
+                api_partinfo_kitspace.get_part_info(unsolved[slc], distributors)
+                progress.update(len(unsolved[slc]))
+
+            # Done with the scraping progress bar so delete it or else we get an
+            # error when the program terminates.
+            progress.close()
+
+        # Transfer the results
+        solved_dist = set()
+        api_partinfo_kitspace.fill_part_info(queries, distributors, currency, solved_dist)
+        return solved_dist
 
 
 distributor_class.register(api_partinfo_kitspace, 50)
```

### Comparing `kicost-1.1.6/kicost/distributors/dist_local_template.py` & `kicost-1.1.8/kicost/distributors/dist_local_template.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 # THE SOFTWARE.
 
 # Libraries.
 import re
 import sys
 import hashlib
 
-from ..global_vars import SEPRTR, DEBUG_OVERVIEW, DEBUG_OBSESSIVE, W_BADPRICE
-from .. import DistData
+from .. import DistData, SEPRTR, W_BADPRICE
 # Distributors definitions.
 from .distributor import distributor_class
+from .log__ import debug_overview, debug_obsessive, warning
 
 __all__ = ['dist_local_template']
 
 if sys.version_info[0] < 3:
     from urlparse import urlsplit, urlunsplit
 
     def to_bytes(val):
@@ -64,24 +64,27 @@
 
 
 class dist_local_template(distributor_class):
     name = 'Local'
     type = 'local'
     enabled = True
     url = None
+    # We don't add distributors here, they are collected in query_part_info
+    api_distributors = []
 
     @staticmethod
-    def init_dist_dict():
-        # We don't add distributors here, they are collected in query_part_info
-        pass
+    def configure(ops):
+        for k, v in ops.items():
+            if k == 'enable':
+                dist_local_template.enabled = v
+        debug_obsessive('Local API configured to enabled {}'.format(dist_local_template.enabled))
 
     @staticmethod
-    def query_part_info(parts, distributors, currency):
-        """ Fill-in part information for locally-sourced parts not handled by Octopart.
-            IMPORTANT: `distributors` can be modified. """
+    def update_distributors(parts, distributors):
+        """ Looks for user defined distributors """
         # This loops through all the parts and finds any that are sourced from
         # local distributors that are not normally searched and places them into
         # the distributor disctionary.
         for part in parts:
             # Find the various distributors for this part by
             # looking for leading fields terminated by SEPRTR.
             for key in part.fields:
@@ -92,20 +95,25 @@
 
                 # If the distributor is not in the list of web-scrapable distributors,
                 # then it's a local distributor. Copy the local distributor template
                 # and add it to the table of distributors.
                 # Note: If the user excludes a web-scrapable distributors (using --exclude)
                 # and then adds it as a local distributor (using fields) it will be added.
                 if dist not in distributors:
-                    distributor_class.logger.log(DEBUG_OVERVIEW, 'Creating \'{}\' local distributor profile...'.format(dist))
+                    debug_overview('Creating \'{}\' local distributor profile...'.format(dist))
                     new_dist = distributor_class.get_distributor_template('local_template')
                     new_dist.label.name = dist  # Set dist name for spreadsheet header.
                     distributor_class.add_distributor(dist, new_dist)
                     distributors.append(dist)
+                    dist_local_template.api_distributors.append(dist)
 
+    @staticmethod
+    def query_part_info(parts, distributors, currency):
+        """ Fill-in part information for locally-sourced parts not handled by Octopart. """
+        solved = set()
         # Loop through the parts looking for those sourced by local distributors
         # that won't be found online. Place any user-added info for these parts
         # (such as pricing) into the part dictionary.
         for p in parts:
             # Find the manufacturer's part number if it exists.
             pn = p.fields.get('manf#')  # Returns None if no manf# field.
 
@@ -126,15 +134,15 @@
                 if link:
                     url_parts = list(urlsplit(link))
                     if url_parts[0] == '':
                         url_parts[0] = u'http'
                     link = urlunsplit(url_parts)
                 else:
                     # This happens when no part URL is found.
-                    distributor_class.logger.log(DEBUG_OBSESSIVE, 'No part URL found for local \'{}\' distributor!'.format(dist))
+                    debug_obsessive('No part URL found for local \'{}\' distributor!'.format(dist))
                 dd.url = link
 
                 price_tiers = {}
                 try:
                     local_currency = re.findall('[a-zA-Z]{3}', pricing)[0].upper()
                 except Exception:
                     local_currency = currency
@@ -145,20 +153,24 @@
                     if len(splitted) == 2:
                         qty, price = splitted
                         if local_currency:
                             dd.currency = local_currency
                         try:
                             price_tiers[int(qty)] = float(price)
                         except ValueError:
-                            distributor_class.logger.warning(W_BADPRICE+'Malformed pricing number: `{}` at {}'.format(old_pricing, p.refs))
+                            warning(W_BADPRICE, 'Malformed pricing number: `{}` at {}'.format(old_pricing, p.refs))
                     else:
-                        distributor_class.logger.warning(W_BADPRICE+'Malformed pricing entry: `{}` at {}'.format(qty_price, p.refs))
+                        warning(W_BADPRICE, 'Malformed pricing entry: `{}` at {}'.format(qty_price, p.refs))
                 # dd.moq = min(price_tiers.keys())
                 if not price_tiers:
                     # This happens when no pricing info is found.
-                    distributor_class.logger.log(DEBUG_OBSESSIVE, 'No pricing information found for local \'{}\' distributor!'.format(dist))
+                    debug_obsessive('No pricing information found for local \'{}\' distributor!'.format(dist))
                 dd.price_tiers = price_tiers
                 # Update the DistData for this distributor
                 p.dd[dist] = dd
+                # We have data for this distributor. Avoid marking normal distributors.
+                if dist in dist_local_template.api_distributors:
+                    solved.add(dist)
+        return solved
 
 
 distributor_class.register(dist_local_template, 100)
```

### Comparing `kicost-1.1.6/kicost/distributors/distributors_info.py` & `kicost-1.1.8/kicost/distributors/distributors_info.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/distributors/global_vars.py` & `kicost-1.1.8/kicost/distributors/global_vars.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/edas/__init__.py` & `kicost-1.1.8/kicost/edas/__init__.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/edas/eda.py` & `kicost-1.1.8/kicost/edas/eda.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 import os
 import re
 from collections import OrderedDict
-from ..global_vars import logger, DEBUG_OVERVIEW, SEPRTR, DEBUG_OBSESSIVE, W_FLDOVR
+from .. import DEBUG_OVERVIEW, DEBUG_OBSESSIVE, SEPRTR, W_FLDOVR
 from ..distributors import get_distributors_iter
 
 __all__ = ['eda_class', 'field_name_translations']
 
 
 # Generate a dictionary to translate all the different ways people might want
 # to refer to part numbers, vendor numbers, manufacture name and such.
@@ -151,20 +151,20 @@
                 return
             f = field_name_translations.get(f, f)
             if f in ignore_fields:
                 return
             # Is distributor related?
             if f in ('cat#', 'pricing', 'link'):
                 # Add it to the default local distributor
-                logger.log(DEBUG_OBSESSIVE, 'Assigning name "{}" to "Local" distributor'.format(f))
+                eda_class.logger.log(DEBUG_OBSESSIVE, 'Assigning name "{}" to "Local" distributor'.format(f))
                 f = 'Local:' + f
         # Note: here we allow a field to "clear" another definition (assigning an empty value)
         # This is because we assume that "kicost*" fields are defined on purpose, not just inherited from the library
         new_fields[f] = v.strip()
-        logger.log(DEBUG_OBSESSIVE, '{} Field {} -> {}={}'.format(ref, name_ori, f, v))
+        eda_class.logger.log(DEBUG_OBSESSIVE, '{} Field {} -> {}={}'.format(ref, name_ori, f, v))
 
     @staticmethod
     def process_fields(parts, variant, ignore_fields, distributors):
         new_parts = OrderedDict()
         for ref, fields in parts.items():
             new_fields = OrderedDict()
             # Add the fields from lowest to highest priority.
@@ -185,15 +185,15 @@
                 v = v.strip()
                 already_defined = f in new_fields
                 if not v and already_defined:
                     # For regular fields we avoid one alias clearing another.
                     # Example: if manf# was defined as XXX and now we have mnp='' we avoid getting manf#=''
                     continue
                 if already_defined and new_fields[f]:
-                    logger.warning(W_FLDOVR+'Warning: in {} overwriting {}={} with {}={}'.format(ref, f, new_fields[f], old_name, v))
+                    eda_class.logger.warning(W_FLDOVR+'Warning: in {} overwriting {}={} with {}={}'.format(ref, f, new_fields[f], old_name, v))
                 new_fields[f] = v
             # 2) kicost:FIELD
             for f, v in fields.items():
                 if f.startswith('kicost' + SEPRTR):
                     eda_class.process_kicost_field(f[7:], v, new_fields, ignore_fields, distributors, f, ref)
             # 3) kicost.VARIANT:  (highest priority)
             for f, v in fields.items():
@@ -201,15 +201,15 @@
                     continue
                 sep_pos = f.index(SEPRTR)
                 var = f[7:sep_pos]
                 if not re.match(variant, var, flags=re.IGNORECASE):
                     # Not for the current variant
                     continue
                 name = f[sep_pos+1:]
-                logger.log(DEBUG_OBSESSIVE, 'Matched Variant ... ' + var + '.' + name)
+                eda_class.logger.log(DEBUG_OBSESSIVE, 'Matched Variant ... ' + var + '.' + name)
                 eda_class.process_kicost_field(name, v, new_fields, ignore_fields, distributors, f, ref)
             # TODO: What about the other cases?
             # * Has ':' but doesn't start with "kicost"
             new_parts[ref] = new_fields
         return new_parts
 
     @staticmethod
@@ -241,15 +241,15 @@
            Remove components that are assigned to a variant that is not the current variant,
            or which are "do not populate" (DNP). (Any component that does not have a variant
            is assigned the current variant so it will not be removed unless it is also DNP.)
 
            @param components Part components in a `list()` of `dict()`, format given by the EDA modules.
            @return `list()` of `dict()`.
         '''
-        logger.log(DEBUG_OVERVIEW, '# Removing do not populate parts...')
+        eda_class.logger.log(DEBUG_OVERVIEW, '# Removing do not populate parts...')
         accepted_components = OrderedDict()
         for ref, fields in components.items():
             # Remove DNPs.
             dnp = fields.get('dnp', '0')
             # Interpret empty strings as 0. See #471 discussion.
             if dnp == '':
                 dnp = '0'
```

### Comparing `kicost-1.1.6/kicost/edas/eda_altium.py` & `kicost-1.1.8/kicost/edas/eda_altium.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 # Libraries.
 import sys
 import os
 import copy  # Necessary because Py2 doesn't have copy in list.
 from datetime import datetime
 from bs4 import BeautifulSoup  # To Read XML files.
 import re  # Regular expression parser.
-from ..global_vars import DEBUG_OVERVIEW, ERR_INPUTFILE, KiCostError  # Debug configurations.
 from .tools import field_name_translations, PART_REF_REGEX_NOT_ALLOWED
 from .eda import eda_class
+from .log__ import debug_overview
+from .. import KiCostError, ERR_INPUTFILE
 
 ALTIUM_NONE = '[NoParam]'  # Value of Altium to `None`.
 ALTIUM_PART_SEPRTR = r'(?<!\\),\s*'  # Separator for the part numbers in a list, remove the lateral spaces.
 FILE_REGEX = r'\<GRID[\s\S]+<COLUMNS>[\s\S]+<COLUMN[\s\S]+<\/COLUMNS>[\s\S]+<ROWS>[\s\S]+\<ROW[\s\S]+\<\/ROWS>[\s\S]+\<\/GRID>'
 
 __all__ = ['eda_altium']
 
@@ -97,26 +98,26 @@
 
 def get_part_groups(in_file):
     '''@brief Get groups of identical parts from an XML file and return them as a dictionary.
        @param in_file `str()` with the file name.
        @return `dict()` of the parts designed. The keys are the componentes references.
     '''
     # Read-in the schematic XML file to get a tree and get its root.
-    eda_class.logger.log(DEBUG_OVERVIEW, '# Getting from XML \'{}\' Altium BoM...'.format(
+    debug_overview('# Getting from XML \'{}\' Altium BoM...'.format(
                                     os.path.basename(in_file)))
     file_h = open(in_file)
     root = BeautifulSoup(file_h, 'lxml')
     file_h.close()
 
     # Get the header of the XML file of Altium, so KiCost is able to to
     # to get all the informations in the file.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Getting the XML table header...')
+    debug_overview('Getting the XML table header...')
     header = [extract_field(entry, 'name') for entry in root.find('columns').find_all('column')]
 
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Getting components...')
+    debug_overview('Getting components...')
     accepted_components = {}
     for row in root.find('rows').find_all('row'):
 
         # Get the values for the fields in each library part (if any).
         refs, fields = extract_fields_row(row, header)
         for i in range(len(refs)):
             ref = refs[i]
```

### Comparing `kicost-1.1.6/kicost/edas/eda_kicad.py` & `kicost-1.1.8/kicost/edas/eda_kicad.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 # Libraries.
 import os
 from datetime import datetime
 import re
 from bs4 import BeautifulSoup
 from collections import OrderedDict
-from ..global_vars import DEBUG_OVERVIEW, SEPRTR
+from .. import SEPRTR
 from .eda import eda_class
+from .log__ import debug_overview
 
 
 __all__ = ['eda_kicad']
 
 
 def extract_fields(part):
     ''' Extract XML fields from the part in a library or schematic. '''
@@ -65,32 +66,32 @@
 
 def get_part_groups(in_file):
     '''Get groups of identical parts from an XML file and return them as a dictionary.
        @param in_file `str()` with the file name.
        @return `dict()` of the parts designed. The keys are the componentes references.
     '''
     # Read-in the schematic XML file to get a tree and get its root.
-    eda_class.logger.log(DEBUG_OVERVIEW, '# Getting from XML \'{}\' KiCad BoM...'.format(
+    debug_overview('# Getting from XML \'{}\' KiCad BoM...'.format(
                                     os.path.basename(in_file)))
     file_h = open(in_file)
     root = BeautifulSoup(file_h, 'lxml')
     file_h.close()
 
     # Get the general information of the project BoM XML file.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Getting authorship data...')
+    debug_overview('Getting authorship data...')
     title = root.find('title_block')
 
     prj_info = dict()
     prj_info['title'] = title_find_all(title, 'title') or os.path.basename(in_file)
     prj_info['company'] = title_find_all(title, 'company')
     prj_info['date'] = title_find_all(root, 'date') or (datetime.fromtimestamp(os.path.getmtime(in_file)).strftime("%Y-%m-%d %H:%M:%S") + ' (file)')
 
     # Make a dictionary from the fields in the parts library so these field
     # values can be instantiated into the individual components in the schematic.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Getting parts library...')
+    debug_overview('Getting parts library...')
     libparts = {}
     if root.find('libparts'):
         for p in root.find('libparts').find_all('libpart'):
 
             # Get the values for the fields in each library part (if any).
             fields = extract_fields(p)
 
@@ -104,27 +105,27 @@
                     libparts[str(p['lib']) + SEPRTR + str(alias.string)] = fields
             except AttributeError:
                 pass  # No aliases for this part.
 
     # Find the components used in the schematic and elaborate
     # them with global values from the libraries and local values
     # from the schematic.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Getting components...')
+    debug_overview('Getting components...')
     components = OrderedDict()
     for c in root.find('components').find_all('comp'):
 
         # Find the library used for this component.
         libsource = c.find('libsource')
         if libsource:
             # Create the key to look up the part in the libparts dict.
             # libpart = str(libsource['lib'] + SEPRTR + libsource['part'])
             libpart = str(libsource['lib']) + SEPRTR + str(libsource['part'])
         else:
             libpart = '???'
-            eda_class.logger.log(DEBUG_OVERVIEW, 'Footprint library not assigned to {}'.format(''))  # TODO
+            debug_overview('Footprint library not assigned to {}'.format(''))  # TODO
 
         # Initialize the fields from the global values in the libparts dict entry.
         # (These will get overwritten by any local values down below.)
         # (Use an empty dict if no part exists in the library.)
         fields = libparts.get(libpart, OrderedDict()).copy()  # Make a copy! Don't use reference!
 
         # Store the part key and its value.
```

### Comparing `kicost-1.1.6/kicost/edas/generic_csv.py` & `kicost-1.1.8/kicost/edas/generic_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,18 @@
 # Libraries.
 import sys
 import os
 from datetime import datetime
 from collections import OrderedDict
 import csv  # CSV file reader.
 import re  # Regular expression parser.
-from ..global_vars import DEBUG_OVERVIEW, ERR_INPUTFILE, KiCostError, W_DUPWRONG
 from .tools import field_name_translations, split_refs
 from .eda import eda_class
+from .log__ import debug_overview, warning
+from .. import KiCostError, ERR_INPUTFILE, W_DUPWRONG
 
 
 GENERIC_PREFIX = 'GEN'  # Part reference prefix to use when no references are present.
 
 __all__ = ['generic_csv']
 
 
@@ -50,15 +51,15 @@
     # Get the correspondent first valid value of `vals` look from a key
     # in `header`, but using `header_file` to access `vals`. Used to get
     # the designator reference `refs` and quantity `qty`.
     idx = [i for i, x in enumerate(header) if x == key]
     value = None
     for i in idx:
         if len(idx) > 1 and value is not None and value != vals[header_file[i]]:
-            eda_class.logger.warning(W_DUPWRONG+'Found different duplicated information for \'{}\': \'{}\'=!\'{}\'. Will be used the last.'.format(
+            warning(W_DUPWRONG, 'Found different duplicated information for \'{}\': \'{}\'=!\'{}\'. Will be used the last.'.format(
                 key, value, vals[header_file[i]]))
         value = vals[header_file[i]]
         if value:
             break
     return value
 
 
@@ -98,17 +99,17 @@
                 # This is for Python 3 where the values are already unicode.
                 value = vals.get(h_file)
             else:
                 # For Python 2, create unicode versions of strings.
                 value = vals.get(h_file, '').decode('utf-8')
             try:
                 if value and fields[h] != value:
-                    eda_class.logger.warning(W_DUPWRONG+'Found different duplicated information for {} in '
-                                             'the titles [\'{}\', \'{}\']: \'{}\'=!\'{}\'. Will be used \'{}\'.'.
-                                             format(refs, h, h_file, fields[h], value, value))
+                    warning(W_DUPWRONG, 'Found different duplicated information for {} in '
+                            'the titles [\'{}\', \'{}\']: \'{}\'=!\'{}\'. Will be used \'{}\'.'.
+                            format(refs, h, h_file, fields[h], value, value))
             except KeyError:
                 pass
             finally:
                 # Use the translated header title, this is used to deal
                 # with duplicated information that could be found by
                 # translating header titles that are the same for KiCost.
                 fields[h] = value
@@ -126,15 +127,15 @@
 
 
 def get_part_groups(in_file, distributors):
     '''Get groups of identical parts from an generic CSV file and return them as a dictionary.
        @param in_file `str()` with the file name.
        @return `dict()` of the parts designed. The keys are the components references.
     '''
-    eda_class.logger.log(DEBUG_OVERVIEW, '# Getting from CSV \'{}\' BoM...'.format(
+    debug_overview('# Getting from CSV \'{}\' BoM...'.format(
                                     os.path.basename(in_file)))
     try:
         file_h = open(in_file, 'r')
         content = file_h.read()
     except UnicodeDecodeError:  # It happens with some Windows CSV files on Python 3.
         file_h.close()
         file_h = open(in_file, 'r', encoding='ISO-8859-1')
@@ -150,18 +151,18 @@
     except csv.Error:
         # If the CSV file only has a single column of data, there may be no
         # delimiter so just set the delimiter to a comma.
         dialect = csv.Sniffer().sniff(',,,', [','])
 
     # The first line in the file must be the column header.
     content = content.splitlines()
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Getting CSV header...')
+    debug_overview('Getting CSV header...')
     header_file = next(csv.reader(content, delimiter=dialect.delimiter))
     if len(set(header_file)) < len(header_file):
-        eda_class.logger.warning(W_DUPWRONG+'There is a duplicated header title in the file. This could cause loss of information.')
+        warning(W_DUPWRONG, 'There is a duplicated header title in the file. This could cause loss of information.')
 
     # Standardize the header titles and remove the spaces before
     # and after, striping the text improve the user experience.
     header = [field_name_translations.get(hdr.strip().lower(), hdr.strip().lower()) for hdr in header_file]
 
     # Examine the first line to see if it really is a header.
     # If the first line contains a column header that is not in the list of
@@ -189,15 +190,15 @@
             header = ['qty', 'manf#', 'refs']
     else:
         # OK, the first line is a header, so remove it from the data.
         content.pop(0)  # Remove the header from the content.
 
     # Make a dictionary from the fields in the parts library so these field
     # values can be instantiated into the individual components in the schematic.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Getting parts...')
+    debug_overview('Getting parts...')
 
     # Read the each line content.
     accepted_components = OrderedDict()
     gen_cntr = 0
     for row in content:
         # Get the values for the fields in each library part (if any).
         refs, fields, gen_cntr = extract_fields(row, header, header_file, dialect, gen_cntr)
```

### Comparing `kicost-1.1.6/kicost/edas/tools.py` & `kicost-1.1.8/kicost/edas/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 __webpage__ = 'https://github.com/hildogjr/'
 __company__ = 'University of Campinas - Brazil'
 
 # Libraries.
 import re  # Regular expression parser and matches.
 from collections import OrderedDict
 from .. import PartGroup
-from ..global_vars import SEPRTR, DEBUG_OVERVIEW, DEBUG_OBSESSIVE, DEBUG_DETAILED, DEBUG_FULL, ERR_FIELDS, KiCostError, W_INCQTY, W_REPMAN, W_MANQTY
 from ..distributors import get_distributors_iter
-from .eda import eda_class, field_name_translations
+from .eda import field_name_translations
+from .log__ import debug_overview, debug_obsessive, debug_detailed, debug_full, warning, is_debug_full
+from .. import KiCostError, SEPRTR, ERR_FIELDS, W_INCQTY, W_REPMAN, W_MANQTY
 
 __all__ = ['partgroup_qty', 'groups_sort', 'order_refs', 'subpartqty_split', 'group_parts']
 
 # Qty and part separators are escaped by preceding with '\' = (?<!\\)
 QTY_SEPRTR = r'(?<!\\)\s*[:]\s*'  # Separator for the subpart quantity and the part number, remove the lateral spaces.
 PART_SEPRTR = r'(?<!\\)\s*\|\s*'             # Separator for the part numbers in a list, remove the lateral spaces.
 PART_SEPRTR_LEGACY = r'(?<!\\)\s*[;,\|]\s*'  # Legacy version
@@ -106,16 +107,16 @@
        parts of different BOMs (in the mode of multifiles).
        @param components Part components in a `list()` of `dict()`, format given by the EDA modules.
        @param fields_merge Data fields of the `dict()` variable to be merged and ignored to make the identical components group
        (before be scraped in the distributors web site).
        @return `list()` of `dict()`
     """
 
-    eda_class.logger.log(DEBUG_OVERVIEW, '# Grouping parts...')
-    ultra_debug = eda_class.logger.getEffectiveLevel() <= DEBUG_FULL
+    debug_overview('# Grouping parts...')
+    ultra_debug = is_debug_full()
 
     # All codes to scrape, do not include code field name of distributors
     # that will not be scraped. This definition is used to create and check
     # the identical groups or subsplit the seemingly identical parts.
     FIELDS_MANFCAT = ([d + '#' for d in get_distributors_iter()] + ['manf#'])
     # Calculated all the fields that never have to be used to create the hash keys.
     # These include all the manufacture company and codes, distributors codes
@@ -131,15 +132,15 @@
             raise KiCostError('Manufacturer/distributor codes and manufacture company "{}"'
                               ' can\'t be ignored to create the components groups.'.format(c), ERR_FIELDS)
     FIELDS_NOT_HASH = FIELDS_NOT_HASH + fields_merge  # Not use the fields do merge to create the hash.
 
     # Now partition the parts into groups of like components.
     # First, get groups of identical components but ignore any manufacturer's
     # part numbers that may be assigned. Just collect those in a list for each group.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Getting groups of identical components...')
+    debug_overview('Getting groups of identical components...')
     component_groups = OrderedDict()
     for ref, fields in components.items():  # part references and field values.
 
         # Take the field keys and values of each part and create a hash.
         # Use the hash as the key to a dictionary that stores lists of
         # part references that have identical field values. The important fields
         # are the reference prefix ('R', 'C', etc.), value, and footprint.
@@ -167,19 +168,19 @@
             # Add next ref for identical part to the list.
             grp.refs.append(ref)
             # Also add any manufacturer's part number (or None) and each distributor
             # stock catalogue code to the group's list.
             for f in FIELDS_MANFCAT:
                 grp.manfcat_codes[f][get_manfcat(fields, f)] = True
     if ultra_debug:
-        eda_class.logger.log(DEBUG_FULL, '\n\n\n1++++++++++++++' + str(len(component_groups)))
+        debug_full('\n\n\n1++++++++++++++' + str(len(component_groups)))
         for g, grp in list(component_groups.items()):
-            eda_class.logger.log(DEBUG_FULL, '\n' + str(grp.refs))
+            debug_full('\n' + str(grp.refs))
             for r in grp.refs:
-                eda_class.logger.log(DEBUG_FULL, str(r) + str(components[r]))
+                debug_full(str(r) + str(components[r]))
 
     # Now we have groups of seemingly identical parts. But some of the parts
     # within a group may have different manufacturer's part numbers, and these
     # groups may need to be split into smaller groups of parts all having the
     # same manufacturer's number. Here are the cases that need to be handled:
     #   One manf# number (and one cat# for each distributor):
     #       All parts have the same manf#. Don't split this group.
@@ -192,15 +193,15 @@
     #       the group into two smaller groups of parts all having the same
     #       manf# and distributor#.
     #   Three or more manf# (or distributor#):
     #       Split this group into smaller groups, each one with parts having
     #       the same manf# and distributor#, even if it's `None`. It's
     #       impossible to determine which manf# the `None` parts should be
     #       assigned to, so leave their manf# as `None`.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Checking the seemingly identical parts group...')
+    debug_overview('Checking the seemingly identical parts group...')
     new_component_groups = []  # Copy new component groups into this.
     for g, grp in component_groups.items():
         num_manfcat_codes = {f: len(grp.manfcat_codes[f]) for f in FIELDS_MANFCAT}
         if all([num_manfcat_codes[f] == 1 or (num_manfcat_codes[f] == 2 and None in grp.manfcat_codes[f]) for f in FIELDS_MANFCAT]):
             new_component_groups.append(grp)
             # CASE ONE and TWO:
             # Single manf# and distributor catalogue. Or a seemingly
@@ -237,25 +238,25 @@
                 # Use get() which returns `None` if the component has no
                 # manf# or distributor# field. That will match if the
                 # group manf_num is also None. So append the par to the group.
                 if all([get_manfcat(components[ref], f) == manfcat_num[f] for f in FIELDS_MANFCAT]):
                     sub_group.refs.append(ref)
             new_component_groups.append(sub_group)  # Append one part of the split group.
     if ultra_debug:
-        eda_class.logger.log(DEBUG_FULL, '\n\n\n2++++++++++++++' + str(len(new_component_groups)))
+        debug_full('\n\n\n2++++++++++++++' + str(len(new_component_groups)))
         for grp in new_component_groups:
-            eda_class.logger.log(DEBUG_FULL, '\n' + str(grp.refs))
+            debug_full('\n' + str(grp.refs))
             for r in grp.refs:
-                eda_class.logger.log(DEBUG_FULL, str(r) + ' ' + str(components[r]))
+                debug_full(str(r) + ' ' + str(components[r]))
 
     # If the identical components grouped have difference in the `fields_merge`
     # so replace this field with a string composed line-by-line with the
     # occurrences (definition `SGROUP_SEPRTR`) preceded with the refs
     # collapsed plus `SEPRTR`. Implementation of the ISSUE #102.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Merging field asked in the identical components groups...')
+    debug_overview('Merging field asked in the identical components groups...')
     if fields_merge:
         fields_merge = [field_name_translations.get(f.lower(), f.lower()) for f in fields_merge]
         for grp in new_component_groups:
             components_grp = [components[i] for i in grp.refs]
             for f in fields_merge:
                 values_field = set([cmp.get(f, '') for cmp in components_grp])  # Different values
                 ocurrences = {v_g: [r for r in grp.refs if components[r].get(f, '') == v_g] for v_g in values_field if v_g}
@@ -263,23 +264,23 @@
                     if f == 'desc' and len(ocurrences) == 2 and '' in ocurrences:
                         value = ''.join(list(ocurrences.keys()))
                     else:
                         value = SGROUP_SEPRTR.join([order_refs(r)[0] + SEPRTR + ' ' + t for t, r in sorted(ocurrences.items())])
                     for r in grp.refs:
                         components[r][f] = value
     if ultra_debug:
-        eda_class.logger.log(DEBUG_FULL, '\n\n\n3++++++++++++++' + str(len(new_component_groups)))
+        debug_full('\n\n\n3++++++++++++++' + str(len(new_component_groups)))
         for grp in new_component_groups:
-            eda_class.logger.log(DEBUG_FULL, grp.refs)
+            debug_full(grp.refs)
             for r in grp.refs:
-                eda_class.logger.log(DEBUG_FULL, str(r) + str(components[r]))
+                debug_full(str(r) + str(components[r]))
 
     # Now get the values of all fields within the members of a group.
     # These will become the field values for ALL members of that group.
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Propagating field values to identical components...')
+    debug_overview('Propagating field values to identical components...')
     for grp in new_component_groups:
         grp_fields = OrderedDict()
         # Multiprojects has a list of qty's
         # So we use a list and reduce it to one single element if needed
         grp_qtys = [0]*c_prjs
         for ref in grp.refs:
             comp = components[ref]
@@ -306,62 +307,62 @@
             for i in range(c_prjs):
                 grp_qtys[i] += qty[i]
         grp_fields['manf#_qty'] = grp_qtys[0] if c_prjs == 1 else grp_qtys
         grp.fields = grp_fields
 
     # Now return the list of identical part groups.
     if ultra_debug:
-        eda_class.logger.log(DEBUG_FULL, '\n\n\n4------------')
+        debug_full('\n\n\n4------------')
         for grp in new_component_groups:
-            eda_class.logger.log(DEBUG_FULL, grp.refs)
-            eda_class.logger.log(DEBUG_FULL, grp.fields)
+            debug_full(grp.refs)
+            debug_full(grp.fields)
             for r in grp.refs:
-                eda_class.logger.log(DEBUG_FULL, str(r) + str(components[r]))
-        eda_class.logger.log(DEBUG_FULL, '\n\n\n------------')
+                debug_full(str(r) + str(components[r]))
+        debug_full('\n\n\n------------')
     return new_component_groups
 
 
 def groups_sort(new_component_groups):
     '''@brief Order the groups in a alphabetical way.
 
        Put the components groups in the spreadsheet rows in a specific order
        using the reference string of the components. The order is defined
        by BOM_ORDER.
        @param components Part components in a `list()` of `dict()`, format given by the EDA modules.
        @return Same as input.
     '''
 
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Sorting the groups for better visualization...')
+    debug_overview('Sorting the groups for better visualization...')
 
     ref_identifiers = re.split(r'(?<![\W\*\/])\s*,\s*|\s*,\s*(?![\W\*\/])',
                                BOM_ORDER, flags=re.IGNORECASE)
     component_groups_order_old = list(range(0, len(new_component_groups)))
     component_groups_order_new = list()
     component_groups_refs = [new_component_groups[g].fields.get('reference') for g in component_groups_order_old]
-    eda_class.logger.log(DEBUG_OBSESSIVE, 'All ref identifier: {}'.format(ref_identifiers))
-    eda_class.logger.log(DEBUG_OBSESSIVE, '{} groups of components.'.format(len(component_groups_order_old)))
-    eda_class.logger.log(DEBUG_OBSESSIVE, 'Identifiers founded {}.'.format(component_groups_refs))
+    debug_obsessive('All ref identifier: {}'.format(ref_identifiers))
+    debug_obsessive('{} groups of components.'.format(len(component_groups_order_old)))
+    debug_obsessive('Identifiers founded {}.'.format(component_groups_refs))
     for ref_identifier in ref_identifiers:
         component_groups_ref_match = [i for i in range(0, len(component_groups_refs)) if ref_identifier == component_groups_refs[i].lower()]
-        eda_class.logger.log(DEBUG_OBSESSIVE, 'Identifier: {} in {}.'.format(ref_identifier, component_groups_ref_match))
+        debug_obsessive('Identifier: {} in {}.'.format(ref_identifier, component_groups_ref_match))
         if len(component_groups_ref_match) > 0:
             # If found more than one group with the reference, use the 'manf#'
             # as second order criteria.
             if len(component_groups_ref_match) > 1:
                 try:
                     for item in component_groups_ref_match:
                         component_groups_order_old.remove(item)
                 except ValueError:
                     pass
                 # Examine 'manf#' and refs to get the order.
                 # Order by refs that have 'manf#' codes, that ones that don't have stay at the end of the group.
                 group_manf_list = [new_component_groups[h].fields.get('manf#') for h in component_groups_ref_match]
                 group_refs_list = [new_component_groups[h].refs for h in component_groups_ref_match]
                 sorted_groups = sorted(range(len(group_refs_list)), key=lambda k: (group_manf_list[k] is None,  group_refs_list[k]))
-                eda_class.logger.log(DEBUG_OBSESSIVE, '{} > order: {}'.format(group_manf_list, sorted_groups))
+                debug_obsessive('{} > order: {}'.format(group_manf_list, sorted_groups))
                 component_groups_ref_match = [component_groups_ref_match[i] for i in sorted_groups]
                 component_groups_order_new += component_groups_ref_match
             else:
                 try:
                     component_groups_order_old.remove(component_groups_ref_match[0])
                 except ValueError:
                     pass
@@ -381,15 +382,15 @@
        For each designator...
        For designator with a "single subpart" check with the quantity
        is more than one.
 
        @param components Part components in a `list()` of `dict()`, format given by the EDA modules.
        @return Same as the input.
     '''
-    eda_class.logger.log(DEBUG_OVERVIEW, 'Splitting subparts in the manufacture / distributors codes...')
+    debug_overview('Splitting subparts in the manufacture / distributors codes...')
 
     FIELDS_MANF = [d+'#' for d in distributors]
     FIELDS_MANF.append('manf#')
     split_extra_fields = [f.lower() for f in split_extra_fields]
     split_extra_fields.append('pricing')
 
     split_components = OrderedDict()
@@ -408,19 +409,19 @@
                 subparts = subpart_list(part[field_code])
                 subparts_qty_field = len(subparts)
                 subparts_qty = max(subparts_qty, subparts_qty_field)  # Quantity of sub parts.
                 # Print a warning and an user tip in the case of different subpart quantities
                 # associated in different `manf#`/distributors# of the same component.
                 if subparts_qty_field != subparts_qty:
                     problem_manf_code = (field_code if subparts_qty > subparts_qty_field else field_code_last)
-                    eda_class.logger.warning(W_INCQTY+'Found a different subpart quantity between the code fields {c} and {lc}.\n'
-                                             '\tYou should consider use \"{pc}={m}\" on {r} to disambiguate that.'
-                                             .format(c=field_code_last, lc=field_code, r=part_ref,
-                                                     pc=problem_manf_code,
-                                                     m=';'.join(subpart_list(part[problem_manf_code])+['']*abs(subparts_qty - subparts_qty_field))))
+                    warning(W_INCQTY, 'Found a different subpart quantity between the code fields {c} and {lc}.\n'
+                                      '\tYou should consider use \"{pc}={m}\" on {r} to disambiguate that.'
+                                      .format(c=field_code_last, lc=field_code, r=part_ref,
+                                              pc=problem_manf_code,
+                                              m=';'.join(subpart_list(part[problem_manf_code])+['']*abs(subparts_qty - subparts_qty_field))))
                 field_code_last = field_code
                 fields_found.append(field_code)
                 subparts_manf_code[field_code] = subparts
         if not fields_found:
             split_components[part_ref] = part
             # TODO What about other fields?
             continue  # If not manf/distributor code pass to next.
@@ -436,15 +437,15 @@
         # Divide the pricing fields (won't apply quantity, this is why this is a separated list)
         subparts_extra = {}
         for field, value in part.items():
             for extra_field in split_extra_fields:
                 if field == extra_field or field.endswith(':' + extra_field):
                     subparts_extra[field] = subpart_list(value, legacy=False)
 
-        eda_class.logger.log(DEBUG_DETAILED, '{} >> {}'.format(part_ref, fields_found))
+        debug_detailed('{} >> {}'.format(part_ref, fields_found))
 
         # Second, if more than one subpart, split the sub parts as
         # new components with the same description, footprint, and
         # so on... Get the subpart.
         is_multi = subparts_qty > 1
         part_actual = part
         part_actual_value = part_actual['value']
@@ -475,38 +476,38 @@
                 # U1.3:{'manf#':'PARTG3'}
                 if subparts_index >= len(subparts_manf_code[field_manf_dist_code]):
                     continue
                 p_manf_code = subparts_manf_code[field_manf_dist_code][subparts_index]
                 subpart_qty, subpart_part = manf_code_qtypart(p_manf_code)
                 subpart_actual[field_manf_dist_code] = subpart_part
                 subpart_actual[field_manf_dist_code+'_qty'] = subpart_qty
-                eda_class.logger.log(DEBUG_OBSESSIVE, subpart_actual)
+                debug_obsessive(subpart_actual)
                 # Warn the user about different quantities asigned to different `manf#`
                 # and catalogue number of same part/subpart. Which may be a type error by
                 # the user.
                 if p_manf_code and p_manf_code_prior and subpart_qty_prior != subpart_qty:
-                    eda_class.logger.warning(W_INCQTY+'Different quantities signed between \"{f}={c}\" and \"{fl}={cl}\" at \"{r}\". Make sure that is right.'.
-                                             format(f=field_manf_dist_code, fl=field_manf_dist_code_prior,
-                                                    c=p_manf_code, cl=p_manf_code_prior, r=order_refs(list(components.keys()))[0]))
+                    warning(W_INCQTY, 'Different quantities signed between \"{f}={c}\" and \"{fl}={cl}\" at \"{r}\". Make sure that is right.'.
+                                      format(f=field_manf_dist_code, fl=field_manf_dist_code_prior,
+                                             c=p_manf_code, cl=p_manf_code_prior, r=order_refs(list(components.keys()))[0]))
                 # Memorize prior value for the above warning
                 subpart_qty_prior = subpart_qty
                 p_manf_code_prior = p_manf_code
                 field_manf_dist_code_prior = field_manf_dist_code
             if is_multi:
                 # Update other fields
                 for field, values in subparts_extra.items():
                     subpart_actual[field] = values[subparts_index] if subparts_index < len(values) else ''
                 # Update the split `manf`(manufactures names).
                 if subparts_manf[subparts_index] != REPLICATE_MANF:
                     # If the actual manufacture name is the defined as `REPLICATE_MANF`
                     # replicate the last one.
                     p_manf = subparts_manf[subparts_index]
                 elif p_manf is None:
-                    eda_class.logger.warning(W_REPMAN+'Asking to repeat a manufacturer in the first entry (at {})'.
-                                             format(order_refs(list(components.keys()))[0]))
+                    warning(W_REPMAN, 'Asking to repeat a manufacturer in the first entry (at {})'.
+                                      format(order_refs(list(components.keys()))[0]))
                 subpart_actual['manf'] = p_manf
                 # Update the reference of the part.
                 ref = part_ref + SUB_SEPRTR + str(subparts_index + 1)
             else:
                 ref = part_ref
             split_components[ref] = subpart_actual
     return split_components
@@ -515,15 +516,15 @@
 def qty2float(value):
     try:
         if isinstance(value, str) and '/' in value:
             vals = value.split('/')
             return float(vals[0])/float(vals[1])
         return float(value)
     except ValueError:
-        eda_class.logger.warning(W_MANQTY+'Malformed `manf#_qty`: ' + str(value))
+        warning(W_MANQTY, 'Malformed `manf#_qty`: ' + str(value))
         return 1.0
 
 
 def partgroup_qty(component):
     """@brief Take the components grouped quantity.
 
        Calculate the string of the quantity of the group parsing the
@@ -534,15 +535,15 @@
        recorded the quantities used in each project.
 
        @param components Part component `dict()`, format given by the EDA modules.
        @return Quantity of the manf# part used.
     """
     qty = component.fields.get('manf#_qty')
 
-    eda_class.logger.log(DEBUG_OBSESSIVE, 'Qty>> {}\t {}*{}'.format(component.refs, qty, component.fields.get('manf#')))
+    debug_obsessive('Qty>> {}\t {}*{}'.format(component.refs, qty, component.fields.get('manf#')))
 
     if isinstance(qty, list):
         # Multifiles BOM case, the quantities in the list represent
         # each project read by the order. Do not `CEILING` because
         # this is will be made in the total columns that sum all
         # the quantities needed in all projects BOMs.
         string = ['={{}}*({qp})'.format(qp=i) for i in qty]
@@ -616,15 +617,15 @@
             part = strings[0].strip() + strings[1].strip()
         if qty == '':
             qty = '1'
     else:
         qty = '1'
         part = ''.join(strings)
     part = re.sub(ESC_FIND, r'\1', part)  # Remove any escape backslashes preceding PART_SEPRTR.
-    eda_class.logger.log(DEBUG_OBSESSIVE, 'part/qty>> {}\t\tpart>>{}\tqty>>{}'.format(subpart, part, qty))
+    debug_obsessive('part/qty>> {}\t\tpart>>{}\tqty>>{}'.format(subpart, part, qty))
     return qty, part
 
 
 def get_refnum(refnum):
     if not refnum:
         return 0
     return int(re.match(r'\d+', refnum).group(0))
```

### Comparing `kicost-1.1.6/kicost/global_vars.py` & `kicost-1.1.8/kicost/global_vars.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,32 +20,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 """Stuff that everybody else needs to know about."""
 
-import logging
-
 PLATFORM_WINDOWS_STARTS_WITH = 'win32'
 PLATFORM_LINUX_STARTS_WITH = 'linux'
 PLATFORM_MACOS_STARTS_WITH = 'darwin'
 
-# The root logger of the application. This has to be the root logger to catch
-# output from libraries (e.g. requests) as well.
-logger = None
-
-DEBUG_OVERVIEW = logging.DEBUG
-DEBUG_DETAILED = logging.DEBUG-1
-DEBUG_OBSESSIVE = logging.DEBUG-2
-DEBUG_HTTP_HEADERS = logging.DEBUG-3
-DEBUG_HTTP_RESPONSES = logging.DEBUG-4
-DEBUG_FULL = logging.DEBUG-9
-# Minimum possible log level is logging.DEBUG-9 !
-
 SEPRTR = ':'  # Delimiter between library:component, distributor:field, etc.
 
 # Default language used by GUI and spreadsheet generation and number presentation.
 DEFAULT_LANGUAGE = 'en_US'
 DEFAULT_CURRENCY = 'USD'  # Default currency assigned.
 
 # Default maximum column width for the cell adjust
@@ -57,15 +43,15 @@
 ERR_KICADCONFIG = 3  # An error related to KiCad configuration
 ERR_KICOSTCONFIG = 4  # An error related to KiCost configuration
 ERR_SCRAPE = 5  # Error trying to get prices
 ERR_INPUTFILE = 6  # Error parsing input files
 ERR_FIELDS = 7  # Some inconsistency with the fields
 
 # Warning codes
-W_TRANS = '(WC001) '  # Problem wit field translate
+W_TRANS = '(WC001) '  # Problem with field translate
 W_NOMANP = '(WC002) '  # No manf# or distributor#
 W_CONF = '(WC003) '  # Problem during --un/setup
 W_NOPURCH = '(WC004) '  # No valid field for purchase
 W_NOQTY = '(WC005) '  # No valid qty for purchase
 W_ASSQTY = '(WC006) '  # Assigned qty during scrape
 W_NOINFO = '(WC007) '  # No info during scrape
 NO_PRICE = '(WC008) '  # No price during scrape
@@ -73,19 +59,21 @@
 W_FLDOVR = '(WC010) '  # Field overwrite
 W_DUPWRONG = '(WC011) '  # Inconsistency in duplicated data
 W_INCQTY = '(WC012) '  # Inconsistency in qty
 W_REPMAN = '(WC013) '  # Asking to repeat a manufacturer
 W_MANQTY = '(WC014) '  # Malformed manf#_qty
 W_AMBIPN = '(WC015) '  # Ambiguous mpn, needs better manf
 W_LOCFAIL = '(WC016) '  # Failed to set the locale
+W_APIFAIL = '(WC017) '  # Failed to init an API
+W_CONFIG = '(WC018) '  # Config file warning
+W_CMDLINE = '(WC019) '  # Command line warning
+W_NOAPI = '(WC020) '  # No API with this name
 
-
-class PartHtmlError(Exception):
-    '''Exception for failed retrieval of an HTML parse tree for a part.'''
-    pass
+# Data types for the options common to various APIs
+BASE_OP_TYPES = {'enable': bool, 'cache_ttl': (int, float), 'cache_path': str}
 
 
 class wxPythonNotPresent(Exception):
     '''Exception for failed retrieval of an HTML parse tree for a part.'''
     pass
 
 
@@ -93,14 +81,48 @@
     '''Exception for any error while running kicost().'''
     def __init__(self, msg, id):
         super(self.__class__, self).__init__(msg)
         self.msg = msg
         self.id = id
 
 
-def get_logger():
-    return logger
-
-
-def set_logger(lg):
-    global logger
-    logger = lg
+class DistData(object):
+    '''@brief Data from a distributor related to a part.'''
+    def __init__(self):
+        self.part_num = None  # Distributor catalogue number.
+        self.url = None  # Purchase distributor URL for the spefic part.
+        self.price_tiers = {}  # Price break tiers; [[qty1, price1][qty2, price2]...]
+        self.qty_avail = None  # Available quantity.
+        self.qty_increment = None
+        # self.info_dist = None  # Currently unused.
+        self.currency = None  # Default currency.
+        self.moq = None  # Minimum order quantity allowd by the distributor.
+        self.extra_info = {}
+
+
+# Class for storing part group information.
+class PartGroup(object):
+    '''@brief Class to group components.'''
+    def __init__(self):
+        # None by default, here to avoid try/except in the code
+        self.datasheet = None
+        self.lifecycle = None
+        self.specs = {}  # Miscellaneous data from the queries
+        self.min_price = None  # Filled by the spreadsheet code, expressed in the main currency
+        # Values derived from manf#_qty
+        self.qty = None  # Quantity for each project, just a number if only 1 project
+        self.qty_str = None  # Formulas to compute the quantity in the spreadsheet
+        self.qty_total_spreadsheet = 0  # Total quantity for all projects for the spreadsheet
+        # Distributor data
+        self.dd = {}
+
+    def update_specs(self, specs):
+        for code, inf in specs.items():
+            name, value = inf
+            if code in self.specs:
+                # Already here
+                old_name, old_value = self.specs[code]
+                if name not in old_name:
+                    name = old_name + ', ' + name
+                if old_value is not None and value not in old_value:
+                    value = old_value + ', ' + value
+            self.specs[code] = (name, value)
```

### Comparing `kicost-1.1.6/kicost/kicad_config.py` & `kicost-1.1.8/kicost/kicad_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 import sys
 import re
 
 try:
     import sexpdata  # Try to use a external updated library.
 except ImportError:
     from . import sexpdata  # Use the local file.
-from .global_vars import PLATFORM_MACOS_STARTS_WITH, PLATFORM_WINDOWS_STARTS_WITH, KiCostError, ERR_KICADCONFIG  # Debug, language and default configurations.
+from .global_vars import PLATFORM_MACOS_STARTS_WITH, PLATFORM_WINDOWS_STARTS_WITH, ERR_KICADCONFIG  # Debug, language and default configurations.
+from . import KiCostError
 
 __all__ = ['get_app_config_path',
            'PATH_KICAD_CONFIG', 'PATH_EESCHEMA_CONFIG',
            'bom_plugin_add_entry', 'bom_plugin_remove_entry',
            'fields_add_entry', 'fields_remove_entry']
```

### Comparing `kicost-1.1.6/kicost/kicost.ico` & `kicost-1.1.8/kicost/kicost.ico`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/kicost.py` & `kicost-1.1.8/kicost/kicost.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,46 +41,62 @@
 
 # Libraries.
 import sys
 import os
 import pprint
 from collections import OrderedDict
 from copy import copy
+from math import ceil
 
 # Stops UnicodeDecodeError exceptions.
 try:
     reload(sys)
     sys.setdefaultencoding('utf8')
 except NameError:
     pass  # Happens if reload is attempted in Python 3.
 
 # Only export this routine for use by the outside world.
 __all__ = ['kicost', 'output_filename', 'kicost_gui_notdependences', 'query_part_info']
 
-from .global_vars import (DEFAULT_CURRENCY, DEBUG_OVERVIEW, SEPRTR, DEBUG_DETAILED, DEF_MAX_COLUMN_W, get_logger, ERR_KICOSTCONFIG, ERR_ARGS, KiCostError,
-                          W_TRANS, W_NOMANP)
+from .global_vars import DEFAULT_CURRENCY, SEPRTR, DEF_MAX_COLUMN_W, ERR_KICOSTCONFIG, ERR_ARGS, W_TRANS, W_NOMANP
 # * Import the KiCost libraries functions.
 # Import information for various EDA tools.
-from .edas.tools import field_name_translations, subpartqty_split, group_parts, PRJ_STR_DECLARE, PRJPART_SPRTR
+from .edas.tools import field_name_translations, subpartqty_split, group_parts, PRJ_STR_DECLARE, PRJPART_SPRTR, partgroup_qty
 from .edas import get_part_groups
 # Creation of the final XLSX spreadsheet.
 from .spreadsheet import create_spreadsheet, Spreadsheet
 # Import the scrape API
 from .distributors import get_dist_parts_info, get_registered_apis, get_distributors_iter, get_distributor_info
-
-logger = get_logger()
+from . import debug_detailed, debug_overview, is_debug_detailed, is_debug_overview, error, warning, KiCostError
 
 
 def query_part_info(parts, dist_list, currency=DEFAULT_CURRENCY):
-    if logger.getEffectiveLevel() <= DEBUG_OVERVIEW:
+    """ Used to get the parts price and information.
+        Also used from outside KiCost. """
+    if is_debug_overview():
         api_list = [d.name + ('(Disabled)' if not d.enabled else '') for d in get_registered_apis()]
-        logger.log(DEBUG_OVERVIEW, 'Scrape API list ' + str(api_list))
+        debug_overview('Scrape API list ' + str(api_list))
     get_dist_parts_info(parts, dist_list, currency)
 
 
+def solve_parts_qtys(parts, multi_prj, prj_info):
+    """ Used to fill the qty_str, qty and qty_total_spreadsheet members of the parts.
+        Also used from outside KiCost. """
+    for part in parts:
+        part.qty_str, part.qty = partgroup_qty(part)
+        # Total for all boards
+        if multi_prj:
+            total = 0
+            for i_prj, p_info in enumerate(prj_info):
+                total += part.qty[i_prj] * p_info['qty']
+        else:
+            total = part.qty * prj_info[0]['qty']
+        part.qty_total_spreadsheet = ceil(total)
+
+
 def kicost(in_file, eda_name, out_filename, user_fields, ignore_fields, group_fields, translate_fields, variant, dist_list, collapse_refs=True,
            suppress_cat_url=True, currency=DEFAULT_CURRENCY, max_column_width=DEF_MAX_COLUMN_W, split_extra_fields=[],
            board_qty=[Spreadsheet.DEFAULT_BUILD_QTY]):
     ''' @brief Run KiCost.
 
     Take a schematic input file and create an output file with a cost spreadsheet in xlsx format.
 
@@ -108,32 +124,32 @@
     # re-translate default field names.
     if translate_fields:
         if len(translate_fields) % 2 == 1:
             raise KiCostError('Translation fields argument should have an even number of words.', ERR_ARGS)
         for c in range(0, len(translate_fields), 2):
             # field_name_translations.keys(), field_name_translations.values()
             if translate_fields[c] in field_name_translations.values():
-                logger.warning(W_TRANS+"Unable to re-translate \"{}\" to \"{}\", this is used as an internal field name.".format(
-                               translate_fields[c].lower(), translate_fields[c+1].lower()))
+                warning(W_TRANS, "Unable to re-translate \"{}\" to \"{}\", this is used as an internal field name.".
+                        format(translate_fields[c].lower(), translate_fields[c+1].lower()))
                 continue
             if translate_fields[c+1] != '~':
                 field_name_translations.update({translate_fields[c].lower(): translate_fields[c+1].lower()})
             else:
                 field_name_translations.pop(translate_fields[c].lower(), None)
 
     # Check the integrity of the user personal fields, this should not
     # be any of the reserved fields.
     # This is checked after the translation `dict` is complete, so an
     # before used name field on the translate dictionary can be used
     # user field.
     user_fields = list(OrderedDict([(lv, 1) for lv in user_fields]))  # Avoid repeated fields
     for f in user_fields:
         if f.lower() in field_name_translations:
-            logger.warning(W_TRANS+"\"{f}\" field is a reserved field and can not be used as user field."
-                           " Try to remove it from internal dictionary using `--translate_fields {f} ~`".format(f=f.lower()))
+            warning(W_TRANS, "\"{f}\" field is a reserved field and can not be used as user field."
+                    " Try to remove it from internal dictionary using `--translate_fields {f} ~`".format(f=f.lower()))
             user_fields.remove(f)
 
     c_files = len(in_file)
     # Deal with some code exception (only one EDA tool or variant
     # informed in the multiple BOM files input).
     # This code is never used when called from __main__
     if not isinstance(in_file, list):
@@ -160,15 +176,15 @@
         if c_files > 1:
             # In the case of multiple BOM files, add the project prefix identifier
             # to each reference/designator. Use the field 'manf#_qty' to set
             # the quantity for each project, creating a `list()` with length
             # of number of BOM files. This vector will be used in the `group_parts()`
             # to create groups with elements of same 'manf#' that came from different
             # projects.
-            logger.log(DEBUG_OVERVIEW, 'Multi BOMs detected, attaching project identification to references...')
+            debug_overview('Multi BOMs detected, attaching project identification to references...')
             qty_base = ['0'] * c_files  # Zero for all projects
             for p_ref, p_fields in p.items():
                 # Copy the qty to the position corresponding to this project
                 qty_base[i_prj] = p_fields.get('manf#_qty', '1')
                 p_fields['manf#_qty'] = copy(qty_base)
                 parts[PRJ_STR_DECLARE + str(i_prj) + PRJPART_SPRTR + p_ref] = p_fields
         else:
@@ -209,47 +225,57 @@
     all_fields = set()
     for p in parts:
         all_fields.update(p.fields)
     if 'manf#' not in all_fields:
         new_list = []
         for d in dist_list:
             if d+'#' not in all_fields:
-                logger.warning(W_NOMANP+"No 'manf#' and '%s#' field in any part: no information by '%s'.",
-                               d, get_distributor_info(d).label.name)
+                warning(W_NOMANP, "No 'manf#' and '{}#' field in any part: no information by '{}'.".
+                        format(d, get_distributor_info(d).label.name))
             else:
                 new_list.append(d)
         dist_list = new_list
     # Debug the resulting list
-    if logger.isEnabledFor(DEBUG_DETAILED):
-        logger.log(DEBUG_DETAILED, 'Distributors: ' + pprint.pformat(dist_list))
-    # Get the distributor pricing/qty/etc for each part.
+    if is_debug_detailed():
+        debug_detailed('Distributors: ' + pprint.pformat(dist_list))
+    #
+    # Solve the quantity for each group
+    #
+    # Make sure we have the number of boards for each project
+    for p_info in prj_info:
+        if 'qty' not in p_info:
+            p_info['qty'] = Spreadsheet.DEFAULT_BUILD_QTY
+    multi_prj = len(prj_info) > 1
+    # Compute the qtys
+    solve_parts_qtys(parts, multi_prj, prj_info)
+    # Get the distributor pricing/etc for each part.
     query_part_info(parts, dist_list, currency)
 
     # Create the part pricing spreadsheet.
     create_spreadsheet(parts, prj_info, out_filename, dist_list, currency, collapse_refs, suppress_cat_url,
                        user_fields, '-'.join(variant) if len(variant) > 1 else variant[0], max_column_width)
 
     # Print component groups for debugging purposes.
-    if logger.isEnabledFor(DEBUG_DETAILED):
+    if is_debug_detailed():
         for part in parts:
             for f in dir(part):
                 if f.startswith('__'):
                     continue
                 elif f.startswith('html_trees'):
                     continue
                 else:
                     head = '{} = '.format(f)
                     try:
-                        logger.log(DEBUG_DETAILED, head + pprint.pformat(part.__dict__[f]))
+                        debug_detailed(head + pprint.pformat(part.__dict__[f]))
                     except TypeError:
                         # Python 2.7 pprint has some problem ordering None and strings.
-                        logger.log(DEBUG_DETAILED, head + str(part.__dict__[f]))
+                        debug_detailed(head + str(part.__dict__[f]))
                     except KeyError:
                         pass
-            logger.log(DEBUG_DETAILED, '')
+            debug_detailed('')
 
 
 # Maximum length of the name of the spreadsheet output generate, this is used in the multifiles to limit the
 # automatic name generation.
 FILE_OUTPUT_MAX_NAME = 10
 # Minimum length of characters to use of the input files to create the name of the spreadsheet output file.
 # This is used in the multifile BoM and have prioritize in the `FILE_OUTPUT_MAX_NAME` definition.
@@ -286,14 +312,14 @@
     _end = max(int(FILE_OUTPUT_MAX_NAME/len(files_input)), FILE_OUTPUT_MIN_INPUT-len(FILE_OUTPUT_INPUT_SEP))
     file_name = FILE_OUTPUT_INPUT_SEP.join([os.path.splitext(os.path.basename(input_name))[0][:_end] for input_name in files_input])
     file_output = os.path.join(dir_output, file_name + '.xlsx')
     return file_output
 
 
 def kicost_gui_notdependences():
-    logger.error('You don\'t have the wxPython dependence to run the GUI interface.')
-    logger.error('Run once of the following commands in a terminal to install it:')
-    logger.error('pip3 install -U wxPython # For Windows & macOS')
-    logger.error('sudo apt-get install python3-wxgtk4.0 # Modern Linux derived from Debian, like Ubuntu')
-    logger.error('pip install -U -f https://extras.wxpython.org/wxPython4/extras/linux/gtk3/ubuntu-16.04 wxPython # For Linux 16.04')
-    logger.error('Or download the last version from <https://wxpython.org/pages/downloads/>')
+    error('You don\'t have the wxPython dependence to run the GUI interface.')
+    error('Run once of the following commands in a terminal to install it:')
+    error('pip3 install -U wxPython # For Windows & macOS')
+    error('sudo apt-get install python3-wxgtk4.0 # Modern Linux derived from Debian, like Ubuntu')
+    error('pip install -U -f https://extras.wxpython.org/wxPython4/extras/linux/gtk3/ubuntu-16.04 wxPython # For Linux 16.04')
+    error('Or download the last version from <https://wxpython.org/pages/downloads/>')
     sys.exit(ERR_KICOSTCONFIG)
```

### Comparing `kicost-1.1.6/kicost/kicost_config.py` & `kicost-1.1.8/kicost/kicost_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 # This script aims to be a post installation configuration script, setting
 # shortcuts, plugins, ...
 
 
 # Python libraries.
 import os
 import sys
-from .global_vars import (PLATFORM_WINDOWS_STARTS_WITH, PLATFORM_MACOS_STARTS_WITH, PLATFORM_LINUX_STARTS_WITH, get_logger, KiCostError, ERR_KICADCONFIG,
+from .global_vars import (PLATFORM_WINDOWS_STARTS_WITH, PLATFORM_MACOS_STARTS_WITH, PLATFORM_LINUX_STARTS_WITH, ERR_KICADCONFIG,
                           ERR_KICOSTCONFIG, W_CONF)
 from .kicad_config import get_app_config_path, bom_plugin_add_entry, bom_plugin_remove_entry, fields_add_entry, fields_remove_entry
+from . import info, error, warning, KiCostError
 if sys.platform.startswith(PLATFORM_WINDOWS_STARTS_WITH):
     from .os_windows import reg_set, reg_del, reg_get
     if sys.version_info < (3, 0):
         import _winreg as winreg
     else:
         import winreg
 
 __all__ = ['kicost_setup', 'kicost_unsetup']
 
-logger = get_logger()
 EESCHEMA_KICOST_FIELDS = ['manf#', 'desc', 'variant']
 WIN_USR_FOLDERS = r'SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders'
 
 ###############################################################################
 # Auxiliary functions.
 ###############################################################################
 
@@ -73,39 +73,39 @@
         have_gui = False
     if have_gui:
         cmd_opt = '--gui'
     else:
         cmd_opt = '-wi'
     icon_path = os.path.join(kicost_path, 'kicost.ico')
     if sys.platform.startswith(PLATFORM_MACOS_STARTS_WITH):  # Mac-OS.
-        logger.warning(W_CONF+'I don\'t know how to create the context menu on OSX')
+        warning(W_CONF, 'I don\'t know how to create the context menu on OSX')
         return False
     elif sys.platform.startswith(PLATFORM_WINDOWS_STARTS_WITH):
         reg_set(r'xmlfile\shell\KiCost\command', None, 'kicost {opt} "%1"'.format(opt=cmd_opt), winreg.HKEY_CLASSES_ROOT)
         reg_set(r'xmlfile\shell\KiCost', 'Icon', icon_path, winreg.HKEY_CLASSES_ROOT)
         reg_set(r'csvfile\shell\KiCost\command', None, 'kicost {opt} "%1"'.format(opt=cmd_opt), winreg.HKEY_CLASSES_ROOT)
         reg_set(r'csvfile\shell\KiCost', 'Icon', icon_path, winreg.HKEY_CLASSES_ROOT)
         return True
     elif sys.platform.startswith(PLATFORM_LINUX_STARTS_WITH):
-        logger.warning(W_CONF+'I don\'t know how to create the context menu on Linux')
+        warning(W_CONF, 'I don\'t know how to create the context menu on Linux')
         return False
 
 
 def delete_os_contex_menu():
     '''Delete the OS context menu to recognized KiCost files (XML/CSV).'''
     if sys.platform.startswith(PLATFORM_MACOS_STARTS_WITH):  # Mac-OS.
-        logger.warning(W_CONF+'I don\'t know how to create the context menu on OSX.')
+        warning(W_CONF, 'I don\'t know how to create the context menu on OSX.')
         return False
     elif sys.platform.startswith(PLATFORM_WINDOWS_STARTS_WITH):
         return (reg_del(r'xmlfile\shell\KiCost\command', winreg.HKEY_CLASSES_ROOT) and
                 reg_del(r'xmlfile\shell\KiCost', winreg.HKEY_CLASSES_ROOT) and
                 reg_del(r'csvfile\shell\KiCost\command', winreg.HKEY_CLASSES_ROOT) and
                 reg_del(r'csvfile\shell\KiCost', winreg.HKEY_CLASSES_ROOT))
     elif sys.platform.startswith(PLATFORM_LINUX_STARTS_WITH):
-        logger.warning(W_CONF+'I don\'t know how to create the context menu on Linux.')
+        warning(W_CONF, 'I don\'t know how to create the context menu on Linux.')
         return False
 
 
 def create_shortcut(target, directory, name, icon, location=None,
                     description='', category='', terminal='false'):
     '''Generic routine to create shortcuts.'''
     if not location:
@@ -134,15 +134,15 @@
         with open(path, 'w') as shortcut:
             shortcut.write(content)
             shortcut.close()
         import stat
         os.chmod(path, stat.S_IREAD | stat.S_IWRITE | stat.S_IEXEC)
         return True
     else:
-        logger.warning(W_CONF+'Unrecognized OS.\nShortcut not created!')
+        warning(W_CONF, 'Unrecognized OS.\nShortcut not created!')
         return False
     return
 
 
 ###############################################################################
 # Main functions.
 ###############################################################################
@@ -169,27 +169,27 @@
     # Check if KiCost really exist.
     kicost_path = get_kicost_path()
     kicost_file_path = os.path.join(kicost_path, 'kicost.py')
     # Check if KiCad is installed.
     kicad_config_path = get_app_config_path('kicad')
     if not os.path.isdir(kicad_config_path):
         raise KiCostError('KiCad configuration folder not found.', ERR_KICADCONFIG)
-    logger.info('KiCost identified at \'{}\', proceeding with it configuration in file \'{}\'...'.format(kicost_path, kicad_config_path))
+    info('KiCost identified at \'{}\', proceeding with it configuration in file \'{}\'...'.format(kicost_path, kicad_config_path))
     # Check if wxPython is present.
     try:
         import wx  # wxWidgets for Python.
-        logger.info('GUI requirements (wxPython) identified.')
+        info('GUI requirements (wxPython) identified.')
         have_gui = True
     except ImportError:
         from .kicost import kicost_gui_notdependences
         kicost_gui_notdependences
         have_gui = False
     except Exception as e:
         # TODO: Really?! What can drive us here?
-        logger.error(e)
+        error(e)
         have_gui = False
         pass
 
     if not have_gui:
         MESSAGE = 'Do want to install the GUI requirement packages? (Y/n)\n'
         if sys.version_info >= (3, 0):
             ans = input(MESSAGE)
@@ -200,124 +200,124 @@
                 from pip import main as pipmain
             except ImportError:
                 from pip._internal import main as pipmain
             pipmain(['install', 'wxpython'])
             have_gui = True  # now the Graphical User Interface is installed.
 
     if have_gui:
-        logger.info('Creating app shortcuts...')
+        info('Creating app shortcuts...')
         if sys.platform.startswith(PLATFORM_MACOS_STARTS_WITH):  # Mac-OS.
-            logger.warning(W_CONF+'I don\'t know the desktop folder of mac-OS.')
+            warning(W_CONF, 'I don\'t know the desktop folder of mac-OS.')
             shotcut_directories = []
         elif sys.platform.startswith(PLATFORM_WINDOWS_STARTS_WITH):
             shotcut_directories = [os.path.normpath(reg_get(WIN_USR_FOLDERS, 'Desktop'))]
         elif sys.platform.startswith(PLATFORM_LINUX_STARTS_WITH):
             shotcut_directories = [os.path.expanduser(os.path.join("~", "Desktop"))]
         else:
-            logger.warning(W_CONF+'Not recognized OS.\nShortcut not created!')
+            warning(W_CONF, 'Not recognized OS.\nShortcut not created!')
         for shotcut_directory in shotcut_directories:
             if not create_shortcut('kicost', shotcut_directory,
                                    'KiCost', os.path.join(kicost_path, 'kicost.ico'), '',
                                    'Generate a Cost Bill of Material for EDA softwares', 'BOM'):
-                logger.warning(W_CONF+'Failed to create the KiCost shortcut!')
+                warning(W_CONF, 'Failed to create the KiCost shortcut!')
                 break
-        logger.info('Check your desktop for the KiCost shortcut.')
+        info('Check your desktop for the KiCost shortcut.')
 
-    logger.info('Creating OS context integration...')
+    info('Creating OS context integration...')
     if create_os_contex_menu(kicost_path):
-        logger.info('KiCost listed at the OS context menu for the associated files.')
+        info('KiCost listed at the OS context menu for the associated files.')
     else:
-        logger.warning(W_CONF+'Failed to create KiCost OS context menu integration.')
+        warning(W_CONF, 'Failed to create KiCost OS context menu integration.')
 
     if have_gui:
-        logger.info('Setting the GUI to display the NEWS message...')
+        info('Setting the GUI to display the NEWS message...')
         try:
             from .kicost_gui import CONFIG_FILE, GUI_NEWS_MESSAGE_ENTRY
             configHandle = wx.Config(CONFIG_FILE)
             configHandle.Write(GUI_NEWS_MESSAGE_ENTRY, 'True')
-            logger.info('The user interface will display the NEWS message on first startup.')
+            info('The user interface will display the NEWS message on first startup.')
         except Exception:
-            logger.warning(W_CONF+'Failed to set to display the news message on GUI.')
+            warning(W_CONF, 'Failed to set to display the news message on GUI.')
 
-    logger.info('Creating KiCad integration...')
+    info('Creating KiCad integration...')
     if not os.path.isfile(os.path.join(kicad_config_path, 'eeschema')):
-        logger.error('###  ---> Eeschema was never started. start it and after run `kicost --setup` to configure.')
+        error('###  ---> Eeschema was never started. start it and after run `kicost --setup` to configure.')
     else:
         try:
-            logger.info('Adding KiCost to Eeschema plugin list...')
+            info('Adding KiCost to Eeschema plugin list...')
             try:
                 if have_gui:
                     bom_plugin_add_entry(kicost_file_path, 'kicost --gui "%I"', 'KiCost')
                 else:
                     bom_plugin_add_entry(kicost_file_path, 'kicost -qwi "%I"', 'KiCost')
-                logger.info('KiCost added to KiCad plugin list.')
+                info('KiCost added to KiCad plugin list.')
             except Exception:
-                logger.warning(W_CONF+'Fail to add KiCost to Eeschema plugin list.')
-            logger.info('Adding the KiCost fields to Eeschema template...')
+                warning(W_CONF, 'Fail to add KiCost to Eeschema plugin list.')
+            info('Adding the KiCost fields to Eeschema template...')
             try:
                 fields_add_entry(EESCHEMA_KICOST_FIELDS)
-                logger.info('{} fields added to Eeschema template.'.format(EESCHEMA_KICOST_FIELDS))
+                info('{} fields added to Eeschema template.'.format(EESCHEMA_KICOST_FIELDS))
             except Exception:
-                logger.warning(W_CONF+'Failed to add {} to Eeschema fields template.'.format(EESCHEMA_KICOST_FIELDS))
+                warning(W_CONF, 'Failed to add {} to Eeschema fields template.'.format(EESCHEMA_KICOST_FIELDS))
         except Exception:
-            logger.warning(W_CONF+'Fail to create KiCad-KiCost integration.')
+            warning(W_CONF, 'Fail to create KiCad-KiCost integration.')
 
-    logger.info('KiCost setup configuration finished.')
+    info('KiCost setup configuration finished.')
     return
 
 
 def kicost_unsetup():
     '''Create all the configuration used by KiCost.'''
 
-    logger.info('Removing BOM plugin entry from Eeschema configuration...')
+    info('Removing BOM plugin entry from Eeschema configuration...')
     try:
         bom_plugin_remove_entry('KiCost')
-        logger.info('BOM plugin entry removed from Eeschema configuration.')
+        info('BOM plugin entry removed from Eeschema configuration.')
     except Exception:
-        logger.warning(W_CONF+'Error to remove KiCost from Eeschema plugin list.')
+        warning(W_CONF, 'Error to remove KiCost from Eeschema plugin list.')
 
-    logger.info('Removing KiCost fields to Eeschema template...')
+    info('Removing KiCost fields to Eeschema template...')
     try:
         fields_remove_entry(EESCHEMA_KICOST_FIELDS)
-        logger.info('{} fields removed to Eeschema template.'.format(EESCHEMA_KICOST_FIELDS))
+        info('{} fields removed to Eeschema template.'.format(EESCHEMA_KICOST_FIELDS))
     except Exception:
-        logger.warning(W_CONF+'Error to remove {} to Eeschema fields template.'.format(EESCHEMA_KICOST_FIELDS))
+        warning(W_CONF, 'Error to remove {} to Eeschema fields template.'.format(EESCHEMA_KICOST_FIELDS))
 
-    logger.info('Deleting KiCost shortcuts...')
+    info('Deleting KiCost shortcuts...')
     if sys.platform.startswith(PLATFORM_MACOS_STARTS_WITH):  # Mac-OS.
-        logger.warning(W_CONF+'I don\'t kwon the desktop folder of mac-OS.')
+        warning(W_CONF, 'I don\'t kwon the desktop folder of mac-OS.')
         kicost_shortcuts = []
     elif sys.platform.startswith(PLATFORM_WINDOWS_STARTS_WITH):
         kicost_shortcuts = [os.path.normpath(reg_get(WIN_USR_FOLDERS, 'Desktop'))]
         kicost_shortcuts = [os.path.join(sc, 'KiCost.lnk') for sc in kicost_shortcuts]
     elif sys.platform.startswith(PLATFORM_LINUX_STARTS_WITH):
         kicost_shortcuts = [os.path.expanduser(os.path.join('~', 'Desktop'))]
         for count in range(len(kicost_shortcuts)):
             kicost_shortcuts[count] = os.path.join(kicost_shortcuts[count], 'KiCost.desktop')
     else:
-        logger.warning(W_CONF+'Unrecognized OS.\nShortcut not created!')
+        warning(W_CONF, 'Unrecognized OS.\nShortcut not created!')
     try:
         for kicost_shortcut in kicost_shortcuts:
             kicost_shortcut = os.path.expandvars(kicost_shortcut)
             try:
                 os.remove(kicost_shortcut)
             except OSError:
                 pass
     except Exception:
-        logger.warning(W_CONF+'Fail to remove kiCost shortcuts.')
-    logger.info('KiCost shortcuts deleted.')
+        warning(W_CONF, 'Fail to remove kiCost shortcuts.')
+    info('KiCost shortcuts deleted.')
 
-    logger.info('Removing KiCost from the \'Open with...\' OS context menu...')
+    info('Removing KiCost from the \'Open with...\' OS context menu...')
     try:
         delete_os_contex_menu()
-        logger.info('KiCost removed from the \'Open with...\' OS context menu.')
+        info('KiCost removed from the \'Open with...\' OS context menu.')
     except Exception:
-        logger.warning(W_CONF+'Fail to remove kiCost from OS context menu.')
+        warning(W_CONF, 'Fail to remove kiCost from OS context menu.')
 
-    logger.info('KiCost setup configuration finished.')
+    info('KiCost setup configuration finished.')
     return
 
 
 ###############################################################################
 # Main entrypoint.
 ###############################################################################
 if __name__ == '__main__':
```

### Comparing `kicost-1.1.6/kicost/kicost_gui.py` & `kicost-1.1.8/kicost/kicost_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 # Author information.
 __author__ = 'Hildo Guillardi Júnior'
 __webpage__ = 'https://github.com/hildogjr/'
 __company__ = 'University of Campinas - Brazil'
 
 from .global_vars import (wxPythonNotPresent, PLATFORM_MACOS_STARTS_WITH, PLATFORM_LINUX_STARTS_WITH, PLATFORM_WINDOWS_STARTS_WITH,
-                          DEBUG_OVERVIEW, DEBUG_OBSESSIVE, get_logger, KiCostError, W_LOCFAIL)
+                          W_LOCFAIL)
+from . import KiCostError
 
 # Libraries.
 try:
     import wx  # wxWidgets for Python.
     wx_old = int(wx.__version__[0]) <= 3
 except ImportError:
     raise wxPythonNotPresent()
@@ -48,15 +49,16 @@
 from traceback import format_tb
 import re  # Regular expression parser.
 import locale
 from .currency_converter import list_currencies, get_currency_symbol, get_currency_name
 import requests
 
 # KiCost libraries.
-from . import __version__  # Version control by @xesscorp and collaborator.
+from . import (__version__, info, error, warning, debug_overview, debug_general, get_logger, is_debug_obsessive, is_debug_overview,
+               debug_obsessive)  # Version control by @xesscorp and collaborator.
 from .kicost import kicost, output_filename  # kicost core functions.
 from .distributors import init_distributor_dict, get_distributors_iter, get_distributor_info, get_dist_name_from_label, set_distributors_progress
 from .edas import file_eda_match, get_registered_eda_names, get_eda_label, get_registered_eda_labels
 from .log import CustomFormatter
 py_2 = sys.version_info < (3, 0)
 if sys.platform.startswith("win32"):
     from .os_windows import reg_enum_keys, reg_get
@@ -92,16 +94,14 @@
 PAGE_UPDATE = 'https://pypi.python.org/pypi/kicost'  # Page with the last official version.
 # https://github.com/hildogjr/KiCost/blob/master/kicost/version.py
 PAGE_DEV = 'https://github.com/hildogjr/KiCost/issues/'
 PAGE_POWERED_BY = 'https://kitspace.org/'
 
 kicostPath = os.path.dirname(os.path.abspath(__file__))  # Application dir.
 
-logger = get_logger()
-
 
 # ======================================================================
 class ResultEvent(wx.PyEvent):
     """Simple event to carry arbitrary result data."""
     def __init__(self, id, data=None):
         """Init Result Event."""
         wx.PyEvent.__init__(self)
@@ -122,62 +122,62 @@
         self.start()
 
     def run(self):
         """ Run KiCost and post stuff, but don't touch the GUI in a direct way """
         args = self.args
         # Run KiCost main function and print in the log the elapsed time.
         start_time = time.time()
-        logger.info('Starting cost processing ...')
+        info('Starting cost processing ...')
         try:
-            if logger.isEnabledFor(DEBUG_OBSESSIVE):
-                logger.debug('Arguments for kicost: ' + str(args.__dict__))
+            if is_debug_obsessive():
+                debug_general('Arguments for kicost: ' + str(args.__dict__))
             kicost(in_file=args.input, eda_name=args.eda_name,
                    out_filename=args.output, collapse_refs=args.collapse_refs,
                    user_fields=args.fields, ignore_fields=args.ignore_fields,
                    group_fields=args.group_fields, translate_fields=args.translate_fields,
                    variant=args.variant,
                    dist_list=args.include, currency=args.currency)
         except KiCostError as e:
-            logger.error(e)
+            error(e)
             # We are done, notify the main thread
             wx.PostEvent(self.wxObject, ResultEvent(self.event_id))
             return
         except Exception as e:
-            if logger.isEnabledFor(DEBUG_OVERVIEW):
+            if is_debug_overview():
                 # Inform a traceback
                 (type, value, traceback) = sys.exc_info()
                 trace = format_tb(traceback)
                 for line in trace:
-                    logger.info(line[:-1])
-            logger.error('Internal error: ' + str(e))
+                    info(line[:-1])
+            error('Internal error: ' + str(e))
             # We are done, notify the main thread
             wx.PostEvent(self.wxObject, ResultEvent(self.event_id))
             return
         finally:
             init_distributor_dict()  # Restore distributors modified during the execution of KiCost motor.
-        logger.log(DEBUG_OVERVIEW, 'Elapsed time: {} seconds'.format(time.time() - start_time))
-        logger.info('Finished cost processing.')
+        debug_overview('Elapsed time: {} seconds'.format(time.time() - start_time))
+        info('Finished cost processing.')
         # Convert to ODS
         try:
             if args.convert_to_ods:
-                logger.log(DEBUG_OVERVIEW, 'Converting \'{}\' to ODS file...'.format(os.path.basename(args.output)))
+                debug_overview('Converting \'{}\' to ODS file...'.format(os.path.basename(args.output)))
                 subprocess.run((libreoffice_executable, '--headless', '--convert-to', 'ods', args.output,
                                 '--outdir', os.path.dirname(args.output)), check=True)
                 # os.remove(args.output)  # Delete the older file.
                 args.output = os.path.splitext(args.output)[0] + '.ods'
         except subprocess.CalledProcessError as e:
-            logger.log(DEBUG_OVERVIEW, '\'{}\' could be not converted to ODS: {}'.format(os.path.basename(args.output), e))
+            debug_overview('\'{}\' could be not converted to ODS: {}'.format(os.path.basename(args.output), e))
             pass
         # Open the spreadsheet
         try:
             if args.open_spreadsheet:
-                logger.log(DEBUG_OVERVIEW, 'Opening the output file \'{}\'...'.format(os.path.basename(args.output)))
+                debug_overview('Opening the output file \'{}\'...'.format(os.path.basename(args.output)))
                 open_file(args.output)
         except Exception as e:
-            logger.log(DEBUG_OVERVIEW, '\'{}\' could be not opened: {}'.format(os.path.basename(args.output), e))
+            debug_overview('\'{}\' could be not opened: {}'.format(os.path.basename(args.output), e))
         # We are done, notify the main thread
         wx.PostEvent(self.wxObject, ResultEvent(self.event_id))
 
 
 # ======================================================================
 def open_file(filepath):
     '''@brief Open a file with the default application in different OSs.
@@ -186,15 +186,15 @@
     if sys.platform.startswith(PLATFORM_MACOS_STARTS_WITH):  # Mac-OS.
         subprocess.call(('open', filepath))
     elif sys.platform.startswith(PLATFORM_WINDOWS_STARTS_WITH):  # Windows.
         os.startfile(filepath)
     elif sys.platform.startswith(PLATFORM_LINUX_STARTS_WITH):  # Linux.
         subprocess.call(('xdg-open', filepath))
     else:
-        logger.info('Not recognized OS. The spreadsheet file will not be automatically opened.')
+        info('Not recognized OS. The spreadsheet file will not be automatically opened.')
 
 
 # ======================================================================
 class FileDropTarget(wx.FileDropTarget):
     ''' This object implements Drop Target functionality for Files.
         @param Window handle.
     '''
@@ -414,31 +414,31 @@
         bSizer6.Add(self.m_checkBox_XLSXtoODS, 0, wx.ALL, 5)
         # LibreOffice identification
         global libreoffice_executable
         if sys.platform.startswith("win32"):
             libreoffice_reg = r'SOFTWARE\LibreOffice\LibreOffice'
             libreoffice_installations = reg_enum_keys(libreoffice_reg, HKEY_LOCAL_MACHINE)
             if libreoffice_installations:
-                logger.log(DEBUG_OVERVIEW, 'Found LibreOffice {} installation(s) version(s).'.format(libreoffice_installations))
+                debug_overview('Found LibreOffice {} installation(s) version(s).'.format(libreoffice_installations))
                 libreoffice_installations.sort(key=StrictVersion)
                 # TODO: os.path.join(os.path.join?
                 libreoffice_executable = reg_get(os.path.join(libreoffice_reg, os.path.join(libreoffice_reg, libreoffice_installations[-1]), 'Path'),
                                                  HKEY_LOCAL_MACHINE)
-                logger.log(DEBUG_OVERVIEW, 'Last LibreOffice installation at {}.'.format(libreoffice_executable))
+                debug_overview('Last LibreOffice installation at {}.'.format(libreoffice_executable))
             else:
-                logger.log(DEBUG_OVERVIEW, 'LibreOffice not found.')
+                debug_overview('LibreOffice not found.')
                 libreoffice_executable = None
         else:
             from distutils.spawn import find_executable
             libreoffice_executable = find_executable('libreoffice')
         # Create a control to convert the XLSX to ODS quietly.
         if libreoffice_executable:
             self.m_checkBox_XLSXtoODS.Enable()  # Recognized LibreOffice.
         else:
-            logger.log(DEBUG_OBSESSIVE, 'LibreOffice not found.')
+            debug_obsessive('LibreOffice not found.')
             self.m_checkBox_XLSXtoODS.SetValue(False)
 
         self.m_checkBox_openSpreadsheet = wx.CheckBox(self.m_panel1, wx.ID_ANY, u"Open spreadsheet", wx.DefaultPosition, wx.DefaultSize, 0)
         self.m_checkBox_openSpreadsheet.SetValue(True)
         self.m_checkBox_openSpreadsheet.SetToolTip(wx.ToolTip(u"Open the spreadsheet after finish the KiCost scrape."))
         bSizer6.Add(self.m_checkBox_openSpreadsheet, 0, wx.ALL, 5)
 
@@ -633,15 +633,15 @@
 
         # Set the application windows title and configurations.
         self.SetTitle('KiCost v' + __version__)
         self.SetIcon(wx.Icon(os.path.join(kicostPath, 'kicost.ico'), wx.BITMAP_TYPE_ICO))
 
         self.set_properties()
         self.SetDropTarget(FileDropTarget(self))  # Start the drop file in all the window.
-        logger.log(DEBUG_OVERVIEW, 'Loaded KiCost v' + __version__)
+        debug_overview('Loaded KiCost v' + __version__)
 
         # Set up event handler for any worker thread results
         # It will receive notifications from the KiCost thread
         self.event_id = wx.NewId() if wx_old else wx.NewIdRef().GetId()
         self.Connect(-1, -1, self.event_id, self.update_kicost_run)
 
     def __del__(self):
@@ -827,30 +827,30 @@
         class argments:
             pass
         args = argments()
 
         args.input = re.split(SEP_FILES, self.m_comboBox_files.GetValue())
         for f in args.input:
             if not os.path.isfile(f):
-                logger.info('No valid file(s) selected.')
+                info('No valid file(s) selected.')
                 self.m_button_run.Enable()
                 return  # Not a valid file(s).
 
         spreadsheet_file = self.m_text_saveas.GetValue()
         # Handle case where output is going into an existing spreadsheet file.
         if os.path.isfile(spreadsheet_file):
             if not self.m_checkBox_overwrite.GetValue():
                 dlg = wx.MessageDialog(self, "The file output \'{}\' already exit, do you want overwrite?"
                                        .format(os.path.basename(spreadsheet_file)),
                                        "Confirm Overwrite",
                                        wx.YES_NO | wx.YES_DEFAULT | wx.ICON_QUESTION | wx.STAY_ON_TOP | wx.CENTER)
                 result = dlg.ShowModal()
                 dlg.Destroy()
                 if result == wx.ID_NO:
-                    logger.info('Not able to overwrite \'{}\'...'.format(os.path.basename(spreadsheet_file)))
+                    info('Not able to overwrite \'{}\'...'.format(os.path.basename(spreadsheet_file)))
                     return
         spreadsheet_file = os.path.splitext(spreadsheet_file)[0] + '.xlsx'  # Force the output (for the CLI interface) to be .XLSX.
         args.output = spreadsheet_file
 
         if self.m_textCtrl_extraCmd.GetValue():
             extra_commands = ' ' + self.m_textCtrl_extraCmd.GetValue()
         else:
@@ -1041,15 +1041,15 @@
                     # elif isinstance(wxElement_handle, wx._core.Button):
                     # elif isinstance(wxElement_handle, wx._core.StaticText):
                 except KeyError:
                     continue
 
             del configHandle  # Close the file / Windows registry sock.
         except Exception as e:
-            logger.log(DEBUG_OVERVIEW, 'Configurations not recovered: <'+str(e)+'>.')
+            debug_overview('Configurations not recovered: <'+str(e)+'>.')
 
     # ----------------------------------------------------------------------
     def save_properties(self):
         ''' @brief Save the current proprieties of the graphical elements.'''
         try:
             configHandle = wx.Config(CONFIG_FILE)
 
@@ -1091,15 +1091,15 @@
                     # elif isinstance(wxElement_handle, wx._core.Button):
                     # elif isinstance(wxElement_handle, wx._core.StaticText):
                 except KeyError:
                     continue
 
             del configHandle  # Close the file / Windows registry sock.
         except Exception as e:
-            logger.log(DEBUG_OVERVIEW, 'Configurations not saved: <'+str(e)+'>.')
+            debug_overview('Configurations not saved: <'+str(e)+'>.')
 
     def show_news_message(self):
         '''Shows a message bos if the news of the last version installed.'''
         history_file = open(os.path.join(kicostPath, 'HISTORY.rst'))
         history = history_file.read()
         history_file.close()
         search_news = re.compile(r'History\s+[\=\-\_]+\s+(?P<version>[\w\.]+)\s*\((?P<data>.+)\)\s+[\=\-\_]+\s+(?P<news>(?:\n|.)*?)\s+[\d\.]+', re.IGNORECASE)
@@ -1167,33 +1167,33 @@
         @param String file file names or list.
         (it will be used for plugin implementation on future KiCad6-Eeschema).
     '''
     app = wx.App(redirect=False)
     loc = wx.Locale(wx.LANGUAGE_DEFAULT if not force_en_us else wx.LANGUAGE_ENGLISH_US)
     if not loc.IsOk():
         if not force_en_us:
-            logger.warning(W_LOCFAIL+"Failed to set the default locale, try using `--force_en_us`")
+            warning(W_LOCFAIL, "Failed to set the default locale, try using `--force_en_us`")
         else:
-            logger.warning(W_LOCFAIL+"`--force_en_us` doesn't seem to help")
+            warning(W_LOCFAIL, "`--force_en_us` doesn't seem to help")
     elif not loc.GetLocale() and not loc.GetName():
-        logger.warning(W_LOCFAIL+"Unsupported locale"+(", try using `--force_en_us`" if not force_en_us else ""))
+        warning(W_LOCFAIL, "Unsupported locale"+(", try using `--force_en_us`" if not force_en_us else ""))
     else:
         try:
             sys_loc_name = locale.getlocale()
         except ValueError:
-            logger.warning(W_LOCFAIL+"Unsupported locale (python)"+(", try using `--force_en_us`" if not force_en_us else ""))
+            warning(W_LOCFAIL, "Unsupported locale (python)"+(", try using `--force_en_us`" if not force_en_us else ""))
             sys_loc_name = 'unsupported'
-        logger.debug('wxWidgets locale {} ({}) system: {}'.format(loc.GetLocale(), loc.GetName(), sys_loc_name))
+        debug_general('wxWidgets locale {} ({}) system: {}'.format(loc.GetLocale(), loc.GetName(), sys_loc_name))
     frame = formKiCost(None)
     # Use the GUI for progress
     set_distributors_progress(ProgressGUI)
     ProgressGUI.frame = frame
     # Redirect the logging system to the GUI area
     logger_stream = GUI_Stream(frame.m_textCtrl_messages)
-    for handler in logger.handlers:
+    for handler in get_logger().handlers:
         if py_2:
             handler.stream = logger_stream
         else:
             handler.setStream(logger_stream)
         # Reset the formatter so it realizes that we aren't using a terminal
         handler.setFormatter(CustomFormatter(logger_stream))
 
@@ -1203,15 +1203,15 @@
 
     frame.Show()
     app.MainLoop()
 
     # Restore the channel print output to terminal.
     # Necessary if KiCost was called by other software?
     sys.stderr = sys.__stderr__
-    for handler in logger.handlers:
+    for handler in get_logger().handlers:
         if py_2:
             handler.stream = sys.stderr
         else:
             handler.setStream(sys.stderr)
         handler.setFormatter(CustomFormatter(sys.stderr))
```

### Comparing `kicost-1.1.6/kicost/kicost_kicadplugin.py` & `kicost-1.1.8/kicost/kicost_kicadplugin.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/kitspace.png` & `kicost-1.1.8/kicost/kitspace.png`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/log.py` & `kicost-1.1.8/kicost/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 """
 Log module
 
 Handles logging initialization and formating.
 """
+import io
+import os
 import sys
+import traceback
 import logging
 no_colorama = False
 try:
     from colorama import init as colorama_init, Fore, Back, Style
 except ImportError:
     no_colorama = True
 # If colorama isn't installed use an ANSI basic replacement
@@ -116,14 +119,36 @@
     def log_totals(self):
         if MyLogger.warn_cnt:
             filt_msg = ''
             if MyLogger.n_filtered:
                 filt_msg = ', {} filtered'.format(MyLogger.n_filtered)
             self.info('Found {} unique warning/s ({} total{})'.format(MyLogger.warn_cnt, MyLogger.warn_tcnt, filt_msg))
 
+    def findCaller(self, stack_info=False, stacklevel=1):
+        f = sys._getframe(1)
+        # Skip frames from logging module
+        while '/logging/' in os.path.normcase(f.f_code.co_filename):
+            f = f.f_back
+        # Apply the indicated stacklevel
+        while stacklevel > 1:
+            f = f.f_back
+            stacklevel -= 1
+        # Skip the __init__.py wrappers
+        fname = os.path.normcase(f.f_code.co_filename)
+        if fname.endswith('__init__.py') or fname.endswith('log__.py'):
+            f = f.f_back
+        # Create the stack info if needed
+        sinfo = None
+        if stack_info:
+            out = io.StringIO()
+            out.write(u"Stack (most recent call last):\n")
+            traceback.print_stack(f, file=out)
+            sinfo = out.getvalue().rstrip(u"\n")
+        return os.path.normcase(f.f_code.co_filename), f.f_lineno, f.f_code.co_name, sinfo
+
 
 def set_verbosity(logger, debug, quiet):
     # Choose the log level
     if debug is not None:
         log_level = logging.DEBUG + 1 - debug
     elif quiet is True:
         log_level = logging.ERROR
```

### Comparing `kicost-1.1.6/kicost/os_windows.py` & `kicost-1.1.8/kicost/os_windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 __author__ = 'Hildo Guillardi Júnior'
 __webpage__ = 'https://github.com/hildogjr/'
 __company__ = 'University of Campinas - Brazil'
 # This script aims to be a post installation configuration script, setting
 # shortcuts, plugins, ...
 
 import sys
-from .global_vars import get_logger
-logger = get_logger()
+from . import error
 
 if sys.platform.startswith('win32'):
     # Create the functions to deal with Windows registry, from http://stackoverflow.com/a/35286642
     if sys.version_info < (3, 0):
         from _winreg import (OpenKey, HKEY_CURRENT_USER, ConnectRegistry, KEY_READ, KEY_WOW64_64KEY, EnumValue, CloseKey, EnumKey, QueryValueEx, REG_SZ,
                              CreateKey, KEY_WRITE, SetValueEx, DeleteKey)
         OpenKeyError = WindowsError
@@ -119,15 +118,15 @@
                 registry_key = OpenKey(reg, path, 0, KEY_WRITE | KEY_WOW64_64KEY)
             SetValueEx(registry_key, name, 0, key_type, value)
             CloseKey(reg)
             # Update the Windows behaviour.
             # SendMessage(win32con.HWND_BROADCAST, win32con.WM_SETTINGCHANGE, 0, 'Environment')
             return True
         except ConnectRegistryError:
-            logger.error('You should run this command as system administrator: run the terminal as administrator and type the command again.')
+            error('You should run this command as system administrator: run the terminal as administrator and type the command again.')
         except WindowsError:
             pass
         return False
 
     def reg_del(name, key=HKEY_CURRENT_USER):
         # Delete a registry key on Windows.
         try:
@@ -135,11 +134,11 @@
             # registry_key = OpenKey(reg, name_base, 0, KEY_ALL_ACCESS)
             DeleteKey(reg, name)
             CloseKey(reg)
             # Update the Windows behaviour.
             # SendMessage(win32con.HWND_BROADCAST, win32con.WM_SETTINGCHANGE, 0, 'Environment')
             return True
         except ConnectRegistryError:
-            logger.error('You should run this command as system administrator: run the terminal as administrator and type the command again.')
+            error('You should run this command as system administrator: run the terminal as administrator and type the command again.')
         except WindowsError:
             pass
         return False
```

### Comparing `kicost-1.1.6/kicost/sexpdata.py` & `kicost-1.1.8/kicost/sexpdata.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/kicost/spreadsheet.py` & `kicost-1.1.8/kicost/spreadsheet.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,32 +24,30 @@
 
 # Author information.
 __author__ = 'Hildo Guillardi Júnior'
 __webpage__ = 'https://github.com/hildogjr/'
 __company__ = 'University of Campinas - Brazil'
 
 # Debug, language and default configurations.
-from .global_vars import (SEPRTR, DEFAULT_CURRENCY, DEFAULT_LANGUAGE, DEBUG_OVERVIEW, DEBUG_DETAILED, DEF_MAX_COLUMN_W, get_logger, W_NOPURCH, W_NOQTY,
-                          ERR_FIELDS, KiCostError)
+from .global_vars import SEPRTR, DEFAULT_CURRENCY, DEFAULT_LANGUAGE, DEF_MAX_COLUMN_W, W_NOPURCH, W_NOQTY, ERR_FIELDS
 
 # Python libraries.
 import os
 from datetime import datetime
 from math import ceil
 from textwrap import wrap
 import re  # Regular expression parser.
 import xlsxwriter  # XLSX file interpreter.
 from xlsxwriter.utility import xl_rowcol_to_cell, xl_range_abs
 from validators import url as validate_url  # URL validator.
 
 # KiCost libraries.
-from .version import __version__  # Version control by @xesscorp and collaborator.
 from .distributors import get_distributor_info, ORDER_COL_USERFIELDS
-from .edas.tools import partgroup_qty, order_refs, PART_REF_REGEX
-from . import DistData
+from .edas.tools import order_refs, PART_REF_REGEX
+from . import DistData, __version__, warning, debug_overview, debug_detailed, debug_general, KiCostError
 
 from .currency_converter import CurrencyConverter, get_currency_symbol, format_currency
 currency_convert = CurrencyConverter().convert
 
 __all__ = ['create_spreadsheet', 'create_worksheet', 'Spreadsheet']
 
 
@@ -101,16 +99,20 @@
     DATE_FIELD_LABEL = '$ date:'
     # Default value for number of boards to build.
     DEFAULT_BUILD_QTY = 100
     # About and credit message at the end of the spreadsheet.
     ABOUT_MSG = 'KiCost\N{REGISTERED SIGN} v' + __version__
     # Try to group references as ranges
     COLLAPSE_REFS = True
+    # Sort the groups
+    SORT_GROUPS = True
     # Don't add the link column
     SUPPRESS_CAT_URL = True
+    # Don't add the description column
+    SUPPRESS_DIST_DESC = True
     # Columns to add to the global section
     USER_FIELDS = []
     # List of selected distributors
     DISTRIBUTORS = []
     # Sort the distributors alphabetically.
     # But first the web distributors and then the local ones
     SORT_DISTRIBUTORS = True
@@ -279,15 +281,15 @@
         self.worksheet_name = worksheet_name
         self.purchase_description_seprtr = SEPRTR  # Purchase description separator.
         self.prj_info = prj_info
         self.START_ROW = self.PRJ_INFO_START+1+self.PRJ_INFO_ROWS*len(prj_info)
         # Currency format and symbol definition
         self.set_currency(currency)
         # Extra information characteristics of the components gotten in the page that will be displayed as comment in the 'cat#' column.
-        self.extra_info_display = ['value', 'tolerance', 'footprint', 'power', 'current', 'voltage', 'frequency', 'temp_coeff', 'manf', 'size']
+        self.extra_info_display = ['desc', 'value', 'tolerance', 'footprint', 'power', 'current', 'voltage', 'frequency', 'temp_coeff', 'manf', 'size']
         # Create the worksheet that holds the pricing information.
         self.wks = workbook.add_worksheet(worksheet_name)
         # Data to performe cell size adjust
         self.col_widths = {}
         self.row_heights = {}
         self.col_levels = {}
         self.collapsed = set()
@@ -339,20 +341,20 @@
             cur_w = self.col_widths.get(col, Spreadsheet.MIN_COL_WIDTH)
             self.col_widths[col] = min(max(w, cur_w), Spreadsheet.MAX_COL_WIDTH)
         if h > 1:
             cur_h = self.row_heights.get(row, 1)
             if h > cur_h:
                 self.row_heights[row] = h
 
-    def adjust_row_and_col_sizes(self, logger):
+    def adjust_row_and_col_sizes(self):
         """ Adjust the column and row sizes using the values computed by compute_cell_size """
-        logger.log(DEBUG_OVERVIEW, 'Adjusting cell sizes')
-        logger.log(DEBUG_DETAILED, 'Column adjusts: ' + str(self.col_widths))
-        logger.log(DEBUG_DETAILED, 'Row adjusts: ' + str(self.row_heights))
-        logger.log(DEBUG_DETAILED, 'Levels: ' + str(self.col_levels))
+        debug_overview('Adjusting cell sizes')
+        debug_detailed('Column adjusts: ' + str(self.col_widths))
+        debug_detailed('Row adjusts: ' + str(self.row_heights))
+        debug_detailed('Levels: ' + str(self.col_levels))
         for i, width in self.col_widths.items():
             level = self.col_levels.get(i, 0)
             if level:
                 ops = {'level': level}
                 if i in self.collapsed:
                     # Libreoffice 7 workaround: collapsed cols aren't collapsed at start-up
                     ops['hidden'] = 1
@@ -419,19 +421,19 @@
         self.wks.conditional_format(rng, ops)
 
     def conditional_format(self, row, col, criteria, format, value=None):
         self.conditional_format_r(xl_range(row, col, row), criteria, format, value)
 
 
 def create_spreadsheet(parts, prj_info, spreadsheet_filename, dist_list, currency=DEFAULT_CURRENCY,
-                       collapse_refs=True, suppress_cat_url=True, user_fields=[], variant=' ', max_column_width=DEF_MAX_COLUMN_W):
+                       collapse_refs=True, suppress_cat_url=True, user_fields=[], variant=' ',
+                       max_column_width=DEF_MAX_COLUMN_W, suppress_dist_desc=True):
     '''Create a spreadsheet using the info for the parts (including their HTML trees).'''
     basename = os.path.basename(spreadsheet_filename)
-    logger = get_logger()
-    logger.log(DEBUG_OVERVIEW, 'Creating the \'{}\' spreadsheet...'.format(basename))
+    debug_overview('Creating the \'{}\' spreadsheet...'.format(basename))
     # Adjust the name of the work_sheet (add variant and limit len)
     worksheet_name = os.path.splitext(basename)[0]  # Default name for pricing worksheet.
     variant = variant.strip()
     if len(variant) > 0:
         # Append an indication of the variant to the worksheet title.
         # Remove any special characters that might be illegal in a
         # worksheet name since the variant might be a regular expression.
@@ -443,26 +445,27 @@
         worksheet_name += variant
     else:
         worksheet_name = worksheet_name[:Spreadsheet.MAX_LEN_WORKSHEET_NAME]
     # Create spreadsheet file.
     with xlsxwriter.Workbook(spreadsheet_filename) as workbook:
         Spreadsheet.COLLAPSE_REFS = collapse_refs
         Spreadsheet.SUPPRESS_CAT_URL = suppress_cat_url
+        Spreadsheet.SUPPRESS_DIST_DESC = suppress_dist_desc
         Spreadsheet.USER_FIELDS = user_fields
         Spreadsheet.DISTRIBUTORS = dist_list
         if max_column_width:
             Spreadsheet.ADJUST_ROW_AND_COL_SIZE = True
             Spreadsheet.MAX_COL_WIDTH = max_column_width
         else:
             Spreadsheet.ADJUST_ROW_AND_COL_SIZE = False
         ss = Spreadsheet(workbook, worksheet_name, prj_info, currency)
-        create_worksheet(ss, logger, parts)
+        create_worksheet(ss, parts)
 
 
-def create_worksheet(ss, logger, parts):
+def create_worksheet(ss, parts):
     '''Create a worksheet using the info for the parts (including their HTML trees).'''
     # Force all currency related cells to use the "currency_format"
     ss.WRK_FORMATS['total_cost_currency']['num_format'] = ss.currency_format
     ss.WRK_FORMATS['unit_cost_currency']['num_format'] = ss.currency_format
     ss.WRK_FORMATS['currency']['num_format'] = ss.currency_format
     ss.WRK_FORMATS['currency_unit']['num_format'] = ss.currency_format_unit
     # Enable test wrap if we will adjust the sizes
@@ -493,46 +496,43 @@
     LABEL_ROW = START_ROW + 1
     COL_HDR_ROW = LABEL_ROW + 1
     if not ss.SUPPRESS_CAT_URL:
         # Add a extra column for the hyperlink.
         d_width = len(ss.DISTRIBUTOR_COLUMNS)
         ss.DISTRIBUTOR_COLUMNS.update({'link': {'col': d_width, 'level': 2, 'label': 'URL', 'width': 15, 'comment': 'Distributor catalog link (ctrl-click).'}})
         ss.DISTRIBUTOR_COLUMNS['part_num']['comment'] = 'Distributor-assigned catalog number for each part. Extra distributor data is shown as comment.'
+    if not ss.SUPPRESS_DIST_DESC:
+        # Add a extra column for the description.
+        d_width = len(ss.DISTRIBUTOR_COLUMNS)
+        ss.DISTRIBUTOR_COLUMNS.update({'description': {'col': d_width, 'level': 2, 'label': 'Description', 'width': 15, 'comment': 'Distributor description'}})
 
     # Make a list of alphabetically-ordered distributors with web distributors before locals.
-    logger.log(DEBUG_OVERVIEW, 'Sorting the distributors...')
+    debug_overview('Sorting the distributors...')
     if ss.SORT_DISTRIBUTORS:
         web_dists = sorted([d for d in ss.DISTRIBUTORS if get_distributor_info(d).is_web()])
         local_dists = sorted([d for d in ss.DISTRIBUTORS if get_distributor_info(d).is_local()])
         dist_list = web_dists + local_dists
     else:
         dist_list = ss.DISTRIBUTORS
-    # Make sure we have the number of boards for each project
-    for p_info in prj_info:
-        if 'qty' not in p_info:
-            p_info['qty'] = ss.DEFAULT_BUILD_QTY
-    # Compute some values needed for the parts
-    for part in parts:
-        part.qty_str, part.qty = partgroup_qty(part)
 
     # Fill the global information (not distributor-specific)
     # Skip the prices, will fill them after we fill the distributors
     # dist_1st_col = the column immediately to the right of the global data.
     # qty_col = the column where the quantity needed of each part is stored.
-    dist_1st_col, refs_col, qty_col, columns_global = add_globals_to_worksheet(ss, logger, START_ROW, START_COL, TOTAL_COST_ROW, parts, dist_list)
+    dist_1st_col, refs_col, qty_col, columns_global = add_globals_to_worksheet(ss, START_ROW, START_COL, TOTAL_COST_ROW, parts, dist_list)
     ss.globals_width = dist_1st_col - 1
 
     # Fill the distributors information
-    logger.log(DEBUG_OVERVIEW, 'Writing the distributors information...')
+    debug_overview('Writing the distributors information...')
     next_col = dist_1st_col
     for dist in dist_list:
-        next_col = add_dist_to_worksheet(ss, logger, columns_global, START_ROW, next_col, UNIT_COST_ROW, TOTAL_COST_ROW, refs_col, qty_col, dist, parts)
+        next_col = add_dist_to_worksheet(ss, columns_global, START_ROW, next_col, UNIT_COST_ROW, TOTAL_COST_ROW, refs_col, qty_col, dist, parts)
 
     # Fill the global prices
-    next_line = add_global_prices_to_workheet(ss, logger, START_ROW, START_COL, TOTAL_COST_ROW, parts, dist_list, columns_global)
+    next_line = add_global_prices_to_workheet(ss, START_ROW, START_COL, TOTAL_COST_ROW, parts, dist_list, columns_global)
 
     for i_prj, p_info in enumerate(prj_info):
         # Add project information to track the project (in a printed version of the BOM) and the date because of price variations.
         i_prj_str = str(i_prj) if len(prj_info) > 1 else ''
         if ss.INCLUDE_PRJ_INFO:
             wks.write(next_row, START_COL, 'Prj{}:'.format(i_prj_str), ss.wrk_formats['proj_info_field'])
             wks.write(next_row, START_COL+1, p_info['title'], ss.wrk_formats['proj_info'])
@@ -580,30 +580,30 @@
         ss.add_date(next_line+1, START_COL)
         next_line += 1
     # Add the KiCost package information at the end of the spreadsheet to debug
     # information at the forum and "advertising".
     wks.write(next_line+1, START_COL, ss.ABOUT_MSG, ss.wrk_formats['about_msg'])
     # Optionally adjust cell sizes
     if ss.ADJUST_ROW_AND_COL_SIZE:
-        ss.adjust_row_and_col_sizes(logger)
+        ss.adjust_row_and_col_sizes()
 
 
 def get_ref_key(part):
     ''' Helper function to sort the references '''
     match = PART_REF_REGEX.match(part.first_ref)
     if not match:
         return [part.collapsed_refs, 0, 0]
     subpart_num = match.group('subpart_num')
     return [match.group('prefix'), int(match.group('ref_num')), int(subpart_num) if subpart_num else 0]
 
 
-def add_globals_to_worksheet(ss, logger, start_row, start_col, total_cost_row, parts, dist_list):
+def add_globals_to_worksheet(ss, start_row, start_col, total_cost_row, parts, dist_list):
     '''Add global part data to the spreadsheet.'''
 
-    logger.log(DEBUG_OVERVIEW, 'Writing the global information...')
+    debug_overview('Writing the global information...')
 
     wks = ss.wks
     # Columns for the various types of global part data.
     columns = ss.GLOBAL_COLUMNS.copy()
     # Created a list of columns sorted by column position
     columns_list = [None] * len(columns)
     for id, data in columns.items():
@@ -660,15 +660,15 @@
 
     # Add label for global section.
     wks.merge_range(row, start_col, row, start_col + num_cols - 1, "Global Part Info", ss.wrk_formats['global'])
     row += 1  # Go to next row.
 
     # Add column headers.
     # Memorize the columns positions, this `col`
-    logger.debug(columns_list)
+    debug_general(columns_list)
     col = {}
     for c, k in enumerate(columns_list):
         ss.write_string(row, c, columns[k]['label'], 'header')
         wks.write_comment(row, c, columns[k]['comment'])
         ss.set_column(c, columns[k]['width'], columns[k]['level'])
         col[k] = c
     row += 1  # Go to next row.
@@ -677,15 +677,16 @@
     # Order the references and collapse, if asked:
     # e.g. J3, J2, J1, J6 => J1, J2, J3 J6. # `collapse=False`
     # e.g. J3, J2, J1, J6 => J1-J3, J6.. # `collapse=True`
     for part in parts:
         part.collapsed_refs, part.first_ref = order_refs(part.refs, collapse=ss.COLLAPSE_REFS, ref_sep=ss.PART_NSEQ_SEPRTR)
 
     # Then, order the part references with priority ref prefix, ref num, and subpart num.
-    parts.sort(key=get_ref_key)
+    if ss.SORT_GROUPS:
+        parts.sort(key=get_ref_key)
 
     # Add the global part data to the spreadsheet.
     col_qty = start_col + col['qty']
     col_refs = start_col + col['refs']
     for part in parts:
 
         # Enter part references.
@@ -720,51 +721,47 @@
                 # TODO add future dependence of "electro-grammar" (https://github.com/kitspace/electro-grammar)
                 field_value_footprint = re.findall(r'\:(.*)', field_value)
                 if field_value_footprint:
                     field_value = field_value_footprint[0]
             ss.write_string(row, n_col, field_value, cell_format)
 
         # Enter total part quantity needed.
+        total = part.qty_total_spreadsheet
         if num_prj > 1:
             # Multifiles BOM case, write each quantity and after,
             # in the 'qty' column the total quantity as ceil of
             # the total quantity (to ceil use a Microsoft Excel
             # compatible function.
-            total = 0
             for i_prj, p_info in enumerate(ss.prj_info):
                 value = part.qty[i_prj] * p_info['qty']
                 if part.qty[i_prj]:
                     ss.num_parts[i_prj] += 1
-                total += value
                 id = str(i_prj)
                 # Qty.PrjN
                 wks.write_formula(row, start_col + col['qty_prj'+id], part.qty_str[i_prj].format('BoardQty'+id), ss.wrk_formats['part_format'], value=value)
             # Build Quantity
-            total = ceil(total)
             wks.write_formula(row, col_qty,
                               '=CEILING(SUM({}:{}),1)'.format(xl_rowcol_to_cell(row, start_col + col['qty_prj0']),
                                                               xl_rowcol_to_cell(row, col_qty-1)),
                               ss.wrk_formats['part_format'],
                               value=total)
         else:
             # Build Quantity
-            total = ceil(part.qty * ss.prj_info[0]['qty'])
             wks.write_formula(row, col_qty, part.qty_str.format('BoardQty'), ss.wrk_formats['part_format'], value=total)
-        part.qty_total_spreadsheet = total
         row += 1  # Go to next row.
 
     # Return column following the globals so we know where to start next set of cells.
     # Also return the columns where the references and quantity needed of each part are stored.
     return start_col + num_cols, col_refs, col_qty, col
 
 
-def add_global_prices_to_workheet(ss, logger, start_row, start_col, total_cost_row, parts, dist_list, col):
+def add_global_prices_to_workheet(ss, start_row, start_col, total_cost_row, parts, dist_list, col):
     '''Add global prices data to the spreadsheet.'''
 
-    logger.log(DEBUG_OVERVIEW, 'Writing the global prices information...')
+    debug_overview('Writing the global prices information...')
     wks = ss.wks
     num_cols = len(col)
     num_parts = len(parts)
     num_prj = len(ss.prj_info)
     used_currencies = set()
     row = start_row + 2
     PART_INFO_FIRST_ROW = row  # Starting row of part info.
@@ -890,15 +887,15 @@
         ss.define_name_ref('PURCHASE_DESCRIPTION', next_line, col['ext_price'])
 
     # Get the actual currency rate to use.
     next_line = row + 1
     if not used_currencies:
         used_currencies.add(DEFAULT_CURRENCY)
     used_currencies = sorted(list(used_currencies))
-    logger.log(DEBUG_OVERVIEW, 'Getting distributor currency convertion rate {} to {}...'.format(used_currencies, ss.currency))
+    debug_overview('Getting distributor currency convertion rate {} to {}...'.format(used_currencies, ss.currency))
     if len(used_currencies) > 1:
         if ss.currency in used_currencies:
             used_currencies.remove(ss.currency)
         wks.write(next_line, start_col + col['value'],
                   'Used currency rates:', ss.wrk_formats['description'])
         next_line = next_line + 1
     for used_currency in used_currencies:
@@ -912,21 +909,21 @@
             next_line = next_line + 1
 
     # Return column following the globals so we know where to start next set of cells.
     # Also return the columns where the references and quantity needed of each part are stored.
     return next_line
 
 
-def add_dist_to_worksheet(ss, logger, columns_global, start_row, start_col, unit_cost_row, total_cost_row, part_ref_col, part_qty_col, dist, parts):
+def add_dist_to_worksheet(ss, columns_global, start_row, start_col, unit_cost_row, total_cost_row, part_ref_col, part_qty_col, dist, parts):
     '''Add distributor-specific part data to the spreadsheet.'''
 
     info = get_distributor_info(dist)
     order = info.order
     label = info.label.name
-    logger.log(DEBUG_OVERVIEW, '# Writing {}'.format(label))
+    debug_overview('# Writing {}'.format(label))
     wks = ss.wks
     # Columns for the various types of distributor-specific part data.
     columns = ss.DISTRIBUTOR_COLUMNS
     num_cols = len(columns)
     row = start_row  # Start building distributor section at this row.
 
     # Add label for this distributor.
@@ -950,14 +947,16 @@
     PART_INFO_LAST_ROW = PART_INFO_FIRST_ROW + num_parts - 1  # Last row of part info.
 
     col_part_num = start_col + columns['part_num']['col']
     col_purch = start_col + columns['purch']['col']
     col_unit_price = start_col + columns['unit_price']['col']
     col_ext_price = start_col + columns['ext_price']['col']
     col_moq = start_col + columns['moq']['col']
+    if not ss.SUPPRESS_DIST_DESC:
+        col_desc = start_col + columns['description']['col']
     total_cost = 0
     # How many parts were found at this distributor
     n_price_found = 0
     if num_prj > 1:
         n_price_found_l = [0]*num_prj
         total_cost_l = [0]*num_prj
     # Empty object used when no data is available for a distributor
@@ -969,15 +968,15 @@
         price_tiers = dd.price_tiers  # Extract price tiers from distributor HTML page tree.
         dist_qty_avail = dd.qty_avail
         # If the part number doesn't exist, just leave this row blank.
         # if dist_part_num is None or dist_qty_avail is None or len(price_tiers) == 0:
         if dist_part_num is None:
             row += 1  # Skip this row and go to the next.
             continue
-        dist_info_dist = {}  # Not implemented
+        dist_info_dist = dd.extra_info
         dist_currency = dd.currency  # Extract currency used by the distributor.
 
         # Enter distributor part number for ordering purposes.
         if dist_part_num:
             wks.write(row, col_part_num, dist_part_num, ss.wrk_formats['part_format'])
         else:
             if ss.SUPPRESS_CAT_URL:
@@ -1006,14 +1005,17 @@
         else:
             wks.write(row, col_avail, 'NonStk', ss.wrk_formats['not_stocked'])
             wks.write_comment(row, col_avail, 'This part is listed but is not stocked.')
 
         # Purchase quantity always starts as blank because nothing has been purchased yet.
         wks.write(row, col_purch, '', ss.wrk_formats['part_format'])
 
+        if not ss.SUPPRESS_DIST_DESC and 'desc' in dist_info_dist:
+            ss.write_string(row, col_desc, dist_info_dist['desc'], 'part_format')
+
         # Add pricing information if it exists. (Unit$/Ext$)
         if price_tiers:
             # Update the "parts found information"
             n_price_found += 1
             part_qty_cell = xl_rowcol_to_cell(row, part_qty_col)
             purch_cell = xl_rowcol_to_cell(row, col_purch)
             # Add the price for a single unit if it doesn't already exist in the tiers.
@@ -1175,15 +1177,15 @@
     if order.url:
         ss.write_url(ORDER_HEADER, col_purch-1, order.url, string='Buy here')
 
     # Write the spreadsheet code to multiple lines to create the purchase codes to
     # be used in this current distributor.
     cols = order.cols
     if not cols:
-        logger.log(DEBUG_OVERVIEW, "Purchase list codes for {d} will not be generated: no information provided.".format(d=label))
+        debug_overview("Purchase list codes for {d} will not be generated: no information provided.".format(d=label))
         return start_col + num_cols  # If not created the distributor definition, jump this final code part.
 
     if ORDER_COL_USERFIELDS in cols:
         # It is requested all the user fields at the purchase code,
         # replace the virtual annotation provided by `ORDER_COL_USERFIELDS`
         # by all user fields in the spreadsheet. This keep the compatibility
         # and configuration possibility for other features.
@@ -1191,19 +1193,19 @@
         del cols[idx]
         cols_user = list(columns_global.keys())
         for r in set(cols+['refs', 'qty', 'value', 'footprint', 'unit_price', 'ext_price', 'manf#', 'part_num', 'purch', 'desc']):
             try:
                 cols_user.remove(r)
             except ValueError:
                 pass
-        logger.log(DEBUG_OVERVIEW, "Add the {f} information for the {d} purchase list code.".format(d=label, f=cols_user))
+        debug_overview("Add the {f} information for the {d} purchase list code.".format(d=label, f=cols_user))
         cols[idx:idx] = cols_user
 
     if not('purch' in cols and ('part_num' in cols or 'manf#' in cols)):
-        logger.log(DEBUG_OVERVIEW, "Purchase list codes for {d} will not be generated: no stock# of manf# format defined.".format(d=label))
+        debug_overview("Purchase list codes for {d} will not be generated: no stock# of manf# format defined.".format(d=label))
         return start_col + num_cols  # Skip the order creation.
 
     # Create the order using the fields specified by each distributor.
     ORDER_FIRST_ROW = ORDER_FIRST_ROW + num_parts + 1
     first_part = PART_INFO_FIRST_ROW
     last_part = PART_INFO_FIRST_ROW + num_parts - 1
     # The columns needed for this distributor
@@ -1214,28 +1216,30 @@
         # with don't find, it belongs to the global part.
         if col in columns:
             info_col = start_col + columns[col]['col']
         elif col in columns_global:
             info_col = columns_global[col]
         else:
             info_col = 0
-            logger.warning(W_NOPURCH+"Not valid field `{f}` for purchase list at {d}.".format(f=col, d=label))
+            if col is not None:
+                # None is used to generate an empty column, isn't a problem
+                warning(W_NOPURCH, "Not valid field `{f}` for purchase list at {d}.".format(f=col, d=label))
         cell = xl_range(first_part, info_col, last_part)
         # Deal with conversion and string replace necessary to the correct distributors
         # code understanding.
         if col is None or (col not in columns and col not in columns_global):
             # Create an empty column escaping all the information, same when is asked
             # for a not present filed at the global column (`columns_global`) part or
             # distributors columns part (`columns`).
             order_part_info.append('""')
         elif col == 'purch':
             # Add text conversion if is a numeric cell.
             # Also make it a multiple of the MOQ.
             # Note: IF(ISNUMBER({moq}),{moq},1) prevents a /0 error
-            order_part_info.append('TEXT(ROUNDUP({purch}/IF(ISNUMBER({moq}),{moq},1))*{moq},"##0")'.format(purch=cell, moq=moq_range))
+            order_part_info.append('TEXT(ROUNDUP({purch}/IF(ISNUMBER({moq}),{moq},1),0)*{moq},"##0")'.format(purch=cell, moq=moq_range))
         elif col in ['part_num', 'manf#']:
             # Part number goes without changes
             order_part_info.append(cell)
         else:
             # All comment and description columns (that are not quantity and catalogue code)
             # These are text informative columns.
             # They can include the purchase designator
@@ -1256,15 +1260,15 @@
     # These are the columns where the part catalog numbers and purchase quantities can be found.
     if 'part_num' in cols:
         part_col = col_part_num
     elif 'manf#' in cols:
         part_col = start_col + columns_global['manf#']
     else:
         part_col = 0
-        logger.warning(W_NOQTY+"The {d} distributor order info doesn't include the part number.")
+        warning(W_NOQTY, "The {} distributor order info doesn't include the part number.".format(dist))
     part_range = xl_range(first_part, part_col, last_part)
     qty_col = col_purch
     qty_range = xl_range(first_part, qty_col, last_part)
     conditional = '=IF(ISNUMBER({qty})*({qty}>={moq})*({catn}<>""),{{}}&CHAR(10),"")'.format(qty=qty_range, catn=part_range, moq=moq_range)
     array_range = xl_range(ORDER_FIRST_ROW, ORDER_START_COL, ORDER_FIRST_ROW + num_parts - 1)
     # Concatenation operator plus distributor code delimiter.
     delimiter = '&"' + order.delimiter + '"&'
```

### Comparing `kicost-1.1.6/kicost.egg-info/PKG-INFO` & `kicost-1.1.8/kicost.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kicost
-Version: 1.1.6
+Version: 1.1.8
 Summary: Build cost spreadsheet for a KiCad project.
 Home-page: https://hildogjr.github.io/KiCost
 Author: XESS Corporation
 Author-email: info@xess.com
 License: MIT
 Project-URL: Doc, https://hildogjr.github.io/KiCost
 Project-URL: Git, https://github.com/hildogjr/KiCost
@@ -51,15 +51,24 @@
         .. image:: https://raw.githubusercontent.com/hildogjr/KiCost/master/docs/block_diag.png
         .. image:: https://raw.githubusercontent.com/hildogjr/KiCost/master/docs/gui.png
         
         
         Latest updates
         --------------
         
-        1.1.5 (2021-05-??)
+        1.1.8 (2022-05-09)
+        ______________________
+        * Add Digi-Key API
+        * Add Mouser API
+        * Add Farnell/Newark API (Element14)
+        * Add TME API
+        * Add cache for all APIs (including KitSpace and Octopart)
+        
+        
+        1.1.6 (2021-10-14)
         ______________________
         * Fix the Farnell import code order
         * Fix LCSC link and add BOM import links of all
         * Fix reference sorting and crashes
         * Add the user custom field capability to order quote
         * Add cell size adjust algorithm (use --max_column_width 0 to disable it)
         * Add ``pricing`` processing for subparts.
@@ -70,28 +79,21 @@
         
         
         1.1.4 (2020-03-24)
         ______________________
         * Add TME and Arrow to Kitspace API.
         * Others cosmetic and internal changes.
         
-        
-        1.1.3 (2019-12-31)
-        ______________________
-        * Fix the Digikey using Digi-Reel information.
-        * Added LCSC as distributor into the Kitspace API (the list can be used to JLCPCB).
-        * Parinfo kitspace API now just return the asked distributors (before was given all the avaliable distributors).
-        
-        Access https://github.com/hildogjr/KiCost/blob/master/HISTORY.rst for full development history.
+        Access https://github.com/hildogjr/KiCost/blob/master/kicost/HISTORY.rst for full development history.
 Keywords: KiCAD,BOM,electronics
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `kicost-1.1.6/kicost.egg-info/SOURCES.txt` & `kicost-1.1.8/kicost.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
+requirements.txt
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/block_diag.png
 docs/conf.py
+docs/configuration.rst
 docs/contributing.rst
 docs/gui.png
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/kicost.currency_converter.rst
 docs/kicost.distributors.rst
@@ -22,23 +24,25 @@
 docs/readme.rst
 docs/usage.rst
 kicost/AUTHORS.rst
 kicost/HISTORY.rst
 kicost/__init__.py
 kicost/__main__.py
 kicost/ansi.py
+kicost/config.py
 kicost/global_vars.py
 kicost/kicad_config.py
 kicost/kicost.ico
 kicost/kicost.py
 kicost/kicost_config.py
 kicost/kicost_gui.py
 kicost/kicost_kicadplugin.py
 kicost/kitspace.png
 kicost/log.py
+kicost/log__.py
 kicost/os_windows.py
 kicost/sexpdata.py
 kicost/spreadsheet.py
 kicost/version.py
 kicost.egg-info/PKG-INFO
 kicost.egg-info/SOURCES.txt
 kicost.egg-info/dependency_links.txt
@@ -48,22 +52,28 @@
 kicost.egg-info/top_level.txt
 kicost/currency_converter/__init__.py
 kicost/currency_converter/currency_converter.py
 kicost/currency_converter/currency_tables.py
 kicost/currency_converter/default_rates.py
 kicost/currency_converter/download_rates.py
 kicost/distributors/__init__.py
+kicost/distributors/api_digikey.py
+kicost/distributors/api_element14.py
+kicost/distributors/api_mouser.py
 kicost/distributors/api_octopart.py
 kicost/distributors/api_partinfo_kitspace.py
+kicost/distributors/api_tme.py
 kicost/distributors/dist_local_template.py
 kicost/distributors/distributor.py
 kicost/distributors/distributors_info.py
 kicost/distributors/global_vars.py
+kicost/distributors/log__.py
 kicost/edas/__init__.py
 kicost/edas/eda.py
 kicost/edas/eda_altium.py
 kicost/edas/eda_kicad.py
 kicost/edas/generic_csv.py
+kicost/edas/log__.py
 kicost/edas/tools.py
 tests/__init__.py
 tests/dummy-web-server.py
 tests/test_kicost.py
```

### Comparing `kicost-1.1.6/setup.py` & `kicost-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                          r')')
         history_lastest = re.search(update_format, history_full).group('last_history').strip()
         if history_lastest:
             if SHOW_LAST_HISTORY == 1:
                 history_lastest = history_lastest.replace('History\n-------', 'Latest update\n-------------')
             else:
                 history_lastest = history_lastest.replace('History\n-------', 'Latest updates\n--------------')
-            history = history_lastest + '\n\nAccess https://github.com/hildogjr/KiCost/blob/master/HISTORY.rst for full development history.'
+            history = history_lastest + '\n\nAccess https://github.com/hildogjr/KiCost/blob/master/kicost/HISTORY.rst for full development history.'
         else:
             history = history_full
     except Exception:
         history = history_full
         pass
 
 # KiCost Python packages requirements to run-time.
@@ -138,31 +138,31 @@
         'Doc': 'https://hildogjr.github.io/KiCost',
         'Git': 'https://github.com/hildogjr/KiCost',
     },
     packages=setuptools.find_packages(),
     entry_points={'console_scripts': ['kicost = kicost.__main__:main']},
     package_dir={'kicost': 'kicost'},
     include_package_data=True,
-    package_data={'kicost': ['*.gif', '*.png']},
+    package_data={'kicost': ['*.gif', '*.png', '*.txt']},
     # data_files=data_files,
     scripts=[],
     install_requires=requirements,
     license="MIT",
     zip_safe=False,
     keywords='KiCAD, BOM, electronics',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
     ],
     test_suite='tests',
     tests_require=test_requirements,
     cmdclass={
         'develop': PostDevelopCommand,
```

### Comparing `kicost-1.1.6/tests/dummy-web-server.py` & `kicost-1.1.8/tests/dummy-web-server.py`

 * *Files identical despite different names*

### Comparing `kicost-1.1.6/tests/test_kicost.py` & `kicost-1.1.8/tests/test_kicost.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     try:
         subprocess.check_output(cmd, stderr=subprocess.STDOUT)
     except subprocess.CalledProcessError as e:
         logging.error(e.output.decode('utf-8'))
         raise
 
 
-def run_test(name, inputs, output, extra=None, price=True, ret_err=0):
+def run_test(name, inputs, output, extra=None, price=True, ret_err=0, config_file=None):
     if not os.path.isdir(TESTDIR + '/result_test'):
         os.mkdir(TESTDIR + '/result_test')
     if not os.path.isdir(TESTDIR + '/log_test'):
         os.mkdir(TESTDIR + '/log_test')
     # Always fake the currency rates
     os.environ['KICOST_CURRENCY_RATES'] = TESTDIR + '/currency_rates.xml'
     # Now choose between recording the KitSpace queries or fake them
@@ -294,14 +294,18 @@
         server = subprocess.Popen(TESTDIR + '/dummy-web-server.py', stdout=fo, stderr=fe)
     # Run KiCost
     cmd = ['src/kicost', '--debug', '10']
     if not price:
         cmd.append('--no_price')
     if extra:
         cmd.extend(extra)
+    if config_file is not None:
+        cmd.extend(['-c', TESTDIR + '/configs/' + config_file])
+    else:
+        cmd.extend(['-c', TESTDIR + '/configs/default.yaml'])
     out_xlsx = TESTDIR + '/' + output + '.xlsx'
     cmd.extend(['-o', out_xlsx])
     cmd.extend(['-wi'] + [TESTDIR + '/' + n for n in inputs])
     log_running('Testing', cmd)
     log_err = open(TESTDIR + '/log_test/' + output + '_error.log', 'w+t')
     log_out = open(TESTDIR + '/log_test/' + output + '_out.log', 'w+t')
     ret = subprocess.call(cmd, stderr=log_err, stdout=log_out)
@@ -328,25 +332,25 @@
             xlsx_to_csv(output, 'result_test', price)
             check_diff(output + '.csv')
             xlsx_to_txt(output, 'result_test')
             check_diff(output + '.xlsx.txt')
     logging.info(output+' OK')
 
 
-def run_test_check(name, inputs=None, output=None, extra=None, price=True, ret_err=0):
+def run_test_check(name, inputs=None, output=None, extra=None, price=True, ret_err=0, config_file=None):
     logging.debug('Test name: ' + name)
     if inputs is None:
         inputs = name
     if isinstance(inputs, str):
         inputs = [inputs]
     if output is None:
         output = inputs[0]
         if output.endswith('.csv'):
             output = output[:-4]
-    run_test(name, inputs, output, extra, price, ret_err)
+    run_test(name, inputs, output, extra, price, ret_err, config_file)
 
 
 def check_errors(errors):
     res = []
     global last_err
     for error in errors:
         m = re.search(error, last_err, re.MULTILINE)
@@ -357,19 +361,29 @@
 
 
 def test_300_010():
     run_test_check('300-010')
 
 
 def test_acquire_PWM_1():
-    run_test_check('acquire-PWM')
+    run_test_check('acquire-PWM', config_file='kitspace_no_cache.yaml')
+
+
+def test_acquire_PWM_dk():
+    name = 'acquire_PWM_dk'
+    run_test_check(name, 'acquire-PWM', name, extra=['--include', 'digikey'], config_file='digikey.yaml')
+
+
+def test_acquire_PWM_eur_dk():
+    name = 'acquire_PWM_eur_dk'
+    run_test_check(name, 'acquire-PWM', name, extra=['--include', 'digikey', '--currency', 'EUR'], config_file='digikey_eur.yaml')
 
 
 def test_acquire_PWM_2():
-    run_test_check('acquire-PWM_2')
+    run_test_check('acquire-PWM_2', config_file='kitspace_no_cache.yaml')
 
 
 def test_Aeronav_R():
     run_test_check('Aeronav_R')
 
 
 def test_b3u():
@@ -481,23 +495,23 @@
 
 
 def test_Parts():
     run_test_check('TestParts')
 
 
 def test_part_list_big():
-    run_test_check('part_list_big.csv')
+    run_test_check('part_list_big.csv', config_file='kitspace_no_cache.yaml')
 
 
 def test_part_list_small_hdr():
-    run_test_check('part_list_small.csv')
+    run_test_check('part_list_small.csv', config_file='kitspace_no_cache.yaml')
 
 
 def test_part_list_small_nohdr():
-    run_test_check('part_list_small_nohdr.csv')
+    run_test_check('part_list_small_nohdr.csv', config_file='kitspace_no_cache.yaml')
 
 
 def test_multiproject_1():
     run_test_check('multiproject_1 (1 single)', 'multipart')
     run_test_check('multiproject_1 (2 single)', 'multipart2')
     run_test_check('multiproject_1', ['multipart', 'multipart2.xml'], 'multipart1+2')
 
@@ -569,15 +583,15 @@
     # Data from the fields is added to the web-scraped data
     run_test_check('scrape_over')
 
 
 def test_scrape_over_2():
     # Data from the fields relaces the web-scraped data.
     # For this we exclude the distributor with --exclude
-    run_test_check('scrape_over_2', 'scrape_over', 'scrape_over_2', extra=['--exclude', 'rs'])
+    run_test_check('scrape_over_2', 'scrape_over', 'scrape_over_2', extra=['--exclude', 'rs'], config_file='kitspace_no_cache.yaml')
 
 
 def test_manf_no_manf_num():
     # Two similar parts, but from different manufacturer and no manf#
     # Issue #474
     run_test_check('manf_no_manf_num')
 
@@ -645,38 +659,57 @@
     # File with a wrong currency, disable collapse
     name = 'rare_refs_no_collapse'
     run_test_check(name, 'rare_refs', name, extra=['--no_collapse'], price=False)
 
 
 def test_octopart_1p():
     name = 'octopart_1'
-    run_test_check(name + 'p', name, name + 'p', extra=['--octopart_key', OCTOPART_KEY, '--octopart_level', '4p'])
+    run_test_check(name + 'p', name, name + 'p', extra=['--octopart_key', OCTOPART_KEY, '--octopart_level', '4p'], config_file='octopart_no_cache.yaml')
 
 
 def test_octopart_1n():
     name = 'octopart_1'
-    run_test_check(name + 'n', name, name + 'n', extra=['--octopart_key', OCTOPART_KEY, '--octopart_level', '4'])
+    run_test_check(name + 'n', name, name + 'n', config_file='octopart_no_cache.yaml')
 
 
 def test_octopart_1_ambi():
     name = 'octopart_1_ambi'
-    run_test_check(name, extra=['--octopart_key', OCTOPART_KEY, '--octopart_level', '4p'])
+    run_test_check(name, extra=['--octopart_key', OCTOPART_KEY, '--octopart_level', '4p'], config_file='octopart_no_cache.yaml')
     check_errors([r'Using "Adafruit Industries" for manf#="4062"', r'Ambiguous manf#="4062" please use manf to select the right one, choices:'])
 
 
 def test_octopart_2n():
     name = 'octopart_2'
-    run_test_check(name + 'n', name, name + 'n', extra=['--octopart_key', OCTOPART_KEY, '--octopart_level', '4'])
+    run_test_check(name + 'n', name, name + 'n', extra=['--disable_api', 'KitSpace'], config_file='octopart.yaml')
 
 
 def test_337():
     # Test for issue #337
     run_test_check('test_337_UserFieldCombining', extra=['--field', 'Supplier'], price=False)
 
 
+def test_mouser_1():
+    test_name = 'mouser_1'
+    fields = ['S1MN', 'S1PN', 'S2MN', 'S2PN']
+    extra = ['--split_extra_fields'] + fields + ['-f'] + fields + ['--include', 'mouser']
+    run_test_check(test_name, 'complex_multipart', test_name, extra=extra, config_file='mouser.yaml')
+
+
+def test_element14_1():
+    test_name = 'element14_1'
+    extra = ['--include', 'farnell', 'newark']
+    run_test_check(test_name, 'safelink_receiver', test_name, extra=extra, config_file='element14.yaml')
+
+
+def test_tme_1():
+    test_name = 'tme_1'
+    extra = ['--include', 'tme']
+    run_test_check(test_name, 'safelink_receiver', test_name, extra=extra, config_file='tme.yaml')
+
+
 class TestKicost(unittest.TestCase):
 
     def setUp(self):
         pass
 
     def test_something(self):
         pass
```

