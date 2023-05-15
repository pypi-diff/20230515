# Comparing `tmp/yafowil.widget.array-1.7.tar.gz` & `tmp/yafowil.widget.array-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yafowil.widget.array-1.7.tar", last modified: Thu Oct  6 07:52:10 2022, max compression
+gzip compressed data, was "yafowil.widget.array-2.0a1.tar", last modified: Mon May 15 12:34:07 2023, max compression
```

## Comparing `yafowil.widget.array-1.7.tar` & `yafowil.widget.array-2.0a1.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      299 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/.jshintrc
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2242 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1398 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      124 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6392 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      553 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5689 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/bootstrap.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      672 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/buildout.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1694 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil/widget/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1083 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11140 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/example.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/bootstrap/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1220 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/bootstrap/widget.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      403 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/icon_add.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      584 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/icon_down.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      392 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/icon_down_disabled.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      221 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/icon_remove.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      560 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/icon_up.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      382 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/icon_up_disabled.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1517 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/widget.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/plone5/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1844 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/plone5/widget.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9077 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/resources/widget.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    80343 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10140 2022-10-06 07:52:09.000000 yafowil.widget.array-1.7/src/yafowil/widget/array/widget.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6392 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1299 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      126 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       48 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2022-10-06 07:52:10.000000 yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2498 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      124 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5214 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      573 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-05-15 12:34:07.540385 yafowil.widget.array-2.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1719 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil/widget/array/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4203 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11140 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/bootstrap/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1361 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/bootstrap/widget.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      403 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/icon_add.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      584 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/icon_down.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      392 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/icon_down_disabled.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      221 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/icon_remove.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      560 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/icon_up.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      382 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/icon_up_disabled.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1536 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/widget.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/plone5/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1880 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/plone5/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9161 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4362 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/widget.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    83506 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10208 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil/widget/array/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:34:07.536385 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5214 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1312 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      109 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:34:07.000000 yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yafowil.widget.array-1.7/CHANGES.rst` & `yafowil.widget.array-2.0a1/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Changes
 =======
 
+2.0a1 (2023-05-15)
+------------------
+
+- Add ``webresource`` support.
+  [rnix]
+
+- Add ``inside_template`` JS utility function.
+  [rnix]
+
+- ``array.hooks`` are deprecated. Use ``on_array_event`` instead.
+  [rnix]
+
+- Rewrite JavaScript using ES6.
+  [rnix]
+
+
 1.7 (2022-10-06)
 ----------------
 
 - Introduce new method ``set_value_index`` to allow correct custom indexing
   in index hooks.
   [lenadax]
```

### Comparing `yafowil.widget.array-1.7/LICENSE.rst` & `yafowil.widget.array-2.0a1/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 License
 =======
 
 Copyright (c) 2011-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
-Copyright (c) 2021, Yafowil Contributors
+Copyright (c) 2021-2022, Yafowil Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `yafowil.widget.array-1.7/README.rst` & `yafowil.widget.array-2.0a1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 Contributors
 ============
 
 - Robert Niederreiter
 
 - Georg Bernhard
 
+- Lena Daxenbichler
```

### Comparing `yafowil.widget.array-1.7/setup.py` & `yafowil.widget.array-2.0a1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.7'
+version = '2.0a1'
 shortdesc = 'Array Widget for YAFOWIL'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
-tests_require = ['yafowil[test]']
 
 
 setup(
     name='yafowil.widget.array',
     version=version,
     description=shortdesc,
     long_description=longdesc,
@@ -44,18 +43,22 @@
     namespace_packages=['yafowil', 'yafowil.widget'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
         'yafowil>2.1.99',
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
     test_suite="yafowil.widget.array.tests",
     entry_points="""
     [yafowil.plugin]
     register = yafowil.widget.array:register
     example = yafowil.widget.array.example:get_example
     """
 )
```

### Comparing `yafowil.widget.array-1.7/src/yafowil/widget/array/example.py` & `yafowil.widget.array-2.0a1/src/yafowil/widget/array/example.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/icon_down.png` & `yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/icon_down.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.array-1.7/src/yafowil/widget/array/resources/default/images/icon_up.png` & `yafowil.widget.array-2.0a1/src/yafowil/widget/array/resources/default/images/icon_up.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.array-1.7/src/yafowil/widget/array/tests.py` & `yafowil.widget.array-2.0a1/src/yafowil/widget/array/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from node.utils import UNSET
 from odict import odict
 from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.compat import IS_PY2
 from yafowil.tests import fxml
 from yafowil.tests import YafowilTestCase
+import os
 import unittest
-import yafowil.loader  # noqa
 
 
 if not IS_PY2:
     from importlib import reload
 
 
+def np(path):
+    return path.replace('/', os.path.sep)
+
+
 class TestArrayWidget(YafowilTestCase):
 
     def setUp(self):
         super(TestArrayWidget, self).setUp()
+        from yafowil.widget import array
         from yafowil.widget.array import widget
         reload(widget)
+        array.register()
 
     def test_array_with_missing_entry_definition(self):
         form = factory(
             'form',
             name='myform',
             props={'action': 'myaction'})
         form['myarray'] = factory(
             'array',
             props={'label': 'My Array'})
-        err = self.expect_error(
-            Exception,
-            form
-        )
+        with self.assertRaises(Exception) as arc:
+            form()
         msg = 'Empty array widget defined'
-        self.assertEqual(str(err), msg)
+        self.assertEqual(str(arc.exception), msg)
 
     def test_empty_array(self):
         # Create empty array widget
         form = factory(
             'form',
             name='myform',
             props={'action': 'myaction'})
@@ -57,15 +61,15 @@
             "          <class 'yafowil.base.Widget'>: label",
             "          <class 'yafowil.base.Widget'>: actions",
             "      <class 'yafowil.base.Widget'>: body",
             "    <class 'yafowil.base.Widget'>: myfield",
             ""
         ])
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data"
               id="form-myform" method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
