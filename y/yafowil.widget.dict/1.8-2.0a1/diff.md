# Comparing `tmp/yafowil.widget.dict-1.8.tar.gz` & `tmp/yafowil.widget.dict-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yafowil.widget.dict-1.8.tar", last modified: Thu Jul  9 11:47:00 2020, max compression
+gzip compressed data, was "yafowil.widget.dict-2.0a1.tar", last modified: Mon May 15 12:43:24 2023, max compression
```

## Comparing `yafowil.widget.dict-1.8.tar` & `yafowil.widget.dict-2.0a1.tar`

### file list

```diff
@@ -1,61 +1,51 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1536 2020-07-06 05:15:27.000000 yafowil.widget.dict-1.8/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1732 2020-07-09 11:46:07.000000 yafowil.widget.dict-1.8/setup.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2368 2020-07-09 11:46:32.000000 yafowil.widget.dict-1.8/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      682 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/buildout.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)      119 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/MANIFEST.in
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)      287 2020-02-03 10:06:57.000000 yafowil.widget.dict-1.8/bootstrap.sh
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1394 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/i18n.sh
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1741 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2019-04-25 18:08:04.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      124 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       48 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/top_level.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6638 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil.widget.dict.egg-info/PKG-INFO
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/__pycache__/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      238 2020-02-26 06:52:26.000000 yafowil.widget.dict-1.8/src/yafowil/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/__pycache__/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      245 2020-02-26 06:52:26.000000 yafowil.widget.dict-1.8/src/yafowil/widget/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1071 2020-07-06 05:15:27.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6693 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/widget.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/bootstrap/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      911 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/bootstrap/widget.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      382 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/icon_up_disabled.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      221 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/icon_remove.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      584 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/icon_down.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      392 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/icon_down_disabled.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      403 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/icon_add.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      560 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/icon_up.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      985 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/widget.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/plone5/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1613 2019-04-25 18:07:46.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/plone5/widget.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/__pycache__/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5625 2020-02-26 06:52:26.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/__pycache__/widget.cpython-37.pyc
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2112 2020-02-26 06:52:26.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/__pycache__/example.cpython-37.pyc
--rw-r--r--   0 rnix      (1000) rnix      (1000)      968 2020-07-07 09:01:37.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      843 2020-02-03 10:06:57.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/de/LC_MESSAGES/yafowil.widget.dict.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      804 2020-02-03 10:06:57.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/en/LC_MESSAGES/yafowil.widget.dict.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)      650 2020-02-03 10:06:57.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/yafowil.widget.dict.pot
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8085 2020-02-03 10:06:57.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/widget.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23588 2020-07-06 05:15:27.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1997 2020-02-03 10:06:57.000000 yafowil.widget.dict-1.8/src/yafowil/widget/dict/example.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      379 2020-07-09 11:46:14.000000 yafowil.widget.dict-1.8/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6638 2020-07-09 11:47:00.000000 yafowil.widget.dict-1.8/PKG-INFO
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2819 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      119 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5412 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      402 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1753 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.455559 yafowil.widget.dict-2.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4175 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1997 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.455559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      843 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/de/LC_MESSAGES/yafowil.widget.dict.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.455559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      804 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/en/LC_MESSAGES/yafowil.widget.dict.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      650 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/yafowil.widget.dict.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/bootstrap/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1005 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/bootstrap/widget.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      403 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/icon_add.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      584 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/icon_down.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      392 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/icon_down_disabled.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      221 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/icon_remove.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      560 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/icon_up.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      382 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/icon_up_disabled.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1079 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/widget.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/plone5/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1707 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/plone5/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7024 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3483 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/widget.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    25846 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9956 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:43:24.459559 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5412 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1475 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      107 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:43:24.000000 yafowil.widget.dict-2.0a1/src/yafowil.widget.dict.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yafowil.widget.dict-1.8/LICENSE.rst` & `yafowil.widget.dict-2.0a1/LICENSE.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,27 @@
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

### Comparing `yafowil.widget.dict-1.8/setup.py` & `yafowil.widget.dict-2.0a1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.8'
+version = '2.0a1'
 shortdesc = 'Dict/Mapping Widget for YAFOWIL'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
-tests_require = ['yafowil[test]']
 
 
 setup(
     name='yafowil.widget.dict',
     version=version,
     description=shortdesc,
     long_description=longdesc,
@@ -31,31 +30,35 @@
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     keywords='yafowil form widget dict mapping',
-    author='BlueDynamics Alliance',
-    author_email='dev@bluedynamics.com',
-    url=u'http://pypi.python.org/pypi/yafowil.widget.dict',
+    author='Yafowil Contributors',
+    author_email='dev@conestack.org',
+    url=u'http://github.com/conestack/yafowil.widget.dict',
     license='Simplified BSD',
     packages=find_packages('src'),
     package_dir={'': 'src'},
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
     test_suite="yafowil.widget.dict.tests",
     entry_points="""
     [yafowil.plugin]
     register = yafowil.widget.dict:register
     example = yafowil.widget.dict.example:get_example
     """
 )
