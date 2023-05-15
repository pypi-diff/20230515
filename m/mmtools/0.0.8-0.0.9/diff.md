# Comparing `tmp/mmtools-0.0.8.tar.gz` & `tmp/mmtools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmtools-0.0.8.tar", last modified: Mon May 25 06:19:56 2020, max compression
+gzip compressed data, was "dist/mmtools-0.0.9.tar", last modified: Thu Oct 22 06:39:59 2020, max compression
```

## Comparing `mmtools-0.0.8.tar` & `mmtools-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-05-25 06:19:56.000000 mmtools-0.0.8/
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-05-25 06:19:56.000000 mmtools-0.0.8/mmtools/
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     1619 2020-05-25 06:00:46.000000 mmtools-0.0.8/mmtools/config.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2020-05-25 06:00:46.000000 mmtools-0.0.8/mmtools/__init__.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     4257 2020-05-25 06:00:46.000000 mmtools-0.0.8/mmtools/watch.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2147 2020-05-25 06:00:46.000000 mmtools-0.0.8/mmtools/status.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     4489 2020-05-25 06:19:25.000000 mmtools-0.0.8/mmtools/arguments.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     4006 2020-05-25 06:00:46.000000 mmtools-0.0.8/mmtools/mattermost.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1195 2020-05-25 06:18:14.000000 mmtools-0.0.8/setup.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2020-05-25 06:19:56.000000 mmtools-0.0.8/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3570 2020-05-25 06:19:56.000000 mmtools-0.0.8/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2219 2020-05-25 06:00:46.000000 mmtools-0.0.8/README.md
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-05-25 06:19:56.000000 mmtools-0.0.8/mmtools.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      348 2020-05-25 06:19:56.000000 mmtools-0.0.8/mmtools.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       67 2020-05-25 06:19:56.000000 mmtools-0.0.8/mmtools.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-05-25 06:19:56.000000 mmtools-0.0.8/mmtools.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        8 2020-05-25 06:19:56.000000 mmtools-0.0.8/mmtools.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3570 2020-05-25 06:19:56.000000 mmtools-0.0.8/mmtools.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      110 2020-05-25 06:19:56.000000 mmtools-0.0.8/mmtools.egg-info/entry_points.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-05-25 06:08:44.000000 mmtools-0.0.8/mmtools.egg-info/zip-safe
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-10-22 06:39:59.000000 mmtools-0.0.9/
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-10-22 06:39:59.000000 mmtools-0.0.9/mmtools/
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     1619 2020-05-25 06:00:46.000000 mmtools-0.0.9/mmtools/config.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2020-05-25 06:00:46.000000 mmtools-0.0.9/mmtools/__init__.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     4257 2020-05-25 06:00:46.000000 mmtools-0.0.9/mmtools/watch.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2147 2020-05-25 06:00:46.000000 mmtools-0.0.9/mmtools/status.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     4489 2020-10-22 06:39:02.000000 mmtools-0.0.9/mmtools/arguments.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     4006 2020-05-25 06:00:46.000000 mmtools-0.0.9/mmtools/mattermost.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1195 2020-10-22 06:39:04.000000 mmtools-0.0.9/setup.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2020-10-22 06:39:59.000000 mmtools-0.0.9/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3570 2020-10-22 06:39:59.000000 mmtools-0.0.9/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2219 2020-05-25 06:00:46.000000 mmtools-0.0.9/README.md
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-10-22 06:39:59.000000 mmtools-0.0.9/mmtools.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      348 2020-10-22 06:39:59.000000 mmtools-0.0.9/mmtools.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       67 2020-10-22 06:39:59.000000 mmtools-0.0.9/mmtools.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-10-22 06:39:59.000000 mmtools-0.0.9/mmtools.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        8 2020-10-22 06:39:59.000000 mmtools-0.0.9/mmtools.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3570 2020-10-22 06:39:59.000000 mmtools-0.0.9/mmtools.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      110 2020-10-22 06:39:59.000000 mmtools-0.0.9/mmtools.egg-info/entry_points.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-05-25 06:08:44.000000 mmtools-0.0.9/mmtools.egg-info/zip-safe
```

### Comparing `mmtools-0.0.8/mmtools/config.py` & `mmtools-0.0.9/mmtools/config.py`

 * *Files identical despite different names*

### Comparing `mmtools-0.0.8/mmtools/watch.py` & `mmtools-0.0.9/mmtools/watch.py`

 * *Files identical despite different names*

### Comparing `mmtools-0.0.8/mmtools/status.py` & `mmtools-0.0.9/mmtools/status.py`

 * *Files identical despite different names*

### Comparing `mmtools-0.0.8/mmtools/arguments.py` & `mmtools-0.0.9/mmtools/arguments.py`

 * *Files identical despite different names*

### Comparing `mmtools-0.0.8/mmtools/mattermost.py` & `mmtools-0.0.9/mmtools/mattermost.py`

 * *Files identical despite different names*

### Comparing `mmtools-0.0.8/setup.py` & `mmtools-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), "rb") as f:
     long_description = f.read().decode('utf-8')
 
 setup(
     name="mmtools",
-    version="0.0.8",
+    version="0.0.9",
     author="Fredrik Borg",
     zip_safe=True,
     author_email="fredrikb.borg@gmail.com",
     description="mmtools",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="ISC",
```

### Comparing `mmtools-0.0.8/PKG-INFO` & `mmtools-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: mmtools
 Home-page: https://github.com/frbor/mmtools
 Author: Fredrik Borg
 Author-email: fredrikb.borg@gmail.com
 License: ISC
 Description: # mmtools - i3 status bar and notification script for Mattermost
```

### Comparing `mmtools-0.0.8/README.md` & `mmtools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mmtools-0.0.8/mmtools.egg-info/PKG-INFO` & `mmtools-0.0.9/mmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: mmtools
 Home-page: https://github.com/frbor/mmtools
 Author: Fredrik Borg
 Author-email: fredrikb.borg@gmail.com
 License: ISC
 Description: # mmtools - i3 status bar and notification script for Mattermost
```

