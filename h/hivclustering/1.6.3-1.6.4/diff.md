# Comparing `tmp/hivclustering-1.6.3.tar.gz` & `tmp/hivclustering-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hivclustering-1.6.3.tar", last modified: Mon Jul 20 20:01:56 2020, max compression
+gzip compressed data, was "hivclustering-1.6.4.tar", last modified: Mon May 15 19:24:20 2023, max compression
```

## Comparing `hivclustering-1.6.3.tar` & `hivclustering-1.6.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2020-07-20 20:01:56.000000 hivclustering-1.6.3/
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering/
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering/data/
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering/data/HBL/
--rw-r--r--   0 sweaver    (554) veg        (576)    11479 2019-03-05 17:22:02.000000 hivclustering-1.6.3/hivclustering/data/HBL/CycleSupport.bf
--rw-r--r--   0 sweaver    (554) veg        (576)     6622 2019-03-05 17:22:02.000000 hivclustering-1.6.3/hivclustering/data/HBL/DegreeDistributions.bf
--rw-r--r--   0 sweaver    (554) veg        (576)      616 2015-08-31 19:36:41.000000 hivclustering-1.6.3/hivclustering/data/HBL/ExtractACluster.bf
--rw-r--r--   0 sweaver    (554) veg        (576)      837 2019-03-05 17:22:02.000000 hivclustering-1.6.3/hivclustering/data/HBL/ExtractSequences.bf
--rw-r--r--   0 sweaver    (554) veg        (576)     8264 2015-08-31 19:36:41.000000 hivclustering-1.6.3/hivclustering/data/HBL/SimulateSequence.bf
--rw-r--r--   0 sweaver    (554) veg        (576)     3512 2020-07-20 19:37:54.000000 hivclustering-1.6.3/hivclustering/data/HBL/TriangleSupport.bf
--rw-r--r--   0 sweaver    (554) veg        (576)       92 2019-03-05 17:22:02.000000 hivclustering-1.6.3/hivclustering/__init__.py
--rw-r--r--   0 sweaver    (554) veg        (576)     5580 2019-09-04 16:11:50.000000 hivclustering-1.6.3/hivclustering/ll.py
--rw-r--r--   0 sweaver    (554) veg        (576)   107327 2020-07-20 19:37:54.000000 hivclustering-1.6.3/hivclustering/mtnetwork.py
--rwxr-xr-x   0 sweaver    (554) veg        (576)    43610 2020-07-20 19:37:54.000000 hivclustering-1.6.3/hivclustering/networkbuild.py
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering.egg-info/
--rw-r--r--   0 sweaver    (554) veg        (576)      264 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering.egg-info/PKG-INFO
--rw-r--r--   0 sweaver    (554) veg        (576)      621 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering.egg-info/SOURCES.txt
--rw-r--r--   0 sweaver    (554) veg        (576)        1 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering.egg-info/dependency_links.txt
--rw-r--r--   0 sweaver    (554) veg        (576)       47 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering.egg-info/requires.txt
--rw-r--r--   0 sweaver    (554) veg        (576)       14 2020-07-20 20:01:56.000000 hivclustering-1.6.3/hivclustering.egg-info/top_level.txt
-drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2020-07-20 20:01:56.000000 hivclustering-1.6.3/scripts/
--rwxr-xr-x   0 sweaver    (554) veg        (576)    23567 2019-03-05 17:22:02.000000 hivclustering-1.6.3/scripts/TNS
--rwxr-xr-x   0 sweaver    (554) veg        (576)     9069 2020-07-20 19:37:54.000000 hivclustering-1.6.3/scripts/hivnetworkannotate
--rwxr-xr-x   0 sweaver    (554) veg        (576)    33221 2020-07-20 19:41:22.000000 hivclustering-1.6.3/scripts/hivnetworkcsv
--rw-r--r--   0 sweaver    (554) veg        (576)     8869 2020-07-20 19:37:54.000000 hivclustering-1.6.3/README.md
--rw-r--r--   0 sweaver    (554) veg        (576)      777 2020-07-20 20:01:28.000000 hivclustering-1.6.3/setup.py
--rw-r--r--   0 sweaver    (554) veg        (576)      264 2020-07-20 20:01:56.000000 hivclustering-1.6.3/PKG-INFO
--rw-r--r--   0 sweaver    (554) veg        (576)       38 2020-07-20 20:01:56.000000 hivclustering-1.6.3/setup.cfg
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.904826 hivclustering-1.6.4/
+-rw-r--r--   0 sweaver    (554) veg        (576)      225 2023-05-15 19:24:20.903826 hivclustering-1.6.4/PKG-INFO
+-rw-r--r--   0 sweaver    (554) veg        (576)     8869 2020-07-20 19:37:54.000000 hivclustering-1.6.4/README.md
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.896826 hivclustering-1.6.4/hivclustering/
+-rw-r--r--   0 sweaver    (554) veg        (576)       92 2019-03-05 17:22:02.000000 hivclustering-1.6.4/hivclustering/__init__.py
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.891826 hivclustering-1.6.4/hivclustering/data/
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.902826 hivclustering-1.6.4/hivclustering/data/HBL/
+-rw-r--r--   0 sweaver    (554) veg        (576)    11479 2019-03-05 17:22:02.000000 hivclustering-1.6.4/hivclustering/data/HBL/CycleSupport.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)     6622 2019-03-05 17:22:02.000000 hivclustering-1.6.4/hivclustering/data/HBL/DegreeDistributions.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)      616 2015-08-31 19:36:41.000000 hivclustering-1.6.4/hivclustering/data/HBL/ExtractACluster.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)      837 2019-03-05 17:22:02.000000 hivclustering-1.6.4/hivclustering/data/HBL/ExtractSequences.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)     8264 2015-08-31 19:36:41.000000 hivclustering-1.6.4/hivclustering/data/HBL/SimulateSequence.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)     3512 2020-07-20 19:37:54.000000 hivclustering-1.6.4/hivclustering/data/HBL/TriangleSupport.bf
+-rw-r--r--   0 sweaver    (554) veg        (576)     5580 2019-09-04 16:11:50.000000 hivclustering-1.6.4/hivclustering/ll.py
+-rw-r--r--   0 sweaver    (554) veg        (576)   107327 2020-07-20 19:37:54.000000 hivclustering-1.6.4/hivclustering/mtnetwork.py
+-rwxr-xr-x   0 sweaver    (554) veg        (576)    43610 2020-07-20 19:37:54.000000 hivclustering-1.6.4/hivclustering/networkbuild.py
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.899826 hivclustering-1.6.4/hivclustering.egg-info/
+-rw-r--r--   0 sweaver    (554) veg        (576)      225 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/PKG-INFO
+-rw-r--r--   0 sweaver    (554) veg        (576)      621 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/SOURCES.txt
+-rw-r--r--   0 sweaver    (554) veg        (576)        1 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/dependency_links.txt
+-rw-r--r--   0 sweaver    (554) veg        (576)       48 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/requires.txt
+-rw-r--r--   0 sweaver    (554) veg        (576)       14 2023-05-15 19:24:20.000000 hivclustering-1.6.4/hivclustering.egg-info/top_level.txt
+drwxr-xr-x   0 sweaver    (554) veg        (576)        0 2023-05-15 19:24:20.903826 hivclustering-1.6.4/scripts/
+-rwxr-xr-x   0 sweaver    (554) veg        (576)    23567 2019-03-05 17:22:02.000000 hivclustering-1.6.4/scripts/TNS
+-rwxr-xr-x   0 sweaver    (554) veg        (576)     9069 2020-07-20 19:37:54.000000 hivclustering-1.6.4/scripts/hivnetworkannotate
+-rwxr-xr-x   0 sweaver    (554) veg        (576)    33221 2020-07-20 19:41:22.000000 hivclustering-1.6.4/scripts/hivnetworkcsv
+-rw-r--r--   0 sweaver    (554) veg        (576)       38 2023-05-15 19:24:20.904826 hivclustering-1.6.4/setup.cfg
+-rw-r--r--   0 sweaver    (554) veg        (576)      778 2023-05-15 19:24:11.000000 hivclustering-1.6.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hivclustering-1.6.3/hivclustering/data/HBL/CycleSupport.bf` & `hivclustering-1.6.4/hivclustering/data/HBL/CycleSupport.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering/data/HBL/DegreeDistributions.bf` & `hivclustering-1.6.4/hivclustering/data/HBL/DegreeDistributions.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering/data/HBL/ExtractACluster.bf` & `hivclustering-1.6.4/hivclustering/data/HBL/ExtractACluster.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering/data/HBL/ExtractSequences.bf` & `hivclustering-1.6.4/hivclustering/data/HBL/ExtractSequences.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering/data/HBL/SimulateSequence.bf` & `hivclustering-1.6.4/hivclustering/data/HBL/SimulateSequence.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering/data/HBL/TriangleSupport.bf` & `hivclustering-1.6.4/hivclustering/data/HBL/TriangleSupport.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering/ll.py` & `hivclustering-1.6.4/hivclustering/ll.py`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering/mtnetwork.py` & `hivclustering-1.6.4/hivclustering/mtnetwork.py`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering/networkbuild.py` & `hivclustering-1.6.4/hivclustering/networkbuild.py`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/hivclustering.egg-info/SOURCES.txt` & `hivclustering-1.6.4/hivclustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/scripts/TNS` & `hivclustering-1.6.4/scripts/TNS`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/scripts/hivnetworkannotate` & `hivclustering-1.6.4/scripts/hivnetworkannotate`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/scripts/hivnetworkcsv` & `hivclustering-1.6.4/scripts/hivnetworkcsv`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/README.md` & `hivclustering-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.3/setup.py` & `hivclustering-1.6.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from os.path import abspath, join, split
 from setuptools import setup
 
 sys.path.insert(0, join(split(abspath(__file__))[0], 'lib'))
 
 setup(name='hivclustering',
-      version="1.6.3",
+      version="1.6.4",
       description='HIV molecular clustering tools',
       author='Sergei Kosakovsky Pond',
       author_email='spond@ucsd.edu',
       url='http://github.com/veg/hivclustering',
       license='MIT License',
       packages=['hivclustering'],
       package_data={'hivclustering': [
@@ -21,11 +21,11 @@
     scripts=[
         'scripts/hivnetworkcsv',
         'scripts/TNS',
         'scripts/hivnetworkannotate'
     ],
     install_requires=[
         'bioext >= 0.19.0',
-        'hyphy-python >= 0.1.9',
+        'hyphy-python >= 0.1.11',
         'hppy >= 0.9.9',
         ],
      )
```

