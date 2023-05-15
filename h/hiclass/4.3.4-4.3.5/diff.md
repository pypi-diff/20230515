# Comparing `tmp/hiclass-4.3.4.tar.gz` & `tmp/hiclass-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiclass-4.3.4.tar", last modified: Wed May 10 09:19:16 2023, max compression
+gzip compressed data, was "hiclass-4.3.5.tar", last modified: Mon May 15 13:36:43 2023, max compression
```

## Comparing `hiclass-4.3.4.tar` & `hiclass-4.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:19:16.039438 hiclass-4.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-10 09:18:52.000000 hiclass-4.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 09:18:52.000000 hiclass-4.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-05-10 09:19:16.039438 hiclass-4.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14300 2023-05-10 09:18:52.000000 hiclass-4.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:19:16.039438 hiclass-4.3.4/hiclass/
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/BinaryPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/ConstantClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/HierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/LocalClassifierPerLevel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/LocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/LocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 09:19:16.039438 hiclass-4.3.4/hiclass/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:19:16.039438 hiclass-4.3.4/hiclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-10 09:19:16.039438 hiclass-4.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-10 09:18:52.000000 hiclass-4.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:19:16.039438 hiclass-4.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_BinaryPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_ConstantClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_HierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_LocalClassifierPerLevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_LocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_LocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-05-10 09:18:52.000000 hiclass-4.3.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:43.385334 hiclass-4.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-15 13:36:12.000000 hiclass-4.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 13:36:12.000000 hiclass-4.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-05-15 13:36:43.385334 hiclass-4.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14300 2023-05-15 13:36:12.000000 hiclass-4.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:43.385334 hiclass-4.3.5/hiclass/
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-15 13:36:12.000000 hiclass-4.3.5/hiclass/BinaryPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-15 13:36:12.000000 hiclass-4.3.5/hiclass/ConstantClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-05-15 13:36:12.000000 hiclass-4.3.5/hiclass/HierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-15 13:36:12.000000 hiclass-4.3.5/hiclass/LocalClassifierPerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-15 13:36:12.000000 hiclass-4.3.5/hiclass/LocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-15 13:36:12.000000 hiclass-4.3.5/hiclass/LocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-15 13:36:12.000000 hiclass-4.3.5/hiclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-15 13:36:43.385334 hiclass-4.3.5/hiclass/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-15 13:36:12.000000 hiclass-4.3.5/hiclass/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:43.381334 hiclass-4.3.5/hiclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-05-15 13:36:43.000000 hiclass-4.3.5/hiclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-15 13:36:43.000000 hiclass-4.3.5/hiclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:36:43.000000 hiclass-4.3.5/hiclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 13:36:43.000000 hiclass-4.3.5/hiclass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 13:36:43.000000 hiclass-4.3.5/hiclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 13:36:43.000000 hiclass-4.3.5/hiclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-15 13:36:43.385334 hiclass-4.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-15 13:36:12.000000 hiclass-4.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:36:43.385334 hiclass-4.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-05-15 13:36:12.000000 hiclass-4.3.5/tests/test_BinaryPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-15 13:36:12.000000 hiclass-4.3.5/tests/test_ConstantClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-15 13:36:12.000000 hiclass-4.3.5/tests/test_HierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-15 13:36:12.000000 hiclass-4.3.5/tests/test_LocalClassifierPerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-15 13:36:12.000000 hiclass-4.3.5/tests/test_LocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-15 13:36:12.000000 hiclass-4.3.5/tests/test_LocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-15 13:36:12.000000 hiclass-4.3.5/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-05-15 13:36:12.000000 hiclass-4.3.5/versioneer.py
```

### Comparing `hiclass-4.3.4/LICENSE` & `hiclass-4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/PKG-INFO` & `hiclass-4.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclass
-Version: 4.3.4
+Version: 4.3.5
 Summary: Hierarchical Classification Library.
 Author: Fabio Malcher Miranda, Niklas Koehnecke
 Author-email: fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/hiclass/issues
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/hiclass
 Project-URL: Related Software, https://gitlab.com/dacs-hpi
