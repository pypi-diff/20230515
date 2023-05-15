# Comparing `tmp/pymadx-2.0.0.tar.gz` & `tmp/pymadx-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymadx-2.0.0.tar", last modified: Fri Mar 17 08:58:59 2023, max compression
+gzip compressed data, was "pymadx-2.0.1.tar", last modified: Mon May 15 09:19:07 2023, max compression
```

## Comparing `pymadx-2.0.0.tar` & `pymadx-2.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.688465 pymadx-2.0.0/
--rw-r--r--   0 lnevay     (501) staff       (20)      180 2023-03-16 11:05:21.000000 pymadx-2.0.0/.gitignore
--rw-r--r--   0 lnevay     (501) staff       (20)    35148 2020-05-18 14:15:57.000000 pymadx-2.0.0/COPYING.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      614 2020-05-18 14:15:57.000000 pymadx-2.0.0/LICENCE.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      694 2023-03-16 11:03:10.000000 pymadx-2.0.0/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)     2391 2023-03-17 08:58:59.688583 pymadx-2.0.0/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      652 2023-03-16 13:42:46.000000 pymadx-2.0.0/README.md
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.678573 pymadx-2.0.0/docs/
--rw-r--r--   0 lnevay     (501) staff       (20)      610 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)      808 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/make.bat
--rw-r--r--   0 lnevay     (501) staff       (20)   339117 2023-03-16 13:46:02.000000 pymadx-2.0.0/docs/pymadx.pdf
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.681682 pymadx-2.0.0/docs/source/
--rw-r--r--   0 lnevay     (501) staff       (20)      187 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/source/authorship.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      997 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/source/building.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5479 2023-03-16 11:07:33.000000 pymadx-2.0.0/docs/source/conf.py
--rw-r--r--   0 lnevay     (501) staff       (20)      610 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/source/converting.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.681916 pymadx-2.0.0/docs/source/figures/
--rw-r--r--   0 lnevay     (501) staff       (20)    29085 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/source/figures/optics.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)      550 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/source/index.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      998 2023-03-16 13:43:41.000000 pymadx-2.0.0/docs/source/installation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      904 2023-03-15 23:03:59.000000 pymadx-2.0.0/docs/source/licence.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1026 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/source/moduledocs.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5010 2020-05-18 14:15:57.000000 pymadx-2.0.0/docs/source/plotting.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     6895 2022-04-26 16:30:09.000000 pymadx-2.0.0/docs/source/tfsloading.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     4499 2023-03-16 11:16:00.000000 pymadx-2.0.0/docs/source/version_history.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1324 2023-03-17 08:37:56.000000 pymadx-2.0.0/pyproject.toml
--rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-03-17 08:58:59.688875 pymadx-2.0.0/setup.cfg
--rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-16 10:54:27.000000 pymadx-2.0.0/setup.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.676107 pymadx-2.0.0/src/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.682750 pymadx-2.0.0/src/obsolete/
--rw-r--r--   0 lnevay     (501) staff       (20)     5635 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/obsolete/TfsArray.py
--rw-r--r--   0 lnevay     (501) staff       (20)      835 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/obsolete/_Convert_depr.py
--rw-r--r--   0 lnevay     (501) staff       (20)     7506 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/obsolete/_Visualisation_deprecated.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.685106 pymadx-2.0.0/src/pymadx/
--rw-r--r--   0 lnevay     (501) staff       (20)     5225 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/Beam.py
--rw-r--r--   0 lnevay     (501) staff       (20)    15037 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/Builder.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.686607 pymadx-2.0.0/src/pymadx/Compare/
--rw-r--r--   0 lnevay     (501) staff       (20)     5137 2022-09-07 09:32:28.000000 pymadx-2.0.0/src/pymadx/Compare/_MadxMadxComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     5169 2022-09-07 09:33:07.000000 pymadx-2.0.0/src/pymadx/Compare/_MadxTransportComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      169 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/Compare/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.687494 pymadx-2.0.0/src/pymadx/Convert/
--rw-r--r--   0 lnevay     (501) staff       (20)      334 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/Convert/_Mad8ToMadx.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12503 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/Convert/_TfsToPtc.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     4405 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/Convert/_Transport2Madx.py
--rw-r--r--   0 lnevay     (501) staff       (20)      338 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/Convert/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    60175 2022-09-07 09:32:54.000000 pymadx-2.0.0/src/pymadx/Data.py
--rw-r--r--   0 lnevay     (501) staff       (20)    23024 2022-02-07 20:10:21.000000 pymadx-2.0.0/src/pymadx/Plot.py
--rw-r--r--   0 lnevay     (501) staff       (20)     9189 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/Ptc.py
--rw-r--r--   0 lnevay     (501) staff       (20)    18684 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/PtcAnalysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1325 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/_General.py
--rw-r--r--   0 lnevay     (501) staff       (20)     7578 2020-05-18 14:15:57.000000 pymadx-2.0.0/src/pymadx/_Mad8.py
--rw-r--r--   0 lnevay     (501) staff       (20)      783 2023-03-15 23:02:35.000000 pymadx-2.0.0/src/pymadx/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-03-17 08:58:59.000000 pymadx-2.0.0/src/pymadx/_version.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.686015 pymadx-2.0.0/src/pymadx.egg-info/
--rw-r--r--   0 lnevay     (501) staff       (20)     2391 2023-03-17 08:58:59.000000 pymadx-2.0.0/src/pymadx.egg-info/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)     1332 2023-03-17 08:58:59.000000 pymadx-2.0.0/src/pymadx.egg-info/SOURCES.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-17 08:58:59.000000 pymadx-2.0.0/src/pymadx.egg-info/dependency_links.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-16 11:01:01.000000 pymadx-2.0.0/src/pymadx.egg-info/not-zip-safe
--rw-r--r--   0 lnevay     (501) staff       (20)       74 2023-03-17 08:58:59.000000 pymadx-2.0.0/src/pymadx.egg-info/requires.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        7 2023-03-17 08:58:59.000000 pymadx-2.0.0/src/pymadx.egg-info/top_level.txt
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.687714 pymadx-2.0.0/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:15:57.000000 pymadx-2.0.0/tests/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.687833 pymadx-2.0.0/tests/test_input/
--rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:15:57.000000 pymadx-2.0.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-17 08:58:59.688305 pymadx-2.0.0/tests/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:15:57.000000 pymadx-2.0.0/tests/tests/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      565 2020-05-18 14:15:57.000000 pymadx-2.0.0/tests/tests/test_Data.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.206402 pymadx-2.0.1/
+-rw-r--r--   0 lnevay     (501) staff       (20)      180 2023-03-16 11:05:21.000000 pymadx-2.0.1/.gitignore
+-rw-r--r--   0 lnevay     (501) staff       (20)    35148 2020-05-18 14:15:57.000000 pymadx-2.0.1/COPYING.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      614 2023-03-17 09:00:20.000000 pymadx-2.0.1/LICENCE.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      694 2023-03-16 11:03:10.000000 pymadx-2.0.1/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)     2437 2023-05-15 09:19:07.206503 pymadx-2.0.1/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      652 2023-03-16 13:42:46.000000 pymadx-2.0.1/README.md
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.197025 pymadx-2.0.1/docs/
+-rw-r--r--   0 lnevay     (501) staff       (20)      610 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)      808 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/make.bat
+-rw-r--r--   0 lnevay     (501) staff       (20)   339117 2023-03-16 13:46:02.000000 pymadx-2.0.1/docs/pymadx.pdf
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.199729 pymadx-2.0.1/docs/source/
+-rw-r--r--   0 lnevay     (501) staff       (20)      187 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/source/authorship.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      997 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/source/building.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5479 2023-03-16 11:07:33.000000 pymadx-2.0.1/docs/source/conf.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      610 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/source/converting.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.199844 pymadx-2.0.1/docs/source/figures/
+-rw-r--r--   0 lnevay     (501) staff       (20)    29085 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/source/figures/optics.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)      550 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/source/index.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      998 2023-03-16 13:43:41.000000 pymadx-2.0.1/docs/source/installation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      904 2023-03-15 23:03:59.000000 pymadx-2.0.1/docs/source/licence.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1026 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/source/moduledocs.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5010 2020-05-18 14:15:57.000000 pymadx-2.0.1/docs/source/plotting.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     6895 2022-04-26 16:30:09.000000 pymadx-2.0.1/docs/source/tfsloading.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     4719 2023-05-15 09:17:45.000000 pymadx-2.0.1/docs/source/version_history.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1371 2023-05-15 09:14:43.000000 pymadx-2.0.1/pyproject.toml
+-rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-05-15 09:19:07.206754 pymadx-2.0.1/setup.cfg
+-rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-16 10:54:27.000000 pymadx-2.0.1/setup.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.194408 pymadx-2.0.1/src/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.200437 pymadx-2.0.1/src/obsolete/
+-rw-r--r--   0 lnevay     (501) staff       (20)     5635 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/obsolete/TfsArray.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      835 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/obsolete/_Convert_depr.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     7506 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/obsolete/_Visualisation_deprecated.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.203049 pymadx-2.0.1/src/pymadx/
+-rw-r--r--   0 lnevay     (501) staff       (20)     5225 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/Beam.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    15037 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.204968 pymadx-2.0.1/src/pymadx/Compare/
+-rw-r--r--   0 lnevay     (501) staff       (20)     5137 2022-09-07 09:32:28.000000 pymadx-2.0.1/src/pymadx/Compare/_MadxMadxComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     5169 2022-09-07 09:33:07.000000 pymadx-2.0.1/src/pymadx/Compare/_MadxTransportComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      169 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/Compare/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.205720 pymadx-2.0.1/src/pymadx/Convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)      334 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/Convert/_Mad8ToMadx.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12503 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/Convert/_TfsToPtc.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     4405 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/Convert/_Transport2Madx.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      338 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/Convert/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    60193 2023-03-27 10:03:16.000000 pymadx-2.0.1/src/pymadx/Data.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    25130 2023-04-17 11:50:06.000000 pymadx-2.0.1/src/pymadx/Plot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     9189 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/Ptc.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    18684 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/PtcAnalysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1325 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/_General.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     7578 2020-05-18 14:15:57.000000 pymadx-2.0.1/src/pymadx/_Mad8.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      783 2023-03-15 23:02:35.000000 pymadx-2.0.1/src/pymadx/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-05-15 09:19:07.000000 pymadx-2.0.1/src/pymadx/_version.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.204460 pymadx-2.0.1/src/pymadx.egg-info/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2437 2023-05-15 09:19:07.000000 pymadx-2.0.1/src/pymadx.egg-info/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)     1332 2023-05-15 09:19:07.000000 pymadx-2.0.1/src/pymadx.egg-info/SOURCES.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-05-15 09:19:07.000000 pymadx-2.0.1/src/pymadx.egg-info/dependency_links.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-16 11:01:01.000000 pymadx-2.0.1/src/pymadx.egg-info/not-zip-safe
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2023-05-15 09:19:07.000000 pymadx-2.0.1/src/pymadx.egg-info/requires.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        7 2023-05-15 09:19:07.000000 pymadx-2.0.1/src/pymadx.egg-info/top_level.txt
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.205846 pymadx-2.0.1/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:15:57.000000 pymadx-2.0.1/tests/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.205939 pymadx-2.0.1/tests/test_input/
+-rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:15:57.000000 pymadx-2.0.1/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:19:07.206282 pymadx-2.0.1/tests/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:15:57.000000 pymadx-2.0.1/tests/tests/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      565 2020-05-18 14:15:57.000000 pymadx-2.0.1/tests/tests/test_Data.py
```

### Comparing `pymadx-2.0.0/COPYING.txt` & `pymadx-2.0.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/LICENCE.txt` & `pymadx-2.0.1/LICENCE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pymadx Copyright (C) Royal Holloway, University of London 2020
+pymadx Copyright (C) Royal Holloway, University of London 2023
 
 pymadx is free software: you can redistribute it and/or modify 
 it under the terms of the GNU General Public License as published 
 by the Free Software Foundation version 3 of the License.
 
 pymadx is distributed in the hope that it will be useful, but 
 WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `pymadx-2.0.0/Makefile` & `pymadx-2.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/PKG-INFO` & `pymadx-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pymadx
-Version: 2.0.0
+Version: 2.0.1
 Summary: Package for loading MADX output.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
-License: pymadx Copyright (C) Royal Holloway, University of London 2020
+License: pymadx Copyright (C) Royal Holloway, University of London 2023
         
         pymadx is free software: you can redistribute it and/or modify 
         it under the terms of the GNU General Public License as published 
         by the Free Software Foundation version 3 of the License.
         
         pymadx is distributed in the hope that it will be useful, but 
         WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -29,18 +29,20 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pytransport
+Provides-Extra: dev
 License-File: LICENCE.txt
+License-File: COPYING.txt
 
 #pymadx#
 
 A python package containing both utilities for processing and analysing MADX output.
 
 ## Authors ##
```

