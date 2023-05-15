# Comparing `tmp/pynamodb_mate-5.3.4.8.tar.gz` & `tmp/pynamodb_mate-5.3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb_mate-5.3.4.8.tar", last modified: Sat Feb  4 03:26:45 2023, max compression
+gzip compressed data, was "pynamodb_mate-5.3.4.9.tar", last modified: Mon May 15 05:54:30 2023, max compression
```

## Comparing `pynamodb_mate-5.3.4.8.tar` & `pynamodb_mate-5.3.4.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.994855 pynamodb_mate-5.3.4.8/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2021-12-12 20:41:31.000000 pynamodb_mate-5.3.4.8/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1123 2021-12-10 15:02:06.000000 pynamodb_mate-5.3.4.8/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      321 2023-01-02 00:03:52.000000 pynamodb_mate-5.3.4.8/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     6847 2023-02-04 03:26:45.994695 pynamodb_mate-5.3.4.8/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     5635 2023-01-03 16:25:39.000000 pynamodb_mate-5.3.4.8/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.988067 pynamodb_mate-5.3.4.8/pynamodb_mate/
--rw-r--r--   0 sanhehu    (505) staff       (20)     2528 2023-01-03 15:58:06.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       95 2023-02-04 03:24:30.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/_version.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.989984 pynamodb_mate-5.3.4.8/pynamodb_mate/attributes/
--rw-r--r--   0 sanhehu    (505) staff       (20)       60 2023-01-02 04:02:01.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/attributes/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1894 2023-01-03 15:46:56.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/attributes/compressed.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3694 2023-01-03 15:31:08.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/attributes/encrypted.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5370 2023-01-03 15:58:56.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/attributes/s3backed.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1764 2023-01-02 04:07:35.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/cipher.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      336 2023-01-02 03:26:54.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/compat.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.990246 pynamodb_mate-5.3.4.8/pynamodb_mate/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2021-12-10 15:02:06.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1321 2021-12-12 16:12:07.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/helpers.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    12065 2023-02-01 15:30:01.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/models.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.990483 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/
--rw-r--r--   0 sanhehu    (505) staff       (20)      109 2023-01-03 00:54:55.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.991514 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/
--rw-r--r--   0 sanhehu    (505) staff       (20)      393 2023-01-03 01:31:45.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3023 2023-01-03 01:32:05.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/abstract.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.992383 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/backend/
--rw-r--r--   0 sanhehu    (505) staff       (20)       33 2023-01-03 01:32:12.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/backend/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3561 2023-01-03 16:40:50.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/backend/dynamodb.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1866 2023-01-03 16:40:43.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/backend/in_memory.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1120 2022-08-09 02:32:09.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/multi_layer.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      152 2022-08-08 20:24:08.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/utils.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.992985 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/status_tracker/
--rw-r--r--   0 sanhehu    (505) staff       (20)      295 2023-02-04 00:12:17.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/status_tracker/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    27080 2023-02-04 03:09:58.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/status_tracker/impl.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.994354 pynamodb_mate-5.3.4.8/pynamodb_mate/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)      208 2023-02-01 15:30:01.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/tests/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      598 2023-02-01 15:30:01.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/tests/base.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1240 2023-01-02 00:03:52.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/tests/helper.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      370 2023-01-02 00:03:52.000000 pynamodb_mate-5.3.4.8/pynamodb_mate/tests/paths.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-04 03:26:45.988871 pynamodb_mate-5.3.4.8/pynamodb_mate.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     6847 2023-02-04 03:26:45.000000 pynamodb_mate-5.3.4.8/pynamodb_mate.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     1258 2023-02-04 03:26:45.000000 pynamodb_mate-5.3.4.8/pynamodb_mate.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-02-04 03:26:45.000000 pynamodb_mate-5.3.4.8/pynamodb_mate.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      378 2023-02-04 03:26:45.000000 pynamodb_mate-5.3.4.8/pynamodb_mate.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       14 2023-02-04 03:26:45.000000 pynamodb_mate-5.3.4.8/pynamodb_mate.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     6212 2023-02-04 00:32:25.000000 pynamodb_mate-5.3.4.8/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      208 2023-01-02 00:03:52.000000 pynamodb_mate-5.3.4.8/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      643 2023-01-02 00:03:52.000000 pynamodb_mate-5.3.4.8/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       13 2023-01-02 00:03:52.000000 pynamodb_mate-5.3.4.8/requirements-encrypt.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      189 2023-02-01 15:30:01.000000 pynamodb_mate-5.3.4.8/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      127 2023-02-01 15:30:01.000000 pynamodb_mate-5.3.4.8/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-02-04 03:26:45.994983 pynamodb_mate-5.3.4.8/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7555 2023-01-02 00:03:52.000000 pynamodb_mate-5.3.4.8/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.926158 pynamodb_mate-5.3.4.9/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2022-12-26 12:25:06.000000 pynamodb_mate-5.3.4.9/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2022-12-26 12:25:06.000000 pynamodb_mate-5.3.4.9/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      321 2022-12-26 13:43:20.000000 pynamodb_mate-5.3.4.9/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6908 2023-05-15 05:54:30.926000 pynamodb_mate-5.3.4.9/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5696 2023-02-17 04:31:53.000000 pynamodb_mate-5.3.4.9/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.921948 pynamodb_mate-5.3.4.9/pynamodb_mate/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2528 2023-01-17 00:25:46.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       95 2023-05-15 04:52:11.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.923203 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       60 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1894 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/compressed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3694 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/encrypted.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5370 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/s3backed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1764 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/cipher.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.923342 pynamodb_mate-5.3.4.9/pynamodb_mate/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2022-12-26 12:25:06.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1321 2022-12-26 12:25:06.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/helpers.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12065 2023-01-17 00:59:45.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/models.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.923523 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      109 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.924081 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      393 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3023 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/abstract.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.924484 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       33 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3561 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1866 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/in_memory.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/multi_layer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      152 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.924745 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/status_tracker/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-02-17 04:31:53.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/status_tracker/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    27101 2023-05-15 04:51:28.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/status_tracker/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.925688 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      208 2023-01-16 20:19:31.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      598 2023-01-16 20:34:26.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/base.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1240 2022-12-26 13:46:07.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2022-12-26 13:46:35.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.922660 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6908 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1258 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      378 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       14 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6475 2023-05-15 04:53:41.000000 pynamodb_mate-5.3.4.9/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      208 2022-12-26 13:49:49.000000 pynamodb_mate-5.3.4.9/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      643 2022-12-26 13:50:07.000000 pynamodb_mate-5.3.4.9/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       13 2022-12-26 13:47:00.000000 pynamodb_mate-5.3.4.9/requirements-encrypt.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      189 2023-01-16 19:59:46.000000 pynamodb_mate-5.3.4.9/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      127 2023-01-16 17:39:27.000000 pynamodb_mate-5.3.4.9/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-15 05:54:30.926198 pynamodb_mate-5.3.4.9/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7555 2022-12-26 13:48:05.000000 pynamodb_mate-5.3.4.9/setup.py
```

### Comparing `pynamodb_mate-5.3.4.8/LICENSE.txt` & `pynamodb_mate-5.3.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/PKG-INFO` & `pynamodb_mate-5.3.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pynamodb_mate
-Version: 5.3.4.8
+Version: 5.3.4.9
 Summary: Provide Additional Features for pynamodb.
 Home-page: https://github.com/MacHu-GWU/pynamodb_mate-project
