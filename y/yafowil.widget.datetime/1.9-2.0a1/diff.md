# Comparing `tmp/yafowil.widget.datetime-1.9.tar.gz` & `tmp/yafowil.widget.datetime-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yafowil.widget.datetime-1.9.tar", last modified: Fri Mar 10 11:08:55 2017, max compression
+gzip compressed data, was "yafowil.widget.datetime-2.0a1.tar", last modified: Mon May 15 12:41:55 2023, max compression
```

## Comparing `yafowil.widget.datetime-1.9.tar` & `yafowil.widget.datetime-2.0a1.tar`

### file list

```diff
@@ -1,52 +1,124 @@
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    13467 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/widget.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    13732 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/widget.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2173 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/example.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/en/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1718 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/yafowil.widget.datetime.po
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      934 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/yafowil.widget.datetime.mo
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1361 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/yafowil.widget.datetime.pot
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/de/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1815 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/yafowil.widget.datetime.po
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1032 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/yafowil.widget.datetime.mo
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2101 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.timepicker.bootstrap.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2101 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.timepicker.plone5.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     6298 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.datepicker.bootstrap.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1789 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.timepicker.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    76324 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.datepicker.js
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     6298 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.datepicker.plone5.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    67624 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.timepicker.js
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      685 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/widget-plone5.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     3329 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/widget.js
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      597 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/widget-bootstrap.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       61 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/widget.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    35806 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.datepicker.min.js
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     3702 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/resources/jquery.ui.datepicker.css
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2034 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/__init__.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      681 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/tests.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil/widget/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/not-zip-safe
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       23 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/namespace_packages.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      132 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/entry_points.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/dependency_links.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       68 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/requires.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1911 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/SOURCES.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        8 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/top_level.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     7045 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/PKG-INFO
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      504 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/README.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1576 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/setup.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2889 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/CHANGES.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       59 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/setup.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1537 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/LICENSE.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       72 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/MANIFEST.in
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     7045 2017-03-10 11:08:55.000000 yafowil.widget.datetime-1.9/PKG-INFO
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.754052 yafowil.widget.datetime-2.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3908 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6635 2023-05-15 12:41:55.754052 yafowil.widget.datetime-2.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      575 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:41:55.754052 yafowil.widget.datetime-2.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1775 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.746052 yafowil.widget.datetime-2.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.746052 yafowil.widget.datetime-2.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.750052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.750052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2381 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3115 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.750052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.746052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.750052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1032 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/yafowil.widget.datetime.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1815 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/yafowil.widget.datetime.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.746052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.750052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      934 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/yafowil.widget.datetime.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1718 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/yafowil.widget.datetime.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1361 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/yafowil.widget.datetime.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.750052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5992 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/datepicker.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    81533 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/datepicker.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    31587 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/datepicker.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.754052 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      883 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ar-tn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      905 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ar.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      644 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/az.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      806 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/bg.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      728 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/bm.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1413 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/bn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      707 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/br.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      622 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/bs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      709 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      783 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/cs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      604 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/cy.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      775 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/da.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      701 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/de.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      916 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/el.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      734 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/en-AU.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      720 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/en-CA.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      727 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/en-GB.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      684 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/en-IE.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      689 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/en-NZ.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      691 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/en-ZA.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      721 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/eo.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      716 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/es.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      794 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/et.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      729 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/eu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      874 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/fa.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      731 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/fi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      692 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/fo.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      828 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/fr-CH.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      734 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/fr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      619 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/gl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      741 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/he.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1141 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/hi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      575 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/hr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      738 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/hu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      954 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/hy.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      633 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/id.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      684 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/is.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      817 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/it-CH.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      723 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/it.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      700 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ja.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1170 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ka.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      833 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/kk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1257 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/km.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      775 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ko.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      774 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/lt.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      714 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/lv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      691 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/me.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      840 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/mk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      841 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/mn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1193 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/mr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      626 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ms.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      733 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/nl-BE.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      716 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/nl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      720 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/no.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      676 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/oc.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      732 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/pl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      697 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/pt-BR.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      749 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/pt.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      702 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ro.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      933 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ru.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1199 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/si.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      736 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/sk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      640 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/sl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      729 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/sq.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      672 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/sr-latn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      849 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/sr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      689 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/sv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      712 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/sw.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1139 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/ta.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      949 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/tg.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1010 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/th.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      740 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/tk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      693 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/tr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      895 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/uk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      895 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/uz-cyrl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      727 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/uz-latn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      740 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/vi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      824 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/zh-CN.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      863 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/locales/zh-TW.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2321 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/timepicker.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17830 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8677 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/resources/widget.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    25475 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15524 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:41:55.750052 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6635 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5534 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      115 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       82 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:41:55.000000 yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/widget.py` & `yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 from bda.intellidatetime import LocalePattern
 from bda.intellidatetime import convert
 from datetime import datetime
 from node.utils import UNSET
 from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.base import fetch_value
+from yafowil.common import generic_emptyvalue_extractor
 from yafowil.common import generic_extractor
 from yafowil.common import generic_required_extractor
+from yafowil.compat import IS_PY2
 from yafowil.tsf import TSF
 from yafowil.utils import attr_value
 from yafowil.utils import css_managed_props
 from yafowil.utils import cssclasses
 from yafowil.utils import cssid
 from yafowil.utils import managedprops
 
 
 _ = TSF('yafowil.widget.datetime')
 
 
 def time_data_defs(widget, data):
-    format = attr_value('format', widget, data)
-    if format not in ['number', 'string', 'tuple']:
-        raise ValueError(u"Unknown format '{}'".format(format))
+    format_ = attr_value('format', widget, data)
+    if format_ not in ['number', 'string', 'tuple']:
+        raise ValueError(u"Unknown format '{}'".format(format_))
     unit = attr_value('unit', widget, data)
     if unit not in ['minutes', 'hours']:
         raise ValueError(u"Unknown unit '{}'".format(unit))
-    return format, unit
+    return format_, unit
 
 
-@managedprops('format', 'unit', 'daytime')
+@managedprops('format', 'unit', 'daytime', 'clock')
 def time_extractor(widget, data):
-    format, unit = time_data_defs(widget, data)
+    format_, unit = time_data_defs(widget, data)
     extracted = data.extracted
     if extracted == UNSET or extracted == '':
         return UNSET
     if len(extracted) > 5:
         message = _('input_not_valid_time', default=u'Not a valid time input.')
         raise ExtractionError(message)
     elif len(extracted) == 5:
@@ -43,44 +45,54 @@
         minutes = extracted[3:]
     elif len(extracted) == 4 and extracted.find(':') == -1:
         hours = extracted[:2]
         minutes = extracted[2:]
     else:
         extracted = extracted.split(':')
         if len(extracted) != 2:
-            message = _('failed_to_parse_time',
-                        default=u'Failed to parse time input.')
+            message = _(
+                'failed_to_parse_time',
+                default=u'Failed to parse time input.'
+            )
             raise ExtractionError(message)
         hours, minutes = extracted
     try:
         hours = int(hours)
     except ValueError:
