# Comparing `tmp/decorrelation-0.1.0.tar.gz` & `tmp/decorrelation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorrelation-0.1.0.tar", last modified: Wed Apr 12 21:43:20 2023, max compression
+gzip compressed data, was "decorrelation-0.2.0.tar", last modified: Mon May 15 02:51:28 2023, max compression
```

## Comparing `decorrelation-0.1.0.tar` & `decorrelation-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:43:20.165218 decorrelation-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    33253 2023-04-12 21:42:51.000000 decorrelation-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 21:42:51.000000 decorrelation-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-12 21:43:20.165218 decorrelation-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-12 21:42:51.000000 decorrelation-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:43:20.165218 decorrelation-0.1.0/decorrelation/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/co.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/pl.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/shp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:43:20.165218 decorrelation-0.1.0/decorrelation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:43:19.000000 decorrelation-0.1.0/decorrelation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-12 21:42:51.000000 decorrelation-0.1.0/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 21:43:20.165218 decorrelation-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-12 21:42:51.000000 decorrelation-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:51:28.433784 decorrelation-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    33253 2023-05-15 02:50:59.000000 decorrelation-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 02:50:59.000000 decorrelation-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 02:51:28.433784 decorrelation-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 02:50:59.000000 decorrelation-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:51:28.429784 decorrelation-0.2.0/decorrelation/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:51:28.433784 decorrelation-0.2.0/decorrelation/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/cli/co.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/cli/pl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/cli/shp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:51:28.433784 decorrelation-0.2.0/decorrelation/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/cli/utils/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/cli/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/co.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/pl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/shp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-15 02:50:59.000000 decorrelation-0.2.0/decorrelation/sparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:51:28.433784 decorrelation-0.2.0/decorrelation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 02:51:28.000000 decorrelation-0.2.0/decorrelation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-15 02:51:28.000000 decorrelation-0.2.0/decorrelation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 02:51:28.000000 decorrelation-0.2.0/decorrelation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-15 02:51:28.000000 decorrelation-0.2.0/decorrelation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 02:51:27.000000 decorrelation-0.2.0/decorrelation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-15 02:51:28.000000 decorrelation-0.2.0/decorrelation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 02:51:28.000000 decorrelation-0.2.0/decorrelation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-15 02:50:59.000000 decorrelation-0.2.0/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 02:51:28.433784 decorrelation-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-15 02:50:59.000000 decorrelation-0.2.0/setup.py
```

### Comparing `decorrelation-0.1.0/LICENSE` & `decorrelation-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decorrelation-0.1.0/PKG-INFO` & `decorrelation-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorrelation
-Version: 0.1.0
+Version: 0.2.0
 Summary: An InSAR postprocessing tool
 Home-page: https://github.com/kanglcn/decorrelation
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA
 Classifier: Development Status :: 4 - Beta
@@ -57,14 +57,31 @@
 
 ## How to use
 
 ``` python
 import decorrelation as dc
 ```
 