-Download-URL: https://pypi.python.org/pypi/pynamodb_mate/5.3.4.8#downloads
+Download-URL: https://pypi.python.org/pypi/pynamodb_mate/5.3.4.9#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -47,14 +47,16 @@
 
 .. image:: https://img.shields.io/pypi/l/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
+.. image:: https://img.shields.io/pypi/dm/pynamodb-mate.svg
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
       :target: https://pynamodb_mate.readthedocs.io/
```

### Comparing `pynamodb_mate-5.3.4.8/README.rst` & `pynamodb_mate-5.3.4.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 .. image:: https://img.shields.io/pypi/l/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
+.. image:: https://img.shields.io/pypi/dm/pynamodb-mate.svg
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
       :target: https://pynamodb_mate.readthedocs.io/
```

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/__init__.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/__init__.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/attributes/compressed.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/compressed.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/attributes/encrypted.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/encrypted.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/attributes/s3backed.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/s3backed.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/cipher.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/cipher.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/helpers.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/helpers.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/models.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/models.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/abstract.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/abstract.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/backend/dynamodb.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/dynamodb.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/backend/in_memory.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/in_memory.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/cache/multi_layer.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/multi_layer.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/patterns/status_tracker/impl.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/status_tracker/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
     ) -> "BaseStatusTracker":
         """
         A factory method to create new instance of a tracker.
         """
         JOB_ID = cls.JOB_ID if job_id is None else job_id
         kwargs = dict(
             key=cls.make_key(task_id, JOB_ID),
-            value=cls.make_value(status),
+            value=cls.make_value(status, JOB_ID),
         )
         if data is not None:
             kwargs["data"] = data
         return cls(**kwargs)
 
     @classmethod
     def new(
@@ -504,15 +504,15 @@
     def set_status(self, status: int) -> "BaseStatusTracker":
         """
         Set the status of the task. Don't do this directly::
 
             self.value = self.make_value(self.job_id, ...)
         """
         _update_context[self.key]["value"] = {"old": self.value}
-        self.value = self.make_value(status)
+        self.value = self.make_value(status, self.job_id)
         _update_context[self.key]["value"]["new"] = self.value
         _update_context[self.key]["value"]["act"] = BaseStatusTracker.value.set(
             self.value
         )
         return self
 
     def set_update_time(
```

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/tests/base.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/tests/base.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate/tests/helper.py` & `pynamodb_mate-5.3.4.9/pynamodb_mate/tests/helper.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate.egg-info/PKG-INFO` & `pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pynamodb-mate
-Version: 5.3.4.8
+Version: 5.3.4.9
 Summary: Provide Additional Features for pynamodb.
 Home-page: https://github.com/MacHu-GWU/pynamodb_mate-project