-        message = _('hours_not_a_number',
-                    default=u'Hours not a number.')
+        message = _(
+            'hours_not_a_number',
+            default=u'Hours not a number.'
+        )
         raise ExtractionError(message)
     try:
         minutes = int(minutes)
     except ValueError:
-        message = _('minutes_not_a_number',
-                    default=u'Minutes not a number.')
+        message = _(
+            'minutes_not_a_number',
+            default=u'Minutes not a number.'
+        )
         raise ExtractionError(message)
     daytime = attr_value('daytime', widget, data)
     timepicker = attr_value('timepicker', widget, data)
     if daytime or timepicker:
         if hours < 0 or hours > 23:
-            message = _('invalid_hours_range',
-                        default=u'Hours must be in range 0..23.')
+            message = _(
+                'invalid_hours_range',
+                default=u'Hours must be in range 0..23.'
+            )
             raise ExtractionError(message)
         if minutes < 0 or minutes > 59:
-            message = _('invalid_minutes_range',
-                        default=u'Minutes must be in range 0..59.')
+            message = _(
+                'invalid_minutes_range',
+                default=u'Minutes must be in range 0..59.'
+            )
             raise ExtractionError(message)
-    if format == 'string':
+    if format_ == 'string':
         return '{:02d}:{:02d}'.format(hours, minutes)
-    if format == 'tuple':
+    if format_ == 'tuple':
         return (hours, minutes)
     if unit == 'hours':
         return hours + (minutes / 60.0)
     return hours * 60 + minutes
 
 
 def render_time_input(widget, data, value, postfix=None, css_class=False):
@@ -95,122 +107,154 @@
     disabled = 'disabled' if attr_value('disabled', widget, data) else None
     attrs = {
         'type': 'text',
         'value': value,
         'name_': widgetname,
         'id': cssid(widget, 'input', postfix),
         'size': 5,
-        'disabled': disabled,
+        'disabled': disabled
     }
     class_ = [attr_value('timeinput_class', widget, data)]
     timepicker = attr_value('timepicker', widget, data)
     if timepicker and not disabled:
         class_.append(attr_value('timepicker_class', widget, data))
+        attrs['data-time-locale'] = attr_value('locale', widget, data)
+        attrs['data-time-clock'] = attr_value('clock', widget, data)
+        attrs['data-time-minutes_step'] = attr_value(
+            'minutes_step',
+            widget,
+            data
+        )
     if css_class:
         attrs['class_'] = cssclasses(widget, data, additional=class_)
     else:
         attrs['class_'] = ' '.join(class_)
     return tag('input', **attrs)
 
 
-def time_value(format, unit, time):
-    if format == 'tuple':
+def time_value(format_, unit, time):
+    if format_ == 'tuple':
         if not time:
             return ''
-        time = '{:02d}:{:02d}'.format(*time)
-    elif format == 'number':
+        time = '{:02d}:{:02d}'.format(*(int(time[0]), int(time[1])))
+    elif format_ == 'number':
         if time is UNSET or time == '':
             return ''
         if unit == 'hours':
             hours = int(time)
             minutes = int(round((time - int(time)) * 60.0))
             time = '{:02d}:{:02d}'.format(hours, minutes)
         else:
-            hours = time / 60
+            if IS_PY2:
+                hours = time / 60
+            else:
+                hours = time // 60
             minutes = time % 60
             time = '{:02d}:{:02d}'.format(hours, minutes)
     return time
 
 
-@managedprops('format', 'unit', 'disabled', 'timepicker',
-              'timepicker_class', *css_managed_props)
+@managedprops(
+    'format', 'unit', 'disabled', 'timepicker', 'timepicker_class', 'clock',
+    'minutes_step', 'locale', *css_managed_props
+)
 def time_edit_renderer(widget, data):
-    format, unit = time_data_defs(widget, data)
-    time = time_value(format, unit, fetch_value(widget, data))
+    format_, unit = time_data_defs(widget, data)
+    time = time_value(format_, unit, fetch_value(widget, data))
     return render_time_input(widget, data, time, css_class=True)
 
 
 @managedprops('format', 'unit', 'class')
 def time_display_renderer(widget, data):
-    format, unit = time_data_defs(widget, data)
+    format_, unit = time_data_defs(widget, data)
     value = data.value
     if not value:
         return u''
     attrs = {
         'id': cssid(widget, 'display'),
         'class_': 'display-{}'.format(attr_value('class', widget, data))
     }
-    return data.tag('div', time_value(format, unit, value), **attrs)
+    return data.tag('div', time_value(format_, unit, value), **attrs)
 
 
 factory.register(
     'time',
-    extractors=[generic_extractor, generic_required_extractor,
-                time_extractor],
+    extractors=[
+        generic_extractor,
+        generic_required_extractor,
+        time_extractor,
+        generic_emptyvalue_extractor
+    ],
     edit_renderers=[time_edit_renderer],
     display_renderers=[time_display_renderer])
 
-factory.doc['blueprint']['time'] = \
-"""Add-on blueprint `yafowil.widget.datetime 
-<http://github.com/bluedynamics/yafowil.widget.datetime/>`_ .
+factory.doc['blueprint']['time'] = """\
+Add-on blueprint `yafowil.widget.datetime
+<http://github.com/conestack/yafowil.widget.datetime/>`_ .
 """
 
 factory.defaults['time.default'] = ''
 
 factory.defaults['time.class'] = 'time'
 
 factory.defaults['time.required_class'] = 'required'
 
 factory.defaults['time.timeinput_class'] = 'timeinput'
-factory.doc['props']['time.timeinput_class'] = \
-"""CSS class rendered on time input field.
+factory.doc['props']['time.timeinput_class'] = """\
+CSS class rendered on time input field.
 """
 
 factory.defaults['time.timepicker_class'] = 'timepicker'
-factory.doc['props']['time.timepicker_class'] = \
-"""jquery.ui timepicker binds to this class.
+factory.doc['props']['time.timepicker_class'] = """\
+jquery.ui timepicker binds to this class.
 """
 
 factory.defaults['time.disabled'] = False
 
 factory.defaults['time.timepicker'] = False
-factory.doc['props']['time.timepicker'] = \
-"""Flag whether time picker is enabled.
+factory.doc['props']['time.timepicker'] = """\
+Flag whether time picker is enabled.
 """
 
 factory.defaults['time.format'] = 'string'
-factory.doc['props']['time.format'] = \
-"""Define widget value and extraction format. Either 'string', 'number' or
+factory.doc['props']['time.format'] = """\
+Define widget value and extraction format. Either 'string', 'number' or
 'tuple'.
 """
 
 factory.defaults['time.unit'] = 'hours'
-factory.doc['props']['time.unit'] = \
-"""Only considered if 'format' is 'number'. If unit is 'hours' value is float,
+factory.doc['props']['time.unit'] = """\
+Only considered if 'format' is 'number'. If unit is 'hours' value is float,
 otherwise integer.
 """
 
 factory.defaults['time.daytime'] = False