@@ -116,15 +120,15 @@
             "          <class 'yafowil.base.Widget'>: label",
             "          <class 'yafowil.base.Widget'>: actions",
             "      <class 'yafowil.base.Widget'>: body",
             "    <class 'yafowil.base.Widget'>: myfield",
             ""
         ])
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-remove array-sort" id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
                   <th>My Array</th>
@@ -151,15 +155,15 @@
             props={
                 'label': 'My Array',
                 'class': 'specialclass',
             })
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array specialclass array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               ...
             </table>
@@ -183,15 +187,15 @@
                 'label': 'My Array',
                 'class': 'specialclass',
             },
             mode='display')
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <table>
             <thead>
               <tr>
                 <th>My Array</th>
               </tr>
@@ -241,15 +245,15 @@
             "        <class 'yafowil.base.Widget'>: row",
             "          <class 'yafowil.base.Widget'>: label",
             "      <class 'yafowil.base.Widget'>: body",
             "    <class 'yafowil.base.Widget'>: myfield",
             ""
         ])
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-static" id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
                   <th>My Array</th>
@@ -271,20 +275,18 @@
         form['myarray'] = factory(
             'array',
             props={'label': 'My Compound Array'})
         form['myarray']['mycompound'] = factory(
             'compound',
             props={'structural': True})
 
-        err = self.expect_error(
-            Exception,
-            form
-        )
+        with self.assertRaises(Exception) as arc:
+            form()
         msg = 'Compound templates for arrays must not be structural.'
-        self.assertEqual(str(err), msg)
+        self.assertEqual(str(arc.exception), msg)
 
         # Now with valid compound template
         form['myarray'] = factory(
             'array',
             props={'label': 'My Compound Array'})
         form['myarray']['mycompound'] = factory('compound')
         form['myarray']['mycompound']['f1'] = factory(
@@ -305,15 +307,15 @@
             "      <class 'yafowil.base.Widget'>: body",
             "    <class 'yafowil.base.Widget'>: mycompound",
             "      <class 'yafowil.base.Widget'>: f1",
             "      <class 'yafowil.base.Widget'>: f2",
             ""
         ])
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               ...
             </table>
@@ -364,15 +366,15 @@
             "            <class 'yafowil.base.Widget'>: label",
             "            <class 'yafowil.base.Widget'>: actions",
             "        <class 'yafowil.base.Widget'>: body",
             "      <class 'yafowil.base.Widget'>: myfield",
             ""
         ])
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarrayarray">
             <table>
             ...
             </table>
@@ -406,23 +408,22 @@
             'array',
             value=object(),
             props={'label': 'My Array'})
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
 
-        err = self.expect_error(
-            ValueError,
-            form
-        )
-        if IS_PY2:
-            msg = "Expected list or dict as value. Got '<type 'object'>'"
-        else:
-            msg = "Expected list or dict as value. Got '<class 'object'>'"
-        self.assertEqual(str(err), msg)
+        with self.assertRaises(ValueError) as arc:
+            form()
+        msg = (
+            "Expected list or dict as value. Got '<type 'object'>'"
+            if IS_PY2
+            else "Expected list or dict as value. Got '<class 'object'>'"
+        )
+        self.assertEqual(str(arc.exception), msg)
 
     def test_array_with_preset_values_disable_add_action(self):
         # Value as list. Disable ``add``
         form = factory(
             'form',
             name='myform',
             props={'action': 'myaction'})
@@ -433,15 +434,15 @@
                 'label': 'My Array',
                 'add': False,
             })
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-remove array-sort" id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
                   <th>My Array</th>
