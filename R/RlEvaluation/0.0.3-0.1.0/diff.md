# Comparing `tmp/RlEvaluation-0.0.3.tar.gz` & `tmp/RlEvaluation-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RlEvaluation-0.0.3.tar", last modified: Fri Mar  3 17:16:02 2023, max compression
+gzip compressed data, was "RlEvaluation-0.1.0.tar", last modified: Mon May 15 21:07:06 2023, max compression
```

## Comparing `RlEvaluation-0.0.3.tar` & `RlEvaluation-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0        0 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/_utils/__init__.py
--rw-r--r--   0        0        0      969 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/_utils/data.py
--rw-r--r--   0        0        0     1229 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/_utils/jit.py
--rw-r--r--   0        0        0      257 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/_utils/numba.py
--rw-r--r--   0        0        0     1055 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/hypers.py
--rw-r--r--   0        0        0     1238 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/intervals.py
--rw-r--r--   0        0        0        0 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/py.typed
--rw-r--r--   0        0        0      658 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/tools.py
--rw-r--r--   0        0        0        0 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/utils/__init__.py
--rw-r--r--   0        0        0      140 2023-03-03 17:15:22.077054 RlEvaluation-0.0.3/RlEvaluation/utils/math.py
--rw-r--r--   0        0        0      830 2023-03-03 17:16:00.901348 RlEvaluation-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-03 17:15:22.081054 RlEvaluation-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 17:15:22.081054 RlEvaluation-0.0.3/tests/_utils/__init__.py
--rw-r--r--   0        0        0      828 2023-03-03 17:15:22.081054 RlEvaluation-0.0.3/tests/_utils/test_data.py
--rw-r--r--   0        0        0      578 2023-03-03 17:15:22.081054 RlEvaluation-0.0.3/tests/test_hypers.py
--rw-r--r--   0        0        0      306 2023-03-03 17:15:22.081054 RlEvaluation-0.0.3/tests/test_utils/mock_data.py
--rw-r--r--   0        0        0      187 1970-01-01 00:00:00.000000 RlEvaluation-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/README.md
+-rw-r--r--   0        0        0     2991 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/ResultData.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/__init__.py
+-rw-r--r--   0        0        0     2175 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/data.py
+-rw-r--r--   0        0        0     1229 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/jit.py
+-rw-r--r--   0        0        0       62 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/logging.py
+-rw-r--r--   0        0        0      257 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/_utils/numba.py
+-rw-r--r--   0        0        0     1052 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/hypers.py
+-rw-r--r--   0        0        0     1192 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/intervals.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/py.typed
+-rw-r--r--   0        0        0      358 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/temporal.py
+-rw-r--r--   0        0        0      658 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/tools.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/utils/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-15 21:06:20.892501 RlEvaluation-0.1.0/RlEvaluation/utils/math.py
+-rw-r--r--   0        0        0      831 2023-05-15 21:07:03.756936 RlEvaluation-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/_utils/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/_utils/test_data.py
+-rw-r--r--   0        0        0      404 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/test_hypers.py
+-rw-r--r--   0        0        0      716 2023-05-15 21:06:20.896502 RlEvaluation-0.1.0/tests/test_utils/mock_data.py
+-rw-r--r--   0        0        0      188 1970-01-01 00:00:00.000000 RlEvaluation-0.1.0/PKG-INFO
```

### Comparing `RlEvaluation-0.0.3/RlEvaluation/_utils/jit.py` & `RlEvaluation-0.1.0/RlEvaluation/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `RlEvaluation-0.0.3/RlEvaluation/hypers.py` & `RlEvaluation-0.1.0/RlEvaluation/hypers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import pandas as pd
 import enum
-from typing import cast, Any
 from RlEvaluation._utils.numba import over_first_axis
-from RlEvaluation._utils.data import Reducer, normalizeDataType
+from RlEvaluation._utils.data import Reducer, normalizeDataType, compileReducer
 from RlEvaluation.utils.math import mean
 from RlEvaluation.tools import subsetDF
 
 class Preference(enum.Enum):
     high = 'high'
     low = 'low'
 
-def selectBestHypers(df: pd.DataFrame, column: str, prefer: Preference, reducer: Reducer = mean):
-    f = cast(Any, reducer)
+def select_best_hypers(df: pd.DataFrame, column: str, prefer: Preference, reducer: Reducer = mean):
+    f = compileReducer(reducer)
     data = normalizeDataType(df, 2, col=column)
     # TODO: report uncertainty in hyper selection
     reduced = over_first_axis(data, f)
 
     if prefer == Preference.high:
         best_idx = reduced.argmax()
     elif prefer == Preference.low:
         best_idx = reduced.argmin()
     else:
         raise UnknownPreferenceException()
 
-    return df.iloc[[int(best_idx)]]
+    idx = int(best_idx)
+    return idx
 
 def sliceOverHyper(df: pd.DataFrame, hyper: str):
     values = df[hyper].unique()
 
     for v in values:
         sub = subsetDF(df, { hyper: v })
         yield v, sub.reset_index()
```

### Comparing `RlEvaluation-0.0.3/RlEvaluation/intervals.py` & `RlEvaluation-0.1.0/RlEvaluation/intervals.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import numpy as np
 from numba import prange
-from RlEvaluation._utils.data import normalizeDataType, compileReducer, Data, Reducer
+from RlEvaluation._utils.data import compileReducer, Reducer
 from RlEvaluation._utils.jit import try2pjit
 
 RandomState = np.random.RandomState
 
-def bootstrap(data: Data, column: str = '', statistic: Reducer = np.mean, coverage: float = 0.95, bootstraps: int = 10000, rng: RandomState = RandomState()):
-    data = normalizeDataType(data, dims=2, col=column)
+def bootstrap(data: np.ndarray, statistic: Reducer = np.mean, coverage: float = 0.95, bootstraps: int = 2000, rng: np.random.Generator | None = None):
+    rng = rng or np.random.default_rng()
+    assert data.ndim == 2
 
     return _bootstrap(
         data=data,
         statistic=compileReducer(statistic),
         coverage=coverage,
         bootstraps=bootstraps,
-        seed=rng.randint(2**32),
+        rng=rng,
     )
 
 @try2pjit
-def _bootstrap(data: np.ndarray, statistic: Reducer, coverage: float, bootstraps: int, seed: int):
-    np.random.seed(seed)
+def _bootstrap(data: np.ndarray, statistic: Reducer, coverage: float, bootstraps: int, rng: np.random.Generator):
     samples, measurements = data.shape
 
     alpha = (1 - coverage) / 2
 
     out = np.empty((3, measurements))
     for i in prange(measurements):
         bs = np.empty(bootstraps)
```

### Comparing `RlEvaluation-0.0.3/RlEvaluation/tools.py` & `RlEvaluation-0.1.0/RlEvaluation/tools.py`

 * *Files identical despite different names*

### Comparing `RlEvaluation-0.0.3/pyproject.toml` & `RlEvaluation-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.3"
+version = "0.1.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -23,25 +23,25 @@
 
 [tool.mypy]
 mypy_path = "typings"
 ignore_missing_imports = true
 
 [project]
 name = "RlEvaluation"
-version = "0.0.3"
+version = "0.1.0"
 description = ""
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "pandas>=1.5.3",
-    "numba>=0.56.4",
+    "numba>=0.57.0",
     "numpy>=1.23.5",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

