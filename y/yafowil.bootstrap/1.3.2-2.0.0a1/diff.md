# Comparing `tmp/yafowil.bootstrap-1.3.2.tar.gz` & `tmp/yafowil.bootstrap-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafowil.bootstrap-1.3.2.tar", last modified: Mon Dec  5 12:02:18 2022, max compression
+gzip compressed data, was "yafowil.bootstrap-2.0.0a1.tar", last modified: Mon May 15 12:28:21 2023, max compression
```

## Comparing `yafowil.bootstrap-1.3.2.tar` & `yafowil.bootstrap-2.0.0a1.tar`

### file list

```diff
@@ -1,38 +1,117 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      852 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5234 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1363 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1431 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      924 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3223 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/common.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/css/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    21368 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/css/bootstrap-theme.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18860 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/css/bootstrap-theme.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)   132546 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/css/bootstrap.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)   109518 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/css/bootstrap.min.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/fonts/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    20335 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 rnix      (1000) rnix      (1000)    62927 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 rnix      (1000) rnix      (1000)    41280 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23320 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/js/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    60681 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/js/bootstrap.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    31819 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/js/bootstrap.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      167 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/tests.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 12:02:18.240447 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5234 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1161 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      112 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       46 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2022-12-05 12:02:18.000000 yafowil.bootstrap-1.3.2/src/yafowil.bootstrap.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.601839 yafowil.bootstrap-2.0.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1400 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1398 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5293 2023-05-15 12:28:21.601839 yafowil.bootstrap-2.0.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1975 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      452 2023-05-15 12:28:21.601839 yafowil.bootstrap-2.0.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1275 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.585839 yafowil.bootstrap-2.0.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.585839 yafowil.bootstrap-2.0.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.585839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6200 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3320 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/bs3.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4029 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/bs4.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4065 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/bs5.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.585839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.585839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.589839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    25682 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap-theme.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    48005 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap-theme.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23411 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap-theme.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    75600 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   145933 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   390887 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   121457 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   540434 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap.min.css.map
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.589839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/fonts/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    20127 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   108738 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    45404 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23424 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18028 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.589839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/js/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    75484 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/js/bootstrap.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    39680 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/js/bootstrap.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      484 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/js/npm.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.585839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.589839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    67472 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap-grid.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   157879 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap-grid.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    50636 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap-grid.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   115037 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4784 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap-reboot.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    77416 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap-reboot.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3922 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap-reboot.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    32534 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   199412 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   511248 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   161409 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   650715 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/css/bootstrap.min.css.map
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.593839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   236864 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/bootstrap.bundle.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   409586 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/bootstrap.bundle.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    84378 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/bootstrap.bundle.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   316181 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   144033 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/bootstrap.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   254480 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/bootstrap.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    63467 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/bootstrap.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   192479 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs4/js/bootstrap.min.js.map
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.585839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.597839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    70538 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-grid.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   196535 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-grid.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    51319 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-grid.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   117439 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    70612 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   196539 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    51394 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   117516 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5850 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-reboot.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   105138 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-reboot.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4646 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-reboot.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    35330 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5827 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   105151 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4718 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    41570 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    71584 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-utilities.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   192271 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-utilities.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    53479 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-utilities.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   111875 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    71451 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   192214 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    53407 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   111710 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   204136 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   536547 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   162720 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   449111 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   203803 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap.rtl.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   536461 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap.rtl.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   162825 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap.rtl.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   661035 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/css/bootstrap.rtl.min.css.map
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.601839 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   208492 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.bundle.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   425643 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.bundle.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    78468 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.bundle.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   327261 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   139019 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.esm.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   288320 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.esm.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    72016 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.esm.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   222508 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   148168 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   289522 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    59511 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   217145 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs5/js/bootstrap.min.js.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5265 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/tests.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:28:21.585839 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5293 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5663 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:28:21.000000 yafowil.bootstrap-2.0.0a1/src/yafowil.bootstrap.egg-info/top_level.txt
```

### Comparing `yafowil.bootstrap-1.3.2/LICENSE.rst` & `yafowil.bootstrap-2.0.0a1/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 License
 =======
 
 Copyright (c) 2012-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
-Copyright (c) 2021-2022, Yafowil Contributors
+Copyright (c) 2021, Yafowil Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `yafowil.bootstrap-1.3.2/setup.py` & `yafowil.bootstrap-2.0.0a1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.3.2'
+version = '2.0.0a1'
 shortdesc = 'Bootstrap Styles for YAFOWIL'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
 
@@ -37,21 +37,15 @@
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['yafowil'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
-        'yafowil>1.99',
+        'webresource',
+        'yafowil>2.2.99'
     ],
-    extras_require=dict(
-        test=[
-            'yafowil[test]'
-        ]
-    ),
-    test_suite="yafowil.bootstrap.tests.test_suite",
     entry_points="""
     [yafowil.plugin]
     register = yafowil.bootstrap:register
-    configure = yafowil.bootstrap:configure
     """
 )
```

### Comparing `yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/common.py` & `yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/bs3.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     if data.errors:
         return 'form-group has-error'
     return 'form-group'
 
 
 def configure_factory():
     # set theme
-    factory.theme = 'bootstrap'
+    factory.theme = 'bootstrap3'
 
     # common defaults
     factory.defaults['text.class'] = 'text form-control'
 
     factory.defaults['textarea.class'] = 'textarea form-control'
 
     factory.defaults['lines.class'] = 'lines form-control'
@@ -45,55 +45,62 @@
     factory.defaults['error.message_class'] = 'text-danger'
 
     factory.defaults['help.position'] = 'after'
     factory.defaults['help.tag'] = 'p'
     factory.defaults['help.class'] = 'help-block'
 
     # yafowil.widget.array
-    factory.defaults['array.table_class'] = \
-        'table table-condensed'
+    factory.defaults['array.table_class'] = 'table table-condensed'
 
     # yafowil.widget.autocomplete
     factory.defaults['autocomplete.class'] = 'autocomplete form-control'
 
     # yafowil.widget.chosen
     factory.defaults['chosen.class'] = 'chosen form-control'
 
     # yafowil.widget.datetime
     factory.defaults['datetime.datepicker_class'] = 'datepicker form-control'
     factory.defaults['datetime.timepicker_class'] = 'timepicker form-control'
     factory.defaults['time.timepicker_class'] = 'timepicker form-control'
 
     # yafowil.widget.dict
-    factory.defaults['dict.table_class'] = \
-        'dictwidget table table-condensed'
+    factory.defaults['dict.table_class'] = 'dictwidget table table-condensed'
     factory.defaults['dict.key_class'] = 'form-control'
     factory.defaults['dict.value_class'] = 'form-control'
 
     # yafowil.widget.wysihtml5
     factory.defaults['wysihtml5.class'] = 'wysihtml5 form-control'
 
 
 def register_macros():
     # common
-    factory.register_macro('form', 'form', {
-        'form.class': 'form-horizontal',
-    })
-    factory.register_macro('field', 'field:label:div:help:error', {
-        'label.class_add': 'col-sm-2',
-        'div.class_add': 'col-sm-10',
-    })
-    factory.register_macro('button', 'submit', {
-        'submit.class': 'btn',
-        'submit.class_add': 'btn-default',
-    })
+    factory.register_macro('form', 'form', {'form.class': 'form-horizontal'})
+    factory.register_macro(
+        'field',
+        'field:label:div:help:error',
+        {
+            'label.class_add': 'col-sm-2',
+            'div.class_add': 'col-sm-10'
+        }
+    )
+    factory.register_macro(
+        'button',
+        'submit', {
+            'submit.class': 'btn',
+            'submit.class_add': 'btn-default'
+        }
+    )
 
     # yafowil.widget.array
-    factory.register_macro('array', 'field:label:help:error:array', {
-        'array.label': ' ',
-        'field.class': bs_field_class,
-        'label.class_add': 'col-sm-2',
-        'array.class_add': 'col-sm-10',
-        'help.class_add': 'col-sm-offset-2 col-sm-10',
-        'error.class_add': 'col-sm-offset-2 col-sm-10',
-    })
+    factory.register_macro(
+        'array',
+        'field:label:help:error:array',
+        {
+            'array.label': ' ',
+            'field.class': bs_field_class,
+            'label.class_add': 'col-sm-2',
+            'array.class_add': 'col-sm-10',
+            'help.class_add': 'col-sm-offset-2 col-sm-10',
+            'error.class_add': 'col-sm-offset-2 col-sm-10'
+        }
+    )
     factory.register_macro('arrayfield', 'field:label:help:error', {})
```

### Comparing `yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/css/bootstrap-theme.css` & `yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap-theme.min.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,442 +1,6 @@
 /*!
- * Bootstrap v3.2.0 (http://getbootstrap.com)
- * Copyright 2011-2014 Twitter, Inc.
+ * Bootstrap v3.4.1 (https://getbootstrap.com/)
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
- */
-
-.btn-default,
-.btn-primary,
-.btn-success,
-.btn-info,
-.btn-warning,
-.btn-danger {
-  text-shadow: 0 -1px 0 rgba(0, 0, 0, .2);
-  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, .15), 0 1px 1px rgba(0, 0, 0, .075);
-          box-shadow: inset 0 1px 0 rgba(255, 255, 255, .15), 0 1px 1px rgba(0, 0, 0, .075);
-}
-.btn-default:active,
-.btn-primary:active,
-.btn-success:active,
-.btn-info:active,
-.btn-warning:active,
-.btn-danger:active,
-.btn-default.active,
-.btn-primary.active,
-.btn-success.active,
-.btn-info.active,
-.btn-warning.active,
-.btn-danger.active {
-  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);
-          box-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);
-}
-.btn:active,
-.btn.active {
-  background-image: none;
-}
-.btn-default {
-  text-shadow: 0 1px 0 #fff;
-  background-image: -webkit-linear-gradient(top, #fff 0%, #e0e0e0 100%);
-  background-image:      -o-linear-gradient(top, #fff 0%, #e0e0e0 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#fff), to(#e0e0e0));
-  background-image:         linear-gradient(to bottom, #fff 0%, #e0e0e0 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffffffff', endColorstr='#ffe0e0e0', GradientType=0);
-  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
-  background-repeat: repeat-x;
-  border-color: #dbdbdb;
-  border-color: #ccc;
-}
-.btn-default:hover,
-.btn-default:focus {
-  background-color: #e0e0e0;
-  background-position: 0 -15px;
-}
-.btn-default:active,
-.btn-default.active {
-  background-color: #e0e0e0;
-  border-color: #dbdbdb;
-}
-.btn-default:disabled,
-.btn-default[disabled] {
-  background-color: #e0e0e0;
-  background-image: none;
-}
-.btn-primary {
-  background-image: -webkit-linear-gradient(top, #428bca 0%, #2d6ca2 100%);
-  background-image:      -o-linear-gradient(top, #428bca 0%, #2d6ca2 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#428bca), to(#2d6ca2));
-  background-image:         linear-gradient(to bottom, #428bca 0%, #2d6ca2 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff428bca', endColorstr='#ff2d6ca2', GradientType=0);
-  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
-  background-repeat: repeat-x;
-  border-color: #2b669a;
-}
-.btn-primary:hover,
-.btn-primary:focus {
-  background-color: #2d6ca2;
-  background-position: 0 -15px;
-}
-.btn-primary:active,
-.btn-primary.active {
-  background-color: #2d6ca2;
-  border-color: #2b669a;
-}
-.btn-primary:disabled,
-.btn-primary[disabled] {
-  background-color: #2d6ca2;
-  background-image: none;
-}
-.btn-success {
-  background-image: -webkit-linear-gradient(top, #5cb85c 0%, #419641 100%);
-  background-image:      -o-linear-gradient(top, #5cb85c 0%, #419641 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#5cb85c), to(#419641));
-  background-image:         linear-gradient(to bottom, #5cb85c 0%, #419641 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff5cb85c', endColorstr='#ff419641', GradientType=0);
-  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
-  background-repeat: repeat-x;
-  border-color: #3e8f3e;
-}
-.btn-success:hover,
-.btn-success:focus {
-  background-color: #419641;
-  background-position: 0 -15px;
-}
-.btn-success:active,
-.btn-success.active {
-  background-color: #419641;
-  border-color: #3e8f3e;
-}
-.btn-success:disabled,
-.btn-success[disabled] {
-  background-color: #419641;
-  background-image: none;
-}
-.btn-info {
-  background-image: -webkit-linear-gradient(top, #5bc0de 0%, #2aabd2 100%);
-  background-image:      -o-linear-gradient(top, #5bc0de 0%, #2aabd2 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#5bc0de), to(#2aabd2));
-  background-image:         linear-gradient(to bottom, #5bc0de 0%, #2aabd2 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff5bc0de', endColorstr='#ff2aabd2', GradientType=0);
-  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
-  background-repeat: repeat-x;
-  border-color: #28a4c9;
-}
-.btn-info:hover,
-.btn-info:focus {
-  background-color: #2aabd2;
-  background-position: 0 -15px;
-}
-.btn-info:active,
-.btn-info.active {
-  background-color: #2aabd2;
-  border-color: #28a4c9;
-}
-.btn-info:disabled,
-.btn-info[disabled] {
-  background-color: #2aabd2;
-  background-image: none;
-}
-.btn-warning {
-  background-image: -webkit-linear-gradient(top, #f0ad4e 0%, #eb9316 100%);
-  background-image:      -o-linear-gradient(top, #f0ad4e 0%, #eb9316 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#f0ad4e), to(#eb9316));
-  background-image:         linear-gradient(to bottom, #f0ad4e 0%, #eb9316 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff0ad4e', endColorstr='#ffeb9316', GradientType=0);
-  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
-  background-repeat: repeat-x;
-  border-color: #e38d13;
-}
-.btn-warning:hover,
-.btn-warning:focus {
-  background-color: #eb9316;
-  background-position: 0 -15px;
-}
-.btn-warning:active,
-.btn-warning.active {
-  background-color: #eb9316;
-  border-color: #e38d13;
-}
-.btn-warning:disabled,
-.btn-warning[disabled] {
-  background-color: #eb9316;
-  background-image: none;
-}
-.btn-danger {
-  background-image: -webkit-linear-gradient(top, #d9534f 0%, #c12e2a 100%);
-  background-image:      -o-linear-gradient(top, #d9534f 0%, #c12e2a 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#d9534f), to(#c12e2a));
-  background-image:         linear-gradient(to bottom, #d9534f 0%, #c12e2a 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffd9534f', endColorstr='#ffc12e2a', GradientType=0);
-  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
-  background-repeat: repeat-x;
-  border-color: #b92c28;
-}
-.btn-danger:hover,
-.btn-danger:focus {
-  background-color: #c12e2a;
-  background-position: 0 -15px;
-}
-.btn-danger:active,
-.btn-danger.active {
-  background-color: #c12e2a;
-  border-color: #b92c28;
-}
-.btn-danger:disabled,
-.btn-danger[disabled] {
-  background-color: #c12e2a;
-  background-image: none;
-}
-.thumbnail,
-.img-thumbnail {
-  -webkit-box-shadow: 0 1px 2px rgba(0, 0, 0, .075);
-          box-shadow: 0 1px 2px rgba(0, 0, 0, .075);
-}
-.dropdown-menu > li > a:hover,
-.dropdown-menu > li > a:focus {
-  background-color: #e8e8e8;
-  background-image: -webkit-linear-gradient(top, #f5f5f5 0%, #e8e8e8 100%);
-  background-image:      -o-linear-gradient(top, #f5f5f5 0%, #e8e8e8 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#f5f5f5), to(#e8e8e8));
-  background-image:         linear-gradient(to bottom, #f5f5f5 0%, #e8e8e8 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff5f5f5', endColorstr='#ffe8e8e8', GradientType=0);
-  background-repeat: repeat-x;
-}
-.dropdown-menu > .active > a,
-.dropdown-menu > .active > a:hover,
-.dropdown-menu > .active > a:focus {
-  background-color: #357ebd;
-  background-image: -webkit-linear-gradient(top, #428bca 0%, #357ebd 100%);
-  background-image:      -o-linear-gradient(top, #428bca 0%, #357ebd 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#428bca), to(#357ebd));
-  background-image:         linear-gradient(to bottom, #428bca 0%, #357ebd 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff428bca', endColorstr='#ff357ebd', GradientType=0);
-  background-repeat: repeat-x;
-}
-.navbar-default {
-  background-image: -webkit-linear-gradient(top, #fff 0%, #f8f8f8 100%);
-  background-image:      -o-linear-gradient(top, #fff 0%, #f8f8f8 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#fff), to(#f8f8f8));
-  background-image:         linear-gradient(to bottom, #fff 0%, #f8f8f8 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffffffff', endColorstr='#fff8f8f8', GradientType=0);
-  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
-  background-repeat: repeat-x;
-  border-radius: 4px;
-  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, .15), 0 1px 5px rgba(0, 0, 0, .075);
-          box-shadow: inset 0 1px 0 rgba(255, 255, 255, .15), 0 1px 5px rgba(0, 0, 0, .075);
-}
-.navbar-default .navbar-nav > .active > a {
-  background-image: -webkit-linear-gradient(top, #ebebeb 0%, #f3f3f3 100%);
-  background-image:      -o-linear-gradient(top, #ebebeb 0%, #f3f3f3 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#ebebeb), to(#f3f3f3));
-  background-image:         linear-gradient(to bottom, #ebebeb 0%, #f3f3f3 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffebebeb', endColorstr='#fff3f3f3', GradientType=0);
-  background-repeat: repeat-x;
-  -webkit-box-shadow: inset 0 3px 9px rgba(0, 0, 0, .075);
-          box-shadow: inset 0 3px 9px rgba(0, 0, 0, .075);
-}
-.navbar-brand,
-.navbar-nav > li > a {
-  text-shadow: 0 1px 0 rgba(255, 255, 255, .25);
-}
-.navbar-inverse {
-  background-image: -webkit-linear-gradient(top, #3c3c3c 0%, #222 100%);
-  background-image:      -o-linear-gradient(top, #3c3c3c 0%, #222 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#3c3c3c), to(#222));
-  background-image:         linear-gradient(to bottom, #3c3c3c 0%, #222 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff3c3c3c', endColorstr='#ff222222', GradientType=0);
-  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
-  background-repeat: repeat-x;
-}
-.navbar-inverse .navbar-nav > .active > a {
-  background-image: -webkit-linear-gradient(top, #222 0%, #282828 100%);
-  background-image:      -o-linear-gradient(top, #222 0%, #282828 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#222), to(#282828));
-  background-image:         linear-gradient(to bottom, #222 0%, #282828 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff222222', endColorstr='#ff282828', GradientType=0);
-  background-repeat: repeat-x;
-  -webkit-box-shadow: inset 0 3px 9px rgba(0, 0, 0, .25);
-          box-shadow: inset 0 3px 9px rgba(0, 0, 0, .25);
-}
-.navbar-inverse .navbar-brand,
-.navbar-inverse .navbar-nav > li > a {
-  text-shadow: 0 -1px 0 rgba(0, 0, 0, .25);
-}
-.navbar-static-top,
-.navbar-fixed-top,
-.navbar-fixed-bottom {
-  border-radius: 0;
-}
-.alert {
-  text-shadow: 0 1px 0 rgba(255, 255, 255, .2);
-  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, .25), 0 1px 2px rgba(0, 0, 0, .05);
-          box-shadow: inset 0 1px 0 rgba(255, 255, 255, .25), 0 1px 2px rgba(0, 0, 0, .05);
-}
-.alert-success {
-  background-image: -webkit-linear-gradient(top, #dff0d8 0%, #c8e5bc 100%);
-  background-image:      -o-linear-gradient(top, #dff0d8 0%, #c8e5bc 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#dff0d8), to(#c8e5bc));
-  background-image:         linear-gradient(to bottom, #dff0d8 0%, #c8e5bc 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffdff0d8', endColorstr='#ffc8e5bc', GradientType=0);
-  background-repeat: repeat-x;
-  border-color: #b2dba1;
-}
-.alert-info {
-  background-image: -webkit-linear-gradient(top, #d9edf7 0%, #b9def0 100%);
-  background-image:      -o-linear-gradient(top, #d9edf7 0%, #b9def0 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#d9edf7), to(#b9def0));
-  background-image:         linear-gradient(to bottom, #d9edf7 0%, #b9def0 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffd9edf7', endColorstr='#ffb9def0', GradientType=0);
-  background-repeat: repeat-x;
-  border-color: #9acfea;
-}
-.alert-warning {
-  background-image: -webkit-linear-gradient(top, #fcf8e3 0%, #f8efc0 100%);
-  background-image:      -o-linear-gradient(top, #fcf8e3 0%, #f8efc0 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#fcf8e3), to(#f8efc0));
-  background-image:         linear-gradient(to bottom, #fcf8e3 0%, #f8efc0 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#fffcf8e3', endColorstr='#fff8efc0', GradientType=0);
-  background-repeat: repeat-x;
-  border-color: #f5e79e;
-}
-.alert-danger {
-  background-image: -webkit-linear-gradient(top, #f2dede 0%, #e7c3c3 100%);
-  background-image:      -o-linear-gradient(top, #f2dede 0%, #e7c3c3 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#f2dede), to(#e7c3c3));
-  background-image:         linear-gradient(to bottom, #f2dede 0%, #e7c3c3 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff2dede', endColorstr='#ffe7c3c3', GradientType=0);
-  background-repeat: repeat-x;
-  border-color: #dca7a7;
-}
-.progress {
-  background-image: -webkit-linear-gradient(top, #ebebeb 0%, #f5f5f5 100%);
-  background-image:      -o-linear-gradient(top, #ebebeb 0%, #f5f5f5 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#ebebeb), to(#f5f5f5));
-  background-image:         linear-gradient(to bottom, #ebebeb 0%, #f5f5f5 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffebebeb', endColorstr='#fff5f5f5', GradientType=0);
-  background-repeat: repeat-x;
-}
-.progress-bar {
-  background-image: -webkit-linear-gradient(top, #428bca 0%, #3071a9 100%);
-  background-image:      -o-linear-gradient(top, #428bca 0%, #3071a9 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#428bca), to(#3071a9));
-  background-image:         linear-gradient(to bottom, #428bca 0%, #3071a9 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff428bca', endColorstr='#ff3071a9', GradientType=0);
-  background-repeat: repeat-x;
-}
-.progress-bar-success {
-  background-image: -webkit-linear-gradient(top, #5cb85c 0%, #449d44 100%);
-  background-image:      -o-linear-gradient(top, #5cb85c 0%, #449d44 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#5cb85c), to(#449d44));
-  background-image:         linear-gradient(to bottom, #5cb85c 0%, #449d44 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff5cb85c', endColorstr='#ff449d44', GradientType=0);
-  background-repeat: repeat-x;
-}
-.progress-bar-info {
-  background-image: -webkit-linear-gradient(top, #5bc0de 0%, #31b0d5 100%);
-  background-image:      -o-linear-gradient(top, #5bc0de 0%, #31b0d5 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#5bc0de), to(#31b0d5));
-  background-image:         linear-gradient(to bottom, #5bc0de 0%, #31b0d5 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff5bc0de', endColorstr='#ff31b0d5', GradientType=0);
-  background-repeat: repeat-x;
-}
-.progress-bar-warning {
-  background-image: -webkit-linear-gradient(top, #f0ad4e 0%, #ec971f 100%);
-  background-image:      -o-linear-gradient(top, #f0ad4e 0%, #ec971f 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#f0ad4e), to(#ec971f));
-  background-image:         linear-gradient(to bottom, #f0ad4e 0%, #ec971f 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff0ad4e', endColorstr='#ffec971f', GradientType=0);
-  background-repeat: repeat-x;
-}
-.progress-bar-danger {
-  background-image: -webkit-linear-gradient(top, #d9534f 0%, #c9302c 100%);
-  background-image:      -o-linear-gradient(top, #d9534f 0%, #c9302c 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#d9534f), to(#c9302c));
-  background-image:         linear-gradient(to bottom, #d9534f 0%, #c9302c 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffd9534f', endColorstr='#ffc9302c', GradientType=0);
-  background-repeat: repeat-x;
-}
-.progress-bar-striped {
-  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:      -o-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:         linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-}
-.list-group {
-  border-radius: 4px;
-  -webkit-box-shadow: 0 1px 2px rgba(0, 0, 0, .075);
-          box-shadow: 0 1px 2px rgba(0, 0, 0, .075);
-}
-.list-group-item.active,
-.list-group-item.active:hover,
-.list-group-item.active:focus {
-  text-shadow: 0 -1px 0 #3071a9;
-  background-image: -webkit-linear-gradient(top, #428bca 0%, #3278b3 100%);
-  background-image:      -o-linear-gradient(top, #428bca 0%, #3278b3 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#428bca), to(#3278b3));
-  background-image:         linear-gradient(to bottom, #428bca 0%, #3278b3 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff428bca', endColorstr='#ff3278b3', GradientType=0);
-  background-repeat: repeat-x;
-  border-color: #3278b3;
-}
-.panel {
-  -webkit-box-shadow: 0 1px 2px rgba(0, 0, 0, .05);
-          box-shadow: 0 1px 2px rgba(0, 0, 0, .05);
-}
-.panel-default > .panel-heading {
-  background-image: -webkit-linear-gradient(top, #f5f5f5 0%, #e8e8e8 100%);
-  background-image:      -o-linear-gradient(top, #f5f5f5 0%, #e8e8e8 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#f5f5f5), to(#e8e8e8));
-  background-image:         linear-gradient(to bottom, #f5f5f5 0%, #e8e8e8 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff5f5f5', endColorstr='#ffe8e8e8', GradientType=0);
-  background-repeat: repeat-x;
-}
-.panel-primary > .panel-heading {
-  background-image: -webkit-linear-gradient(top, #428bca 0%, #357ebd 100%);
-  background-image:      -o-linear-gradient(top, #428bca 0%, #357ebd 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#428bca), to(#357ebd));
-  background-image:         linear-gradient(to bottom, #428bca 0%, #357ebd 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff428bca', endColorstr='#ff357ebd', GradientType=0);
-  background-repeat: repeat-x;
-}
-.panel-success > .panel-heading {
-  background-image: -webkit-linear-gradient(top, #dff0d8 0%, #d0e9c6 100%);
-  background-image:      -o-linear-gradient(top, #dff0d8 0%, #d0e9c6 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#dff0d8), to(#d0e9c6));
-  background-image:         linear-gradient(to bottom, #dff0d8 0%, #d0e9c6 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffdff0d8', endColorstr='#ffd0e9c6', GradientType=0);
-  background-repeat: repeat-x;
-}
-.panel-info > .panel-heading {
-  background-image: -webkit-linear-gradient(top, #d9edf7 0%, #c4e3f3 100%);
-  background-image:      -o-linear-gradient(top, #d9edf7 0%, #c4e3f3 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#d9edf7), to(#c4e3f3));
-  background-image:         linear-gradient(to bottom, #d9edf7 0%, #c4e3f3 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffd9edf7', endColorstr='#ffc4e3f3', GradientType=0);
-  background-repeat: repeat-x;
-}
-.panel-warning > .panel-heading {
-  background-image: -webkit-linear-gradient(top, #fcf8e3 0%, #faf2cc 100%);
-  background-image:      -o-linear-gradient(top, #fcf8e3 0%, #faf2cc 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#fcf8e3), to(#faf2cc));
-  background-image:         linear-gradient(to bottom, #fcf8e3 0%, #faf2cc 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#fffcf8e3', endColorstr='#fffaf2cc', GradientType=0);
-  background-repeat: repeat-x;
-}
-.panel-danger > .panel-heading {
-  background-image: -webkit-linear-gradient(top, #f2dede 0%, #ebcccc 100%);
-  background-image:      -o-linear-gradient(top, #f2dede 0%, #ebcccc 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#f2dede), to(#ebcccc));
-  background-image:         linear-gradient(to bottom, #f2dede 0%, #ebcccc 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff2dede', endColorstr='#ffebcccc', GradientType=0);
-  background-repeat: repeat-x;
-}
-.well {
-  background-image: -webkit-linear-gradient(top, #e8e8e8 0%, #f5f5f5 100%);
-  background-image:      -o-linear-gradient(top, #e8e8e8 0%, #f5f5f5 100%);
-  background-image: -webkit-gradient(linear, left top, left bottom, from(#e8e8e8), to(#f5f5f5));
-  background-image:         linear-gradient(to bottom, #e8e8e8 0%, #f5f5f5 100%);
-  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffe8e8e8', endColorstr='#fff5f5f5', GradientType=0);
-  background-repeat: repeat-x;
-  border-color: #dcdcdc;
-  -webkit-box-shadow: inset 0 1px 3px rgba(0, 0, 0, .05), 0 1px 0 rgba(255, 255, 255, .1);
-          box-shadow: inset 0 1px 3px rgba(0, 0, 0, .05), 0 1px 0 rgba(255, 255, 255, .1);
-}
-/*# sourceMappingURL=bootstrap-theme.css.map */
+ */.btn-danger,.btn-default,.btn-info,.btn-primary,.btn-success,.btn-warning{text-shadow:0 -1px 0 rgba(0,0,0,.2);-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.15),0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 0 rgba(255,255,255,.15),0 1px 1px rgba(0,0,0,.075)}.btn-danger.active,.btn-danger:active,.btn-default.active,.btn-default:active,.btn-info.active,.btn-info:active,.btn-primary.active,.btn-primary:active,.btn-success.active,.btn-success:active,.btn-warning.active,.btn-warning:active{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-danger.disabled,.btn-danger[disabled],.btn-default.disabled,.btn-default[disabled],.btn-info.disabled,.btn-info[disabled],.btn-primary.disabled,.btn-primary[disabled],.btn-success.disabled,.btn-success[disabled],.btn-warning.disabled,.btn-warning[disabled],fieldset[disabled] .btn-danger,fieldset[disabled] .btn-default,fieldset[disabled] .btn-info,fieldset[disabled] .btn-primary,fieldset[disabled] .btn-success,fieldset[disabled] .btn-warning{-webkit-box-shadow:none;box-shadow:none}.btn-danger .badge,.btn-default .badge,.btn-info .badge,.btn-primary .badge,.btn-success .badge,.btn-warning .badge{text-shadow:none}.btn.active,.btn:active{background-image:none}.btn-default{background-image:-webkit-linear-gradient(top,#fff 0,#e0e0e0 100%);background-image:-o-linear-gradient(top,#fff 0,#e0e0e0 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#fff),to(#e0e0e0));background-image:linear-gradient(to bottom,#fff 0,#e0e0e0 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffffffff', endColorstr='#ffe0e0e0', GradientType=0);filter:progid:DXImageTransform.Microsoft.gradient(enabled=false);background-repeat:repeat-x;border-color:#dbdbdb;text-shadow:0 1px 0 #fff;border-color:#ccc}.btn-default:focus,.btn-default:hover{background-color:#e0e0e0;background-position:0 -15px}.btn-default.active,.btn-default:active{background-color:#e0e0e0;border-color:#dbdbdb}.btn-default.disabled,.btn-default.disabled.active,.btn-default.disabled.focus,.btn-default.disabled:active,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled],.btn-default[disabled].active,.btn-default[disabled].focus,.btn-default[disabled]:active,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default,fieldset[disabled] .btn-default.active,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:active,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#e0e0e0;background-image:none}.btn-primary{background-image:-webkit-linear-gradient(top,#337ab7 0,#265a88 100%);background-image:-o-linear-gradient(top,#337ab7 0,#265a88 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#337ab7),to(#265a88));background-image:linear-gradient(to bottom,#337ab7 0,#265a88 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff337ab7', endColorstr='#ff265a88', GradientType=0);filter:progid:DXImageTransform.Microsoft.gradient(enabled=false);background-repeat:repeat-x;border-color:#245580}.btn-primary:focus,.btn-primary:hover{background-color:#265a88;background-position:0 -15px}.btn-primary.active,.btn-primary:active{background-color:#265a88;border-color:#245580}.btn-primary.disabled,.btn-primary.disabled.active,.btn-primary.disabled.focus,.btn-primary.disabled:active,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled],.btn-primary[disabled].active,.btn-primary[disabled].focus,.btn-primary[disabled]:active,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary,fieldset[disabled] .btn-primary.active,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:active,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#265a88;background-image:none}.btn-success{background-image:-webkit-linear-gradient(top,#5cb85c 0,#419641 100%);background-image:-o-linear-gradient(top,#5cb85c 0,#419641 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#5cb85c),to(#419641));background-image:linear-gradient(to bottom,#5cb85c 0,#419641 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff5cb85c', endColorstr='#ff419641', GradientType=0);filter:progid:DXImageTransform.Microsoft.gradient(enabled=false);background-repeat:repeat-x;border-color:#3e8f3e}.btn-success:focus,.btn-success:hover{background-color:#419641;background-position:0 -15px}.btn-success.active,.btn-success:active{background-color:#419641;border-color:#3e8f3e}.btn-success.disabled,.btn-success.disabled.active,.btn-success.disabled.focus,.btn-success.disabled:active,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled],.btn-success[disabled].active,.btn-success[disabled].focus,.btn-success[disabled]:active,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success,fieldset[disabled] .btn-success.active,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:active,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#419641;background-image:none}.btn-info{background-image:-webkit-linear-gradient(top,#5bc0de 0,#2aabd2 100%);background-image:-o-linear-gradient(top,#5bc0de 0,#2aabd2 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#5bc0de),to(#2aabd2));background-image:linear-gradient(to bottom,#5bc0de 0,#2aabd2 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff5bc0de', endColorstr='#ff2aabd2', GradientType=0);filter:progid:DXImageTransform.Microsoft.gradient(enabled=false);background-repeat:repeat-x;border-color:#28a4c9}.btn-info:focus,.btn-info:hover{background-color:#2aabd2;background-position:0 -15px}.btn-info.active,.btn-info:active{background-color:#2aabd2;border-color:#28a4c9}.btn-info.disabled,.btn-info.disabled.active,.btn-info.disabled.focus,.btn-info.disabled:active,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled],.btn-info[disabled].active,.btn-info[disabled].focus,.btn-info[disabled]:active,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info,fieldset[disabled] .btn-info.active,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:active,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#2aabd2;background-image:none}.btn-warning{background-image:-webkit-linear-gradient(top,#f0ad4e 0,#eb9316 100%);background-image:-o-linear-gradient(top,#f0ad4e 0,#eb9316 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#f0ad4e),to(#eb9316));background-image:linear-gradient(to bottom,#f0ad4e 0,#eb9316 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff0ad4e', endColorstr='#ffeb9316', GradientType=0);filter:progid:DXImageTransform.Microsoft.gradient(enabled=false);background-repeat:repeat-x;border-color:#e38d13}.btn-warning:focus,.btn-warning:hover{background-color:#eb9316;background-position:0 -15px}.btn-warning.active,.btn-warning:active{background-color:#eb9316;border-color:#e38d13}.btn-warning.disabled,.btn-warning.disabled.active,.btn-warning.disabled.focus,.btn-warning.disabled:active,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled],.btn-warning[disabled].active,.btn-warning[disabled].focus,.btn-warning[disabled]:active,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning,fieldset[disabled] .btn-warning.active,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:active,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#eb9316;background-image:none}.btn-danger{background-image:-webkit-linear-gradient(top,#d9534f 0,#c12e2a 100%);background-image:-o-linear-gradient(top,#d9534f 0,#c12e2a 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#d9534f),to(#c12e2a));background-image:linear-gradient(to bottom,#d9534f 0,#c12e2a 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffd9534f', endColorstr='#ffc12e2a', GradientType=0);filter:progid:DXImageTransform.Microsoft.gradient(enabled=false);background-repeat:repeat-x;border-color:#b92c28}.btn-danger:focus,.btn-danger:hover{background-color:#c12e2a;background-position:0 -15px}.btn-danger.active,.btn-danger:active{background-color:#c12e2a;border-color:#b92c28}.btn-danger.disabled,.btn-danger.disabled.active,.btn-danger.disabled.focus,.btn-danger.disabled:active,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled],.btn-danger[disabled].active,.btn-danger[disabled].focus,.btn-danger[disabled]:active,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger,fieldset[disabled] .btn-danger.active,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:active,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#c12e2a;background-image:none}.img-thumbnail,.thumbnail{-webkit-box-shadow:0 1px 2px rgba(0,0,0,.075);box-shadow:0 1px 2px rgba(0,0,0,.075)}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{background-image:-webkit-linear-gradient(top,#f5f5f5 0,#e8e8e8 100%);background-image:-o-linear-gradient(top,#f5f5f5 0,#e8e8e8 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#f5f5f5),to(#e8e8e8));background-image:linear-gradient(to bottom,#f5f5f5 0,#e8e8e8 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff5f5f5', endColorstr='#ffe8e8e8', GradientType=0);background-repeat:repeat-x;background-color:#e8e8e8}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{background-image:-webkit-linear-gradient(top,#337ab7 0,#2e6da4 100%);background-image:-o-linear-gradient(top,#337ab7 0,#2e6da4 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#337ab7),to(#2e6da4));background-image:linear-gradient(to bottom,#337ab7 0,#2e6da4 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff337ab7', endColorstr='#ff2e6da4', GradientType=0);background-repeat:repeat-x;background-color:#2e6da4}.navbar-default{background-image:-webkit-linear-gradient(top,#fff 0,#f8f8f8 100%);background-image:-o-linear-gradient(top,#fff 0,#f8f8f8 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#fff),to(#f8f8f8));background-image:linear-gradient(to bottom,#fff 0,#f8f8f8 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffffffff', endColorstr='#fff8f8f8', GradientType=0);background-repeat:repeat-x;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false);border-radius:4px;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.15),0 1px 5px rgba(0,0,0,.075);box-shadow:inset 0 1px 0 rgba(255,255,255,.15),0 1px 5px rgba(0,0,0,.075)}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.open>a{background-image:-webkit-linear-gradient(top,#dbdbdb 0,#e2e2e2 100%);background-image:-o-linear-gradient(top,#dbdbdb 0,#e2e2e2 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#dbdbdb),to(#e2e2e2));background-image:linear-gradient(to bottom,#dbdbdb 0,#e2e2e2 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffdbdbdb', endColorstr='#ffe2e2e2', GradientType=0);background-repeat:repeat-x;-webkit-box-shadow:inset 0 3px 9px rgba(0,0,0,.075);box-shadow:inset 0 3px 9px rgba(0,0,0,.075)}.navbar-brand,.navbar-nav>li>a{text-shadow:0 1px 0 rgba(255,255,255,.25)}.navbar-inverse{background-image:-webkit-linear-gradient(top,#3c3c3c 0,#222 100%);background-image:-o-linear-gradient(top,#3c3c3c 0,#222 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#3c3c3c),to(#222));background-image:linear-gradient(to bottom,#3c3c3c 0,#222 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff3c3c3c', endColorstr='#ff222222', GradientType=0);background-repeat:repeat-x;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false);border-radius:4px}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.open>a{background-image:-webkit-linear-gradient(top,#080808 0,#0f0f0f 100%);background-image:-o-linear-gradient(top,#080808 0,#0f0f0f 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#080808),to(#0f0f0f));background-image:linear-gradient(to bottom,#080808 0,#0f0f0f 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff080808', endColorstr='#ff0f0f0f', GradientType=0);background-repeat:repeat-x;-webkit-box-shadow:inset 0 3px 9px rgba(0,0,0,.25);box-shadow:inset 0 3px 9px rgba(0,0,0,.25)}.navbar-inverse .navbar-brand,.navbar-inverse .navbar-nav>li>a{text-shadow:0 -1px 0 rgba(0,0,0,.25)}.navbar-fixed-bottom,.navbar-fixed-top,.navbar-static-top{border-radius:0}@media (max-width:767px){.navbar .navbar-nav .open .dropdown-menu>.active>a,.navbar .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-image:-webkit-linear-gradient(top,#337ab7 0,#2e6da4 100%);background-image:-o-linear-gradient(top,#337ab7 0,#2e6da4 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#337ab7),to(#2e6da4));background-image:linear-gradient(to bottom,#337ab7 0,#2e6da4 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff337ab7', endColorstr='#ff2e6da4', GradientType=0);background-repeat:repeat-x}}.alert{text-shadow:0 1px 0 rgba(255,255,255,.2);-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.25),0 1px 2px rgba(0,0,0,.05);box-shadow:inset 0 1px 0 rgba(255,255,255,.25),0 1px 2px rgba(0,0,0,.05)}.alert-success{background-image:-webkit-linear-gradient(top,#dff0d8 0,#c8e5bc 100%);background-image:-o-linear-gradient(top,#dff0d8 0,#c8e5bc 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#dff0d8),to(#c8e5bc));background-image:linear-gradient(to bottom,#dff0d8 0,#c8e5bc 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffdff0d8', endColorstr='#ffc8e5bc', GradientType=0);background-repeat:repeat-x;border-color:#b2dba1}.alert-info{background-image:-webkit-linear-gradient(top,#d9edf7 0,#b9def0 100%);background-image:-o-linear-gradient(top,#d9edf7 0,#b9def0 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#d9edf7),to(#b9def0));background-image:linear-gradient(to bottom,#d9edf7 0,#b9def0 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffd9edf7', endColorstr='#ffb9def0', GradientType=0);background-repeat:repeat-x;border-color:#9acfea}.alert-warning{background-image:-webkit-linear-gradient(top,#fcf8e3 0,#f8efc0 100%);background-image:-o-linear-gradient(top,#fcf8e3 0,#f8efc0 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#fcf8e3),to(#f8efc0));background-image:linear-gradient(to bottom,#fcf8e3 0,#f8efc0 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fffcf8e3', endColorstr='#fff8efc0', GradientType=0);background-repeat:repeat-x;border-color:#f5e79e}.alert-danger{background-image:-webkit-linear-gradient(top,#f2dede 0,#e7c3c3 100%);background-image:-o-linear-gradient(top,#f2dede 0,#e7c3c3 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#f2dede),to(#e7c3c3));background-image:linear-gradient(to bottom,#f2dede 0,#e7c3c3 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff2dede', endColorstr='#ffe7c3c3', GradientType=0);background-repeat:repeat-x;border-color:#dca7a7}.progress{background-image:-webkit-linear-gradient(top,#ebebeb 0,#f5f5f5 100%);background-image:-o-linear-gradient(top,#ebebeb 0,#f5f5f5 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#ebebeb),to(#f5f5f5));background-image:linear-gradient(to bottom,#ebebeb 0,#f5f5f5 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffebebeb', endColorstr='#fff5f5f5', GradientType=0);background-repeat:repeat-x}.progress-bar{background-image:-webkit-linear-gradient(top,#337ab7 0,#286090 100%);background-image:-o-linear-gradient(top,#337ab7 0,#286090 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#337ab7),to(#286090));background-image:linear-gradient(to bottom,#337ab7 0,#286090 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff337ab7', endColorstr='#ff286090', GradientType=0);background-repeat:repeat-x}.progress-bar-success{background-image:-webkit-linear-gradient(top,#5cb85c 0,#449d44 100%);background-image:-o-linear-gradient(top,#5cb85c 0,#449d44 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#5cb85c),to(#449d44));background-image:linear-gradient(to bottom,#5cb85c 0,#449d44 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff5cb85c', endColorstr='#ff449d44', GradientType=0);background-repeat:repeat-x}.progress-bar-info{background-image:-webkit-linear-gradient(top,#5bc0de 0,#31b0d5 100%);background-image:-o-linear-gradient(top,#5bc0de 0,#31b0d5 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#5bc0de),to(#31b0d5));background-image:linear-gradient(to bottom,#5bc0de 0,#31b0d5 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff5bc0de', endColorstr='#ff31b0d5', GradientType=0);background-repeat:repeat-x}.progress-bar-warning{background-image:-webkit-linear-gradient(top,#f0ad4e 0,#ec971f 100%);background-image:-o-linear-gradient(top,#f0ad4e 0,#ec971f 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#f0ad4e),to(#ec971f));background-image:linear-gradient(to bottom,#f0ad4e 0,#ec971f 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff0ad4e', endColorstr='#ffec971f', GradientType=0);background-repeat:repeat-x}.progress-bar-danger{background-image:-webkit-linear-gradient(top,#d9534f 0,#c9302c 100%);background-image:-o-linear-gradient(top,#d9534f 0,#c9302c 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#d9534f),to(#c9302c));background-image:linear-gradient(to bottom,#d9534f 0,#c9302c 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffd9534f', endColorstr='#ffc9302c', GradientType=0);background-repeat:repeat-x}.progress-bar-striped{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.list-group{border-radius:4px;-webkit-box-shadow:0 1px 2px rgba(0,0,0,.075);box-shadow:0 1px 2px rgba(0,0,0,.075)}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{text-shadow:0 -1px 0 #286090;background-image:-webkit-linear-gradient(top,#337ab7 0,#2b669a 100%);background-image:-o-linear-gradient(top,#337ab7 0,#2b669a 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#337ab7),to(#2b669a));background-image:linear-gradient(to bottom,#337ab7 0,#2b669a 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff337ab7', endColorstr='#ff2b669a', GradientType=0);background-repeat:repeat-x;border-color:#2b669a}.list-group-item.active .badge,.list-group-item.active:focus .badge,.list-group-item.active:hover .badge{text-shadow:none}.panel{-webkit-box-shadow:0 1px 2px rgba(0,0,0,.05);box-shadow:0 1px 2px rgba(0,0,0,.05)}.panel-default>.panel-heading{background-image:-webkit-linear-gradient(top,#f5f5f5 0,#e8e8e8 100%);background-image:-o-linear-gradient(top,#f5f5f5 0,#e8e8e8 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#f5f5f5),to(#e8e8e8));background-image:linear-gradient(to bottom,#f5f5f5 0,#e8e8e8 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff5f5f5', endColorstr='#ffe8e8e8', GradientType=0);background-repeat:repeat-x}.panel-primary>.panel-heading{background-image:-webkit-linear-gradient(top,#337ab7 0,#2e6da4 100%);background-image:-o-linear-gradient(top,#337ab7 0,#2e6da4 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#337ab7),to(#2e6da4));background-image:linear-gradient(to bottom,#337ab7 0,#2e6da4 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff337ab7', endColorstr='#ff2e6da4', GradientType=0);background-repeat:repeat-x}.panel-success>.panel-heading{background-image:-webkit-linear-gradient(top,#dff0d8 0,#d0e9c6 100%);background-image:-o-linear-gradient(top,#dff0d8 0,#d0e9c6 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#dff0d8),to(#d0e9c6));background-image:linear-gradient(to bottom,#dff0d8 0,#d0e9c6 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffdff0d8', endColorstr='#ffd0e9c6', GradientType=0);background-repeat:repeat-x}.panel-info>.panel-heading{background-image:-webkit-linear-gradient(top,#d9edf7 0,#c4e3f3 100%);background-image:-o-linear-gradient(top,#d9edf7 0,#c4e3f3 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#d9edf7),to(#c4e3f3));background-image:linear-gradient(to bottom,#d9edf7 0,#c4e3f3 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffd9edf7', endColorstr='#ffc4e3f3', GradientType=0);background-repeat:repeat-x}.panel-warning>.panel-heading{background-image:-webkit-linear-gradient(top,#fcf8e3 0,#faf2cc 100%);background-image:-o-linear-gradient(top,#fcf8e3 0,#faf2cc 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#fcf8e3),to(#faf2cc));background-image:linear-gradient(to bottom,#fcf8e3 0,#faf2cc 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fffcf8e3', endColorstr='#fffaf2cc', GradientType=0);background-repeat:repeat-x}.panel-danger>.panel-heading{background-image:-webkit-linear-gradient(top,#f2dede 0,#ebcccc 100%);background-image:-o-linear-gradient(top,#f2dede 0,#ebcccc 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#f2dede),to(#ebcccc));background-image:linear-gradient(to bottom,#f2dede 0,#ebcccc 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fff2dede', endColorstr='#ffebcccc', GradientType=0);background-repeat:repeat-x}.well{background-image:-webkit-linear-gradient(top,#e8e8e8 0,#f5f5f5 100%);background-image:-o-linear-gradient(top,#e8e8e8 0,#f5f5f5 100%);background-image:-webkit-gradient(linear,left top,left bottom,from(#e8e8e8),to(#f5f5f5));background-image:linear-gradient(to bottom,#e8e8e8 0,#f5f5f5 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffe8e8e8', endColorstr='#fff5f5f5', GradientType=0);background-repeat:repeat-x;border-color:#dcdcdc;-webkit-box-shadow:inset 0 1px 3px rgba(0,0,0,.05),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 3px rgba(0,0,0,.05),0 1px 0 rgba(255,255,255,.1)}
+/*# sourceMappingURL=bootstrap-theme.min.css.map */
```

### Comparing `yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/css/bootstrap.css` & `yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 /*!
- * Bootstrap v3.2.0 (http://getbootstrap.com)
- * Copyright 2011-2014 Twitter, Inc.
+ * Bootstrap v3.4.1 (https://getbootstrap.com/)
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  */
-
-/*! normalize.css v3.0.1 | MIT License | git.io/normalize */
+/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
 html {
   font-family: sans-serif;
+  -ms-text-size-adjust: 100%;
   -webkit-text-size-adjust: 100%;
-      -ms-text-size-adjust: 100%;
 }
 body {
   margin: 0;
 }
 article,
 aside,
 details,
 figcaption,
 figure,
 footer,
 header,
 hgroup,
 main,
+menu,
 nav,
 section,
 summary {
   display: block;
 }
 audio,
 canvas,
@@ -39,68 +39,72 @@
   height: 0;
 }
 [hidden],
 template {
   display: none;
 }
 a {
-  background: transparent;
+  background-color: transparent;
 }
 a:active,
 a:hover {
   outline: 0;
 }
 abbr[title] {
-  border-bottom: 1px dotted;
+  border-bottom: none;
+  text-decoration: underline;
+  -webkit-text-decoration: underline dotted;
+  -moz-text-decoration: underline dotted;
+  text-decoration: underline dotted;
 }
 b,
 strong {
   font-weight: bold;
 }
 dfn {
   font-style: italic;
 }
 h1 {
-  margin: .67em 0;
   font-size: 2em;
+  margin: 0.67em 0;
 }
 mark {
-  color: #000;
   background: #ff0;
+  color: #000;
 }
 small {
   font-size: 80%;
 }
 sub,
 sup {
-  position: relative;
   font-size: 75%;
   line-height: 0;
+  position: relative;
   vertical-align: baseline;
 }
 sup {
-  top: -.5em;
+  top: -0.5em;
 }
 sub {
-  bottom: -.25em;
+  bottom: -0.25em;
 }
 img {
   border: 0;
 }
 svg:not(:root) {
   overflow: hidden;
 }
 figure {
   margin: 1em 40px;
 }
 hr {
-  height: 0;
   -webkit-box-sizing: content-box;
-     -moz-box-sizing: content-box;
-          box-sizing: content-box;
+  -moz-box-sizing: content-box;
+  box-sizing: content-box;
+  height: 0;
 }
 pre {
   overflow: auto;
 }
 code,
 kbd,
 pre,
@@ -109,17 +113,17 @@
   font-size: 1em;
 }
 button,
 input,
 optgroup,
 select,
 textarea {
-  margin: 0;
-  font: inherit;
   color: inherit;
+  font: inherit;
+  margin: 0;
 }
 button {
   overflow: visible;
 }
 button,
 select {
   text-transform: none;
@@ -133,90 +137,92 @@
 }
 button[disabled],
 html input[disabled] {
   cursor: default;
 }
 button::-moz-focus-inner,
 input::-moz-focus-inner {
-  padding: 0;
   border: 0;
+  padding: 0;
 }
 input {
   line-height: normal;
 }
 input[type="checkbox"],
 input[type="radio"] {
   -webkit-box-sizing: border-box;
-     -moz-box-sizing: border-box;
-          box-sizing: border-box;
+  -moz-box-sizing: border-box;
+  box-sizing: border-box;
   padding: 0;
 }
 input[type="number"]::-webkit-inner-spin-button,
 input[type="number"]::-webkit-outer-spin-button {
   height: auto;
 }
 input[type="search"] {
-  -webkit-box-sizing: content-box;
-     -moz-box-sizing: content-box;
-          box-sizing: content-box;
   -webkit-appearance: textfield;
+  -webkit-box-sizing: content-box;
+  -moz-box-sizing: content-box;
+  box-sizing: content-box;
 }
 input[type="search"]::-webkit-search-cancel-button,
 input[type="search"]::-webkit-search-decoration {
   -webkit-appearance: none;
 }
 fieldset {
-  padding: .35em .625em .75em;
-  margin: 0 2px;
   border: 1px solid #c0c0c0;
+  margin: 0 2px;
+  padding: 0.35em 0.625em 0.75em;
 }
 legend {
-  padding: 0;
   border: 0;
+  padding: 0;
 }
 textarea {
   overflow: auto;
 }
 optgroup {
   font-weight: bold;
 }
 table {
-  border-spacing: 0;
   border-collapse: collapse;
+  border-spacing: 0;
 }
 td,
 th {
   padding: 0;
 }
+/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
 @media print {
-  * {
+  *,
+  *:before,
+  *:after {
     color: #000 !important;
     text-shadow: none !important;
     background: transparent !important;
     -webkit-box-shadow: none !important;
-            box-shadow: none !important;
+    box-shadow: none !important;
   }
   a,
   a:visited {
     text-decoration: underline;
   }
   a[href]:after {
     content: " (" attr(href) ")";
   }
   abbr[title]:after {
     content: " (" attr(title) ")";
   }
-  a[href^="javascript:"]:after,
-  a[href^="#"]:after {
+  a[href^="#"]:after,
+  a[href^="javascript:"]:after {
     content: "";
   }
   pre,
   blockquote {
     border: 1px solid #999;
-
     page-break-inside: avoid;
   }
   thead {
     display: table-header-group;
   }
   tr,
   img {
@@ -231,64 +237,60 @@
     orphans: 3;
     widows: 3;
   }
   h2,
   h3 {
     page-break-after: avoid;
   }
-  select {
-    background: #fff !important;
-  }
   .navbar {
     display: none;
   }
-  .table td,
-  .table th {
-    background-color: #fff !important;
-  }
   .btn > .caret,
   .dropup > .btn > .caret {
     border-top-color: #000 !important;
   }
   .label {
     border: 1px solid #000;
   }
   .table {
     border-collapse: collapse !important;
   }
+  .table td,
+  .table th {
+    background-color: #fff !important;
+  }
   .table-bordered th,
   .table-bordered td {
     border: 1px solid #ddd !important;
   }
 }
 @font-face {
-  font-family: 'Glyphicons Halflings';
-
-  src: url('../fonts/glyphicons-halflings-regular.eot');
-  src: url('../fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../fonts/glyphicons-halflings-regular.woff') format('woff'), url('../fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
+  font-family: "Glyphicons Halflings";
+  src: url("../fonts/glyphicons-halflings-regular.eot");
+  src: url("../fonts/glyphicons-halflings-regular.eot?#iefix") format("embedded-opentype"), url("../fonts/glyphicons-halflings-regular.woff2") format("woff2"), url("../fonts/glyphicons-halflings-regular.woff") format("woff"), url("../fonts/glyphicons-halflings-regular.ttf") format("truetype"), url("../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular") format("svg");
 }
 .glyphicon {
   position: relative;
   top: 1px;
   display: inline-block;
-  font-family: 'Glyphicons Halflings';
+  font-family: "Glyphicons Halflings";
   font-style: normal;
-  font-weight: normal;
+  font-weight: 400;
   line-height: 1;
-
   -webkit-font-smoothing: antialiased;
   -moz-osx-font-smoothing: grayscale;
 }
 .glyphicon-asterisk:before {
-  content: "\2a";
+  content: "\002a";
 }
 .glyphicon-plus:before {
-  content: "\2b";
+  content: "\002b";
 }
-.glyphicon-euro:before {
+.glyphicon-euro:before,
+.glyphicon-eur:before {
   content: "\20ac";
 }
 .glyphicon-minus:before {
   content: "\2212";
 }
 .glyphicon-cloud:before {
   content: "\2601";
@@ -874,56 +876,240 @@
 }
 .glyphicon-tree-conifer:before {
   content: "\e199";
 }
 .glyphicon-tree-deciduous:before {
   content: "\e200";
 }
+.glyphicon-cd:before {
+  content: "\e201";
+}
+.glyphicon-save-file:before {
+  content: "\e202";
+}
+.glyphicon-open-file:before {
+  content: "\e203";
+}
+.glyphicon-level-up:before {
+  content: "\e204";
+}
+.glyphicon-copy:before {
+  content: "\e205";
+}
+.glyphicon-paste:before {
+  content: "\e206";
+}
+.glyphicon-alert:before {
+  content: "\e209";
+}
+.glyphicon-equalizer:before {
+  content: "\e210";
+}
+.glyphicon-king:before {
+  content: "\e211";
+}
+.glyphicon-queen:before {
+  content: "\e212";
+}
+.glyphicon-pawn:before {
+  content: "\e213";
+}
+.glyphicon-bishop:before {
+  content: "\e214";
+}
+.glyphicon-knight:before {
+  content: "\e215";
+}
+.glyphicon-baby-formula:before {
+  content: "\e216";
+}
+.glyphicon-tent:before {
+  content: "\26fa";
+}
+.glyphicon-blackboard:before {
+  content: "\e218";
+}
+.glyphicon-bed:before {
+  content: "\e219";
+}
+.glyphicon-apple:before {
+  content: "\f8ff";
+}
+.glyphicon-erase:before {
+  content: "\e221";
+}
+.glyphicon-hourglass:before {
+  content: "\231b";
+}
+.glyphicon-lamp:before {
+  content: "\e223";
+}
+.glyphicon-duplicate:before {
+  content: "\e224";
+}
+.glyphicon-piggy-bank:before {
+  content: "\e225";
+}
+.glyphicon-scissors:before {
+  content: "\e226";
+}
+.glyphicon-bitcoin:before {
+  content: "\e227";
+}
+.glyphicon-btc:before {
+  content: "\e227";
+}
+.glyphicon-xbt:before {
+  content: "\e227";
+}
+.glyphicon-yen:before {
+  content: "\00a5";
+}
+.glyphicon-jpy:before {
+  content: "\00a5";
+}
+.glyphicon-ruble:before {
+  content: "\20bd";
+}
+.glyphicon-rub:before {
+  content: "\20bd";
+}
+.glyphicon-scale:before {
+  content: "\e230";
+}
+.glyphicon-ice-lolly:before {
+  content: "\e231";
+}
+.glyphicon-ice-lolly-tasted:before {
+  content: "\e232";
+}
+.glyphicon-education:before {
+  content: "\e233";
+}
+.glyphicon-option-horizontal:before {
+  content: "\e234";
+}
+.glyphicon-option-vertical:before {
+  content: "\e235";
+}
+.glyphicon-menu-hamburger:before {
+  content: "\e236";
+}
+.glyphicon-modal-window:before {
+  content: "\e237";
+}
+.glyphicon-oil:before {
+  content: "\e238";
+}
+.glyphicon-grain:before {
+  content: "\e239";
+}
+.glyphicon-sunglasses:before {
+  content: "\e240";
+}
+.glyphicon-text-size:before {
+  content: "\e241";
+}
+.glyphicon-text-color:before {
+  content: "\e242";
+}
+.glyphicon-text-background:before {
+  content: "\e243";
+}
+.glyphicon-object-align-top:before {
+  content: "\e244";
+}
+.glyphicon-object-align-bottom:before {
+  content: "\e245";
+}
+.glyphicon-object-align-horizontal:before {
+  content: "\e246";
+}
+.glyphicon-object-align-left:before {
+  content: "\e247";
+}
+.glyphicon-object-align-vertical:before {
+  content: "\e248";
+}
+.glyphicon-object-align-right:before {
+  content: "\e249";
+}
+.glyphicon-triangle-right:before {
+  content: "\e250";
+}
+.glyphicon-triangle-left:before {
+  content: "\e251";
+}
+.glyphicon-triangle-bottom:before {
+  content: "\e252";
+}
+.glyphicon-triangle-top:before {
+  content: "\e253";
+}
+.glyphicon-console:before {
+  content: "\e254";
+}
+.glyphicon-superscript:before {
+  content: "\e255";
+}
+.glyphicon-subscript:before {
+  content: "\e256";
+}
+.glyphicon-menu-left:before {
+  content: "\e257";
+}
+.glyphicon-menu-right:before {
+  content: "\e258";
+}
+.glyphicon-menu-down:before {
+  content: "\e259";
+}
+.glyphicon-menu-up:before {
+  content: "\e260";
+}
 * {
   -webkit-box-sizing: border-box;
-     -moz-box-sizing: border-box;
-          box-sizing: border-box;
+  -moz-box-sizing: border-box;
+  box-sizing: border-box;
 }
 *:before,
 *:after {
   -webkit-box-sizing: border-box;
-     -moz-box-sizing: border-box;
-          box-sizing: border-box;
+  -moz-box-sizing: border-box;
+  box-sizing: border-box;
 }
 html {
   font-size: 10px;
-
   -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
 }
 body {
   font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
   font-size: 14px;
   line-height: 1.42857143;
-  color: #333;
+  color: #333333;
   background-color: #fff;
 }
 input,
 button,
 select,
 textarea {
   font-family: inherit;
   font-size: inherit;
   line-height: inherit;
 }
 a {
-  color: #428bca;
+  color: #337ab7;
   text-decoration: none;
 }
 a:hover,
 a:focus {
-  color: #2a6496;
+  color: #23527c;
   text-decoration: underline;
 }
 a:focus {
-  outline: thin dotted;
   outline: 5px auto -webkit-focus-ring-color;
   outline-offset: -2px;
 }
 figure {
   margin: 0;
 }
 img {
@@ -931,43 +1117,41 @@
 }
 .img-responsive,
 .thumbnail > img,
 .thumbnail a > img,
 .carousel-inner > .item > img,
 .carousel-inner > .item > a > img {
   display: block;
-  width: 100% \9;
   max-width: 100%;
   height: auto;
 }
 .img-rounded {
   border-radius: 6px;
 }
 .img-thumbnail {
-  display: inline-block;
-  width: 100% \9;
-  max-width: 100%;
-  height: auto;
   padding: 4px;
   line-height: 1.42857143;
   background-color: #fff;
   border: 1px solid #ddd;
   border-radius: 4px;
-  -webkit-transition: all .2s ease-in-out;
-       -o-transition: all .2s ease-in-out;
-          transition: all .2s ease-in-out;
+  -webkit-transition: all 0.2s ease-in-out;
+  -o-transition: all 0.2s ease-in-out;
+  transition: all 0.2s ease-in-out;
+  display: inline-block;
+  max-width: 100%;
+  height: auto;
 }
 .img-circle {
   border-radius: 50%;
 }
 hr {
   margin-top: 20px;
   margin-bottom: 20px;
   border: 0;
-  border-top: 1px solid #eee;
+  border-top: 1px solid #eeeeee;
 }
 .sr-only {
   position: absolute;
   width: 1px;
   height: 1px;
   padding: 0;
   margin: -1px;
@@ -980,14 +1164,17 @@
   position: static;
   width: auto;
   height: auto;
   margin: 0;
   overflow: visible;
   clip: auto;
 }
+[role="button"] {
+  cursor: pointer;
+}
 h1,
 h2,
 h3,
 h4,
 h5,
 h6,
 .h1,
@@ -1021,17 +1208,17 @@
 h6 .small,
 .h1 .small,
 .h2 .small,
 .h3 .small,
 .h4 .small,
 .h5 .small,
 .h6 .small {
-  font-weight: normal;
+  font-weight: 400;
   line-height: 1;
-  color: #777;
+  color: #777777;
 }
 h1,
 .h1,
 h2,
 .h2,
 h3,
 .h3 {
@@ -1113,20 +1300,17 @@
     font-size: 21px;
   }
 }
 small,
 .small {
   font-size: 85%;
 }
-cite {
-  font-style: normal;
-}
 mark,
 .mark {
-  padding: .2em;
+  padding: 0.2em;
   background-color: #fcf8e3;
 }
 .text-left {
   text-align: left;
 }
 .text-right {
   text-align: right;
@@ -1146,81 +1330,91 @@
 .text-uppercase {
   text-transform: uppercase;
 }
 .text-capitalize {
   text-transform: capitalize;
 }
 .text-muted {
-  color: #777;
+  color: #777777;
 }
 .text-primary {
-  color: #428bca;
+  color: #337ab7;
 }
-a.text-primary:hover {
-  color: #3071a9;
+a.text-primary:hover,
+a.text-primary:focus {
+  color: #286090;
 }
 .text-success {
   color: #3c763d;
 }
-a.text-success:hover {
+a.text-success:hover,
+a.text-success:focus {
   color: #2b542c;
 }
 .text-info {
   color: #31708f;
 }
-a.text-info:hover {
+a.text-info:hover,
+a.text-info:focus {
   color: #245269;
 }
 .text-warning {
   color: #8a6d3b;
 }
-a.text-warning:hover {
+a.text-warning:hover,
+a.text-warning:focus {
   color: #66512c;
 }
 .text-danger {
   color: #a94442;
 }
-a.text-danger:hover {
+a.text-danger:hover,
+a.text-danger:focus {
   color: #843534;
 }
 .bg-primary {
   color: #fff;
-  background-color: #428bca;
+  background-color: #337ab7;
 }
-a.bg-primary:hover {
-  background-color: #3071a9;
+a.bg-primary:hover,
+a.bg-primary:focus {
+  background-color: #286090;
 }
 .bg-success {
   background-color: #dff0d8;
 }
-a.bg-success:hover {
+a.bg-success:hover,
+a.bg-success:focus {
   background-color: #c1e2b3;
 }
 .bg-info {
   background-color: #d9edf7;
 }
-a.bg-info:hover {
+a.bg-info:hover,
+a.bg-info:focus {
   background-color: #afd9ee;
 }
 .bg-warning {
   background-color: #fcf8e3;
 }
-a.bg-warning:hover {
+a.bg-warning:hover,
+a.bg-warning:focus {
   background-color: #f7ecb5;
 }
 .bg-danger {
   background-color: #f2dede;
 }
-a.bg-danger:hover {
+a.bg-danger:hover,
+a.bg-danger:focus {
   background-color: #e4b9b9;
 }
 .page-header {
   padding-bottom: 9px;
   margin: 40px 0 20px;
-  border-bottom: 1px solid #eee;
+  border-bottom: 1px solid #eeeeee;
 }
 ul,
 ol {
   margin-top: 0;
   margin-bottom: 10px;
 }
 ul ul,
@@ -1231,16 +1425,16 @@
 }
 .list-unstyled {
   padding-left: 0;
   list-style: none;
 }
 .list-inline {
   padding-left: 0;
-  margin-left: -5px;
   list-style: none;
+  margin-left: -5px;
 }
 .list-inline > li {
   display: inline-block;
   padding-right: 5px;
   padding-left: 5px;
 }
 dl {
@@ -1248,93 +1442,88 @@
   margin-bottom: 20px;
 }
 dt,
 dd {
   line-height: 1.42857143;
 }
 dt {
-  font-weight: bold;
+  font-weight: 700;
 }
 dd {
   margin-left: 0;
 }
 @media (min-width: 768px) {
   .dl-horizontal dt {
     float: left;
     width: 160px;
-    overflow: hidden;
     clear: left;
     text-align: right;
+    overflow: hidden;
     text-overflow: ellipsis;
     white-space: nowrap;
   }
   .dl-horizontal dd {
     margin-left: 180px;
   }
 }
 abbr[title],
 abbr[data-original-title] {
   cursor: help;
-  border-bottom: 1px dotted #777;
 }
 .initialism {
   font-size: 90%;
   text-transform: uppercase;
 }
 blockquote {
   padding: 10px 20px;
   margin: 0 0 20px;
   font-size: 17.5px;
-  border-left: 5px solid #eee;
+  border-left: 5px solid #eeeeee;
 }
 blockquote p:last-child,
 blockquote ul:last-child,
 blockquote ol:last-child {
   margin-bottom: 0;
 }
 blockquote footer,
 blockquote small,
 blockquote .small {
   display: block;
   font-size: 80%;
   line-height: 1.42857143;
-  color: #777;
+  color: #777777;
 }
 blockquote footer:before,
 blockquote small:before,
 blockquote .small:before {
-  content: '\2014 \00A0';
+  content: "\2014 \00A0";
 }
 .blockquote-reverse,
 blockquote.pull-right {
   padding-right: 15px;
   padding-left: 0;
   text-align: right;
-  border-right: 5px solid #eee;
+  border-right: 5px solid #eeeeee;
   border-left: 0;
 }
 .blockquote-reverse footer:before,
 blockquote.pull-right footer:before,
 .blockquote-reverse small:before,
 blockquote.pull-right small:before,
 .blockquote-reverse .small:before,
 blockquote.pull-right .small:before {
-  content: '';
+  content: "";
 }
 .blockquote-reverse footer:after,
 blockquote.pull-right footer:after,
 .blockquote-reverse small:after,
 blockquote.pull-right small:after,
 .blockquote-reverse .small:after,
 blockquote.pull-right .small:after {
-  content: '\00A0 \2014';
-}
-blockquote:before,
-blockquote:after {
-  content: "";
+  content: "\00A0 \2014";
 }
 address {
   margin-bottom: 20px;
   font-style: normal;
   line-height: 1.42857143;
 }
 code,
@@ -1352,30 +1541,31 @@
 }
 kbd {
   padding: 2px 4px;
   font-size: 90%;
   color: #fff;
   background-color: #333;
   border-radius: 3px;
-  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, .25);
-          box-shadow: inset 0 -1px 0 rgba(0, 0, 0, .25);
+  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
+  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
 }
 kbd kbd {
   padding: 0;
   font-size: 100%;
+  font-weight: 700;
   -webkit-box-shadow: none;
-          box-shadow: none;
+  box-shadow: none;
 }
 pre {
   display: block;
   padding: 9.5px;
   margin: 0 0 10px;
   font-size: 13px;
   line-height: 1.42857143;
-  color: #333;
+  color: #333333;
   word-break: break-all;
   word-wrap: break-word;
   background-color: #f5f5f5;
   border: 1px solid #ccc;
   border-radius: 4px;
 }
 pre code {
@@ -1417,21 +1607,87 @@
   margin-right: auto;
   margin-left: auto;
 }
 .row {
   margin-right: -15px;
   margin-left: -15px;
 }
-.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
+.row-no-gutters {
+  margin-right: 0;
+  margin-left: 0;
+}
+.row-no-gutters [class*="col-"] {
+  padding-right: 0;
+  padding-left: 0;
+}
+.col-xs-1,
+.col-sm-1,
+.col-md-1,
+.col-lg-1,
+.col-xs-2,
+.col-sm-2,
+.col-md-2,
+.col-lg-2,
+.col-xs-3,
+.col-sm-3,
+.col-md-3,
+.col-lg-3,
+.col-xs-4,
+.col-sm-4,
+.col-md-4,
+.col-lg-4,
+.col-xs-5,
+.col-sm-5,
+.col-md-5,
+.col-lg-5,
+.col-xs-6,
+.col-sm-6,
+.col-md-6,
+.col-lg-6,
+.col-xs-7,
+.col-sm-7,
+.col-md-7,
+.col-lg-7,
+.col-xs-8,
+.col-sm-8,
+.col-md-8,
+.col-lg-8,
+.col-xs-9,
+.col-sm-9,
+.col-md-9,
+.col-lg-9,
+.col-xs-10,
+.col-sm-10,
+.col-md-10,
+.col-lg-10,
+.col-xs-11,
+.col-sm-11,
+.col-md-11,
+.col-lg-11,
+.col-xs-12,
+.col-sm-12,
+.col-md-12,
+.col-lg-12 {
   position: relative;
   min-height: 1px;
   padding-right: 15px;
   padding-left: 15px;
 }
-.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
+.col-xs-1,
+.col-xs-2,
+.col-xs-3,
+.col-xs-4,
+.col-xs-5,
+.col-xs-6,
+.col-xs-7,
+.col-xs-8,
+.col-xs-9,
+.col-xs-10,
+.col-xs-11,
+.col-xs-12 {
   float: left;
 }
 .col-xs-12 {
   width: 100%;
 }
 .col-xs-11 {
   width: 91.66666667%;
@@ -1577,18 +1833,29 @@
 .col-xs-offset-2 {
   margin-left: 16.66666667%;
 }
 .col-xs-offset-1 {
   margin-left: 8.33333333%;
 }
 .col-xs-offset-0 {
-  margin-left: 0;
+  margin-left: 0%;
 }
 @media (min-width: 768px) {
-  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
+  .col-sm-1,
+  .col-sm-2,
+  .col-sm-3,
+  .col-sm-4,
+  .col-sm-5,
+  .col-sm-6,
+  .col-sm-7,
+  .col-sm-8,
+  .col-sm-9,
+  .col-sm-10,
+  .col-sm-11,
+  .col-sm-12 {
     float: left;
   }
   .col-sm-12 {
     width: 100%;
   }
   .col-sm-11 {
     width: 91.66666667%;
@@ -1734,19 +2001,30 @@
   .col-sm-offset-2 {
     margin-left: 16.66666667%;
   }
   .col-sm-offset-1 {
     margin-left: 8.33333333%;
   }
   .col-sm-offset-0 {
-    margin-left: 0;
+    margin-left: 0%;
   }
 }
 @media (min-width: 992px) {
-  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
+  .col-md-1,
+  .col-md-2,
+  .col-md-3,
+  .col-md-4,
+  .col-md-5,
+  .col-md-6,
+  .col-md-7,
+  .col-md-8,
+  .col-md-9,
+  .col-md-10,
+  .col-md-11,
+  .col-md-12 {
     float: left;
   }
   .col-md-12 {
     width: 100%;
   }
   .col-md-11 {
     width: 91.66666667%;
@@ -1892,19 +2170,30 @@
   .col-md-offset-2 {
     margin-left: 16.66666667%;
   }
   .col-md-offset-1 {
     margin-left: 8.33333333%;
   }
   .col-md-offset-0 {
-    margin-left: 0;
+    margin-left: 0%;
   }
 }
 @media (min-width: 1200px) {
-  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
+  .col-lg-1,
+  .col-lg-2,
+  .col-lg-3,
+  .col-lg-4,
+  .col-lg-5,
+  .col-lg-6,
+  .col-lg-7,
+  .col-lg-8,
+  .col-lg-9,
+  .col-lg-10,
+  .col-lg-11,
+  .col-lg-12 {
     float: left;
   }
   .col-lg-12 {
     width: 100%;
   }
   .col-lg-11 {
     width: 91.66666667%;
@@ -2050,20 +2339,37 @@
   .col-lg-offset-2 {
     margin-left: 16.66666667%;
   }
   .col-lg-offset-1 {
     margin-left: 8.33333333%;
   }
   .col-lg-offset-0 {
-    margin-left: 0;
+    margin-left: 0%;
   }
 }
 table {
   background-color: transparent;
 }
+table col[class*="col-"] {
+  position: static;
+  display: table-column;
+  float: none;
+}
+table td[class*="col-"],
+table th[class*="col-"] {
+  position: static;
+  display: table-cell;
+  float: none;
+}
+caption {
+  padding-top: 8px;
+  padding-bottom: 8px;
+  color: #777777;
+  text-align: left;
+}
 th {
   text-align: left;
 }
 .table {
   width: 100%;
   max-width: 100%;
   margin-bottom: 20px;
@@ -2116,33 +2422,20 @@
 .table-bordered > tfoot > tr > td {
   border: 1px solid #ddd;
 }
 .table-bordered > thead > tr > th,
 .table-bordered > thead > tr > td {
   border-bottom-width: 2px;
 }
-.table-striped > tbody > tr:nth-child(odd) > td,
-.table-striped > tbody > tr:nth-child(odd) > th {
+.table-striped > tbody > tr:nth-of-type(odd) {
   background-color: #f9f9f9;
 }
-.table-hover > tbody > tr:hover > td,
-.table-hover > tbody > tr:hover > th {
+.table-hover > tbody > tr:hover {
   background-color: #f5f5f5;
 }
-table col[class*="col-"] {
-  position: static;
-  display: table-column;
-  float: none;
-}
-table td[class*="col-"],
-table th[class*="col-"] {
-  position: static;
-  display: table-cell;
-  float: none;
-}
 .table > thead > tr > td.active,
 .table > tbody > tr > td.active,
 .table > tfoot > tr > td.active,
 .table > thead > tr > th.active,
 .table > tbody > tr > th.active,
 .table > tfoot > tr > th.active,
 .table > thead > tr.active > td,
@@ -2240,21 +2533,23 @@
 .table-hover > tbody > tr > td.danger:hover,
 .table-hover > tbody > tr > th.danger:hover,
 .table-hover > tbody > tr.danger:hover > td,
 .table-hover > tbody > tr:hover > .danger,
 .table-hover > tbody > tr.danger:hover > th {
   background-color: #ebcccc;
 }
+.table-responsive {
+  min-height: 0.01%;
+  overflow-x: auto;
+}
 @media screen and (max-width: 767px) {
   .table-responsive {
     width: 100%;
     margin-bottom: 15px;
-    overflow-x: auto;
     overflow-y: hidden;
-    -webkit-overflow-scrolling: touch;
     -ms-overflow-style: -ms-autohiding-scrollbar;
     border: 1px solid #ddd;
   }
   .table-responsive > .table {
     margin-bottom: 0;
   }
   .table-responsive > .table > thead > tr > th,
@@ -2300,142 +2595,174 @@
 legend {
   display: block;
   width: 100%;
   padding: 0;
   margin-bottom: 20px;
   font-size: 21px;
   line-height: inherit;
-  color: #333;
+  color: #333333;
   border: 0;
   border-bottom: 1px solid #e5e5e5;
 }
 label {
   display: inline-block;
   max-width: 100%;
   margin-bottom: 5px;
-  font-weight: bold;
+  font-weight: 700;
 }
 input[type="search"] {
   -webkit-box-sizing: border-box;
-     -moz-box-sizing: border-box;
-          box-sizing: border-box;
+  -moz-box-sizing: border-box;
+  box-sizing: border-box;
+  -webkit-appearance: none;
+  -moz-appearance: none;
+  appearance: none;
 }
 input[type="radio"],
 input[type="checkbox"] {
   margin: 4px 0 0;
   margin-top: 1px \9;
   line-height: normal;
 }
+input[type="radio"][disabled],
+input[type="checkbox"][disabled],
+input[type="radio"].disabled,
+input[type="checkbox"].disabled,
+fieldset[disabled] input[type="radio"],
+fieldset[disabled] input[type="checkbox"] {
+  cursor: not-allowed;
+}
 input[type="file"] {
   display: block;
 }
 input[type="range"] {
   display: block;
   width: 100%;
 }
 select[multiple],
 select[size] {
   height: auto;
 }
 input[type="file"]:focus,
 input[type="radio"]:focus,
 input[type="checkbox"]:focus {
-  outline: thin dotted;
   outline: 5px auto -webkit-focus-ring-color;
   outline-offset: -2px;
 }
 output {
   display: block;
   padding-top: 7px;
   font-size: 14px;
   line-height: 1.42857143;
-  color: #555;
+  color: #555555;
 }
 .form-control {
   display: block;
   width: 100%;
   height: 34px;
   padding: 6px 12px;
   font-size: 14px;
   line-height: 1.42857143;
-  color: #555;
+  color: #555555;
   background-color: #fff;
   background-image: none;
   border: 1px solid #ccc;
   border-radius: 4px;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075);
-          box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075);
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
+  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
+  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
   -webkit-transition: border-color ease-in-out .15s, -webkit-box-shadow ease-in-out .15s;
-       -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
-          transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
+  transition: border-color ease-in-out .15s, -webkit-box-shadow ease-in-out .15s;
+  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
+  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s, -webkit-box-shadow ease-in-out .15s;
 }
 .form-control:focus {
   border-color: #66afe9;
   outline: 0;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, .6);
-          box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, .6);
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 8px rgba(102, 175, 233, 0.6);
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 8px rgba(102, 175, 233, 0.6);
 }
 .form-control::-moz-placeholder {
-  color: #777;
+  color: #999;
   opacity: 1;
 }
 .form-control:-ms-input-placeholder {
-  color: #777;
+  color: #999;
 }
 .form-control::-webkit-input-placeholder {
-  color: #777;
+  color: #999;
+}
+.form-control::-ms-expand {
+  background-color: transparent;
+  border: 0;
 }
 .form-control[disabled],
 .form-control[readonly],
 fieldset[disabled] .form-control {
-  cursor: not-allowed;
-  background-color: #eee;
+  background-color: #eeeeee;
   opacity: 1;
 }
+.form-control[disabled],
+fieldset[disabled] .form-control {
+  cursor: not-allowed;
+}
 textarea.form-control {
   height: auto;
 }
-input[type="search"] {
-  -webkit-appearance: none;
-}
-input[type="date"],
-input[type="time"],
-input[type="datetime-local"],
-input[type="month"] {
-  line-height: 34px;
-  line-height: 1.42857143 \0;
-}
-input[type="date"].input-sm,
-input[type="time"].input-sm,
-input[type="datetime-local"].input-sm,
-input[type="month"].input-sm {
-  line-height: 30px;
-}
-input[type="date"].input-lg,
-input[type="time"].input-lg,
-input[type="datetime-local"].input-lg,
-input[type="month"].input-lg {
-  line-height: 46px;
+@media screen and (-webkit-min-device-pixel-ratio: 0) {
+  input[type="date"].form-control,
+  input[type="time"].form-control,
+  input[type="datetime-local"].form-control,
+  input[type="month"].form-control {
+    line-height: 34px;
+  }
+  input[type="date"].input-sm,
+  input[type="time"].input-sm,
+  input[type="datetime-local"].input-sm,
+  input[type="month"].input-sm,
+  .input-group-sm input[type="date"],
+  .input-group-sm input[type="time"],
+  .input-group-sm input[type="datetime-local"],
+  .input-group-sm input[type="month"] {
+    line-height: 30px;
+  }
+  input[type="date"].input-lg,
+  input[type="time"].input-lg,
+  input[type="datetime-local"].input-lg,
+  input[type="month"].input-lg,
+  .input-group-lg input[type="date"],
+  .input-group-lg input[type="time"],
+  .input-group-lg input[type="datetime-local"],
+  .input-group-lg input[type="month"] {
+    line-height: 46px;
+  }
 }
 .form-group {
   margin-bottom: 15px;
 }
 .radio,
 .checkbox {
   position: relative;
   display: block;
-  min-height: 20px;
   margin-top: 10px;
   margin-bottom: 10px;
 }
+.radio.disabled label,
+.checkbox.disabled label,
+fieldset[disabled] .radio label,
+fieldset[disabled] .checkbox label {
+  cursor: not-allowed;
+}
 .radio label,
 .checkbox label {
+  min-height: 20px;
   padding-left: 20px;
   margin-bottom: 0;
-  font-weight: normal;
+  font-weight: 400;
   cursor: pointer;
 }
 .radio input[type="radio"],
 .radio-inline input[type="radio"],
 .checkbox input[type="checkbox"],
 .checkbox-inline input[type="checkbox"] {
   position: absolute;
@@ -2444,193 +2771,243 @@
 }
 .radio + .radio,
 .checkbox + .checkbox {
   margin-top: -5px;
 }
 .radio-inline,
 .checkbox-inline {
+  position: relative;
   display: inline-block;
   padding-left: 20px;
   margin-bottom: 0;
-  font-weight: normal;
+  font-weight: 400;
   vertical-align: middle;
   cursor: pointer;
 }
-.radio-inline + .radio-inline,
-.checkbox-inline + .checkbox-inline {
-  margin-top: 0;
-  margin-left: 10px;
-}
-input[type="radio"][disabled],
-input[type="checkbox"][disabled],
-input[type="radio"].disabled,
-input[type="checkbox"].disabled,
-fieldset[disabled] input[type="radio"],
-fieldset[disabled] input[type="checkbox"] {
-  cursor: not-allowed;
-}
 .radio-inline.disabled,
 .checkbox-inline.disabled,
 fieldset[disabled] .radio-inline,
 fieldset[disabled] .checkbox-inline {
   cursor: not-allowed;
 }
-.radio.disabled label,
-.checkbox.disabled label,
-fieldset[disabled] .radio label,
-fieldset[disabled] .checkbox label {
-  cursor: not-allowed;
+.radio-inline + .radio-inline,
+.checkbox-inline + .checkbox-inline {
+  margin-top: 0;
+  margin-left: 10px;
 }
 .form-control-static {
+  min-height: 34px;
   padding-top: 7px;
   padding-bottom: 7px;
   margin-bottom: 0;
 }
 .form-control-static.input-lg,
 .form-control-static.input-sm {
   padding-right: 0;
   padding-left: 0;
 }
-.input-sm,
-.form-horizontal .form-group-sm .form-control {
+.input-sm {
   height: 30px;
   padding: 5px 10px;
   font-size: 12px;
   line-height: 1.5;
   border-radius: 3px;
 }
 select.input-sm {
   height: 30px;
   line-height: 30px;
 }
 textarea.input-sm,
 select[multiple].input-sm {
   height: auto;
 }
-.input-lg,
-.form-horizontal .form-group-lg .form-control {
+.form-group-sm .form-control {
+  height: 30px;
+  padding: 5px 10px;
+  font-size: 12px;
+  line-height: 1.5;
+  border-radius: 3px;
+}
+.form-group-sm select.form-control {
+  height: 30px;
+  line-height: 30px;
+}
+.form-group-sm textarea.form-control,
+.form-group-sm select[multiple].form-control {
+  height: auto;
+}
+.form-group-sm .form-control-static {
+  height: 30px;
+  min-height: 32px;
+  padding: 6px 10px;
+  font-size: 12px;
+  line-height: 1.5;
+}
+.input-lg {
   height: 46px;
   padding: 10px 16px;
   font-size: 18px;
-  line-height: 1.33;
+  line-height: 1.3333333;
   border-radius: 6px;
 }
 select.input-lg {
   height: 46px;
   line-height: 46px;
 }
 textarea.input-lg,
 select[multiple].input-lg {
   height: auto;
 }
+.form-group-lg .form-control {
+  height: 46px;
+  padding: 10px 16px;
+  font-size: 18px;
+  line-height: 1.3333333;
+  border-radius: 6px;
+}
+.form-group-lg select.form-control {
+  height: 46px;
+  line-height: 46px;
+}
+.form-group-lg textarea.form-control,
+.form-group-lg select[multiple].form-control {
+  height: auto;
+}
+.form-group-lg .form-control-static {
+  height: 46px;
+  min-height: 38px;
+  padding: 11px 16px;
+  font-size: 18px;
+  line-height: 1.3333333;
+}
 .has-feedback {
   position: relative;
 }
 .has-feedback .form-control {
   padding-right: 42.5px;
 }
 .form-control-feedback {
   position: absolute;
-  top: 25px;
+  top: 0;
   right: 0;
   z-index: 2;
   display: block;
   width: 34px;
   height: 34px;
   line-height: 34px;
   text-align: center;
+  pointer-events: none;
 }
-.input-lg + .form-control-feedback {
+.input-lg + .form-control-feedback,
+.input-group-lg + .form-control-feedback,
+.form-group-lg .form-control + .form-control-feedback {
   width: 46px;
   height: 46px;
   line-height: 46px;
 }
-.input-sm + .form-control-feedback {
+.input-sm + .form-control-feedback,
+.input-group-sm + .form-control-feedback,
+.form-group-sm .form-control + .form-control-feedback {
   width: 30px;
   height: 30px;
   line-height: 30px;
 }
 .has-success .help-block,
 .has-success .control-label,
 .has-success .radio,
 .has-success .checkbox,
 .has-success .radio-inline,
-.has-success .checkbox-inline {
+.has-success .checkbox-inline,
+.has-success.radio label,
+.has-success.checkbox label,
+.has-success.radio-inline label,
+.has-success.checkbox-inline label {
   color: #3c763d;
 }
 .has-success .form-control {
   border-color: #3c763d;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075);
-          box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075);
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
 }
 .has-success .form-control:focus {
   border-color: #2b542c;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 6px #67b168;
-          box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 6px #67b168;
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
 }
 .has-success .input-group-addon {
   color: #3c763d;
   background-color: #dff0d8;
   border-color: #3c763d;
 }
 .has-success .form-control-feedback {
   color: #3c763d;
 }
 .has-warning .help-block,
 .has-warning .control-label,
 .has-warning .radio,
 .has-warning .checkbox,
 .has-warning .radio-inline,
-.has-warning .checkbox-inline {
+.has-warning .checkbox-inline,
+.has-warning.radio label,
+.has-warning.checkbox label,
+.has-warning.radio-inline label,
+.has-warning.checkbox-inline label {
   color: #8a6d3b;
 }
 .has-warning .form-control {
   border-color: #8a6d3b;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075);
-          box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075);
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
 }
 .has-warning .form-control:focus {
   border-color: #66512c;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 6px #c0a16b;
-          box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 6px #c0a16b;
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
 }
 .has-warning .input-group-addon {
   color: #8a6d3b;
   background-color: #fcf8e3;
   border-color: #8a6d3b;
 }
 .has-warning .form-control-feedback {
   color: #8a6d3b;
 }
 .has-error .help-block,
 .has-error .control-label,
 .has-error .radio,
 .has-error .checkbox,
 .has-error .radio-inline,
-.has-error .checkbox-inline {
+.has-error .checkbox-inline,
+.has-error.radio label,
+.has-error.checkbox label,
+.has-error.radio-inline label,
+.has-error.checkbox-inline label {
   color: #a94442;
 }
 .has-error .form-control {
   border-color: #a94442;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075);
-          box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075);
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
 }
 .has-error .form-control:focus {
   border-color: #843534;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 6px #ce8483;
-          box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 6px #ce8483;
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
 }
 .has-error .input-group-addon {
   color: #a94442;
   background-color: #f2dede;
   border-color: #a94442;
 }
 .has-error .form-control-feedback {
   color: #a94442;
 }
+.has-feedback label ~ .form-control-feedback {
+  top: 25px;
+}
 .has-feedback label.sr-only ~ .form-control-feedback {
   top: 0;
 }
 .help-block {
   display: block;
   margin-top: 5px;
   margin-bottom: 10px;
@@ -2643,14 +3020,17 @@
     vertical-align: middle;
   }
   .form-inline .form-control {
     display: inline-block;
     width: auto;
     vertical-align: middle;
   }
+  .form-inline .form-control-static {
+    display: inline-block;
+  }
   .form-inline .input-group {
     display: inline-table;
     vertical-align: middle;
   }
   .form-inline .input-group .input-group-addon,
   .form-inline .input-group .input-group-btn,
   .form-inline .input-group .form-control {
@@ -2703,359 +3083,440 @@
   .form-horizontal .control-label {
     padding-top: 7px;
     margin-bottom: 0;
     text-align: right;
   }
 }
 .form-horizontal .has-feedback .form-control-feedback {
-  top: 0;
   right: 15px;
 }
 @media (min-width: 768px) {
   .form-horizontal .form-group-lg .control-label {
-    padding-top: 14.3px;
+    padding-top: 11px;
+    font-size: 18px;
   }
 }
 @media (min-width: 768px) {
   .form-horizontal .form-group-sm .control-label {
     padding-top: 6px;
+    font-size: 12px;
   }
 }
 .btn {
   display: inline-block;
-  padding: 6px 12px;
   margin-bottom: 0;
-  font-size: 14px;
   font-weight: normal;
-  line-height: 1.42857143;
   text-align: center;
   white-space: nowrap;
   vertical-align: middle;
+  -ms-touch-action: manipulation;
+  touch-action: manipulation;
   cursor: pointer;
-  -webkit-user-select: none;
-     -moz-user-select: none;
-      -ms-user-select: none;
-          user-select: none;
   background-image: none;
   border: 1px solid transparent;
+  padding: 6px 12px;
+  font-size: 14px;
+  line-height: 1.42857143;
   border-radius: 4px;
+  -webkit-user-select: none;
+  -moz-user-select: none;
+  -ms-user-select: none;
+  user-select: none;
 }
 .btn:focus,
 .btn:active:focus,
-.btn.active:focus {
-  outline: thin dotted;
+.btn.active:focus,
+.btn.focus,
+.btn:active.focus,
+.btn.active.focus {
   outline: 5px auto -webkit-focus-ring-color;
   outline-offset: -2px;
 }
 .btn:hover,
-.btn:focus {
+.btn:focus,
+.btn.focus {
   color: #333;
   text-decoration: none;
 }
 .btn:active,
 .btn.active {
   background-image: none;
   outline: 0;
-  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);
-          box-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);
+  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
+  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
 }
 .btn.disabled,
 .btn[disabled],
 fieldset[disabled] .btn {
-  pointer-events: none;
   cursor: not-allowed;
   filter: alpha(opacity=65);
+  opacity: 0.65;
   -webkit-box-shadow: none;
-          box-shadow: none;
-  opacity: .65;
+  box-shadow: none;
+}
+a.btn.disabled,
+fieldset[disabled] a.btn {
+  pointer-events: none;
 }
 .btn-default {
   color: #333;
   background-color: #fff;
   border-color: #ccc;
 }
-.btn-default:hover,
 .btn-default:focus,
-.btn-default:active,
-.btn-default.active,
-.open > .dropdown-toggle.btn-default {
+.btn-default.focus {
+  color: #333;
+  background-color: #e6e6e6;
+  border-color: #8c8c8c;
+}
+.btn-default:hover {
   color: #333;
   background-color: #e6e6e6;
   border-color: #adadad;
 }
 .btn-default:active,
 .btn-default.active,
 .open > .dropdown-toggle.btn-default {
+  color: #333;
+  background-color: #e6e6e6;
   background-image: none;
+  border-color: #adadad;
+}
+.btn-default:active:hover,
+.btn-default.active:hover,
+.open > .dropdown-toggle.btn-default:hover,
+.btn-default:active:focus,
+.btn-default.active:focus,
+.open > .dropdown-toggle.btn-default:focus,
+.btn-default:active.focus,
+.btn-default.active.focus,
+.open > .dropdown-toggle.btn-default.focus {
+  color: #333;
+  background-color: #d4d4d4;
+  border-color: #8c8c8c;
 }
-.btn-default.disabled,
-.btn-default[disabled],
-fieldset[disabled] .btn-default,
 .btn-default.disabled:hover,
 .btn-default[disabled]:hover,
 fieldset[disabled] .btn-default:hover,
 .btn-default.disabled:focus,
 .btn-default[disabled]:focus,
 fieldset[disabled] .btn-default:focus,
-.btn-default.disabled:active,
-.btn-default[disabled]:active,
-fieldset[disabled] .btn-default:active,
-.btn-default.disabled.active,
-.btn-default[disabled].active,
-fieldset[disabled] .btn-default.active {
+.btn-default.disabled.focus,
+.btn-default[disabled].focus,
+fieldset[disabled] .btn-default.focus {
   background-color: #fff;
   border-color: #ccc;
 }
 .btn-default .badge {
   color: #fff;
   background-color: #333;
 }
 .btn-primary {
   color: #fff;
-  background-color: #428bca;
-  border-color: #357ebd;
+  background-color: #337ab7;
+  border-color: #2e6da4;
 }
-.btn-primary:hover,
 .btn-primary:focus,
-.btn-primary:active,
-.btn-primary.active,
-.open > .dropdown-toggle.btn-primary {
+.btn-primary.focus {
+  color: #fff;
+  background-color: #286090;
+  border-color: #122b40;
+}
+.btn-primary:hover {
   color: #fff;
-  background-color: #3071a9;
-  border-color: #285e8e;
+  background-color: #286090;
+  border-color: #204d74;
 }
 .btn-primary:active,
 .btn-primary.active,
 .open > .dropdown-toggle.btn-primary {
+  color: #fff;
+  background-color: #286090;
   background-image: none;
+  border-color: #204d74;
+}
+.btn-primary:active:hover,
+.btn-primary.active:hover,
+.open > .dropdown-toggle.btn-primary:hover,
+.btn-primary:active:focus,
+.btn-primary.active:focus,
+.open > .dropdown-toggle.btn-primary:focus,
+.btn-primary:active.focus,
+.btn-primary.active.focus,
+.open > .dropdown-toggle.btn-primary.focus {
+  color: #fff;
+  background-color: #204d74;
+  border-color: #122b40;
 }
-.btn-primary.disabled,
-.btn-primary[disabled],
-fieldset[disabled] .btn-primary,
 .btn-primary.disabled:hover,
 .btn-primary[disabled]:hover,
 fieldset[disabled] .btn-primary:hover,
 .btn-primary.disabled:focus,
 .btn-primary[disabled]:focus,
 fieldset[disabled] .btn-primary:focus,
-.btn-primary.disabled:active,
-.btn-primary[disabled]:active,
-fieldset[disabled] .btn-primary:active,
-.btn-primary.disabled.active,
-.btn-primary[disabled].active,
-fieldset[disabled] .btn-primary.active {
-  background-color: #428bca;
-  border-color: #357ebd;
+.btn-primary.disabled.focus,
+.btn-primary[disabled].focus,
+fieldset[disabled] .btn-primary.focus {
+  background-color: #337ab7;
+  border-color: #2e6da4;
 }
 .btn-primary .badge {
-  color: #428bca;
+  color: #337ab7;
   background-color: #fff;
 }
 .btn-success {
   color: #fff;
   background-color: #5cb85c;
   border-color: #4cae4c;
 }
-.btn-success:hover,
 .btn-success:focus,
-.btn-success:active,
-.btn-success.active,
-.open > .dropdown-toggle.btn-success {
+.btn-success.focus {
+  color: #fff;
+  background-color: #449d44;
+  border-color: #255625;
+}
+.btn-success:hover {
   color: #fff;
   background-color: #449d44;
   border-color: #398439;
 }
 .btn-success:active,
 .btn-success.active,
 .open > .dropdown-toggle.btn-success {
+  color: #fff;
+  background-color: #449d44;
   background-image: none;
+  border-color: #398439;
+}
+.btn-success:active:hover,
+.btn-success.active:hover,
+.open > .dropdown-toggle.btn-success:hover,
+.btn-success:active:focus,
+.btn-success.active:focus,
+.open > .dropdown-toggle.btn-success:focus,
+.btn-success:active.focus,
+.btn-success.active.focus,
+.open > .dropdown-toggle.btn-success.focus {
+  color: #fff;
+  background-color: #398439;
+  border-color: #255625;
 }
-.btn-success.disabled,
-.btn-success[disabled],
-fieldset[disabled] .btn-success,
 .btn-success.disabled:hover,
 .btn-success[disabled]:hover,
 fieldset[disabled] .btn-success:hover,
 .btn-success.disabled:focus,
 .btn-success[disabled]:focus,
 fieldset[disabled] .btn-success:focus,
-.btn-success.disabled:active,
-.btn-success[disabled]:active,
-fieldset[disabled] .btn-success:active,
-.btn-success.disabled.active,
-.btn-success[disabled].active,
-fieldset[disabled] .btn-success.active {
+.btn-success.disabled.focus,
+.btn-success[disabled].focus,
+fieldset[disabled] .btn-success.focus {
   background-color: #5cb85c;
   border-color: #4cae4c;
 }
 .btn-success .badge {
   color: #5cb85c;
   background-color: #fff;
 }
 .btn-info {
   color: #fff;
   background-color: #5bc0de;
   border-color: #46b8da;
 }
-.btn-info:hover,
 .btn-info:focus,
-.btn-info:active,
-.btn-info.active,
-.open > .dropdown-toggle.btn-info {
+.btn-info.focus {
+  color: #fff;
+  background-color: #31b0d5;
+  border-color: #1b6d85;
+}
+.btn-info:hover {
   color: #fff;
   background-color: #31b0d5;
   border-color: #269abc;
 }
 .btn-info:active,
 .btn-info.active,
 .open > .dropdown-toggle.btn-info {
+  color: #fff;
+  background-color: #31b0d5;
   background-image: none;
+  border-color: #269abc;
+}
+.btn-info:active:hover,
+.btn-info.active:hover,
+.open > .dropdown-toggle.btn-info:hover,
+.btn-info:active:focus,
+.btn-info.active:focus,
+.open > .dropdown-toggle.btn-info:focus,
+.btn-info:active.focus,
+.btn-info.active.focus,
+.open > .dropdown-toggle.btn-info.focus {
+  color: #fff;
+  background-color: #269abc;
+  border-color: #1b6d85;
 }
-.btn-info.disabled,
-.btn-info[disabled],
-fieldset[disabled] .btn-info,
 .btn-info.disabled:hover,
 .btn-info[disabled]:hover,
 fieldset[disabled] .btn-info:hover,
 .btn-info.disabled:focus,
 .btn-info[disabled]:focus,
 fieldset[disabled] .btn-info:focus,
-.btn-info.disabled:active,
-.btn-info[disabled]:active,
-fieldset[disabled] .btn-info:active,
-.btn-info.disabled.active,
-.btn-info[disabled].active,
-fieldset[disabled] .btn-info.active {
+.btn-info.disabled.focus,
+.btn-info[disabled].focus,
+fieldset[disabled] .btn-info.focus {
   background-color: #5bc0de;
   border-color: #46b8da;
 }
 .btn-info .badge {
   color: #5bc0de;
   background-color: #fff;
 }
 .btn-warning {
   color: #fff;
   background-color: #f0ad4e;
   border-color: #eea236;
 }
-.btn-warning:hover,
 .btn-warning:focus,
-.btn-warning:active,
-.btn-warning.active,
-.open > .dropdown-toggle.btn-warning {
+.btn-warning.focus {
+  color: #fff;
+  background-color: #ec971f;
+  border-color: #985f0d;
+}
+.btn-warning:hover {
   color: #fff;
   background-color: #ec971f;
   border-color: #d58512;
 }
 .btn-warning:active,
 .btn-warning.active,
 .open > .dropdown-toggle.btn-warning {
+  color: #fff;
+  background-color: #ec971f;
   background-image: none;
+  border-color: #d58512;
+}
+.btn-warning:active:hover,
+.btn-warning.active:hover,
+.open > .dropdown-toggle.btn-warning:hover,
+.btn-warning:active:focus,
+.btn-warning.active:focus,
+.open > .dropdown-toggle.btn-warning:focus,
+.btn-warning:active.focus,
+.btn-warning.active.focus,
+.open > .dropdown-toggle.btn-warning.focus {
+  color: #fff;
+  background-color: #d58512;
+  border-color: #985f0d;
 }
-.btn-warning.disabled,
-.btn-warning[disabled],
-fieldset[disabled] .btn-warning,
 .btn-warning.disabled:hover,
 .btn-warning[disabled]:hover,
 fieldset[disabled] .btn-warning:hover,
 .btn-warning.disabled:focus,
 .btn-warning[disabled]:focus,
 fieldset[disabled] .btn-warning:focus,
-.btn-warning.disabled:active,
-.btn-warning[disabled]:active,
-fieldset[disabled] .btn-warning:active,
-.btn-warning.disabled.active,
-.btn-warning[disabled].active,
-fieldset[disabled] .btn-warning.active {
+.btn-warning.disabled.focus,
+.btn-warning[disabled].focus,
+fieldset[disabled] .btn-warning.focus {
   background-color: #f0ad4e;
   border-color: #eea236;
 }
 .btn-warning .badge {
   color: #f0ad4e;
   background-color: #fff;
 }
 .btn-danger {
   color: #fff;
   background-color: #d9534f;
   border-color: #d43f3a;
 }
-.btn-danger:hover,
 .btn-danger:focus,
-.btn-danger:active,
-.btn-danger.active,
-.open > .dropdown-toggle.btn-danger {
+.btn-danger.focus {
+  color: #fff;
+  background-color: #c9302c;
+  border-color: #761c19;
+}
+.btn-danger:hover {
   color: #fff;
   background-color: #c9302c;
   border-color: #ac2925;
 }
 .btn-danger:active,
 .btn-danger.active,
 .open > .dropdown-toggle.btn-danger {
+  color: #fff;
+  background-color: #c9302c;
   background-image: none;
+  border-color: #ac2925;
+}
+.btn-danger:active:hover,
+.btn-danger.active:hover,
+.open > .dropdown-toggle.btn-danger:hover,
+.btn-danger:active:focus,
+.btn-danger.active:focus,
+.open > .dropdown-toggle.btn-danger:focus,
+.btn-danger:active.focus,
+.btn-danger.active.focus,
+.open > .dropdown-toggle.btn-danger.focus {
+  color: #fff;
+  background-color: #ac2925;
+  border-color: #761c19;
 }
-.btn-danger.disabled,
-.btn-danger[disabled],
-fieldset[disabled] .btn-danger,
 .btn-danger.disabled:hover,
 .btn-danger[disabled]:hover,
 fieldset[disabled] .btn-danger:hover,
 .btn-danger.disabled:focus,
 .btn-danger[disabled]:focus,
 fieldset[disabled] .btn-danger:focus,
-.btn-danger.disabled:active,
-.btn-danger[disabled]:active,
-fieldset[disabled] .btn-danger:active,
-.btn-danger.disabled.active,
-.btn-danger[disabled].active,
-fieldset[disabled] .btn-danger.active {
+.btn-danger.disabled.focus,
+.btn-danger[disabled].focus,
+fieldset[disabled] .btn-danger.focus {
   background-color: #d9534f;
   border-color: #d43f3a;
 }
 .btn-danger .badge {
   color: #d9534f;
   background-color: #fff;
 }
 .btn-link {
-  font-weight: normal;
-  color: #428bca;
-  cursor: pointer;
+  font-weight: 400;
+  color: #337ab7;
   border-radius: 0;
 }
 .btn-link,
 .btn-link:active,
+.btn-link.active,
 .btn-link[disabled],
 fieldset[disabled] .btn-link {
   background-color: transparent;
   -webkit-box-shadow: none;
-          box-shadow: none;
+  box-shadow: none;
 }
 .btn-link,
 .btn-link:hover,
 .btn-link:focus,
 .btn-link:active {
   border-color: transparent;
 }
 .btn-link:hover,
 .btn-link:focus {
-  color: #2a6496;
+  color: #23527c;
   text-decoration: underline;
   background-color: transparent;
 }
 .btn-link[disabled]:hover,
 fieldset[disabled] .btn-link:hover,
 .btn-link[disabled]:focus,
 fieldset[disabled] .btn-link:focus {
-  color: #777;
+  color: #777777;
   text-decoration: none;
 }
 .btn-lg,
 .btn-group-lg > .btn {
   padding: 10px 16px;
   font-size: 18px;
-  line-height: 1.33;
+  line-height: 1.3333333;
   border-radius: 6px;
 }
 .btn-sm,
 .btn-group-sm > .btn {
   padding: 5px 10px;
   font-size: 12px;
   line-height: 1.5;
@@ -3078,17 +3539,17 @@
 input[type="submit"].btn-block,
 input[type="reset"].btn-block,
 input[type="button"].btn-block {
   width: 100%;
 }
 .fade {
   opacity: 0;
-  -webkit-transition: opacity .15s linear;
-       -o-transition: opacity .15s linear;
-          transition: opacity .15s linear;
+  -webkit-transition: opacity 0.15s linear;
+  -o-transition: opacity 0.15s linear;
+  transition: opacity 0.15s linear;
 }
 .fade.in {
   opacity: 1;
 }
 .collapse {
   display: none;
 }
@@ -3101,28 +3562,36 @@
 tbody.collapse.in {
   display: table-row-group;
 }
 .collapsing {
   position: relative;
   height: 0;
   overflow: hidden;
-  -webkit-transition: height .35s ease;
-       -o-transition: height .35s ease;
-          transition: height .35s ease;
+  -webkit-transition-property: height, visibility;
+  -o-transition-property: height, visibility;
+  transition-property: height, visibility;
+  -webkit-transition-duration: 0.35s;
+  -o-transition-duration: 0.35s;
+  transition-duration: 0.35s;
+  -webkit-transition-timing-function: ease;
+  -o-transition-timing-function: ease;
+  transition-timing-function: ease;
 }
 .caret {
   display: inline-block;
   width: 0;
   height: 0;
   margin-left: 2px;
   vertical-align: middle;
-  border-top: 4px solid;
+  border-top: 4px dashed;
+  border-top: 4px solid \9;
   border-right: 4px solid transparent;
   border-left: 4px solid transparent;
 }
+.dropup,
 .dropdown {
   position: relative;
 }
 .dropdown-toggle:focus {
   outline: 0;
 }
 .dropdown-menu {
@@ -3135,21 +3604,20 @@
   min-width: 160px;
   padding: 5px 0;
   margin: 2px 0 0;
   font-size: 14px;
   text-align: left;
   list-style: none;
   background-color: #fff;
-  -webkit-background-clip: padding-box;
-          background-clip: padding-box;
+  background-clip: padding-box;
   border: 1px solid #ccc;
-  border: 1px solid rgba(0, 0, 0, .15);
+  border: 1px solid rgba(0, 0, 0, 0.15);
   border-radius: 4px;
-  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
-          box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
+  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
+  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
 }
 .dropdown-menu.pull-right {
   right: 0;
   left: auto;
 }
 .dropdown-menu .divider {
   height: 1px;
@@ -3157,37 +3625,37 @@
   overflow: hidden;
   background-color: #e5e5e5;
 }
 .dropdown-menu > li > a {
   display: block;
   padding: 3px 20px;
   clear: both;
-  font-weight: normal;
+  font-weight: 400;
   line-height: 1.42857143;
-  color: #333;
+  color: #333333;
   white-space: nowrap;
 }
 .dropdown-menu > li > a:hover,
 .dropdown-menu > li > a:focus {
   color: #262626;
   text-decoration: none;
   background-color: #f5f5f5;
 }
 .dropdown-menu > .active > a,
 .dropdown-menu > .active > a:hover,
 .dropdown-menu > .active > a:focus {
   color: #fff;
   text-decoration: none;
-  background-color: #428bca;
+  background-color: #337ab7;
   outline: 0;
 }
 .dropdown-menu > .disabled > a,
 .dropdown-menu > .disabled > a:hover,
 .dropdown-menu > .disabled > a:focus {
-  color: #777;
+  color: #777777;
 }
 .dropdown-menu > .disabled > a:hover,
 .dropdown-menu > .disabled > a:focus {
   text-decoration: none;
   cursor: not-allowed;
   background-color: transparent;
   background-image: none;
@@ -3208,15 +3676,15 @@
   left: 0;
 }
 .dropdown-header {
   display: block;
   padding: 3px 20px;
   font-size: 12px;
   line-height: 1.42857143;
-  color: #777;
+  color: #777777;
   white-space: nowrap;
 }
 .dropdown-backdrop {
   position: fixed;
   top: 0;
   right: 0;
   bottom: 0;
@@ -3227,21 +3695,22 @@
   right: 0;
   left: auto;
 }
 .dropup .caret,
 .navbar-fixed-bottom .dropdown .caret {
   content: "";
   border-top: 0;
-  border-bottom: 4px solid;
+  border-bottom: 4px dashed;
+  border-bottom: 4px solid \9;
 }
 .dropup .dropdown-menu,
 .navbar-fixed-bottom .dropdown .dropdown-menu {
   top: auto;
   bottom: 100%;
-  margin-bottom: 1px;
+  margin-bottom: 2px;
 }
 @media (min-width: 768px) {
   .navbar-right .dropdown-menu {
     right: 0;
     left: auto;
   }
   .navbar-right .dropdown-menu-left {
@@ -3266,27 +3735,24 @@
 .btn-group-vertical > .btn:focus,
 .btn-group > .btn:active,
 .btn-group-vertical > .btn:active,
 .btn-group > .btn.active,
 .btn-group-vertical > .btn.active {
   z-index: 2;
 }
-.btn-group > .btn:focus,
-.btn-group-vertical > .btn:focus {
-  outline: 0;
-}
 .btn-group .btn + .btn,
 .btn-group .btn + .btn-group,
 .btn-group .btn-group + .btn,
 .btn-group .btn-group + .btn-group {
   margin-left: -1px;
 }
 .btn-toolbar {
   margin-left: -5px;
 }
+.btn-toolbar .btn,
 .btn-toolbar .btn-group,
 .btn-toolbar .input-group {
   float: left;
 }
 .btn-toolbar > .btn,
 .btn-toolbar > .btn-group,
 .btn-toolbar > .input-group {
@@ -3309,20 +3775,20 @@
 }
 .btn-group > .btn-group {
   float: left;
 }
 .btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
   border-radius: 0;
 }
-.btn-group > .btn-group:first-child > .btn:last-child,
-.btn-group > .btn-group:first-child > .dropdown-toggle {
+.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
+.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
   border-top-right-radius: 0;
   border-bottom-right-radius: 0;
 }
-.btn-group > .btn-group:last-child > .btn:first-child {
+.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
   border-top-left-radius: 0;
   border-bottom-left-radius: 0;
 }
 .btn-group .dropdown-toggle:active,
 .btn-group.open .dropdown-toggle {
   outline: 0;
 }
@@ -3331,20 +3797,20 @@
   padding-left: 8px;
 }
 .btn-group > .btn-lg + .dropdown-toggle {
   padding-right: 12px;
   padding-left: 12px;
 }
 .btn-group.open .dropdown-toggle {
-  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);
-          box-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);
+  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
+  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
 }
 .btn-group.open .dropdown-toggle.btn-link {
   -webkit-box-shadow: none;
-          box-shadow: none;
+  box-shadow: none;
 }
 .btn .caret {
   margin-left: 0;
 }
 .btn-lg .caret {
   border-width: 5px 5px 0;
   border-bottom-width: 0;
@@ -3370,21 +3836,23 @@
   margin-top: -1px;
   margin-left: 0;
 }
 .btn-group-vertical > .btn:not(:first-child):not(:last-child) {
   border-radius: 0;
 }
 .btn-group-vertical > .btn:first-child:not(:last-child) {
+  border-top-left-radius: 4px;
   border-top-right-radius: 4px;
   border-bottom-right-radius: 0;
   border-bottom-left-radius: 0;
 }
 .btn-group-vertical > .btn:last-child:not(:first-child) {
   border-top-left-radius: 0;
   border-top-right-radius: 0;
+  border-bottom-right-radius: 4px;
   border-bottom-left-radius: 4px;
 }
 .btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
   border-radius: 0;
 }
 .btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
 .btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
@@ -3409,20 +3877,21 @@
 }
 .btn-group-justified > .btn-group .btn {
   width: 100%;
 }
 .btn-group-justified > .btn-group .dropdown-menu {
   left: auto;
 }
-[data-toggle="buttons"] > .btn > input[type="radio"],
-[data-toggle="buttons"] > .btn > input[type="checkbox"] {
+[data-toggle="buttons"] > .btn input[type="radio"],
+[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
+[data-toggle="buttons"] > .btn input[type="checkbox"],
+[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
   position: absolute;
-  z-index: -1;
-  filter: alpha(opacity=0);
-  opacity: 0;
+  clip: rect(0, 0, 0, 0);
+  pointer-events: none;
 }
 .input-group {
   position: relative;
   display: table;
   border-collapse: separate;
 }
 .input-group[class*="col-"] {
@@ -3433,21 +3902,24 @@
 .input-group .form-control {
   position: relative;
   z-index: 2;
   float: left;
   width: 100%;
   margin-bottom: 0;
 }
+.input-group .form-control:focus {
+  z-index: 3;
+}
 .input-group-lg > .form-control,
 .input-group-lg > .input-group-addon,
 .input-group-lg > .input-group-btn > .btn {
   height: 46px;
   padding: 10px 16px;
   font-size: 18px;
-  line-height: 1.33;
+  line-height: 1.3333333;
   border-radius: 6px;
 }
 select.input-group-lg > .form-control,
 select.input-group-lg > .input-group-addon,
 select.input-group-lg > .input-group-btn > .btn {
   height: 46px;
   line-height: 46px;
@@ -3498,19 +3970,19 @@
   width: 1%;
   white-space: nowrap;
   vertical-align: middle;
 }
 .input-group-addon {
   padding: 6px 12px;
   font-size: 14px;
-  font-weight: normal;
+  font-weight: 400;
   line-height: 1;
-  color: #555;
+  color: #555555;
   text-align: center;
-  background-color: #eee;
+  background-color: #eeeeee;
   border: 1px solid #ccc;
   border-radius: 4px;
 }
 .input-group-addon.input-sm {
   padding: 5px 10px;
   font-size: 12px;
   border-radius: 3px;
@@ -3568,14 +4040,15 @@
 }
 .input-group-btn:first-child > .btn,
 .input-group-btn:first-child > .btn-group {
   margin-right: -1px;
 }
 .input-group-btn:last-child > .btn,
 .input-group-btn:last-child > .btn-group {
+  z-index: 2;
   margin-left: -1px;
 }
 .nav {
   padding-left: 0;
   margin-bottom: 0;
   list-style: none;
 }
@@ -3587,31 +4060,31 @@
   position: relative;
   display: block;
   padding: 10px 15px;
 }
 .nav > li > a:hover,
 .nav > li > a:focus {
   text-decoration: none;
-  background-color: #eee;
+  background-color: #eeeeee;
 }
 .nav > li.disabled > a {
-  color: #777;
+  color: #777777;
 }
 .nav > li.disabled > a:hover,
 .nav > li.disabled > a:focus {
-  color: #777;
+  color: #777777;
   text-decoration: none;
   cursor: not-allowed;
   background-color: transparent;
 }
 .nav .open > a,
 .nav .open > a:hover,
 .nav .open > a:focus {
-  background-color: #eee;
-  border-color: #428bca;
+  background-color: #eeeeee;
+  border-color: #337ab7;
 }
 .nav .nav-divider {
   height: 1px;
   margin: 9px 0;
   overflow: hidden;
   background-color: #e5e5e5;
 }
@@ -3628,20 +4101,20 @@
 .nav-tabs > li > a {
   margin-right: 2px;
   line-height: 1.42857143;
   border: 1px solid transparent;
   border-radius: 4px 4px 0 0;
 }
 .nav-tabs > li > a:hover {
-  border-color: #eee #eee #ddd;
+  border-color: #eeeeee #eeeeee #ddd;
 }
 .nav-tabs > li.active > a,
 .nav-tabs > li.active > a:hover,
 .nav-tabs > li.active > a:focus {
-  color: #555;
+  color: #555555;
   cursor: default;
   background-color: #fff;
   border: 1px solid #ddd;
   border-bottom-color: transparent;
 }
 .nav-tabs.nav-justified {
   width: 100%;
@@ -3696,15 +4169,15 @@
 .nav-pills > li + li {
   margin-left: 2px;
 }
 .nav-pills > li.active > a,
 .nav-pills > li.active > a:hover,
 .nav-pills > li.active > a:focus {
   color: #fff;
-  background-color: #428bca;
+  background-color: #337ab7;
 }
 .nav-stacked > li {
   float: none;
 }
 .nav-stacked > li + li {
   margin-top: 2px;
   margin-left: 0;
@@ -3782,28 +4255,28 @@
     float: left;
   }
 }
 .navbar-collapse {
   padding-right: 15px;
   padding-left: 15px;
   overflow-x: visible;
-  -webkit-overflow-scrolling: touch;
   border-top: 1px solid transparent;
-  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, .1);
-          box-shadow: inset 0 1px 0 rgba(255, 255, 255, .1);
+  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
+  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
+  -webkit-overflow-scrolling: touch;
 }
 .navbar-collapse.in {
   overflow-y: auto;
 }
 @media (min-width: 768px) {
   .navbar-collapse {
     width: auto;
     border-top: 0;
     -webkit-box-shadow: none;
-            box-shadow: none;
+    box-shadow: none;
   }
   .navbar-collapse.collapse {
     display: block !important;
     height: auto !important;
     padding-bottom: 0;
     overflow: visible !important;
   }
@@ -3813,24 +4286,46 @@
   .navbar-fixed-top .navbar-collapse,
   .navbar-static-top .navbar-collapse,
   .navbar-fixed-bottom .navbar-collapse {
     padding-right: 0;
     padding-left: 0;
   }
 }
+.navbar-fixed-top,
+.navbar-fixed-bottom {
+  position: fixed;
+  right: 0;
+  left: 0;
+  z-index: 1030;
+}
 .navbar-fixed-top .navbar-collapse,
 .navbar-fixed-bottom .navbar-collapse {
   max-height: 340px;
 }
-@media (max-width: 480px) and (orientation: landscape) {
+@media (max-device-width: 480px) and (orientation: landscape) {
   .navbar-fixed-top .navbar-collapse,
   .navbar-fixed-bottom .navbar-collapse {
     max-height: 200px;
   }
 }
+@media (min-width: 768px) {
+  .navbar-fixed-top,
+  .navbar-fixed-bottom {
+    border-radius: 0;
+  }
+}
+.navbar-fixed-top {
+  top: 0;
+  border-width: 0 0 1px;
+}
+.navbar-fixed-bottom {
+  bottom: 0;
+  margin-bottom: 0;
+  border-width: 1px 0 0;
+}
 .container > .navbar-header,
 .container-fluid > .navbar-header,
 .container > .navbar-collapse,
 .container-fluid > .navbar-collapse {
   margin-right: -15px;
   margin-left: -15px;
 }
@@ -3848,62 +4343,40 @@
   border-width: 0 0 1px;
 }
 @media (min-width: 768px) {
   .navbar-static-top {
     border-radius: 0;
   }
 }
-.navbar-fixed-top,
-.navbar-fixed-bottom {
-  position: fixed;
-  right: 0;
-  left: 0;
-  z-index: 1030;
-  -webkit-transform: translate3d(0, 0, 0);
-       -o-transform: translate3d(0, 0, 0);
-          transform: translate3d(0, 0, 0);
-}
-@media (min-width: 768px) {
-  .navbar-fixed-top,
-  .navbar-fixed-bottom {
-    border-radius: 0;
-  }
-}
-.navbar-fixed-top {
-  top: 0;
-  border-width: 0 0 1px;
-}
-.navbar-fixed-bottom {
-  bottom: 0;
-  margin-bottom: 0;
-  border-width: 1px 0 0;
-}
 .navbar-brand {
   float: left;
   height: 50px;
   padding: 15px 15px;
   font-size: 18px;
   line-height: 20px;
 }
 .navbar-brand:hover,
 .navbar-brand:focus {
   text-decoration: none;
 }
+.navbar-brand > img {
+  display: block;
+}
 @media (min-width: 768px) {
   .navbar > .container .navbar-brand,
   .navbar > .container-fluid .navbar-brand {
     margin-left: -15px;
   }
 }
 .navbar-toggle {
   position: relative;
   float: right;
   padding: 9px 10px;
-  margin-top: 8px;
   margin-right: 15px;
+  margin-top: 8px;
   margin-bottom: 8px;
   background-color: transparent;
   background-image: none;
   border: 1px solid transparent;
   border-radius: 4px;
 }
 .navbar-toggle:focus {
@@ -3936,15 +4409,15 @@
     position: static;
     float: none;
     width: auto;
     margin-top: 0;
     background-color: transparent;
     border: 0;
     -webkit-box-shadow: none;
-            box-shadow: none;
+    box-shadow: none;
   }
   .navbar-nav .open .dropdown-menu > li > a,
   .navbar-nav .open .dropdown-menu .dropdown-header {
     padding: 5px 15px 5px 25px;
   }
   .navbar-nav .open .dropdown-menu > li > a {
     line-height: 20px;
@@ -3962,48 +4435,40 @@
   .navbar-nav > li {
     float: left;
   }
   .navbar-nav > li > a {
     padding-top: 15px;
     padding-bottom: 15px;
   }
-  .navbar-nav.navbar-right:last-child {
-    margin-right: -15px;
-  }
-}
-@media (min-width: 768px) {
-  .navbar-left {
-    float: left !important;
-  }
-  .navbar-right {
-    float: right !important;
-  }
 }
 .navbar-form {
   padding: 10px 15px;
-  margin-top: 8px;
   margin-right: -15px;
-  margin-bottom: 8px;
   margin-left: -15px;
   border-top: 1px solid transparent;
   border-bottom: 1px solid transparent;
-  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, .1), 0 1px 0 rgba(255, 255, 255, .1);
-          box-shadow: inset 0 1px 0 rgba(255, 255, 255, .1), 0 1px 0 rgba(255, 255, 255, .1);
+  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
+  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
+  margin-top: 8px;
+  margin-bottom: 8px;
 }
 @media (min-width: 768px) {
   .navbar-form .form-group {
     display: inline-block;
     margin-bottom: 0;
     vertical-align: middle;
   }
   .navbar-form .form-control {
     display: inline-block;
     width: auto;
     vertical-align: middle;
   }
+  .navbar-form .form-control-static {
+    display: inline-block;
+  }
   .navbar-form .input-group {
     display: inline-table;
     vertical-align: middle;
   }
   .navbar-form .input-group .input-group-addon,
   .navbar-form .input-group .input-group-btn,
   .navbar-form .input-group .form-control {
@@ -4036,36 +4501,39 @@
     top: 0;
   }
 }
 @media (max-width: 767px) {
   .navbar-form .form-group {
     margin-bottom: 5px;
   }
+  .navbar-form .form-group:last-child {
+    margin-bottom: 0;
+  }
 }
 @media (min-width: 768px) {
   .navbar-form {
     width: auto;
     padding-top: 0;
     padding-bottom: 0;
     margin-right: 0;
     margin-left: 0;
     border: 0;
     -webkit-box-shadow: none;
-            box-shadow: none;
-  }
-  .navbar-form.navbar-right:last-child {
-    margin-right: -15px;
+    box-shadow: none;
   }
 }
 .navbar-nav > li > .dropdown-menu {
   margin-top: 0;
   border-top-left-radius: 0;
   border-top-right-radius: 0;
 }
 .navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
+  margin-bottom: 0;
+  border-top-left-radius: 4px;
+  border-top-right-radius: 4px;
   border-bottom-right-radius: 0;
   border-bottom-left-radius: 0;
 }
 .navbar-btn {
   margin-top: 8px;
   margin-bottom: 8px;
 }
@@ -4083,15 +4551,24 @@
 }
 @media (min-width: 768px) {
   .navbar-text {
     float: left;
     margin-right: 15px;
     margin-left: 15px;
   }
-  .navbar-text.navbar-right:last-child {
+}
+@media (min-width: 768px) {
+  .navbar-left {
+    float: left !important;
+  }
+  .navbar-right {
+    float: right !important;
+    margin-right: -15px;
+  }
+  .navbar-right ~ .navbar-right {
     margin-right: 0;
   }
 }
 .navbar-default {
   background-color: #f8f8f8;
   border-color: #e7e7e7;
 }
@@ -4122,28 +4599,14 @@
 }
 .navbar-default .navbar-nav > .disabled > a,
 .navbar-default .navbar-nav > .disabled > a:hover,
 .navbar-default .navbar-nav > .disabled > a:focus {
   color: #ccc;
   background-color: transparent;
 }
-.navbar-default .navbar-toggle {
-  border-color: #ddd;
-}
-.navbar-default .navbar-toggle:hover,
-.navbar-default .navbar-toggle:focus {
-  background-color: #ddd;
-}
-.navbar-default .navbar-toggle .icon-bar {
-  background-color: #888;
-}
-.navbar-default .navbar-collapse,
-.navbar-default .navbar-form {
-  border-color: #e7e7e7;
-}
 .navbar-default .navbar-nav > .open > a,
 .navbar-default .navbar-nav > .open > a:hover,
 .navbar-default .navbar-nav > .open > a:focus {
   color: #555;
   background-color: #e7e7e7;
 }
 @media (max-width: 767px) {
@@ -4164,14 +4627,28 @@
   .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
   .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
   .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
     color: #ccc;
     background-color: transparent;
   }
 }
+.navbar-default .navbar-toggle {
+  border-color: #ddd;
+}
+.navbar-default .navbar-toggle:hover,
+.navbar-default .navbar-toggle:focus {
+  background-color: #ddd;
+}
+.navbar-default .navbar-toggle .icon-bar {
+  background-color: #888;
+}
+.navbar-default .navbar-collapse,
+.navbar-default .navbar-form {
+  border-color: #e7e7e7;
+}
 .navbar-default .navbar-link {
   color: #777;
 }
 .navbar-default .navbar-link:hover {
   color: #333;
 }
 .navbar-default .btn-link {
@@ -4188,26 +4665,26 @@
   color: #ccc;
 }
 .navbar-inverse {
   background-color: #222;
   border-color: #080808;
 }
 .navbar-inverse .navbar-brand {
-  color: #777;
+  color: #9d9d9d;
 }
 .navbar-inverse .navbar-brand:hover,
 .navbar-inverse .navbar-brand:focus {
   color: #fff;
   background-color: transparent;
 }
 .navbar-inverse .navbar-text {
-  color: #777;
+  color: #9d9d9d;
 }
 .navbar-inverse .navbar-nav > li > a {
-  color: #777;
+  color: #9d9d9d;
 }
 .navbar-inverse .navbar-nav > li > a:hover,
 .navbar-inverse .navbar-nav > li > a:focus {
   color: #fff;
   background-color: transparent;
 }
 .navbar-inverse .navbar-nav > .active > a,
@@ -4218,43 +4695,29 @@
 }
 .navbar-inverse .navbar-nav > .disabled > a,
 .navbar-inverse .navbar-nav > .disabled > a:hover,
 .navbar-inverse .navbar-nav > .disabled > a:focus {
   color: #444;
   background-color: transparent;
 }
-.navbar-inverse .navbar-toggle {
-  border-color: #333;
-}
-.navbar-inverse .navbar-toggle:hover,
-.navbar-inverse .navbar-toggle:focus {
-  background-color: #333;
-}
-.navbar-inverse .navbar-toggle .icon-bar {
-  background-color: #fff;
-}
-.navbar-inverse .navbar-collapse,
-.navbar-inverse .navbar-form {
-  border-color: #101010;
-}
 .navbar-inverse .navbar-nav > .open > a,
 .navbar-inverse .navbar-nav > .open > a:hover,
 .navbar-inverse .navbar-nav > .open > a:focus {
   color: #fff;
   background-color: #080808;
 }
 @media (max-width: 767px) {
   .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
     border-color: #080808;
   }
   .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
     background-color: #080808;
   }
   .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
-    color: #777;
+    color: #9d9d9d;
   }
   .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
   .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
     color: #fff;
     background-color: transparent;
   }
   .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
@@ -4266,22 +4729,36 @@
   .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
   .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
   .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
     color: #444;
     background-color: transparent;
   }
 }
+.navbar-inverse .navbar-toggle {
+  border-color: #333;
+}
+.navbar-inverse .navbar-toggle:hover,
+.navbar-inverse .navbar-toggle:focus {
+  background-color: #333;
+}
+.navbar-inverse .navbar-toggle .icon-bar {
+  background-color: #fff;
+}
+.navbar-inverse .navbar-collapse,
+.navbar-inverse .navbar-form {
+  border-color: #101010;
+}
 .navbar-inverse .navbar-link {
-  color: #777;
+  color: #9d9d9d;
 }
 .navbar-inverse .navbar-link:hover {
   color: #fff;
 }
 .navbar-inverse .btn-link {
-  color: #777;
+  color: #9d9d9d;
 }
 .navbar-inverse .btn-link:hover,
 .navbar-inverse .btn-link:focus {
   color: #fff;
 }
 .navbar-inverse .btn-link[disabled]:hover,
 fieldset[disabled] .navbar-inverse .btn-link:hover,
@@ -4301,15 +4778,15 @@
 }
 .breadcrumb > li + li:before {
   padding: 0 5px;
   color: #ccc;
   content: "/\00a0";
 }
 .breadcrumb > .active {
-  color: #777;
+  color: #777777;
 }
 .pagination {
   display: inline-block;
   padding-left: 0;
   margin: 20px 0;
   border-radius: 4px;
 }
@@ -4319,65 +4796,67 @@
 .pagination > li > a,
 .pagination > li > span {
   position: relative;
   float: left;
   padding: 6px 12px;
   margin-left: -1px;
   line-height: 1.42857143;
-  color: #428bca;
+  color: #337ab7;
   text-decoration: none;
   background-color: #fff;
   border: 1px solid #ddd;
 }
+.pagination > li > a:hover,
+.pagination > li > span:hover,
+.pagination > li > a:focus,
+.pagination > li > span:focus {
+  z-index: 2;
+  color: #23527c;
+  background-color: #eeeeee;
+  border-color: #ddd;
+}
 .pagination > li:first-child > a,
 .pagination > li:first-child > span {
   margin-left: 0;
   border-top-left-radius: 4px;
   border-bottom-left-radius: 4px;
 }
 .pagination > li:last-child > a,
 .pagination > li:last-child > span {
   border-top-right-radius: 4px;
   border-bottom-right-radius: 4px;
 }
-.pagination > li > a:hover,
-.pagination > li > span:hover,
-.pagination > li > a:focus,
-.pagination > li > span:focus {
-  color: #2a6496;
-  background-color: #eee;
-  border-color: #ddd;
-}
 .pagination > .active > a,
 .pagination > .active > span,
 .pagination > .active > a:hover,
 .pagination > .active > span:hover,
 .pagination > .active > a:focus,
 .pagination > .active > span:focus {
-  z-index: 2;
+  z-index: 3;
   color: #fff;
   cursor: default;
-  background-color: #428bca;
-  border-color: #428bca;
+  background-color: #337ab7;
+  border-color: #337ab7;
 }
 .pagination > .disabled > span,
 .pagination > .disabled > span:hover,
 .pagination > .disabled > span:focus,
 .pagination > .disabled > a,
 .pagination > .disabled > a:hover,
 .pagination > .disabled > a:focus {
-  color: #777;
+  color: #777777;
   cursor: not-allowed;
   background-color: #fff;
   border-color: #ddd;
 }
 .pagination-lg > li > a,
 .pagination-lg > li > span {
   padding: 10px 16px;
   font-size: 18px;
+  line-height: 1.3333333;
 }
 .pagination-lg > li:first-child > a,
 .pagination-lg > li:first-child > span {
   border-top-left-radius: 6px;
   border-bottom-left-radius: 6px;
 }
 .pagination-lg > li:last-child > a,
@@ -4385,14 +4864,15 @@
   border-top-right-radius: 6px;
   border-bottom-right-radius: 6px;
 }
 .pagination-sm > li > a,
 .pagination-sm > li > span {
   padding: 5px 10px;
   font-size: 12px;
+  line-height: 1.5;
 }
 .pagination-sm > li:first-child > a,
 .pagination-sm > li:first-child > span {
   border-top-left-radius: 3px;
   border-bottom-left-radius: 3px;
 }
 .pagination-sm > li:last-child > a,
@@ -4416,43 +4896,43 @@
   background-color: #fff;
   border: 1px solid #ddd;
   border-radius: 15px;
 }
 .pager li > a:hover,
 .pager li > a:focus {
   text-decoration: none;
-  background-color: #eee;
+  background-color: #eeeeee;
 }
 .pager .next > a,
 .pager .next > span {
   float: right;
 }
 .pager .previous > a,
 .pager .previous > span {
   float: left;
 }
 .pager .disabled > a,
 .pager .disabled > a:hover,
 .pager .disabled > a:focus,
 .pager .disabled > span {
-  color: #777;
+  color: #777777;
   cursor: not-allowed;
   background-color: #fff;
 }
 .label {
   display: inline;
-  padding: .2em .6em .3em;
+  padding: 0.2em 0.6em 0.3em;
   font-size: 75%;
-  font-weight: bold;
+  font-weight: 700;
   line-height: 1;
   color: #fff;
   text-align: center;
   white-space: nowrap;
   vertical-align: baseline;
-  border-radius: .25em;
+  border-radius: 0.25em;
 }
 a.label:hover,
 a.label:focus {
   color: #fff;
   text-decoration: none;
   cursor: pointer;
 }
@@ -4460,26 +4940,26 @@
   display: none;
 }
 .btn .label {
   position: relative;
   top: -1px;
 }
 .label-default {
-  background-color: #777;
+  background-color: #777777;
 }
 .label-default[href]:hover,
 .label-default[href]:focus {
   background-color: #5e5e5e;
 }
 .label-primary {
-  background-color: #428bca;
+  background-color: #337ab7;
 }
 .label-primary[href]:hover,
 .label-primary[href]:focus {
-  background-color: #3071a9;
+  background-color: #286090;
 }
 .label-success {
   background-color: #5cb85c;
 }
 .label-success[href]:hover,
 .label-success[href]:focus {
   background-color: #449d44;
@@ -4511,73 +4991,85 @@
   padding: 3px 7px;
   font-size: 12px;
   font-weight: bold;
   line-height: 1;
   color: #fff;
   text-align: center;
   white-space: nowrap;
-  vertical-align: baseline;
-  background-color: #777;
+  vertical-align: middle;
+  background-color: #777777;
   border-radius: 10px;
 }
 .badge:empty {
   display: none;
 }
 .btn .badge {
   position: relative;
   top: -1px;
 }
-.btn-xs .badge {
+.btn-xs .badge,
+.btn-group-xs > .btn .badge {
   top: 0;
   padding: 1px 5px;
 }
 a.badge:hover,
 a.badge:focus {
   color: #fff;
   text-decoration: none;
   cursor: pointer;
 }
-a.list-group-item.active > .badge,
+.list-group-item.active > .badge,
 .nav-pills > .active > a > .badge {
-  color: #428bca;
+  color: #337ab7;
   background-color: #fff;
 }
+.list-group-item > .badge {
+  float: right;
+}
+.list-group-item > .badge + .badge {
+  margin-right: 5px;
+}
 .nav-pills > li > a > .badge {
   margin-left: 3px;
 }
 .jumbotron {
-  padding: 30px;
+  padding-top: 30px;
+  padding-bottom: 30px;
   margin-bottom: 30px;
   color: inherit;
-  background-color: #eee;
+  background-color: #eeeeee;
 }
 .jumbotron h1,
 .jumbotron .h1 {
   color: inherit;
 }
 .jumbotron p {
   margin-bottom: 15px;
   font-size: 21px;
   font-weight: 200;
 }
 .jumbotron > hr {
   border-top-color: #d5d5d5;
 }
-.container .jumbotron {
+.container .jumbotron,
+.container-fluid .jumbotron {
+  padding-right: 15px;
+  padding-left: 15px;
   border-radius: 6px;
 }
 .jumbotron .container {
   max-width: 100%;
 }
 @media screen and (min-width: 768px) {
   .jumbotron {
     padding-top: 48px;
     padding-bottom: 48px;
   }
-  .container .jumbotron {
+  .container .jumbotron,
+  .container-fluid .jumbotron {
     padding-right: 60px;
     padding-left: 60px;
   }
   .jumbotron h1,
   .jumbotron .h1 {
     font-size: 63px;
   }
@@ -4586,31 +5078,31 @@
   display: block;
   padding: 4px;
   margin-bottom: 20px;
   line-height: 1.42857143;
   background-color: #fff;
   border: 1px solid #ddd;
   border-radius: 4px;
-  -webkit-transition: all .2s ease-in-out;
-       -o-transition: all .2s ease-in-out;
-          transition: all .2s ease-in-out;
+  -webkit-transition: border 0.2s ease-in-out;
+  -o-transition: border 0.2s ease-in-out;
+  transition: border 0.2s ease-in-out;
 }
 .thumbnail > img,
 .thumbnail a > img {
   margin-right: auto;
   margin-left: auto;
 }
 a.thumbnail:hover,
 a.thumbnail:focus,
 a.thumbnail.active {
-  border-color: #428bca;
+  border-color: #337ab7;
 }
 .thumbnail .caption {
   padding: 9px;
-  color: #333;
+  color: #333333;
 }
 .alert {
   padding: 15px;
   margin-bottom: 20px;
   border: 1px solid transparent;
   border-radius: 4px;
 }
@@ -4709,113 +5201,121 @@
 }
 .progress {
   height: 20px;
   margin-bottom: 20px;
   overflow: hidden;
   background-color: #f5f5f5;
   border-radius: 4px;
-  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, .1);
-          box-shadow: inset 0 1px 2px rgba(0, 0, 0, .1);
+  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
+  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
 }
 .progress-bar {
   float: left;
-  width: 0;
+  width: 0%;
   height: 100%;
   font-size: 12px;
   line-height: 20px;
   color: #fff;
   text-align: center;
-  background-color: #428bca;
-  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, .15);
-          box-shadow: inset 0 -1px 0 rgba(0, 0, 0, .15);
-  -webkit-transition: width .6s ease;
-       -o-transition: width .6s ease;
-          transition: width .6s ease;
+  background-color: #337ab7;
+  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
+  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
+  -webkit-transition: width 0.6s ease;
+  -o-transition: width 0.6s ease;
+  transition: width 0.6s ease;
 }
 .progress-striped .progress-bar,
 .progress-bar-striped {
-  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:      -o-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:         linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
+  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
   -webkit-background-size: 40px 40px;
-          background-size: 40px 40px;
+  background-size: 40px 40px;
 }
 .progress.active .progress-bar,
 .progress-bar.active {
   -webkit-animation: progress-bar-stripes 2s linear infinite;
-       -o-animation: progress-bar-stripes 2s linear infinite;
-          animation: progress-bar-stripes 2s linear infinite;
-}
-.progress-bar[aria-valuenow="1"],
-.progress-bar[aria-valuenow="2"] {
-  min-width: 30px;
-}
-.progress-bar[aria-valuenow="0"] {
-  min-width: 30px;
-  color: #777;
-  background-color: transparent;
-  background-image: none;
-  -webkit-box-shadow: none;
-          box-shadow: none;
+  -o-animation: progress-bar-stripes 2s linear infinite;
+  animation: progress-bar-stripes 2s linear infinite;
 }
 .progress-bar-success {
   background-color: #5cb85c;
 }
 .progress-striped .progress-bar-success {
-  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:      -o-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:         linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
+  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
 }
 .progress-bar-info {
   background-color: #5bc0de;
 }
 .progress-striped .progress-bar-info {
-  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:      -o-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:         linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
+  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
 }
 .progress-bar-warning {
   background-color: #f0ad4e;
 }
 .progress-striped .progress-bar-warning {
-  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:      -o-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:         linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
+  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
 }
 .progress-bar-danger {
   background-color: #d9534f;
 }
 .progress-striped .progress-bar-danger {
-  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:      -o-linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
-  background-image:         linear-gradient(45deg, rgba(255, 255, 255, .15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, .15) 50%, rgba(255, 255, 255, .15) 75%, transparent 75%, transparent);
+  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
+}
+.media {
+  margin-top: 15px;
+}
+.media:first-child {
+  margin-top: 0;
 }
 .media,
 .media-body {
   overflow: hidden;
   zoom: 1;
 }
-.media,
-.media .media {
-  margin-top: 15px;
-}
-.media:first-child {
-  margin-top: 0;
+.media-body {
+  width: 10000px;
 }
 .media-object {
   display: block;
 }
-.media-heading {
-  margin: 0 0 5px;
+.media-object.img-thumbnail {
+  max-width: none;
 }
+.media-right,
+.media > .pull-right {
+  padding-left: 10px;
+}
+.media-left,
 .media > .pull-left {
-  margin-right: 10px;
+  padding-right: 10px;
 }
-.media > .pull-right {
-  margin-left: 10px;
+.media-left,
+.media-right,
+.media-body {
+  display: table-cell;
+  vertical-align: top;
+}
+.media-middle {
+  vertical-align: middle;
+}
+.media-bottom {
+  vertical-align: bottom;
+}
+.media-heading {
+  margin-top: 0;
+  margin-bottom: 5px;
 }
 .media-list {
   padding-left: 0;
   list-style: none;
 }
 .list-group {
   padding-left: 0;
@@ -4834,55 +5334,38 @@
   border-top-right-radius: 4px;
 }
 .list-group-item:last-child {
   margin-bottom: 0;
   border-bottom-right-radius: 4px;
   border-bottom-left-radius: 4px;
 }
-.list-group-item > .badge {
-  float: right;
-}
-.list-group-item > .badge + .badge {
-  margin-right: 5px;
-}
-a.list-group-item {
-  color: #555;
-}
-a.list-group-item .list-group-item-heading {
-  color: #333;
-}
-a.list-group-item:hover,
-a.list-group-item:focus {
-  color: #555;
-  text-decoration: none;
-  background-color: #f5f5f5;
-}
 .list-group-item.disabled,
 .list-group-item.disabled:hover,
 .list-group-item.disabled:focus {
-  color: #777;
-  background-color: #eee;
+  color: #777777;
+  cursor: not-allowed;
+  background-color: #eeeeee;
 }
 .list-group-item.disabled .list-group-item-heading,
 .list-group-item.disabled:hover .list-group-item-heading,
 .list-group-item.disabled:focus .list-group-item-heading {
   color: inherit;
 }
 .list-group-item.disabled .list-group-item-text,
 .list-group-item.disabled:hover .list-group-item-text,
 .list-group-item.disabled:focus .list-group-item-text {
-  color: #777;
+  color: #777777;
 }
 .list-group-item.active,
 .list-group-item.active:hover,
 .list-group-item.active:focus {
   z-index: 2;
   color: #fff;
-  background-color: #428bca;
-  border-color: #428bca;
+  background-color: #337ab7;
+  border-color: #337ab7;
 }
 .list-group-item.active .list-group-item-heading,
 .list-group-item.active:hover .list-group-item-heading,
 .list-group-item.active:focus .list-group-item-heading,
 .list-group-item.active .list-group-item-heading > small,
 .list-group-item.active:hover .list-group-item-heading > small,
 .list-group-item.active:focus .list-group-item-heading > small,
@@ -4890,100 +5373,148 @@
 .list-group-item.active:hover .list-group-item-heading > .small,
 .list-group-item.active:focus .list-group-item-heading > .small {
   color: inherit;
 }
 .list-group-item.active .list-group-item-text,
 .list-group-item.active:hover .list-group-item-text,
 .list-group-item.active:focus .list-group-item-text {
-  color: #e1edf7;
+  color: #c7ddef;
+}
+a.list-group-item,
+button.list-group-item {
+  color: #555;
+}
+a.list-group-item .list-group-item-heading,
+button.list-group-item .list-group-item-heading {
+  color: #333;
+}
+a.list-group-item:hover,
+button.list-group-item:hover,
+a.list-group-item:focus,
+button.list-group-item:focus {
+  color: #555;
+  text-decoration: none;
+  background-color: #f5f5f5;
+}
+button.list-group-item {
+  width: 100%;
+  text-align: left;
 }
 .list-group-item-success {
   color: #3c763d;
   background-color: #dff0d8;
 }
-a.list-group-item-success {
+a.list-group-item-success,
+button.list-group-item-success {
   color: #3c763d;
 }
-a.list-group-item-success .list-group-item-heading {
+a.list-group-item-success .list-group-item-heading,
+button.list-group-item-success .list-group-item-heading {
   color: inherit;
 }
 a.list-group-item-success:hover,
-a.list-group-item-success:focus {
+button.list-group-item-success:hover,
+a.list-group-item-success:focus,
+button.list-group-item-success:focus {
   color: #3c763d;
   background-color: #d0e9c6;
 }
 a.list-group-item-success.active,
+button.list-group-item-success.active,
 a.list-group-item-success.active:hover,
-a.list-group-item-success.active:focus {
+button.list-group-item-success.active:hover,
+a.list-group-item-success.active:focus,
+button.list-group-item-success.active:focus {
   color: #fff;
   background-color: #3c763d;
   border-color: #3c763d;
 }
 .list-group-item-info {
   color: #31708f;
   background-color: #d9edf7;
 }
-a.list-group-item-info {
+a.list-group-item-info,
+button.list-group-item-info {
   color: #31708f;
 }
-a.list-group-item-info .list-group-item-heading {
+a.list-group-item-info .list-group-item-heading,
+button.list-group-item-info .list-group-item-heading {
   color: inherit;
 }
 a.list-group-item-info:hover,
-a.list-group-item-info:focus {
+button.list-group-item-info:hover,
+a.list-group-item-info:focus,
+button.list-group-item-info:focus {
   color: #31708f;
   background-color: #c4e3f3;
 }
 a.list-group-item-info.active,
+button.list-group-item-info.active,
 a.list-group-item-info.active:hover,
-a.list-group-item-info.active:focus {
+button.list-group-item-info.active:hover,
+a.list-group-item-info.active:focus,
+button.list-group-item-info.active:focus {
   color: #fff;
   background-color: #31708f;
   border-color: #31708f;
 }
 .list-group-item-warning {
   color: #8a6d3b;
   background-color: #fcf8e3;
 }
-a.list-group-item-warning {
+a.list-group-item-warning,
+button.list-group-item-warning {
   color: #8a6d3b;
 }
-a.list-group-item-warning .list-group-item-heading {
+a.list-group-item-warning .list-group-item-heading,
+button.list-group-item-warning .list-group-item-heading {
   color: inherit;
 }
 a.list-group-item-warning:hover,
-a.list-group-item-warning:focus {
+button.list-group-item-warning:hover,
+a.list-group-item-warning:focus,
+button.list-group-item-warning:focus {
   color: #8a6d3b;
   background-color: #faf2cc;
 }
 a.list-group-item-warning.active,
+button.list-group-item-warning.active,
 a.list-group-item-warning.active:hover,
-a.list-group-item-warning.active:focus {
+button.list-group-item-warning.active:hover,
+a.list-group-item-warning.active:focus,
+button.list-group-item-warning.active:focus {
   color: #fff;
   background-color: #8a6d3b;
   border-color: #8a6d3b;
 }
 .list-group-item-danger {
   color: #a94442;
   background-color: #f2dede;
 }
-a.list-group-item-danger {
+a.list-group-item-danger,
+button.list-group-item-danger {
   color: #a94442;
 }
-a.list-group-item-danger .list-group-item-heading {
+a.list-group-item-danger .list-group-item-heading,
+button.list-group-item-danger .list-group-item-heading {
   color: inherit;
 }
 a.list-group-item-danger:hover,
-a.list-group-item-danger:focus {
+button.list-group-item-danger:hover,
+a.list-group-item-danger:focus,
+button.list-group-item-danger:focus {
   color: #a94442;
   background-color: #ebcccc;
 }
 a.list-group-item-danger.active,
+button.list-group-item-danger.active,
 a.list-group-item-danger.active:hover,
-a.list-group-item-danger.active:focus {
+button.list-group-item-danger.active:hover,
+a.list-group-item-danger.active:focus,
+button.list-group-item-danger.active:focus {
   color: #fff;
   background-color: #a94442;
   border-color: #a94442;
 }
 .list-group-item-heading {
   margin-top: 0;
   margin-bottom: 5px;
@@ -4993,16 +5524,16 @@
   line-height: 1.3;
 }
 .panel {
   margin-bottom: 20px;
   background-color: #fff;
   border: 1px solid transparent;
   border-radius: 4px;
-  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, .05);
-          box-shadow: 0 1px 1px rgba(0, 0, 0, .05);
+  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
+  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
 }
 .panel-body {
   padding: 15px;
 }
 .panel-heading {
   padding: 10px 15px;
   border-bottom: 1px solid transparent;
@@ -5014,57 +5545,82 @@
 }
 .panel-title {
   margin-top: 0;
   margin-bottom: 0;
   font-size: 16px;
   color: inherit;
 }
-.panel-title > a {
+.panel-title > a,
+.panel-title > small,
+.panel-title > .small,
+.panel-title > small > a,
+.panel-title > .small > a {
   color: inherit;
 }
 .panel-footer {
   padding: 10px 15px;
   background-color: #f5f5f5;
   border-top: 1px solid #ddd;
   border-bottom-right-radius: 3px;
   border-bottom-left-radius: 3px;
 }
-.panel > .list-group {
+.panel > .list-group,
+.panel > .panel-collapse > .list-group {
   margin-bottom: 0;
 }
-.panel > .list-group .list-group-item {
+.panel > .list-group .list-group-item,
+.panel > .panel-collapse > .list-group .list-group-item {
   border-width: 1px 0;
   border-radius: 0;
 }
-.panel > .list-group:first-child .list-group-item:first-child {
+.panel > .list-group:first-child .list-group-item:first-child,
+.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
   border-top: 0;
   border-top-left-radius: 3px;
   border-top-right-radius: 3px;
 }
-.panel > .list-group:last-child .list-group-item:last-child {
+.panel > .list-group:last-child .list-group-item:last-child,
+.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
   border-bottom: 0;
   border-bottom-right-radius: 3px;
   border-bottom-left-radius: 3px;
 }
+.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
+  border-top-left-radius: 0;
+  border-top-right-radius: 0;
+}
 .panel-heading + .list-group .list-group-item:first-child {
   border-top-width: 0;
 }
 .list-group + .panel-footer {
   border-top-width: 0;
 }
 .panel > .table,
 .panel > .table-responsive > .table,
 .panel > .panel-collapse > .table {
   margin-bottom: 0;
 }
+.panel > .table caption,
+.panel > .table-responsive > .table caption,
+.panel > .panel-collapse > .table caption {
+  padding-right: 15px;
+  padding-left: 15px;
+}
 .panel > .table:first-child,
 .panel > .table-responsive:first-child > .table:first-child {
   border-top-left-radius: 3px;
   border-top-right-radius: 3px;
 }
+.panel > .table:first-child > thead:first-child > tr:first-child,
+.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
+.panel > .table:first-child > tbody:first-child > tr:first-child,
+.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
+  border-top-left-radius: 3px;
+  border-top-right-radius: 3px;
+}
 .panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
 .panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
 .panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
 .panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
 .panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
 .panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
 .panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
@@ -5082,14 +5638,21 @@
   border-top-right-radius: 3px;
 }
 .panel > .table:last-child,
 .panel > .table-responsive:last-child > .table:last-child {
   border-bottom-right-radius: 3px;
   border-bottom-left-radius: 3px;
 }
+.panel > .table:last-child > tbody:last-child > tr:last-child,
+.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
+.panel > .table:last-child > tfoot:last-child > tr:last-child,
+.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
+  border-bottom-right-radius: 3px;
+  border-bottom-left-radius: 3px;
+}
 .panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
 .panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
 .panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
 .panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
 .panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
 .panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
 .panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
@@ -5103,15 +5666,17 @@
 .panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
 .panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
 .panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
 .panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
   border-bottom-right-radius: 3px;
 }
 .panel > .panel-body + .table,
-.panel > .panel-body + .table-responsive {
+.panel > .panel-body + .table-responsive,
+.panel > .table + .panel-body,
+.panel > .table-responsive + .panel-body {
   border-top: 1px solid #ddd;
 }
 .panel > .table > tbody:first-child > tr:first-child th,
 .panel > .table > tbody:first-child > tr:first-child td {
   border-top: 0;
 }
 .panel > .table-bordered,
@@ -5179,58 +5744,59 @@
 }
 .panel-group .panel + .panel {
   margin-top: 5px;
 }
 .panel-group .panel-heading {
   border-bottom: 0;
 }
-.panel-group .panel-heading + .panel-collapse > .panel-body {
+.panel-group .panel-heading + .panel-collapse > .panel-body,
+.panel-group .panel-heading + .panel-collapse > .list-group {
   border-top: 1px solid #ddd;
 }
 .panel-group .panel-footer {
   border-top: 0;
 }
 .panel-group .panel-footer + .panel-collapse .panel-body {
   border-bottom: 1px solid #ddd;
 }
 .panel-default {
   border-color: #ddd;
 }
 .panel-default > .panel-heading {
-  color: #333;
+  color: #333333;
   background-color: #f5f5f5;
   border-color: #ddd;
 }
 .panel-default > .panel-heading + .panel-collapse > .panel-body {
   border-top-color: #ddd;
 }
 .panel-default > .panel-heading .badge {
   color: #f5f5f5;
-  background-color: #333;
+  background-color: #333333;
 }
 .panel-default > .panel-footer + .panel-collapse > .panel-body {
   border-bottom-color: #ddd;
 }
 .panel-primary {
-  border-color: #428bca;
+  border-color: #337ab7;
 }
 .panel-primary > .panel-heading {
   color: #fff;
-  background-color: #428bca;
-  border-color: #428bca;
+  background-color: #337ab7;
+  border-color: #337ab7;
 }
 .panel-primary > .panel-heading + .panel-collapse > .panel-body {
-  border-top-color: #428bca;
+  border-top-color: #337ab7;
 }
 .panel-primary > .panel-heading .badge {
-  color: #428bca;
+  color: #337ab7;
   background-color: #fff;
 }
 .panel-primary > .panel-footer + .panel-collapse > .panel-body {
-  border-bottom-color: #428bca;
+  border-bottom-color: #337ab7;
 }
 .panel-success {
   border-color: #d6e9c6;
 }
 .panel-success > .panel-heading {
   color: #3c763d;
   background-color: #dff0d8;
@@ -5306,42 +5872,43 @@
   height: 0;
   padding: 0;
   overflow: hidden;
 }
 .embed-responsive .embed-responsive-item,
 .embed-responsive iframe,
 .embed-responsive embed,
-.embed-responsive object {
+.embed-responsive object,
+.embed-responsive video {
   position: absolute;
   top: 0;
   bottom: 0;
   left: 0;
   width: 100%;
   height: 100%;
   border: 0;
 }
-.embed-responsive.embed-responsive-16by9 {
+.embed-responsive-16by9 {
   padding-bottom: 56.25%;
 }
-.embed-responsive.embed-responsive-4by3 {
+.embed-responsive-4by3 {
   padding-bottom: 75%;
 }
 .well {
   min-height: 20px;
   padding: 19px;
   margin-bottom: 20px;
   background-color: #f5f5f5;
   border: 1px solid #e3e3e3;
   border-radius: 4px;
-  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .05);
-          box-shadow: inset 0 1px 1px rgba(0, 0, 0, .05);
+  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
+  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
 }
 .well blockquote {
   border-color: #ddd;
-  border-color: rgba(0, 0, 0, .15);
+  border-color: rgba(0, 0, 0, 0.15);
 }
 .well-lg {
   padding: 24px;
   border-radius: 6px;
 }
 .well-sm {
   padding: 9px;
@@ -5351,30 +5918,32 @@
   float: right;
   font-size: 21px;
   font-weight: bold;
   line-height: 1;
   color: #000;
   text-shadow: 0 1px 0 #fff;
   filter: alpha(opacity=20);
-  opacity: .2;
+  opacity: 0.2;
 }
 .close:hover,
 .close:focus {
   color: #000;
   text-decoration: none;
   cursor: pointer;
   filter: alpha(opacity=50);
-  opacity: .5;
+  opacity: 0.5;
 }
 button.close {
-  -webkit-appearance: none;
   padding: 0;
   cursor: pointer;
   background: transparent;
   border: 0;
+  -webkit-appearance: none;
+  -moz-appearance: none;
+  appearance: none;
 }
 .modal-open {
   overflow: hidden;
 }
 .modal {
   position: fixed;
   top: 0;
@@ -5384,46 +5953,49 @@
   z-index: 1050;
   display: none;
   overflow: hidden;
   -webkit-overflow-scrolling: touch;
   outline: 0;
 }
 .modal.fade .modal-dialog {
-  -webkit-transition: -webkit-transform .3s ease-out;
-       -o-transition:      -o-transform .3s ease-out;
-          transition:         transform .3s ease-out;
-  -webkit-transform: translate3d(0, -25%, 0);
-       -o-transform: translate3d(0, -25%, 0);
-          transform: translate3d(0, -25%, 0);
+  -webkit-transform: translate(0, -25%);
+  -ms-transform: translate(0, -25%);
+  -o-transform: translate(0, -25%);
+  transform: translate(0, -25%);
+  -webkit-transition: -webkit-transform 0.3s ease-out;
+  -o-transition: -o-transform 0.3s ease-out;
+  transition: -webkit-transform 0.3s ease-out;
+  transition: transform 0.3s ease-out;
+  transition: transform 0.3s ease-out, -webkit-transform 0.3s ease-out, -o-transform 0.3s ease-out;
 }
 .modal.in .modal-dialog {
-  -webkit-transform: translate3d(0, 0, 0);
-       -o-transform: translate3d(0, 0, 0);
-          transform: translate3d(0, 0, 0);
+  -webkit-transform: translate(0, 0);
+  -ms-transform: translate(0, 0);
+  -o-transform: translate(0, 0);
+  transform: translate(0, 0);
 }
 .modal-open .modal {
   overflow-x: hidden;
   overflow-y: auto;
 }
 .modal-dialog {
   position: relative;
   width: auto;
   margin: 10px;
 }
 .modal-content {
   position: relative;
   background-color: #fff;
-  -webkit-background-clip: padding-box;
-          background-clip: padding-box;
+  background-clip: padding-box;
   border: 1px solid #999;
-  border: 1px solid rgba(0, 0, 0, .2);
+  border: 1px solid rgba(0, 0, 0, 0.2);
   border-radius: 6px;
+  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
+  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
   outline: 0;
-  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, .5);
-          box-shadow: 0 3px 9px rgba(0, 0, 0, .5);
 }
 .modal-backdrop {
   position: fixed;
   top: 0;
   right: 0;
   bottom: 0;
   left: 0;
@@ -5432,18 +6004,17 @@
 }
 .modal-backdrop.fade {
   filter: alpha(opacity=0);
   opacity: 0;
 }
 .modal-backdrop.in {
   filter: alpha(opacity=50);
-  opacity: .5;
+  opacity: 0.5;
 }
 .modal-header {
-  min-height: 16.42857143px;
   padding: 15px;
   border-bottom: 1px solid #e5e5e5;
 }
 .modal-header .close {
   margin-top: -2px;
 }
 .modal-title {
@@ -5478,39 +6049,52 @@
 }
 @media (min-width: 768px) {
   .modal-dialog {
     width: 600px;
     margin: 30px auto;
   }
   .modal-content {
-    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, .5);
-            box-shadow: 0 5px 15px rgba(0, 0, 0, .5);
+    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
+    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
   }
   .modal-sm {
     width: 300px;
   }
 }
 @media (min-width: 992px) {
   .modal-lg {
     width: 900px;
   }
 }
 .tooltip {
   position: absolute;
   z-index: 1070;
   display: block;
+  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
+  font-style: normal;
+  font-weight: 400;
+  line-height: 1.42857143;
+  line-break: auto;
+  text-align: left;
+  text-align: start;
+  text-decoration: none;
+  text-shadow: none;
+  text-transform: none;
+  letter-spacing: normal;
+  word-break: normal;
+  word-spacing: normal;
+  word-wrap: normal;
+  white-space: normal;
   font-size: 12px;
-  line-height: 1.4;
-  visibility: visible;
   filter: alpha(opacity=0);
   opacity: 0;
 }
 .tooltip.in {
   filter: alpha(opacity=90);
-  opacity: .9;
+  opacity: 0.9;
 }
 .tooltip.top {
   padding: 5px 0;
   margin-top: -3px;
 }
 .tooltip.right {
   padding: 0 5px;
@@ -5520,46 +6104,32 @@
   padding: 5px 0;
   margin-top: 3px;
 }
 .tooltip.left {
   padding: 0 5px;
   margin-left: -3px;
 }
-.tooltip-inner {
-  max-width: 200px;
-  padding: 3px 8px;
-  color: #fff;
-  text-align: center;
-  text-decoration: none;
-  background-color: #000;
-  border-radius: 4px;
-}
-.tooltip-arrow {
-  position: absolute;
-  width: 0;
-  height: 0;
-  border-color: transparent;
-  border-style: solid;
-}
 .tooltip.top .tooltip-arrow {
   bottom: 0;
   left: 50%;
   margin-left: -5px;
   border-width: 5px 5px 0;
   border-top-color: #000;
 }
 .tooltip.top-left .tooltip-arrow {
+  right: 5px;
   bottom: 0;
-  left: 5px;
+  margin-bottom: -5px;
   border-width: 5px 5px 0;
   border-top-color: #000;
 }
 .tooltip.top-right .tooltip-arrow {
-  right: 5px;
   bottom: 0;
+  left: 5px;
+  margin-bottom: -5px;
   border-width: 5px 5px 0;
   border-top-color: #000;
 }
 .tooltip.right .tooltip-arrow {
   top: 50%;
   left: 0;
   margin-top: -5px;
@@ -5578,163 +6148,223 @@
   left: 50%;
   margin-left: -5px;
   border-width: 0 5px 5px;
   border-bottom-color: #000;
 }
 .tooltip.bottom-left .tooltip-arrow {
   top: 0;
-  left: 5px;
+  right: 5px;
+  margin-top: -5px;
   border-width: 0 5px 5px;
   border-bottom-color: #000;
 }
 .tooltip.bottom-right .tooltip-arrow {
   top: 0;
-  right: 5px;
+  left: 5px;
+  margin-top: -5px;
   border-width: 0 5px 5px;
   border-bottom-color: #000;
 }
+.tooltip-inner {
+  max-width: 200px;
+  padding: 3px 8px;
+  color: #fff;
+  text-align: center;
+  background-color: #000;
+  border-radius: 4px;
+}
+.tooltip-arrow {
+  position: absolute;
+  width: 0;
+  height: 0;
+  border-color: transparent;
+  border-style: solid;
+}
 .popover {
   position: absolute;
   top: 0;
   left: 0;
   z-index: 1060;
   display: none;
   max-width: 276px;
   padding: 1px;
+  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
+  font-style: normal;
+  font-weight: 400;
+  line-height: 1.42857143;
+  line-break: auto;
   text-align: left;
+  text-align: start;
+  text-decoration: none;
+  text-shadow: none;
+  text-transform: none;
+  letter-spacing: normal;
+  word-break: normal;
+  word-spacing: normal;
+  word-wrap: normal;
   white-space: normal;
+  font-size: 14px;
   background-color: #fff;
-  -webkit-background-clip: padding-box;
-          background-clip: padding-box;
+  background-clip: padding-box;
   border: 1px solid #ccc;
-  border: 1px solid rgba(0, 0, 0, .2);
+  border: 1px solid rgba(0, 0, 0, 0.2);
   border-radius: 6px;
-  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, .2);
-          box-shadow: 0 5px 10px rgba(0, 0, 0, .2);
+  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
+  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
 }
 .popover.top {
   margin-top: -10px;
 }
 .popover.right {
   margin-left: 10px;
 }
 .popover.bottom {
   margin-top: 10px;
 }
 .popover.left {
   margin-left: -10px;
 }
-.popover-title {
-  padding: 8px 14px;
-  margin: 0;
-  font-size: 14px;
-  font-weight: normal;
-  line-height: 18px;
-  background-color: #f7f7f7;
-  border-bottom: 1px solid #ebebeb;
-  border-radius: 5px 5px 0 0;
-}
-.popover-content {
-  padding: 9px 14px;
+.popover > .arrow {
+  border-width: 11px;
 }
 .popover > .arrow,
 .popover > .arrow:after {
   position: absolute;
   display: block;
   width: 0;
   height: 0;
   border-color: transparent;
   border-style: solid;
 }
-.popover > .arrow {
-  border-width: 11px;
-}
 .popover > .arrow:after {
   content: "";
   border-width: 10px;
 }
 .popover.top > .arrow {
   bottom: -11px;
   left: 50%;
   margin-left: -11px;
-  border-top-color: #999;
-  border-top-color: rgba(0, 0, 0, .25);
+  border-top-color: #999999;
+  border-top-color: rgba(0, 0, 0, 0.25);
   border-bottom-width: 0;
 }
 .popover.top > .arrow:after {
   bottom: 1px;
   margin-left: -10px;
   content: " ";
   border-top-color: #fff;
   border-bottom-width: 0;
 }
 .popover.right > .arrow {
   top: 50%;
   left: -11px;
   margin-top: -11px;
-  border-right-color: #999;
-  border-right-color: rgba(0, 0, 0, .25);
+  border-right-color: #999999;
+  border-right-color: rgba(0, 0, 0, 0.25);
   border-left-width: 0;
 }
 .popover.right > .arrow:after {
   bottom: -10px;
   left: 1px;
   content: " ";
   border-right-color: #fff;
   border-left-width: 0;
 }
 .popover.bottom > .arrow {
   top: -11px;
   left: 50%;
   margin-left: -11px;
   border-top-width: 0;
-  border-bottom-color: #999;
-  border-bottom-color: rgba(0, 0, 0, .25);
+  border-bottom-color: #999999;
+  border-bottom-color: rgba(0, 0, 0, 0.25);
 }
 .popover.bottom > .arrow:after {
   top: 1px;
   margin-left: -10px;
   content: " ";
   border-top-width: 0;
   border-bottom-color: #fff;
 }
 .popover.left > .arrow {
   top: 50%;
   right: -11px;
   margin-top: -11px;
   border-right-width: 0;
-  border-left-color: #999;
-  border-left-color: rgba(0, 0, 0, .25);
+  border-left-color: #999999;
+  border-left-color: rgba(0, 0, 0, 0.25);
 }
 .popover.left > .arrow:after {
   right: 1px;
   bottom: -10px;
   content: " ";
   border-right-width: 0;
   border-left-color: #fff;
 }
+.popover-title {
+  padding: 8px 14px;
+  margin: 0;
+  font-size: 14px;
+  background-color: #f7f7f7;
+  border-bottom: 1px solid #ebebeb;
+  border-radius: 5px 5px 0 0;
+}
+.popover-content {
+  padding: 9px 14px;
+}
 .carousel {
   position: relative;
 }
 .carousel-inner {
   position: relative;
   width: 100%;
   overflow: hidden;
 }
 .carousel-inner > .item {
   position: relative;
   display: none;
-  -webkit-transition: .6s ease-in-out left;
-       -o-transition: .6s ease-in-out left;
-          transition: .6s ease-in-out left;
+  -webkit-transition: 0.6s ease-in-out left;
+  -o-transition: 0.6s ease-in-out left;
+  transition: 0.6s ease-in-out left;
 }
 .carousel-inner > .item > img,
 .carousel-inner > .item > a > img {
   line-height: 1;
 }
+@media all and (transform-3d), (-webkit-transform-3d) {
+  .carousel-inner > .item {
+    -webkit-transition: -webkit-transform 0.6s ease-in-out;
+    -o-transition: -o-transform 0.6s ease-in-out;
+    transition: -webkit-transform 0.6s ease-in-out;
+    transition: transform 0.6s ease-in-out;
+    transition: transform 0.6s ease-in-out, -webkit-transform 0.6s ease-in-out, -o-transform 0.6s ease-in-out;
+    -webkit-backface-visibility: hidden;
+    backface-visibility: hidden;
+    -webkit-perspective: 1000px;
+    perspective: 1000px;
+  }
+  .carousel-inner > .item.next,
+  .carousel-inner > .item.active.right {
+    -webkit-transform: translate3d(100%, 0, 0);
+    transform: translate3d(100%, 0, 0);
+    left: 0;
+  }
+  .carousel-inner > .item.prev,
+  .carousel-inner > .item.active.left {
+    -webkit-transform: translate3d(-100%, 0, 0);
+    transform: translate3d(-100%, 0, 0);
+    left: 0;
+  }
+  .carousel-inner > .item.next.left,
+  .carousel-inner > .item.prev.right,
+  .carousel-inner > .item.active {
+    -webkit-transform: translate3d(0, 0, 0);
+    transform: translate3d(0, 0, 0);
+    left: 0;
+  }
+}
 .carousel-inner > .active,
 .carousel-inner > .next,
 .carousel-inner > .prev {
   display: block;
 }
 .carousel-inner > .active {
   left: 0;
@@ -5766,52 +6396,54 @@
   top: 0;
   bottom: 0;
   left: 0;
   width: 15%;
   font-size: 20px;
   color: #fff;
   text-align: center;
-  text-shadow: 0 1px 2px rgba(0, 0, 0, .6);
+  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
+  background-color: rgba(0, 0, 0, 0);
   filter: alpha(opacity=50);
-  opacity: .5;
+  opacity: 0.5;
 }
 .carousel-control.left {
-  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, .5) 0%, rgba(0, 0, 0, .0001) 100%);
-  background-image:      -o-linear-gradient(left, rgba(0, 0, 0, .5) 0%, rgba(0, 0, 0, .0001) 100%);
-  background-image: -webkit-gradient(linear, left top, right top, from(rgba(0, 0, 0, .5)), to(rgba(0, 0, 0, .0001)));
-  background-image:         linear-gradient(to right, rgba(0, 0, 0, .5) 0%, rgba(0, 0, 0, .0001) 100%);
+  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
+  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
+  background-image: -webkit-gradient(linear, left top, right top, from(rgba(0, 0, 0, 0.5)), to(rgba(0, 0, 0, 0.0001)));
+  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
   filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
   background-repeat: repeat-x;
 }
 .carousel-control.right {
   right: 0;
   left: auto;
-  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, .0001) 0%, rgba(0, 0, 0, .5) 100%);
-  background-image:      -o-linear-gradient(left, rgba(0, 0, 0, .0001) 0%, rgba(0, 0, 0, .5) 100%);
-  background-image: -webkit-gradient(linear, left top, right top, from(rgba(0, 0, 0, .0001)), to(rgba(0, 0, 0, .5)));
-  background-image:         linear-gradient(to right, rgba(0, 0, 0, .0001) 0%, rgba(0, 0, 0, .5) 100%);
+  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
+  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
+  background-image: -webkit-gradient(linear, left top, right top, from(rgba(0, 0, 0, 0.0001)), to(rgba(0, 0, 0, 0.5)));
+  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
   filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
   background-repeat: repeat-x;
 }
 .carousel-control:hover,
 .carousel-control:focus {
   color: #fff;
   text-decoration: none;
-  filter: alpha(opacity=90);
   outline: 0;
-  opacity: .9;
+  filter: alpha(opacity=90);
+  opacity: 0.9;
 }
 .carousel-control .icon-prev,
 .carousel-control .icon-next,
 .carousel-control .glyphicon-chevron-left,
 .carousel-control .glyphicon-chevron-right {
   position: absolute;
   top: 50%;
   z-index: 5;
   display: inline-block;
+  margin-top: -10px;
 }
 .carousel-control .icon-prev,
 .carousel-control .glyphicon-chevron-left {
   left: 50%;
   margin-left: -10px;
 }
 .carousel-control .icon-next,
@@ -5819,22 +6451,22 @@
   right: 50%;
   margin-right: -10px;
 }
 .carousel-control .icon-prev,
 .carousel-control .icon-next {
   width: 20px;
   height: 20px;
-  margin-top: -10px;
   font-family: serif;
+  line-height: 1;
 }
 .carousel-control .icon-prev:before {
-  content: '\2039';
+  content: "\2039";
 }
 .carousel-control .icon-next:before {
-  content: '\203a';
+  content: "\203a";
 }
 .carousel-indicators {
   position: absolute;
   bottom: 10px;
   left: 50%;
   z-index: 15;
   width: 60%;
@@ -5867,36 +6499,36 @@
   bottom: 20px;
   left: 15%;
   z-index: 10;
   padding-top: 20px;
   padding-bottom: 20px;
   color: #fff;
   text-align: center;
-  text-shadow: 0 1px 2px rgba(0, 0, 0, .6);
+  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
 }
 .carousel-caption .btn {
   text-shadow: none;
 }
 @media screen and (min-width: 768px) {
   .carousel-control .glyphicon-chevron-left,
   .carousel-control .glyphicon-chevron-right,
   .carousel-control .icon-prev,
   .carousel-control .icon-next {
     width: 30px;
     height: 30px;
-    margin-top: -15px;
+    margin-top: -10px;
     font-size: 30px;
   }
   .carousel-control .glyphicon-chevron-left,
   .carousel-control .icon-prev {
-    margin-left: -15px;
+    margin-left: -10px;
   }
   .carousel-control .glyphicon-chevron-right,
   .carousel-control .icon-next {
-    margin-right: -15px;
+    margin-right: -10px;
   }
   .carousel-caption {
     right: 20%;
     left: 20%;
     padding-bottom: 30px;
   }
   .carousel-indicators {
@@ -5927,14 +6559,16 @@
 .navbar-header:after,
 .navbar-collapse:before,
 .navbar-collapse:after,
 .pager:before,
 .pager:after,
 .panel-body:before,
 .panel-body:after,
+.modal-header:before,
+.modal-header:after,
 .modal-footer:before,
 .modal-footer:after {
   display: table;
   content: " ";
 }
 .clearfix:after,
 .dl-horizontal dd:after,
@@ -5946,14 +6580,15 @@
 .btn-group-vertical > .btn-group:after,
 .nav:after,
 .navbar:after,
 .navbar-header:after,
 .navbar-collapse:after,
 .pager:after,
 .panel-body:after,
+.modal-header:after,
 .modal-footer:after {
   clear: both;
 }
 .center-block {
   display: block;
   margin-right: auto;
   margin-left: auto;
@@ -5978,21 +6613,17 @@
   color: transparent;
   text-shadow: none;
   background-color: transparent;
   border: 0;
 }
 .hidden {
   display: none !important;
-  visibility: hidden !important;
 }
 .affix {
   position: fixed;
-  -webkit-transform: translate3d(0, 0, 0);
-       -o-transform: translate3d(0, 0, 0);
-          transform: translate3d(0, 0, 0);
 }
 @-ms-viewport {
   width: device-width;
 }
 .visible-xs,
 .visible-sm,
 .visible-md,
@@ -6014,15 +6645,15 @@
   display: none !important;
 }
 @media (max-width: 767px) {
   .visible-xs {
     display: block !important;
   }
   table.visible-xs {
-    display: table;
+    display: table !important;
   }
   tr.visible-xs {
     display: table-row !important;
   }
   th.visible-xs,
   td.visible-xs {
     display: table-cell !important;
@@ -6044,15 +6675,15 @@
   }
 }
 @media (min-width: 768px) and (max-width: 991px) {
   .visible-sm {
     display: block !important;
   }
   table.visible-sm {
-    display: table;
+    display: table !important;
   }
   tr.visible-sm {
     display: table-row !important;
   }
   th.visible-sm,
   td.visible-sm {
     display: table-cell !important;
@@ -6074,15 +6705,15 @@
   }
 }
 @media (min-width: 992px) and (max-width: 1199px) {
   .visible-md {
     display: block !important;
   }
   table.visible-md {
-    display: table;
+    display: table !important;
   }
   tr.visible-md {
     display: table-row !important;
   }
   th.visible-md,
   td.visible-md {
     display: table-cell !important;
@@ -6104,15 +6735,15 @@
   }
 }
 @media (min-width: 1200px) {
   .visible-lg {
     display: block !important;
   }
   table.visible-lg {
-    display: table;
+    display: table !important;
   }
   tr.visible-lg {
     display: table-row !important;
   }
   th.visible-lg,
   td.visible-lg {
     display: table-cell !important;
@@ -6157,15 +6788,15 @@
   display: none !important;
 }
 @media print {
   .visible-print {
     display: block !important;
   }
   table.visible-print {
-    display: table;
+    display: table !important;
   }
   tr.visible-print {
     display: table-row !important;
   }
   th.visible-print,
   td.visible-print {
     display: table-cell !important;
@@ -6196,8 +6827,8 @@
   }
 }
 @media print {
   .hidden-print {
     display: none !important;
   }
 }
-/*# sourceMappingURL=bootstrap.css.map */
+/*# sourceMappingURL=bootstrap.css.map */
```

### Comparing `yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/css/bootstrap.min.css` & `yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/css/bootstrap.min.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,5 +1,6 @@
 /*!
- * Bootstrap v3.2.0 (http://getbootstrap.com)
- * Copyright 2011-2014 Twitter, Inc.
+ * Bootstrap v3.4.1 (https://getbootstrap.com/)
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
- *//*! normalize.css v3.0.1 | MIT License | git.io/normalize */html{font-family:sans-serif;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background:0 0}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{margin:.67em 0;font-size:2em}mark{color:#000;background:#ff0}small{font-size:80%}sub,sup{position:relative;font-size:75%;line-height:0;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{height:0;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{margin:0;font:inherit;color:inherit}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{padding:0;border:0}input{line-height:normal}input[type=checkbox],input[type=radio]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;-webkit-appearance:textfield}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{padding:.35em .625em .75em;margin:0 2px;border:1px solid silver}legend{padding:0;border:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-spacing:0;border-collapse:collapse}td,th{padding:0}@media print{*{color:#000!important;text-shadow:none!important;background:transparent!important;-webkit-box-shadow:none!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100%!important}p,h2,h3{orphans:3;widows:3}h2,h3{page-break-after:avoid}select{background:#fff!important}.navbar{display:none}.table td,.table th{background-color:#fff!important}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table-bordered th,.table-bordered td{border:1px solid #ddd!important}}@font-face{font-family:'Glyphicons Halflings';src:url(../fonts/glyphicons-halflings-regular.eot);src:url(../fonts/glyphicons-halflings-regular.eot?#iefix) format('embedded-opentype'),url(../fonts/glyphicons-halflings-regular.woff) format('woff'),url(../fonts/glyphicons-halflings-regular.ttf) format('truetype'),url(../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular) format('svg')}.glyphicon{position:relative;top:1px;display:inline-block;font-family:'Glyphicons Halflings';font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\2a"}.glyphicon-plus:before{content:"\2b"}.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:before,:after{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:rgba(0,0,0,0)}body{font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}input,button,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#428bca;text-decoration:none}a:hover,a:focus{color:#2a6496;text-decoration:underline}a:focus{outline:thin dotted;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.img-responsive,.thumbnail>img,.thumbnail a>img,.carousel-inner>.item>img,.carousel-inner>.item>a>img{display:block;width:100% \9;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{display:inline-block;width:100% \9;max-width:100%;height:auto;padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}h1,h2,h3,h4,h5,h6,.h1,.h2,.h3,.h4,.h5,.h6{font-family:inherit;font-weight:500;line-height:1.1;color:inherit}h1 small,h2 small,h3 small,h4 small,h5 small,h6 small,.h1 small,.h2 small,.h3 small,.h4 small,.h5 small,.h6 small,h1 .small,h2 .small,h3 .small,h4 .small,h5 .small,h6 .small,.h1 .small,.h2 .small,.h3 .small,.h4 .small,.h5 .small,.h6 .small{font-weight:400;line-height:1;color:#777}h1,.h1,h2,.h2,h3,.h3{margin-top:20px;margin-bottom:10px}h1 small,.h1 small,h2 small,.h2 small,h3 small,.h3 small,h1 .small,.h1 .small,h2 .small,.h2 .small,h3 .small,.h3 .small{font-size:65%}h4,.h4,h5,.h5,h6,.h6{margin-top:10px;margin-bottom:10px}h4 small,.h4 small,h5 small,.h5 small,h6 small,.h6 small,h4 .small,.h4 .small,h5 .small,.h5 .small,h6 .small,.h6 .small{font-size:75%}h1,.h1{font-size:36px}h2,.h2{font-size:30px}h3,.h3{font-size:24px}h4,.h4{font-size:18px}h5,.h5{font-size:14px}h6,.h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}small,.small{font-size:85%}cite{font-style:normal}mark,.mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#777}.text-primary{color:#428bca}a.text-primary:hover{color:#3071a9}.text-success{color:#3c763d}a.text-success:hover{color:#2b542c}.text-info{color:#31708f}a.text-info:hover{color:#245269}.text-warning{color:#8a6d3b}a.text-warning:hover{color:#66512c}.text-danger{color:#a94442}a.text-danger:hover{color:#843534}.bg-primary{color:#fff;background-color:#428bca}a.bg-primary:hover{background-color:#3071a9}.bg-success{background-color:#dff0d8}a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ul,ol{margin-top:0;margin-bottom:10px}ul ul,ol ul,ul ol,ol ol{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;margin-left:-5px;list-style:none}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dt,dd{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;overflow:hidden;clear:left;text-align:right;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[title],abbr[data-original-title]{cursor:help;border-bottom:1px dotted #777}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote p:last-child,blockquote ul:last-child,blockquote ol:last-child{margin-bottom:0}blockquote footer,blockquote small,blockquote .small{display:block;font-size:80%;line-height:1.42857143;color:#777}blockquote footer:before,blockquote small:before,blockquote .small:before{content:'\2014 \00A0'}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse footer:before,blockquote.pull-right footer:before,.blockquote-reverse small:before,blockquote.pull-right small:before,.blockquote-reverse .small:before,blockquote.pull-right .small:before{content:''}.blockquote-reverse footer:after,blockquote.pull-right footer:after,.blockquote-reverse small:after,blockquote.pull-right small:after,.blockquote-reverse .small:after,blockquote.pull-right .small:after{content:'\00A0 \2014'}blockquote:before,blockquote:after{content:""}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.25);box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;-webkit-box-shadow:none;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.col-xs-1,.col-sm-1,.col-md-1,.col-lg-1,.col-xs-2,.col-sm-2,.col-md-2,.col-lg-2,.col-xs-3,.col-sm-3,.col-md-3,.col-lg-3,.col-xs-4,.col-sm-4,.col-md-4,.col-lg-4,.col-xs-5,.col-sm-5,.col-md-5,.col-lg-5,.col-xs-6,.col-sm-6,.col-md-6,.col-lg-6,.col-xs-7,.col-sm-7,.col-md-7,.col-lg-7,.col-xs-8,.col-sm-8,.col-md-8,.col-lg-8,.col-xs-9,.col-sm-9,.col-md-9,.col-lg-9,.col-xs-10,.col-sm-10,.col-md-10,.col-lg-10,.col-xs-11,.col-sm-11,.col-md-11,.col-lg-11,.col-xs-12,.col-sm-12,.col-md-12,.col-lg-12{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9,.col-xs-10,.col-xs-11,.col-xs-12{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-sm-10,.col-sm-11,.col-sm-12{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-md-10,.col-md-11,.col-md-12{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-lg-10,.col-lg-11,.col-lg-12{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>thead>tr>th,.table>tbody>tr>th,.table>tfoot>tr>th,.table>thead>tr>td,.table>tbody>tr>td,.table>tfoot>tr>td{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>th,.table>caption+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>td,.table>thead:first-child>tr:first-child>td{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>thead>tr>th,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>tbody>tr>td,.table-condensed>tfoot>tr>td{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>thead>tr>th,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>tbody>tr>td,.table-bordered>tfoot>tr>td{border:1px solid #ddd}.table-bordered>thead>tr>th,.table-bordered>thead>tr>td{border-bottom-width:2px}.table-striped>tbody>tr:nth-child(odd)>td,.table-striped>tbody>tr:nth-child(odd)>th{background-color:#f9f9f9}.table-hover>tbody>tr:hover>td,.table-hover>tbody>tr:hover>th{background-color:#f5f5f5}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}.table>thead>tr>td.active,.table>tbody>tr>td.active,.table>tfoot>tr>td.active,.table>thead>tr>th.active,.table>tbody>tr>th.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>tbody>tr.active>td,.table>tfoot>tr.active>td,.table>thead>tr.active>th,.table>tbody>tr.active>th,.table>tfoot>tr.active>th{background-color:#f5f5f5}.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover,.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr.active:hover>th{background-color:#e8e8e8}.table>thead>tr>td.success,.table>tbody>tr>td.success,.table>tfoot>tr>td.success,.table>thead>tr>th.success,.table>tbody>tr>th.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>tbody>tr.success>td,.table>tfoot>tr.success>td,.table>thead>tr.success>th,.table>tbody>tr.success>th,.table>tfoot>tr.success>th{background-color:#dff0d8}.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover,.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr.success:hover>th{background-color:#d0e9c6}.table>thead>tr>td.info,.table>tbody>tr>td.info,.table>tfoot>tr>td.info,.table>thead>tr>th.info,.table>tbody>tr>th.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>tbody>tr.info>td,.table>tfoot>tr.info>td,.table>thead>tr.info>th,.table>tbody>tr.info>th,.table>tfoot>tr.info>th{background-color:#d9edf7}.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover,.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr.info:hover>th{background-color:#c4e3f3}.table>thead>tr>td.warning,.table>tbody>tr>td.warning,.table>tfoot>tr>td.warning,.table>thead>tr>th.warning,.table>tbody>tr>th.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>tbody>tr.warning>td,.table>tfoot>tr.warning>td,.table>thead>tr.warning>th,.table>tbody>tr.warning>th,.table>tfoot>tr.warning>th{background-color:#fcf8e3}.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover,.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr.warning:hover>th{background-color:#faf2cc}.table>thead>tr>td.danger,.table>tbody>tr>td.danger,.table>tfoot>tr>td.danger,.table>thead>tr>th.danger,.table>tbody>tr>th.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>tbody>tr.danger>td,.table>tfoot>tr.danger>td,.table>thead>tr.danger>th,.table>tbody>tr.danger>th,.table>tfoot>tr.danger>th{background-color:#f2dede}.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover,.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr.danger:hover>th{background-color:#ebcccc}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-x:auto;overflow-y:hidden;-webkit-overflow-scrolling:touch;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>thead>tr>th,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tfoot>tr>td{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>thead>tr>th:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child{border-left:0}.table-responsive>.table-bordered>thead>tr>th:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>th,.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>td{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}input[type=radio],input[type=checkbox]{margin:4px 0 0;margin-top:1px \9;line-height:normal}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=file]:focus,input[type=radio]:focus,input[type=checkbox]:focus{outline:thin dotted;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:7px;font-size:14px;line-height:1.42857143;color:#555}.form-control{display:block;width:100%;height:34px;padding:6px 12px;font-size:14px;line-height:1.42857143;color:#555;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#777;opacity:1}.form-control:-ms-input-placeholder{color:#777}.form-control::-webkit-input-placeholder{color:#777}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{cursor:not-allowed;background-color:#eee;opacity:1}textarea.form-control{height:auto}input[type=search]{-webkit-appearance:none}input[type=date],input[type=time],input[type=datetime-local],input[type=month]{line-height:34px;line-height:1.42857143 \0}input[type=date].input-sm,input[type=time].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm{line-height:30px}input[type=date].input-lg,input[type=time].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg{line-height:46px}.form-group{margin-bottom:15px}.radio,.checkbox{position:relative;display:block;min-height:20px;margin-top:10px;margin-bottom:10px}.radio label,.checkbox label{padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.radio input[type=radio],.radio-inline input[type=radio],.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox]{position:absolute;margin-top:4px \9;margin-left:-20px}.radio+.radio,.checkbox+.checkbox{margin-top:-5px}.radio-inline,.checkbox-inline{display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.radio-inline+.radio-inline,.checkbox-inline+.checkbox-inline{margin-top:0;margin-left:10px}input[type=radio][disabled],input[type=checkbox][disabled],input[type=radio].disabled,input[type=checkbox].disabled,fieldset[disabled] input[type=radio],fieldset[disabled] input[type=checkbox]{cursor:not-allowed}.radio-inline.disabled,.checkbox-inline.disabled,fieldset[disabled] .radio-inline,fieldset[disabled] .checkbox-inline{cursor:not-allowed}.radio.disabled label,.checkbox.disabled label,fieldset[disabled] .radio label,fieldset[disabled] .checkbox label{cursor:not-allowed}.form-control-static{padding-top:7px;padding-bottom:7px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm,.form-horizontal .form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}textarea.input-sm,select[multiple].input-sm{height:auto}.input-lg,.form-horizontal .form-group-lg .form-control{height:46px;padding:10px 16px;font-size:18px;line-height:1.33;border-radius:6px}select.input-lg{height:46px;line-height:46px}textarea.input-lg,select[multiple].input-lg{height:auto}.has-feedback{position:relative}.has-feedback .form-control{padding-right:42.5px}.form-control-feedback{position:absolute;top:25px;right:0;z-index:2;display:block;width:34px;height:34px;line-height:34px;text-align:center}.input-lg+.form-control-feedback{width:46px;height:46px;line-height:46px}.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .help-block,.has-success .control-label,.has-success .radio,.has-success .checkbox,.has-success .radio-inline,.has-success .checkbox-inline{color:#3c763d}.has-success .form-control{border-color:#3c763d;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#2b542c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168}.has-success .input-group-addon{color:#3c763d;background-color:#dff0d8;border-color:#3c763d}.has-success .form-control-feedback{color:#3c763d}.has-warning .help-block,.has-warning .control-label,.has-warning .radio,.has-warning .checkbox,.has-warning .radio-inline,.has-warning .checkbox-inline{color:#8a6d3b}.has-warning .form-control{border-color:#8a6d3b;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#66512c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b}.has-warning .input-group-addon{color:#8a6d3b;background-color:#fcf8e3;border-color:#8a6d3b}.has-warning .form-control-feedback{color:#8a6d3b}.has-error .help-block,.has-error .control-label,.has-error .radio,.has-error .checkbox,.has-error .radio-inline,.has-error .checkbox-inline{color:#a94442}.has-error .form-control{border-color:#a94442;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#843534;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483}.has-error .input-group-addon{color:#a94442;background-color:#f2dede;border-color:#a94442}.has-error .form-control-feedback{color:#a94442}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn,.form-inline .input-group .form-control{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .radio,.form-inline .checkbox{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .radio label,.form-inline .checkbox label{padding-left:0}.form-inline .radio input[type=radio],.form-inline .checkbox input[type=checkbox]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .radio,.form-horizontal .checkbox,.form-horizontal .radio-inline,.form-horizontal .checkbox-inline{padding-top:7px;margin-top:0;margin-bottom:0}.form-horizontal .radio,.form-horizontal .checkbox{min-height:27px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:7px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{top:0;right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:14.3px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px}}.btn{display:inline-block;padding:6px 12px;margin-bottom:0;font-size:14px;font-weight:400;line-height:1.42857143;text-align:center;white-space:nowrap;vertical-align:middle;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;background-image:none;border:1px solid transparent;border-radius:4px}.btn:focus,.btn:active:focus,.btn.active:focus{outline:thin dotted;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn:hover,.btn:focus{color:#333;text-decoration:none}.btn:active,.btn.active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{pointer-events:none;cursor:not-allowed;filter:alpha(opacity=65);-webkit-box-shadow:none;box-shadow:none;opacity:.65}.btn-default{color:#333;background-color:#fff;border-color:#ccc}.btn-default:hover,.btn-default:focus,.btn-default:active,.btn-default.active,.open>.dropdown-toggle.btn-default{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default:active,.btn-default.active,.open>.dropdown-toggle.btn-default{background-image:none}.btn-default.disabled,.btn-default[disabled],fieldset[disabled] .btn-default,.btn-default.disabled:hover,.btn-default[disabled]:hover,fieldset[disabled] .btn-default:hover,.btn-default.disabled:focus,.btn-default[disabled]:focus,fieldset[disabled] .btn-default:focus,.btn-default.disabled:active,.btn-default[disabled]:active,fieldset[disabled] .btn-default:active,.btn-default.disabled.active,.btn-default[disabled].active,fieldset[disabled] .btn-default.active{background-color:#fff;border-color:#ccc}.btn-default .badge{color:#fff;background-color:#333}.btn-primary{color:#fff;background-color:#428bca;border-color:#357ebd}.btn-primary:hover,.btn-primary:focus,.btn-primary:active,.btn-primary.active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#3071a9;border-color:#285e8e}.btn-primary:active,.btn-primary.active,.open>.dropdown-toggle.btn-primary{background-image:none}.btn-primary.disabled,.btn-primary[disabled],fieldset[disabled] .btn-primary,.btn-primary.disabled:hover,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary:hover,.btn-primary.disabled:focus,.btn-primary[disabled]:focus,fieldset[disabled] .btn-primary:focus,.btn-primary.disabled:active,.btn-primary[disabled]:active,fieldset[disabled] .btn-primary:active,.btn-primary.disabled.active,.btn-primary[disabled].active,fieldset[disabled] .btn-primary.active{background-color:#428bca;border-color:#357ebd}.btn-primary .badge{color:#428bca;background-color:#fff}.btn-success{color:#fff;background-color:#5cb85c;border-color:#4cae4c}.btn-success:hover,.btn-success:focus,.btn-success:active,.btn-success.active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#449d44;border-color:#398439}.btn-success:active,.btn-success.active,.open>.dropdown-toggle.btn-success{background-image:none}.btn-success.disabled,.btn-success[disabled],fieldset[disabled] .btn-success,.btn-success.disabled:hover,.btn-success[disabled]:hover,fieldset[disabled] .btn-success:hover,.btn-success.disabled:focus,.btn-success[disabled]:focus,fieldset[disabled] .btn-success:focus,.btn-success.disabled:active,.btn-success[disabled]:active,fieldset[disabled] .btn-success:active,.btn-success.disabled.active,.btn-success[disabled].active,fieldset[disabled] .btn-success.active{background-color:#5cb85c;border-color:#4cae4c}.btn-success .badge{color:#5cb85c;background-color:#fff}.btn-info{color:#fff;background-color:#5bc0de;border-color:#46b8da}.btn-info:hover,.btn-info:focus,.btn-info:active,.btn-info.active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info:active,.btn-info.active,.open>.dropdown-toggle.btn-info{background-image:none}.btn-info.disabled,.btn-info[disabled],fieldset[disabled] .btn-info,.btn-info.disabled:hover,.btn-info[disabled]:hover,fieldset[disabled] .btn-info:hover,.btn-info.disabled:focus,.btn-info[disabled]:focus,fieldset[disabled] .btn-info:focus,.btn-info.disabled:active,.btn-info[disabled]:active,fieldset[disabled] .btn-info:active,.btn-info.disabled.active,.btn-info[disabled].active,fieldset[disabled] .btn-info.active{background-color:#5bc0de;border-color:#46b8da}.btn-info .badge{color:#5bc0de;background-color:#fff}.btn-warning{color:#fff;background-color:#f0ad4e;border-color:#eea236}.btn-warning:hover,.btn-warning:focus,.btn-warning:active,.btn-warning.active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning:active,.btn-warning.active,.open>.dropdown-toggle.btn-warning{background-image:none}.btn-warning.disabled,.btn-warning[disabled],fieldset[disabled] .btn-warning,.btn-warning.disabled:hover,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning:hover,.btn-warning.disabled:focus,.btn-warning[disabled]:focus,fieldset[disabled] .btn-warning:focus,.btn-warning.disabled:active,.btn-warning[disabled]:active,fieldset[disabled] .btn-warning:active,.btn-warning.disabled.active,.btn-warning[disabled].active,fieldset[disabled] .btn-warning.active{background-color:#f0ad4e;border-color:#eea236}.btn-warning .badge{color:#f0ad4e;background-color:#fff}.btn-danger{color:#fff;background-color:#d9534f;border-color:#d43f3a}.btn-danger:hover,.btn-danger:focus,.btn-danger:active,.btn-danger.active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger:active,.btn-danger.active,.open>.dropdown-toggle.btn-danger{background-image:none}.btn-danger.disabled,.btn-danger[disabled],fieldset[disabled] .btn-danger,.btn-danger.disabled:hover,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger:hover,.btn-danger.disabled:focus,.btn-danger[disabled]:focus,fieldset[disabled] .btn-danger:focus,.btn-danger.disabled:active,.btn-danger[disabled]:active,fieldset[disabled] .btn-danger:active,.btn-danger.disabled.active,.btn-danger[disabled].active,fieldset[disabled] .btn-danger.active{background-color:#d9534f;border-color:#d43f3a}.btn-danger .badge{color:#d9534f;background-color:#fff}.btn-link{font-weight:400;color:#428bca;cursor:pointer;border-radius:0}.btn-link,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:hover,.btn-link:focus,.btn-link:active{border-color:transparent}.btn-link:hover,.btn-link:focus{color:#2a6496;text-decoration:underline;background-color:transparent}.btn-link[disabled]:hover,fieldset[disabled] .btn-link:hover,.btn-link[disabled]:focus,fieldset[disabled] .btn-link:focus{color:#777;text-decoration:none}.btn-lg,.btn-group-lg>.btn{padding:10px 16px;font-size:18px;line-height:1.33;border-radius:6px}.btn-sm,.btn-group-sm>.btn{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-xs,.btn-group-xs>.btn{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=submit].btn-block,input[type=reset].btn-block,input[type=button].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition:height .35s ease;-o-transition:height .35s ease;transition:height .35s ease}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px solid;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:hover,.dropdown-menu>li>a:focus{color:#262626;text-decoration:none;background-color:#f5f5f5}.dropdown-menu>.active>a,.dropdown-menu>.active>a:hover,.dropdown-menu>.active>a:focus{color:#fff;text-decoration:none;background-color:#428bca;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:hover,.dropdown-menu>.disabled>a:focus{color:#777}.dropdown-menu>.disabled>a:hover,.dropdown-menu>.disabled>a:focus{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false)}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#777;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px solid}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:1px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group>.btn,.btn-group-vertical>.btn{position:relative;float:left}.btn-group>.btn:hover,.btn-group-vertical>.btn:hover,.btn-group>.btn:focus,.btn-group-vertical>.btn:focus,.btn-group>.btn:active,.btn-group-vertical>.btn:active,.btn-group>.btn.active,.btn-group-vertical>.btn.active{z-index:2}.btn-group>.btn:focus,.btn-group-vertical>.btn:focus{outline:0}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child>.btn:last-child,.btn-group>.btn-group:first-child>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn>input[type=radio],[data-toggle=buttons]>.btn>input[type=checkbox]{position:absolute;z-index:-1;filter:alpha(opacity=0);opacity:0}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:46px;padding:10px 16px;font-size:18px;line-height:1.33;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:46px;line-height:46px}textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn,select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn,select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn{height:auto}.input-group-addon,.input-group-btn,.input-group .form-control{display:table-cell}.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child),.input-group .form-control:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:6px 12px;font-size:14px;font-weight:400;line-height:1;color:#555;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:10px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=radio],.input-group-addon input[type=checkbox]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle),.input-group-btn:last-child>.btn-group:not(:last-child)>.btn{border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:first-child>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:hover,.input-group-btn>.btn:focus,.input-group-btn>.btn:active{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:hover,.nav>li>a:focus{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#777}.nav>li.disabled>a:hover,.nav>li.disabled>a:focus{color:#777;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:hover,.nav .open>a:focus{background-color:#eee;border-color:#428bca}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:hover,.nav-tabs>li.active>a:focus{color:#555;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:hover,.nav-tabs.nav-justified>.active>a:focus{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:hover,.nav-tabs.nav-justified>.active>a:focus{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:hover,.nav-pills>li.active>a:focus{color:#fff;background-color:#428bca}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:hover,.nav-tabs-justified>.active>a:focus{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:hover,.nav-tabs-justified>.active>a:focus{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;-webkit-overflow-scrolling:touch;border-top:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1)}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;-webkit-box-shadow:none;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse,.navbar-fixed-bottom .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-top .navbar-collapse,.navbar-fixed-bottom .navbar-collapse{max-height:340px}@media (max-width:480px) and (orientation:landscape){.navbar-fixed-top .navbar-collapse,.navbar-fixed-bottom .navbar-collapse{max-height:200px}}.container>.navbar-header,.container-fluid>.navbar-header,.container>.navbar-collapse,.container-fluid>.navbar-collapse{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container>.navbar-header,.container-fluid>.navbar-header,.container>.navbar-collapse,.container-fluid>.navbar-collapse{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-fixed-top,.navbar-fixed-bottom{position:fixed;right:0;left:0;z-index:1030;-webkit-transform:translate3d(0,0,0);-o-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}@media (min-width:768px){.navbar-fixed-top,.navbar-fixed-bottom{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:hover,.navbar-brand:focus{text-decoration:none}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-top:8px;margin-right:15px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;-webkit-box-shadow:none;box-shadow:none}.navbar-nav .open .dropdown-menu>li>a,.navbar-nav .open .dropdown-menu .dropdown-header{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:hover,.navbar-nav .open .dropdown-menu>li>a:focus{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}.navbar-nav.navbar-right:last-child{margin-right:-15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important}}.navbar-form{padding:10px 15px;margin-top:8px;margin-right:-15px;margin-bottom:8px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1)}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn,.navbar-form .input-group .form-control{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .radio,.navbar-form .checkbox{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .radio label,.navbar-form .checkbox label{padding-left:0}.navbar-form .radio input[type=radio],.navbar-form .checkbox input[type=checkbox]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}.navbar-form.navbar-right:last-child{margin-right:-15px}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:8px;margin-bottom:8px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}.navbar-text.navbar-right:last-child{margin-right:0}}.navbar-default{background-color:#f8f8f8;border-color:#e7e7e7}.navbar-default .navbar-brand{color:#777}.navbar-default .navbar-brand:hover,.navbar-default .navbar-brand:focus{color:#5e5e5e;background-color:transparent}.navbar-default .navbar-text{color:#777}.navbar-default .navbar-nav>li>a{color:#777}.navbar-default .navbar-nav>li>a:hover,.navbar-default .navbar-nav>li>a:focus{color:#333;background-color:transparent}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:hover,.navbar-default .navbar-nav>.active>a:focus{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:hover,.navbar-default .navbar-nav>.disabled>a:focus{color:#ccc;background-color:transparent}.navbar-default .navbar-toggle{border-color:#ddd}.navbar-default .navbar-toggle:hover,.navbar-default .navbar-toggle:focus{background-color:#ddd}.navbar-default .navbar-toggle .icon-bar{background-color:#888}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#e7e7e7}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:hover,.navbar-default .navbar-nav>.open>a:focus{color:#555;background-color:#e7e7e7}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#777}.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover,.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus{color:#333;background-color:transparent}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus{color:#ccc;background-color:transparent}}.navbar-default .navbar-link{color:#777}.navbar-default .navbar-link:hover{color:#333}.navbar-default .btn-link{color:#777}.navbar-default .btn-link:hover,.navbar-default .btn-link:focus{color:#333}.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:hover,.navbar-default .btn-link[disabled]:focus,fieldset[disabled] .navbar-default .btn-link:focus{color:#ccc}.navbar-inverse{background-color:#222;border-color:#080808}.navbar-inverse .navbar-brand{color:#777}.navbar-inverse .navbar-brand:hover,.navbar-inverse .navbar-brand:focus{color:#fff;background-color:transparent}.navbar-inverse .navbar-text{color:#777}.navbar-inverse .navbar-nav>li>a{color:#777}.navbar-inverse .navbar-nav>li>a:hover,.navbar-inverse .navbar-nav>li>a:focus{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:hover,.navbar-inverse .navbar-nav>.active>a:focus{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:hover,.navbar-inverse .navbar-nav>.disabled>a:focus{color:#444;background-color:transparent}.navbar-inverse .navbar-toggle{border-color:#333}.navbar-inverse .navbar-toggle:hover,.navbar-inverse .navbar-toggle:focus{background-color:#333}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#101010}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:hover,.navbar-inverse .navbar-nav>.open>a:focus{color:#fff;background-color:#080808}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#777}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus{color:#444;background-color:transparent}}.navbar-inverse .navbar-link{color:#777}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#777}.navbar-inverse .btn-link:hover,.navbar-inverse .btn-link:focus{color:#fff}.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:hover,.navbar-inverse .btn-link[disabled]:focus,fieldset[disabled] .navbar-inverse .btn-link:focus{color:#444}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#777}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:6px 12px;margin-left:-1px;line-height:1.42857143;color:#428bca;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>li>a:hover,.pagination>li>span:hover,.pagination>li>a:focus,.pagination>li>span:focus{color:#2a6496;background-color:#eee;border-color:#ddd}.pagination>.active>a,.pagination>.active>span,.pagination>.active>a:hover,.pagination>.active>span:hover,.pagination>.active>a:focus,.pagination>.active>span:focus{z-index:2;color:#fff;cursor:default;background-color:#428bca;border-color:#428bca}.pagination>.disabled>span,.pagination>.disabled>span:hover,.pagination>.disabled>span:focus,.pagination>.disabled>a,.pagination>.disabled>a:hover,.pagination>.disabled>a:focus{color:#777;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:10px 16px;font-size:18px}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:hover,.pager li>a:focus{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:hover,.pager .disabled>a:focus,.pager .disabled>span{color:#777;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:hover,a.label:focus{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#777}.label-default[href]:hover,.label-default[href]:focus{background-color:#5e5e5e}.label-primary{background-color:#428bca}.label-primary[href]:hover,.label-primary[href]:focus{background-color:#3071a9}.label-success{background-color:#5cb85c}.label-success[href]:hover,.label-success[href]:focus{background-color:#449d44}.label-info{background-color:#5bc0de}.label-info[href]:hover,.label-info[href]:focus{background-color:#31b0d5}.label-warning{background-color:#f0ad4e}.label-warning[href]:hover,.label-warning[href]:focus{background-color:#ec971f}.label-danger{background-color:#d9534f}.label-danger[href]:hover,.label-danger[href]:focus{background-color:#c9302c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;background-color:#777;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-xs .badge{top:0;padding:1px 5px}a.badge:hover,a.badge:focus{color:#fff;text-decoration:none;cursor:pointer}a.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#428bca;background-color:#fff}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron h1,.jumbotron .h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron{border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron{padding-right:60px;padding-left:60px}.jumbotron h1,.jumbotron .h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.thumbnail>img,.thumbnail a>img{margin-right:auto;margin-left:auto}a.thumbnail:hover,a.thumbnail:focus,a.thumbnail.active{border-color:#428bca}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#2b542c}.alert-info{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#245269}.alert-warning{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.alert-warning hr{border-top-color:#f7e1b5}.alert-warning .alert-link{color:#66512c}.alert-danger{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.alert-danger hr{border-top-color:#e4b9c0}.alert-danger .alert-link{color:#843534}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@-o-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#428bca;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-striped .progress-bar,.progress-bar-striped{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);-webkit-background-size:40px 40px;background-size:40px 40px}.progress.active .progress-bar,.progress-bar.active{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar[aria-valuenow="1"],.progress-bar[aria-valuenow="2"]{min-width:30px}.progress-bar[aria-valuenow="0"]{min-width:30px;color:#777;background-color:transparent;background-image:none;-webkit-box-shadow:none;box-shadow:none}.progress-bar-success{background-color:#5cb85c}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#5bc0de}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#f0ad4e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#d9534f}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media,.media-body{overflow:hidden;zoom:1}.media,.media .media{margin-top:15px}.media:first-child{margin-top:0}.media-object{display:block}.media-heading{margin:0 0 5px}.media>.pull-left{margin-right:10px}.media>.pull-right{margin-left:10px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}a.list-group-item{color:#555}a.list-group-item .list-group-item-heading{color:#333}a.list-group-item:hover,a.list-group-item:focus{color:#555;text-decoration:none;background-color:#f5f5f5}.list-group-item.disabled,.list-group-item.disabled:hover,.list-group-item.disabled:focus{color:#777;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text{color:#777}.list-group-item.active,.list-group-item.active:hover,.list-group-item.active:focus{z-index:2;color:#fff;background-color:#428bca;border-color:#428bca}.list-group-item.active .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>.small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:hover .list-group-item-text,.list-group-item.active:focus .list-group-item-text{color:#e1edf7}.list-group-item-success{color:#3c763d;background-color:#dff0d8}a.list-group-item-success{color:#3c763d}a.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:hover,a.list-group-item-success:focus{color:#3c763d;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:hover,a.list-group-item-success.active:focus{color:#fff;background-color:#3c763d;border-color:#3c763d}.list-group-item-info{color:#31708f;background-color:#d9edf7}a.list-group-item-info{color:#31708f}a.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:hover,a.list-group-item-info:focus{color:#31708f;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:hover,a.list-group-item-info.active:focus{color:#fff;background-color:#31708f;border-color:#31708f}.list-group-item-warning{color:#8a6d3b;background-color:#fcf8e3}a.list-group-item-warning{color:#8a6d3b}a.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:hover,a.list-group-item-warning:focus{color:#8a6d3b;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:hover,a.list-group-item-warning.active:focus{color:#fff;background-color:#8a6d3b;border-color:#8a6d3b}.list-group-item-danger{color:#a94442;background-color:#f2dede}a.list-group-item-danger{color:#a94442}a.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:hover,a.list-group-item-danger:focus{color:#a94442;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:hover,a.list-group-item-danger.active:focus{color:#fff;background-color:#a94442;border-color:#a94442}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group{margin-bottom:0}.panel>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.table,.panel>.table-responsive>.table,.panel>.panel-collapse>.table{margin-bottom:0}.panel>.table:first-child,.panel>.table-responsive:first-child>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table:last-child,.panel>.table-responsive:last-child>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child th,.panel>.table>tbody:first-child>tr:first-child td{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child{border-left:0}.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child{border-right:0}.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#428bca}.panel-primary>.panel-heading{color:#fff;background-color:#428bca;border-color:#428bca}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#428bca}.panel-primary>.panel-heading .badge{color:#428bca;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#428bca}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#3c763d}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#31708f}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#faebcc}.panel-warning>.panel-heading{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#faebcc}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#8a6d3b}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#faebcc}.panel-danger{border-color:#ebccd1}.panel-danger>.panel-heading{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ebccd1}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#a94442}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ebccd1}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive iframe,.embed-responsive embed,.embed-responsive object{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;filter:alpha(opacity=20);opacity:.2}.close:hover,.close:focus{color:#000;text-decoration:none;cursor:pointer;filter:alpha(opacity=50);opacity:.5}button.close{-webkit-appearance:none;padding:0;cursor:pointer;background:0 0;border:0}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transition:-webkit-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:transform .3s ease-out;-webkit-transform:translate3d(0,-25%,0);-o-transform:translate3d(0,-25%,0);transform:translate3d(0,-25%,0)}.modal.in .modal-dialog{-webkit-transform:translate3d(0,0,0);-o-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;outline:0;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5)}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{filter:alpha(opacity=0);opacity:0}.modal-backdrop.in{filter:alpha(opacity=50);opacity:.5}.modal-header{min-height:16.43px;padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:15px}.modal-footer{padding:15px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-size:12px;line-height:1.4;visibility:visible;filter:alpha(opacity=0);opacity:0}.tooltip.in{filter:alpha(opacity=90);opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;text-decoration:none;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{bottom:0;left:5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{right:5px;bottom:0;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;left:5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;right:5px;border-width:0 5px 5px;border-bottom-color:#000}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;text-align:left;white-space:normal;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2)}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover-title{padding:8px 14px;margin:0;font-size:14px;font-weight:400;line-height:18px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow{border-width:11px}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>img,.carousel-inner>.item>a>img{line-height:1}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);filter:alpha(opacity=50);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.5)),to(rgba(0,0,0,.0001)));background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.0001)),to(rgba(0,0,0,.5)));background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);background-repeat:repeat-x}.carousel-control:hover,.carousel-control:focus{color:#fff;text-decoration:none;filter:alpha(opacity=90);outline:0;opacity:.9}.carousel-control .icon-prev,.carousel-control .icon-next,.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right{position:absolute;top:50%;z-index:5;display:inline-block}.carousel-control .icon-prev,.carousel-control .glyphicon-chevron-left{left:50%;margin-left:-10px}.carousel-control .icon-next,.carousel-control .glyphicon-chevron-right{right:50%;margin-right:-10px}.carousel-control .icon-prev,.carousel-control .icon-next{width:20px;height:20px;margin-top:-10px;font-family:serif}.carousel-control .icon-prev:before{content:'\2039'}.carousel-control .icon-next:before{content:'\203a'}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:#000 \9;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-prev,.carousel-control .icon-next{width:30px;height:30px;margin-top:-15px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-15px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-15px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.clearfix:before,.clearfix:after,.dl-horizontal dd:before,.dl-horizontal dd:after,.container:before,.container:after,.container-fluid:before,.container-fluid:after,.row:before,.row:after,.form-horizontal .form-group:before,.form-horizontal .form-group:after,.btn-toolbar:before,.btn-toolbar:after,.btn-group-vertical>.btn-group:before,.btn-group-vertical>.btn-group:after,.nav:before,.nav:after,.navbar:before,.navbar:after,.navbar-header:before,.navbar-header:after,.navbar-collapse:before,.navbar-collapse:after,.pager:before,.pager:after,.panel-body:before,.panel-body:after,.modal-footer:before,.modal-footer:after{display:table;content:" "}.clearfix:after,.dl-horizontal dd:after,.container:after,.container-fluid:after,.row:after,.form-horizontal .form-group:after,.btn-toolbar:after,.btn-group-vertical>.btn-group:after,.nav:after,.navbar:after,.navbar-header:after,.navbar-collapse:after,.pager:after,.panel-body:after,.modal-footer:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important;visibility:hidden!important}.affix{position:fixed;-webkit-transform:translate3d(0,0,0);-o-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}@-ms-viewport{width:device-width}.visible-xs,.visible-sm,.visible-md,.visible-lg{display:none!important}.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table}tr.visible-xs{display:table-row!important}th.visible-xs,td.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table}tr.visible-sm{display:table-row!important}th.visible-sm,td.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table}tr.visible-md{display:table-row!important}th.visible-md,td.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table}tr.visible-lg{display:table-row!important}th.visible-lg,td.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table}tr.visible-print{display:table-row!important}th.visible-print,td.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}
+ *//*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */html{font-family:sans-serif;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:none;text-decoration:underline;-webkit-text-decoration:underline dotted;-moz-text-decoration:underline dotted;text-decoration:underline dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{font-size:2em;margin:.67em 0}mark{background:#ff0;color:#000}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;height:0}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{color:inherit;font:inherit;margin:0}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}input{line-height:normal}input[type=checkbox],input[type=radio]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-appearance:textfield;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{border:1px solid silver;margin:0 2px;padding:.35em .625em .75em}legend{border:0;padding:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-collapse:collapse;border-spacing:0}td,th{padding:0}/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */@media print{*,:after,:before{color:#000!important;text-shadow:none!important;background:0 0!important;-webkit-box-shadow:none!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}h2,h3,p{orphans:3;widows:3}h2,h3{page-break-after:avoid}.navbar{display:none}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table td,.table th{background-color:#fff!important}.table-bordered td,.table-bordered th{border:1px solid #ddd!important}}@font-face{font-family:"Glyphicons Halflings";src:url(../fonts/glyphicons-halflings-regular.eot);src:url(../fonts/glyphicons-halflings-regular.eot?#iefix) format("embedded-opentype"),url(../fonts/glyphicons-halflings-regular.woff2) format("woff2"),url(../fonts/glyphicons-halflings-regular.woff) format("woff"),url(../fonts/glyphicons-halflings-regular.ttf) format("truetype"),url(../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular) format("svg")}.glyphicon{position:relative;top:1px;display:inline-block;font-family:"Glyphicons Halflings";font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\002a"}.glyphicon-plus:before{content:"\002b"}.glyphicon-eur:before,.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:after,:before{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:rgba(0,0,0,0)}body{font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}button,input,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#337ab7;text-decoration:none}a:focus,a:hover{color:#23527c;text-decoration:underline}a:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.carousel-inner>.item>a>img,.carousel-inner>.item>img,.img-responsive,.thumbnail a>img,.thumbnail>img{display:block;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out;display:inline-block;max-width:100%;height:auto}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}[role=button]{cursor:pointer}.h1,.h2,.h3,.h4,.h5,.h6,h1,h2,h3,h4,h5,h6{font-family:inherit;font-weight:500;line-height:1.1;color:inherit}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-weight:400;line-height:1;color:#777}.h1,.h2,.h3,h1,h2,h3{margin-top:20px;margin-bottom:10px}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small{font-size:65%}.h4,.h5,.h6,h4,h5,h6{margin-top:10px;margin-bottom:10px}.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-size:75%}.h1,h1{font-size:36px}.h2,h2{font-size:30px}.h3,h3{font-size:24px}.h4,h4{font-size:18px}.h5,h5{font-size:14px}.h6,h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}.small,small{font-size:85%}.mark,mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#777}.text-primary{color:#337ab7}a.text-primary:focus,a.text-primary:hover{color:#286090}.text-success{color:#3c763d}a.text-success:focus,a.text-success:hover{color:#2b542c}.text-info{color:#31708f}a.text-info:focus,a.text-info:hover{color:#245269}.text-warning{color:#8a6d3b}a.text-warning:focus,a.text-warning:hover{color:#66512c}.text-danger{color:#a94442}a.text-danger:focus,a.text-danger:hover{color:#843534}.bg-primary{color:#fff;background-color:#337ab7}a.bg-primary:focus,a.bg-primary:hover{background-color:#286090}.bg-success{background-color:#dff0d8}a.bg-success:focus,a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:focus,a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:focus,a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:focus,a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ol,ul{margin-top:0;margin-bottom:10px}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;list-style:none;margin-left:-5px}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dd,dt{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;clear:left;text-align:right;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[data-original-title],abbr[title]{cursor:help}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote ol:last-child,blockquote p:last-child,blockquote ul:last-child{margin-bottom:0}blockquote .small,blockquote footer,blockquote small{display:block;font-size:80%;line-height:1.42857143;color:#777}blockquote .small:before,blockquote footer:before,blockquote small:before{content:"\2014 \00A0"}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse .small:before,.blockquote-reverse footer:before,.blockquote-reverse small:before,blockquote.pull-right .small:before,blockquote.pull-right footer:before,blockquote.pull-right small:before{content:""}.blockquote-reverse .small:after,.blockquote-reverse footer:after,.blockquote-reverse small:after,blockquote.pull-right .small:after,blockquote.pull-right footer:after,blockquote.pull-right small:after{content:"\00A0 \2014"}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.25);box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;font-weight:700;-webkit-box-shadow:none;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.row-no-gutters{margin-right:0;margin-left:0}.row-no-gutters [class*=col-]{padding-right:0;padding-left:0}.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}caption{padding-top:8px;padding-bottom:8px;color:#777;text-align:left}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>tbody>tr>td,.table>tbody>tr>th,.table>tfoot>tr>td,.table>tfoot>tr>th,.table>thead>tr>td,.table>thead>tr>th{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>td,.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>td,.table>thead:first-child>tr:first-child>th{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>tbody>tr>td,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>td,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>thead>tr>th{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>tbody>tr>td,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>td,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border:1px solid #ddd}.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border-bottom-width:2px}.table-striped>tbody>tr:nth-of-type(odd){background-color:#f9f9f9}.table-hover>tbody>tr:hover{background-color:#f5f5f5}.table>tbody>tr.active>td,.table>tbody>tr.active>th,.table>tbody>tr>td.active,.table>tbody>tr>th.active,.table>tfoot>tr.active>td,.table>tfoot>tr.active>th,.table>tfoot>tr>td.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>thead>tr.active>th,.table>thead>tr>td.active,.table>thead>tr>th.active{background-color:#f5f5f5}.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr.active:hover>th,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover{background-color:#e8e8e8}.table>tbody>tr.success>td,.table>tbody>tr.success>th,.table>tbody>tr>td.success,.table>tbody>tr>th.success,.table>tfoot>tr.success>td,.table>tfoot>tr.success>th,.table>tfoot>tr>td.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>thead>tr.success>th,.table>thead>tr>td.success,.table>thead>tr>th.success{background-color:#dff0d8}.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr.success:hover>th,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover{background-color:#d0e9c6}.table>tbody>tr.info>td,.table>tbody>tr.info>th,.table>tbody>tr>td.info,.table>tbody>tr>th.info,.table>tfoot>tr.info>td,.table>tfoot>tr.info>th,.table>tfoot>tr>td.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>thead>tr.info>th,.table>thead>tr>td.info,.table>thead>tr>th.info{background-color:#d9edf7}.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr.info:hover>th,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover{background-color:#c4e3f3}.table>tbody>tr.warning>td,.table>tbody>tr.warning>th,.table>tbody>tr>td.warning,.table>tbody>tr>th.warning,.table>tfoot>tr.warning>td,.table>tfoot>tr.warning>th,.table>tfoot>tr>td.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>thead>tr.warning>th,.table>thead>tr>td.warning,.table>thead>tr>th.warning{background-color:#fcf8e3}.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr.warning:hover>th,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover{background-color:#faf2cc}.table>tbody>tr.danger>td,.table>tbody>tr.danger>th,.table>tbody>tr>td.danger,.table>tbody>tr>th.danger,.table>tfoot>tr.danger>td,.table>tfoot>tr.danger>th,.table>tfoot>tr>td.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>thead>tr.danger>th,.table>thead>tr>td.danger,.table>thead>tr>th.danger{background-color:#f2dede}.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr.danger:hover>th,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover{background-color:#ebcccc}.table-responsive{min-height:.01%;overflow-x:auto}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-y:hidden;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>td,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>thead>tr>th{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;-webkit-appearance:none;-moz-appearance:none;appearance:none}input[type=checkbox],input[type=radio]{margin:4px 0 0;margin-top:1px\9;line-height:normal}fieldset[disabled] input[type=checkbox],fieldset[disabled] input[type=radio],input[type=checkbox].disabled,input[type=checkbox][disabled],input[type=radio].disabled,input[type=radio][disabled]{cursor:not-allowed}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:7px;font-size:14px;line-height:1.42857143;color:#555}.form-control{display:block;width:100%;height:34px;padding:6px 12px;font-size:14px;line-height:1.42857143;color:#555;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;-webkit-transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s,-webkit-box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#999;opacity:1}.form-control:-ms-input-placeholder{color:#999}.form-control::-webkit-input-placeholder{color:#999}.form-control::-ms-expand{background-color:transparent;border:0}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{background-color:#eee;opacity:1}.form-control[disabled],fieldset[disabled] .form-control{cursor:not-allowed}textarea.form-control{height:auto}@media screen and (-webkit-min-device-pixel-ratio:0){input[type=date].form-control,input[type=datetime-local].form-control,input[type=month].form-control,input[type=time].form-control{line-height:34px}.input-group-sm input[type=date],.input-group-sm input[type=datetime-local],.input-group-sm input[type=month],.input-group-sm input[type=time],input[type=date].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm,input[type=time].input-sm{line-height:30px}.input-group-lg input[type=date],.input-group-lg input[type=datetime-local],.input-group-lg input[type=month],.input-group-lg input[type=time],input[type=date].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg,input[type=time].input-lg{line-height:46px}}.form-group{margin-bottom:15px}.checkbox,.radio{position:relative;display:block;margin-top:10px;margin-bottom:10px}.checkbox.disabled label,.radio.disabled label,fieldset[disabled] .checkbox label,fieldset[disabled] .radio label{cursor:not-allowed}.checkbox label,.radio label{min-height:20px;padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox],.radio input[type=radio],.radio-inline input[type=radio]{position:absolute;margin-top:4px\9;margin-left:-20px}.checkbox+.checkbox,.radio+.radio{margin-top:-5px}.checkbox-inline,.radio-inline{position:relative;display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.checkbox-inline.disabled,.radio-inline.disabled,fieldset[disabled] .checkbox-inline,fieldset[disabled] .radio-inline{cursor:not-allowed}.checkbox-inline+.checkbox-inline,.radio-inline+.radio-inline{margin-top:0;margin-left:10px}.form-control-static{min-height:34px;padding-top:7px;padding-bottom:7px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}select[multiple].input-sm,textarea.input-sm{height:auto}.form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.form-group-sm select.form-control{height:30px;line-height:30px}.form-group-sm select[multiple].form-control,.form-group-sm textarea.form-control{height:auto}.form-group-sm .form-control-static{height:30px;min-height:32px;padding:6px 10px;font-size:12px;line-height:1.5}.input-lg{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-lg{height:46px;line-height:46px}select[multiple].input-lg,textarea.input-lg{height:auto}.form-group-lg .form-control{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.form-group-lg select.form-control{height:46px;line-height:46px}.form-group-lg select[multiple].form-control,.form-group-lg textarea.form-control{height:auto}.form-group-lg .form-control-static{height:46px;min-height:38px;padding:11px 16px;font-size:18px;line-height:1.3333333}.has-feedback{position:relative}.has-feedback .form-control{padding-right:42.5px}.form-control-feedback{position:absolute;top:0;right:0;z-index:2;display:block;width:34px;height:34px;line-height:34px;text-align:center;pointer-events:none}.form-group-lg .form-control+.form-control-feedback,.input-group-lg+.form-control-feedback,.input-lg+.form-control-feedback{width:46px;height:46px;line-height:46px}.form-group-sm .form-control+.form-control-feedback,.input-group-sm+.form-control-feedback,.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .checkbox,.has-success .checkbox-inline,.has-success .control-label,.has-success .help-block,.has-success .radio,.has-success .radio-inline,.has-success.checkbox label,.has-success.checkbox-inline label,.has-success.radio label,.has-success.radio-inline label{color:#3c763d}.has-success .form-control{border-color:#3c763d;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#2b542c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168}.has-success .input-group-addon{color:#3c763d;background-color:#dff0d8;border-color:#3c763d}.has-success .form-control-feedback{color:#3c763d}.has-warning .checkbox,.has-warning .checkbox-inline,.has-warning .control-label,.has-warning .help-block,.has-warning .radio,.has-warning .radio-inline,.has-warning.checkbox label,.has-warning.checkbox-inline label,.has-warning.radio label,.has-warning.radio-inline label{color:#8a6d3b}.has-warning .form-control{border-color:#8a6d3b;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#66512c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b}.has-warning .input-group-addon{color:#8a6d3b;background-color:#fcf8e3;border-color:#8a6d3b}.has-warning .form-control-feedback{color:#8a6d3b}.has-error .checkbox,.has-error .checkbox-inline,.has-error .control-label,.has-error .help-block,.has-error .radio,.has-error .radio-inline,.has-error.checkbox label,.has-error.checkbox-inline label,.has-error.radio label,.has-error.radio-inline label{color:#a94442}.has-error .form-control{border-color:#a94442;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#843534;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483}.has-error .input-group-addon{color:#a94442;background-color:#f2dede;border-color:#a94442}.has-error .form-control-feedback{color:#a94442}.has-feedback label~.form-control-feedback{top:25px}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .form-control-static{display:inline-block}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .form-control,.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .checkbox,.form-inline .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .checkbox label,.form-inline .radio label{padding-left:0}.form-inline .checkbox input[type=checkbox],.form-inline .radio input[type=radio]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .checkbox,.form-horizontal .checkbox-inline,.form-horizontal .radio,.form-horizontal .radio-inline{padding-top:7px;margin-top:0;margin-bottom:0}.form-horizontal .checkbox,.form-horizontal .radio{min-height:27px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:7px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:11px;font-size:18px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px;font-size:12px}}.btn{display:inline-block;margin-bottom:0;font-weight:400;text-align:center;white-space:nowrap;vertical-align:middle;-ms-touch-action:manipulation;touch-action:manipulation;cursor:pointer;background-image:none;border:1px solid transparent;padding:6px 12px;font-size:14px;line-height:1.42857143;border-radius:4px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.btn.active.focus,.btn.active:focus,.btn.focus,.btn:active.focus,.btn:active:focus,.btn:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn.focus,.btn:focus,.btn:hover{color:#333;text-decoration:none}.btn.active,.btn:active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{cursor:not-allowed;filter:alpha(opacity=65);opacity:.65;-webkit-box-shadow:none;box-shadow:none}a.btn.disabled,fieldset[disabled] a.btn{pointer-events:none}.btn-default{color:#333;background-color:#fff;border-color:#ccc}.btn-default.focus,.btn-default:focus{color:#333;background-color:#e6e6e6;border-color:#8c8c8c}.btn-default:hover{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{color:#333;background-color:#e6e6e6;background-image:none;border-color:#adadad}.btn-default.active.focus,.btn-default.active:focus,.btn-default.active:hover,.btn-default:active.focus,.btn-default:active:focus,.btn-default:active:hover,.open>.dropdown-toggle.btn-default.focus,.open>.dropdown-toggle.btn-default:focus,.open>.dropdown-toggle.btn-default:hover{color:#333;background-color:#d4d4d4;border-color:#8c8c8c}.btn-default.disabled.focus,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled].focus,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#fff;border-color:#ccc}.btn-default .badge{color:#fff;background-color:#333}.btn-primary{color:#fff;background-color:#337ab7;border-color:#2e6da4}.btn-primary.focus,.btn-primary:focus{color:#fff;background-color:#286090;border-color:#122b40}.btn-primary:hover{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#286090;background-image:none;border-color:#204d74}.btn-primary.active.focus,.btn-primary.active:focus,.btn-primary.active:hover,.btn-primary:active.focus,.btn-primary:active:focus,.btn-primary:active:hover,.open>.dropdown-toggle.btn-primary.focus,.open>.dropdown-toggle.btn-primary:focus,.open>.dropdown-toggle.btn-primary:hover{color:#fff;background-color:#204d74;border-color:#122b40}.btn-primary.disabled.focus,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled].focus,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#337ab7;border-color:#2e6da4}.btn-primary .badge{color:#337ab7;background-color:#fff}.btn-success{color:#fff;background-color:#5cb85c;border-color:#4cae4c}.btn-success.focus,.btn-success:focus{color:#fff;background-color:#449d44;border-color:#255625}.btn-success:hover{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#449d44;background-image:none;border-color:#398439}.btn-success.active.focus,.btn-success.active:focus,.btn-success.active:hover,.btn-success:active.focus,.btn-success:active:focus,.btn-success:active:hover,.open>.dropdown-toggle.btn-success.focus,.open>.dropdown-toggle.btn-success:focus,.open>.dropdown-toggle.btn-success:hover{color:#fff;background-color:#398439;border-color:#255625}.btn-success.disabled.focus,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled].focus,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#5cb85c;border-color:#4cae4c}.btn-success .badge{color:#5cb85c;background-color:#fff}.btn-info{color:#fff;background-color:#5bc0de;border-color:#46b8da}.btn-info.focus,.btn-info:focus{color:#fff;background-color:#31b0d5;border-color:#1b6d85}.btn-info:hover{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#31b0d5;background-image:none;border-color:#269abc}.btn-info.active.focus,.btn-info.active:focus,.btn-info.active:hover,.btn-info:active.focus,.btn-info:active:focus,.btn-info:active:hover,.open>.dropdown-toggle.btn-info.focus,.open>.dropdown-toggle.btn-info:focus,.open>.dropdown-toggle.btn-info:hover{color:#fff;background-color:#269abc;border-color:#1b6d85}.btn-info.disabled.focus,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled].focus,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#5bc0de;border-color:#46b8da}.btn-info .badge{color:#5bc0de;background-color:#fff}.btn-warning{color:#fff;background-color:#f0ad4e;border-color:#eea236}.btn-warning.focus,.btn-warning:focus{color:#fff;background-color:#ec971f;border-color:#985f0d}.btn-warning:hover{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#ec971f;background-image:none;border-color:#d58512}.btn-warning.active.focus,.btn-warning.active:focus,.btn-warning.active:hover,.btn-warning:active.focus,.btn-warning:active:focus,.btn-warning:active:hover,.open>.dropdown-toggle.btn-warning.focus,.open>.dropdown-toggle.btn-warning:focus,.open>.dropdown-toggle.btn-warning:hover{color:#fff;background-color:#d58512;border-color:#985f0d}.btn-warning.disabled.focus,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled].focus,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#f0ad4e;border-color:#eea236}.btn-warning .badge{color:#f0ad4e;background-color:#fff}.btn-danger{color:#fff;background-color:#d9534f;border-color:#d43f3a}.btn-danger.focus,.btn-danger:focus{color:#fff;background-color:#c9302c;border-color:#761c19}.btn-danger:hover{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#c9302c;background-image:none;border-color:#ac2925}.btn-danger.active.focus,.btn-danger.active:focus,.btn-danger.active:hover,.btn-danger:active.focus,.btn-danger:active:focus,.btn-danger:active:hover,.open>.dropdown-toggle.btn-danger.focus,.open>.dropdown-toggle.btn-danger:focus,.open>.dropdown-toggle.btn-danger:hover{color:#fff;background-color:#ac2925;border-color:#761c19}.btn-danger.disabled.focus,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled].focus,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#d9534f;border-color:#d43f3a}.btn-danger .badge{color:#d9534f;background-color:#fff}.btn-link{font-weight:400;color:#337ab7;border-radius:0}.btn-link,.btn-link.active,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:active,.btn-link:focus,.btn-link:hover{border-color:transparent}.btn-link:focus,.btn-link:hover{color:#23527c;text-decoration:underline;background-color:transparent}.btn-link[disabled]:focus,.btn-link[disabled]:hover,fieldset[disabled] .btn-link:focus,fieldset[disabled] .btn-link:hover{color:#777;text-decoration:none}.btn-group-lg>.btn,.btn-lg{padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.btn-group-sm>.btn,.btn-sm{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-group-xs>.btn,.btn-xs{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=button].btn-block,input[type=reset].btn-block,input[type=submit].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition-property:height,visibility;-o-transition-property:height,visibility;transition-property:height,visibility;-webkit-transition-duration:.35s;-o-transition-duration:.35s;transition-duration:.35s;-webkit-transition-timing-function:ease;-o-transition-timing-function:ease;transition-timing-function:ease}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px dashed;border-top:4px solid\9;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown,.dropup{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{color:#262626;text-decoration:none;background-color:#f5f5f5}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{color:#fff;text-decoration:none;background-color:#337ab7;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{color:#777}.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false)}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#777;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px dashed;border-bottom:4px solid\9}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:2px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group-vertical>.btn,.btn-group>.btn{position:relative;float:left}.btn-group-vertical>.btn.active,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:hover,.btn-group>.btn.active,.btn-group>.btn:active,.btn-group>.btn:focus,.btn-group>.btn:hover{z-index:2}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn,.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn input[type=checkbox],[data-toggle=buttons]>.btn input[type=radio],[data-toggle=buttons]>.btn-group>.btn input[type=checkbox],[data-toggle=buttons]>.btn-group>.btn input[type=radio]{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group .form-control:focus{z-index:3}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:46px;line-height:46px}select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn,textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn,textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn{height:auto}.input-group .form-control,.input-group-addon,.input-group-btn{display:table-cell}.input-group .form-control:not(:first-child):not(:last-child),.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:6px 12px;font-size:14px;font-weight:400;line-height:1;color:#555;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:10px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=checkbox],.input-group-addon input[type=radio]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn-group:not(:last-child)>.btn,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:first-child>.btn-group:not(:first-child)>.btn,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:active,.input-group-btn>.btn:focus,.input-group-btn>.btn:hover{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{z-index:2;margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:focus,.nav>li>a:hover{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#777}.nav>li.disabled>a:focus,.nav>li.disabled>a:hover{color:#777;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:focus,.nav .open>a:hover{background-color:#eee;border-color:#337ab7}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:focus,.nav-tabs>li.active>a:hover{color:#555;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:focus,.nav-pills>li.active>a:hover{color:#fff;background-color:#337ab7}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;border-top:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1);-webkit-overflow-scrolling:touch}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;-webkit-box-shadow:none;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-bottom,.navbar-fixed-top{position:fixed;right:0;left:0;z-index:1030}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:340px}@media (max-device-width:480px) and (orientation:landscape){.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:200px}}@media (min-width:768px){.navbar-fixed-bottom,.navbar-fixed-top{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:focus,.navbar-brand:hover{text-decoration:none}.navbar-brand>img{display:block}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-right:15px;margin-top:8px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;-webkit-box-shadow:none;box-shadow:none}.navbar-nav .open .dropdown-menu .dropdown-header,.navbar-nav .open .dropdown-menu>li>a{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:focus,.navbar-nav .open .dropdown-menu>li>a:hover{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}}.navbar-form{padding:10px 15px;margin-right:-15px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);margin-top:8px;margin-bottom:8px}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .form-control-static{display:inline-block}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .form-control,.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .checkbox,.navbar-form .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .checkbox label,.navbar-form .radio label{padding-left:0}.navbar-form .checkbox input[type=checkbox],.navbar-form .radio input[type=radio]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}.navbar-form .form-group:last-child{margin-bottom:0}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{margin-bottom:0;border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:8px;margin-bottom:8px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important;margin-right:-15px}.navbar-right~.navbar-right{margin-right:0}}.navbar-default{background-color:#f8f8f8;border-color:#e7e7e7}.navbar-default .navbar-brand{color:#777}.navbar-default .navbar-brand:focus,.navbar-default .navbar-brand:hover{color:#5e5e5e;background-color:transparent}.navbar-default .navbar-text{color:#777}.navbar-default .navbar-nav>li>a{color:#777}.navbar-default .navbar-nav>li>a:focus,.navbar-default .navbar-nav>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:focus,.navbar-default .navbar-nav>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:focus,.navbar-default .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:focus,.navbar-default .navbar-nav>.open>a:hover{color:#555;background-color:#e7e7e7}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#777}.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-default .navbar-toggle{border-color:#ddd}.navbar-default .navbar-toggle:focus,.navbar-default .navbar-toggle:hover{background-color:#ddd}.navbar-default .navbar-toggle .icon-bar{background-color:#888}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#e7e7e7}.navbar-default .navbar-link{color:#777}.navbar-default .navbar-link:hover{color:#333}.navbar-default .btn-link{color:#777}.navbar-default .btn-link:focus,.navbar-default .btn-link:hover{color:#333}.navbar-default .btn-link[disabled]:focus,.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:focus,fieldset[disabled] .navbar-default .btn-link:hover{color:#ccc}.navbar-inverse{background-color:#222;border-color:#080808}.navbar-inverse .navbar-brand{color:#9d9d9d}.navbar-inverse .navbar-brand:focus,.navbar-inverse .navbar-brand:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-text{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:focus,.navbar-inverse .navbar-nav>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:focus,.navbar-inverse .navbar-nav>.disabled>a:hover{color:#444;background-color:transparent}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:focus,.navbar-inverse .navbar-nav>.open>a:hover{color:#fff;background-color:#080808}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#444;background-color:transparent}}.navbar-inverse .navbar-toggle{border-color:#333}.navbar-inverse .navbar-toggle:focus,.navbar-inverse .navbar-toggle:hover{background-color:#333}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#101010}.navbar-inverse .navbar-link{color:#9d9d9d}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#9d9d9d}.navbar-inverse .btn-link:focus,.navbar-inverse .btn-link:hover{color:#fff}.navbar-inverse .btn-link[disabled]:focus,.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:focus,fieldset[disabled] .navbar-inverse .btn-link:hover{color:#444}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#777}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:6px 12px;margin-left:-1px;line-height:1.42857143;color:#337ab7;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li>a:focus,.pagination>li>a:hover,.pagination>li>span:focus,.pagination>li>span:hover{z-index:2;color:#23527c;background-color:#eee;border-color:#ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>.active>a,.pagination>.active>a:focus,.pagination>.active>a:hover,.pagination>.active>span,.pagination>.active>span:focus,.pagination>.active>span:hover{z-index:3;color:#fff;cursor:default;background-color:#337ab7;border-color:#337ab7}.pagination>.disabled>a,.pagination>.disabled>a:focus,.pagination>.disabled>a:hover,.pagination>.disabled>span,.pagination>.disabled>span:focus,.pagination>.disabled>span:hover{color:#777;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:10px 16px;font-size:18px;line-height:1.3333333}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px;line-height:1.5}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:focus,.pager li>a:hover{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:focus,.pager .disabled>a:hover,.pager .disabled>span{color:#777;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:focus,a.label:hover{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#777}.label-default[href]:focus,.label-default[href]:hover{background-color:#5e5e5e}.label-primary{background-color:#337ab7}.label-primary[href]:focus,.label-primary[href]:hover{background-color:#286090}.label-success{background-color:#5cb85c}.label-success[href]:focus,.label-success[href]:hover{background-color:#449d44}.label-info{background-color:#5bc0de}.label-info[href]:focus,.label-info[href]:hover{background-color:#31b0d5}.label-warning{background-color:#f0ad4e}.label-warning[href]:focus,.label-warning[href]:hover{background-color:#ec971f}.label-danger{background-color:#d9534f}.label-danger[href]:focus,.label-danger[href]:hover{background-color:#c9302c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:middle;background-color:#777;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-group-xs>.btn .badge,.btn-xs .badge{top:0;padding:1px 5px}a.badge:focus,a.badge:hover{color:#fff;text-decoration:none;cursor:pointer}.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#337ab7;background-color:#fff}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding-top:30px;padding-bottom:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron .h1,.jumbotron h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron,.container-fluid .jumbotron{padding-right:15px;padding-left:15px;border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron,.container-fluid .jumbotron{padding-right:60px;padding-left:60px}.jumbotron .h1,.jumbotron h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:border .2s ease-in-out;-o-transition:border .2s ease-in-out;transition:border .2s ease-in-out}.thumbnail a>img,.thumbnail>img{margin-right:auto;margin-left:auto}a.thumbnail.active,a.thumbnail:focus,a.thumbnail:hover{border-color:#337ab7}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#2b542c}.alert-info{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#245269}.alert-warning{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.alert-warning hr{border-top-color:#f7e1b5}.alert-warning .alert-link{color:#66512c}.alert-danger{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.alert-danger hr{border-top-color:#e4b9c0}.alert-danger .alert-link{color:#843534}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@-o-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0%;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#337ab7;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-bar-striped,.progress-striped .progress-bar{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);-webkit-background-size:40px 40px;background-size:40px 40px}.progress-bar.active,.progress.active .progress-bar{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar-success{background-color:#5cb85c}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#5bc0de}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#f0ad4e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#d9534f}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media{margin-top:15px}.media:first-child{margin-top:0}.media,.media-body{overflow:hidden;zoom:1}.media-body{width:10000px}.media-object{display:block}.media-object.img-thumbnail{max-width:none}.media-right,.media>.pull-right{padding-left:10px}.media-left,.media>.pull-left{padding-right:10px}.media-body,.media-left,.media-right{display:table-cell;vertical-align:top}.media-middle{vertical-align:middle}.media-bottom{vertical-align:bottom}.media-heading{margin-top:0;margin-bottom:5px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.list-group-item.disabled,.list-group-item.disabled:focus,.list-group-item.disabled:hover{color:#777;cursor:not-allowed;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text{color:#777}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{z-index:2;color:#fff;background-color:#337ab7;border-color:#337ab7}.list-group-item.active .list-group-item-heading,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:focus .list-group-item-text,.list-group-item.active:hover .list-group-item-text{color:#c7ddef}a.list-group-item,button.list-group-item{color:#555}a.list-group-item .list-group-item-heading,button.list-group-item .list-group-item-heading{color:#333}a.list-group-item:focus,a.list-group-item:hover,button.list-group-item:focus,button.list-group-item:hover{color:#555;text-decoration:none;background-color:#f5f5f5}button.list-group-item{width:100%;text-align:left}.list-group-item-success{color:#3c763d;background-color:#dff0d8}a.list-group-item-success,button.list-group-item-success{color:#3c763d}a.list-group-item-success .list-group-item-heading,button.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:focus,a.list-group-item-success:hover,button.list-group-item-success:focus,button.list-group-item-success:hover{color:#3c763d;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:focus,a.list-group-item-success.active:hover,button.list-group-item-success.active,button.list-group-item-success.active:focus,button.list-group-item-success.active:hover{color:#fff;background-color:#3c763d;border-color:#3c763d}.list-group-item-info{color:#31708f;background-color:#d9edf7}a.list-group-item-info,button.list-group-item-info{color:#31708f}a.list-group-item-info .list-group-item-heading,button.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:focus,a.list-group-item-info:hover,button.list-group-item-info:focus,button.list-group-item-info:hover{color:#31708f;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:focus,a.list-group-item-info.active:hover,button.list-group-item-info.active,button.list-group-item-info.active:focus,button.list-group-item-info.active:hover{color:#fff;background-color:#31708f;border-color:#31708f}.list-group-item-warning{color:#8a6d3b;background-color:#fcf8e3}a.list-group-item-warning,button.list-group-item-warning{color:#8a6d3b}a.list-group-item-warning .list-group-item-heading,button.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:focus,a.list-group-item-warning:hover,button.list-group-item-warning:focus,button.list-group-item-warning:hover{color:#8a6d3b;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:focus,a.list-group-item-warning.active:hover,button.list-group-item-warning.active,button.list-group-item-warning.active:focus,button.list-group-item-warning.active:hover{color:#fff;background-color:#8a6d3b;border-color:#8a6d3b}.list-group-item-danger{color:#a94442;background-color:#f2dede}a.list-group-item-danger,button.list-group-item-danger{color:#a94442}a.list-group-item-danger .list-group-item-heading,button.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:focus,a.list-group-item-danger:hover,button.list-group-item-danger:focus,button.list-group-item-danger:hover{color:#a94442;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:focus,a.list-group-item-danger.active:hover,button.list-group-item-danger.active,button.list-group-item-danger.active:focus,button.list-group-item-danger.active:hover{color:#fff;background-color:#a94442;border-color:#a94442}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>.small,.panel-title>.small>a,.panel-title>a,.panel-title>small,.panel-title>small>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group,.panel>.panel-collapse>.list-group{margin-bottom:0}.panel>.list-group .list-group-item,.panel>.panel-collapse>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child,.panel>.panel-collapse>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child,.panel>.panel-collapse>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.panel-heading+.panel-collapse>.list-group .list-group-item:first-child{border-top-left-radius:0;border-top-right-radius:0}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.panel-collapse>.table,.panel>.table,.panel>.table-responsive>.table{margin-bottom:0}.panel>.panel-collapse>.table caption,.panel>.table caption,.panel>.table-responsive>.table caption{padding-right:15px;padding-left:15px}.panel>.table-responsive:first-child>.table:first-child,.panel>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child,.panel>.table:first-child>thead:first-child>tr:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table-responsive:last-child>.table:last-child,.panel>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive,.panel>.table+.panel-body,.panel>.table-responsive+.panel-body{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child td,.panel>.table>tbody:first-child>tr:first-child th{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.list-group,.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#337ab7}.panel-primary>.panel-heading{color:#fff;background-color:#337ab7;border-color:#337ab7}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#337ab7}.panel-primary>.panel-heading .badge{color:#337ab7;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#337ab7}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#3c763d}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#31708f}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#faebcc}.panel-warning>.panel-heading{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#faebcc}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#8a6d3b}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#faebcc}.panel-danger{border-color:#ebccd1}.panel-danger>.panel-heading{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ebccd1}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#a94442}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ebccd1}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive embed,.embed-responsive iframe,.embed-responsive object,.embed-responsive video{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;filter:alpha(opacity=20);opacity:.2}.close:focus,.close:hover{color:#000;text-decoration:none;cursor:pointer;filter:alpha(opacity=50);opacity:.5}button.close{padding:0;cursor:pointer;background:0 0;border:0;-webkit-appearance:none;-moz-appearance:none;appearance:none}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transform:translate(0,-25%);-ms-transform:translate(0,-25%);-o-transform:translate(0,-25%);transform:translate(0,-25%);-webkit-transition:-webkit-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:-webkit-transform .3s ease-out;transition:transform .3s ease-out;transition:transform .3s ease-out,-webkit-transform .3s ease-out,-o-transform .3s ease-out}.modal.in .modal-dialog{-webkit-transform:translate(0,0);-ms-transform:translate(0,0);-o-transform:translate(0,0);transform:translate(0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5);outline:0}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{filter:alpha(opacity=0);opacity:0}.modal-backdrop.in{filter:alpha(opacity=50);opacity:.5}.modal-header{padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:15px}.modal-footer{padding:15px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:12px;filter:alpha(opacity=0);opacity:0}.tooltip.in{filter:alpha(opacity=90);opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{right:5px;bottom:0;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{bottom:0;left:5px;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;right:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;left:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:14px;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2)}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover>.arrow{border-width:11px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.popover-title{padding:8px 14px;margin:0;font-size:14px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>a>img,.carousel-inner>.item>img{line-height:1}@media all and (transform-3d),(-webkit-transform-3d){.carousel-inner>.item{-webkit-transition:-webkit-transform .6s ease-in-out;-o-transition:-o-transform .6s ease-in-out;transition:-webkit-transform .6s ease-in-out;transition:transform .6s ease-in-out;transition:transform .6s ease-in-out,-webkit-transform .6s ease-in-out,-o-transform .6s ease-in-out;-webkit-backface-visibility:hidden;backface-visibility:hidden;-webkit-perspective:1000px;perspective:1000px}.carousel-inner>.item.active.right,.carousel-inner>.item.next{-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0);left:0}.carousel-inner>.item.active.left,.carousel-inner>.item.prev{-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0);left:0}.carousel-inner>.item.active,.carousel-inner>.item.next.left,.carousel-inner>.item.prev.right{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0);left:0}}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);background-color:rgba(0,0,0,0);filter:alpha(opacity=50);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.5)),to(rgba(0,0,0,.0001)));background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.0001)),to(rgba(0,0,0,.5)));background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);background-repeat:repeat-x}.carousel-control:focus,.carousel-control:hover{color:#fff;text-decoration:none;outline:0;filter:alpha(opacity=90);opacity:.9}.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{position:absolute;top:50%;z-index:5;display:inline-block;margin-top:-10px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{left:50%;margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{right:50%;margin-right:-10px}.carousel-control .icon-next,.carousel-control .icon-prev{width:20px;height:20px;font-family:serif;line-height:1}.carousel-control .icon-prev:before{content:"\2039"}.carousel-control .icon-next:before{content:"\203a"}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:#000\9;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{width:30px;height:30px;margin-top:-10px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-10px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.btn-group-vertical>.btn-group:after,.btn-group-vertical>.btn-group:before,.btn-toolbar:after,.btn-toolbar:before,.clearfix:after,.clearfix:before,.container-fluid:after,.container-fluid:before,.container:after,.container:before,.dl-horizontal dd:after,.dl-horizontal dd:before,.form-horizontal .form-group:after,.form-horizontal .form-group:before,.modal-footer:after,.modal-footer:before,.modal-header:after,.modal-header:before,.nav:after,.nav:before,.navbar-collapse:after,.navbar-collapse:before,.navbar-header:after,.navbar-header:before,.navbar:after,.navbar:before,.pager:after,.pager:before,.panel-body:after,.panel-body:before,.row:after,.row:before{display:table;content:" "}.btn-group-vertical>.btn-group:after,.btn-toolbar:after,.clearfix:after,.container-fluid:after,.container:after,.dl-horizontal dd:after,.form-horizontal .form-group:after,.modal-footer:after,.modal-header:after,.nav:after,.navbar-collapse:after,.navbar-header:after,.navbar:after,.pager:after,.panel-body:after,.row:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important}.affix{position:fixed}@-ms-viewport{width:device-width}.visible-lg,.visible-md,.visible-sm,.visible-xs{display:none!important}.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table!important}tr.visible-xs{display:table-row!important}td.visible-xs,th.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table!important}tr.visible-sm{display:table-row!important}td.visible-sm,th.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table!important}tr.visible-md{display:table-row!important}td.visible-md,th.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table!important}tr.visible-lg{display:table-row!important}td.visible-lg,th.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table!important}tr.visible-print{display:table-row!important}td.visible-print,th.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}
+/*# sourceMappingURL=bootstrap.min.css.map */
```

### Comparing `yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/js/bootstrap.js` & `yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/js/bootstrap.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,40 @@
 /*!
- * Bootstrap v3.2.0 (http://getbootstrap.com)
- * Copyright 2011-2014 Twitter, Inc.
- * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
+ * Bootstrap v3.4.1 (https://getbootstrap.com/)
+ * Copyright 2011-2019 Twitter, Inc.
+ * Licensed under the MIT license
  */
 
 if (typeof jQuery === 'undefined') {
     throw new Error('Bootstrap\'s JavaScript requires jQuery')
 }
 
++
+function($) {
+    'use strict';
+    var version = $.fn.jquery.split(' ')[0].split('.')
+    if ((version[0] < 2 && version[1] < 9) || (version[0] == 1 && version[1] == 9 && version[2] < 1) || (version[0] > 3)) {
+        throw new Error('Bootstrap\'s JavaScript requires jQuery version 1.9.1 or higher, but lower than version 4')
+    }
+}(jQuery);
+
 /* ========================================================================
- * Bootstrap: transition.js v3.2.0
- * http://getbootstrap.com/javascript/#transitions
+ * Bootstrap: transition.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#transitions
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
 
-    // CSS TRANSITION SUPPORT (Shoutout: http://www.modernizr.com/)
+    // CSS TRANSITION SUPPORT (Shoutout: https://modernizr.com/)
     // ============================================================
 
     function transitionEnd() {
         var el = document.createElement('bootstrap')
 
         var transEndEventNames = {
             WebkitTransition: 'webkitTransitionEnd',
@@ -41,15 +50,15 @@
                 }
             }
         }
 
         return false // explicit for ie8 (  ._.)
     }
 
-    // http://blog.alexmaccaw.com/css-transitions
+    // https://blog.alexmaccaw.com/css-transitions
     $.fn.emulateTransitionEnd = function(duration) {
         var called = false
         var $el = this
         $(this).one('bsTransitionEnd', function() {
             called = true
         })
         var callback = function() {
@@ -72,18 +81,18 @@
             }
         }
     })
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: alert.js v3.2.0
- * http://getbootstrap.com/javascript/#alerts
+ * Bootstrap: alert.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#alerts
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
@@ -92,31 +101,34 @@
     // ======================
 
     var dismiss = '[data-dismiss="alert"]'
     var Alert = function(el) {
         $(el).on('click', dismiss, this.close)
     }
 
-    Alert.VERSION = '3.2.0'
+    Alert.VERSION = '3.4.1'
+
+    Alert.TRANSITION_DURATION = 150
 
     Alert.prototype.close = function(e) {
         var $this = $(this)
         var selector = $this.attr('data-target')
 
         if (!selector) {
             selector = $this.attr('href')
             selector = selector && selector.replace(/.*(?=#[^\s]*$)/, '') // strip for ie7
         }
 
-        var $parent = $(selector)
+        selector = selector === '#' ? [] : selector
+        var $parent = $(document).find(selector)
 
         if (e) e.preventDefault()
 
         if (!$parent.length) {
-            $parent = $this.hasClass('alert') ? $this : $this.parent()
+            $parent = $this.closest('.alert')
         }
 
         $parent.trigger(e = $.Event('close.bs.alert'))
 
         if (e.isDefaultPrevented()) return
 
         $parent.removeClass('in')
@@ -125,15 +137,15 @@
             // detach from parent, fire event then clean up data
             $parent.detach().trigger('closed.bs.alert').remove()
         }
 
         $.support.transition && $parent.hasClass('fade') ?
             $parent
             .one('bsTransitionEnd', removeElement)
-            .emulateTransitionEnd(150) :
+            .emulateTransitionEnd(Alert.TRANSITION_DURATION) :
             removeElement()
     }
 
 
     // ALERT PLUGIN DEFINITION
     // =======================
 
@@ -166,18 +178,18 @@
     // ==============
 
     $(document).on('click.bs.alert.data-api', dismiss, Alert.prototype.close)
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: button.js v3.2.0
- * http://getbootstrap.com/javascript/#buttons
+ * Bootstrap: button.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#buttons
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
@@ -187,58 +199,64 @@
 
     var Button = function(element, options) {
         this.$element = $(element)
         this.options = $.extend({}, Button.DEFAULTS, options)
         this.isLoading = false
     }
 
-    Button.VERSION = '3.2.0'
+    Button.VERSION = '3.4.1'
 
     Button.DEFAULTS = {
         loadingText: 'loading...'
     }
 
     Button.prototype.setState = function(state) {
         var d = 'disabled'
         var $el = this.$element
         var val = $el.is('input') ? 'val' : 'html'
         var data = $el.data()
 
-        state = state + 'Text'
+        state += 'Text'
 
         if (data.resetText == null) $el.data('resetText', $el[val]())
 
-        $el[val](data[state] == null ? this.options[state] : data[state])
-
         // push to event loop to allow forms to submit
         setTimeout($.proxy(function() {
+            $el[val](data[state] == null ? this.options[state] : data[state])
+
             if (state == 'loadingText') {
                 this.isLoading = true
-                $el.addClass(d).attr(d, d)
+                $el.addClass(d).attr(d, d).prop(d, true)
             } else if (this.isLoading) {
                 this.isLoading = false
-                $el.removeClass(d).removeAttr(d)
+                $el.removeClass(d).removeAttr(d).prop(d, false)
             }
         }, this), 0)
     }
 
     Button.prototype.toggle = function() {
         var changed = true
         var $parent = this.$element.closest('[data-toggle="buttons"]')
 
         if ($parent.length) {
             var $input = this.$element.find('input')
             if ($input.prop('type') == 'radio') {
-                if ($input.prop('checked') && this.$element.hasClass('active')) changed = false
-                else $parent.find('.active').removeClass('active')
+                if ($input.prop('checked')) changed = false
+                $parent.find('.active').removeClass('active')
+                this.$element.addClass('active')
+            } else if ($input.prop('type') == 'checkbox') {
+                if (($input.prop('checked')) !== this.$element.hasClass('active')) changed = false
+                this.$element.toggleClass('active')
             }
-            if (changed) $input.prop('checked', !this.$element.hasClass('active')).trigger('change')
+            $input.prop('checked', this.$element.hasClass('active'))
+            if (changed) $input.trigger('change')
+        } else {
+            this.$element.attr('aria-pressed', !this.$element.hasClass('active'))
+            this.$element.toggleClass('active')
         }
-
-        if (changed) this.$element.toggleClass('active')
     }
 
 
     // BUTTON PLUGIN DEFINITION
     // ========================
 
     function Plugin(option) {
@@ -268,63 +286,78 @@
         return this
     }
 
 
     // BUTTON DATA-API
     // ===============
 
-    $(document).on('click.bs.button.data-api', '[data-toggle^="button"]', function(e) {
-        var $btn = $(e.target)
-        if (!$btn.hasClass('btn')) $btn = $btn.closest('.btn')
-        Plugin.call($btn, 'toggle')
-        e.preventDefault()
-    })
+    $(document)
+        .on('click.bs.button.data-api', '[data-toggle^="button"]', function(e) {
+            var $btn = $(e.target).closest('.btn')
+            Plugin.call($btn, 'toggle')
+            if (!($(e.target).is('input[type="radio"], input[type="checkbox"]'))) {
+                // Prevent double click on radios, and the double selections (so cancellation) on checkboxes
+                e.preventDefault()
+                // The target component still receive the focus
+                if ($btn.is('input,button')) $btn.trigger('focus')
+                else $btn.find('input:visible,button:visible').first().trigger('focus')
+            }
+        })
+        .on('focus.bs.button.data-api blur.bs.button.data-api', '[data-toggle^="button"]', function(e) {
+            $(e.target).closest('.btn').toggleClass('focus', /^focus(in)?$/.test(e.type))
+        })
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: carousel.js v3.2.0
- * http://getbootstrap.com/javascript/#carousel
+ * Bootstrap: carousel.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#carousel
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
 
     // CAROUSEL CLASS DEFINITION
     // =========================
 
     var Carousel = function(element, options) {
-        this.$element = $(element).on('keydown.bs.carousel', $.proxy(this.keydown, this))
+        this.$element = $(element)
         this.$indicators = this.$element.find('.carousel-indicators')
         this.options = options
-        this.paused =
-            this.sliding =
-            this.interval =
-            this.$active =
-            this.$items = null
+        this.paused = null
+        this.sliding = null
+        this.interval = null
+        this.$active = null
+        this.$items = null
 
-        this.options.pause == 'hover' && this.$element
+        this.options.keyboard && this.$element.on('keydown.bs.carousel', $.proxy(this.keydown, this))
+
+        this.options.pause == 'hover' && !('ontouchstart' in document.documentElement) && this.$element
             .on('mouseenter.bs.carousel', $.proxy(this.pause, this))
             .on('mouseleave.bs.carousel', $.proxy(this.cycle, this))
     }
 
-    Carousel.VERSION = '3.2.0'
+    Carousel.VERSION = '3.4.1'
+
+    Carousel.TRANSITION_DURATION = 600
 
     Carousel.DEFAULTS = {
         interval: 5000,
         pause: 'hover',
-        wrap: true
+        wrap: true,
+        keyboard: true
     }
 
     Carousel.prototype.keydown = function(e) {
+        if (/input|textarea/i.test(e.target.tagName)) return
         switch (e.which) {
             case 37:
                 this.prev();
                 break
             case 39:
                 this.next();
                 break
@@ -348,26 +381,36 @@
     }
 
     Carousel.prototype.getItemIndex = function(item) {
         this.$items = item.parent().children('.item')
         return this.$items.index(item || this.$active)
     }
 
+    Carousel.prototype.getItemForDirection = function(direction, active) {
+        var activeIndex = this.getItemIndex(active)
+        var willWrap = (direction == 'prev' && activeIndex === 0) ||
+            (direction == 'next' && activeIndex == (this.$items.length - 1))
+        if (willWrap && !this.options.wrap) return active
+        var delta = direction == 'prev' ? -1 : 1
+        var itemIndex = (activeIndex + delta) % this.$items.length
+        return this.$items.eq(itemIndex)
+    }
+
     Carousel.prototype.to = function(pos) {
         var that = this
         var activeIndex = this.getItemIndex(this.$active = this.$element.find('.item.active'))
 
         if (pos > (this.$items.length - 1) || pos < 0) return
 
         if (this.sliding) return this.$element.one('slid.bs.carousel', function() {
             that.to(pos)
         }) // yes, "slid"
         if (activeIndex == pos) return this.pause().cycle()
 
-        return this.slide(pos > activeIndex ? 'next' : 'prev', $(this.$items[pos]))
+        return this.slide(pos > activeIndex ? 'next' : 'prev', this.$items.eq(pos))
     }
 
     Carousel.prototype.pause = function(e) {
         e || (this.paused = true)
 
         if (this.$element.find('.next, .prev').length && $.support.transition) {
             this.$element.trigger($.support.transition.end)
@@ -387,25 +430,19 @@
     Carousel.prototype.prev = function() {
         if (this.sliding) return
         return this.slide('prev')
     }
 
     Carousel.prototype.slide = function(type, next) {
         var $active = this.$element.find('.item.active')
-        var $next = next || $active[type]()
+        var $next = next || this.getItemForDirection(type, $active)
         var isCycling = this.interval
         var direction = type == 'next' ? 'left' : 'right'
-        var fallback = type == 'next' ? 'first' : 'last'
         var that = this
 
-        if (!$next.length) {
-            if (!this.options.wrap) return
-            $next = this.$element.find('.item')[fallback]()
-        }
-
         if ($next.hasClass('active')) return (this.sliding = false)
 
         var relatedTarget = $next[0]
         var slideEvent = $.Event('slide.bs.carousel', {
             relatedTarget: relatedTarget,
             direction: direction
         })
@@ -424,27 +461,29 @@
 
         var slidEvent = $.Event('slid.bs.carousel', {
             relatedTarget: relatedTarget,
             direction: direction
         }) // yes, "slid"
         if ($.support.transition && this.$element.hasClass('slide')) {
             $next.addClass(type)
-            $next[0].offsetWidth // force reflow
+            if (typeof $next === 'object' && $next.length) {
+                $next[0].offsetWidth // force reflow
+            }
             $active.addClass(direction)
             $next.addClass(direction)
             $active
                 .one('bsTransitionEnd', function() {
                     $next.removeClass([type, direction].join(' ')).addClass('active')
                     $active.removeClass(['active', direction].join(' '))
                     that.sliding = false
                     setTimeout(function() {
                         that.$element.trigger(slidEvent)
                     }, 0)
                 })
-                .emulateTransitionEnd($active.css('transition-duration').slice(0, -1) * 1000)
+                .emulateTransitionEnd(Carousel.TRANSITION_DURATION)
         } else {
             $active.removeClass('active')
             $next.addClass('active')
             this.sliding = false
             this.$element.trigger(slidEvent)
         }
 
@@ -485,98 +524,128 @@
         return this
     }
 
 
     // CAROUSEL DATA-API
     // =================
 
-    $(document).on('click.bs.carousel.data-api', '[data-slide], [data-slide-to]', function(e) {
-        var href
+    var clickHandler = function(e) {
         var $this = $(this)
-        var $target = $($this.attr('data-target') || (href = $this.attr('href')) && href.replace(/.*(?=#[^\s]+$)/, '')) // strip for ie7
+        var href = $this.attr('href')
+        if (href) {
+            href = href.replace(/.*(?=#[^\s]+$)/, '') // strip for ie7
+        }
+
+        var target = $this.attr('data-target') || href
+        var $target = $(document).find(target)
+
         if (!$target.hasClass('carousel')) return
+
         var options = $.extend({}, $target.data(), $this.data())
         var slideIndex = $this.attr('data-slide-to')
         if (slideIndex) options.interval = false
 
         Plugin.call($target, options)
 
         if (slideIndex) {
             $target.data('bs.carousel').to(slideIndex)
         }
 
         e.preventDefault()
-    })
+    }
+
+    $(document)
+        .on('click.bs.carousel.data-api', '[data-slide]', clickHandler)
+        .on('click.bs.carousel.data-api', '[data-slide-to]', clickHandler)
 
     $(window).on('load', function() {
         $('[data-ride="carousel"]').each(function() {
             var $carousel = $(this)
             Plugin.call($carousel, $carousel.data())
         })
     })
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: collapse.js v3.2.0
- * http://getbootstrap.com/javascript/#collapse
+ * Bootstrap: collapse.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#collapse
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
+/* jshint latedef: false */
 
 +
 function($) {
     'use strict';
 
     // COLLAPSE PUBLIC CLASS DEFINITION
     // ================================
 
     var Collapse = function(element, options) {
         this.$element = $(element)
         this.options = $.extend({}, Collapse.DEFAULTS, options)
+        this.$trigger = $('[data-toggle="collapse"][href="#' + element.id + '"],' +
+            '[data-toggle="collapse"][data-target="#' + element.id + '"]')
         this.transitioning = null
 
-        if (this.options.parent) this.$parent = $(this.options.parent)
+        if (this.options.parent) {
+            this.$parent = this.getParent()
+        } else {
+            this.addAriaAndCollapsedClass(this.$element, this.$trigger)
+        }
+
         if (this.options.toggle) this.toggle()
     }
 
-    Collapse.VERSION = '3.2.0'
+    Collapse.VERSION = '3.4.1'
+
+    Collapse.TRANSITION_DURATION = 350
 
     Collapse.DEFAULTS = {
         toggle: true
     }
 
     Collapse.prototype.dimension = function() {
         var hasWidth = this.$element.hasClass('width')
         return hasWidth ? 'width' : 'height'
     }
 
     Collapse.prototype.show = function() {
         if (this.transitioning || this.$element.hasClass('in')) return
 
+        var activesData
+        var actives = this.$parent && this.$parent.children('.panel').children('.in, .collapsing')
+
+        if (actives && actives.length) {
+            activesData = actives.data('bs.collapse')
+            if (activesData && activesData.transitioning) return
+        }
+
         var startEvent = $.Event('show.bs.collapse')
         this.$element.trigger(startEvent)
         if (startEvent.isDefaultPrevented()) return
 
-        var actives = this.$parent && this.$parent.find('> .panel > .in')
-
         if (actives && actives.length) {
-            var hasData = actives.data('bs.collapse')
-            if (hasData && hasData.transitioning) return
             Plugin.call(actives, 'hide')
-            hasData || actives.data('bs.collapse', null)
+            activesData || actives.data('bs.collapse', null)
         }
 
         var dimension = this.dimension()
 
         this.$element
             .removeClass('collapse')
             .addClass('collapsing')[dimension](0)
+            .attr('aria-expanded', true)
+
+        this.$trigger
+            .removeClass('collapsed')
+            .attr('aria-expanded', true)
 
         this.transitioning = 1
 
         var complete = function() {
             this.$element
                 .removeClass('collapsing')
                 .addClass('collapse in')[dimension]('')
@@ -587,15 +656,15 @@
 
         if (!$.support.transition) return complete.call(this)
 
         var scrollSize = $.camelCase(['scroll', dimension].join('-'))
 
         this.$element
             .one('bsTransitionEnd', $.proxy(complete, this))
-            .emulateTransitionEnd(350)[dimension](this.$element[0][scrollSize])
+            .emulateTransitionEnd(Collapse.TRANSITION_DURATION)[dimension](this.$element[0][scrollSize])
     }
 
     Collapse.prototype.hide = function() {
         if (this.transitioning || !this.$element.hasClass('in')) return
 
         var startEvent = $.Event('hide.bs.collapse')
         this.$element.trigger(startEvent)
@@ -603,49 +672,80 @@
 
         var dimension = this.dimension()
 
         this.$element[dimension](this.$element[dimension]())[0].offsetHeight
 
         this.$element
             .addClass('collapsing')
-            .removeClass('collapse')
-            .removeClass('in')
+            .removeClass('collapse in')
+            .attr('aria-expanded', false)
+
+        this.$trigger
+            .addClass('collapsed')
+            .attr('aria-expanded', false)
 
         this.transitioning = 1
 
         var complete = function() {
             this.transitioning = 0
             this.$element
-                .trigger('hidden.bs.collapse')
                 .removeClass('collapsing')
                 .addClass('collapse')
+                .trigger('hidden.bs.collapse')
         }
 
         if (!$.support.transition) return complete.call(this)
 
         this.$element[dimension](0)
             .one('bsTransitionEnd', $.proxy(complete, this))
-            .emulateTransitionEnd(350)
+            .emulateTransitionEnd(Collapse.TRANSITION_DURATION)
     }
 
     Collapse.prototype.toggle = function() {
         this[this.$element.hasClass('in') ? 'hide' : 'show']()
     }
 
+    Collapse.prototype.getParent = function() {
+        return $(document).find(this.options.parent)
+            .find('[data-toggle="collapse"][data-parent="' + this.options.parent + '"]')
+            .each($.proxy(function(i, element) {
+                var $element = $(element)
+                this.addAriaAndCollapsedClass(getTargetFromTrigger($element), $element)
+            }, this))
+            .end()
+    }
+
+    Collapse.prototype.addAriaAndCollapsedClass = function($element, $trigger) {
+        var isOpen = $element.hasClass('in')
+
+        $element.attr('aria-expanded', isOpen)
+        $trigger
+            .toggleClass('collapsed', !isOpen)
+            .attr('aria-expanded', isOpen)
+    }
+
+    function getTargetFromTrigger($trigger) {
+        var href
+        var target = $trigger.attr('data-target') ||
+            (href = $trigger.attr('href')) && href.replace(/.*(?=#[^\s]+$)/, '') // strip for ie7
+
+        return $(document).find(target)
+    }
+
 
     // COLLAPSE PLUGIN DEFINITION
     // ==========================
 
     function Plugin(option) {
         return this.each(function() {
             var $this = $(this)
             var data = $this.data('bs.collapse')
             var options = $.extend({}, Collapse.DEFAULTS, $this.data(), typeof option == 'object' && option)
 
-            if (!data && options.toggle && option == 'show') option = !option
+            if (!data && options.toggle && /show|hide/.test(option)) options.toggle = false
             if (!data) $this.data('bs.collapse', (data = new Collapse(this, options)))
             if (typeof option == 'string') data[option]()
         })
     }
 
     var old = $.fn.collapse
 
@@ -662,40 +762,32 @@
     }
 
 
     // COLLAPSE DATA-API
     // =================
 
     $(document).on('click.bs.collapse.data-api', '[data-toggle="collapse"]', function(e) {
-        var href
         var $this = $(this)
-        var target = $this.attr('data-target') ||
-            e.preventDefault() ||
-            (href = $this.attr('href')) && href.replace(/.*(?=#[^\s]+$)/, '') // strip for ie7
-        var $target = $(target)
+
+        if (!$this.attr('data-target')) e.preventDefault()
+
+        var $target = getTargetFromTrigger($this)
         var data = $target.data('bs.collapse')
         var option = data ? 'toggle' : $this.data()
-        var parent = $this.attr('data-parent')
-        var $parent = parent && $(parent)
-
-        if (!data || !data.transitioning) {
-            if ($parent) $parent.find('[data-toggle="collapse"][data-parent="' + parent + '"]').not($this).addClass('collapsed')
-            $this[$target.hasClass('in') ? 'addClass' : 'removeClass']('collapsed')
-        }
 
         Plugin.call($target, option)
     })
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: dropdown.js v3.2.0
- * http://getbootstrap.com/javascript/#dropdowns
+ * Bootstrap: dropdown.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#dropdowns
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
@@ -705,109 +797,122 @@
 
     var backdrop = '.dropdown-backdrop'
     var toggle = '[data-toggle="dropdown"]'
     var Dropdown = function(element) {
         $(element).on('click.bs.dropdown', this.toggle)
     }
 
-    Dropdown.VERSION = '3.2.0'
+    Dropdown.VERSION = '3.4.1'
+
+    function getParent($this) {
+        var selector = $this.attr('data-target')
+
+        if (!selector) {
+            selector = $this.attr('href')
+            selector = selector && /#[A-Za-z]/.test(selector) && selector.replace(/.*(?=#[^\s]*$)/, '') // strip for ie7
+        }
+
+        var $parent = selector !== '#' ? $(document).find(selector) : null
+
+        return $parent && $parent.length ? $parent : $this.parent()
+    }
+
+    function clearMenus(e) {
+        if (e && e.which === 3) return
+        $(backdrop).remove()
+        $(toggle).each(function() {
+            var $this = $(this)
+            var $parent = getParent($this)
+            var relatedTarget = {
+                relatedTarget: this
+            }
+
+            if (!$parent.hasClass('open')) return
+
+            if (e && e.type == 'click' && /input|textarea/i.test(e.target.tagName) && $.contains($parent[0], e.target)) return
+
+            $parent.trigger(e = $.Event('hide.bs.dropdown', relatedTarget))
+
+            if (e.isDefaultPrevented()) return
+
+            $this.attr('aria-expanded', 'false')
+            $parent.removeClass('open').trigger($.Event('hidden.bs.dropdown', relatedTarget))
+        })
+    }
 
     Dropdown.prototype.toggle = function(e) {
         var $this = $(this)
 
         if ($this.is('.disabled, :disabled')) return
 
         var $parent = getParent($this)
         var isActive = $parent.hasClass('open')
 
         clearMenus()
 
         if (!isActive) {
             if ('ontouchstart' in document.documentElement && !$parent.closest('.navbar-nav').length) {
                 // if mobile we use a backdrop because click events don't delegate
-                $('<div class="dropdown-backdrop"/>').insertAfter($(this)).on('click', clearMenus)
+                $(document.createElement('div'))
+                    .addClass('dropdown-backdrop')
+                    .insertAfter($(this))
+                    .on('click', clearMenus)
             }
 
             var relatedTarget = {
                 relatedTarget: this
             }
             $parent.trigger(e = $.Event('show.bs.dropdown', relatedTarget))
 
             if (e.isDefaultPrevented()) return
 
-            $this.trigger('focus')
+            $this
+                .trigger('focus')
+                .attr('aria-expanded', 'true')
 
             $parent
                 .toggleClass('open')
-                .trigger('shown.bs.dropdown', relatedTarget)
+                .trigger($.Event('shown.bs.dropdown', relatedTarget))
         }
 
         return false
     }
 
     Dropdown.prototype.keydown = function(e) {
-        if (!/(38|40|27)/.test(e.keyCode)) return
+        if (!/(38|40|27|32)/.test(e.which) || /input|textarea/i.test(e.target.tagName)) return
 
         var $this = $(this)
 
         e.preventDefault()
         e.stopPropagation()
 
         if ($this.is('.disabled, :disabled')) return
 
         var $parent = getParent($this)
         var isActive = $parent.hasClass('open')
 
-        if (!isActive || (isActive && e.keyCode == 27)) {
+        if (!isActive && e.which != 27 || isActive && e.which == 27) {
             if (e.which == 27) $parent.find(toggle).trigger('focus')
             return $this.trigger('click')
         }
 
-        var desc = ' li:not(.divider):visible a'
-        var $items = $parent.find('[role="menu"]' + desc + ', [role="listbox"]' + desc)
+        var desc = ' li:not(.disabled):visible a'
+        var $items = $parent.find('.dropdown-menu' + desc)
 
         if (!$items.length) return
 
-        var index = $items.index($items.filter(':focus'))
+        var index = $items.index(e.target)
 
-        if (e.keyCode == 38 && index > 0) index-- // up
-        if (e.keyCode == 40 && index < $items.length - 1) index++ // down
+        if (e.which == 38 && index > 0) index-- // up
+        if (e.which == 40 && index < $items.length - 1) index++ // down
         if (!~index) index = 0
 
         $items.eq(index).trigger('focus')
     }
 
-    function clearMenus(e) {
-        if (e && e.which === 3) return
-        $(backdrop).remove()
-        $(toggle).each(function() {
-            var $parent = getParent($(this))
-            var relatedTarget = {
-                relatedTarget: this
-            }
-            if (!$parent.hasClass('open')) return
-            $parent.trigger(e = $.Event('hide.bs.dropdown', relatedTarget))
-            if (e.isDefaultPrevented()) return
-            $parent.removeClass('open').trigger('hidden.bs.dropdown', relatedTarget)
-        })
-    }
-
-    function getParent($this) {
-        var selector = $this.attr('data-target')
-
-        if (!selector) {
-            selector = $this.attr('href')
-            selector = selector && /#[A-Za-z]/.test(selector) && selector.replace(/.*(?=#[^\s]*$)/, '') // strip for ie7
-        }
-
-        var $parent = selector && $(selector)
-
-        return $parent && $parent.length ? $parent : $this.parent()
-    }
-
 
     // DROPDOWN PLUGIN DEFINITION
     // ==========================
 
     function Plugin(option) {
         return this.each(function() {
             var $this = $(this)
@@ -838,23 +943,24 @@
 
     $(document)
         .on('click.bs.dropdown.data-api', clearMenus)
         .on('click.bs.dropdown.data-api', '.dropdown form', function(e) {
             e.stopPropagation()
         })
         .on('click.bs.dropdown.data-api', toggle, Dropdown.prototype.toggle)
-        .on('keydown.bs.dropdown.data-api', toggle + ', [role="menu"], [role="listbox"]', Dropdown.prototype.keydown)
+        .on('keydown.bs.dropdown.data-api', toggle, Dropdown.prototype.keydown)
+        .on('keydown.bs.dropdown.data-api', '.dropdown-menu', Dropdown.prototype.keydown)
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: modal.js v3.2.0
- * http://getbootstrap.com/javascript/#modals
+ * Bootstrap: modal.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#modals
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
@@ -862,28 +968,35 @@
     // MODAL CLASS DEFINITION
     // ======================
 
     var Modal = function(element, options) {
         this.options = options
         this.$body = $(document.body)
         this.$element = $(element)
-        this.$backdrop =
-            this.isShown = null
+        this.$dialog = this.$element.find('.modal-dialog')
+        this.$backdrop = null
+        this.isShown = null
+        this.originalBodyPad = null
         this.scrollbarWidth = 0
+        this.ignoreBackdropClick = false
+        this.fixedContent = '.navbar-fixed-top, .navbar-fixed-bottom'
 
         if (this.options.remote) {
             this.$element
                 .find('.modal-content')
                 .load(this.options.remote, $.proxy(function() {
                     this.$element.trigger('loaded.bs.modal')
                 }, this))
         }
     }
 
-    Modal.VERSION = '3.2.0'
+    Modal.VERSION = '3.4.1'
+
+    Modal.TRANSITION_DURATION = 300
+    Modal.BACKDROP_TRANSITION_DURATION = 150
 
     Modal.DEFAULTS = {
         backdrop: true,
         keyboard: true,
         show: true
     }
 
@@ -900,52 +1013,59 @@
         this.$element.trigger(e)
 
         if (this.isShown || e.isDefaultPrevented()) return
 
         this.isShown = true
 
         this.checkScrollbar()
+        this.setScrollbar()
         this.$body.addClass('modal-open')
 
-        this.setScrollbar()
         this.escape()
+        this.resize()
 
         this.$element.on('click.dismiss.bs.modal', '[data-dismiss="modal"]', $.proxy(this.hide, this))
 
+        this.$dialog.on('mousedown.dismiss.bs.modal', function() {
+            that.$element.one('mouseup.dismiss.bs.modal', function(e) {
+                if ($(e.target).is(that.$element)) that.ignoreBackdropClick = true
+            })
+        })
+
         this.backdrop(function() {
             var transition = $.support.transition && that.$element.hasClass('fade')
 
             if (!that.$element.parent().length) {
                 that.$element.appendTo(that.$body) // don't move modals dom position
             }
 
             that.$element
                 .show()
                 .scrollTop(0)
 
+            that.adjustDialog()
+
             if (transition) {
                 that.$element[0].offsetWidth // force reflow
             }
 
-            that.$element
-                .addClass('in')
-                .attr('aria-hidden', false)
+            that.$element.addClass('in')
 
             that.enforceFocus()
 
             var e = $.Event('shown.bs.modal', {
                 relatedTarget: _relatedTarget
             })
 
             transition ?
-                that.$element.find('.modal-dialog') // wait for modal to slide in
+                that.$dialog // wait for modal to slide in
                 .one('bsTransitionEnd', function() {
                     that.$element.trigger('focus').trigger(e)
                 })
-                .emulateTransitionEnd(300) :
+                .emulateTransitionEnd(Modal.TRANSITION_DURATION) :
                 that.$element.trigger('focus').trigger(e)
         })
     }
 
     Modal.prototype.hide = function(e) {
         if (e) e.preventDefault()
 
@@ -953,57 +1073,70 @@
 
         this.$element.trigger(e)
 
         if (!this.isShown || e.isDefaultPrevented()) return
 
         this.isShown = false
 
-        this.$body.removeClass('modal-open')
-
-        this.resetScrollbar()
         this.escape()
+        this.resize()
 
         $(document).off('focusin.bs.modal')
 
         this.$element
             .removeClass('in')
-            .attr('aria-hidden', true)
             .off('click.dismiss.bs.modal')
+            .off('mouseup.dismiss.bs.modal')
+
+        this.$dialog.off('mousedown.dismiss.bs.modal')
 
         $.support.transition && this.$element.hasClass('fade') ?
             this.$element
             .one('bsTransitionEnd', $.proxy(this.hideModal, this))
-            .emulateTransitionEnd(300) :
+            .emulateTransitionEnd(Modal.TRANSITION_DURATION) :
             this.hideModal()
     }
 
     Modal.prototype.enforceFocus = function() {
         $(document)
             .off('focusin.bs.modal') // guard against infinite focus loop
             .on('focusin.bs.modal', $.proxy(function(e) {
-                if (this.$element[0] !== e.target && !this.$element.has(e.target).length) {
+                if (document !== e.target &&
+                    this.$element[0] !== e.target &&
+                    !this.$element.has(e.target).length) {
                     this.$element.trigger('focus')
                 }
             }, this))
     }
 
     Modal.prototype.escape = function() {
         if (this.isShown && this.options.keyboard) {
-            this.$element.on('keyup.dismiss.bs.modal', $.proxy(function(e) {
+            this.$element.on('keydown.dismiss.bs.modal', $.proxy(function(e) {
                 e.which == 27 && this.hide()
             }, this))
         } else if (!this.isShown) {
-            this.$element.off('keyup.dismiss.bs.modal')
+            this.$element.off('keydown.dismiss.bs.modal')
+        }
+    }
+
+    Modal.prototype.resize = function() {
+        if (this.isShown) {
+            $(window).on('resize.bs.modal', $.proxy(this.handleUpdate, this))
+        } else {
+            $(window).off('resize.bs.modal')
         }
     }
 
     Modal.prototype.hideModal = function() {
         var that = this
         this.$element.hide()
         this.backdrop(function() {
+            that.$body.removeClass('modal-open')
+            that.resetAdjustments()
+            that.resetScrollbar()
             that.$element.trigger('hidden.bs.modal')
         })
     }
 
     Modal.prototype.removeBackdrop = function() {
         this.$backdrop && this.$backdrop.remove()
         this.$backdrop = null
@@ -1012,66 +1145,114 @@
     Modal.prototype.backdrop = function(callback) {
         var that = this
         var animate = this.$element.hasClass('fade') ? 'fade' : ''
 
         if (this.isShown && this.options.backdrop) {
             var doAnimate = $.support.transition && animate
 
-            this.$backdrop = $('<div class="modal-backdrop ' + animate + '" />')
+            this.$backdrop = $(document.createElement('div'))
+                .addClass('modal-backdrop ' + animate)
                 .appendTo(this.$body)
 
             this.$element.on('click.dismiss.bs.modal', $.proxy(function(e) {
+                if (this.ignoreBackdropClick) {
+                    this.ignoreBackdropClick = false
+                    return
+                }
                 if (e.target !== e.currentTarget) return
                 this.options.backdrop == 'static' ?
-                    this.$element[0].focus.call(this.$element[0]) :
-                    this.hide.call(this)
+                    this.$element[0].focus() :
+                    this.hide()
             }, this))
 
             if (doAnimate) this.$backdrop[0].offsetWidth // force reflow
 
             this.$backdrop.addClass('in')
 
             if (!callback) return
 
             doAnimate ?
                 this.$backdrop
                 .one('bsTransitionEnd', callback)
-                .emulateTransitionEnd(150) :
+                .emulateTransitionEnd(Modal.BACKDROP_TRANSITION_DURATION) :
                 callback()
 
         } else if (!this.isShown && this.$backdrop) {
             this.$backdrop.removeClass('in')
 
             var callbackRemove = function() {
                 that.removeBackdrop()
                 callback && callback()
             }
             $.support.transition && this.$element.hasClass('fade') ?
                 this.$backdrop
                 .one('bsTransitionEnd', callbackRemove)
-                .emulateTransitionEnd(150) :
+                .emulateTransitionEnd(Modal.BACKDROP_TRANSITION_DURATION) :
                 callbackRemove()
 
         } else if (callback) {
             callback()
         }
     }
 
+    // these following methods are used to handle overflowing modals
+
+    Modal.prototype.handleUpdate = function() {
+        this.adjustDialog()
+    }
+
+    Modal.prototype.adjustDialog = function() {
+        var modalIsOverflowing = this.$element[0].scrollHeight > document.documentElement.clientHeight
+
+        this.$element.css({
+            paddingLeft: !this.bodyIsOverflowing && modalIsOverflowing ? this.scrollbarWidth : '',
+            paddingRight: this.bodyIsOverflowing && !modalIsOverflowing ? this.scrollbarWidth : ''
+        })
+    }
+
+    Modal.prototype.resetAdjustments = function() {
+        this.$element.css({
+            paddingLeft: '',
+            paddingRight: ''
+        })
+    }
+
     Modal.prototype.checkScrollbar = function() {
-        if (document.body.clientWidth >= window.innerWidth) return
-        this.scrollbarWidth = this.scrollbarWidth || this.measureScrollbar()
+        var fullWindowWidth = window.innerWidth
+        if (!fullWindowWidth) { // workaround for missing window.innerWidth in IE8
+            var documentElementRect = document.documentElement.getBoundingClientRect()
+            fullWindowWidth = documentElementRect.right - Math.abs(documentElementRect.left)
+        }
+        this.bodyIsOverflowing = document.body.clientWidth < fullWindowWidth
+        this.scrollbarWidth = this.measureScrollbar()
     }
 
     Modal.prototype.setScrollbar = function() {
         var bodyPad = parseInt((this.$body.css('padding-right') || 0), 10)
-        if (this.scrollbarWidth) this.$body.css('padding-right', bodyPad + this.scrollbarWidth)
+        this.originalBodyPad = document.body.style.paddingRight || ''
+        var scrollbarWidth = this.scrollbarWidth
+        if (this.bodyIsOverflowing) {
+            this.$body.css('padding-right', bodyPad + scrollbarWidth)
+            $(this.fixedContent).each(function(index, element) {
+                var actualPadding = element.style.paddingRight
+                var calculatedPadding = $(element).css('padding-right')
+                $(element)
+                    .data('padding-right', actualPadding)
+                    .css('padding-right', parseFloat(calculatedPadding) + scrollbarWidth + 'px')
+            })
+        }
     }
 
     Modal.prototype.resetScrollbar = function() {
-        this.$body.css('padding-right', '')
+        this.$body.css('padding-right', this.originalBodyPad)
+        $(this.fixedContent).each(function(index, element) {
+            var padding = $(element).data('padding-right')
+            $(element).removeData('padding-right')
+            element.style.paddingRight = padding ? padding : ''
+        })
     }
 
     Modal.prototype.measureScrollbar = function() { // thx walsh
         var scrollDiv = document.createElement('div')
         scrollDiv.className = 'modal-scrollbar-measure'
         this.$body.append(scrollDiv)
         var scrollbarWidth = scrollDiv.offsetWidth - scrollDiv.clientWidth
@@ -1112,15 +1293,18 @@
 
     // MODAL DATA-API
     // ==============
 
     $(document).on('click.bs.modal.data-api', '[data-toggle="modal"]', function(e) {
         var $this = $(this)
         var href = $this.attr('href')
-        var $target = $($this.attr('data-target') || (href && href.replace(/.*(?=#[^\s]+$)/, ''))) // strip for ie7
+        var target = $this.attr('data-target') ||
+            (href && href.replace(/.*(?=#[^\s]+$)/, '')) // strip for ie7
+
+        var $target = $(document).find(target)
         var option = $target.data('bs.modal') ? 'toggle' : $.extend({
             remote: !/#/.test(href) && href
         }, $target.data(), $this.data())
 
         if ($this.is('a')) e.preventDefault()
 
         $target.one('show.bs.modal', function(showEvent) {
@@ -1131,65 +1315,214 @@
         })
         Plugin.call($target, option, this)
     })
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: tooltip.js v3.2.0
- * http://getbootstrap.com/javascript/#tooltip
+ * Bootstrap: tooltip.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#tooltip
  * Inspired by the original jQuery.tipsy by Jason Frame
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
-
 +
 function($) {
     'use strict';
 
+    var DISALLOWED_ATTRIBUTES = ['sanitize', 'whiteList', 'sanitizeFn']
+
+    var uriAttrs = [
+        'background',
+        'cite',
+        'href',
+        'itemtype',
+        'longdesc',
+        'poster',
+        'src',
+        'xlink:href'
+    ]
+
+    var ARIA_ATTRIBUTE_PATTERN = /^aria-[\w-]*$/i
+
+    var DefaultWhitelist = {
+        // Global attributes allowed on any supplied element below.
+        '*': ['class', 'dir', 'id', 'lang', 'role', ARIA_ATTRIBUTE_PATTERN],
+        a: ['target', 'href', 'title', 'rel'],
+        area: [],
+        b: [],
+        br: [],
+        col: [],
+        code: [],
+        div: [],
+        em: [],
+        hr: [],
+        h1: [],
+        h2: [],
+        h3: [],
+        h4: [],
+        h5: [],
+        h6: [],
+        i: [],
+        img: ['src', 'alt', 'title', 'width', 'height'],
+        li: [],
+        ol: [],
+        p: [],
+        pre: [],
+        s: [],
+        small: [],
+        span: [],
+        sub: [],
+        sup: [],
+        strong: [],
+        u: [],
+        ul: []
+    }
+
+    /**
+     * A pattern that recognizes a commonly useful subset of URLs that are safe.
+     *
+     * Shoutout to Angular 7 https://github.com/angular/angular/blob/7.2.4/packages/core/src/sanitization/url_sanitizer.ts
+     */
+    var SAFE_URL_PATTERN = /^(?:(?:https?|mailto|ftp|tel|file):|[^&:/?#]*(?:[/?#]|$))/gi
+
+    /**
+     * A pattern that matches safe data URLs. Only matches image, video and audio types.
+     *
+     * Shoutout to Angular 7 https://github.com/angular/angular/blob/7.2.4/packages/core/src/sanitization/url_sanitizer.ts
+     */
+    var DATA_URL_PATTERN = /^data:(?:image\/(?:bmp|gif|jpeg|jpg|png|tiff|webp)|video\/(?:mpeg|mp4|ogg|webm)|audio\/(?:mp3|oga|ogg|opus));base64,[a-z0-9+/]+=*$/i
+
+    function allowedAttribute(attr, allowedAttributeList) {
+        var attrName = attr.nodeName.toLowerCase()
+
+        if ($.inArray(attrName, allowedAttributeList) !== -1) {
+            if ($.inArray(attrName, uriAttrs) !== -1) {
+                return Boolean(attr.nodeValue.match(SAFE_URL_PATTERN) || attr.nodeValue.match(DATA_URL_PATTERN))
+            }
+
+            return true
+        }
+
+        var regExp = $(allowedAttributeList).filter(function(index, value) {
+            return value instanceof RegExp
+        })
+
+        // Check if a regular expression validates the attribute.
+        for (var i = 0, l = regExp.length; i < l; i++) {
+            if (attrName.match(regExp[i])) {
+                return true
+            }
+        }
+
+        return false
+    }
+
+    function sanitizeHtml(unsafeHtml, whiteList, sanitizeFn) {
+        if (unsafeHtml.length === 0) {
+            return unsafeHtml
+        }
+
+        if (sanitizeFn && typeof sanitizeFn === 'function') {
+            return sanitizeFn(unsafeHtml)
+        }
+
+        // IE 8 and below don't support createHTMLDocument
+        if (!document.implementation || !document.implementation.createHTMLDocument) {
+            return unsafeHtml
+        }
+
+        var createdDocument = document.implementation.createHTMLDocument('sanitization')
+        createdDocument.body.innerHTML = unsafeHtml
+
+        var whitelistKeys = $.map(whiteList, function(el, i) {
+            return i
+        })
+        var elements = $(createdDocument.body).find('*')
+
+        for (var i = 0, len = elements.length; i < len; i++) {
+            var el = elements[i]
+            var elName = el.nodeName.toLowerCase()
+
+            if ($.inArray(elName, whitelistKeys) === -1) {
+                el.parentNode.removeChild(el)
+
+                continue
+            }
+
+            var attributeList = $.map(el.attributes, function(el) {
+                return el
+            })
+            var whitelistedAttributes = [].concat(whiteList['*'] || [], whiteList[elName] || [])
+
+            for (var j = 0, len2 = attributeList.length; j < len2; j++) {
+                if (!allowedAttribute(attributeList[j], whitelistedAttributes)) {
+                    el.removeAttribute(attributeList[j].nodeName)
+                }
+            }
+        }
+
+        return createdDocument.body.innerHTML
+    }
+
     // TOOLTIP PUBLIC CLASS DEFINITION
     // ===============================
 
     var Tooltip = function(element, options) {
-        this.type =
-            this.options =
-            this.enabled =
-            this.timeout =
-            this.hoverState =
-            this.$element = null
+        this.type = null
+        this.options = null
+        this.enabled = null
+        this.timeout = null
+        this.hoverState = null
+        this.$element = null
+        this.inState = null
 
         this.init('tooltip', element, options)
     }
 
-    Tooltip.VERSION = '3.2.0'
+    Tooltip.VERSION = '3.4.1'
+
+    Tooltip.TRANSITION_DURATION = 150
 
     Tooltip.DEFAULTS = {
         animation: true,
         placement: 'top',
         selector: false,
         template: '<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>',
         trigger: 'hover focus',
         title: '',
         delay: 0,
         html: false,
         container: false,
         viewport: {
             selector: 'body',
             padding: 0
-        }
+        },
+        sanitize: true,
+        sanitizeFn: null,
+        whiteList: DefaultWhitelist
     }
 
     Tooltip.prototype.init = function(type, element, options) {
         this.enabled = true
         this.type = type
         this.$element = $(element)
         this.options = this.getOptions(options)
-        this.$viewport = this.options.viewport && $(this.options.viewport.selector || this.options.viewport)
+        this.$viewport = this.options.viewport && $(document).find($.isFunction(this.options.viewport) ? this.options.viewport.call(this, this.$element) : (this.options.viewport.selector || this.options.viewport))
+        this.inState = {
+            click: false,
+            hover: false,
+            focus: false
+        }
+
+        if (this.$element[0] instanceof document.constructor && !this.options.selector) {
+            throw new Error('`selector` option must be specified when initializing ' + this.type + ' on the window.document object!')
+        }
 
         var triggers = this.options.trigger.split(' ')
 
         for (var i = triggers.length; i--;) {
             var trigger = triggers[i]
 
             if (trigger == 'click') {
@@ -1212,23 +1545,35 @@
     }
 
     Tooltip.prototype.getDefaults = function() {
         return Tooltip.DEFAULTS
     }
 
     Tooltip.prototype.getOptions = function(options) {
-        options = $.extend({}, this.getDefaults(), this.$element.data(), options)
+        var dataAttributes = this.$element.data()
+
+        for (var dataAttr in dataAttributes) {
+            if (dataAttributes.hasOwnProperty(dataAttr) && $.inArray(dataAttr, DISALLOWED_ATTRIBUTES) !== -1) {
+                delete dataAttributes[dataAttr]
+            }
+        }
+
+        options = $.extend({}, this.getDefaults(), dataAttributes, options)
 
         if (options.delay && typeof options.delay == 'number') {
             options.delay = {
                 show: options.delay,
                 hide: options.delay
             }
         }
 
+        if (options.sanitize) {
+            options.template = sanitizeHtml(options.template, options.whiteList, options.sanitizeFn)
+        }
+
         return options
     }
 
     Tooltip.prototype.getDelegateOptions = function() {
         var options = {}
         var defaults = this.getDefaults()
 
@@ -1244,34 +1589,57 @@
             obj : $(obj.currentTarget).data('bs.' + this.type)
 
         if (!self) {
             self = new this.constructor(obj.currentTarget, this.getDelegateOptions())
             $(obj.currentTarget).data('bs.' + this.type, self)
         }
 
+        if (obj instanceof $.Event) {
+            self.inState[obj.type == 'focusin' ? 'focus' : 'hover'] = true
+        }
+
+        if (self.tip().hasClass('in') || self.hoverState == 'in') {
+            self.hoverState = 'in'
+            return
+        }
+
         clearTimeout(self.timeout)
 
         self.hoverState = 'in'
 
         if (!self.options.delay || !self.options.delay.show) return self.show()
 
         self.timeout = setTimeout(function() {
             if (self.hoverState == 'in') self.show()
         }, self.options.delay.show)
     }
 
+    Tooltip.prototype.isInStateTrue = function() {
+        for (var key in this.inState) {
+            if (this.inState[key]) return true
+        }
+
+        return false
+    }
+
     Tooltip.prototype.leave = function(obj) {
         var self = obj instanceof this.constructor ?
             obj : $(obj.currentTarget).data('bs.' + this.type)
 
         if (!self) {
             self = new this.constructor(obj.currentTarget, this.getDelegateOptions())
             $(obj.currentTarget).data('bs.' + this.type, self)
         }
 
+        if (obj instanceof $.Event) {
+            self.inState[obj.type == 'focusout' ? 'focus' : 'hover'] = false
+        }
+
+        if (self.isInStateTrue()) return
+
         clearTimeout(self.timeout)
 
         self.hoverState = 'out'
 
         if (!self.options.delay || !self.options.delay.hide) return self.hide()
 
         self.timeout = setTimeout(function() {
@@ -1281,15 +1649,15 @@
 
     Tooltip.prototype.show = function() {
         var e = $.Event('show.bs.' + this.type)
 
         if (this.hasContent() && this.enabled) {
             this.$element.trigger(e)
 
-            var inDom = $.contains(document.documentElement, this.$element[0])
+            var inDom = $.contains(this.$element[0].ownerDocument.documentElement, this.$element[0])
             if (e.isDefaultPrevented() || !inDom) return
             var that = this
 
             var $tip = this.tip()
 
             var tipId = this.getUID(this.type)
 
@@ -1313,49 +1681,52 @@
                     top: 0,
                     left: 0,
                     display: 'block'
                 })
                 .addClass(placement)
                 .data('bs.' + this.type, this)
 
-            this.options.container ? $tip.appendTo(this.options.container) : $tip.insertAfter(this.$element)
+            this.options.container ? $tip.appendTo($(document).find(this.options.container)) : $tip.insertAfter(this.$element)
+            this.$element.trigger('inserted.bs.' + this.type)
 
             var pos = this.getPosition()
             var actualWidth = $tip[0].offsetWidth
             var actualHeight = $tip[0].offsetHeight
 
             if (autoPlace) {
                 var orgPlacement = placement
-                var $parent = this.$element.parent()
-                var parentDim = this.getPosition($parent)
+                var viewportDim = this.getPosition(this.$viewport)
 
-                placement = placement == 'bottom' && pos.top + pos.height + actualHeight - parentDim.scroll > parentDim.height ? 'top' :
-                    placement == 'top' && pos.top - parentDim.scroll - actualHeight < 0 ? 'bottom' :
-                    placement == 'right' && pos.right + actualWidth > parentDim.width ? 'left' :
-                    placement == 'left' && pos.left - actualWidth < parentDim.left ? 'right' :
+                placement = placement == 'bottom' && pos.bottom + actualHeight > viewportDim.bottom ? 'top' :
+                    placement == 'top' && pos.top - actualHeight < viewportDim.top ? 'bottom' :
+                    placement == 'right' && pos.right + actualWidth > viewportDim.width ? 'left' :
+                    placement == 'left' && pos.left - actualWidth < viewportDim.left ? 'right' :
                     placement
 
                 $tip
                     .removeClass(orgPlacement)
                     .addClass(placement)
             }
 
             var calculatedOffset = this.getCalculatedOffset(placement, pos, actualWidth, actualHeight)
 
             this.applyPlacement(calculatedOffset, placement)
 
             var complete = function() {
+                var prevHoverState = that.hoverState
                 that.$element.trigger('shown.bs.' + that.type)
                 that.hoverState = null
+
+                if (prevHoverState == 'out') that.leave(that)
             }
 
             $.support.transition && this.$tip.hasClass('fade') ?
                 $tip
                 .one('bsTransitionEnd', complete)
-                .emulateTransitionEnd(150) :
+                .emulateTransitionEnd(Tooltip.TRANSITION_DURATION) :
                 complete()
         }
     }
 
     Tooltip.prototype.applyPlacement = function(offset, placement) {
         var $tip = this.tip()
         var width = $tip[0].offsetWidth
@@ -1365,16 +1736,16 @@
         var marginTop = parseInt($tip.css('margin-top'), 10)
         var marginLeft = parseInt($tip.css('margin-left'), 10)
 
         // we must check for NaN for ie 8/9
         if (isNaN(marginTop)) marginTop = 0
         if (isNaN(marginLeft)) marginLeft = 0
 
-        offset.top = offset.top + marginTop
-        offset.left = offset.left + marginLeft
+        offset.top += marginTop
+        offset.left += marginLeft
 
         // $.fn.offset doesn't round pixel values
         // so we use setOffset directly with our own function B-0
         $.offset.setOffset($tip[0], $.extend({
             using: function(props) {
                 $tip.css({
                     top: Math.round(props.top),
@@ -1394,86 +1765,118 @@
         }
 
         var delta = this.getViewportAdjustedDelta(placement, offset, actualWidth, actualHeight)
 
         if (delta.left) offset.left += delta.left
         else offset.top += delta.top
 
-        var arrowDelta = delta.left ? delta.left * 2 - width + actualWidth : delta.top * 2 - height + actualHeight
-        var arrowPosition = delta.left ? 'left' : 'top'
-        var arrowOffsetPosition = delta.left ? 'offsetWidth' : 'offsetHeight'
+        var isVertical = /top|bottom/.test(placement)
+        var arrowDelta = isVertical ? delta.left * 2 - width + actualWidth : delta.top * 2 - height + actualHeight
+        var arrowOffsetPosition = isVertical ? 'offsetWidth' : 'offsetHeight'
 
         $tip.offset(offset)
-        this.replaceArrow(arrowDelta, $tip[0][arrowOffsetPosition], arrowPosition)
+        this.replaceArrow(arrowDelta, $tip[0][arrowOffsetPosition], isVertical)
     }
 
-    Tooltip.prototype.replaceArrow = function(delta, dimension, position) {
-        this.arrow().css(position, delta ? (50 * (1 - delta / dimension) + '%') : '')
+    Tooltip.prototype.replaceArrow = function(delta, dimension, isVertical) {
+        this.arrow()
+            .css(isVertical ? 'left' : 'top', 50 * (1 - delta / dimension) + '%')
+            .css(isVertical ? 'top' : 'left', '')
     }
 
     Tooltip.prototype.setContent = function() {
         var $tip = this.tip()
         var title = this.getTitle()
 
-        $tip.find('.tooltip-inner')[this.options.html ? 'html' : 'text'](title)
+        if (this.options.html) {
+            if (this.options.sanitize) {
+                title = sanitizeHtml(title, this.options.whiteList, this.options.sanitizeFn)
+            }
+
+            $tip.find('.tooltip-inner').html(title)
+        } else {
+            $tip.find('.tooltip-inner').text(title)
+        }
+
         $tip.removeClass('fade in top bottom left right')
     }
 
-    Tooltip.prototype.hide = function() {
+    Tooltip.prototype.hide = function(callback) {
         var that = this
-        var $tip = this.tip()
+        var $tip = $(this.$tip)
         var e = $.Event('hide.bs.' + this.type)
 
-        this.$element.removeAttr('aria-describedby')
-
         function complete() {
             if (that.hoverState != 'in') $tip.detach()
-            that.$element.trigger('hidden.bs.' + that.type)
+            if (that.$element) { // TODO: Check whether guarding this code with this `if` is really necessary.
+                that.$element
+                    .removeAttr('aria-describedby')
+                    .trigger('hidden.bs.' + that.type)
+            }
+            callback && callback()
         }
 
         this.$element.trigger(e)
 
         if (e.isDefaultPrevented()) return
 
         $tip.removeClass('in')
 
-        $.support.transition && this.$tip.hasClass('fade') ?
+        $.support.transition && $tip.hasClass('fade') ?
             $tip
             .one('bsTransitionEnd', complete)
-            .emulateTransitionEnd(150) :
+            .emulateTransitionEnd(Tooltip.TRANSITION_DURATION) :
             complete()
 
         this.hoverState = null
 
         return this
     }
 
     Tooltip.prototype.fixTitle = function() {
         var $e = this.$element
-        if ($e.attr('title') || typeof($e.attr('data-original-title')) != 'string') {
+        if ($e.attr('title') || typeof $e.attr('data-original-title') != 'string') {
             $e.attr('data-original-title', $e.attr('title') || '').attr('title', '')
         }
     }
 
     Tooltip.prototype.hasContent = function() {
         return this.getTitle()
     }
 
     Tooltip.prototype.getPosition = function($element) {
         $element = $element || this.$element
+
         var el = $element[0]
         var isBody = el.tagName == 'BODY'
-        return $.extend({}, (typeof el.getBoundingClientRect == 'function') ? el.getBoundingClientRect() : null, {
-            scroll: isBody ? document.documentElement.scrollTop || document.body.scrollTop : $element.scrollTop(),
-            width: isBody ? $(window).width() : $element.outerWidth(),
-            height: isBody ? $(window).height() : $element.outerHeight()
-        }, isBody ? {
+
+        var elRect = el.getBoundingClientRect()
+        if (elRect.width == null) {
+            // width and height are missing in IE8, so compute them manually; see https://github.com/twbs/bootstrap/issues/14093
+            elRect = $.extend({}, elRect, {
+                width: elRect.right - elRect.left,
+                height: elRect.bottom - elRect.top
+            })
+        }
+        var isSvg = window.SVGElement && el instanceof window.SVGElement
+        // Avoid using $.offset() on SVGs since it gives incorrect results in jQuery 3.
+        // See https://github.com/twbs/bootstrap/issues/20280
+        var elOffset = isBody ? {
             top: 0,
             left: 0
-        } : $element.offset())
+        } : (isSvg ? null : $element.offset())
+        var scroll = {
+            scroll: isBody ? document.documentElement.scrollTop || document.body.scrollTop : $element.scrollTop()
+        }
+        var outerDims = isBody ? {
+            width: $(window).width(),
+            height: $(window).height()
+        } : null
+
+        return $.extend({}, elRect, scroll, outerDims, elOffset)
     }
 
     Tooltip.prototype.getCalculatedOffset = function(placement, pos, actualWidth, actualHeight) {
         return placement == 'bottom' ? {
                 top: pos.top + pos.height,
                 left: pos.left + pos.width / 2 - actualWidth / 2
             } :
@@ -1512,15 +1915,15 @@
                 delta.top = viewportDimensions.top + viewportDimensions.height - bottomEdgeOffset
             }
         } else {
             var leftEdgeOffset = pos.left - viewportPadding
             var rightEdgeOffset = pos.left + viewportPadding + actualWidth
             if (leftEdgeOffset < viewportDimensions.left) { // left overflow
                 delta.left = viewportDimensions.left - leftEdgeOffset
-            } else if (rightEdgeOffset > viewportDimensions.width) { // right overflow
+            } else if (rightEdgeOffset > viewportDimensions.right) { // right overflow
                 delta.left = viewportDimensions.left + viewportDimensions.width - rightEdgeOffset
             }
         }
 
         return delta
     }
 
@@ -1538,29 +1941,27 @@
     Tooltip.prototype.getUID = function(prefix) {
         do prefix += ~~(Math.random() * 1000000)
         while (document.getElementById(prefix))
         return prefix
     }
 
     Tooltip.prototype.tip = function() {
-        return (this.$tip = this.$tip || $(this.options.template))
+        if (!this.$tip) {
+            this.$tip = $(this.options.template)
+            if (this.$tip.length != 1) {
+                throw new Error(this.type + ' `template` option must consist of exactly 1 top-level element!')
+            }
+        }
+        return this.$tip
     }
 
     Tooltip.prototype.arrow = function() {
         return (this.$arrow = this.$arrow || this.tip().find('.tooltip-arrow'))
     }
 
-    Tooltip.prototype.validate = function() {
-        if (!this.$element[0].parentNode) {
-            this.hide()
-            this.$element = null
-            this.options = null
-        }
-    }
-
     Tooltip.prototype.enable = function() {
         this.enabled = true
     }
 
     Tooltip.prototype.disable = function() {
         this.enabled = false
     }
@@ -1575,33 +1976,52 @@
             self = $(e.currentTarget).data('bs.' + this.type)
             if (!self) {
                 self = new this.constructor(e.currentTarget, this.getDelegateOptions())
                 $(e.currentTarget).data('bs.' + this.type, self)
             }
         }
 
-        self.tip().hasClass('in') ? self.leave(self) : self.enter(self)
+        if (e) {
+            self.inState.click = !self.inState.click
+            if (self.isInStateTrue()) self.enter(self)
+            else self.leave(self)
+        } else {
+            self.tip().hasClass('in') ? self.leave(self) : self.enter(self)
+        }
     }
 
     Tooltip.prototype.destroy = function() {
+        var that = this
         clearTimeout(this.timeout)
-        this.hide().$element.off('.' + this.type).removeData('bs.' + this.type)
+        this.hide(function() {
+            that.$element.off('.' + that.type).removeData('bs.' + that.type)
+            if (that.$tip) {
+                that.$tip.detach()
+            }
+            that.$tip = null
+            that.$arrow = null
+            that.$viewport = null
+            that.$element = null
+        })
     }
 
+    Tooltip.prototype.sanitizeHtml = function(unsafeHtml) {
+        return sanitizeHtml(unsafeHtml, this.options.whiteList, this.options.sanitizeFn)
+    }
 
     // TOOLTIP PLUGIN DEFINITION
     // =========================
 
     function Plugin(option) {
         return this.each(function() {
             var $this = $(this)
             var data = $this.data('bs.tooltip')
             var options = typeof option == 'object' && option
 
-            if (!data && option == 'destroy') return
+            if (!data && /destroy|hide/.test(option)) return
             if (!data) $this.data('bs.tooltip', (data = new Tooltip(this, options)))
             if (typeof option == 'string') data[option]()
         })
     }
 
     var old = $.fn.tooltip
 
@@ -1616,18 +2036,18 @@
         $.fn.tooltip = old
         return this
     }
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: popover.js v3.2.0
- * http://getbootstrap.com/javascript/#popovers
+ * Bootstrap: popover.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#popovers
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
@@ -1637,15 +2057,15 @@
 
     var Popover = function(element, options) {
         this.init('popover', element, options)
     }
 
     if (!$.fn.tooltip) throw new Error('Popover requires tooltip.js')
 
-    Popover.VERSION = '3.2.0'
+    Popover.VERSION = '3.4.1'
 
     Popover.DEFAULTS = $.extend({}, $.fn.tooltip.Constructor.DEFAULTS, {
         placement: 'right',
         trigger: 'click',
         content: '',
         template: '<div class="popover" role="tooltip"><div class="arrow"></div><h3 class="popover-title"></h3><div class="popover-content"></div></div>'
     })
@@ -1663,18 +2083,33 @@
     }
 
     Popover.prototype.setContent = function() {
         var $tip = this.tip()
         var title = this.getTitle()
         var content = this.getContent()
 
-        $tip.find('.popover-title')[this.options.html ? 'html' : 'text'](title)
-        $tip.find('.popover-content').empty()[ // we use append for html objects to maintain js events
-            this.options.html ? (typeof content == 'string' ? 'html' : 'append') : 'text'
-        ](content)
+        if (this.options.html) {
+            var typeContent = typeof content
+
+            if (this.options.sanitize) {
+                title = this.sanitizeHtml(title)
+
+                if (typeContent === 'string') {
+                    content = this.sanitizeHtml(content)
+                }
+            }
+
+            $tip.find('.popover-title').html(title)
+            $tip.find('.popover-content').children().detach().end()[
+                typeContent === 'string' ? 'html' : 'append'
+            ](content)
+        } else {
+            $tip.find('.popover-title').text(title)
+            $tip.find('.popover-content').children().detach().end().text(content)
+        }
 
         $tip.removeClass('fade top bottom left right in')
 
         // IE8 doesn't accept hiding via the `:empty` pseudo selector, we have to do
         // this manually by checking the contents.
         if (!$tip.find('.popover-title').html()) $tip.find('.popover-title').hide()
     }
@@ -1693,30 +2128,25 @@
                 o.content)
     }
 
     Popover.prototype.arrow = function() {
         return (this.$arrow = this.$arrow || this.tip().find('.arrow'))
     }
 
-    Popover.prototype.tip = function() {
-        if (!this.$tip) this.$tip = $(this.options.template)
-        return this.$tip
-    }
-
 
     // POPOVER PLUGIN DEFINITION
     // =========================
 
     function Plugin(option) {
         return this.each(function() {
             var $this = $(this)
             var data = $this.data('bs.popover')
             var options = typeof option == 'object' && option
 
-            if (!data && option == 'destroy') return
+            if (!data && /destroy|hide/.test(option)) return
             if (!data) $this.data('bs.popover', (data = new Popover(this, options)))
             if (typeof option == 'string') data[option]()
         })
     }
 
     var old = $.fn.popover
 
@@ -1731,70 +2161,67 @@
         $.fn.popover = old
         return this
     }
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: scrollspy.js v3.2.0
- * http://getbootstrap.com/javascript/#scrollspy
+ * Bootstrap: scrollspy.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#scrollspy
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
 
     // SCROLLSPY CLASS DEFINITION
     // ==========================
 
     function ScrollSpy(element, options) {
-        var process = $.proxy(this.process, this)
-
-        this.$body = $('body')
-        this.$scrollElement = $(element).is('body') ? $(window) : $(element)
+        this.$body = $(document.body)
+        this.$scrollElement = $(element).is(document.body) ? $(window) : $(element)
         this.options = $.extend({}, ScrollSpy.DEFAULTS, options)
         this.selector = (this.options.target || '') + ' .nav li > a'
         this.offsets = []
         this.targets = []
         this.activeTarget = null
         this.scrollHeight = 0
 
-        this.$scrollElement.on('scroll.bs.scrollspy', process)
+        this.$scrollElement.on('scroll.bs.scrollspy', $.proxy(this.process, this))
         this.refresh()
         this.process()
     }
 
-    ScrollSpy.VERSION = '3.2.0'
+    ScrollSpy.VERSION = '3.4.1'
 
     ScrollSpy.DEFAULTS = {
         offset: 10
     }
 
     ScrollSpy.prototype.getScrollHeight = function() {
         return this.$scrollElement[0].scrollHeight || Math.max(this.$body[0].scrollHeight, document.documentElement.scrollHeight)
     }
 
     ScrollSpy.prototype.refresh = function() {
+        var that = this
         var offsetMethod = 'offset'
         var offsetBase = 0
 
-        if (!$.isWindow(this.$scrollElement[0])) {
-            offsetMethod = 'position'
-            offsetBase = this.$scrollElement.scrollTop()
-        }
-
         this.offsets = []
         this.targets = []
         this.scrollHeight = this.getScrollHeight()
 
-        var self = this
+        if (!$.isWindow(this.$scrollElement[0])) {
+            offsetMethod = 'position'
+            offsetBase = this.$scrollElement.scrollTop()
+        }
 
         this.$body
             .find(this.selector)
             .map(function() {
                 var $el = $(this)
                 var href = $el.data('target') || $el.attr('href')
                 var $href = /^#./.test(href) && $(href)
@@ -1806,16 +2233,16 @@
                         [$href[offsetMethod]().top + offsetBase, href]
                     ]) || null
             })
             .sort(function(a, b) {
                 return a[0] - b[0]
             })
             .each(function() {
-                self.offsets.push(this[0])
-                self.targets.push(this[1])
+                that.offsets.push(this[0])
+                that.targets.push(this[1])
             })
     }
 
     ScrollSpy.prototype.process = function() {
         var scrollTop = this.$scrollElement.scrollTop() + this.options.offset
         var scrollHeight = this.getScrollHeight()
         var maxScroll = this.options.offset + scrollHeight - this.$scrollElement.height()
@@ -1828,32 +2255,31 @@
             this.refresh()
         }
 
         if (scrollTop >= maxScroll) {
             return activeTarget != (i = targets[targets.length - 1]) && this.activate(i)
         }
 
-        if (activeTarget && scrollTop <= offsets[0]) {
-            return activeTarget != (i = targets[0]) && this.activate(i)
+        if (activeTarget && scrollTop < offsets[0]) {
+            this.activeTarget = null
+            return this.clear()
         }
 
         for (i = offsets.length; i--;) {
             activeTarget != targets[i] &&
                 scrollTop >= offsets[i] &&
-                (!offsets[i + 1] || scrollTop <= offsets[i + 1]) &&
+                (offsets[i + 1] === undefined || scrollTop < offsets[i + 1]) &&
                 this.activate(targets[i])
         }
     }
 
     ScrollSpy.prototype.activate = function(target) {
         this.activeTarget = target
 
-        $(this.selector)
-            .parentsUntil(this.options.target, '.active')
-            .removeClass('active')
+        this.clear()
 
         var selector = this.selector +
             '[data-target="' + target + '"],' +
             this.selector + '[href="' + target + '"]'
 
         var active = $(selector)
             .parents('li')
@@ -1864,14 +2290,20 @@
                 .closest('li.dropdown')
                 .addClass('active')
         }
 
         active.trigger('activate.bs.scrollspy')
     }
 
+    ScrollSpy.prototype.clear = function() {
+        $(this.selector)
+            .parentsUntil(this.options.target, '.active')
+            .removeClass('active')
+    }
+
 
     // SCROLLSPY PLUGIN DEFINITION
     // ===========================
 
     function Plugin(option) {
         return this.each(function() {
             var $this = $(this)
@@ -1907,99 +2339,122 @@
             Plugin.call($spy, $spy.data())
         })
     })
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: tab.js v3.2.0
- * http://getbootstrap.com/javascript/#tabs
+ * Bootstrap: tab.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#tabs
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
 
     // TAB CLASS DEFINITION
     // ====================
 
     var Tab = function(element) {
+        // jscs:disable requireDollarBeforejQueryAssignment
         this.element = $(element)
+        // jscs:enable requireDollarBeforejQueryAssignment
     }
 
-    Tab.VERSION = '3.2.0'
+    Tab.VERSION = '3.4.1'
+
+    Tab.TRANSITION_DURATION = 150
 
     Tab.prototype.show = function() {
         var $this = this.element
         var $ul = $this.closest('ul:not(.dropdown-menu)')
         var selector = $this.data('target')
 
         if (!selector) {
             selector = $this.attr('href')
             selector = selector && selector.replace(/.*(?=#[^\s]*$)/, '') // strip for ie7
         }
 
         if ($this.parent('li').hasClass('active')) return
 
-        var previous = $ul.find('.active:last a')[0]
-        var e = $.Event('show.bs.tab', {
-            relatedTarget: previous
+        var $previous = $ul.find('.active:last a')
+        var hideEvent = $.Event('hide.bs.tab', {
+            relatedTarget: $this[0]
+        })
+        var showEvent = $.Event('show.bs.tab', {
+            relatedTarget: $previous[0]
         })
 
-        $this.trigger(e)
+        $previous.trigger(hideEvent)
+        $this.trigger(showEvent)
 
-        if (e.isDefaultPrevented()) return
+        if (showEvent.isDefaultPrevented() || hideEvent.isDefaultPrevented()) return
 
-        var $target = $(selector)
+        var $target = $(document).find(selector)
 
         this.activate($this.closest('li'), $ul)
         this.activate($target, $target.parent(), function() {
+            $previous.trigger({
+                type: 'hidden.bs.tab',
+                relatedTarget: $this[0]
+            })
             $this.trigger({
                 type: 'shown.bs.tab',
-                relatedTarget: previous
+                relatedTarget: $previous[0]
             })
         })
     }
 
     Tab.prototype.activate = function(element, container, callback) {
         var $active = container.find('> .active')
         var transition = callback &&
             $.support.transition &&
-            $active.hasClass('fade')
+            ($active.length && $active.hasClass('fade') || !!container.find('> .fade').length)
 
         function next() {
             $active
                 .removeClass('active')
                 .find('> .dropdown-menu > .active')
                 .removeClass('active')
+                .end()
+                .find('[data-toggle="tab"]')
+                .attr('aria-expanded', false)
 
-            element.addClass('active')
+            element
+                .addClass('active')
+                .find('[data-toggle="tab"]')
+                .attr('aria-expanded', true)
 
             if (transition) {
                 element[0].offsetWidth // reflow for transition
                 element.addClass('in')
             } else {
                 element.removeClass('fade')
             }
 
-            if (element.parent('.dropdown-menu')) {
-                element.closest('li.dropdown').addClass('active')
+            if (element.parent('.dropdown-menu').length) {
+                element
+                    .closest('li.dropdown')
+                    .addClass('active')
+                    .end()
+                    .find('[data-toggle="tab"]')
+                    .attr('aria-expanded', true)
             }
 
             callback && callback()
         }
 
-        transition ?
+        $active.length && transition ?
             $active
             .one('bsTransitionEnd', next)
-            .emulateTransitionEnd(150) :
+            .emulateTransitionEnd(Tab.TRANSITION_DURATION) :
             next()
 
         $active.removeClass('in')
     }
 
 
     // TAB PLUGIN DEFINITION
@@ -2029,61 +2484,89 @@
         return this
     }
 
 
     // TAB DATA-API
     // ============
 
-    $(document).on('click.bs.tab.data-api', '[data-toggle="tab"], [data-toggle="pill"]', function(e) {
+    var clickHandler = function(e) {
         e.preventDefault()
         Plugin.call($(this), 'show')
-    })
+    }
+
+    $(document)
+        .on('click.bs.tab.data-api', '[data-toggle="tab"]', clickHandler)
+        .on('click.bs.tab.data-api', '[data-toggle="pill"]', clickHandler)
 
 }(jQuery);
 
 /* ========================================================================
- * Bootstrap: affix.js v3.2.0
- * http://getbootstrap.com/javascript/#affix
+ * Bootstrap: affix.js v3.4.1
+ * https://getbootstrap.com/docs/3.4/javascript/#affix
  * ========================================================================
- * Copyright 2011-2014 Twitter, Inc.
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
  * ======================================================================== */
 
 
 +
 function($) {
     'use strict';
 
     // AFFIX CLASS DEFINITION
     // ======================
 
     var Affix = function(element, options) {
         this.options = $.extend({}, Affix.DEFAULTS, options)
 
-        this.$target = $(this.options.target)
+        var target = this.options.target === Affix.DEFAULTS.target ? $(this.options.target) : $(document).find(this.options.target)
+
+        this.$target = target
             .on('scroll.bs.affix.data-api', $.proxy(this.checkPosition, this))
             .on('click.bs.affix.data-api', $.proxy(this.checkPositionWithEventLoop, this))
 
         this.$element = $(element)
-        this.affixed =
-            this.unpin =
-            this.pinnedOffset = null
+        this.affixed = null
+        this.unpin = null
+        this.pinnedOffset = null
 
         this.checkPosition()
     }
 
-    Affix.VERSION = '3.2.0'
+    Affix.VERSION = '3.4.1'
 
     Affix.RESET = 'affix affix-top affix-bottom'
 
     Affix.DEFAULTS = {
         offset: 0,
         target: window
     }
 
+    Affix.prototype.getState = function(scrollHeight, height, offsetTop, offsetBottom) {
+        var scrollTop = this.$target.scrollTop()
+        var position = this.$element.offset()
+        var targetHeight = this.$target.height()
+
+        if (offsetTop != null && this.affixed == 'top') return scrollTop < offsetTop ? 'top' : false
+
+        if (this.affixed == 'bottom') {
+            if (offsetTop != null) return (scrollTop + this.unpin <= position.top) ? false : 'bottom'
+            return (scrollTop + targetHeight <= scrollHeight - offsetBottom) ? false : 'bottom'
+        }
+
+        var initializing = this.affixed == null
+        var colliderTop = initializing ? scrollTop : position.top
+        var colliderHeight = initializing ? targetHeight : height
+
+        if (offsetTop != null && scrollTop <= offsetTop) return 'top'
+        if (offsetBottom != null && (colliderTop + colliderHeight >= scrollHeight - offsetBottom)) return 'bottom'
+
+        return false
+    }
+
     Affix.prototype.getPinnedOffset = function() {
         if (this.pinnedOffset) return this.pinnedOffset
         this.$element.removeClass(Affix.RESET).addClass('affix')
         var scrollTop = this.$target.scrollTop()
         var position = this.$element.offset()
         return (this.pinnedOffset = position.top - scrollTop)
     }
@@ -2091,50 +2574,48 @@
     Affix.prototype.checkPositionWithEventLoop = function() {
         setTimeout($.proxy(this.checkPosition, this), 1)
     }
 
     Affix.prototype.checkPosition = function() {
         if (!this.$element.is(':visible')) return
 
-        var scrollHeight = $(document).height()
-        var scrollTop = this.$target.scrollTop()
-        var position = this.$element.offset()
+        var height = this.$element.height()
         var offset = this.options.offset
         var offsetTop = offset.top
         var offsetBottom = offset.bottom
+        var scrollHeight = Math.max($(document).height(), $(document.body).height())
 
         if (typeof offset != 'object') offsetBottom = offsetTop = offset
         if (typeof offsetTop == 'function') offsetTop = offset.top(this.$element)
         if (typeof offsetBottom == 'function') offsetBottom = offset.bottom(this.$element)
 
-        var affix = this.unpin != null && (scrollTop + this.unpin <= position.top) ? false :
-            offsetBottom != null && (position.top + this.$element.height() >= scrollHeight - offsetBottom) ? 'bottom' :
-            offsetTop != null && (scrollTop <= offsetTop) ? 'top' : false
+        var affix = this.getState(scrollHeight, height, offsetTop, offsetBottom)
 
-        if (this.affixed === affix) return
-        if (this.unpin != null) this.$element.css('top', '')
+        if (this.affixed != affix) {
+            if (this.unpin != null) this.$element.css('top', '')
 
-        var affixType = 'affix' + (affix ? '-' + affix : '')
-        var e = $.Event(affixType + '.bs.affix')
+            var affixType = 'affix' + (affix ? '-' + affix : '')
+            var e = $.Event(affixType + '.bs.affix')
 
-        this.$element.trigger(e)
+            this.$element.trigger(e)
 
-        if (e.isDefaultPrevented()) return
+            if (e.isDefaultPrevented()) return
 
-        this.affixed = affix
-        this.unpin = affix == 'bottom' ? this.getPinnedOffset() : null
+            this.affixed = affix
+            this.unpin = affix == 'bottom' ? this.getPinnedOffset() : null
 
-        this.$element
-            .removeClass(Affix.RESET)
-            .addClass(affixType)
-            .trigger($.Event(affixType.replace('affix', 'affixed')))
+            this.$element
+                .removeClass(Affix.RESET)
+                .addClass(affixType)
+                .trigger(affixType.replace('affix', 'affixed') + '.bs.affix')
+        }
 
         if (affix == 'bottom') {
             this.$element.offset({
-                top: scrollHeight - this.$element.height() - offsetBottom
+                top: scrollHeight - height - offsetBottom
             })
         }
     }
 
 
     // AFFIX PLUGIN DEFINITION
     // =======================
@@ -2171,15 +2652,15 @@
     $(window).on('load', function() {
         $('[data-spy="affix"]').each(function() {
             var $spy = $(this)
             var data = $spy.data()
 
             data.offset = data.offset || {}
 
-            if (data.offsetBottom) data.offset.bottom = data.offsetBottom
-            if (data.offsetTop) data.offset.top = data.offsetTop
+            if (data.offsetBottom != null) data.offset.bottom = data.offsetBottom
+            if (data.offsetTop != null) data.offset.top = data.offsetTop
 
             Plugin.call($spy, data)
         })
     })
 
 }(jQuery);
```

### Comparing `yafowil.bootstrap-1.3.2/src/yafowil/bootstrap/resources/js/bootstrap.min.js` & `yafowil.bootstrap-2.0.0a1/src/yafowil/bootstrap/resources/bs3/js/bootstrap.min.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,863 +1,1043 @@
 /*!
- * Bootstrap v3.2.0 (http://getbootstrap.com)
- * Copyright 2011-2014 Twitter, Inc.
- * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
+ * Bootstrap v3.4.1 (https://getbootstrap.com/)
+ * Copyright 2011-2019 Twitter, Inc.
+ * Licensed under the MIT license
  */
-if ("undefined" == typeof jQuery) throw new Error("Bootstrap's JavaScript requires jQuery"); + function(a) {
+if ("undefined" == typeof jQuery) throw new Error("Bootstrap's JavaScript requires jQuery");
+! function(t) {
     "use strict";
-
-    function b() {
-        var a = document.createElement("bootstrap"),
-            b = {
-                WebkitTransition: "webkitTransitionEnd",
-                MozTransition: "transitionend",
-                OTransition: "oTransitionEnd otransitionend",
-                transition: "transitionend"
-            };
-        for (var c in b)
-            if (void 0 !== a.style[c]) return {
-                end: b[c]
-            };
-        return !1
-    }
-    a.fn.emulateTransitionEnd = function(b) {
-        var c = !1,
-            d = this;
-        a(this).one("bsTransitionEnd", function() {
-            c = !0
+    var e = jQuery.fn.jquery.split(" ")[0].split(".");
+    if (e[0] < 2 && e[1] < 9 || 1 == e[0] && 9 == e[1] && e[2] < 1 || 3 < e[0]) throw new Error("Bootstrap's JavaScript requires jQuery version 1.9.1 or higher, but lower than version 4")
+}(),
+function(n) {
+    "use strict";
+    n.fn.emulateTransitionEnd = function(t) {
+        var e = !1,
+            i = this;
+        n(this).one("bsTransitionEnd", function() {
+            e = !0
         });
-        var e = function() {
-            c || a(d).trigger(a.support.transition.end)
-        };
-        return setTimeout(e, b), this
-    }, a(function() {
-        a.support.transition = b(), a.support.transition && (a.event.special.bsTransitionEnd = {
-            bindType: a.support.transition.end,
-            delegateType: a.support.transition.end,
-            handle: function(b) {
-                return a(b.target).is(this) ? b.handleObj.handler.apply(this, arguments) : void 0
+        return setTimeout(function() {
+            e || n(i).trigger(n.support.transition.end)
+        }, t), this
+    }, n(function() {
+        n.support.transition = function o() {
+            var t = document.createElement("bootstrap"),
+                e = {
+                    WebkitTransition: "webkitTransitionEnd",
+                    MozTransition: "transitionend",
+                    OTransition: "oTransitionEnd otransitionend",
+                    transition: "transitionend"
+                };
+            for (var i in e)
+                if (t.style[i] !== undefined) return {
+                    end: e[i]
+                };
+            return !1
+        }(), n.support.transition && (n.event.special.bsTransitionEnd = {
+            bindType: n.support.transition.end,
+            delegateType: n.support.transition.end,
+            handle: function(t) {
+                if (n(t.target).is(this)) return t.handleObj.handler.apply(this, arguments)
             }
         })
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(s) {
     "use strict";
-
-    function b(b) {
-        return this.each(function() {
-            var c = a(this),
-                e = c.data("bs.alert");
-            e || c.data("bs.alert", e = new d(this)), "string" == typeof b && e[b].call(c)
-        })
-    }
-    var c = '[data-dismiss="alert"]',
-        d = function(b) {
-            a(b).on("click", c, this.close)
+    var e = '[data-dismiss="alert"]',
+        a = function(t) {
+            s(t).on("click", e, this.close)
         };
-    d.VERSION = "3.2.0", d.prototype.close = function(b) {
-        function c() {
-            f.detach().trigger("closed.bs.alert").remove()
+    a.VERSION = "3.4.1", a.TRANSITION_DURATION = 150, a.prototype.close = function(t) {
+        var e = s(this),
+            i = e.attr("data-target");
+        i || (i = (i = e.attr("href")) && i.replace(/.*(?=#[^\s]*$)/, "")), i = "#" === i ? [] : i;
+        var o = s(document).find(i);
+
+        function n() {
+            o.detach().trigger("closed.bs.alert").remove()
         }
-        var d = a(this),
-            e = d.attr("data-target");
-        e || (e = d.attr("href"), e = e && e.replace(/.*(?=#[^\s]*$)/, ""));
-        var f = a(e);
-        b && b.preventDefault(), f.length || (f = d.hasClass("alert") ? d : d.parent()), f.trigger(b = a.Event("close.bs.alert")), b.isDefaultPrevented() || (f.removeClass("in"), a.support.transition && f.hasClass("fade") ? f.one("bsTransitionEnd", c).emulateTransitionEnd(150) : c())
+        t && t.preventDefault(), o.length || (o = e.closest(".alert")), o.trigger(t = s.Event("close.bs.alert")), t.isDefaultPrevented() || (o.removeClass("in"), s.support.transition && o.hasClass("fade") ? o.one("bsTransitionEnd", n).emulateTransitionEnd(a.TRANSITION_DURATION) : n())
     };
-    var e = a.fn.alert;
-    a.fn.alert = b, a.fn.alert.Constructor = d, a.fn.alert.noConflict = function() {
-        return a.fn.alert = e, this
-    }, a(document).on("click.bs.alert.data-api", c, d.prototype.close)
-}(jQuery), + function(a) {
+    var t = s.fn.alert;
+    s.fn.alert = function o(i) {
+        return this.each(function() {
+            var t = s(this),
+                e = t.data("bs.alert");
+            e || t.data("bs.alert", e = new a(this)), "string" == typeof i && e[i].call(t)
+        })
+    }, s.fn.alert.Constructor = a, s.fn.alert.noConflict = function() {
+        return s.fn.alert = t, this
+    }, s(document).on("click.bs.alert.data-api", e, a.prototype.close)
+}(jQuery),
+function(s) {
     "use strict";
+    var n = function(t, e) {
+        this.$element = s(t), this.options = s.extend({}, n.DEFAULTS, e), this.isLoading = !1
+    };
 
-    function b(b) {
+    function i(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.button"),
-                f = "object" == typeof b && b;
-            e || d.data("bs.button", e = new c(this, f)), "toggle" == b ? e.toggle() : b && e.setState(b)
+            var t = s(this),
+                e = t.data("bs.button"),
+                i = "object" == typeof o && o;
+            e || t.data("bs.button", e = new n(this, i)), "toggle" == o ? e.toggle() : o && e.setState(o)
         })
     }
-    var c = function(b, d) {
-        this.$element = a(b), this.options = a.extend({}, c.DEFAULTS, d), this.isLoading = !1
-    };
-    c.VERSION = "3.2.0", c.DEFAULTS = {
+    n.VERSION = "3.4.1", n.DEFAULTS = {
         loadingText: "loading..."
-    }, c.prototype.setState = function(b) {
-        var c = "disabled",
-            d = this.$element,
-            e = d.is("input") ? "val" : "html",
-            f = d.data();
-        b += "Text", null == f.resetText && d.data("resetText", d[e]()), d[e](null == f[b] ? this.options[b] : f[b]), setTimeout(a.proxy(function() {
-            "loadingText" == b ? (this.isLoading = !0, d.addClass(c).attr(c, c)) : this.isLoading && (this.isLoading = !1, d.removeClass(c).removeAttr(c))
+    }, n.prototype.setState = function(t) {
+        var e = "disabled",
+            i = this.$element,
+            o = i.is("input") ? "val" : "html",
+            n = i.data();
+        t += "Text", null == n.resetText && i.data("resetText", i[o]()), setTimeout(s.proxy(function() {
+            i[o](null == n[t] ? this.options[t] : n[t]), "loadingText" == t ? (this.isLoading = !0, i.addClass(e).attr(e, e).prop(e, !0)) : this.isLoading && (this.isLoading = !1, i.removeClass(e).removeAttr(e).prop(e, !1))
         }, this), 0)
-    }, c.prototype.toggle = function() {
-        var a = !0,
-            b = this.$element.closest('[data-toggle="buttons"]');
-        if (b.length) {
-            var c = this.$element.find("input");
-            "radio" == c.prop("type") && (c.prop("checked") && this.$element.hasClass("active") ? a = !1 : b.find(".active").removeClass("active")), a && c.prop("checked", !this.$element.hasClass("active")).trigger("change")
-        }
-        a && this.$element.toggleClass("active")
-    };
-    var d = a.fn.button;
-    a.fn.button = b, a.fn.button.Constructor = c, a.fn.button.noConflict = function() {
-        return a.fn.button = d, this
-    }, a(document).on("click.bs.button.data-api", '[data-toggle^="button"]', function(c) {
-        var d = a(c.target);
-        d.hasClass("btn") || (d = d.closest(".btn")), b.call(d, "toggle"), c.preventDefault()
+    }, n.prototype.toggle = function() {
+        var t = !0,
+            e = this.$element.closest('[data-toggle="buttons"]');
+        if (e.length) {
+            var i = this.$element.find("input");
+            "radio" == i.prop("type") ? (i.prop("checked") && (t = !1), e.find(".active").removeClass("active"), this.$element.addClass("active")) : "checkbox" == i.prop("type") && (i.prop("checked") !== this.$element.hasClass("active") && (t = !1), this.$element.toggleClass("active")), i.prop("checked", this.$element.hasClass("active")), t && i.trigger("change")
+        } else this.$element.attr("aria-pressed", !this.$element.hasClass("active")), this.$element.toggleClass("active")
+    };
+    var t = s.fn.button;
+    s.fn.button = i, s.fn.button.Constructor = n, s.fn.button.noConflict = function() {
+        return s.fn.button = t, this
+    }, s(document).on("click.bs.button.data-api", '[data-toggle^="button"]', function(t) {
+        var e = s(t.target).closest(".btn");
+        i.call(e, "toggle"), s(t.target).is('input[type="radio"], input[type="checkbox"]') || (t.preventDefault(), e.is("input,button") ? e.trigger("focus") : e.find("input:visible,button:visible").first().trigger("focus"))
+    }).on("focus.bs.button.data-api blur.bs.button.data-api", '[data-toggle^="button"]', function(t) {
+        s(t.target).closest(".btn").toggleClass("focus", /^focus(in)?$/.test(t.type))
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(p) {
     "use strict";
+    var c = function(t, e) {
+        this.$element = p(t), this.$indicators = this.$element.find(".carousel-indicators"), this.options = e, this.paused = null, this.sliding = null, this.interval = null, this.$active = null, this.$items = null, this.options.keyboard && this.$element.on("keydown.bs.carousel", p.proxy(this.keydown, this)), "hover" == this.options.pause && !("ontouchstart" in document.documentElement) && this.$element.on("mouseenter.bs.carousel", p.proxy(this.pause, this)).on("mouseleave.bs.carousel", p.proxy(this.cycle, this))
+    };
 
-    function b(b) {
+    function r(n) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.carousel"),
-                f = a.extend({}, c.DEFAULTS, d.data(), "object" == typeof b && b),
-                g = "string" == typeof b ? b : f.slide;
-            e || d.data("bs.carousel", e = new c(this, f)), "number" == typeof b ? e.to(b) : g ? e[g]() : f.interval && e.pause().cycle()
+            var t = p(this),
+                e = t.data("bs.carousel"),
+                i = p.extend({}, c.DEFAULTS, t.data(), "object" == typeof n && n),
+                o = "string" == typeof n ? n : i.slide;
+            e || t.data("bs.carousel", e = new c(this, i)), "number" == typeof n ? e.to(n) : o ? e[o]() : i.interval && e.pause().cycle()
         })
     }
-    var c = function(b, c) {
-        this.$element = a(b).on("keydown.bs.carousel", a.proxy(this.keydown, this)), this.$indicators = this.$element.find(".carousel-indicators"), this.options = c, this.paused = this.sliding = this.interval = this.$active = this.$items = null, "hover" == this.options.pause && this.$element.on("mouseenter.bs.carousel", a.proxy(this.pause, this)).on("mouseleave.bs.carousel", a.proxy(this.cycle, this))
-    };
-    c.VERSION = "3.2.0", c.DEFAULTS = {
+    c.VERSION = "3.4.1", c.TRANSITION_DURATION = 600, c.DEFAULTS = {
         interval: 5e3,
         pause: "hover",
-        wrap: !0
-    }, c.prototype.keydown = function(a) {
-        switch (a.which) {
-            case 37:
-                this.prev();
-                break;
-            case 39:
-                this.next();
-                break;
-            default:
-                return
-        }
-        a.preventDefault()
-    }, c.prototype.cycle = function(b) {
-        return b || (this.paused = !1), this.interval && clearInterval(this.interval), this.options.interval && !this.paused && (this.interval = setInterval(a.proxy(this.next, this), this.options.interval)), this
-    }, c.prototype.getItemIndex = function(a) {
-        return this.$items = a.parent().children(".item"), this.$items.index(a || this.$active)
-    }, c.prototype.to = function(b) {
-        var c = this,
-            d = this.getItemIndex(this.$active = this.$element.find(".item.active"));
-        return b > this.$items.length - 1 || 0 > b ? void 0 : this.sliding ? this.$element.one("slid.bs.carousel", function() {
-            c.to(b)
-        }) : d == b ? this.pause().cycle() : this.slide(b > d ? "next" : "prev", a(this.$items[b]))
-    }, c.prototype.pause = function(b) {
-        return b || (this.paused = !0), this.$element.find(".next, .prev").length && a.support.transition && (this.$element.trigger(a.support.transition.end), this.cycle(!0)), this.interval = clearInterval(this.interval), this
+        wrap: !0,
+        keyboard: !0
+    }, c.prototype.keydown = function(t) {
+        if (!/input|textarea/i.test(t.target.tagName)) {
+            switch (t.which) {
+                case 37:
+                    this.prev();
+                    break;
+                case 39:
+                    this.next();
+                    break;
+                default:
+                    return
+            }
+            t.preventDefault()
+        }
+    }, c.prototype.cycle = function(t) {
+        return t || (this.paused = !1), this.interval && clearInterval(this.interval), this.options.interval && !this.paused && (this.interval = setInterval(p.proxy(this.next, this), this.options.interval)), this
+    }, c.prototype.getItemIndex = function(t) {
+        return this.$items = t.parent().children(".item"), this.$items.index(t || this.$active)
+    }, c.prototype.getItemForDirection = function(t, e) {
+        var i = this.getItemIndex(e);
+        if (("prev" == t && 0 === i || "next" == t && i == this.$items.length - 1) && !this.options.wrap) return e;
+        var o = (i + ("prev" == t ? -1 : 1)) % this.$items.length;
+        return this.$items.eq(o)
+    }, c.prototype.to = function(t) {
+        var e = this,
+            i = this.getItemIndex(this.$active = this.$element.find(".item.active"));
+        if (!(t > this.$items.length - 1 || t < 0)) return this.sliding ? this.$element.one("slid.bs.carousel", function() {
+            e.to(t)
+        }) : i == t ? this.pause().cycle() : this.slide(i < t ? "next" : "prev", this.$items.eq(t))
+    }, c.prototype.pause = function(t) {
+        return t || (this.paused = !0), this.$element.find(".next, .prev").length && p.support.transition && (this.$element.trigger(p.support.transition.end), this.cycle(!0)), this.interval = clearInterval(this.interval), this
     }, c.prototype.next = function() {
-        return this.sliding ? void 0 : this.slide("next")
+        if (!this.sliding) return this.slide("next")
     }, c.prototype.prev = function() {
-        return this.sliding ? void 0 : this.slide("prev")
-    }, c.prototype.slide = function(b, c) {
-        var d = this.$element.find(".item.active"),
-            e = c || d[b](),
-            f = this.interval,
-            g = "next" == b ? "left" : "right",
-            h = "next" == b ? "first" : "last",
-            i = this;
-        if (!e.length) {
-            if (!this.options.wrap) return;
-            e = this.$element.find(".item")[h]()
-        }
-        if (e.hasClass("active")) return this.sliding = !1;
-        var j = e[0],
-            k = a.Event("slide.bs.carousel", {
-                relatedTarget: j,
-                direction: g
+        if (!this.sliding) return this.slide("prev")
+    }, c.prototype.slide = function(t, e) {
+        var i = this.$element.find(".item.active"),
+            o = e || this.getItemForDirection(t, i),
+            n = this.interval,
+            s = "next" == t ? "left" : "right",
+            a = this;
+        if (o.hasClass("active")) return this.sliding = !1;
+        var r = o[0],
+            l = p.Event("slide.bs.carousel", {
+                relatedTarget: r,
+                direction: s
             });
-        if (this.$element.trigger(k), !k.isDefaultPrevented()) {
-            if (this.sliding = !0, f && this.pause(), this.$indicators.length) {
+        if (this.$element.trigger(l), !l.isDefaultPrevented()) {
+            if (this.sliding = !0, n && this.pause(), this.$indicators.length) {
                 this.$indicators.find(".active").removeClass("active");
-                var l = a(this.$indicators.children()[this.getItemIndex(e)]);
-                l && l.addClass("active")
+                var h = p(this.$indicators.children()[this.getItemIndex(o)]);
+                h && h.addClass("active")
             }
-            var m = a.Event("slid.bs.carousel", {
-                relatedTarget: j,
-                direction: g
+            var d = p.Event("slid.bs.carousel", {
+                relatedTarget: r,
+                direction: s
             });
-            return a.support.transition && this.$element.hasClass("slide") ? (e.addClass(b), e[0].offsetWidth, d.addClass(g), e.addClass(g), d.one("bsTransitionEnd", function() {
-                e.removeClass([b, g].join(" ")).addClass("active"), d.removeClass(["active", g].join(" ")), i.sliding = !1, setTimeout(function() {
-                    i.$element.trigger(m)
+            return p.support.transition && this.$element.hasClass("slide") ? (o.addClass(t), "object" == typeof o && o.length && o[0].offsetWidth, i.addClass(s), o.addClass(s), i.one("bsTransitionEnd", function() {
+                o.removeClass([t, s].join(" ")).addClass("active"), i.removeClass(["active", s].join(" ")), a.sliding = !1, setTimeout(function() {
+                    a.$element.trigger(d)
                 }, 0)
-            }).emulateTransitionEnd(1e3 * d.css("transition-duration").slice(0, -1))) : (d.removeClass("active"), e.addClass("active"), this.sliding = !1, this.$element.trigger(m)), f && this.cycle(), this
+            }).emulateTransitionEnd(c.TRANSITION_DURATION)) : (i.removeClass("active"), o.addClass("active"), this.sliding = !1, this.$element.trigger(d)), n && this.cycle(), this
+        }
+    };
+    var t = p.fn.carousel;
+    p.fn.carousel = r, p.fn.carousel.Constructor = c, p.fn.carousel.noConflict = function() {
+        return p.fn.carousel = t, this
+    };
+    var e = function(t) {
+        var e = p(this),
+            i = e.attr("href");
+        i && (i = i.replace(/.*(?=#[^\s]+$)/, ""));
+        var o = e.attr("data-target") || i,
+            n = p(document).find(o);
+        if (n.hasClass("carousel")) {
+            var s = p.extend({}, n.data(), e.data()),
+                a = e.attr("data-slide-to");
+            a && (s.interval = !1), r.call(n, s), a && n.data("bs.carousel").to(a), t.preventDefault()
         }
     };
-    var d = a.fn.carousel;
-    a.fn.carousel = b, a.fn.carousel.Constructor = c, a.fn.carousel.noConflict = function() {
-        return a.fn.carousel = d, this
-    }, a(document).on("click.bs.carousel.data-api", "[data-slide], [data-slide-to]", function(c) {
-        var d, e = a(this),
-            f = a(e.attr("data-target") || (d = e.attr("href")) && d.replace(/.*(?=#[^\s]+$)/, ""));
-        if (f.hasClass("carousel")) {
-            var g = a.extend({}, f.data(), e.data()),
-                h = e.attr("data-slide-to");
-            h && (g.interval = !1), b.call(f, g), h && f.data("bs.carousel").to(h), c.preventDefault()
-        }
-    }), a(window).on("load", function() {
-        a('[data-ride="carousel"]').each(function() {
-            var c = a(this);
-            b.call(c, c.data())
+    p(document).on("click.bs.carousel.data-api", "[data-slide]", e).on("click.bs.carousel.data-api", "[data-slide-to]", e), p(window).on("load", function() {
+        p('[data-ride="carousel"]').each(function() {
+            var t = p(this);
+            r.call(t, t.data())
         })
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(a) {
     "use strict";
+    var r = function(t, e) {
+        this.$element = a(t), this.options = a.extend({}, r.DEFAULTS, e), this.$trigger = a('[data-toggle="collapse"][href="#' + t.id + '"],[data-toggle="collapse"][data-target="#' + t.id + '"]'), this.transitioning = null, this.options.parent ? this.$parent = this.getParent() : this.addAriaAndCollapsedClass(this.$element, this.$trigger), this.options.toggle && this.toggle()
+    };
 
-    function b(b) {
+    function n(t) {
+        var e, i = t.attr("data-target") || (e = t.attr("href")) && e.replace(/.*(?=#[^\s]+$)/, "");
+        return a(document).find(i)
+    }
+
+    function l(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.collapse"),
-                f = a.extend({}, c.DEFAULTS, d.data(), "object" == typeof b && b);
-            !e && f.toggle && "show" == b && (b = !b), e || d.data("bs.collapse", e = new c(this, f)), "string" == typeof b && e[b]()
+            var t = a(this),
+                e = t.data("bs.collapse"),
+                i = a.extend({}, r.DEFAULTS, t.data(), "object" == typeof o && o);
+            !e && i.toggle && /show|hide/.test(o) && (i.toggle = !1), e || t.data("bs.collapse", e = new r(this, i)), "string" == typeof o && e[o]()
         })
     }
-    var c = function(b, d) {
-        this.$element = a(b), this.options = a.extend({}, c.DEFAULTS, d), this.transitioning = null, this.options.parent && (this.$parent = a(this.options.parent)), this.options.toggle && this.toggle()
-    };
-    c.VERSION = "3.2.0", c.DEFAULTS = {
+    r.VERSION = "3.4.1", r.TRANSITION_DURATION = 350, r.DEFAULTS = {
         toggle: !0
-    }, c.prototype.dimension = function() {
-        var a = this.$element.hasClass("width");
-        return a ? "width" : "height"
-    }, c.prototype.show = function() {
+    }, r.prototype.dimension = function() {
+        return this.$element.hasClass("width") ? "width" : "height"
+    }, r.prototype.show = function() {
         if (!this.transitioning && !this.$element.hasClass("in")) {
-            var c = a.Event("show.bs.collapse");
-            if (this.$element.trigger(c), !c.isDefaultPrevented()) {
-                var d = this.$parent && this.$parent.find("> .panel > .in");
-                if (d && d.length) {
-                    var e = d.data("bs.collapse");
-                    if (e && e.transitioning) return;
-                    b.call(d, "hide"), e || d.data("bs.collapse", null)
+            var t, e = this.$parent && this.$parent.children(".panel").children(".in, .collapsing");
+            if (!(e && e.length && (t = e.data("bs.collapse")) && t.transitioning)) {
+                var i = a.Event("show.bs.collapse");
+                if (this.$element.trigger(i), !i.isDefaultPrevented()) {
+                    e && e.length && (l.call(e, "hide"), t || e.data("bs.collapse", null));
+                    var o = this.dimension();
+                    this.$element.removeClass("collapse").addClass("collapsing")[o](0).attr("aria-expanded", !0), this.$trigger.removeClass("collapsed").attr("aria-expanded", !0), this.transitioning = 1;
+                    var n = function() {
+                        this.$element.removeClass("collapsing").addClass("collapse in")[o](""), this.transitioning = 0, this.$element.trigger("shown.bs.collapse")
+                    };
+                    if (!a.support.transition) return n.call(this);
+                    var s = a.camelCase(["scroll", o].join("-"));
+                    this.$element.one("bsTransitionEnd", a.proxy(n, this)).emulateTransitionEnd(r.TRANSITION_DURATION)[o](this.$element[0][s])
                 }
-                var f = this.dimension();
-                this.$element.removeClass("collapse").addClass("collapsing")[f](0), this.transitioning = 1;
-                var g = function() {
-                    this.$element.removeClass("collapsing").addClass("collapse in")[f](""), this.transitioning = 0, this.$element.trigger("shown.bs.collapse")
-                };
-                if (!a.support.transition) return g.call(this);
-                var h = a.camelCase(["scroll", f].join("-"));
-                this.$element.one("bsTransitionEnd", a.proxy(g, this)).emulateTransitionEnd(350)[f](this.$element[0][h])
             }
         }
-    }, c.prototype.hide = function() {
+    }, r.prototype.hide = function() {
         if (!this.transitioning && this.$element.hasClass("in")) {
-            var b = a.Event("hide.bs.collapse");
-            if (this.$element.trigger(b), !b.isDefaultPrevented()) {
-                var c = this.dimension();
-                this.$element[c](this.$element[c]())[0].offsetHeight, this.$element.addClass("collapsing").removeClass("collapse").removeClass("in"), this.transitioning = 1;
-                var d = function() {
-                    this.transitioning = 0, this.$element.trigger("hidden.bs.collapse").removeClass("collapsing").addClass("collapse")
+            var t = a.Event("hide.bs.collapse");
+            if (this.$element.trigger(t), !t.isDefaultPrevented()) {
+                var e = this.dimension();
+                this.$element[e](this.$element[e]())[0].offsetHeight, this.$element.addClass("collapsing").removeClass("collapse in").attr("aria-expanded", !1), this.$trigger.addClass("collapsed").attr("aria-expanded", !1), this.transitioning = 1;
+                var i = function() {
+                    this.transitioning = 0, this.$element.removeClass("collapsing").addClass("collapse").trigger("hidden.bs.collapse")
                 };
-                return a.support.transition ? void this.$element[c](0).one("bsTransitionEnd", a.proxy(d, this)).emulateTransitionEnd(350) : d.call(this)
+                if (!a.support.transition) return i.call(this);
+                this.$element[e](0).one("bsTransitionEnd", a.proxy(i, this)).emulateTransitionEnd(r.TRANSITION_DURATION)
             }
         }
-    }, c.prototype.toggle = function() {
+    }, r.prototype.toggle = function() {
         this[this.$element.hasClass("in") ? "hide" : "show"]()
+    }, r.prototype.getParent = function() {
+        return a(document).find(this.options.parent).find('[data-toggle="collapse"][data-parent="' + this.options.parent + '"]').each(a.proxy(function(t, e) {
+            var i = a(e);
+            this.addAriaAndCollapsedClass(n(i), i)
+        }, this)).end()
+    }, r.prototype.addAriaAndCollapsedClass = function(t, e) {
+        var i = t.hasClass("in");
+        t.attr("aria-expanded", i), e.toggleClass("collapsed", !i).attr("aria-expanded", i)
     };
-    var d = a.fn.collapse;
-    a.fn.collapse = b, a.fn.collapse.Constructor = c, a.fn.collapse.noConflict = function() {
-        return a.fn.collapse = d, this
-    }, a(document).on("click.bs.collapse.data-api", '[data-toggle="collapse"]', function(c) {
-        var d, e = a(this),
-            f = e.attr("data-target") || c.preventDefault() || (d = e.attr("href")) && d.replace(/.*(?=#[^\s]+$)/, ""),
-            g = a(f),
-            h = g.data("bs.collapse"),
-            i = h ? "toggle" : e.data(),
-            j = e.attr("data-parent"),
-            k = j && a(j);
-        h && h.transitioning || (k && k.find('[data-toggle="collapse"][data-parent="' + j + '"]').not(e).addClass("collapsed"), e[g.hasClass("in") ? "addClass" : "removeClass"]("collapsed")), b.call(g, i)
+    var t = a.fn.collapse;
+    a.fn.collapse = l, a.fn.collapse.Constructor = r, a.fn.collapse.noConflict = function() {
+        return a.fn.collapse = t, this
+    }, a(document).on("click.bs.collapse.data-api", '[data-toggle="collapse"]', function(t) {
+        var e = a(this);
+        e.attr("data-target") || t.preventDefault();
+        var i = n(e),
+            o = i.data("bs.collapse") ? "toggle" : e.data();
+        l.call(i, o)
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(a) {
     "use strict";
+    var r = '[data-toggle="dropdown"]',
+        o = function(t) {
+            a(t).on("click.bs.dropdown", this.toggle)
+        };
 
-    function b(b) {
-        b && 3 === b.which || (a(e).remove(), a(f).each(function() {
-            var d = c(a(this)),
-                e = {
+    function l(t) {
+        var e = t.attr("data-target");
+        e || (e = (e = t.attr("href")) && /#[A-Za-z]/.test(e) && e.replace(/.*(?=#[^\s]*$)/, ""));
+        var i = "#" !== e ? a(document).find(e) : null;
+        return i && i.length ? i : t.parent()
+    }
+
+    function s(o) {
+        o && 3 === o.which || (a(".dropdown-backdrop").remove(), a(r).each(function() {
+            var t = a(this),
+                e = l(t),
+                i = {
                     relatedTarget: this
                 };
-            d.hasClass("open") && (d.trigger(b = a.Event("hide.bs.dropdown", e)), b.isDefaultPrevented() || d.removeClass("open").trigger("hidden.bs.dropdown", e))
+            e.hasClass("open") && (o && "click" == o.type && /input|textarea/i.test(o.target.tagName) && a.contains(e[0], o.target) || (e.trigger(o = a.Event("hide.bs.dropdown", i)), o.isDefaultPrevented() || (t.attr("aria-expanded", "false"), e.removeClass("open").trigger(a.Event("hidden.bs.dropdown", i)))))
         }))
     }
-
-    function c(b) {
-        var c = b.attr("data-target");
-        c || (c = b.attr("href"), c = c && /#[A-Za-z]/.test(c) && c.replace(/.*(?=#[^\s]*$)/, ""));
-        var d = c && a(c);
-        return d && d.length ? d : b.parent()
-    }
-
-    function d(b) {
-        return this.each(function() {
-            var c = a(this),
-                d = c.data("bs.dropdown");
-            d || c.data("bs.dropdown", d = new g(this)), "string" == typeof b && d[b].call(c)
-        })
-    }
-    var e = ".dropdown-backdrop",
-        f = '[data-toggle="dropdown"]',
-        g = function(b) {
-            a(b).on("click.bs.dropdown", this.toggle)
-        };
-    g.VERSION = "3.2.0", g.prototype.toggle = function(d) {
+    o.VERSION = "3.4.1", o.prototype.toggle = function(t) {
         var e = a(this);
         if (!e.is(".disabled, :disabled")) {
-            var f = c(e),
-                g = f.hasClass("open");
-            if (b(), !g) {
-                "ontouchstart" in document.documentElement && !f.closest(".navbar-nav").length && a('<div class="dropdown-backdrop"/>').insertAfter(a(this)).on("click", b);
-                var h = {
+            var i = l(e),
+                o = i.hasClass("open");
+            if (s(), !o) {
+                "ontouchstart" in document.documentElement && !i.closest(".navbar-nav").length && a(document.createElement("div")).addClass("dropdown-backdrop").insertAfter(a(this)).on("click", s);
+                var n = {
                     relatedTarget: this
                 };
-                if (f.trigger(d = a.Event("show.bs.dropdown", h)), d.isDefaultPrevented()) return;
-                e.trigger("focus"), f.toggleClass("open").trigger("shown.bs.dropdown", h)
+                if (i.trigger(t = a.Event("show.bs.dropdown", n)), t.isDefaultPrevented()) return;
+                e.trigger("focus").attr("aria-expanded", "true"), i.toggleClass("open").trigger(a.Event("shown.bs.dropdown", n))
             }
             return !1
         }
-    }, g.prototype.keydown = function(b) {
-        if (/(38|40|27)/.test(b.keyCode)) {
-            var d = a(this);
-            if (b.preventDefault(), b.stopPropagation(), !d.is(".disabled, :disabled")) {
-                var e = c(d),
-                    g = e.hasClass("open");
-                if (!g || g && 27 == b.keyCode) return 27 == b.which && e.find(f).trigger("focus"), d.trigger("click");
-                var h = " li:not(.divider):visible a",
-                    i = e.find('[role="menu"]' + h + ', [role="listbox"]' + h);
-                if (i.length) {
-                    var j = i.index(i.filter(":focus"));
-                    38 == b.keyCode && j > 0 && j--, 40 == b.keyCode && j < i.length - 1 && j++, ~j || (j = 0), i.eq(j).trigger("focus")
+    }, o.prototype.keydown = function(t) {
+        if (/(38|40|27|32)/.test(t.which) && !/input|textarea/i.test(t.target.tagName)) {
+            var e = a(this);
+            if (t.preventDefault(), t.stopPropagation(), !e.is(".disabled, :disabled")) {
+                var i = l(e),
+                    o = i.hasClass("open");
+                if (!o && 27 != t.which || o && 27 == t.which) return 27 == t.which && i.find(r).trigger("focus"), e.trigger("click");
+                var n = i.find(".dropdown-menu li:not(.disabled):visible a");
+                if (n.length) {
+                    var s = n.index(t.target);
+                    38 == t.which && 0 < s && s--, 40 == t.which && s < n.length - 1 && s++, ~s || (s = 0), n.eq(s).trigger("focus")
                 }
             }
         }
     };
-    var h = a.fn.dropdown;
-    a.fn.dropdown = d, a.fn.dropdown.Constructor = g, a.fn.dropdown.noConflict = function() {
-        return a.fn.dropdown = h, this
-    }, a(document).on("click.bs.dropdown.data-api", b).on("click.bs.dropdown.data-api", ".dropdown form", function(a) {
-        a.stopPropagation()
-    }).on("click.bs.dropdown.data-api", f, g.prototype.toggle).on("keydown.bs.dropdown.data-api", f + ', [role="menu"], [role="listbox"]', g.prototype.keydown)
-}(jQuery), + function(a) {
-    "use strict";
-
-    function b(b, d) {
+    var t = a.fn.dropdown;
+    a.fn.dropdown = function e(i) {
         return this.each(function() {
-            var e = a(this),
-                f = e.data("bs.modal"),
-                g = a.extend({}, c.DEFAULTS, e.data(), "object" == typeof b && b);
-            f || e.data("bs.modal", f = new c(this, g)), "string" == typeof b ? f[b](d) : g.show && f.show(d)
+            var t = a(this),
+                e = t.data("bs.dropdown");
+            e || t.data("bs.dropdown", e = new o(this)), "string" == typeof i && e[i].call(t)
         })
-    }
-    var c = function(b, c) {
-        this.options = c, this.$body = a(document.body), this.$element = a(b), this.$backdrop = this.isShown = null, this.scrollbarWidth = 0, this.options.remote && this.$element.find(".modal-content").load(this.options.remote, a.proxy(function() {
+    }, a.fn.dropdown.Constructor = o, a.fn.dropdown.noConflict = function() {
+        return a.fn.dropdown = t, this
+    }, a(document).on("click.bs.dropdown.data-api", s).on("click.bs.dropdown.data-api", ".dropdown form", function(t) {
+        t.stopPropagation()
+    }).on("click.bs.dropdown.data-api", r, o.prototype.toggle).on("keydown.bs.dropdown.data-api", r, o.prototype.keydown).on("keydown.bs.dropdown.data-api", ".dropdown-menu", o.prototype.keydown)
+}(jQuery),
+function(a) {
+    "use strict";
+    var s = function(t, e) {
+        this.options = e, this.$body = a(document.body), this.$element = a(t), this.$dialog = this.$element.find(".modal-dialog"), this.$backdrop = null, this.isShown = null, this.originalBodyPad = null, this.scrollbarWidth = 0, this.ignoreBackdropClick = !1, this.fixedContent = ".navbar-fixed-top, .navbar-fixed-bottom", this.options.remote && this.$element.find(".modal-content").load(this.options.remote, a.proxy(function() {
             this.$element.trigger("loaded.bs.modal")
         }, this))
     };
-    c.VERSION = "3.2.0", c.DEFAULTS = {
+
+    function r(o, n) {
+        return this.each(function() {
+            var t = a(this),
+                e = t.data("bs.modal"),
+                i = a.extend({}, s.DEFAULTS, t.data(), "object" == typeof o && o);
+            e || t.data("bs.modal", e = new s(this, i)), "string" == typeof o ? e[o](n) : i.show && e.show(n)
+        })
+    }
+    s.VERSION = "3.4.1", s.TRANSITION_DURATION = 300, s.BACKDROP_TRANSITION_DURATION = 150, s.DEFAULTS = {
         backdrop: !0,
         keyboard: !0,
         show: !0
-    }, c.prototype.toggle = function(a) {
-        return this.isShown ? this.hide() : this.show(a)
-    }, c.prototype.show = function(b) {
-        var c = this,
-            d = a.Event("show.bs.modal", {
-                relatedTarget: b
+    }, s.prototype.toggle = function(t) {
+        return this.isShown ? this.hide() : this.show(t)
+    }, s.prototype.show = function(i) {
+        var o = this,
+            t = a.Event("show.bs.modal", {
+                relatedTarget: i
             });
-        this.$element.trigger(d), this.isShown || d.isDefaultPrevented() || (this.isShown = !0, this.checkScrollbar(), this.$body.addClass("modal-open"), this.setScrollbar(), this.escape(), this.$element.on("click.dismiss.bs.modal", '[data-dismiss="modal"]', a.proxy(this.hide, this)), this.backdrop(function() {
-            var d = a.support.transition && c.$element.hasClass("fade");
-            c.$element.parent().length || c.$element.appendTo(c.$body), c.$element.show().scrollTop(0), d && c.$element[0].offsetWidth, c.$element.addClass("in").attr("aria-hidden", !1), c.enforceFocus();
+        this.$element.trigger(t), this.isShown || t.isDefaultPrevented() || (this.isShown = !0, this.checkScrollbar(), this.setScrollbar(), this.$body.addClass("modal-open"), this.escape(), this.resize(), this.$element.on("click.dismiss.bs.modal", '[data-dismiss="modal"]', a.proxy(this.hide, this)), this.$dialog.on("mousedown.dismiss.bs.modal", function() {
+            o.$element.one("mouseup.dismiss.bs.modal", function(t) {
+                a(t.target).is(o.$element) && (o.ignoreBackdropClick = !0)
+            })
+        }), this.backdrop(function() {
+            var t = a.support.transition && o.$element.hasClass("fade");
+            o.$element.parent().length || o.$element.appendTo(o.$body), o.$element.show().scrollTop(0), o.adjustDialog(), t && o.$element[0].offsetWidth, o.$element.addClass("in"), o.enforceFocus();
             var e = a.Event("shown.bs.modal", {
-                relatedTarget: b
+                relatedTarget: i
             });
-            d ? c.$element.find(".modal-dialog").one("bsTransitionEnd", function() {
-                c.$element.trigger("focus").trigger(e)
-            }).emulateTransitionEnd(300) : c.$element.trigger("focus").trigger(e)
+            t ? o.$dialog.one("bsTransitionEnd", function() {
+                o.$element.trigger("focus").trigger(e)
+            }).emulateTransitionEnd(s.TRANSITION_DURATION) : o.$element.trigger("focus").trigger(e)
         }))
-    }, c.prototype.hide = function(b) {
-        b && b.preventDefault(), b = a.Event("hide.bs.modal"), this.$element.trigger(b), this.isShown && !b.isDefaultPrevented() && (this.isShown = !1, this.$body.removeClass("modal-open"), this.resetScrollbar(), this.escape(), a(document).off("focusin.bs.modal"), this.$element.removeClass("in").attr("aria-hidden", !0).off("click.dismiss.bs.modal"), a.support.transition && this.$element.hasClass("fade") ? this.$element.one("bsTransitionEnd", a.proxy(this.hideModal, this)).emulateTransitionEnd(300) : this.hideModal())
-    }, c.prototype.enforceFocus = function() {
-        a(document).off("focusin.bs.modal").on("focusin.bs.modal", a.proxy(function(a) {
-            this.$element[0] === a.target || this.$element.has(a.target).length || this.$element.trigger("focus")
+    }, s.prototype.hide = function(t) {
+        t && t.preventDefault(), t = a.Event("hide.bs.modal"), this.$element.trigger(t), this.isShown && !t.isDefaultPrevented() && (this.isShown = !1, this.escape(), this.resize(), a(document).off("focusin.bs.modal"), this.$element.removeClass("in").off("click.dismiss.bs.modal").off("mouseup.dismiss.bs.modal"), this.$dialog.off("mousedown.dismiss.bs.modal"), a.support.transition && this.$element.hasClass("fade") ? this.$element.one("bsTransitionEnd", a.proxy(this.hideModal, this)).emulateTransitionEnd(s.TRANSITION_DURATION) : this.hideModal())
+    }, s.prototype.enforceFocus = function() {
+        a(document).off("focusin.bs.modal").on("focusin.bs.modal", a.proxy(function(t) {
+            document === t.target || this.$element[0] === t.target || this.$element.has(t.target).length || this.$element.trigger("focus")
         }, this))
-    }, c.prototype.escape = function() {
-        this.isShown && this.options.keyboard ? this.$element.on("keyup.dismiss.bs.modal", a.proxy(function(a) {
-            27 == a.which && this.hide()
-        }, this)) : this.isShown || this.$element.off("keyup.dismiss.bs.modal")
-    }, c.prototype.hideModal = function() {
-        var a = this;
+    }, s.prototype.escape = function() {
+        this.isShown && this.options.keyboard ? this.$element.on("keydown.dismiss.bs.modal", a.proxy(function(t) {
+            27 == t.which && this.hide()
+        }, this)) : this.isShown || this.$element.off("keydown.dismiss.bs.modal")
+    }, s.prototype.resize = function() {
+        this.isShown ? a(window).on("resize.bs.modal", a.proxy(this.handleUpdate, this)) : a(window).off("resize.bs.modal")
+    }, s.prototype.hideModal = function() {
+        var t = this;
         this.$element.hide(), this.backdrop(function() {
-            a.$element.trigger("hidden.bs.modal")
+            t.$body.removeClass("modal-open"), t.resetAdjustments(), t.resetScrollbar(), t.$element.trigger("hidden.bs.modal")
         })
-    }, c.prototype.removeBackdrop = function() {
+    }, s.prototype.removeBackdrop = function() {
         this.$backdrop && this.$backdrop.remove(), this.$backdrop = null
-    }, c.prototype.backdrop = function(b) {
-        var c = this,
-            d = this.$element.hasClass("fade") ? "fade" : "";
+    }, s.prototype.backdrop = function(t) {
+        var e = this,
+            i = this.$element.hasClass("fade") ? "fade" : "";
         if (this.isShown && this.options.backdrop) {
-            var e = a.support.transition && d;
-            if (this.$backdrop = a('<div class="modal-backdrop ' + d + '" />').appendTo(this.$body), this.$element.on("click.dismiss.bs.modal", a.proxy(function(a) {
-                    a.target === a.currentTarget && ("static" == this.options.backdrop ? this.$element[0].focus.call(this.$element[0]) : this.hide.call(this))
-                }, this)), e && this.$backdrop[0].offsetWidth, this.$backdrop.addClass("in"), !b) return;
-            e ? this.$backdrop.one("bsTransitionEnd", b).emulateTransitionEnd(150) : b()
+            var o = a.support.transition && i;
+            if (this.$backdrop = a(document.createElement("div")).addClass("modal-backdrop " + i).appendTo(this.$body), this.$element.on("click.dismiss.bs.modal", a.proxy(function(t) {
+                    this.ignoreBackdropClick ? this.ignoreBackdropClick = !1 : t.target === t.currentTarget && ("static" == this.options.backdrop ? this.$element[0].focus() : this.hide())
+                }, this)), o && this.$backdrop[0].offsetWidth, this.$backdrop.addClass("in"), !t) return;
+            o ? this.$backdrop.one("bsTransitionEnd", t).emulateTransitionEnd(s.BACKDROP_TRANSITION_DURATION) : t()
         } else if (!this.isShown && this.$backdrop) {
             this.$backdrop.removeClass("in");
-            var f = function() {
-                c.removeBackdrop(), b && b()
+            var n = function() {
+                e.removeBackdrop(), t && t()
             };
-            a.support.transition && this.$element.hasClass("fade") ? this.$backdrop.one("bsTransitionEnd", f).emulateTransitionEnd(150) : f()
-        } else b && b()
-    }, c.prototype.checkScrollbar = function() {
-        document.body.clientWidth >= window.innerWidth || (this.scrollbarWidth = this.scrollbarWidth || this.measureScrollbar())
-    }, c.prototype.setScrollbar = function() {
-        var a = parseInt(this.$body.css("padding-right") || 0, 10);
-        this.scrollbarWidth && this.$body.css("padding-right", a + this.scrollbarWidth)
-    }, c.prototype.resetScrollbar = function() {
-        this.$body.css("padding-right", "")
-    }, c.prototype.measureScrollbar = function() {
-        var a = document.createElement("div");
-        a.className = "modal-scrollbar-measure", this.$body.append(a);
-        var b = a.offsetWidth - a.clientWidth;
-        return this.$body[0].removeChild(a), b
-    };
-    var d = a.fn.modal;
-    a.fn.modal = b, a.fn.modal.Constructor = c, a.fn.modal.noConflict = function() {
-        return a.fn.modal = d, this
-    }, a(document).on("click.bs.modal.data-api", '[data-toggle="modal"]', function(c) {
-        var d = a(this),
-            e = d.attr("href"),
-            f = a(d.attr("data-target") || e && e.replace(/.*(?=#[^\s]+$)/, "")),
-            g = f.data("bs.modal") ? "toggle" : a.extend({
-                remote: !/#/.test(e) && e
-            }, f.data(), d.data());
-        d.is("a") && c.preventDefault(), f.one("show.bs.modal", function(a) {
-            a.isDefaultPrevented() || f.one("hidden.bs.modal", function() {
-                d.is(":visible") && d.trigger("focus")
+            a.support.transition && this.$element.hasClass("fade") ? this.$backdrop.one("bsTransitionEnd", n).emulateTransitionEnd(s.BACKDROP_TRANSITION_DURATION) : n()
+        } else t && t()
+    }, s.prototype.handleUpdate = function() {
+        this.adjustDialog()
+    }, s.prototype.adjustDialog = function() {
+        var t = this.$element[0].scrollHeight > document.documentElement.clientHeight;
+        this.$element.css({
+            paddingLeft: !this.bodyIsOverflowing && t ? this.scrollbarWidth : "",
+            paddingRight: this.bodyIsOverflowing && !t ? this.scrollbarWidth : ""
+        })
+    }, s.prototype.resetAdjustments = function() {
+        this.$element.css({
+            paddingLeft: "",
+            paddingRight: ""
+        })
+    }, s.prototype.checkScrollbar = function() {
+        var t = window.innerWidth;
+        if (!t) {
+            var e = document.documentElement.getBoundingClientRect();
+            t = e.right - Math.abs(e.left)
+        }
+        this.bodyIsOverflowing = document.body.clientWidth < t, this.scrollbarWidth = this.measureScrollbar()
+    }, s.prototype.setScrollbar = function() {
+        var t = parseInt(this.$body.css("padding-right") || 0, 10);
+        this.originalBodyPad = document.body.style.paddingRight || "";
+        var n = this.scrollbarWidth;
+        this.bodyIsOverflowing && (this.$body.css("padding-right", t + n), a(this.fixedContent).each(function(t, e) {
+            var i = e.style.paddingRight,
+                o = a(e).css("padding-right");
+            a(e).data("padding-right", i).css("padding-right", parseFloat(o) + n + "px")
+        }))
+    }, s.prototype.resetScrollbar = function() {
+        this.$body.css("padding-right", this.originalBodyPad), a(this.fixedContent).each(function(t, e) {
+            var i = a(e).data("padding-right");
+            a(e).removeData("padding-right"), e.style.paddingRight = i || ""
+        })
+    }, s.prototype.measureScrollbar = function() {
+        var t = document.createElement("div");
+        t.className = "modal-scrollbar-measure", this.$body.append(t);
+        var e = t.offsetWidth - t.clientWidth;
+        return this.$body[0].removeChild(t), e
+    };
+    var t = a.fn.modal;
+    a.fn.modal = r, a.fn.modal.Constructor = s, a.fn.modal.noConflict = function() {
+        return a.fn.modal = t, this
+    }, a(document).on("click.bs.modal.data-api", '[data-toggle="modal"]', function(t) {
+        var e = a(this),
+            i = e.attr("href"),
+            o = e.attr("data-target") || i && i.replace(/.*(?=#[^\s]+$)/, ""),
+            n = a(document).find(o),
+            s = n.data("bs.modal") ? "toggle" : a.extend({
+                remote: !/#/.test(i) && i
+            }, n.data(), e.data());
+        e.is("a") && t.preventDefault(), n.one("show.bs.modal", function(t) {
+            t.isDefaultPrevented() || n.one("hidden.bs.modal", function() {
+                e.is(":visible") && e.trigger("focus")
             })
-        }), b.call(f, g, this)
+        }), r.call(n, s, this)
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(g) {
     "use strict";
+    var o = ["sanitize", "whiteList", "sanitizeFn"],
+        a = ["background", "cite", "href", "itemtype", "longdesc", "poster", "src", "xlink:href"],
+        t = {
+            "*": ["class", "dir", "id", "lang", "role", /^aria-[\w-]*$/i],
+            a: ["target", "href", "title", "rel"],
+            area: [],
+            b: [],
+            br: [],
+            col: [],
+            code: [],
+            div: [],
+            em: [],
+            hr: [],
+            h1: [],
+            h2: [],
+            h3: [],
+            h4: [],
+            h5: [],
+            h6: [],
+            i: [],
+            img: ["src", "alt", "title", "width", "height"],
+            li: [],
+            ol: [],
+            p: [],
+            pre: [],
+            s: [],
+            small: [],
+            span: [],
+            sub: [],
+            sup: [],
+            strong: [],
+            u: [],
+            ul: []
+        },
+        r = /^(?:(?:https?|mailto|ftp|tel|file):|[^&:/?#]*(?:[/?#]|$))/gi,
+        l = /^data:(?:image\/(?:bmp|gif|jpeg|jpg|png|tiff|webp)|video\/(?:mpeg|mp4|ogg|webm)|audio\/(?:mp3|oga|ogg|opus));base64,[a-z0-9+/]+=*$/i;
 
-    function b(b) {
-        return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.tooltip"),
-                f = "object" == typeof b && b;
-            (e || "destroy" != b) && (e || d.data("bs.tooltip", e = new c(this, f)), "string" == typeof b && e[b]())
-        })
+    function u(t, e) {
+        var i = t.nodeName.toLowerCase();
+        if (-1 !== g.inArray(i, e)) return -1 === g.inArray(i, a) || Boolean(t.nodeValue.match(r) || t.nodeValue.match(l));
+        for (var o = g(e).filter(function(t, e) {
+                return e instanceof RegExp
+            }), n = 0, s = o.length; n < s; n++)
+            if (i.match(o[n])) return !0;
+        return !1
+    }
+
+    function n(t, e, i) {
+        if (0 === t.length) return t;
+        if (i && "function" == typeof i) return i(t);
+        if (!document.implementation || !document.implementation.createHTMLDocument) return t;
+        var o = document.implementation.createHTMLDocument("sanitization");
+        o.body.innerHTML = t;
+        for (var n = g.map(e, function(t, e) {
+                return e
+            }), s = g(o.body).find("*"), a = 0, r = s.length; a < r; a++) {
+            var l = s[a],
+                h = l.nodeName.toLowerCase();
+            if (-1 !== g.inArray(h, n))
+                for (var d = g.map(l.attributes, function(t) {
+                        return t
+                    }), p = [].concat(e["*"] || [], e[h] || []), c = 0, f = d.length; c < f; c++) u(d[c], p) || l.removeAttribute(d[c].nodeName);
+            else l.parentNode.removeChild(l)
+        }
+        return o.body.innerHTML
     }
-    var c = function(a, b) {
-        this.type = this.options = this.enabled = this.timeout = this.hoverState = this.$element = null, this.init("tooltip", a, b)
+    var m = function(t, e) {
+        this.type = null, this.options = null, this.enabled = null, this.timeout = null, this.hoverState = null, this.$element = null, this.inState = null, this.init("tooltip", t, e)
     };
-    c.VERSION = "3.2.0", c.DEFAULTS = {
+    m.VERSION = "3.4.1", m.TRANSITION_DURATION = 150, m.DEFAULTS = {
         animation: !0,
         placement: "top",
         selector: !1,
         template: '<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>',
         trigger: "hover focus",
         title: "",
         delay: 0,
         html: !1,
         container: !1,
         viewport: {
             selector: "body",
             padding: 0
-        }
-    }, c.prototype.init = function(b, c, d) {
-        this.enabled = !0, this.type = b, this.$element = a(c), this.options = this.getOptions(d), this.$viewport = this.options.viewport && a(this.options.viewport.selector || this.options.viewport);
-        for (var e = this.options.trigger.split(" "), f = e.length; f--;) {
-            var g = e[f];
-            if ("click" == g) this.$element.on("click." + this.type, this.options.selector, a.proxy(this.toggle, this));
-            else if ("manual" != g) {
-                var h = "hover" == g ? "mouseenter" : "focusin",
-                    i = "hover" == g ? "mouseleave" : "focusout";
-                this.$element.on(h + "." + this.type, this.options.selector, a.proxy(this.enter, this)), this.$element.on(i + "." + this.type, this.options.selector, a.proxy(this.leave, this))
+        },
+        sanitize: !0,
+        sanitizeFn: null,
+        whiteList: t
+    }, m.prototype.init = function(t, e, i) {
+        if (this.enabled = !0, this.type = t, this.$element = g(e), this.options = this.getOptions(i), this.$viewport = this.options.viewport && g(document).find(g.isFunction(this.options.viewport) ? this.options.viewport.call(this, this.$element) : this.options.viewport.selector || this.options.viewport), this.inState = {
+                click: !1,
+                hover: !1,
+                focus: !1
+            }, this.$element[0] instanceof document.constructor && !this.options.selector) throw new Error("`selector` option must be specified when initializing " + this.type + " on the window.document object!");
+        for (var o = this.options.trigger.split(" "), n = o.length; n--;) {
+            var s = o[n];
+            if ("click" == s) this.$element.on("click." + this.type, this.options.selector, g.proxy(this.toggle, this));
+            else if ("manual" != s) {
+                var a = "hover" == s ? "mouseenter" : "focusin",
+                    r = "hover" == s ? "mouseleave" : "focusout";
+                this.$element.on(a + "." + this.type, this.options.selector, g.proxy(this.enter, this)), this.$element.on(r + "." + this.type, this.options.selector, g.proxy(this.leave, this))
             }
         }
-        this.options.selector ? this._options = a.extend({}, this.options, {
+        this.options.selector ? this._options = g.extend({}, this.options, {
             trigger: "manual",
             selector: ""
         }) : this.fixTitle()
-    }, c.prototype.getDefaults = function() {
-        return c.DEFAULTS
-    }, c.prototype.getOptions = function(b) {
-        return b = a.extend({}, this.getDefaults(), this.$element.data(), b), b.delay && "number" == typeof b.delay && (b.delay = {
-            show: b.delay,
-            hide: b.delay
-        }), b
-    }, c.prototype.getDelegateOptions = function() {
-        var b = {},
-            c = this.getDefaults();
-        return this._options && a.each(this._options, function(a, d) {
-            c[a] != d && (b[a] = d)
-        }), b
-    }, c.prototype.enter = function(b) {
-        var c = b instanceof this.constructor ? b : a(b.currentTarget).data("bs." + this.type);
-        return c || (c = new this.constructor(b.currentTarget, this.getDelegateOptions()), a(b.currentTarget).data("bs." + this.type, c)), clearTimeout(c.timeout), c.hoverState = "in", c.options.delay && c.options.delay.show ? void(c.timeout = setTimeout(function() {
-            "in" == c.hoverState && c.show()
-        }, c.options.delay.show)) : c.show()
-    }, c.prototype.leave = function(b) {
-        var c = b instanceof this.constructor ? b : a(b.currentTarget).data("bs." + this.type);
-        return c || (c = new this.constructor(b.currentTarget, this.getDelegateOptions()), a(b.currentTarget).data("bs." + this.type, c)), clearTimeout(c.timeout), c.hoverState = "out", c.options.delay && c.options.delay.hide ? void(c.timeout = setTimeout(function() {
-            "out" == c.hoverState && c.hide()
-        }, c.options.delay.hide)) : c.hide()
-    }, c.prototype.show = function() {
-        var b = a.Event("show.bs." + this.type);
+    }, m.prototype.getDefaults = function() {
+        return m.DEFAULTS
+    }, m.prototype.getOptions = function(t) {
+        var e = this.$element.data();
+        for (var i in e) e.hasOwnProperty(i) && -1 !== g.inArray(i, o) && delete e[i];
+        return (t = g.extend({}, this.getDefaults(), e, t)).delay && "number" == typeof t.delay && (t.delay = {
+            show: t.delay,
+            hide: t.delay
+        }), t.sanitize && (t.template = n(t.template, t.whiteList, t.sanitizeFn)), t
+    }, m.prototype.getDelegateOptions = function() {
+        var i = {},
+            o = this.getDefaults();
+        return this._options && g.each(this._options, function(t, e) {
+            o[t] != e && (i[t] = e)
+        }), i
+    }, m.prototype.enter = function(t) {
+        var e = t instanceof this.constructor ? t : g(t.currentTarget).data("bs." + this.type);
+        if (e || (e = new this.constructor(t.currentTarget, this.getDelegateOptions()), g(t.currentTarget).data("bs." + this.type, e)), t instanceof g.Event && (e.inState["focusin" == t.type ? "focus" : "hover"] = !0), e.tip().hasClass("in") || "in" == e.hoverState) e.hoverState = "in";
+        else {
+            if (clearTimeout(e.timeout), e.hoverState = "in", !e.options.delay || !e.options.delay.show) return e.show();
+            e.timeout = setTimeout(function() {
+                "in" == e.hoverState && e.show()
+            }, e.options.delay.show)
+        }
+    }, m.prototype.isInStateTrue = function() {
+        for (var t in this.inState)
+            if (this.inState[t]) return !0;
+        return !1
+    }, m.prototype.leave = function(t) {
+        var e = t instanceof this.constructor ? t : g(t.currentTarget).data("bs." + this.type);
+        if (e || (e = new this.constructor(t.currentTarget, this.getDelegateOptions()), g(t.currentTarget).data("bs." + this.type, e)), t instanceof g.Event && (e.inState["focusout" == t.type ? "focus" : "hover"] = !1), !e.isInStateTrue()) {
+            if (clearTimeout(e.timeout), e.hoverState = "out", !e.options.delay || !e.options.delay.hide) return e.hide();
+            e.timeout = setTimeout(function() {
+                "out" == e.hoverState && e.hide()
+            }, e.options.delay.hide)
+        }
+    }, m.prototype.show = function() {
+        var t = g.Event("show.bs." + this.type);
         if (this.hasContent() && this.enabled) {
-            this.$element.trigger(b);
-            var c = a.contains(document.documentElement, this.$element[0]);
-            if (b.isDefaultPrevented() || !c) return;
-            var d = this,
-                e = this.tip(),
-                f = this.getUID(this.type);
-            this.setContent(), e.attr("id", f), this.$element.attr("aria-describedby", f), this.options.animation && e.addClass("fade");
-            var g = "function" == typeof this.options.placement ? this.options.placement.call(this, e[0], this.$element[0]) : this.options.placement,
-                h = /\s?auto?\s?/i,
-                i = h.test(g);
-            i && (g = g.replace(h, "") || "top"), e.detach().css({
+            this.$element.trigger(t);
+            var e = g.contains(this.$element[0].ownerDocument.documentElement, this.$element[0]);
+            if (t.isDefaultPrevented() || !e) return;
+            var i = this,
+                o = this.tip(),
+                n = this.getUID(this.type);
+            this.setContent(), o.attr("id", n), this.$element.attr("aria-describedby", n), this.options.animation && o.addClass("fade");
+            var s = "function" == typeof this.options.placement ? this.options.placement.call(this, o[0], this.$element[0]) : this.options.placement,
+                a = /\s?auto?\s?/i,
+                r = a.test(s);
+            r && (s = s.replace(a, "") || "top"), o.detach().css({
                 top: 0,
                 left: 0,
                 display: "block"
-            }).addClass(g).data("bs." + this.type, this), this.options.container ? e.appendTo(this.options.container) : e.insertAfter(this.$element);
-            var j = this.getPosition(),
-                k = e[0].offsetWidth,
-                l = e[0].offsetHeight;
-            if (i) {
-                var m = g,
-                    n = this.$element.parent(),
-                    o = this.getPosition(n);
-                g = "bottom" == g && j.top + j.height + l - o.scroll > o.height ? "top" : "top" == g && j.top - o.scroll - l < 0 ? "bottom" : "right" == g && j.right + k > o.width ? "left" : "left" == g && j.left - k < o.left ? "right" : g, e.removeClass(m).addClass(g)
-            }
-            var p = this.getCalculatedOffset(g, j, k, l);
-            this.applyPlacement(p, g);
-            var q = function() {
-                d.$element.trigger("shown.bs." + d.type), d.hoverState = null
+            }).addClass(s).data("bs." + this.type, this), this.options.container ? o.appendTo(g(document).find(this.options.container)) : o.insertAfter(this.$element), this.$element.trigger("inserted.bs." + this.type);
+            var l = this.getPosition(),
+                h = o[0].offsetWidth,
+                d = o[0].offsetHeight;
+            if (r) {
+                var p = s,
+                    c = this.getPosition(this.$viewport);
+                s = "bottom" == s && l.bottom + d > c.bottom ? "top" : "top" == s && l.top - d < c.top ? "bottom" : "right" == s && l.right + h > c.width ? "left" : "left" == s && l.left - h < c.left ? "right" : s, o.removeClass(p).addClass(s)
+            }
+            var f = this.getCalculatedOffset(s, l, h, d);
+            this.applyPlacement(f, s);
+            var u = function() {
+                var t = i.hoverState;
+                i.$element.trigger("shown.bs." + i.type), i.hoverState = null, "out" == t && i.leave(i)
             };
-            a.support.transition && this.$tip.hasClass("fade") ? e.one("bsTransitionEnd", q).emulateTransitionEnd(150) : q()
+            g.support.transition && this.$tip.hasClass("fade") ? o.one("bsTransitionEnd", u).emulateTransitionEnd(m.TRANSITION_DURATION) : u()
         }
-    }, c.prototype.applyPlacement = function(b, c) {
-        var d = this.tip(),
-            e = d[0].offsetWidth,
-            f = d[0].offsetHeight,
-            g = parseInt(d.css("margin-top"), 10),
-            h = parseInt(d.css("margin-left"), 10);
-        isNaN(g) && (g = 0), isNaN(h) && (h = 0), b.top = b.top + g, b.left = b.left + h, a.offset.setOffset(d[0], a.extend({
-            using: function(a) {
-                d.css({
-                    top: Math.round(a.top),
-                    left: Math.round(a.left)
+    }, m.prototype.applyPlacement = function(t, e) {
+        var i = this.tip(),
+            o = i[0].offsetWidth,
+            n = i[0].offsetHeight,
+            s = parseInt(i.css("margin-top"), 10),
+            a = parseInt(i.css("margin-left"), 10);
+        isNaN(s) && (s = 0), isNaN(a) && (a = 0), t.top += s, t.left += a, g.offset.setOffset(i[0], g.extend({
+            using: function(t) {
+                i.css({
+                    top: Math.round(t.top),
+                    left: Math.round(t.left)
                 })
             }
-        }, b), 0), d.addClass("in");
-        var i = d[0].offsetWidth,
-            j = d[0].offsetHeight;
-        "top" == c && j != f && (b.top = b.top + f - j);
-        var k = this.getViewportAdjustedDelta(c, b, i, j);
-        k.left ? b.left += k.left : b.top += k.top;
-        var l = k.left ? 2 * k.left - e + i : 2 * k.top - f + j,
-            m = k.left ? "left" : "top",
-            n = k.left ? "offsetWidth" : "offsetHeight";
-        d.offset(b), this.replaceArrow(l, d[0][n], m)
-    }, c.prototype.replaceArrow = function(a, b, c) {
-        this.arrow().css(c, a ? 50 * (1 - a / b) + "%" : "")
-    }, c.prototype.setContent = function() {
-        var a = this.tip(),
-            b = this.getTitle();
-        a.find(".tooltip-inner")[this.options.html ? "html" : "text"](b), a.removeClass("fade in top bottom left right")
-    }, c.prototype.hide = function() {
-        function b() {
-            "in" != c.hoverState && d.detach(), c.$element.trigger("hidden.bs." + c.type)
-        }
-        var c = this,
-            d = this.tip(),
-            e = a.Event("hide.bs." + this.type);
-        return this.$element.removeAttr("aria-describedby"), this.$element.trigger(e), e.isDefaultPrevented() ? void 0 : (d.removeClass("in"), a.support.transition && this.$tip.hasClass("fade") ? d.one("bsTransitionEnd", b).emulateTransitionEnd(150) : b(), this.hoverState = null, this)
-    }, c.prototype.fixTitle = function() {
-        var a = this.$element;
-        (a.attr("title") || "string" != typeof a.attr("data-original-title")) && a.attr("data-original-title", a.attr("title") || "").attr("title", "")
-    }, c.prototype.hasContent = function() {
+        }, t), 0), i.addClass("in");
+        var r = i[0].offsetWidth,
+            l = i[0].offsetHeight;
+        "top" == e && l != n && (t.top = t.top + n - l);
+        var h = this.getViewportAdjustedDelta(e, t, r, l);
+        h.left ? t.left += h.left : t.top += h.top;
+        var d = /top|bottom/.test(e),
+            p = d ? 2 * h.left - o + r : 2 * h.top - n + l,
+            c = d ? "offsetWidth" : "offsetHeight";
+        i.offset(t), this.replaceArrow(p, i[0][c], d)
+    }, m.prototype.replaceArrow = function(t, e, i) {
+        this.arrow().css(i ? "left" : "top", 50 * (1 - t / e) + "%").css(i ? "top" : "left", "")
+    }, m.prototype.setContent = function() {
+        var t = this.tip(),
+            e = this.getTitle();
+        this.options.html ? (this.options.sanitize && (e = n(e, this.options.whiteList, this.options.sanitizeFn)), t.find(".tooltip-inner").html(e)) : t.find(".tooltip-inner").text(e), t.removeClass("fade in top bottom left right")
+    }, m.prototype.hide = function(t) {
+        var e = this,
+            i = g(this.$tip),
+            o = g.Event("hide.bs." + this.type);
+
+        function n() {
+            "in" != e.hoverState && i.detach(), e.$element && e.$element.removeAttr("aria-describedby").trigger("hidden.bs." + e.type), t && t()
+        }
+        if (this.$element.trigger(o), !o.isDefaultPrevented()) return i.removeClass("in"), g.support.transition && i.hasClass("fade") ? i.one("bsTransitionEnd", n).emulateTransitionEnd(m.TRANSITION_DURATION) : n(), this.hoverState = null, this
+    }, m.prototype.fixTitle = function() {
+        var t = this.$element;
+        (t.attr("title") || "string" != typeof t.attr("data-original-title")) && t.attr("data-original-title", t.attr("title") || "").attr("title", "")
+    }, m.prototype.hasContent = function() {
         return this.getTitle()
-    }, c.prototype.getPosition = function(b) {
-        b = b || this.$element;
-        var c = b[0],
-            d = "BODY" == c.tagName;
-        return a.extend({}, "function" == typeof c.getBoundingClientRect ? c.getBoundingClientRect() : null, {
-            scroll: d ? document.documentElement.scrollTop || document.body.scrollTop : b.scrollTop(),
-            width: d ? a(window).width() : b.outerWidth(),
-            height: d ? a(window).height() : b.outerHeight()
-        }, d ? {
-            top: 0,
-            left: 0
-        } : b.offset())
-    }, c.prototype.getCalculatedOffset = function(a, b, c, d) {
-        return "bottom" == a ? {
-            top: b.top + b.height,
-            left: b.left + b.width / 2 - c / 2
-        } : "top" == a ? {
-            top: b.top - d,
-            left: b.left + b.width / 2 - c / 2
-        } : "left" == a ? {
-            top: b.top + b.height / 2 - d / 2,
-            left: b.left - c
+    }, m.prototype.getPosition = function(t) {
+        var e = (t = t || this.$element)[0],
+            i = "BODY" == e.tagName,
+            o = e.getBoundingClientRect();
+        null == o.width && (o = g.extend({}, o, {
+            width: o.right - o.left,
+            height: o.bottom - o.top
+        }));
+        var n = window.SVGElement && e instanceof window.SVGElement,
+            s = i ? {
+                top: 0,
+                left: 0
+            } : n ? null : t.offset(),
+            a = {
+                scroll: i ? document.documentElement.scrollTop || document.body.scrollTop : t.scrollTop()
+            },
+            r = i ? {
+                width: g(window).width(),
+                height: g(window).height()
+            } : null;
+        return g.extend({}, o, a, r, s)
+    }, m.prototype.getCalculatedOffset = function(t, e, i, o) {
+        return "bottom" == t ? {
+            top: e.top + e.height,
+            left: e.left + e.width / 2 - i / 2
+        } : "top" == t ? {
+            top: e.top - o,
+            left: e.left + e.width / 2 - i / 2
+        } : "left" == t ? {
+            top: e.top + e.height / 2 - o / 2,
+            left: e.left - i
         } : {
-            top: b.top + b.height / 2 - d / 2,
-            left: b.left + b.width
+            top: e.top + e.height / 2 - o / 2,
+            left: e.left + e.width
         }
-    }, c.prototype.getViewportAdjustedDelta = function(a, b, c, d) {
-        var e = {
+    }, m.prototype.getViewportAdjustedDelta = function(t, e, i, o) {
+        var n = {
             top: 0,
             left: 0
         };
-        if (!this.$viewport) return e;
-        var f = this.options.viewport && this.options.viewport.padding || 0,
-            g = this.getPosition(this.$viewport);
-        if (/right|left/.test(a)) {
-            var h = b.top - f - g.scroll,
-                i = b.top + f - g.scroll + d;
-            h < g.top ? e.top = g.top - h : i > g.top + g.height && (e.top = g.top + g.height - i)
+        if (!this.$viewport) return n;
+        var s = this.options.viewport && this.options.viewport.padding || 0,
+            a = this.getPosition(this.$viewport);
+        if (/right|left/.test(t)) {
+            var r = e.top - s - a.scroll,
+                l = e.top + s - a.scroll + o;
+            r < a.top ? n.top = a.top - r : l > a.top + a.height && (n.top = a.top + a.height - l)
         } else {
-            var j = b.left - f,
-                k = b.left + f + c;
-            j < g.left ? e.left = g.left - j : k > g.width && (e.left = g.left + g.width - k)
-        }
-        return e
-    }, c.prototype.getTitle = function() {
-        var a, b = this.$element,
-            c = this.options;
-        return a = b.attr("data-original-title") || ("function" == typeof c.title ? c.title.call(b[0]) : c.title)
-    }, c.prototype.getUID = function(a) {
-        do a += ~~(1e6 * Math.random()); while (document.getElementById(a));
-        return a
-    }, c.prototype.tip = function() {
-        return this.$tip = this.$tip || a(this.options.template)
-    }, c.prototype.arrow = function() {
+            var h = e.left - s,
+                d = e.left + s + i;
+            h < a.left ? n.left = a.left - h : d > a.right && (n.left = a.left + a.width - d)
+        }
+        return n
+    }, m.prototype.getTitle = function() {
+        var t = this.$element,
+            e = this.options;
+        return t.attr("data-original-title") || ("function" == typeof e.title ? e.title.call(t[0]) : e.title)
+    }, m.prototype.getUID = function(t) {
+        for (; t += ~~(1e6 * Math.random()), document.getElementById(t););
+        return t
+    }, m.prototype.tip = function() {
+        if (!this.$tip && (this.$tip = g(this.options.template), 1 != this.$tip.length)) throw new Error(this.type + " `template` option must consist of exactly 1 top-level element!");
+        return this.$tip
+    }, m.prototype.arrow = function() {
         return this.$arrow = this.$arrow || this.tip().find(".tooltip-arrow")
-    }, c.prototype.validate = function() {
-        this.$element[0].parentNode || (this.hide(), this.$element = null, this.options = null)
-    }, c.prototype.enable = function() {
+    }, m.prototype.enable = function() {
         this.enabled = !0
-    }, c.prototype.disable = function() {
+    }, m.prototype.disable = function() {
         this.enabled = !1
-    }, c.prototype.toggleEnabled = function() {
+    }, m.prototype.toggleEnabled = function() {
         this.enabled = !this.enabled
-    }, c.prototype.toggle = function(b) {
-        var c = this;
-        b && (c = a(b.currentTarget).data("bs." + this.type), c || (c = new this.constructor(b.currentTarget, this.getDelegateOptions()), a(b.currentTarget).data("bs." + this.type, c))), c.tip().hasClass("in") ? c.leave(c) : c.enter(c)
-    }, c.prototype.destroy = function() {
-        clearTimeout(this.timeout), this.hide().$element.off("." + this.type).removeData("bs." + this.type)
+    }, m.prototype.toggle = function(t) {
+        var e = this;
+        t && ((e = g(t.currentTarget).data("bs." + this.type)) || (e = new this.constructor(t.currentTarget, this.getDelegateOptions()), g(t.currentTarget).data("bs." + this.type, e))), t ? (e.inState.click = !e.inState.click, e.isInStateTrue() ? e.enter(e) : e.leave(e)) : e.tip().hasClass("in") ? e.leave(e) : e.enter(e)
+    }, m.prototype.destroy = function() {
+        var t = this;
+        clearTimeout(this.timeout), this.hide(function() {
+            t.$element.off("." + t.type).removeData("bs." + t.type), t.$tip && t.$tip.detach(), t.$tip = null, t.$arrow = null, t.$viewport = null, t.$element = null
+        })
+    }, m.prototype.sanitizeHtml = function(t) {
+        return n(t, this.options.whiteList, this.options.sanitizeFn)
     };
-    var d = a.fn.tooltip;
-    a.fn.tooltip = b, a.fn.tooltip.Constructor = c, a.fn.tooltip.noConflict = function() {
-        return a.fn.tooltip = d, this
-    }
-}(jQuery), + function(a) {
-    "use strict";
-
-    function b(b) {
+    var e = g.fn.tooltip;
+    g.fn.tooltip = function i(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.popover"),
-                f = "object" == typeof b && b;
-            (e || "destroy" != b) && (e || d.data("bs.popover", e = new c(this, f)), "string" == typeof b && e[b]())
+            var t = g(this),
+                e = t.data("bs.tooltip"),
+                i = "object" == typeof o && o;
+            !e && /destroy|hide/.test(o) || (e || t.data("bs.tooltip", e = new m(this, i)), "string" == typeof o && e[o]())
         })
+    }, g.fn.tooltip.Constructor = m, g.fn.tooltip.noConflict = function() {
+        return g.fn.tooltip = e, this
     }
-    var c = function(a, b) {
-        this.init("popover", a, b)
+}(jQuery),
+function(n) {
+    "use strict";
+    var s = function(t, e) {
+        this.init("popover", t, e)
     };
-    if (!a.fn.tooltip) throw new Error("Popover requires tooltip.js");
-    c.VERSION = "3.2.0", c.DEFAULTS = a.extend({}, a.fn.tooltip.Constructor.DEFAULTS, {
+    if (!n.fn.tooltip) throw new Error("Popover requires tooltip.js");
+    s.VERSION = "3.4.1", s.DEFAULTS = n.extend({}, n.fn.tooltip.Constructor.DEFAULTS, {
         placement: "right",
         trigger: "click",
         content: "",
         template: '<div class="popover" role="tooltip"><div class="arrow"></div><h3 class="popover-title"></h3><div class="popover-content"></div></div>'
-    }), c.prototype = a.extend({}, a.fn.tooltip.Constructor.prototype), c.prototype.constructor = c, c.prototype.getDefaults = function() {
-        return c.DEFAULTS
-    }, c.prototype.setContent = function() {
-        var a = this.tip(),
-            b = this.getTitle(),
-            c = this.getContent();
-        a.find(".popover-title")[this.options.html ? "html" : "text"](b), a.find(".popover-content").empty()[this.options.html ? "string" == typeof c ? "html" : "append" : "text"](c), a.removeClass("fade top bottom left right in"), a.find(".popover-title").html() || a.find(".popover-title").hide()
-    }, c.prototype.hasContent = function() {
+    }), ((s.prototype = n.extend({}, n.fn.tooltip.Constructor.prototype)).constructor = s).prototype.getDefaults = function() {
+        return s.DEFAULTS
+    }, s.prototype.setContent = function() {
+        var t = this.tip(),
+            e = this.getTitle(),
+            i = this.getContent();
+        if (this.options.html) {
+            var o = typeof i;
+            this.options.sanitize && (e = this.sanitizeHtml(e), "string" === o && (i = this.sanitizeHtml(i))), t.find(".popover-title").html(e), t.find(".popover-content").children().detach().end()["string" === o ? "html" : "append"](i)
+        } else t.find(".popover-title").text(e), t.find(".popover-content").children().detach().end().text(i);
+        t.removeClass("fade top bottom left right in"), t.find(".popover-title").html() || t.find(".popover-title").hide()
+    }, s.prototype.hasContent = function() {
         return this.getTitle() || this.getContent()
-    }, c.prototype.getContent = function() {
-        var a = this.$element,
-            b = this.options;
-        return a.attr("data-content") || ("function" == typeof b.content ? b.content.call(a[0]) : b.content)
-    }, c.prototype.arrow = function() {
+    }, s.prototype.getContent = function() {
+        var t = this.$element,
+            e = this.options;
+        return t.attr("data-content") || ("function" == typeof e.content ? e.content.call(t[0]) : e.content)
+    }, s.prototype.arrow = function() {
         return this.$arrow = this.$arrow || this.tip().find(".arrow")
-    }, c.prototype.tip = function() {
-        return this.$tip || (this.$tip = a(this.options.template)), this.$tip
     };
-    var d = a.fn.popover;
-    a.fn.popover = b, a.fn.popover.Constructor = c, a.fn.popover.noConflict = function() {
-        return a.fn.popover = d, this
+    var t = n.fn.popover;
+    n.fn.popover = function e(o) {
+        return this.each(function() {
+            var t = n(this),
+                e = t.data("bs.popover"),
+                i = "object" == typeof o && o;
+            !e && /destroy|hide/.test(o) || (e || t.data("bs.popover", e = new s(this, i)), "string" == typeof o && e[o]())
+        })
+    }, n.fn.popover.Constructor = s, n.fn.popover.noConflict = function() {
+        return n.fn.popover = t, this
     }
-}(jQuery), + function(a) {
+}(jQuery),
+function(s) {
     "use strict";
 
-    function b(c, d) {
-        var e = a.proxy(this.process, this);
-        this.$body = a("body"), this.$scrollElement = a(a(c).is("body") ? window : c), this.options = a.extend({}, b.DEFAULTS, d), this.selector = (this.options.target || "") + " .nav li > a", this.offsets = [], this.targets = [], this.activeTarget = null, this.scrollHeight = 0, this.$scrollElement.on("scroll.bs.scrollspy", e), this.refresh(), this.process()
+    function n(t, e) {
+        this.$body = s(document.body), this.$scrollElement = s(t).is(document.body) ? s(window) : s(t), this.options = s.extend({}, n.DEFAULTS, e), this.selector = (this.options.target || "") + " .nav li > a", this.offsets = [], this.targets = [], this.activeTarget = null, this.scrollHeight = 0, this.$scrollElement.on("scroll.bs.scrollspy", s.proxy(this.process, this)), this.refresh(), this.process()
     }
 
-    function c(c) {
+    function e(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.scrollspy"),
-                f = "object" == typeof c && c;
-            e || d.data("bs.scrollspy", e = new b(this, f)), "string" == typeof c && e[c]()
+            var t = s(this),
+                e = t.data("bs.scrollspy"),
+                i = "object" == typeof o && o;
+            e || t.data("bs.scrollspy", e = new n(this, i)), "string" == typeof o && e[o]()
         })
     }
-    b.VERSION = "3.2.0", b.DEFAULTS = {
+    n.VERSION = "3.4.1", n.DEFAULTS = {
         offset: 10
-    }, b.prototype.getScrollHeight = function() {
+    }, n.prototype.getScrollHeight = function() {
         return this.$scrollElement[0].scrollHeight || Math.max(this.$body[0].scrollHeight, document.documentElement.scrollHeight)
-    }, b.prototype.refresh = function() {
-        var b = "offset",
-            c = 0;
-        a.isWindow(this.$scrollElement[0]) || (b = "position", c = this.$scrollElement.scrollTop()), this.offsets = [], this.targets = [], this.scrollHeight = this.getScrollHeight();
-        var d = this;
-        this.$body.find(this.selector).map(function() {
-            var d = a(this),
-                e = d.data("target") || d.attr("href"),
-                f = /^#./.test(e) && a(e);
-            return f && f.length && f.is(":visible") && [
-                [f[b]().top + c, e]
+    }, n.prototype.refresh = function() {
+        var t = this,
+            o = "offset",
+            n = 0;
+        this.offsets = [], this.targets = [], this.scrollHeight = this.getScrollHeight(), s.isWindow(this.$scrollElement[0]) || (o = "position", n = this.$scrollElement.scrollTop()), this.$body.find(this.selector).map(function() {
+            var t = s(this),
+                e = t.data("target") || t.attr("href"),
+                i = /^#./.test(e) && s(e);
+            return i && i.length && i.is(":visible") && [
+                [i[o]().top + n, e]
             ] || null
-        }).sort(function(a, b) {
-            return a[0] - b[0]
+        }).sort(function(t, e) {
+            return t[0] - e[0]
         }).each(function() {
-            d.offsets.push(this[0]), d.targets.push(this[1])
+            t.offsets.push(this[0]), t.targets.push(this[1])
         })
-    }, b.prototype.process = function() {
-        var a, b = this.$scrollElement.scrollTop() + this.options.offset,
-            c = this.getScrollHeight(),
-            d = this.options.offset + c - this.$scrollElement.height(),
-            e = this.offsets,
-            f = this.targets,
-            g = this.activeTarget;
-        if (this.scrollHeight != c && this.refresh(), b >= d) return g != (a = f[f.length - 1]) && this.activate(a);
-        if (g && b <= e[0]) return g != (a = f[0]) && this.activate(a);
-        for (a = e.length; a--;) g != f[a] && b >= e[a] && (!e[a + 1] || b <= e[a + 1]) && this.activate(f[a])
-    }, b.prototype.activate = function(b) {
-        this.activeTarget = b, a(this.selector).parentsUntil(this.options.target, ".active").removeClass("active");
-        var c = this.selector + '[data-target="' + b + '"],' + this.selector + '[href="' + b + '"]',
-            d = a(c).parents("li").addClass("active");
-        d.parent(".dropdown-menu").length && (d = d.closest("li.dropdown").addClass("active")), d.trigger("activate.bs.scrollspy")
-    };
-    var d = a.fn.scrollspy;
-    a.fn.scrollspy = c, a.fn.scrollspy.Constructor = b, a.fn.scrollspy.noConflict = function() {
-        return a.fn.scrollspy = d, this
-    }, a(window).on("load.bs.scrollspy.data-api", function() {
-        a('[data-spy="scroll"]').each(function() {
-            var b = a(this);
-            c.call(b, b.data())
+    }, n.prototype.process = function() {
+        var t, e = this.$scrollElement.scrollTop() + this.options.offset,
+            i = this.getScrollHeight(),
+            o = this.options.offset + i - this.$scrollElement.height(),
+            n = this.offsets,
+            s = this.targets,
+            a = this.activeTarget;
+        if (this.scrollHeight != i && this.refresh(), o <= e) return a != (t = s[s.length - 1]) && this.activate(t);
+        if (a && e < n[0]) return this.activeTarget = null, this.clear();
+        for (t = n.length; t--;) a != s[t] && e >= n[t] && (n[t + 1] === undefined || e < n[t + 1]) && this.activate(s[t])
+    }, n.prototype.activate = function(t) {
+        this.activeTarget = t, this.clear();
+        var e = this.selector + '[data-target="' + t + '"],' + this.selector + '[href="' + t + '"]',
+            i = s(e).parents("li").addClass("active");
+        i.parent(".dropdown-menu").length && (i = i.closest("li.dropdown").addClass("active")), i.trigger("activate.bs.scrollspy")
+    }, n.prototype.clear = function() {
+        s(this.selector).parentsUntil(this.options.target, ".active").removeClass("active")
+    };
+    var t = s.fn.scrollspy;
+    s.fn.scrollspy = e, s.fn.scrollspy.Constructor = n, s.fn.scrollspy.noConflict = function() {
+        return s.fn.scrollspy = t, this
+    }, s(window).on("load.bs.scrollspy.data-api", function() {
+        s('[data-spy="scroll"]').each(function() {
+            var t = s(this);
+            e.call(t, t.data())
         })
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(r) {
     "use strict";
+    var a = function(t) {
+        this.element = r(t)
+    };
 
-    function b(b) {
+    function e(i) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.tab");
-            e || d.data("bs.tab", e = new c(this)), "string" == typeof b && e[b]()
+            var t = r(this),
+                e = t.data("bs.tab");
+            e || t.data("bs.tab", e = new a(this)), "string" == typeof i && e[i]()
         })
     }
-    var c = function(b) {
-        this.element = a(b)
-    };
-    c.VERSION = "3.2.0", c.prototype.show = function() {
-        var b = this.element,
-            c = b.closest("ul:not(.dropdown-menu)"),
-            d = b.data("target");
-        if (d || (d = b.attr("href"), d = d && d.replace(/.*(?=#[^\s]*$)/, "")), !b.parent("li").hasClass("active")) {
-            var e = c.find(".active:last a")[0],
-                f = a.Event("show.bs.tab", {
-                    relatedTarget: e
+    a.VERSION = "3.4.1", a.TRANSITION_DURATION = 150, a.prototype.show = function() {
+        var t = this.element,
+            e = t.closest("ul:not(.dropdown-menu)"),
+            i = t.data("target");
+        if (i || (i = (i = t.attr("href")) && i.replace(/.*(?=#[^\s]*$)/, "")), !t.parent("li").hasClass("active")) {
+            var o = e.find(".active:last a"),
+                n = r.Event("hide.bs.tab", {
+                    relatedTarget: t[0]
+                }),
+                s = r.Event("show.bs.tab", {
+                    relatedTarget: o[0]
                 });
-            if (b.trigger(f), !f.isDefaultPrevented()) {
-                var g = a(d);
-                this.activate(b.closest("li"), c), this.activate(g, g.parent(), function() {
-                    b.trigger({
+            if (o.trigger(n), t.trigger(s), !s.isDefaultPrevented() && !n.isDefaultPrevented()) {
+                var a = r(document).find(i);
+                this.activate(t.closest("li"), e), this.activate(a, a.parent(), function() {
+                    o.trigger({
+                        type: "hidden.bs.tab",
+                        relatedTarget: t[0]
+                    }), t.trigger({
                         type: "shown.bs.tab",
-                        relatedTarget: e
+                        relatedTarget: o[0]
                     })
                 })
             }
         }
-    }, c.prototype.activate = function(b, c, d) {
-        function e() {
-            f.removeClass("active").find("> .dropdown-menu > .active").removeClass("active"), b.addClass("active"), g ? (b[0].offsetWidth, b.addClass("in")) : b.removeClass("fade"), b.parent(".dropdown-menu") && b.closest("li.dropdown").addClass("active"), d && d()
-        }
-        var f = c.find("> .active"),
-            g = d && a.support.transition && f.hasClass("fade");
-        g ? f.one("bsTransitionEnd", e).emulateTransitionEnd(150) : e(), f.removeClass("in")
-    };
-    var d = a.fn.tab;
-    a.fn.tab = b, a.fn.tab.Constructor = c, a.fn.tab.noConflict = function() {
-        return a.fn.tab = d, this
-    }, a(document).on("click.bs.tab.data-api", '[data-toggle="tab"], [data-toggle="pill"]', function(c) {
-        c.preventDefault(), b.call(a(this), "show")
-    })
-}(jQuery), + function(a) {
+    }, a.prototype.activate = function(t, e, i) {
+        var o = e.find("> .active"),
+            n = i && r.support.transition && (o.length && o.hasClass("fade") || !!e.find("> .fade").length);
+
+        function s() {
+            o.removeClass("active").find("> .dropdown-menu > .active").removeClass("active").end().find('[data-toggle="tab"]').attr("aria-expanded", !1), t.addClass("active").find('[data-toggle="tab"]').attr("aria-expanded", !0), n ? (t[0].offsetWidth, t.addClass("in")) : t.removeClass("fade"), t.parent(".dropdown-menu").length && t.closest("li.dropdown").addClass("active").end().find('[data-toggle="tab"]').attr("aria-expanded", !0), i && i()
+        }
+        o.length && n ? o.one("bsTransitionEnd", s).emulateTransitionEnd(a.TRANSITION_DURATION) : s(), o.removeClass("in")
+    };
+    var t = r.fn.tab;
+    r.fn.tab = e, r.fn.tab.Constructor = a, r.fn.tab.noConflict = function() {
+        return r.fn.tab = t, this
+    };
+    var i = function(t) {
+        t.preventDefault(), e.call(r(this), "show")
+    };
+    r(document).on("click.bs.tab.data-api", '[data-toggle="tab"]', i).on("click.bs.tab.data-api", '[data-toggle="pill"]', i)
+}(jQuery),
+function(l) {
     "use strict";
+    var h = function(t, e) {
+        this.options = l.extend({}, h.DEFAULTS, e);
+        var i = this.options.target === h.DEFAULTS.target ? l(this.options.target) : l(document).find(this.options.target);
+        this.$target = i.on("scroll.bs.affix.data-api", l.proxy(this.checkPosition, this)).on("click.bs.affix.data-api", l.proxy(this.checkPositionWithEventLoop, this)), this.$element = l(t), this.affixed = null, this.unpin = null, this.pinnedOffset = null, this.checkPosition()
+    };
 
-    function b(b) {
+    function i(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.affix"),
-                f = "object" == typeof b && b;
-            e || d.data("bs.affix", e = new c(this, f)), "string" == typeof b && e[b]()
+            var t = l(this),
+                e = t.data("bs.affix"),
+                i = "object" == typeof o && o;
+            e || t.data("bs.affix", e = new h(this, i)), "string" == typeof o && e[o]()
         })
     }
-    var c = function(b, d) {
-        this.options = a.extend({}, c.DEFAULTS, d), this.$target = a(this.options.target).on("scroll.bs.affix.data-api", a.proxy(this.checkPosition, this)).on("click.bs.affix.data-api", a.proxy(this.checkPositionWithEventLoop, this)), this.$element = a(b), this.affixed = this.unpin = this.pinnedOffset = null, this.checkPosition()
-    };
-    c.VERSION = "3.2.0", c.RESET = "affix affix-top affix-bottom", c.DEFAULTS = {
+    h.VERSION = "3.4.1", h.RESET = "affix affix-top affix-bottom", h.DEFAULTS = {
         offset: 0,
         target: window
-    }, c.prototype.getPinnedOffset = function() {
+    }, h.prototype.getState = function(t, e, i, o) {
+        var n = this.$target.scrollTop(),
+            s = this.$element.offset(),
+            a = this.$target.height();
+        if (null != i && "top" == this.affixed) return n < i && "top";
+        if ("bottom" == this.affixed) return null != i ? !(n + this.unpin <= s.top) && "bottom" : !(n + a <= t - o) && "bottom";
+        var r = null == this.affixed,
+            l = r ? n : s.top;
+        return null != i && n <= i ? "top" : null != o && t - o <= l + (r ? a : e) && "bottom"
+    }, h.prototype.getPinnedOffset = function() {
         if (this.pinnedOffset) return this.pinnedOffset;
-        this.$element.removeClass(c.RESET).addClass("affix");
-        var a = this.$target.scrollTop(),
-            b = this.$element.offset();
-        return this.pinnedOffset = b.top - a
-    }, c.prototype.checkPositionWithEventLoop = function() {
-        setTimeout(a.proxy(this.checkPosition, this), 1)
-    }, c.prototype.checkPosition = function() {
+        this.$element.removeClass(h.RESET).addClass("affix");
+        var t = this.$target.scrollTop(),
+            e = this.$element.offset();
+        return this.pinnedOffset = e.top - t
+    }, h.prototype.checkPositionWithEventLoop = function() {
+        setTimeout(l.proxy(this.checkPosition, this), 1)
+    }, h.prototype.checkPosition = function() {
         if (this.$element.is(":visible")) {
-            var b = a(document).height(),
-                d = this.$target.scrollTop(),
-                e = this.$element.offset(),
-                f = this.options.offset,
-                g = f.top,
-                h = f.bottom;
-            "object" != typeof f && (h = g = f), "function" == typeof g && (g = f.top(this.$element)), "function" == typeof h && (h = f.bottom(this.$element));
-            var i = null != this.unpin && d + this.unpin <= e.top ? !1 : null != h && e.top + this.$element.height() >= b - h ? "bottom" : null != g && g >= d ? "top" : !1;
-            if (this.affixed !== i) {
+            var t = this.$element.height(),
+                e = this.options.offset,
+                i = e.top,
+                o = e.bottom,
+                n = Math.max(l(document).height(), l(document.body).height());
+            "object" != typeof e && (o = i = e), "function" == typeof i && (i = e.top(this.$element)), "function" == typeof o && (o = e.bottom(this.$element));
+            var s = this.getState(n, t, i, o);
+            if (this.affixed != s) {
                 null != this.unpin && this.$element.css("top", "");
-                var j = "affix" + (i ? "-" + i : ""),
-                    k = a.Event(j + ".bs.affix");
-                this.$element.trigger(k), k.isDefaultPrevented() || (this.affixed = i, this.unpin = "bottom" == i ? this.getPinnedOffset() : null, this.$element.removeClass(c.RESET).addClass(j).trigger(a.Event(j.replace("affix", "affixed"))), "bottom" == i && this.$element.offset({
-                    top: b - this.$element.height() - h
-                }))
+                var a = "affix" + (s ? "-" + s : ""),
+                    r = l.Event(a + ".bs.affix");
+                if (this.$element.trigger(r), r.isDefaultPrevented()) return;
+                this.affixed = s, this.unpin = "bottom" == s ? this.getPinnedOffset() : null, this.$element.removeClass(h.RESET).addClass(a).trigger(a.replace("affix", "affixed") + ".bs.affix")
             }
+            "bottom" == s && this.$element.offset({
+                top: n - t - o
+            })
         }
     };
-    var d = a.fn.affix;
-    a.fn.affix = b, a.fn.affix.Constructor = c, a.fn.affix.noConflict = function() {
-        return a.fn.affix = d, this
-    }, a(window).on("load", function() {
-        a('[data-spy="affix"]').each(function() {
-            var c = a(this),
-                d = c.data();
-            d.offset = d.offset || {}, d.offsetBottom && (d.offset.bottom = d.offsetBottom), d.offsetTop && (d.offset.top = d.offsetTop), b.call(c, d)
+    var t = l.fn.affix;
+    l.fn.affix = i, l.fn.affix.Constructor = h, l.fn.affix.noConflict = function() {
+        return l.fn.affix = t, this
+    }, l(window).on("load", function() {
+        l('[data-spy="affix"]').each(function() {
+            var t = l(this),
+                e = t.data();
+            e.offset = e.offset || {}, null != e.offsetBottom && (e.offset.bottom = e.offsetBottom), null != e.offsetTop && (e.offset.top = e.offsetTop), i.call(t, e)
         })
     })
 }(jQuery);
```

