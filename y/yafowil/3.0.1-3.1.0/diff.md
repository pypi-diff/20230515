# Comparing `tmp/yafowil-3.0.1.tar.gz` & `tmp/yafowil-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafowil-3.0.1.tar", last modified: Mon Dec  5 11:59:41 2022, max compression
+gzip compressed data, was "yafowil-3.1.0.tar", last modified: Mon May 15 12:22:22 2023, max compression
```

## Comparing `yafowil-3.0.1.tar` & `yafowil-3.1.0.tar`

### file list

```diff
@@ -1,55 +1,89 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.232810 yafowil-3.0.1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    16313 2022-12-05 11:59:41.000000 yafowil-3.0.1/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1404 2022-12-05 11:59:41.000000 yafowil-3.0.1/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       86 2022-12-05 11:59:41.000000 yafowil-3.0.1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)    26509 2022-12-05 11:59:41.232810 yafowil-3.0.1/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1825 2022-12-05 11:59:41.000000 yafowil-3.0.1/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2022-12-05 11:59:41.232810 yafowil-3.0.1/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2035 2022-12-05 11:59:41.000000 yafowil-3.0.1/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.228810 yafowil-3.0.1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.232810 yafowil-3.0.1/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      100 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    29701 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/base.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    76554 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/common.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      291 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/compat.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9002 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/compound.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1877 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/controller.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8733 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/example.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.232810 yafowil-3.0.1/src/yafowil/i18n/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       24 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/i18n/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.232810 yafowil-3.0.1/src/yafowil/i18n/locales/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.228810 yafowil-3.0.1/src/yafowil/i18n/locales/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.232810 yafowil-3.0.1/src/yafowil/i18n/locales/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2207 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/i18n/locales/de/LC_MESSAGES/yafowil.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4455 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/i18n/locales/de/LC_MESSAGES/yafowil.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.228810 yafowil-3.0.1/src/yafowil/i18n/locales/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.232810 yafowil-3.0.1/src/yafowil/i18n/locales/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2115 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/i18n/locales/en/LC_MESSAGES/yafowil.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4364 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/i18n/locales/en/LC_MESSAGES/yafowil.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3719 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/i18n/locales/yafowil.pot
--rw-r--r--   0 rnix      (1000) rnix      (1000)      595 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/loader.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      875 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/persistence.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2784 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/resources.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5308 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/table.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.232810 yafowil-3.0.1/src/yafowil/tests/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2012 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    39086 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_base.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)   146825 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_common.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    31511 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_compound.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7714 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_controller.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7304 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_persistence.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2178 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_resources.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10316 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_table.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      516 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_tsf.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    24553 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tests/test_utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1072 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/tsf.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    13944 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil/utils.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-12-05 11:59:41.232810 yafowil-3.0.1/src/yafowil.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    26509 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1255 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      107 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2022-12-05 11:59:41.000000 yafowil-3.0.1/src/yafowil.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.020044 yafowil-3.1.0/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17505 2023-05-15 12:22:17.000000 yafowil-3.1.0/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1404 2022-04-02 11:07:40.000000 yafowil-3.1.0/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       86 2022-04-02 11:07:40.000000 yafowil-3.1.0/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    28069 2023-05-15 12:22:22.020044 yafowil-3.1.0/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1825 2022-04-02 11:07:40.000000 yafowil-3.1.0/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-05-15 12:22:22.020044 yafowil-3.1.0/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2035 2023-05-15 12:11:43.000000 yafowil-3.1.0/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.016044 yafowil-3.1.0/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.016044 yafowil-3.1.0/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      100 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    29715 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/base.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9006 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/button.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5624 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/checkbox.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    16661 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/common.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      291 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/compat.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9002 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/compound.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1877 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/controller.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10301 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/datatypes.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1946 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/email.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8733 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/example.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7324 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/field.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6980 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/file.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1050 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/hidden.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.020044 yafowil-3.1.0/src/yafowil/i18n/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       24 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/i18n/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.020044 yafowil-3.1.0/src/yafowil/i18n/locales/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.016044 yafowil-3.1.0/src/yafowil/i18n/locales/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.020044 yafowil-3.1.0/src/yafowil/i18n/locales/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2382 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/i18n/locales/de/LC_MESSAGES/yafowil.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4594 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/i18n/locales/de/LC_MESSAGES/yafowil.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.016044 yafowil-3.1.0/src/yafowil/i18n/locales/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.020044 yafowil-3.1.0/src/yafowil/i18n/locales/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2277 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/i18n/locales/en/LC_MESSAGES/yafowil.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4490 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/i18n/locales/en/LC_MESSAGES/yafowil.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3771 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/i18n/locales/yafowil.pot
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2995 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/lines.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1032 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/loader.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3839 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/number.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6181 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/password.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      875 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/persistence.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1580 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/proxy.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2784 2022-10-28 06:29:53.000000 yafowil-3.1.0/src/yafowil/resources.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1097 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/search.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    13813 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/select.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5332 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/table.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1205 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tag.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.020044 yafowil-3.1.0/src/yafowil/tests/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4577 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    39146 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_base.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4227 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_button.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12707 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_checkbox.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11653 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_common.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    31457 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_compound.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7660 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_controller.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    29324 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_datatypes.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3555 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_email.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7288 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_field.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10124 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_file.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3084 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_hidden.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6443 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_lines.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6445 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_number.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5725 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_password.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7274 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_persistence.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2707 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_proxy.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2178 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/tests/test_resources.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1600 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_search.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    56659 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_select.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10241 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_table.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      810 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_tag.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2097 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_text.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2185 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_textarea.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      526 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_tsf.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2258 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_url.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12815 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/tests/test_utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1720 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/text.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3251 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/textarea.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1072 2022-04-02 11:07:40.000000 yafowil-3.1.0/src/yafowil/tsf.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1687 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/url.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12194 2023-05-04 15:16:54.000000 yafowil-3.1.0/src/yafowil/utils.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:22:22.016044 yafowil-3.1.0/src/yafowil.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    28069 2023-05-15 12:22:22.000000 yafowil-3.1.0/src/yafowil.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2180 2023-05-15 12:22:22.000000 yafowil-3.1.0/src/yafowil.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:22:22.000000 yafowil-3.1.0/src/yafowil.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      107 2023-05-15 12:22:22.000000 yafowil-3.1.0/src/yafowil.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:22:22.000000 yafowil-3.1.0/src/yafowil.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-04-02 11:08:02.000000 yafowil-3.1.0/src/yafowil.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2023-05-15 12:22:22.000000 yafowil-3.1.0/src/yafowil.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:22:22.000000 yafowil-3.1.0/src/yafowil.egg-info/top_level.txt
```

### Comparing `yafowil-3.0.1/CHANGES.rst` & `yafowil-3.1.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,57 @@
 
 History
 =======
 
