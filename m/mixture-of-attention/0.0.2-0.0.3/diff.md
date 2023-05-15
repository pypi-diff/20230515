# Comparing `tmp/mixture-of-attention-0.0.2.tar.gz` & `tmp/mixture-of-attention-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-attention-0.0.2.tar", last modified: Mon May 15 18:51:38 2023, max compression
+gzip compressed data, was "mixture-of-attention-0.0.3.tar", last modified: Mon May 15 19:26:05 2023, max compression
```

## Comparing `mixture-of-attention-0.0.2.tar` & `mixture-of-attention-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/mixture_of_attention/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/mixture_of_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/mixture_of_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/mixture_of_attention/mixture_of_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/mixture_of_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/mixture_of_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/mixture_of_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/mixture_of_attention/mixture_of_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/setup.py
```

### Comparing `mixture-of-attention-0.0.2/LICENSE` & `mixture-of-attention-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.2/PKG-INFO` & `mixture-of-attention-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.2/README.md` & `mixture-of-attention-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.2/mixture_of_attention/attend.py` & `mixture-of-attention-0.0.3/mixture_of_attention/attend.py`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.2/mixture_of_attention/mixture_of_attention.py` & `mixture-of-attention-0.0.3/mixture_of_attention/mixture_of_attention.py`

 * *Files 12% similar despite different names*

```diff
@@ -180,14 +180,16 @@
         **kwargs
     ):
         super().__init__()
         dim_context = default(dim_context, dim)
         self.num_routed_queries = num_routed_queries
         self.num_routed_key_values = num_routed_key_values
 
+        self.null_routed_token = nn.Parameter(torch.randn(1, 1, dim))
+
         self.query_router = CoordinateDescentRouter(
             dim,
             num_routing_tokens = num_experts,
             use_triton = use_triton,
             **kwargs
         )
 
@@ -204,14 +206,18 @@
             dim_head = dim_head,
             heads = heads,
             groups = num_experts,
             dropout = dropout,
             flash = flash_attn
         )
 
+    @property
+    def device(self):
+        return next(self.parameters()).device
+
     def forward(
         self,
         x,
         context = None,
         mask = None,
         context_mask = None,
         num_routed_queries = None,
@@ -251,20 +257,34 @@
             context = key_values,
             mask = key_value_mask,
             values_scale = key_value_scores,
         )
 
         attn_out = attn_out * query_scores
 
-        if need_route_queries:
-            out = torch.zeros_like(x)
+        if not need_route_queries:
+            return attn_out
 
-            query_indices = repeat(query_indices, 'b g n -> b (g n) d', d = x.shape[-1])
-            attn_out = rearrange(attn_out, 'b g n d -> b (g n) d')
+        out = torch.zeros_like(x)
+        counts = torch.zeros(x.shape[:-1], device = x.device)
 
-            numer = out.scatter_add(1, query_indices, attn_out)
-            denom = out.scatter_add(1, query_indices, torch.ones_like(attn_out))
-            out = numer / denom.clamp(min = 1e-5)
-        else:
-            out = attn_out
+        query_indices = rearrange(query_indices, 'b g n -> b (g n)')
+        attn_out = rearrange(attn_out, 'b g n d -> b (g n) d')
+
+        expanded_query_indices = repeat(query_indices, 'b n -> b n d', d = x.shape[-1])
+
+        attn_out_summed = out.scatter_add(1, expanded_query_indices, attn_out)
+
+        counts = counts.scatter_add(1, query_indices, torch.ones(attn_out.shape[:-1], device = self.device))
+        counts = rearrange(counts, '... -> ... 1')
+
+        scatter_meaned = attn_out_summed / counts.clamp(min = 1e-5)
+
+        # for the positions that were not routed, use a learned routing token instead of just 0s
+
+        out = torch.where(
+            counts > 0,
+            scatter_meaned,
+            self.null_routed_token
+        )
 
         return out
```

### Comparing `mixture-of-attention-0.0.2/mixture_of_attention.egg-info/PKG-INFO` & `mixture-of-attention-0.0.3/mixture_of_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.2/setup.py` & `mixture-of-attention-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'mixture-of-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Mixture of Attention',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/mixture-of-attention',
   keywords = [
```

