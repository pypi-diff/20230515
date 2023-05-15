# Comparing `tmp/yafowil.widget.cron-1.2.tar.gz` & `tmp/yafowil.widget.cron-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yafowil.widget.cron-1.2.tar", last modified: Sat May 30 14:11:40 2020, max compression
+gzip compressed data, was "yafowil.widget.cron-2.0a1.tar", last modified: Mon May 15 12:40:28 2023, max compression
```

## Comparing `yafowil.widget.cron-1.2.tar` & `yafowil.widget.cron-2.0a1.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1671 2020-05-30 14:10:54.000000 yafowil.widget.cron-1.2/setup.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1234 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/TODO.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1537 2020-05-12 17:26:55.000000 yafowil.widget.cron-1.2/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      717 2020-05-30 14:11:12.000000 yafowil.widget.cron-1.2/CHANGES.rst
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/widget/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6049 2020-05-12 17:19:45.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/widget.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1148 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)      637 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.mo
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1153 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)      641 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1080 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/yafowil.widget.cron.pot
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14632 2020-05-12 17:22:22.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/tests.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/resources/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    21138 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/resources/widget.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2173 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/resources/widget.less
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2755 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/resources/widget.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)      614 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1432 2020-05-12 14:04:26.000000 yafowil.widget.cron-1.2/src/yafowil/widget/cron/example.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)       80 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/widget/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)       80 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       53 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/top_level.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      124 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1114 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4259 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2020-04-29 09:54:01.000000 yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4259 2020-05-30 14:11:40.000000 yafowil.widget.cron-1.2/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      501 2020-04-29 09:53:59.000000 yafowil.widget.cron-1.2/README.rst
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.992502 yafowil.widget.cron-2.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      978 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3639 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      521 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:40:28.992502 yafowil.widget.cron-2.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1729 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1580 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      637 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1148 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      641 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1153 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1080 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/yafowil.widget.cron.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/resources/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2835 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/resources/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    20557 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9386 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/resources/widget.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15686 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6046 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:40:28.988502 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3639 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1107 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      107 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       60 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:40:28.000000 yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yafowil.widget.cron-1.2/setup.py` & `yafowil.widget.cron-2.0a1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# -*- coding: utf-8 -*-
-"""Installer for the yafowil.widget.cron package."""
 from setuptools import find_packages
 from setuptools import setup
+import os
 
 
-version = '1.2'
+def read_file(name):
+    with open(os.path.join(os.path.dirname(__file__), name)) as f:
+        return f.read()
+
+
+version = '2.0a1'
 shortdesc = 'Cron widget for YAFOWIL'