+3.1.0 (2023-05-15)
+------------------
+
+- Refactor datatype conversion. Datatype related extractors and utils are
+  contained in ``yafowil.datatype`` now. Fix datatype conversion for ``bytes``
+  type.
+  [rnix]
+
+- Split up ``yafowil.common`` module [rnix]
+
+  - Move ``button`` and ``submit`` blueprints to ``yafowil.button``.
+
+  - Move ``checkbox`` blueprint to ``yafowil.checkbox``.
+
+  - Move ``email`` blueprint to ``yafowil.email``.
+
+  - Move ``field``, ``label``, ``help`` and ``error`` blueprints to ``yafowil.field``.
+
+  - Move ``file`` blueprint to ``yafowil.file``.
+
+  - Move ``hidden`` blueprint to ``yafowil.hidden``.
+
+  - Move ``lines`` blueprint to ``yafowil.lines``.
+
+  - Move ``number`` blueprint to ``yafowil.number``.
+
+  - Move ``password`` blueprint to ``yafowil.password``.
+
+  - Move ``proxy`` blueprint to ``yafowil.proxy``.
+
+  - Move ``search`` blueprint to ``yafowil.search``.
+
+  - Move ``select`` blueprint to ``yafowil.select``.
+
+  - Move ``tag`` blueprint to ``yafowil.tag``.
+
+  - Move ``text`` blueprint to ``yafowil.text``.
+
+  - Move ``textarea`` blueprint to ``yafowil.textarea``.
+
+  - Move ``url`` blueprint to ``yafowil.url``.
+
+- Tests work with pytest.
+  [rnix]
+
+
 3.0.1 (2022-12-05)
 ------------------
 
 - File extractor raises an ``ExtractionError`` if file action is ``replace``
   but no file is uploaded instead of silently changing the action to ``keep``.
   [rnix]
```

### Comparing `yafowil-3.0.1/LICENSE.rst` & `yafowil-3.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/PKG-INFO` & `yafowil-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yafowil
-Version: 3.0.1
+Version: 3.1.0
 Summary: YAFOWIL - declarative, framework independent, flexible HTML forms
 Home-page: http://github.com/conestack/yafowil
 Author: Yafowil Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Description: yafowil
         =======
@@ -69,14 +69,60 @@
         - Christian Scholz aka MrTopf
         
         
         
         History
         =======
         
+        3.1.0 (2023-05-15)
+        ------------------
+        
+        - Refactor datatype conversion. Datatype related extractors and utils are
+          contained in ``yafowil.datatype`` now. Fix datatype conversion for ``bytes``
+          type.
+          [rnix]
+        
+        - Split up ``yafowil.common`` module [rnix]
+        
+          - Move ``button`` and ``submit`` blueprints to ``yafowil.button``.
+        
+          - Move ``checkbox`` blueprint to ``yafowil.checkbox``.
+        
+          - Move ``email`` blueprint to ``yafowil.email``.
+        
+          - Move ``field``, ``label``, ``help`` and ``error`` blueprints to ``yafowil.field``.
+        
+          - Move ``file`` blueprint to ``yafowil.file``.
+        
+          - Move ``hidden`` blueprint to ``yafowil.hidden``.
+        
+          - Move ``lines`` blueprint to ``yafowil.lines``.
+        
+          - Move ``number`` blueprint to ``yafowil.number``.
+        
+          - Move ``password`` blueprint to ``yafowil.password``.
+        
+          - Move ``proxy`` blueprint to ``yafowil.proxy``.
+        
+          - Move ``search`` blueprint to ``yafowil.search``.
+        
+          - Move ``select`` blueprint to ``yafowil.select``.
+        
+          - Move ``tag`` blueprint to ``yafowil.tag``.
+        
+          - Move ``text`` blueprint to ``yafowil.text``.
+        
+          - Move ``textarea`` blueprint to ``yafowil.textarea``.
+        
+          - Move ``url`` blueprint to ``yafowil.url``.
+        
+        - Tests work with pytest.
+          [rnix]
+        
+        
         3.0.1 (2022-12-05)
         ------------------
         
         - File extractor raises an ``ExtractionError`` if file action is ``replace``
           but no file is uploaded instead of silently changing the action to ``keep``.
           [rnix]
```

### Comparing `yafowil-3.0.1/README.rst` & `yafowil-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/setup.py` & `yafowil-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '3.0.1'
+version = '3.1.0'
 shortdesc = 'YAFOWIL - declarative, framework independent, flexible HTML forms'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
 
@@ -51,15 +51,15 @@
     license='Simplified BSD',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['yafowil'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'node>=1.0',
+        'node>=1.2',
         'setuptools',
         'webresource'
     ],
     tests_require=[
         'lxml',
         'zope.testrunner'
     ],
```

### Comparing `yafowil-3.0.1/src/yafowil/base.py` & `yafowil-3.1.0/src/yafowil/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 from node.behaviors import Attributes
 from node.behaviors import DictStorage
 from node.behaviors import MappingAdopt
 from node.behaviors import MappingConstraints
 from node.behaviors import MappingNode
+from node.behaviors import MappingOrder
 from node.behaviors import NodeAttributes
 from node.behaviors import OdictStorage
-from node.behaviors import Order
 from node.utils import UNSET
 from node.utils import instance_property
 from plumber import plumbing
 from threading import RLock
 from yafowil.compat import ITER_TYPES
 from yafowil.compat import STR_TYPE
 from yafowil.utils import Tag
@@ -256,15 +256,15 @@
         ).format(name, self.parent.dottedpath))
 
 
 @plumbing(
     Attributes,
     MappingConstraints,
     MappingAdopt,
-    Order,
+    MappingOrder,
     MappingNode,
     OdictStorage)
 class Widget(object):
     """Base Widget Class.
     """
     attributes_factory = WidgetAttributes
