# Comparing `tmp/dl2050nn-1.0.73.tar.gz` & `tmp/dl2050nn-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl2050nn-1.0.73.tar", last modified: Mon May 15 21:06:12 2023, max compression
+gzip compressed data, was "dist/dl2050nn-1.0.8.tar", last modified: Thu Nov 19 10:46:03 2020, max compression
```

## Comparing `dl2050nn-1.0.73.tar` & `dl2050nn-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 jn         (501) staff       (20)        0 2023-05-15 21:06:12.942290 dl2050nn-1.0.73/
--rw-r--r--   0 jn         (501) staff       (20)      559 2023-05-15 21:06:12.942336 dl2050nn-1.0.73/PKG-INFO
-drwxr-xr-x   0 jn         (501) staff       (20)        0 2023-05-15 21:06:12.942264 dl2050nn-1.0.73/dl2050nn/
--rw-r--r--   0 jn         (501) staff       (20)      777 2022-01-10 16:59:53.806514 dl2050nn-1.0.73/dl2050nn/__config__.py
--rw-r--r--   0 jn         (501) staff       (20)        0 2019-12-19 00:55:00.000000 dl2050nn-1.0.73/dl2050nn/__init__.py
--rw-r--r--   0 jn         (501) staff       (20)       18 2023-05-15 21:06:12.897893 dl2050nn-1.0.73/dl2050nn/__version__.py
--rw-r--r--   0 jn         (501) staff       (20)     4054 2022-01-20 10:55:49.519714 dl2050nn-1.0.73/dl2050nn/cbs.py
--rw-r--r--   0 jn         (501) staff       (20)    12923 2022-11-29 13:15:20.738898 dl2050nn-1.0.73/dl2050nn/data.py
--rw-r--r--   0 jn         (501) staff       (20)    15762 2022-11-22 15:37:28.454163 dl2050nn-1.0.73/dl2050nn/etc.py
--rw-r--r--   0 jn         (501) staff       (20)     5303 2023-04-02 15:46:36.231541 dl2050nn-1.0.73/dl2050nn/learner.py
--rw-r--r--   0 jn         (501) staff       (20)     6764 2022-06-15 10:10:29.526716 dl2050nn-1.0.73/dl2050nn/log.py
--rw-r--r--   0 jn         (501) staff       (20)      385 2020-06-11 09:57:52.000000 dl2050nn-1.0.73/dl2050nn/loss.py
--rw-r--r--   0 jn         (501) staff       (20)     4847 2022-08-30 08:42:12.761610 dl2050nn-1.0.73/dl2050nn/metrics.py
--rw-r--r--   0 jn         (501) staff       (20)    12589 2023-05-15 21:06:05.993258 dl2050nn-1.0.73/dl2050nn/models.py
--rw-r--r--   0 jn         (501) staff       (20)     7495 2023-02-21 09:47:11.903181 dl2050nn-1.0.73/dl2050nn/optimizers.py
--rw-r--r--   0 jn         (501) staff       (20)    10029 2023-05-04 14:50:21.583997 dl2050nn-1.0.73/dl2050nn/results.py
--rw-r--r--   0 jn         (501) staff       (20)     3237 2022-06-15 10:14:31.679083 dl2050nn-1.0.73/dl2050nn/runner.py
--rw-r--r--   0 jn         (501) staff       (20)     7592 2022-01-07 14:37:01.742140 dl2050nn-1.0.73/dl2050nn/tabular.py
--rw-r--r--   0 jn         (501) staff       (20)      331 2020-05-29 18:11:17.000000 dl2050nn-1.0.73/dl2050nn/transforms.py
--rw-r--r--   0 jn         (501) staff       (20)       39 2020-11-19 09:53:05.000000 dl2050nn-1.0.73/setup.cfg
--rw-r--r--   0 jn         (501) staff       (20)     1037 2022-01-10 17:04:51.013662 dl2050nn-1.0.73/setup.py
+drwxr-xr-x   0 jneto      (501) staff       (20)        0 2020-11-19 10:46:03.614464 dl2050nn-1.0.8/
+-rw-r--r--   0 jneto      (501) staff       (20)      499 2020-11-19 10:46:03.614548 dl2050nn-1.0.8/PKG-INFO
+drwxr-xr-x   0 jneto      (501) staff       (20)        0 2020-11-19 10:46:03.614365 dl2050nn-1.0.8/dl2050nn/
+-rw-r--r--   0 jneto      (501) staff       (20)        0 2019-12-19 00:55:00.000000 dl2050nn-1.0.8/dl2050nn/__init__.py
+-rw-r--r--   0 jneto      (501) staff       (20)     4090 2020-11-09 10:43:02.075886 dl2050nn-1.0.8/dl2050nn/cbs.py
+-rw-r--r--   0 jneto      (501) staff       (20)    12396 2020-11-17 09:56:29.411999 dl2050nn-1.0.8/dl2050nn/data.py
+-rw-r--r--   0 jneto      (501) staff       (20)    12402 2020-11-09 10:43:25.996413 dl2050nn-1.0.8/dl2050nn/etc.py
+-rw-r--r--   0 jneto      (501) staff       (20)     5488 2020-11-09 10:43:34.794759 dl2050nn-1.0.8/dl2050nn/learner.py
+-rw-r--r--   0 jneto      (501) staff       (20)     9156 2020-11-09 10:43:41.702894 dl2050nn-1.0.8/dl2050nn/log.py
+-rw-r--r--   0 jneto      (501) staff       (20)      385 2020-06-11 09:57:52.000000 dl2050nn-1.0.8/dl2050nn/loss.py
+-rw-r--r--   0 jneto      (501) staff       (20)     4271 2020-09-02 07:07:37.000000 dl2050nn-1.0.8/dl2050nn/metrics.py
+-rw-r--r--   0 jneto      (501) staff       (20)     9310 2020-10-09 12:52:04.869968 dl2050nn-1.0.8/dl2050nn/models.py
+-rw-r--r--   0 jneto      (501) staff       (20)     7052 2020-11-19 08:47:35.711062 dl2050nn-1.0.8/dl2050nn/optimizers.py
+-rw-r--r--   0 jneto      (501) staff       (20)     9933 2020-10-14 10:25:46.443389 dl2050nn-1.0.8/dl2050nn/results.py
+-rw-r--r--   0 jneto      (501) staff       (20)     7592 2020-11-09 10:44:13.512840 dl2050nn-1.0.8/dl2050nn/tabular.py
+-rw-r--r--   0 jneto      (501) staff       (20)      331 2020-05-29 18:11:17.000000 dl2050nn-1.0.8/dl2050nn/transforms.py
+-rw-r--r--   0 jneto      (501) staff       (20)       39 2020-11-19 09:53:05.683295 dl2050nn-1.0.8/setup.cfg
+-rw-r--r--   0 jneto      (501) staff       (20)     1208 2020-11-19 10:46:03.357371 dl2050nn-1.0.8/setup.py
```

### Comparing `dl2050nn-1.0.73/dl2050nn/cbs.py` & `dl2050nn-1.0.8/dl2050nn/cbs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import re
-import random
-from functools import partial
+import time, re, os
+import math, random
 import numpy as np
 import pandas as pd
+from functools import partial
 import torch
+from torch import tensor
 import matplotlib.pyplot as plt
 import matplotlib as mpl
-from dl2050utils.core import listify, camel2snake
-from dl2050nn.etc import *
+from dlogicutils.core import listify, camel2snake
+from nn2.etc import *
 
 
 def randn(n): return random.randint(0,n)
 
 
 class Callback():
     _order=0
```

### Comparing `dl2050nn-1.0.73/dl2050nn/data.py` & `dl2050nn-1.0.8/dl2050nn/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,231 +1,224 @@
 import random
+import feather
 import numpy as np
 import torch
 import torchvision.transforms as transforms
 from PIL import Image
 from IPython.display import display
-from dl2050utils.core import *
-from dl2050utils.fs import get_dir_files, get_dir_dirs
-from dl2050nn.etc import *
-from dl2050nn.tabular import DataFrameProcessor
+from dlogicutils.core import *
+from dlogicutils.fs import get_dir_files, get_dir_dirs
+from nn2.etc import *
+from nn2.tabular import DataFrameProcessor
 
 # if regr:
 #     yrange = [df[c_dep].astype('float32').min(), df[c_dep].astype('float32').max()]
 
+
 ################################################################################################################################
 #  DataLoader
 #
 # TODO: num_workers, pin_memory
 ################################################################################################################################
 
 def get_balanced_idxs(c_idxs, p=0.):
     p = min(max(p,0.),1.)
     szs = np.array([len(e) for e in c_idxs])
     n = szs.sum()
     bp0 = np.array([len(c)/n for c in c_idxs])
     bp1 = np.array([1/len(c_idxs)]*len(c_idxs))
-    bp = bp0 + p*(bp1-bp0)
+    bp = bp0+p*(bp1-bp0)
     m = bp/bp0
     szs2 = np.round((szs*m/m.min())).astype(int)
     z = np.array([])
     for i in range(len(c_idxs)):
