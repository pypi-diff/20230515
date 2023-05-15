# Comparing `tmp/clickzetta-sqlalchemy-0.6.3.tar.gz` & `tmp/clickzetta-sqlalchemy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-sqlalchemy-0.6.3.tar", last modified: Thu Apr  6 11:33:33 2023, max compression
+gzip compressed data, was "clickzetta-sqlalchemy-0.6.4.tar", last modified: Mon May 15 07:30:03 2023, max compression
```

## Comparing `clickzetta-sqlalchemy-0.6.3.tar` & `clickzetta-sqlalchemy-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-04-06 11:33:33.642754 clickzetta-sqlalchemy-0.6.3/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      423 2023-04-06 11:33:33.642624 clickzetta-sqlalchemy-0.6.3/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-04-06 11:33:33.640562 clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      423 2023-04-06 11:33:33.000000 clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)      560 2023-04-06 11:33:33.000000 clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-04-06 11:33:33.000000 clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-04-06 11:33:33.000000 clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-04-06 11:33:33.000000 clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      642 2023-04-06 11:33:33.000000 clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       22 2023-04-06 11:33:33.000000 clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-04-06 11:33:33.642800 clickzetta-sqlalchemy-0.6.3/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1877 2023-04-06 11:33:13.000000 clickzetta-sqlalchemy-0.6.3/setup.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-04-06 11:33:33.642409 clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      499 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1079 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1626 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/_types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20343 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/base.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1146 2023-02-24 06:29:49.000000 clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/parse_url.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2742 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/requirements.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-04-06 11:33:13.000000 clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-15 07:30:03.934908 clickzetta-sqlalchemy-0.6.4/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      423 2023-05-15 07:30:03.934746 clickzetta-sqlalchemy-0.6.4/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-15 07:30:03.932909 clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      423 2023-05-15 07:30:03.000000 clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      560 2023-05-15 07:30:03.000000 clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-15 07:30:03.000000 clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-15 07:30:03.000000 clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-15 07:30:03.000000 clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      633 2023-05-15 07:30:03.000000 clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       22 2023-05-15 07:30:03.000000 clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-15 07:30:03.934959 clickzetta-sqlalchemy-0.6.4/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1868 2023-05-10 03:55:44.000000 clickzetta-sqlalchemy-0.6.4/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-15 07:30:03.934549 clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      499 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1079 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1626 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/_types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20343 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/base.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1146 2023-02-24 06:29:49.000000 clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/parse_url.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2742 2023-02-24 03:50:44.000000 clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/requirements.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-10 03:55:44.000000 clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/version.py
```

### Comparing `clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/SOURCES.txt` & `clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.6.3/clickzetta_sqlalchemy.egg-info/requires.txt` & `clickzetta-sqlalchemy-0.6.4/clickzetta_sqlalchemy.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 proto-plus<2.0.0dev,>=1.22.0
 packaging<24.0.0dev,>=14.3
 protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 python-dateutil<3.0dev,>=2.7.2
 requests<3.0.0dev,>=2.21.0
-sqlalchemy<=1.4.27,>=1.2.0
+sqlalchemy==2.0.6
 future
-clickzetta-connector==0.6.3
+clickzetta-connector==0.6.4
 
 [all]
 pandas>=1.0.0
 db-dtypes<2.0.0dev,>=0.3.0
 ipywidgets==7.7.1
 geopandas<1.0dev,>=0.9.0
 Shapely<2.0dev,>=1.6.0
```

### Comparing `clickzetta-sqlalchemy-0.6.3/setup.py` & `clickzetta-sqlalchemy-0.6.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 release_status = "Development Status :: 3 - Alpha"
 dependencies = [
     "proto-plus >= 1.22.0, <2.0.0dev",
     "packaging >= 14.3, <24.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "python-dateutil >= 2.7.2, <3.0dev",
     "requests >= 2.21.0, < 3.0.0dev",
-    "sqlalchemy>=1.2.0,<=1.4.27",
+    "sqlalchemy==2.0.6",
     "future",
-    'clickzetta-connector==0.6.3',
+    'clickzetta-connector==0.6.4',
 ]
 extras = {
     "pandas": ["pandas>=1.0.0", "db-dtypes>=0.3.0,<2.0.0dev"],
     "ipywidgets": ["ipywidgets==7.7.1"],
     "geopandas": ["geopandas>=0.9.0, <1.0dev", "Shapely>=1.6.0, <2.0dev"],
     "ipython": ["ipython>=7.0.1,!=8.1.0"],
     "tqdm": ["tqdm >= 4.7.4, <5.0.0dev"],
```

### Comparing `clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/_helpers.py` & `clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/_types.py` & `clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/_types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/base.py` & `clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/parse_url.py` & `clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/parse_url.py`

 * *Files identical despite different names*

### Comparing `clickzetta-sqlalchemy-0.6.3/sqlalchemy_clickzetta/requirements.py` & `clickzetta-sqlalchemy-0.6.4/sqlalchemy_clickzetta/requirements.py`

 * *Files identical despite different names*