```

### Comparing `yafowil-3.0.1/src/yafowil/compound.py` & `yafowil-3.1.0/src/yafowil/compound.py`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/src/yafowil/controller.py` & `yafowil-3.1.0/src/yafowil/controller.py`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/src/yafowil/example.py` & `yafowil-3.1.0/src/yafowil/example.py`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/src/yafowil/i18n/locales/de/LC_MESSAGES/yafowil.mo` & `yafowil-3.1.0/src/yafowil/i18n/locales/de/LC_MESSAGES/yafowil.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -35,20 +35,26 @@
 
 msgid "email_address_not_valid"
 msgstr "Eingabe ist keine gültige E-Mail Adresse."
 
 msgid "file_delete"
 msgstr "Lösche bestehende Datei"
 
+msgid "file_invalid_mimetype"
+msgstr "Ungültiger Dateityp hochgeladen"
+
 msgid "file_keep"
 msgstr "Behalte bestehende Datei"
 
 msgid "file_replace"
 msgstr "Ersetze bestehende Datei"
 
+msgid "file_replace_no_upload"
+msgstr "Datei kann nicht ersetzt werden. Keine Datei hochgeladen"
+
 msgid "filename"
 msgstr "Dateiname:"
 
 msgid "generic_datatype_message"
 msgstr "Eingabekonvertierung fehlgeschlagen"
 
 msgid "input_number_maximum_value"
```

### Comparing `yafowil-3.0.1/src/yafowil/i18n/locales/de/LC_MESSAGES/yafowil.po` & `yafowil-3.1.0/src/yafowil/i18n/locales/en/LC_MESSAGES/yafowil.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,183 +1,179 @@
-# German translations for yafowil.
+# English translations for yafowil.
 # Copyright (C) 2014 ORGANIZATION
 # This file is distributed under the same license as the yafowil project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2014.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: yafowil 2.1pre1\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-03-21 16:26+0100\n"
+"POT-Creation-Date: 2023-03-18 10:23+0100\n"
 "PO-Revision-Date: 2014-04-30 17:34+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: de <LL@li.org>\n"
+"Language-Team: en <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "Generated-By: Babel 1.3\n"
 
-#. Default: Mandatory field was empty
-#: src/yafowil/common.py:126
-msgid "required_message"
-msgstr "Feld erfordert eine Eingabe"
-
 #. Default: string
-#: src/yafowil/common.py:232
+#: src/yafowil/datatypes.py:194
 msgid "datatype_str"
-msgstr "ASCII Zeichenkette"
+msgstr "string"
 
 #. Default: unicode
-#: src/yafowil/common.py:233
+#: src/yafowil/datatypes.py:195
 msgid "datatype_unicode"
-msgstr "Zeichenkette"
+msgstr "unicode"
 
 #. Default: integer
-#: src/yafowil/common.py:234
+#: src/yafowil/datatypes.py:196
 msgid "datatype_integer"
-msgstr "Ganzzahl"
+msgstr "integer"
 
 #. Default: floating point number
-#: src/yafowil/common.py:235
+#: src/yafowil/datatypes.py:197
 msgid "datatype_float"
-msgstr "Gleitkommazahl"
+msgstr "floating point"
 
 #. Default: UUID
-#: src/yafowil/common.py:236
+#: src/yafowil/datatypes.py:198
 msgid "datatype_uuid"
 msgstr "UUID"
 
 #. Default: long integer
 #. pragma: no cover
-#: src/yafowil/common.py:239
+#: src/yafowil/datatypes.py:201
 msgid "datatype_long"
-msgstr "Ganzzahl"
+msgstr "integer"
 
 #. Default: Input conversion failed.
-#: src/yafowil/common.py:291
+#: src/yafowil/datatypes.py:259
 msgid "generic_datatype_message"
-msgstr "Eingabekonvertierung fehlgeschlagen"
+msgstr "Input conversion failed."
 
 #. Default: Input is not a valid ${datatype}.
-#: src/yafowil/common.py:298
+#: src/yafowil/datatypes.py:266
 msgid "standard_datatype_message"
-msgstr "Eingabe ist keine gültige ${datatype}."
+msgstr "Input is not a valid ${datatype}."
+
+#. Default: Mandatory field was empty
+#: src/yafowil/common.py:90
+msgid "required_message"
+msgstr "Mandatory field was empty"
 
 #. Default: Input must have at least ${len} characters.
-#: src/yafowil/common.py:801
+#: src/yafowil/common.py:707
 msgid "minlength_extraction_error"
-msgstr "Eingabe muss mindestens ${len} Zeichen lang sein."
+msgstr "Input must have at least ${len} characters."
 
 #. Default: Input contains illegal characters.
-#: src/yafowil/common.py:827
+#: src/yafowil/common.py:733
 msgid "ascii_extractor_error"
-msgstr "Eingabe enthält ungültige Zeichen"
+msgstr "Input contains illegal characters."
 
 #. Default: Password too weak
-#: src/yafowil/common.py:962
+#: src/yafowil/common.py:876
 msgid "weak_password_message"
-msgstr "Passwort zu schwach"
+msgstr "Password too weak"
 
 #. Default: Yes
-#: src/yafowil/common.py:1098
+#: src/yafowil/common.py:1022
 msgid "yes"
-msgstr "Ja"
+msgstr "Yes"
 
 #. Default: No
-#: src/yafowil/common.py:1099
+#: src/yafowil/common.py:1023
 msgid "no"
-msgstr "Nein"
+msgstr "No"
 
 #. Default: Unset
 #. XXX: never used right now?
-#: src/yafowil/common.py:1100
+#: src/yafowil/common.py:1024
 msgid "unset"
-msgstr "Ohne Wert"
+msgstr "Unset"
+
+#. Default: Cannot replace file. No file uploaded.
+#: src/yafowil/common.py:1453
+msgid "file_replace_no_upload"
+msgstr "Cannot replace file. No file uploaded."
+
+#. Default: Mimetype of uploaded file not matches
+#: src/yafowil/common.py:1487
+msgid "file_invalid_mimetype"
+msgstr "Mimetype of uploaded file not matches"
 
 #. Default: No file
-#: src/yafowil/common.py:1557
+#: src/yafowil/common.py:1537
 msgid "no_file"
-msgstr "Keine Datei"
+msgstr "No file"
 
 #. Default: Unknown
-#: src/yafowil/common.py:1562
+#: src/yafowil/common.py:1542
 msgid "unknown"
-msgstr "Unbekannt"
+msgstr "Unknown"
 
 #. Default: Filename: 
-#: src/yafowil/common.py:1563
+#: src/yafowil/common.py:1543
 msgid "filename"
-msgstr "Dateiname:"
+msgstr "Filename:"
 
 #. Default: Mimetype: 
-#: src/yafowil/common.py:1564
+#: src/yafowil/common.py:1544
 msgid "mimetype"
-msgstr "Dateityp:"
+msgstr "Mimetype:"
 
 #. Default: Size: 
-#: src/yafowil/common.py:1565
+#: src/yafowil/common.py:1545
 msgid "size"
-msgstr "Größe:"
+msgstr "Size:"
 
 #. Default: Keep Existing file
-#: src/yafowil/common.py:1627
+#: src/yafowil/common.py:1620
 msgid "file_keep"
