# Comparing `tmp/trame-client-2.7.5.tar.gz` & `tmp/trame-client-2.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-client-2.7.5.tar", last modified: Mon Mar 27 16:28:24 2023, max compression
+gzip compressed data, was "trame-client-2.7.6.tar", last modified: Mon May 15 21:25:18 2023, max compression
```

## Comparing `trame-client-2.7.5.tar` & `trame-client-2.7.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.961432 trame-client-2.7.5/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-03-27 16:27:52.000000 trame-client-2.7.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      234 2023-03-27 16:27:52.000000 trame-client-2.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3518 2023-03-27 16:28:24.961432 trame-client-2.7.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2785 2023-03-27 16:27:52.000000 trame-client-2.7.5/README.rst
--rw-r--r--   0 root         (0) root         (0)      842 2023-03-27 16:28:24.961432 trame-client-2.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 16:27:52.000000 trame-client-2.7.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       56 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame/modules/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       56 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      137 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame/widgets/client.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame/widgets/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame_client/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/LICENSE
--rw-r--r--   0 root         (0) root         (0)       82 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame_client/encoders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/encoders/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame_client/module/
--rw-r--r--   0 root         (0) root         (0)      455 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame_client/module/vue2-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame_client/module/vue2-www/css/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-03-27 16:28:13.000000 trame-client-2.7.5/trame_client/module/vue2-www/css/app.0b077e70.css
--rw-r--r--   0 root         (0) root         (0)     3963 2023-03-27 16:28:13.000000 trame-client-2.7.5/trame_client/module/vue2-www/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame_client/module/vue2-www/js/
--rw-r--r--   0 root         (0) root         (0)    22780 2023-03-27 16:28:13.000000 trame-client-2.7.5/trame_client/module/vue2-www/js/app.1733a6d7.js
--rw-r--r--   0 root         (0) root         (0)   169923 2023-03-27 16:28:13.000000 trame-client-2.7.5/trame_client/module/vue2-www/js/chunk-vendors.ec946a94.js
--rw-r--r--   0 root         (0) root         (0)     4506 2023-03-27 16:28:13.000000 trame-client-2.7.5/trame_client/module/vue2-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   107302 2023-03-27 16:28:13.000000 trame-client-2.7.5/trame_client/module/vue2-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/module/vue2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.961432 trame-client-2.7.5/trame_client/module/vue3-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.961432 trame-client-2.7.5/trame_client/module/vue3-www/assets/
--rw-r--r--   0 root         (0) root         (0)   107394 2023-03-27 16:28:19.000000 trame-client-2.7.5/trame_client/module/vue3-www/assets/index-eabf8301.js
--rw-r--r--   0 root         (0) root         (0)     3940 2023-03-27 16:28:19.000000 trame-client-2.7.5/trame_client/module/vue3-www/index.html
--rw-r--r--   0 root         (0) root         (0)     4506 2023-03-27 16:28:19.000000 trame-client-2.7.5/trame_client/module/vue3-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   128872 2023-03-27 16:28:19.000000 trame-client-2.7.5/trame_client/module/vue3-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/module/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.961432 trame-client-2.7.5/trame_client/resources/
--rw-r--r--   0 root         (0) root         (0)     7243 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/resources/attributes.json
--rw-r--r--   0 root         (0) root         (0)        2 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/resources/events.json
--rw-r--r--   0 root         (0) root         (0)      580 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/resources/vue.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.961432 trame-client-2.7.5/trame_client/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2301 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/ui/core.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.961432 trame-client-2.7.5/trame_client/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      205 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.961432 trame-client-2.7.5/trame_client/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19678 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/widgets/core.py
--rw-r--r--   0 root         (0) root         (0)     3482 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)   193844 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/widgets/html.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-03-27 16:27:52.000000 trame-client-2.7.5/trame_client/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 16:28:24.957432 trame-client-2.7.5/trame_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3518 2023-03-27 16:28:24.000000 trame-client-2.7.5/trame_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1448 2023-03-27 16:28:24.000000 trame-client-2.7.5/trame_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 16:28:24.000000 trame-client-2.7.5/trame_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-27 16:28:24.000000 trame-client-2.7.5/trame_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.662747 trame-client-2.7.6/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 21:24:45.000000 trame-client-2.7.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-15 21:24:45.000000 trame-client-2.7.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-05-15 21:25:18.662747 trame-client-2.7.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-05-15 21:24:45.000000 trame-client-2.7.6/README.rst
+-rw-r--r--   0 root         (0) root         (0)      842 2023-05-15 21:25:18.662747 trame-client-2.7.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 21:24:45.000000 trame-client-2.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/modules/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/widgets/client.py
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/widgets/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame_client/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client/encoders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/encoders/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client/module/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client/module/vue2-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client/module/vue2-www/css/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/css/app.0b077e70.css
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.658747 trame-client-2.7.6/trame_client/module/vue2-www/js/
+-rw-r--r--   0 root         (0) root         (0)    23163 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/js/app.4ae908a0.js
+-rw-r--r--   0 root         (0) root         (0)   169923 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/js/chunk-vendors.ec946a94.js
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   107302 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/module/vue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.658747 trame-client-2.7.6/trame_client/module/vue3-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.658747 trame-client-2.7.6/trame_client/module/vue3-www/assets/
+-rw-r--r--   0 root         (0) root         (0)   107764 2023-05-15 21:25:13.000000 trame-client-2.7.6/trame_client/module/vue3-www/assets/index-e4900adb.js
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-05-15 21:25:13.000000 trame-client-2.7.6/trame_client/module/vue3-www/index.html
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-05-15 21:25:12.000000 trame-client-2.7.6/trame_client/module/vue3-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   128872 2023-05-15 21:25:12.000000 trame-client-2.7.6/trame_client/module/vue3-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/module/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.658747 trame-client-2.7.6/trame_client/resources/
+-rw-r--r--   0 root         (0) root         (0)     7243 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/resources/attributes.json
+-rw-r--r--   0 root         (0) root         (0)        2 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/resources/events.json
+-rw-r--r--   0 root         (0) root         (0)      580 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/resources/vue.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.662747 trame-client-2.7.6/trame_client/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/ui/core.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.662747 trame-client-2.7.6/trame_client/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      205 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.662747 trame-client-2.7.6/trame_client/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/core.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)   193844 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/html.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-05-15 21:25:18.000000 trame-client-2.7.6/trame_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-05-15 21:25:18.000000 trame-client-2.7.6/trame_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 21:25:18.000000 trame-client-2.7.6/trame_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-15 21:25:18.000000 trame-client-2.7.6/trame_client.egg-info/top_level.txt
```

### Comparing `trame-client-2.7.5/LICENSE` & `trame-client-2.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/PKG-INFO` & `trame-client-2.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 2.7.5
+Version: 2.7.6
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-2.7.5/README.rst` & `trame-client-2.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/setup.cfg` & `trame-client-2.7.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-client
-version = 2.7.5
+version = 2.7.6
 description = Internal client of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-client-2.7.5/trame_client/LICENSE` & `trame-client-2.7.6/trame_client/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/encoders/numpy.py` & `trame-client-2.7.6/trame_client/encoders/numpy.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/module/vue2-www/css/app.0b077e70.css` & `trame-client-2.7.6/trame_client/module/vue2-www/css/app.0b077e70.css`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/module/vue2-www/index.html` & `trame-client-2.7.6/trame_client/module/vue2-www/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -78,8 +78,8 @@
           transform: rotate(0deg); /* Firefox 16+, IE 10+, Opera */
         }
         100% {
           -webkit-transform: rotate(360deg); /* Chrome, Opera 15+, Safari 3.1+ */
           -ms-transform: rotate(360deg); /* IE 9 */
           transform: rotate(360deg); /* Firefox 16+, IE 10+, Opera */
         }
-      }</style><script defer="defer" src="js/chunk-vendors.ec946a94.js"></script><script defer="defer" src="js/app.1733a6d7.js"></script><link href="css/app.0b077e70.css" rel="stylesheet"></head><body style="margin: 0; padding: 0;"><noscript><strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"><div style="position:absolute;top:0;left:0;width:100%;height:100%;z-index:1000;"><div class="trame__loader"></div><div class="trame__message">Loading...</div></div></div></body></html>
+      }</style><script defer="defer" src="js/chunk-vendors.ec946a94.js"></script><script defer="defer" src="js/app.4ae908a0.js"></script><link href="css/app.0b077e70.css" rel="stylesheet"></head><body style="margin: 0; padding: 0;"><noscript><strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"><div style="position:absolute;top:0;left:0;width:100%;height:100%;z-index:1000;"><div class="trame__loader"></div><div class="trame__message">Loading...</div></div></div></body></html>
```

