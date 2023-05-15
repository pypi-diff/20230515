# Comparing `tmp/bdfrx-1.0.5.tar.gz` & `tmp/bdfrx-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdfrx-1.0.5.tar", last modified: Fri May  5 03:29:52 2023, max compression
+gzip compressed data, was "bdfrx-1.0.6.tar", last modified: Mon May 15 00:22:33 2023, max compression
```

## Comparing `bdfrx-1.0.5.tar` & `bdfrx-1.0.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.204241 bdfrx-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-05-05 03:29:38.000000 bdfrx-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-05 03:29:52.204241 bdfrx-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-05-05 03:29:38.000000 bdfrx-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.200241 bdfrx-1.0.5/bdfrx/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/bdfrx.db
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    23005 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/default_config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_authenticator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.204241 bdfrx-1.0.5/bdfrx/site_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/catbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/delay_for_reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/download_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/erome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.204241 bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/gfycat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/imgur.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/pornhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/redgifs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/self_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/vidble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/vreddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.200241 bdfrx-1.0.5/bdfrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-05 03:29:38.000000 bdfrx-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:29:52.208241 bdfrx-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.204241 bdfrx-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.021522 bdfrx-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-05-15 00:22:06.000000 bdfrx-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-15 00:22:33.021522 bdfrx-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-05-15 00:22:06.000000 bdfrx-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.013522 bdfrx-1.0.6/bdfrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/bdfrx.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/default_config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_authenticator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.017522 bdfrx-1.0.6/bdfrx/site_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/catbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/delay_for_reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/download_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/erome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.017522 bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/gfycat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/imgur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/pornhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/redgifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/self_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/vidble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/vreddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.013522 bdfrx-1.0.6/bdfrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-15 00:22:33.000000 bdfrx-1.0.6/bdfrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-15 00:22:06.000000 bdfrx-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 00:22:33.021522 bdfrx-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.021522 bdfrx-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_resource.py
```

### Comparing `bdfrx-1.0.5/LICENSE` & `bdfrx-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/PKG-INFO` & `bdfrx-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,15 +696,15 @@
 License-File: LICENSE
 
 # Bulk Downloader for Reddit x
 
 [![PyPI Status](https://img.shields.io/pypi/status/bdfrx?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![PyPI version](https://img.shields.io/pypi/v/bdfrx.svg?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![Python Test](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml)
-[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&label=linting)](https://github.com/charliermarsh/ruff)
+[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=Python)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 This is a tool to download submissions from Reddit. BDFRx is flexible and can be used in scripts if needed through an extensive command-line interface. [List of currently supported sources](#list-of-currently-supported-sources)
 
 If you wish to open an issue, please read [the guide on opening issues](docs/CONTRIBUTING.md#opening-an-issue) to ensure that your issue is clear and contains everything it needs to for the developers to investigate.
```

### Comparing `bdfrx-1.0.5/README.md` & `bdfrx-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Bulk Downloader for Reddit x
 
 [![PyPI Status](https://img.shields.io/pypi/status/bdfrx?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![PyPI version](https://img.shields.io/pypi/v/bdfrx.svg?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![Python Test](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml)
-[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&label=linting)](https://github.com/charliermarsh/ruff)
+[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=Python)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 This is a tool to download submissions from Reddit. BDFRx is flexible and can be used in scripts if needed through an extensive command-line interface. [List of currently supported sources](#list-of-currently-supported-sources)
 
 If you wish to open an issue, please read [the guide on opening issues](docs/CONTRIBUTING.md#opening-an-issue) to ensure that your issue is clear and contains everything it needs to for the developers to investigate.
```

### Comparing `bdfrx-1.0.5/bdfrx/__main__.py` & `bdfrx-1.0.6/bdfrx/__main__.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/bdfrx.db` & `bdfrx-1.0.6/bdfrx/bdfrx.db`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/completion.py` & `bdfrx-1.0.6/bdfrx/completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/configuration.py` & `bdfrx-1.0.6/bdfrx/configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/connector.py` & `bdfrx-1.0.6/bdfrx/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             if client_secret and client_secret.lower() == "none":
                 client_secret = None
             if not self.cfg_parser.has_option("DEFAULT", "user_token"):
                 logger.log(9, "Commencing OAuth2 authentication")
                 scopes = self.cfg_parser.get("DEFAULT", "scopes", fallback="identity, history, read, save")
                 scopes = OAuth2Authenticator.split_scopes(scopes)
                 oauth2_authenticator = OAuth2Authenticator(
-                    scopes=scopes,
+                    wanted_scopes=scopes,
                     client_id=client_id,
                     client_secret=client_secret,
                     user_agent=self.user_agent,
                 )
                 token = oauth2_authenticator.retrieve_new_token()
                 self.cfg_parser["DEFAULT"]["user_token"] = token
                 with Path(self.config_location).open(mode="w") as file:
```

### Comparing `bdfrx-1.0.5/bdfrx/download_filter.py` & `bdfrx-1.0.6/bdfrx/download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/downloader.py` & `bdfrx-1.0.6/bdfrx/downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/file_name_formatter.py` & `bdfrx-1.0.6/bdfrx/file_name_formatter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/oauth2.py` & `bdfrx-1.0.6/bdfrx/oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/resource.py` & `bdfrx-1.0.6/bdfrx/resource.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/base_downloader.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/catbox.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/catbox.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/delay_for_reddit.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/delay_for_reddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/direct.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/direct.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/download_factory.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/download_factory.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/erome.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/erome.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/gallery.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/gallery.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/gfycat.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/gfycat.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/imgur.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/imgur.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/pornhub.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/pornhub.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/redgifs.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/redgifs.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/self_post.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/self_post.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/vidble.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/vidble.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/vreddit.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/vreddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx/site_downloaders/youtube.py` & `bdfrx-1.0.6/bdfrx/site_downloaders/youtube.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/bdfrx.egg-info/PKG-INFO` & `bdfrx-1.0.6/bdfrx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,15 +696,15 @@
 License-File: LICENSE
 
 # Bulk Downloader for Reddit x
 
 [![PyPI Status](https://img.shields.io/pypi/status/bdfrx?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![PyPI version](https://img.shields.io/pypi/v/bdfrx.svg?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![Python Test](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml)
-[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&label=linting)](https://github.com/charliermarsh/ruff)
+[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=Python)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 This is a tool to download submissions from Reddit. BDFRx is flexible and can be used in scripts if needed through an extensive command-line interface. [List of currently supported sources](#list-of-currently-supported-sources)
 
 If you wish to open an issue, please read [the guide on opening issues](docs/CONTRIBUTING.md#opening-an-issue) to ensure that your issue is clear and contains everything it needs to for the developers to investigate.
```

### Comparing `bdfrx-1.0.5/bdfrx.egg-info/SOURCES.txt` & `bdfrx-1.0.6/bdfrx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/pyproject.toml` & `bdfrx-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 package-data = {"bdfrx" = ["default_config.cfg", "bdfrx.db",]}
 
 [project.optional-dependencies]
 dev = [
     "black>=23.3.0",
     "pre-commit>=3.3.1",
     "pytest>=7.3.1",
-    "refurb>=1.16.0",
     "ruff>=0.0.264",
 ]
 
 [project.urls]
 "Homepage" = "https://omegarazer.github.io/bulk-downloader-for-reddit-x"
 "Source" = "https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x"
 "Bug Reports" = "https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/issues"
```

### Comparing `bdfrx-1.0.5/tests/test_completion.py` & `bdfrx-1.0.6/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/tests/test_configuration.py` & `bdfrx-1.0.6/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/tests/test_connector.py` & `bdfrx-1.0.6/tests/test_connector.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/tests/test_download_filter.py` & `bdfrx-1.0.6/tests/test_download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/tests/test_downloader.py` & `bdfrx-1.0.6/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/tests/test_file_name_formatter.py` & `bdfrx-1.0.6/tests/test_file_name_formatter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/tests/test_oauth2.py` & `bdfrx-1.0.6/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.5/tests/test_resource.py` & `bdfrx-1.0.6/tests/test_resource.py`

 * *Files identical despite different names*

