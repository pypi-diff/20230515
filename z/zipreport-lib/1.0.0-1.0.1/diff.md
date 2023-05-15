# Comparing `tmp/zipreport-lib-1.0.0.tar.gz` & `tmp/zipreport-lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipreport-lib-1.0.0.tar", last modified: Mon May  9 17:25:40 2022, max compression
+gzip compressed data, was "zipreport-lib-1.0.1.tar", last modified: Mon May 15 15:59:25 2023, max compression
```

## Comparing `zipreport-lib-1.0.0.tar` & `zipreport-lib-1.0.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1088 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/LICENSE
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4819 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3821 2022-05-09 17:20:24.000000 zipreport-lib-1.0.0/README.md
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       38 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/setup.cfg
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2487 2022-05-09 17:05:14.000000 zipreport-lib-1.0.0/setup.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/tests/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-22 16:58:01.000000 zipreport-lib-1.0.0/tests/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/tests/fileutils/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-22 12:25:07.000000 zipreport-lib-1.0.0/tests/fileutils/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5235 2020-07-24 10:35:50.000000 zipreport-lib-1.0.0/tests/fileutils/basefs.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      756 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/fileutils/basezip.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3454 2020-11-22 04:19:51.000000 zipreport-lib-1.0.0/tests/fileutils/test_diskfs.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1339 2020-07-23 10:00:42.000000 zipreport-lib-1.0.0/tests/fileutils/test_pathcache.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2547 2020-07-24 18:01:09.000000 zipreport-lib-1.0.0/tests/fileutils/test_zip.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1539 2020-07-24 10:35:50.000000 zipreport-lib-1.0.0/tests/fileutils/test_zipfs.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/tests/processors/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/processors/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      735 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/processors/base.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2843 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/processors/test_mime.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/tests/render/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/render/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      772 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/render/base.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/tests/render/filters/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/render/filters/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    16028 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/render/filters/base.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1968 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/render/filters/test_jinjafilters.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      590 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/render/test_jinjaloader.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1673 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/render/test_jinjarender.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/tests/report/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-23 07:55:01.000000 zipreport-lib-1.0.0/tests/report/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3281 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/report/test_builder.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2147 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/report/test_job.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1515 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/tests/report/test_loader.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      568 2020-11-22 04:42:34.000000 zipreport-lib-1.0.0/tests/utils.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      135 2022-05-09 17:01:37.000000 zipreport-lib-1.0.0/zipreport/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/cli/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/cli/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5221 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/cli/console.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/cli/debug/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/cli/debug/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     8476 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/cli/debug/server.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/fileutils/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       96 2020-07-23 04:44:59.000000 zipreport-lib-1.0.0/zipreport/fileutils/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/fileutils/backend/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-23 04:38:48.000000 zipreport-lib-1.0.0/zipreport/fileutils/backend/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4140 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/fileutils/backend/zip.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4801 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/fileutils/diskfs.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1398 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/fileutils/interface.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3630 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/fileutils/pathcache.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3838 2021-11-14 16:26:47.000000 zipreport-lib-1.0.0/zipreport/fileutils/zipfs.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/misc/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       27 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/misc/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      655 2020-11-22 04:42:34.000000 zipreport-lib-1.0.0/zipreport/misc/html.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/processors/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      200 2021-11-14 16:07:06.000000 zipreport-lib-1.0.0/zipreport/processors/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      143 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/processors/interface.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3001 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/processors/mime.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2211 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/processors/weasyprint.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3075 2021-11-14 16:07:06.000000 zipreport-lib-1.0.0/zipreport/processors/wkhtmltopdf.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4873 2020-10-14 10:13:11.000000 zipreport-lib-1.0.0/zipreport/processors/zipreport.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/report/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      207 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/report/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5827 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/report/builder.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1274 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/report/const.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5884 2020-11-22 04:56:45.000000 zipreport-lib-1.0.0/zipreport/report/job.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2603 2020-10-14 06:19:51.000000 zipreport-lib-1.0.0/zipreport/report/loader.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1901 2020-11-29 15:58:21.000000 zipreport-lib-1.0.0/zipreport/report/reportfile.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/template/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       80 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/template/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport/template/jinja/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/template/jinja/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4985 2022-05-09 17:10:20.000000 zipreport-lib-1.0.0/zipreport/template/jinja/filters.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      913 2020-10-14 06:18:55.000000 zipreport-lib-1.0.0/zipreport/template/jinjaloader.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3242 2020-11-29 15:58:28.000000 zipreport-lib-1.0.0/zipreport/template/jinjarender.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      126 2022-05-09 17:05:14.000000 zipreport-lib-1.0.0/zipreport/version.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3195 2021-11-14 16:07:06.000000 zipreport-lib-1.0.0/zipreport/zipreport.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-05-09 17:25:40.506673 zipreport-lib-1.0.0/zipreport_lib.egg-info/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4819 2022-05-09 17:25:40.000000 zipreport-lib-1.0.0/zipreport_lib.egg-info/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1929 2022-05-09 17:25:40.000000 zipreport-lib-1.0.0/zipreport_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-05-09 17:25:40.000000 zipreport-lib-1.0.0/zipreport_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       58 2022-05-09 17:25:40.000000 zipreport-lib-1.0.0/zipreport_lib.egg-info/entry_points.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-05-09 03:05:06.000000 zipreport-lib-1.0.0/zipreport_lib.egg-info/not-zip-safe
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       61 2022-05-09 17:25:40.000000 zipreport-lib-1.0.0/zipreport_lib.egg-info/requires.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       16 2022-05-09 17:25:40.000000 zipreport-lib-1.0.0/zipreport_lib.egg-info/top_level.txt
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1088 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/LICENSE
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4883 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/PKG-INFO
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3821 2022-05-09 17:32:34.000000 zipreport-lib-1.0.1/README.md
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       38 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/setup.cfg
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2551 2023-05-15 15:58:28.000000 zipreport-lib-1.0.1/setup.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.141871 zipreport-lib-1.0.1/tests/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-22 16:58:01.000000 zipreport-lib-1.0.1/tests/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/fileutils/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-22 12:25:07.000000 zipreport-lib-1.0.1/tests/fileutils/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5235 2020-07-24 10:35:50.000000 zipreport-lib-1.0.1/tests/fileutils/basefs.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      756 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/fileutils/basezip.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3454 2020-11-22 04:19:51.000000 zipreport-lib-1.0.1/tests/fileutils/test_diskfs.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1339 2020-07-23 10:00:42.000000 zipreport-lib-1.0.1/tests/fileutils/test_pathcache.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2547 2020-07-24 18:01:09.000000 zipreport-lib-1.0.1/tests/fileutils/test_zip.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1539 2020-07-24 10:35:50.000000 zipreport-lib-1.0.1/tests/fileutils/test_zipfs.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/processors/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/processors/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      735 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/processors/base.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2843 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/processors/test_mime.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/render/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      772 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/base.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/render/filters/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/filters/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    16028 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/filters/base.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1968 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/filters/test_jinjafilters.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      590 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/test_jinjaloader.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1673 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/test_jinjarender.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/report/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-23 07:55:01.000000 zipreport-lib-1.0.1/tests/report/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3281 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/report/test_builder.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2147 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/report/test_job.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1515 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/report/test_loader.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      568 2020-11-22 04:42:34.000000 zipreport-lib-1.0.1/tests/utils.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      135 2022-05-09 17:01:37.000000 zipreport-lib-1.0.1/zipreport/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/cli/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/cli/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5221 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/cli/console.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/cli/debug/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/cli/debug/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     8476 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/cli/debug/server.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/fileutils/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       96 2020-07-23 04:44:59.000000 zipreport-lib-1.0.1/zipreport/fileutils/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/fileutils/backend/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-23 04:38:48.000000 zipreport-lib-1.0.1/zipreport/fileutils/backend/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4140 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/fileutils/backend/zip.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4801 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/fileutils/diskfs.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1398 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/fileutils/interface.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3630 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/fileutils/pathcache.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3838 2021-11-14 16:26:47.000000 zipreport-lib-1.0.1/zipreport/fileutils/zipfs.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/misc/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       27 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/misc/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      655 2020-11-22 04:42:34.000000 zipreport-lib-1.0.1/zipreport/misc/html.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/processors/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      200 2021-11-14 16:07:06.000000 zipreport-lib-1.0.1/zipreport/processors/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      143 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/processors/interface.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3001 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/processors/mime.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2211 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/processors/weasyprint.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3075 2021-11-14 16:07:06.000000 zipreport-lib-1.0.1/zipreport/processors/wkhtmltopdf.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4873 2020-10-14 10:13:11.000000 zipreport-lib-1.0.1/zipreport/processors/zipreport.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/report/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      207 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/report/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5827 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/report/builder.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1274 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/report/const.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5884 2020-11-22 04:56:45.000000 zipreport-lib-1.0.1/zipreport/report/job.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2603 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/report/loader.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1901 2020-11-29 15:58:21.000000 zipreport-lib-1.0.1/zipreport/report/reportfile.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/template/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       80 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/template/__init__.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/template/jinja/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/template/jinja/__init__.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4985 2022-05-09 17:10:20.000000 zipreport-lib-1.0.1/zipreport/template/jinja/filters.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      913 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/template/jinjaloader.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3242 2020-11-29 15:58:28.000000 zipreport-lib-1.0.1/zipreport/template/jinjarender.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      126 2023-05-15 15:59:08.000000 zipreport-lib-1.0.1/zipreport/version.py
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3195 2021-11-14 16:07:06.000000 zipreport-lib-1.0.1/zipreport/zipreport.py
+drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport_lib.egg-info/
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4883 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1929 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       58 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-05-09 03:05:06.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       61 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/requires.txt
+-rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       16 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/top_level.txt
```

### Comparing `zipreport-lib-1.0.0/LICENSE` & `zipreport-lib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/PKG-INFO` & `zipreport-lib-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: Joao Pinheiro
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
 Project-URL: Tracker, https://github.com/zipreport/zipreport/issues
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Printing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: weasyprint
 License-File: LICENSE