### Comparing `trame-client-2.7.5/trame_client/module/vue2-www/js/app.1733a6d7.js` & `trame-client-2.7.6/trame_client/module/vue2-www/js/app.4ae908a0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 (function() {
     "use strict";
     var t = {
-            8327: function(t, e, n) {
+            4031: function(t, e, n) {
                 var s = n(6080),
                     r = (n(8674), n(9601), n(7727), Vue),
                     i = n.n(r),
                     a = function() {
                         var t = this,
                             e = t._self._c;
                         return e("trame-connect", {
@@ -175,15 +175,15 @@
                     return t.priority - e.priority
                 }
 
                 function O(t) {
                     L.addAttachement = t
                 }
                 const A = 2e6,
-                    k = {
+                    j = {
                         priority: 0,
                         async decorate(t) {
                             if (null === t || void 0 === t) return t;
                             if (t.constructor && t.constructor === File) {
                                 const {
                                     name: e,
                                     lastModified: n,
@@ -211,22 +211,22 @@
                                     content: a,
                                     _filter: ["content"]
                                 }
                             }
                             return t
                         }
                     },
-                    j = {
+                    k = {
                         priority: 0,
                         async decorate(t) {
                             if (null === t || void 0 === t) return t;
                             if ("string" === typeof t) return t;
                             if (t.constructor && t.constructor === FileList || t.length) {
                                 const e = [];
-                                for (let n = 0; n < t.length; n++) e.push(await k.decorate(t[n]));
+                                for (let n = 0; n < t.length; n++) e.push(await j.decorate(t[n]));
                                 return e
                             }
                             return t
                         }
                     },
                     U = {
                         priority: 0,
@@ -234,22 +234,22 @@
                             if (null === t || void 0 === t) return t;
                             if ("string" === typeof t) return t;
                             if (t.constructor && t.constructor === Object) {
                                 const e = {},
                                     n = Object.keys(t);
                                 for (let s = 0; s < n.length; s++) {
                                     const r = n[s];
-                                    e[r] = t[r], e[r] = await j.decorate(e[r]), e[r] = await k.decorate(e[r])
+                                    e[r] = t[r], e[r] = await k.decorate(e[r]), e[r] = await j.decorate(e[r])
                                 }
                                 return e
                             }
                             return t
                         }
                     },
-                    E = [k, j, U];
+                    E = [j, k, U];
 
                 function Z(t) {
                     E.push(t), E.sort(x)
                 }
                 async function V(t) {
                     let e = t;
                     for (let n = 0; n < E.length; n++) {
@@ -287,25 +287,25 @@
                 function D(t, e = 2) {
                     return B(t, ["B", "KB", "MB", "GB", "TB", "PB"], 1024, e)
                 }
                 var H = {
                     number: B,
                     bytes: D
                 };
-                async function K(t, e, n = "application/octet-stream") {
+                async function M(t, e, n = "application/octet-stream") {
                     const s = await Promise.resolve(e),
                         r = new Blob([s], {
                             type: n
                         }),
                         i = URL.createObjectURL(r),
                         a = document.createElement("a");
                     a.setAttribute("href", i), a.setAttribute("download", t), document.body.appendChild(a), a.click(), document.body.removeChild(a), setTimeout((() => URL.revokeObjectURL(i)), 1e3)
                 }
 
-                function M(t, e = window) {
+                function K(t, e = window) {
                     let n = e;
                     const s = t.split(".");
                     for (let r = 0; r < s.length; r++) n = n[s[r]];
                     return n
                 }
 
                 function F(t) {
@@ -354,16 +354,16 @@
                 }
 
                 function G(t) {
                     const e = [];
                     return J("", e, t), e
                 }
                 var X = {
-                    download: K,
-                    get: M,
+                    download: M,
+                    get: K,
                     safe: F,
                     tree: G,
                     vtk: P,
                     fmt: H
                 };
 
                 function Y(t) {
@@ -877,15 +877,15 @@
                         }, [e("path", {
                             attrs: {
                                 d: "M4,1C2.89,1 2,1.89 2,3V7C2,8.11 2.89,9 4,9H1V11H13V9H10C11.11,9 12,8.11 12,7V3C12,1.89 11.11,1 10,1H4M4,3H10V7H4V3M14,13C12.89,13 12,13.89 12,15V19C12,20.11 12.89,21 14,21H11V23H23V21H20C21.11,21 22,20.11 22,19V15C22,13.89 21.11,13 20,13H14M3.88,13.46L2.46,14.88L4.59,17L2.46,19.12L3.88,20.54L6,18.41L8.12,20.54L9.54,19.12L7.41,17L9.54,14.88L8.12,13.46L6,15.59L3.88,13.46M14,15H20V19H14V15Z"
                             }
                         })]), t._v(" " + t._s(t.message) + " ")])])])
                     },
                     At = [],
-                    kt = {
+                    jt = {
                         name: "Reconnect",
                         props: {
                             message: {
                                 type: String,
                                 default: "Click to reconnect..."
                             },
                             maxRetry: {
@@ -914,25 +914,25 @@
                             }), this.delay)))
                         },
                         beforeDestroy() {
                             this.resetRetry()
                         },
                         inject: ["trame"]
                     },
