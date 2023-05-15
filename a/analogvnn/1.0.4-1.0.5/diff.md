# Comparing `tmp/analogvnn-1.0.4.tar.gz` & `tmp/analogvnn-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analogvnn-1.0.4.tar", last modified: Wed May 10 23:45:55 2023, max compression
+gzip compressed data, was "analogvnn-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `analogvnn-1.0.4.tar` & `analogvnn-1.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    17182 2023-01-25 01:41:18.328863 analogvnn-1.0.4/LICENSE
--rw-r--r--   0        0        0     2823 2023-05-10 23:42:25.531782 analogvnn-1.0.4/README.md
--rw-r--r--   0        0        0      728 2023-03-07 11:00:42.959136 analogvnn-1.0.4/analogvnn/__init__.py
--rw-r--r--   0        0        0     2873 2023-03-21 17:16:13.013355 analogvnn-1.0.4/analogvnn/backward/BackwardFunction.py
--rw-r--r--   0        0        0      930 2023-01-25 01:41:18.236582 analogvnn-1.0.4/analogvnn/backward/BackwardIdentity.py
--rw-r--r--   0        0        0    10140 2023-03-21 17:16:13.013355 analogvnn-1.0.4/analogvnn/backward/BackwardModule.py
--rw-r--r--   0        0        0      894 2023-01-25 01:41:18.245026 analogvnn-1.0.4/analogvnn/backward/BackwardUsingForward.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.232132 analogvnn-1.0.4/analogvnn/backward/__init__.py
--rw-r--r--   0        0        0       43 2023-03-07 11:00:42.961641 analogvnn-1.0.4/analogvnn/fn/__init__.py
--rw-r--r--   0        0        0      609 2023-03-07 11:00:42.963657 analogvnn-1.0.4/analogvnn/fn/dirac_delta.py
--rw-r--r--   0        0        0     1998 2023-01-25 01:41:18.238101 analogvnn-1.0.4/analogvnn/fn/reduce_precision.py
--rw-r--r--   0        0        0     1145 2023-01-25 01:41:18.238665 analogvnn-1.0.4/analogvnn/fn/test.py
--rw-r--r--   0        0        0      435 2023-01-25 01:41:18.243027 analogvnn-1.0.4/analogvnn/fn/to_matrix.py
--rw-r--r--   0        0        0     2154 2023-01-25 01:41:18.245026 analogvnn-1.0.4/analogvnn/fn/train.py
--rw-r--r--   0        0        0     6149 2023-03-21 17:16:13.013355 analogvnn-1.0.4/analogvnn/graph/AccumulateGrad.py
--rw-r--r--   0        0        0    16888 2023-03-21 17:16:13.013355 analogvnn-1.0.4/analogvnn/graph/AcyclicDirectedGraph.py
--rw-r--r--   0        0        0     3091 2023-05-08 04:09:29.467715 analogvnn-1.0.4/analogvnn/graph/ArgsKwargs.py
--rw-r--r--   0        0        0    12447 2023-05-08 04:22:49.100096 analogvnn-1.0.4/analogvnn/graph/BackwardGraph.py
--rw-r--r--   0        0        0     4580 2023-03-21 17:16:13.013355 analogvnn-1.0.4/analogvnn/graph/ForwardGraph.py
--rw-r--r--   0        0        0      503 2023-01-25 01:41:18.246026 analogvnn-1.0.4/analogvnn/graph/GraphEnum.py
--rw-r--r--   0        0        0     1655 2023-03-21 17:16:13.020383 analogvnn-1.0.4/analogvnn/graph/ModelGraph.py
--rw-r--r--   0        0        0     4036 2023-05-08 04:03:55.473530 analogvnn-1.0.4/analogvnn/graph/ModelGraphState.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.243027 analogvnn-1.0.4/analogvnn/graph/__init__.py
--rw-r--r--   0        0        0     2444 2023-03-07 11:00:42.977680 analogvnn-1.0.4/analogvnn/graph/to_graph_viz_digraph.py
--rw-r--r--   0        0        0     3326 2023-03-21 17:16:13.020383 analogvnn-1.0.4/analogvnn/nn/Linear.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.248023 analogvnn-1.0.4/analogvnn/nn/__init__.py
--rw-r--r--   0        0        0     1149 2023-01-25 01:41:18.251094 analogvnn-1.0.4/analogvnn/nn/activation/Activation.py
--rw-r--r--   0        0        0      944 2023-01-25 01:41:18.256113 analogvnn-1.0.4/analogvnn/nn/activation/BinaryStep.py
--rw-r--r--   0        0        0     3336 2023-03-21 17:16:13.020383 analogvnn-1.0.4/analogvnn/nn/activation/ELU.py
--rw-r--r--   0        0        0     2052 2023-01-25 01:41:18.261162 analogvnn-1.0.4/analogvnn/nn/activation/Gaussian.py
--rw-r--r--   0        0        0     1622 2023-03-21 17:16:13.020383 analogvnn-1.0.4/analogvnn/nn/activation/Identity.py
--rw-r--r--   0        0        0     4197 2023-03-21 17:16:13.020383 analogvnn-1.0.4/analogvnn/nn/activation/ReLU.py
--rw-r--r--   0        0        0      979 2023-01-25 01:41:18.260166 analogvnn-1.0.4/analogvnn/nn/activation/SiLU.py
--rw-r--r--   0        0        0     1953 2023-01-25 01:41:18.259178 analogvnn-1.0.4/analogvnn/nn/activation/Sigmoid.py
--rw-r--r--   0        0        0     1765 2023-01-25 01:41:18.260166 analogvnn-1.0.4/analogvnn/nn/activation/Tanh.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.249123 analogvnn-1.0.4/analogvnn/nn/activation/__init__.py
--rw-r--r--   0        0        0      895 2023-01-25 01:41:18.263373 analogvnn-1.0.4/analogvnn/nn/module/FullSequential.py
--rw-r--r--   0        0        0     9179 2023-05-08 02:47:38.140435 analogvnn-1.0.4/analogvnn/nn/module/Layer.py
--rw-r--r--   0        0        0    10854 2023-05-08 03:50:03.052825 analogvnn-1.0.4/analogvnn/nn/module/Model.py
--rw-r--r--   0        0        0     1470 2023-01-25 01:41:18.268523 analogvnn-1.0.4/analogvnn/nn/module/Sequential.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.257237 analogvnn-1.0.4/analogvnn/nn/module/__init__.py
--rw-r--r--   0        0        0     7169 2023-03-21 17:16:13.023398 analogvnn-1.0.4/analogvnn/nn/noise/GaussianNoise.py
--rw-r--r--   0        0        0     7025 2023-03-21 17:16:13.023398 analogvnn-1.0.4/analogvnn/nn/noise/LaplacianNoise.py
--rw-r--r--   0        0        0      154 2023-03-07 11:00:42.987197 analogvnn-1.0.4/analogvnn/nn/noise/Noise.py
--rw-r--r--   0        0        0    10404 2023-03-21 17:16:13.023398 analogvnn-1.0.4/analogvnn/nn/noise/PoissonNoise.py
--rw-r--r--   0        0        0     6860 2023-03-21 17:16:13.020383 analogvnn-1.0.4/analogvnn/nn/noise/UniformNoise.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.263373 analogvnn-1.0.4/analogvnn/nn/noise/__init__.py
--rw-r--r--   0        0        0     2044 2023-03-07 11:00:42.990199 analogvnn-1.0.4/analogvnn/nn/normalize/Clamp.py
--rw-r--r--   0        0        0     4469 2023-03-21 17:16:13.023398 analogvnn-1.0.4/analogvnn/nn/normalize/LPNorm.py
--rw-r--r--   0        0        0      170 2023-03-07 11:00:42.991704 analogvnn-1.0.4/analogvnn/nn/normalize/Normalize.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.267528 analogvnn-1.0.4/analogvnn/nn/normalize/__init__.py
--rw-r--r--   0        0        0      166 2023-03-07 11:00:42.992711 analogvnn-1.0.4/analogvnn/nn/precision/Precision.py
--rw-r--r--   0        0        0     3092 2023-03-21 17:16:13.023398 analogvnn-1.0.4/analogvnn/nn/precision/ReducePrecision.py
--rw-r--r--   0        0        0     2554 2023-03-21 17:16:13.023398 analogvnn-1.0.4/analogvnn/nn/precision/StochasticReducePrecision.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.269514 analogvnn-1.0.4/analogvnn/nn/precision/__init__.py
--rw-r--r--   0        0        0     8351 2023-05-10 23:32:54.454703 analogvnn-1.0.4/analogvnn/parameter/PseudoParameter.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.276870 analogvnn-1.0.4/analogvnn/parameter/__init__.py
--rw-r--r--   0        0        0     7965 2023-03-21 17:16:13.023398 analogvnn-1.0.4/analogvnn/utils/TensorboardModelLog.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.277865 analogvnn-1.0.4/analogvnn/utils/__init__.py
--rw-r--r--   0        0        0      591 2023-03-07 11:00:42.998714 analogvnn-1.0.4/analogvnn/utils/common_types.py
--rw-r--r--   0        0        0     2390 2023-03-07 11:00:42.999711 analogvnn-1.0.4/analogvnn/utils/get_model_summaries.py
--rw-r--r--   0        0        0     3016 2023-03-21 17:16:13.033447 analogvnn-1.0.4/analogvnn/utils/is_cpu_cuda.py
--rw-r--r--   0        0        0    35029 2023-03-21 17:16:13.023398 analogvnn-1.0.4/analogvnn/utils/render_autograd_graph.py
--rw-r--r--   0        0        0     1011 2023-01-25 01:41:18.284864 analogvnn-1.0.4/analogvnn/utils/to_tensor_parameter.py
--rw-r--r--   0        0        0     4474 2023-05-10 23:03:55.737068 analogvnn-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     6077 1970-01-01 00:00:00.000000 analogvnn-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    17182 2023-01-25 01:41:18.328863 analogvnn-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2823 2023-05-15 06:56:59.430140 analogvnn-1.0.5/README.md
+-rw-r--r--   0        0        0      728 2023-03-07 11:00:42.959136 analogvnn-1.0.5/analogvnn/__init__.py
+-rw-r--r--   0        0        0     2873 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/backward/BackwardFunction.py
+-rw-r--r--   0        0        0      930 2023-01-25 01:41:18.236582 analogvnn-1.0.5/analogvnn/backward/BackwardIdentity.py
+-rw-r--r--   0        0        0    10140 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/backward/BackwardModule.py
+-rw-r--r--   0        0        0      894 2023-01-25 01:41:18.245026 analogvnn-1.0.5/analogvnn/backward/BackwardUsingForward.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.232132 analogvnn-1.0.5/analogvnn/backward/__init__.py
+-rw-r--r--   0        0        0       43 2023-03-07 11:00:42.961641 analogvnn-1.0.5/analogvnn/fn/__init__.py
+-rw-r--r--   0        0        0      609 2023-03-07 11:00:42.963657 analogvnn-1.0.5/analogvnn/fn/dirac_delta.py
+-rw-r--r--   0        0        0     1998 2023-01-25 01:41:18.238101 analogvnn-1.0.5/analogvnn/fn/reduce_precision.py
+-rw-r--r--   0        0        0     1145 2023-01-25 01:41:18.238665 analogvnn-1.0.5/analogvnn/fn/test.py
+-rw-r--r--   0        0        0      435 2023-01-25 01:41:18.243027 analogvnn-1.0.5/analogvnn/fn/to_matrix.py
+-rw-r--r--   0        0        0     2154 2023-01-25 01:41:18.245026 analogvnn-1.0.5/analogvnn/fn/train.py
+-rw-r--r--   0        0        0     6149 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/graph/AccumulateGrad.py
+-rw-r--r--   0        0        0    16888 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/graph/AcyclicDirectedGraph.py
+-rw-r--r--   0        0        0     3091 2023-05-08 04:09:29.467715 analogvnn-1.0.5/analogvnn/graph/ArgsKwargs.py
+-rw-r--r--   0        0        0    12600 2023-05-15 06:51:03.515932 analogvnn-1.0.5/analogvnn/graph/BackwardGraph.py
+-rw-r--r--   0        0        0     4580 2023-03-21 17:16:13.013355 analogvnn-1.0.5/analogvnn/graph/ForwardGraph.py
+-rw-r--r--   0        0        0      503 2023-01-25 01:41:18.246026 analogvnn-1.0.5/analogvnn/graph/GraphEnum.py
+-rw-r--r--   0        0        0     1655 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/graph/ModelGraph.py
+-rw-r--r--   0        0        0     4036 2023-05-08 04:03:55.473530 analogvnn-1.0.5/analogvnn/graph/ModelGraphState.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.243027 analogvnn-1.0.5/analogvnn/graph/__init__.py
+-rw-r--r--   0        0        0     2444 2023-03-07 11:00:42.977680 analogvnn-1.0.5/analogvnn/graph/to_graph_viz_digraph.py
+-rw-r--r--   0        0        0     3326 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/Linear.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.248023 analogvnn-1.0.5/analogvnn/nn/__init__.py
+-rw-r--r--   0        0        0     1149 2023-01-25 01:41:18.251094 analogvnn-1.0.5/analogvnn/nn/activation/Activation.py
+-rw-r--r--   0        0        0      944 2023-01-25 01:41:18.256113 analogvnn-1.0.5/analogvnn/nn/activation/BinaryStep.py
+-rw-r--r--   0        0        0     3336 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/activation/ELU.py
+-rw-r--r--   0        0        0     2052 2023-01-25 01:41:18.261162 analogvnn-1.0.5/analogvnn/nn/activation/Gaussian.py
+-rw-r--r--   0        0        0     1622 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/activation/Identity.py
+-rw-r--r--   0        0        0     4197 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/activation/ReLU.py
+-rw-r--r--   0        0        0      979 2023-01-25 01:41:18.260166 analogvnn-1.0.5/analogvnn/nn/activation/SiLU.py
+-rw-r--r--   0        0        0     1953 2023-01-25 01:41:18.259178 analogvnn-1.0.5/analogvnn/nn/activation/Sigmoid.py
+-rw-r--r--   0        0        0     1765 2023-01-25 01:41:18.260166 analogvnn-1.0.5/analogvnn/nn/activation/Tanh.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.249123 analogvnn-1.0.5/analogvnn/nn/activation/__init__.py
+-rw-r--r--   0        0        0      895 2023-01-25 01:41:18.263373 analogvnn-1.0.5/analogvnn/nn/module/FullSequential.py
+-rw-r--r--   0        0        0     9179 2023-05-08 02:47:38.140435 analogvnn-1.0.5/analogvnn/nn/module/Layer.py
+-rw-r--r--   0        0        0    10854 2023-05-08 03:50:03.052825 analogvnn-1.0.5/analogvnn/nn/module/Model.py
+-rw-r--r--   0        0        0     1470 2023-01-25 01:41:18.268523 analogvnn-1.0.5/analogvnn/nn/module/Sequential.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.257237 analogvnn-1.0.5/analogvnn/nn/module/__init__.py
+-rw-r--r--   0        0        0     7169 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/noise/GaussianNoise.py
+-rw-r--r--   0        0        0     7025 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/noise/LaplacianNoise.py
+-rw-r--r--   0        0        0      154 2023-03-07 11:00:42.987197 analogvnn-1.0.5/analogvnn/nn/noise/Noise.py
+-rw-r--r--   0        0        0    10404 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/noise/PoissonNoise.py
+-rw-r--r--   0        0        0     6860 2023-03-21 17:16:13.020383 analogvnn-1.0.5/analogvnn/nn/noise/UniformNoise.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.263373 analogvnn-1.0.5/analogvnn/nn/noise/__init__.py
+-rw-r--r--   0        0        0     2044 2023-03-07 11:00:42.990199 analogvnn-1.0.5/analogvnn/nn/normalize/Clamp.py
+-rw-r--r--   0        0        0     4469 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/normalize/LPNorm.py
+-rw-r--r--   0        0        0      170 2023-03-07 11:00:42.991704 analogvnn-1.0.5/analogvnn/nn/normalize/Normalize.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.267528 analogvnn-1.0.5/analogvnn/nn/normalize/__init__.py
+-rw-r--r--   0        0        0      166 2023-03-07 11:00:42.992711 analogvnn-1.0.5/analogvnn/nn/precision/Precision.py
+-rw-r--r--   0        0        0     3092 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/precision/ReducePrecision.py
+-rw-r--r--   0        0        0     2554 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/nn/precision/StochasticReducePrecision.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.269514 analogvnn-1.0.5/analogvnn/nn/precision/__init__.py
+-rw-r--r--   0        0        0     7950 2023-05-11 10:00:01.960587 analogvnn-1.0.5/analogvnn/parameter/PseudoParameter.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.276870 analogvnn-1.0.5/analogvnn/parameter/__init__.py
+-rw-r--r--   0        0        0     7965 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/utils/TensorboardModelLog.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.277865 analogvnn-1.0.5/analogvnn/utils/__init__.py
+-rw-r--r--   0        0        0      591 2023-03-07 11:00:42.998714 analogvnn-1.0.5/analogvnn/utils/common_types.py
+-rw-r--r--   0        0        0     2390 2023-03-07 11:00:42.999711 analogvnn-1.0.5/analogvnn/utils/get_model_summaries.py
+-rw-r--r--   0        0        0     3016 2023-03-21 17:16:13.033447 analogvnn-1.0.5/analogvnn/utils/is_cpu_cuda.py
+-rw-r--r--   0        0        0    35029 2023-03-21 17:16:13.023398 analogvnn-1.0.5/analogvnn/utils/render_autograd_graph.py
+-rw-r--r--   0        0        0     1011 2023-01-25 01:41:18.284864 analogvnn-1.0.5/analogvnn/utils/to_tensor_parameter.py
+-rw-r--r--   0        0        0     4474 2023-05-15 06:41:23.024517 analogvnn-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6077 1970-01-01 00:00:00.000000 analogvnn-1.0.5/PKG-INFO
```

### Comparing `analogvnn-1.0.4/LICENSE` & `analogvnn-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/README.md` & `analogvnn-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/__init__.py` & `analogvnn-1.0.5/analogvnn/__init__.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/backward/BackwardFunction.py` & `analogvnn-1.0.5/analogvnn/backward/BackwardFunction.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/backward/BackwardIdentity.py` & `analogvnn-1.0.5/analogvnn/backward/BackwardIdentity.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/backward/BackwardModule.py` & `analogvnn-1.0.5/analogvnn/backward/BackwardModule.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/backward/BackwardUsingForward.py` & `analogvnn-1.0.5/analogvnn/backward/BackwardUsingForward.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/fn/dirac_delta.py` & `analogvnn-1.0.5/analogvnn/fn/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/fn/reduce_precision.py` & `analogvnn-1.0.5/analogvnn/fn/reduce_precision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/fn/test.py` & `analogvnn-1.0.5/analogvnn/fn/test.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/fn/train.py` & `analogvnn-1.0.5/analogvnn/fn/train.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/graph/AccumulateGrad.py` & `analogvnn-1.0.5/analogvnn/graph/AccumulateGrad.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/graph/AcyclicDirectedGraph.py` & `analogvnn-1.0.5/analogvnn/graph/AcyclicDirectedGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/graph/ArgsKwargs.py` & `analogvnn-1.0.5/analogvnn/graph/ArgsKwargs.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/graph/BackwardGraph.py` & `analogvnn-1.0.5/analogvnn/graph/BackwardGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,15 +263,14 @@
         if isinstance(module, Layer) and isinstance(module.backward_function, BackwardModule):
             module = module.backward_function
 
         if isinstance(module, BackwardModule):
             grad_inputs = module._call_impl_backward(*grad_outputs.inputs.args, **grad_outputs.inputs.kwargs)
             return ArgsKwargs.to_args_kwargs_object(grad_inputs)
 
