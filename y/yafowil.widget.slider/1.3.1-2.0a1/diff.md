# Comparing `tmp/yafowil.widget.slider-1.3.1.tar.gz` & `tmp/yafowil.widget.slider-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yafowil.widget.slider-1.3.1.tar", last modified: Sat May 30 14:17:14 2020, max compression
+gzip compressed data, was "yafowil.widget.slider-2.0a1.tar", last modified: Mon May 15 12:53:57 2023, max compression
```

## Comparing `yafowil.widget.slider-1.3.1.tar` & `yafowil.widget.slider-2.0a1.tar`

### file list

```diff
@@ -1,35 +1,31 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1751 2020-05-30 14:15:52.000000 yafowil.widget.slider-1.3.1/setup.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1537 2020-05-30 14:16:50.000000 yafowil.widget.slider-1.3.1/LICENSE.rst
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       48 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/requires.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)        8 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/top_level.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       23 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/namespace_packages.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)        1 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/dependency_links.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)      112 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/entry_points.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     1055 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/SOURCES.txt
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     4190 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/PKG-INFO
--rw-rw-r--   0 rnix      (1000) rnix      (1000)        1 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/not-zip-safe
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     5952 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/widget.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9052 2018-06-20 20:40:14.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/tests.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/resources/
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     2395 2016-07-14 12:05:58.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/resources/jquery.ui.slider.plone5.css
--rw-rw-r--   0 rnix      (1000) rnix      (1000)    10202 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/resources/jquery.ui.slider.min.js
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     2395 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/resources/jquery.ui.slider.bootstrap.css
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     1314 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/resources/jquery.ui.slider.css
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     3635 2020-05-06 06:17:10.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/resources/widget.js
--rw-rw-r--   0 rnix      (1000) rnix      (1000)    18135 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/resources/jquery.ui.slider.js
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       47 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/resources/widget.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1530 2018-06-20 20:40:14.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/__init__.py
--rw-rw-r--   0 rnix      (1000) rnix      (1000)     5521 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/example.py
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       56 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/widget/__init__.py
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       56 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/src/yafowil/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/setup.cfg
--rw-rw-r--   0 rnix      (1000) rnix      (1000)       72 2015-12-13 18:41:49.000000 yafowil.widget.slider-1.3.1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)      603 2020-05-30 14:16:03.000000 yafowil.widget.slider-1.3.1/HISTORY.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4190 2020-05-30 14:17:14.000000 yafowil.widget.slider-1.3.1/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      558 2018-06-20 20:40:14.000000 yafowil.widget.slider-1.3.1/README.rst
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:53:57.532914 yafowil.widget.slider-2.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      905 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3742 2023-05-15 12:53:57.532914 yafowil.widget.slider-2.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      691 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:53:57.532914 yafowil.widget.slider-2.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1725 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:53:57.528914 yafowil.widget.slider-2.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:53:57.532914 yafowil.widget.slider-2.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:53:57.532914 yafowil.widget.slider-2.0a1/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:53:57.532914 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1576 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9078 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:53:57.532914 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/resources/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1230 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/resources/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18206 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7972 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/resources/widget.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10665 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6436 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:53:57.532914 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3742 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      801 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      111 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:53:57.000000 yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yafowil.widget.slider-1.3.1/LICENSE.rst` & `yafowil.widget.slider-2.0a1/LICENSE.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-
 License
 =======
 
-Copyright (c) 2013-2020, BlueDynamics Alliance, Austria, Germany, Switzerland
+Copyright (c) 2013-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
+Copyright (c) 2021-2022, Yafowil Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this 
+* Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
-* Redistributions in binary form must reproduce the above copyright notice, this 
-  list of conditions and the following disclaimer in the documentation and/or 
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
   other materials provided with the distribution.