-longdesc = '\n\n'.join([
-    open('README.rst').read(),
-    open('CHANGES.rst').read(),
-    open('LICENSE.rst').read(),
-])
-tests_require = ['yafowil[test]']
+longdesc = '\n\n'.join([read_file(name) for name in [
+    'README.rst',
+    'CHANGES.rst',
+    'LICENSE.rst'
+]])
 
 
 setup(
     name='yafowil.widget.cron',
     version=version,
     description=shortdesc,
     long_description=longdesc,
@@ -27,32 +30,36 @@
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     keywords='',
-    author='BlueDynamics Alliance',
-    author_email='dev@bluedynamics.com',
-    url=u'http://pypi.python.org/pypi/yafowil.widget.cron',
+    author='Yafowil Contributors',
+    author_email='dev@conestack.org',
+    url=u'http://github.com/conestack/yafowil.widget.cron',
     license='Simplified BSD',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['yafowil', 'yafowil.widget'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
         'crontab',
         'yafowil>2.2',
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
     test_suite="yafowil.widget.cron.tests",
     entry_points="""
     [yafowil.plugin]
     register = yafowil.widget.cron:register
     example = yafowil.widget.cron.example:get_example
     """
 )
```

### Comparing `yafowil.widget.cron-1.2/LICENSE.rst` & `yafowil.widget.cron-2.0a1/LICENSE.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-
 License
 =======
 
-Copyright (c) 2010-2020, BlueDynamics Alliance, Austria, Germany, Switzerland
+Copyright (c) 2010-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
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

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/widget.py` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     display_renderers=[
         cron_display_renderer
     ]
 )
 
 factory.doc['blueprint']['cron'] = """\
 Add-on blueprint
-`yafowil.widget.cron <http://github.com/bluedynamics/yafowil.widget.cron/>`_ .
+`yafowil.widget.cron <http://github.com/conestack/yafowil.widget.cron/>`_ .
 """
 
 factory.defaults['cron.class'] = 'crontab widget'
 factory.doc['props']['cron.class'] = """\
 CSS classes for cron widget wrapper DOM element.
 """
```

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.po` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.mo` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.mo`

 * *Files identical despite different names*

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.po` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.mo` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.mo`

 * *Files identical despite different names*

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/locales/yafowil.widget.cron.pot` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/locales/yafowil.widget.cron.pot`

 * *Files identical despite different names*

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/tests.py` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from node.utils import UNSET
 from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.compat import IS_PY2
 from yafowil.tests import fxml
 from yafowil.tests import YafowilTestCase
 from yafowil.utils import EMPTY_VALUE
-import yafowil.loader  # noqa
+import os
+import unittest
 
 
 if not IS_PY2:
     from importlib import reload
 
 
+def np(path):
+    return path.replace('/', os.path.sep)
+
+
 class TestCronWidget(YafowilTestCase):
 
     def setUp(self):
         super(TestCronWidget, self).setUp()
+        from yafowil.widget import cron
         from yafowil.widget.cron import widget
         reload(widget)
+        cron.register()
 
     def test_edit_renderer(self):
         # Render widget
         widget = factory(
             'cron',
             name='cronwidget')
-        self.check_output("""
+        self.checkOutput("""
         <div class="crontab widget" id="input-cronwidget">
           <div class="cron-value minute">
             <input class="hidden" id="input-cronwidget-minute"
                    name="cronwidget.minute" type="hidden" value=""/>
             <button class="btn btn-sm edit">Minute</button>
           </div>
           <div class="cron-value hour">
@@ -65,29 +72,29 @@
             'cron',
             name='cronwidget',
             props={
                 'lang': 'de',
                 'start_year': 2010,
                 'end_year': 2020
             })
-        self.check_output("""
+        self.checkOutput("""
         <div class="crontab widget"
              data-end_year='2020'
              data-lang='de'
              data-start_year='2010'
              id="input-cronwidget">...</div>
         """, widget())
 
     def test_display_renderer(self):
         widget = factory(
             'cron',
             name='cronwidget',
             value='* * * * *',
             mode='display')
-        self.check_output("""
+        self.checkOutput("""
         <div class="display-crontab widget" id="display-cronwidget">
           <code>* * * * *</code>
         </div>
         """, fxml(widget()))
 
     def test_extraction_empty_request(self):
         widget = factory(
@@ -250,15 +257,15 @@
 
     def test_preset_values(self):
         value = '0,10,20,30,40,50 0,6,12,18 1,15,30 3,6,9,12 1,3,5 2017'
         widget = factory(
             'cron',
             name='cronwidget',
             value=value)
-        self.check_output("""
+        self.checkOutput("""
         ...name="cronwidget.minute" type="hidden" value="0,10,20,30,40,50"
         ...name="cronwidget.hour" type="hidden" value="0,6,12,18"
         ...name="cronwidget.dom" type="hidden" value="1,15,30"
         ...name="cronwidget.month" type="hidden" value="3,6,9,12"
         ...name="cronwidget.dow" type="hidden" value="1,3,5"
         ...name="cronwidget.year" type="hidden" value="2017"
         ...
@@ -345,15 +352,15 @@
         )
 
         value = '1 2 3 4 5'
         widget = factory(
             'cron',
             name='cronwidget',
             value=value)
-        self.check_output("""
+        self.checkOutput("""
         ...name="cronwidget.minute" type="hidden" value="1"
         ...name="cronwidget.hour" type="hidden" value="2"
         ...name="cronwidget.dom" type="hidden" value="3"
         ...name="cronwidget.month" type="hidden" value="4"
         ...name="cronwidget.dow" type="hidden" value="5"
         ...name="cronwidget.year" type="hidden" value="*"
         ...
@@ -373,15 +380,15 @@
             'div:cron',
             name='cronwidget',
             value=value,
             props={
                 'leaf': True,
                 'div.class': 'wrapper-div'
             })
-        self.check_output("""
+        self.checkOutput("""
         <div class="wrapper-div"><div class="crontab widget" ...>...</div></div>
         """, widget())
 
         request = {
             'cronwidget.month': u'1',
             'cronwidget.dom': u'2',
             'cronwidget.hour': u'3',
@@ -422,10 +429,33 @@
         )
         year = data['year']
         self.assertEqual(
             [year.name, year.value, year.extracted, year.errors],
             ['year', '2017,2018,2019', '*', []]
         )
 
+    def test_resources(self):
+        factory.theme = 'default'
+        resources = factory.get_resources('yafowil.widget.cron')
+        self.assertTrue(resources.directory.endswith(np('/cron/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.cron')
+        self.assertEqual(resources.path, 'yafowil-cron')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/cron/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-cron')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(styles[0].directory.endswith(np('/cron/resources')))
+        self.assertEqual(styles[0].path, 'yafowil-cron')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
 
 if __name__ == '__main__':
-    unittest.main()                                          # pragma: no cover
+    unittest.main()
```

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/resources/widget.js` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/resources/widget.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,433 +1,376 @@
-/* jslint browser: true */
-/* global jQuery, yafowil */
-/*
- * yafowil cron widget
- *
- * Optional: bdajax
- */
-
-if (window.yafowil === undefined) {
-    window.yafowil = {};
-}
-
-(function($, yafowil) {
+var yafowil_cron = (function(exports, $) {
     'use strict';
 
-    $(document).ready(function() {
-        // initial binding
-        yafowil.cron.binder();
-
-        // add after ajax binding if bdajax present
-        if (window.bdajax !== undefined) {
-            $.extend(window.bdajax.binders, {
-                cron_binder: yafowil.cron.binder
-            });
+    let i18n = {
+        en: {
+            select_minutes: 'Select Minutes',
+            select_hours: 'Select Hours',
+            select_dom: 'Select Day of Month',
+            select_month: 'Select Month',
+            select_dow: 'Select Day of Week',
+            select_year: 'Select Year',
+            select_all: 'Select All',
+            monthmap: {
+                1: 'January',
+                2: 'February',
+                3: 'March',
+                4: 'April',
+                5: 'May',
+                6: 'June',
+                7: 'July',
+                8: 'August',
+                9: 'September',
+                10: 'October',
+                11: 'November',
+                12: 'December'
+            },
+            dowmap: {
+                1: 'Monday',
+                2: 'Tuesday',
+                3: 'Wednesday',
+                4: 'Thursday',
+                5: 'Friday',
+                6: 'Saturday',
+                0: 'Sunday'
+            },
+            summary: 'Summary',
+            no_minutes_selected: 'No minutes selected',
+            selected_minutes: 'Minutes: ',
+            all_minutes_selected: 'Every minute',
+            no_hours_selected: 'No hour selected',
+            selected_hours: 'Hours: ',
+            all_hours_selected: 'Every hour',
+            no_dom_selected: 'No day of month selected',
+            selected_dom: 'Days of month: ',
+            all_dom_selected: 'Every day of month',
+            no_month_selected: 'No month selected',
+            selected_month: 'Month: ',
+            all_month_selected: 'Every month',
+            no_dow_selected: 'No day of week selected',
+            selected_dow: 'Days of week: ',
+            all_dow_selected: 'Every day of week',
+            no_year_selected: 'No year selected',
+            selected_years: 'Years: ',
+            all_years_selected: 'Every year'
+        },
+        de: {
+            select_minutes: 'Minuten auswählen',
+            select_hours: 'Stunden auswählen',
+            select_dom: 'Monatstage auswählen',
+            select_month: 'Monate auswählen',
+            select_dow: 'Wochentage auswählen',
+            select_year: 'Jahre auswählen',
+            select_all: 'Alle auswählen',
+            monthmap: {
+                1: 'Jänner',
+                2: 'Feber',
+                3: 'März',
+                4: 'April',
+                5: 'Mai',
+                6: 'Juni',
+                7: 'Juli',
+                8: 'August',
+                9: 'September',
+                10: 'Oktober',
+                11: 'November',
+                12: 'Dezember'
+            },
+            dowmap: {
+                1: 'Montag',
+                2: 'Dienstag',
+                3: 'Mittwoch',
+                4: 'Donnerstag',
+                5: 'Freitag',
+                6: 'Samstag',
+                0: 'Sonntag'
+            },
+            summary: 'Zusammenfassung',
+            no_minutes_selected: 'Keine Minuten ausgewählt',
+            selected_minutes: 'Minuten: ',
+            all_minutes_selected: 'Jede Minute',
+            no_hours_selected: 'Keine Stunden ausgewählt',
+            selected_hours: 'Stunden: ',
+            all_hours_selected: 'Jede Stunde',
+            no_dom_selected: 'Keine Monatstage ausgewählt',
+            selected_dom: 'Monatstage: ',
+            all_dom_selected: 'Alle Monatstage',
+            no_month_selected: 'Keine Monate ausgewählt',
+            selected_month: 'Monate: ',
+            all_month_selected: 'Jedes Monat',
+            no_dow_selected: 'Keine Wochentage ausgewählt',
+            selected_dow: 'Wochentage: ',
+            all_dow_selected: 'Jeder Wochentag',
+            no_year_selected: 'Kein Jahr ausgewählt',
+            selected_years: 'Jahre: ',
+            all_years_selected: 'Jedes Jahr'
         }
-    });
-
-    $.extend(yafowil, {
+    };
 
-        cron: {
-            i18n: {
-                en: {
-                    select_minutes: 'Select Minutes',
-                    select_hours: 'Select Hours',
-                    select_dom: 'Select Day of Month',
-                    select_month: 'Select Month',
-                    select_dow: 'Select Day of Week',
-                    select_year: 'Select Year',
-                    select_all: 'Select All',
-                    monthmap: {
-                        1: 'January',
-                        2: 'February',
-                        3: 'March',
-                        4: 'April',
-                        5: 'May',
-                        6: 'June',
-                        7: 'July',
-                        8: 'August',
-                        9: 'September',
-                        10: 'October',
-                        11: 'November',
-                        12: 'December'
-                    },
-                    dowmap: {
-                        1: 'Monday',
-                        2: 'Tuesday',
-                        3: 'Wednesday',
-                        4: 'Thursday',
-                        5: 'Friday',
-                        6: 'Saturday',
-                        0: 'Sunday'
-                    },
-                    summary: 'Summary',
-                    no_minutes_selected: 'No minutes selected',
-                    selected_minutes: 'Minutes: ',
-                    all_minutes_selected: 'Every minute',
-                    no_hours_selected: 'No hour selected',
-                    selected_hours: 'Hours: ',
-                    all_hours_selected: 'Every hour',
-                    no_dom_selected: 'No day of month selected',
-                    selected_dom: 'Days of month: ',
-                    all_dom_selected: 'Every day of month',
-                    no_month_selected: 'No month selected',
-                    selected_month: 'Month: ',
-                    all_month_selected: 'Every month',
-                    no_dow_selected: 'No day of week selected',
-                    selected_dow: 'Days of week: ',
-                    all_dow_selected: 'Every day of week',
-                    no_year_selected: 'No year selected',
-                    selected_years: 'Years: ',
-                    all_years_selected: 'Every year'
-                },
-                de: {
-                    select_minutes: 'Minuten auswählen',
-                    select_hours: 'Stunden auswählen',
-                    select_dom: 'Monatstage auswählen',
-                    select_month: 'Monate auswählen',
-                    select_dow: 'Wochentage auswählen',
-                    select_year: 'Jahre auswählen',
-                    select_all: 'Alle auswählen',
-                    monthmap: {
-                        1: 'Jänner',
-                        2: 'Feber',
-                        3: 'März',
-                        4: 'April',
-                        5: 'Mai',
-                        6: 'Juni',
-                        7: 'Juli',
-                        8: 'August',
-                        9: 'September',
-                        10: 'Oktober',
-                        11: 'November',
-                        12: 'Dezember'
-                    },
-                    dowmap: {
-                        1: 'Montag',
-                        2: 'Dienstag',
-                        3: 'Mittwoch',
-                        4: 'Donnerstag',
-                        5: 'Freitag',
-                        6: 'Samstag',
-                        0: 'Sonntag'
-                    },
-                    summary: 'Zusammenfassung',
-                    no_minutes_selected: 'Keine Minuten ausgewählt',
-                    selected_minutes: 'Minuten: ',
-                    all_minutes_selected: 'Jede Minute',
-                    no_hours_selected: 'Keine Stunden ausgewählt',
-                    selected_hours: 'Stunden: ',
-                    all_hours_selected: 'Jede Stunde',
-                    no_dom_selected: 'Keine Monatstage ausgewählt',
-                    selected_dom: 'Monatstage: ',
-                    all_dom_selected: 'Alle Monatstage',
-                    no_month_selected: 'Keine Monate ausgewählt',
-                    selected_month: 'Monate: ',
-                    all_month_selected: 'Jedes Monat',
-                    no_dow_selected: 'Keine Wochentage ausgewählt',
-                    selected_dow: 'Wochentage: ',
-                    all_dow_selected: 'Jeder Wochentag',
-                    no_year_selected: 'Kein Jahr ausgewählt',
-                    selected_years: 'Jahre: ',
-                    all_years_selected: 'Jedes Jahr'
+    class CronWidget {
+        static initialize(context) {
+            $('.crontab.widget', context).each(function() {
+                let elem = $(this);
+                if (window.yafowil_array !== undefined &&
+                    window.yafowil_array.inside_template(elem)) {
+                    return;
                 }
-            },
-
-            binder: function(context) {
-                $('.crontab.widget', context).each(function() {
-                    new yafowil.cron.Widget($(this), 'edit');
-                });
-                $('.display-crontab.widget', context).each(function() {
-                    new yafowil.cron.Widget($(this), 'display');
-                });
-            }
+                new CronWidget(elem, 'edit');
+            });
+            $('.display-crontab.widget', context).each(function() {
+                let elem = $(this);
+                if (window.yafowil_array !== undefined &&
+                    window.yafowil_array.inside_template(elem)) {
+                    return;
+                }
+                new CronWidget(elem, 'display');
+            });
         }
-    });
-
-    yafowil.cron.Widget = function(root, mode) {
-        this.root = root;
-        this.mode = mode;
-
-        var lang = root.data('lang');
-        this.lang = lang ? lang : this.lang;
-
-        var start_year = root.data('start_year');
-        this.start_year = start_year ? start_year : this.start_year;
-
-        var end_year = root.data('end_year');
-        this.end_year = end_year ? end_year : this.end_year;
-
-        this.pressed = false;
-
-        this.value = {
-            minute: [],
-            hour: [],
-            dom: [],
-            month: [],
-            dow: [],
-            year: []
-        };
-
-        var summary_container_template =
-            '<article class="crontab_summary">' +
-            '<strong>' + this.translate('summary') + '</strong>' +
-            '<p class="summary"></p>' +
-            '</article>';
-
-        if (mode === 'display') {
-            this.parse($('code', root).text());
+        constructor(root, mode) {
+            root.data('yafowil-cron', this);
+            this.root = root;
+            this.mode = mode;
+            let lang = root.data('lang');
+            this.lang = lang ? lang : 'en';
+            let start_year = root.data('start_year');
+            this.start_year = start_year ? start_year : new Date().getFullYear();
+            let end_year = root.data('end_year');
+            this.end_year = end_year ? end_year : new Date().getFullYear() + 9;
+            this.pressed = false;
+            this.value = {
+                minute: [],
+                hour: [],
+                dom: [],
+                month: [],
+                dow: [],
+                year: []
+            };
+            let summary_container_template =
+                '<article class="crontab_summary">' +
+                '<strong>' + this.translate('summary') + '</strong>' +
+                '<p class="summary"></p>' +
+                '</article>';
+            if (mode === 'display') {
+                this.parse($('code', root).text());
+                root.append($(summary_container_template));
+                this.update_summary();
+                return;
+            }
+            let that = this;
+            $('input[type="hidden"]', root).each(function() {
+                that.parse_from_input($(this));
+            });
             root.append($(summary_container_template));
             this.update_summary();
-            return;
+            this.edit_area = $('.editarea', root);
+            this.edit_area.on('mousedown touchstart', function(evt) {
+                that.pressed = true;
+            });
+            $(document).on('mouseup touchend', function(evt) {
+                that.pressed = false;
+            });
+            $('button.edit', root).on('click', function(evt) {
+                evt.preventDefault();
+                that.show_edit_section($(this));
+            });
         }
-
-        var that = this;
-
-        $('input[type="hidden"]', root).each(function() {
-            that.parse_from_input($(this));
-        });
-
-        root.append($(summary_container_template));
-        this.update_summary();
-
-        this.edit_area = $('.editarea', root);
-        this.edit_area.on('mousedown touchstart', function(evt) {
-            that.pressed = true;
-        });
-
-        $(document).on('mouseup touchend', function(evt) {
-            that.pressed = false;
-        });
-
-        $('button.edit', root).on('click', function(evt) {
-            evt.preventDefault();
-            that.show_edit_section($(this));
-        });
-    };
-
-    yafowil.cron.Widget.prototype = {
-        lang: 'en',
-        start_year: new Date().getFullYear(),
-        end_year: new Date().getFullYear() + 9,
-
-        show_edit_section: function(trigger) {
-            var cnt,
+        show_edit_section(trigger) {
+            let cnt,
                 edit_area = this.edit_area,
                 container = this.get_edit_section(trigger),
                 mode = this.get_mode(container);
             if (edit_area.is(':visible') && edit_area.hasClass(mode)) {
                 container.removeClass('active');
                 edit_area.attr('class', 'editarea').html('').hide();
                 return;
             }
-            var header = $('<h4 />'),
+            let header = $('<h4 />'),
                 content = $('<div class="editcontainer" />');
             if (mode === 'minute') {
                 header.text(this.translate('select_minutes'));
                 for (cnt = 0; cnt <= 59; cnt++) {
                     content.append(this.make_button(cnt, cnt, mode));
                 }
             } else if (mode === 'hour') {
                 header.text(this.translate('select_hours'));
-                var hour;
+                let hour;
                 for (cnt = 1; cnt <= 24; cnt++) {
-                    // "0" should be rendered as last element.
                     hour = cnt < 24 ? cnt : 0;
                     content.append(this.make_button(hour, hour, mode));
                 }
             } else if (mode === 'dom') {
                 header.text(this.translate('select_dom'));
                 for (cnt = 1; cnt <= 31; cnt++) {
                     content.append(this.make_button(cnt, cnt, mode));
                 }
             } else if (mode === 'month') {
                 header.text(this.translate('select_month'));
-                var monthmap = this.monthmap();
+                let monthmap = this.monthmap();
                 for (cnt = 1; cnt <= 12; cnt++) {
                     content.append(this.make_button(cnt, monthmap[cnt], mode));
                 }
             } else if (mode === 'dow') {
                 header.text(this.translate('select_dow'));
-                var dowmap = this.dowmap(),
+                let dowmap = this.dowmap(),
                     dow;
                 for (cnt = 1; cnt <= 7; cnt++) {
-                    // "0" should be rendered as last element.
                     dow = cnt < 7 ? cnt : 0;
                     content.append(this.make_button(dow, dowmap[dow], mode));
                 }
             } else if (mode === 'year') {
                 header.text(this.translate('select_year'));
                 for (cnt = this.start_year; cnt <= this.end_year; cnt++) {
                     content.append(this.make_button(cnt, cnt, mode));
                 }
             }
             header = header.add(this.make_button_all(mode));
             content = header.add(content);
             edit_area.html(content).attr('class', 'editarea ' + mode).show();
             container.addClass('active');
-        },
-
-        make_button_all: function(mode) {
-            var button = $(
+        }
+        make_button_all(mode) {
+            let button = $(
                 '<button class="btn btn-sm select_all">' +
                 this.translate('select_all') +
                 '</button>'
             );
             if (this.value[mode].length >= this.maxlengths()[mode]) {
                 button.addClass('active');
             }
-            var that = this;
+            let that = this;
             button.on('click', function(evt) {
                 evt.preventDefault();
-                var $this = $(this);
+                let $this = $(this);
                 if ($this.hasClass('active')) {
-                    // clear
                     $this.parent().find('.editcontainer button').each(function() {
                         $(this).removeClass('active');
                     });
                     $this.removeClass('active');
                     that.parse_part('', mode);
                 } else {
-                    // select all
                     $this.parent().find('.editcontainer button').each(function() {
                         $(this).removeClass('active').addClass('active');
                     });
                     $this.removeClass('active').addClass('active');
                     that.parse_part('*', mode);
                 }
                 that.serialize_to_input();
                 that.update_summary();
             });
             return button;
-        },
-
-        make_button: function(value, name, mode) {
-            var button = $(
+        }
+        make_button(value, name, mode) {
+            let button = $(
                 '<button class="btn btn-sm" name=' + value + '>' +
                 name +
                 '</button>'
             );
             if (this.has(value, mode)) {
                 button.addClass('active');
             }
-            var that = this;
-
-            var handler = function(evt) {
+            let that = this;
+            let handler = function(evt) {
                 evt.preventDefault();
-                var elem = $(this);
-                var container = that.edit_area;
+                let elem = $(this);
+                let container = that.edit_area;
                 if (elem.hasClass('active')) {
                     that.remove(elem.attr('name'), that.get_mode(container));
                     that.serialize_to_input();
                     elem.removeClass('active');
                 } else {
                     that.add(elem.attr('name'), that.get_mode(container));
                     that.serialize_to_input();
                     elem.addClass('active');
                 }
                 that.update_summary();
             };
-
             button.on('click', function(evt) {
                 evt.preventDefault();
             }).on('mousedown touchstart',
                 handler
             ).on('mouseenter touchenter', function(evt) {
                 if (evt.shiftKey === false && that.pressed === false) {
                     return;
                 }
                 handler.bind(this)(evt);
             }).on('mouseup touchend', function(evt) {
                 that.pressed = false;
             });
             return button;
-        },
-
-        maxlengths: function() {
+        }
+        maxlengths() {
             return {
                 minute: 60,
                 hour: 24,
                 dom: 31,
                 month: 12,
                 dow: 7,
                 year: this.end_year - this.start_year + 1
             };
-        },
-
-        translate: function(msg) {
-            return yafowil.cron.i18n[this.lang][msg];
-        },
-
-        monthmap: function() {
-            return yafowil.cron.i18n[this.lang].monthmap;
-        },
-
-        dowmap: function() {
-            return yafowil.cron.i18n[this.lang].dowmap;
-        },
-
-        get_edit_section: function(elem) {
+        }
+        translate(msg) {
+            return i18n[this.lang][msg];
+        }
+        monthmap() {
+            return i18n[this.lang].monthmap;
+        }
+        dowmap() {
+            return i18n[this.lang].dowmap;
+        }
+        get_edit_section(elem) {
             return elem.closest('.cron-value');
-        },
-
-        get_mode: function(elem) {
-            var klass = elem.attr('class');
+        }
+        get_mode(elem) {
+            let klass = elem.attr('class');
             if (klass.indexOf('minute') !== -1) {
                 return 'minute';
             } else if (klass.indexOf('hour') !== -1) {
                 return 'hour';
             } else if (klass.indexOf('dom') !== -1) {
                 return 'dom';
             } else if (klass.indexOf('month') !== -1) {
                 return 'month';
             } else if (klass.indexOf('dow') !== -1) {
                 return 'dow';
             } else if (klass.indexOf('year') !== -1) {
                 return 'year';
             }
-        },
-
-        add: function(value, mode) {
+        }
+        add(value, mode) {
             this.value[mode].push(value.toString());
-        },
-
-        remove: function(value, mode) {
-            var index = this.value[mode].indexOf(value.toString());
+        }
+        remove(value, mode) {
+            let index = this.value[mode].indexOf(value.toString());
             if (index > -1) {
                 this.value[mode].splice(index, 1);
             }
-        },
-
-        has: function(value, mode) {
+        }
+        has(value, mode) {
             return this.value[mode].indexOf(value.toString()) > -1;
-        },
-
-        parse: function(value) {
+        }
+        parse(value) {
             value = value.split(' ');
             if (value.length === 5) {
-                // year is optional
                 value.push('*');
             }
             this.parse_part(value[0].trim(), 'minute');
             this.parse_part(value[1].trim(), 'hour');
             this.parse_part(value[2].trim(), 'dom');
             this.parse_part(value[3].trim(), 'month');
             this.parse_part(value[4].trim(), 'dow');
             this.parse_part(value[5].trim(), 'year');
-        },
-
-        parse_part: function(value, mode) {
+        }
+        parse_part(value, mode) {
             if (typeof value === 'string') {
                 value = value.split(',');
             }
             this.value[mode] = [];
-            var cnt;
+            let cnt;
             if (value[0] === '*') {
-                var start, end;
+                let start, end;
                 if (mode === 'minute') {
                     start = 0;
                     end = 59;
                 } else if (mode === 'hour') {
                     start = 0;
                     end = 23;
                 } else if (mode === 'dom') {
@@ -443,56 +386,51 @@
                     start = this.start_year;
                     end = this.end_year;
                 }
                 for (cnt = start; cnt < end + 1; cnt++) {
                     this.value[mode].push(cnt.toString());
                 }
             } else {
-                var val;
+                let val;
                 for (cnt = 0; cnt < value.length; cnt++) {
                     val = value[cnt];
                     if (val === '') {
                         continue;
                     }
                     val = parseInt(val, 10).toString();
                     this.value[mode].push(val);
                 }
             }
-        },
-
-        serialize: function(mode) {
-            var vals = this.value[mode];
+        }
+        serialize(mode) {
+            let vals = this.value[mode];
             vals.sort(function(a, b) {
-                // int-sort - otherwise it's a lexical sort.
                 return parseInt(a, 10) - parseInt(b, 10);
             });
-            var maxlength = this.maxlengths()[mode];
+            let maxlength = this.maxlengths()[mode];
             if (vals.length >= maxlength) {
                 return '*';
             } else {
                 return vals.join(',');
             }
-        },
-
-        parse_from_input: function(input) {
+        }
+        parse_from_input(input) {
             this.parse_part(
                 input.val(),
                 this.get_mode(this.get_edit_section(input))
             );
-        },
-
-        serialize_to_input: function() {
-            var container = this.edit_area,
+        }
+        serialize_to_input() {
+            let container = this.edit_area,
                 mode = this.get_mode(container),
                 input = $('.cron-value.' + mode + ' input', this.root);
             input.val(this.serialize(mode));
-        },
-
-        group_value: function(arr) {
-            var groups = [],
+        }
+        group_value(arr) {
+            let groups = [],
                 group = [],
                 idx,
                 nidx;
             for (idx = 0; idx < arr.length; idx++) {
                 nidx = idx + 1;
                 if (idx === arr.length - 1) {
                     group.push(arr[idx]);
@@ -502,21 +440,19 @@
                 } else {
                     group.push(arr[idx]);
                     groups.push(group);
                     group = [];
                 }
             }
             return groups;
-        },
-
-        update_summary: function() {
+        }
+        update_summary() {
             $('.crontab_summary .summary', this.root).html(this.summarize());
-        },
-
-        summarize: function() {
+        }
+        summarize() {
             return [
                 this.format_part(
                     'minute', 'no_minutes_selected',
                     'selected_minutes', 'all_minutes_selected'
                 ),
                 this.format_part(
                     'hour', 'no_hours_selected',
@@ -537,38 +473,35 @@
                     this.dowmap()
                 ),
                 this.format_part(
                     'year', 'no_year_selected',
                     'selected_years', 'all_years_selected'
                 )
             ].join('<br/>');
-        },
-
-        format_part: function(value_name, no_values_selected,
-            values_selected, all_values_selected,
-            value_map) {
-            var value = this.value[value_name],
+        }
+        format_part(value_name, no_values_selected, values_selected,
+            all_values_selected, value_map) {
+            let value = this.value[value_name],
                 value_len = value.length,
                 max_len = this.maxlengths()[value_name],
                 ret;
             if (value_len === 0) {
                 ret = this.translate(no_values_selected);
             } else if (value_len < max_len) {
                 ret = this.translate(values_selected) + this.format_groups(
                     this.group_value(value),
                     value_map
                 );
             } else {
                 ret = this.translate(all_values_selected);
             }
             return ret;
-        },
-
-        format_groups: function(groups, value_map) {
-            var ret = '',
+        }
+        format_groups(groups, value_map) {
+            let ret = '',
                 idx,
                 group;
             for (idx = 0; idx < groups.length; idx++) {
                 group = groups[idx];
                 if (group.length === 1) {
                     ret += this.display_value(group[0], value_map);
                 } else {
@@ -580,18 +513,55 @@
                     );
                 }
                 if (idx !== groups.length - 1) {
                     ret += ', ';
                 }
             }
             return ret;
-        },
-
-        display_value: function(value, value_map) {
+        }
+        display_value(value, value_map) {
             if (value_map) {
                 return value_map[value];
             }
             return value;
         }
-    };
+    }
+
+    function cron_on_array_add(inst, context) {
+        CronWidget.initialize(context);
+    }
+
+    function register_array_subscribers() {
+        if (window.yafowil_array === undefined) {
+            return;
+        }
+        window.yafowil_array.on_array_event('on_add', cron_on_array_add);
+    }
+
+    $(function() {
+        if (window.ts !== undefined) {
+            ts.ajax.register(CronWidget.initialize, true);
+        } else if (window.bdajax !== undefined) {
+            bdajax.register(CronWidget.initialize, true);
+        } else {
+            CronWidget.initialize();
+        }
+        register_array_subscribers();
+    });
+
+    exports.CronWidget = CronWidget;
+    exports.cron_on_array_add = cron_on_array_add;
+    exports.i18n = i18n;
+    exports.register_array_subscribers = register_array_subscribers;
+
+    Object.defineProperty(exports, '__esModule', {
+        value: true
+    });
+
+
+    window.yafowil = window.yafowil || {};
+    window.yafowil.cron = exports;
+
+
+    return exports;
 
-})(jQuery, yafowil);
+})({}, jQuery);
```

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/resources/widget.css` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/resources/widget.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,24 @@
 .clearfix::after {
   content: "";
   display: table;
   clear: both;
 }
+
 .crontab.widget .cron-value {
   display: inline-block;
   margin-right: 2px;
 }
 .crontab.widget .crontab_summary {
   margin-top: 1em;
 }
 .crontab.widget .editarea {
   display: none;
   width: 100%;
 }
-.crontab.widget .editarea .active {
-  background-color: yellow;
-}
-.crontab.widget .editarea .select_all {
-  margin: 1em 0;
-}
-.crontab.widget .editarea .editcontainer::after {
-  content: "";
-  display: table;
-  clear: both;
-}
-.crontab.widget .editarea .editcontainer button {
-  display: block;
-  vertical-align: top;
-  float: left;
-  margin: 0 2px 2px 0;
-  padding: 0.4em;
-}
-.crontab.widget .editarea .editcontainer button:last-child::after {
-  clear: both;
-}
 .crontab.widget .editarea.minute .editcontainer button {
   width: 3em;
 }
 .crontab.widget .editarea.minute .editcontainer button:nth-child(11),
 .crontab.widget .editarea.minute .editcontainer button:nth-child(21),
 .crontab.widget .editarea.minute .editcontainer button:nth-child(31),
 .crontab.widget .editarea.minute .editcontainer button:nth-child(41),
@@ -81,7 +61,29 @@
 .crontab.widget .editarea.year .editcontainer button:nth-child(51),
 .crontab.widget .editarea.year .editcontainer button:nth-child(61),
 .crontab.widget .editarea.year .editcontainer button:nth-child(71),
 .crontab.widget .editarea.year .editcontainer button:nth-child(81),
 .crontab.widget .editarea.year .editcontainer button:nth-child(91) {
   clear: left;
 }
+.crontab.widget .editarea .active {
+  background-color: var(--yafowil-accent-color, #0d6efd);
+  color: var(--yafowil-accent-font-color, #fff);
+}
+.crontab.widget .editarea .select_all {
+  margin: 1em 0;
+}
+.crontab.widget .editarea .editcontainer::after {
+  content: "";
+  display: table;
+  clear: both;
+}
+.crontab.widget .editarea .editcontainer button {
+  display: block;
+  vertical-align: top;
+  float: left;
+  margin: 0 2px 2px 0;
+  padding: 0.4em;
+}
+.crontab.widget .editarea .editcontainer button:last-child::after {
+  clear: both;
+}
```

### Comparing `yafowil.widget.cron-1.2/src/yafowil/widget/cron/example.py` & `yafowil.widget.cron-2.0a1/src/yafowil/widget/cron/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from node.utils import UNSET
 from yafowil.base import factory
 
 
 DOC_CRON = """
 Crontab widget
 --------------
```

### Comparing `yafowil.widget.cron-1.2/src/yafowil.widget.cron.egg-info/SOURCES.txt` & `yafowil.widget.cron-2.0a1/src/yafowil.widget.cron.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
-TODO.rst
 setup.py
 src/yafowil/__init__.py
 src/yafowil.widget.cron.egg-info/PKG-INFO
 src/yafowil.widget.cron.egg-info/SOURCES.txt
 src/yafowil.widget.cron.egg-info/dependency_links.txt
 src/yafowil.widget.cron.egg-info/entry_points.txt
 src/yafowil.widget.cron.egg-info/namespace_packages.txt
@@ -21,8 +20,8 @@
 src/yafowil/widget/cron/locales/yafowil.widget.cron.pot
 src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.mo
 src/yafowil/widget/cron/locales/de/LC_MESSAGES/yafowil.widget.cron.po
 src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.mo
 src/yafowil/widget/cron/locales/en/LC_MESSAGES/yafowil.widget.cron.po
 src/yafowil/widget/cron/resources/widget.css
 src/yafowil/widget/cron/resources/widget.js
-src/yafowil/widget/cron/resources/widget.less
+src/yafowil/widget/cron/resources/widget.min.js
```

