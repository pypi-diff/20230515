# Comparing `tmp/benchmarx-0.0.8-py3-none-any.whl.zip` & `tmp/benchmarx-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,26 @@
-Zip file size: 22962 bytes, number of entries: 22
+Zip file size: 43858 bytes, number of entries: 40
+-rw-r--r--  2.0 unx     1202 b- defN 23-May-12 19:03 benchmarx/__init__.py
+-rw-r--r--  2.0 unx    11189 b- defN 23-May-14 18:00 benchmarx/src/NeuralNetworkTraining.py
+-rw-r--r--  2.0 unx     1543 b- defN 23-May-12 12:42 benchmarx/src/ProxGD_custom_linesearch.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-14 21:58 benchmarx/src/__init__.py
+-rw-r--r--  2.0 unx    21138 b- defN 23-May-14 18:10 benchmarx/src/benchmark.py
+-rw-r--r--  2.0 unx     5271 b- defN 23-May-14 17:55 benchmarx/src/benchmark_result.py
+-rw-r--r--  2.0 unx     1333 b- defN 23-Apr-27 19:34 benchmarx/src/custom_optimizer.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-30 18:47 benchmarx/src/defaults.py
+-rw-r--r--  2.0 unx     2073 b- defN 23-May-13 18:59 benchmarx/src/log_loss.py
+-rw-r--r--  2.0 unx     2258 b- defN 23-May-13 18:59 benchmarx/src/log_loss_l2_reg.py
+-rw-r--r--  2.0 unx      495 b- defN 23-May-14 17:57 benchmarx/src/methods.py
+-rw-r--r--  2.0 unx     1212 b- defN 23-May-14 17:54 benchmarx/src/metrics.py
+-rw-r--r--  2.0 unx    20912 b- defN 23-May-14 21:08 benchmarx/src/plotter.py
+-rw-r--r--  2.0 unx      779 b- defN 23-May-13 20:00 benchmarx/src/problem.py
+-rw-r--r--  2.0 unx     1402 b- defN 23-May-13 20:35 benchmarx/src/qadratic_problem_real_data.py
+-rw-r--r--  2.0 unx     1916 b- defN 23-May-12 13:01 benchmarx/src/quadratic_problem.py
+-rw-r--r--  2.0 unx      831 b- defN 23-May-13 19:39 benchmarx/src/rastrigin.py
+-rw-r--r--  2.0 unx      810 b- defN 23-May-13 19:40 benchmarx/src/rosenbrock.py
 -rw-r--r--  2.0 unx    11189 b- defN 23-May-14 18:00 src/NeuralNetworkTraining.py
 -rw-r--r--  2.0 unx     1543 b- defN 23-May-12 12:42 src/ProxGD_custom_linesearch.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-14 21:58 src/__init__.py
 -rw-r--r--  2.0 unx    21138 b- defN 23-May-14 18:10 src/benchmark.py
 -rw-r--r--  2.0 unx     5271 b- defN 23-May-14 17:55 src/benchmark_result.py
 -rw-r--r--  2.0 unx     1333 b- defN 23-Apr-27 19:34 src/custom_optimizer.py
 -rw-r--r--  2.0 unx       46 b- defN 23-Apr-30 18:47 src/defaults.py
@@ -12,13 +30,13 @@
 -rw-r--r--  2.0 unx     1212 b- defN 23-May-14 17:54 src/metrics.py
 -rw-r--r--  2.0 unx    20912 b- defN 23-May-14 21:08 src/plotter.py
 -rw-r--r--  2.0 unx      779 b- defN 23-May-13 20:00 src/problem.py
 -rw-r--r--  2.0 unx     1402 b- defN 23-May-13 20:35 src/qadratic_problem_real_data.py
 -rw-r--r--  2.0 unx     1916 b- defN 23-May-12 13:01 src/quadratic_problem.py
 -rw-r--r--  2.0 unx      831 b- defN 23-May-13 19:39 src/rastrigin.py
 -rw-r--r--  2.0 unx      810 b- defN 23-May-13 19:40 src/rosenbrock.py
