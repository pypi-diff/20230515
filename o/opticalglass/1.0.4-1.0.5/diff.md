# Comparing `tmp/opticalglass-1.0.4.tar.gz` & `tmp/opticalglass-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opticalglass-1.0.4.tar", last modified: Wed Oct 12 21:47:45 2022, max compression
+gzip compressed data, was "opticalglass-1.0.5.tar", last modified: Mon May 15 18:06:56 2023, max compression
```

## Comparing `opticalglass-1.0.4.tar` & `opticalglass-1.0.5.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.505496 opticalglass-1.0.4/
--rw-r--r--   0 Mike       (501) staff       (20)      409 2022-10-12 21:26:35.000000 opticalglass-1.0.4/.gitignore
--rw-r--r--   0 Mike       (501) staff       (20)      511 2022-10-12 18:00:24.000000 opticalglass-1.0.4/.readthedocs.yaml
--rw-r--r--   0 Mike       (501) staff       (20)       82 2022-08-22 05:03:42.000000 opticalglass-1.0.4/AUTHORS.rst
--rw-r--r--   0 Mike       (501) staff       (20)     1829 2022-10-12 21:32:26.000000 opticalglass-1.0.4/CHANGELOG.rst
--rw-r--r--   0 Mike       (501) staff       (20)     1530 2022-05-27 23:29:36.000000 opticalglass-1.0.4/LICENSE
--rw-r--r--   0 Mike       (501) staff       (20)     1925 2022-10-12 21:47:45.505828 opticalglass-1.0.4/PKG-INFO
--rw-r--r--   0 Mike       (501) staff       (20)     1195 2022-08-24 19:03:29.000000 opticalglass-1.0.4/README.rst
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.384808 opticalglass-1.0.4/docs/
--rw-r--r--   0 Mike       (501) staff       (20)      580 2022-08-22 05:07:24.000000 opticalglass-1.0.4/docs/Makefile
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.387039 opticalglass-1.0.4/docs/OG_Pandas_intro/
--rw-r--r--   0 Mike       (501) staff       (20)    12795 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Pandas_intro/OG_Pandas_intro.rst
--rw-r--r--   0 Mike       (501) staff       (20)     7299 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Pandas_intro/output_22_1.png
--rw-r--r--   0 Mike       (501) staff       (20)    61882 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Pandas_intro/output_24_1.png
--rw-r--r--   0 Mike       (501) staff       (20)    10963 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Pandas_intro/output_26_1.png
--rw-r--r--   0 Mike       (501) staff       (20)     6723 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Pandas_intro/output_38_1.png
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.389236 opticalglass-1.0.4/docs/OG_Quickstart/
--rw-r--r--   0 Mike       (501) staff       (20)     4552 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Quickstart/OG_Quickstart.rst
--rw-r--r--   0 Mike       (501) staff       (20)     9253 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Quickstart/output_16_1.png
--rw-r--r--   0 Mike       (501) staff       (20)     9253 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Quickstart/output_17_1.png
--rw-r--r--   0 Mike       (501) staff       (20)    42503 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Quickstart/output_19_0.png
--rw-r--r--   0 Mike       (501) staff       (20)     7172 2022-05-27 23:29:36.000000 opticalglass-1.0.4/docs/OG_Quickstart/output_28_1.png
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.401216 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/
--rw-------   0 Mike       (501) staff       (20)     7402 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/OG_RefractiveIndexInfo.rst
--rw-r--r--   0 Mike       (501) staff       (20)   408002 2022-05-28 05:13:35.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/RII_page_copy_data_link.png
--rw-r--r--   0 Mike       (501) staff       (20)   119917 2022-05-28 05:12:53.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/RII_page_data_links.png
--rw-r--r--   0 Mike       (501) staff       (20)   222578 2022-05-28 05:20:25.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/RII_page_rindexdata.png
--rw-r--r--   0 Mike       (501) staff       (20)   130825 2022-05-28 05:20:03.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/RII_page_top.png
--rw-------   0 Mike       (501) staff       (20)    13628 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_19_1.png
--rw-------   0 Mike       (501) staff       (20)    10140 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_21_1.png
--rw-------   0 Mike       (501) staff       (20)    13000 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_23_1.png
--rw-------   0 Mike       (501) staff       (20)    16537 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_26_1.png
--rw-------   0 Mike       (501) staff       (20)    12405 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_29_1.png
--rw-------   0 Mike       (501) staff       (20)    11717 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_33_1.png
--rw-------   0 Mike       (501) staff       (20)    13641 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_36_1.png
--rw-------   0 Mike       (501) staff       (20)    32051 2022-05-29 17:40:46.000000 opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_9_1.png
--rw-r--r--   0 Mike       (501) staff       (20)     3842 2022-08-22 05:07:34.000000 opticalglass-1.0.4/docs/README.rst
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.423571 opticalglass-1.0.4/docs/_images/
--rw-r--r--   0 Mike       (501) staff       (20)   738660 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/BuchdahlCoefficients.png
--rw-r--r--   0 Mike       (501) staff       (20)   726663 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/BuchdahlDispersion.png
--rw-r--r--   0 Mike       (501) staff       (20)   762462 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/CatalogSelection.png
--rw-r--r--   0 Mike       (501) staff       (20)   224020 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/GlassMap.png
--rw-r--r--   0 Mike       (501) staff       (20)    11091 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/IndexVsWvl.png
--rw-r--r--   0 Mike       (501) staff       (20)   765658 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/PartialDispersion.png
--rw-r--r--   0 Mike       (501) staff       (20)   244335 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/PartialMap.png
--rw-r--r--   0 Mike       (501) staff       (20)   840039 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/RefractiveIndex.png
--rw-r--r--   0 Mike       (501) staff       (20)    42333 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/_images/output_11_0.png
--rw-r--r--   0 Mike       (501) staff       (20)       41 2022-08-22 04:12:02.000000 opticalglass-1.0.4/docs/authors.rst
--rw-r--r--   0 Mike       (501) staff       (20)       43 2022-08-22 04:12:02.000000 opticalglass-1.0.4/docs/changelog.rst
--rw-r--r--   0 Mike       (501) staff       (20)     6569 2022-08-24 19:03:29.000000 opticalglass-1.0.4/docs/conf.py
--rw-r--r--   0 Mike       (501) staff       (20)      737 2022-08-22 05:06:20.000000 opticalglass-1.0.4/docs/index.rst
--rw-r--r--   0 Mike       (501) staff       (20)       63 2022-08-22 05:06:31.000000 opticalglass-1.0.4/docs/license.rst
--rw-r--r--   0 Mike       (501) staff       (20)      787 2021-09-21 20:40:59.000000 opticalglass-1.0.4/docs/make.bat
--rw-r--r--   0 Mike       (501) staff       (20)     2362 2022-08-24 19:03:29.000000 opticalglass-1.0.4/docs/opticalglass.rst
--rw-r--r--   0 Mike       (501) staff       (20)      361 2022-08-25 21:42:02.000000 opticalglass-1.0.4/docs/requirements.txt
--rw-r--r--   0 Mike       (501) staff       (20)      346 2022-08-24 19:03:29.000000 opticalglass-1.0.4/pyproject.toml
--rw-r--r--   0 Mike       (501) staff       (20)     1566 2022-10-12 21:47:45.508195 opticalglass-1.0.4/setup.cfg
--rw-r--r--   0 Mike       (501) staff       (20)      724 2022-10-12 17:49:38.000000 opticalglass-1.0.4/setup.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.376452 opticalglass-1.0.4/src/
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.439004 opticalglass-1.0.4/src/opticalglass/
--rw-r--r--   0 Mike       (501) staff       (20)     2228 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/__init__.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     5766 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/buchdahl.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     1851 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/caselessDictionary.py
--rw-r--r--   0 Mike       (501) staff       (20)     2804 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/cdgm.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.499178 opticalglass-1.0.4/src/opticalglass/data/
--rw-r--r--   0 Mike       (501) staff       (20)   674304 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/CDGM.xls
--rw-r--r--   0 Mike       (501) staff       (20)   454924 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/HIKARI.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)   731648 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/HIKARI_prev.xls
--rw-r--r--   0 Mike       (501) staff       (20)  1234441 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/HOYA.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)  1269672 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/HOYA_prev.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)   252743 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/OHARA.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)   265141 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/OHARA_prev.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)   450048 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/SCHOTT.xls
--rw-r--r--   0 Mike       (501) staff       (20)   449024 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/SCHOTT_prev.xls
--rw-r--r--   0 Mike       (501) staff       (20)   160596 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/SUMITA.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)    58113 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/robb1983_data_final.txt
--rw-r--r--   0 Mike       (501) staff       (20)      165 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/data/~$HIKARI.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)    27474 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/glass.py
--rw-r--r--   0 Mike       (501) staff       (20)      834 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/glasserror.py
--rw-r--r--   0 Mike       (501) staff       (20)     4040 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/glassfactory.py
--rwxr-xr-x   0 Mike       (501) staff       (20)    15776 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/glassmap.py
--rw-r--r--   0 Mike       (501) staff       (20)    10922 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/glassmapviewer.py
--rw-r--r--   0 Mike       (501) staff       (20)     2283 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/glasspolygons.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     3525 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/hikari.py
--rw-r--r--   0 Mike       (501) staff       (20)     3021 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/hoya.py
--rw-r--r--   0 Mike       (501) staff       (20)     2211 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/modelglass.py
--rw-r--r--   0 Mike       (501) staff       (20)     2921 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/ohara.py
--rw-r--r--   0 Mike       (501) staff       (20)     2919 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/openpyxl_script.py
--rw-r--r--   0 Mike       (501) staff       (20)     7638 2022-10-12 07:18:56.000000 opticalglass-1.0.4/src/opticalglass/opticalmedium.py
--rw-r--r--   0 Mike       (501) staff       (20)    13538 2022-08-31 22:30:51.000000 opticalglass-1.0.4/src/opticalglass/rindexinfo.py
--rw-r--r--   0 Mike       (501) staff       (20)     3163 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/schott.py
--rw-r--r--   0 Mike       (501) staff       (20)     3783 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/spectral_lines.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     3223 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/sumita.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.504472 opticalglass-1.0.4/src/opticalglass/test/
--rwxr-xr-x   0 Mike       (501) staff       (20)      879 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/cmd_line_example.py
--rw-r--r--   0 Mike       (501) staff       (20)     1969 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/test_cdgm.py
--rw-r--r--   0 Mike       (501) staff       (20)     3050 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/test_glassfactory.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     2200 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/test_hikari.py
--rw-r--r--   0 Mike       (501) staff       (20)     2060 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/test_hoya.py
--rw-r--r--   0 Mike       (501) staff       (20)     2071 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/test_ohara.py
--rw-r--r--   0 Mike       (501) staff       (20)     1814 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/test_schott.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     2452 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/test_sumita.py
--rw-r--r--   0 Mike       (501) staff       (20)     3767 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/test_transmission.py
--rw-r--r--   0 Mike       (501) staff       (20)     1193 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/test/util.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     1941 2022-08-24 19:03:29.000000 opticalglass-1.0.4/src/opticalglass/util.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.445295 opticalglass-1.0.4/src/opticalglass.egg-info/
--rw-r--r--   0 Mike       (501) staff       (20)     1925 2022-10-12 21:47:45.000000 opticalglass-1.0.4/src/opticalglass.egg-info/PKG-INFO
--rw-r--r--   0 Mike       (501) staff       (20)     3280 2022-10-12 21:47:45.000000 opticalglass-1.0.4/src/opticalglass.egg-info/SOURCES.txt
--rw-r--r--   0 Mike       (501) staff       (20)        1 2022-10-12 21:47:45.000000 opticalglass-1.0.4/src/opticalglass.egg-info/dependency_links.txt
--rw-r--r--   0 Mike       (501) staff       (20)       58 2022-10-12 21:47:45.000000 opticalglass-1.0.4/src/opticalglass.egg-info/entry_points.txt
--rw-r--r--   0 Mike       (501) staff       (20)        1 2022-08-23 03:14:07.000000 opticalglass-1.0.4/src/opticalglass.egg-info/not-zip-safe
--rw-r--r--   0 Mike       (501) staff       (20)      167 2022-10-12 21:47:45.000000 opticalglass-1.0.4/src/opticalglass.egg-info/requires.txt
--rw-r--r--   0 Mike       (501) staff       (20)       13 2022-10-12 21:47:45.000000 opticalglass-1.0.4/src/opticalglass.egg-info/top_level.txt
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2022-10-12 21:47:45.505052 opticalglass-1.0.4/update/
--rw-r--r--   0 Mike       (501) staff       (20)     1266 2019-01-17 05:29:49.000000 opticalglass-1.0.4/update/catupdate.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.629862 opticalglass-1.0.5/
+-rw-r--r--   0 Mike       (501) staff       (20)      409 2022-10-12 21:26:35.000000 opticalglass-1.0.5/.gitignore
+-rw-r--r--   0 Mike       (501) staff       (20)      511 2022-10-12 18:00:24.000000 opticalglass-1.0.5/.readthedocs.yaml
+-rw-r--r--   0 Mike       (501) staff       (20)       82 2022-08-22 05:03:42.000000 opticalglass-1.0.5/AUTHORS.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     1937 2023-05-15 17:59:41.000000 opticalglass-1.0.5/CHANGELOG.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     1530 2022-05-27 23:29:36.000000 opticalglass-1.0.5/LICENSE
+-rw-r--r--   0 Mike       (501) staff       (20)     2135 2023-05-15 18:06:56.630163 opticalglass-1.0.5/PKG-INFO
+-rw-r--r--   0 Mike       (501) staff       (20)     1405 2023-05-15 18:04:09.000000 opticalglass-1.0.5/README.rst
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.450422 opticalglass-1.0.5/docs/
+-rw-r--r--   0 Mike       (501) staff       (20)      580 2022-08-22 05:07:24.000000 opticalglass-1.0.5/docs/Makefile
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.456154 opticalglass-1.0.5/docs/OG_Pandas_intro/
+-rw-r--r--   0 Mike       (501) staff       (20)    12795 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/OG_Pandas_intro.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     7299 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/output_22_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)    61882 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/output_24_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)    10963 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/output_26_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)     6723 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/output_38_1.png
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.462107 opticalglass-1.0.5/docs/OG_Quickstart/
+-rw-r--r--   0 Mike       (501) staff       (20)     4552 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/OG_Quickstart.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     9253 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/output_16_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)     9253 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/output_17_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)    42503 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/output_19_0.png
+-rw-r--r--   0 Mike       (501) staff       (20)     7172 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/output_28_1.png
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.488668 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/
+-rw-------   0 Mike       (501) staff       (20)     7402 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/OG_RefractiveIndexInfo.rst
+-rw-r--r--   0 Mike       (501) staff       (20)   408002 2022-05-28 05:13:35.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_copy_data_link.png
+-rw-r--r--   0 Mike       (501) staff       (20)   119917 2022-05-28 05:12:53.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_data_links.png
+-rw-r--r--   0 Mike       (501) staff       (20)   222578 2022-05-28 05:20:25.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_rindexdata.png
+-rw-r--r--   0 Mike       (501) staff       (20)   130825 2022-05-28 05:20:03.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_top.png
+-rw-------   0 Mike       (501) staff       (20)    13628 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_19_1.png
+-rw-------   0 Mike       (501) staff       (20)    10140 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_21_1.png
+-rw-------   0 Mike       (501) staff       (20)    13000 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_23_1.png
+-rw-------   0 Mike       (501) staff       (20)    16537 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_26_1.png
+-rw-------   0 Mike       (501) staff       (20)    12405 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_29_1.png
+-rw-------   0 Mike       (501) staff       (20)    11717 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_33_1.png
+-rw-------   0 Mike       (501) staff       (20)    13641 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_36_1.png
+-rw-------   0 Mike       (501) staff       (20)    32051 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_9_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)     3842 2022-08-22 05:07:34.000000 opticalglass-1.0.5/docs/README.rst
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.529918 opticalglass-1.0.5/docs/_images/
+-rw-r--r--   0 Mike       (501) staff       (20)   738660 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/BuchdahlCoefficients.png
+-rw-r--r--   0 Mike       (501) staff       (20)   726663 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/BuchdahlDispersion.png
+-rw-r--r--   0 Mike       (501) staff       (20)   762462 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/CatalogSelection.png
+-rw-r--r--   0 Mike       (501) staff       (20)   224020 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/GlassMap.png
+-rw-r--r--   0 Mike       (501) staff       (20)    11091 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/IndexVsWvl.png
+-rw-r--r--   0 Mike       (501) staff       (20)   765658 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/PartialDispersion.png
+-rw-r--r--   0 Mike       (501) staff       (20)   244335 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/PartialMap.png
+-rw-r--r--   0 Mike       (501) staff       (20)   840039 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/RefractiveIndex.png
+-rw-r--r--   0 Mike       (501) staff       (20)    42333 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/output_11_0.png
+-rw-r--r--   0 Mike       (501) staff       (20)       41 2022-08-22 04:12:02.000000 opticalglass-1.0.5/docs/authors.rst
+-rw-r--r--   0 Mike       (501) staff       (20)       43 2022-08-22 04:12:02.000000 opticalglass-1.0.5/docs/changelog.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     6569 2023-05-15 17:57:53.000000 opticalglass-1.0.5/docs/conf.py
+-rw-r--r--   0 Mike       (501) staff       (20)      737 2022-08-22 05:06:20.000000 opticalglass-1.0.5/docs/index.rst
+-rw-r--r--   0 Mike       (501) staff       (20)       63 2022-08-22 05:06:31.000000 opticalglass-1.0.5/docs/license.rst
+-rw-r--r--   0 Mike       (501) staff       (20)      787 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/make.bat
+-rw-r--r--   0 Mike       (501) staff       (20)     2362 2022-08-24 19:03:29.000000 opticalglass-1.0.5/docs/opticalglass.rst
+-rw-r--r--   0 Mike       (501) staff       (20)      361 2022-08-25 21:42:02.000000 opticalglass-1.0.5/docs/requirements.txt
+-rw-r--r--   0 Mike       (501) staff       (20)      346 2022-08-24 19:03:29.000000 opticalglass-1.0.5/pyproject.toml
+-rw-r--r--   0 Mike       (501) staff       (20)     1566 2023-05-15 18:06:56.631671 opticalglass-1.0.5/setup.cfg
+-rw-r--r--   0 Mike       (501) staff       (20)      724 2022-10-12 17:49:38.000000 opticalglass-1.0.5/setup.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.431683 opticalglass-1.0.5/src/
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.550873 opticalglass-1.0.5/src/opticalglass/
+-rw-r--r--   0 Mike       (501) staff       (20)     2228 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/__init__.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     5766 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/buchdahl.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     1851 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/caselessDictionary.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2804 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/cdgm.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.614461 opticalglass-1.0.5/src/opticalglass/data/
+-rw-r--r--   0 Mike       (501) staff       (20)   674304 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/CDGM.xls
+-rw-r--r--   0 Mike       (501) staff       (20)   454924 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/HIKARI.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)   731648 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/HIKARI_prev.xls
+-rw-r--r--   0 Mike       (501) staff       (20)  1234441 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/HOYA.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)  1269672 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/HOYA_prev.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)   252743 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/OHARA.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)   265141 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/OHARA_prev.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)   450048 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/SCHOTT.xls
+-rw-r--r--   0 Mike       (501) staff       (20)   449024 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/SCHOTT_prev.xls
+-rw-r--r--   0 Mike       (501) staff       (20)   160596 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/SUMITA.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)    58113 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/robb1983_data_final.txt
+-rw-r--r--   0 Mike       (501) staff       (20)      165 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/~$HIKARI.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)    27474 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glass.py
+-rw-r--r--   0 Mike       (501) staff       (20)      834 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glasserror.py
+-rw-r--r--   0 Mike       (501) staff       (20)     4040 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glassfactory.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)    15776 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glassmap.py
+-rw-r--r--   0 Mike       (501) staff       (20)    10922 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glassmapviewer.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2283 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glasspolygons.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     3525 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/hikari.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3021 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/hoya.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2211 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/modelglass.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2921 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/ohara.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2919 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/openpyxl_script.py
+-rw-r--r--   0 Mike       (501) staff       (20)     7531 2023-01-01 20:40:31.000000 opticalglass-1.0.5/src/opticalglass/optical_glass_agf_class.py
+-rw-r--r--   0 Mike       (501) staff       (20)     7638 2023-05-15 05:55:23.000000 opticalglass-1.0.5/src/opticalglass/opticalmedium.py
+-rw-r--r--   0 Mike       (501) staff       (20)    14320 2023-05-15 06:40:19.000000 opticalglass-1.0.5/src/opticalglass/rindexinfo.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3163 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/schott.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3783 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/spectral_lines.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     3223 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/sumita.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.627024 opticalglass-1.0.5/src/opticalglass/test/
+-rwxr-xr-x   0 Mike       (501) staff       (20)      879 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/cmd_line_example.py
+-rw-r--r--   0 Mike       (501) staff       (20)     1969 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_cdgm.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3050 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_glassfactory.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     2200 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_hikari.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2060 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_hoya.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2071 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_ohara.py
+-rw-r--r--   0 Mike       (501) staff       (20)     1814 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_schott.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     2452 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_sumita.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3767 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_transmission.py
+-rw-r--r--   0 Mike       (501) staff       (20)     1193 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/util.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     1941 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/util.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.554262 opticalglass-1.0.5/src/opticalglass.egg-info/
+-rw-r--r--   0 Mike       (501) staff       (20)     2135 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/PKG-INFO
+-rw-r--r--   0 Mike       (501) staff       (20)     3324 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/SOURCES.txt
+-rw-r--r--   0 Mike       (501) staff       (20)        1 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/dependency_links.txt
+-rw-r--r--   0 Mike       (501) staff       (20)       58 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/entry_points.txt
+-rw-r--r--   0 Mike       (501) staff       (20)        1 2022-08-23 03:14:07.000000 opticalglass-1.0.5/src/opticalglass.egg-info/not-zip-safe
+-rw-r--r--   0 Mike       (501) staff       (20)      167 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/requires.txt
+-rw-r--r--   0 Mike       (501) staff       (20)       13 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/top_level.txt
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.628398 opticalglass-1.0.5/update/
+-rw-r--r--   0 Mike       (501) staff       (20)     1266 2019-01-17 05:29:49.000000 opticalglass-1.0.5/update/catupdate.py
```

### Comparing `opticalglass-1.0.4/CHANGELOG.rst` & `opticalglass-1.0.5/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .. currentmodule:: opticalglass
 
 =========
 Changelog
 =========
 
