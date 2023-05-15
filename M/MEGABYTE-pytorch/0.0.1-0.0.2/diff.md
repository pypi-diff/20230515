# Comparing `tmp/MEGABYTE-pytorch-0.0.1.tar.gz` & `tmp/MEGABYTE-pytorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.0.1.tar", last modified: Mon May 15 03:39:26 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.0.2.tar", last modified: Mon May 15 04:00:10 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.0.1.tar` & `MEGABYTE-pytorch-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:39:26.046929 MEGABYTE-pytorch-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 03:39:15.000000 MEGABYTE-pytorch-0.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:39:26.046929 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 03:39:15.000000 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-15 03:39:15.000000 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 03:39:26.046929 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 03:39:26.000000 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 03:39:26.000000 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 03:39:26.000000 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 03:39:26.000000 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 03:39:26.000000 MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 03:39:26.046929 MEGABYTE-pytorch-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-15 03:39:15.000000 MEGABYTE-pytorch-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 03:39:26.046929 MEGABYTE-pytorch-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 03:39:15.000000 MEGABYTE-pytorch-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 04:00:10.000000 MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 04:00:10.233631 MEGABYTE-pytorch-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 03:59:56.000000 MEGABYTE-pytorch-0.0.2/setup.py
```

### Comparing `MEGABYTE-pytorch-0.0.1/LICENSE` & `MEGABYTE-pytorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch/megabyte.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import math
 import functools
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
-from einops_exts import rearrange_with_anon_dims
-from einops import rearrange, reduce, repeat
+from einops import rearrange, reduce, repeat, pack, unpack
 
 # helpers
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
 
+def pack_one(t, pattern):
+    return pack([t], pattern)
+
+def unpack_one(t, ps, pattern):
+    return unpack(t, ps, pattern)[0]
+
 def remainder_to_mult(num, mult):
     return (mult - num % mult) % mult
 
 def cast_tuple(t, length = 1):
     return t if isinstance(t, tuple) else ((t,) * length)
 
 def reduce_mult(nums):
@@ -137,15 +142,14 @@
             sim = sim + attn_bias
 
         i, j = sim.shape[-2:]
         mask_value = -torch.finfo(sim.dtype).max
         mask = torch.ones((i, j), dtype = torch.bool, device = device).triu(j - i + 1)
         sim = sim.masked_fill(mask, mask_value)
 
-        sim = sim - sim.amax(dim = -1, keepdim = True).detach()
         attn = sim.softmax(dim = -1)
         attn = self.dropout(attn)
 
         out = einsum('b h i j, b j d -> b h i d', attn, v)
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
@@ -240,50 +244,53 @@
         total_seq_len = reduce_mult(self.max_seq_len)
         device = next(self.parameters()).device
 
         if not exists(prime):
             prime = torch.empty((default_batch_size, 0), dtype = torch.long, device = device)
 
         seq = prime
+        batch = seq.shape[0]
 
         for _ in range(total_seq_len - seq.shape[-1]):
             logits = self.forward(seq)[:, -1]
             logits = top_k(logits, thres = filter_thres)
             sampled = gumbel_sample(logits, dim = -1, temperature = temperature)
             seq = torch.cat((seq, rearrange(sampled, 'b -> b 1')), dim = -1)
 
-        return rearrange_with_anon_dims(seq, 'b (...d) -> b ...d', d = self.max_seq_len)
+        return seq.reshape(batch, *self.max_seq_len)
 
     def forward_empty(self, batch_size):
         # take care of special case
         # where you sample from input of 0 (start token only)
 
         tokens = repeat(self.start_tokens, 'd -> b 1 d', b = batch_size)
 
         for transformer in self.transformers:
             tokens = transformer(tokens)
 
         return self.to_logits(tokens)
 
     def forward(self, ids, return_loss = False):
+        batch = ids.shape[0]
+
         assert ids.ndim in {2, self.stages + 1}
         flattened_dims = ids.ndim == 2
         ids_orig_ndim = ids.ndim
 
         if ids.numel() == 0:
             return self.forward_empty(ids.shape[0])
 
         if flattened_dims:
             # allow for ids to be given in the shape of (batch, seq)
             # in which case it will be auto-padded to the next nearest multiple of depth seq len
             seq_len = ids.shape[-1]
             multiple_of = reduce_mult(self.max_seq_len[1:])
             padding = remainder_to_mult(seq_len, multiple_of)
             ids = F.pad(ids, (0, padding), value = self.pad_id)
-            ids = rearrange_with_anon_dims(ids, 'b (l ...d) -> b l ...d', d = self.max_seq_len[1:])
+            ids = ids.reshape(batch, -1, *self.max_seq_len[1:])
 
         b, *prec_dims, device = *ids.shape, ids.device
 
         # check some dimensions
 
         assert prec_dims[0] <= self.max_seq_len[0], 'the first dimension of your axial autoregressive transformer must be less than the first tuple element of max_seq_len (like any autoregressive transformer)'
         assert tuple(prec_dims[1:]) == tuple(self.max_seq_len[1:]), 'all subsequent dimensions must match exactly'
