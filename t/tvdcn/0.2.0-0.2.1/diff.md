# Comparing `tmp/tvdcn-0.2.0.tar.gz` & `tmp/tvdcn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.2.0.tar", last modified: Sun May 14 05:10:39 2023, max compression
+gzip compressed data, was "tvdcn-0.2.1.tar", last modified: Mon May 15 13:24:41 2023, max compression
```

## Comparing `tvdcn-0.2.0.tar` & `tvdcn-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.509884 tvdcn-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 05:08:47.000000 tvdcn-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-14 05:10:39.509884 tvdcn-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-14 05:08:47.000000 tvdcn-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-14 05:08:47.000000 tvdcn-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 05:10:39.509884 tvdcn-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-14 05:08:47.000000 tvdcn-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.501884 tvdcn-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.501884 tvdcn-0.2.0/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.501884 tvdcn-0.2.0/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.505884 tvdcn-0.2.0/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.505884 tvdcn-0.2.0/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32946 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22667 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26400 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19207 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26783 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.505884 tvdcn-0.2.0/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.509884 tvdcn-0.2.0/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35826 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    38646 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/ops/mask_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-14 05:08:47.000000 tvdcn-0.2.0/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:10:39.501884 tvdcn-0.2.0/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-14 05:10:39.000000 tvdcn-0.2.0/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 05:10:39.000000 tvdcn-0.2.0/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 05:10:39.000000 tvdcn-0.2.0/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 05:10:39.000000 tvdcn-0.2.0/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 05:10:39.000000 tvdcn-0.2.0/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 05:10:39.000000 tvdcn-0.2.0/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.516272 tvdcn-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 13:22:47.000000 tvdcn-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-15 13:24:41.516272 tvdcn-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-15 13:22:47.000000 tvdcn-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-15 13:22:47.000000 tvdcn-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-15 13:24:41.516272 tvdcn-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-15 13:22:47.000000 tvdcn-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.508272 tvdcn-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.508272 tvdcn-0.2.1/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.508272 tvdcn-0.2.1/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.512272 tvdcn-0.2.1/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.512272 tvdcn-0.2.1/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18868 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22525 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19325 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22862 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26441 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.512272 tvdcn-0.2.1/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.516272 tvdcn-0.2.1/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35826 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38646 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/ops/mask_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-15 13:22:47.000000 tvdcn-0.2.1/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:24:41.508272 tvdcn-0.2.1/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-15 13:24:41.000000 tvdcn-0.2.1/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-15 13:24:41.000000 tvdcn-0.2.1/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:24:41.000000 tvdcn-0.2.1/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:24:41.000000 tvdcn-0.2.1/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 13:24:41.000000 tvdcn-0.2.1/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 13:24:41.000000 tvdcn-0.2.1/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.2.0/LICENSE.txt` & `tvdcn-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/PKG-INFO` & `tvdcn-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.0
+Version: 0.2.1
 Summary: Torchvision Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.2.0/README.md` & `tvdcn-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/pyproject.toml` & `tvdcn-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/setup.cfg` & `tvdcn-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/setup.py` & `tvdcn-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             nvcc_flags = nvcc_flags.split(' ')
         extra_compile_args['nvcc'] = nvcc_flags
 
     if sys.platform == 'win32':
         define_macros += [(f'{PACKAGE_ROOT}_EXPORTS', None)]
         define_macros += [('USE_PYTHON', None)]
         extra_compile_args['cxx'].append('/MP')
+        extra_compile_args['cxx'].append('/Zc:preprocessor')
 
     if debug_mode:
         print('Compiling in debug mode')
         extra_compile_args['cxx'].append('-g')
         extra_compile_args['cxx'].append('-O0')
         if 'nvcc' in extra_compile_args:
             # we have to remove '-OX' and '-g' flag if exists and append
```

### Comparing `tvdcn-0.2.0/tests/test_grad.py` & `tvdcn-0.2.1/tests/test_grad.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import torch
 from torch.autograd.gradcheck import gradcheck
 
 import tvdcn
 from utils.deform_conv_test_args import DeformConvTestArgs
 
 
-def test_deform_conv(dim=2):
+def test_deform_conv(dim=2,
+                     transposed=False,
+                     dtype=torch.float64,
+                     device='cpu'):
     torch.manual_seed(12)
-    conv_func = getattr(tvdcn, f'deform_conv{dim}d')
-    args = DeformConvTestArgs(dim=dim, device='cuda', dtype=torch.float64, batch_size=1)
+    conv_func = getattr(tvdcn, f'deform_conv{"_transpose" if transposed else ""}{dim}d')
+    args = DeformConvTestArgs(dim=dim, transposed=transposed, dtype=dtype, device=device)
     print(args)
 
     c_res = conv_func(args.input,
                       args.weight,
                       args.offset,
                       args.mask,
                       args.bias,
@@ -36,47 +39,9 @@
                                                  args.dilation,
                                                  args.weight_groups),
         (args.input, args.weight, args.offset, args.mask, args.bias), nondet_tol=args.tol)
     args.zero_grad()
     print('grad_check:', grad_ok)
 
 
-def test_deform_conv_transpose(dim=2):
-    torch.manual_seed(12)
-    conv_func = getattr(tvdcn, f'deform_conv_transpose{dim}d')
-    args = DeformConvTestArgs(transposed=True, dim=dim, device='cuda', dtype=torch.float64, batch_size=1)
-    print(args)
-
-    c_res = conv_func(args.input,
-                      args.weight,
-                      args.offset,
-                      args.mask,
-                      args.bias,
-                      args.stride,
-                      args.padding,
-                      args.output_padding,
-                      args.dilation,
-                      args.weight_groups)
-    c_res.sum().backward()
-    c_input_grad = args.input.grad.clone()
-    c_weight_grad = args.weight.grad.clone()
-    c_offset_grad = args.offset.grad.clone()
-    c_mask_grad = args.mask.grad.clone()
-    c_bias_grad = args.bias.grad.clone()
-    args.zero_grad()
-    print(c_res)
-
-    grad_ok = gradcheck(
-        lambda inp, wei, off, msk, bi: conv_func(inp, wei, off, msk, bi,
-                                                 args.stride,
-                                                 args.padding,
-                                                 args.output_padding,
-                                                 args.dilation,
-                                                 args.weight_groups),
-        (args.input, args.weight, args.offset, args.mask, args.bias), nondet_tol=args.tol)
-    args.zero_grad()
-    print('grad_check:', grad_ok)
-
-
 if __name__ == '__main__':
     test_deform_conv()
-    test_deform_conv_transpose()
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,142 +1,141 @@
 #include <ATen/ATen.h>
 #include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ scalar_t sample(
                     const at::TensorAccessor<scalar_t, 3> input,
-                    const int b,
-                    const int c,
-                    const int width,
-                    const int x) {
+                    const index_t b,
+                    const index_t c,
+                    const index_t width,
+                    const index_t x) {
                 return (0 <= x && x < width) ? input[b][c][x] : static_cast<scalar_t>(0);
             }
 
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ scalar_t interpolate_sample(
                     const at::TensorAccessor<scalar_t, 3> input,
-                    const int b,
-                    const int c,
-                    const int width,
+                    const index_t b,
+                    const index_t c,
+                    const index_t width,
                     const scalar_t x) {
                 if (x <= -1 || width <= x)
                     return 0;
 
-                int x_l = floor(x);
-                int x_h = x_l + 1;
+                index_t x_l = floor(x);
+                index_t x_h = x_l + 1;
 
                 scalar_t dx_h = x - x_l;
                 scalar_t dx_l = 1 - dx_h;
 
                 bool valid_x_l = x_l >= 0;
                 bool valid_x_h = x_h < width;
 
                 scalar_t val = 0;
                 if (valid_x_l) val += dx_l * input[b][c][x_l];
                 if (valid_x_h) val += dx_h * input[b][c][x_h];
                 return val;
             }
 
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ void insert(
                     at::TensorAccessor<scalar_t, 3> output,
-                    const int b,
-                    const int c,
-                    const int width,
-                    const int x,
+                    const index_t b,
+                    const index_t c,
+                    const index_t width,
+                    const index_t x,
                     const scalar_t val) {
                 if (0 <= x && x < width)
                     output[b][c][x] += val;
             }
 
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ void interpolate_insert(
                     at::TensorAccessor<scalar_t, 3> output,
-                    const int b,
-                    const int c,
-                    const int width,
+                    const index_t b,
+                    const index_t c,
+                    const index_t width,
                     const scalar_t x,
                     const scalar_t val) {
-                int x_l = floor(x);
-                int x_h = x_l + 1;
+                index_t x_l = floor(x);
+                index_t x_h = x_l + 1;
 
                 scalar_t dx_h = x - x_l;
                 scalar_t dx_l = 1 - dx_h;
 
                 bool valid_x_l = 0 <= x_l && x_l < width;
                 bool valid_x_h = 0 <= x_h && x_h < width;
 
                 if (valid_x_l) output[b][c][x_l] += dx_l * val;
                 if (valid_x_h) output[b][c][x_h] += dx_h * val;
             }
 
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ scalar_t coordinate_weight(
                     const at::TensorAccessor<scalar_t, 3> input,
-                    const int b,
-                    const int c,
-                    const int width,
+                    const index_t b,
+                    const index_t c,
+                    const index_t width,
                     const scalar_t x) {
-                int x_l = floor(x);
-                int x_h = x_l + 1;
+                index_t x_l = floor(x);
+                index_t x_h = x_l + 1;
 
                 scalar_t dx_h = 1;
                 scalar_t dx_l = -1;
 
                 bool valid_x_l = 0 <= x_l && x_l < width;
                 bool valid_x_h = 0 <= x_h && x_h < width;
 
                 scalar_t val = 0;
                 if (valid_x_l) val += dx_l * input[b][c][x_l];
                 if (valid_x_h) val += dx_h * input[b][c][x_h];
                 return val;
             }
         }
 