+Version 1.0.5
+=============
+Enable :class:`~.rindexinfo.RIIMedium` to be saved and restored as JSON files.
+
 Version 1.0.4
 =============
 Allow extrapolation for :class:`~.opticalmedium.InterpolatedMedium` refractive index interpolation function. Cleanup help and other references to transported classes from **ray-optics**. Fix version export in build process.
 
 Version 1.0.3
 =============
 Remove :meth:`~.opticalmedium.OpticalMedium.transmission_data` from the required interfaces for :class:`~.opticalmedium.OpticalMedium`. Add :class:`~.opticalmedium.ConstantIndex` class for minimal material definition support. Add a new module, :mod:`~.modelglass`, with class :class:`~.modelglass.ModelGlass` to handle glasses specified by refractive index and v-number. Redo package layout using pyscaffold and use versioning from importlib.metadata.
```

### Comparing `opticalglass-1.0.4/LICENSE` & `opticalglass-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/PKG-INFO` & `opticalglass-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalglass
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tools for reading optical glass catalogs
 Home-page: https://github.com/mjhoptics/opticalglass
 Author: Michael J Hayford
 Author-email: mjhoptics@gmail.com
 License: BSD-3-Clause
 Keywords: glass, optical glass, refractive index, optics,,glass catalog
 Platform: any