-factory.doc['props']['time.daytime'] = \
-"""Flag whether value is day of time. Setting this property or 'timepicker'
+factory.doc['props']['time.daytime'] = """\
+Flag whether value is day of time. Setting this property or 'timepicker'
 property above to True results in day time range validation.
 """
 
+factory.defaults['time.clock'] = '24'
+factory.doc['props']['time.clock'] = """\
+Defines which clock to use in timepicker. Either `24` for 24-hour-clock or `12`
+for 12-hour-clock. Defaults to `24`
+"""
+
+factory.defaults['time.locale'] = 'en'
+factory.doc['props']['time.locale'] = """\
+Widget locale. Used for translations in timepicker widget.
+"""
 
-@managedprops('required', 'time', 'locale', 'tzinfo')
+factory.defaults['time.minutes_step'] = '5'
+factory.doc['props']['time.minutes_step'] = """\
+Defines step between time options. Used in timepicker widget.
+"""
+
+
+@managedprops('required', 'time', 'locale', 'tzinfo', 'clock')
 def datetime_extractor(widget, data):
     time = None
     if attr_value('time', widget, data):
         time = data.request.get('{}.time'.format(widget.dottedpath))
     required = attr_value('required', widget, data)
     if not required and not data.extracted and not time:
         return ''
@@ -244,29 +288,30 @@
 
 
 def render_datetime_input(widget, data, date, time):
     tag = data.tag
     timeinput = ''
     if time:
         timeinput = render_time_input(widget, data, time, postfix='time')
-    additional_classes = [attr_value('dateinput_class', widget, data)]
-    datepicker = attr_value('datepicker', widget, data)
     disabled = attr_value('disabled', widget, data)
-    if datepicker and not disabled:
-        datepicker_class = attr_value('datepicker_class', widget, data)
-        additional_classes.append(datepicker_class)
     attrs = {
         'type': 'text',
-        'value':  date,
+        'value': date,
         'name_': widget.dottedpath,
         'id': cssid(widget, 'input'),
-        'class_': cssclasses(widget, data, additional=additional_classes),
         'size': 10,
-        'disabled': 'disabled' if disabled else None,
+        'disabled': 'disabled' if disabled else None
     }
+    additional_classes = [attr_value('dateinput_class', widget, data)]
+    datepicker = attr_value('datepicker', widget, data)
+    if datepicker and not disabled:
+        datepicker_class = attr_value('datepicker_class', widget, data)
+        additional_classes.append(datepicker_class)
+        attrs['data-date-locale'] = attr_value('locale', widget, data)
+    attrs['class_'] = cssclasses(widget, data, additional=additional_classes)
     return tag('input', **attrs) + timeinput
 
 
 @managedprops('locale', 'delimiter', 'time', 'disabled', 'timepicker',
               'timepicker_class', 'datepicker', 'datepicker_class',
               *css_managed_props)
 def datetime_edit_renderer(widget, data):
@@ -283,124 +328,150 @@
         if time:
             time = format_time(data.extracted)
     if not date:
         date = fetch_value(widget, data)
     return render_datetime_input(widget, data, date, time)
 
 
-@managedprops('format', 'class')
+@managedprops('format', 'class', 'unset_display_value')
 def datetime_display_renderer(widget, data, value=None):
     """Note: This renderer function optionally accepts value as parameter,
     which is used in favor of data.value if defined. Thus it can be used as
     utility function inside custom blueprints with the need of datetime
     display rendering.
     """
     value = value if value else data.value
     if not value:
-        return u''
-    format = widget.attrs['format']
-    if callable(format):
-        value = format(widget, data)
+        value = attr_value('empty_display_value', widget, data)
+        if not value:
+            return u''
     else:
-        value = value.strftime(format)
+        format_ = widget.attrs['format']
+        if callable(format_):
+            value = format_(widget, data)
+        else:
+            value = value.strftime(format_)
     attrs = {
         'id': cssid(widget, 'display'),
         'class_': 'display-{}'.format(attr_value('class', widget, data))
     }
     return data.tag('div', value, **attrs)
 
 
 factory.register(
     'datetime',
-    extractors=[generic_extractor, generic_required_extractor,
-                datetime_extractor],
+    extractors=[
+        generic_extractor,
+        generic_required_extractor,
+        datetime_extractor,
+        generic_emptyvalue_extractor
+    ],
     edit_renderers=[datetime_edit_renderer],
     display_renderers=[datetime_display_renderer])
 
-factory.doc['blueprint']['datetime'] = \
-"""Add-on blueprint `yafowil.widget.datetime 
-<http://github.com/bluedynamics/yafowil.widget.datetime/>`_ .
+factory.doc['blueprint']['datetime'] = """\
+Add-on blueprint `yafowil.widget.datetime
+<http://github.com/conestack/yafowil.widget.datetime/>`_ .
 """
 
 factory.defaults['datetime.default'] = ''
 
 factory.defaults['datetime.class'] = 'datetime'
 
 factory.defaults['datetime.required_class'] = 'required'
 
 factory.defaults['datetime.dateinput_class'] = 'dateinput'
-factory.doc['props']['datetime.dateinput_class'] = \
-"""CSS class rendered on date input field.
+factory.doc['props']['datetime.dateinput_class'] = """\
+CSS class rendered on date input field.
 """
 
 factory.defaults['datetime.datepicker_class'] = 'datepicker'
-factory.doc['props']['datetime.datepicker_class'] = \
-"""jquery.ui datepicker binds to this class.
+factory.doc['props']['datetime.datepicker_class'] = """\
+jquery.ui datepicker binds to this class.
 """
 
 factory.defaults['datetime.timeinput_class'] = 'timeinput'
-factory.doc['props']['datetime.timeinput_class'] = \
-"""CSS class rendered on time input field.
+factory.doc['props']['datetime.timeinput_class'] = """\
+CSS class rendered on time input field.
 """
 
 factory.defaults['datetime.timepicker_class'] = 'timepicker'
-factory.doc['props']['datetime.timepicker_class'] = \
-"""jquery.ui timepicker binds to this class.
+factory.doc['props']['datetime.timepicker_class'] = """\
+jquery.ui timepicker binds to this class.
 """
 
 factory.defaults['datetime.disabled'] = False
 
 factory.defaults['datetime.datepicker'] = False
-factory.doc['props']['datetime.datepicker_class'] = \
-"""Flag whether date picker is enabled.
+factory.doc['props']['datetime.datepicker_class'] = """\
+Flag whether date picker is enabled.
 """
 
 factory.defaults['datetime.time'] = False
-factory.doc['props']['datetime.time'] = \
-"""Flag whether time input should be rendered.
+factory.doc['props']['datetime.time'] = """\
+Flag whether time input should be rendered.
 
 ``time`` may be a callable taking widget and data as parameters expect to
 return a boolean.
 """
 
 factory.defaults['datetime.timepicker'] = False