-        template<bool deformable, bool modulated, typename scalar_t>
+        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
         static void arr2col_kernel(
-                const int n_kernels,
+                const index_t n_kernels,
                 const at::TensorAccessor<scalar_t, 3> input,
                 const at::TensorAccessor<scalar_t, 5> offset,
                 const at::TensorAccessor<scalar_t, 4> mask,
-                const int width,
-                const int weight_w,
-                const int pad_w,
-                const int stride_w,
-                const int dilation_w,
-                const int out_w,
-                const int in_channels,
-                const int c_per_offset_group,
-                const int c_per_mask_group,
+                const index_t width,
+                const index_t weight_w,
+                const index_t pad_w,
+                const index_t stride_w,
+                const index_t dilation_w,
+                const index_t out_w,
+                const index_t in_channels,
+                const index_t c_per_offset_group,
+                const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 4> columns) {
-            CPU_1D_KERNEL_LOOP(index, n_kernels) {
-                const int w = index % out_w;
-                const int c = (index / out_w) % in_channels;
-                const int b = index / (out_w * in_channels);
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                const index_t w = index % out_w;
+                const index_t c = (index / out_w) % in_channels;
+                const index_t b = index / (out_w * in_channels);
 
-                const int offset_group_idx = c / c_per_offset_group;
-                const int mask_group_idx = c / c_per_mask_group;
+                const index_t offset_group_idx = c / c_per_offset_group;
+                const index_t mask_group_idx = c / c_per_mask_group;
 
-                for (int i = 0; i < weight_w; ++i) {
-                    const int x = (w * stride_w - pad_w) + i * dilation_w;
+                for (index_t i = 0; i < weight_w; ++i) {
+                    const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
                     const scalar_t val =
                             deformable ?
                             interpolate_sample(
                                     input, b, c, width,
                                     x + offset[b][offset_group_idx][i][0][w])
                                        : sample(input, b, c, width, x);
 
                     const scalar_t mask_val =
-                            modulated ?
-                            mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                            modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
 
                     columns[c][i][b][w] = val * mask_val;
                 }
             }
         }
 
         void arr2col_cpu(
@@ -147,76 +146,78 @@
                 const int width,
                 const int weight_w,
                 const int pad_w,
                 const int stride_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
-            const int n_kernels = in_channels * out_w * batch_sz;
-            const int c_per_offset_group = deformable ? in_channels / n_offset_grps : 1;
-            const int c_per_mask_group = modulated ? in_channels / n_mask_grps : 1;
+            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w;
+            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     input.scalar_type(), "arr2col_cpu", ([&] {
-                auto columns_accessor = columns.accessor<scalar_t, 4>();
-                TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                    arr2col_kernel<deformable, modulated>(
-                            n_kernels,
-                            input.accessor<scalar_t, 3>(),
-                            offset.accessor<scalar_t, 5>(),
-                            mask.accessor<scalar_t, 4>(),
-                            width,
-                            weight_w,
-                            pad_w,
-                            stride_w,
-                            dilation_w,
-                            out_w,
-                            in_channels,
-                            c_per_offset_group,
-                            c_per_mask_group,
-                            columns_accessor);
+                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                    auto columns_accessor =
+                            columns.accessor<scalar_t, 4>();
+                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                        arr2col_kernel<deformable, modulated, scalar_t, index_t>(
+                                n_kernels,
+                                input.accessor<scalar_t, 3>(),
+                                offset.accessor<scalar_t, 5>(),
+                                mask.accessor<scalar_t, 4>(),
+                                width,
+                                weight_w,
+                                pad_w,
+                                stride_w,
+                                dilation_w,
+                                out_w,
+                                in_channels,
+                                c_per_offset_group,
+                                c_per_mask_group,
+                                columns_accessor);
+                    }));
                 }));
             }));
         }
 
-        template<bool deformable, bool modulated, typename scalar_t>
+        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
         static void col2arr_kernel(
-                const int n_kernels,
+                const index_t n_kernels,
                 const at::TensorAccessor<scalar_t, 4> columns,
                 const at::TensorAccessor<scalar_t, 5> offset,
                 const at::TensorAccessor<scalar_t, 4> mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int pad_w,
-                const int stride_w,
-                const int dilation_w,
-                const int out_w,
-                const int c_per_offset_group,
-                const int c_per_mask_group,
+                const index_t in_channels,
+                const index_t width,
+                const index_t weight_w,
+                const index_t pad_w,
+                const index_t stride_w,
+                const index_t dilation_w,
+                const index_t out_w,
+                const index_t c_per_offset_group,
+                const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 3> grad_input) {
-            CPU_1D_KERNEL_LOOP(index, n_kernels) {
-                const int i = index % weight_w;
-                const int w = (index / weight_w) % out_w;
-                const int c = (index / (weight_w * out_w)) % in_channels;
-                const int b = (index / (weight_w * out_w * in_channels));
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                const index_t i = index % weight_w;
+                const index_t w = (index / weight_w) % out_w;
+                const index_t c = (index / (weight_w * out_w)) % in_channels;
+                const index_t b = (index / (weight_w * out_w * in_channels));
 
-                const int offset_group_idx = c / c_per_offset_group;
-                const int mask_group_idx = c / c_per_mask_group;
+                const index_t offset_group_idx = c / c_per_offset_group;
+                const index_t mask_group_idx = c / c_per_mask_group;
 
-                const int x = (w * stride_w - pad_w) + i * dilation_w;
+                const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
                 const scalar_t mask_val =
-                        modulated ?
-                        mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                        modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
 
                 const scalar_t val = columns[c][i][b][w] * mask_val;
 
                 if (deformable)
                     interpolate_insert(
                             grad_input, b, c, width,
                             x + offset[b][offset_group_idx][i][0][w],
@@ -234,85 +235,87 @@
                 const int width,
                 const int weight_w,
                 const int pad_w,
                 const int stride_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
-            const int n_kernels = batch_sz * in_channels * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / n_offset_grps : 1;
-            const int c_per_mask_group = modulated ? in_channels / n_mask_grps : 1;
+            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w * weight_w;
+            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "col2arr_cpu", ([&] {
-                auto grad_input_accessor = grad_input.accessor<scalar_t, 3>();
-                TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                    col2arr_kernel<deformable, modulated>(
-                            n_kernels,
-                            columns.accessor<scalar_t, 4>(),
-                            offset.accessor<scalar_t, 5>(),
-                            mask.accessor<scalar_t, 4>(),
-                            in_channels,
-                            width,
-                            weight_w,
-                            pad_w,
-                            stride_w,
-                            dilation_w,
-                            out_w,
-                            c_per_offset_group,
-                            c_per_mask_group,
-                            grad_input_accessor);
+                TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
+                    auto grad_input_accessor =
+                            grad_input.accessor<scalar_t, 3>();
+                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                        col2arr_kernel<deformable, modulated, scalar_t, index_t>(
+                                n_kernels,
+                                columns.accessor<scalar_t, 4>(),
+                                offset.accessor<scalar_t, 5>(),
+                                mask.accessor<scalar_t, 4>(),
+                                in_channels,
+                                width,
+                                weight_w,
+                                pad_w,
+                                stride_w,
+                                dilation_w,
+                                out_w,
+                                c_per_offset_group,
+                                c_per_mask_group,
+                                grad_input_accessor);
+                    }));
                 }));
             }));
         }
 
-        template<bool modulated, typename scalar_t>
+        template<bool modulated, typename scalar_t, typename index_t>
         static void deform_conv1d_compute_grad_offset_kernel(
-                const int n_kernels,
+                const index_t n_kernels,
                 const at::TensorAccessor<scalar_t, 4> columns,
                 const at::TensorAccessor<scalar_t, 3> input,
                 const at::TensorAccessor<scalar_t, 5> offset,
                 const at::TensorAccessor<scalar_t, 4> mask,
-                const int width,
-                const int weight_w,
-                const int pad_w,
-                const int stride_w,
-                const int dilation_w,
-                const int out_w,
-                const int n_offset_grps,
-                const int c_per_offset_group,
-                const int c_per_mask_group,
+                const index_t width,
+                const index_t weight_w,
+                const index_t pad_w,
+                const index_t stride_w,
+                const index_t dilation_w,
+                const index_t out_w,
+                const index_t offset_groups,
+                const index_t c_per_offset_group,
+                const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 5> grad_offset) {
-            CPU_1D_KERNEL_LOOP(index, n_kernels) {
-                const int i = index % weight_w;
-                const int w = (index / weight_w) % out_w;
-                const int g = (index / (weight_w * out_w)) % n_offset_grps;
-                const int b = index / (weight_w * out_w * n_offset_grps);
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                const index_t i = index % weight_w;
+                const index_t w = (index / weight_w) % out_w;
+                const index_t g = (index / (weight_w * out_w)) % offset_groups;
+                const index_t b = index / (weight_w * out_w * offset_groups);
 
                 scalar_t grad_offset_val = 0;
 
-                const int c_start = g * c_per_offset_group;
-                const int c_end = c_start + c_per_offset_group;
-                for (int c = c_start; c < c_end; ++c) {
-                    const int mask_group_idx = c / c_per_mask_group;
+                const index_t c_start = g * c_per_offset_group;
+                const index_t c_end = c_start + c_per_offset_group;
+                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t mask_group_idx = c / c_per_mask_group;
 
-                    const int x = (w * stride_w - pad_w) + i * dilation_w;
+                    const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
                     const scalar_t weight = coordinate_weight(
                             input, b, c, width,
                             x + offset[b][g][i][0][w]);
 
                     const scalar_t mask_val =
-                            modulated ?
-                            mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                            modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
 
                     grad_offset_val += columns[c][i][b][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][0][w] = grad_offset_val;
             }
         }
@@ -326,78 +329,81 @@
                 const int width,
                 const int weight_w,
                 const int pad_w,
                 const int stride_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (!deformable) return;
-            const int n_kernels = batch_sz * n_offset_grps * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / n_offset_grps : 1;
-            const int c_per_mask_group = modulated ? in_channels / n_mask_grps : 1;
+            const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_w * weight_w;
+            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv1d_compute_grad_offset_cpu", ([&] {
-                auto grad_offset_accessor = grad_offset.accessor<scalar_t, 5>();
-                TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                    deform_conv1d_compute_grad_offset_kernel<modulated>(
-                            n_kernels,
-                            columns.accessor<scalar_t, 4>(),
-                            input.accessor<scalar_t, 3>(),
-                            offset.accessor<scalar_t, 5>(),
-                            mask.accessor<scalar_t, 4>(),
-                            width,
-                            weight_w,
-                            pad_w,
-                            stride_w,
-                            dilation_w,
-                            out_w,
-                            n_offset_grps,
-                            c_per_offset_group,
-                            c_per_mask_group,
-                            grad_offset_accessor);
+                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                    auto grad_offset_accessor =
+                            grad_offset.accessor<scalar_t, 5>();
+                    TVDCN_DISPATCH_CONDITION(modulated, ([&] {
+                        deform_conv1d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
+                                n_kernels,
+                                columns.accessor<scalar_t, 4>(),
+                                input.accessor<scalar_t, 3>(),
+                                offset.accessor<scalar_t, 5>(),
+                                mask.accessor<scalar_t, 4>(),
+                                width,
+                                weight_w,
+                                pad_w,
+                                stride_w,
+                                dilation_w,
+                                out_w,
+                                offset_groups,
+                                c_per_offset_group,
+                                c_per_mask_group,
+                                grad_offset_accessor);
+                    }));
                 }));
             }));
         }
 
