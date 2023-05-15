# Comparing `tmp/RlEvaluation-0.1.0.tar.gz` & `tmp/RlEvaluation-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RlEvaluation-0.1.0.tar", last modified: Mon May 15 21:07:06 2023, max compression
+gzip compressed data, was "RlEvaluation-0.1.1.tar", last modified: Mon May 15 21:26:02 2023, max compression
```

## Comparing `RlEvaluation-0.1.0.tar` & `RlEvaluation-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/README.md
--rw-r--r--   0        0        0     2991 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/ResultData.py
--rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/__init__.py
--rw-r--r--   0        0        0     2175 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/data.py
--rw-r--r--   0        0        0     1229 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/jit.py
--rw-r--r--   0        0        0       62 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/logging.py
--rw-r--r--   0        0        0      257 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/numba.py
--rw-r--r--   0        0        0     1052 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/hypers.py
--rw-r--r--   0        0        0     1192 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/intervals.py
--rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/py.typed
--rw-r--r--   0        0        0      358 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/temporal.py
--rw-r--r--   0        0        0      658 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/tools.py
--rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/utils/__init__.py
--rw-r--r--   0        0        0      140 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/utils/math.py
--rw-r--r--   0        0        0      831 2023-05-15 21:07:03.756936 RlEvaluation-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/_utils/__init__.py
--rw-r--r--   0        0        0     2164 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/_utils/test_data.py
--rw-r--r--   0        0        0      404 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/test_hypers.py
--rw-r--r--   0        0        0      716 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/test_utils/mock_data.py
--rw-r--r--   0        0        0      188 1970-01-01 00:00:00.000000 RlEvaluation-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/README.md
+-rw-r--r--   0        0        0     3064 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/ResultData.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/_utils/__init__.py
+-rw-r--r--   0        0        0     2175 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/_utils/data.py
+-rw-r--r--   0        0        0     1229 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/_utils/jit.py
+-rw-r--r--   0        0        0       62 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/_utils/logging.py
+-rw-r--r--   0        0        0      257 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/_utils/numba.py
+-rw-r--r--   0        0        0     1052 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/hypers.py
+-rw-r--r--   0        0        0     1192 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/intervals.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/py.typed
+-rw-r--r--   0        0        0      358 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/temporal.py
+-rw-r--r--   0        0        0      658 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/tools.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/utils/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/RlEvaluation/utils/math.py
+-rw-r--r--   0        0        0      831 2023-05-15 21:25:59.844978 RlEvaluation-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/tests/_utils/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/tests/_utils/test_data.py
+-rw-r--r--   0        0        0      404 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/tests/test_hypers.py
+-rw-r--r--   0        0        0      716 2023-05-15 21:25:27.868839 RlEvaluation-0.1.1/tests/test_utils/mock_data.py
+-rw-r--r--   0        0        0      188 1970-01-01 00:00:00.000000 RlEvaluation-0.1.1/PKG-INFO
```

### Comparing `RlEvaluation-0.1.0/RlEvaluation/ResultData.py` & `RlEvaluation-0.1.1/RlEvaluation/ResultData.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,17 @@
         return Hypers.select_best_hypers(self._data, f'{metric}.summary', pref, statistic)
 
     def get_learning_curve(self, metric: str, idx: int):
         data = self._data[metric].iloc[idx]
         data = np.asarray(data)
         return Intervals.bootstrap(data)
 
+    def get_at_idx(self, idx: int):
+        return self._data.iloc[idx]
+
     # --------------
     # -- Internal --
     # --------------
     def _prep_data(self):
         # if not wide format, then convert
         self._data = du.make_wide_format(self._data, self._hypers, self._metrics, self._run)
```

### Comparing `RlEvaluation-0.1.0/RlEvaluation/_utils/data.py` & `RlEvaluation-0.1.1/RlEvaluation/_utils/data.py`

 * *Files identical despite different names*

### Comparing `RlEvaluation-0.1.0/RlEvaluation/_utils/jit.py` & `RlEvaluation-0.1.1/RlEvaluation/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `RlEvaluation-0.1.0/RlEvaluation/hypers.py` & `RlEvaluation-0.1.1/RlEvaluation/hypers.py`

 * *Files identical despite different names*

### Comparing `RlEvaluation-0.1.0/RlEvaluation/intervals.py` & `RlEvaluation-0.1.1/RlEvaluation/intervals.py`

 * *Files identical despite different names*

### Comparing `RlEvaluation-0.1.0/RlEvaluation/tools.py` & `RlEvaluation-0.1.1/RlEvaluation/tools.py`

 * *Files identical despite different names*

### Comparing `RlEvaluation-0.1.0/pyproject.toml` & `RlEvaluation-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.0"
+version = "0.1.1"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -23,15 +23,15 @@
 
 [tool.mypy]
 mypy_path = "typings"
 ignore_missing_imports = true
 
 [project]
 name = "RlEvaluation"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "pandas>=1.5.3",
     "numba>=0.57.0",
```

### Comparing `RlEvaluation-0.1.0/tests/_utils/test_data.py` & `RlEvaluation-0.1.1/tests/_utils/test_data.py`

 * *Files identical despite different names*

### Comparing `RlEvaluation-0.1.0/tests/test_utils/mock_data.py` & `RlEvaluation-0.1.1/tests/test_utils/mock_data.py`

 * *Files identical despite different names*