-        for _ in range(szs2[i]//szs[i]):
-            z = np.concatenate((z,np.array(c_idxs[i])))
+        for _ in range(szs2[i]//szs[i]): z = np.concatenate((z,np.array(c_idxs[i])))
         z = np.concatenate((z,np.array(c_idxs[i])[:szs2[i]%szs[i]]))
     z = np.random.permutation(z)
     return z.astype(int)
 
+
 def collate(b):
     x,y = zip(*b)
     return torch.stack(x),torch.stack(y)
 
 class SimpleSampler():
     def __init__(self, ds, bs):
-        self.n,self.bs = len(ds),bs
-    def set_balance(self, p):
-        pass
+        self.n, self.bs = len(ds), bs
+    def set_balance(self, p): pass
     def __iter__(self):
         self.idxs = list(range(0,self.n))
         for i in range(0, self.n, self.bs): yield self.idxs[i:i+self.bs]
 
 class RandomSampler():
-    def __init__(self, ds, bs, c_idxs):
-        self.n,self.bs,self.c_idxs,self.p = len(ds),bs,c_idxs,None
-    def set_balance(self, p):
-        self.p = p
+    def __init__(self, ds, bs, c_idxs): self.n, self.bs, self.c_idxs, self.p = len(ds), bs, c_idxs, None
+    def set_balance(self, p): self.p = p
     def __iter__(self):
-        if self.p is None or self.c_idxs is None:
+        if self.p is None:
             self.idxs = list(np.random.permutation(np.arange(self.n)))
         else:
             self.idxs = list(get_balanced_idxs(self.c_idxs, p=self.p))
         for i in range(0, self.n, self.bs): yield self.idxs[i:i+self.bs]
 
+
 class DataLoader():
     def __init__(self, ds, bs=64, shuffle=False, collate_fn=collate):
         self.ds, self.bs, self.collate_fn, self.n = ds, bs, collate_fn, len(ds)
         self.sampler = SimpleSampler(ds, bs) if not shuffle else RandomSampler(ds, bs, self.ds.c_idxs)
     def set_balance(self, p): self.sampler.set_balance(p)
     def __len__(self): return math.ceil(len(self.ds)/self.bs)
     def __iter__(self):
         for b in self.sampler: yield self.collate_fn([self.ds[i] for i in b])
 
+
 ################################################################################################################################
-# Dataset, Data
-#
-# Classification: y type is list or numpy long
-# Mask of integers: 2D classification
-# Mask of floats: ???
-# Regression: y type is float scalar
-#
+#  Dataset, Data
 ################################################################################################################################
 
 class Dataset():
-    def __init__(self, x, y, aug_size=None, clsf=False, cls_to_idx=None, cls=None, regr=False, trfs=[], show=True):
-        self.x,self.y,self.aug_size,self.clsf,self.regr,self.trfs,self.show = x,y,aug_size,clsf,regr,trfs or [],show
-        self.bps,self.c_idxs = None,None
+    def __init__(self, x, y, clsf=False, cls_to_idx=None, regr=False, trfs=[]):
+        self.x, self.y, self.clsf, self.regr, self.trfs = x, y, clsf, regr, trfs or []
+        self.bps = None
+        self.cls, self.c, self.cls_to_idx, self.c_idxs, self.c_szs, self.c_dist = None, None, None, None, None, None
         if clsf:
-            y,self.cls,self.c,self.labels,self.cls_to_idx,self.c_idxs,self.c_szs,self.c_dist = prep_cls(y, cls_to_idx=cls_to_idx, cls=cls)
-            self.y = y.astype(np.int32)
-            if show: show_clsf_stats(self.y, self.c, self.cls, self.c_szs, self.c_dist)
-        else:
-            self.y = y.astype(np.float32)
-        self.x = x #.astype(np.float64)
-        
-    def __len__(self): return self.aug_size or len(self.x)
+            assert type(y)==list
+            self.labels = [str(e) for e in y]
+            if cls_to_idx is None:
+                self.cls = sorted(list(set(self.labels)))
+                self.cls_to_idx = {self.cls[i]: i for i in range(len(self.cls))}
+            else:
+                self.cls = [e for e in cls_to_idx]
+                self.cls_to_idx = cls_to_idx
+                for label in self.labels:
+                    if label not in self.cls:
+                        print(f'Label {label} not found in cls_to_idx')
+                        raise Exception()
+            self.c = len(self.cls)
+            self.y = torch.tensor([self.cls_to_idx[label] for label in self.labels])
+            self.c_idxs, self.c_szs, self.c_dist = get_cls_dist(self.labels, self.cls_to_idx)
+            print(f'\n{self.__class__.__name__} for Classification: size: {len(self.y)}, cls: {self.c}')
+            show_dist(self.labels)
+    def __len__(self): return len(self.x)
     def __getitem__(self, i):
-        if self.aug_size: i=random.randint(0,len(self.x)-1)
         x,y = self.load(self.x[i], self.y[i])
-        for trf in self.trfs: x,y=trf(x,y)
-        x = torch.from_numpy(x).float()
-        y = torch.from_numpy(y) if len(y.shape)>0 else torch.tensor(y).float()
-        if self.clsf: y = y.long()
+        for trf in self.trfs: x = trf(x)
         return x,y
     def load(self, x, y): return x,y
-    def show_data(self, idxs, labels=None):
+    def show(self, idxs, labels=None):
         for idx in listify(idxs):
             x,y = self[idx]
             print(x.shape, y.shape)
     def show_trfs(self, n=8): self.show([random.randint(0,len(self))]*n)
     def encode(self, x, y): pass
     def decode(self,x,y): return x.numpy(),y.item()
 
 
 class Data:
-    def __init__(self, ds1, ds2, bs=64, show=True):
-        self.ds1,self.ds2, self.bs,self.show =  ds1,ds2,bs,show
+    def __init__(self, ds1, ds2, clsf=False, regr=False, bs=64):
+        self.ds1, self.ds2 =  ds1, ds2
+        self.clsf, self.regr, self.bs = clsf, regr, bs
         # w, pin = 0, torch.cuda.is_available()
         self.dl1 = DataLoader(ds1, bs=bs, shuffle=True)
         self.dl2 = DataLoader(ds2, bs=bs, shuffle=False) if ds2 is not None else None
 
     def show_batch(self, n=8): self.ds1.show(next(iter(self.dl1.sampler))[:n])
     def show_batch_2(self, n=8): self.ds2.show(next(iter(self.dl2.sampler))[:n])
     def show_trfs(self, n=8): self.ds1.show_trfs(n=n)
 
     @property
-    def clsf(self): return self.ds1.clsf
-    @property
-    def regr(self): return self.ds1.regr
-    @property
     def c(self): return self.ds1.c if self.clsf else None
     @property
     def cls(self): return self.ds1.cls if self.clsf else None
     @property
     def cls_to_idx(self): return self.ds1.cls_to_idx if self.clsf else None
 
-    @classmethod
-    def from_numpy(cls, x1, y1, x2, y2, aug_size1=None, aug_size2=None, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64, show=True):
-        ds1 = Dataset(x1, y1,aug_size=aug_size1, clsf=clsf, regr=regr, trfs=trfs1, show=show)
-        ds2 = Dataset(x2, y2, aug_size=aug_size2, clsf=clsf, regr=regr, trfs=trfs2, show=show)
-        return cls(ds1, ds2, bs=bs)
-
-################################################################################################################################
-#  SignalDataset, SignalData
-################################################################################################################################
-
-class SignalDataset(Dataset):    
-    def __init__(self, *args, **kwargs):
-        super(SignalDataset, self).__init__(*args, **kwargs)
-    def show_data(self, idxs, labels=None):
-        idxs, labels = listify(idxs), listify(labels)
-        for i,idx in enumerate(idxs):
-            x,y = self.decode(*self[idx])
-            if self.clsf: y = self.cls[y]
-            label = labels[i] if len(labels) else y
-            sigshow(x, label or y)
-
-class SignalData(Data):
-    def __init__(self, x1, y1, x2, y2, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64, show=True):
-        ds1 = SignalDataset(x1, y1, clsf=clsf, regr=regr, trfs=trfs1, show=show)
-        ds2 = SignalDataset(x2, y2, clsf=clsf, regr=regr, trfs=trfs2, show=show)
-        super(SignalData, self).__init__(ds1, ds2, bs=bs)
-        
-    @classmethod
-    def from_numpy(cls, x1, y1, x2, y2, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64, show=True):
-        # x1,x2 = torch.from_numpy(x1).float(),torch.from_numpy(x2).float()
-        # if clsf: y1, y2 = list(y1), list(y2)
-        # else: y1, y2 = torch.from_numpy(y1).float(), torch.from_numpy(y2).float()
-        return cls(x1, y1, x2, y2, clsf=clsf, regr=regr, trfs1=trfs1, trfs2=trfs2, bs=bs, show=show)
 
 ################################################################################################################################
 #  ImageDataset, ImageDatasetMem, ImageData
 ################################################################################################################################
 
 class ImageDataset(Dataset):    
     def load(self,x,y): return Image.open(x),y
     def decode(self, x, y): return transforms.ToPILImage()(x),y
-    def show_data(self, idxs, labels=None):
+    def show(self, idxs, labels=None):
         idxs, labels = listify(idxs), listify(labels)
         x,y = zip(*[self.decode(*self[idx]) for idx in idxs])
         x = np.stack([np.array(x) for x in x])
         if self.clsf: y = [self.cls[e] for e in y]
         imgrid(x, labels or y)
 
 
 class ImageDatasetMem(ImageDataset):
     def load(self,x,y): return x,y
     def decode(self,x,y): return x.numpy().transpose((1,2,0)),y
 
 
 class ImageData(Data):
-    def __init__(self, x1, y1, x2, y2, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64, ds_class=ImageDataset, show=True):
-        ds1 = ds_class(x1, y1, clsf=clsf, regr=regr, trfs=trfs1, show=show)
-        ds2 = ds_class(x2, y2, clsf=clsf, regr=regr, trfs=trfs2, cls_to_idx=ds1.cls_to_idx, show=show)
-        super(ImageData, self).__init__(ds1, ds2, clsf=clsf, regr=regr, bs=bs, show=show)
+    def __init__(self, x1, y1, x2, y2, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64, ds_class=ImageDataset):
+        ds1 = ds_class(x1, y1, clsf=clsf, regr=regr, trfs=trfs1)
+        ds2 = ds_class(x2, y2, clsf=clsf, regr=regr, trfs=trfs2, cls_to_idx=ds1.cls_to_idx)
+        super(ImageData, self).__init__(ds1, ds2, clsf=clsf, regr=regr, bs=bs)
         
     @classmethod
     def from_folder(cls, path1, path2, types=None, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64):
         x, y = [[],[]], [[],[]]
         cls_names = [d.stem for d in get_dir_dirs(path1)]
         for i,path in enumerate([path1, path2]):
             for c in cls_names:
                 for f in get_dir_files(path/f'{c}', types):
                     x[i].append(f)
                     y[i].append(c)
         return cls(x[0], y[0], x[1], y[1], clsf=clsf, regr=regr, trfs1=trfs1, trfs2=trfs2, bs=bs)
 
     @classmethod
-    def from_numpy(cls, x1, y1, x2, y2, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64, show=True):
+    def from_numpy(cls, x1, y1, x2, y2, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64):
         x1, y1, x2, y2 = T(x1).float(), y1, T(x2).float(), y2
-        return cls(x1, y1, x2, y2, clsf=clsf, regr=regr, trfs1=trfs1, trfs2=trfs2, bs=bs, ds_class=ImageDatasetMem, show=show)
+        return cls(x1, y1, x2, y2, clsf=clsf, regr=regr, trfs1=trfs1, trfs2=trfs2, bs=bs, ds_class=ImageDatasetMem)
+
+################################################################################################################################
+#  SignalDataset, SignalData
+################################################################################################################################
+
+class SignalDataset(Dataset):    
+    def show(self, idxs, labels=None):
+        idxs, labels = listify(idxs), listify(labels)
+        for i,idx in enumerate(idxs):
+            x,y = self.decode(*self[idx])
+            if self.clsf: y = self.cls[y]
+            label = labels[i] if len(labels) else y
+            sigshow(x, label or y)
+
+class SignalData(Data):
+    def __init__(self, x1, y1, x2, y2, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64):
+        ds1 = SignalDataset(x1, y1, clsf=clsf, regr=regr, trfs=trfs1)
+        ds2 = SignalDataset(x2, y2, clsf=clsf, regr=regr, trfs=trfs2)
+        super(SignalData, self).__init__(ds1, ds2, clsf=clsf, regr=regr, bs=bs)
+        
+    @classmethod
+    def from_numpy(cls, x1, y1, x2, y2, clsf=False, regr=False, trfs1=[], trfs2=[], bs=64):
+        x1, x2 = torch.from_numpy(x1).float(), torch.from_numpy(x2).float()
+        if clsf: y1, y2 = list(y1), list(y2)
+        else: y1, y2 = torch.from_numpy(y1).float(), torch.from_numpy(y2).float()
+        return cls(x1, y1, x2, y2, clsf=clsf, regr=regr, trfs1=trfs1, trfs2=trfs2, bs=bs)
+
 
 ################################################################################################################################
 #   TabularDataset, TabularData
 ################################################################################################################################
 
 class TabularDataset(Dataset):
-    def __init__(self, df, dfp, proc, clsf=False, cls_to_idx=None, regr=False, show=True):
+    def __init__(self, df, dfp, proc, clsf=False, cls_to_idx=None, regr=False):
         self.df, self.dfp = df, dfp
         x  = dfp[proc.c2].values
         x = torch.from_numpy(x).float()
         y = [str(e) for e in df[proc.c_dep].values]
         super(TabularDataset, self).__init__(x, y, clsf=clsf, cls_to_idx=cls_to_idx, regr=regr)
-        if show and len(proc.get_emb_szs()): print(f'Embeddings: {proc.get_emb_szs()}')
+        if len(proc.get_emb_szs()): print(f'Embeddings: {proc.get_emb_szs()}')
 
-    def show_data(self, idxs, labels=None, cols=None):
+    def show(self, idxs, labels=None, cols=None):
         df = self.df.iloc[listify(idxs)][cols or self.df.columns]
         df['results'] = labels
         display(df)
 
 
 class TabularData(Data):
     def __init__(self, df1, df1p, df2, df2p, proc, clsf=False, regr=False, bs=128):
```

### Comparing `dl2050nn-1.0.73/dl2050nn/etc.py` & `dl2050nn-1.0.8/dl2050nn/etc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,23 @@
 import random
 import math
-import datetime
+import itertools
+from collections import defaultdict, Counter, OrderedDict
+from collections.abc import Iterable, Iterator, Generator, Collection
+import sys, datetime
+from pathlib import Path
 import numpy as np
 import pandas as pd
 import torch
 from matplotlib import pyplot as plt
 import seaborn as sns
-from dl2050utils.core import *
-from dl2050utils.ju import in_ipynb
-from IPython.display import display
+from dlogicutils.core import *
+from dlogicutils.ju import in_ipynb
 T = torch.tensor
 
-def get_logprobs(model, x, cuda=True):
-    x = torch.Tensor(x)
-    if cuda and torch.cuda.is_available():
-        x = x.cuda()
-    with torch.no_grad():
-        y2 = model(x)
-    return y2.detach().cpu().numpy()
-
-def get_logprobs_with_batch(model, x, bs=256, cuda=True):
-    return np.vstack([get_logprobs(model, x[i*bs:(i+1)*bs], cuda=cuda) for i in range(math.ceil(len(x)/bs))])
-
-def get_probs_from_logprobs(y2):
-    return np.exp(np.max(y2, axis=1))
-    return np.exp(y2[:,1])
-
-def get_preds_from_logprobs(y2):
-    return y2.argmax(axis=1)
-
-def get_probs(model, x):
-    y2 = get_logprobs(model, x)
-    return get_probs_from_logprobs(y2)
-
-def get_preds(model, x):
-    y2 = get_logprobs(model, x)
-    return get_preds_from_logprobs(y2)
-
-def get_prob_positive(probs, preds):
-    probs2 = np.zeros(len(probs))
-    m = np.where(preds==1)
-    probs2[m] = probs[m]
-    return np.round(probs2,2)
-
-def predict(model, x):
-    x = torch.Tensor(x).cuda()
-    with torch.no_grad():
-        y2 = model(x)
-    y2 = y2.detach().cpu().numpy()
-    preds = y2.argmax(axis=1)
-    return preds
-
-def norm(x):
-    m,s = x.mean(), x.std()
-    return (x-m)/s if s>0 else x
-
-def rebalance_xy(x, y, n=None, k=None):
-    if n is None and k is None:
-        return x,y
-    k1 = len(np.where(y==1)[0])
-    k0 = n if k is None else k1*k
-    m = np.hstack((np.where(y==0)[0][:k0],np.where(y==1)[0]))
-    return x[m],y[m]
-
-def frmt_n(n): return f'{n:,}'.replace(',','.')
-
-def show_clsf_stats(y, c, cls, c_szs, c_dist):
-    df = pd.concat([
-        pd.DataFrame(np.arange(0,len(cls)),columns=['cls']),
-        pd.DataFrame(cls,columns=['labels']),
-        pd.DataFrame(c_szs,columns=['size']),
-        pd.DataFrame(c_dist,columns=['dist'])
-    ], axis=1)
-    print(f'\nClassification dataset: {frmt_n(len(y))} records, {frmt_n(c)} classes')
-    if len(y.shape)>1: print(f'Total number of labels {y.shape} -> {np.asarray(c_szs).sum():,}')
-    display(df)
-
-def prep_cls(y, cls_to_idx=None, cls=None):
-    assert (type(y)==list or type(y)==np.ndarray)
-    
-    size,labels,cls2idx,cls2 = 0,None,None,None
-    if type(y)==list:
-        size = len(y)
-        labels = [str(e) for e in y]
-        if cls_to_idx is not None:
-            cls2idx = cls_to_idx
-            cls2 = [e for e in cls2idx]
-            for label in labels:
-                if label not in cls2:
-                    raise Exception(f'Label {label} not found in cls_to_idx')
-        else:
-            cls2 = sorted(list(set(labels)))
-            cls2idx = {cls2[i]: i for i in range(len(cls2))}
-        if type(y[0])==str:
-            y = [cls2idx[label] for label in labels]
-        y = np.asarray(y)
-        c_idxs = [(y==cls2idx[c]).nonzero()[0] for c in cls2idx]
-    else:
-        y1 = y.flatten()
-        size = len(y1)
-        cls1 = np.unique(y1)
-        c_idxs = [(y==cls1[c]).nonzero()[0] for c in cls1]
-        cls2 = cls or cls1
-    c_szs = [e.shape[0] for e in c_idxs]
-    c_dist = [e.shape[0]/size for e in c_idxs]
-    return y,cls2,len(cls2),labels,cls2idx,c_idxs,c_szs,c_dist
-
-def np_split(x, y, p=.8):
-    idx = np.random.permutation(x.shape[0])
-    k = int(x.shape[0]*p)
-    x,y = x[idx].copy(),y[idx].copy()
-    return x[:k],y[:k],x[k:],y[k:]
-
 def get_sample(x1, y1, x2, y2, sz=1000, sz2=None):
     if sz2 is None: sz2=sz
     p = np.random.permutation(len(x1))
     x1, y1 = x1[p], y1[p]
     p = np.random.permutation(len(x2))
     x2, y2 = x2[p], y2[p]
     return x1[:sz], y1[:sz], x2[:sz2], y2[:sz2]
@@ -190,39 +92,34 @@
 def t2s(t): return f'{int(t)//60:02d}:{int(t)%60:02d}'
 
 
 def get_date_str(): 
     d = datetime.datetime.now()
     return  f'{d.year:04d}{d.month:02d}{d.day:02d}-{d.hour:02d}{d.minute:02d}{d.second:02d}'
 
+
 def get_log_fname(path):
     dirname = path/'runs'
     fname = f'{dirname}/run-{get_date_str()}.csv'
     return fname, dirname
 
+
 def save_model(model, path, stats):
     state = {'state_dict': model.state_dict(), 'stats': stats}
     torch.save(state, path)
 
-def load_model(model, path, cuda=False, inference=False, show=False):
-    state = torch.load(path, map_location='cpu')
+
+def load_model(model, path):
+    state = torch.load(path,  map_location='cpu')
     model.load_state_dict(state['state_dict'])
-    stats = state['stats']
-    if show:
-        pd.options.display.float_format = '{:,.4f}'.format
-        display(pd.DataFrame.from_dict(stats))
-    if cuda and torch.cuda.is_available():
-        model.cuda()
-    if inference:
-        model.eval()
-    return stats
+    return state['stats']
 
 
-def get_model_n_params(model):
-    return sum([p.numel() for p in model.parameters()])
+def get_model_n_params(model): return sum([p.numel() for p in model.parameters()])
+
 
 def xy_shuffle_split(x, y, p=0.2):
     msk = np.random.permutation(len(x))
     n = int(len(x)*p)
     return x[msk[:n]], y[msk[:n]], x[msk[n:]], y[msk[n:]]
 
 
@@ -269,20 +166,19 @@
 
 
 def table(cols, vals):
     pd.options.display.float_format = '{:,.4f}'.format
     display(pd.DataFrame(vals, columns=cols))
 
 
-# Deprecated
-# def show_dist(y):
-#     df = pd.DataFrame(y, columns=['count'])['count'].value_counts()
-#     df = pd.DataFrame(df, index=df.index, columns=['count'])
-#     df['p'] = df['count']/sum(df['count'])
-#     display(df)
+def show_dist(y):
+    df = pd.DataFrame(y, columns=['count'])['count'].value_counts()
+    df = pd.DataFrame(df, index=df.index, columns=['count'])
+    df['p'] = df['count']/sum(df['count'])
+    display(df)
     # print(get_cls_dist_string(self.cls, self.c_szs, self.c_dist))
 
 
 # def calc_norm(self):
 #     xs, ys = [], []
 #     for i in range(len(self)):
 #         x, y = self[i]
```

### Comparing `dl2050nn-1.0.73/dl2050nn/learner.py` & `dl2050nn-1.0.8/dl2050nn/learner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,42 @@
+import os
+import numpy as np
 import torch
-from functools import partial
-import shutil
-from dl2050nn.cbs import CancelBatchException, CancelEpochException, CancelTrainException, LR_Find, Recorder
-from dl2050nn.optimizers import *
-from dl2050nn.log import LoggerCallback
-from dl2050nn.etc import *
+from IPython.display import display, clear_output
+from dlogicutils.core import listify, camel2snake
+from nn2.cbs import CancelBatchException, CancelEpochException, CancelTrainException, LR_Find, Recorder
+from nn2.optimizers import *
+from nn2.log import LoggerCallback
+from nn2.metrics import accuracy
+from nn2.etc import *
+
 
 class Learner():
 
-    def __init__(self, data, model, opt=Adam, loss_f=None, metrics=[], cbs=[], device=None, model_name=None, pre=None, path='/data', save=True, show=True):
+    def __init__(self, data, model, opt=Adam, loss_f=None, metrics=[], cbs=[], device=None, name=None, path='.', save=True, load=False, plot=True):
         if not path.is_dir(): raise Exception()
         if not (path/'models').exists(): (path/'models').mkdir()
-        self.model = model
-        self.model_name,self.path = model_name or str(model.__class__.__name__),path
+        self.name, self.path = name if name is not None else str(model.__class__.__name__), path
+        self.path_model = path/'models'/f'{name}.pth.tar'
         self.data = data
         self.device = 'cpu' if not torch.cuda.is_available() else torch.device(0) if device is None else torch.device(device)
-        if show: print(f'Learner: device={self.device}\nBatch size: {data.bs}')
+        print(f'Learner: device={self.device}\nBatch size: {data.bs}')
+        self.model = model.to(self.device)
         self.opt = opt
         self.optf = self.opt(model.parameters())
         self.loss_f = loss_f
         if self.loss_f is not None: self.loss_f = self.loss_f.to(self.device)
         self.metrics = metrics
         self._init_cbs([LoggerCallback]+cbs)
         self.ep, self.train = 0, False
-        self._save,self.show = save,show
-        if pre:
-            self.load(model_name=pre, update_best=False, show=show)
-        self.model.to(self.device)
+        self._save, self._plot = save, plot
+        if load: self.load()
 
     @property
     def df_best(self): return self.logger.df_best
-
-    def load(self, model_name=None, update_best=True, show=True):
-        p = self.path/'models'/f'{model_name or self.model_name}.pth.tar'
-        stats = load_model(self.model, p, show=show)
-        if not update_best: return
-        self.eval()
-        self.logger.df_best = pd.DataFrame.from_dict(stats)
-        k = 4+len(self.metrics)
-        self.logger.best = self.logger.df_best.iloc[0,k]
-
-    def save(self, model_name=None):
-        p = self.path/'models'/f'{model_name or self.model_name}.pth.tar'
-        save_model(self.model, p, self.logger.df_best.to_dict())
-
-    def backup_model(self, backup_name):
-        p = self.path/f'models/{backup_name}.pth.tar'
-        shutil.copy(self.path/f'models/{self.model_name}.pth.tar', p)
-        print(f'Model backup up: {p}')
     
     def _init_cbs(self, cbs):
         self.cbs = []
         for cb in cbs:
             cb = cb()
             cb.set_learner(self)
             setattr(self, cb.name, cb)
@@ -89,16 +74,16 @@
             self('after_fit')
 
     def all_batches(self, dl):
         if not dl: return
         self.iters = len(dl)
         try:
             for self.iter,(x,y) in enumerate(dl):
-                if len(x)>2: self.one_batch(x, y)
-                # else: print('Skiping batch smaller that 2')
+                if len(x) > 2: self.one_batch(x, y)
+                else: print('Batch smaller that 3, skiping')
                 if self.train: self.epf += 1./self.iters
         except CancelEpochException: self('after_cancel_epoch')
 
     def one_batch(self, x, y):
         try:
             self.x, self.y = x, y
             if self('begin_batch'): return
@@ -120,20 +105,39 @@
     def lr_find(self, max_iter=100, min_lr=1e-6, max_lr=1e1):
         # Backup all cbs
         self._init_cbs([partial(LR_Find, max_iter=max_iter, min_lr=min_lr, max_lr=max_lr), Recorder])
         self.fit(10)
         # Reset optimizer status
 
     def eval(self):
-        if not self.data.dl2:
-            return
+        if not self.data.dl2: return
         self.model.eval()
         with torch.no_grad(): 
             if not self('begin_validate'): self.all_batches(self.data.dl2)
 
+    def save(self, name=None):
+        path_model = self.path_model if name is None else self.path/'models'/f'{name}.pth.tar'
+        save_model(self.model, path_model, self.logger.df_best.to_dict())
+
+    def load(self, name=None, mute=False, update_best=True):
+        path_model = self.path_model if name is None else self.path/'models'/f'{name}.pth.tar'
+        self.logger.best = 0.0 if self.logger.maximize else 1e9
+        self.logger.df_best = None
+        stats = load_model(self.model, path_model)
+        df_best = pd.DataFrame.from_dict(stats)
+        if not mute:
+            print(f'=> model loaded {path_model}')
+            # display(df_best)
+        if update_best:
+            self.logger.df_best = df_best
+            k = 4+len(self.metrics)
+            self.logger.best = self.logger.df_best.iloc[0,k]
+            self.eval()
+            if not mute: self.logger.show_best()
+
     def predict(self, x):
         x = self.data.encode(x)
         self.model.eval()
         with torch.no_grad():
             x = x.to(self.device)
             y = self.model(x)
         return y.detach().cpu()
```

### Comparing `dl2050nn-1.0.73/dl2050nn/log.py` & `dl2050nn-1.0.8/dl2050nn/log.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import time
-import os
-from pathlib import Path
+import datetime, time, re, os
 import numpy as np
 import pandas as pd
 import pickle
 import gc
 import torch
 import matplotlib.pyplot as plt
-from IPython.display import display
-from dl2050utils.ju import disablePrint, enablePrint, force_print
-from dl2050nn.etc import *
-from dl2050nn.cbs import Callback
-from dl2050nn.metrics import *
+from IPython.display import display, clear_output
+from dlogicutils.ju import disablePrint, enablePrint, force_print
+from nn2.etc import *
+from nn2.cbs import Callback
+from nn2.metrics import *
+
 
 def key_metric(learner): return 4+len(learner.metrics)
 
 def metrics_str(metrics):
     if not len(metrics): return ''
     s = ' M: ['
     for v in metrics: s += f'{v:.4f}, '
@@ -77,14 +76,16 @@
             fname, dirname = get_log_fname(self.path)
             if not os.path.exists(dirname): os.makedirs(dirname)
             self.logf = open(fname, 'w', 1)
         self.best = 0.0 if self.maximize else 1e9
         self.results = []
         self.y_ep, self.y2_ep, self.stats_1, self.stats_2, self.t0, self.t1 = None, None, None, None, 0, 0
         self.df, self.df_best = None, None
+        print(f'Logging to {self.mode}')
+        if self.file: print(f'Logging to file: {self.fname}')
         pd.options.display.float_format = '{:,.4f}'.format
         
     def reset_stats(self):
         self.y_ep = torch.tensor([]).long() if self.data.clsf else torch.tensor([]).float()
         self.y2_ep = torch.tensor([]).float()
         self.loss_t, self.n, self.metrics_v = 0., 0, [0.]*len(self.metrics)
         
@@ -103,46 +104,41 @@
 
     def update_historic(self):
         row = [self.ep, self.t2] + [self.loss1] + [e for e in self.metrics1] + [self.loss2] + [e for e in self.metrics2]
         self.results.append(row)
         self.df = pd.DataFrame(self.results, columns=self.cols)
        
     def log_epoch(self):
-        if self.mode == 'ipynb' and self.show and self.eps > 1:
+        if self.mode == 'ipynb' and self._plot and self.eps > 1:
             x = self.df['Epoch'].values
             y = self.df[['Loss_1', 'Loss_2']].values
             y0, y1 = y[:,0], y[:,1] if self.data.dl2 is not None else None
             plot_update(self.fig, self.ax, x, y0, y1)
         s = log_str(self.ep, self.t2, self.loss1, self.loss2, self.metrics1, self.metrics2, self.new_best, valid=self.data.dl2 is not None)
-        if self.show: print(s)
+        print(s)
 
     def begin_fit(self):
         if self.data.dl2 is None: self.best = 1e9
-        if self.mode == 'ipynb' and self.show and self.eps > 1: self.fig, self.ax = plot_init(0, self.eps)
+        if self.mode == 'ipynb' and self._plot and self.eps > 1: self.fig, self.ax = plot_init(0, self.eps)
         self.cols = ['Epoch', 'Time', 'Loss_1'] + [f'{e.__name__}_1' for e in self.metrics] + ['Loss_2'] + [f'{e.__name__}_2' for e in self.metrics]
-        if self.show:
-            if self.file:
-                print(f'Logging to file: {self.fname}')
-            else:
-                print(f'Logging to {self.mode}')
         
     def begin_epoch(self):
         self.t0 = time.time()
         self.reset_stats()
         
     def begin_validate(self):
         self.t1 = time.time() - self.t0
         self.stats_1 = [v for v in self.stats()]
         self.reset_stats()
             
     def after_loss(self):
         with torch.no_grad(): self.accumulate()
         
     def after_batch(self):
-        if self.show: printProgressBar(self.iter, self.iters, f'Ep: {self.ep:d} {"train" if self.train else "eval"}:')
+        printProgressBar(self.iter, self.iters, f'Ep: {self.ep:d} {"train" if self.train else "eval"}:')
 
     def after_epoch(self):
         self.t2 = time.time() - self.t0 if self.t0 is not None else time.time()
         self.stats_2 = [v for v in self.stats()] if self.data.dl2 is not None else [0]*len(self.stats_1)
         self.loss1, self.loss2 = self.stats_1[0], self.stats_2[0] if self.data.dl2 is not None else 0.
         self.metrics1, self.metrics2 = [v for v in self.stats_1[1:]], [v for v in self.stats_2[1:]]
         loss_metric = not len(self.metrics) or self.data.dl2 is None
@@ -160,17 +156,73 @@
         self.update_historic()
         self.log_epoch()
         if self.new_best:
             self.df_best = self.df[self.df['Epoch']==self.ep]
             if self._save: self.save()
         
     def after_fit(self):
-        if self.show: print(f'\nBest: {self.best:.4f}')
+        print(f'\nBest: {self.best:.4f}')
         plt.ioff()
 
     def show_best(self): display(self.df_best)
 
     def plot_loss1_metric2(self):
         if self.df is None: return
         col_ids = [2, 4+len(self.metrics)]
         z = self.df.iloc[:,col_ids].values
         plot(*list(zip(*z))); plt.show(); time.sleep(.01)
+
+
+class Runner:
+    def __init__(self, path, data, get_learner, nruns=10, eps=10, name='Runner', desc='', load=False):
+        self.get_learner, self.data = get_learner, data
+        self.nruns, self.eps, self.name, self.desc = nruns, eps, name, desc
+        if not Path(f'{path}/runners').exists(): Path(f'{path}/runners').mkdir()
+        self.fname = f'{path}/runners/{name}'
+        self.learner, self.df, self.best = None, None, 0.
+        if load: self.load()
+
+    def __call__(self, mute=True):
+        self.best, self.best_file = 0., None
+        if mute: disablePrint()
+        for i in range(self.nruns):
+            force_print(f'\rRun {i}')
+            learner = self.get_learner(self.data, name= f'{self.name}_{i}', plot=False)
+            self.learner = learner
+            learner.fit(self.eps)
+            learner.load(mute=True)
+            df1 = learner.logger.df_best
+            df1['Best'] = ''
+            self.df = df1.copy() if self.df is None else pd.concat((self.df,df1),ignore_index=True)
+            if learner.logger.best > self.best:
+                self.best, self.best_file = learner.logger.best, f'{self.name}_{i}'
+                print(f'New best: {self.best:.4f}')
+                display(self.df.iloc[[-1]])
+            self.df['Best'] = ''
+            self.df.loc[self.df.iloc[:,key_metric(learner)]==self.best, 'Best'] = '*'
+            self.save()
+            learner.close()
+            del learner
+            gc.collect()
+        self.save()
+        print(f'\nBest file: {self.best_file}')
+        display(self.df)
+        enablePrint()
+
+    def save(self):
+        meta = {'desc': self.desc, 'best': self.best, 'best_file': self.best_file}
+        pickle.dump(meta, open(self.fname+'.pickle', 'wb'))
+        self.df.to_csv(self.fname+'.csv', index=False)
+
+    def load(self):
+        p_pickle, p_csv = Path(f'{self.fname}.pickle'), Path(f'{self.fname}.csv')
+        if not p_pickle.exists() or not p_csv.exists(): return
+        meta = pickle.load(open(self.fname+'.pickle', 'rb'))
+        if not 'cols' in meta or not 'best' in meta or not 'best_file' in meta: return
+        print(f'Loaded from file {self.fname}: {meta}')
+        self.desc, self.best, self.best_file = meta['desc'], meta['best'], meta['best_file']
+        self.df = pd.read_csv(self.fname+'.csv')
+        self.df['Best'] = self.df['Best'].fillna('')
+
+    def df_best(self):
+        if self.learner is None: return None
+        return self.df[self.df.iloc[:,key_metric(self.learner)]==self.best].iloc[[0]]
```

### Comparing `dl2050nn-1.0.73/dl2050nn/metrics.py` & `dl2050nn-1.0.8/dl2050nn/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 import math
 import numpy as np
 import pandas as pd
 import torch
+import sklearn.metrics as sk_metrics
 from sklearn.metrics import roc_auc_score
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import seaborn as sns
 
+
 """
-    Sensitivity (Recall):
-        Proportion of actual positive cases that got predicted as positive
-        The more sensitive a test is, the fewer false negative results
-        TP / (TP+FN) = TP / P
-
-    Specificity (Recall):
-        Proportion of actual negatives, which got predicted as the negative
-        The more specific a test is, the fewer false positive results
-        TN / (TN+FP) = TN / N
-
-    Precision (PPV):
-        A measure of exactness: out of those predicted positive, how many are actual positive
-        Good measure when the costs of False Positive is high (ex: email spam)
-        TP / (TP+FP) = TP / P2
+    Precision:
+        A measure of exactness.
+        Out of those predicted positive, how many are actual positive.
+        Good measure when the costs of False Positive is high (ex: email spam).
 
     Recall:
         A measure of a classifiers completeness.
         How many of the Actual Positives the model captured.
         Good measure when the costs of False Negatives is high (ex: fraud detection or sick patient detection).
 
     F1 Score (or F-score)
@@ -41,45 +33,40 @@
 
     Suppose a computer program for recognizing dogs in photographs identifies 8 dogs in a picture containing 12 dogs and
     some cats. Of the 8 dogs identified, 5 actually are dogs (true positives), while the rest are cats (false positives).
     The program's recal is 5/12 and the precision is 5/8.
 
 """
 
+
 def accuracy(y2, y):
     y2 = torch.max(y2, dim=1)[1]
     return (y2==y).float().mean().item()
 
 def recall(y2, y): # TPR = TP/P (same as sensitivity)
     y2 = torch.max(y2, dim=1)[1]
     tp = torch.mul((y2==y), y.byte()).sum().item()
     p = (y==1).sum().item()
-    # r = float(tp) / float(p) if p>0 else 0.0
-    return tp/p if p>0 else 0.0
-
-def precision(y2, y): # TP/(TP+FP)
-    y2 = torch.max(y2, dim=1)[1]
-    tp = torch.mul((y2==y), y.byte()).sum().item()
-    p2 = (y2==1).sum().item()
-    return tp/p2 if p2>0 else 0.0
+    r = float(tp) / float(p) if p>0 else 0.0
+    return r
 
-def sensitivity(y2, y): # (same as recall)
+def sensitivity(y2, y): # TPR = TP/P (same as recall)
     return recall(y2, y)
 
 def specificity(y2, y): # TNR = TN/N
     y2 = torch.max(y2, dim=1)[1]
     tn = torch.mul((y2==y), y.byte()^1).sum().item()
     n = (y==0).sum().item()
     return tn/n if n>0 else 0.0
 
-def balanced_accuracy(y2, y):
-    return (sensitivity(y2,y)+specificity(y2,y))/2
-
-def balanced_accuracy_mult(y2, y):
-    return (sensitivity(y2,y)*specificity(y2,y))/2
+def precision(y2, y): # TP/(TP+FP)
+    y2 = torch.max(y2, dim=1)[1]
+    tp = torch.mul((y2==y), y.byte()).sum().item()
+    p = (y2==1).sum().item()
+    return tp/p if p>0 else 0.0
 
 def accuracy2(y2, y, threshold=0.5):
     y2 = (y2 > threshold).byte()
     y = y.byte()
     return (y2==y).float().mean().item()
 
 def precision2(y2, y, threshold=0.5):
```

### Comparing `dl2050nn-1.0.73/dl2050nn/models.py` & `dl2050nn-1.0.8/dl2050nn/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,231 +1,119 @@
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from dl2050nn.etc import get_cnn_szs
+from nn2.etc import get_model_n_params, get_cnn_szs
 
-def model_stats(model, bottle=None, szs=None, show_szs=False):
-    p = sum([p.numel() for p in model.parameters()])
-    s = f'{str(model.__class__.__name__)}: params {p/1e6:,.1f}m'
-    if bottle: s+=f', bottles {bottle}' 
-    if szs: s+=f', input_sz: {szs[0]}, last_conv_sz {szs[-1]}'
-    if szs and show_szs: s+=f'\n\tszs: {szs}'
-    print(s)
 
 def init_layer(l):
     if getattr(l, 'bias', None) is not None: nn.init.constant_(l.bias, 0) # l.bias.data.zero_()
     if isinstance(l, (nn.BatchNorm1d, nn.BatchNorm2d)): l.weight.data.fill_(1)
     if isinstance(l, (nn.Linear,)): nn.init.kaiming_normal_(l.weight)
     if isinstance(l, (nn.Embedding,)): l.weight.data.normal_(0., 2./math.sqrt(l.weight.data.size(1)))
         #sc = 2/(w.size(1)+1)
         #w.uniform_(-sc, sc)
     if isinstance(l, (nn.Conv1d, nn.Conv2d)): nn.init.kaiming_normal_(l.weight)
 
+
 def init_net(m):
     init_layer(m)
     for l in m.children(): init_net(l)
 
+
 def noop(x): return x
     
+
 # def ReLU_Sim(x): return x.clamp_min(0.) - 0.5
 class ReLU_Sim(nn.Module):
     def forward(self, x): return x.clamp_min(0.) - 0.5
 
+
 class Mish(nn.Module):
     def __init__(self): super().__init__()
     def forward(self, x): return x *( torch.tanh(F.softplus(x)))
 
+
 default_act =  Mish() # nn.ReLU(inplace=True), Mish()
 
+
 class Sigmoid(nn.Module):
     def __init__(self, yrange=None):
         super().__init__()
         self.yrange = yrange
     def forward(self, x):
         return torch.sigmoid(x) if self.yrange is None else self.y_range[0]+(self.yrange[1]-self.yrange[0])*torch.sigmoid(x)
 
 # def sigmoid(input, eps=1e-7):
 #     "Same as `torch.sigmoid`, plus clamping to `(eps,1-eps)"
 #     return input.sigmoid().clamp(eps,1-eps)
 
+
 class Flatten(nn.Module):
     def forward(self, x): return x.view(x.size(0), -1)
 
-def Linear(n1, n2, p=None, bn=True, act=default_act):
+
+def Linear(n1, n2, p=0.0, bn=True, act=default_act):
     net = []
     if bn:
         batch = nn.BatchNorm1d(num_features=n1)
         init_layer(batch)
         net += [batch]
     if p is not None: net += [nn.Dropout(p=p)]
     linear = nn.Linear(in_features=n1, out_features=n2)
     init_layer(linear)
     net += [linear]
-    if act: net+=[act]
+    if act: net += [act]
     return nn.Sequential(*net)
 
-def LinearFinal(n1, n2, p=None, act=nn.LogSoftmax(dim=1)):
-    return Linear(n1, n2, p=p, bn=False, act=act)
+def LinearFinal(n1, n2, p=None, act=nn.LogSoftmax(dim=1)): return Linear(n1, n2, p=p, bn=False, act=act)
+
 
 def Conv2D(n1, n2, ks=3, stride=1, zero_bn=False, act=True):
     bn = nn.BatchNorm2d(n1)
     nn.init.constant_(bn.weight, 0. if zero_bn else 1.)
     conv = nn.Conv2d(n1, n2, kernel_size=ks, stride=stride, padding=ks//2, bias=False)
     layers = [bn, conv]
     if act: layers.append(default_act)
     return nn.Sequential(*layers)
     # PREVIOUS: return F.relu(self.batch(self.conv(x)))
 
+
 def Conv1D(n1, n2, ks=3, stride=1, zero_bn=False, act=True):
     bn = nn.BatchNorm1d(n1)
     nn.init.constant_(bn.weight, 0. if zero_bn else 1.)
     conv = nn.Conv1d(n1, n2, kernel_size=ks, stride=stride, padding=ks//2, bias=False)
     layers = [bn, conv]
     if act: layers.append(default_act)
     return nn.Sequential(*layers)
 
+
 class ResBlock2D(nn.Module):
     def __init__(self, ni, nf, stride=1):
         super().__init__()
         layers  = [Conv2D(ni, nf, stride=stride),
                    Conv2D(nf, nf, zero_bn=True, act=False)]
         self.convs = nn.Sequential(*layers)
         self.idconv = noop if ni==nf else Conv2D(ni, nf, ks=1, act=False)
         self.pool = noop if stride==1 else nn.AvgPool2d(2, ceil_mode=True)
+    
     def forward(self, x): return default_act(self.convs(x) + self.idconv(self.pool(x)))
 
+
 class ResBlock1D(nn.Module):
-    def __init__(self, n1, n2, ks=3, stride=1):
+    def __init__(self, ni, nf, ks=3, stride=1):
         super().__init__()
-        layers  = [Conv1D(n1, n2, ks=ks, stride=stride),
-                   Conv1D(n2, n2, ks=ks, zero_bn=True, act=False)]
+        layers  = [Conv1D(ni, nf, ks=ks, stride=stride),
+                   Conv1D(nf, nf, ks=ks, zero_bn=True, act=False)]
         self.convs = nn.Sequential(*layers)
-        self.idconv = noop if n1==n2 else Conv1D(n1, n2, ks=1, act=False)
+        self.idconv = noop if ni==nf else Conv1D(ni, nf, ks=1, act=False)
         self.pool = noop if stride==1 else nn.AvgPool1d(2, ceil_mode=True)
-    def forward(self, x): return default_act(self.convs(x) + self.idconv(self.pool(x)))
-
-class Resnet(nn.Module):
-    def __init__(self, data, layers=[64, 64, 64], p=None):
-        super(Resnet, self).__init__()
-        sz = [int(e) for e in data.ds1[0][0].shape]
-        n1, n2 = sz[0], 32
-        net = [ResBlock2D(n1, n2, stride=2)]
-        n1 = n2
-        for n2 in layers:
-            net += [ResBlock2D(n1, n2, stride=2)]
-            n1 = n2
-        net += [nn.AdaptiveMaxPool2d(1)]
-        net += [Flatten()]
-        net += [Linear(layers[-1], 1024, p=p)]
-        net += [LinearFinal(1024, data.c, p=None)]
-        self.net = nn.Sequential(*net)
-        p = sum([p.numel() for p in self.parameters()])
-        self.szs = get_cnn_szs(self, sz)
-        print(f'\nResnet: params: {p:,.0f}, img_sz: {sz}, last_conv {self.szs[-1]}: ')
-
-    def forward(self, x):
-        return self.net(x)
-
-# ####################################################################################################
-# UNet 1D
-# ####################################################################################################
-
-class Encoder(nn.Module):
-    def __init__(self, chs):
-        super().__init__()
-        self.enc_blocks = nn.ModuleList([ResBlock1D(chs[i], chs[i+1], ks=7) for i in range(len(chs)-1)])
-        self.pool = nn.MaxPool1d(2)
-    
-    def forward(self, x):
-        encs = []
-        for block in self.enc_blocks:
-            x = block(x)
-            encs.append(x)
-            x = self.pool(x)
-        return encs
-
-class Decoder(nn.Module):
-    def __init__(self, chs):
-        super().__init__()
-        chs = chs[1::][::-1]
-        self.chs = chs
-        self.upconvs = nn.ModuleList([nn.ConvTranspose1d(chs[i], chs[i+1], 2, stride=2, padding=0) for i in range(len(chs)-1)])
-        self.dec_blocks = nn.ModuleList([Conv1D(chs[i], chs[i+1], ks=5) for i in range(len(chs)-1)]) 
-        
-    def forward(self, x, encs):
-        for i in range(len(self.chs)-1):
-            x = self.upconvs[i](x)
-            x2 = self.crop(encs[i], x)
-            x = torch.cat([x, x2], dim=1)
-            x = self.dec_blocks[i](x)
-        return x
-    
-    def crop(self, encs, x):
-        k = x.shape[2]
-        return encs[:,:,:k]
-
-class UNet1D(nn.Module):
-    def __init__(self, chs, c, retain_dim=True, show=False):
-        super().__init__()
-        self.encoder = Encoder(chs)
-        self.decoder = Decoder(chs)
-        self.head = nn.Sequential(*[Conv1D(chs[1], c, ks=1), Conv1D(c, c, ks=1, zero_bn=True, act=False)])
-        self.retain_dim  = retain_dim
-        self.softmax = nn.LogSoftmax(dim=1)
-        if show: model_stats(self)
 
-    def forward(self, x):
-        out_sz = x.shape[2]
-        encs = self.encoder(x)
-        x = self.decoder(encs[::-1][0], encs[::-1][1:])
-        x = self.head(x)
-        if self.retain_dim: x = torch.nn.functional.interpolate(x,out_sz)
-        x = self.softmax(x)
-        return x
-
-################################################################################################################################
-#  SignalNet
-################################################################################################################################
-
-class SignalNet(nn.Module):
-    def __init__(self, ch, n, c, p=0., show=False):
-        super().__init__()
-        n1,sz = ch,n
-        n2 = min((n1+1)*8,64)
-        net = []
-        szs = [(n1,sz)]
-        for _ in range(3):
-            net += [Conv1D(n1, n2, stride=2)]
-            n1, sz = n2, int(sz/2)
-            szs += [(n1,sz)]
-        bottle = int((int(math.log2(sz)))/2)
-        for _ in range(bottle):
-            net += [ResBlock1D(n1, n1*2, ks=3, stride=2)]
-            n1, sz = n1*2, int(sz/2)
-            szs += [(n1,sz)]
-            net += [nn.MaxPool1d(2)]  # AvgPool1d, MaxPool1d
-            sz = int(sz/2)
-            szs += [(n1,sz)]
-        net += [nn.AdaptiveMaxPool1d(1)]
-        net += [Flatten()]
-        self.emb = nn.Sequential(*net)
-        net += [Linear(n1, 1024, p=p)]
-        self.emb_fc = nn.Sequential(*net)
-        net += [LinearFinal(1024, c, p=None)]
-        self.net = nn.Sequential(*net)
-        if show: model_stats(self, bottle=bottle, szs=szs, show_szs=True)
-
-    def forward(self, x): return self.net(x)
-    def get_emb(self, x): return self.emb(x).detach().cpu().numpy()
-    def get_emb_fc(self, x): return self.emb_fc(x).detach().cpu().numpy()
+    def forward(self, x): return default_act(self.convs(x) + self.idconv(self.pool(x)))
 
-################################################################################################################################
-#  TabularNet
-################################################################################################################################
 
 class TabularNet(nn.Module):
     def __init__(self, data, szs, emb_p, ps):
         super().__init__()
         self.ncats, self.nconts = data.ncats, data.nconts
         self.embs = nn.ModuleList([nn.Embedding(c, s) for c,s in data.emb_szs])
         self.nemb = sum(e.embedding_dim for e in self.embs)
@@ -250,21 +138,75 @@
             x = self.emb_drop(x)
         if self.nconts!=0:
             # x_cont = self.bn_cont(x_cont)
             x = torch.cat([x, x_cont], 1) if self.nemb!=0 else x_cont
         x = self.fcs(x)
         return x
 
-################################################################################################################################
-#  Etc
-################################################################################################################################
-
-# x = torch.randn(1, 1, 250)
-# l = ResBlock1D(1, 64)
-# l(x).shape
+
+class SignalNet(nn.Module):
+    def __init__(self, data, p=0.):
+        super(SignalNet, self).__init__()
+        x,_ = data.ds1[0]
+        n1, sz = x.shape[0], x.shape[1]
+        n2 = min((n1+1)*8,64)
+        net = []
+        szs = [(n1,sz)]
+        for i in range(3):
+            net += [Conv1D(n1, n2, stride=2)]
+            n1, sz = n2, int(sz/2)
+            szs += [(n1,sz)]
+        bottle = int((int(math.log2(sz)))/2)
+        for i in range(bottle):
+            net += [ResBlock1D(n1, n1*2, ks=3, stride=2)]
+            n1, sz = n1*2, int(sz/2)
+            szs += [(n1,sz)]
+            net += [nn.MaxPool1d(2)]  # AvgPool1d, MaxPool1d
+            sz = int(sz/2)
+            szs += [(n1,sz)]
+        net += [nn.AdaptiveMaxPool1d(1)]
+        net += [Flatten()]
+        net += [Linear(1*n1, 1024, p=p)]
+        net += [LinearFinal(1024, data.c, p=None)]
+        self.net = nn.Sequential(*net)
+        p = sum([p.numel() for p in self.parameters()])
+        print(f'SignalNet: params: {p:,.0f}, signal_sz: {szs[0]}, bottles: {bottle}, last_conv {szs[-1]}')
+        # print(szs)
+
+    def forward(self, x): return self.net(x)
+
+
+class Resnet(nn.Module):
+    def __init__(self, data, layers=[64, 64, 64], p=None):
+        super(Resnet, self).__init__()
+        sz = [int(e) for e in data.ds1[0][0].shape]
+        n1, n2 = sz[0], 32
+        net = [ResBlock2D(n1, n2, stride=2)]
+        n1 = n2
+        for n2 in layers:
+            net += [ResBlock2D(n1, n2, stride=2)]
+            n1 = n2
+        net += [nn.AdaptiveMaxPool2d(1)]
+        net += [Flatten()]
+        net += [Linear(layers[-1], 1024, p=p)]
+        net += [LinearFinal(1024, data.c, p=None)]
+        self.net = nn.Sequential(*net)
+        p = sum([p.numel() for p in self.parameters()])
+        self.szs = get_cnn_szs(self, sz)
+        print(f'\nResnet: params: {p:,.0f}, img_sz: {sz}, last_conv {self.szs[-1]}: ')
+
+    def forward(self, x): return self.net(x)
+
+
+
+
+
+
+
+
 
 # class ResBlock(nn.Module):
 #     def __init__(self, expansion, ni, nh, stride=1):
 #         super().__init__()
 #         nf,ni = nh*expansion,ni*expansion
 #         layers  = [conv_layer(ni, nh, 3, stride=stride),
 #                    conv_layer(nh, nf, 3, zero_bn=True, act=False)
```

### Comparing `dl2050nn-1.0.73/dl2050nn/optimizers.py` & `dl2050nn-1.0.8/dl2050nn/optimizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from functools import partial
 import torch
 from torch import tensor
-from dl2050utils.core import listify
+from dlogicutils.core import listify
 import matplotlib.pyplot as plt
-from dl2050nn.etc import *
-from dl2050nn.cbs import *
+from nn2.etc import *
+from nn2.cbs import *
 
 
 def merge(os, dest, f):
     for o in os:
         for k,v in f(o).items():
             if k not in dest: dest[k] = v
 
@@ -60,29 +60,28 @@
     f1 = combine_scheds([0.3, 0.7], [sched_cos(start, end, cycle), sched_cos(end, start, cycle)], cycle)
     if sched2 is None: return f1
     return combine_scheds_mult(f1, sched2(1., factor, None))
 
 
 class ParamScheduler(Callback):
     def __init__(self, pname, sched_funcs):
-        self.pname,self.sched_funcs = pname,listify(sched_funcs)
+        self.pname, self.sched_funcs = pname, listify(sched_funcs)
 
     def plot(self, eps=4, label=None):
         fig = plt.figure(figsize=(5, 3))
         epf = torch.linspace(0.0,eps,100*eps)
         plt.plot(epf, [self.sched_funcs[0](e, eps) for e in epf], label=label)
         plt.show()
         plt.pause(.001)
 
     def begin_batch(self): 
         if not self.train: return
         # Pytorch optimizer
         if not hasattr(self.optf, 'hypers'):
-            for pg in self.optf.param_groups:
-                pg['lr'] = self.sched_funcs[0](self.epf, self.eps)
+            for pg in self.optf.param_groups: pg['lr'] = self.sched_funcs[0](self.epf, self.eps)
             return
         # NN2 optimizer
         fs = self.sched_funcs
         if len(fs)==1: fs = fs*len(self.optf.param_groups)
         for f,h in zip(fs,self.optf.hypers): h[self.pname] = f(self.epf, self.eps)
 
 
@@ -116,26 +115,23 @@
 
 # Stats
 
 def average_grad(state, p, mom, dampening=False, **kwargs):
     "Keeps track of the avg grads of `p` in `state` with `mom`."
     if 'grad_avg' not in state: state['grad_avg'] = torch.zeros_like(p.grad.data)
     damp = 1-mom if dampening else 1.
-    # state['grad_avg'].mul_(mom).add_(damp, p.grad.data) -> OLD DEPRECRATED
-    state['grad_avg'].mul_(mom).add_(p.grad.data, alpha=damp) # NEW TO BE TESTED
+    state['grad_avg'].mul_(mom).add_(damp, p.grad.data)
     return state
 average_grad.defaults = dict(mom=0.9)
 
 
 def average_sqr_grad(state, p, sqr_mom, dampening=True, **kwargs):
     if 'sqr_avg' not in state: state['sqr_avg'] = torch.zeros_like(p.grad.data)
     damp = 1-sqr_mom if dampening else 1.
-    # state['sqr_avg'].mul_(sqr_mom).addcmul_(damp, p.grad.data, p.grad.data) # -> OLD DEPRECRATED
-    # state['sqr_avg'].mul_(sqr_mom).addcmul_(p.grad.data, p.grad.data, damp) # NEW TO BE TESTED
-    state['sqr_avg'].mul_(sqr_mom).addcmul_(p.grad.data, p.grad.data, value=damp)
+    state['sqr_avg'].mul_(sqr_mom).addcmul_(damp, p.grad.data, p.grad.data)
     return state
 average_sqr_grad.defaults = dict(sqr_mom=0.99)
 
 
 def step_stat(state, p, **kwargs):
     if 'step' not in state: state['step'] = 0
     state['step'] += 1
@@ -147,53 +143,51 @@
 def weight_decay(p, lr, wd, do_wd=True, **kwargs):
     if do_wd and wd!=0: p.data.mul_(1 - lr*wd)
     return p
 #weight_decay.defaults = dict(wd=0.)
 
 
 def l2_reg(p, lr, wd, do_wd=True, **kwargs):
-    if do_wd and wd!=0:
-        p.grad.data.add_(p.data, alpha=wd)
+    if do_wd and wd!=0: p.grad.data.add_(wd, p.data)
     return p
 #l2_reg.defaults = dict(wd=0.)
 
 
 def sgd_step(p, lr, **kwargs):
-    p.data.add_(p.grad.data, alpha=-lr)
+    p.data.add_(-lr, p.grad.data)
     return p
 #sgd_step._defaults = dict(lr=0.01)
 
 
 def momentum_step(p, lr, grad_avg, **kwargs):
-    p.data.add_(grad_avg, alpha=-lr)
+    p.data.add_(-lr, grad_avg)
     return p
 
 
 def debias(mom, damp, step): return damp * (1 - mom**step) / (1-mom)
 
 
 def adam_step(p, lr, mom, step, sqr_mom, grad_avg, sqr_avg, epsilon, **kwargs):
     "Step for Adam with `lr` on `p`"
     debias1 = debias(mom, 1-mom, step)
     debias2 = debias(sqr_mom, 1-sqr_mom, step)
-    # p.data.addcdiv_(-lr / debias1, grad_avg, (sqr_avg/debias2).sqrt() + epsilon)
-    p.data.addcdiv_(grad_avg, (sqr_avg/debias2).sqrt()+epsilon, value=-lr/debias1)
+    p.data.addcdiv_(-lr / debias1, grad_avg, (sqr_avg/debias2).sqrt() + epsilon)
     return p
 #adam_step._defaults = dict(epsilon=1e-5, lr=0.01,)
 
 
 def lamb_step(p, lr, mom, step, sqr_mom, grad_avg, sqr_avg, epsilon, **kwargs):
     "Step for LAMB with `lr` on `p`"
     debias1 = debias(mom, 1-mom, step)
     debias2 = debias(sqr_mom, 1-sqr_mom, step)
     r1 = p.data.pow(2).mean().sqrt()
     step = (grad_avg/debias1) / ((sqr_avg/debias2).sqrt()+epsilon)
     r2 = step.pow(2).mean().sqrt()
     q = 1 if r1 == 0 or r2 == 0 else min(r1/r2,10)
-    p.data.add_(step, alpha=-lr*q)
+    p.data.add_(-lr * q, step)
     return p
 #lamb_step._defaults = dict(epsilon=1e-6, wd=0.)
 
 
 # Optimizers
 
 def SGD(params, lr=0.01, mom=0., wd=1e-5, decouple_wd=True):
```

### Comparing `dl2050nn-1.0.73/dl2050nn/results.py` & `dl2050nn-1.0.8/dl2050nn/results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
+from sklearn.metrics import confusion_matrix
 import matplotlib.pyplot as plt
 import matplotlib as mpl
+from nn2.data import TabularDataset
+from nn2.etc import *
 from IPython.display import display
 import sklearn
-from dl2050nn.etc import *
-from dl2050nn.data import TabularDataset
 # https://en.wikipedia.org/wiki/Sensitivity_and_specificity
 
 epsilon = 1e-9
 scols = ['p','n','tp','fp','tn','fn','tpr','fpr','tnr','fnr','accuracy','error_rate','precision','recall',
          'sensitivity','specificity']
 
 def df_stats_by_class(cm):
@@ -71,50 +72,45 @@
     specificity = tnr
     pcaptured = tp/ptotal
     z = zip(probs,preds,actuals,nn,nnp,p,n,tp,fp,tn,fn,tpr,fpr,tnr,fnr,accuracy,error_rate,precision,recall,sensitivity,specificity,pcaptured)
     cols = ['prob','pred','actual','size','size%']+scols+['pcaptured']
     df = pd.DataFrame(z, columns=cols)
     if thresholds:
         ths = [t/thresholds if t>0 else -.00001 for t in range(0,thresholds)[::-1]]
-        ths2, idxs = [], []
-        for t in ths:
-            idxs1 = np.where(probs>t)[0]
-            if len(idxs1):
-                ths2.append(t)
-                idxs.append(max(idxs1))
+        idxs = [max(np.where(probs>t)[0]) for t in ths]
         df = df.iloc[idxs].copy()
-        df.insert(0, 'threshold', ths2)
+        df.insert(0, 'threshold', ths)
         df.drop(columns=['prob','pred','actual'], inplace=True)
     return df
 
 def plot_cmap(data):
     fig, ax = plt.subplots(figsize=(8, 8))
     cmap=sns.diverging_palette(0, 160, as_cmap=True)
     cmap=mpl.cm.Blues
     cmap = sns.diverging_palette(0, 180, sep=40, s=100, as_cmap=True)
     sns.heatmap(data, vmin=-1, vmax=1, cmap=cmap, square=True, ax=ax)
     plt.show()
     plt.pause(.001)
 
-def calc_cm(c, actuals, preds):
+def plot_confusion(c, actuals, preds):
     cm = np.zeros((c, c), dtype=int)
     cm_p = np.zeros((c, c), dtype=np.float)
     for i in range(preds.shape[0]): cm[int(actuals[i])][int(preds[i])] += 1
     for i in range(cm.shape[0]): cm_p[i,:] = cm[i,:] / cm[i,:].sum()
     cm_p = 100.0*cm_p
-    return cm,cm_p
-
-def plot_confusion(cm, cm_p):
     fig = plt.figure(figsize=(20, 5))
     ax1, ax2 = fig.add_subplot(121), fig.add_subplot(122)
     sns.set(font_scale=1.0)
     sns.heatmap(cm, cmap=mpl.cm.Blues, annot=True, fmt='d', ax=ax1)
     sns.heatmap(cm_p, cmap=mpl.cm.Blues, annot=True, fmt='.2f', ax=ax2)
+    ax1.set_title(f'Total: {preds.shape[0]}')
+    ax2.set_title(f'Total: 100.00%')
     plt.show()
     plt.pause(.001)
+    return cm
 
 def calc_prc(y, y2):
     mask = np.argsort(-y2)
     y, y2 = y[mask], y2[mask]
     recall = np.array([0]+[((y2>=t)[y==1]==y[y==1]).sum()/(y==1).sum() for t in y2]+[1])
     precision = np.array([1]+[(y[y2>=t]==1).sum()/(y2>=t).sum() for t in y2]+[0])
     auc_pr = np.trapz(precision, recall)
@@ -124,32 +120,29 @@
     mask = np.argsort(-y2)
     y, y2 = y[mask], y2[mask]
     fpr = np.array([0]+[((y2>=t)[y==0]!=y[y==0]).sum()/(y==0).sum() for t in y2])
     tpr = np.array([0]+[((y2>=t)[y==1]==y[y==1]).sum()/(y==1).sum() for t in y2])
     auc = np.trapz(tpr, fpr)
     return auc, fpr, tpr
 
-# def np_resample_with_mean(x,k): return np.mean(x[:k*(len(x)//k)].reshape(-1, k), 1)
-
 def plot_roc(y, y2):
     fpr,tpr,_ = sklearn.metrics.roc_curve(y, y2)
     auc = auc = np.trapz(tpr, fpr)
     precision,recall,_ = sklearn.metrics.precision_recall_curve(y, y2)
     auc_pr = np.trapz(precision, recall)
     # auc, fpr, tpr = calc_roc(y, y2)
     # auc_pr, precision, recall = calc_prc(y, y2)
     _, axs = plt.subplots(1,2, figsize=(14,5))
     axs[0].plot(fpr, tpr, label=f'AUC = {auc:.3f})')
     axs[0].plot([0., 1.], [0., 1.], 'k--')
     axs[0].set_title('ROC')
     axs[0].set_xlabel('FPR')
     axs[0].set_ylabel('TPR = Recall')
     axs[0].legend(loc='best')
-    cut = len(recall) - int(len(recall)/100)
-    axs[1].plot(recall[:cut], precision[:cut], label=f'AUC_PR = {auc_pr:.3f})')
+    axs[1].plot(recall, precision,  label=f'AUC_PR = {auc_pr:.3f})')
     axs[1].plot([0., 1.], [1., 0.], 'k--')
     axs[1].set_title('ROC - Precision/Recall')
     axs[1].set_xlabel('Recall')
     axs[1].set_ylabel('Precision')
     axs[1].legend(loc='best')
     plt.show()
     plt.pause(.001)
@@ -184,74 +177,83 @@
     prob = get_probs(y2) if data.c>2 else get_probs_bin(y2)
     pred = get_preds(prob)
     df['prob'] = prob
     df['pred'] = pred
     df['pred_label'] = [data.cls[e] for e in pred]
     return df
 
+
+# ???
+def get_probs_for_actuals(y2, actuals):
+    probs = np.exp(y2)
+    mask = np.zeros((probs.shape[0], probs.shape[1]))
+    mask[np.arange(actuals.shape[0]),actuals] = 1
+    return probs[mask.astype(bool)]
+
+
+# ???
+def df_predict_clsf(learner, df, have_actuals=False):
+    df = df.copy()
+    if 'prob' in df.columns: df=df.drop(columns='prob')
+    data = learner.data
+    y2 = learner.predict(df)
+    y2 = y2.numpy()
+    prob = get_probs(y2) if data.c>2 else get_probs_bin(y2)
+    pred = get_preds(y2)
+    pred_label = [data.cls[e] for e in pred]
+    df['prob'] = prob
+    df['pred'] = pred
+    df['pred_label'] = pred_label
+    if have_actuals:
+        actuals = df[data.proc.c_dep] 
+        df['actual'] = actuals.values
+        df['actual_label'] = [data.cls[e] for e in actuals.values]
+        df['error'] = (df['pred']!=df['actual'])*1
+    df = df.sort_values(by=['prob'], ascending=[False])
+    return df
+
+
+
 class Results_Clsf():
-    def __init__(self, learner=None, y2=None, y=None):
-        assert learner is not None or (y2 is not None and y is not None), 'required either learner or y2 and y'
-        if learner is not None:
-            y2,y = learner.logger.y2_ep.cpu().numpy(),learner.logger.y_ep.cpu().numpy()
-        self.actuals = y
-        self.c = len(np.unique(y))
-        self.probs = get_probs_bin(y2) if self.c==2 else get_probs(y2)
-        self.preds = get_preds(self.probs)
-    def all(self, thresholds=10):
+    def __init__(self, data, probs, actuals):
+        self.data, self.probs, self.actuals = data, probs, actuals
+        self.preds = get_preds(probs)
+#         self.probs_for_actuals = get_probs_for_actuals(y2, self.actuals)
+#         self.probs_sorted = np.argsort(self.probs_for_actuals)[::-1]
+    def show_all(self, thresholds=10):
         self.confusion()
         self.roc()
-        self.stats()
+        display(self.df_stats(thresholds=thresholds))
     def confusion(self, t=None):
-        if self.c!=2: raise ValueError('More than two classes')
-        cm,cm_p = calc_cm(self.c, self.actuals, self.preds)
-        plot_confusion(cm, cm_p)
-        display(pd.DataFrame([{'Total':cm.sum()}]))
-        display(pd.DataFrame(cm.sum(axis=0)).transpose())
-        display(pd.DataFrame(cm.sum(axis=1)))
-        display(df_stats_by_class(cm))
-    def stats(self, thresholds=10):
-        if self.c!=2: raise ValueError('More than two classes')
+        show_dist(self.actuals)
         display(df_stats_binary(self.preds, self.actuals))
-        display(df_stats_cum(self.probs, self.actuals, thresholds=thresholds))
+        if t is None:
+            preds = self.preds
+        else:
+            if self.data.c!=2: raise ValueError('More than two classes')
+            preds = (self.probs>t)*1
+        cm = plot_confusion(self.data.c, self.actuals, preds)
+        display(df_stats_by_class(cm))
+    def df_stats(self, thresholds=10):
+        if self.data.c!=2: raise ValueError('More than two classes')
+        return df_stats_cum(self.probs, self.actuals, thresholds=thresholds)
     def roc(self):
-        if self.c!=2: raise ValueError('More than two classes')
+        if self.data.c!=2: raise ValueError('More than two classes')
         plot_roc(self.actuals, self.probs)
-    def get_correct(self, actual=None, n=8):
-        idx = np.where(self.actuals==self.preds)[0]
-        if actual is not None:
-            idx = [i for i in idx if self.actuals[i]==actual]
-        if n: idx = idx[:n]
-        return idx
-    def get_wrong(self, actual=None, n=8):
-        idx = np.where(self.actuals!=self.preds)[0]
-        if actual is not None:
-            idx = [i for i in idx if self.actuals[i]==actual]
-        if n: idx = idx[:n]
-        return idx
-    def get_most_confident(self, actual=None, pred=None, n=8):
-        idx = np.argsort(np.absolute(self.probs-.5))[::-1]
-        if actual is not None:
-            idx = [e for e in idx if self.actuals[e]==actual]
-        if pred is not None:
-            idx = [e for e in idx if self.preds[e]==pred]
-        if n: idx = idx[:n]
-        return idx
-    def get_least_confident(self, actual=None, pred=None, n=8):
-        idx = np.argsort(np.absolute(self.probs-.5))
-        if actual is not None:
-            idx = [e for e in idx if self.actuals[e]==actual]
-        if pred is not None:
-            idx = [e for e in idx if self.preds[e]==pred]
-        if n: idx = idx[:n]
-        return idx
+#     def show_best(self, n=8, **kwargs):  self.show_set(self.data.ds2, self.probs_sorted[:n], **kwargs)
+#     def show_worst(self, n=8, **kwargs): self.show_set(self.data.ds2, self.probs_sorted[-n:][::-1], **kwargs)
+#     def show_set(self, ds, idxs, **kwargs):
+#         labels = [f'{ds.labels[i]}:{self.actuals[i]} -> {ds.cls[self.preds[i]]}:{self.preds[i]} (p={self.probs_for_actuals[i]:.4f})'
+#                     for i in idxs]
+#         ds.show(list(idxs), labels=labels, **kwargs)
+
 
 class Results_Clsf_Tabular(Results_Clsf):
     def __init__(self, data, df):
         assert 'prob' in df.columns
         assert data.proc.c_dep in df.columns
         self.proc, self.df = data.proc, df
-        super(Results_Clsf_Tabular, self).__init__(df['prob'].values, df[data.proc.c_dep].values)
+        super(Results_Clsf_Tabular, self).__init__(data, df['prob'].values, df[data.proc.c_dep].values)
         # self.df['prob'] = self.probs if self.data.c>2 else self.probs_bin
     # def corr_cat(self): get_corr(self.df, self.proc.c_cat, plot=True)
     # def corr_cont(self): get_corr(self.df, self.proc.c_cont, plot=True)
     # def corr_prob(self): get_corr(self.df, self.proc.c_cat+self.proc.c_cont+[self.proc.c_dep, 'prob'], c='prob', plot=True)
```

### Comparing `dl2050nn-1.0.73/dl2050nn/tabular.py` & `dl2050nn-1.0.8/dl2050nn/tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pickle
-from dl2050utils.df import df_add_datepart
+from dlogicutils.df import df_add_datepart
 
 
 def scaller_norm(s, _mean, _std): return (s-_mean)/_std if _std>0 else s
 
 def scaller_minmax(s, _min, _max): return ((s-_min)/(_max-_min)-0.5)*2.0 if (_max-_min)>0 else s
 
 def scaller_rank(s):
```

