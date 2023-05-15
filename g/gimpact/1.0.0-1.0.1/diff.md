# Comparing `tmp/gimpact-1.0.0.tar.gz` & `tmp/gimpact-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimpact-1.0.0.tar", last modified: Mon May  9 13:25:57 2022, max compression
+gzip compressed data, was "gimpact-1.0.1.tar", last modified: Mon May 15 12:56:49 2023, max compression
```

## Comparing `gimpact-1.0.0.tar` & `gimpact-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwxrwx   0        0        0        0 2022-05-09 13:25:57.266767 gimpact-1.0.0/
-drwxrwxrwx   0        0        0        0 2022-05-09 13:25:56.894236 gimpact-1.0.0/GIMPACT/
-drwxrwxrwx   0        0        0        0 2022-05-09 13:25:56.961241 gimpact-1.0.0/GIMPACT/include/
-drwxrwxrwx   0        0        0        0 2022-05-09 13:25:57.054767 gimpact-1.0.0/GIMPACT/include/GIMPACT/
--rw-rw-rw-   0        0        0    13665 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_boxpruning.h
--rw-rw-rw-   0        0        0     3964 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_contact.h
--rw-rw-rw-   0        0        0    47642 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_geometry.h
--rw-rw-rw-   0        0        0     4200 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_math.h
--rw-rw-rw-   0        0        0    36117 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_memory.h
--rw-rw-rw-   0        0        0     7570 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_radixsort.h
--rw-rw-rw-   0        0        0     3647 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_tri_capsule_collision.h
--rw-rw-rw-   0        0        0     7516 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_tri_collision.h
--rw-rw-rw-   0        0        0     1817 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_tri_sphere_collision.h
--rw-rw-rw-   0        0        0    18168 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_trimesh.h
--rw-rw-rw-   0        0        0     1552 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/GIMPACT/gimpact.h
--rw-rw-rw-   0        0        0    22224 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/include/simplify.h
-drwxrwxrwx   0        0        0        0 2022-05-09 13:25:57.166769 gimpact-1.0.0/GIMPACT/src/
--rw-rw-rw-   0        0        0    17661 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_boxpruning.cpp
--rw-rw-rw-   0        0        0     4265 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_contact.cpp
--rw-rw-rw-   0        0        0     1692 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_math.cpp
--rw-rw-rw-   0        0        0    26992 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_memory.cpp
--rw-rw-rw-   0        0        0     9055 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_tri_tri_overlap.cpp
--rw-rw-rw-   0        0        0    14705 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_trimesh.cpp
--rw-rw-rw-   0        0        0     9466 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_trimesh_capsule_collision.cpp
--rw-rw-rw-   0        0        0     4653 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_trimesh_ray_collision.cpp
--rw-rw-rw-   0        0        0     6522 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_trimesh_sphere_collision.cpp
--rw-rw-rw-   0        0        0    10387 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gim_trimesh_trimesh_collision.cpp
--rw-rw-rw-   0        0        0     1297 2021-03-20 16:50:42.000000 gimpact-1.0.0/GIMPACT/src/gimpact.cpp
--rw-rw-rw-   0        0        0     1542 2021-03-20 16:50:42.000000 gimpact-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      158 2022-05-06 12:49:35.000000 gimpact-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3162 2022-05-09 13:25:57.258784 gimpact-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1938 2022-05-09 11:34:43.000000 gimpact-1.0.0/README.md
--rw-rw-rw-   0        0        0  1400154 2022-05-06 11:49:14.000000 gimpact-1.0.0/gimpact.cpp
-drwxrwxrwx   0        0        0        0 2022-05-09 13:25:57.239767 gimpact-1.0.0/gimpact.egg-info/
--rw-rw-rw-   0        0        0     3162 2022-05-09 13:25:56.000000 gimpact-1.0.0/gimpact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1130 2022-05-09 13:25:56.000000 gimpact-1.0.0/gimpact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-09 13:25:56.000000 gimpact-1.0.0/gimpact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-05-09 13:25:56.000000 gimpact-1.0.0/gimpact.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2022-05-09 13:25:56.000000 gimpact-1.0.0/gimpact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6135 2021-03-20 16:50:43.000000 gimpact-1.0.0/gimpact.pxd
--rw-rw-rw-   0        0        0    23143 2021-03-20 16:50:43.000000 gimpact-1.0.0/gimpact.pyx
--rw-rw-rw-   0        0        0      127 2022-05-09 11:46:37.000000 gimpact-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-05-09 13:25:57.266767 gimpact-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3219 2022-05-09 13:20:34.000000 gimpact-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-09 13:25:57.254767 gimpact-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2021-03-20 16:50:43.000000 gimpact-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0    12667 2021-03-20 16:50:43.000000 gimpact-1.0.0/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:56:49.648098 gimpact-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-15 12:56:49.367091 gimpact-1.0.1/GIMPACT/
+drwxrwxrwx   0        0        0        0 2023-05-15 12:56:49.448099 gimpact-1.0.1/GIMPACT/include/
+drwxrwxrwx   0        0        0        0 2023-05-15 12:56:49.533093 gimpact-1.0.1/GIMPACT/include/GIMPACT/
+-rw-rw-rw-   0        0        0    13665 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_boxpruning.h
+-rw-rw-rw-   0        0        0     3964 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_contact.h
+-rw-rw-rw-   0        0        0    47642 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_geometry.h
+-rw-rw-rw-   0        0        0     4200 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_math.h
+-rw-rw-rw-   0        0        0    36117 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_memory.h
+-rw-rw-rw-   0        0        0     7570 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_radixsort.h
+-rw-rw-rw-   0        0        0     3647 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_tri_capsule_collision.h
+-rw-rw-rw-   0        0        0     7516 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_tri_collision.h
+-rw-rw-rw-   0        0        0     1817 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_tri_sphere_collision.h
+-rw-rw-rw-   0        0        0    18168 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_trimesh.h
+-rw-rw-rw-   0        0        0     1552 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/GIMPACT/gimpact.h
+-rw-rw-rw-   0        0        0    22224 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/include/simplify.h
+drwxrwxrwx   0        0        0        0 2023-05-15 12:56:49.594092 gimpact-1.0.1/GIMPACT/src/
+-rw-rw-rw-   0        0        0    17661 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_boxpruning.cpp
+-rw-rw-rw-   0        0        0     4265 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_contact.cpp
+-rw-rw-rw-   0        0        0     1692 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_math.cpp
+-rw-rw-rw-   0        0        0    26992 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_memory.cpp
+-rw-rw-rw-   0        0        0     9055 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_tri_tri_overlap.cpp
+-rw-rw-rw-   0        0        0    14705 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_trimesh.cpp
+-rw-rw-rw-   0        0        0     9466 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_trimesh_capsule_collision.cpp
+-rw-rw-rw-   0        0        0     4653 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_trimesh_ray_collision.cpp
+-rw-rw-rw-   0        0        0     6522 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_trimesh_sphere_collision.cpp
+-rw-rw-rw-   0        0        0    10387 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gim_trimesh_trimesh_collision.cpp
+-rw-rw-rw-   0        0        0     1297 2021-03-20 16:50:42.000000 gimpact-1.0.1/GIMPACT/src/gimpact.cpp
+-rw-rw-rw-   0        0        0     1542 2021-03-20 16:50:42.000000 gimpact-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      158 2022-05-06 12:49:35.000000 gimpact-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4747 2023-05-15 12:56:49.639093 gimpact-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1938 2022-05-09 11:34:43.000000 gimpact-1.0.1/README.md
+-rw-rw-rw-   0        0        0  1400154 2022-05-06 11:49:14.000000 gimpact-1.0.1/gimpact.cpp
+drwxrwxrwx   0        0        0        0 2023-05-15 12:56:49.632090 gimpact-1.0.1/gimpact.egg-info/
+-rw-rw-rw-   0        0        0     4747 2023-05-15 12:56:49.000000 gimpact-1.0.1/gimpact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1100 2023-05-15 12:56:49.000000 gimpact-1.0.1/gimpact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 12:56:49.000000 gimpact-1.0.1/gimpact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 12:56:49.000000 gimpact-1.0.1/gimpact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6135 2021-03-20 16:50:43.000000 gimpact-1.0.1/gimpact.pxd
+-rw-rw-rw-   0        0        0    23143 2021-03-20 16:50:43.000000 gimpact-1.0.1/gimpact.pyx
+-rw-rw-rw-   0        0        0     1077 2023-05-15 12:36:57.000000 gimpact-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 12:56:49.648098 gimpact-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3136 2023-05-15 12:55:57.000000 gimpact-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:56:49.636090 gimpact-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2021-03-20 16:50:43.000000 gimpact-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0    12667 2021-03-20 16:50:43.000000 gimpact-1.0.1/tests/tests.py
```

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_boxpruning.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_boxpruning.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_contact.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_contact.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_geometry.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_geometry.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_math.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_math.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_memory.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_memory.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_radixsort.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_radixsort.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_tri_capsule_collision.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_tri_capsule_collision.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_tri_collision.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_tri_collision.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_tri_sphere_collision.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_tri_sphere_collision.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gim_trimesh.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gim_trimesh.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/GIMPACT/gimpact.h` & `gimpact-1.0.1/GIMPACT/include/GIMPACT/gimpact.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/include/simplify.h` & `gimpact-1.0.1/GIMPACT/include/simplify.h`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_boxpruning.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_boxpruning.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_contact.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_contact.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_math.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_math.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_memory.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_memory.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_tri_tri_overlap.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_tri_tri_overlap.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_trimesh.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_trimesh.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_trimesh_capsule_collision.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_trimesh_capsule_collision.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_trimesh_ray_collision.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_trimesh_ray_collision.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_trimesh_sphere_collision.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_trimesh_sphere_collision.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gim_trimesh_trimesh_collision.cpp` & `gimpact-1.0.1/GIMPACT/src/gim_trimesh_trimesh_collision.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/GIMPACT/src/gimpact.cpp` & `gimpact-1.0.1/GIMPACT/src/gimpact.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/LICENSE` & `gimpact-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/README.md` & `gimpact-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/gimpact.cpp` & `gimpact-1.0.1/gimpact.cpp`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/gimpact.egg-info/SOURCES.txt` & `gimpact-1.0.1/gimpact.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,11 +28,10 @@
 GIMPACT/src/gim_trimesh_ray_collision.cpp
 GIMPACT/src/gim_trimesh_sphere_collision.cpp
 GIMPACT/src/gim_trimesh_trimesh_collision.cpp
 GIMPACT/src/gimpact.cpp
 gimpact.egg-info/PKG-INFO
 gimpact.egg-info/SOURCES.txt
 gimpact.egg-info/dependency_links.txt
-gimpact.egg-info/requires.txt
 gimpact.egg-info/top_level.txt
 tests/__init__.py
 tests/tests.py
```

