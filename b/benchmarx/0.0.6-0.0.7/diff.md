# Comparing `tmp/benchmarx-0.0.6-py3-none-any.whl.zip` & `tmp/benchmarx-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 22961 bytes, number of entries: 22
+Zip file size: 22972 bytes, number of entries: 22
 -rw-r--r--  2.0 unx    11189 b- defN 23-May-14 18:00 src/NeuralNetworkTraining.py
 -rw-r--r--  2.0 unx     1543 b- defN 23-May-12 12:42 src/ProxGD_custom_linesearch.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-14 21:58 src/__init__.py
 -rw-r--r--  2.0 unx    21138 b- defN 23-May-14 18:10 src/benchmark.py
 -rw-r--r--  2.0 unx     5271 b- defN 23-May-14 17:55 src/benchmark_result.py
 -rw-r--r--  2.0 unx     1333 b- defN 23-Apr-27 19:34 src/custom_optimizer.py
 -rw-r--r--  2.0 unx       46 b- defN 23-Apr-30 18:47 src/defaults.py
@@ -12,13 +12,13 @@
 -rw-r--r--  2.0 unx     1212 b- defN 23-May-14 17:54 src/metrics.py
 -rw-r--r--  2.0 unx    20912 b- defN 23-May-14 21:08 src/plotter.py
 -rw-r--r--  2.0 unx      779 b- defN 23-May-13 20:00 src/problem.py
 -rw-r--r--  2.0 unx     1402 b- defN 23-May-13 20:35 src/qadratic_problem_real_data.py
 -rw-r--r--  2.0 unx     1916 b- defN 23-May-12 13:01 src/quadratic_problem.py
 -rw-r--r--  2.0 unx      831 b- defN 23-May-13 19:39 src/rastrigin.py
 -rw-r--r--  2.0 unx      810 b- defN 23-May-13 19:40 src/rosenbrock.py
--rw-r--r--  2.0 unx     1074 b- defN 23-May-14 22:05 benchmarx-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      881 b- defN 23-May-14 22:05 benchmarx-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 22:05 benchmarx-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-14 22:05 benchmarx-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1691 b- defN 23-May-14 22:05 benchmarx-0.0.6.dist-info/RECORD
-22 files, 76950 bytes uncompressed, 20261 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx     1074 b- defN 23-May-14 22:10 benchmarx-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      881 b- defN 23-May-14 22:10 benchmarx-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 22:10 benchmarx-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-14 22:10 benchmarx-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1692 b- defN 23-May-14 22:10 benchmarx-0.0.7.dist-info/RECORD
+22 files, 76961 bytes uncompressed, 20272 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: src/rastrigin.py
 Comment: 
 
 Filename: src/rosenbrock.py
 Comment: 
 
-Filename: benchmarx-0.0.6.dist-info/LICENSE
+Filename: benchmarx-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: benchmarx-0.0.6.dist-info/METADATA
+Filename: benchmarx-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: benchmarx-0.0.6.dist-info/WHEEL
+Filename: benchmarx-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: benchmarx-0.0.6.dist-info/top_level.txt
+Filename: benchmarx-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: benchmarx-0.0.6.dist-info/RECORD
+Filename: benchmarx-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `benchmarx-0.0.6.dist-info/LICENSE` & `benchmarx-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `benchmarx-0.0.6.dist-info/METADATA` & `benchmarx-0.0.7.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmarx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools for benchmarking optimization methods
 Home-page: https://github.com/AlexToW/benchmarx
 Author: AlexToW
 Author-email: Salex <31salex31@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AlexToW/benchmarx
 Project-URL: Bug Tracker, https://github.com/AlexToW/benchmarx/issues
```

## Comparing `benchmarx-0.0.6.dist-info/RECORD` & `benchmarx-0.0.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 src/metrics.py,sha256=y3PTp4d1HrOhnK5euAxL1k-p-bzfXk25Kh2Kj0gYR-0,1212
 src/plotter.py,sha256=DiLxAIQ3b1l7-iNPftkkJDQOu_-aGtKXT6c-NRK4Pmg,20912
 src/problem.py,sha256=zKPzjgh3Wp7Z_q-wfjePELq6khwhBKcT2Xwt3Ok1-pA,779
 src/qadratic_problem_real_data.py,sha256=OnZrwv5-0i2nFlw1qjmlGSf3DYcjeULdBcGnlFnHrtQ,1402
 src/quadratic_problem.py,sha256=4o2u2B7OvFgQEFD-ULZep55DU58IsbaiW4wbIWHsStw,1916
 src/rastrigin.py,sha256=4TQXNTsDEip3WYrjDODscWOM5fSM7TzcTKUIcN5o1yY,831
 src/rosenbrock.py,sha256=8iZ_nWBvmz8qVGka3Svgy7AQdBksk7zlLGZQNBuAVq4,810
-benchmarx-0.0.6.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-benchmarx-0.0.6.dist-info/METADATA,sha256=NuZdYc2JtNt2e8FtA3zmbALMkdAWH-p6I_dfzOysptk,881
-benchmarx-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-benchmarx-0.0.6.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
-benchmarx-0.0.6.dist-info/RECORD,,
+benchmarx-0.0.7.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+benchmarx-0.0.7.dist-info/METADATA,sha256=zUUqrgwr1q3Ti8sV1-q5tWXNIewaljXwQPMxY-aU0S0,881
+benchmarx-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+benchmarx-0.0.7.dist-info/top_level.txt,sha256=eScFY_msf3bRhwga3xmGC7NZAaN0Y9jNNesRHU8gEjg,14
+benchmarx-0.0.7.dist-info/RECORD,,
```