-msgstr "Behalte bestehende Datei"
+msgstr "Keep Existing file"
 
 #. Default: Replace existing file
-#: src/yafowil/common.py:1628
+#: src/yafowil/common.py:1621
 msgid "file_replace"
-msgstr "Ersetze bestehende Datei"
+msgstr "Replace existing file"
 
 #. Default: Delete existing file
-#: src/yafowil/common.py:1629
+#: src/yafowil/common.py:1622
 msgid "file_delete"
-msgstr "Lösche bestehende Datei"
+msgstr "Delete existing file"
 
 #. Default: Input not a valid email address.
-#: src/yafowil/common.py:1882
+#: src/yafowil/common.py:1901
 msgid "email_address_not_valid"
-msgstr "Eingabe ist keine gültige E-Mail Adresse."
+msgstr "Input not a valid email address."
 
 #. Default: Input not a valid web address.
-#: src/yafowil/common.py:1934
+#: src/yafowil/common.py:1954
 msgid "web_address_not_valid"
-msgstr "Eingabe ist keine gültige Webadresse."
+msgstr "Input not a valid web address."
 
 #. Default: Value has to be at minimum ${min}.
-#: src/yafowil/common.py:2010
+#: src/yafowil/common.py:2032
 msgid "input_number_minimum_value"
-msgstr "Wert muss mindestens ${min} betragen."
+msgstr "Value has to be at minimum ${min}."
 
 #. Default: Value has to be at maximum ${max}.
-#: src/yafowil/common.py:2016
+#: src/yafowil/common.py:2038
 msgid "input_number_maximum_value"
-msgstr "Wert darf maximal ${max} betragen."
+msgstr "Value has to be at maximum ${max}."
 
 #. Default: Value ${val} has to be in stepping of ${step} based on a floor
 #. value of ${minimum}
-#: src/yafowil/common.py:2025
+#: src/yafowil/common.py:2047
 msgid "input_number_step_and_minimum_value"
 msgstr ""
-"Wert ${val} muss mindestens ${minimum} betragen und durch ${step} teilbar "
-"sein."
+"Value ${val} has to be in stepping of ${step} based on a floor value of "
+"${minimum}"
 
 #. Default: Value ${val} has to be in stepping of ${step}
-#: src/yafowil/common.py:2035
+#: src/yafowil/common.py:2057
 msgid "input_number_step_value"
-msgstr "Wert ${val} muss durch ${step} teilbar sein."
-
-#: src/yafowil/tests/test_tsf.py:11
-msgid "foo"
-msgstr ""
-
-#. Default: Bar
-#: src/yafowil/tests/test_tsf.py:12
-msgid "bar"
-msgstr ""
-
-#. Default: Baz ${bam}
-#: src/yafowil/tests/test_tsf.py:14
-msgid "baz"
-msgstr ""
+msgstr "Value ${val} has to be in stepping of ${step}"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yafowil-3.0.1/src/yafowil/i18n/locales/en/LC_MESSAGES/yafowil.mo` & `yafowil-3.1.0/src/yafowil/i18n/locales/en/LC_MESSAGES/yafowil.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -35,20 +35,26 @@
 
 msgid "email_address_not_valid"
 msgstr "Input not a valid email address."
 
 msgid "file_delete"
 msgstr "Delete existing file"
 
+msgid "file_invalid_mimetype"
+msgstr "Mimetype of uploaded file not matches"
+
 msgid "file_keep"
 msgstr "Keep Existing file"
 
 msgid "file_replace"
 msgstr "Replace existing file"
 
+msgid "file_replace_no_upload"
+msgstr "Cannot replace file. No file uploaded."
+
 msgid "filename"
 msgstr "Filename:"
 
 msgid "generic_datatype_message"
 msgstr "Input conversion failed."
 
 msgid "input_number_maximum_value"
```

### Comparing `yafowil-3.0.1/src/yafowil/i18n/locales/yafowil.pot` & `yafowil-3.1.0/src/yafowil/i18n/locales/yafowil.pot`

 * *Files 12% similar despite different names*

```diff
@@ -1,179 +1,175 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2022-03-21 16:26+0100\n"
+"POT-Creation-Date: 2023-03-18 10:23+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Lingua 4.14\n"
-
-#. Default: Mandatory field was empty
-#: ./src/yafowil/common.py:126
-msgid "required_message"
-msgstr ""
+"Generated-By: Lingua 4.15.0\n"
 
 #. Default: string
-#: ./src/yafowil/common.py:232
+#: ./src/yafowil/datatypes.py:194
 msgid "datatype_str"
 msgstr ""
 
 #. Default: unicode
-#: ./src/yafowil/common.py:233
+#: ./src/yafowil/datatypes.py:195
 msgid "datatype_unicode"
 msgstr ""
 
 #. Default: integer
-#: ./src/yafowil/common.py:234
+#: ./src/yafowil/datatypes.py:196
 msgid "datatype_integer"
 msgstr ""
 
 #. Default: floating point number
-#: ./src/yafowil/common.py:235
+#: ./src/yafowil/datatypes.py:197
 msgid "datatype_float"
 msgstr ""
 
 #. Default: UUID
-#: ./src/yafowil/common.py:236
+#: ./src/yafowil/datatypes.py:198
 msgid "datatype_uuid"
 msgstr ""
 
 #. Default: long integer
 #. pragma: no cover
-#: ./src/yafowil/common.py:239
+#: ./src/yafowil/datatypes.py:201
 msgid "datatype_long"
 msgstr ""
 
 #. Default: Input conversion failed.
-#: ./src/yafowil/common.py:291
+#: ./src/yafowil/datatypes.py:259
 msgid "generic_datatype_message"
 msgstr ""
 
 #. Default: Input is not a valid ${datatype}.
-#: ./src/yafowil/common.py:298
+#: ./src/yafowil/datatypes.py:266
 msgid "standard_datatype_message"
 msgstr ""
 
+#. Default: Mandatory field was empty
+#: ./src/yafowil/common.py:90
+msgid "required_message"
+msgstr ""
+
 #. Default: Input must have at least ${len} characters.
-#: ./src/yafowil/common.py:801
+#: ./src/yafowil/common.py:707
 msgid "minlength_extraction_error"
 msgstr ""
 
 #. Default: Input contains illegal characters.
-#: ./src/yafowil/common.py:827
+#: ./src/yafowil/common.py:733
 msgid "ascii_extractor_error"
 msgstr ""
 
 #. Default: Password too weak
-#: ./src/yafowil/common.py:962
+#: ./src/yafowil/common.py:876
 msgid "weak_password_message"
 msgstr ""
 
 #. Default: Yes
