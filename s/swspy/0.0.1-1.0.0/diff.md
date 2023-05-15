# Comparing `tmp/swspy-0.0.1.tar.gz` & `tmp/swspy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swspy-0.0.1.tar", last modified: Fri Jul 30 07:49:43 2021, max compression
+gzip compressed data, was "dist/swspy-1.0.0.tar", last modified: Mon May 15 11:56:20 2023, max compression
```

## Comparing `swspy-0.0.1.tar` & `swspy-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxr-xr-x   0 eart0504   (503) staff       (20)        0 2021-07-30 07:49:43.315623 swspy-0.0.1/
--rw-r--r--   0 eart0504   (503) staff       (20)      547 2021-07-30 07:49:43.315327 swspy-0.0.1/PKG-INFO
--rw-r--r--   0 eart0504   (503) staff       (20)        0 2021-07-30 07:40:01.000000 swspy-0.0.1/README.md
--rw-r--r--   0 eart0504   (503) staff       (20)       38 2021-07-30 07:49:43.315733 swspy-0.0.1/setup.cfg
--rw-r--r--   0 eart0504   (503) staff       (20)      723 2021-07-30 07:48:12.000000 swspy-0.0.1/setup.py
-drwxr-xr-x   0 eart0504   (503) staff       (20)        0 2021-07-30 07:49:43.306807 swspy-0.0.1/swspy/
--rw-r--r--   0 eart0504   (503) staff       (20)      267 2021-07-30 07:40:45.000000 swspy-0.0.1/swspy/__init__.py
--rw-r--r--   0 eart0504   (503) staff       (20)      718 2021-07-30 07:43:08.000000 swspy-0.0.1/swspy/split.py
-drwxr-xr-x   0 eart0504   (503) staff       (20)        0 2021-07-30 07:49:43.314830 swspy-0.0.1/swspy.egg-info/
--rw-r--r--   0 eart0504   (503) staff       (20)      547 2021-07-30 07:49:42.000000 swspy-0.0.1/swspy.egg-info/PKG-INFO
--rw-r--r--   0 eart0504   (503) staff       (20)      167 2021-07-30 07:49:42.000000 swspy-0.0.1/swspy.egg-info/SOURCES.txt
--rw-r--r--   0 eart0504   (503) staff       (20)        1 2021-07-30 07:49:42.000000 swspy-0.0.1/swspy.egg-info/dependency_links.txt
--rw-r--r--   0 eart0504   (503) staff       (20)        6 2021-07-30 07:49:42.000000 swspy-0.0.1/swspy.egg-info/top_level.txt
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/
+-rw-r--r--   0 eart0504   (502) staff       (20)     1397 2023-05-15 11:56:20.000000 swspy-1.0.0/PKG-INFO
+-rw-r--r--   0 eart0504   (502) staff       (20)      665 2021-09-23 13:10:11.000000 swspy-1.0.0/README.md
+-rw-r--r--   0 eart0504   (502) staff       (20)       38 2023-05-15 11:56:20.000000 swspy-1.0.0/setup.cfg
+-rw-r--r--   0 eart0504   (502) staff       (20)      723 2023-05-15 11:54:59.000000 swspy-1.0.0/setup.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy/
+-rw-r--r--   0 eart0504   (502) staff       (20)      436 2021-09-23 09:04:50.000000 swspy-1.0.0/swspy/__init__.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy/automate/
+-rw-r--r--   0 eart0504   (502) staff       (20)      127 2021-09-23 09:03:55.000000 swspy-1.0.0/swspy/automate/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)    15124 2022-07-11 11:27:06.000000 swspy-1.0.0/swspy/automate/automation_manager.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy/io/
+-rw-r--r--   0 eart0504   (502) staff       (20)      126 2021-08-25 10:24:55.000000 swspy-1.0.0/swspy/io/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     9048 2021-12-03 10:26:14.000000 swspy-1.0.0/swspy/io/load.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy/splitting/
+-rw-r--r--   0 eart0504   (502) staff       (20)      133 2023-04-04 15:14:25.000000 swspy-1.0.0/swspy/splitting/__init__.py
+-rw-r--r--   0 eart0504   (502) staff       (20)     7008 2023-04-17 13:05:11.000000 swspy-1.0.0/swspy/splitting/forward_model.py
+-rw-r--r--   0 eart0504   (502) staff       (20)   113994 2023-05-15 11:18:33.000000 swspy-1.0.0/swspy/splitting/split.py
+drwxr-xr-x   0 eart0504   (502) staff       (20)        0 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/
+-rw-r--r--   0 eart0504   (502) staff       (20)     1397 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/PKG-INFO
+-rw-r--r--   0 eart0504   (502) staff       (20)      340 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/SOURCES.txt
+-rw-r--r--   0 eart0504   (502) staff       (20)        1 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/dependency_links.txt
+-rw-r--r--   0 eart0504   (502) staff       (20)        6 2023-05-15 11:56:20.000000 swspy-1.0.0/swspy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `swspy-0.0.1/setup.py` & `swspy-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="swspy",
-    version="0.0.1",
+    version="1.0.0",
     author="Tom Hudson",
     author_email="thomas.hudson@earth.ox.ac.uk",
     description="A package for automatically calculating shear wave splitting for large earthquake catalogues.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TomSHudson/swspy/",
     packages=setuptools.find_packages(),
```

