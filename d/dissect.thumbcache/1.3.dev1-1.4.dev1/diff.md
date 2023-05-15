# Comparing `tmp/dissect.thumbcache-1.3.dev1.tar.gz` & `tmp/dissect.thumbcache-1.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.thumbcache-1.3.dev1.tar", last modified: Thu Mar 16 13:05:09 2023, max compression
+gzip compressed data, was "dissect.thumbcache-1.4.dev1.tar", last modified: Mon May 15 12:48:41 2023, max compression
```

## Comparing `dissect.thumbcache-1.3.dev1.tar` & `dissect.thumbcache-1.4.dev1.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.273059 dissect.thumbcache-1.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-16 13:04:50.000000 dissect.thumbcache-1.3.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-03-16 13:05:09.273059 dissect.thumbcache-1.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.241058 dissect.thumbcache-1.3.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.245058 dissect.thumbcache-1.3.dev1/dissect/thumbcache/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/c_thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/thumbcache_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.245058 dissect.thumbcache-1.3.dev1/dissect/thumbcache/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/tools/extract_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/tools/extract_with_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/dissect/thumbcache/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.241058 dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-03-16 13:05:09.000000 dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-03-16 13:05:09.000000 dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:05:09.000000 dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-16 13:05:09.000000 dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:05:09.000000 dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:05:09.000000 dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-16 13:04:56.000000 dissect.thumbcache-1.3.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:05:09.273059 dissect.thumbcache-1.3.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.245058 dissect.thumbcache-1.3.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.241058 dissect.thumbcache-1.3.dev1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.253058 dissect.thumbcache-1.3.dev1/tests/data/windows_10/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_1280.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_1920.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_2560.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_768.db
--rw-r--r--   0 runner    (1001) docker     (123)  3145728 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_custom_stream.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.261058 dissect.thumbcache-1.3.dev1/tests/data/windows_11/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_1280.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_1920.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_2560.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_768.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_custom_stream.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.261058 dissect.thumbcache-1.3.dev1/tests/data/windows_7/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_7/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_7/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_7/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_7/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_7/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_7/thumbcache_sr.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.265059 dissect.thumbcache-1.3.dev1/tests/data/windows_81/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_1600.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:09.273059 dissect.thumbcache-1.3.dev1/tests/data/windows_vista/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/test_thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tests/test_thumbcachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:04:51.000000 dissect.thumbcache-1.3.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.571665 dissect.thumbcache-1.4.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.575666 dissect.thumbcache-1.4.dev1/dissect/thumbcache/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/c_thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/thumbcache_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.575666 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/extract_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/extract_with_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.575666 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-15 12:48:29.000000 dissect.thumbcache-1.4.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.575666 dissect.thumbcache-1.4.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.571665 dissect.thumbcache-1.4.dev1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.587666 dissect.thumbcache-1.4.dev1/tests/data/windows_10/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_1280.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_1920.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_2560.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_768.db
+-rw-r--r--   0 runner    (1001) docker     (123)  3145728 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_custom_stream.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.595667 dissect.thumbcache-1.4.dev1/tests/data/windows_11/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_1280.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_1920.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_2560.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_768.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_custom_stream.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.595667 dissect.thumbcache-1.4.dev1/tests/data/windows_7/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_sr.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.599667 dissect.thumbcache-1.4.dev1/tests/data/windows_81/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_1600.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_sr.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/test_thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/test_thumbcachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tox.ini
```

### Comparing `dissect.thumbcache-1.3.dev1/LICENSE` & `dissect.thumbcache-1.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/PKG-INFO` & `dissect.thumbcache-1.4.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.thumbcache
-Version: 1.3.dev1
+Version: 1.4.dev1
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
 Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.9
```

### Comparing `dissect.thumbcache-1.3.dev1/README.md` & `dissect.thumbcache-1.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/dissect/thumbcache/c_thumbcache.py` & `dissect.thumbcache-1.4.dev1/dissect/thumbcache/c_thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/dissect/thumbcache/index.py` & `dissect.thumbcache-1.4.dev1/dissect/thumbcache/index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/dissect/thumbcache/thumbcache.py` & `dissect.thumbcache-1.4.dev1/dissect/thumbcache/thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/dissect/thumbcache/thumbcache_file.py` & `dissect.thumbcache-1.4.dev1/dissect/thumbcache/thumbcache_file.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/dissect/thumbcache/tools/extract_images.py` & `dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/extract_images.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/dissect/thumbcache/tools/extract_with_index.py` & `dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/extract_with_index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/dissect/thumbcache/tools/utils.py` & `dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/PKG-INFO` & `dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.thumbcache
-Version: 1.3.dev1
+Version: 1.4.dev1
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
 Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.9
```

### Comparing `dissect.thumbcache-1.3.dev1/dissect.thumbcache.egg-info/SOURCES.txt` & `dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -74,8 +74,11 @@
 tests/data/windows_81/thumbcache_wide.db
 tests/data/windows_81/thumbcache_wide_alternate.db
 tests/data/windows_vista/thumbcache_1024.db
 tests/data/windows_vista/thumbcache_256.db
 tests/data/windows_vista/thumbcache_32.db
 tests/data/windows_vista/thumbcache_96.db
 tests/data/windows_vista/thumbcache_idx.db
-tests/data/windows_vista/thumbcache_sr.db
+tests/data/windows_vista/thumbcache_sr.db
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.thumbcache-1.3.dev1/pyproject.toml` & `dissect.thumbcache-1.4.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_16.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_16.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_256.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_32.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_96.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_96.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_10/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_16.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_16.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_256.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_32.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_48.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_48.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_11/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_7/thumbcache_256.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_7/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_256.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_32.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_81/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_256.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_32.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_96.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_96.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/data/windows_vista/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/test_index.py` & `dissect.thumbcache-1.4.dev1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/test_thumbcache.py` & `dissect.thumbcache-1.4.dev1/tests/test_thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tests/test_thumbcachefile.py` & `dissect.thumbcache-1.4.dev1/tests/test_thumbcachefile.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.3.dev1/tox.ini` & `dissect.thumbcache-1.4.dev1/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -51,7 +51,27 @@
 
 [flake8]
 max-line-length = 120
 extend-ignore =
     # See https://github.com/PyCQA/pycodestyle/issues/373
     E203,
 statistics = True
+
+[testenv:docs-build]
+allowlist_externals = make
+deps =
+    sphinx
+    sphinx-autoapi
+    sphinx_argparse_cli
+    sphinx-copybutton
+    sphinx-design
+    furo
+commands =
+    make -C tests/docs clean
+    make -C tests/docs html
+
+[testenv:docs-linkcheck]
+allowlist_externals = make
+deps = {[testenv:docs-build]deps}
+commands =
+    make -C tests/docs clean
+    make -C tests/docs linkcheck
```

