# Comparing `tmp/yafowil.widget.image-1.6.tar.gz` & `tmp/yafowil.widget.image-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yafowil.widget.image-1.6.tar", last modified: Thu Oct  6 07:59:45 2022, max compression
+gzip compressed data, was "yafowil.widget.image-2.0a1.tar", last modified: Mon May 15 12:44:45 2023, max compression
```

## Comparing `yafowil.widget.image-1.6.tar` & `yafowil.widget.image-2.0a1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1587 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1398 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5505 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      553 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1694 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      565 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      608 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/configure.zcml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4031 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/example.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1259 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2295 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1230 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2261 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1693 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/locales/yafowil.widget.image.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/resources/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/resources/widget.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1293 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/resources/widget.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/testing/
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/testing/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      698 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/testing/dummy.jpg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1239 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/testing/dummy.pdf
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1853 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/testing/dummy.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)    40608 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      785 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12283 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil/widget/image/widget.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5505 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1341 2022-10-06 07:59:45.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      126 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       48 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2022-10-06 07:59:44.000000 yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1674 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4391 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      574 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1736 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1588 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      608 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/configure.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4031 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1259 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2295 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1230 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2261 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1693 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/yafowil.widget.image.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1468 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      747 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/widget.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      698 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.jpg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1239 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.pdf
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1853 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    41672 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      785 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12283 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4391 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1380 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      109 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yafowil.widget.image-1.6/CHANGES.rst` & `yafowil.widget.image-2.0a1/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 Changes
 =======
 
-1.6 (2022-10-06)
-----------------
+2.0a1 (2023-05-15)
+------------------
+
+- Add ``webresource`` support.
+  [rnix]
+
+- Rewrite JavaScript using ES6.
+  [rnix]
 
 - Introduce ``rounddpi`` flag for image blueprint. Pillow, as of version 6.0,
   no longer rounds reported DPI values for BMP, JPEG and PNG images, but image
   manipulation programs may not produce accurate DPI values.
   [rnix]
```

### Comparing `yafowil.widget.image-1.6/LICENSE.rst` & `yafowil.widget.image-2.0a1/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 License
 =======
 
 Copyright (c) 2012-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
-Copyright (c) 2021, Yafowil Contributors
+Copyright (c) 2021-2022, Yafowil Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `yafowil.widget.image-1.6/README.rst` & `yafowil.widget.image-2.0a1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,7 +16,9 @@
 
 Contributors
 ============
 
 - Robert Niederreiter
 
 - Georg Bernhard
+
+- Lena Daxenbichler
```

### Comparing `yafowil.widget.image-1.6/setup.py` & `yafowil.widget.image-2.0a1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.6'
+version = '2.0a1'
 shortdesc = 'Image Widget for YAFOWIL'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
-tests_require = ['yafowil[test]']
 
 
 setup(
     name='yafowil.widget.image',
     version=version,
     description=shortdesc,
     long_description=longdesc,
@@ -41,21 +40,26 @@
     license='Simplified BSD',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['yafowil', 'yafowil.widget'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
+        'Pillow',
         'setuptools',
-        'yafowil>2.1.99',
+        'yafowil>2.1.99'
     ],
-    tests_require=tests_require,
-    extras_require=dict(
-        test=tests_require,
-    ),
+    tests_require=[
+        'lxml',
+        'zope.testrunner'
+    ],
+    extras_require=dict(test=[
+        'lxml',
+        'zope.testrunner'
+    ]),
     test_suite="yafowil.widget.image.tests",
     entry_points="""
     [yafowil.plugin]
     register = yafowil.widget.image:register
     example = yafowil.widget.image.example:get_example
     """
 )
```

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/configure.zcml` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/configure.zcml`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/example.py` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/example.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/locales/yafowil.widget.image.pot` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/yafowil.widget.image.pot`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/testing/dummy.jpg` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.jpg`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/testing/dummy.pdf` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.pdf`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/testing/dummy.png` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/tests.py` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 from yafowil.base import factory
 from yafowil.compat import IS_PY2
 from yafowil.tests import fxml
 from yafowil.tests import YafowilTestCase
 from yafowil.widget.image.utils import aspect_ratio_approximate
 from yafowil.widget.image.utils import same_aspect_ratio
 from yafowil.widget.image.utils import scale_size