-#: ./src/yafowil/common.py:1098
+#: ./src/yafowil/common.py:1022
 msgid "yes"
 msgstr ""
 
 #. Default: No
-#: ./src/yafowil/common.py:1099
+#: ./src/yafowil/common.py:1023
 msgid "no"
 msgstr ""
 
 #. Default: Unset
 #. XXX: never used right now?
-#: ./src/yafowil/common.py:1100
+#: ./src/yafowil/common.py:1024
 msgid "unset"
 msgstr ""
 
+#. Default: Cannot replace file. No file uploaded.
+#: ./src/yafowil/common.py:1453
+msgid "file_replace_no_upload"
+msgstr ""
+
+#. Default: Mimetype of uploaded file not matches
+#: ./src/yafowil/common.py:1487
+msgid "file_invalid_mimetype"
+msgstr ""
+
 #. Default: No file
-#: ./src/yafowil/common.py:1557
+#: ./src/yafowil/common.py:1537
 msgid "no_file"
 msgstr ""
 
 #. Default: Unknown
-#: ./src/yafowil/common.py:1562
+#: ./src/yafowil/common.py:1542
 msgid "unknown"
 msgstr ""
 
 #. Default: Filename: 
-#: ./src/yafowil/common.py:1563
+#: ./src/yafowil/common.py:1543
 msgid "filename"
 msgstr ""
 
 #. Default: Mimetype: 
-#: ./src/yafowil/common.py:1564
+#: ./src/yafowil/common.py:1544
 msgid "mimetype"
 msgstr ""
 
 #. Default: Size: 
-#: ./src/yafowil/common.py:1565
+#: ./src/yafowil/common.py:1545
 msgid "size"
 msgstr ""
 
 #. Default: Keep Existing file
-#: ./src/yafowil/common.py:1627
+#: ./src/yafowil/common.py:1620
 msgid "file_keep"
 msgstr ""
 
 #. Default: Replace existing file
-#: ./src/yafowil/common.py:1628
+#: ./src/yafowil/common.py:1621
 msgid "file_replace"
 msgstr ""
 
 #. Default: Delete existing file
-#: ./src/yafowil/common.py:1629
+#: ./src/yafowil/common.py:1622
 msgid "file_delete"
 msgstr ""
 
 #. Default: Input not a valid email address.
-#: ./src/yafowil/common.py:1882
+#: ./src/yafowil/common.py:1901
 msgid "email_address_not_valid"
 msgstr ""
 
 #. Default: Input not a valid web address.
-#: ./src/yafowil/common.py:1934
+#: ./src/yafowil/common.py:1954
 msgid "web_address_not_valid"
 msgstr ""
 
 #. Default: Value has to be at minimum ${min}.
-#: ./src/yafowil/common.py:2010
+#: ./src/yafowil/common.py:2032
 msgid "input_number_minimum_value"
 msgstr ""
 
 #. Default: Value has to be at maximum ${max}.
-#: ./src/yafowil/common.py:2016
+#: ./src/yafowil/common.py:2038
 msgid "input_number_maximum_value"
 msgstr ""
 
 #. Default: Value ${val} has to be in stepping of ${step} based on a floor
 #. value of ${minimum}
-#: ./src/yafowil/common.py:2025
+#: ./src/yafowil/common.py:2047
 msgid "input_number_step_and_minimum_value"
 msgstr ""
 
 #. Default: Value ${val} has to be in stepping of ${step}
-#: ./src/yafowil/common.py:2035
+#: ./src/yafowil/common.py:2057
 msgid "input_number_step_value"
 msgstr ""
-
-#: ./src/yafowil/tests/test_tsf.py:11
-msgid "foo"
-msgstr ""
-
-#. Default: Bar
-#: ./src/yafowil/tests/test_tsf.py:12
-msgid "bar"
-msgstr ""
-
-#. Default: Baz ${bam}
-#: ./src/yafowil/tests/test_tsf.py:14
-msgid "baz"
-msgstr ""
```

### Comparing `yafowil-3.0.1/src/yafowil/persistence.py` & `yafowil-3.1.0/src/yafowil/persistence.py`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/src/yafowil/resources.py` & `yafowil-3.1.0/src/yafowil/resources.py`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/src/yafowil/table.py` & `yafowil-3.1.0/src/yafowil/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 from yafowil.base import factory
 from yafowil.compound import compound_extractor
 from yafowil.compound import compound_renderer
 from yafowil.compound import hybrid_extractor
 from yafowil.utils import attr_value
 from yafowil.utils import css_managed_props
 from yafowil.utils import cssclasses
```

### Comparing `yafowil-3.0.1/src/yafowil/tests/test_base.py` & `yafowil-3.1.0/src/yafowil/tests/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 import webresource as wr
 
 
 ###############################################################################
 # Helpers
 ###############################################################################
 
-def test_extractor(widget, data):
+def _test_extractor(widget, data):
     return 'e1'
 
 
-def test_edit_renderer(widget, data):
+def _test_edit_renderer(widget, data):
     return 'r1, {}, {}, {}'.format(
         widget.__name__,
         str(data),
         str(widget.attributes)
     )
 
 
-def test_getter(widget, data):
+def _test_getter(widget, data):
     return 'Test Value'
 
 
-def test_preprocessor(widget, data):
-    data.attrs['test_preprocessor'] = 'called'
+def _test_preprocessor(widget, data):
+    data.attrs['_test_preprocessor'] = 'called'
     return data
 
 
 ###############################################################################
 # Tests
 ###############################################################################
 
@@ -91,29 +91,29 @@
         self.assertEqual(str(arc.exception), "'Invalid name of root element'")
 
         # It fails if sub path element is wrong
         with self.assertRaises(KeyError):
             data['fieldset']['age'].fetch('root.unknown')
 
     def test_Widget(self):
-        def test_extractor2(widget, data):
+        def _test_extractor2(widget, data):
             return 'e2'
 
-        def test_extractor3(widget, data):
+        def _test_extractor3(widget, data):
             number = data.request[widget.__name__]
             try:
                 return int(number)
             except Exception:
                 raise ExtractionError('e3: Integer expected, got %s' % number)
             return number
 
         def fail_extractor(widget, data):
             raise ValueError('extractor has to fail')
 
-        def test_edit_renderer2(widget, data):
+        def _test_edit_renderer2(widget, data):
             return 'r2, {}, {}, {}'.format(
                 widget.__name__,
                 str(data),
                 str(widget.attributes)
             )
 
         def fail_edit_renderer(widget, data):
