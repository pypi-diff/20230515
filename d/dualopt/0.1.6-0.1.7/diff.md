# Comparing `tmp/dualopt-0.1.6.tar.gz` & `tmp/dualopt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualopt-0.1.6.tar", last modified: Mon May 15 04:15:02 2023, max compression
+gzip compressed data, was "dualopt-0.1.7.tar", last modified: Mon May 15 05:39:56 2023, max compression
```

## Comparing `dualopt-0.1.6.tar` & `dualopt-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 04:15:02.408810 dualopt-0.1.6/
--rw-rw-rw-   0        0        0     1091 2023-05-15 01:40:42.000000 dualopt-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      772 2023-05-15 04:15:02.407811 dualopt-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-05-15 01:40:40.000000 dualopt-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 04:15:02.316812 dualopt-0.1.6/dualopt/
--rw-rw-rw-   0        0        0       96 2023-05-15 04:13:43.000000 dualopt-0.1.6/dualopt/__init__.py
--rw-rw-rw-   0        0        0     6067 2023-05-15 01:47:53.000000 dualopt-0.1.6/dualopt/classification.py
-drwxrwxrwx   0        0        0        0 2023-05-15 04:15:02.405812 dualopt-0.1.6/dualopt.egg-info/
--rw-rw-rw-   0        0        0      772 2023-05-15 04:15:02.000000 dualopt-0.1.6/dualopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-15 04:15:02.000000 dualopt-0.1.6/dualopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 04:15:02.000000 dualopt-0.1.6/dualopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-15 04:15:02.000000 dualopt-0.1.6/dualopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 04:15:02.000000 dualopt-0.1.6/dualopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 04:15:02.409811 dualopt-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-05-15 04:14:46.000000 dualopt-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:39:56.494077 dualopt-0.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-05-15 05:39:35.000000 dualopt-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     4981 2023-05-15 05:39:56.486081 dualopt-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-15 05:39:34.000000 dualopt-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 05:39:56.432122 dualopt-0.1.7/dualopt/
+-rw-rw-rw-   0        0        0       96 2023-05-15 05:39:29.000000 dualopt-0.1.7/dualopt/__init__.py
+-rw-rw-rw-   0        0        0     6067 2023-05-15 05:39:31.000000 dualopt-0.1.7/dualopt/classification.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:39:56.483081 dualopt-0.1.7/dualopt.egg-info/
+-rw-rw-rw-   0        0        0     4981 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 05:39:56.000000 dualopt-0.1.7/dualopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:39:56.494077 dualopt-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-15 05:39:32.000000 dualopt-0.1.7/setup.py
```

### Comparing `dualopt-0.1.6/LICENSE` & `dualopt-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.6/dualopt/classification.py` & `dualopt-0.1.7/dualopt/classification.py`

 * *Files identical despite different names*

### Comparing `dualopt-0.1.6/setup.py` & `dualopt-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'dualopt',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'Dual Optimizer Training',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/DualOpt',
```