-factory.doc['props']['datetime.timepicker'] = \
-"""Flag whether time picker is enabled.
+factory.doc['props']['datetime.timepicker'] = """\
+Flag whether time picker is enabled.
 """
 
 factory.defaults['datetime.datepicker'] = False
-factory.doc['props']['datetime.datepicker'] = \
-"""Flag whether date picker is enabled.
+factory.doc['props']['datetime.datepicker'] = """\
+Flag whether date picker is enabled.
+"""
+
+factory.defaults['datetime.clock'] = '24'
+factory.doc['props']['datetime.clock'] = """\
+Defines which clock to use in timepicker. Either `24` for 24-hour-clock or `12`
+for 12-hour-clock. Defaults to `24`
+"""
+
+factory.defaults['datetime.minutes_step'] = '5'
+factory.doc['props']['datetime.minutes_step'] = """\
+Defines step between time options. Defaults to 5.
 """
 
 factory.defaults['datetime.tzinfo'] = None
-factory.doc['props']['datetime.tzinfo'] = \
-"""Python datetime tzinfo object.
+factory.doc['props']['datetime.tzinfo'] = """\
+Python datetime tzinfo object.
 
-``tzinfo`` may be a callable taking widget and data as parameters expect to 
+``tzinfo`` may be a callable taking widget and data as parameters expect to
 return a tzinfo instance.
 """
 
-factory.defaults['datetime.locale'] = 'iso'
-factory.doc['props']['datetime.locale'] = \
-"""Date input format locale. ``yafowil.widget.datetime`` uses
-`bda.intellidatetime <http://pypi.python.org/pypi/bda.intellidatetime/>`_ for
-input parsing. Take a look at this package for available locales.
+factory.defaults['datetime.locale'] = 'en'
+factory.doc['props']['datetime.locale'] = """\
+Widget locale. Used for translations, calendar weekday start and date input
+format.
 
-``locale`` may be a callable taking widget and data as parameters expect to 
+``locale`` may be a callable taking widget and data as parameters expect to
 return a locale string.
+
+This widget uses
+`bda.intellidatetime <http://pypi.python.org/pypi/bda.intellidatetime/>`_ for
+input parsing. Take a look at this package for details about the parsing rules.
 """
 
 factory.defaults['datetime.delimiter'] = '.'
-factory.doc['props']['datetime.delimiter'] = \
-"""Delimiter used to render date in input field.
+factory.doc['props']['datetime.delimiter'] = """\
+Delimiter used to render date in input field.
 
-``delimiter`` may be a callable taking widget and data as parameters expect to 
+``delimiter`` may be a callable taking widget and data as parameters expect to
 return a delimiter string.
 """
 
 factory.defaults['datetime.format'] = '%Y.%m.%d %H:%M'
-factory.doc['props']['datetime.format'] = \
-"""Pattern accepted by ``datetime.strftime`` or callable taking widget and 
-data as parameters returning unicode or utf-8 string. Used if widget mode is 
+factory.doc['props']['datetime.format'] = """\
+Pattern accepted by ``datetime.strftime`` or callable taking widget and
+data as parameters returning unicode or utf-8 string. Used if widget mode is
 ``display``.
 """
+
+factory.defaults['datetime.empty_display_value'] = None
+factory.doc['props']['datetime.empty_display_value'] = """\
+Value to display if no datetime value set. Used if widget mode is ``display``.
+"""
```

### Comparing `yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/example.py` & `yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,146 @@
 from yafowil.base import factory
 
 
 DOC_DATE = """
-Date
-----
+Date Picker
+-----------
 
 Date input.
 
 .. code-block:: python
 
     date = factory('#field:datetime', props={
         'label': 'Enter date or use date picker',
         'required': 'Date Field is required',
-        'locale': 'de',
         'datepicker': True,
     })
 """
 
+
 def date_example():
     form = factory('fieldset', name='yafowil.widget.datetime.date')
     form['date'] = factory('#field:datetime', props={
         'label': 'Enter date or use date picker',
         'required': 'Date Field is required',
-        'locale': 'de',
         'datepicker': True,
     })
     return {
         'widget': form,
         'doc': DOC_DATE,
         'title': 'Date',
     }
 
 
 DOC_TIME = """
-Time
-----
+Time Picker
+-----------
 
 Time input.
 
+Set the 'clock' property to either 12 or 24 hours format (defaults to 24).
+
 .. code-block:: python
 
     time = factory('#field:time', props={
         'label': 'Select time',
         'required': 'Time Field is required',
         'timepicker': True,
+        'clock': '12'
     })
 """
 
+
 def time_example():
     form = factory('fieldset', name='yafowil.widget.datetime.time')
     form['time'] = factory('#field:time', props={
         'label': 'Select time',
         'required': 'Time Field is required',
         'timepicker': True,
+        'clock': '12'
     })
     return {
         'widget': form,
         'doc': DOC_TIME,
         'title': 'Time',
     }
 
 
+DOC_MINUTES = """
+Minutes
+-------
+
+Sets the interval for minute cells.
+
+Set the 'minutes_step' property to a number between 1 and 60 (defaults to 5).
+
+.. code-block:: python
+
+    time = factory('#field:time', props={
+        'label': 'Select time',
+        'required': 'Time Field is required',
+        'timepicker': True,
+        'clock': '24',
+        'minutes_step': '15'
+    })
+"""
+
+
+def minutes_example():
+    form = factory('fieldset', name='yafowil.widget.datetime.minutes_step')
+    form['time'] = factory('#field:time', props={
+        'label': 'Select time',
+        'required': 'Time Field is required',
+        'timepicker': True,
+        'clock': '24',
+        'minutes_step': '15'
+    })
+    return {
+        'widget': form,
+        'doc': DOC_MINUTES,
+        'title': 'Minutes'
+    }
+
+
 DOC_DATETIME = """
-Datetime
---------
+Datetime Picker
+---------------
 
 Date and time input.
 
 .. code-block:: python
 
     datetime = factory('#field:datetime', props={
         'label': 'Enter date and time',
         'required': 'Datetime Field is required',
         'locale': 'de',
         'datepicker': True,
         'time': True,
-        'timepicker': True,
+        'timepicker': True
     })
 """
 
+
 def datetime_example():
     form = factory('fieldset', name='yafowil.widget.datetime.datetime')
     form['datetime'] = factory('#field:datetime', props={
         'label': 'Enter date and time',
         'required': 'Datetime Field is required',
         'locale': 'de',
         'datepicker': True,
         'time': True,
-        'timepicker': True,
+        'timepicker': True
     })
     return {
         'widget': form,
         'doc': DOC_DATETIME,
-        'title': 'Datetime',
+        'title': 'Datetime'
     }
 
 
 def get_example():
     return [
         date_example(),
         time_example(),
-        datetime_example(),
+        minutes_example(),
+        datetime_example()
     ]