@@ -125,182 +125,182 @@
                 str(data),
                 str(widget.attributes)
             )
 
         def fail_display_renderer(widget, data):
             raise ValueError('display renderer has to fail')
 
-        def test_getter2(widget, data):
+        def _test_getter2(widget, data):
             return 999
 
         # The widget class
         test_request = {'MYUID': 'New Test Value'}
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor)],
-            [('1', test_edit_renderer)],
+            [('1', _test_extractor)],
+            [('1', _test_edit_renderer)],
             [('1', test_display_renderer)],
-            [('1', test_preprocessor)],
+            [('1', _test_preprocessor)],
             'MYUID',
-            test_getter,
+            _test_getter,
             dict(test1='Test1', test2='Test2'))
 
         self.checkOutput("""
         r1,
         MYUID,
         <RuntimeData MYUID, value='Test Value', extracted=<UNSET>,
-        attrs={'test_preprocessor': 'called'} at ...>,
+        attrs={'_test_preprocessor': 'called'} at ...>,
         {...'test1': 'Test1'...}
         """, testwidget())
 
         # A passed in request does not trigger extraction
         self.checkOutput("""
         r1,
         MYUID,
         <RuntimeData MYUID, value='Test Value', extracted=<UNSET>,
-        attrs={'test_preprocessor': 'called'} at ...>,
+        attrs={'_test_preprocessor': 'called'} at ...>,
         {...'test2': 'Test2'...}
         """, testwidget(request=test_request))
 
         # Extraction is an explicit task
         data = testwidget.extract(test_request)
         self.checkOutput("""
         <RuntimeData MYUID, value='Test Value', extracted='e1',
-        attrs={'test_preprocessor': 'called'} at ...>
+        attrs={'_test_preprocessor': 'called'} at ...>
         """, str(data))
 
-        self.assertEqual(data.attrs['test_preprocessor'], 'called')
+        self.assertEqual(data.attrs['_test_preprocessor'], 'called')
 
         # Preprocessor is only called once!
-        data.attrs['test_preprocessor'] = 'reset'
+        data.attrs['_test_preprocessor'] = 'reset'
         data = testwidget._runpreprocessors(data)
-        self.assertEqual(data.attrs['test_preprocessor'], 'reset')
+        self.assertEqual(data.attrs['_test_preprocessor'], 'reset')
 
         # Different cases
 
         # a.1) defaults: edit
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor)],
-            [('1', test_edit_renderer)],
+            [('1', _test_extractor)],
+            [('1', _test_edit_renderer)],
             [('1', test_display_renderer)],
             [],
             'MYUID',
-            test_getter,
+            _test_getter,
             dict(test1='Test1', test2='Test2'))
         self.checkOutput("""
         r1,
         MYUID,
         <RuntimeData MYUID, value='Test Value', extracted=<UNSET> at ...>,
         {...'test1': 'Test1'...}
         """, testwidget())
 
         # a.2) mode display
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor)],
-            [('1', test_edit_renderer)],
+            [('1', _test_extractor)],
+            [('1', _test_edit_renderer)],
             [('1', test_display_renderer)],
             [],
             'MYUID',
-            test_getter,
+            _test_getter,
             dict(test1='Test1', test2='Test2'),
             mode='display')
         self.checkOutput("""
         disr1,
         MYUID,
         <RuntimeData MYUID, value='Test Value', extracted=<UNSET> at ...>,
         {...'test2': 'Test2'...}
         """, testwidget())
 
         # a.3) mode skip
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor)],
-            [('1', test_edit_renderer)],
+            [('1', _test_extractor)],
+            [('1', _test_edit_renderer)],
             [('1', test_display_renderer)],
             [],
             'MYUID',
-            test_getter,
+            _test_getter,
             dict(test1='Test1', test2='Test2'),
             mode='skip')
         self.assertEqual(testwidget(), u'')
 
         # a.4) mode w/o renderer
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor)],
+            [('1', _test_extractor)],
             [],
             [],
             [],
             'MYUID',
-            test_getter,
+            _test_getter,
             dict(test1='Test1', test2='Test2'),
             mode='display')
         with self.assertRaises(ValueError) as arc:
             testwidget()
         msg = "no renderers given for widget 'MYUID' at mode 'display'"
         self.assertEqual(str(arc.exception), msg)
 
         # b.1) two extractors w/o request
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor), ('2', test_extractor2)],
-            [('1', test_edit_renderer), ('2', test_edit_renderer2)],
+            [('1', _test_extractor), ('2', _test_extractor2)],
+            [('1', _test_edit_renderer), ('2', _test_edit_renderer2)],
             [('1', test_display_renderer)],
             [],
             'MYUID2',
-            test_getter,
+            _test_getter,
             dict(test1='Test1', test2='Test2'))
         self.checkOutput("""
         r2,
         MYUID2,
         <RuntimeData MYUID2, value='Test Value', extracted=<UNSET> at ...>,
         {...'test1': 'Test1'...}
         """, testwidget())
 
         # b.2) extractor with request, non int has to fail
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor3)],
-            [('1', test_edit_renderer)],
+            [('1', _test_extractor3)],
+            [('1', _test_edit_renderer)],
             [('1', test_display_renderer)],
             [],
             'MYUID2',
-            test_getter2,
+            _test_getter2,
             dict(test1='Test1', test2='Test2'))
 
         self.checkOutput("""
         <RuntimeData MYUID2, value=999, extracted=<UNSET>, 1 error(s) at ...>
         """, str(testwidget.extract({'MYUID2': 'ABC'})))
 
         # b.3) extractor with request, but mode display
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor3)],
-            [('1', test_edit_renderer)],
+            [('1', _test_extractor3)],
+            [('1', _test_edit_renderer)],
             [('1', test_display_renderer)],
             [],
             'MYUID2',