+import os
 import PIL
 import pkg_resources
 import unittest
-import yafowil.loader  # noqa
 
 
 if IS_PY2:
     from StringIO import StringIO
 else:
     from importlib import reload
     from io import BytesIO as StringIO
 
 
+def np(path):
+    return path.replace('/', os.path.sep)
+
+
 class TestUtils(unittest.TestCase):
 
     def test_aspect_ratio_approximate(self):
         self.assertEqual(
             aspect_ratio_approximate((640, 480)),
             Decimal('1.33')
         )
@@ -42,16 +46,18 @@
         self.assertEqual(scale_size((640, 480), (None, 3)), (4, 3))
 
 
 class TestImageWidget(YafowilTestCase):
 
     def setUp(self):
         super(TestImageWidget, self).setUp()
+        from yafowil.widget import image
         from yafowil.widget.image import widget
         reload(widget)
+        image.register()
 
     def dummy_file_data(self, filename):
         path = pkg_resources.resource_filename(
             'yafowil.widget.image', 'testing/%s' % filename)
         with open(path, 'rb') as file:
             data = file.read()
         return data
@@ -85,15 +91,15 @@
         form = factory(
             'form',
             name='myform',
             props={
                 'action': 'myaction'
             })
         form['image'] = factory('image')
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <input accept="image/*" class="image" id="input-myform-image"
                  name="myform.image" type="file"/>
         </form>
         """, fxml(form()))
 
@@ -107,15 +113,15 @@
             })
         form['image'] = factory(
             'image',
             value={
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             })
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <input accept="image/*" class="image" id="input-myform-image"
                  name="myform.image" type="file"/>
           <div id="radio-myform-image-keep">
             <input checked="checked" class="image" id="input-myform-image-keep"
                    name="myform.image-action" type="radio" value="keep"/>
@@ -149,15 +155,15 @@
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             },
             props={
                 'src': 'http://www.example.com/someimage.png',
                 'alt': 'Alternative text'
             })
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <img alt="Alternative text" class="image-preview"
                id="image-preview-myform-image"
                src="http://www.example.com/someimage.png?nocache=..."/>
           <input accept="image/*" class="image" id="input-myform-image"
                  name="myform.image" type="file"/>
@@ -179,15 +185,15 @@
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             },
             props={
                 'src': 'http://www.example.com/someimage?format=png',
                 'alt': 'Alternative text'
             })
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <img alt="Alternative text" class="image-preview"
                id="image-preview-myform-image"
                src="http://www.example.com/someimage?format=png&amp;nocache=..."/>
           <input accept="image/*" class="image" id="input-myform-image"
                  name="myform.image" type="file"/>
@@ -209,15 +215,15 @@
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             },
             props={
                 'src': lambda w, d: 'http://www.example.com/otherimage.png',
                 'alt': 'Alternative text'
             })
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <img alt="Alternative text" class="image-preview"
                id="image-preview-myform-image"
                src="http://www.example.com/otherimage.png?nocache=..."/>
           <input accept="image/*" class="image" id="input-myform-image"
                  name="myform.image" type="file"/>
@@ -240,25 +246,25 @@
                 'mimetype': 'image/png'
             },
             props={
                 'src': 'http://www.example.com/someimage.png',
                 'alt': 'Alternative text'
             },
             mode='display')
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <img alt="Alternative text"
                src="http://www.example.com/someimage.png"/>
         </form>
         """, fxml(form()))
 
         # Rendering is skipped if no source
         form['image'].attrs['src'] = None
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data"
               id="form-myform" method="post" novalidate="novalidate"/>
         """, fxml(form()))
 
     def test_extract_empty(self):
         # Extract empty (submitted but no upload)
         image = factory(
@@ -278,15 +284,15 @@
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         })
         self.assertEqual(data.errors, [])
         self.assertEqual(data.value, UNSET)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
 
     def test_extract_keep(self):
@@ -302,21 +308,21 @@
             'image': {
                 'file': StringIO(self.dummy_jpg),
                 'mimetype': 'image/jpg'
             },
             'image-action': 'keep'
         })
         self.assertEqual(data.errors, [])
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'keep'),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.value.items())))
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'keep'),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         extracted = data.extracted['file'].read()
         self.assertTrue(extracted.startswith(b'\x89PNG\r\n'))
@@ -335,20 +341,20 @@
             'image': {
                 'file': StringIO(self.dummy_jpg),
                 'mimetype': 'image/jpg'
             },
             'image-action': 'replace'
         })
         self.assertEqual(data.errors, [])
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'replace'),
         ('file', <... at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.value.items())))
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'replace'),
         ('file', <... at ...>),
         ('image', <PIL.JpegImagePlugin.JpegImageFile image mode=RGB size=50x50 at ...>),
         ('mimetype', 'image/jpg')]
         """, str(sorted(data.extracted.items())))
         extracted = data.extracted['file'].read()
         self.assertTrue(extracted.startswith(b'\xff\xd8\xff\xe0\x00\x10JFIF'))