--rw-r--r--  2.0 unx     1074 b- defN 23-May-14 22:37 benchmarx-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      881 b- defN 23-May-14 22:37 benchmarx-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 22:37 benchmarx-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-14 22:37 benchmarx-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1691 b- defN 23-May-14 22:37 benchmarx-0.0.8.dist-info/RECORD
-22 files, 76950 bytes uncompressed, 20262 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx     1074 b- defN 23-May-14 22:45 benchmarx-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      881 b- defN 23-May-14 22:45 benchmarx-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 22:45 benchmarx-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-14 22:45 benchmarx-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3237 b- defN 23-May-14 22:45 benchmarx-0.0.9.dist-info/RECORD
+40 files, 152912 bytes uncompressed, 38740 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -1,7 +1,61 @@
+Filename: benchmarx/__init__.py
+Comment: 
+
+Filename: benchmarx/src/NeuralNetworkTraining.py
+Comment: 
+
+Filename: benchmarx/src/ProxGD_custom_linesearch.py
+Comment: 
+
+Filename: benchmarx/src/__init__.py
+Comment: 
+
+Filename: benchmarx/src/benchmark.py
+Comment: 
+
+Filename: benchmarx/src/benchmark_result.py
+Comment: 
+
+Filename: benchmarx/src/custom_optimizer.py
+Comment: 
+
+Filename: benchmarx/src/defaults.py
+Comment: 
+
+Filename: benchmarx/src/log_loss.py
+Comment: 
+
+Filename: benchmarx/src/log_loss_l2_reg.py
+Comment: 
+
+Filename: benchmarx/src/methods.py
+Comment: 
+
+Filename: benchmarx/src/metrics.py
+Comment: 
+
+Filename: benchmarx/src/plotter.py
+Comment: 
+
+Filename: benchmarx/src/problem.py
+Comment: 
+
+Filename: benchmarx/src/qadratic_problem_real_data.py
+Comment: 
+
+Filename: benchmarx/src/quadratic_problem.py
+Comment: 
+
+Filename: benchmarx/src/rastrigin.py
+Comment: 
+
+Filename: benchmarx/src/rosenbrock.py
+Comment: 
+
 Filename: src/NeuralNetworkTraining.py
 Comment: 
 
 Filename: src/ProxGD_custom_linesearch.py
 Comment: 
 
 Filename: src/__init__.py
@@ -45,23 +99,23 @@
 
 Filename: src/rastrigin.py
 Comment: 
 
 Filename: src/rosenbrock.py
 Comment: 
 
-Filename: benchmarx-0.0.8.dist-info/LICENSE
+Filename: benchmarx-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: benchmarx-0.0.8.dist-info/METADATA
+Filename: benchmarx-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: benchmarx-0.0.8.dist-info/WHEEL
+Filename: benchmarx-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: benchmarx-0.0.8.dist-info/top_level.txt
+Filename: benchmarx-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: benchmarx-0.0.8.dist-info/RECORD
+Filename: benchmarx-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `benchmarx-0.0.8.dist-info/LICENSE` & `benchmarx-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `benchmarx-0.0.8.dist-info/METADATA` & `benchmarx-0.0.9.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmarx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for benchmarking optimization methods
 Home-page: https://github.com/AlexToW/benchmarx
 Author: AlexToW
 Author-email: Salex <31salex31@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AlexToW/benchmarx
 Project-URL: Bug Tracker, https://github.com/AlexToW/benchmarx/issues
