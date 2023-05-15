# Comparing `tmp/acids-msprior-1.0.5.tar.gz` & `tmp/acids-msprior-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-msprior-1.0.5.tar", last modified: Sun May 14 11:10:42 2023, max compression
+gzip compressed data, was "acids-msprior-1.0.6.tar", last modified: Mon May 15 18:48:43 2023, max compression
```

## Comparing `acids-msprior-1.0.5.tar` & `acids-msprior-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:10:42.655165 acids-msprior-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-14 11:10:42.655165 acids-msprior-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:10:42.651165 acids-msprior-1.0.5/acids_msprior.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-14 11:10:42.000000 acids-msprior-1.0.5/acids_msprior.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-14 11:10:42.000000 acids-msprior-1.0.5/acids_msprior.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:10:42.000000 acids-msprior-1.0.5/acids_msprior.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-14 11:10:42.000000 acids-msprior-1.0.5/acids_msprior.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-14 11:10:42.000000 acids-msprior-1.0.5/acids_msprior.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 11:10:42.000000 acids-msprior-1.0.5/acids_msprior.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:10:42.655165 acids-msprior-1.0.5/msprior/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19774 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:10:42.655165 acids-msprior-1.0.5/msprior/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/configs/decoder_only.gin
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/configs/encoder_decoder.gin
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/configs/encoder_decoder_continuous.gin
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/configs/recurrent.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/scripted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:10:42.655165 acids-msprior-1.0.5/msprior_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior_scripts/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior_scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior_scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior_scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/msprior_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 11:10:42.655165 acids-msprior-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:10:42.655165 acids-msprior-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-14 11:07:31.000000 acids-msprior-1.0.5/tests/test_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:48:43.976650 acids-msprior-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 18:48:43.976650 acids-msprior-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:48:43.972650 acids-msprior-1.0.6/acids_msprior.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 18:48:43.000000 acids-msprior-1.0.6/acids_msprior.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-15 18:48:43.000000 acids-msprior-1.0.6/acids_msprior.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:48:43.000000 acids-msprior-1.0.6/acids_msprior.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 18:48:43.000000 acids-msprior-1.0.6/acids_msprior.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 18:48:43.000000 acids-msprior-1.0.6/acids_msprior.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 18:48:43.000000 acids-msprior-1.0.6/acids_msprior.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:48:43.972650 acids-msprior-1.0.6/msprior/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19976 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:48:43.972650 acids-msprior-1.0.6/msprior/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/configs/decoder_only.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/configs/encoder_decoder.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/configs/encoder_decoder_continuous.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/configs/recurrent.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/scripted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:48:43.976650 acids-msprior-1.0.6/msprior_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior_scripts/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior_scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior_scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior_scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/msprior_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:48:43.976650 acids-msprior-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:48:43.976650 acids-msprior-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-15 18:45:17.000000 acids-msprior-1.0.6/tests/test_configs.py
```

### Comparing `acids-msprior-1.0.5/PKG-INFO` & `acids-msprior-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.5
+Version: 1.0.6
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.5 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.6 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.5/README.md` & `acids-msprior-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/acids_msprior.egg-info/PKG-INFO` & `acids-msprior-1.0.6/acids_msprior.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.5
+Version: 1.0.6
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.5 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.6 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.5/acids_msprior.egg-info/SOURCES.txt` & `acids-msprior-1.0.6/acids_msprior.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior/attention.py` & `acids-msprior-1.0.6/msprior/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import math
 from typing import Callable, Dict, Optional, Sequence, Tuple
 
 import cached_conv as cc
 import gin
 import pytorch_lightning as pl
 import torch
@@ -287,30 +288,34 @@
                  num_tokens: int,
                  num_features: int,
                  num_quantizers: int,
                  from_pretrained: Optional[str] = None) -> None:
         super().__init__()
         self.from_pretrained = from_pretrained
 
+        self.embedder = nn.Embedding(num_quantizers * num_tokens, num_features)
+        self.proj = None
+
         if from_pretrained is not None:
-            model = torch.jit.load(from_pretrained).eval()
-            embeds = []
-            for n, p in model.encoder.rvq.named_buffers():
-                if n[-14:] == "codebook.embed":
-                    embeds.append(p)
-            embeds = torch.cat(embeds, 0)
-
-            self.embedder = nn.Embedding(num_quantizers * num_tokens,
-                                         embeds.shape[-1])
-            self.embedder.weight.data.copy_(embeds)
-            self.proj = nn.Linear(embeds.shape[-1], num_features)
-        else:
-            self.embedder = nn.Embedding(num_quantizers * num_tokens,
-                                         num_features)
-            self.proj = None
+            if hasattr(model.encoder, "rvq"):
+                model = torch.jit.load(from_pretrained).eval()
+                embeds = []
+                for n, p in model.encoder.rvq.named_buffers():
+                    if n[-14:] == "codebook.embed":
+                        embeds.append(p)
+                embeds = torch.cat(embeds, 0)
+
+                self.embedder = nn.Embedding(num_quantizers * num_tokens,
+                                             embeds.shape[-1])
+                self.embedder.weight.data.copy_(embeds)
+                self.proj = nn.Linear(embeds.shape[-1], num_features)
+            else:
+                logging.warn(
+                    "pretrained_embedding is only compatible with discrete rave models, skiping"
+                )
 
         self.num_quantizers = num_quantizers
         self.num_tokens = num_tokens
 
     def forward(self, x: torch.Tensor,
                 sum_over_quantizers: bool) -> torch.Tensor:
         if sum_over_quantizers:
