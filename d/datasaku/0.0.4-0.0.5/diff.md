# Comparing `tmp/datasaku-0.0.4.tar.gz` & `tmp/datasaku-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasaku-0.0.4.tar", last modified: Wed Apr 12 19:38:51 2023, max compression
+gzip compressed data, was "datasaku-0.0.5.tar", last modified: Mon May 15 20:32:48 2023, max compression
```

## Comparing `datasaku-0.0.4.tar` & `datasaku-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-12 19:38:51.026108 datasaku-0.0.4/
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1073 2023-01-10 15:17:32.000000 datasaku-0.0.4/LICENSE
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)       21 2023-01-11 16:48:37.000000 datasaku-0.0.4/MANIFEST.in
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2779 2023-04-12 19:38:51.025715 datasaku-0.0.4/PKG-INFO
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1054 2023-04-12 19:19:55.000000 datasaku-0.0.4/README.md
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      910 2023-04-12 19:38:39.000000 datasaku-0.0.4/pyproject.toml
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)      330 2023-01-11 15:30:04.000000 datasaku-0.0.4/requirements.txt
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)       38 2023-04-12 19:38:51.026200 datasaku-0.0.4/setup.cfg
-drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-12 19:38:51.011350 datasaku-0.0.4/src/
-drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-12 19:38:51.020273 datasaku-0.0.4/src/datasaku/
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/__init__.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      504 2023-01-11 12:03:25.000000 datasaku-0.0.4/src/datasaku/datasaku_calendar.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     5285 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/datasaku_geo.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     6849 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/datasaku_google.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1178 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/datasaku_nlp.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1931 2023-01-11 16:56:32.000000 datasaku-0.0.4/src/datasaku/datasaku_pandas.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     6170 2023-01-11 12:10:15.000000 datasaku-0.0.4/src/datasaku/datasaku_presto.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     4854 2023-04-12 19:34:36.000000 datasaku-0.0.4/src/datasaku/datasaku_s3.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     2798 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/datasaku_snowflake.py
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     1519 2023-01-11 15:43:56.000000 datasaku-0.0.4/src/datasaku/datasaku_starburst.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1748 2023-01-10 15:17:35.000000 datasaku-0.0.4/src/datasaku/datasaku_viz.py
-drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-12 19:38:51.024944 datasaku-0.0.4/src/datasaku.egg-info/
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2779 2023-04-12 19:38:50.000000 datasaku-0.0.4/src/datasaku.egg-info/PKG-INFO
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)      580 2023-04-12 19:38:51.000000 datasaku-0.0.4/src/datasaku.egg-info/SOURCES.txt
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)        1 2023-04-12 19:38:50.000000 datasaku-0.0.4/src/datasaku.egg-info/dependency_links.txt
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      330 2023-04-12 19:38:50.000000 datasaku-0.0.4/src/datasaku.egg-info/requires.txt
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)        9 2023-04-12 19:38:50.000000 datasaku-0.0.4/src/datasaku.egg-info/top_level.txt
+drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-05-15 20:32:48.683588 datasaku-0.0.5/
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1073 2023-01-10 15:17:32.000000 datasaku-0.0.5/LICENSE
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)       21 2023-01-11 16:48:37.000000 datasaku-0.0.5/MANIFEST.in
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2779 2023-05-15 20:32:48.683117 datasaku-0.0.5/PKG-INFO
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1054 2023-04-12 19:19:55.000000 datasaku-0.0.5/README.md
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      910 2023-05-15 20:31:45.000000 datasaku-0.0.5/pyproject.toml
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)      360 2023-05-15 20:30:47.000000 datasaku-0.0.5/requirements.txt
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)       38 2023-05-15 20:32:48.683651 datasaku-0.0.5/setup.cfg
+drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-05-15 20:32:48.660871 datasaku-0.0.5/src/
+drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-05-15 20:32:48.679343 datasaku-0.0.5/src/datasaku/
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-01-10 15:17:34.000000 datasaku-0.0.5/src/datasaku/__init__.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      504 2023-01-11 12:03:25.000000 datasaku-0.0.5/src/datasaku/datasaku_calendar.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     5285 2023-01-10 15:17:34.000000 datasaku-0.0.5/src/datasaku/datasaku_geo.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     6849 2023-01-10 15:17:34.000000 datasaku-0.0.5/src/datasaku/datasaku_google.py
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2319 2023-05-15 20:26:43.000000 datasaku-0.0.5/src/datasaku/datasaku_minio.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1178 2023-01-10 15:17:34.000000 datasaku-0.0.5/src/datasaku/datasaku_nlp.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1931 2023-01-11 16:56:32.000000 datasaku-0.0.5/src/datasaku/datasaku_pandas.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     6170 2023-01-11 12:10:15.000000 datasaku-0.0.5/src/datasaku/datasaku_presto.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     4854 2023-04-12 19:34:36.000000 datasaku-0.0.5/src/datasaku/datasaku_s3.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     2798 2023-01-10 15:17:34.000000 datasaku-0.0.5/src/datasaku/datasaku_snowflake.py
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     1519 2023-01-11 15:43:56.000000 datasaku-0.0.5/src/datasaku/datasaku_starburst.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1748 2023-01-10 15:17:35.000000 datasaku-0.0.5/src/datasaku/datasaku_viz.py
+drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-05-15 20:32:48.682477 datasaku-0.0.5/src/datasaku.egg-info/
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2779 2023-05-15 20:32:48.000000 datasaku-0.0.5/src/datasaku.egg-info/PKG-INFO
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)      611 2023-05-15 20:32:48.000000 datasaku-0.0.5/src/datasaku.egg-info/SOURCES.txt
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)        1 2023-05-15 20:32:48.000000 datasaku-0.0.5/src/datasaku.egg-info/dependency_links.txt
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      360 2023-05-15 20:32:48.000000 datasaku-0.0.5/src/datasaku.egg-info/requires.txt
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)        9 2023-05-15 20:32:48.000000 datasaku-0.0.5/src/datasaku.egg-info/top_level.txt
```

### Comparing `datasaku-0.0.4/LICENSE` & `datasaku-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/PKG-INFO` & `datasaku-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasaku
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Author-email: kurangdoa <rando.bayor@gmail.com>
 License: Copyright (c) 2022 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `datasaku-0.0.4/README.md` & `datasaku-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/pyproject.toml` & `datasaku-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datasaku"
 dynamic = ["dependencies"]
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="kurangdoa", email="rando.bayor@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_geo.py` & `datasaku-0.0.5/src/datasaku/datasaku_geo.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_google.py` & `datasaku-0.0.5/src/datasaku/datasaku_google.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_nlp.py` & `datasaku-0.0.5/src/datasaku/datasaku_nlp.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_pandas.py` & `datasaku-0.0.5/src/datasaku/datasaku_pandas.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_presto.py` & `datasaku-0.0.5/src/datasaku/datasaku_presto.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_s3.py` & `datasaku-0.0.5/src/datasaku/datasaku_s3.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_snowflake.py` & `datasaku-0.0.5/src/datasaku/datasaku_snowflake.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_starburst.py` & `datasaku-0.0.5/src/datasaku/datasaku_starburst.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku/datasaku_viz.py` & `datasaku-0.0.5/src/datasaku/datasaku_viz.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.4/src/datasaku.egg-info/PKG-INFO` & `datasaku-0.0.5/src/datasaku.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasaku
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Author-email: kurangdoa <rando.bayor@gmail.com>
 License: Copyright (c) 2022 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `datasaku-0.0.4/src/datasaku.egg-info/SOURCES.txt` & `datasaku-0.0.5/src/datasaku.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 requirements.txt
 src/datasaku/__init__.py
 src/datasaku/datasaku_calendar.py
 src/datasaku/datasaku_geo.py
 src/datasaku/datasaku_google.py
+src/datasaku/datasaku_minio.py
 src/datasaku/datasaku_nlp.py
 src/datasaku/datasaku_pandas.py
 src/datasaku/datasaku_presto.py
 src/datasaku/datasaku_s3.py
 src/datasaku/datasaku_snowflake.py
 src/datasaku/datasaku_starburst.py
 src/datasaku/datasaku_viz.py
```