```

### Comparing `yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/yafowil.widget.datetime.po` & `yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/yafowil.widget.datetime.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/yafowil.widget.datetime.mo` & `yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/en/LC_MESSAGES/yafowil.widget.datetime.mo`

 * *Files identical despite different names*

### Comparing `yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/yafowil.widget.datetime.pot` & `yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/yafowil.widget.datetime.pot`

 * *Files identical despite different names*

### Comparing `yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/yafowil.widget.datetime.po` & `yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/yafowil.widget.datetime.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.datetime-1.9/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/yafowil.widget.datetime.mo` & `yafowil.widget.datetime-2.0a1/src/yafowil/widget/datetime/locales/de/LC_MESSAGES/yafowil.widget.datetime.mo`

 * *Files identical despite different names*

### Comparing `yafowil.widget.datetime-1.9/src/yafowil.widget.datetime.egg-info/PKG-INFO` & `yafowil.widget.datetime-2.0a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,280 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yafowil.widget.datetime
-Version: 1.9
+Version: 2.0a1
 Summary: Datetime Widget for YAFOWIL
-Home-page: http://pypi.python.org/pypi/yafowil.widget.datetime
-Author: BlueDynamics Alliance
-Author-email: dev@bluedynamics.com
+Home-page: http://github.com/conestack/yafowil.widget.datetime
+Author: Yafowil Contributors
+Author-email: dev@conestack.org
 License: Simplified BSD