```

### Comparing `acids-msprior-1.0.5/msprior/configs/decoder_only.gin` & `acids-msprior-1.0.6/msprior/configs/decoder_only.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior/configs/encoder_decoder.gin` & `acids-msprior-1.0.6/msprior/configs/encoder_decoder.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior/configs/encoder_decoder_continuous.gin` & `acids-msprior-1.0.6/msprior/configs/encoder_decoder_continuous.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior/dataset.py` & `acids-msprior-1.0.6/msprior/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior/preprocessor.py` & `acids-msprior-1.0.6/msprior/preprocessor.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior/scripted.py` & `acids-msprior-1.0.6/msprior/scripted.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,17 @@
                 self.encoder_input_type = "discrete"
             elif isinstance(encoder_embedder(), FeatureEmbedding):
                 if vae_path is not None:
                     self.encoder_input_type = "vae"
                     self.feature_vae = torch.jit.load(vae_path).eval()
                     num_inputs += self.feature_vae.latent_size
                 else:
-                    num_inputs += 163  # TODO: put that somewhere in configuration files
+                    feature_dim = gin.get_bindings(
+                        "attention.FeatureEmbedding")["in_features"]
+                    num_inputs += feature_dim
                     self.encoder_input_type = "full"
             else:
                 raise ValueError(
                     f"Unknown encoder embedder {encoder_embedder}")
 
             self.encoder_ratio = gin.get_bindings(
                 "decoder/attention.TransformerLayer")["encoder_out_ratio"]
@@ -90,17 +92,21 @@
         ]
 
         if self.encoder_input_type == "none":
             pass
         elif self.encoder_input_type == "discrete":
             input_labels.append("semantic tokens")
         elif self.encoder_input_type == "vae":
-            input_labels.extend([f"semantic latent {i}" for i in range(8)])
+            input_labels.extend([
+                f"semantic latent {i}"
+                for i in range(self.feature_vae.latent_size)
+            ])
         elif self.encoder_input_type == "full":
-            input_labels.extend([f"semantic feature {i}" for i in range(163)])
+            input_labels.extend(
+                [f"semantic feature {i}" for i in range(feature_dim)])
         else:
             raise ValueError(
                 f"Encoder input type {self.encoder_input_type} not understood."
             )
 
         output_labels = [
             f"rave latent {i+1}" for i in range(self.num_rave_quantizers)
```

### Comparing `acids-msprior-1.0.5/msprior/task.py` & `acids-msprior-1.0.6/msprior/task.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior/utils.py` & `acids-msprior-1.0.6/msprior/utils.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior_scripts/compact.py` & `acids-msprior-1.0.6/msprior_scripts/compact.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior_scripts/export.py` & `acids-msprior-1.0.6/msprior_scripts/export.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior_scripts/main_cli.py` & `acids-msprior-1.0.6/msprior_scripts/main_cli.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior_scripts/preprocess.py` & `acids-msprior-1.0.6/msprior_scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/msprior_scripts/train.py` & `acids-msprior-1.0.6/msprior_scripts/train.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/setup.py` & `acids-msprior-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/tests/test_attention.py` & `acids-msprior-1.0.6/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/tests/test_cache.py` & `acids-msprior-1.0.6/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.5/tests/test_configs.py` & `acids-msprior-1.0.6/tests/test_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 
 
 @pytest.mark.parametrize("config,continuous,listen", configs, ids=names)
 def test_config(config, continuous, listen):
     gin.clear_config()
     gin.parse_config_file(config)
 
-    model = ScriptedPrior(from_continuous=continuous, initial_listen=listen)
+    model = ScriptedPrior(
+        from_continuous=continuous,
+        initial_listen=listen,
+    )
 
     if listen and not continuous:
         x = torch.randint(0, 16, (1, model.forward_params[0], 8)).float()
         y = model(x)
         assert torch.allclose(y[:, :-1].float(), x[:, :y.shape[1] - 1].float())
 
         x = torch.randint(0, 16, (4, model.forward_params[0], 8)).float()
```

