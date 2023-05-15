# Comparing `tmp/platform-library-0.0.6.tar.gz` & `tmp/platform-library-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-library-0.0.6.tar", last modified: Thu May 11 06:40:19 2023, max compression
+gzip compressed data, was "platform-library-0.0.7.tar", last modified: Mon May 15 12:18:35 2023, max compression
```

## Comparing `platform-library-0.0.6.tar` & `platform-library-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.675411 platform-library-0.0.6/
--rw-r--r--   0 Artyom     (501) staff       (20)     1078 2022-11-08 13:08:16.000000 platform-library-0.0.6/LICENSE
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-11 06:40:19.675289 platform-library-0.0.6/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.0.6/README-public.md
--rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.0.6/README.md
--rw-r--r--   0 Artyom     (501) staff       (20)      552 2023-05-11 06:38:46.000000 platform-library-0.0.6/pyproject.toml
--rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-05-11 06:40:19.675449 platform-library-0.0.6/setup.cfg
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.673208 platform-library-0.0.6/src/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.674349 platform-library-0.0.6/src/platform_library.egg-info/
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)      454 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/SOURCES.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/dependency_links.txt
--rw-r--r--   0 Artyom     (501) staff       (20)       15 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/requires.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-05-11 06:40:19.000000 platform-library-0.0.6/src/platform_library.egg-info/top_level.txt
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.673323 platform-library-0.0.6/src/plib/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.674767 platform-library-0.0.6/src/plib/auth/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.0.6/src/plib/auth/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.0.6/src/plib/auth/encrypt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.0.6/src/plib/auth/jwt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.0.6/src/plib/auth/o2auth.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-11 06:40:19.675145 platform-library-0.0.6/src/plib/licensing/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.0.6/src/plib/licensing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     4037 2023-05-11 06:38:08.000000 platform-library-0.0.6/src/plib/licensing/api.py
--rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.0.6/src/plib/licensing/exceptions.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.677415 platform-library-0.0.7/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1078 2022-11-08 13:08:16.000000 platform-library-0.0.7/LICENSE
+-rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-15 12:18:35.677298 platform-library-0.0.7/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.0.7/README-public.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.0.7/README.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      593 2023-05-15 12:18:09.000000 platform-library-0.0.7/pyproject.toml
+-rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-05-15 12:18:35.677452 platform-library-0.0.7/setup.cfg
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.674019 platform-library-0.0.7/src/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.675549 platform-library-0.0.7/src/platform_library.egg-info/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)      509 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/SOURCES.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/dependency_links.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)       51 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/requires.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/top_level.txt
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.674213 platform-library-0.0.7/src/plib/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.676369 platform-library-0.0.7/src/plib/auth/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.0.7/src/plib/auth/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.0.7/src/plib/auth/encrypt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.0.7/src/plib/auth/jwt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.0.7/src/plib/auth/o2auth.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.676767 platform-library-0.0.7/src/plib/licensing/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.0.7/src/plib/licensing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     4037 2023-05-11 06:38:08.000000 platform-library-0.0.7/src/plib/licensing/api.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.0.7/src/plib/licensing/exceptions.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.677137 platform-library-0.0.7/src/plib/tracing/
+-rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.0.7/src/plib/tracing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     3019 2023-05-15 12:18:09.000000 platform-library-0.0.7/src/plib/tracing/utils.py
```

### Comparing `platform-library-0.0.6/LICENSE` & `platform-library-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.6/PKG-INFO` & `platform-library-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for easy developing 3DiVi Platform
 Author-email: Artyom Vakilov <a.vakilov@3divi.com>
 License: MIT License
         
         Copyright (c) 2022 3DiVi Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.0.6/README.md` & `platform-library-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.6/pyproject.toml` & `platform-library-0.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "platform-library"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Artyom Vakilov", email="a.vakilov@3divi.com" },
 ]
 
 description = "A library for easy developing 3DiVi Platform"
 readme = "README-public.md"
 license = { file="LICENSE" }
@@ -16,9 +16,9 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "PyJWT", "requests"
+    "PyJWT", "requests", "opentelemetry-exporter-otlp == 1.17.0"
 ]
```

### Comparing `platform-library-0.0.6/src/platform_library.egg-info/PKG-INFO` & `platform-library-0.0.7/src/platform_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for easy developing 3DiVi Platform
 Author-email: Artyom Vakilov <a.vakilov@3divi.com>
 License: MIT License
         
         Copyright (c) 2022 3DiVi Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.0.6/src/plib/auth/encrypt.py` & `platform-library-0.0.7/src/plib/auth/encrypt.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.6/src/plib/auth/o2auth.py` & `platform-library-0.0.7/src/plib/auth/o2auth.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.6/src/plib/licensing/api.py` & `platform-library-0.0.7/src/plib/licensing/api.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.6/src/plib/licensing/exceptions.py` & `platform-library-0.0.7/src/plib/licensing/exceptions.py`

 * *Files identical despite different names*