@@ -367,20 +373,20 @@
             'image': {
                 'file': StringIO(self.dummy_jpg),
                 'mimetype': 'image/jpg'
             },
             'image-action': 'delete'
         })
         self.assertEqual(data.errors, [])
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'delete'),
         ('file', <UNSET>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.value.items())))
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'delete'),
         ('file', <UNSET>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
 
     def test_extract_mimetype_empty(self):
         # Image ``accept`` might be undefined.
@@ -392,15 +398,15 @@
             })
         data = image.extract({
             'image': {
                 'file': StringIO(self.dummy_jpg),
                 'mimetype': 'image/jpg'
             }
         })
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('file', <... at ...>),
         ('image', <PIL.JpegImagePlugin.JpegImageFile image mode=RGB size=50x50 at ...),
         ('mimetype', 'image/jpg')]
         """, str(sorted(data.extracted.items())))
 
     def test_extract_mimetype_incompatible(self):
@@ -413,20 +419,17 @@
             })
         request = {
             'image': {
                 'file': StringIO(self.dummy_jpg),
                 'mimetype': 'image/jpg'
             }
         }
-        err = self.expect_error(
-            ValueError,
-            image.extract,
-            request
-        )
-        self.assertEqual(str(err), 'Incompatible mimetype text/*')
+        with self.assertRaises(ValueError) as arc:
+            image.extract(request)
+        self.assertEqual(str(arc.exception), 'Incompatible mimetype text/*')
 
     def test_extract_mimetype_wrong_type(self):
         image = factory(
             'image',
             name='image',
             props={
                 'accept': 'image/png'
@@ -451,15 +454,15 @@
             })
         data = image.extract({
             'image': {
                 'file': StringIO(self.dummy_jpg),
                 'mimetype': 'image/jpg'
             }
         })
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('file', <... at ...>),
         ('image', <PIL.JpegImagePlugin.JpegImageFile image mode=RGB size=50x50 at ...>),
         ('mimetype', 'image/jpg')]
         """, str(sorted(data.extracted.items())))
 
     def test_extract_mimtype_not_image(self):
@@ -480,15 +483,15 @@
             data.errors,
             [ExtractionError('Uploaded file is not an image.')]
         )
 
     def test_extract_from_image_foundations(self):
         buffer = StringIO(self.dummy_png)
         image = PIL.Image.open(buffer)
