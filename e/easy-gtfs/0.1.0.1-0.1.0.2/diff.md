# Comparing `tmp/easy_gtfs-0.1.0.1.tar.gz` & `tmp/easy_gtfs-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gtfs-0.1.0.1.tar", max compression
+gzip compressed data, was "easy_gtfs-0.1.0.2.tar", max compression
```

## Comparing `easy_gtfs-0.1.0.1.tar` & `easy_gtfs-0.1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       24 2023-05-15 16:23:22.412176 easy_gtfs-0.1.0.1/easy_gtfs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 16:24:21.223177 easy_gtfs-0.1.0.1/easy_gtfs/managers/__init__.py
--rw-r--r--   0        0        0     7000 2023-05-15 16:21:53.793005 easy_gtfs-0.1.0.1/easy_gtfs/managers/agencymanager.py
--rw-r--r--   0        0        0      730 2023-05-15 16:16:25.863078 easy_gtfs-0.1.0.1/easy_gtfs/managers/errormanager.py
--rw-r--r--   0        0        0        0 2023-05-15 16:24:14.442747 easy_gtfs-0.1.0.1/easy_gtfs/models/__init__.py
--rw-r--r--   0        0        0      369 2023-05-15 16:20:49.948447 easy_gtfs-0.1.0.1/easy_gtfs/models/errors.py
--rw-r--r--   0        0        0        0 2023-05-15 14:09:30.614598 easy_gtfs-0.1.0.1/easy_gtfs/objects/__init__.py
--rw-r--r--   0        0        0     2614 2023-05-15 16:12:40.836501 easy_gtfs-0.1.0.1/easy_gtfs/objects/agency.py
--rw-r--r--   0        0        0     1269 2023-05-15 16:12:05.818115 easy_gtfs-0.1.0.1/easy_gtfs/utility.py
--rw-r--r--   0        0        0     1389 2023-05-15 15:26:25.897851 easy_gtfs-0.1.0.1/easy_gtfs/variables.py
--rw-r--r--   0        0        0      343 2023-05-15 16:27:43.921227 easy_gtfs-0.1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 14:06:25.799294 easy_gtfs-0.1.0.1/README.md
--rw-r--r--   0        0        0      411 1970-01-01 00:00:00.000000 easy_gtfs-0.1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-15 16:28:56.423189 easy_gtfs-0.1.0.2/easy_gtfs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:24:21.223177 easy_gtfs-0.1.0.2/easy_gtfs/managers/__init__.py
+-rw-r--r--   0        0        0     7000 2023-05-15 16:21:53.793005 easy_gtfs-0.1.0.2/easy_gtfs/managers/agencymanager.py
+-rw-r--r--   0        0        0      730 2023-05-15 16:16:25.863078 easy_gtfs-0.1.0.2/easy_gtfs/managers/errormanager.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:24:14.442747 easy_gtfs-0.1.0.2/easy_gtfs/models/__init__.py
+-rw-r--r--   0        0        0      369 2023-05-15 16:20:49.948447 easy_gtfs-0.1.0.2/easy_gtfs/models/errors.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:09:30.614598 easy_gtfs-0.1.0.2/easy_gtfs/objects/__init__.py
+-rw-r--r--   0        0        0     2614 2023-05-15 16:12:40.836501 easy_gtfs-0.1.0.2/easy_gtfs/objects/agency.py
+-rw-r--r--   0        0        0     1269 2023-05-15 16:12:05.818115 easy_gtfs-0.1.0.2/easy_gtfs/utility.py
+-rw-r--r--   0        0        0     1389 2023-05-15 15:26:25.897851 easy_gtfs-0.1.0.2/easy_gtfs/variables.py
+-rw-r--r--   0        0        0      343 2023-05-15 16:28:33.751198 easy_gtfs-0.1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 14:06:25.799294 easy_gtfs-0.1.0.2/README.md
+-rw-r--r--   0        0        0      411 1970-01-01 00:00:00.000000 easy_gtfs-0.1.0.2/PKG-INFO
```

### Comparing `easy_gtfs-0.1.0.1/easy_gtfs/managers/agencymanager.py` & `easy_gtfs-0.1.0.2/easy_gtfs/managers/agencymanager.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.1/easy_gtfs/managers/errormanager.py` & `easy_gtfs-0.1.0.2/easy_gtfs/managers/errormanager.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.1/easy_gtfs/objects/agency.py` & `easy_gtfs-0.1.0.2/easy_gtfs/objects/agency.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.1/easy_gtfs/utility.py` & `easy_gtfs-0.1.0.2/easy_gtfs/utility.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.1/easy_gtfs/variables.py` & `easy_gtfs-0.1.0.2/easy_gtfs/variables.py`

 * *Files identical despite different names*