-* Neither the name of the BlueDynamics Alliance nor the names of its 
-  contributors may be used to endorse or promote products derived from this 
-  software without specific prior written permission.
-      
-THIS SOFTWARE IS PROVIDED BY BlueDynamics Alliance ``AS IS`` AND ANY
-EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL BlueDynamics Alliance BE LIABLE FOR ANY
-DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `yafowil.widget.slider-1.3.1/src/yafowil.widget.slider.egg-info/SOURCES.txt` & `yafowil.widget.slider-2.0a1/src/yafowil.widget.slider.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-HISTORY.rst
+CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.py
 src/yafowil/__init__.py
 src/yafowil.widget.slider.egg-info/PKG-INFO
 src/yafowil.widget.slider.egg-info/SOURCES.txt
@@ -13,14 +13,10 @@
 src/yafowil.widget.slider.egg-info/requires.txt
 src/yafowil.widget.slider.egg-info/top_level.txt
 src/yafowil/widget/__init__.py
 src/yafowil/widget/slider/__init__.py
 src/yafowil/widget/slider/example.py
 src/yafowil/widget/slider/tests.py
 src/yafowil/widget/slider/widget.py
-src/yafowil/widget/slider/resources/jquery.ui.slider.bootstrap.css
-src/yafowil/widget/slider/resources/jquery.ui.slider.css
-src/yafowil/widget/slider/resources/jquery.ui.slider.js
-src/yafowil/widget/slider/resources/jquery.ui.slider.min.js
-src/yafowil/widget/slider/resources/jquery.ui.slider.plone5.css
 src/yafowil/widget/slider/resources/widget.css
-src/yafowil/widget/slider/resources/widget.js
+src/yafowil/widget/slider/resources/widget.js
+src/yafowil/widget/slider/resources/widget.min.js
```

### Comparing `yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/widget.py` & `yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/widget.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,15 +33,27 @@
     if widget.dottedpath in data.request:
         val = data.request[widget.dottedpath]
         if val:
             return int(val)
     return UNSET
 
 
-js_options = ['orientation', 'range', 'min', 'max', 'step', 'slide', 'change']
+js_options = [
+    'orientation',
+    'range',
+    'min',
+    'max',
+    'step',
+    'scroll_step',
+    'thickness',
+    'handle_diameter',
+    'slide',
+    'change'
+]
+
 
 @managedprops(*['show_value', 'unit', 'height', 'data'] + js_options)
 def slider_edit_renderer(widget, data):
     value = fetch_value(widget, data)
     content = ''
     range = attr_value('range', widget, data)
     if range is True:
@@ -109,71 +121,86 @@
 
 factory.register(
     'slider',
     extractors=[slider_extractor],
     edit_renderers=[slider_edit_renderer],
     display_renderers=[slider_display_renderer])
 
-factory.doc['blueprint']['slider'] = \
-"""Add-on blueprint `yafowil.widget.slider
-<http://github.com/bluedynamics/yafowil.widget.slider/>`_ .
+factory.doc['blueprint']['slider'] = """\
+Add-on blueprint `yafowil.widget.slider
+<http://github.com/conestack/yafowil.widget.slider/>`_ .
 """
 
 factory.defaults['slider.default'] = ''
 
 factory.defaults['slider.class'] = 'yafowil_slider'
 
 factory.defaults['slider.show_value'] = False
-factory.doc['props']['slider.show_value'] = \
-"""Show value in addition to slider.
+factory.doc['props']['slider.show_value'] = """\
+Show value in addition to slider.
 """
 
 factory.defaults['slider.unit'] = ''
-factory.doc['props']['slider.unit'] = \
-"""Slider value unit.
+factory.doc['props']['slider.unit'] = """\
+Slider value unit.
 """
 
 factory.defaults['slider.orientation'] = None
-factory.doc['props']['slider.orientation'] = \
-"""Slider Orientation. Either ``horizontal`` or ``vertical``.
+factory.doc['props']['slider.orientation'] = """\
+Slider Orientation. Either ``horizontal`` or ``vertical``.
 """
 
 factory.defaults['slider.height'] = None
-factory.doc['props']['slider.height'] = \
-"""Height of slider if orientation is ``vertical`` in pixel.
+factory.doc['props']['slider.height'] = """\
+Height of slider if orientation is ``vertical`` in pixel.
+"""
+
+factory.defaults['slider.handle_diameter'] = 20
+factory.doc['props']['slider.handle_diameter'] = """\
+Diameter of slider handle in pixel.
+"""
+
+factory.defaults['slider.thickness'] = 8
+factory.doc['props']['slider.thickness'] = """\
+Thickness of slider track in pixel.
 """
 
 factory.defaults['slider.range'] = None
-factory.doc['props']['slider.range'] = \
-"""Slider Range. Either ``True``, ``'min'`` or ``'max'``.
+factory.doc['props']['slider.range'] = """\
+Slider Range. Either ``True``, ``'min'`` or ``'max'``.
+"""
+
+factory.defaults['slider.min'] = 0
+factory.doc['props']['slider.min'] = """\
+Minimum slider value. Defaults to 0.
 """
 