@@ -318,19 +325,17 @@
             is_last = ind == (self.stages - 1)
 
             stage_tokens = torch.cat((
                 start_tokens,
                 stage_tokens,
             ), dim = -2)
 
-            *prec_dims, _, _ = stage_tokens.shape
-
-            stage_tokens = rearrange(stage_tokens, '... n d -> (...) n d')
+            stage_tokens, ps = pack_one(stage_tokens, '* n d')
             attended = transformer(stage_tokens)
-            attended = rearrange_with_anon_dims(attended, '(...b) n d -> ...b n d', b = prec_dims)
+            attended = unpack_one(attended, ps, '* n d')
 
             start_tokens = rearrange(attended[..., :-1, :], '... n d -> ... n 1 d')
 
         logits = self.to_logits(attended)
 
         logits = logits[..., 1:, :]
```

### Comparing `MEGABYTE-pytorch-0.0.1/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.0.2/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.1/PKG-INFO` & `MEGABYTE-pytorch-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.1/README.md` & `MEGABYTE-pytorch-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 <img src="./MEGABYTE.png" width="450px"></img>
 
 ## MEGABYTE-pytorch
 
 Implementation of <a href="https://arxiv.org/abs/2305.07185">MEGABYTE</a>, Predicting Million-byte Sequences with Multiscale Transformers, in Pytorch
 
+## Appreciation
+
+- <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for the generous sponsorship to work on and open source cutting edge artificial intelligence research
+
 ## Install
 
 ```bash
 $ pip install MEGABYTE-pytorch
 ```
 
 ## Usage
 
 ```python
 import torch
 from MEGABYTE_pytorch import MEGABYTE
 
 model = MEGABYTE(
-    num_tokens = 16000,             # number of tokens, in the paper they had a codebook size of 16k
+    num_tokens = 16000,             # number of tokens
     dim = 512,                      # transformer model dimension
     max_seq_len = (1024, 4),        # sequence length for global and then local
     depth = (6, 4),                 # number of layers for global and then local
     dim_head = 64,                  # dimension per head
     heads = 8,                      # number of attention heads
 )
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 [./MEGABYTE.png] ## MEGABYTE-pytorch Implementation of MEGABYTE, Predicting
-Million-byte Sequences with Multiscale Transformers, in Pytorch ## Install
-```bash $ pip install MEGABYTE-pytorch ``` ## Usage ```python import torch from
+Million-byte Sequences with Multiscale Transformers, in Pytorch ## Appreciation
+- Stability and ð¤_Huggingface for the generous sponsorship to work on and
+open source cutting edge artificial intelligence research ## Install ```bash $
+pip install MEGABYTE-pytorch ``` ## Usage ```python import torch from
 MEGABYTE_pytorch import MEGABYTE model = MEGABYTE( num_tokens = 16000, # number
-of tokens, in the paper they had a codebook size of 16k dim = 512, #
-transformer model dimension max_seq_len = (1024, 4), # sequence length for
-global and then local depth = (6, 4), # number of layers for global and then
-local dim_head = 64, # dimension per head heads = 8, # number of attention
-heads ) x = torch.randint(0, 16000, (1, 1024, 4)) loss = model(x, return_loss =
-True) loss.backward() # then after much training logits = model(x) # and sample
-from the logits accordingly # or you can use the generate function sampled =
-model.generate(temperature = 0.9, filter_thres = 0.9) # (1, 1024, 4) ``` ##
-Citations ```bibtex @misc{yu2023megabyte, title = {MEGABYTE: Predicting
-Million-byte Sequences with Multiscale Transformers}, author = {Lili Yu and
-DÃ¡niel Simig and Colin Flaherty and Armen Aghajanyan and Luke Zettlemoyer and
-Mike Lewis}, year = {2023}, eprint = {2305.07185}, archivePrefix = {arXiv},
-primaryClass = {cs.LG} } ```
+of tokens dim = 512, # transformer model dimension max_seq_len = (1024, 4), #
+sequence length for global and then local depth = (6, 4), # number of layers
+for global and then local dim_head = 64, # dimension per head heads = 8, #
+number of attention heads ) x = torch.randint(0, 16000, (1, 1024, 4)) loss =
+model(x, return_loss = True) loss.backward() # then after much training logits
+= model(x) # and sample from the logits accordingly # or you can use the
+generate function sampled = model.generate(temperature = 0.9, filter_thres =
+0.9) # (1, 1024, 4) ``` ## Citations ```bibtex @misc{yu2023megabyte, title =
+{MEGABYTE: Predicting Million-byte Sequences with Multiscale Transformers},
+author = {Lili Yu and DÃ¡niel Simig and Colin Flaherty and Armen Aghajanyan and
+Luke Zettlemoyer and Mike Lewis}, year = {2023}, eprint = {2305.07185},
+archivePrefix = {arXiv}, primaryClass = {cs.LG} } ```
```

### Comparing `MEGABYTE-pytorch-0.0.1/setup.py` & `MEGABYTE-pytorch-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'transformers'
   ],
   install_requires=[
     'einops>=0.6.1',
-    'einops-exts',
     'torch>=1.10'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
```

