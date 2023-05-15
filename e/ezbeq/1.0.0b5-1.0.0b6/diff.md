# Comparing `tmp/ezbeq-1.0.0b5.tar.gz` & `tmp/ezbeq-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-1.0.0b5.tar", last modified: Sun May 14 20:48:02 2023, max compression
+gzip compressed data, was "ezbeq-1.0.0b6.tar", last modified: Mon May 15 21:28:07 2023, max compression
```

## Comparing `ezbeq-1.0.0b5.tar` & `ezbeq-1.0.0b6.tar`

### file list

```diff
@@ -1,73 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.028172 ezbeq-1.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-14 20:48:02.028172 ezbeq-1.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.016172 ezbeq-1.0.0b5/ezbeq/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 20:47:23.000000 ezbeq-1.0.0b5/ezbeq/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.020172 ezbeq-1.0.0b5/ezbeq/apis/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/audiotypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/authors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/apis/years.py
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/htp1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/iir.py
--rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/jriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    41613 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/minidsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/ezbeq/qsys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.020172 ezbeq-1.0.0b5/ezbeq/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-14 20:46:46.000000 ezbeq-1.0.0b5/ezbeq/ui/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.016172 ezbeq-1.0.0b5/ezbeq/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.024172 ezbeq-1.0.0b5/ezbeq/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/css/main.79943053.css
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/css/main.79943053.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.024172 ezbeq-1.0.0b5/ezbeq/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   947949 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/js/main.7604d882.js
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/js/main.7604d882.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  4159946 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/js/main.7604d882.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.028172 ezbeq-1.0.0b5/ezbeq/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-greek-ext-400-normal.169619821ea93019d1bb.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-14 20:47:22.000000 ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.020172 ezbeq-1.0.0b5/ezbeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-14 20:48:02.000000 ezbeq-1.0.0b5/ezbeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-14 20:48:02.000000 ezbeq-1.0.0b5/ezbeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:48:02.000000 ezbeq-1.0.0b5/ezbeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-14 20:48:02.000000 ezbeq-1.0.0b5/ezbeq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:48:02.000000 ezbeq-1.0.0b5/ezbeq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-14 20:48:02.000000 ezbeq-1.0.0b5/ezbeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 20:48:02.000000 ezbeq-1.0.0b5/ezbeq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:48:02.028172 ezbeq-1.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:48:02.028172 ezbeq-1.0.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-05-14 20:45:41.000000 ezbeq-1.0.0b5/tests/test_minidsp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:28:07.360616 ezbeq-1.0.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-15 21:28:07.360616 ezbeq-1.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:28:07.356616 ezbeq-1.0.0b6/ezbeq/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:28:07.356616 ezbeq-1.0.0b6/ezbeq/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/audiotypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/apis/years.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/htp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/iir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/jriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41613 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/minidsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/ezbeq/qsys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:28:07.360616 ezbeq-1.0.0b6/ezbeq/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/apple-touch-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:28:07.360616 ezbeq-1.0.0b6/ezbeq/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   859749 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/index-ade3d6f6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/index-fce6f16f.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 21:27:27.000000 ezbeq-1.0.0b6/ezbeq/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-15 21:27:26.000000 ezbeq-1.0.0b6/ezbeq/ui/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:28:07.356616 ezbeq-1.0.0b6/ezbeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-15 21:28:07.000000 ezbeq-1.0.0b6/ezbeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-15 21:28:07.000000 ezbeq-1.0.0b6/ezbeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:28:07.000000 ezbeq-1.0.0b6/ezbeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 21:28:07.000000 ezbeq-1.0.0b6/ezbeq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:28:07.000000 ezbeq-1.0.0b6/ezbeq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-15 21:28:07.000000 ezbeq-1.0.0b6/ezbeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 21:28:07.000000 ezbeq-1.0.0b6/ezbeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:28:07.360616 ezbeq-1.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:28:07.360616 ezbeq-1.0.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-05-15 21:26:12.000000 ezbeq-1.0.0b6/tests/test_minidsp_api.py
```

### Comparing `ezbeq-1.0.0b5/LICENSE` & `ezbeq-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/PKG-INFO` & `ezbeq-1.0.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ezbeq-1.0.0b5/README.md` & `ezbeq-1.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/audiotypes.py` & `ezbeq-1.0.0b6/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/catalogue.py` & `ezbeq-1.0.0b6/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/contenttypes.py` & `ezbeq-1.0.0b6/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/devices.py` & `ezbeq-1.0.0b6/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/languages.py` & `ezbeq-1.0.0b6/ezbeq/apis/languages.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/meta.py` & `ezbeq-1.0.0b6/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/search.py` & `ezbeq-1.0.0b6/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/ws.py` & `ezbeq-1.0.0b6/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/apis/years.py` & `ezbeq-1.0.0b6/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/catalogue.py` & `ezbeq-1.0.0b6/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/config.py` & `ezbeq-1.0.0b6/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/device.py` & `ezbeq-1.0.0b6/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/htp1.py` & `ezbeq-1.0.0b6/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/iir.py` & `ezbeq-1.0.0b6/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/jriver.py` & `ezbeq-1.0.0b6/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/main.py` & `ezbeq-1.0.0b6/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/minidsp.py` & `ezbeq-1.0.0b6/ezbeq/minidsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/qsys.py` & `ezbeq-1.0.0b6/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-1.0.0b6/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-1.0.0b6/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/apple-touch-icon.png` & `ezbeq-1.0.0b6/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/favicon-16x16.png` & `ezbeq-1.0.0b6/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/favicon-32x32.png` & `ezbeq-1.0.0b6/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/favicon.ico` & `ezbeq-1.0.0b6/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/mstile-150x150.png` & `ezbeq-1.0.0b6/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-1.0.0b6/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-all-400-normal.c5d001fa922fa66a147f.woff` & `ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-cyrillic-400-normal.71a33b6b50457b2c903a.woff2` & `ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-cyrillic-ext-400-normal.804378952da8a10faae2.woff2` & `ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-greek-400-normal.c35e4c3958e209d17b31.woff2` & `ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-latin-400-normal.b009a76ad6afe4ebd301.woff2` & `ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-latin-ext-400-normal.861b791f9de857a6e7bc.woff2` & `ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq/ui/static/media/roboto-vietnamese-400-normal.3230f9b040f3c630e0c3.woff2` & `ezbeq-1.0.0b6/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/ezbeq.egg-info/PKG-INFO` & `ezbeq-1.0.0b6/ezbeq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ezbeq-1.0.0b5/ezbeq.egg-info/requires.txt` & `ezbeq-1.0.0b6/ezbeq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/setup.py` & `ezbeq-1.0.0b6/setup.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b5/tests/test_minidsp_api.py` & `ezbeq-1.0.0b6/tests/test_minidsp_api.py`

 * *Files identical despite different names*

