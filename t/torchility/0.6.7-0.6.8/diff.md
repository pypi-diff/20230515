# Comparing `tmp/torchility-0.6.7.tar.gz` & `tmp/torchility-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.6.7.tar", last modified: Sat May 13 05:21:56 2023, max compression
+gzip compressed data, was "torchility-0.6.8.tar", last modified: Mon May 15 08:02:25 2023, max compression
```

## Comparing `torchility-0.6.7.tar` & `torchility-0.6.8.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-13 05:21:56.981634 torchility-0.6.7/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.7/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-13 05:21:56.979591 torchility-0.6.7/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.7/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-13 05:21:56.952404 torchility-0.6.7/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1740 2023-05-13 04:54:21.000000 torchility-0.6.7/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.7/examples/2-mnist_callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-05 13:48:59.000000 torchility-0.6.7/examples/3-mnist_interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1709 2022-03-31 07:25:03.000000 torchility-0.6.7/examples/4-mnist_model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.7/examples/5-mnist_lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.7/examples/6-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-13 05:21:56.982057 torchility-0.6.7/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-05-05 12:13:44.000000 torchility-0.6.7/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-13 05:21:56.961636 torchility-0.6.7/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-13 05:20:50.000000 torchility-0.6.7/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-13 05:21:56.969753 torchility-0.6.7/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.7/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1153 2023-03-28 13:49:32.000000 torchility-0.6.7/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.6.7/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.7/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)    10012 2023-03-19 09:26:35.000000 torchility-0.6.7/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1022 2023-05-13 05:20:20.000000 torchility-0.6.7/torchility/datamodule.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.7/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.7/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4932 2023-03-28 13:36:07.000000 torchility-0.6.7/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5971 2023-03-28 13:41:27.000000 torchility-0.6.7/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    12337 2023-05-13 05:03:46.000000 torchility-0.6.7/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-13 05:21:56.976960 torchility-0.6.7/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       68 2022-06-01 16:09:54.000000 torchility-0.6.7/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.7/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6050 2023-05-05 01:14:22.000000 torchility-0.6.7/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.7/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-13 05:21:56.965266 torchility-0.6.7/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-13 05:21:56.000000 torchility-0.6.7/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      820 2023-05-13 05:21:56.000000 torchility-0.6.7/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-13 05:21:56.000000 torchility-0.6.7/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-05-13 05:21:56.000000 torchility-0.6.7/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-13 05:21:56.000000 torchility-0.6.7/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.452181 torchility-0.6.8/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.8/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-15 08:02:25.451704 torchility-0.6.8/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.8/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.435612 torchility-0.6.8/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1728 2023-05-13 05:23:14.000000 torchility-0.6.8/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.8/examples/2-mnist_callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.6.8/examples/3-mnist_interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.6.8/examples/4-mnist_model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.8/examples/5-mnist_lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.8/examples/6-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-15 08:02:25.452448 torchility-0.6.8/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-05-05 12:13:44.000000 torchility-0.6.8/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.439312 torchility-0.6.8/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-15 08:01:49.000000 torchility-0.6.8/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.446736 torchility-0.6.8/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.8/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1191 2023-05-15 06:05:49.000000 torchility-0.6.8/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.6.8/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.8/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     9501 2023-05-15 07:53:51.000000 torchility-0.6.8/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1092 2023-05-15 07:41:02.000000 torchility-0.6.8/torchility/datamodule.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.8/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.8/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5023 2023-05-15 07:26:34.000000 torchility-0.6.8/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6612 2023-05-15 07:34:33.000000 torchility-0.6.8/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    10601 2023-05-15 05:43:20.000000 torchility-0.6.8/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.450911 torchility-0.6.8/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       96 2023-05-15 04:51:01.000000 torchility-0.6.8/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2512 2023-05-15 07:06:33.000000 torchility-0.6.8/torchility/utils/metric_utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.8/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6050 2023-05-05 01:14:22.000000 torchility-0.6.8/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.8/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.441696 torchility-0.6.8/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      853 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.6.7/LICENSE` & `torchility-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/PKG-INFO` & `torchility-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.7
+Version: 0.6.8
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.6.7/README.md` & `torchility-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/examples/1-mnist.py` & `torchility-0.6.8/examples/1-mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 # 3. --- 优化器
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
 
 
 # 4. --- 训练