-        template<bool deformable, typename scalar_t>
+        template<bool deformable, typename scalar_t, typename index_t>
         static void deform_conv1d_compute_grad_mask_kernel(
-                const int n_kernels,
+                const index_t n_kernels,
                 const at::TensorAccessor<scalar_t, 4> columns,
                 const at::TensorAccessor<scalar_t, 3> input,
                 const at::TensorAccessor<scalar_t, 5> offset,
-                const int width,
-                const int weight_w,
-                const int pad_w,
-                const int stride_w,
-                const int dilation_w,
-                const int out_w,
-                const int n_mask_grps,
-                const int c_per_offset_group,
-                const int c_per_mask_group,
+                const index_t width,
+                const index_t weight_w,
+                const index_t pad_w,
+                const index_t stride_w,
+                const index_t dilation_w,
+                const index_t out_w,
+                const index_t mask_groups,
+                const index_t c_per_offset_group,
+                const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 4> grad_mask) {
-            CPU_1D_KERNEL_LOOP(index, n_kernels) {
-                const int i = index % weight_w;
-                const int w = (index / weight_w) % out_w;
-                const int g = (index / (weight_w * out_w)) % n_mask_grps;
-                const int b = index / (out_w * weight_w * n_mask_grps);
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                const index_t i = index % weight_w;
+                const index_t w = (index / weight_w) % out_w;
+                const index_t g = (index / (weight_w * out_w)) % mask_groups;
+                const index_t b = index / (out_w * weight_w * mask_groups);
 
                 scalar_t grad_mask_val = 0;
 
-                const int c_start = g * c_per_mask_group;
-                const int c_end = c_start + c_per_mask_group;
-                for (int c = c_start; c < c_end; ++c) {
-                    const int offset_group_idx = c / c_per_offset_group;
+                const index_t c_start = g * c_per_mask_group;
+                const index_t c_end = c_start + c_per_mask_group;
+                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t offset_group_idx = c / c_per_offset_group;
 
-                    const int x = (w * stride_w - pad_w) + i * dilation_w;
+                    const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
                     const scalar_t val =
                             deformable ?
                             interpolate_sample(
                                     input, b, c, width,
                                     x + offset[b][offset_group_idx][i][0][w])
                                        : sample(input, b, c, width, x);
@@ -417,41 +423,44 @@
                 const int width,
                 const int weight_w,
                 const int pad_w,
                 const int stride_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (!modulated) return;
-            const int n_kernels = batch_sz * n_mask_grps * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / n_offset_grps : 1;
-            const int c_per_mask_group = modulated ? in_channels / n_mask_grps : 1;
+            const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_w * weight_w;
+            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv1d_compute_grad_mask_cpu", ([&] {
-                auto grad_mask_accessor = grad_mask.accessor<scalar_t, 4>();
-                TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                    deform_conv1d_compute_grad_mask_kernel<deformable>(
-                            n_kernels,
-                            columns.accessor<scalar_t, 4>(),
-                            input.accessor<scalar_t, 3>(),
-                            offset.accessor<scalar_t, 5>(),
-                            width,
-                            weight_w,
-                            pad_w,
-                            stride_w,
-                            dilation_w,
-                            out_w,
-                            n_mask_grps,
-                            c_per_offset_group,
-                            c_per_mask_group,
-                            grad_mask_accessor);
+                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                    auto grad_mask_accessor =
+                            grad_mask.accessor<scalar_t, 4>();
+                    TVDCN_DISPATCH_CONDITION(deformable, ([&] {
+                        deform_conv1d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
+                                n_kernels,
+                                columns.accessor<scalar_t, 4>(),
+                                input.accessor<scalar_t, 3>(),
+                                offset.accessor<scalar_t, 5>(),
+                                width,
+                                weight_w,
+                                pad_w,
+                                stride_w,
+                                dilation_w,
+                                out_w,
+                                mask_groups,
+                                c_per_offset_group,
+                                c_per_mask_group,
+                                grad_mask_accessor);
+                    }));
                 }));
             }));
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,582 +1,752 @@
 #include <ATen/ATen.h>
 #include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ scalar_t sample(
-                    const at::TensorAccessor<scalar_t, 4> input,
-                    const int b,
-                    const int c,
-                    const int height,
-                    const int width,
-                    const int y,
-                    const int x) {
-                return (0 <= y && y < height && 0 <= x && x < width) ? input[b][c][y][x] : static_cast<scalar_t>(0);
+                    const at::TensorAccessor<scalar_t, 5> input,
+                    const index_t b,
+                    const index_t c,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const index_t z,
+                    const index_t y,
+                    const index_t x) {
+                return (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width) ?
+                       input[b][c][z][y][x] : static_cast<scalar_t>(0);
             }
 
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ scalar_t interpolate_sample(
-                    const at::TensorAccessor<scalar_t, 4> input,
-                    const int b,
-                    const int c,
-                    const int height,
-                    const int width,
+                    const at::TensorAccessor<scalar_t, 5> input,
+                    const index_t b,
+                    const index_t c,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const scalar_t z,
                     const scalar_t y,
                     const scalar_t x) {
-                if (y <= -1 || height <= y || x <= -1 || width <= x)
+                if (z <= -1 || depth <= z || y <= -1 || height <= y || x <= -1 || width <= x)
                     return 0;
 
-                int y_l = floor(y);
-                int y_h = y_l + 1;
-                int x_l = floor(x);
-                int x_h = x_l + 1;
+                index_t z_l = floor(z);
+                index_t z_h = z_l + 1;
+                index_t y_l = floor(y);
+                index_t y_h = y_l + 1;
+                index_t x_l = floor(x);
+                index_t x_h = x_l + 1;
 
+                scalar_t dz_h = z - z_l;
                 scalar_t dy_h = y - y_l;
                 scalar_t dx_h = x - x_l;
+                scalar_t dz_l = 1 - dz_h;
                 scalar_t dy_l = 1 - dy_h;
                 scalar_t dx_l = 1 - dx_h;
 
+                bool valid_z_l = z_l >= 0;
+                bool valid_z_h = z_h < depth;
                 bool valid_y_l = y_l >= 0;
                 bool valid_y_h = y_h < height;
                 bool valid_x_l = x_l >= 0;
                 bool valid_x_h = x_h < width;
 
                 scalar_t val = 0;
-                if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
-                if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
-                if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
-                if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
+                if (valid_z_l && valid_y_l && valid_x_l)
+                    val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
+                if (valid_z_l && valid_y_l && valid_x_h)
+                    val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
+                if (valid_z_l && valid_y_h && valid_x_l)
+                    val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
+                if (valid_z_l && valid_y_h && valid_x_h)
+                    val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
+                if (valid_z_h && valid_y_l && valid_x_l)
+                    val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
+                if (valid_z_h && valid_y_l && valid_x_h)
+                    val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
+                if (valid_z_h && valid_y_h && valid_x_l)
+                    val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
+                if (valid_z_h && valid_y_h && valid_x_h)
+                    val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
                 return val;
             }
 
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ void insert(
-                    at::TensorAccessor<scalar_t, 4> output,
-                    const int b,
-                    const int c,
-                    const int height,
-                    const int width,
-                    const int y,
-                    const int x,
+                    at::TensorAccessor<scalar_t, 5> output,
+                    const index_t b,
+                    const index_t c,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const index_t z,
+                    const index_t y,
+                    const index_t x,
                     const scalar_t val) {
-                if (0 <= y && y < height && 0 <= x && x < width)
-                    output[b][c][y][x] += val;
+                if (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width)
+                    output[b][c][z][y][x] += val;
             }
 
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ void interpolate_insert(
-                    at::TensorAccessor<scalar_t, 4> output,
-                    const int b,
-                    const int c,
-                    const int height,
-                    const int width,
+                    at::TensorAccessor<scalar_t, 5> output,
+                    const index_t b,
+                    const index_t c,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const scalar_t z,
                     const scalar_t y,
                     const scalar_t x,
                     const scalar_t val) {
-                int y_l = floor(y);
-                int y_h = y_l + 1;
-                int x_l = floor(x);
-                int x_h = x_l + 1;
+                index_t z_l = floor(z);
+                index_t z_h = z_l + 1;
+                index_t y_l = floor(y);
+                index_t y_h = y_l + 1;
+                index_t x_l = floor(x);
+                index_t x_h = x_l + 1;
 
+                scalar_t dz_h = z - z_l;
                 scalar_t dy_h = y - y_l;
                 scalar_t dx_h = x - x_l;
+                scalar_t dz_l = 1 - dz_h;
                 scalar_t dy_l = 1 - dy_h;
                 scalar_t dx_l = 1 - dx_h;
 
+                bool valid_z_l = 0 <= z_l && z_l < depth;
+                bool valid_z_h = 0 <= z_h && z_h < depth;
                 bool valid_y_l = 0 <= y_l && y_l < height;
                 bool valid_y_h = 0 <= y_h && y_h < height;
                 bool valid_x_l = 0 <= x_l && x_l < width;
                 bool valid_x_h = 0 <= x_h && x_h < width;
 
-                if (valid_y_l && valid_x_l) output[b][c][y_l][x_l] += dy_l * dx_l * val;
-                if (valid_y_l && valid_x_h) output[b][c][y_l][x_h] += dy_l * dx_h * val;
-                if (valid_y_h && valid_x_l) output[b][c][y_h][x_l] += dy_h * dx_l * val;
-                if (valid_y_h && valid_x_h) output[b][c][y_h][x_h] += dy_h * dx_h * val;
+                if (valid_z_l && valid_y_l && valid_x_l)
+                    output[b][c][z_l][y_l][x_l] += dz_l * dy_l * dx_l * val;
+                if (valid_z_l && valid_y_l && valid_x_h)
+                    output[b][c][z_l][y_l][x_h] += dz_l * dy_l * dx_h * val;
+                if (valid_z_l && valid_y_h && valid_x_l)
+                    output[b][c][z_l][y_h][x_l] += dz_l * dy_h * dx_l * val;
+                if (valid_z_l && valid_y_h && valid_x_h)
+                    output[b][c][z_l][y_h][x_h] += dz_l * dy_h * dx_h * val;
+                if (valid_z_h && valid_y_l && valid_x_l)
+                    output[b][c][z_h][y_l][x_l] += dz_h * dy_l * dx_l * val;
+                if (valid_z_h && valid_y_l && valid_x_h)
+                    output[b][c][z_h][y_l][x_h] += dz_h * dy_l * dx_h * val;
+                if (valid_z_h && valid_y_h && valid_x_l)
+                    output[b][c][z_h][y_h][x_l] += dz_h * dy_h * dx_l * val;
+                if (valid_z_h && valid_y_h && valid_x_h)
+                    output[b][c][z_h][y_h][x_h] += dz_h * dy_h * dx_h * val;
             }
 
