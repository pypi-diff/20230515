# Comparing `tmp/yafowil.widget.select2-1.4.tar.gz` & `tmp/yafowil.widget.select2-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yafowil.widget.select2-1.4.tar", last modified: Mon Jul 16 14:16:32 2018, max compression
+gzip compressed data, was "yafowil.widget.select2-2.0a1.tar", last modified: Mon May 15 12:51:11 2023, max compression
```

## Comparing `yafowil.widget.select2-1.4.tar` & `yafowil.widget.select2-2.0a1.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/MANIFEST.in
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4466 2018-07-16 14:16:31.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      130 2018-07-16 14:16:31.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2018-02-02 08:08:27.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2018-07-16 14:16:31.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       48 2018-07-16 14:16:31.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2018-07-16 14:16:31.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4769 2018-07-16 14:16:31.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2018-07-16 14:16:31.000000 yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/top_level.txt
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/src/yafowil/widget/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      790 2018-07-16 12:38:35.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6817 2018-07-16 12:38:35.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8362 2018-07-16 12:38:35.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/example.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    21998 2018-07-16 12:38:35.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/widget.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      378 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/widget.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4365 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/widget.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1030 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.jquery.json
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1858 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_sk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      953 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_de.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      829 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_id.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      940 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_az.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      878 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_fi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      774 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ms.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      809 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ko.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      694 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_zh-CN.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      706 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_zh-TW.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      793 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_is.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      769 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_tr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1732 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/component.json
--rw-r--r--   0 rnix      (1000) rnix      (1000)      750 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ja.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      996 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_rs.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1849 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2-spinner.gif
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1082 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_lt.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      789 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_no.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1019 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_bg.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      897 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_vi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      785 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_sv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1277 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_gl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1145 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_fa.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1318 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ar.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1078 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_pl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      890 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ca.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4174 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/README.md
--rw-r--r--   0 rnix      (1000) rnix      (1000)      791 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_da.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      937 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_lv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3347 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2-bootstrap.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)      940 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_hr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      740 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_hu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_he.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1016 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ka.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1040 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_en.js.template
--rw-r--r--   0 rnix      (1000) rnix      (1000)      789 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_nl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      840 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ro.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      824 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_et.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      804 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_it.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1109 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ru.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)   146080 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1251 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_eu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      613 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      845 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2x2.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)      939 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/LICENSE
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1066 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_el.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1929 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_cs.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1015 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_fr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_pt-PT.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1353 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_uk.js
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1490 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/release.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      807 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_pt-BR.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1001 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_th.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_es.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    19336 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1002 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_mk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    65514 2018-02-02 08:08:24.000000 yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2018-07-16 12:38:35.000000 yafowil.widget.select2-1.4/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1537 2018-07-16 12:38:35.000000 yafowil.widget.select2-1.4/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4769 2018-07-16 14:16:32.000000 yafowil.widget.select2-1.4/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1728 2018-07-16 14:16:04.000000 yafowil.widget.select2-1.4/setup.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      771 2018-07-16 14:15:58.000000 yafowil.widget.select2-1.4/HISTORY.rst
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.554625 yafowil.widget.select2-2.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1028 2023-05-15 12:46:13.000000 yafowil.widget.select2-2.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2022-10-30 11:16:34.000000 yafowil.widget.select2-2.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4858 2023-05-15 12:51:11.554625 yafowil.widget.select2-2.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      708 2023-05-15 12:50:43.000000 yafowil.widget.select2-2.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:51:11.554625 yafowil.widget.select2-2.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1731 2023-05-15 12:46:13.000000 yafowil.widget.select2-2.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2282 2022-10-30 11:16:34.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8299 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.554625 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      939 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/LICENSE
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4174 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/README.md
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1732 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/component.json
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1490 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/release.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3347 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2-bootstrap.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1849 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2-spinner.gif
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    19336 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1030 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.jquery.json
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   146080 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    65514 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      613 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1318 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ar.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      940 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_az.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1019 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_bg.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      890 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1929 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_cs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      791 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_da.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      953 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_de.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1066 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_el.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1040 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_en.js.template
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_es.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      824 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_et.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1251 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_eu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1145 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fa.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      878 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1015 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1277 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_gl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_he.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      940 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_hr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      740 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_hu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      829 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_id.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      793 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_is.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      804 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_it.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      750 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ja.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1016 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ka.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      809 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ko.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1082 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_lt.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      937 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_lv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1002 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_mk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      774 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ms.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      789 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_nl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      789 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_no.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1078 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      807 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pt-BR.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pt-PT.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      840 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ro.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      996 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_rs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1109 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ru.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1858 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_sk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      785 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_sv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1001 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_th.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      769 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_tr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1353 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_uk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      897 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_vi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      694 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_zh-CN.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      706 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_zh-TW.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      845 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2x2.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1771 2022-10-30 11:16:34.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4110 2023-03-13 08:17:16.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1597 2023-03-13 08:17:16.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11732 2022-10-30 11:16:34.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    22033 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4858 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4517 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      130 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-04-02 11:08:00.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/SOURCES.txt` & `yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-HISTORY.rst
+CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.py
 src/yafowil/__init__.py
 src/yafowil.widget.select2.egg-info/PKG-INFO
 src/yafowil.widget.select2.egg-info/SOURCES.txt
@@ -15,14 +15,15 @@
 src/yafowil/widget/__init__.py
 src/yafowil/widget/select2/__init__.py
 src/yafowil/widget/select2/example.py
 src/yafowil/widget/select2/tests.py
 src/yafowil/widget/select2/widget.py
 src/yafowil/widget/select2/resources/widget.css
 src/yafowil/widget/select2/resources/widget.js
+src/yafowil/widget/select2/resources/widget.min.js
 src/yafowil/widget/select2/resources/select2/LICENSE
 src/yafowil/widget/select2/resources/select2/README.md
 src/yafowil/widget/select2/resources/select2/component.json
 src/yafowil/widget/select2/resources/select2/release.sh
 src/yafowil/widget/select2/resources/select2/select2-bootstrap.css
 src/yafowil/widget/select2/resources/select2/select2-spinner.gif
 src/yafowil/widget/select2/resources/select2/select2.css
```

### Comparing `yafowil.widget.select2-1.4/src/yafowil.widget.select2.egg-info/PKG-INFO` & `yafowil.widget.select2-2.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,62 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yafowil.widget.select2
-Version: 1.4
+Version: 2.0a1
 Summary: Select2 widget for YAFOWIL
-Home-page: https://github.com/bluedynamics/yafowil.widget.select2
-Author: BlueDynamics Alliance
-Author-email: dev@bluedynamics.com
+Home-page: http://github.com/conestack/yafowil.widget.select2
+Author: Yafowil Contributors
+Author-email: dev@conestack.org
 License: Simplified BSD