-        grad_dict = {}
         inputs = module_inputs_outputs.inputs.args + list(module_inputs_outputs.inputs.kwargs.values())
         outputs = []
         outputs_grads = []
         module_parameters = []
 
         if len(inputs) == 0:
             return ArgsKwargs(
@@ -287,30 +286,32 @@
             outputs.append(module_inputs_outputs.outputs.kwargs[i])
             outputs_grads.append(grad_outputs.inputs.kwargs[i])
 
         if isinstance(module, nn.Module):
             module_parameters = list(module.parameters())
             inputs += module_parameters
 
+        grad_dict = {id(i): None for i in inputs}
+        filtered_inputs = [i for i in inputs if i is not None and i.requires_grad]
         out_grads = torch.autograd.grad(
             outputs=outputs,
-            inputs=inputs,
+            inputs=filtered_inputs,
             grad_outputs=outputs_grads,
             retain_graph=True,
             allow_unused=True
         )
         for i, v in enumerate(out_grads):
-            grad_dict[inputs[i]] = v
+            grad_dict[id(filtered_inputs[i])] = v
 
         for i in module_parameters:
-            if grad_dict[i] is None:
+            if grad_dict[id(i)] is None:
                 continue
 
             if i.grad is None:
-                i.grad = grad_dict[i]
+                i.grad = grad_dict[id(i)]
             else:
-                i.grad += grad_dict[i]
+                i.grad += grad_dict[id(i)]
 
         return ArgsKwargs(
-            args=[grad_dict[i] for i in module_inputs_outputs.inputs.args],
-            kwargs={key: grad_dict[value] for key, value in module_inputs_outputs.inputs.kwargs.items()}
+            args=[grad_dict[id(i)] for i in module_inputs_outputs.inputs.args],
+            kwargs={key: grad_dict[id(value)] for key, value in module_inputs_outputs.inputs.kwargs.items()}
         )
```

### Comparing `analogvnn-1.0.4/analogvnn/graph/ForwardGraph.py` & `analogvnn-1.0.5/analogvnn/graph/ForwardGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/graph/ModelGraph.py` & `analogvnn-1.0.5/analogvnn/graph/ModelGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/graph/ModelGraphState.py` & `analogvnn-1.0.5/analogvnn/graph/ModelGraphState.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/graph/to_graph_viz_digraph.py` & `analogvnn-1.0.5/analogvnn/graph/to_graph_viz_digraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/Linear.py` & `analogvnn-1.0.5/analogvnn/nn/Linear.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/Activation.py` & `analogvnn-1.0.5/analogvnn/nn/activation/Activation.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/BinaryStep.py` & `analogvnn-1.0.5/analogvnn/nn/activation/BinaryStep.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/ELU.py` & `analogvnn-1.0.5/analogvnn/nn/activation/ELU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/Gaussian.py` & `analogvnn-1.0.5/analogvnn/nn/activation/Gaussian.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/Identity.py` & `analogvnn-1.0.5/analogvnn/nn/activation/Identity.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/ReLU.py` & `analogvnn-1.0.5/analogvnn/nn/activation/ReLU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/SiLU.py` & `analogvnn-1.0.5/analogvnn/nn/activation/SiLU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/Sigmoid.py` & `analogvnn-1.0.5/analogvnn/nn/activation/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/activation/Tanh.py` & `analogvnn-1.0.5/analogvnn/nn/activation/Tanh.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/module/FullSequential.py` & `analogvnn-1.0.5/analogvnn/nn/module/FullSequential.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/module/Layer.py` & `analogvnn-1.0.5/analogvnn/nn/module/Layer.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/module/Model.py` & `analogvnn-1.0.5/analogvnn/nn/module/Model.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/module/Sequential.py` & `analogvnn-1.0.5/analogvnn/nn/module/Sequential.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/noise/GaussianNoise.py` & `analogvnn-1.0.5/analogvnn/nn/noise/GaussianNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/noise/LaplacianNoise.py` & `analogvnn-1.0.5/analogvnn/nn/noise/LaplacianNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/noise/PoissonNoise.py` & `analogvnn-1.0.5/analogvnn/nn/noise/PoissonNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/noise/UniformNoise.py` & `analogvnn-1.0.5/analogvnn/nn/noise/UniformNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/normalize/Clamp.py` & `analogvnn-1.0.5/analogvnn/nn/normalize/Clamp.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/normalize/LPNorm.py` & `analogvnn-1.0.5/analogvnn/nn/normalize/LPNorm.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/precision/ReducePrecision.py` & `analogvnn-1.0.5/analogvnn/nn/precision/ReducePrecision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/nn/precision/StochasticReducePrecision.py` & `analogvnn-1.0.5/analogvnn/nn/precision/StochasticReducePrecision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/parameter/PseudoParameter.py` & `analogvnn-1.0.5/analogvnn/parameter/PseudoParameter.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,34 +119,14 @@
 
         return f'{PseudoParameter.__name__}(' \
                f'transform={self.transformation}' \
                f', original={self.original}' \
                f')'
 
     @property
-    def grad(self):
-        """Returns the gradient of the parameter.
-
-        Returns:
-            Tensor: the gradient.
-        """
-
-        return self._transformed.grad
-
-    @grad.setter
-    def grad(self, grad: Tensor):
-        """Sets the gradient of the parameter.
-
-        Args:
-            grad (Tensor): the gradient.
-        """
-
-        self._transformed.grad = grad
-
-    @property
     def transformation(self):
         """Returns the transformation.
 
         Returns:
             Callable: the transformation.
         """
 
@@ -183,16 +163,16 @@
             tensor_to: Any,
             property_name: str,
             setter: bool = True
     ):
         """Substitutes a member of a tensor as property of another tensor.
 
         Args:
-            tensor_from (Any): the tensor to substitute from.
-            tensor_to (Any): the tensor to substitute to.
+            tensor_from (Any): the tensor property to substitute.
+            tensor_to (Any): the tensor property to substitute to.
             property_name (str): the name of the property.
             setter (bool): whether to substitute the setter.
         """
 
         def getter_fn(self):
             return getattr(tensor_to, property_name)