### Comparing `gimpact-1.0.0/gimpact.pxd` & `gimpact-1.0.1/gimpact.pxd`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/gimpact.pyx` & `gimpact-1.0.1/gimpact.pyx`

 * *Files identical despite different names*

### Comparing `gimpact-1.0.0/setup.py` & `gimpact-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Package meta-data.
 NAME = 'gimpact'
 DESCRIPTION = 'An unofficial python extension for the GImpact collision library.'
 URL = 'https://github.com/StephenNneji'
 AUTHOR = 'Stephen Nneji'
 EMAIL = 'steve.nneji@gmail.com'
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 
 path=os.path.abspath(os.path.dirname(__file__))
 try:
     with open(os.path.join(path, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
@@ -71,14 +71,12 @@
           'Programming Language :: Python :: 3.4',
           'Programming Language :: Python :: 3.5',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Cython'
       ],
-      keywords='GImpact,Trimesh,Collision detection,Cython',
+      keywords='GImpact, Trimesh, Collision detection, Cython',
       cmdclass={"build_ext": build_ext},
       ext_modules=[Extension("", [])],
-      test_suite='tests',
-      install_requires = ['numpy>=1.18.5'],
-      tests_require=['numpy>=1.18.5'],
+      test_suite='tests'
 )
```

### Comparing `gimpact-1.0.0/tests/tests.py` & `gimpact-1.0.1/tests/tests.py`

 * *Files identical despite different names*