@@ -495,15 +496,15 @@
                 'label': 'My Array',
                 'sort': False,
             })
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove" id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
                   <th>My Array</th>
@@ -559,15 +560,15 @@
                 'remove': False,
                 'sort': False,
             })
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array" id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
                   <th>My Array</th>
@@ -622,15 +623,15 @@
             "        <class 'yafowil.base.Widget'>: row",
             "          <class 'yafowil.base.Widget'>: label",
             "      <class 'yafowil.base.Widget'>: body",
             "    <class 'yafowil.base.Widget'>: myfield",
             ""
         ])
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-static" id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
                   <th>My Array</th>
@@ -670,15 +671,15 @@
             'array',
             value=['1', '2'],
             props={'label': 'My Array'})
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               <thead>
                 ...
@@ -742,20 +743,18 @@
             'array',
             value=value,
             props={'label': 'My Array'})
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
 
-        err = self.expect_error(
-            Exception,
-            form
-        )
+        with self.assertRaises(Exception) as arc:
+            form()
         msg = "Array value error. invalid literal for int() with base 10: 'a'"
-        self.assertEqual(str(err), msg)
+        self.assertEqual(str(arc.exception), msg)
 
     def test_array_with_preset_value_as_dict(self):
         # Valid dict value
         form = factory(
             'form',
             name='myform',
             props={'action': 'myaction'})
@@ -766,15 +765,15 @@
             'array',
             value=value,
             props={'label': 'My Array'})
         form['myarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               <thead>
                 ...
@@ -826,15 +825,15 @@
         form['myarray']['mycompound']['f1'] = factory(
             'field:label:text',
             props={'label': 'F1'})
         form['myarray']['mycompound']['f2'] = factory(
             'field:label:text',
             props={'label': 'F2'})
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               <thead>
                 ...
@@ -903,15 +902,15 @@
         form['myarray']['subarray'] = factory(
             'array',
             props={'label': 'Subrray'})
         form['myarray']['subarray']['myfield'] = factory(
             'field:label:text',
             props={'label': 'My Field'})
         rendered = form()
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               <thead>
                 ...
@@ -1104,15 +1103,15 @@
             "      <class 'yafowil.base.Widget'>: compoundinsub",
             "        <class 'yafowil.base.Widget'>: f1",
             "        <class 'yafowil.base.Widget'>: f2",
             ""
         ])
 
         rendered = form()
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
@@ -1475,15 +1474,15 @@
                 'myarray',
                 ['4', '3', '2', '1'],
                 [],
                 [ExtractionError('Array is required')]
             ]
         )
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform" method="post" novalidate="novalidate">
           <div class="error">
             <div class="errormessage">Array is required</div>
             <div class="array error array-add array-remove array-sort" id="array-myform-myarray">
               ...
             </div>
           </div>
@@ -1526,15 +1525,15 @@
         )
         arrd1 = data['myarray']['1']
         self.assertEqual(
             [arrd1.name, arrd1.value, arrd1.extracted, arrd1.errors],
             ['1', UNSET, '', [ExtractionError('My Field is required')]]
         )
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               ...
               <tbody>
@@ -1859,15 +1858,15 @@
         form['myarray']['mycompound']['f1'] = factory(
             'field:label:text',
             props={'label': 'F1'},
             mode='display')
         form['myarray']['mycompound']['f2'] = factory(
             'field:label:text',
             props={'label': 'F2', 'disabled': 'disabled'})
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               ...
                   <td class="widget">
@@ -1904,15 +1903,15 @@
         form['myarray'] = factory(
             'array',
             props={'label': lambda: 'Callable label'})
         form['myarray']['f1'] = factory(
             'field:label:text',
             props={'label': 'F1'},
             mode='display')
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-myarray">
             <table>
               <thead>
                 <tr>
@@ -1979,15 +1978,15 @@
             "              <class 'yafowil.base.Widget'>: label",
             "              <class 'yafowil.base.Widget'>: actions",
             "          <class 'yafowil.base.Widget'>: body",
             "        <class 'yafowil.base.Widget'>: textfield",
             ""
         ])
 