-                    jt = kt,
+                    kt = jt,
                     Ut = {
                         container: "style_container_n4xKQ",
                         center: "style_center_xzh58",
                         button: "style_button_kGhdk"
                     };
 
                 function Et(t) {
                     this["$style"] = Ut.locals || Ut
                 }
-                var Zt = (0, lt.Z)(jt, Ot, At, !1, Et, null, null),
+                var Zt = (0, lt.Z)(kt, Ot, At, !1, Et, null, null),
                     Vt = Zt.exports,
                     It = function() {
                         var t = this;
                         t._self._c;
                         return t._t("default", null, null, t.state)
                     },
                     Nt = [];
@@ -988,16 +988,16 @@
                         provide() {
                             return {
                                 state: this
                             }
                         }
                     },
                     Ht = Dt,
-                    Kt = (0, lt.Z)(Ht, It, Nt, !1, null, null, null),
-                    Mt = Kt.exports;
+                    Mt = (0, lt.Z)(Ht, It, Nt, !1, null, null, null),
+                    Kt = Mt.exports;
                 let Ft = 1;
 
                 function qt() {
                     return "trame_style_elem_" + Ft++
                 }
                 var zt, Jt, Gt = {
                         name: "TrameStyle",
@@ -1036,59 +1036,87 @@
                         name: "TrameExec",
                         props: ["event"],
                         methods: {
                             exec(t) {
                                 void 0 === t ? this.$emit("exec", this.event) : this.$emit("exec", t)
                             }
                         }
+                    };
+                const {
+                    inject: te,
+                    ref: ee,
+                    onBeforeMount: ne,
+                    onBeforeUnmount: se,
+                    watch: re
+                } = window.Vue;
+                var ie = {
+                        props: ["name"],
+                        setup(t) {
+                            const e = te("trame"),
+                                n = ee(null);
+
+                            function s() {
+                                const s = e.state.get(t.name);
+                                s !== n.value && (n.value = s)
+                            }
+                            return re((() => t.name), s), ne((() => {
+                                e.$on("stateChange", s), s()
+                            })), se((() => {
+                                e.$off("stateChange", s)
+                            })), {
+                                computed: n
+                            }
+                        },
+                        template: '<slot :value="computed"></slot>'
                     },
