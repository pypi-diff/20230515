# Comparing `tmp/bicm-3.0.0.tar.gz` & `tmp/bicm-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bicm-3.0.0.tar", last modified: Thu Apr 20 14:02:46 2023, max compression
+gzip compressed data, was "bicm-3.0.1.tar", last modified: Mon May 15 16:08:26 2023, max compression
```

## Comparing `bicm-3.0.0.tar` & `bicm-3.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-04-20 14:02:46.872950 bicm-3.0.0/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1068 2023-01-04 08:23:41.000000 bicm-3.0.0/LICENSE.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     4602 2023-04-20 14:02:46.872950 bicm-3.0.0/PKG-INFO
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     3928 2023-04-20 13:13:38.000000 bicm-3.0.0/README.md
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-04-20 14:02:46.872950 bicm-3.0.0/bicm/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      471 2023-04-06 09:27:43.000000 bicm-3.0.0/bicm/__init__.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    72178 2023-04-20 12:32:35.000000 bicm-3.0.0/bicm/graph_classes.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    40970 2023-04-20 08:23:16.000000 bicm-3.0.0/bicm/models_functions.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    11883 2023-04-20 08:31:25.000000 bicm-3.0.0/bicm/network_functions.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     6409 2023-01-04 08:23:41.000000 bicm-3.0.0/bicm/poibin.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     9439 2023-04-06 09:27:43.000000 bicm-3.0.0/bicm/solver_functions.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-04-20 14:02:46.872950 bicm-3.0.0/bicm.egg-info/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     4602 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/PKG-INFO
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      415 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/SOURCES.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/dependency_links.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       50 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/requires.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       11 2023-04-20 14:02:46.000000 bicm-3.0.0/bicm.egg-info/top_level.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-04-20 14:02:46.872950 bicm-3.0.0/setup.cfg
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1042 2023-04-06 09:27:43.000000 bicm-3.0.0/setup.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-04-20 14:02:46.872950 bicm-3.0.0/tests/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     9480 2023-01-04 08:23:41.000000 bicm-3.0.0/tests/BiCM_test.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-01-04 08:23:41.000000 bicm-3.0.0/tests/__init__.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1804 2023-01-08 16:20:56.000000 bicm-3.0.0/tests/biwcm_c.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     2378 2023-01-08 16:20:56.000000 bicm-3.0.0/tests/biwcm_d.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     7224 2023-01-08 16:20:57.000000 bicm-3.0.0/tests/biwcm_main.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      462 2023-01-04 18:33:41.000000 bicm-3.0.0/tests/delta_converter.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-05-15 16:08:26.132260 bicm-3.0.1/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1068 2023-01-04 08:23:41.000000 bicm-3.0.1/LICENSE.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     5275 2023-05-15 16:08:26.132260 bicm-3.0.1/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     3928 2023-04-20 13:13:38.000000 bicm-3.0.1/README.md
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-05-15 16:08:26.132260 bicm-3.0.1/bicm/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      471 2023-05-15 16:05:15.000000 bicm-3.0.1/bicm/__init__.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    73867 2023-05-15 15:40:13.000000 bicm-3.0.1/bicm/graph_classes.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    40970 2023-04-20 08:23:16.000000 bicm-3.0.1/bicm/models_functions.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    11883 2023-04-20 08:31:25.000000 bicm-3.0.1/bicm/network_functions.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6409 2023-01-04 08:23:41.000000 bicm-3.0.1/bicm/poibin.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     9439 2023-04-06 09:27:43.000000 bicm-3.0.1/bicm/solver_functions.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-05-15 16:08:26.132260 bicm-3.0.1/bicm.egg-info/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     5275 2023-05-15 16:08:26.000000 bicm-3.0.1/bicm.egg-info/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      415 2023-05-15 16:08:26.000000 bicm-3.0.1/bicm.egg-info/SOURCES.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-05-15 16:08:26.000000 bicm-3.0.1/bicm.egg-info/dependency_links.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       50 2023-05-15 16:08:26.000000 bicm-3.0.1/bicm.egg-info/requires.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       11 2023-05-15 16:08:26.000000 bicm-3.0.1/bicm.egg-info/top_level.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-05-15 16:08:26.132260 bicm-3.0.1/setup.cfg
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1042 2023-05-15 16:06:51.000000 bicm-3.0.1/setup.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-05-15 16:08:26.132260 bicm-3.0.1/tests/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     9480 2023-01-04 08:23:41.000000 bicm-3.0.1/tests/BiCM_test.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-01-04 08:23:41.000000 bicm-3.0.1/tests/__init__.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1804 2023-01-08 16:20:56.000000 bicm-3.0.1/tests/biwcm_c.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     2378 2023-01-08 16:20:56.000000 bicm-3.0.1/tests/biwcm_d.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     7224 2023-01-08 16:20:57.000000 bicm-3.0.1/tests/biwcm_main.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      462 2023-01-04 18:33:41.000000 bicm-3.0.1/tests/delta_converter.py
```

### Comparing `bicm-3.0.0/LICENSE.txt` & `bicm-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bicm-3.0.0/PKG-INFO` & `bicm-3.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: bicm
-Version: 3.0.0
-Summary: Package for bipartite configuration model
-Home-page: https://github.com/mat701/BiCM
-Author: Matteo Bruno
-Author-email: matteobruno180@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ﻿## BiCM package
 
 This is a Python package for the computation of the maximum entropy bipartite configuration model (BiCM) and the projection of bipartite networks on one layer. It was developed with Python 3.5.
 
 You can install this package via pip: 
 
     pip install bicm
