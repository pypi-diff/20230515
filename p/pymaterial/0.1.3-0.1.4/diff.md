# Comparing `tmp/pymaterial-0.1.3.tar.gz` & `tmp/pymaterial-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymaterial-0.1.3.tar", last modified: Thu Mar 30 15:08:34 2023, max compression
+gzip compressed data, was "pymaterial-0.1.4.tar", last modified: Mon May 15 11:10:36 2023, max compression
```

## Comparing `pymaterial-0.1.3.tar` & `pymaterial-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1086 2023-03-30 15:08:15.738788 pymaterial-0.1.3/LICENSE
--rw-r--r--   0        0        0     1414 2023-03-30 15:08:15.738788 pymaterial-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.738788 pymaterial-0.1.3/pymaterial/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.738788 pymaterial-0.1.3/pymaterial/combis/__init__.py
--rw-r--r--   0        0        0       28 2023-03-30 15:08:15.738788 pymaterial-0.1.3/pymaterial/combis/clt/README.md
--rw-r--r--   0        0        0       66 2023-03-30 15:08:15.738788 pymaterial-0.1.3/pymaterial/combis/clt/__init__.py
--rw-r--r--   0        0        0     5110 2023-03-30 15:08:15.738788 pymaterial-0.1.3/pymaterial/combis/clt/ply.py
--rw-r--r--   0        0        0    12527 2023-03-30 15:08:15.738788 pymaterial-0.1.3/pymaterial/combis/clt/stackup.py
--rw-r--r--   0        0        0      172 2023-03-30 15:08:15.738788 pymaterial-0.1.3/pymaterial/failures/__init__.py
--rw-r--r--   0        0        0     3284 2023-03-30 15:08:15.738788 pymaterial-0.1.3/pymaterial/failures/cuntze.py
--rw-r--r--   0        0        0     1208 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/failures/ifailure.py
--rw-r--r--   0        0        0     3160 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/failures/maxstress.py
--rw-r--r--   0        0        0     2087 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/failures/mises.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/failures/puck.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/failures/tsai_hill.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/failures/tsai_wu.py
--rw-r--r--   0        0        0      139 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/library/README.md
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/library/__init__.py
--rw-r--r--   0        0        0      268 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/materials/__init__.py
--rw-r--r--   0        0        0      518 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/materials/anisotropic.py
--rw-r--r--   0        0        0      987 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/materials/isotropic.py
--rw-r--r--   0        0        0     1978 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/materials/material.py
--rw-r--r--   0        0        0     1500 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/materials/orthotropic.py
--rw-r--r--   0        0        0     1683 2023-03-30 15:08:15.742788 pymaterial-0.1.3/pymaterial/materials/transversely_isotropic.py
--rw-r--r--   0        0        0      693 2023-03-30 15:08:34.782757 pymaterial-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/combis/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/combis/clt/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/combis/clt/test_ply.py
--rw-r--r--   0        0        0     5684 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/combis/clt/test_stackup.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/failures/__init__.py
--rw-r--r--   0        0        0      461 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/failures/test_cuntze.py
--rw-r--r--   0        0        0     1825 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/failures/test_max_stress.py
--rw-r--r--   0        0        0     1180 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/failures/test_mises.py
--rw-r--r--   0        0        0        0 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/materials/__init__.py
--rw-r--r--   0        0        0      930 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/materials/test_isotropic.py
--rw-r--r--   0        0        0      651 2023-03-30 15:08:15.742788 pymaterial-0.1.3/tests/materials/test_orthotropic.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 pymaterial-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-15 11:10:17.722280 pymaterial-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1414 2023-05-15 11:10:17.722280 pymaterial-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.722280 pymaterial-0.1.4/pymaterial/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.722280 pymaterial-0.1.4/pymaterial/combis/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/combis/clt/README.md
+-rw-r--r--   0        0        0       66 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/combis/clt/__init__.py
+-rw-r--r--   0        0        0     5110 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/combis/clt/ply.py
+-rw-r--r--   0        0        0    12527 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/combis/clt/stackup.py
+-rw-r--r--   0        0        0      172 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/failures/__init__.py
+-rw-r--r--   0        0        0     3284 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/failures/cuntze.py
+-rw-r--r--   0        0        0     1208 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/failures/ifailure.py
+-rw-r--r--   0        0        0     3160 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/failures/maxstress.py
+-rw-r--r--   0        0        0     2087 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/failures/mises.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/failures/puck.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/failures/tsai_hill.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/failures/tsai_wu.py
+-rw-r--r--   0        0        0      139 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/library/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/library/__init__.py
+-rw-r--r--   0        0        0      268 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/materials/__init__.py
+-rw-r--r--   0        0        0      518 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/materials/anisotropic.py
+-rw-r--r--   0        0        0      987 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/materials/isotropic.py
+-rw-r--r--   0        0        0     1978 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/materials/material.py
+-rw-r--r--   0        0        0     1500 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/materials/orthotropic.py
+-rw-r--r--   0        0        0     1683 2023-05-15 11:10:17.726280 pymaterial-0.1.4/pymaterial/materials/transversely_isotropic.py
+-rw-r--r--   0        0        0      693 2023-05-15 11:10:36.150643 pymaterial-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/combis/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/combis/clt/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/combis/clt/test_ply.py
+-rw-r--r--   0        0        0     5684 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/combis/clt/test_stackup.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/failures/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/failures/test_cuntze.py
+-rw-r--r--   0        0        0     1825 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/failures/test_max_stress.py
+-rw-r--r--   0        0        0     1180 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/failures/test_mises.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/materials/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/materials/test_isotropic.py
+-rw-r--r--   0        0        0      651 2023-05-15 11:10:17.726280 pymaterial-0.1.4/tests/materials/test_orthotropic.py
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 pymaterial-0.1.4/PKG-INFO
```

### Comparing `pymaterial-0.1.3/LICENSE` & `pymaterial-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/README.md` & `pymaterial-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/combis/clt/ply.py` & `pymaterial-0.1.4/pymaterial/combis/clt/ply.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/combis/clt/stackup.py` & `pymaterial-0.1.4/pymaterial/combis/clt/stackup.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/failures/cuntze.py` & `pymaterial-0.1.4/pymaterial/failures/cuntze.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/failures/ifailure.py` & `pymaterial-0.1.4/pymaterial/failures/ifailure.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/failures/maxstress.py` & `pymaterial-0.1.4/pymaterial/failures/maxstress.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/failures/mises.py` & `pymaterial-0.1.4/pymaterial/failures/mises.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/materials/anisotropic.py` & `pymaterial-0.1.4/pymaterial/materials/anisotropic.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/materials/isotropic.py` & `pymaterial-0.1.4/pymaterial/materials/isotropic.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/materials/material.py` & `pymaterial-0.1.4/pymaterial/materials/material.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/materials/orthotropic.py` & `pymaterial-0.1.4/pymaterial/materials/orthotropic.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pymaterial/materials/transversely_isotropic.py` & `pymaterial-0.1.4/pymaterial/materials/transversely_isotropic.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/pyproject.toml` & `pymaterial-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 test = [
     "pytest>=7.2.1",
     "pytest-cov>=4.0.0",
 ]
 
 [project]
 name = "pymaterial"
