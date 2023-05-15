# Comparing `tmp/pywayne-1.0.0.3.8.tar.gz` & `tmp/pywayne-1.0.0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.3.8.tar", last modified: Fri Feb 10 11:33:33 2023, max compression
+gzip compressed data, was "pywayne-1.0.0.3.9.tar", last modified: Mon May 15 07:59:08 2023, max compression
```

## Comparing `pywayne-1.0.0.3.8.tar` & `pywayne-1.0.0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-02-10 11:33:33.535933 pywayne-1.0.0.3.8/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.8/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)      970 2023-02-10 11:33:33.535806 pywayne-1.0.0.3.8/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      547 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.8/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-02-10 11:33:33.535032 pywayne-1.0.0.3.8/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      173 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.8/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-02-04 02:47:36.000000 pywayne-1.0.0.3.8/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    15728 2022-11-28 03:15:31.000000 pywayne-1.0.0.3.8/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7353 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.8/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.8/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.8/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)     6904 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.8/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-02-10 11:33:33.535600 pywayne-1.0.0.3.8/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)      970 2023-02-10 11:33:33.000000 pywayne-1.0.0.3.8/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      305 2023-02-10 11:33:33.000000 pywayne-1.0.0.3.8/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2023-02-10 11:33:33.000000 pywayne-1.0.0.3.8/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      133 2023-02-10 11:33:33.000000 pywayne-1.0.0.3.8/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2023-02-10 11:33:33.000000 pywayne-1.0.0.3.8/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2023-02-10 11:33:33.535978 pywayne-1.0.0.3.8/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1409 2023-02-10 11:33:20.000000 pywayne-1.0.0.3.8/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-05-15 07:59:08.559360 pywayne-1.0.0.3.9/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)      951 2023-05-15 07:59:08.559225 pywayne-1.0.0.3.9/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      528 2023-02-10 11:37:25.000000 pywayne-1.0.0.3.9/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-05-15 07:59:08.558157 pywayne-1.0.0.3.9/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      173 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-02-04 02:47:36.000000 pywayne-1.0.0.3.9/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16676 2023-05-15 07:58:38.000000 pywayne-1.0.0.3.9/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7353 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6904 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-05-15 07:59:08.559014 pywayne-1.0.0.3.9/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)      951 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      305 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      133 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2023-05-15 07:59:08.559414 pywayne-1.0.0.3.9/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1409 2023-05-15 07:58:46.000000 pywayne-1.0.0.3.9/setup.py
```

### Comparing `pywayne-1.0.0.3.8/LICENSE` & `pywayne-1.0.0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.8/PKG-INFO` & `pywayne-1.0.0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.3.8
+Version: 1.0.0.3.9
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,16 +16,14 @@
 
 ## Currently includes:
 - data-structure
 - dsp
 - gui
 - math
 - tools
-- tt_api
-- ocs_api
 
 # Installation
 Try to run "pip install pywayne" in your commond line tool.
 
 # How to use
 from pywayne.tools import *
```

### Comparing `pywayne-1.0.0.3.8/pywayne/data_structure.py` & `pywayne-1.0.0.3.9/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.8/pywayne/dsp.py` & `pywayne-1.0.0.3.9/pywayne/dsp.py`

 * *Files 3% similar despite different names*

```diff
@@ -371,14 +371,45 @@
             cutoff = self._mincutoff + self._beta * abs(self._dx)
             self._alpha = self._alpha(cutoff)
             result = self._val + self._alpha * (val - self._val)
         self._val = result
         return result
 
 
+class CalcEnergy:
+    def __init__(self, alpha=10, beta=20, gamma=1):
+        """
+        Calculate energy of given signal
+        :param alpha: local mean window
+        :param beta: remote diff window
+        :param gamma: power of energy, currently set to 1
+        """
+        self.alpha = alpha
+        self.beta = beta
+        self.gamma = gamma
+
+    def apply(self, data: np.ndarray):
+        """
+        Apply energy calculator w.r.t. input data
+        :param data: N*d input array
+        :return: N*d energy
+        """
+        if len(data.shape) == 1:
+            data = data.reshape((-1, 1))
+        energy = np.vstack((
+            np.zeros((self.alpha + self.beta - 1, data.shape[1])),
+            np.apply_along_axis(
+                lambda x: np.convolve(np.abs(x), np.ones(self.alpha) / self.alpha, 'valid'),
+                0,
+                data[self.beta:] - data[:-self.beta]
+            )
+        ))
+        return energy
+
+
 class CurveSimilarity:
     """
     用于计算曲线x和曲线y的相似度
 
     Author:   wangye
     Datetime: 2019/6/24 23:17
```

### Comparing `pywayne-1.0.0.3.8/pywayne/gui.py` & `pywayne-1.0.0.3.9/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.8/pywayne/math.py` & `pywayne-1.0.0.3.9/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.8/pywayne/plot.py` & `pywayne-1.0.0.3.9/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.8/pywayne/tools.py` & `pywayne-1.0.0.3.9/pywayne/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.8/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.3.9/pywayne.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.3.8
+Version: 1.0.0.3.9
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,16 +16,14 @@
 
 ## Currently includes:
 - data-structure
 - dsp
 - gui
 - math
 - tools
-- tt_api
-- ocs_api
 
 # Installation
 Try to run "pip install pywayne" in your commond line tool.
 
 # How to use
 from pywayne.tools import *
```

### Comparing `pywayne-1.0.0.3.8/setup.py` & `pywayne-1.0.0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return [line for line in lineiter if line and not line.startswith("#") and not line.startswith("~")]
 
 
 install_reqs = parse_requirements('requirements.txt')
 
 setuptools.setup(
     name="pywayne",
-    version="1.0.0.3.8",
+    version="1.0.0.3.9",
     author="Wayne",
     author_email="wang121ye@hotmail.com",
     description="Some useful tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wangyendt/wangye_algorithm_lib",
     classifiers=[
```