-Description: This is a **datetime widget** for for `YAFOWIL 
-        <http://pypi.python.org/pypi/yafowil>`_ 
-        
-        It utilizes/integrates `jquery.ui.datepicker 
-        <http://docs.jquery.com/UI/Datepicker>`_ for/in YAFOWIL providing a 
-        datepicker function on a text input.
-        
-        - `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#datetime>`_
-        - `DEMO - see it Live <http://demo.yafowil.info/++widget++yafowil.widget.datetime/index.html>`_
-        
-        
-        Contributors
-        ============
-        
-        - Robert Niederrreiter <rnix [at] squarewave [dot] at>
-        
-        History
-        =======
-        
-        1.9 (2017-03-10)
-        ----------------
-        
-        - Add dedicated Plone 5 related CSS.
-          [rnix, 2017-03-06]
-        
-        - Introduce dedicated ``timeinput_class`` and ``dateinput_class`` widget
-          properties. Used for CSS styling. Styling was previously bound to
-          ``datepicker_class`` and ``timepicker_class`` class, but these are skipped
-          if no date and timepicker widgets should be displayed.
-          [rnix, 2017-03-06]
-        
-        - Change default ``datetime.delimiter`` to ``.``.
-          [rnix, 2017-03-06]
-        
-        - Change default ``datetime.format`` to ``%Y.%m.%d %H:%M``.
-          [rnix, 2017-03-06]
-        
-        
-        1.8 (2017-03-01)
-        ----------------
-        
-        - Add dedicated CSS for ``plone5`` theme provided by ``yafowil.plone``.
-          [rnix, 2016-06-28]
-        
-        - Use ``yafowil.utils.entry_point`` decorator.
-          [rnix, 2016-06-28]
-        
-        
-        1.7.1 (2015-06-25)
-        ------------------
-        
-        - Resolve JSHint errors and warnings.
-          [thet]
-        
-        
-        1.7 (2015-01-23)
-        ----------------
-        
-        - Remove calendar icon.
-          [rnix, 2014-07-29]
-        
-        - Update jquery UI datepicker to 1.10.3 and use latest jquery ui boostrap
-          styles.
-          [rnix, 2014-07-05]
-        
-        
-        1.6 (2014-06-03)
-        ----------------
-        
-        - Add translations, package depends now ``yafowil`` >= 2.1
-          [rnix, 2014-04-30]
-        
-        
-        1.5.2
-        -----
-        
-        - Restrict timepicker binding to context
-          [rnix, 2014-03-19]
-        
-        1.5.1
-        -----
-        
-        - Time blueprint example.
-          [rnix, 2012-11-03]
-        
-        1.5
-        ---
-        
-        - use ``yafowil.utils.attr_value`` wherever possible.
-          [rnix, 2012-10-25]
-        
-        - Add ``time`` blueprint.
-          [rnix, 2012-10-23]
-        
-        1.4
-        ---
-        
-        - Adopt resource providing
-          [rnix, 2012-06-12]
-        
-        - Add example widget
-          [rnix, 2012-06-12]
-        
-        1.3
-        ---
-        
-        - Sanitize formatting of date: iso always uses dash now, defaults to
-          international iso format using dash.
-          [jensens, 2012-05-09]
-        
-        - property ``format`` can be callable now. Expect to returns formatted date.
-          properties ``delimiter``, ``time``, ``tzinfo`` or ``locale`` can be callables
-          too now. All callables taking ``widget, data`` as parameters.
-          [jensens, 2012-05-09]
-        
-        - Add documentation for ``datetime`` blueprint properties.
-          [rnix, 2012-04-17]
-        
-        - Add ``delimiter`` blueprint property.
-          [rnix, 2012-04-17]
-        
-        1.2
-        ---
-        
-        - Add ``render_datetime_input`` and ``render_datetime_display`` helper
-          functions. Useful for custom widgets with different data preperation.
-          [rnix, 2012-03-06]
-        
-        - Modified to work with YAFOWIL 1.3
-          [agitator, 2012-02-19]
-        
-        - Extend display renderer to wrap value like ``generic_display_renderer``.
-          [rnix, 2011-12-18]
-        
-        - Add default css class to datetime blueprint.
-          [rnix, 2011-12-18]
-        
-        - Add datepicker binder function to ``yafowil.widget.array`` hooks if found.
-          [rnix, 2011-10-05]
-        
-        1.1
-        ---
-        
-        - Adopt to yafowil 1.2.
-          [jensens, 2011-09-20]
-        
-        - Make ready for z2c.autoinclude+Plone (only if available).
-          [jensens, 2011-09-20]
-        
-        1.0
-        ---
-        
-        - Add display renderer.
-          [rnix, 2011-08-04]
-        
-        - Adopt to yafowil 1.1.
-          [rnix, 2011-07-08]
-        
-        0.9.1
-        -----
-        
-        - Test coverage.
-          [rnix, 2011-05-07]
-        
-        0.9
-        ---
-        
-        - Made it work.
-          [rnix]
-        
-        License
-        =======
-        
-        Copyright (c) 2010-2017, BlueDynamics Alliance, Austria, Germany, Switzerland
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this 
-          list of conditions and the following disclaimer.
-        * Redistributions in binary form must reproduce the above copyright notice, this 
-          list of conditions and the following disclaimer in the documentation and/or 
-          other materials provided with the distribution.
-        * Neither the name of the BlueDynamics Alliance nor the names of its 
-          contributors may be used to endorse or promote products derived from this 
-          software without specific prior written permission.
-              
-        THIS SOFTWARE IS PROVIDED BY BlueDynamics Alliance ``AS IS`` AND ANY
-        EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL BlueDynamics Alliance BE LIABLE FOR ANY
-        DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-        ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-        (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-        SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: test
+License-File: LICENSE.rst
+
+This is a **datetime widget** for for `YAFOWIL 
+<http://pypi.python.org/pypi/yafowil>`_ 
+
+It utilizes
+`vanillajs datepicker <https://github.com/mymth/vanillajs-datepicker/releases/tag/v1.1.4>`_.
+Included are the basic datepicker Javascripts and a slightly modified version
+of the datepicker bootstrap CSS.
+
+- `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#datetime>`_
+- `DEMO - see it Live <http://demo.yafowil.info/++widget++yafowil.widget.datetime/index.html>`_
+
+
+Contributors
+============
+
+- Robert Niederrreiter
+
+- Georg Bernhard
+
+- Lena Daxenbichler
+
+
+Changes
+=======
+
+2.0a1 (2023-05-15)
+------------------
+
+- Add ``webresource`` support.
+  [rnix]
+
+- Prevent initialize if widget is part of array template.
+  [lenadax]
+
+- Extend JS by:
+  ``datepicker_on_array_add``,
+  ``timeepicker_on_array_add``,
+  ``register_datepicker_array_subscribers``,
+  ``register_timepicker_array_subscribers``
+  to enable usage in ``yafowil.widget.array``.
+  [lenadax]
+
+- Get rid of JQuery UI.
+  [lenadax]
+
+- Rewrite JavaScript using ES6. Utilize vanillajs-datepicker
+  [lenadax]
+
+
+1.12 (2020-07-09)
+-----------------
+
+- Add ``datetime.empty_display_value`` property.
+  [rnix]
+
+- Cast hour and minute values to int in ``time_value`` if ``format`` is
+  ``tuple``.
+  [rnix]
+
+- Do not mask built-in ``format`` function in ``widget`` module.
+  [rnix]
+
+
+1.11 (2018-11-07)
+-----------------
+
+- Add ``yafowil.common.generic_emptyvalue_extractor`` to ``time`` and
+  ``datetime`` blueprints.
+  [rnix]
+
+
+1.10 (2018-07-16)
+-----------------
+
+- Python 3 compatibility.
+  [rnix]
+
+- Convert doctests to unittests.
+  [rnix]
+
+
+1.9 (2017-03-10)
+----------------
+
+- Add dedicated Plone 5 related CSS.
+  [rnix, 2017-03-06]
+
+- Introduce dedicated ``timeinput_class`` and ``dateinput_class`` widget
+  properties. Used for CSS styling. Styling was previously bound to
+  ``datepicker_class`` and ``timepicker_class`` class, but these are skipped
+  if no date and timepicker widgets should be displayed.
+  [rnix, 2017-03-06]
+
+- Change default ``datetime.delimiter`` to ``.``.
+  [rnix, 2017-03-06]
+
+- Change default ``datetime.format`` to ``%Y.%m.%d %H:%M``.
+  [rnix, 2017-03-06]
+
+
+1.8 (2017-03-01)
+----------------
+
+- Add dedicated CSS for ``plone5`` theme provided by ``yafowil.plone``.
+  [rnix, 2016-06-28]
+
+- Use ``yafowil.utils.entry_point`` decorator.
+  [rnix, 2016-06-28]
+
+
+1.7.1 (2015-06-25)
+------------------
+
+- Resolve JSHint errors and warnings.
+  [thet]
+
+
+1.7 (2015-01-23)
+----------------
+
+- Remove calendar icon.
+  [rnix, 2014-07-29]
+
+- Update jquery UI datepicker to 1.10.3 and use latest jquery ui boostrap
+  styles.
+  [rnix, 2014-07-05]
+
+
+1.6 (2014-06-03)
+----------------
+
+- Add translations, package depends now ``yafowil`` >= 2.1
+  [rnix, 2014-04-30]
+
+
+1.5.2
+-----
+
+- Restrict timepicker binding to context
+  [rnix, 2014-03-19]
+
+1.5.1
+-----
+
+- Time blueprint example.
+  [rnix, 2012-11-03]
+
+1.5
+---
+
+- use ``yafowil.utils.attr_value`` wherever possible.
+  [rnix, 2012-10-25]
+
+- Add ``time`` blueprint.
+  [rnix, 2012-10-23]
+
+1.4
+---
+
+- Adopt resource providing
+  [rnix, 2012-06-12]
+
+- Add example widget
+  [rnix, 2012-06-12]
+
+1.3
+---
+
+- Sanitize formatting of date: iso always uses dash now, defaults to
+  international iso format using dash.
+  [jensens, 2012-05-09]
+
+- property ``format`` can be callable now. Expect to returns formatted date.
+  properties ``delimiter``, ``time``, ``tzinfo`` or ``locale`` can be callables
+  too now. All callables taking ``widget, data`` as parameters.
+  [jensens, 2012-05-09]
+
+- Add documentation for ``datetime`` blueprint properties.
+  [rnix, 2012-04-17]
+
+- Add ``delimiter`` blueprint property.
+  [rnix, 2012-04-17]
+
+1.2
+---
+
+- Add ``render_datetime_input`` and ``render_datetime_display`` helper
+  functions. Useful for custom widgets with different data preperation.
+  [rnix, 2012-03-06]
+
+- Modified to work with YAFOWIL 1.3
+  [agitator, 2012-02-19]
+
+- Extend display renderer to wrap value like ``generic_display_renderer``.
+  [rnix, 2011-12-18]
+
+- Add default css class to datetime blueprint.
+  [rnix, 2011-12-18]
+
+- Add datepicker binder function to ``yafowil.widget.array`` hooks if found.
+  [rnix, 2011-10-05]
+
+1.1
+---
+
+- Adopt to yafowil 1.2.
+  [jensens, 2011-09-20]
+
+- Make ready for z2c.autoinclude+Plone (only if available).
+  [jensens, 2011-09-20]
+
+1.0
+---
+
+- Add display renderer.
+  [rnix, 2011-08-04]
+
+- Adopt to yafowil 1.1.
+  [rnix, 2011-07-08]
+
+0.9.1
+-----
+
+- Test coverage.
+  [rnix, 2011-05-07]
+
+0.9
+---
+
+- Made it work.
+  [rnix]
+
+
+License
+=======
+
+Copyright (c) 2010-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
+Copyright (c) 2021-2022, Yafowil Contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `yafowil.widget.datetime-1.9/CHANGES.rst` & `yafowil.widget.datetime-2.0a1/CHANGES.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,66 @@
-
-History
+Changes
 =======
 
+2.0a1 (2023-05-15)
+------------------
+
+- Add ``webresource`` support.
+  [rnix]
+
+- Prevent initialize if widget is part of array template.
+  [lenadax]
+
+- Extend JS by:
+  ``datepicker_on_array_add``,
+  ``timeepicker_on_array_add``,
+  ``register_datepicker_array_subscribers``,
+  ``register_timepicker_array_subscribers``
+  to enable usage in ``yafowil.widget.array``.
+  [lenadax]
+
+- Get rid of JQuery UI.
+  [lenadax]
+
+- Rewrite JavaScript using ES6. Utilize vanillajs-datepicker
+  [lenadax]
+
+
+1.12 (2020-07-09)
+-----------------
+
+- Add ``datetime.empty_display_value`` property.
+  [rnix]
+
+- Cast hour and minute values to int in ``time_value`` if ``format`` is
+  ``tuple``.
+  [rnix]
+
+- Do not mask built-in ``format`` function in ``widget`` module.
+  [rnix]
+
+
+1.11 (2018-11-07)
+-----------------
+
+- Add ``yafowil.common.generic_emptyvalue_extractor`` to ``time`` and
+  ``datetime`` blueprints.
+  [rnix]
+
+
+1.10 (2018-07-16)
+-----------------
+
+- Python 3 compatibility.
+  [rnix]
+
+- Convert doctests to unittests.
+  [rnix]
+
+
 1.9 (2017-03-10)
 ----------------
 
 - Add dedicated Plone 5 related CSS.
   [rnix, 2017-03-06]
 
 - Introduce dedicated ``timeinput_class`` and ``dateinput_class`` widget
```

### Comparing `yafowil.widget.datetime-1.9/PKG-INFO` & `yafowil.widget.datetime-2.0a1/src/yafowil.widget.datetime.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,280 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yafowil.widget.datetime
-Version: 1.9
+Version: 2.0a1
 Summary: Datetime Widget for YAFOWIL
-Home-page: http://pypi.python.org/pypi/yafowil.widget.datetime
-Author: BlueDynamics Alliance
-Author-email: dev@bluedynamics.com
+Home-page: http://github.com/conestack/yafowil.widget.datetime
+Author: Yafowil Contributors
+Author-email: dev@conestack.org
 License: Simplified BSD
-Description: This is a **datetime widget** for for `YAFOWIL 
-        <http://pypi.python.org/pypi/yafowil>`_ 
-        
-        It utilizes/integrates `jquery.ui.datepicker 
-        <http://docs.jquery.com/UI/Datepicker>`_ for/in YAFOWIL providing a 
-        datepicker function on a text input.
-        
-        - `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#datetime>`_
-        - `DEMO - see it Live <http://demo.yafowil.info/++widget++yafowil.widget.datetime/index.html>`_
-        
-        
-        Contributors
-        ============
-        
-        - Robert Niederrreiter <rnix [at] squarewave [dot] at>
-        
-        History
-        =======
-        
-        1.9 (2017-03-10)
-        ----------------
-        
-        - Add dedicated Plone 5 related CSS.
-          [rnix, 2017-03-06]
-        
-        - Introduce dedicated ``timeinput_class`` and ``dateinput_class`` widget
-          properties. Used for CSS styling. Styling was previously bound to
-          ``datepicker_class`` and ``timepicker_class`` class, but these are skipped
-          if no date and timepicker widgets should be displayed.
-          [rnix, 2017-03-06]
-        
-        - Change default ``datetime.delimiter`` to ``.``.
-          [rnix, 2017-03-06]
-        
-        - Change default ``datetime.format`` to ``%Y.%m.%d %H:%M``.
-          [rnix, 2017-03-06]
-        
-        
-        1.8 (2017-03-01)
-        ----------------
-        
-        - Add dedicated CSS for ``plone5`` theme provided by ``yafowil.plone``.
-          [rnix, 2016-06-28]
-        
-        - Use ``yafowil.utils.entry_point`` decorator.
-          [rnix, 2016-06-28]
-        
-        
-        1.7.1 (2015-06-25)
-        ------------------
-        
-        - Resolve JSHint errors and warnings.
-          [thet]
-        
-        
-        1.7 (2015-01-23)
-        ----------------
-        
-        - Remove calendar icon.
-          [rnix, 2014-07-29]
-        
-        - Update jquery UI datepicker to 1.10.3 and use latest jquery ui boostrap
-          styles.
-          [rnix, 2014-07-05]
-        
-        
-        1.6 (2014-06-03)
-        ----------------
-        
-        - Add translations, package depends now ``yafowil`` >= 2.1
-          [rnix, 2014-04-30]
-        
-        
-        1.5.2
-        -----
-        
-        - Restrict timepicker binding to context
-          [rnix, 2014-03-19]
-        
-        1.5.1
-        -----
-        
-        - Time blueprint example.
-          [rnix, 2012-11-03]
-        
-        1.5
-        ---
-        
-        - use ``yafowil.utils.attr_value`` wherever possible.
-          [rnix, 2012-10-25]
-        
-        - Add ``time`` blueprint.
-          [rnix, 2012-10-23]
-        
-        1.4
-        ---
-        
-        - Adopt resource providing
-          [rnix, 2012-06-12]
-        
-        - Add example widget
-          [rnix, 2012-06-12]
-        
-        1.3
-        ---
-        
-        - Sanitize formatting of date: iso always uses dash now, defaults to
-          international iso format using dash.
-          [jensens, 2012-05-09]
-        
-        - property ``format`` can be callable now. Expect to returns formatted date.
-          properties ``delimiter``, ``time``, ``tzinfo`` or ``locale`` can be callables
-          too now. All callables taking ``widget, data`` as parameters.
-          [jensens, 2012-05-09]
-        
-        - Add documentation for ``datetime`` blueprint properties.
-          [rnix, 2012-04-17]
-        
-        - Add ``delimiter`` blueprint property.
-          [rnix, 2012-04-17]
-        
-        1.2
-        ---
-        
-        - Add ``render_datetime_input`` and ``render_datetime_display`` helper
-          functions. Useful for custom widgets with different data preperation.
-          [rnix, 2012-03-06]
-        
-        - Modified to work with YAFOWIL 1.3
-          [agitator, 2012-02-19]
-        
-        - Extend display renderer to wrap value like ``generic_display_renderer``.
-          [rnix, 2011-12-18]
-        
-        - Add default css class to datetime blueprint.
-          [rnix, 2011-12-18]
-        
-        - Add datepicker binder function to ``yafowil.widget.array`` hooks if found.
-          [rnix, 2011-10-05]
-        
-        1.1
-        ---
-        
-        - Adopt to yafowil 1.2.
-          [jensens, 2011-09-20]
-        
-        - Make ready for z2c.autoinclude+Plone (only if available).
-          [jensens, 2011-09-20]
-        
-        1.0
-        ---
-        
-        - Add display renderer.
-          [rnix, 2011-08-04]
-        
-        - Adopt to yafowil 1.1.
-          [rnix, 2011-07-08]
-        
-        0.9.1
-        -----
-        
-        - Test coverage.
-          [rnix, 2011-05-07]
-        
-        0.9
-        ---
-        
-        - Made it work.
-          [rnix]
-        
-        License
-        =======
-        
-        Copyright (c) 2010-2017, BlueDynamics Alliance, Austria, Germany, Switzerland
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this 
-          list of conditions and the following disclaimer.
-        * Redistributions in binary form must reproduce the above copyright notice, this 
-          list of conditions and the following disclaimer in the documentation and/or 
-          other materials provided with the distribution.
-        * Neither the name of the BlueDynamics Alliance nor the names of its 
-          contributors may be used to endorse or promote products derived from this 
-          software without specific prior written permission.
-              
-        THIS SOFTWARE IS PROVIDED BY BlueDynamics Alliance ``AS IS`` AND ANY
-        EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL BlueDynamics Alliance BE LIABLE FOR ANY
-        DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-        ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-        (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-        SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: test
+License-File: LICENSE.rst
+
+This is a **datetime widget** for for `YAFOWIL 
+<http://pypi.python.org/pypi/yafowil>`_ 
+
+It utilizes
+`vanillajs datepicker <https://github.com/mymth/vanillajs-datepicker/releases/tag/v1.1.4>`_.
+Included are the basic datepicker Javascripts and a slightly modified version
+of the datepicker bootstrap CSS.
+
+- `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#datetime>`_
+- `DEMO - see it Live <http://demo.yafowil.info/++widget++yafowil.widget.datetime/index.html>`_
+
+
+Contributors
+============
+
+- Robert Niederrreiter
+
+- Georg Bernhard
+
+- Lena Daxenbichler
+
+
+Changes
+=======
+
+2.0a1 (2023-05-15)
+------------------
+
+- Add ``webresource`` support.
+  [rnix]
+
+- Prevent initialize if widget is part of array template.
+  [lenadax]
+
+- Extend JS by:
+  ``datepicker_on_array_add``,
+  ``timeepicker_on_array_add``,
+  ``register_datepicker_array_subscribers``,
+  ``register_timepicker_array_subscribers``
+  to enable usage in ``yafowil.widget.array``.
+  [lenadax]
+
+- Get rid of JQuery UI.
+  [lenadax]
+
+- Rewrite JavaScript using ES6. Utilize vanillajs-datepicker
+  [lenadax]
+
+
+1.12 (2020-07-09)
+-----------------
+
+- Add ``datetime.empty_display_value`` property.
+  [rnix]
+
+- Cast hour and minute values to int in ``time_value`` if ``format`` is
+  ``tuple``.
+  [rnix]
+
+- Do not mask built-in ``format`` function in ``widget`` module.
+  [rnix]
+
+
+1.11 (2018-11-07)
+-----------------
+
+- Add ``yafowil.common.generic_emptyvalue_extractor`` to ``time`` and
+  ``datetime`` blueprints.
+  [rnix]
+
+
+1.10 (2018-07-16)
+-----------------
+
+- Python 3 compatibility.
+  [rnix]
+
+- Convert doctests to unittests.
+  [rnix]
+
+
+1.9 (2017-03-10)
+----------------
+
+- Add dedicated Plone 5 related CSS.
+  [rnix, 2017-03-06]
+
+- Introduce dedicated ``timeinput_class`` and ``dateinput_class`` widget
+  properties. Used for CSS styling. Styling was previously bound to
+  ``datepicker_class`` and ``timepicker_class`` class, but these are skipped
+  if no date and timepicker widgets should be displayed.
+  [rnix, 2017-03-06]
+
+- Change default ``datetime.delimiter`` to ``.``.
+  [rnix, 2017-03-06]
+
+- Change default ``datetime.format`` to ``%Y.%m.%d %H:%M``.
+  [rnix, 2017-03-06]
+
+
+1.8 (2017-03-01)
+----------------
+
+- Add dedicated CSS for ``plone5`` theme provided by ``yafowil.plone``.
+  [rnix, 2016-06-28]
+
+- Use ``yafowil.utils.entry_point`` decorator.
+  [rnix, 2016-06-28]
+
+
+1.7.1 (2015-06-25)
+------------------
+
+- Resolve JSHint errors and warnings.
+  [thet]
+
+
+1.7 (2015-01-23)
+----------------
+
+- Remove calendar icon.
+  [rnix, 2014-07-29]
+
+- Update jquery UI datepicker to 1.10.3 and use latest jquery ui boostrap
+  styles.
+  [rnix, 2014-07-05]
+
+
+1.6 (2014-06-03)
+----------------
+
+- Add translations, package depends now ``yafowil`` >= 2.1
+  [rnix, 2014-04-30]
+
+
+1.5.2
+-----
+
+- Restrict timepicker binding to context
+  [rnix, 2014-03-19]
+
+1.5.1
+-----
+
+- Time blueprint example.
+  [rnix, 2012-11-03]
+
+1.5
+---
+
+- use ``yafowil.utils.attr_value`` wherever possible.
+  [rnix, 2012-10-25]
+
+- Add ``time`` blueprint.
+  [rnix, 2012-10-23]
+
+1.4
+---
+
+- Adopt resource providing
+  [rnix, 2012-06-12]
+
+- Add example widget
+  [rnix, 2012-06-12]
+
+1.3
+---
+
+- Sanitize formatting of date: iso always uses dash now, defaults to
+  international iso format using dash.
+  [jensens, 2012-05-09]
+
+- property ``format`` can be callable now. Expect to returns formatted date.
+  properties ``delimiter``, ``time``, ``tzinfo`` or ``locale`` can be callables
+  too now. All callables taking ``widget, data`` as parameters.
+  [jensens, 2012-05-09]
+
+- Add documentation for ``datetime`` blueprint properties.
+  [rnix, 2012-04-17]
+
+- Add ``delimiter`` blueprint property.
+  [rnix, 2012-04-17]
+
+1.2
+---
+
+- Add ``render_datetime_input`` and ``render_datetime_display`` helper
+  functions. Useful for custom widgets with different data preperation.
+  [rnix, 2012-03-06]
+
+- Modified to work with YAFOWIL 1.3
+  [agitator, 2012-02-19]
+
+- Extend display renderer to wrap value like ``generic_display_renderer``.
+  [rnix, 2011-12-18]
+
+- Add default css class to datetime blueprint.
+  [rnix, 2011-12-18]
+
+- Add datepicker binder function to ``yafowil.widget.array`` hooks if found.
+  [rnix, 2011-10-05]
+
+1.1
+---
+
+- Adopt to yafowil 1.2.
+  [jensens, 2011-09-20]
+
+- Make ready for z2c.autoinclude+Plone (only if available).
+  [jensens, 2011-09-20]
+
+1.0
+---
+
+- Add display renderer.
+  [rnix, 2011-08-04]
+
+- Adopt to yafowil 1.1.
+  [rnix, 2011-07-08]
+
+0.9.1
+-----
+
+- Test coverage.
+  [rnix, 2011-05-07]
+
+0.9
+---
+
+- Made it work.
+  [rnix]
+
+
+License
+=======
+
+Copyright (c) 2010-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
+Copyright (c) 2021-2022, Yafowil Contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