-                    te = {
+                    ae = {
                         TrameApp: wt,
                         TrameConnect: ut,
                         TrameLoading: xt,
                         TrameReconnect: Vt,
                         TrameTemplate: yt,
-                        TrameStateResolver: Mt,
+                        TrameStateResolver: Kt,
                         TrameStyle: Qt,
-                        TrameExec: Wt
+                        TrameExec: Wt,
+                        TrameGetter: ie
                     },
-                    ee = {
+                    oe = {
                         install(t) {
-                            Object.keys(te).forEach((e => {
-                                t.component(e, te[e])
+                            Object.keys(ae).forEach((e => {
+                                t.component(e, ae[e])
                             }))
                         }
                     };
-                const ne = "TrameConnect";
+                const le = "TrameConnect";
 
-                function se() {
-                    const t = S.getStatus(ne),
+                function ce() {
+                    const t = S.getStatus(le),
                         e = document.querySelector(".trame__message");
                     e && (e.innerHTML = t.message || t.type)
                 }
-                async function re(t) {
-                    t.use(ee);
-                    const e = S.getClient(ne);
+                async function ue(t) {
+                    t.use(oe);
+                    const e = S.getClient(le);
                     try {
                         await e.connect(S.configDecorator({
                             application: "trame",
                             useUrl: !0
                         }))
                     } catch (r) {
-                        return void se()
+                        return void ce()
                     }
-                    e.onConnectionError(se), e.onConnectionClose(se), O(e.getConnection().getSession().addAttachment);
+                    e.onConnectionError(ce), e.onConnectionClose(ce), O(e.getConnection().getSession().addAttachment);
                     const {
                         state: n
                     } = await e.getRemote().Trame.getState();
                     await rt(Object.keys(n), n), new t((0, s.Z)((0, s.Z)({}, tt), {}, {
                         render: t => t(wt)
                     })).$mount("#app")
                 }
-                re(i())
+                ue(i())
             }
         },
         e = {};
 
     function n(s) {
         var r = e[s];
         if (void 0 !== r) return r.exports;
@@ -1177,12 +1205,12 @@
                     for (e && e(s); c < a.length; c++) i = a[c], n.o(t, i) && t[i] && t[i][0](), t[i] = 0;
                     return n.O(u)
                 },
                 s = self["webpackChunktrame_components"] = self["webpackChunktrame_components"] || [];
             s.forEach(e.bind(null, 0)), s.push = e.bind(null, s.push.bind(s))
         }();
     var s = n.O(void 0, [998], (function() {
-        return n(8327)
+        return n(4031)
     }));
     s = n.O(s)
 })();
-//# sourceMappingURL=app.1733a6d7.js.map
+//# sourceMappingURL=app.4ae908a0.js.map
```

### Comparing `trame-client-2.7.5/trame_client/module/vue2-www/js/chunk-vendors.ec946a94.js` & `trame-client-2.7.6/trame_client/module/vue2-www/js/chunk-vendors.ec946a94.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/module/vue2-www/logo.png` & `trame-client-2.7.6/trame_client/module/vue2-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/module/vue2-www/vue.global.js` & `trame-client-2.7.6/trame_client/module/vue2-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/module/vue3-www/assets/index-eabf8301.js` & `trame-client-2.7.6/trame_client/module/vue3-www/assets/index-e4900adb.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4127,34 +4127,61 @@
                 n === void 0 ? e("exec", Go(t.event)) : e("exec", n)
             }
             return {
                 exec: r
             }
         }
     },