-        self.check_output("""
+        self.checkOutput("""
         <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>
         """, str(image))
         buffer.seek(0)
         data = buffer.read()
         self.assertTrue(data.startswith(b'\x89PNG\r\n'))
         self.assertTrue(data.endswith(b'\xaeB`\x82'))
         self.assertEqual(image.size, (50, 50))
@@ -684,21 +687,21 @@
         data = image.extract(request)
         self.assertEqual(
             sorted(data.extracted.keys()),
             ['action', 'file', 'image', 'mimetype', 'scales']
         )
         self.assertEqual(data.extracted['action'], 'new')
         self.assertEqual(data.extracted['mimetype'], 'image/png')
-        self.check_output("""
+        self.checkOutput("""
         <... at ...>
         """, str(data.extracted['file']))
-        self.check_output("""
+        self.checkOutput("""
         <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>
         """, str(data.extracted['image']))
-        self.check_output("""
+        self.checkOutput("""
         [('landscape', <PIL.Image.Image image mode=RGBA size=40x40 at ...>),
         ('micro', <PIL.Image.Image image mode=RGBA size=20x20 at ...>),
         ('portrait', <PIL.Image.Image image mode=RGBA size=40x40 at ...>)]
         """, str(sorted(data.extracted['scales'].items())))
         # save images to testing folder for manual inspection
         for name, image in data.extracted['scales'].items():
             path = pkg_resources.resource_filename(
@@ -766,15 +769,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=20x20 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -795,15 +798,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=40x20 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -828,15 +831,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=20x40 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -862,15 +865,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=20x40 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -892,15 +895,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=50x20 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -927,15 +930,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_file_data('crop_size_40_20.png')),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=30x18 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=40x20 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -962,15 +965,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_file_data('crop_size_40_20.png')),
                 'mimetype': 'image/png'
             },
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=18x30 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=40x20 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -997,15 +1000,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_file_data('crop_size_20_40.png')),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=30x18 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=20x40 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -1032,15 +1035,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_file_data('crop_size_20_40.png')),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=18x30 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=20x40 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -1062,15 +1065,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=30x30 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -1092,15 +1095,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=40x50 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -1122,15 +1125,15 @@
         request = {
             'image': {
                 'file': StringIO(self.dummy_png),
                 'mimetype': 'image/png'
             }
         }
         data = image.extract(request)
-        self.check_output("""
+        self.checkOutput("""
         [('action', 'new'),
         ('cropped', <PIL.Image.Image image mode=RGBA size=48x40 at ...>),
         ('file', <... at ...>),
         ('image', <PIL.PngImagePlugin.PngImageFile image mode=RGBA size=50x50 at ...>),
         ('mimetype', 'image/png')]
         """, str(sorted(data.extracted.items())))
         # save cropped image to testing folder for manual inspection
@@ -1145,10 +1148,33 @@
         out = StringIO()
         image.save(out, 'png', quality=100)
         out.seek(0)
         data = out.read()
         self.assertTrue(data.startswith(b'\x89PNG\r\n'))
         self.assertTrue(data.endswith(b'\x00IEND\xaeB`\x82'))
 
+    def test_resources(self):
+        factory.theme = 'default'
+        resources = factory.get_resources('yafowil.widget.image')
+        self.assertTrue(resources.directory.endswith(np('/image/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.image')
+        self.assertEqual(resources.path, 'yafowil-image')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/image/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-image')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(styles[0].directory.endswith(np('/image/resources')))
+        self.assertEqual(styles[0].path, 'yafowil-image')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/utils.py` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/utils.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil/widget/image/widget.py` & `yafowil.widget.image-2.0a1/src/yafowil/widget/image/widget.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-1.6/src/yafowil.widget.image.egg-info/SOURCES.txt` & `yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
-setup.cfg
 setup.py
 src/yafowil/__init__.py
 src/yafowil.widget.image.egg-info/PKG-INFO
 src/yafowil.widget.image.egg-info/SOURCES.txt
 src/yafowil.widget.image.egg-info/dependency_links.txt
 src/yafowil.widget.image.egg-info/entry_points.txt
 src/yafowil.widget.image.egg-info/namespace_packages.txt
@@ -23,11 +22,12 @@
 src/yafowil/widget/image/locales/yafowil.widget.image.pot
 src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo
 src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po
 src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo
 src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po
 src/yafowil/widget/image/resources/widget.css
 src/yafowil/widget/image/resources/widget.js
+src/yafowil/widget/image/resources/widget.min.js
 src/yafowil/widget/image/testing/__init__.py
 src/yafowil/widget/image/testing/dummy.jpg
 src/yafowil/widget/image/testing/dummy.pdf
 src/yafowil/widget/image/testing/dummy.png
```