-Description-Content-Type: UNKNOWN
-Description: yafowil.widget.select2
-        ======================
-        
-        This is the Select2 widget for `yafowil <http://pypi.python.org/pypi/yafowil>`_,
-        based on `Select2 http://ivaynberg.github.com/select2/`_
+Description: This is a **selection** widget for
+        `YAFOWIL <http://pypi.python.org/pypi/yafowil>`_,
+        based on `Select2 <http://ivaynberg.github.com/select2/>`_
         
         - `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#select2>`_
-        
         - `DEMO - see it Live <http://demo.yafowil.info/++widget++yafowil.widget.select2/index.html>`_
-        
         - `Select2 <http://ivaynberg.github.com/select2/>`_
         
+        
         Source Code
         ===========
         
         The sources are in a GIT DVCS with its main branches at
-        `github <http://github.com/bluedynamics/yafowil.widget.select2>`_.
+        `github <http://github.com/conestack/yafowil.widget.select2>`_.
         
         We'd be happy to see many forks and pull-requests to make YAFOWIL even better.
         
-        The source code of Select2 can be found on
-        `github https://github.com/ivaynberg/select2`_.
         
         Contributors
         ============
         
         - Johannes Raggam
         
         - Robert Niederreiter
         
         - Georg Bernhard
         
-        History
+        - Lena Daxenbichler
+        
+        
+        Changes
         =======
         
+        2.0a1 (2023-05-15)
+        ------------------
+        
+        - Add ``webresource`` support.
+          [rnix]
+        
+        - Extend JS by ``select2_on_array_add``, ``register_array_subscribers``
+          to enable usage in ``yafowil.widget.array``.
+          [lenadax]
+        
+        - Rewrite JavaScript using ES6.
+          [lenadax]
+        
+        
         1.4 (2018-07-16)
         ----------------
         
         - Python 3 compatibility.
           [rnix]
         
         - Convert doctests to unittests.
@@ -84,37 +95,37 @@
         
         1.0
         ---
         
         - Make it work.
           [thet]
         
+        
         License
         =======
         
-        Copyright (c) 2012-2018, BlueDynamics Alliance, Austria, Germany, Switzerland
+        Copyright (c) 2012-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
+        Copyright (c) 2021-2022, Yafowil Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
-        * Redistributions of source code must retain the above copyright notice, this 
+        * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
-        * Redistributions in binary form must reproduce the above copyright notice, this 
-          list of conditions and the following disclaimer in the documentation and/or 
+        
+        * Redistributions in binary form must reproduce the above copyright notice, this
+          list of conditions and the following disclaimer in the documentation and/or
           other materials provided with the distribution.
-        * Neither the name of the BlueDynamics Alliance nor the names of its 
-          contributors may be used to endorse or promote products derived from this 
-          software without specific prior written permission.
-              
-        THIS SOFTWARE IS PROVIDED BY BlueDynamics Alliance ``AS IS`` AND ANY
-        EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
         WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL BlueDynamics Alliance BE LIABLE FOR ANY