@@ -100,9 +80,7 @@
 
 [Saracco2017] [F. Saracco, M. J. Straka, R. Di Clemente, A. Gabrielli, G. Caldarelli, and T. Squartini, Inferring monopartite projections of bipartite networks: an entropy-based approach, New J. Phys. 19, 053022 (2017)](http://stacks.iop.org/1367-2630/19/i=5/a=053022)
 
 
 _Author_:
 
 [Matteo Bruno](https://csl.sony.it/member/matteo-bruno/) (BiCM) (a.k.a. [mat701](https://github.com/mat701))
-
-
```

### Comparing `bicm-3.0.0/bicm/graph_classes.py` & `bicm-3.0.1/bicm/graph_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,16 +282,35 @@
             self.r_y = np.random.rand(self.r_n_cols).astype(np.float64)
         elif self.initial_guess == 'uniform':
             self.r_x = np.ones(self.r_n_rows, dtype=np.float64)  # All probabilities will be 1/2 initially
             self.r_y = np.ones(self.r_n_cols, dtype=np.float64)
         elif self.initial_guess == 'degrees':
             self.r_x = self.r_rows_deg.astype(np.float64)
             self.r_y = self.r_cols_deg.astype(np.float64)
+        elif isinstance(self.initial_guess, (tuple, list, np.ndarray)):
+            if len(self.initial_guess) == 2 and type(self.initial_guess[0]) in [tuple, list, np.ndarray]:
+                if len(self.initial_guess[0]) == self.r_n_rows and len(self.initial_guess[1]) == self.r_n_cols:
+                    self.r_x = np.array(self.initial_guess[0])
+                    self.r_y = np.array(self.initial_guess[1])
+                elif len(self.initial_guess[0]) == self.n_rows and len(self.initial_guess[1]) == self.n_cols:
+                    self.r_x[self.r_invert_rows_deg] = self.initial_guess[0][self.nonfixed_rows]
+                    self.r_y[self.r_invert_cols_deg] = self.initial_guess[1][self.nonfixed_cols]
+                else:
+                    raise ValueError('The size of the given initial condition is not the same of the input graph')
+            else:
+                if len(self.initial_guess) == self.r_n_rows + self.r_n_cols:
+                    self.r_x = np.array(self.initial_guess[:self.r_n_rows])
+                    self.r_y = np.array(self.initial_guess[self.r_n_rows:])
+                elif len(self.initial_guess[0]) == self.n_rows and len(self.initial_guess[1]) == self.n_cols:
+                    self.r_x[self.r_invert_rows_deg] = self.initial_guess[:self.r_n_rows][self.nonfixed_rows]
+                    self.r_y[self.r_invert_cols_deg] = self.initial_guess[self.r_n_rows:][self.nonfixed_cols]
+                else:
+                    raise ValueError('The size of the given initial condition is not the same of the input graph')
         else:
-            raise ValueError('initial_guess must be None, "chung_lu", "random", "uniform" or "degrees"')
+            raise ValueError('Initial_guess must be None, "chung_lu", "random", "uniform", "degrees" or an array or a tuple of 2 lists/numpy arrays')
         if not self.exp:
             if self.weighted:  # Avoid negative thetas
                 normalization = max(np.max(self.r_x), np.max(self.r_y))
                 if normalization >= 1:
                     self.r_x /= 2 * normalization
                     self.r_y /= 2 * normalization
             self.r_theta_x = - np.log(self.r_x)
@@ -1514,14 +1533,17 @@
         :type degree_sequences: list, numpy.array, tuple
         """
         if self.is_initialized:
             print('Graph already contains edges or has a degree sequence. Use clean_edges() first.')
         else:
             self._initialize_graph(degree_sequences=degree_sequences)
 
+    def set_to_continuous(self):
+        self.continuous_weights = True
+
     def clean_edges(self):
         """Clean the edges of the graph.
         """
         self.biadjacency = None
         self.edgelist = None
         self.adj_list = None
         self.rows_deg = None
```

### Comparing `bicm-3.0.0/bicm/models_functions.py` & `bicm-3.0.1/bicm/models_functions.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.0/bicm/network_functions.py` & `bicm-3.0.1/bicm/network_functions.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.0/bicm/poibin.py` & `bicm-3.0.1/bicm/poibin.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.0/bicm/solver_functions.py` & `bicm-3.0.1/bicm/solver_functions.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.0/setup.py` & `bicm-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bicm",
-    version="3.0.0",
+    version="3.0.1",
     author="Matteo Bruno",
     author_email="matteobruno180@gmail.com",
     description="Package for bipartite configuration model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mat701/BiCM",
     packages=setuptools.find_packages(),
```

### Comparing `bicm-3.0.0/tests/BiCM_test.py` & `bicm-3.0.1/tests/BiCM_test.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.0/tests/biwcm_c.py` & `bicm-3.0.1/tests/biwcm_c.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.0/tests/biwcm_d.py` & `bicm-3.0.1/tests/biwcm_d.py`

 * *Files identical despite different names*

### Comparing `bicm-3.0.0/tests/biwcm_main.py` & `bicm-3.0.1/tests/biwcm_main.py`

 * *Files identical despite different names*