```

### Comparing `analogvnn-1.0.4/analogvnn/utils/TensorboardModelLog.py` & `analogvnn-1.0.5/analogvnn/utils/TensorboardModelLog.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/utils/common_types.py` & `analogvnn-1.0.5/analogvnn/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/utils/get_model_summaries.py` & `analogvnn-1.0.5/analogvnn/utils/get_model_summaries.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/utils/is_cpu_cuda.py` & `analogvnn-1.0.5/analogvnn/utils/is_cpu_cuda.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/utils/render_autograd_graph.py` & `analogvnn-1.0.5/analogvnn/utils/render_autograd_graph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/analogvnn/utils/to_tensor_parameter.py` & `analogvnn-1.0.5/analogvnn/utils/to_tensor_parameter.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.4/pyproject.toml` & `analogvnn-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [tool.setuptools]
 py-modules = ['analogvnn']
 
 [project]
 # $ pip install analogvnn
 name = "analogvnn"
-version = "1.0.4"
+version = "1.0.5"
 description = "A fully modular framework for modeling and optimizing analog/photonic neural networks"  # Optional
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["deep-learning", "analog", "photonics", "neural-network", "framework", "pytorch"]
 authors = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
```

### Comparing `analogvnn-1.0.4/PKG-INFO` & `analogvnn-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analogvnn
-Version: 1.0.4
+Version: 1.0.5
 Summary: A fully modular framework for modeling and optimizing analog/photonic neural networks
 Keywords: deep-learning,analog,photonics,neural-network,framework,pytorch
 Author-email: Vivswan Shah <vivswanshah@pitt.edu>
 Maintainer-email: Vivswan Shah <vivswanshah@pitt.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