-trainer = Trainer(model, F.cross_entropy, opt, epochs=2, logger=False, reset_dl=1)            # 训练器
+trainer = Trainer(model, F.cross_entropy, opt, epochs=2, logger=False)            # 训练器
 trainer.fit(train_dl, val_dl)                                       # 训练、验证
 trainer.test(test_dl)                                               # 测试
 trainer.predict(test_dl, has_label=True)
 
 """ 使用GPU
 # 默认情况下自动选择可用的GPU，如下两种形式相同
 trainer = Trainer()
```

### Comparing `torchility-0.6.7/examples/2-mnist_callbacks.py` & `torchility-0.6.8/examples/2-mnist_callbacks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/examples/3-mnist_interpreter.py` & `torchility-0.6.8/examples/3-mnist_interpreter.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/examples/4-mnist_model_analysis.py` & `torchility-0.6.8/examples/4-mnist_model_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 warnings.simplefilter("ignore")
 
 
 # 1. --- 数据
 data_dir = './datasets'
 transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
-train_ds, val_ds, _ = random_split(mnist_full, [5000, 5000, 50000])
+train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
 train_dl = DataLoader(train_ds, batch_size=32)
 val_dl = DataLoader(val_ds, batch_size=32)
 test_dl = DataLoader(test_ds, batch_size=32)
 
 
 # 2. --- 模型
@@ -40,12 +40,12 @@
 
 
 # 4. --- 训练
 backward_analyzer = ModelAnalyzer('backward')                       # 对各层反向梯度进行分析
 forward_analyzer = ModelAnalyzer('forward')                         # 对各层前向输出进行分析
 trainer = Trainer(model, F.cross_entropy, opt, epochs=2,
                   callbacks=[backward_analyzer, forward_analyzer])  # 训练器
-trainer.fit(train_dl,)                                     # 训练、验证
+trainer.fit(train_dl)
 
 
 # 5. --- 显示分析结果图像
 # 在命令行中运行 tensorboard --logdir=./logs，通过浏览器查看
```

### Comparing `torchility-0.6.7/examples/5-mnist_lr_find.py` & `torchility-0.6.8/examples/5-mnist_lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/examples/6-graph_node_clasification_DGL.py` & `torchility-0.6.8/examples/6-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/setup.py` & `torchility-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/torchility/callbacks/interpreters.py` & `torchility-0.6.8/torchility/callbacks/interpreters.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/torchility/callbacks/performances.py` & `torchility-0.6.8/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/torchility/callbacks/progress.py` & `torchility-0.6.8/torchility/callbacks/progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from pytorch_lightning.callbacks import ProgressBar
 from pytorch_lightning.callbacks.callback import Callback
 from itertools import chain
-from typing import Any, Dict, Optional, Type
 import pytorch_lightning as pl
-from pytorch_lightning.utilities.types import STEP_OUTPUT
 
 
 class ProgressMix:
     """
     获取训练过程信息的混入类。
 
     实现类至少需要包含如下4个方法，以得到当前的batch序号：
@@ -19,143 +17,136 @@
             self.train_batch_id = batch_idx + 1
         def on_validation_batch_end(self, trainer, pl_module, outputs, batch, batch_idx, dataloader_idx):
             self.val_batch_id = batch_idx + 1
         def on_test_batch_end(self, trainer, pl_module, outputs, batch, batch_idx, dataloader_idx):
             self.test_batch_id = batch_idx + 1
     """
 
-    def get_info(self, trainer, stage, unit):
-        """get training, validation or testing output infomation from Trainer by stage and unit.
-
+    def get_info(self, trainer, stage):
+        """
+        返回当前epoch数，总epoch数，当前batch总，总batch数。
         Args:
             trainer (Trainer): Trainer.
             stage (str): 'train', 'val' or 'test'.
-            unit (str): 'step' or 'epoch'.
         Returns:
-            [int, int, int, int, dict]: current epoch, total epochs, current batch, total batchs, information dict
+            [int, int, int, int]: current epoch, total epochs, current batch, total batchs
         """
-        info = trainer.progress_bar_callback.get_metrics(trainer, trainer.task_module)
-        info_dict = {self._key(k): v for k, v in info.items() if self._check_info(k, stage, unit)}
         if stage == 'train':
             c_batch = self.train_batch_id
             num_batch = trainer.num_training_batches
         elif stage == 'val':
             c_batch = self.val_batch_id
             num_batch = self._total_val_batches(trainer)
         else:
             c_batch = self.test_batch_id
             num_batch = sum(trainer.num_test_batches)
         c_epoch = trainer.current_epoch + 1
         num_epoch = trainer.max_epochs
 
-        return c_epoch, num_epoch, c_batch, num_batch, info_dict
+        return c_epoch, num_epoch, c_batch, num_batch
 
     def _total_val_batches(self, trainer):
         total_val_batches = 0
         is_val_epoch = (trainer.current_epoch + 1) % trainer.check_val_every_n_epoch == 0
         total_val_batches = sum(trainer.num_val_batches) if is_val_epoch else 0
         return total_val_batches
 
-    def _key(self, k):
-        return k.replace('_step', '').replace('_epoch', '').replace('train_', '').replace('val_', '').replace('test_', '')
-
-    def _check_info(self, info_key, stage, unit):
-        key_split = info_key.split('_')
-        if key_split[0] != stage or key_split[-1] != unit:
-            return False
+    def get_epoch_loss(self, trainer, stage):
+        cbk_metrics = trainer.callback_metrics
+        if stage == 'train':
+            return {'loss': cbk_metrics['train_loss_epoch']}
         else:
-            return True
+            return {self._loss_key(k):v for k,v in cbk_metrics.items() if f'{stage}_loss_epoch' in k}
 
+    def _loss_key(self, k):
+        if '/dataloader_idx_' in k:
+            return f"loss/{k.split('_')[-1]}"
+        elif k=='test_loss_epoch':
+            return 'loss'
+        else:
+            return k
 
 class SimpleBar(ProgressBar, ProgressMix):
     """
     仅输出文本信息的进度条
     """
 
     def __init__(self):
         self.train_batch_id = 0
         self.val_batch_id = 0
         self.test_batch_id = 0
 
     def disable(self):
         self.enable = True
-    
-    def on_train_batch_end(self, trainer: "pl.Trainer",
-                           pl_module: "pl.LightningModule",
-                           outputs,
-                           batch,
-                           batch_idx: int) -> None:
+
+    def on_train_batch_end(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule", outputs, batch, batch_idx: int):
         self.train_batch_id = batch_idx + 1
-        c_epoch, num_epoch, c_batch, num_batch, info_dict = self.get_info(trainer, 'train', 'step')
+        c_epoch, num_epoch, c_batch, num_batch = self.get_info(trainer, 'train')
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = 'TRAIN >'
-        info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in info_dict.items()])
+        info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in outputs.items()])
         print(f"{progress} {stage} {info}", end="\r", flush=True)
         return super().on_train_batch_end(trainer, pl_module, outputs, batch, batch_idx)
 
     def on_train_epoch_end(self, trainer, pl_module):
-        train_c_epoch, train_num_epoch, train_c_batch, train_num_batch, train_info_dict = self.get_info(
-            trainer, 'train', 'epoch')
-        val_c_epoch, val_num_epoch, val_c_batch, val_num_batch, val_info_dict = self.get_info(trainer, 'val', 'epoch')
+        train_c_epoch, train_num_epoch, _, train_num_batch = self.get_info(trainer, 'train')
+        _, _, _, val_num_batch = self.get_info(trainer, 'val')
+
+        train_info_dict = self.get_epoch_loss(trainer, 'train')
+        train_info_dict.update(trainer.train_epoch_metric_values)
+
+        val_info_dict = {}
+        if len(trainer.datamodule.val_dataloader()) > 0:
+            val_info_dict = self.get_epoch_loss(trainer, 'val')
+            val_info_dict.update(trainer.val_epoch_metric_values)
 
         progress = f"E:{train_c_epoch:>3d}/{train_num_epoch:<3d} B:{train_num_batch:>4} {val_num_batch:<4}"
         train_stage = 'TRAIN >'
         train_info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in train_info_dict.items()])
+
         val_stage = '  VAL >'
         val_info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in val_info_dict.items()])
         if not val_info:
             val_stage = ''
         print(progress, train_stage, train_info, val_stage, val_info)
-    
-    def on_validation_batch_end(self, trainer: "pl.Trainer",
-                                pl_module: "pl.LightningModule",
-                                outputs,
-                                batch, 
-                                batch_idx: int,
-                                dataloader_idx: int = 0):
+
+    def on_validation_batch_end(self, trainer, pl_module, outputs, batch, batch_idx, dataloader_idx: int = 0):
         self.val_batch_id = batch_idx + 1
-        c_epoch, num_epoch, c_batch, num_batch, info_dict = self.get_info(trainer, 'val', 'step')
+        c_epoch, num_epoch, c_batch, num_batch  = self.get_info(trainer, 'val')
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = '  VAL >'
-        info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in info_dict.items()])
+        info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in outputs.items()])
         print(f"{progress} {stage} {info}", end="\r", flush=True)
         return super().on_validation_batch_end(trainer, pl_module, outputs, batch, batch_idx, dataloader_idx)
 
     def on_test_epoch_start(self, trainer, pl_module):
         print('-' * 23)
-    
-    def on_test_batch_end(self, trainer: "pl.Trainer",
-                          pl_module: "pl.LightningModule",
-                          outputs,
-                          batch,
-                          batch_idx: int,
-                          dataloader_idx: int = 0):
+
+    def on_test_batch_end(self, trainer, pl_module, outputs, batch, batch_idx: int, dataloader_idx: int = 0):
         self.test_batch_id = batch_idx + 1
-        c_epoch, num_epoch, c_batch, num_batch, info_dict = self.get_info(trainer, 'test', 'step')
+        c_epoch, num_epoch, c_batch, num_batch = self.get_info(trainer, 'test')
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = ' TEST >'
-        info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in info_dict.items()])
+        info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in outputs.items()])
         print(f"{progress} {stage} {info}", end="\r", flush=True)
         return super().on_test_batch_end(trainer, pl_module, outputs, batch, batch_idx, dataloader_idx)
 
     def on_test_epoch_end(self, trainer, pl_module):