```

### Comparing `yafowil.widget.dict-1.8/CHANGES.rst` & `yafowil.widget.dict-2.0a1/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 Changes
 =======
 
+2.0a1 (2023-05-15)
+------------------
+
+- Add ``webresource`` support.
+  [rnix]
+
+- Extend JS by ``dict_on_array_add`` and ``register_array_subscribers``
+  functions to enable usage in ``yafowil.widget.array``.
+  [lenadax]
+
+- Add support for key and value datatypes.
+  [rnix]
+
+- Rewrite JavaScript using ES6.
+  [rnix]
+
+- Remove B/C property callback tests. Property callbacks always
+  gets passed ``widget`` and ``data`` as of yafowil 3.0.0.
+  [rnix]
+
+
 1.8 (2020-07-09)
 ----------------
 
 - Fix re-rendering of widget if values required but empty dict passed.
   [rnix]
 
 - Remove ``dict_builder``. Entire widget is rendered now in ``dict_renderer``
```

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/icon_down.png` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/icon_down.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/images/icon_up.png` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/images/icon_up.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/default/widget.css` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/default/widget.css`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 .dict_actions a {
     line-height:16px;
     font-size:16px;
     padding-left:16px;
     text-decoration:none;
     float:right;
     margin-top:1px;
+    background: none;
+}
+.dict_actions span {
+    color: var(--yafowil-accent-color, #0d6efd);
 }
 .dict_actions a.dict_row_add {
     background:url('images/icon_add.png') 50% 50% no-repeat;
 }
 .dict_actions a.dict_row_remove {
     background:url('images/icon_remove.png') 50% 50% no-repeat;
 }
```

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/resources/plone5/widget.css` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/resources/plone5/widget.css`

 * *Files 5% similar despite different names*

