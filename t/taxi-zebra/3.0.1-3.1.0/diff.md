# Comparing `tmp/taxi_zebra-3.0.1.tar.gz` & `tmp/taxi_zebra-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxi_zebra-3.0.1.tar", last modified: Fri Jul  8 13:49:10 2022, max compression
+gzip compressed data, was "taxi_zebra-3.1.0.tar", last modified: Mon May 15 10:21:56 2023, max compression
```

## Comparing `taxi_zebra-3.0.1.tar` & `taxi_zebra-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 13:49:10.203201 taxi_zebra-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-07-08 13:49:10.203201 taxi_zebra-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      252 2022-07-08 13:49:10.203201 taxi_zebra-3.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      904 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 13:49:10.199201 taxi_zebra-3.0.1/taxi_zebra/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/taxi_zebra/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10279 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/taxi_zebra/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/taxi_zebra/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/taxi_zebra/roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     6014 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/taxi_zebra/ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-07-08 13:48:54.000000 taxi_zebra-3.0.1/taxi_zebra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 13:49:10.203201 taxi_zebra-3.0.1/taxi_zebra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-07-08 13:49:10.000000 taxi_zebra-3.0.1/taxi_zebra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-07-08 13:49:10.000000 taxi_zebra-3.0.1/taxi_zebra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 13:49:10.000000 taxi_zebra-3.0.1/taxi_zebra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-07-08 13:49:10.000000 taxi_zebra-3.0.1/taxi_zebra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-08 13:49:10.000000 taxi_zebra-3.0.1/taxi_zebra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-08 13:49:10.000000 taxi_zebra-3.0.1/taxi_zebra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-05-15 10:21:56.758171 taxi_zebra-3.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/taxi_zebra/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10302 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/taxi_zebra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/taxi_zebra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 10:21:56.000000 taxi_zebra-3.1.0/taxi_zebra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:21:56.754171 taxi_zebra-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-15 10:21:37.000000 taxi_zebra-3.1.0/tests/test_backend.py
```

### Comparing `taxi_zebra-3.0.1/README.rst` & `taxi_zebra-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `taxi_zebra-3.0.1/setup.py` & `taxi_zebra-3.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 from taxi_zebra import __version__
 
 
 install_requires = [
     'requests>=2.3.0',
-    'taxi~=6.0',
+    'taxi~=6.2',
     'click>=7.0',
 ]
 
 setup(
     name='taxi_zebra',
     version=__version__,
     packages=find_packages(),
     description='Zebra backend for Taxi',
+    long_description='Zebra backend for Taxi',
     author='Sylvain Fankhauser',
     author_email='sylvain.fankhauser@liip.ch',
-    url='https://github.com/sephii/taxi-zebra',
+    url='https://github.com/liip/taxi-zebra',
     install_requires=install_requires,
     license='wtfpl',
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points={
         'taxi.backends': 'zebra = taxi_zebra.backend:ZebraBackend',
         'taxi.commands': ['zebra = taxi_zebra.commands'],
     },
     classifiers=[
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ]
 )
```

### Comparing `taxi_zebra-3.0.1/taxi_zebra/backend.py` & `taxi_zebra-3.1.0/taxi_zebra/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                                              '%Y-%m-%d').date()
                 except (ValueError, TypeError):
                     date = None
 
                 setattr(p, date_attr, date)
 
             for activity in project['activities']:
-                a = Activity(activity['id'], activity['name'])
+                a = Activity(activity['id'], activity['name'], activity['is_active'])
                 p.add_activity(a)
 
                 if activity['alias']:
                     p.aliases[activity['alias']] = activity['id']
 
             projects_list.append(p)
```

### Comparing `taxi_zebra-3.0.1/taxi_zebra/commands.py` & `taxi_zebra-3.1.0/taxi_zebra/commands.py`

 * *Files identical despite different names*

### Comparing `taxi_zebra-3.0.1/taxi_zebra/ui.py` & `taxi_zebra-3.1.0/taxi_zebra/ui.py`

 * *Files identical despite different names*

### Comparing `taxi_zebra-3.0.1/taxi_zebra/utils.py` & `taxi_zebra-3.1.0/taxi_zebra/utils.py`

 * *Files identical despite different names*

