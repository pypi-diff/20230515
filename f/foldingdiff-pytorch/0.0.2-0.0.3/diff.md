# Comparing `tmp/foldingdiff-pytorch-0.0.2.tar.gz` & `tmp/foldingdiff-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foldingdiff-pytorch-0.0.2.tar", last modified: Sun May 14 15:41:25 2023, max compression
+gzip compressed data, was "foldingdiff-pytorch-0.0.3.tar", last modified: Mon May 15 09:03:41 2023, max compression
```

## Comparing `foldingdiff-pytorch-0.0.2.tar` & `foldingdiff-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/foldingdiff_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:41.423918 foldingdiff-pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-15 09:03:41.423918 foldingdiff-pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:41.419918 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/foldingdiff_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:41.423918 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-15 09:03:41.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 09:03:41.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:03:41.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 09:03:41.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 09:03:41.000000 foldingdiff-pytorch-0.0.3/foldingdiff_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:03:41.423918 foldingdiff-pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-15 09:03:30.000000 foldingdiff-pytorch-0.0.3/setup.py
```

### Comparing `foldingdiff-pytorch-0.0.2/PKG-INFO` & `foldingdiff-pytorch-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldingdiff-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial implementation of foldingdiff in PyTorch.
 Home-page: https://github.com/dohlee/foldingdiff-pytorch
 Author: Dohoon Lee
 Author-email: dohlee.bioinfo@gmail.com
 License: MIT
 Keywords: artificial intelligence,bioinformatics,computational biology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/data.py` & `foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,14 @@
         self.T = T
         self.max_len = max_len
 
         # Cosine variance schedule
         t = torch.arange(T + 1)
         f_t = torch.cos((t / T + s) / (1 + s) * math.pi / 2.0).square()
         self.alpha_bar = f_t / f_t[0]
-        self.beta = torch.clip(1 - self.alpha_bar[1:] / self.alpha_bar[:-1], min=0.001, max=0.999)
-        self.alpha = 1 - self.beta
 
         self.alpha_bar_sqrt = torch.sqrt(self.alpha_bar)
         self.one_minus_alpha_bar_sqrt = torch.sqrt(1 - self.alpha_bar)
 
         if mu is None:
             feats = []
             for r in self.records:
```

### Comparing `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/foldingdiff_pytorch.py` & `foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/foldingdiff_pytorch.py`

 * *Files identical despite different names*

### Comparing `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/sample.py` & `foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,60 +3,72 @@
 import math
 
 from tqdm import tqdm
 
 from foldingdiff_pytorch import FoldingDiff
 from foldingdiff_pytorch.util import wrap
 
+DEFAULT_MU = [
+    -1.311676263809204,
+    0.620250940322876,
+    0.3829933702945709,
+    1.940455198287964,
+    2.0217323303222656,
+    2.108278274536133
+]
 
 def parse_argument():
     parser = argparse.ArgumentParser()
     parser.add_argument('--ckpt', type=str, default='Model checkpoint')
     parser.add_argument('--timepoints', type=int, default=1000)
+    parser.add_argument('--num-residues', type=int, default=64)
+    parser.add_argument('--batch-size', type=int, default=10)
+    parser.add_argument('--mu', type=int, nargs='+', default=DEFAULT_MU)
     parser.add_argument('--output', type=str, required=True)
     return parser.parse_args()
 
 def main():
     args = parse_argument()
     T = args.timepoints
+    mu = torch.tensor(args.mu).float()
 
     # Load model
     model = FoldingDiff()
 
     state_dict = torch.load(args.ckpt)['state_dict']
     model.load_state_dict(state_dict)
 
     model.eval()
 
     s = 8e-3
     t = torch.arange(T + 1)
     f_t = torch.cos((t / T + s) / (1 + s) * math.pi / 2.0).square()
     alpha_bar = f_t / f_t[0]
-    beta = torch.cat([torch.tensor([0.0]), torch.clip(1 - alpha_bar[1:] / alpha_bar[:-1], min=0.001, max=0.999)])
+    beta = torch.cat([torch.tensor([0.0]), torch.clip(1 - alpha_bar[1:] / alpha_bar[:-1], min=1e-5, max=1 - 1e-5)])
     alpha = 1 - beta
 
     trajectory = []
     with torch.no_grad():
 
-        x = wrap(torch.randn(1, 64, 6))
-        trajectory.append(x)
+        x = wrap(torch.randn(args.batch_size, args.num_residues, 6))
+        trajectory.append(x.unsqueeze(1))
 
         for t in tqdm(range(T, 0, -1), desc='sampling'):
             sigma_t = math.sqrt( (1 - alpha_bar[t-1]) / (1 - alpha_bar[t]) * beta[t] )
 
             # Sample from N(0, sigma_t^2)
             if t > 1:
-                z = torch.randn(1, 64, 6) * sigma_t
+                z = torch.randn(args.batch_size, args.num_residues, 6) * sigma_t
             else:
-                z = torch.zeros(1, 64, 6)
+                z = torch.zeros(args.batch_size, args.num_residues, 6)
 
             # Update x
             t_tensor = torch.tensor([t]).long().unsqueeze(0)
             x = wrap( 1 / math.sqrt(alpha[t]) * (x - beta[t] / math.sqrt(1 - alpha_bar[t]) * model(x, t_tensor)) + z)
 
-            trajectory.append(x)
+            trajectory.append(x.unsqueeze(1))
 
-    trajectory = torch.cat(trajectory, dim=0)
+    trajectory = wrap( torch.cat(trajectory, dim=1) + mu )
     torch.save(trajectory, args.output)
 
 if __name__ == '__main__':
     main()
```

### Comparing `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/train.py` & `foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/train.py`

 * *Files identical despite different names*

### Comparing `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/util.py` & `foldingdiff-pytorch-0.0.3/foldingdiff_pytorch/util.py`

 * *Files identical despite different names*

### Comparing `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/PKG-INFO` & `foldingdiff-pytorch-0.0.3/foldingdiff_pytorch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldingdiff-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial implementation of foldingdiff in PyTorch.
 Home-page: https://github.com/dohlee/foldingdiff-pytorch
 Author: Dohoon Lee
 Author-email: dohlee.bioinfo@gmail.com
 License: MIT
 Keywords: artificial intelligence,bioinformatics,computational biology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `foldingdiff-pytorch-0.0.2/setup.py` & `foldingdiff-pytorch-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'foldingdiff-pytorch',
   packages = find_packages(exclude=[]),
   include_package_data = True,
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Unofficial implementation of foldingdiff in PyTorch.',
   author = 'Dohoon Lee',
   author_email = 'dohlee.bioinfo@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/dohlee/foldingdiff-pytorch',
   keywords = [
```