-            template<typename scalar_t>
+            template<typename scalar_t, typename index_t>
             __forceinline__ scalar_t coordinate_weight(
-                    const at::TensorAccessor<scalar_t, 4> input,
-                    const int b,
-                    const int c,
-                    const int height,
-                    const int width,
+                    const at::TensorAccessor<scalar_t, 5> input,
+                    const index_t b,
+                    const index_t c,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const scalar_t z,
                     const scalar_t y,
                     const scalar_t x,
-                    const int direction) {
-                int y_l = floor(y);
-                int y_h = y_l + 1;
-                int x_l = floor(x);
-                int x_h = x_l + 1;
-
-                scalar_t dy_h = (direction == 0) ? static_cast<scalar_t>(1) : y - y_l;
-                scalar_t dy_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dy_h;
-                scalar_t dx_h = (direction == 1) ? static_cast<scalar_t>(1) : x - x_l;
-                scalar_t dx_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dx_h;
+                    const index_t direction) {
+                index_t z_l = floor(z);
+                index_t z_h = z_l + 1;
+                index_t y_l = floor(y);
+                index_t y_h = y_l + 1;
+                index_t x_l = floor(x);
+                index_t x_h = x_l + 1;
+
+                scalar_t dz_h = (direction == 0) ? static_cast<scalar_t>(1) : z - z_l;
+                scalar_t dy_h = (direction == 1) ? static_cast<scalar_t>(1) : y - y_l;
+                scalar_t dx_h = (direction == 2) ? static_cast<scalar_t>(1) : x - x_l;
+                scalar_t dz_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dz_h;
+                scalar_t dy_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dy_h;
+                scalar_t dx_l = (direction == 2) ? static_cast<scalar_t>(-1) : 1 - dx_h;
 
+                bool valid_z_l = 0 <= z_l && z_l < depth;
+                bool valid_z_h = 0 <= z_h && z_h < depth;
                 bool valid_y_l = 0 <= y_l && y_l < height;
                 bool valid_y_h = 0 <= y_h && y_h < height;
                 bool valid_x_l = 0 <= x_l && x_l < width;
                 bool valid_x_h = 0 <= x_h && x_h < width;
 
                 scalar_t val = 0;
-                if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
-                if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
-                if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
-                if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
+                if (valid_z_l && valid_y_l && valid_x_l)
+                    val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
+                if (valid_z_l && valid_y_l && valid_x_h)
+                    val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
+                if (valid_z_l && valid_y_h && valid_x_l)
+                    val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
+                if (valid_z_l && valid_y_h && valid_x_h)
+                    val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
+                if (valid_z_h && valid_y_l && valid_x_l)
+                    val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
+                if (valid_z_h && valid_y_l && valid_x_h)
+                    val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
+                if (valid_z_h && valid_y_h && valid_x_l)
+                    val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
+                if (valid_z_h && valid_y_h && valid_x_h)
+                    val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
                 return val;
             }
         }
 
-        template<bool deformable, bool modulated, typename scalar_t>
-        static void im2col_kernel(
-                const int n_kernels,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int pad_h,
-                const int pad_w,
-                const int stride_h,
-                const int stride_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int in_channels,
-                const int c_per_offset_group,
-                const int c_per_mask_group,
-                at::TensorAccessor<scalar_t, 6> columns) {
-            CPU_1D_KERNEL_LOOP(index, n_kernels) {
-                const int w = index % out_w;
-                const int h = (index / out_w) % out_h;
-                const int c = (index / (out_w * out_h)) % in_channels;
-                const int b = index / (out_w * out_h * in_channels);
-
-                const int offset_group_idx = c / c_per_offset_group;
-                const int mask_group_idx = c / c_per_mask_group;
-
-                for (int i = 0; i < weight_h; ++i) {
-                    for (int j = 0; j < weight_w; ++j) {
-                        const int y = (h * stride_h - pad_h) + i * dilation_h;
-                        const int x = (w * stride_w - pad_w) + j * dilation_w;
-
-                        const scalar_t val =
-                                deformable ?
-                                interpolate_sample(
-                                        input, b, c, height, width,
-                                        y + offset[b][offset_group_idx][i][j][0][h][w],
-                                        x + offset[b][offset_group_idx][i][j][1][h][w])
-                                           : sample(input, b, c, height, width, y, x);
-
-                        const scalar_t mask_val =
-                                modulated ? mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+        static void vol2col_kernel(
+                const index_t n_kernels,
+                const at::TensorAccessor<scalar_t, 5> input,
+                const at::TensorAccessor<scalar_t, 9> offset,
+                const at::TensorAccessor<scalar_t, 8> mask,
+                const index_t depth,
+                const index_t height,
+                const index_t width,
+                const index_t weight_d,
+                const index_t weight_h,
+                const index_t weight_w,
+                const index_t pad_d,
+                const index_t pad_h,
+                const index_t pad_w,
+                const index_t stride_d,
+                const index_t stride_h,
+                const index_t stride_w,
+                const index_t dilation_d,
+                const index_t dilation_h,
+                const index_t dilation_w,
+                const index_t out_d,
+                const index_t out_h,
+                const index_t out_w,
+                const index_t in_channels,
+                const index_t c_per_offset_group,
+                const index_t c_per_mask_group,
+                at::TensorAccessor<scalar_t, 8> columns) {
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                const index_t w = index % out_w;
+                const index_t h = (index / out_w) % out_h;
+                const index_t d = (index / (out_w * out_h)) % out_d;
+                const index_t c = (index / (out_w * out_h * out_d)) % in_channels;
+                const index_t b = index / (out_w * out_h * out_d * in_channels);
+
+                const index_t offset_group_idx = c / c_per_offset_group;
+                const index_t mask_group_idx = c / c_per_mask_group;
+
+                for (index_t i = 0; i < weight_d; ++i) {
+                    for (index_t j = 0; j < weight_h; ++j) {
+                        for (index_t k = 0; k < weight_w; ++k) {
+                            const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                            const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                            const index_t x = (w * stride_w - pad_w) + k * dilation_w;
+
+                            const scalar_t val =
+                                    deformable ?
+                                    interpolate_sample(
+                                            input, b, c, depth, height, width,
+                                            z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                            y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                            x + offset[b][offset_group_idx][i][j][k][2][d][h][w])
+                                               : sample(input, b, c, depth, height, width, z, y, x);
+
+                            const scalar_t mask_val =
+                                    modulated ?
+                                    mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
 
-                        columns[c][i][j][b][h][w] = val * mask_val;
+                            columns[c][i][j][k][b][d][h][w] = val * mask_val;
+                        }
                     }
                 }
             }
         }
 
-        void im2col_cpu(
+        void vol2col_cpu(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
+                const int depth,
                 const int height,
                 const int width,
+                const int weight_d,
                 const int weight_h,
                 const int weight_w,
+                const int pad_d,
                 const int pad_h,
                 const int pad_w,
+                const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
+                const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
-            const int n_kernels = in_channels * out_h * out_w * batch_sz;
-            const int c_per_offset_group = deformable ? in_channels / n_offset_grps : 1;
-            const int c_per_mask_group = modulated ? in_channels / n_mask_grps : 1;
+            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_d * out_h * out_w;
+            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "im2col_cpu", ([&] {
-                auto columns_accessor = columns.accessor<scalar_t, 6>();
-                TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                    im2col_kernel<deformable, modulated>(
-                            n_kernels,
-                            input.accessor<scalar_t, 4>(),
-                            offset.accessor<scalar_t, 7>(),
-                            mask.accessor<scalar_t, 6>(),
-                            height,
-                            width,
-                            weight_h,
-                            weight_w,
-                            pad_h,
-                            pad_w,
-                            stride_h,
-                            stride_w,
-                            dilation_h,
-                            dilation_w,
-                            out_h,
-                            out_w,
-                            in_channels,
-                            c_per_offset_group,
-                            c_per_mask_group,
-                            columns_accessor);
+                    input.scalar_type(), "vol2col_cpu", ([&] {
+                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                    auto columns_accessor =
+                            columns.accessor<scalar_t, 8>();
+                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                        vol2col_kernel<deformable, modulated, scalar_t, index_t>(
+                                n_kernels,
+                                input.accessor<scalar_t, 5>(),
+                                offset.accessor<scalar_t, 9>(),
+                                mask.accessor<scalar_t, 8>(),
+                                depth,
+                                height,
+                                width,
+                                weight_d,
+                                weight_h,
+                                weight_w,
+                                pad_d,
+                                pad_h,
+                                pad_w,
+                                stride_d,
+                                stride_h,
+                                stride_w,
+                                dilation_d,
+                                dilation_h,
+                                dilation_w,
+                                out_d,
+                                out_h,
+                                out_w,
+                                in_channels,
+                                c_per_offset_group,
+                                c_per_mask_group,
+                                columns_accessor);
+                    }));
                 }));
             }));
         }
 
-        template<bool deformable, bool modulated, typename scalar_t>
-        static void col2im_kernel(
-                const int n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int pad_h,
-                const int pad_w,
-                const int stride_h,
-                const int stride_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int c_per_offset_group,
-                const int c_per_mask_group,
-                at::TensorAccessor<scalar_t, 4> grad_input) {
-            CPU_1D_KERNEL_LOOP(index, n_kernels) {
-                const int j = index % weight_w;
-                const int i = (index / weight_w) % weight_h;
-                const int w = (index / (weight_w * weight_h)) % out_w;
-                const int h = (index / (weight_w * weight_h * out_w)) % out_h;
-                const int c = (index / (weight_w * weight_h * out_w * out_h)) % in_channels;
-                const int b = (index / (weight_w * weight_h * out_w * out_h * in_channels));
-
-                const int offset_group_idx = c / c_per_offset_group;
-                const int mask_group_idx = c / c_per_mask_group;
-
-                const int y = (h * stride_h - pad_h) + i * dilation_h;
-                const int x = (w * stride_w - pad_w) + j * dilation_w;
+        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+        static void col2vol_kernel(
+                const index_t n_kernels,
+                const at::TensorAccessor<scalar_t, 8> columns,
+                const at::TensorAccessor<scalar_t, 9> offset,
+                const at::TensorAccessor<scalar_t, 8> mask,
+                const index_t in_channels,
+                const index_t depth,
+                const index_t height,
+                const index_t width,
+                const index_t weight_d,
+                const index_t weight_h,
+                const index_t weight_w,
+                const index_t pad_d,
+                const index_t pad_h,
+                const index_t pad_w,
+                const index_t stride_d,
+                const index_t stride_h,
+                const index_t stride_w,
+                const index_t dilation_d,
+                const index_t dilation_h,
+                const index_t dilation_w,
+                const index_t out_d,
+                const index_t out_h,
+                const index_t out_w,
+                const index_t c_per_offset_group,
+                const index_t c_per_mask_group,
+                at::TensorAccessor<scalar_t, 5> grad_input) {
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                const index_t k = index % weight_w;
+                const index_t j = (index / weight_w) % weight_h;
+                const index_t i = (index / (weight_w * weight_h)) % weight_d;
+                const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
+                const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
+                const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                const index_t c = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % in_channels;
+                const index_t b = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * in_channels));
+
+                const index_t offset_group_idx = c / c_per_offset_group;
+                const index_t mask_group_idx = c / c_per_mask_group;
+
+                const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
                 const scalar_t mask_val =
-                        modulated ?
-                        mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+                        modulated ? mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
 
-                const scalar_t val = columns[c][i][j][b][h][w] * mask_val;
+                const scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
 
                 if (deformable)
                     interpolate_insert(
-                            grad_input, b, c, height, width,
-                            y + offset[b][offset_group_idx][i][j][0][h][w],
-                            x + offset[b][offset_group_idx][i][j][1][h][w],
+                            grad_input, b, c, depth, height, width,
+                            z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                            y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                            x + offset[b][offset_group_idx][i][j][k][2][d][h][w],
                             val);
                 else
-                    insert(grad_input, b, c, height, width, y, x, val);
+                    insert(grad_input, b, c, depth, height, width, z, y, x, val);
             }
         }
 