@@ -44,15 +45,15 @@
 - Reports are packed in a single file for easy distribution or bundling;
 - Optional MIME processor to embed resources in a single email message;
 - Support for generated JS content (with zipreport-server or zipreport-cli);
 - Support for headers, page numbers and ToC (via PagedJS, see below);
 
 **Requirements**:
 
-- Python >= 3.6
+- Python >= 3.7
 - Jinja2 >= 3.1 
 - Compatible backend for pdf generation (zipreport-server, zipreport-cli, xhtmltopdf, or WeasyPrint);
 
 Note: For previous Jinja2 versions, zipreport-lib 0.9.5 is functionally similar.
 
 ### Installation
```

### Comparing `zipreport-lib-1.0.0/README.md` & `zipreport-lib-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - Reports are packed in a single file for easy distribution or bundling;
 - Optional MIME processor to embed resources in a single email message;
 - Support for generated JS content (with zipreport-server or zipreport-cli);
 - Support for headers, page numbers and ToC (via PagedJS, see below);
 
 **Requirements**:
 
-- Python >= 3.6
+- Python >= 3.7
 - Jinja2 >= 3.1 
 - Compatible backend for pdf generation (zipreport-server, zipreport-cli, xhtmltopdf, or WeasyPrint);
 
 Note: For previous Jinja2 versions, zipreport-lib 0.9.5 is functionally similar.
 
 ### Installation