@@ -45,14 +45,19 @@
     * Schott
     * Sumita
 
 .. note::
 
    All rights and ownership of the data is retained by the original owners, i.e the respective manufacturers.
 
+Interface to RefractiveIndex.INFO database
+------------------------------------------
+
+An interface to the RefractiveIndex.INFO database, using both the InterpolatedMedium and RIIMedium classes, is available.
+
 Documentation
 -------------
 
 The documentation for **opticalglass** is hosted at `Read the Docs <https://opticalglass.readthedocs.io>`_
 
 .. _pyscaffold-notes:
```

### Comparing `opticalglass-1.0.4/README.rst` & `opticalglass-1.0.5/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     * Schott
     * Sumita
 
 .. note::
 
    All rights and ownership of the data is retained by the original owners, i.e the respective manufacturers.
 
+Interface to RefractiveIndex.INFO database
+------------------------------------------
+
+An interface to the RefractiveIndex.INFO database, using both the InterpolatedMedium and RIIMedium classes, is available.
+
 Documentation
 -------------
 
 The documentation for **opticalglass** is hosted at `Read the Docs <https://opticalglass.readthedocs.io>`_
 
 .. _pyscaffold-notes:
```

### Comparing `opticalglass-1.0.4/docs/Makefile` & `opticalglass-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Pandas_intro/OG_Pandas_intro.rst` & `opticalglass-1.0.5/docs/OG_Pandas_intro/OG_Pandas_intro.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Pandas_intro/output_22_1.png` & `opticalglass-1.0.5/docs/OG_Pandas_intro/output_22_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Pandas_intro/output_24_1.png` & `opticalglass-1.0.5/docs/OG_Pandas_intro/output_24_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Pandas_intro/output_26_1.png` & `opticalglass-1.0.5/docs/OG_Pandas_intro/output_26_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Pandas_intro/output_38_1.png` & `opticalglass-1.0.5/docs/OG_Pandas_intro/output_38_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Quickstart/OG_Quickstart.rst` & `opticalglass-1.0.5/docs/OG_Quickstart/OG_Quickstart.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Quickstart/output_16_1.png` & `opticalglass-1.0.5/docs/OG_Quickstart/output_16_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Quickstart/output_17_1.png` & `opticalglass-1.0.5/docs/OG_Quickstart/output_17_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Quickstart/output_19_0.png` & `opticalglass-1.0.5/docs/OG_Quickstart/output_19_0.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_Quickstart/output_28_1.png` & `opticalglass-1.0.5/docs/OG_Quickstart/output_28_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/OG_RefractiveIndexInfo.rst` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/OG_RefractiveIndexInfo.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/RII_page_copy_data_link.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_copy_data_link.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/RII_page_data_links.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_data_links.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/RII_page_rindexdata.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_rindexdata.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/RII_page_top.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_top.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_19_1.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_19_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_21_1.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_21_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_23_1.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_23_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_26_1.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_26_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_29_1.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_29_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_33_1.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_33_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_36_1.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_36_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/OG_RefractiveIndexInfo/output_9_1.png` & `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_9_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/README.rst` & `opticalglass-1.0.5/docs/README.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/BuchdahlCoefficients.png` & `opticalglass-1.0.5/docs/_images/BuchdahlCoefficients.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/BuchdahlDispersion.png` & `opticalglass-1.0.5/docs/_images/BuchdahlDispersion.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/CatalogSelection.png` & `opticalglass-1.0.5/docs/_images/CatalogSelection.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/GlassMap.png` & `opticalglass-1.0.5/docs/_images/GlassMap.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/IndexVsWvl.png` & `opticalglass-1.0.5/docs/_images/IndexVsWvl.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/PartialDispersion.png` & `opticalglass-1.0.5/docs/_images/PartialDispersion.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/PartialMap.png` & `opticalglass-1.0.5/docs/_images/PartialMap.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/RefractiveIndex.png` & `opticalglass-1.0.5/docs/_images/RefractiveIndex.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/_images/output_11_0.png` & `opticalglass-1.0.5/docs/_images/output_11_0.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/conf.py` & `opticalglass-1.0.5/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 sys.path.insert(0, os.path.join(__location__, "../src"))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'opticalglass'
-copyright = '2017-2022, Michael J. Hayford'
+copyright = '2017-2023, Michael J. Hayford'
 author = 'Michael J. Hayford'
 
 # version: The short X.Y version.
 # release: The full version, including alpha/beta/rc tags.
 try:
     from opticalglass import __version__ as version
 except ImportError:
```