-factory.defaults['slider.min'] = None
-factory.doc['props']['slider.min'] = \
-"""Minimum slider value. Defaults to 0.
+factory.defaults['slider.max'] = 100
+factory.doc['props']['slider.max'] = """\
+Maximum slider value value. Defaults to 100.
 """
 
-factory.defaults['slider.max'] = None
-factory.doc['props']['slider.max'] = \
-"""Maximum slider value value. Defaults to 100.
+factory.defaults['slider.step'] = 1
+factory.doc['props']['slider.step'] = """\
+Snap slider to increments.
 """
 
-factory.defaults['slider.step'] = None
-factory.doc['props']['slider.step'] = \
-"""Snap slider to increments.
+factory.defaults['slider.scroll_step'] = None
+factory.doc['props']['slider.scroll_step'] = """\
+Customize snapping on scroll.
 """
 
 factory.defaults['slider.slide'] = None
-factory.doc['props']['slider.slide'] = \
-"""Optional Javascript ``slide`` callback as string.
+factory.doc['props']['slider.slide'] = """\
+Optional Javascript ``slide`` callback as string.
 """
 
 factory.defaults['slider.change'] = None
-factory.doc['props']['slider.change'] = \
-"""Optional Javascript ``change`` callback as string.
+factory.doc['props']['slider.change'] = """\
+Optional Javascript ``change`` callback as string.
 """
 
 factory.defaults['slider.data'] = dict()
-factory.doc['props']['slider.data'] = \
-"""Additional data redered as HTML data attributes on slider wrapper
+factory.doc['props']['slider.data'] = """\
+Additional data redered as HTML data attributes on slider wrapper
 DOM Element.
 """
```

### Comparing `yafowil.widget.slider-1.3.1/src/yafowil/widget/slider/tests.py` & `yafowil.widget.slider-2.0a1/src/yafowil/widget/slider/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from node.utils import UNSET
-from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.compat import IS_PY2
-from yafowil.tests import YafowilTestCase
 from yafowil.tests import fxml
-import yafowil.loader
+from yafowil.tests import YafowilTestCase
+import os
+import unittest
 
 
 if not IS_PY2:
     from importlib import reload
 
 
+def np(path):
+    return path.replace('/', os.path.sep)
+
+
 class TestSliderWidget(YafowilTestCase):
 
     def setUp(self):
         super(TestSliderWidget, self).setUp()
+        from yafowil.widget import slider
         from yafowil.widget.slider import widget
         reload(widget)
+        slider.register()
 
     def test_render_no_range(self):
         # Render no range
         widget = factory(
             'slider',
             name='sliderfield')
-        self.check_output("""
-        <div class="yafowil_slider">
+        self.checkOutput("""
+        <div class="yafowil_slider" data-handle_diameter="20" data-max="100"
+             data-min="0" data-step="1" data-thickness="8">
           <input class="slider_value" id="input-sliderfield" name="sliderfield"
                  style="display:none;" type="text" value=""/>
           <div class="slider"> </div>
         </div>
         """, fxml(widget()))
 
     def test_extract_no_range(self):
@@ -51,16 +58,17 @@
 
     def test_render_no_range_preset_value(self):
         # Render no range, preset value
         widget = factory(
             'slider',
             name='sliderfield',
             value=3)
-        self.check_output("""
-        <div class="yafowil_slider">
+        self.checkOutput("""
+        <div class="yafowil_slider" data-handle_diameter="20" data-max="100"
+             data-min="0" data-step="1" data-thickness="8">
           <input class="slider_value" id="input-sliderfield" name="sliderfield"
                  style="display:none;" type="text" value="3"/>
           <div class="slider">
           </div>
         </div>
         """, fxml(widget()))
 
@@ -89,16 +97,17 @@
             'slider',
             name='sliderfield',
             value=20,
             props={
                 'show_value': True,
                 'unit': 'Unit'
             })