```

### Comparing `zipreport-lib-1.0.0/setup.py` & `zipreport-lib-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,21 +39,22 @@
         'Tracker': 'https://github.com/zipreport/zipreport/issues',
     },
     python_requires='>={}.{}'.format(*REQUIRED_PYTHON),
     description='Python HTML to PDF reporting engine',
     license='MIT',
     long_description=description,
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Text Processing :: Markup :: HTML',
         'Topic :: Printing',
     ],
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
@@ -63,15 +64,15 @@
     install_requires=[
         "jinja2>=3.1",
         "requests>=2.22.0"
     ],
     zip_safe=False,
     tests_require=[
         "jinja2>=3.1",
-        "requests>=2.22.0"
+        "requests>=2.22.0",
         "coverage==4.4.1",
         "mock>=1.0.1",
         "flake8>=2.1.0",
         "tox>=1.7.0",
         "codecov>=2.0.0",
         "pytest-cov>=2.8.1",
     ],
```

### Comparing `zipreport-lib-1.0.0/tests/fileutils/basefs.py` & `zipreport-lib-1.0.1/tests/fileutils/basefs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/fileutils/basezip.py` & `zipreport-lib-1.0.1/tests/fileutils/basezip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/fileutils/test_diskfs.py` & `zipreport-lib-1.0.1/tests/fileutils/test_diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/fileutils/test_pathcache.py` & `zipreport-lib-1.0.1/tests/fileutils/test_pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/fileutils/test_zip.py` & `zipreport-lib-1.0.1/tests/fileutils/test_zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/fileutils/test_zipfs.py` & `zipreport-lib-1.0.1/tests/fileutils/test_zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/processors/base.py` & `zipreport-lib-1.0.1/tests/processors/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/processors/test_mime.py` & `zipreport-lib-1.0.1/tests/processors/test_mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/render/base.py` & `zipreport-lib-1.0.1/tests/render/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/render/filters/base.py` & `zipreport-lib-1.0.1/tests/render/filters/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/render/filters/test_jinjafilters.py` & `zipreport-lib-1.0.1/tests/render/filters/test_jinjafilters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/render/test_jinjaloader.py` & `zipreport-lib-1.0.1/tests/render/test_jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/render/test_jinjarender.py` & `zipreport-lib-1.0.1/tests/render/test_jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/report/test_builder.py` & `zipreport-lib-1.0.1/tests/report/test_builder.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/report/test_job.py` & `zipreport-lib-1.0.1/tests/report/test_job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/report/test_loader.py` & `zipreport-lib-1.0.1/tests/report/test_loader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/tests/utils.py` & `zipreport-lib-1.0.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/cli/console.py` & `zipreport-lib-1.0.1/zipreport/cli/console.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/cli/debug/server.py` & `zipreport-lib-1.0.1/zipreport/cli/debug/server.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/fileutils/backend/zip.py` & `zipreport-lib-1.0.1/zipreport/fileutils/backend/zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/fileutils/diskfs.py` & `zipreport-lib-1.0.1/zipreport/fileutils/diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/fileutils/interface.py` & `zipreport-lib-1.0.1/zipreport/fileutils/interface.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/fileutils/pathcache.py` & `zipreport-lib-1.0.1/zipreport/fileutils/pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/fileutils/zipfs.py` & `zipreport-lib-1.0.1/zipreport/fileutils/zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/misc/html.py` & `zipreport-lib-1.0.1/zipreport/misc/html.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/processors/mime.py` & `zipreport-lib-1.0.1/zipreport/processors/mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/processors/weasyprint.py` & `zipreport-lib-1.0.1/zipreport/processors/weasyprint.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/processors/wkhtmltopdf.py` & `zipreport-lib-1.0.1/zipreport/processors/wkhtmltopdf.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/processors/zipreport.py` & `zipreport-lib-1.0.1/zipreport/processors/zipreport.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/report/builder.py` & `zipreport-lib-1.0.1/zipreport/report/builder.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/report/const.py` & `zipreport-lib-1.0.1/zipreport/report/const.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/report/job.py` & `zipreport-lib-1.0.1/zipreport/report/job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/report/loader.py` & `zipreport-lib-1.0.1/zipreport/report/loader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/report/reportfile.py` & `zipreport-lib-1.0.1/zipreport/report/reportfile.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/template/jinja/filters.py` & `zipreport-lib-1.0.1/zipreport/template/jinja/filters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/template/jinjaloader.py` & `zipreport-lib-1.0.1/zipreport/template/jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/template/jinjarender.py` & `zipreport-lib-1.0.1/zipreport/template/jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport/zipreport.py` & `zipreport-lib-1.0.1/zipreport/zipreport.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.0/zipreport_lib.egg-info/PKG-INFO` & `zipreport-lib-1.0.1/zipreport_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: Joao Pinheiro
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
 Project-URL: Tracker, https://github.com/zipreport/zipreport/issues
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Printing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: weasyprint
 License-File: LICENSE
@@ -44,15 +45,15 @@
 - Reports are packed in a single file for easy distribution or bundling;
 - Optional MIME processor to embed resources in a single email message;
 - Support for generated JS content (with zipreport-server or zipreport-cli);
 - Support for headers, page numbers and ToC (via PagedJS, see below);
 
 **Requirements**:
 
-- Python >= 3.6
+- Python >= 3.7
 - Jinja2 >= 3.1 
 - Compatible backend for pdf generation (zipreport-server, zipreport-cli, xhtmltopdf, or WeasyPrint);
 
 Note: For previous Jinja2 versions, zipreport-lib 0.9.5 is functionally similar.
 
 ### Installation
```

### Comparing `zipreport-lib-1.0.0/zipreport_lib.egg-info/SOURCES.txt` & `zipreport-lib-1.0.1/zipreport_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

