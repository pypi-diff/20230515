# Comparing `tmp/dabbas-0.1.6.tar.gz` & `tmp/dabbas-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dabbas-0.1.6.tar", last modified: Fri May  5 11:00:21 2023, max compression
+gzip compressed data, was "dabbas-0.1.8.tar", last modified: Mon May 15 11:30:57 2023, max compression
```

## Comparing `dabbas-0.1.6.tar` & `dabbas-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-05 11:00:21.625780 dabbas-0.1.6/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-05 11:00:21.625599 dabbas-0.1.6/PKG-INFO
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-05 11:00:21.623264 dabbas-0.1.6/atlas/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       21 2023-04-23 17:17:29.000000 dabbas-0.1.6/atlas/__init__.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     6280 2023-04-24 17:54:58.000000 dabbas-0.1.6/atlas/atlas.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     8113 2023-04-24 09:22:52.000000 dabbas-0.1.6/atlas/boundary.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1385 2023-04-23 19:44:53.000000 dabbas-0.1.6/atlas/db.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2793 2023-04-23 19:43:28.000000 dabbas-0.1.6/atlas/schema.py
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-05 11:00:21.624089 dabbas-0.1.6/dabbas/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      134 2023-04-19 15:30:00.000000 dabbas-0.1.6/dabbas/__init__.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2399 2023-04-19 03:44:35.000000 dabbas-0.1.6/dabbas/cache.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1174 2023-05-05 10:59:29.000000 dabbas-0.1.6/dabbas/connection.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2748 2023-04-19 15:29:41.000000 dabbas-0.1.6/dabbas/main.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     5366 2023-04-23 18:14:37.000000 dabbas-0.1.6/dabbas/map.py
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-05 11:00:21.625268 dabbas-0.1.6/dabbas.egg-info/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-05 11:00:21.000000 dabbas-0.1.6/dabbas.egg-info/PKG-INFO
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      354 2023-05-05 11:00:21.000000 dabbas-0.1.6/dabbas.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)        1 2023-05-05 11:00:21.000000 dabbas-0.1.6/dabbas.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       58 2023-05-05 11:00:21.000000 dabbas-0.1.6/dabbas.egg-info/entry_points.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      101 2023-05-05 11:00:21.000000 dabbas-0.1.6/dabbas.egg-info/requires.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       13 2023-05-05 11:00:21.000000 dabbas-0.1.6/dabbas.egg-info/top_level.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       38 2023-05-05 11:00:21.625844 dabbas-0.1.6/setup.cfg
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      895 2023-05-05 11:00:16.000000 dabbas-0.1.6/setup.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:30:57.773878 dabbas-0.1.8/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-15 11:30:57.773591 dabbas-0.1.8/PKG-INFO
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:30:57.770791 dabbas-0.1.8/atlas/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       21 2023-04-23 17:17:29.000000 dabbas-0.1.8/atlas/__init__.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     6280 2023-04-24 17:54:58.000000 dabbas-0.1.8/atlas/atlas.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     8113 2023-04-24 09:22:52.000000 dabbas-0.1.8/atlas/boundary.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1479 2023-05-15 11:11:09.000000 dabbas-0.1.8/atlas/db.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2793 2023-04-23 19:43:28.000000 dabbas-0.1.8/atlas/schema.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:30:57.772006 dabbas-0.1.8/dabbas/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      134 2023-04-19 15:30:00.000000 dabbas-0.1.8/dabbas/__init__.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2399 2023-04-19 03:44:35.000000 dabbas-0.1.8/dabbas/cache.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1294 2023-05-15 11:00:11.000000 dabbas-0.1.8/dabbas/connection.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2748 2023-04-19 15:29:41.000000 dabbas-0.1.8/dabbas/main.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     5376 2023-05-15 11:10:48.000000 dabbas-0.1.8/dabbas/map.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:30:57.773322 dabbas-0.1.8/dabbas.egg-info/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      354 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)        1 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       58 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/entry_points.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      101 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/requires.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       13 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/top_level.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       38 2023-05-15 11:30:57.773927 dabbas-0.1.8/setup.cfg
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      895 2023-05-15 11:30:57.000000 dabbas-0.1.8/setup.py
```

### Comparing `dabbas-0.1.6/atlas/atlas.py` & `dabbas-0.1.8/atlas/atlas.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.6/atlas/boundary.py` & `dabbas-0.1.8/atlas/boundary.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.6/atlas/db.py` & `dabbas-0.1.8/atlas/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import psycopg2
 import os
 
 DB_ANON_KEY = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyAgCiAgICAicm9sZSI6ICJhbm9uIiwKICAgICJpc3MiOiAic3VwYWJhc2UtZGVtbyIsCiAgICAiaWF0IjogMTY0MTc2OTIwMCwKICAgICJleHAiOiAxNzk5NTM1NjAwCn0.dc_X5iR_VP_qT0zsiyj_I_OZ2T9FtRU2BBNWN8Bu4GE'
 DB_ADMIN_KEY = "eeyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InRqbHNsYWR0dGJvbG93b29pc3JwIiwicm9sZSI6InNlcnZpY2Vfcm9sZSIsImlhdCI6MTY4MTEyMDQ5MSwiZXhwIjoxOTk2Njk2NDkxfQ.GzE799I13MX10Pbnn--h0_kSkX2md8JqCrTZyiAwniE"
 
 
-
 def sql(query):
     try:
-        conn = psycopg2.connect(database="postgres", user="postgres",
-                                password="Nikhilsaraf401", host="34.131.74.243", port="5432")
+        conn = psycopg2.connect(database="postgres", 
+                                user="reader",
+                                password='password',
+                                host="34.131.74.243", 
+                                port="5432")
         cursor = conn.cursor()
         cursor.execute(query)
         rows = cursor.fetchall()
         cursor.close()
         conn.close()
         return rows
     except Exception as e:
@@ -31,9 +33,10 @@
         conn.close()
 
 
 key = os.getenv('ATLAS_KEY')
 
 assert key is not None, "ATLAS_KEY is required"
 
-boundary_supabase = create_client('https://tjlsladttbolowooisrp.supabase.co', key)
+boundary_supabase = create_client(
+    'https://tjlsladttbolowooisrp.supabase.co', key)
 poi_supabase = create_client('https://tjlsladttbolowooisrp.supabase.co', key)
```

### Comparing `dabbas-0.1.6/atlas/schema.py` & `dabbas-0.1.8/atlas/schema.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.6/dabbas/cache.py` & `dabbas-0.1.8/dabbas/cache.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.6/dabbas/main.py` & `dabbas-0.1.8/dabbas/main.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.6/dabbas/map.py` & `dabbas-0.1.8/dabbas/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,17 @@
     df = df.copy()
     if len(df) == 0:
         raise Exception('No data in Dataset to create geometry')
 
     if type(geometry) == str and geometry in df:
         if format in format_map:
             df.loc[:, 'geometry'] = df.loc[:,
-                                           col].apply(format_map[format])
+                                           geometry].apply(format_map[format])
         else:
-            df.loc[:, 'geometry'] = df.loc[:, col]
+            df.loc[:, 'geometry'] = df.loc[:, geometry]
         return df
 
     for col in geometry:
         if col in df:
             if format in format_map:
                 df.loc[:, 'geometry'] = df.loc[:,
                                                col].apply(format_map[format])
```

### Comparing `dabbas-0.1.6/setup.py` & `dabbas-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dabbas",
-    version="0.1.6",
+    version="0.1.8",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "db = db.main:main",
             "dabbas = db.main:main",
         ],
     },
```