```

### Comparing `hiclass-4.3.4/README.md` & `hiclass-4.3.5/README.md`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/hiclass/BinaryPolicy.py` & `hiclass-4.3.5/hiclass/BinaryPolicy.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/hiclass/ConstantClassifier.py` & `hiclass-4.3.5/hiclass/ConstantClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/hiclass/HierarchicalClassifier.py` & `hiclass-4.3.5/hiclass/HierarchicalClassifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     array([['a', ''],
        ['b', 'c']])
     """
     try:
         depth = max([len(row) for row in y])
     except TypeError:
         return y
-    y = np.array(y)
+    y = np.array(y, dtype=object)
     leveled_y = [[i for i in row] + [""] * (depth - len(row)) for row in y]
     return np.array(leveled_y)
 
 
 class HierarchicalClassifier(abc.ABC):
     """Abstract class for the local hierarchical classifiers.
```

### Comparing `hiclass-4.3.4/hiclass/LocalClassifierPerLevel.py` & `hiclass-4.3.5/hiclass/LocalClassifierPerLevel.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/hiclass/LocalClassifierPerNode.py` & `hiclass-4.3.5/hiclass/LocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/hiclass/LocalClassifierPerParentNode.py` & `hiclass-4.3.5/hiclass/LocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/hiclass/metrics.py` & `hiclass-4.3.5/hiclass/metrics.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/hiclass.egg-info/PKG-INFO` & `hiclass-4.3.5/hiclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclass
-Version: 4.3.4
+Version: 4.3.5
 Summary: Hierarchical Classification Library.
 Author: Fabio Malcher Miranda, Niklas Koehnecke
 Author-email: fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/hiclass/issues
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/hiclass
 Project-URL: Related Software, https://gitlab.com/dacs-hpi
```

### Comparing `hiclass-4.3.4/hiclass.egg-info/SOURCES.txt` & `hiclass-4.3.5/hiclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/setup.py` & `hiclass-4.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 URL_ISSUES = "https://github.com/scikit-learn-contrib/hiclass/issues"
 EMAIL = "fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de"
 AUTHOR = "Fabio Malcher Miranda, Niklas Koehnecke"
 REQUIRES_PYTHON = ">=3.7,<3.11"
 KEYWORDS = ["hierarchical classification"]
 DACS_SOFTWARE = "https://gitlab.com/dacs-hpi"
 # What packages are required for this module to be executed?
-REQUIRED = ["networkx", "numpy<1.24", "scikit-learn"]
+REQUIRED = ["networkx", "numpy", "scikit-learn"]
 
 # What packages are optional?
 # 'fancy feature': ['django'],}
 EXTRAS = {"ray": ["ray>=1.11.0"]}
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
```

### Comparing `hiclass-4.3.4/tests/test_BinaryPolicy.py` & `hiclass-4.3.5/tests/test_BinaryPolicy.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/tests/test_ConstantClassifier.py` & `hiclass-4.3.5/tests/test_ConstantClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/tests/test_HierarchicalClassifier.py` & `hiclass-4.3.5/tests/test_HierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.4/tests/test_LocalClassifierPerLevel.py` & `hiclass-4.3.5/tests/test_LocalClassifierPerLevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,19 +151,22 @@
 @pytest.fixture
 def empty_levels():
     X = [
         [1],
         [2],
         [3],
     ]
-    y = [
-        ["1"],
-        ["2", "2.1"],
-        ["3", "3.1", "3.1.2"],
-    ]
+    y = np.array(
+        [
+            ["1"],
+            ["2", "2.1"],
+            ["3", "3.1", "3.1.2"],
+        ],
+        dtype=object,
+    )
     return X, y
 
 
 def test_empty_levels(empty_levels):
     lcppn = LocalClassifierPerLevel()
     X, y = empty_levels
     lcppn.fit(X, y)
```

### Comparing `hiclass-4.3.4/tests/test_LocalClassifierPerNode.py` & `hiclass-4.3.5/tests/test_LocalClassifierPerNode.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,19 +212,22 @@
 @pytest.fixture
 def empty_levels():
     X = [
         [1],
         [2],
         [3],
     ]