```

## Comparing `benchmarx-0.0.8.dist-info/RECORD` & `benchmarx-0.0.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+benchmarx/__init__.py,sha256=wrnxGD5be6fvLC3oaGRHLiJEi-Ip95MY6gLrGxvoSco,1202
+benchmarx/src/NeuralNetworkTraining.py,sha256=c46UhHwkogRAlr64GfQV2gPCZ_GN1rapuceNKdjLCUE,11189
+benchmarx/src/ProxGD_custom_linesearch.py,sha256=ppVBl70iNZPYlNufPAdlO981nq3xM0Xs78yJlF-3NeE,1543
+benchmarx/src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchmarx/src/benchmark.py,sha256=UAP_3hj9TwmXRZ499CqGofOeIvaNHQFxLS29aLe6j34,21138
+benchmarx/src/benchmark_result.py,sha256=AatCEM7vQVgDr4aYhj9cOC5UTiD7vAYOTotLxONc368,5271
+benchmarx/src/custom_optimizer.py,sha256=i2sQMlDPPj-7Kl1jSO2B5shjNfWw-hdAf1j9wO58Hks,1333
+benchmarx/src/defaults.py,sha256=M6beOgsxCa35smUdXKL5OmdLStGT5EpqU4cqTWoq2l8,46
+benchmarx/src/log_loss.py,sha256=HQI_PWxBcTq44CDbwMGODHF0FXLM71j6ihYmKG_plM8,2073
+benchmarx/src/log_loss_l2_reg.py,sha256=t_PoOE2XdYn24Q1amqN19TEeKlYfCzh8Y3ZibKmVr1k,2258
+benchmarx/src/methods.py,sha256=aUHWjMUVQP0oX2ib-h3BlgnjLUUE-tgnhGuIJAiZv24,495
+benchmarx/src/metrics.py,sha256=y3PTp4d1HrOhnK5euAxL1k-p-bzfXk25Kh2Kj0gYR-0,1212
+benchmarx/src/plotter.py,sha256=DiLxAIQ3b1l7-iNPftkkJDQOu_-aGtKXT6c-NRK4Pmg,20912
+benchmarx/src/problem.py,sha256=zKPzjgh3Wp7Z_q-wfjePELq6khwhBKcT2Xwt3Ok1-pA,779
+benchmarx/src/qadratic_problem_real_data.py,sha256=OnZrwv5-0i2nFlw1qjmlGSf3DYcjeULdBcGnlFnHrtQ,1402
+benchmarx/src/quadratic_problem.py,sha256=4o2u2B7OvFgQEFD-ULZep55DU58IsbaiW4wbIWHsStw,1916
+benchmarx/src/rastrigin.py,sha256=4TQXNTsDEip3WYrjDODscWOM5fSM7TzcTKUIcN5o1yY,831
+benchmarx/src/rosenbrock.py,sha256=8iZ_nWBvmz8qVGka3Svgy7AQdBksk7zlLGZQNBuAVq4,810
 src/NeuralNetworkTraining.py,sha256=c46UhHwkogRAlr64GfQV2gPCZ_GN1rapuceNKdjLCUE,11189
 src/ProxGD_custom_linesearch.py,sha256=ppVBl70iNZPYlNufPAdlO981nq3xM0Xs78yJlF-3NeE,1543
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/benchmark.py,sha256=UAP_3hj9TwmXRZ499CqGofOeIvaNHQFxLS29aLe6j34,21138
 src/benchmark_result.py,sha256=AatCEM7vQVgDr4aYhj9cOC5UTiD7vAYOTotLxONc368,5271
 src/custom_optimizer.py,sha256=i2sQMlDPPj-7Kl1jSO2B5shjNfWw-hdAf1j9wO58Hks,1333
 src/defaults.py,sha256=M6beOgsxCa35smUdXKL5OmdLStGT5EpqU4cqTWoq2l8,46
@@ -11,12 +29,12 @@
 src/metrics.py,sha256=y3PTp4d1HrOhnK5euAxL1k-p-bzfXk25Kh2Kj0gYR-0,1212
 src/plotter.py,sha256=DiLxAIQ3b1l7-iNPftkkJDQOu_-aGtKXT6c-NRK4Pmg,20912
 src/problem.py,sha256=zKPzjgh3Wp7Z_q-wfjePELq6khwhBKcT2Xwt3Ok1-pA,779
 src/qadratic_problem_real_data.py,sha256=OnZrwv5-0i2nFlw1qjmlGSf3DYcjeULdBcGnlFnHrtQ,1402
 src/quadratic_problem.py,sha256=4o2u2B7OvFgQEFD-ULZep55DU58IsbaiW4wbIWHsStw,1916
 src/rastrigin.py,sha256=4TQXNTsDEip3WYrjDODscWOM5fSM7TzcTKUIcN5o1yY,831
 src/rosenbrock.py,sha256=8iZ_nWBvmz8qVGka3Svgy7AQdBksk7zlLGZQNBuAVq4,810
-benchmarx-0.0.8.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-benchmarx-0.0.8.dist-info/METADATA,sha256=iigLdC3QuNg2f7MZnPOB8QtC_VlDUY6YLHyCFFjhMYY,881
-benchmarx-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-benchmarx-0.0.8.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
-benchmarx-0.0.8.dist-info/RECORD,,
+benchmarx-0.0.9.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+benchmarx-0.0.9.dist-info/METADATA,sha256=QGaHLiTT7wOFdiBZWRoPBlwQuI-ErkyEVfTNGMa8qJo,881
+benchmarx-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+benchmarx-0.0.9.dist-info/top_level.txt,sha256=MfrTyVCft_w_XEedN18FSN-e0vbVeZ5GAh8WEU2_tiE,10
+benchmarx-0.0.9.dist-info/RECORD,,
```