-        self.check_output("""
-        <div class="yafowil_slider">
+        self.checkOutput("""
+        <div class="yafowil_slider" data-handle_diameter="20" data-max="100"
+             data-min="0" data-step="1" data-thickness="8">
           <input class="slider_value" id="input-sliderfield" name="sliderfield"
                  style="display:none;" type="text" value="20"/>
           <span class="unit">Unit: </span>
           <span class="slider_value">20</span>
           <div class="slider"> </div>
         </div>
         """, fxml(widget()))
@@ -107,16 +116,17 @@
         # Render range
         widget = factory(
             'slider',
             name='sliderfield',
             props={
                 'range': True
             })
-        self.check_output("""
-        <div class="yafowil_slider" data-range="true">
+        self.checkOutput("""
+        <div class="yafowil_slider" data-handle_diameter="20" data-max="100"
+             data-min="0" data-range="true" data-step="1" data-thickness="8">
           <input class="lower_value" id="input-lower-sliderfield"
                  name="sliderfield.lower" style="display:none;"
                  type="text" value=""/>
           <input class="upper_value" id="input-upper-sliderfield"
                  name="sliderfield.upper" style="display:none;"
                  type="text" value=""/>
           <div class="slider">
@@ -156,16 +166,17 @@
         widget = factory(
             'slider',
             name='sliderfield',
             value=[2, 4],
             props={
                 'range': True
             })
-        self.check_output("""
-        <div class="yafowil_slider" data-range="true">
+        self.checkOutput("""
+        <div class="yafowil_slider" data-handle_diameter="20" data-max="100"
+             data-min="0" data-range="true" data-step="1" data-thickness="8">
           <input class="lower_value" id="input-lower-sliderfield"
                  name="sliderfield.lower" style="display:none;"
                  type="text" value="2"/>
           <input class="upper_value" id="input-upper-sliderfield"
                  name="sliderfield.upper" style="display:none;"
                  type="text" value="4"/>
           <div class="slider"> </div>
@@ -218,21 +229,23 @@
                 'slide': 'some_ns.some_callback',
                 'change': 'some_ns.some_callback',
                 'data': {'mydata': 1}
             })
         self.assertEqual(widget(), (
             '<div class="yafowil_slider" '
             'data-change=\'some_ns.some_callback\' '
+            'data-handle_diameter=\'20\' '
             'data-max=\'50\' '
             'data-min=\'1\' '
             'data-mydata=\'1\' '
             'data-orientation=\'vertical\' '
             'data-range=\'true\' '
             'data-slide=\'some_ns.some_callback\' '
-            'data-step=\'5\'><input '
+            'data-step=\'5\' '
+            'data-thickness=\'8\'><input '
             'class="lower_value" '
             'id="input-lower-sliderfield" '
             'name="sliderfield.lower" '
             'style="display:none;" '
             'type="text" '
             'value="2" /><input '
             'class="upper_value" '
@@ -250,32 +263,51 @@
 
     def test_render_display_mode(self):
         # Render display mode, fails
         widget = factory(
             'slider',
             name='sliderfield',
             mode='display')
-        err = self.expect_error(
-            NotImplementedError,
-            widget
-        )
+        with self.assertRaises(NotImplementedError) as arc:
+            widget()
         msg = '``yafowil.widget.slider`` does not support display mode yet'
-        self.assertEqual(str(err), msg)
+        self.assertEqual(str(arc.exception), msg)
 
     def test_reserved_data_attribute(self):
         # Render reserved data attribute, fails
         widget = factory(
             'slider',
             name='sliderfield',
             props={
                 'data': {'min': 1}
             })
-        err = self.expect_error(
-            ValueError,
-            widget
-        )
+        with self.assertRaises(ValueError) as arc:
+            widget()
         msg = "Additional data dict contains reserved attribute name 'min'"
-        self.assertEqual(str(err), msg)
+        self.assertEqual(str(arc.exception), msg)
+
+    def test_resources(self):
+        factory.theme = 'default'
+        resources = factory.get_resources('yafowil.widget.slider')
+        self.assertTrue(resources.directory.endswith(np('/slider/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.slider')
+        self.assertEqual(resources.path, 'yafowil-slider')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/slider/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-slider')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(styles[0].directory.endswith(np('/slider/resources')))
+        self.assertEqual(styles[0].path, 'yafowil-slider')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
 
 
 if __name__ == '__main__':
-    unittest.main()                                          # pragma: no cover
+    unittest.main()
```