### Comparing `opticalglass-1.0.4/docs/index.rst` & `opticalglass-1.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/make.bat` & `opticalglass-1.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/docs/opticalglass.rst` & `opticalglass-1.0.5/docs/opticalglass.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/setup.cfg` & `opticalglass-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/setup.py` & `opticalglass-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/__init__.py` & `opticalglass-1.0.5/src/opticalglass/__init__.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/buchdahl.py` & `opticalglass-1.0.5/src/opticalglass/buchdahl.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/caselessDictionary.py` & `opticalglass-1.0.5/src/opticalglass/caselessDictionary.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/cdgm.py` & `opticalglass-1.0.5/src/opticalglass/cdgm.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/CDGM.xls` & `opticalglass-1.0.5/src/opticalglass/data/CDGM.xls`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/HIKARI.xlsx` & `opticalglass-1.0.5/src/opticalglass/data/HIKARI.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/HIKARI_prev.xls` & `opticalglass-1.0.5/src/opticalglass/data/HIKARI_prev.xls`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/HOYA.xlsx` & `opticalglass-1.0.5/src/opticalglass/data/HOYA.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/HOYA_prev.xlsx` & `opticalglass-1.0.5/src/opticalglass/data/HOYA_prev.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/OHARA.xlsx` & `opticalglass-1.0.5/src/opticalglass/data/OHARA.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/OHARA_prev.xlsx` & `opticalglass-1.0.5/src/opticalglass/data/OHARA_prev.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/SCHOTT.xls` & `opticalglass-1.0.5/src/opticalglass/data/SCHOTT.xls`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/SCHOTT_prev.xls` & `opticalglass-1.0.5/src/opticalglass/data/SCHOTT_prev.xls`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/SUMITA.xlsx` & `opticalglass-1.0.5/src/opticalglass/data/SUMITA.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/data/robb1983_data_final.txt` & `opticalglass-1.0.5/src/opticalglass/data/robb1983_data_final.txt`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/glass.py` & `opticalglass-1.0.5/src/opticalglass/glass.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/glasserror.py` & `opticalglass-1.0.5/src/opticalglass/glasserror.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/glassfactory.py` & `opticalglass-1.0.5/src/opticalglass/glassfactory.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/glassmap.py` & `opticalglass-1.0.5/src/opticalglass/glassmap.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/glassmapviewer.py` & `opticalglass-1.0.5/src/opticalglass/glassmapviewer.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/glasspolygons.py` & `opticalglass-1.0.5/src/opticalglass/glasspolygons.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/hikari.py` & `opticalglass-1.0.5/src/opticalglass/hikari.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/hoya.py` & `opticalglass-1.0.5/src/opticalglass/hoya.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/modelglass.py` & `opticalglass-1.0.5/src/opticalglass/modelglass.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/ohara.py` & `opticalglass-1.0.5/src/opticalglass/ohara.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/openpyxl_script.py` & `opticalglass-1.0.5/src/opticalglass/openpyxl_script.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/opticalmedium.py` & `opticalglass-1.0.5/src/opticalglass/opticalmedium.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/rindexinfo.py` & `opticalglass-1.0.5/src/opticalglass/rindexinfo.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import requests
 import urllib.parse
 
 import numpy as np
 from scipy.interpolate import interp1d
 
 import yaml