-        c_epoch, num_epoch, c_batch, num_batch, info_dict = self.get_info(trainer, 'test', 'epoch')
+        c_epoch, num_epoch, c_batch, num_batch = self.get_info(trainer, 'test')
+        info_dict = self.get_epoch_loss(trainer, 'test')
+        info_dict.update(trainer.test_epoch_metric_values)
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = ' TEST >'
         info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in info_dict.items()])
         print(progress, stage, info)
 
 
 PrintProgressBar = SimpleBar
 
 class Progress(Callback, ProgressMix):
-    """
-    把获取信息之类的工具转移到该类中，令PrintProgressBar作为该类的子类。将PrintProgressBar改名为SimpleBar。
-    """
-
     def __init__(self, unit='epoch'):
         assert unit in ['epoch', 'step'], '`unit` must be epoch or step'
         self.unit = unit
 
         self.train_batch_id = 0
         self.val_batch_id = 0
         self.test_batch_id = 0
@@ -166,55 +157,64 @@
 
     def on_train_epoch_start(self, trainer, pl_module):
         if self.unit == 'epoch':
             self.curent_epoch = {'train_epoch': None, 'val_epoch': None}
         else:
             self.curent_epoch = {'train_epoch': [], 'val_epoch': []}
 
-    def on_train_batch_end(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule", outputs: STEP_OUTPUT, batch: Any, batch_idx: int) -> None:
+    def on_train_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         self.train_batch_id = batch_idx + 1
         if self.unit == 'step':
-            _, _, _, _, info_dict = self.get_info(trainer, 'train', 'step')
-            self.curent_epoch['train_epoch'].append(info_dict)
-        return super().on_train_batch_end(trainer, pl_module, outputs, batch, batch_idx)
-    
-    def on_validation_batch_end(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule", outputs: Optional[STEP_OUTPUT], batch: Any, batch_idx: int, dataloader_idx: int = 0) -> None:
+            self.curent_epoch['train_epoch'].append(outputs)
+
+    def on_validation_batch_end(self, trainer, pl_module, outputs, batch, batch_idx, dataloader_idx=0):
         self.val_batch_id = batch_idx + 1
         if self.unit == 'step':
-            _, _, _, _, info_dict = self.get_info(trainer, 'val', 'step')
-            self.curent_epoch['val_epoch'].append(info_dict)
-        return super().on_validation_batch_end(trainer, pl_module, outputs, batch, batch_idx, dataloader_idx)
+            self.curent_epoch['val_epoch'].append(outputs)
 
     def on_validation_epoch_end(self, trainer, pl_module):
         if self.unit == 'epoch':
-            _, _, _, _, info_dict = self.get_info(trainer, 'val', 'epoch')
+            info_dict = self.get_epoch_loss(trainer, 'val')
+            info_dict.update(trainer.val_epoch_metric_values)
             self.curent_epoch['val_epoch'] = info_dict
 
     def on_train_epoch_end(self, trainer, pl_module):
         if self.unit == 'epoch':
-            _, _, _, _, info_dict = self.get_info(trainer, 'train', 'epoch')
+            info_dict = self.get_epoch_loss(trainer, 'train')
+            info_dict.update(trainer.train_epoch_metric_values)
             self.curent_epoch['train_epoch'] = info_dict
         self.progress_info.append(self.curent_epoch)
+    
+    def on_test_epoch_end(self, trainer, pl_module):
+        if self.unit == 'epoch':
+            info_dict = self.get_epoch_loss(trainer, 'test')
+            info_dict.update(trainer.test_epoch_metric_values)
+            self.curent_epoch['test_epoch'] = info_dict
 
     def on_train_end(self, trainer, pl_module):
         if self.unit == 'epoch':
             metrics = self.progress_info[0]['train_epoch'].keys()
             train_info = {
                 metric: [e['train_epoch'][metric] for e in self.progress_info]
                 for metric in metrics
             }
+            if len(trainer.datamodule.val_dataloader()) > 0:
+                metrics = self.progress_info[0]['val_epoch'].keys()
+            else:
+                metrics = {}
             val_info = {
                 metric: [e['val_epoch'][metric] for e in self.progress_info if e['val_epoch']]
                 for metric in metrics
             }
             trainer.progress = {'train': train_info, 'val': val_info}
         else:
             metrics = self.progress_info[0]['train_epoch'][0].keys()
             train_info = {
                 metric: list(chain.from_iterable([[b[metric] for b in e['train_epoch']] for e in self.progress_info]))
                 for metric in metrics
             }
+            metrics = self.progress_info[0]['val_epoch'][0].keys()
             val_info = {
                 metric: list(chain.from_iterable([[b[metric] for b in e['val_epoch']] for e in self.progress_info if e['val_epoch']]))
                 for metric in metrics
             }
-            trainer.progress = {'train': train_info, 'val': val_info}
+            trainer.progress = {'train': train_info, 'val': val_info}
```

### Comparing `torchility-0.6.7/torchility/datamodule.py` & `torchility-0.6.8/torchility/datamodule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytorch_lightning as pl
 from pytorch_lightning.utilities.types import EVAL_DATALOADERS, TRAIN_DATALOADERS
 
 
 class GeneralDataModule(pl.LightningDataModule):
-    def __init__(self, train_dl=None, val_dl=None, test_dl=None, pred_dl=None, reset=0):
+    def __init__(self, train_dl=None, val_dls=None, test_dls=None, pred_dl=None, reset=0):
         super().__init__()
         self.train_dl = train_dl
-        self.val_dl = val_dl
-        self.test_dl = test_dl
+        self.val_dl = val_dls if val_dls is not None else []
+        self.test_dls = test_dls if test_dls is not None else  []
         self.pred_dl = pred_dl
         self.reset = reset > 0
 
     def train_dataloader(self) -> TRAIN_DATALOADERS:
         if self.reset:
             if hasattr(self.train_dl, 'reset'):
                 return self.train_dl.reset()
@@ -19,11 +19,11 @@
                 print('\nWARNING! Training dataloader should have a `reset` method which returns a NEW dataloader instance!!\n')
         return self.train_dl
 
     def val_dataloader(self) -> EVAL_DATALOADERS:
         return self.val_dl
 
     def test_dataloader(self) -> EVAL_DATALOADERS:
-        return self.test_dl
+        return self.test_dls
 
     def predict_dataloader(self) -> EVAL_DATALOADERS:
         return self.pred_dl
```

### Comparing `torchility-0.6.7/torchility/hooks.py` & `torchility-0.6.8/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/torchility/losses.py` & `torchility-0.6.8/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/torchility/metrics.py` & `torchility-0.6.8/torchility/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     （1）torchmetrics.Metric的子类，包括torchmetrics中提供的各种指标。
         如果模型输出结果比较复杂，可重写forward方法，先预处理再调用父类forward方法。
     （2）自定义指标。继承MetricBase，指标的计算方法可以以metric_fn参数传入，或者重写forward方法。
         如果模型输出结果比较复杂，可重写prepare方法预处理。
     （3）提供一个函数等可调用对象作为评价指标，它会被自动封装为MetricBase的对象，运行过程与（2）相同。
     
         这三种方式中，最推荐使用第（1）种方式，因为后两种方式会把每个batch的预测和标签记录下来以计算epoch的结果，
-    可能占用较大存储空间。此外，输出结果中第（1）种指标总是位于（2）和（3）种指标之前。
+    可能占用较大存储空间。
 
     注意：__建议__在torchility.Trainer的metrics参数中，为每个指标指定一个名字，用于在进度中显示。例如，
-        m1 = ('m1_name', metric1)
-        m2 = 'm2_name', metric2     # 括号加不加都一样
+        m1 = ('m1_name', metric1)            或者 {'name': 'm1_name', 'metric': metric1}
+        m2 = 'm2_name', metric2              或者 {'name': 'm2_name', 'metric': metric2}
         trainer = torchility.Trainer(metrics=[m1, m2], ...)
     """
     def __init__(self, metric_fn=None, name=None):
         self.name = self.__class__.__name__ if name is None else name
         if metric_fn:
             self.metric_fn = metric_fn
         else:
@@ -47,14 +47,16 @@
         self.target_batchs.append(targets)
 
     def reset(self):
         self.pred_batchs = []
         self.target_batchs = []
 
     def compute(self):
+        if len(self.pred_batchs) == 0 and len(self.pred_batchs) == 0:
+            return 0.0000
         pred_epoch = concat(self.pred_batchs)
         target_epoch = concat(self.target_batchs)
         return self.metric_fn(pred_epoch, target_epoch)
 
     def clone(self):
         return deepcopy(self)
```

### Comparing `torchility-0.6.7/torchility/tasks.py` & `torchility-0.6.8/torchility/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from pytorch_lightning import LightningModule
 from torchmetrics import Metric
 from .utils import detach_clone
 from torch.optim.lr_scheduler import LRScheduler
 from torch.optim import Optimizer
 from typing import Any
 
+
 class GeneralTaskModule(LightningModule):
     def __init__(self, model, loss, optimizer, metrics=None, **kwargs):
         super().__init__(**kwargs)
         self.model = model
         self.loss_fn = loss
         self.opt = optimizer
         self.metrics = metrics
         self.messages = dict()          # 存放训练、验证、测试过程中的各种消息数据
         self.do_test_loss = True
         self.pred_dataloader_has_label = True
+        self.current_dl_idx = 0
 
     def forward(self, *batch_data):                         # 前向计算
         return self.model(*batch_data)
 
     def on_train_start(self):
         self.metrics ={
             'train': [m.to(self.device) if isinstance(m, Metric) else m for m in self.metrics['train']],
@@ -32,41 +34,52 @@
 
     def training_step(self, batch, batch_nb):               # 训练步
         loss, preds, targets, batch_size = self.do_forward(batch)
         self.log('train_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
 
         preds, targets = detach_clone(preds), detach_clone(targets)
         if self.metrics:
-            self.do_metric(preds, targets, 'train', True, True, batch_size)
+            metric_values = self.do_metric(preds, targets, 'train', batch_size, 0)
         self.messages['train_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
-        return loss
+        metric_values['loss'] = loss
+        return metric_values
 
-    def validation_step(self, batch, batch_nb):             # 验证步
+    def validation_step(self, batch, batch_nb, dataloader_idx=0):             # 验证步
         loss, preds, targets, batch_size = self.do_forward(batch)
         self.log('val_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
 
         preds, targets = detach_clone(preds), detach_clone(targets)
         if self.metrics:
-            self.do_metric(preds, targets, 'val', True, True, batch_size)
+            dl_idx = dataloader_idx if self.multi_val_dataloaders else -1
+            metric_values = self.do_metric(preds, targets, 'val', batch_size, dl_idx)
         self.messages['val_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
-        return {'val_loss': loss}
 
-    def test_step(self, batch, batch_nb):                   # 测试步
+        if self.multi_val_dataloaders:
+            metric_values[f'loss/{dataloader_idx}'] = loss
+        else:
+            metric_values['loss'] = loss
+        return metric_values
+
+    def test_step(self, batch, batch_nb, dataloader_idx=0):                   # 测试步
         loss, preds, targets, batch_size = self.do_forward(batch, self.do_test_loss)
         if loss is not None:
             self.log('test_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
 
         preds, targets = detach_clone(preds), detach_clone(targets)
         if self.metrics:
-            self.do_metric(preds, targets, 'test', True, True, batch_size)
+            dl_idx = dataloader_idx if self.multi_test_dataloaders else -1
+            metric_values = self.do_metric(preds, targets, 'test', batch_size, dl_idx)
         self.messages['test_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
+
         if loss is not None:
-            return {'test_loss': loss}
-        else:
-            return None
+            if self.multi_test_dataloaders:
+                metric_values[f'loss/{dataloader_idx}'] = loss
+            else:
+                metric_values['loss'] = loss
+        return metric_values
 
     def predict_step(self, batch: Any, batch_idx: int, dataloader_idx: int = 0) -> Any:
         _, preds, _, _ = self.do_forward(batch, False, self.pred_dataloader_has_label)
         return preds
 
     def configure_optimizers(self):                         # 优化器
         if isinstance(self.opt, (list, tuple)) and len(self.opt) == 2 \
@@ -90,27 +103,30 @@
         if do_loss:
             loss = self.loss_fn(preds, targets)
         else:
             loss = None
         batch_size = self._batch_size(input_feat)
         return loss, preds, targets, batch_size
 
-    def do_metric(self, preds, targets, state, on_step, on_epoch, batch_size):  # 指标计算
-        metrics = self.metrics[state]
+    def do_metric(self, preds, targets, stage, batch_size, dl_idx):  # 指标计算
+        metrics = self.metrics[stage]
+        metric_values = {}
         for metric in metrics:
-            if isinstance(metric, Metric):
-                metric(preds, targets)
-                self.log(f"{state}_{metric.name}", metric, prog_bar=True, on_step=on_step, on_epoch=on_epoch, metric_attribute=metric, batch_size=batch_size)
+            if (metric.dl_idx >=0 and metric.dl_idx != dl_idx) or (stage not in metric.stages):
+                continue
+            value = metric(preds, targets)
+            if isinstance(value, dict):  # 一个函数中计算多个指标，返回一个字典
+                value_dict = {f"{stage}_{metric.name}{k}_step":v for k, v in value.items()}
+                for k, v in value.items():
+                    metric_values[f"{metric.name}{k}"] = v
+                self.log_dict(value_dict, prog_bar=metric.on_bar, on_step=metric.on_step, on_epoch=False, batch_size=batch_size)
             else:
-                value = metric(preds, targets)
-                if isinstance(value, dict):  # 一个函数中计算多个指标，返回一个字典
-                    value_dict = {f"{state}_{metric.name}{k}_step":v for k, v in value.items()}
-                    self.log_dict(value_dict, prog_bar=True, on_step=on_step, on_epoch=False, batch_size=batch_size)
-                else:
-                    self.log(f"{state}_{metric.name}_step", value, prog_bar=True, on_step=on_step, on_epoch=False, batch_size=batch_size)
+                metric_values[f"{metric.name}"] = value
+                self.log(f"{stage}_{metric.name}_step", value, prog_bar=metric.on_bar, on_step=metric.on_step, on_epoch=False, batch_size=batch_size)
+        return metric_values
 
     def _batch_size(self, inputs):
         """检测batch size以用于输出日志"""
         if isinstance(inputs, (tuple, list)):
             data = inputs[0]
         else:
             data = inputs
```

### Comparing `torchility-0.6.7/torchility/trainer.py` & `torchility-0.6.8/torchility/trainer.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from pytorch_lightning import LightningDataModule
 from pytorch_lightning.loggers import TensorBoardLogger
 from pytorch_lightning.callbacks import ProgressBar
 
 from torchmetrics import Metric
 
 from .callbacks import ResetMetrics, SimpleBar
-from .metrics import MetricBase
 from .tasks import GeneralTaskModule
 from .callbacks import Progress
-from .utils import batches
+from .utils import batches, set_attr
 from .datamodule import GeneralDataModule
 
 def default_args(func):
     signature = inspect.signature(func)
     return {
         k: v.default
         for k, v in signature.parameters.items()
@@ -49,15 +48,15 @@
 
         metrics = self._prepare_metrics(metrics)
         if task_module is None:
             task_kwargs = task_kwargs if task_kwargs is not None else {}
             self.task_module = GeneralTaskModule(model, loss, optimizer, metrics, **task_kwargs)
         else:
             self.task_module = task_module
-        self.datamodule = datamodule
+        self.datamodule = None
 
         #   *************************************
         #   *    Trainer Parameters    --- LIC  *
         #   *************************************
         if epochs is not None:  # for easy use
             self.init_params['max_epochs'] = epochs
         if pltrainer_kwargs.get('log_every_n_steps', None) is None: # log each step
@@ -90,79 +89,55 @@
             self.init_params['reload_dataloaders_every_n_epochs'] = reset_dl
 
         super().__init__(**self.init_params)
 
     def _prepare_metrics(self, metrics, just_for_test=False):
         metrics_ready = {'train': [], 'val':[], 'test':[]}
         for m in metrics:
-            if isinstance(m, (tuple, list)):  # when m is (metric_name, metric)
-                assert len(m) == 2, '`metric` should be a tuple of (metric_name, metric_callable)'
-                name, m = m
-                m.name = name
-            if isinstance(m, (Metric, MetricBase)):
-                if not hasattr(m, 'name'):
-                    m.name = m.__class__.__name__
-                if just_for_test:
-                    metrics_ready['test'].append(m.clone())
-                else:
-                    metrics_ready['train'].append(m)
-                    metrics_ready['val'].append(m.clone())
-                    metrics_ready['test'].append(m.clone())
+            m = set_attr(m)
+            if just_for_test:
+                metrics_ready['test'].append(m)
             else:
-                if not hasattr(m, 'name'):
-                    name = m.__name__ if hasattr(m, '__name__') else type(m).__name__
-                else:
-                    name = m.name
-                if just_for_test:
-                    metrics_ready['test'].append(MetricBase(m, name))
-                else:
-                    metrics_ready['train'].append(MetricBase(m, name))
-                    metrics_ready['val'].append(MetricBase(m, name))
-                    metrics_ready['test'].append(MetricBase(m, name))
+                for stage in m.stages:
+                    metrics_ready[stage].append(m.clone())
+        del metrics
         return metrics_ready if not just_for_test else metrics_ready['test']
 
-    def fit(self, train_dl=None, val_dl=None, epochs=None, ckpt_path=None):
-        if self.datamodule:
-            super().fit(self.task_module, datamodule=self.datamodule, ckpt_path=ckpt_path)
-        else:
-            dm = GeneralDataModule(train_dl=train_dl, val_dl=val_dl, reset=self.reset_dl)
-            # super().fit(self.task_module, train_dataloaders=train_dl, val_dataloaders=val_dl, ckpt_path=ckpt_path)
-            super().fit(self.task_module, datamodule=dm, ckpt_path=ckpt_path)
+    def fit(self, train_dl, val_dls=None, ckpt_path=None):
+        self.task_module.multi_val_dataloaders = False  # 是否使用多个验证dataloader
+        if isinstance(val_dls, (list, tuple)) and len(val_dls) > 1:
+            self.task_module.multi_val_dataloaders = True
+
+        dm = GeneralDataModule(train_dl=train_dl, val_dls=val_dls, reset=self.reset_dl)
+        self.datamodule = dm
+        super().fit(self.task_module, datamodule=dm, ckpt_path=ckpt_path)
         return self.progress
 
-    def test(self, test_dl=None, ckpt_path='best', verbose=True, metrics=None, do_loss=True):  # pylint: disable=arguments-renamed
+    def test(self, test_dls, ckpt_path='best', verbose=True, metrics=None, do_loss=True):  # pylint: disable=arguments-renamed
         """
         Args:
             metrics: 一旦提供了test的metrics，则会将trainer中用于test的metrics覆盖，也就是说可以指定仅用于test的metrics
             do_loss: 在测试时是否计算损失函数，当测试任务和训练任务数据不一致无法计算损失函数时，可设do_loss=False
         """
+        self.task_module.multi_test_dataloaders = False          # 是否使用多个测试dataloader
+        if isinstance(test_dls, (list, tuple)) and len(test_dls) > 1:
+            self.task_module.multi_test_dataloaders = True
+
         self.task_module.do_test_loss = do_loss
         if metrics is not None:  # 如果提供了仅用于test的metrics
             test_metrics = self._prepare_metrics(metrics, just_for_test=True)
             self.task_module.metrics['test'] = test_metrics
 
-        if test_dl is not None:
-            dm = GeneralDataModule(test_dl=test_dl)
-            return super().test(self.task_module, datamodule=dm, ckpt_path=ckpt_path, verbose=verbose)
-            # return super().test(self.task_module, dataloaders=test_dl, ckpt_path=ckpt_path, verbose=verbose)
-        elif self.datamodule and self.datamodule.test_dataloader():
-            return super().test(self.task_module, datamodule=self.datamodule, ckpt_path=ckpt_path, verbose=verbose)
-        else:
-            raise Exception("Dataloader or DataModule is needed!")  # pylint: disable=broad-exception-raised
+        dm = GeneralDataModule(test_dls=test_dls)
+        return super().test(self.task_module, datamodule=dm, ckpt_path=ckpt_path, verbose=verbose)
 
-    def predict(self, pred_dl=None, has_label=False, ckpt_path='best', concat=True):  # pylint: disable=arguments-renamed
+    def predict(self, pred_dl, has_label=False, ckpt_path='best', concat=True):  # pylint: disable=arguments-renamed
         self.task_module.pred_dataloader_has_label = has_label
-        if pred_dl is not None:
-            dm = GeneralDataModule(pred_dl=pred_dl)
-            preds = super().predict(self.task_module, datamodule=dm, return_predictions=True, ckpt_path=ckpt_path)
-            # preds = super().predict(self.task_module, pred_dl, None, return_predictions=True, ckpt_path=ckpt_path)
-        elif self.datamodule and self.datamodule.test_dataloader():
-            preds = super().predict(self.task_module, None, datamodule=self.datamodule, return_predictions=True, ckpt_path=ckpt_path)
-        else:
-            raise Exception("Dataloader or DataModule is needed!")  # pylint: disable=broad-exception-raised
+        dm = GeneralDataModule(pred_dl=pred_dl)
+        preds = super().predict(self.task_module, datamodule=dm, return_predictions=True, ckpt_path=ckpt_path)
         if concat:
             return torch.cat(preds, dim=0)
         else:
             return preds
 
     def predict_with_best(self, *inputs, batch_size=0, train=False):
         """
@@ -212,15 +187,15 @@
     def restore_best(self):
         """
         restore best checkpoint
         """
         model = self.task_module.model
         loss = self.task_module.loss_fn
         opt = self.task_module.opt
-        self.task_module = self.task_module.load_from_checkpoint(self.checkpoint_callback.best_model_path, 
+        self.task_module = self.task_module.load_from_checkpoint(self.checkpoint_callback.best_model_path,
                                                             model=model, loss=loss, optimizer=opt)
         return self.task_module.model
 
     def restore_best_k(self):
         """
         restore best k checkpoints. k is the value of `save_top_k` argument in the `ModelCheckpoint` callback.
         """
@@ -242,15 +217,15 @@
             path: path and filename of the state_dict file.
             mode: 'best' for the best model and others for current model.
         """
         if mode == 'best':
             model = self.task_module.model
             loss = self.task_module.loss_fn
             opt = self.task_module.opt
-            task = self.task_module.load_from_checkpoint(self.checkpoint_callback.best_model_path, 
+            task = self.task_module.load_from_checkpoint(self.checkpoint_callback.best_model_path,
                                                             model=model, loss=loss, optimizer=opt)
             torch.save(task.model.state_dict(), path)
         else:
             torch.save(self.task_module.model.state_dict(), path)
 
     def load_state_dict(self, path='best_model.pth', model=None):
         """load state_dict for pytorch model"""
```

### Comparing `torchility-0.6.7/torchility/utils/plots.py` & `torchility-0.6.8/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/torchility/utils/utils.py` & `torchility-0.6.8/torchility/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/torchility/utils/yaml_config.py` & `torchility-0.6.8/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.7/torchility.egg-info/PKG-INFO` & `torchility-0.6.8/torchility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.7
+Version: 0.6.8
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.6.7/torchility.egg-info/SOURCES.txt` & `torchility-0.6.8/torchility.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 torchility.egg-info/top_level.txt
 torchility/callbacks/__init__.py
 torchility/callbacks/common.py
 torchility/callbacks/interpreters.py
 torchility/callbacks/performances.py
 torchility/callbacks/progress.py
 torchility/utils/__init__.py
+torchility/utils/metric_utils.py
 torchility/utils/plots.py
 torchility/utils/utils.py
 torchility/utils/yaml_config.py
```

