# Comparing `tmp/barbell2_castor-0.6.0.tar.gz` & `tmp/barbell2_castor-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barbell2_castor-0.6.0.tar", last modified: Mon May 15 09:09:05 2023, max compression
+gzip compressed data, was "barbell2_castor-0.7.0.tar", last modified: Mon May 15 09:11:02 2023, max compression
```

## Comparing `barbell2_castor-0.6.0.tar` & `barbell2_castor-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:09:05.765784 barbell2_castor-0.6.0/
--rw-r--r--   0 Ralph      (501) staff       (20)      773 2023-05-15 09:09:05.765491 barbell2_castor-0.6.0/PKG-INFO
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:09:05.762720 barbell2_castor-0.6.0/barbell2_castor/
--rw-r--r--   0 Ralph      (501) staff       (20)      258 2023-05-15 09:09:00.000000 barbell2_castor-0.6.0/barbell2_castor/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     9836 2023-05-15 08:37:51.000000 barbell2_castor-0.6.0/barbell2_castor/api.py
--rw-r--r--   0 Ralph      (501) staff       (20)     6634 2023-05-15 08:37:51.000000 barbell2_castor-0.6.0/barbell2_castor/castor2sqlite.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1511 2023-05-15 08:39:48.000000 barbell2_castor-0.6.0/barbell2_castor/query.py
--rw-r--r--   0 Ralph      (501) staff       (20)      628 2023-05-15 08:37:51.000000 barbell2_castor-0.6.0/barbell2_castor/utils.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:09:05.765112 barbell2_castor-0.6.0/barbell2_castor.egg-info/
--rw-r--r--   0 Ralph      (501) staff       (20)      773 2023-05-15 09:09:05.000000 barbell2_castor-0.6.0/barbell2_castor.egg-info/PKG-INFO
--rw-r--r--   0 Ralph      (501) staff       (20)      416 2023-05-15 09:09:05.000000 barbell2_castor-0.6.0/barbell2_castor.egg-info/SOURCES.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-05-15 09:09:05.000000 barbell2_castor-0.6.0/barbell2_castor.egg-info/dependency_links.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       20 2023-05-15 09:09:05.000000 barbell2_castor-0.6.0/barbell2_castor.egg-info/entry_points.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-05-15 09:09:05.000000 barbell2_castor-0.6.0/barbell2_castor.egg-info/not-zip-safe
--rw-r--r--   0 Ralph      (501) staff       (20)       34 2023-05-15 09:09:05.000000 barbell2_castor-0.6.0/barbell2_castor.egg-info/requires.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       16 2023-05-15 09:09:05.000000 barbell2_castor-0.6.0/barbell2_castor.egg-info/top_level.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       38 2023-05-15 09:09:05.765885 barbell2_castor-0.6.0/setup.cfg
--rw-r--r--   0 Ralph      (501) staff       (20)     1372 2023-05-15 08:37:51.000000 barbell2_castor-0.6.0/setup.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:11:02.199912 barbell2_castor-0.7.0/
+-rw-r--r--   0 Ralph      (501) staff       (20)      773 2023-05-15 09:11:02.199652 barbell2_castor-0.7.0/PKG-INFO
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:11:02.196915 barbell2_castor-0.7.0/barbell2_castor/
+-rw-r--r--   0 Ralph      (501) staff       (20)      264 2023-05-15 09:10:56.000000 barbell2_castor-0.7.0/barbell2_castor/__init__.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     9836 2023-05-15 08:37:51.000000 barbell2_castor-0.7.0/barbell2_castor/api.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     6634 2023-05-15 08:37:51.000000 barbell2_castor-0.7.0/barbell2_castor/castor2sqlite.py
+-rw-r--r--   0 Ralph      (501) staff       (20)     1511 2023-05-15 08:39:48.000000 barbell2_castor-0.7.0/barbell2_castor/query.py
+-rw-r--r--   0 Ralph      (501) staff       (20)      628 2023-05-15 08:37:51.000000 barbell2_castor-0.7.0/barbell2_castor/utils.py
+drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2023-05-15 09:11:02.199112 barbell2_castor-0.7.0/barbell2_castor.egg-info/
+-rw-r--r--   0 Ralph      (501) staff       (20)      773 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/PKG-INFO
+-rw-r--r--   0 Ralph      (501) staff       (20)      416 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/SOURCES.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/dependency_links.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       20 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/entry_points.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)        1 2023-05-15 09:09:05.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/not-zip-safe
+-rw-r--r--   0 Ralph      (501) staff       (20)       34 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/requires.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       16 2023-05-15 09:11:02.000000 barbell2_castor-0.7.0/barbell2_castor.egg-info/top_level.txt
+-rw-r--r--   0 Ralph      (501) staff       (20)       38 2023-05-15 09:11:02.200005 barbell2_castor-0.7.0/setup.cfg
+-rw-r--r--   0 Ralph      (501) staff       (20)     1372 2023-05-15 08:37:51.000000 barbell2_castor-0.7.0/setup.py
```

### Comparing `barbell2_castor-0.6.0/PKG-INFO` & `barbell2_castor-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barbell2_castor
-Version: 0.6.0
+Version: 0.7.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Keywords: barbell2_castor
 Platform: UNKNOWN
```

### Comparing `barbell2_castor-0.6.0/barbell2_castor/api.py` & `barbell2_castor-0.7.0/barbell2_castor/api.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.6.0/barbell2_castor/castor2sqlite.py` & `barbell2_castor-0.7.0/barbell2_castor/castor2sqlite.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.6.0/barbell2_castor/query.py` & `barbell2_castor-0.7.0/barbell2_castor/query.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.6.0/barbell2_castor/utils.py` & `barbell2_castor-0.7.0/barbell2_castor/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_castor-0.6.0/barbell2_castor.egg-info/PKG-INFO` & `barbell2_castor-0.7.0/barbell2_castor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barbell2-castor
-Version: 0.6.0
+Version: 0.7.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Keywords: barbell2_castor
 Platform: UNKNOWN
```

### Comparing `barbell2_castor-0.6.0/setup.py` & `barbell2_castor-0.7.0/setup.py`

 * *Files identical despite different names*