-        void col2im_cpu(
+        void col2vol_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
+                const int depth,
                 const int height,
                 const int width,
+                const int weight_d,
                 const int weight_h,
                 const int weight_w,
+                const int pad_d,
                 const int pad_h,
                 const int pad_w,
+                const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
+                const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
-            const int n_kernels = batch_sz * in_channels * out_h * out_w * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / n_offset_grps : 1;
-            const int c_per_mask_group = modulated ? in_channels / n_mask_grps : 1;
+            const int64_t n_kernels =
+                    (int64_t) batch_sz * in_channels * out_d * out_h * out_w * weight_d * weight_h * weight_w;
+            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2im_cpu", ([&] {
-                auto grad_input_accessor = grad_input.accessor<scalar_t, 4>();
-                TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                    col2im_kernel<deformable, modulated>(
-                            n_kernels,
-                            columns.accessor<scalar_t, 6>(),
-                            offset.accessor<scalar_t, 7>(),
-                            mask.accessor<scalar_t, 6>(),
-                            in_channels,
-                            height,
-                            width,
-                            weight_h,
-                            weight_w,
-                            pad_h,
-                            pad_w,
-                            stride_h,
-                            stride_w,
-                            dilation_h,
-                            dilation_w,
-                            out_h,
-                            out_w,
-                            c_per_offset_group,
-                            c_per_mask_group,
-                            grad_input_accessor);
+                    columns.scalar_type(), "col2vol_cpu", ([&] {
+                TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
+                    auto grad_input_accessor =
+                            grad_input.accessor<scalar_t, 5>();
+                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                        col2vol_kernel<deformable, modulated, scalar_t, index_t>(
+                                n_kernels,
+                                columns.accessor<scalar_t, 8>(),
+                                offset.accessor<scalar_t, 9>(),
+                                mask.accessor<scalar_t, 8>(),
+                                in_channels,
+                                depth,
+                                height,
+                                width,
+                                weight_d,
+                                weight_h,
+                                weight_w,
+                                pad_d,
+                                pad_h,
+                                pad_w,
+                                stride_d,
+                                stride_h,
+                                stride_w,
+                                dilation_d,
+                                dilation_h,
+                                dilation_w,
+                                out_d,
+                                out_h,
+                                out_w,
+                                c_per_offset_group,
+                                c_per_mask_group,
+                                grad_input_accessor);
+                    }));
                 }));
             }));
         }
 
-        template<bool modulated, typename scalar_t>
-        static void deform_conv2d_compute_grad_offset_kernel(
-                const int n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int pad_h,
-                const int pad_w,
-                const int stride_h,
-                const int stride_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int n_offset_grps,
-                const int c_per_offset_group,
-                const int c_per_mask_group,
-                at::TensorAccessor<scalar_t, 7> grad_offset) {
-            CPU_1D_KERNEL_LOOP(index, n_kernels) {
-                const int o = index % 2;
-                const int j = (index / 2) % weight_w;
-                const int i = (index / (2 * weight_w)) % weight_h;
-                const int w = (index / (2 * weight_w * weight_h)) % out_w;
-                const int h = (index / (2 * weight_w * weight_h * out_w)) % out_h;
-                const int g = (index / (2 * weight_w * weight_h * out_w * out_h)) % n_offset_grps;
-                const int b = index / (2 * weight_w * weight_h * out_w * out_h * n_offset_grps);
+        template<bool modulated, typename scalar_t, typename index_t>
+        static void deform_conv3d_compute_grad_offset_kernel(
+                const index_t n_kernels,
+                const at::TensorAccessor<scalar_t, 8> columns,
+                const at::TensorAccessor<scalar_t, 5> input,
+                const at::TensorAccessor<scalar_t, 9> offset,
+                const at::TensorAccessor<scalar_t, 8> mask,
+                const index_t depth,
+                const index_t height,
+                const index_t width,
+                const index_t weight_d,
+                const index_t weight_h,
+                const index_t weight_w,
+                const index_t pad_d,
+                const index_t pad_h,
+                const index_t pad_w,
+                const index_t stride_d,
+                const index_t stride_h,
+                const index_t stride_w,
+                const index_t dilation_d,
+                const index_t dilation_h,
+                const index_t dilation_w,
+                const index_t out_d,
+                const index_t out_h,
+                const index_t out_w,
+                const index_t offset_groups,
+                const index_t c_per_offset_group,
+                const index_t c_per_mask_group,
+                at::TensorAccessor<scalar_t, 9> grad_offset) {
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                const index_t o = index % 3;
+                const index_t k = (index / 3) % weight_w;
+                const index_t j = (index / (3 * weight_w)) % weight_h;
+                const index_t i = (index / (3 * weight_w * weight_h)) % weight_d;
+                const index_t w = (index / (3 * weight_w * weight_h * weight_d)) % out_w;
+                const index_t h = (index / (3 * weight_w * weight_h * weight_d * out_w)) % out_h;
+                const index_t d = (index / (3 * weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                const index_t g =
+                        (index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d)) % offset_groups;
+                const index_t b = index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d * offset_groups);
 
                 scalar_t grad_offset_val = 0;
 
-                const int c_start = g * c_per_offset_group;
-                const int c_end = c_start + c_per_offset_group;
-                for (int c = c_start; c < c_end; ++c) {
-                    const int mask_group_idx = c / c_per_mask_group;
-
-                    const int y = (h * stride_h - pad_h) + i * dilation_h;
-                    const int x = (w * stride_w - pad_w) + j * dilation_w;
-
-                    const scalar_t weight = coordinate_weight(
-                            input, b, c, height, width,
-                            y + offset[b][g][i][j][0][h][w],
-                            x + offset[b][g][i][j][1][h][w],
-                            o);
+                const index_t c_start = g * c_per_offset_group;
+                const index_t c_end = c_start + c_per_offset_group;
+                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t mask_group_idx = c / c_per_mask_group;
+
+                    const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                    const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                    const index_t x = (w * stride_w - pad_w) + k * dilation_w;
+
+                    const scalar_t weight =
+                            coordinate_weight(
+                                    input, b, c, depth, height, width,
+                                    z + offset[b][g][i][j][k][0][d][h][w],
+                                    y + offset[b][g][i][j][k][1][d][h][w],
+                                    x + offset[b][g][i][j][k][2][d][h][w],
+                                    o);
 
                     const scalar_t mask_val =
-                            modulated ?
-                            mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+                            modulated ? mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
 
-                    grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
+                    grad_offset_val += columns[c][i][j][k][b][d][h][w] * weight * mask_val;
                 }
 
-                grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
+                grad_offset[b][g][i][j][k][o][d][h][w] = grad_offset_val;
             }
         }
 
-        void deform_conv2d_compute_grad_offset_cpu(
+        void deform_conv3d_compute_grad_offset_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
+                const int depth,
                 const int height,
                 const int width,
+                const int weight_d,
                 const int weight_h,
                 const int weight_w,
+                const int pad_d,
                 const int pad_h,
                 const int pad_w,
+                const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
+                const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (!deformable) return;
-            const int n_kernels = batch_sz * n_offset_grps * out_h * out_w * weight_h * weight_w * 2;
-            const int c_per_offset_group = deformable ? in_channels / n_offset_grps : 1;
-            const int c_per_mask_group = modulated ? in_channels / n_mask_grps : 1;
+            const int64_t n_kernels =
+                    (int64_t) batch_sz * offset_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w * 3;
+            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_offset_cpu", ([&] {
-                auto grad_offset_accessor = grad_offset.accessor<scalar_t, 7>();
-                TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                    deform_conv2d_compute_grad_offset_kernel<modulated>(
-                            n_kernels,
-                            columns.accessor<scalar_t, 6>(),
-                            input.accessor<scalar_t, 4>(),
-                            offset.accessor<scalar_t, 7>(),
-                            mask.accessor<scalar_t, 6>(),
-                            height,
-                            width,
-                            weight_h,
-                            weight_w,
-                            pad_h,
-                            pad_w,
-                            stride_h,
-                            stride_w,
-                            dilation_h,
-                            dilation_w,
-                            out_h,
-                            out_w,
-                            n_offset_grps,
-                            c_per_offset_group,
-                            c_per_mask_group,
-                            grad_offset_accessor);
+                    columns.scalar_type(), "deform_conv3d_compute_grad_offset_cpu", ([&] {
+                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                    auto grad_offset_accessor =
+                            grad_offset.accessor<scalar_t, 9>();
+                    TVDCN_DISPATCH_CONDITION(modulated, ([&] {
+                        deform_conv3d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
+                                n_kernels,
+                                columns.accessor<scalar_t, 8>(),
+                                input.accessor<scalar_t, 5>(),
+                                offset.accessor<scalar_t, 9>(),
+                                mask.accessor<scalar_t, 8>(),
+                                depth,
+                                height,
+                                width,
+                                weight_d,
+                                weight_h,
+                                weight_w,
+                                pad_d,
+                                pad_h,
+                                pad_w,
+                                stride_d,
+                                stride_h,
+                                stride_w,
+                                dilation_d,
+                                dilation_h,
+                                dilation_w,
+                                out_d,
+                                out_h,
+                                out_w,
+                                offset_groups,
+                                c_per_offset_group,
+                                c_per_mask_group,
+                                grad_offset_accessor);
+                    }));
                 }));
             }));
         }
 
