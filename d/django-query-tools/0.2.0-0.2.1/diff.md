# Comparing `tmp/django_query_tools-0.2.0.tar.gz` & `tmp/django_query_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_query_tools-0.2.0.tar", last modified: Mon May 15 11:39:56 2023, max compression
+gzip compressed data, was "django_query_tools-0.2.1.tar", last modified: Mon May 15 11:45:38 2023, max compression
```

## Comparing `django_query_tools-0.2.0.tar` & `django_query_tools-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 brierto-admin   (503) staff       (20)        0 2023-05-15 11:39:56.882242 django_query_tools-0.2.0/
--rw-r--r--   0 brierto-admin   (503) staff       (20)     1069 2023-05-15 11:33:02.000000 django_query_tools-0.2.0/LICENSE
--rw-r--r--   0 brierto-admin   (503) staff       (20)      105 2023-05-15 11:39:56.882307 django_query_tools-0.2.0/PKG-INFO
--rw-r--r--   0 brierto-admin   (503) staff       (20)     1844 2023-05-11 09:38:02.000000 django_query_tools-0.2.0/README.md
-drwxr-xr-x   0 brierto-admin   (503) staff       (20)        0 2023-05-15 11:39:56.881612 django_query_tools-0.2.0/django_query_tools/
--rw-r--r--   0 brierto-admin   (503) staff       (20)        0 2023-05-10 16:12:20.000000 django_query_tools-0.2.0/django_query_tools/__init__.py
--rw-r--r--   0 brierto-admin   (503) staff       (20)     2823 2023-05-10 15:30:48.000000 django_query_tools-0.2.0/django_query_tools/client.py
--rw-r--r--   0 brierto-admin   (503) staff       (20)     4560 2023-05-15 11:29:00.000000 django_query_tools-0.2.0/django_query_tools/server.py
--rw-r--r--   0 brierto-admin   (503) staff       (20)       22 2023-05-15 11:39:25.000000 django_query_tools-0.2.0/django_query_tools/version.py
-drwxr-xr-x   0 brierto-admin   (503) staff       (20)        0 2023-05-15 11:39:56.882123 django_query_tools-0.2.0/django_query_tools.egg-info/
--rw-r--r--   0 brierto-admin   (503) staff       (20)      105 2023-05-15 11:39:56.000000 django_query_tools-0.2.0/django_query_tools.egg-info/PKG-INFO
--rw-r--r--   0 brierto-admin   (503) staff       (20)      323 2023-05-15 11:39:56.000000 django_query_tools-0.2.0/django_query_tools.egg-info/SOURCES.txt
--rw-r--r--   0 brierto-admin   (503) staff       (20)        1 2023-05-15 11:39:56.000000 django_query_tools-0.2.0/django_query_tools.egg-info/dependency_links.txt
--rw-r--r--   0 brierto-admin   (503) staff       (20)       19 2023-05-15 11:39:56.000000 django_query_tools-0.2.0/django_query_tools.egg-info/top_level.txt
--rw-r--r--   0 brierto-admin   (503) staff       (20)      103 2023-05-15 11:39:56.882553 django_query_tools-0.2.0/setup.cfg
--rw-r--r--   0 brierto-admin   (503) staff       (20)      230 2023-05-10 15:59:21.000000 django_query_tools-0.2.0/setup.py
+drwxr-xr-x   0 brierto-admin   (503) staff       (20)        0 2023-05-15 11:45:38.082374 django_query_tools-0.2.1/
+-rw-r--r--   0 brierto-admin   (503) staff       (20)     1069 2023-05-15 11:33:02.000000 django_query_tools-0.2.1/LICENSE
+-rw-r--r--   0 brierto-admin   (503) staff       (20)      105 2023-05-15 11:45:38.082446 django_query_tools-0.2.1/PKG-INFO
+-rw-r--r--   0 brierto-admin   (503) staff       (20)     1844 2023-05-11 09:38:02.000000 django_query_tools-0.2.1/README.md
+drwxr-xr-x   0 brierto-admin   (503) staff       (20)        0 2023-05-15 11:45:38.081678 django_query_tools-0.2.1/django_query_tools/
+-rw-r--r--   0 brierto-admin   (503) staff       (20)        0 2023-05-10 16:12:20.000000 django_query_tools-0.2.1/django_query_tools/__init__.py
+-rw-r--r--   0 brierto-admin   (503) staff       (20)     2823 2023-05-10 15:30:48.000000 django_query_tools-0.2.1/django_query_tools/client.py
+-rw-r--r--   0 brierto-admin   (503) staff       (20)     4560 2023-05-15 11:29:00.000000 django_query_tools-0.2.1/django_query_tools/server.py
+-rw-r--r--   0 brierto-admin   (503) staff       (20)       22 2023-05-15 11:44:03.000000 django_query_tools-0.2.1/django_query_tools/version.py
+drwxr-xr-x   0 brierto-admin   (503) staff       (20)        0 2023-05-15 11:45:38.082226 django_query_tools-0.2.1/django_query_tools.egg-info/
+-rw-r--r--   0 brierto-admin   (503) staff       (20)      105 2023-05-15 11:45:38.000000 django_query_tools-0.2.1/django_query_tools.egg-info/PKG-INFO
+-rw-r--r--   0 brierto-admin   (503) staff       (20)      323 2023-05-15 11:45:38.000000 django_query_tools-0.2.1/django_query_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 brierto-admin   (503) staff       (20)        1 2023-05-15 11:45:38.000000 django_query_tools-0.2.1/django_query_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 brierto-admin   (503) staff       (20)       19 2023-05-15 11:45:38.000000 django_query_tools-0.2.1/django_query_tools.egg-info/top_level.txt
+-rw-r--r--   0 brierto-admin   (503) staff       (20)      103 2023-05-15 11:45:38.082695 django_query_tools-0.2.1/setup.cfg
+-rw-r--r--   0 brierto-admin   (503) staff       (20)      230 2023-05-10 15:59:21.000000 django_query_tools-0.2.1/setup.py
```

### Comparing `django_query_tools-0.2.0/LICENSE` & `django_query_tools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_query_tools-0.2.0/README.md` & `django_query_tools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_query_tools-0.2.0/django_query_tools/client.py` & `django_query_tools-0.2.1/django_query_tools/client.py`

 * *Files identical despite different names*

### Comparing `django_query_tools-0.2.0/django_query_tools/server.py` & `django_query_tools-0.2.1/django_query_tools/server.py`

 * *Files identical despite different names*