+This package provide functions for InSAR post-processing which refers as
+processing after SAR images co-registration and geocoding. The functions
+include PS/DS identification, coherence matrix estimation, phase linking
+etc.
+
+Most of the python functions in this package provide 2 kind of API, the
+array-based API and the file-based API. The inputs of array-based
+functions generally are numpy or cupy arrays. The inputs of file-based
+functions are string of path to the array stored in disk. The file-based
+functions make use of `dask` package to decrease the memory usage and
+parallelize the job. However, their is performance cost for using
+`dask`, if no parallelization is needed and the memory fits the data,
+the array-based API is recommended.
+
+CLI is also provided and is almost the same as the file-based API. The
+only difference between them is the CLI can not directly show the plot.
+
 Please refer to the
 [Documentation](https://kanglcn.github.io/decorrelation) for detailed
 usage.
 
 **Warning!!!** This package is under intensive development. API is
 subjected to change without any noticement.
 
@@ -79,12 +96,12 @@
   ask questions or leave comments.
 
 ## Contribution
 
 - Pull requests are welcomed! Before making a pull request, please open
   an issue to talk about it.
 - We have notice many excellent open-source packages are rarely paid
-  attention to due to lake of documentation. The package is developed
+  attention to due to lack of documentation. The package is developed
   with the [nbdev](https://nbdev.fast.ai/), a notebook-driven
-  development platform. Developers only needs to simply write notebooks
+  development platform. Developers only need to simply write notebooks
   with lightweight markup and get high-quality documentation, tests,
   continuous integration, and packaging automatically.
```

### Comparing `decorrelation-0.1.0/decorrelation/co.py` & `decorrelation-0.2.0/decorrelation/co.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     }
     ''',
     name = 'emperical_co_sp_kernel',reduce_dims = False,no_return=True
 )
 
 # %% ../nbs/API/co.ipynb 17
 def emperical_co_sp(rslc:cp.ndarray, # rslc stack, dtype: `cupy.complexfloating`
-                    sp_idx:cp.ndarray, # index of sparse data [azimuth_index, range_index], dtype: `cupy.int`, shape: (n_sp,2)
+                    sp_idx:tuple[cp.ndarray,cp.ndarray], # index of sparse data (azimuth_index, range_index), dtype: `cupy.int`, shape: (n_sp,)
                     is_shp_sp:cp.ndarray, # shp bool, dtype: `cupy.bool`
                     block_size:int=128, # the CUDA block size, it only affects the calculation speed
                    )-> tuple[cp.ndarray,cp.ndarray]: # the covariance and coherence matrix `cov` and `coh`
     '''
     Maximum likelihood covariance estimator for sparse data.
     '''
     nlines, width, nimages = rslc.shape
```

### Comparing `decorrelation-0.1.0/decorrelation/pl.py` & `decorrelation-0.2.0/decorrelation/pl.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 __all__ = ['emi', 'temp_coh']
 
 # %% ../nbs/API/pl.ipynb 5
 import cupy as cp
 
 # %% ../nbs/API/pl.ipynb 8
 def emi(coh:cp.ndarray, #complex coherence metrix,dtype cupy.complex
+        ref:int=0, #index of reference image in the phase history output, optional. Default: 0
        )-> tuple[cp.ndarray,cp.ndarray]: # estimated phase history `ph`, dtype complex; quality (minimum eigvalue, dtype float)
     coh_mag = abs(coh)
     coh_mag_inv = cp.linalg.inv(coh_mag)
     min_eigval, min_eig = cp.linalg.eigh(coh_mag_inv*coh)
     min_eigval = min_eigval[...,0]
-    min_eig = min_eig[...,0]
+    # min_eig = min_eig[...,0]
+    min_eig = min_eig[...,0]*min_eig[...,[ref],0].conj()
 
     return min_eig/abs(min_eig), min_eigval
 
-# %% ../nbs/API/pl.ipynb 16
+# %% ../nbs/API/pl.ipynb 17
 def temp_coh(coh:cp.ndarray,# complex coherence metrix, dtype cupy.complex
              ds_ph = cp.ndarray, # complex phase history, dtype cupy.complex
             ):
     nimages = ds_ph.shape[-1]
     assert coh.shape[-2:] == (nimages,nimages), "input dimension not match"
     ds_ph = ds_ph/abs(ds_ph)
     coh = coh/abs(coh)
```

### Comparing `decorrelation-0.1.0/decorrelation/shp.py` & `decorrelation-0.2.0/decorrelation/shp.py`

 * *Files identical despite different names*

### Comparing `decorrelation-0.1.0/decorrelation.egg-info/PKG-INFO` & `decorrelation-0.2.0/decorrelation.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorrelation
-Version: 0.1.0
+Version: 0.2.0
 Summary: An InSAR postprocessing tool
 Home-page: https://github.com/kanglcn/decorrelation
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA
 Classifier: Development Status :: 4 - Beta
@@ -57,14 +57,31 @@
 
 ## How to use
 
 ``` python
 import decorrelation as dc
 ```
 
+This package provide functions for InSAR post-processing which refers as
+processing after SAR images co-registration and geocoding. The functions
+include PS/DS identification, coherence matrix estimation, phase linking
+etc.
+
+Most of the python functions in this package provide 2 kind of API, the
+array-based API and the file-based API. The inputs of array-based
+functions generally are numpy or cupy arrays. The inputs of file-based
+functions are string of path to the array stored in disk. The file-based
+functions make use of `dask` package to decrease the memory usage and
+parallelize the job. However, their is performance cost for using
+`dask`, if no parallelization is needed and the memory fits the data,
+the array-based API is recommended.
+
+CLI is also provided and is almost the same as the file-based API. The
+only difference between them is the CLI can not directly show the plot.
+
 Please refer to the
 [Documentation](https://kanglcn.github.io/decorrelation) for detailed
 usage.
 
 **Warning!!!** This package is under intensive development. API is
 subjected to change without any noticement.
 
@@ -79,12 +96,12 @@
   ask questions or leave comments.
 
 ## Contribution
 
 - Pull requests are welcomed! Before making a pull request, please open
   an issue to talk about it.
 - We have notice many excellent open-source packages are rarely paid
-  attention to due to lake of documentation. The package is developed
+  attention to due to lack of documentation. The package is developed
   with the [nbdev](https://nbdev.fast.ai/), a notebook-driven
-  development platform. Developers only needs to simply write notebooks
+  development platform. Developers only need to simply write notebooks
   with lightweight markup and get high-quality documentation, tests,
   continuous integration, and packaging automatically.
```

### Comparing `decorrelation-0.1.0/setup.py` & `decorrelation-0.2.0/setup.py`

 * *Files identical despite different names*