-        self.check_output("""
+        self.checkOutput("""
         <form action="myaction" enctype="multipart/form-data" id="form-myform"
               method="post" novalidate="novalidate">
           <div class="array array-add array-remove array-sort"
                id="array-myform-array_1">
             <table>
               <thead>
                 <tr>
@@ -2127,10 +2126,83 @@
                 </div>
               </div>
             </div>
           </div>
         </form>
         """, fxml(form()))
 
+    def test_resources(self):
+        factory.theme = 'default'
+        resources = factory.get_resources('yafowil.widget.array')
+        self.assertTrue(resources.directory.endswith(np('/array/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.array')
+        self.assertEqual(resources.path, 'yafowil-array')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/array/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-array')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(
+            styles[0].directory.endswith(np('/array/resources/default'))
+        )
+        self.assertEqual(styles[0].path, 'yafowil-array/default')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
+        factory.theme = 'bootstrap3'
+        resources = factory.get_resources('yafowil.widget.array')
+        self.assertTrue(resources.directory.endswith(np('/array/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.array')
+        self.assertEqual(resources.path, 'yafowil-array')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/array/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-array')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(
+            styles[0].directory.endswith(np('/array/resources/bootstrap'))
+        )
+        self.assertEqual(styles[0].path, 'yafowil-array/bootstrap')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
+        factory.theme = 'plone5'
+        resources = factory.get_resources('yafowil.widget.array')
+        self.assertTrue(resources.directory.endswith(np('/array/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.array')
+        self.assertEqual(resources.path, 'yafowil-array')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/array/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-array')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(
+            styles[0].directory.endswith(np('/array/resources/plone5'))
+        )
+        self.assertEqual(styles[0].path, 'yafowil-array/plone5')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
 
 if __name__ == '__main__':
     unittest.main()                                          # pragma: no cover
```

### Comparing `yafowil.widget.array-1.7/src/yafowil/widget/array/widget.py` & `yafowil.widget.array-2.0a1/src/yafowil/widget/array/widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     return data.tag('input', **input_attrs) + data.rendered
 
 
 factory.register(
     'array_display_proxy',
     extractors=[generic_extractor],
     edit_renderers=[array_display_proxy_renderer],
-    display_renderers=[array_display_proxy_renderer])
+    display_renderers=[array_display_proxy_renderer]
+)
 
 # do not document internal widget
 factory.doc['blueprint']['array_display_proxy'] = UNSET
 
 
 ICON_CSS = {
     'add': 'icon-plus-sign',
@@ -56,15 +57,16 @@
             actions.append(action)
     kw = dict(class_='array_actions')
     return tag('div', *actions, **kw)
 
 
 factory.register(
     'array_actions',
-    edit_renderers=[actions_renderer])
+    edit_renderers=[actions_renderer]
+)
 
 # do not document internal widget
 factory.doc['blueprint']['array_actions'] = UNSET
 
 
 def array_builder(widget, factory):
     table = widget['table'] = factory('table', props={
@@ -272,19 +274,29 @@
         del row['actions_col']
     del widget[CONTAINER]
     set_display_mode(widget)
 
 
 factory.register(
     'array',
-    extractors=[array_extractor, generic_required_extractor],
+    extractors=[
+        array_extractor,
+        generic_required_extractor
+    ],
     edit_renderers=[
-        array_edit_renderer, compound_renderer, array_wrapper_renderer],
-    display_renderers=[array_display_renderer, compound_renderer],
-    builders=[array_builder])
+        array_edit_renderer,
+        compound_renderer,
+        array_wrapper_renderer
+    ],
+    display_renderers=[
+        array_display_renderer,
+        compound_renderer
+    ],
+    builders=[array_builder]
+)
 
 factory.doc['blueprint']['array'] = """\
 Add-on widget `yafowil.widget.array
 <http://github.com/conestack/yafowil.widget.array/>`_.
 """
 
 factory.defaults['array.class'] = 'array'
```

### Comparing `yafowil.widget.array-1.7/src/yafowil.widget.array.egg-info/SOURCES.txt` & `yafowil.widget.array-2.0a1/src/yafowil.widget.array.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-.jshintrc
 CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
-bootstrap.py
-buildout.cfg
 setup.cfg
 setup.py
 src/yafowil/__init__.py
 src/yafowil.widget.array.egg-info/PKG-INFO
 src/yafowil.widget.array.egg-info/SOURCES.txt
 src/yafowil.widget.array.egg-info/dependency_links.txt
 src/yafowil.widget.array.egg-info/entry_points.txt
@@ -18,14 +15,15 @@
 src/yafowil.widget.array.egg-info/top_level.txt
 src/yafowil/widget/__init__.py
 src/yafowil/widget/array/__init__.py
 src/yafowil/widget/array/example.py
 src/yafowil/widget/array/tests.py
 src/yafowil/widget/array/widget.py
 src/yafowil/widget/array/resources/widget.js
+src/yafowil/widget/array/resources/widget.min.js
 src/yafowil/widget/array/resources/bootstrap/widget.css
 src/yafowil/widget/array/resources/default/widget.css
 src/yafowil/widget/array/resources/default/images/icon_add.png
 src/yafowil/widget/array/resources/default/images/icon_down.png
 src/yafowil/widget/array/resources/default/images/icon_down_disabled.png
 src/yafowil/widget/array/resources/default/images/icon_remove.png
 src/yafowil/widget/array/resources/default/images/icon_up.png
```