+import importlib
 
 from typing import Union
 from numpy.typing import NDArray
 
 from opticalglass.opticalmedium import OpticalMedium, InterpolatedMedium
 from .spectral_lines import get_wavelength
 
@@ -381,18 +382,34 @@
             self.kvals_wvls = self.wvls if kvals_wvls is None else kvals_wvls
             self.kvals = kvals
         self.label = label
         self._catalog_name = cat
 
     def __json_encode__(self):
         attrs = dict(vars(self))
+        attrs['cat'] = self._catalog_name
+        del attrs['_catalog_name']
+        del attrs['wvls']
         if hasattr(self, 'yaml_data'):
             del attrs['yaml_data']
+        # Save model name and function name of rndx_fct, so that fct can
+        #  restored later (hopefully)
+        del attrs['rndx_fct']
+        attrs['rndx_fct_module'] = self.rndx_fct.__module__
+        attrs['rndx_fct_name'] = self.rndx_fct.__name__
         return attrs
 
+    def __json_decode__(self, **attrs):
+        module_name = attrs.pop('rndx_fct_module')
+        fct_name = attrs.pop('rndx_fct_name')
+        # try to import module and look up function - then assign to rndx_fct
+        mod = importlib.import_module(module_name)
+        rndx_fct = getattr(mod, fct_name)
+        self.__init__(rndx_fct=rndx_fct, **attrs)
+
     def name(self) -> str:
         return self.label
 
     def catalog_name(self) -> str:
         return self._catalog_name
 
     def glass_code(self) -> str:
@@ -427,22 +444,23 @@
 
     def transmission_data(self, thi=10.0):
         t = thi*1.0e3
         t_vals = np.exp(-4.0*np.pi*t*self.kvals/self.kvals_wvls)
         return self.kvals_wvls, t_vals
 
 
-def summary_plots(opt_medium, opt_medium_yaml):
+def summary_plots(opt_medium, opt_medium_yaml=None):
     """ plot refractive index and thruput data, when available. """
     import matplotlib.pyplot as plt
-    print(f"{[d['type'] for d in opt_medium_yaml['DATA']]}")
+    if opt_medium_yaml is not None:
+        print(f"{[d['type'] for d in opt_medium_yaml['DATA']]}")
 
     plt.plot(opt_medium.wvls, opt_medium.calc_rindex(opt_medium.wvls), label='ref index')
 
     if getattr(opt_medium, 'kvals', None) is not None:
         plt.plot(opt_medium.kvals_wvls, opt_medium.kvals, label='k value')
         plt.plot(*opt_medium.transmission_data(), label='T @ 10mm')
 
     plt.title(f"{opt_medium.catalog_name()}: {opt_medium.name()}")
     plt.xlabel('wavelength (nm)')
 
-    plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
+    plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
```

### Comparing `opticalglass-1.0.4/src/opticalglass/schott.py` & `opticalglass-1.0.5/src/opticalglass/schott.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/spectral_lines.py` & `opticalglass-1.0.5/src/opticalglass/spectral_lines.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/sumita.py` & `opticalglass-1.0.5/src/opticalglass/sumita.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/cmd_line_example.py` & `opticalglass-1.0.5/src/opticalglass/test/cmd_line_example.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/test_cdgm.py` & `opticalglass-1.0.5/src/opticalglass/test/test_cdgm.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/test_glassfactory.py` & `opticalglass-1.0.5/src/opticalglass/test/test_glassfactory.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/test_hikari.py` & `opticalglass-1.0.5/src/opticalglass/test/test_hikari.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/test_hoya.py` & `opticalglass-1.0.5/src/opticalglass/test/test_hoya.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/test_ohara.py` & `opticalglass-1.0.5/src/opticalglass/test/test_ohara.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/test_schott.py` & `opticalglass-1.0.5/src/opticalglass/test/test_schott.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/test_sumita.py` & `opticalglass-1.0.5/src/opticalglass/test/test_sumita.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/test_transmission.py` & `opticalglass-1.0.5/src/opticalglass/test/test_transmission.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/test/util.py` & `opticalglass-1.0.5/src/opticalglass/test/util.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass/util.py` & `opticalglass-1.0.5/src/opticalglass/util.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.4/src/opticalglass.egg-info/PKG-INFO` & `opticalglass-1.0.5/src/opticalglass.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalglass
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tools for reading optical glass catalogs
 Home-page: https://github.com/mjhoptics/opticalglass
 Author: Michael J Hayford
 Author-email: mjhoptics@gmail.com
 License: BSD-3-Clause
 Keywords: glass, optical glass, refractive index, optics,,glass catalog
 Platform: any