-Download-URL: https://pypi.python.org/pypi/pynamodb_mate/5.3.4.8#downloads
+Download-URL: https://pypi.python.org/pypi/pynamodb_mate/5.3.4.9#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -47,14 +47,16 @@
 
 .. image:: https://img.shields.io/pypi/l/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
+.. image:: https://img.shields.io/pypi/dm/pynamodb-mate.svg
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
       :target: https://pynamodb_mate.readthedocs.io/
```

### Comparing `pynamodb_mate-5.3.4.8/pynamodb_mate.egg-info/SOURCES.txt` & `pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/release-history.rst` & `pynamodb_mate-5.3.4.9/release-history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+5.3.4.9 (2023-05-15)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a but that some usages of :meth:`~pynamodb_mate.patterns.status_tracker.impl.BaseStatusTracker.make_value` are missing the parameter job_id.
+
+
 5.3.4.8 (2023-02-03)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - :class:`~pynamodb_mate.patterns.status_tracker.impl.BaseStatusTracker` added ``create_time`` attribute.
 - :class:`~pynamodb_mate.patterns.status_tracker.impl.StatusAndCreateTimeIndex` is renamed to :class:`~pynamodb_mate.patterns.status_tracker.impl.StatusAndUpdateTimeIndex`, and the index now uses ``update_time`` as the range key, and it now uses IncludeProjection.
 - :meth:`pynamodb_mate.patterns.status_tracker.impl.BaseStatusTracker.query_by_status` add ``auto_refresh`` parameter.
```

### Comparing `pynamodb_mate-5.3.4.8/requirements-doc.txt` & `pynamodb_mate-5.3.4.9/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.8/setup.py` & `pynamodb_mate-5.3.4.9/setup.py`

 * *Files identical despite different names*