```diff
@@ -62,13 +62,17 @@
     display:inline-block;
     margin-top:0.3em;
     padding-right:0.45em;
     width:6.5em;
 }
 .dict_actions a {
     float:right;
+    background: none;
+}
+.dict_actions span {
+    color: var(--yafowil-accent-color, #0d6efd);
 }
 .dict_actions a.array_row_up_disabled,
 .dict_actions a.array_row_down_disabled {
     opacity:0.4;
     filter:alpha(opacity=40);
 }
```

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/de/LC_MESSAGES/yafowil.widget.dict.po` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/de/LC_MESSAGES/yafowil.widget.dict.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/en/LC_MESSAGES/yafowil.widget.dict.po` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/en/LC_MESSAGES/yafowil.widget.dict.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/locales/yafowil.widget.dict.pot` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/locales/yafowil.widget.dict.pot`

 * *Files identical despite different names*

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/tests.py` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,34 @@
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
 class TestDictWidget(YafowilTestCase):
 
     def setUp(self):
         super(TestDictWidget, self).setUp()
+        from yafowil.widget import dict
         from yafowil.widget.dict import widget
         reload(widget)
+        dict.register()
 
     def test_empty_dict(self):
         # Create empty Dict widget
         widget = factory(
             'dict',
             name='mydict',
             props={
@@ -38,15 +44,15 @@
             "      <class 'yafowil.base.Widget'>: row",
             "        <class 'yafowil.base.Widget'>: key",
             "        <class 'yafowil.base.Widget'>: value",
             "        <class 'yafowil.base.Widget'>: actions",
             "    <class 'yafowil.base.Widget'>: body",
             ""
         ])
-        self.check_output("""
+        self.checkOutput("""
         <div>
           <input class="hidden" id="input-mydict-exists"
                  name="mydict.exists" type="hidden" value="1"/>
           <table class="dictwidget key-keyfield value-valuefield"
                  id="dictwidget_mydict.entry">
             <thead>
               <tr>
@@ -75,27 +81,14 @@
                 'key_label': lambda w, d: 'Computed Key',
                 'value_label': lambda w, d: 'Computed Value'
             })
         rendered = fxml('<div>{}</div>'.format(widget()))
         self.assertTrue(rendered.find('Computed Key') > -1)
         self.assertTrue(rendered.find('Computed Value') > -1)
 
-    def test_key_label_and_value_label_bc_callables(self):
-        # test B/C callable signature
-        widget = factory(
-            'dict',
-            name='mydict',
-            props={
-                'key_label': lambda: 'B/C Computed Key',
-                'value_label': lambda: 'B/C Computed Value'
-            })
-        rendered = fxml('<div>{}</div>'.format(widget()))
-        self.assertTrue(rendered.find('B/C Computed Key') > -1)
-        self.assertTrue(rendered.find('B/C Computed Value') > -1)
-
     def test_bc_head_property(self):
         # Test B/C ``head`` property
         widget = factory(
             'dict',
             name='mydict',
             props={
                 'head': {
@@ -117,28 +110,14 @@
                     'value': lambda w, d: 'Computed B/C Value',
                 }
             })
         rendered = fxml('<div>{}</div>'.format(widget()))
         self.assertTrue(rendered.find('Computed B/C Key') > -1)
         self.assertTrue(rendered.find('Computed B/C Value') > -1)
 
-    def test_bc_head_property_bc_callables(self):
-        widget = factory(
-            'dict',
-            name='mydict',
-            props={
-                'head': {
-                    'key': lambda: 'B/C Computed B/C Key',
-                    'value': lambda: 'B/C Computed B/C Value',
-                }
-            })
-        rendered = fxml('<div>{}</div>'.format(widget()))
-        self.assertTrue(rendered.find('B/C Computed B/C Key') > -1)
-        self.assertTrue(rendered.find('B/C Computed B/C Value') > -1)
-
     def test_skip_labels(self):
         widget = factory('dict', name='mydict')
         rendered = fxml('<div>{}</div>'.format(widget()))
         # search for empty th
         index = rendered.find('<th> </th>')
         self.assertTrue(index > -1)
         # search for second empty th
@@ -171,15 +150,15 @@
             "        <class 'yafowil.base.Widget'>: actions",
             "      <class 'yafowil.base.Widget'>: entry1",
             "        <class 'yafowil.base.Widget'>: key",
             "        <class 'yafowil.base.Widget'>: value",
             "        <class 'yafowil.base.Widget'>: actions",
             ""
         ])
-        self.check_output("""
+        self.checkOutput("""
         <div>
           ...
           <tbody>
             <tr>
               <td class="key">
                 <input class="keyfield" id="input-mydict-entry0-key"
                        name="mydict.entry0.key" type="text" value="key1"/>
@@ -427,15 +406,15 @@
             "        <class 'yafowil.base.Widget'>: value",
             "    <class 'yafowil.base.Widget'>: body",
             "      <class 'yafowil.base.Widget'>: entry0",
             "        <class 'yafowil.base.Widget'>: key",
             "        <class 'yafowil.base.Widget'>: value",
             ""
         ])
-        self.check_output("""
+        self.checkOutput("""
         <div>
           <input class="hidden" id="input-mydict-exists"
                  name="mydict.exists" type="hidden" value="1"/>
           <table class="dictwidget key-keyfield value-valuefield"
                  id="dictwidget_mydict.entry">
             <thead>
               <tr>
@@ -543,25 +522,65 @@
         # check rendered
         rendered = widget(data=data)
         expected = '<div class="errormessage">'
         self.assertFalse(rendered.find(expected) > -1)
         expected = 'name="mydict.entry0.value" type="text" value="Value1"'
         self.assertTrue(rendered.find(expected) > -1)
 
+    def test_datatype_extraction(self):
+        widget = factory(
+            'error:dict',
+            name='mydict',
+            props={
+                'key_type': int,
+                'value_type': int
+            })
+        request = {
+            'mydict.exists': '1',
+            'mydict.entry0.key': '0',
+            'mydict.entry0.value': '1',
+        }
+        data = widget.extract(request=request)
+        self.assertFalse(data.has_errors)
+        self.assertEqual(
+            data.extracted,
+            odict([(0, 1)])
+        )
+        request = {
+            'mydict.exists': '1',
+            'mydict.entry0.key': 'a',
+            'mydict.entry0.value': '1',
+        }
+        data = widget.extract(request=request)
+        self.assertEqual(
+            data.errors,
+            [ExtractionError('Key a is not a valid integer.',)]
+        )
+        request = {
+            'mydict.exists': '1',
+            'mydict.entry0.key': '0',
+            'mydict.entry0.value': 'b',
+        }
+        data = widget.extract(request=request)
+        self.assertEqual(
+            data.errors,
+            [ExtractionError('Value b is not a valid integer.',)]
+        )
+
     def test_display_dict(self):
         widget = factory(
             'dict',
             name='display_dict',
             value=odict([('foo', 'Foo'), ('bar', 'Bar')]),
             props={
                 'key_label': 'Key',
                 'value_label': 'Value',
             },
             mode='display')
-        self.check_output("""
+        self.checkOutput("""
         <div>
           <h5>Key: Value</h5>
           <dl>
             <dt>foo</dt>
             <dd>Foo</dd>
             <dt>bar</dt>
             <dd>Bar</dd>
@@ -574,15 +593,15 @@
             'dict',
             name='display_dict',
             props={
                 'key_label': 'Key',
                 'value_label': 'Value'
             },
             mode='display')
-        self.check_output("""
+        self.checkOutput("""
         <div>
           <h5>Key: Value</h5>
           <dl/>
         </div>
         """, fxml('<div>{}</div>'.format(widget())))
 
     def test_display_callable_labels(self):
@@ -590,49 +609,33 @@
             'dict',
             name='display_dict',
             props={
                 'key_label': lambda w, d: 'Computed Key',
                 'value_label': lambda w, d: 'Computed Value'
             },
             mode='display')
-        self.check_output("""
+        self.checkOutput("""
         <div>
           <h5>Computed Key: Computed Value</h5>
           <dl/>
         </div>
         """, fxml('<div>{}</div>'.format(widget())))
 
-    def test_display_bc_callable_labels(self):
-        widget = factory(
-            'dict',
-            name='display_dict',
-            props={
-                'key_label': lambda: 'B/C Computed Key',
-                'value_label': lambda: 'B/C Computed Value'
-            },
-            mode='display')
-        self.check_output("""
-        <div>
-          <h5>B/C Computed Key: B/C Computed Value</h5>
-          <dl/>
-        </div>
-        """, fxml('<div>{}</div>'.format(widget())))
-
     def test_display_bc_labels(self):
         widget = factory(
             'dict',
             name='display_dict',
             props={
                 'head': {
                     'key': 'B/C Key',
                     'value': 'B/C Value',
                 }
             },
             mode='display')
-        self.check_output("""
+        self.checkOutput("""
         <div>
           <h5>B/C Key: B/C Value</h5>
           <dl/>
         </div>
         """, fxml('<div>{}</div>'.format(widget())))
 
     def test_display_computed_bc_labels(self):
@@ -642,47 +645,102 @@
             props={
                 'head': {
                     'key': lambda w, d: 'Computed B/C Key',
                     'value': lambda w, d: 'Computed B/C Value',
                 }
             },
             mode='display')
-        self.check_output("""
+        self.checkOutput("""
         <div>
           <h5>Computed B/C Key: Computed B/C Value</h5>
           <dl/>
         </div>
         """, fxml('<div>{}</div>'.format(widget())))
 
-    def test_display_bc_computed_bc_labels(self):
-        widget = factory(
-            'dict',
-            name='display_dict',
-            props={
-                'head': {
-                    'key': lambda: 'B/C Computed B/C Key',
-                    'value': lambda: 'B/C Computed B/C Value',
-                }
-            },
-            mode='display')
-        self.check_output("""
-        <div>
-          <h5>B/C Computed B/C Key: B/C Computed B/C Value</h5>
-          <dl/>
-        </div>
-        """, fxml('<div>{}</div>'.format(widget())))
-
     def test_display_renderer_no_labels(self):
         widget = factory(
             'dict',
             name='display_dict',
             mode='display'
         )
-        self.check_output("""
+        self.checkOutput("""
         <div>
           <dl/>
         </div>
         """, fxml('<div>{}</div>'.format(widget())))
 
+    def test_resources(self):
+        factory.theme = 'default'
+        resources = factory.get_resources('yafowil.widget.dict')
+        self.assertTrue(resources.directory.endswith(np('/dict/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.dict')
+        self.assertEqual(resources.path, 'yafowil-dict')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/dict/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-dict')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(
+            styles[0].directory.endswith(np('/dict/resources/default'))
+        )
+        self.assertEqual(styles[0].path, 'yafowil-dict/default')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
+        factory.theme = 'bootstrap3'
+        resources = factory.get_resources('yafowil.widget.dict')
+        self.assertTrue(resources.directory.endswith(np('/dict/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.dict')
+        self.assertEqual(resources.path, 'yafowil-dict')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/dict/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-dict')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(
+            styles[0].directory.endswith(np('/dict/resources/bootstrap'))
+        )
+        self.assertEqual(styles[0].path, 'yafowil-dict/bootstrap')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
+        factory.theme = 'plone5'
+        resources = factory.get_resources('yafowil.widget.dict')
+        self.assertTrue(resources.directory.endswith(np('/dict/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.dict')
+        self.assertEqual(resources.path, 'yafowil-dict')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(scripts[0].directory.endswith(np('/dict/resources')))
+        self.assertEqual(scripts[0].path, 'yafowil-dict')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(
+            styles[0].directory.endswith(np('/dict/resources/plone5'))
+        )
+        self.assertEqual(styles[0].path, 'yafowil-dict/plone5')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `yafowil.widget.dict-1.8/src/yafowil/widget/dict/example.py` & `yafowil.widget.dict-2.0a1/src/yafowil/widget/dict/example.py`

 * *Files identical despite different names*