-        template<bool deformable, typename scalar_t>
-        static void deform_conv2d_compute_grad_mask_kernel(
-                const int n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int pad_h,
-                const int pad_w,
-                const int stride_h,
-                const int stride_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int n_mask_grps,
-                const int c_per_offset_group,
-                const int c_per_mask_group,
-                at::TensorAccessor<scalar_t, 6> grad_mask) {
-            CPU_1D_KERNEL_LOOP(index, n_kernels) {
-                const int j = index % weight_w;
-                const int i = (index / weight_w) % weight_h;
-                const int w = (index / (weight_w * weight_h)) % out_w;
-                const int h = (index / (weight_w * weight_h * out_w)) % out_h;
-                const int g = (index / (weight_w * weight_h * out_w * out_h)) % n_mask_grps;
-                const int b = index / (out_w * out_h * weight_w * weight_h * n_mask_grps);
+        template<bool deformable, typename scalar_t, typename index_t>
+        static void deform_conv3d_compute_grad_mask_kernel(
+                const index_t n_kernels,
+                const at::TensorAccessor<scalar_t, 8> columns,
+                const at::TensorAccessor<scalar_t, 5> input,
+                const at::TensorAccessor<scalar_t, 9> offset,
+                const index_t depth,
+                const index_t height,
+                const index_t width,
+                const index_t weight_d,
+                const index_t weight_h,
+                const index_t weight_w,
+                const index_t pad_d,
+                const index_t pad_h,
+                const index_t pad_w,
+                const index_t stride_d,
+                const index_t stride_h,
+                const index_t stride_w,
+                const index_t dilation_d,
+                const index_t dilation_h,
+                const index_t dilation_w,
+                const index_t out_d,
+                const index_t out_h,
+                const index_t out_w,
+                const index_t mask_groups,
+                const index_t c_per_offset_group,
+                const index_t c_per_mask_group,
+                at::TensorAccessor<scalar_t, 8> grad_mask) {
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                const index_t k = index % weight_w;
+                const index_t j = (index / weight_w) % weight_h;
+                const index_t i = (index / (weight_w * weight_h)) % weight_d;
+                const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
+                const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
+                const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                const index_t g = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % mask_groups;
+                const index_t b = index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * mask_groups);
 
                 scalar_t grad_mask_val = 0;
 
-                const int c_start = g * c_per_mask_group;
-                const int c_end = c_start + c_per_mask_group;
-                for (int c = c_start; c < c_end; ++c) {
-                    const int offset_group_idx = c / c_per_offset_group;
-
-                    const int y = (h * stride_h - pad_h) + i * dilation_h;
-                    const int x = (w * stride_w - pad_w) + j * dilation_w;
+                const index_t c_start = g * c_per_mask_group;
+                const index_t c_end = c_start + c_per_mask_group;
+                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t offset_group_idx = c / c_per_offset_group;
+
+                    const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                    const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                    const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
                     const scalar_t val =
                             deformable ?
                             interpolate_sample(
-                                    input, b, c, height, width,
-                                    y + offset[b][offset_group_idx][i][j][0][h][w],
-                                    x + offset[b][offset_group_idx][i][j][1][h][w])
-                                       : sample(input, b, c, height, width, y, x);
+                                    input, b, c, depth, height, width,
+                                    z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                    y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                    x + offset[b][offset_group_idx][i][j][k][2][d][h][w])
+                                       : sample(input, b, c, depth, height, width, z, y, x);
 
-                    grad_mask_val += columns[c][i][j][b][h][w] * val;
+                    grad_mask_val += columns[c][i][j][k][b][d][h][w] * val;
                 }
 
-                grad_mask[b][g][i][j][h][w] = grad_mask_val;
+                grad_mask[b][g][i][j][k][d][h][w] = grad_mask_val;
             }
         }
 
-        void deform_conv2d_compute_grad_mask_cpu(
+        void deform_conv3d_compute_grad_mask_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const int in_channels,
+                const int depth,
                 const int height,
                 const int width,
+                const int weight_d,
                 const int weight_h,
                 const int weight_w,
+                const int pad_d,
                 const int pad_h,
                 const int pad_w,
+                const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
+                const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (!modulated) return;
-            const int n_kernels = batch_sz * n_mask_grps * out_h * out_w * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / n_offset_grps : 1;
-            const int c_per_mask_group = modulated ? in_channels / n_mask_grps : 1;
+            const int64_t n_kernels =
+                    (int64_t) batch_sz * mask_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w;
+            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_mask_cpu", ([&] {
-                auto grad_mask_accessor = grad_mask.accessor<scalar_t, 6>();
-                TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                    deform_conv2d_compute_grad_mask_kernel<deformable>(
-                            n_kernels,
-                            columns.accessor<scalar_t, 6>(),
-                            input.accessor<scalar_t, 4>(),
-                            offset.accessor<scalar_t, 7>(),
-                            height,
-                            width,
-                            weight_h,
-                            weight_w,
-                            pad_h,
-                            pad_w,
-                            stride_h,
-                            stride_w,
-                            dilation_h,
-                            dilation_w,
-                            out_h,
-                            out_w,
-                            n_mask_grps,
-                            c_per_offset_group,
-                            c_per_mask_group,
-                            grad_mask_accessor);
+                    columns.scalar_type(), "deform_conv3d_compute_grad_mask_cpu", ([&] {
+                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                    auto grad_mask_accessor =
+                            grad_mask.accessor<scalar_t, 8>();
+                    TVDCN_DISPATCH_CONDITION(deformable, ([&] {
+                        deform_conv3d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
+                                n_kernels,
+                                columns.accessor<scalar_t, 8>(),
+                                input.accessor<scalar_t, 5>(),
+                                offset.accessor<scalar_t, 9>(),
+                                depth,
+                                height,
+                                width,
+                                weight_d,
+                                weight_h,
+                                weight_w,
+                                pad_d,
+                                pad_h,
+                                pad_w,
+                                stride_d,
+                                stride_h,
+                                stride_w,
+                                dilation_d,
+                                dilation_h,
+                                dilation_w,
+                                out_d,
+                                out_h,
+                                out_w,
+                                mask_groups,
+                                c_per_offset_group,
+                                c_per_mask_group,
+                                grad_mask_accessor);
+                    }));
                 }));
             }));
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -76,36 +76,33 @@
     namespace ops {
         at::Tensor deform_conv1d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                int stride,
-                int padding,
-                int dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int stride,
+                const int padding,
+                const int dilation,
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 3)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
             TORCH_CHECK(weight_c.ndimension() == 3)
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_w = input_c.size(2);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
             int out_channels = weight_c.size(0);
@@ -184,20 +181,28 @@
             if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_w,
                                           1,
                                           out_w});
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_w,
                                       out_w});
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0});
             out = out.view({batch_sz / n_parallel_imgs,
                             n_parallel_imgs,
                             out_channels,
                             out_w});
             auto out_buf = at::zeros(
                     {batch_sz / n_parallel_imgs,
                      out_channels,
@@ -264,32 +269,29 @@
         deform_conv1d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                int stride,
-                int padding,
-                int dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int stride,
+                const int padding,
+                const int dilation,
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_w = input_c.size(2);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
             int out_channels = weight_c.size(0);
@@ -311,31 +313,33 @@
 
             // Separate into blocks
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
-            if (deformable) {
+            if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_w,
                                           1,
                                           out_w});
-                grad_offset = grad_offset.view_as(offset_c);
-            }
-            if (modulated) {
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0});
+            grad_offset = grad_offset.view_as(offset_c);
+            if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_w,
                                       out_w});
-                grad_mask = grad_mask.view_as(mask_c);
-            }
+            grad_mask = grad_mask.view_as(mask_c);
 
             // Separate channels into convolution groups
             grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           groups,
                                           out_channels / groups,
                                           out_w}).permute({0, 2, 3, 1, 4}).contiguous();
@@ -431,32 +435,23 @@
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
+
                 for (int g = 0; g < groups; g++) {
                     grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
                 }
             }
 
-            grad_input = grad_input.view({batch_sz,
-                                          in_channels,
-                                          in_w});
-            grad_weight = grad_weight.view({out_channels,
-                                            in_channels / groups,
-                                            weight_w});
-            if (deformable)
-                grad_offset = grad_offset.view({batch_sz,
-                                                offset_groups * weight_w,
-                                                out_w});
-            if (modulated)
-                grad_mask = grad_mask.view({batch_sz,
-                                            mask_groups * weight_w,
-                                            out_w});
+            grad_input = grad_input.view_as(input);
+            grad_weight = grad_weight.view_as(weight);
+            grad_offset = grad_offset.view_as(offset);
+            grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -79,33 +79,30 @@
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::pair<int, int> &stride,
                 const std::pair<int, int> &padding,
                 const std::pair<int, int> &dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 4)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
             TORCH_CHECK(weight_c.ndimension() == 4)
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_h = input_c.size(2);
             int in_w = input_c.size(3);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
@@ -207,22 +204,30 @@
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_h,
                                           weight_w,
                                           2,
                                           out_h,
                                           out_w});
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_h,
                                       weight_w,
                                       out_h,
                                       out_w});
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0, 0, 0});
             out = out.view({batch_sz / n_parallel_imgs,
                             n_parallel_imgs,
                             out_channels,
                             out_h,
                             out_w});
             auto out_buf = at::zeros(
                     {batch_sz / n_parallel_imgs,
@@ -305,29 +310,26 @@
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::pair<int, int> &stride,
                 const std::pair<int, int> &padding,
                 const std::pair<int, int> &dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_h = input_c.size(2);
             int in_w = input_c.size(3);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
@@ -356,35 +358,41 @@
             // Separate into blocks
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_h,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
-            if (deformable) {
+            if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_h,
                                           weight_w,
                                           2,
                                           out_h,
                                           out_w});
-                grad_offset = grad_offset.view_as(offset_c);
-            }
-            if (modulated) {
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0});
+            grad_offset = grad_offset.view_as(offset_c);
+            if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_h,
                                       weight_w,
                                       out_h,
                                       out_w});
-                grad_mask = grad_mask.view_as(mask_c);
-            }
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0, 0, 0});
+            grad_mask = grad_mask.view_as(mask_c);
 
             // Separate channels into convolution groups
             grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           groups,
                                           out_channels / groups,
                                           out_h,
@@ -508,36 +516,23 @@
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
+
                 for (int g = 0; g < groups; g++) {
                     grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
                 }
             }
 
-            grad_input = grad_input.view({batch_sz,
-                                          in_channels,
-                                          in_h,
-                                          in_w});
-            grad_weight = grad_weight.view({out_channels,
-                                            in_channels / groups,
-                                            weight_h,
-                                            weight_w});
-            if (deformable)
-                grad_offset = grad_offset.view({batch_sz,
-                                                offset_groups * 2 * weight_h * weight_w,
-                                                out_h,
-                                                out_w});
-            if (modulated)
-                grad_mask = grad_mask.view({batch_sz,
-                                            mask_groups * weight_h * weight_w,
-                                            out_h,
-                                            out_w});
+            grad_input = grad_input.view_as(input);
+            grad_weight = grad_weight.view_as(weight);
+            grad_offset = grad_offset.view_as(offset);
+            grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -79,33 +79,30 @@
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::tuple<int, int, int> &stride,
                 const std::tuple<int, int, int> &padding,
                 const std::tuple<int, int, int> &dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 5)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
             TORCH_CHECK(weight_c.ndimension() == 5)
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_d = input_c.size(2);
             int in_h = input_c.size(3);
             int in_w = input_c.size(4);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
@@ -232,24 +229,32 @@
                                           weight_d,
                                           weight_h,
                                           weight_w,
                                           3,
                                           out_d,
                                           out_h,
                                           out_w});
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_d,
                                       weight_h,
                                       weight_w,
                                       out_d,
                                       out_h,
                                       out_w});
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0, 0, 0, 0, 0});
             out = out.view({batch_sz / n_parallel_imgs,
                             n_parallel_imgs,
                             out_channels,
                             out_d,
                             out_h,
                             out_w});
             auto out_buf = at::zeros(
@@ -345,29 +350,26 @@
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::tuple<int, int, int> &stride,
                 const std::tuple<int, int, int> &padding,
                 const std::tuple<int, int, int> &dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_d = input_c.size(2);
             int in_h = input_c.size(3);
             int in_w = input_c.size(4);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
@@ -403,39 +405,45 @@
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_d,
                                     in_h,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
-            if (deformable) {
+            if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_d,
                                           weight_h,
                                           weight_w,
                                           3,
                                           out_d,
                                           out_h,
                                           out_w});
-                grad_offset = grad_offset.view_as(offset_c);
-            }
-            if (modulated) {
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0, 0, 0});
+            grad_offset = grad_offset.view_as(offset_c);
+            if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_d,
                                       weight_h,
                                       weight_w,
                                       out_d,
                                       out_h,
                                       out_w});