-            test_getter2,
+            _test_getter2,
             dict(test1='Test1', test2='Test2'),
             mode='display')
         self.checkOutput("""
         <RuntimeData MYUID2, value=999, extracted=<UNSET> ...>
         """, str(testwidget.extract({'MYUID2': '123'})))
 
         # b.4) two extractors with request
         testwidget = Widget(
             'blueprint_names_goes_here',
-            [('1', test_extractor3)],
-            [('1', test_edit_renderer)],
+            [('1', _test_extractor3)],
+            [('1', _test_edit_renderer)],
             [('1', test_display_renderer)],
             [],
             'MYUID2',
-            test_getter2,
+            _test_getter2,
             dict(test1='Test1', test2='Test2'))
         self.checkOutput("""
         <RuntimeData MYUID2, value=999, extracted=123 at ...>
         """, str(testwidget.extract({'MYUID2': '123'})))
 
         # A failing widget
         testwidget = Widget(
@@ -459,59 +459,59 @@
         self.assertTrue(data.has_errors, True)
         self.assertFalse(data['child_0'].has_errors, False)
         self.assertTrue(data['child_1'].has_errors, True)
 
     def test_factory(self):
         # Fill factory with test blueprints
         factory = Factory()
-        factory.register('widget_test', [test_extractor], [test_edit_renderer])
+        factory.register('widget_test', [_test_extractor], [_test_edit_renderer])
         self.assertEqual(
             factory.extractors('widget_test'),
-            [test_extractor]
+            [_test_extractor]
         )
         self.assertEqual(
             factory.edit_renderers('widget_test'),
-            [test_edit_renderer]
+            [_test_edit_renderer]
         )
 
         testwidget = factory(
             'widget_test',
             name='MYFAC',
-            value=test_getter,
+            value=_test_getter,
             props=dict(foo='bar'))
         self.checkOutput("""
         r1,
         MYFAC,
         <RuntimeData MYFAC, value='Test Value', extracted=<UNSET> at ...>,
         {'foo': 'bar'}
         """, testwidget())
 
         factory.register(
             'widget_test',
-            [test_extractor],
-            [test_edit_renderer],
-            preprocessors=[test_preprocessor])
+            [_test_extractor],
+            [_test_edit_renderer],
+            preprocessors=[_test_preprocessor])
         self.assertEqual(
             factory.preprocessors('widget_test'),
-            [test_preprocessor]
+            [_test_preprocessor]
         )
 
-        def test_global_preprocessor(widget, data):
+        def _test_global_preprocessor(widget, data):
             return data
 
-        factory.register_global_preprocessors([test_global_preprocessor])
+        factory.register_global_preprocessors([_test_global_preprocessor])
         self.assertEqual(
             factory.preprocessors('widget_test'),
-            [test_global_preprocessor, test_preprocessor]
+            [_test_global_preprocessor, _test_preprocessor]
         )
 
         testwidget = factory(
             'widget_test',
             name='MYFAC',
-            value=test_getter,
+            value=_test_getter,
             props=dict(foo='bar'), mode='display')
         data = testwidget.extract({})
         self.assertEqual(data.mode, 'display')
 
         # We can create sets of static builders, i.e. to have a validating
         # password field with two input fields in. Here a simpler example
         def create_static_compound(widget, factory):
@@ -810,15 +810,15 @@
 
     def test_widget_tree_manipulation(self):
         # Widget trees provide functionality described in
         # ``node.interfaces.IOrder``, which makes it possible to insert widgets
         # at a specific place in an existing widget tree
 
         factory = Factory()