-        DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
         (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
         LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
         ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
         (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Platform: UNKNOWN
@@ -123,7 +134,8 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: test
```

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/tests.py` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 from collections import OrderedDict
 from node.utils import UNSET
 from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.compat import IS_PY2
 from yafowil.tests import YafowilTestCase
-from yafowil.tests import fxml
-import yafowil.loader
+import os
+import unittest
 
 
 if not IS_PY2:
     from importlib import reload
 
 
+def np(path):
+    return path.replace('/', os.path.sep)
+
+
 class TestSelect2Widget(YafowilTestCase):
 
     def setUp(self):
         super(TestSelect2Widget, self).setUp()
+        from yafowil.widget import select2
         from yafowil.widget.select2 import widget
         reload(widget)
+        select2.register()
 
     def test_render_single(self):
         widget = factory(
             'select2',
             name='single',
             props={
                 'required': True
             })
         self.assertEqual(widget(), (
             '<select class="select2" id="input-single" name="single" '
-            'required="required" />'
+            'required="required"> </select>'
         ))
 
     def test_render_multiple(self):
         widget = factory(
             'select2',
             name='multi',
             props={
                 'required': True,
                 'multiple': True
             })
         self.assertEqual(widget(), (
             '<input id="exists-multi" name="multi-exists" type="hidden" '
             'value="exists" /><select class="select2" id="input-multi" '
-            'multiple="multiple" name="multi" required="required" />'
+            'multiple="multiple" name="multi" required="required"> </select>'
         ))
 
     def test_render_single_tag_mode(self):
         widget = factory(
             'select2',
             name='single',
             props={
@@ -188,28 +194,30 @@
         self.assertEqual(data.extracted, [])
 
     def test_display_renderer_empty(self):
         widget = factory(
             'select2',
             name='empty',
             mode='display')
-        self.assertEqual(widget(),
+        self.assertEqual(
+            widget(),
             '<div class="display-select2" id="display-empty"></div>'
         )
 
     def test_display_renderer_single(self):
         widget = factory(
             'select2',
             name='single',
             value='foo',
             props={
                 'vocabulary': [('foo', 'Foo'), ('bar', 'Bar')]
             },
             mode='display')
-        self.assertEqual(widget(),
+        self.assertEqual(
+            widget(),
             '<div class="display-select2" id="display-single">Foo</div>'
         )
 
     def test_display_renderer_multiple(self):
         widget = factory(
             'select2',
             name='multi',
@@ -220,10 +228,130 @@
             },
             mode='display')
         self.assertEqual(widget(), (
             '<ul class="display-select2" '
             'id="display-multi"><li>Foo</li><li>Bar</li></ul>'
         ))
 
+    # test with display_proxy_renderer
+    def test_extract_with_preset_value_and_display_proxy_renderer(self):
+        widget = factory(
+            'select2',
+            name='multi',
+            value=['1', '2'],
+            mode='display',
+            props={
+                'multiple': True,
+                'inputtag': True,
+                'display_proxy': True
+            })
+        self.assertEqual(widget(), (
+            '<ul class="display-select2" id="display-multi"><li>1</li><li>2</li></ul>'
+            '<input class="select2" id="input-multi" name="multi" type="hidden" value="1" />'
+            '<input class="select2" id="input-multi" name="multi" type="hidden" value="2" />'
+        ))
+
+        request = {'multi': '1,2,3'}
+        data = widget.extract(request)
+        self.assertEqual(widget(data=data), (
+            '<ul class="display-select2" id="display-multi"><li>1</li><li>2</li><li>3</li></ul>'
+            '<input class="select2" id="input-multi" name="multi" type="hidden" value="1" />'
+            '<input class="select2" id="input-multi" name="multi" type="hidden" value="2" />'
+            '<input class="select2" id="input-multi" name="multi" type="hidden" value="3" />'
+        ))
+        self.assertEqual(data.extracted, ['1', '2', '3'])
+
+        request = {'multi': ''}
+        data = widget.extract(request)
+        self.assertEqual(widget(data=data), (
+            '<div class="display-select2" id="display-multi"></div>'
+        ))
+        self.assertEqual(data.extracted, [])
+
+    def test_display_renderer_empty_and_display_proxy_renderer(self):
+        widget = factory(
+            'select2',
+            name='empty',
+            mode='display',
+            props={
+                'display_proxy': True
+            }
+        )
+        self.assertEqual(
+            widget(),
+            '<div class="display-select2" id="display-empty"></div>'
+        )
+
+    def test_display_renderer_single_and_display_proxy_renderer(self):
+        widget = factory(
+            'select2',
+            name='single',
+            value='foo',
+            mode='display',
+            props={
+                'vocabulary': [('foo', 'Foo'), ('bar', 'Bar')],
+                'display_proxy': True
+            },
+        )
+        self.assertEqual(
+            widget(),
+            '<div class="display-select2" id="display-single">Foo</div>'
+            '<input class="select2" id="input-single" name="single" type="hidden" value="foo" />'
+        )
+
+    def test_display_renderer_multiple_and_display_proxy_renderer(self):
+        widget = factory(
+            'select2',
+            name='multi',
+            value=['foo', 'bar'],
+            props={
+                'vocabulary': [('foo', 'Foo'), ('bar', 'Bar')],
+                'multiple': True,
+                'display_proxy': True
+            },
+            mode='display')
+        self.assertEqual(widget(), (
+            '<ul class="display-select2" id="display-multi"><li>Foo</li><li>Bar</li></ul>'
+            '<input class="select2" id="input-multi" name="multi" type="hidden" value="foo" />'
+            '<input class="select2" id="input-multi" name="multi" type="hidden" value="bar" />'
+        ))
+
+    def test_resources(self):
+        factory.theme = 'default'
+        resources = factory.get_resources('yafowil.widget.select2')
+        self.assertTrue(resources.directory.endswith(np('/select2/resources')))
+        self.assertEqual(resources.name, 'yafowil.widget.select2')
+        self.assertEqual(resources.path, 'yafowil-select2')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 2)
+
+        self.assertTrue(
+            scripts[0].directory.endswith(np('/select2/resources/select2'))
+        )
+        self.assertEqual(scripts[0].path, 'yafowil-select2/select2')
+        self.assertEqual(scripts[0].file_name, 'select2.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        self.assertTrue(scripts[1].directory.endswith(np('/select2/resources')))
+        self.assertEqual(scripts[1].path, 'yafowil-select2')
+        self.assertEqual(scripts[1].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[1].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 2)
+
+        self.assertTrue(
+            styles[0].directory.endswith(np('/select2/resources/select2'))
+        )
+        self.assertEqual(styles[0].path, 'yafowil-select2/select2')
+        self.assertEqual(styles[0].file_name, 'select2.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
+
+        self.assertTrue(styles[1].directory.endswith(np('/select2/resources')))
+        self.assertEqual(styles[1].path, 'yafowil-select2')
+        self.assertEqual(styles[1].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[1].file_path))
+
 
 if __name__ == '__main__':
-    unittest.main()                                          # pragma: no cover
+    unittest.main()
```

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/example.py` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,29 +251,35 @@
         'multiple': True,
         'placeholder': 'Select tags',
         'ajaxurl': 'yafowil.widget.select2.json',
         'tags': True,
     })
     select2_6_routes = {'yafowil.widget.select2.json': json_response}
 
-    return [{'widget': select2_1,
-             'doc': DOC_SELECT2_1,
-             'title': TITLE_SELECT2_1},
-            {'widget': select2_2,
-             'doc': DOC_SELECT2_2,
-             'title': TITLE_SELECT2_2},
-            {'widget': select2_3,
-             'doc': DOC_SELECT2_3,
-             'title': TITLE_SELECT2_3},
-            {'widget': select2_4,
-             'routes': select2_4_routes,
-             'doc': DOC_SELECT2_4,
-             'title': TITLE_SELECT2_4},
-            {'widget': select2_5,
-             'routes': select2_5_routes,
-             'doc': DOC_SELECT2_5,
-             'title': TITLE_SELECT2_5},
-            {'widget': select2_6,
-             'routes': select2_6_routes,
-             'doc': DOC_SELECT2_6,
-             'title': TITLE_SELECT2_6}
-           ]
+    return [{
+        'widget': select2_1,
+        'doc': DOC_SELECT2_1,
+        'title': TITLE_SELECT2_1
+    }, {
+        'widget': select2_2,
+        'doc': DOC_SELECT2_2,
+        'title': TITLE_SELECT2_2
+    }, {
+        'widget': select2_3,
+        'doc': DOC_SELECT2_3,
+        'title': TITLE_SELECT2_3
+    }, {
+        'widget': select2_4,
+        'routes': select2_4_routes,
+        'doc': DOC_SELECT2_4,
+        'title': TITLE_SELECT2_4
+    }, {
+        'widget': select2_5,
+        'routes': select2_5_routes,
+        'doc': DOC_SELECT2_5,
+        'title': TITLE_SELECT2_5
+    }, {
+        'widget': select2_6,
+        'routes': select2_6_routes,
+        'doc': DOC_SELECT2_6,
+        'title': TITLE_SELECT2_6
+    }]
```

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/widget.py` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from collections import OrderedDict
 from node.utils import UNSET
 from yafowil.base import factory
-from yafowil.base import fetch_value
-from yafowil.common import generic_extractor
+from yafowil.common import generic_extractor, display_proxy_renderer
 from yafowil.common import generic_required_extractor
-from yafowil.common import select_extractor
-from yafowil.common import select_edit_renderer
-from yafowil.common import select_display_renderer
 from yafowil.common import input_generic_renderer
-from yafowil.utils import managedprops
-from yafowil.utils import data_attrs_helper
+from yafowil.common import select_display_renderer
+from yafowil.common import select_edit_renderer
+from yafowil.common import select_extractor
 from yafowil.utils import attr_value
+from yafowil.utils import data_attrs_helper
+from yafowil.utils import managedprops
 from yafowil.utils import vocabulary
 
 
 select2_options = [
     'width',
     'minimumInputLength',
     'maximumInputLength',
@@ -135,125 +134,133 @@
     return select_display_renderer(widget, data)
 
 
 factory.register(
     'select2',
     extractors=[select2_extractor, generic_required_extractor],
     edit_renderers=[select2_edit_renderer],
-    display_renderers=[select2_display_renderer])
-
-factory.doc['blueprint']['select2'] = \
-"""Add-on blueprint `yafowil.widget.select2 <http://github.com/bluedynamics/yafowil.widget.select2/>`_
+    display_renderers=[
+        select2_display_renderer,
+        display_proxy_renderer
+    ])
+
+factory.doc['blueprint']['select2'] = """\
+Add-on blueprint
+`yafowil.widget.select2 <http://github.com/conestack/yafowil.widget.select2/>`_
 
 `Integrates Select2 Widget <http://ivaynberg.github.io/select2/>`_
 
 `Detailed widget documentation <http://ivaynberg.github.io/select2/#documentation>`_
 """
 
 factory.defaults['select2.size'] = None
 factory.defaults['select2.default'] = []
 factory.defaults['select2.format'] = 'block'
 
 factory.defaults['select2.class'] = 'select2'
 
 factory.defaults['select2.inputtag'] = False
-factory.doc['props']['select2.inputtag'] = \
-"""Render widget as input element instead of selection.
+factory.doc['props']['select2.inputtag'] = """\
+Render widget as input element instead of selection.
 """
 
 factory.defaults['select2.ajaxurl'] = None
-factory.doc['props']['select2.ajaxurl'] = \
-"""Ajax URL to JSON view returning an array of objects like::
+factory.doc['props']['select2.ajaxurl'] = """\
+Ajax URL to JSON view returning an array of objects like::
 
     [{id: 'id', text: 'text'}]
 """
 
 factory.defaults['select2.width'] = None
-factory.doc['props']['select2.width'] = \
-"""Controls the width style attribute of the Select2 container div.
+factory.doc['props']['select2.width'] = """\
+Controls the width style attribute of the Select2 container div.
 The following values are supported:
 
 off
     No width attribute will be set. Keep in mind that the container div copies
     classes from the source element so setting the width attribute may not
     always be necessary.
+
 element
     Uses javascript to calculate the width of the source element.
+
 copy
     Copies the value of the width style attribute set on the source element.
+
 resolve
     First attempts to copy than falls back on element.
+
 other values
     if the width attribute contains a function it will be evaluated, otherwise
     the value is used verbatim.
 """
 
 factory.defaults['select2.minimumInputLength'] = None
-factory.doc['props']['select2.minimumInputLength'] = \
-"""Number of characters necessary to start a search.
+factory.doc['props']['select2.minimumInputLength'] = """\
+Number of characters necessary to start a search.
 """
 
 factory.defaults['select2.maximumInputLength'] = None
-factory.doc['props']['select2.maximumInputLength'] = \
-"""Maximum number of characters that can be entered for an input.
+factory.doc['props']['select2.maximumInputLength'] = """\
+Maximum number of characters that can be entered for an input.
 """
 
 factory.defaults['select2.minimumResultsForSearch'] = None
-factory.doc['props']['select2.minimumResultsForSearch'] = \
-"""The minimum number of results that must be initially (after opening the
+factory.doc['props']['select2.minimumResultsForSearch'] = """\
+The minimum number of results that must be initially (after opening the
 dropdown for the first time) populated in order to keep the search field.
 This is useful for cases where local data is used with just a few results,
 in which case the search box is not very useful and wastes screen space.
 
 The option can be set to a negative value to permanently hide the search field.
 
 Only applies to single-value select boxes.
 """
 
 factory.defaults['select2.maximumSelectionSize'] = None
-factory.doc['props']['select2.maximumSelectionSize'] = \
-"""The maximum number of items that can be selected in a multi-select control.
+factory.doc['props']['select2.maximumSelectionSize'] = """\
+The maximum number of items that can be selected in a multi-select control.
 If this number is less than 1 selection is not limited.
 
 Once the number of selected items reaches the maximum specified the contents
 of the dropdown will be populated by the formatSelectionTooBig function.
 """
 
 factory.defaults['select2.placeholder'] = None
-factory.doc['props']['select2.placeholder'] = \
-"""Initial value that is selected if no other selection is made.
+factory.doc['props']['select2.placeholder'] = """\
+Initial value that is selected if no other selection is made.
 
 The placeholder can also be specified as a data-placeholder attribute on the
 select or input element that Select2 is attached to.
 
 Note that because browsers assume the first option element is selected in
 non-multi-value select boxes an empty first option element must be provided
 (<option></option>) for the placeholder to work.
 """
 
 factory.defaults['select2.placeholderOption'] = None
-factory.doc['props']['select2.placeholderOption'] = \
-"""When attached to a select resolves the option that should be used as the
+factory.doc['props']['select2.placeholderOption'] = """\
+When attached to a select resolves the option that should be used as the
 placeholder. Can either be a function which given the select element should
 return the option element or a string first to indicate that the first option
 should be used.
 
 This option is useful when Select2's default of using the first option only if
 it has no value and no text is not suitable.
 """
 
 factory.defaults['select2.separator'] = None
-factory.doc['props']['select2.separator'] = \
-"""Separator character or string used to delimit ids in value attribute of the
+factory.doc['props']['select2.separator'] = """\
+Separator character or string used to delimit ids in value attribute of the
 multi-valued selects. The default delimiter is the , character.
 """
 
-factory.defaults['select2.allowClear'] = None;
-factory.doc['props']['select2.allowClear'] = \
-"""Whether or not a clear button is displayed when the select box has a
+factory.defaults['select2.allowClear'] = None
+factory.doc['props']['select2.allowClear'] = """\
+Whether or not a clear button is displayed when the select box has a
 selection. The button, when clicked, resets the value of the select box back
 to the placeholder, thus this option is only available when the placeholder is
 specified.
 
 This option only works when the placeholder is specified.
 
 When attached to a select an option with an empty value must be provided. This
@@ -262,80 +269,80 @@
 
 Also, note that this option only works with non-multi-value based selects
 because multi-value selects always provide such a button for every selected
 option.
 """
 
 factory.defaults['select2.multiple'] = None
-factory.doc['props']['select2.multiple'] = \
-"""Whether or not Select2 allows selection of multiple values.
+factory.doc['props']['select2.multiple'] = """\
+Whether or not Select2 allows selection of multiple values.
 
 When Select2 is attached to a select element this value will be ignored and
 select's multiple attribute will be used instead.
 """
 
 factory.defaults['select2.closeOnSelect'] = None
-factory.doc['props']['select2.closeOnSelect'] = \
-"""If set to false the dropdown is not closed after a selection is made,
+factory.doc['props']['select2.closeOnSelect'] = """\
+If set to false the dropdown is not closed after a selection is made,
 allowing for rapid selection of multiple items. By default this option is set
 to true.
 
 Only applies when configured in multi-select mode.
 """
 
 factory.defaults['select2.openOnEnter'] = None
-factory.doc['props']['select2.openOnEnter'] = \
-"""If set to true the dropdown is opened when the user presses the enter key
+factory.doc['props']['select2.openOnEnter'] = """\
+If set to true the dropdown is opened when the user presses the enter key
 and Select2 is closed. By default this option is enabled.
 """
 
 factory.defaults['select2.id'] = None
-factory.doc['props']['select2.id'] = \
-"""Function used to get the id from the choice object or a string representing
+factory.doc['props']['select2.id'] = """\
+Function used to get the id from the choice object or a string representing
 the key under which the id is stored::
 
     id(object)
 
 The default implementation expects the object to have a id property that is
 returned.
 """
 
 factory.defaults['select2.matcher'] = None
-factory.doc['props']['select2.matcher'] = \
-"""Used to determine whether or not the search term matches an option when a
+factory.doc['props']['select2.matcher'] = """\
+Used to determine whether or not the search term matches an option when a
 built-in query function is used. The built in query function is used when
 Select2 is attached to a select, or the local or tags helpers are used::
 
     matcher(term, text, option)
 
 The default implementation is case insensitive and matches anywhere in the
 term::
 
     function(term, text) {
         return text.toUpperCase().indexOf(term.toUpperCase()) >= 0;
     }
 """
 
 factory.defaults['select2.sortResults'] = None
-factory.doc['props']['select2.sortResults'] = \
-"""Used to sort the results list for searching right before display.
+factory.doc['props']['select2.sortResults'] = """\
+Used to sort the results list for searching right before display.
 Useful for sorting matches by relevance to the user's search term::
 
     sortResults(results, container, query)
 
 Defaults to no sorting::
 
     function(results, container, query) {
         return results;
     }
 """
 
 factory.defaults['select2.formatSelection'] = None
-factory.doc['props']['select2.formatSelection'] = \
-"""Function used to render the current selection::
+factory.doc['props']['select2.formatSelection'] = """\
+Function used to render the current selection::
 
     formatSelection(object, container)
 
 The default implementation expects the object to have a text property that is
 returned.
 
 The implementation may choose to append elements directly to the provided
@@ -347,16 +354,16 @@
     format(item) {
         var originalOption = item.element;
         return item.text
     }
 """
 
 factory.defaults['select2.formatResult'] = None
-factory.doc['props']['select2.formatResult'] = \
-"""Function used to render a result that the user can select::
+factory.doc['props']['select2.formatResult'] = """\
+Function used to render a result that the user can select::
 
     formatResult(object, container, query)
 
 The default implementation expects the object to have a text property that is
 returned.
 
 The implementation may choose to append elements directly to the provided
@@ -368,75 +375,75 @@
     format(item) {
         var originalOption = item.element;
         return item.text
     }
 """
 
 factory.defaults['select2.formatResultCssClass'] = None
-factory.doc['props']['select2.formatResultCssClass'] = \
-"""Function used to add css classes to result elements::
+factory.doc['props']['select2.formatResultCssClass'] = """\
+Function used to add css classes to result elements::
 
     formatResultCssClass(object)
 
 By default when attached to a select css classes from options will be
 automatically copied.
 """
 
 factory.defaults['select2.formatNoMatches'] = None
-factory.doc['props']['select2.formatNoMatches'] = \
-"""String containing "No matches" message, or
+factory.doc['props']['select2.formatNoMatches'] = """\
+String containing "No matches" message, or
 Function used to render the message::
 
     formatNoMatches(term)
 """
 
 factory.defaults['select2.formatSearching'] = None
-factory.doc['props']['select2.formatSearching'] = \
-"""String containing "Searching..." message, or
+factory.doc['props']['select2.formatSearching'] = """\
+String containing "Searching..." message, or
 Function used to render the message that is displayed while search is in
 progress::
 
     formatSearching()
 """
 
 factory.defaults['select2.formatInputTooShort'] = None
-factory.doc['props']['select2.formatInputTooShort'] = \
-"""String containing "Search input too short" message, or Function used to
+factory.doc['props']['select2.formatInputTooShort'] = """\
+String containing "Search input too short" message, or Function used to
 render the message::
 
     formatInputTooShort(term, minLength)
 """
 
 factory.defaults['select2.formatInputTooLong'] = None
-factory.doc['props']['select2.formatInputTooLong'] = \
-"""String containing "Search input too long" message, or Function used to
+factory.doc['props']['select2.formatInputTooLong'] = """\
+String containing "Search input too long" message, or Function used to
 render the message::
 
     formatInputTooLong(term, maxLength)
 """
 
 factory.defaults['select2.formatSelectionTooBig'] = None
-factory.doc['props']['select2.formatSelectionTooBig'] = \
-"""String containing "You cannot select any more choices" message, or Function
+factory.doc['props']['select2.formatSelectionTooBig'] = """\
+String containing "You cannot select any more choices" message, or Function
 used to render the message::
 
     formatSelectionTooBig(maxSize)
 """
 
 factory.defaults['select2.formatLoadMore'] = None
-factory.doc['props']['select2.formatLoadMore'] = \
-"""String containing "Loading more results" message, or Function used to
+factory.doc['props']['select2.formatLoadMore'] = """\
+String containing "Loading more results" message, or Function used to
 render the message::
 
     formatLoadMore(pageNumber)
 """
 
 factory.defaults['select2.createSearchChoice'] = None
-factory.doc['props']['select2.createSearchChoice'] = \
-"""Creates a new selectable choice from user's search term. Allows creation of
+factory.doc['props']['select2.createSearchChoice'] = """\
+Creates a new selectable choice from user's search term. Allows creation of
 choices not available via the query function. Useful when the user can create
 choices on the fly, eg for the 'tagging' usecase::
 
     createSearchChoice(term)
 
 If the function returns undefined or null no choice will be created. If a new
 choice is created it is displayed first in the selection list so that user
@@ -444,185 +451,187 @@
 
 When used in combination with input[type=hidden] tag care must be taken to
 sanitize the id attribute of the choice object, especially stripping , as it
 is used as a value separator.
 """
 
 factory.defaults['select2.createSearchChoicePosition'] = None
-factory.doc['props']['select2.createSearchChoicePosition'] = \
-"""Define the position where to insert element created by createSearchChoice.
+factory.doc['props']['select2.createSearchChoicePosition'] = """\
+Define the position where to insert element created by createSearchChoice.
 The following values are supported:
 
 top
     Insert in the top of the list
+
 bottom
     Insert at the end of the list
+
 function
     A custom function. For example if you want to insert the new item in the
     second position::
 
         $("#tags").select2({
             ...
             createSearchChoice: function(term) { ... },
             createSearchChoicePosition: function(list, item) {
                 list.splice(1, 0, item);
             }
         });
 """
 
 factory.defaults['select2.initSelection'] = None
-factory.doc['props']['select2.initSelection'] = \
-"""Called when Select2 is created to allow the user to initialize the
+factory.doc['props']['select2.initSelection'] = """\
+Called when Select2 is created to allow the user to initialize the
 selection based on the value of the element select2 is attached to.
 
 Essentially this is an id->object mapping function::
 
     initSelection(element, callback)
 
 This function will only be called when there is initial input to be processed.
 """
 
 factory.defaults['select2.tokenizer'] = None
-factory.doc['props']['select2.tokenizer'] = \
-"""A tokenizer function can process the input typed into the search field after
+factory.doc['props']['select2.tokenizer'] = """\
+A tokenizer function can process the input typed into the search field after
 every keystroke and extract and select choices. This is useful, for example,
 in tagging scenarios where the user can create tags quickly by separating
 them with a comma or a space instead of pressing enter.
 
 Tokenizer only applies to multi-selects::
 
     tokenizer(input, selection, selectCallback, opts)
 """
 
 factory.defaults['select2.tokenSeparators'] = None
-factory.doc['props']['select2.tokenSeparators'] = \
-"""An array of strings that define token separators for the default tokenizer
+factory.doc['props']['select2.tokenSeparators'] = """\
+An array of strings that define token separators for the default tokenizer
 function. By default, this option is set to an empty array which means
 tokenization using the default tokenizer is disabled. Usually it is sensible
 to set this option to a value similar to [',', ' '].
 """
 
 factory.defaults['select2.query'] = None
-factory.doc['props']['select2.query'] = \
-"""Function used to query results for the search term::
+factory.doc['props']['select2.query'] = """\
+Function used to query results for the search term::
 
     query(options)
 
 In order for this function to work Select2 should be attached to a input
 type='hidden' tag instead of a select.
 """
 
 factory.defaults['select2.ajax'] = None
-factory.doc['props']['select2.ajax'] = \
-"""Options for the built in ajax query function. This object acts as a
+factory.doc['props']['select2.ajax'] = """\
+Options for the built in ajax query function. This object acts as a
 shortcut for having to manually write a function that performs ajax requests.
 The built-in function supports more advanced features such as throttling and
 dropping out-of-order responses.
 
 In order for this function to work Select2 should be attached to a input
 type='hidden' tag instead of a select.
 """
 
 factory.defaults['select2.data'] = None
-factory.doc['props']['select2.data'] = \
-"""Options for the built in query function that works with arrays.
+factory.doc['props']['select2.data'] = """\
+Options for the built in query function that works with arrays.
 
 If this element contains an array, each element in the array must contain id
 and text keys.
 
 Alternatively, this element can be specified as an object in which results
 key must contain the data as an array and a text key can either be the name
 of the key in data items that contains text or a function that retrieves
 the text given a data element from the array.
 """
 
 factory.defaults['select2.tags'] = None
-factory.doc['props']['select2.tags'] = \
-"""Puts Select2 into 'tagging' mode where the user can add new choices and
+factory.doc['props']['select2.tags'] = """\
+Puts Select2 into 'tagging' mode where the user can add new choices and
 pre-existing tags are provided via this options attribute which is either an
 array or a function that returns an array of objects or strings. If strings
 are used instead of objects they will be converted into an object that has
 an id and text attribute equal to the value of the string.
 """
 
 factory.defaults['select2.containerCss'] = None
-factory.doc['props']['select2.containerCss'] = \
-"""Inline css that will be added to select2's container. Either an object
+factory.doc['props']['select2.containerCss'] = """\
+Inline css that will be added to select2's container. Either an object
 containing css property/value key pairs or a function that returns such an
 object.
 """
 
 factory.defaults['select2.containerCssClass'] = None
-factory.doc['props']['select2.containerCssClass'] = \
-"""Css class that will be added to select2's container tag.
+factory.doc['props']['select2.containerCssClass'] = """\
+Css class that will be added to select2's container tag.
 """
 
 factory.defaults['select2.dropdownCss'] = None
-factory.doc['props']['select2.dropdownCss'] = \
-"""Inline css that will be added to select2's dropdown container. Either an
+factory.doc['props']['select2.dropdownCss'] = """\
+Inline css that will be added to select2's dropdown container. Either an
 object containing css property/value key pairs or a function that returns such
 an object.
 """
 
 factory.defaults['select2.dropdownCssClass'] = None
-factory.doc['props']['select2.dropdownCssClass'] = \
-"""Css class that will be added to select2's dropdown container.
+factory.doc['props']['select2.dropdownCssClass'] = """\
+Css class that will be added to select2's dropdown container.
 """
 
 factory.defaults['select2.dropdownAutoWidth'] = None
-factory.doc['props']['select2.dropdownAutoWidth'] = \
-"""When set to true attempts to automatically size the width of the dropdown
+factory.doc['props']['select2.dropdownAutoWidth'] = """\
+When set to true attempts to automatically size the width of the dropdown
 based on content inside.
 """
 
 factory.defaults['select2.adaptContainerCssClass'] = None
-factory.doc['props']['select2.adaptContainerCssClass'] = \
-"""Function that filters/renames css classes as they are copied from the
+factory.doc['props']['select2.adaptContainerCssClass'] = """\
+Function that filters/renames css classes as they are copied from the
 source tag to the select2 container tag::
 
     adaptContainerCssClass(clazz)
 
 The default implementation applies all classes without modification.
 """
 
 factory.defaults['select2.adaptDropdownCssClass'] = None
-factory.doc['props']['select2.adaptDropdownCssClass'] = \
-"""Function that filters/renames css classes as they are copied from the
+factory.doc['props']['select2.adaptDropdownCssClass'] = """\
+Function that filters/renames css classes as they are copied from the
 source tag to the select2 dropdown tag::
 
     adaptDropdownCssClass(clazz)
 
 The default implementation always returns null thereby filtering out all
 classes.
 """
 
 factory.defaults['select2.escapeMarkup'] = None
-factory.doc['props']['select2.escapeMarkup'] = \
-"""String escapeMarkup(String markup)
+factory.doc['props']['select2.escapeMarkup'] = """\
+String escapeMarkup(String markup)
 
 Function used to post-process markup returned from formatter functions. By
 default this function escapes html entities to prevent javascript injection.
 """
 
 factory.defaults['select2.selectOnBlur'] = None
-factory.doc['props']['select2.selectOnBlur'] = \
-"""Set to true if you want Select2 to select the currently highlighted option
+factory.doc['props']['select2.selectOnBlur'] = """\
+Set to true if you want Select2 to select the currently highlighted option
 when it is blurred.
 """
 
 factory.defaults['select2.loadMorePadding'] = None
-factory.doc['props']['select2.loadMorePadding'] = \
-"""Defines how many pixels need to be below the fold before the next page is
+factory.doc['props']['select2.loadMorePadding'] = """\
+Defines how many pixels need to be below the fold before the next page is
 loaded. The default value is 0 which means the result list needs to be
 scrolled all the way to the bottom for the next page of results to be loaded.
 This option can be used to trigger the load sooner, possibly resulting in a
 smoother user experience.
 """
 
 factory.defaults['select2.nextSearchTerm'] = None
-factory.doc['props']['select2.nextSearchTerm'] = \
-"""Function used to determine what the next search term should be.
+factory.doc['props']['select2.nextSearchTerm'] = """\
+Function used to determine what the next search term should be.
 
 Function can be used when the dropdown is configured in single and
 multi-select mode. It is triggered after selecting an item. In single mode
 it is also triggered after initSelection (when provided).
 """
```

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/widget.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,127 +1,135 @@
-/*
- * yafowil select2 widget
- *
- * Optional: bdajax
- */
-
-if (typeof(window.yafowil) == "undefined") yafowil = {};
-
-(function($) {
-
-    $(document).ready(function() {
-        // initial binding
-        yafowil.select2.binder();
-
-        // add after ajax binding if bdajax present
-        if (typeof(window.bdajax) != "undefined") {
-            $.extend(bdajax.binders, {
-                select2_binder: yafowil.select2.binder
+var yafowil_select2 = (function(exports, $) {
+    'use strict';
+
+    class Select2Widget {
+        static initialize(context) {
+            $('.select2', context).each(function(event) {
+                let elem = $(this);
+                if (window.yafowil_array !== undefined &&
+                    window.yafowil_array.inside_template(elem)) {
+                    return;
+                }
+                let options = elem.data();
+                new Select2Widget(elem, options);
             });
         }
-    });
-
-    $.extend(yafowil, {
-
-        select2: {
-
-            extract_value: function(value) {
-                if (typeof value == 'string' &&
-                    value.indexOf('javascript:') == 0) {
-                    value = value.substring(11, value.length);
-                    value = value.split('.');
-                    if (!value.length) {
-                        throw "No function defined";
-                    }
-                    var ctx = window;
-                    var name;
-                    for (var idx in value) {
-                        name = value[idx];
-                        if (typeof(ctx[name]) == "undefined") {
-                            throw "'" + name + "' not found";
+        constructor(elem, ops) {
+            this.elem = elem;
+            this.options = this.init_options(ops);
+            try {
+                this.elem.select2(this.options);
+            } catch (error) {
+                throw `Failed to initialize select2: ${error}`;
+            }
+            elem.data('yafowil-select2', this);
+        }
+        init_options(options) {
+            for (let name in options) {
+                options[name] = this.extract_value(options[name]);
+            }
+            if (options.ajaxurl) {
+                options.ajax = {
+                    url: options.ajaxurl,
+                    dataType: 'json',
+                    data: function(term, page) {
+                        return {
+                            q: term
+                        };
+                    },
+                    results: function(data, page, query) {
+                        if (options.tags && !data.length) {
+                            data.push({
+                                id: query.term,
+                                text: query.term
+                            });
                         }
-                        ctx = ctx[name];
+                        return {
+                            results: data
+                        };
                     }
-                    value = ctx;
-                }
-                return value;
-            },
-
-            update_options: function(options) {
-                var name, value;
-                for (var idx in options) {
-                    name = options[idx];
-                    value = yafowil.select2.extract_value(options[name]);
-                    options[name] = value;
-                }
-                return options;
-            },
+                };
+                options.initSelection = function(element, callback) {
+                    let value = element.val();
+                    if (!value) {
+                        return;
+                    }
+                    let vocab = element.data('vocabulary');
 
-            binder: function(context) {
-                $('.select2', context).each(function(event) {
-                    var elem = $(this);
-                    var options = yafowil.select2.update_options(elem.data());
-                    if (options.ajaxurl) {
-                        options.ajax = {
-                            url: options.ajaxurl,
-                            dataType: 'json',
-                            data: function(term, page) {
-                                return {
-                                    q: term, // search term
-                                };
-                            },
-                            results: function(data, page, query) {
-                                if (options.tags && data.length == 0) {
-                                    data.push({
-                                        id: query.term,
-                                        text: query.term
-                                    });
-                                }
-                                return {
-                                    results: data
-                                };
-                            }
-                        };
-                        options.initSelection = function(element, callback) {
-                            var value = element.val();
-                            if (!value) {
-                                return;
-                            }
-                            var vocabulary = element.data('vocabulary');
-                            var label = function(key) {
-                                if (!vocabulary) {
-                                    return key;
-                                }
-                                var term = vocabulary[key];
-                                if (!term) {
-                                    return key;
-                                }
-                                return term
-                            }
-                            if (!options.multiple) {
-                                callback({
-                                    id: value,
-                                    text: label(value)
-                                });
-                                return;
-                            }
-                            var data = [];
-                            $(element.val().split(",")).each(function() {
-                                data.push({
-                                    id: this,
-                                    text: label(this)
-                                });
+                    function label(key) {
+                        return (!vocab || !vocab[key]) ? key : vocab[key];
+                    }
+                    if (options.multiple) {
+                        let data = [];
+                        $(element.val().split(",")).each(function() {
+                            data.push({
+                                id: this,
+                                text: label(this)
                             });
-                            callback(data);
-                        }
+                        });
+                        callback(data);
+                    } else {
+                        callback({
+                            id: value,
+                            text: label(value)
+                        });
                     }
-                    try {
-                        elem.select2(options);
-                    } catch (error) {
-                        console.log('Failed to initialize select2: ' + error);
+                };
+            }
+            return options;
+        }
+        extract_value(value) {
+            if (typeof value === 'string' && !value.indexOf('javascript:')) {
+                value = value.substring(11, value.length).split('.');
+                if (!value[0].length) {
+                    throw "No function defined";
+                }
+                let ctx = window;
+                for (let name of value) {
+                    if (ctx[name] === undefined) {
+                        throw `${name} not found`;
                     }
-                });
+                    ctx = ctx[name];
+                }
+                value = ctx;
             }
+            return value;
+        }
+    }
+
+    function select2_on_array_add(inst, context) {
+        Select2Widget.initialize(context);
+    }
+
+    function register_array_subscribers() {
+        if (window.yafowil_array === undefined) {
+            return;
         }
+        window.yafowil_array.on_array_event('on_add', select2_on_array_add);
+    }
+
+    $(function() {
+        if (window.ts !== undefined) {
+            ts.ajax.register(Select2Widget.initialize, true);
+        } else if (window.bdajax !== undefined) {
+            bdajax.register(Select2Widget.initialize, true);
+        } else {
+            Select2Widget.initialize();
+        }
+        register_array_subscribers();
+    });
+
+    exports.Select2Widget = Select2Widget;
+    exports.register_array_subscribers = register_array_subscribers;
+
+    Object.defineProperty(exports, '__esModule', {
+        value: true
     });
 
-})(jQuery);
+
+    window.yafowil = window.yafowil || {};
+    window.yafowil.select2 = exports;
+
+
+    return exports;
+
+})({}, jQuery);
```

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.jquery.json` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.jquery.json`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_sk.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_sk.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_de.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_de.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_id.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_id.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_az.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_az.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_fi.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fi.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ms.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ms.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ko.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ko.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_zh-CN.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_zh-CN.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_zh-TW.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_zh-TW.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_is.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_is.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_tr.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_tr.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/component.json` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/component.json`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ja.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ja.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_rs.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_rs.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2-spinner.gif` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_lt.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_lt.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_no.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_no.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_bg.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_bg.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_vi.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_vi.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_sv.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_sv.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_gl.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_gl.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_fa.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fa.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ar.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ar.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_pl.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pl.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ca.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ca.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/README.md` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/README.md`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_da.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_da.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_lv.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_lv.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2-bootstrap.css` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2-bootstrap.css`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_hr.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_hr.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_hu.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_hu.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_he.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_he.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ka.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ka.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_en.js.template` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_en.js.template`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_nl.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_nl.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ro.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ro.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_et.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_et.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_it.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_it.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_ru.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ru.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_eu.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_eu.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.png` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2x2.png` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/LICENSE` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/LICENSE`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_el.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_el.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_cs.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_cs.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_fr.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fr.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_pt-PT.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pt-PT.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_uk.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_uk.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/release.sh` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/release.sh`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_pt-BR.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pt-BR.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_th.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_th.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_es.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_es.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.css` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.css`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2_locale_mk.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_mk.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/src/yafowil/widget/select2/resources/select2/select2.min.js` & `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-1.4/PKG-INFO` & `yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,62 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yafowil.widget.select2
-Version: 1.4
+Version: 2.0a1
 Summary: Select2 widget for YAFOWIL
-Home-page: https://github.com/bluedynamics/yafowil.widget.select2
-Author: BlueDynamics Alliance
-Author-email: dev@bluedynamics.com
+Home-page: http://github.com/conestack/yafowil.widget.select2
+Author: Yafowil Contributors
+Author-email: dev@conestack.org
 License: Simplified BSD
-Description-Content-Type: UNKNOWN
-Description: yafowil.widget.select2
-        ======================
-        
-        This is the Select2 widget for `yafowil <http://pypi.python.org/pypi/yafowil>`_,
-        based on `Select2 http://ivaynberg.github.com/select2/`_
+Description: This is a **selection** widget for
+        `YAFOWIL <http://pypi.python.org/pypi/yafowil>`_,
+        based on `Select2 <http://ivaynberg.github.com/select2/>`_
         
         - `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#select2>`_
-        
         - `DEMO - see it Live <http://demo.yafowil.info/++widget++yafowil.widget.select2/index.html>`_
-        
         - `Select2 <http://ivaynberg.github.com/select2/>`_
         
+        
         Source Code
         ===========
         
         The sources are in a GIT DVCS with its main branches at
-        `github <http://github.com/bluedynamics/yafowil.widget.select2>`_.
+        `github <http://github.com/conestack/yafowil.widget.select2>`_.
         
         We'd be happy to see many forks and pull-requests to make YAFOWIL even better.
         
-        The source code of Select2 can be found on
-        `github https://github.com/ivaynberg/select2`_.
         
         Contributors
         ============
         
         - Johannes Raggam
         
         - Robert Niederreiter
         
         - Georg Bernhard
         
-        History
+        - Lena Daxenbichler
+        
+        
+        Changes
         =======
         
+        2.0a1 (2023-05-15)
+        ------------------
+        
+        - Add ``webresource`` support.
+          [rnix]
+        
+        - Extend JS by ``select2_on_array_add``, ``register_array_subscribers``
+          to enable usage in ``yafowil.widget.array``.
+          [lenadax]
+        
+        - Rewrite JavaScript using ES6.
+          [lenadax]
+        
+        
         1.4 (2018-07-16)
         ----------------
         
         - Python 3 compatibility.
           [rnix]
         
         - Convert doctests to unittests.
@@ -84,37 +95,37 @@
         
         1.0
         ---
         
         - Make it work.
           [thet]
         
+        
         License
         =======
         
-        Copyright (c) 2012-2018, BlueDynamics Alliance, Austria, Germany, Switzerland
+        Copyright (c) 2012-2021, BlueDynamics Alliance, Austria, Germany, Switzerland
+        Copyright (c) 2021-2022, Yafowil Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
-        * Redistributions of source code must retain the above copyright notice, this 
+        * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
-        * Redistributions in binary form must reproduce the above copyright notice, this 
-          list of conditions and the following disclaimer in the documentation and/or 
+        
+        * Redistributions in binary form must reproduce the above copyright notice, this
+          list of conditions and the following disclaimer in the documentation and/or
           other materials provided with the distribution.
-        * Neither the name of the BlueDynamics Alliance nor the names of its 
-          contributors may be used to endorse or promote products derived from this 
-          software without specific prior written permission.
-              
-        THIS SOFTWARE IS PROVIDED BY BlueDynamics Alliance ``AS IS`` AND ANY
-        EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
         WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL BlueDynamics Alliance BE LIABLE FOR ANY
-        DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
         (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
         LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
         ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
         (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Platform: UNKNOWN
@@ -123,7 +134,8 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: test
```

### Comparing `yafowil.widget.select2-1.4/setup.py` & `yafowil.widget.select2-2.0a1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from setuptools import find_packages
 from setuptools import setup
 import os
 
 
-version = '1.4'
+def read_file(name):
+    with open(os.path.join(os.path.dirname(__file__), name)) as f:
+        return f.read()
+
+
+version = '2.0a1'
 shortdesc = 'Select2 widget for YAFOWIL'
-longdesc = open(os.path.join(os.path.dirname(__file__), 'README.rst')).read()
-longdesc += open(os.path.join(os.path.dirname(__file__), 'HISTORY.rst')).read()
-longdesc += open(os.path.join(os.path.dirname(__file__), 'LICENSE.rst')).read()
-tests_require = ['yafowil[test]']
+longdesc = '\n\n'.join([read_file(name) for name in [
+    'README.rst',
+    'CHANGES.rst',
+    'LICENSE.rst'
+]])
 
 
 setup(
     name='yafowil.widget.select2',
     version=version,
     description=shortdesc,
     long_description=longdesc,
@@ -24,30 +30,35 @@
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     keywords='',
-    author='BlueDynamics Alliance',
-    author_email='dev@bluedynamics.com',
-    url=u'https://github.com/bluedynamics/yafowil.widget.select2',
+    author='Yafowil Contributors',
+    author_email='dev@conestack.org',
+    url=u'http://github.com/conestack/yafowil.widget.select2',
     license='Simplified BSD',
     packages=find_packages('src'),
-    package_dir = {'': 'src'},
+    package_dir={'': 'src'},
     namespace_packages=['yafowil', 'yafowil.widget'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
         'yafowil>2.1.99',
     ],
-    tests_require=tests_require,
-    extras_require = dict(
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
     test_suite="yafowil.widget.select2.tests",
     entry_points="""
     [yafowil.plugin]
     register = yafowil.widget.select2:register
     example = yafowil.widget.select2.example:get_example
-    """)
+    """
+)
```

### Comparing `yafowil.widget.select2-1.4/HISTORY.rst` & `yafowil.widget.select2-2.0a1/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,24 @@
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
+- Extend JS by ``select2_on_array_add``, ``register_array_subscribers``
+  to enable usage in ``yafowil.widget.array``.
+  [lenadax]
+
+- Rewrite JavaScript using ES6.
+  [lenadax]
+
+
 1.4 (2018-07-16)
 ----------------
 
 - Python 3 compatibility.
   [rnix]
 
 - Convert doctests to unittests.
```