-                grad_mask = grad_mask.view_as(mask_c);
-            }
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0, 0, 0, 0, 0});
+            grad_mask = grad_mask.view_as(mask_c);
 
             // Separate channels into convolution groups
             grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           groups,
                                           out_channels / groups,
                                           out_d,
@@ -587,40 +595,23 @@
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
+
                 for (int g = 0; g < groups; g++) {
                     grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
                 }
             }
 
-            grad_input = grad_input.view({batch_sz,
-                                          in_channels,
-                                          in_d,
-                                          in_h,
-                                          in_w});
-            grad_weight = grad_weight.view({out_channels,
-                                            in_channels / groups,
-                                            weight_d,
-                                            weight_h,
-                                            weight_w});
-            if (deformable)
-                grad_offset = grad_offset.view({batch_sz,
-                                                offset_groups * 3 * weight_d * weight_h * weight_w,
-                                                out_d,
-                                                out_h,
-                                                out_w});
-            if (modulated)
-                grad_mask = grad_mask.view({batch_sz,
-                                            mask_groups * weight_d * weight_h * weight_w,
-                                            out_d,
-                                            out_h,
-                                            out_w});
+            grad_input = grad_input.view_as(input);
+            grad_weight = grad_weight.view_as(weight);
+            grad_offset = grad_offset.view_as(offset);
+            grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -76,37 +76,34 @@
     namespace ops {
         at::Tensor deform_conv_transpose1d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                int stride,
-                int padding,
-                int output_padding,
-                int dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int stride,
+                const int padding,
+                const int output_padding,
+                const int dilation,
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 3)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
             TORCH_CHECK(weight_c.ndimension() == 3)
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_w = input_c.size(2);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
             int out_channels = weight_c.size(1) * groups;
@@ -187,20 +184,28 @@
             if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_w,
                                           1,
                                           in_w});
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_w,
                                       in_w});
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0});
 
             // Separate channels into convolution groups
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     groups,
                                     in_channels / groups,
                                     in_w}).permute({0, 2, 3, 1, 4}).contiguous();
@@ -252,33 +257,30 @@
         deform_conv_transpose1d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                int stride,
-                int padding,
-                int output_padding,
-                int dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int stride,
+                const int padding,
+                const int output_padding,
+                const int dilation,
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_w = input_c.size(2);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
             int out_channels = weight_c.size(1) * groups;
@@ -307,31 +309,37 @@
                                           out_w});
 
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
-            if (deformable) {
+            if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_w,
                                           1,
                                           in_w});
-                grad_offset = grad_offset.view_as(offset_c);
-            }
-            if (modulated) {
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0});
+            grad_offset = grad_offset.view_as(offset_c);
+            if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_w,
                                       in_w});
-                grad_mask = grad_mask.view_as(mask_c);
-            }
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0});
+            grad_mask = grad_mask.view_as(mask_c);
 
             auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
                                              in_channels,
                                              n_parallel_imgs,
                                              in_w}, input_c.options());
 
             // Separate channels into convolution groups
@@ -431,27 +439,18 @@
             }
 
             grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
                                                   in_channels,
                                                   n_parallel_imgs,
                                                   in_w}).transpose_(1, 2);
             grad_input.copy_(grad_input_buf);
-            grad_input = grad_input.view({batch_sz,
-                                          in_channels,
-                                          in_w});
-            grad_weight = grad_weight.view({in_channels,
-                                            out_channels / groups,
-                                            weight_w});
-            if (deformable)
-                grad_offset = grad_offset.view({batch_sz,
-                                                offset_groups * weight_w,
-                                                in_w});
-            if (modulated)
-                grad_mask = grad_mask.view({batch_sz,
-                                            mask_groups * weight_w,
-                                            in_w});
+
+            grad_input = grad_input.view_as(input);
+            grad_weight = grad_weight.view_as(weight);
+            grad_offset = grad_offset.view_as(offset);
+            grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -80,33 +80,30 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::pair<int, int> &stride,
                 const std::pair<int, int> &padding,
                 const std::pair<int, int> &output_padding,
                 const std::pair<int, int> &dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 4)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
             TORCH_CHECK(weight_c.ndimension() == 4)
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_h = input_c.size(2);
             int in_w = input_c.size(3);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
@@ -211,22 +208,30 @@
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_h,
                                           weight_w,
                                           2,
                                           in_h,
                                           in_w});
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_h,
                                       weight_w,
                                       in_h,
                                       in_w});
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0, 0, 0});
 
             // Separate channels into convolution groups
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     groups,
                                     in_channels / groups,
                                     in_h,
@@ -292,29 +297,26 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::pair<int, int> &stride,
                 const std::pair<int, int> &padding,
                 const std::pair<int, int> &output_padding,
                 const std::pair<int, int> &dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_h = input_c.size(2);
             int in_w = input_c.size(3);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
@@ -352,35 +354,41 @@
 
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_h,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
-            if (deformable) {
+            if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_h,
                                           weight_w,
                                           2,
                                           in_h,
                                           in_w});
-                grad_offset = grad_offset.view_as(offset_c);
-            }
-            if (modulated) {
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0});
+            grad_offset = grad_offset.view_as(offset_c);
+            if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_h,
                                       weight_w,
                                       in_h,
                                       in_w});
-                grad_mask = grad_mask.view_as(mask_c);
-            }
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0, 0, 0});
+            grad_mask = grad_mask.view_as(mask_c);
 
             auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
                                              in_channels,
                                              n_parallel_imgs,
                                              in_h,
                                              in_w}, input_c.options());
 
@@ -505,31 +513,18 @@
 
             grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
                                                   in_channels,
                                                   n_parallel_imgs,
                                                   in_h,
                                                   in_w}).transpose_(1, 2);
             grad_input.copy_(grad_input_buf);
-            grad_input = grad_input.view({batch_sz,
-                                          in_channels,
-                                          in_h,
-                                          in_w});
-            grad_weight = grad_weight.view({in_channels,
-                                            out_channels / groups,
-                                            weight_h,
-                                            weight_w});
-            if (deformable)
-                grad_offset = grad_offset.view({batch_sz,
-                                                offset_groups * 2 * weight_h * weight_w,
-                                                in_h,
-                                                in_w});
-            if (modulated)
-                grad_mask = grad_mask.view({batch_sz,
-                                            mask_groups * weight_h * weight_w,
-                                            in_h,
-                                            in_w});
+
+            grad_input = grad_input.view_as(input);
+            grad_weight = grad_weight.view_as(weight);
+            grad_offset = grad_offset.view_as(offset);
+            grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -80,33 +80,30 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::tuple<int, int, int> &stride,
                 const std::tuple<int, int, int> &padding,
                 const std::tuple<int, int, int> &output_padding,
                 const std::tuple<int, int, int> &dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 5)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
             TORCH_CHECK(weight_c.ndimension() == 5)
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_d = input_c.size(2);
             int in_h = input_c.size(3);
             int in_w = input_c.size(4);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
@@ -236,24 +233,32 @@
                                           weight_d,
                                           weight_h,
                                           weight_w,
                                           3,
                                           in_d,
                                           in_h,
                                           in_w});
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_d,
                                       weight_h,
                                       weight_w,
                                       in_d,
                                       in_h,
                                       in_w});
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0, 0, 0, 0, 0});
 
             // Separate channels into convolution groups
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     groups,
                                     in_channels / groups,
                                     in_d,
@@ -329,29 +334,26 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::tuple<int, int, int> &stride,
                 const std::tuple<int, int, int> &padding,
                 const std::tuple<int, int, int> &output_padding,
                 const std::tuple<int, int, int> &dilation,
-                int groups,
-                int offset_groups,
-                int mask_groups,
-                bool deformable,
-                bool modulated) {
+                const int groups,
+                const int offset_groups,
+                const int mask_groups,
+                const bool deformable,
+                const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
-            if (input_c.is_cuda())
-                at::DeviceGuard guard(input_c.device());
-
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
             int in_d = input_c.size(2);
             int in_h = input_c.size(3);
             int in_w = input_c.size(4);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
@@ -398,39 +400,45 @@
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_d,
                                     in_h,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
-            if (deformable) {
+            if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_d,
                                           weight_h,
                                           weight_w,
                                           3,
                                           in_d,
                                           in_h,
                                           in_w});
-                grad_offset = grad_offset.view_as(offset_c);
-            }
-            if (modulated) {
+            else
+                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0, 0, 0});
+            grad_offset = grad_offset.view_as(offset_c);
+            if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_d,
                                       weight_h,
                                       weight_w,
                                       in_d,
                                       in_h,
                                       in_w});
-                grad_mask = grad_mask.view_as(mask_c);
-            }
+            else
+                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      0, 0, 0, 0, 0, 0, 0});
+            grad_mask = grad_mask.view_as(mask_c);
 
             auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
                                              in_channels,
                                              n_parallel_imgs,
                                              in_d,
                                              in_h,
                                              in_w}, input_c.options());
@@ -580,35 +588,18 @@
             grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
                                                   in_channels,
                                                   n_parallel_imgs,
                                                   in_d,
                                                   in_h,
                                                   in_w}).transpose_(1, 2);
             grad_input.copy_(grad_input_buf);
-            grad_input = grad_input.view({batch_sz,
-                                          in_channels,
-                                          in_d,
-                                          in_h,
-                                          in_w});
-            grad_weight = grad_weight.view({in_channels,
-                                            out_channels / groups,
-                                            weight_d,
-                                            weight_h,
-                                            weight_w});
-            if (deformable)
-                grad_offset = grad_offset.view({batch_sz,
-                                                offset_groups * 3 * weight_d * weight_h * weight_w,
-                                                in_d,
-                                                in_h,
-                                                in_w});
-            if (modulated)
-                grad_mask = grad_mask.view({batch_sz,
-                                            mask_groups * weight_d * weight_h * weight_w,
-                                            in_d,
-                                            in_h,
-                                            in_w});
+
+            grad_input = grad_input.view_as(input);
+            grad_weight = grad_weight.view_as(weight);
+            grad_offset = grad_offset.view_as(offset);
+            grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,16 @@
                 const int width,
                 const int weight_w,
                 const int pad_w,
                 const int stride_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 arr2col_cuda(input,
                              offset,
@@ -34,16 +34,16 @@
                              width,
                              weight_w,
                              pad_w,
                              stride_w,
                              dilation_w,
                              out_w,
                              batch_sz,
-                             n_offset_grps,
-                             n_mask_grps,
+                             offset_groups,
+                             mask_groups,
                              deformable,
                              modulated,
                              columns);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -54,16 +54,16 @@
                             width,
                             weight_w,
                             pad_w,
                             stride_w,
                             dilation_w,
                             out_w,
                             batch_sz,