-        factory.register('widget_test', [test_extractor], [test_edit_renderer])
+        factory.register('widget_test', [_test_extractor], [_test_edit_renderer])
 
         widget = factory('widget_test', name='root')
         widget['1'] = factory('widget_test')
         widget['2'] = factory('widget_test')
         self.checkOutput("""
         <class 'yafowil.base.Widget'>: root
         <class 'yafowil.base.Widget'>: 1
```

### Comparing `yafowil-3.0.1/src/yafowil/tests/test_compound.py` & `yafowil-3.1.0/src/yafowil/tests/test_compound.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from node.utils import UNSET
 from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.controller import Controller
 from yafowil.tests import YafowilTestCase
 from yafowil.tests import fxml
 from yafowil.utils import Tag
-import yafowil.common
-import yafowil.compound  # noqa
 
 
 ###############################################################################
 # Helpers
 ###############################################################################
 
 tag = Tag(lambda msg: msg)
```

### Comparing `yafowil-3.0.1/src/yafowil/tests/test_controller.py` & `yafowil-3.1.0/src/yafowil/tests/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from yafowil.base import factory
 from yafowil.controller import Controller
 from yafowil.tests import fxml
 from yafowil.tests import YafowilTestCase
-import yafowil.common
-import yafowil.compound  # noqa
 
 
 class TestController(YafowilTestCase):
 
     def test_controller(self):
         # Dummy context
         class Context(object):
```

### Comparing `yafowil-3.0.1/src/yafowil/tests/test_persistence.py` & `yafowil-3.1.0/src/yafowil/tests/test_persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from odict import odict
 from yafowil.base import factory
 from yafowil.persistence import attribute_writer
 from yafowil.persistence import node_attribute_writer
 from yafowil.persistence import write_mapping_writer
 from yafowil.tests import YafowilTestCase
 import uuid
-import yafowil.loader  # noqa
 
 
 class TestPersistence(YafowilTestCase):
 
     def test_persistence(self):
         # Test ``attribute_writer``
         form = factory(
```

### Comparing `yafowil-3.0.1/src/yafowil/tests/test_resources.py` & `yafowil-3.1.0/src/yafowil/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/src/yafowil/tests/test_table.py` & `yafowil-3.1.0/src/yafowil/tests/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from node.utils import UNSET
 from odict import odict
 from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.tests import YafowilTestCase
 from yafowil.tests import fxml
-import yafowil.common
-import yafowil.compound
-import yafowil.table  # noqa
 
 
 class TestTable(YafowilTestCase):
     # Table elements are available as blueprints, often one wanta to
     # organize form elements inside a table, providing pretty looking forms
 
     def test_table_blueprint(self):
```

### Comparing `yafowil-3.0.1/src/yafowil/tsf.py` & `yafowil-3.1.0/src/yafowil/tsf.py`

 * *Files identical despite different names*

### Comparing `yafowil-3.0.1/src/yafowil/utils.py` & `yafowil-3.1.0/src/yafowil/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,57 @@
 # -*- coding: utf-8 -*-
 from node.utils import UNSET
 from pkg_resources import iter_entry_points
-from yafowil.compat import BYTES_TYPE
-from yafowil.compat import IS_PY2
-from yafowil.compat import LONG_TYPE
 from yafowil.compat import STR_TYPE
 from yafowil.compat import UNICODE_TYPE
+from zope.deferredimport import deprecated
 import json
 import logging
 import re
 import unicodedata
-import uuid
+
+
+class EmptyValue(object):
+    """Used to identify empty values in conjunction with data type conversion.
+    """
+
+    def __nonzero__(self):
+        return False
+
+    __bool__ = __nonzero__
+
+    def __str__(self):
+        return ''
+
+    def __len__(self):
+        return 0
+
+    def __repr__(self):
+        return '<EMPTY_VALUE>'
+
+    def __copy__(self):
+        return self
+
+    def __deepcopy__(self, memo):
+        return self
+
+    def __lt__(self, other):
+        return False
+
+    def __le__(self, other):
+        return False
+
+    def __gt__(self, other):
+        return False
+
+    def __ge__(self, other):
+        return False
+
+
+EMPTY_VALUE = EmptyValue()
 
 
 class entry_point(object):
     """Decorator for yafowil entry points.
     """
 
     def __init__(self, order=0):
@@ -336,105 +373,19 @@
     if attrs['class_add']:
         _classes += attr_value('class_add', widget, data).split()
     additional = [add for add in additional if add]
     _classes += additional
     return _classes and ' '.join(sorted(_classes)) or None
 
 
-class EmptyValue(object):
-    """Used to identify empty values in conjunction with data type conversion.
-    """
-
-    def __nonzero__(self):
-        return False
-
-    __bool__ = __nonzero__
-
-    def __str__(self):
-        return ''
-
-    def __len__(self):
-        return 0
-
-    def __repr__(self):
-        return '<EMPTY_VALUE>'
-
-
-EMPTY_VALUE = EmptyValue()
-
-
-DATATYPE_PRECONVERTERS = {
-    float: lambda x: isinstance(x, STR_TYPE) and x.replace(',', '.') or x
-}
-# B/C
-DATATYPE_PRECONVERTERS['float'] = DATATYPE_PRECONVERTERS[float]
-DATATYPE_CONVERTERS = {
-    'str': BYTES_TYPE,
-    'unicode': UNICODE_TYPE,
-    'int': int,
-    'integer': int,
-    'long': LONG_TYPE,
-    'float': float,
-    'uuid': uuid.UUID
-}
-
-
-def convert_value_to_datatype(value, datatype, empty_value=EMPTY_VALUE):
-    """Convert given value to datatype.
-
-    Datatype is either a callable or a string out of ``'str'``, ``'unicode'``,
-    ``'int'``, ``'integer'``, ``'long'``, ``'float'`` or ``'uuid'``
-
-    If value is ``UNSET``, return ``UNSET``, regardless of given datatype.
-
-    If value is ``EMPTY_VALUE``, return ``empty_value``, which defaults to
-    ``EMPTY_VALUE`` marker.
-
-    If value is ``None`` or ``''``, return ``empty_value``, which defaults to
-    ``EMPTY_VALUE`` marker. Be aware that empty value marker is even returned
-    if ``str`` datatype, to provide a consistent behavior.
-
-    Converter callables must raise one out of the following exceptions if
-    conversion fails:
-
-        * ``ValueError``
-        * ``UnicodeDecodeError``
-        * ``UnicodeEncodeError``
-    """
-    if value is UNSET:
-        return UNSET
-    if value is EMPTY_VALUE:
-        return empty_value
-    if value in [None, '']:
-        return empty_value
-    if isinstance(datatype, STR_TYPE):
-        converter = DATATYPE_CONVERTERS[datatype]
-    else:
-        converter = datatype
-    try:
-        if isinstance(value, converter):
-            return value
-    except TypeError:
-        # converter is instance of class or function
-        pass
-    preconverter = DATATYPE_PRECONVERTERS.get(datatype)
-    if preconverter:
-        value = preconverter(value)
-    # special case bytes or str buildin type in python 3
-    # uses ascii codec to emulate same behavior as when converting with python2
-    # this is supposed to change in future
-    if not IS_PY2 and converter in (bytes, str):
-        return converter(value, 'ascii')  # pragma: no cover
-    return converter(value)
-
-
-def convert_values_to_datatype(value, datatype, empty_value=EMPTY_VALUE):
-    if isinstance(value, list):
-        res = list()
-        for item in value:
-            res.append(convert_value_to_datatype(
-                item,
-                datatype,
-                empty_value=empty_value
-            ))
-        return res
-    return convert_value_to_datatype(value, datatype, empty_value=empty_value)
+###############################################################################
+# B/C imports
+###############################################################################
+
+deprecated(
+    '``convert_value_to_datatype`` has been moved to ``yafowil.datatypes``.',
+    convert_value_to_datatype='yafowil.datatypes:convert_value_to_datatype',
+)
+deprecated(
+    '``convert_values_to_datatype`` has been moved to ``yafowil.datatypes``.',
+    convert_values_to_datatype='yafowil.datatypes:convert_values_to_datatype',
+)
```

### Comparing `yafowil-3.0.1/src/yafowil.egg-info/PKG-INFO` & `yafowil-3.1.0/src/yafowil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yafowil
-Version: 3.0.1
+Version: 3.1.0
 Summary: YAFOWIL - declarative, framework independent, flexible HTML forms
 Home-page: http://github.com/conestack/yafowil
 Author: Yafowil Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Description: yafowil
         =======
@@ -69,14 +69,60 @@
         - Christian Scholz aka MrTopf
         
         
         
         History
         =======
         
+        3.1.0 (2023-05-15)
+        ------------------
+        
+        - Refactor datatype conversion. Datatype related extractors and utils are
+          contained in ``yafowil.datatype`` now. Fix datatype conversion for ``bytes``
+          type.
+          [rnix]
+        
+        - Split up ``yafowil.common`` module [rnix]
+        
+          - Move ``button`` and ``submit`` blueprints to ``yafowil.button``.
+        
+          - Move ``checkbox`` blueprint to ``yafowil.checkbox``.
+        
+          - Move ``email`` blueprint to ``yafowil.email``.
+        
+          - Move ``field``, ``label``, ``help`` and ``error`` blueprints to ``yafowil.field``.
+        
+          - Move ``file`` blueprint to ``yafowil.file``.
+        
+          - Move ``hidden`` blueprint to ``yafowil.hidden``.
+        
+          - Move ``lines`` blueprint to ``yafowil.lines``.
+        
+          - Move ``number`` blueprint to ``yafowil.number``.
+        
+          - Move ``password`` blueprint to ``yafowil.password``.
+        
+          - Move ``proxy`` blueprint to ``yafowil.proxy``.
+        
+          - Move ``search`` blueprint to ``yafowil.search``.
+        
+          - Move ``select`` blueprint to ``yafowil.select``.
+        
+          - Move ``tag`` blueprint to ``yafowil.tag``.
+        
+          - Move ``text`` blueprint to ``yafowil.text``.
+        
+          - Move ``textarea`` blueprint to ``yafowil.textarea``.
+        
+          - Move ``url`` blueprint to ``yafowil.url``.
+        
+        - Tests work with pytest.
+          [rnix]
+        
+        
         3.0.1 (2022-12-05)
         ------------------
         
         - File extractor raises an ``ExtractionError`` if file action is ``replace``
           but no file is uploaded instead of silently changing the action to ``keep``.
           [rnix]
```