### Comparing `pymadx-2.0.0/README.md` & `pymadx-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/Makefile` & `pymadx-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/make.bat` & `pymadx-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/pymadx.pdf` & `pymadx-2.0.1/docs/pymadx.pdf`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/building.rst` & `pymadx-2.0.1/docs/source/building.rst`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/conf.py` & `pymadx-2.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/converting.rst` & `pymadx-2.0.1/docs/source/converting.rst`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/figures/optics.pdf` & `pymadx-2.0.1/docs/source/figures/optics.pdf`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/index.rst` & `pymadx-2.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/installation.rst` & `pymadx-2.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/licence.rst` & `pymadx-2.0.1/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/moduledocs.rst` & `pymadx-2.0.1/docs/source/moduledocs.rst`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/plotting.rst` & `pymadx-2.0.1/docs/source/plotting.rst`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/tfsloading.rst` & `pymadx-2.0.1/docs/source/tfsloading.rst`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/docs/source/version_history.rst` & `pymadx-2.0.1/docs/source/version_history.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 ===============
 Version History
 ===============
 
-v 2.0.0 - 2023 / 03 / 16
-========================
+v2.0.1 - 2023 / 05 / 15
+=======================
+
+* Reduce Python version requirement to >3.6 instead of 3.7.
+* :code:`pymadx[dev]` installation feature in pip to allow testing / manual requirements.
+* Start of R-Matrix plots - in development.
+
+v2.0.0 - 2023 / 03 / 16
+=======================
 
 * Move to Python 3 entirely. Require at least Python 3.7.
 * Package layout and build system changed to more modern declarative package.
   All source code is now in :code:`pymadx/src/pymadx`. The version number
   throughout the code is dynamically generated from the git tag.
 * Added plot for 1 or 2 machine diagrams only.
 * Fix aperture plots due to typo in code.
 * Fix string type comparison for modern Python (i.e. don't use numpy internal alises).
 
 
-v 1.8.2 - 2021 / 06 / 16
-========================
+v1.8.2 - 2021 / 06 / 16
+=======================
 
 * Fix for plot name filtering.
 * Tweaked orange for solenoids.
 
 
-v 1.8.1 - 2020 / 12 / 16
-========================
+v1.8.1 - 2020 / 12 / 16
+=======================
 
 * Fix for step size in Tfs slicing.
 * More tolerant plotting for machine diagrams with just keyword, S and L as colums (ignoring K1L).
 * Ensure machine diagram x limit is full machine length by default.
 
 
-v 1.8.0 - 2019 / 06 / 08
-========================
+v1.8.0 - 2019 / 06 / 08
+=======================
 
 New Features
 ------------
 
 * Switch to Python 3. Should be Python 2.7 compatible.
 * Venv support in Makefile thanks to Kyrre Ness Sjoebaek.
 * Ability to write out a Tfs instance permitting comlete loading, editing and writing.
@@ -47,56 +54,56 @@
   use it to compare larger amplitude particle tracking where the approximate
   Hamiltonian can be quite wrong.
 * Tolerate minimal aperture columns. i.e. only APER_1. Have to do this
   as there's no standard in writing out apertures and everyone picks their
   own with missing bits of information.
 
 
-v 1.7.1 - 2019 / 04 / 20
-========================
+v1.7.1 - 2019 / 04 / 20
+=======================
 
 Bug Fixes
 ---------
 
 * Fix Data.Aperture.RemoveBelowValue logic, which also applies to GetNonZeroItems.
 * Tolerate no pytransport at import.
 
 
-v 1.7 - 2019 / 02 / 27
-======================
+v1.7 - 2019 / 02 / 27
+=====================
 
 New Features
 ------------
 
 * Return PTC beam definition from the Beam class.
 * Print basic beam summary from TFS file for given element.
 * Ability to split an element loaded from a TFS file correctly.
 
 General
 -------
 
 * Update copyright for 2019.
 
 
-v 1.6 - 2018 / 12 / 12
-======================
+v1.6 - 2018 / 12 / 12
+=====================
 
 General
 -------
 
 * Reimplemented machine diagram drawing to be more efficient when zooming and
   fix zordering so bends and then quadrupoles are always on top.
 * Dispersion optional for optics plotting.
 * H1 and H2 now passed through conversion of MADX TFS to PTC input format.
 * Solenoid added to MADX TFS to PTC converter.
 * Revised bend conversion for MADX TFS to PTC converter.
   
 
-v 1.5 - 2018 / 08 / 24
-======================
+v1.5 - 2018 / 08 / 24
+=====================
 
 New Features
 ------------
 
 * Support for tkicker.
 * Support for kickers in MADX to PTC.
 
@@ -107,29 +114,29 @@
 
 Bug Fixes
 ---------
 
 * Several bugs in Aperture class fixed.
 
 
-v 1.4 - 2018 / 06 / 23
-======================
+v1.4 - 2018 / 06 / 23
+=====================
 
 New Features
 ------------
 
 * Support of just gzipped files as well as tar gzipped.
 
 General
 -------
 
 * Improved SixTrack aperture handling.
 
-v 1.2 - 2018 / 05 / 23
-======================
+v1.2 - 2018 / 05 / 23
+=====================
 
 New Features
 ------------
 
 * Write a beam class instance to a separate file.
 * Add ptc_track maximum aperture to a model.
 * Concatenate TFS instances.
@@ -146,16 +153,16 @@
   
 Bug Fixes
 ---------
 
 * Machine plot now deals with 'COLLIMATOR' type correctly.
 
 
-v 1.1 - 2018 / 04 / 10
-======================
+v1.1 - 2018 / 04 / 10
+=====================
 
 New Features
 ------------
 
 * Improved options for writing PTC job for accurate comparison.
 * Support for subrelativistic machines - correct MADX definition of dispersion.
 * Plots for beam size including dispersion.
@@ -169,16 +176,16 @@
   columns however are element specific (such as L).
 * Fixed exception catching.
 * Fix beam size for subrelativistic machines. MADX really provides Dx/Beta.
 * Fix index searching from S location.
 * Fix PTC analysis.
 * Fix conversion to PTC for fringe fields.
 
-v 1.0 - 2017 / 12 / 05
-======================
+v1.0 - 2017 / 12 / 05
+=====================
 
 New Features
 ------------
 
 * GPL3 licence introduced.
 * Compatability with PIP install system.
 * Manual.
```

### Comparing `pymadx-2.0.0/pyproject.toml` & `pymadx-2.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymadx"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 dynamic = ["version"]
 readme = "README.md"
 description = "Package for loading MADX output."
 license = {file = "LICENCE.txt"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -29,14 +29,15 @@
   "matplotlib>=3.0",
   "numpy>=1.14",
   "importlib-metadata"
 ]
 
 [project.optional-dependencies]
 pytransport = ["pytransport"]
+dev = ["pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 homepage = "http://www.pp.rhul.ac.uk/bdsim/pymadx"
 documentation = "http://www.pp.rhul.ac.uk/bdsim/pymadx"
 repository = "https://bitbucket.org/jairhul/pymadx"
 
 [build-system]
```

### Comparing `pymadx-2.0.0/src/obsolete/TfsArray.py` & `pymadx-2.0.1/src/obsolete/TfsArray.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/obsolete/_Convert_depr.py` & `pymadx-2.0.1/src/obsolete/_Convert_depr.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/obsolete/_Visualisation_deprecated.py` & `pymadx-2.0.1/src/obsolete/_Visualisation_deprecated.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/Beam.py` & `pymadx-2.0.1/src/pymadx/Beam.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/Builder.py` & `pymadx-2.0.1/src/pymadx/Builder.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/Compare/_MadxMadxComparison.py` & `pymadx-2.0.1/src/pymadx/Compare/_MadxMadxComparison.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/Compare/_MadxTransportComparison.py` & `pymadx-2.0.1/src/pymadx/Compare/_MadxTransportComparison.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/Convert/_TfsToPtc.py` & `pymadx-2.0.1/src/pymadx/Convert/_TfsToPtc.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/Convert/_Transport2Madx.py` & `pymadx-2.0.1/src/pymadx/Convert/_Transport2Madx.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/Data.py` & `pymadx-2.0.1/src/pymadx/Data.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,17 +235,19 @@
         self.names = self.columns
         if not {"ORIGIN", "DATE", "TIME", "TYPE"}.issubset(self.header):
             # This isn't TFS.  These are guaranteed in the manual
             # to be written to all TFS files.
             raise ValueError("Malformed TFS.")
 
     def _CalculateSigma(self):
-        """Tries to calculate the sigmas.  If the relevant columns are
+        """
+        Tries to calculate the sigmas.  If the relevant columns are
         not present, e.g. in the case of Tfs Aperture, then this does
-        nothing."""
+        nothing.
+        """
         # check for emittance and energy spread
         ex   = 1e-9
         ey   = 1e-9
         sige = 1e-4
         requiredVariablesH1 = set(['SIGE', 'EX', 'EY'])
         method1 = requiredVariablesH1.issubset(list(self.header.keys()))
         requiredVariablesH2 = set(['EXN', 'EYN', 'GAMMA'])
```

### Comparing `pymadx-2.0.0/src/pymadx/Plot.py` & `pymadx-2.0.1/src/pymadx/Plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,69 @@
     d['y']         = tfsobject.GetColumn('Y')
     d['sigmax']    = tfsobject.GetColumn('SIGMAX')
     d['sigmay']    = tfsobject.GetColumn('SIGMAY')
     d['sigmaxp']   = tfsobject.GetColumn('SIGMAXP')
     d['sigmayp']   = tfsobject.GetColumn('SIGMAYP')
     return d
 
+def _GetRMatrixDataFromTfs(tfsobject):
+    d = {}
+    for key in ['S', 'RE11', 'RE12', 'RE21', 'RE22', 'RE33', 'RE34', 'RE43', 'RE44', 'RE16', 'RE26', 'RE36', 'RE46']:
+        d[key.lower()] = tfsobject.GetColumn(key)
+    return d
+
+def RMatrixOptics(tfsfile, dx=1.0, dpx=1.0, dP=1.0, dy=1.0, dpy=1.0, title=None, outputfilename=None, machine=True):
+    """
+    Plot the propagation of 3 rays with dx, dy, dpx, dpy, and dE independently.
+    :param dx: displacement in x in mm that is propagated
+    :type dx: float
+    :param dpx: displacement in px (component of unit vector) in 1e-3 (e.g. mrad in small angle).
+    :type dpx: float
+    :param dP: displacement in momentum as a percentage
+    :type dP: float
+    :param dy: displacement in x in mm that is propagated
+    :type dy: float
+    :param dyx: displacement in px (component of unit vector) in 1e-3 (e.g. mrad in small angle).
+    :type dyx: float
+    """
+
+    import pymadx.Data as _Data
+    madx = _Data.CheckItsTfs(tfsfile)
+    d = _GetRMatrixDataFromTfs(madx)
+
+    xlabel   = 'x  = '+str(round(dx,3))+' mm'
+    xplabel  = 'xp = '+str(round(dpx,3))+' mrad'
+    xdplabel = 'dP = '+str(round(dP/1e2,3))+' %'
+
+    f1 = _plt.figure("Horizontal", figsize=(9,5))
+    axx = f1.add_subplot(111)
+    axx.plot(d['s'], d['re11']*dx*1e-3,  '-',  label=xlabel)
+    axx.plot(d['s'], d['re12']*dpx*1e-3, '--', label=xplabel)
+    axx.plot(d['s'], d['re16']*dP/1e2,  '-.', label=xdplabel)
+    _plt.legend()
+    _plt.xlabel('S (m)')
+    _plt.tight_layout()
+    if machine:
+        AddMachineLatticeToFigure(f1, madx)
+    
+    ylabel   = 'y  = '+str(round(dy,3))+' mm'
+    yplabel  = 'yp = '+str(round(dpy,3))+' mrad'
+    ydplabel = 'dP = '+str(round(dP/1e2,3))+' %'
+    
+    f2 = _plt.figure("Vertical", figsize=(9,5))
+    axy = f2.add_subplot(111)
+    axy.plot(d['s'], d['re33']*dy*1e-3,  '-',  label=ylabel)
+    axy.plot(d['s'], d['re34']*dpy*1e-3, '--', label=yplabel)
+    axy.plot(d['s'], d['re36']*dP/1e2,  '-.', label=ydplabel)
+    _plt.legend()
+    _plt.xlabel('S (m)')
+    _plt.tight_layout()
+    if machine:
+        AddMachineLatticeToFigure(f2, madx)
+
 def Centroids(tfsfile, title='', outputfilename=None, machine=True):
     """
     Plot the centroid (mean) x and y from the a Tfs file or pymadx.Tfs instance.
 
     tfsfile        - can be either a string or a pymadx.Tfs instance.
     title          - optional title for plot
     outputfilename - optional name to save file to (extension determines format)
```

### Comparing `pymadx-2.0.0/src/pymadx/Ptc.py` & `pymadx-2.0.1/src/pymadx/Ptc.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/PtcAnalysis.py` & `pymadx-2.0.1/src/pymadx/PtcAnalysis.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/_General.py` & `pymadx-2.0.1/src/pymadx/_General.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/_Mad8.py` & `pymadx-2.0.1/src/pymadx/_Mad8.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx/__init__.py` & `pymadx-2.0.1/src/pymadx/__init__.py`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/src/pymadx.egg-info/PKG-INFO` & `pymadx-2.0.1/src/pymadx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pymadx
-Version: 2.0.0
+Version: 2.0.1
 Summary: Package for loading MADX output.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
-License: pymadx Copyright (C) Royal Holloway, University of London 2020
+License: pymadx Copyright (C) Royal Holloway, University of London 2023
         
         pymadx is free software: you can redistribute it and/or modify 
         it under the terms of the GNU General Public License as published 
         by the Free Software Foundation version 3 of the License.
         
         pymadx is distributed in the hope that it will be useful, but 
         WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -29,18 +29,20 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pytransport
+Provides-Extra: dev
 License-File: LICENCE.txt
+License-File: COPYING.txt
 
 #pymadx#
 
 A python package containing both utilities for processing and analysing MADX output.
 
 ## Authors ##
```

### Comparing `pymadx-2.0.0/src/pymadx.egg-info/SOURCES.txt` & `pymadx-2.0.1/src/pymadx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz` & `pymadx-2.0.1/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz`

 * *Files identical despite different names*

### Comparing `pymadx-2.0.0/tests/tests/test_Data.py` & `pymadx-2.0.1/tests/tests/test_Data.py`

 * *Files identical despite different names*

