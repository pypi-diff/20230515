# Comparing `tmp/MEGABYTE-pytorch-0.0.3.tar.gz` & `tmp/MEGABYTE-pytorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.0.3.tar", last modified: Mon May 15 13:44:43 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.0.4.tar", last modified: Mon May 15 14:08:57 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.0.3.tar` & `MEGABYTE-pytorch-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:44:43.736367 MEGABYTE-pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:44:43.732367 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:44:43.736367 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 13:44:43.000000 MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 13:44:43.736367 MEGABYTE-pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:44:43.736367 MEGABYTE-pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 13:44:23.000000 MEGABYTE-pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/setup.py
```

### Comparing `MEGABYTE-pytorch-0.0.3/LICENSE` & `MEGABYTE-pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/megabyte.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, reduce, repeat, pack, unpack
 from einops.layers.torch import Rearrange
 
+from MEGABYTE_pytorch.attend import Attend
+
 # helpers
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
@@ -113,72 +115,67 @@
 class Attention(nn.Module):
     def __init__(
         self,
         *,
         dim,
         dim_head = 64,
         heads = 8,
-        dropout = 0.
+        dropout = 0.,
+        flash = False
     ):
         super().__init__()
         self.scale = dim_head ** -0.5
         self.heads = heads
         inner_dim = dim_head * heads
 
+        self.attend = Attend(
+            causal = True,
+            flash = flash,
+            dropout = dropout
+        )
+
         self.dropout = nn.Dropout(dropout)
         self.norm = RMSNorm(dim)
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim, dim_head * 2, bias = False)
         self.to_out = nn.Linear(inner_dim, dim, bias = False)
 
     def forward(self, x, attn_bias = None):
         h, device = self.heads, x.device
 
         x = self.norm(x)
         q, k, v = (self.to_q(x), *self.to_kv(x).chunk(2, dim = -1))
         q = rearrange(q, 'b n (h d) -> b h n d', h = h)
 
-        q = q * self.scale
-        sim = einsum('b h i d, b j d -> b h i j', q, k)
-
-        if exists(attn_bias):
-            sim = sim + attn_bias
-
-        i, j = sim.shape[-2:]
-        mask_value = -torch.finfo(sim.dtype).max
-        mask = torch.ones((i, j), dtype = torch.bool, device = device).triu(j - i + 1)
-        sim = sim.masked_fill(mask, mask_value)
-
-        attn = sim.softmax(dim = -1)
-        attn = self.dropout(attn)
+        out = self.attend(q, k, v, attn_bias = attn_bias)
 
-        out = einsum('b h i j, b j d -> b h i d', attn, v)
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 class Transformer(nn.Module):
     def __init__(
         self,
         *,
         dim,
         layers,
         dim_head = 64,
         heads = 8,
         attn_dropout = 0.,
         ff_dropout = 0.,
         ff_mult = 4,
-        rel_pos_bias = True
+        rel_pos_bias = True,
+        flash_attn = False
     ):
         super().__init__()
         self.alibi = Alibi(heads = heads) if rel_pos_bias else None
         self.layers = nn.ModuleList([])
 
         for _ in range(layers):
             self.layers.append(nn.ModuleList([
-                Attention(dim = dim, dim_head = dim_head, heads = heads, dropout = attn_dropout),
+                Attention(dim = dim, dim_head = dim_head, heads = heads, dropout = attn_dropout, flash = flash_attn),
                 FeedForward(dim = dim, mult = ff_mult, dropout = ff_dropout)
             ]))
 
         self.norm = RMSNorm(dim)
 
     def forward(self, x):
         n = x.shape[-2]
@@ -202,15 +199,16 @@
         max_seq_len,
         dim_head = 64,
         heads = 8,
         attn_dropout = 0.,
         ff_mult = 4,
         ff_dropout = 0.,
         pad_id = 0,
-        rel_pos_bias = True
+        rel_pos_bias = True,
+        flash_attn = False
     ):
         super().__init__()
 
         # simplified configuration for each stage of the hierarchy
         # depth = (2, 2, 4) would translate to depth 2 at first stage, depth 2 second stage, depth 4 third
         # max_seq_len = (16, 8, 4) would translate to max sequence length of 16 at first stage, length of 8 at second stage, length of 4 for last
 
@@ -240,15 +238,16 @@
                 dim = dim,
                 layers = stage_depth,
                 dim_head = dim_head,
                 heads = heads,
                 attn_dropout = attn_dropout,
                 ff_dropout = ff_dropout,
                 ff_mult = ff_mult,
-                rel_pos_bias = rel_pos_bias
+                rel_pos_bias = rel_pos_bias,
+                flash_attn = flash_attn
             ))
 
         self.to_logits = nn.Linear(dim, num_tokens)
         self.pad_id = pad_id
 
     def generate(self, prime = None, filter_thres = 0.9, temperature = 1., default_batch_size = 1):
         total_seq_len = reduce_mult(self.max_seq_len)
```

### Comparing `MEGABYTE-pytorch-0.0.3/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.3/PKG-INFO` & `MEGABYTE-pytorch-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.3/README.md` & `MEGABYTE-pytorch-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -64,7 +64,16 @@
     author  = {Kumar, Manoj and Dehghani, Mostafa and Houlsby, Neil},
     title   = {Dual PatchNorm},
     publisher = {arXiv},
     year    = {2023},
     copyright = {Creative Commons Attribution 4.0 International}
 }
 ```
+
+```bibtex
+@inproceedings{dao2022flashattention,
+    title   = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+    author  = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+    booktitle = {Advances in Neural Information Processing Systems},
+    year    = {2022}
+}
+```
```

#### html2text {}

```diff
@@ -16,7 +16,12 @@
 author = {Lili Yu and DÃ¡niel Simig and Colin Flaherty and Armen Aghajanyan and
 Luke Zettlemoyer and Mike Lewis}, year = {2023}, eprint = {2305.07185},
 archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc{https://
 doi.org/10.48550/arxiv.2302.01327, doi = {10.48550/ARXIV.2302.01327}, url =
 {https://arxiv.org/abs/2302.01327}, author = {Kumar, Manoj and Dehghani,
 Mostafa and Houlsby, Neil}, title = {Dual PatchNorm}, publisher = {arXiv}, year
 = {2023}, copyright = {Creative Commons Attribution 4.0 International} } ```
+```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
+and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
+and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
+} ```
```

### Comparing `MEGABYTE-pytorch-0.0.3/setup.py` & `MEGABYTE-pytorch-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```

