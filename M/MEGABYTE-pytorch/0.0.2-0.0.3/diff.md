# Comparing `tmp/MEGABYTE-pytorch-0.0.2.tar.gz` & `tmp/MEGABYTE-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.0.2.tar", last modified: Mon May 15 04:00:10 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.0.3.tar", last modified: Mon May 15 13:44:43 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.0.2.tar` & `MEGABYTE-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:44:43.736367 MEGABYTE-pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:44:43.732367 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:44:43.736367 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 13:44:43.736367 MEGABYTE-pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:44:43.736367 MEGABYTE-pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/setup.py
```

### Comparing `MEGABYTE-pytorch-0.0.2/LICENSE` & `MEGABYTE-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch/megabyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import math
 import functools
+
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, reduce, repeat, pack, unpack
+from einops.layers.torch import Rearrange
 
 # helpers
 
 def exists(val):
     return val is not None
 
 def default(val, d):
@@ -217,16 +219,24 @@
 
         self.stages = len(depth)
 
         self.token_emb = nn.Embedding(num_tokens, dim)
         self.start_tokens = nn.Parameter(torch.randn(dim))
 
         self.max_seq_len = max_seq_len
+
         self.pos_embs = nn.ModuleList([nn.Embedding(seq_len, dim) for seq_len in max_seq_len])
 
+        self.patch_embedders = nn.ModuleList([nn.Sequential(
+            Rearrange('... r d -> ... (r d)'),
+            nn.LayerNorm(seq_len * dim),
+            nn.Linear(seq_len * dim, dim),
+            nn.LayerNorm(dim)
+        ) for seq_len in self.max_seq_len[1:]])
+
         self.transformers = nn.ModuleList([])
 
         for stage_depth in depth:
             self.transformers.append(Transformer(
                 dim = dim,
                 layers = stage_depth,
                 dim_head = dim_head,
@@ -301,19 +311,19 @@
 
         # get tokens for all hierarchical stages, reducing by appropriate dimensions
         # and adding the absolute positional embeddings
 
         tokens_at_stages = []
         reduced_tokens = tokens
 
-        for ind, pos_emb in zip(range(len(prec_dims)), reversed(self.pos_embs)):
+        for ind, pos_emb, patch_emb in zip(range(len(prec_dims)), reversed(self.pos_embs), reversed((*self.patch_embedders, None))):
             is_first = ind == 0
 
             if not is_first:
-                reduced_tokens = reduce(reduced_tokens, 'b ... r d -> b ... d', 'sum')
+                reduced_tokens = patch_emb(reduced_tokens)
 
             positions = pos_emb(torch.arange(reduced_tokens.shape[-2], device = device))
             tokens_with_position = reduced_tokens + positions
             tokens_at_stages.insert(0, tokens_with_position)
 
         # get start tokens and append to the coarsest stage
```

### Comparing `MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.2/PKG-INFO` & `MEGABYTE-pytorch-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.2/setup.py` & `MEGABYTE-pytorch-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```