-    Jo = {
+    {
+        inject: Jo,
+        ref: qo,
+        onBeforeMount: Xo,
+        onBeforeUnmount: Yo,
+        watch: Qo
+    } = window.Vue,
+    Zo = {
+        props: ["name"],
+        setup(t) {
+            const e = Jo("trame"),
+                r = qo(null);
+
+            function n() {
+                const u = e.state.get(t.name);
+                u !== r.value && (r.value = u)
+            }
+            return Qo(() => t.name, n), Xo(() => {
+                e.state.addListener(n), n()
+            }), Yo(() => {
+                e.state.removeListener(n)
+            }), {
+                computed: r
+            }
+        },
+        template: '<slot :value="computed"></slot>'
+    },
+    ea = {
         props: {
             message: {
                 type: String,
                 default: "Loading..."
             }
         },
         template: `
         <div style="position:absolute;top:0;left:0;width:100%;height:100%;z-index:1000;">
             <div class="trame__loader"></div>
             <div class="trame__message">{{ message }}</div>
         </div>
     `
     },
     {
-        inject: qo,
-        onMounted: Xo,
-        onBeforeUnmount: Yo
+        inject: ta,
+        onMounted: ra,
+        onBeforeUnmount: na
     } = window.Vue,
-    Qo = {
+    ua = {
         props: {
             message: {
                 type: String,
                 default: "Click to reconnect..."
             },
             maxRetry: {
                 type: Number,
@@ -4162,31 +4189,31 @@
             },
             delay: {
                 type: Number,
                 default: 500
             }
         },
         setup(t) {
-            const e = qo("trame");
+            const e = ta("trame");
             let r = null,
                 n = 0;
             async function u() {
                 await e.connect()
             }
 
             function o() {
                 r && (clearInterval(r), r = null)
             }
-            return Xo(() => {
+            return ra(() => {
                 n = 0;
                 const a = oe.extractURLParameters().reconnect;
                 a && (console.log("reconnect", a), a === "auto" && (r = setInterval(() => {
                     n++ < t.maxRetry ? u() : o()
                 }, t.delay)))
-            }), Yo(() => {
+            }), na(() => {
                 o()
             }), {
                 connect: u
             }
         },
         template: `
     <div style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: 1000;">
@@ -4204,72 +4231,73 @@
           {{ message }}
         </div>
       </div>
     </div>
       `
     },
     {
-        unref: Zo
+        unref: oa
     } = window.Vue;
-let ea = 1;
+let aa = 1;
 
-function ta() {
-    return `trame_style_elem_${ea++}`
+function ia() {
+    return `trame_style_elem_${aa++}`
 }
-const ra = {
+const sa = {
         props: {
             css: {
                 type: String,
                 default: ""
             }
         },
         watch: {
             css(t) {
                 this.updateStyle(t)
             }
         },
         created() {
-            this.elemId = ta(), this.updateStyle(this.css)
+            this.elemId = ia(), this.updateStyle(this.css)
         },
         beforeUnmount() {
             this.removeStyle()
         },
         methods: {
             updateStyle(t) {
-                t = Zo(t);
+                t = oa(t);
                 let e = document.querySelector(`#${this.elemId}`);
                 t ? (e || (e = document.createElement("style"), e.id = this.elemId, document.head.appendChild(e)), e.innerHTML = t) : this.removeStyle()
             },
             removeStyle() {
                 const t = document.querySelector(`#${this.elemId}`);
                 t && t.parentNode.removeChild(t)
             }
         },
         template: '<div class="trame-style" />'
     },
     Ot = {
         TrameApp: Ko,
         TrameExec: Wo,
-        TrameLoading: Jo,
-        TrameReconnect: Qo,
-        TrameStyle: ra,
+        TrameGetter: Zo,
+        TrameLoading: ea,
+        TrameReconnect: ua,
+        TrameStyle: sa,
         TrameTemplate: Vo
     },
-    na = {
+    ca = {
         install(t) {
             Object.keys(Ot).forEach(e => {
                 t.component(e, Ot[e])
             })
         }
     },
     {
-        createApp: ua
+        createApp: fa
     } = window.Vue;
-async function oa() {
-    const t = ua({
+async function Da() {
+    const t = fa({
         template: "<trame-app use-url />"
     });
     let e = _o(t),
         r = et.configDecorator({
             application: "trame",
             useUrl: !0
         });
@@ -4301,13 +4329,13 @@
         try {
             e.client.isConnected() && e.client.getRemote().Trame.sendError(a.join(" "))
         } catch (i) {
             u(i)
         } finally {
             u(...a)
         }
-    }, window.addEventListener("error", a => console.error(`${a.type}: ${a.message}`)), t.use(na), t.provide("trame", e);
+    }, window.addEventListener("error", a => console.error(`${a.type}: ${a.message}`)), t.use(ca), t.provide("trame", e);
     const o = await Ao(e.state.state);
     for (let a = 0; a < o.length; a++) t.use(...o[a]), console.info(`Vue.use(${o[a]})`);
     t.mount("#app")
 }
-oa();
+Da();
```

### Comparing `trame-client-2.7.5/trame_client/module/vue3-www/index.html` & `trame-client-2.7.6/trame_client/module/vue3-www/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         100% {
           -webkit-transform: rotate(360deg); /* Chrome, Opera 15+, Safari 3.1+ */
           -ms-transform: rotate(360deg); /* IE 9 */
           transform: rotate(360deg); /* Firefox 16+, IE 10+, Opera */
         }
       }
     </style>
-    <script type="module" crossorigin src="./assets/index-eabf8301.js"></script>
+    <script type="module" crossorigin src="./assets/index-e4900adb.js"></script>
   </head>
   <body>
     <noscript>
       <strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong>
     </noscript>
     <div id="app">
       <div style="position:absolute;top:0;left:0;width:100%;height:100%;z-index:1000;">
```

### Comparing `trame-client-2.7.5/trame_client/module/vue3-www/logo.png` & `trame-client-2.7.6/trame_client/module/vue3-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/module/vue3-www/vue.global.js` & `trame-client-2.7.6/trame_client/module/vue3-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/resources/attributes.json` & `trame-client-2.7.6/trame_client/resources/attributes.json`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/resources/vue.json` & `trame-client-2.7.6/trame_client/resources/vue.json`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/ui/core.py` & `trame-client-2.7.6/trame_client/ui/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/ui/html.py` & `trame-client-2.7.6/trame_client/ui/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/utils/version.py` & `trame-client-2.7.6/trame_client/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/widgets/core.py` & `trame-client-2.7.6/trame_client/widgets/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/widgets/generator.py` & `trame-client-2.7.6/trame_client/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/widgets/html.py` & `trame-client-2.7.6/trame_client/widgets/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.5/trame_client/widgets/trame.py` & `trame-client-2.7.6/trame_client/widgets/trame.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .core import AbstractElement
 
 __all__ = [
     "Loading",
     "ServerTemplate",
     "Style",
     "JSEval",
+    "Getter",
 ]
 
 
 # -----------------------------------------------------------------------------
 # TrameLoading
 # -----------------------------------------------------------------------------
 class Loading(AbstractElement):
@@ -96,7 +97,24 @@
         """Update style content"""
         self.server.state[self._key] = css_content
 
     @property
     def var_name(self):
         """Name the the state variable used by this widget"""
         return self._key
+
+
+# -----------------------------------------------------------------------------
+# TrameGetter
+# -----------------------------------------------------------------------------
+class Getter(AbstractElement):
+    """Provide means to extract a reactive state variable from its name"""
+
+    def __init__(self, children=None, value_name=None, **kwargs):
+        super().__init__("trame-getter", **kwargs)
+        self._attr_names += [
+            "name",
+        ]
+        if value_name:
+            self._attributes["slot"] = f'v-slot="{{ value: {value_name} }}"'
+        else:
+            self._attributes["slot"] = 'v-slot="{ value }"'
```

### Comparing `trame-client-2.7.5/trame_client.egg-info/PKG-INFO` & `trame-client-2.7.6/trame_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 2.7.5
+Version: 2.7.6
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-2.7.5/trame_client.egg-info/SOURCES.txt` & `trame-client-2.7.6/trame_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 trame_client/module/__init__.py
 trame_client/module/vue2.py
 trame_client/module/vue3.py
 trame_client/module/vue2-www/index.html
 trame_client/module/vue2-www/logo.png
 trame_client/module/vue2-www/vue.global.js
 trame_client/module/vue2-www/css/app.0b077e70.css
-trame_client/module/vue2-www/js/app.1733a6d7.js
+trame_client/module/vue2-www/js/app.4ae908a0.js
 trame_client/module/vue2-www/js/chunk-vendors.ec946a94.js
 trame_client/module/vue3-www/index.html
 trame_client/module/vue3-www/logo.png
 trame_client/module/vue3-www/vue.global.js
-trame_client/module/vue3-www/assets/index-eabf8301.js
+trame_client/module/vue3-www/assets/index-e4900adb.js
 trame_client/resources/attributes.json
 trame_client/resources/events.json
 trame_client/resources/vue.json
 trame_client/ui/__init__.py
 trame_client/ui/core.py
 trame_client/ui/html.py
 trame_client/utils/__init__.py
```