-                            n_offset_grps,
-                            n_mask_grps,
+                            offset_groups,
+                            mask_groups,
                             deformable,
                             modulated,
                             columns);
             }
         }
 
         void col2arr(
@@ -74,16 +74,16 @@
                 const int width,
                 const int weight_w,
                 const int pad_w,
                 const int stride_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 col2arr_cuda(columns,
                              offset,
@@ -92,16 +92,16 @@
                              width,
                              weight_w,
                              pad_w,
                              stride_w,
                              dilation_w,
                              out_w,
                              batch_sz,
-                             n_offset_grps,
-                             n_mask_grps,
+                             offset_groups,
+                             mask_groups,
                              deformable,
                              modulated,
                              grad_input);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -112,16 +112,16 @@
                             width,
                             weight_w,
                             pad_w,
                             stride_w,
                             dilation_w,
                             out_w,
                             batch_sz,
-                            n_offset_grps,
-                            n_mask_grps,
+                            offset_groups,
+                            mask_groups,
                             deformable,
                             modulated,
                             grad_input);
             }
         }
 
         void deform_conv1d_compute_grad_offset(
@@ -133,16 +133,16 @@
                 const int width,
                 const int weight_w,
                 const int pad_w,
                 const int stride_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 deform_conv1d_compute_grad_offset_cuda(columns,
                                                        input,
@@ -152,16 +152,16 @@
                                                        width,
                                                        weight_w,
                                                        pad_w,
                                                        stride_w,
                                                        dilation_w,
                                                        out_w,
                                                        batch_sz,
-                                                       n_offset_grps,
-                                                       n_mask_grps,
+                                                       offset_groups,
+                                                       mask_groups,
                                                        deformable,
                                                        modulated,
                                                        grad_offset);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -173,16 +173,16 @@
                                                       width,
                                                       weight_w,
                                                       pad_w,
                                                       stride_w,
                                                       dilation_w,
                                                       out_w,
                                                       batch_sz,
-                                                      n_offset_grps,
-                                                      n_mask_grps,
+                                                      offset_groups,
+                                                      mask_groups,
                                                       deformable,
                                                       modulated,
                                                       grad_offset);
             }
         }
 
         void deform_conv1d_compute_grad_mask(
@@ -193,16 +193,16 @@
                 const int width,
                 const int weight_w,
                 const int pad_w,
                 const int stride_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 deform_conv1d_compute_grad_mask_cuda(columns,
                                                      input,
@@ -211,16 +211,16 @@
                                                      width,
                                                      weight_w,
                                                      pad_w,
                                                      stride_w,
                                                      dilation_w,
                                                      out_w,
                                                      batch_sz,
-                                                     n_offset_grps,
-                                                     n_mask_grps,
+                                                     offset_groups,
+                                                     mask_groups,
                                                      deformable,
                                                      modulated,
                                                      grad_mask);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -231,16 +231,16 @@
                                                     width,
                                                     weight_w,
                                                     pad_w,
                                                     stride_w,
                                                     dilation_w,
                                                     out_w,
                                                     batch_sz,
-                                                    n_offset_grps,
-                                                    n_mask_grps,
+                                                    offset_groups,
+                                                    mask_groups,
                                                     deformable,
                                                     modulated,
                                                     grad_mask);
             }
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
                 const int stride_h,
                 const int stride_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 im2col_cuda(input,
                             offset,
@@ -46,16 +46,16 @@
                             stride_h,
                             stride_w,
                             dilation_h,
                             dilation_w,
                             out_h,
                             out_w,
                             batch_sz,
-                            n_offset_grps,
-                            n_mask_grps,
+                            offset_groups,
+                            mask_groups,
                             deformable,
                             modulated,
                             columns);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -72,16 +72,16 @@
                            stride_h,
                            stride_w,
                            dilation_h,
                            dilation_w,
                            out_h,
                            out_w,
                            batch_sz,
-                           n_offset_grps,
-                           n_mask_grps,
+                           offset_groups,
+                           mask_groups,
                            deformable,
                            modulated,
                            columns);
             }
         }
 
         void col2im(
@@ -98,16 +98,16 @@
                 const int stride_h,
                 const int stride_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 col2im_cuda(columns,
                             offset,
@@ -122,16 +122,16 @@
                             stride_h,
                             stride_w,
                             dilation_h,
                             dilation_w,
                             out_h,
                             out_w,
                             batch_sz,
-                            n_offset_grps,
-                            n_mask_grps,
+                            offset_groups,
+                            mask_groups,
                             deformable,
                             modulated,
                             grad_input);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -148,16 +148,16 @@
                            stride_h,
                            stride_w,
                            dilation_h,
                            dilation_w,
                            out_h,
                            out_w,
                            batch_sz,
-                           n_offset_grps,
-                           n_mask_grps,
+                           offset_groups,
+                           mask_groups,
                            deformable,
                            modulated,
                            grad_input);
             }
         }
 
         void deform_conv2d_compute_grad_offset(
@@ -175,16 +175,16 @@
                 const int stride_h,
                 const int stride_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 deform_conv2d_compute_grad_offset_cuda(columns,
                                                        input,
@@ -200,16 +200,16 @@
                                                        stride_h,
                                                        stride_w,
                                                        dilation_h,
                                                        dilation_w,
                                                        out_h,
                                                        out_w,
                                                        batch_sz,
-                                                       n_offset_grps,
-                                                       n_mask_grps,
+                                                       offset_groups,
+                                                       mask_groups,
                                                        deformable,
                                                        modulated,
                                                        grad_offset);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -227,16 +227,16 @@
                                                       stride_h,
                                                       stride_w,
                                                       dilation_h,
                                                       dilation_w,
                                                       out_h,
                                                       out_w,
                                                       batch_sz,
-                                                      n_offset_grps,
-                                                      n_mask_grps,
+                                                      offset_groups,
+                                                      mask_groups,
                                                       deformable,
                                                       modulated,
                                                       grad_offset);
             }
         }
 
         void deform_conv2d_compute_grad_mask(
@@ -253,16 +253,16 @@
                 const int stride_h,
                 const int stride_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 deform_conv2d_compute_grad_mask_cuda(columns,
                                                      input,
@@ -277,16 +277,16 @@
                                                      stride_h,
                                                      stride_w,
                                                      dilation_h,
                                                      dilation_w,
                                                      out_h,
                                                      out_w,
                                                      batch_sz,
-                                                     n_offset_grps,
-                                                     n_mask_grps,
+                                                     offset_groups,
+                                                     mask_groups,
                                                      deformable,
                                                      modulated,
                                                      grad_mask);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -303,16 +303,16 @@
                                                     stride_h,
                                                     stride_w,
                                                     dilation_h,
                                                     dilation_w,
                                                     out_h,
                                                     out_w,
                                                     batch_sz,
-                                                    n_offset_grps,
-                                                    n_mask_grps,
+                                                    offset_groups,
+                                                    mask_groups,
                                                     deformable,
                                                     modulated,
                                                     grad_mask);
             }
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.2.1/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,16 @@
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 vol2col_cuda(input,
                              offset,
@@ -58,16 +58,16 @@
                              dilation_d,
                              dilation_h,
                              dilation_w,
                              out_d,
                              out_h,
                              out_w,
                              batch_sz,
-                             n_offset_grps,
-                             n_mask_grps,
+                             offset_groups,
+                             mask_groups,
                              deformable,
                              modulated,
                              columns);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -90,16 +90,16 @@
                             dilation_d,
                             dilation_h,
                             dilation_w,
                             out_d,
                             out_h,
                             out_w,
                             batch_sz,
-                            n_offset_grps,
-                            n_mask_grps,
+                            offset_groups,
+                            mask_groups,
                             deformable,
                             modulated,
                             columns);
             }
         }
 
         void col2vol(
@@ -122,16 +122,16 @@
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 col2vol_cuda(columns,
                              offset,
@@ -152,16 +152,16 @@
                              dilation_d,
                              dilation_h,
                              dilation_w,
                              out_d,
                              out_h,
                              out_w,
                              batch_sz,
-                             n_offset_grps,
-                             n_mask_grps,
+                             offset_groups,
+                             mask_groups,
                              deformable,
                              modulated,
                              grad_input);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -184,16 +184,16 @@
                             dilation_d,
                             dilation_h,
                             dilation_w,
                             out_d,
                             out_h,
                             out_w,
                             batch_sz,
-                            n_offset_grps,
-                            n_mask_grps,
+                            offset_groups,
+                            mask_groups,
                             deformable,
                             modulated,
                             grad_input);
             }
         }
 
         void deform_conv3d_compute_grad_offset(
@@ -217,16 +217,16 @@
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 deform_conv3d_compute_grad_offset_cuda(columns,
                                                        input,
@@ -248,16 +248,16 @@
                                                        dilation_d,
                                                        dilation_h,
                                                        dilation_w,
                                                        out_d,
                                                        out_h,
                                                        out_w,
                                                        batch_sz,
-                                                       n_offset_grps,
-                                                       n_mask_grps,
+                                                       offset_groups,
+                                                       mask_groups,
                                                        deformable,
                                                        modulated,
                                                        grad_offset);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -281,16 +281,16 @@
                                                       dilation_d,
                                                       dilation_h,
                                                       dilation_w,
                                                       out_d,
                                                       out_h,
                                                       out_w,
                                                       batch_sz,
-                                                      n_offset_grps,
-                                                      n_mask_grps,
+                                                      offset_groups,
+                                                      mask_groups,
                                                       deformable,
                                                       modulated,
                                                       grad_offset);
             }
         }
 
         void deform_conv3d_compute_grad_mask(
@@ -313,16 +313,16 @@
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
-                const int n_offset_grps,
-                const int n_mask_grps,
+                const int offset_groups,
+                const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.is_cuda()) {
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 deform_conv3d_compute_grad_mask_cuda(columns,
                                                      input,
@@ -343,16 +343,16 @@
                                                      dilation_d,
                                                      dilation_h,
                                                      dilation_w,
                                                      out_d,
                                                      out_h,
                                                      out_w,
                                                      batch_sz,
-                                                     n_offset_grps,
-                                                     n_mask_grps,
+                                                     offset_groups,
+                                                     mask_groups,
                                                      deformable,
                                                      modulated,
                                                      grad_mask);
 #else
                 AT_ERROR("Not compiled with GPU support");
 #endif
             } else {
@@ -375,16 +375,16 @@
                                                     dilation_d,
                                                     dilation_h,
                                                     dilation_w,
                                                     out_d,
                                                     out_h,
                                                     out_w,
                                                     batch_sz,
-                                                    n_offset_grps,
-                                                    n_mask_grps,
+                                                    offset_groups,
+                                                    mask_groups,
                                                     deformable,
                                                     modulated,
                                                     grad_mask);
             }
         }
     }
 }
```

### Comparing `tvdcn-0.2.0/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.2.1/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/tvdcn/extension.py` & `tvdcn-0.2.1/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/tvdcn/ops/deform_conv.py` & `tvdcn-0.2.1/tvdcn/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.2.1/tvdcn/ops/deform_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/tvdcn/ops/mask_activation.py` & `tvdcn-0.2.1/tvdcn/ops/mask_activation.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/tvdcn/utils.py` & `tvdcn-0.2.1/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.0/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.2.1/tvdcn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.0
+Version: 0.2.1
 Summary: Torchvision Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.2.0/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.2.1/tvdcn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

