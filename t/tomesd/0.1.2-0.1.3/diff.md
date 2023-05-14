# Comparing `tmp/tomesd-0.1.2.tar.gz` & `tmp/tomesd-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomesd-0.1.2.tar", last modified: Wed Apr  5 03:28:00 2023, max compression
+gzip compressed data, was "tomesd-0.1.3.tar", last modified: Sun May 14 22:19:42 2023, max compression
```

## Comparing `tomesd-0.1.2.tar` & `tomesd-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:28:00.183498 tomesd-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-05 03:27:49.000000 tomesd-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-05 03:28:00.183498 tomesd-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-05 03:27:49.000000 tomesd-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 03:28:00.183498 tomesd-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-05 03:27:49.000000 tomesd-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:28:00.183498 tomesd-0.1.2/tomesd/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-05 03:27:49.000000 tomesd-0.1.2/tomesd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-05 03:27:49.000000 tomesd-0.1.2/tomesd/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-04-05 03:27:49.000000 tomesd-0.1.2/tomesd/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-05 03:27:49.000000 tomesd-0.1.2/tomesd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:28:00.183498 tomesd-0.1.2/tomesd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-05 03:28:00.000000 tomesd-0.1.2/tomesd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-05 03:28:00.000000 tomesd-0.1.2/tomesd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 03:28:00.000000 tomesd-0.1.2/tomesd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-05 03:28:00.000000 tomesd-0.1.2/tomesd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 03:28:00.000000 tomesd-0.1.2/tomesd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:19:42.637282 tomesd-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-14 22:19:22.000000 tomesd-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-05-14 22:19:42.633282 tomesd-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-14 22:19:22.000000 tomesd-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 22:19:42.637282 tomesd-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-14 22:19:22.000000 tomesd-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:19:42.633282 tomesd-0.1.3/tomesd/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-14 22:19:22.000000 tomesd-0.1.3/tomesd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-14 22:19:22.000000 tomesd-0.1.3/tomesd/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-05-14 22:19:22.000000 tomesd-0.1.3/tomesd/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-14 22:19:22.000000 tomesd-0.1.3/tomesd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:19:42.633282 tomesd-0.1.3/tomesd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-05-14 22:19:42.000000 tomesd-0.1.3/tomesd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 22:19:42.000000 tomesd-0.1.3/tomesd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:19:42.000000 tomesd-0.1.3/tomesd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 22:19:42.000000 tomesd-0.1.3/tomesd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 22:19:42.000000 tomesd-0.1.3/tomesd.egg-info/top_level.txt
```

### Comparing `tomesd-0.1.2/LICENSE` & `tomesd-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tomesd-0.1.2/PKG-INFO` & `tomesd-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomesd
-Version: 0.1.2
+Version: 0.1.3
 Summary: Token Merging for Stable Diffusion
 Home-page: https://github.com/dbolya/tomesd
 Author: Daniel Bolya
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tomesd-0.1.2/README.md` & `tomesd-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tomesd-0.1.2/tomesd/merge.py` & `tomesd-0.1.3/tomesd/merge.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,44 +15,45 @@
         ).squeeze(-1)
     else:
         return torch.gather(input, dim, index)
 
 
 def bipartite_soft_matching_random2d(metric: torch.Tensor,
                                      w: int, h: int, sx: int, sy: int, r: int,
-                                     no_rand: bool = False) -> Tuple[Callable, Callable]:
+                                     no_rand: bool = False,
+                                     generator: torch.Generator = None) -> Tuple[Callable, Callable]:
     """
     Partitions the tokens into src and dst and merges r tokens from src to dst.
     Dst tokens are partitioned by choosing one randomy in each (sx, sy) region.
 
     Args:
      - metric [B, N, C]: metric to use for similarity
      - w: image width in tokens
      - h: image height in tokens
      - sx: stride in the x dimension for dst, must divide w
      - sy: stride in the y dimension for dst, must divide h
      - r: number of tokens to remove (by merging)
      - no_rand: if true, disable randomness (use top left corner only)
+     - rand_seed: if no_rand is false, and if not None, sets random seed.
     """
     B, N, _ = metric.shape
 
     if r <= 0:
         return do_nothing, do_nothing
 
     gather = mps_gather_workaround if metric.device.type == "mps" else torch.gather
     
     with torch.no_grad():
-        
         hsy, wsx = h // sy, w // sx
 
         # For each sy by sx kernel, randomly assign one token to be dst and the rest src
         if no_rand:
             rand_idx = torch.zeros(hsy, wsx, 1, device=metric.device, dtype=torch.int64)
         else:
-            rand_idx = torch.randint(sy*sx, size=(hsy, wsx, 1), device=metric.device)
+            rand_idx = torch.randint(sy*sx, size=(hsy, wsx, 1), device=generator.device, generator=generator).to(metric.device)
         
         # The image might not divide sx and sy, so we need to work on a view of the top left if the idx buffer instead
         idx_buffer_view = torch.zeros(hsy, wsx, sy*sx, device=metric.device, dtype=torch.int64)
         idx_buffer_view.scatter_(dim=2, index=rand_idx, src=-torch.ones_like(rand_idx, dtype=rand_idx.dtype))
         idx_buffer_view = idx_buffer_view.view(hsy, wsx, sy, sx).transpose(1, 2).reshape(hsy * sy, wsx * sx)
 
         # Image is not divisible by sx or sy so we need to move it into a new buffer
@@ -116,8 +117,8 @@
         out = torch.zeros(B, N, c, device=x.device, dtype=x.dtype)
         out.scatter_(dim=-2, index=b_idx.expand(B, num_dst, c), src=dst)
         out.scatter_(dim=-2, index=gather(a_idx.expand(B, a_idx.shape[1], 1), dim=1, index=unm_idx).expand(B, unm_len, c), src=unm)
         out.scatter_(dim=-2, index=gather(a_idx.expand(B, a_idx.shape[1], 1), dim=1, index=src_idx).expand(B, r, c), src=src)
 
         return out
 
-    return merge, unmerge
+    return merge, unmerge
```

### Comparing `tomesd-0.1.2/tomesd/patch.py` & `tomesd-0.1.3/tomesd/patch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import torch
 import math
 from typing import Type, Dict, Any, Tuple, Callable
 
 from . import merge
-from .utils import isinstance_str
+from .utils import isinstance_str, init_generator
 
 
 
 def compute_merge(x: torch.Tensor, tome_info: Dict[str, Any]) -> Tuple[Callable, ...]:
     original_h, original_w = tome_info["size"]
     original_tokens = original_h * original_w
     downsample = int(math.ceil(math.sqrt(original_tokens // x.shape[1])))
 
     args = tome_info["args"]
 
     if downsample <= args["max_downsample"]:
         w = int(math.ceil(original_w / downsample))
         h = int(math.ceil(original_h / downsample))
         r = int(x.shape[1] * args["ratio"])
-        # If the batch size is odd, then it's not possible for promted and unprompted images to be in the same
+
+        # Re-init the generator if it hasn't already been initialized or device has changed.
+        if args["generator"] is None:
+            args["generator"] = init_generator(x.device)
+        elif args["generator"].device != x.device:
+            args["generator"] = init_generator(x.device, fallback=args["generator"])
+        
+        # If the batch size is odd, then it's not possible for prompted and unprompted images to be in the same
         # batch, which causes artifacts with use_rand, so force it to be off.
         use_rand = False if x.shape[0] % 2 == 1 else args["use_rand"]
-        m, u = merge.bipartite_soft_matching_random2d(x, w, h, args["sx"], args["sy"], r, not use_rand)
+        m, u = merge.bipartite_soft_matching_random2d(x, w, h, args["sx"], args["sy"], r, 
+                                                      no_rand=not use_rand, generator=args["generator"])
     else:
         m, u = (merge.do_nothing, merge.do_nothing)
 
     m_a, u_a = (m, u) if args["merge_attn"]      else (merge.do_nothing, merge.do_nothing)
     m_c, u_c = (m, u) if args["merge_crossattn"] else (merge.do_nothing, merge.do_nothing)
     m_m, u_m = (m, u) if args["merge_mlp"]       else (merge.do_nothing, merge.do_nothing)
 
@@ -220,14 +228,15 @@
         "size": None,
         "hooks": [],
         "args": {
             "ratio": ratio,
             "max_downsample": max_downsample,
             "sx": sx, "sy": sy,
             "use_rand": use_rand,
+            "generator": None,
             "merge_attn": merge_attn,
             "merge_crossattn": merge_crossattn,
             "merge_mlp": merge_mlp
         }
     }
     hook_tome_model(diffusion_model)
 
@@ -238,14 +247,19 @@
             module.__class__ = make_tome_block_fn(module.__class__)
             module._tome_info = diffusion_model._tome_info
 
             # Something introduced in SD 2.0 (LDM only)
             if not hasattr(module, "disable_self_attn") and not is_diffusers:
                 module.disable_self_attn = False
 
+            # Something needed for older versions of diffusers
+            if not hasattr(module, "use_ada_layer_norm_zero") and is_diffusers:
+                module.use_ada_layer_norm = False
+                module.use_ada_layer_norm_zero = False
+
     return model
 
 
 
 
 
 def remove_patch(model: torch.nn.Module):
@@ -258,8 +272,8 @@
             for hook in module._tome_info["hooks"]:
                 hook.remove()
             module._tome_info["hooks"].clear()
 
         if module.__class__.__name__ == "ToMeBlock":
             module.__class__ = module._parent
     
-    return model
+    return model
```

### Comparing `tomesd-0.1.2/tomesd.egg-info/PKG-INFO` & `tomesd-0.1.3/tomesd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomesd
-Version: 0.1.2
+Version: 0.1.3
 Summary: Token Merging for Stable Diffusion
 Home-page: https://github.com/dbolya/tomesd
 Author: Daniel Bolya
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