-    y = [
-        ["1"],
-        ["2", "2.1"],
-        ["3", "3.1", "3.1.2"],
-    ]
+    y = np.array(
+        [
+            ["1"],
+            ["2", "2.1"],
+            ["3", "3.1", "3.1.2"],
+        ],
+        dtype=object,
+    )
     return X, y
 
 
 def test_empty_levels(empty_levels):
     lcppn = LocalClassifierPerNode()
     X, y = empty_levels
     lcppn.fit(X, y)
```

### Comparing `hiclass-4.3.4/tests/test_LocalClassifierPerParentNode.py` & `hiclass-4.3.5/tests/test_LocalClassifierPerParentNode.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,15 +145,22 @@
     assert weights is None
 
 
 @pytest.fixture
 def fitted_logistic_regression():
     digraph = LocalClassifierPerParentNode(local_classifier=LogisticRegression())
     digraph.hierarchy_ = nx.DiGraph(
-        [("r", "1"), ("r", "2"), ("1", "1.1"), ("1", "1.2"), ("2", "2.1"), ("2", "2.2")]
+        [
+            ("r", "1"),
+            ("r", "2"),
+            ("1", "1.1"),
+            ("1", "1.2"),
+            ("2", "2.1"),
+            ("2", "2.2"),
+        ]
     )
     digraph.y_ = np.array([["1", "1.1"], ["1", "1.2"], ["2", "2.1"], ["2", "2.2"]])
     digraph.X_ = np.array([[1, 2], [3, 4], [5, 6], [7, 8]])
     digraph.logger_ = logging.getLogger("LCPPN")
     digraph.max_levels_ = 2
     digraph.dtype_ = "<U3"
     digraph.root_ = "r"
@@ -196,19 +203,22 @@
 @pytest.fixture
 def empty_levels():
     X = [
         [1],
         [2],
         [3],
     ]
-    y = [
-        ["1"],
-        ["2", "2.1"],
-        ["3", "3.1", "3.1.2"],
-    ]
+    y = np.array(
+        [
+            ["1"],
+            ["2", "2.1"],
+            ["3", "3.1", "3.1.2"],
+        ],
+        dtype=object,
+    )
     return X, y
 
 
 def test_empty_levels(empty_levels):
     lcppn = LocalClassifierPerParentNode()
     X, y = empty_levels
     lcppn.fit(X, y)
```

### Comparing `hiclass-4.3.4/tests/test_metrics.py` & `hiclass-4.3.5/tests/test_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 def test_f1():
     y_true = np.array([[1, 2, 3, 4], [1, 2, 5, 6]])
     y_pred = np.array([[1, 2, 5, 6], [1, 2, 3, 4]])
     assert metrics.f1(y_true, y_pred) == 0.5
 
 
 def test_empty_levels_1():
-    y_true = np.array([["2", "3"], ["1"], ["4", "5", "6"]])
-    y_pred = np.array([["1", "", ""], ["2", "3", ""], ["4", "5", "6"]])
+    y_true = np.array([["2", "3"], ["1"], ["4", "5", "6"]], dtype=object)
+    y_pred = np.array([["1", "", ""], ["2", "3", ""], ["4", "5", "6"]], dtype=object)
     assert metrics.f1(y_true, y_pred) == 0.5
     assert metrics.f1(y_true, y_true) == 1
 
 
 def test_empty_levels_2():
-    y_true = np.array([["1"], ["2", "3"], ["4", "5", "6"]])
-    y_pred = np.array([["1", "", ""], ["2", "3", ""], ["4", "5", "6"]])
+    y_true = np.array([["1"], ["2", "3"], ["4", "5", "6"]], dtype=object)
+    y_pred = np.array([["1", "", ""], ["2", "3", ""], ["4", "5", "6"]], dtype=object)
     assert metrics.f1(y_true, y_pred) == 1
     assert metrics.f1(y_true, y_true) == 1
```

### Comparing `hiclass-4.3.4/versioneer.py` & `hiclass-4.3.5/versioneer.py`

 * *Files identical despite different names*