-version = "0.1.3"
+version = "0.1.4"
 description = "pyMaterial, library for material and failure modeling."
 authors = [
     { name = "Willi Zschiebsch", email = "willi.zschiebsch@gmail.com" },
 ]
 dependencies = [
     "numpy>=1.24.1",
 ]
```

### Comparing `pymaterial-0.1.3/tests/combis/clt/test_stackup.py` & `pymaterial-0.1.4/tests/combis/clt/test_stackup.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/tests/failures/test_max_stress.py` & `pymaterial-0.1.4/tests/failures/test_max_stress.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/tests/failures/test_mises.py` & `pymaterial-0.1.4/tests/failures/test_mises.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/tests/materials/test_isotropic.py` & `pymaterial-0.1.4/tests/materials/test_isotropic.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/tests/materials/test_orthotropic.py` & `pymaterial-0.1.4/tests/materials/test_orthotropic.py`

 * *Files identical despite different names*

### Comparing `pymaterial-0.1.3/PKG-INFO` & `pymaterial-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymaterial
-Version: 0.1.3
+Version: 0.1.4
 Summary: pyMaterial, library for material and failure modeling.
 Author-Email: Willi Zschiebsch <willi.zschiebsch@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/Modular-Design/pyMaterial
 Project-URL: Issues, https://github.com/Modular-Design/pyMaterial/issues
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.24.1
```