@@ -45,14 +45,19 @@
     * Schott
     * Sumita
 
 .. note::
 
    All rights and ownership of the data is retained by the original owners, i.e the respective manufacturers.
 
+Interface to RefractiveIndex.INFO database
+------------------------------------------
+
+An interface to the RefractiveIndex.INFO database, using both the InterpolatedMedium and RIIMedium classes, is available.
+
 Documentation
 -------------
 
 The documentation for **opticalglass** is hosted at `Read the Docs <https://opticalglass.readthedocs.io>`_
 
 .. _pyscaffold-notes:
```

### Comparing `opticalglass-1.0.4/src/opticalglass.egg-info/SOURCES.txt` & `opticalglass-1.0.5/src/opticalglass.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 src/opticalglass/glassmapviewer.py
 src/opticalglass/glasspolygons.py
 src/opticalglass/hikari.py
 src/opticalglass/hoya.py
 src/opticalglass/modelglass.py
 src/opticalglass/ohara.py
 src/opticalglass/openpyxl_script.py
+src/opticalglass/optical_glass_agf_class.py
 src/opticalglass/opticalmedium.py
 src/opticalglass/rindexinfo.py
 src/opticalglass/schott.py
 src/opticalglass/spectral_lines.py
 src/opticalglass/sumita.py
 src/opticalglass/util.py
 src/opticalglass.egg-info/PKG-INFO
```

### Comparing `opticalglass-1.0.4/update/catupdate.py` & `opticalglass-1.0.5/update/catupdate.py`

 * *Files identical despite different names*

