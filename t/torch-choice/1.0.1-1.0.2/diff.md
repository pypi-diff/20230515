# Comparing `tmp/torch_choice-1.0.1.tar.gz` & `tmp/torch_choice-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_choice-1.0.1.tar", last modified: Tue Apr 11 02:20:16 2023, max compression
+gzip compressed data, was "torch_choice-1.0.2.tar", last modified: Mon May 15 17:07:20 2023, max compression
```

## Comparing `torch_choice-1.0.1.tar` & `torch_choice-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.029373 torch_choice-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-04-11 02:20:16.029373 torch_choice-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-04-11 02:20:06.000000 torch_choice-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:20:16.029373 torch_choice-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-11 02:20:06.000000 torch_choice-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-11 02:20:06.000000 torch_choice-1.0.1/tests/test_choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-11 02:20:06.000000 torch_choice-1.0.1/tests/test_conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-11 02:20:06.000000 torch_choice-1.0.1/tests/test_nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/torch_choice/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/torch_choice/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/data/choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/data/joint_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/torch_choice/model/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/formula_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.029373 torch_choice-1.0.1/torch_choice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/easy_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/run_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/run_helper_temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/torch_choice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-04-11 02:20:16.000000 torch_choice-1.0.1/torch_choice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-11 02:20:16.000000 torch_choice-1.0.1/torch_choice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:20:16.000000 torch_choice-1.0.1/torch_choice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 02:20:16.000000 torch_choice-1.0.1/torch_choice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.759558 torch_choice-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-05-15 17:07:20.759558 torch_choice-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-05-15 17:07:07.000000 torch_choice-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:07:20.759558 torch_choice-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-15 17:07:07.000000 torch_choice-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-05-15 17:07:07.000000 torch_choice-1.0.2/tests/test_choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-15 17:07:07.000000 torch_choice-1.0.2/tests/test_conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-15 17:07:07.000000 torch_choice-1.0.2/tests/test_nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/torch_choice/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/torch_choice/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/example_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/joint_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/torch_choice/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/formula_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.759558 torch_choice-1.0.2/torch_choice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/easy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/run_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/run_helper_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/torch_choice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-05-15 17:07:20.000000 torch_choice-1.0.2/torch_choice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-15 17:07:20.000000 torch_choice-1.0.2/torch_choice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:07:20.000000 torch_choice-1.0.2/torch_choice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 17:07:20.000000 torch_choice-1.0.2/torch_choice.egg-info/top_level.txt
```

### Comparing `torch_choice-1.0.1/setup.py` & `torch_choice-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="torch_choice",
-    version="1.0.1",
+    version="1.0.2",
     description="A Pytorch Backend Library for Choice Modelling",
     long_description=README,
     long_description_content_type="text/markdown",
     url="",
     author="Tianyu Du",
     author_email="tianyudu@stanford.edu",
     license="MIT",
```

### Comparing `torch_choice-1.0.1/tests/test_choice_dataset.py` & `torch_choice-1.0.2/tests/test_choice_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/tests/test_conditional_logit_model.py` & `torch_choice-1.0.2/tests/test_conditional_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/tests/test_nested_logit_model.py` & `torch_choice-1.0.2/tests/test_nested_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/torch_choice/data/choice_dataset.py` & `torch_choice-1.0.2/torch_choice/data/choice_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/torch_choice/data/joint_dataset.py` & `torch_choice-1.0.2/torch_choice/data/joint_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,7 +95,24 @@
 
         Returns:
             ChoiceDataset: the modified dataset on the new device.
         """
         for d in self.datasets.values():
             d = d.to(device)
         return self
+
+    def clone(self) -> "JointDataset":
+        """Returns a copy of the dataset.
+
+        Returns:
+            JointDataset: a copy of the dataset.
+        """
+        return JointDataset(**{name: d.clone() for (name, d) in self.datasets.items()})
+
+    @property
+    def item_index(self) -> torch.LongTensor:
+        """Returns the current index of each dataset.
+
+        Returns:
+            torch.LongTensor: the indices of items chosen.
+        """
+        return self.datasets["item"].item_index
```

### Comparing `torch_choice-1.0.1/torch_choice/data/utils.py` & `torch_choice-1.0.2/torch_choice/data/utils.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/torch_choice/model/coefficient.py` & `torch_choice-1.0.2/torch_choice/model/coefficient.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/torch_choice/model/conditional_logit_model.py` & `torch_choice-1.0.2/torch_choice/model/conditional_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/torch_choice/model/formula_parser.py` & `torch_choice-1.0.2/torch_choice/model/formula_parser.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/torch_choice/model/nested_logit_model.py` & `torch_choice-1.0.2/torch_choice/model/nested_logit_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
     def forward(self, batch: ChoiceDataset) -> torch.Tensor:
         """An standard forward method for the model, the user feeds a ChoiceDataset batch and the model returns the
             predicted log-likelihood tensor. The main forward passing happens in the _forward() method, but we provide
             this wrapper forward() method for a cleaner API, as forward() only requires a single batch argument.
             For more details about the forward passing, please refer to the _forward() method.
 
-        # TODO: the ConditionaLogitModel returns predicted utility, the NestedLogitModel behaves the same?
+        # TODO: the ConditionalLogitModel returns predicted utility, the NestedLogitModel behaves the same?
 
         Args:
             batch (ChoiceDataset): a ChoiceDataset object containing the data batch.
 
         Returns:
             torch.Tensor: a tensor of shape (num_trips, num_items) including the log probability
             of choosing item i in trip t.
```

### Comparing `torch_choice-1.0.1/torch_choice/utils/easy_data_wrapper.py` & `torch_choice-1.0.2/torch_choice/utils/easy_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/torch_choice/utils/run_helper.py` & `torch_choice-1.0.2/torch_choice/utils/run_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,101 @@
 """
 This is a template script for researchers to train the PyTorch-based model with minimal effort.
 The researcher only needs to initialize the dataset and the model, this training template comes with default
 hyper-parameters including batch size and learning rate. The researcher should experiment with different levels
 of hyper-parameter if the default setting doesn't converge well.
 """
+import numpy as np
 import pandas as pd
 from copy import deepcopy
 import torch
 import torch.nn.functional as F
+import torch.optim
 from torch_choice.data import utils as data_utils
 from torch_choice.utils.std import parameter_std
 from torch_choice.model.conditional_logit_model import ConditionalLogitModel
 from torch_choice.model.nested_logit_model import NestedLogitModel
 
 
-def run(model, dataset, dataset_test=None, batch_size=-1, learning_rate=0.01, num_epochs=5000, report_frequency=None, compute_std=True, return_final_training_log_likelihood=False):
+def run(model, dataset, dataset_test=None, batch_size=-1, learning_rate=0.01, num_epochs=5000, report_frequency=None, compute_std=True, return_final_training_log_likelihood=False, model_optimizer='Adam'):
     """All in one script for the model training and result presentation."""
     if report_frequency is None:
         report_frequency = (num_epochs // 10)
 
     assert isinstance(model, ConditionalLogitModel) or isinstance(model, NestedLogitModel), \
         f'A model of type {type(model)} is not supported by this runner.'
     model = deepcopy(model)  # do not modify the model outside.
     trained_model = deepcopy(model)  # create another copy for returning.
     data_loader = data_utils.create_data_loader(dataset, batch_size=batch_size, shuffle=True)
-    optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
+
+    optimizer = {'SGD': torch.optim.SGD,
+                 'Adagrad': torch.optim.Adagrad,
+                 'Adadelta': torch.optim.Adadelta,
+                 'Adam': torch.optim.Adam}[model_optimizer](model.parameters(), lr=learning_rate)
+
+    # optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
+    # optimizer = torch.optim.Adagrad(model.parameters(), lr=learning_rate)
+    # optimizer = torch.optim.Adadelta(model.parameters(), lr=learning_rate)
+    # scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=10000, gamma=0.1)
+    scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=10000, gamma=0.7)
+    # scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=5000, gamma=0.5)
     print('=' * 20, 'received model', '=' * 20)
     print(model)
     print('=' * 20, 'received dataset', '=' * 20)
     print(dataset)
     print('=' * 20, 'training the model', '=' * 20)
+
+    total_loss_history = list()
+    tol = 0.001  # stop if the loss failed to improve tol proportion of average performance in the last k iterations.
+    k = 5
     # fit the model.
     for e in range(1, num_epochs + 1):
         # track the log-likelihood to minimize.
-        ll, count = 0.0, 0.0
+        ll, count, total_loss = 0.0, 0.0, 0.0
         for batch in data_loader:
             item_index = batch['item'].item_index if isinstance(model, NestedLogitModel) else batch.item_index
             # the model.loss returns negative log-likelihood + regularization term.
             loss = model.loss(batch, item_index)
+            total_loss -= loss
 
-            if (e % report_frequency) == 0:
-                # record log-likelihood.
-                ll -= model.negative_log_likelihood(batch, item_index).detach().item() # * len(batch)
-                count += len(batch)
+            with torch.no_grad():
+                if (e % report_frequency) == 0:
+                    # record log-likelihood.
+                    ll -= model.negative_log_likelihood(batch, item_index).detach().item() # * len(batch)
+                    count += len(batch)
+
+                    pred = model.forward(batch).argmax(dim=1)
+                    acc = (pred == item_index).float().mean().item()
+                    print('Accuracy: ', acc)
 
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
+        scheduler.step()
 
+        current_loss = float(total_loss.detach().item())
+        # if e > k:
+        if False:
+            past_avg = np.mean(total_loss_history[-k:])
+            improvement = (past_avg - current_loss) / past_avg
+            if improvement < tol:
+                print(f'Early stopped at {e} epochs.')
+                break
+        total_loss_history.append(current_loss)
         # ll /= count
         if (e % report_frequency) == 0:
             print(f'Epoch {e}: Log-likelihood={ll}')
 
     if dataset_test is not None:
         test_ll = - model.negative_log_likelihood(dataset_test, dataset_test.item_index).detach().item()
         print('Test set log-likelihood: ', test_ll)
 
+    # final training log-likelihood.
+    ll = - model.negative_log_likelihood(dataset if isinstance(model, ConditionalLogitModel) else dataset.datasets, dataset.item_index).detach().item() # * len(batch)
+
     if not compute_std:
         if return_final_training_log_likelihood:
             return model, ll
         else:
             return model
     else:
         # current methods of computing standard deviation will corrupt the model, load weights into another model for returning.
@@ -90,15 +126,15 @@
             mean = mean_dict[coef_name].cpu().detach().numpy()
             coef_name = coef_name.replace('coef_dict.', '').replace('.coef', '')
             for i in range(mean.size):
                 report.append({'Coefficient': coef_name + f'_{i}',
                             'Estimation': float(mean[i]),
                             'Std. Err.': float(std[i])})
         report = pd.DataFrame(report).set_index('Coefficient')
-        print(f'Training Epochs: {num_epochs}\n')
+        print(f'Training Epochs: stopped at {e}, maximum allowed: {num_epochs}\n')
         print(f'Learning Rate: {learning_rate}\n')
         print(f'Batch Size: {batch_size if batch_size != -1 else len(dataset)} out of {len(dataset)} observations in total\n')
         print(f'Final Log-likelihood: {ll}\n')
         print('Coefficients:\n')
         print(report.to_markdown())
         if return_final_training_log_likelihood:
             return trained_model, ll
```

### Comparing `torch_choice-1.0.1/torch_choice/utils/run_helper_temp.py` & `torch_choice-1.0.2/torch_choice/utils/run_helper_lightning.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,303 +1,236 @@
 """
 This is a template script for researchers to train the PyTorch-based model with minimal effort.
 The researcher only needs to initialize the dataset and the model, this training template comes with default
 hyper-parameters including batch size and learning rate. The researcher should experiment with different levels
 of hyper-parameter if the default setting doesn't converge well.
+
+This is a modified version of the original run_helper.py script, which is modified to work with PyTorch Lightning.
 """
 import time
 from copy import deepcopy
-from typing import List, Union
+from typing import Optional, Union
 
-import numpy as np
 import pandas as pd
 import pytorch_lightning as pl
 import torch
 import torch.nn.functional as F
-from bemb.model import BEMBFlex
-from sklearn import metrics
+from pytorch_lightning.callbacks.early_stopping import EarlyStopping
+from scipy.stats import norm
+
 from torch_choice.data import ChoiceDataset
-from torch_choice.data import utils as data_utils
 from torch_choice.data.utils import create_data_loader
 from torch_choice.model.conditional_logit_model import ConditionalLogitModel
 from torch_choice.model.nested_logit_model import NestedLogitModel
 from torch_choice.utils.std import parameter_std
 
 
 class LightningModelWrapper(pl.LightningModule):
     def __init__(self,
                  model: Union [ConditionalLogitModel, NestedLogitModel],
-                 learning_rate: float=0.3):
-        """The lightning model wrapper for conditional and nested logit model."""
+                 learning_rate: float,
+                 model_optimizer: str):
+        """
+        The pytorch-lightning model wrapper for conditional and nested logit model.
+        Ideally, end users don't need to interact with this class. This wrapper will be called by the run() function.
+        """
         super().__init__()
         self.model = model
         self.learning_rate = learning_rate
+        self.optimizer_class_string = model_optimizer
 
     def __str__(self) -> str:
         return str(self.model)
 
     def forward(self, *args, **kwargs):
         return self.model(*args, **kwargs)
 
     @torch.no_grad()
     def _get_performance_dict(self, batch):
         item_index = batch['item'].item_index if isinstance(self.model, NestedLogitModel) else batch.item_index
-        ll -= self.model.negative_log_likelihood(batch, item_index).detach().item()
+        ll = - self.model.negative_log_likelihood(batch, item_index).detach().item()
         return {'log_likelihood': ll}
 
     def training_step(self, batch, batch_idx):
         item_index = batch['item'].item_index if isinstance(self.model, NestedLogitModel) else batch.item_index
         loss = self.model.loss(batch, item_index)
-        self.log('train_loss', loss, prog_bar=True, batch_size=len(batch))
-        for key, val in self._get_performance_dict(batch).items():
-            self.log('test_' + key, val, prog_bar=True, batch_size=len(batch))
+        self.log('train_loss', loss, prog_bar=False, batch_size=len(batch))
+        # skip computing log-likelihood for training steps to speed up training.
+        # for key, val in self._get_performance_dict(batch).items():
+            # self.log('test_' + key, val, prog_bar=True, batch_size=len(batch))
         return loss
 
     def validation_step(self, batch, batch_idx):
         for key, val in self._get_performance_dict(batch).items():
-            self.log('val_' + key, val, prog_bar=True, batch_size=len(batch))
+            self.log('val_' + key, val, prog_bar=False, batch_size=len(batch))
 
     def test_step(self, batch, batch_idx):
         for key, val in self._get_performance_dict(batch).items():
-            self.log('test_' + key, val, prog_bar=True, batch_size=len(batch))
+            self.log('test_' + key, val, prog_bar=False, batch_size=len(batch))
 
     def configure_optimizers(self):
-        optimizer = torch.optim.Adam(self.parameters(), lr=self.learning_rate)
-        return optimizer
-
-    # def fit_model(self, dataset_list: List[ChoiceDataset], batch_size: int=-1, num_epochs: int=10, num_workers: int=8, **kwargs) -> "LitBEMBFlex":
-    #     """A standard pipeline of model training and evaluation.
-
-    #     Args:
-    #         dataset_list (List[ChoiceDataset]): train_dataset, validation_test, and test_dataset in a list of length 3.
-    #         batch_size (int, optional): batch_size for training and evaluation. Defaults to -1, which indicates full-batch training.
-    #         num_epochs (int, optional): number of epochs for training. Defaults to 10.
-    #         **kwargs: additional keyword argument for the pytorch-lightning Trainer.
-
-    #     Returns:
-    #         LitBEMBFlex: the trained bemb model.
-    #     """
-
-    #     def section_print(input_text):
-    #         """Helper function for printing"""
-    #         print('=' * 20, input_text, '=' * 20)
-    #     # present a summary of the model received.
-    #     section_print('model received')
-    #     print(self)
-
-    #     # present a summary of datasets received.
-    #     section_print('data set received')
-    #     print('[Training dataset]', dataset_list[0])
-    #     print('[Validation dataset]', dataset_list[1])
-    #     print('[Testing dataset]', dataset_list[2])
-
-    #     # create pytorch dataloader objects.
-    #     train = create_data_loader(dataset_list[0], batch_size=batch_size, shuffle=True, num_workers=num_workers)
-    #     validation = create_data_loader(dataset_list[1], batch_size=batch_size, shuffle=False, num_workers=num_workers)
-    #     # WARNING: the test step takes extensive memory cost since it computes likelihood for all items.
-    #     # we run the test step with a much smaller batch_size.
-    #     test = create_data_loader(dataset_list[2], batch_size=batch_size // 10, shuffle=False, num_workers=num_workers)
-
-    #     section_print('train the model')
-    #     trainer = pl.Trainer(gpus=1 if ('cuda' in str(self)) else 0,  # use GPU if the model is currently on the GPU.
-    #                         max_epochs=num_epochs,
-    #                         check_val_every_n_epoch=1,
-    #                         log_every_n_steps=1,
-    #                         **kwargs)
-    #     start_time = time.time()
-    #     trainer.fit(self, train_dataloaders=train, val_dataloaders=validation)
-    #     print(f'time taken: {time.time() - start_time}')
-
-    #     section_print('test performance')
-    #     trainer.test(self, dataloaders=test)
-    #     return self
-
-
-
-def run_original(model, dataset, dataset_test=None, batch_size=-1, learning_rate=0.01, num_epochs=5000, report_frequency=None):
-    """All in one script for the model training and result presentation."""
-    if report_frequency is None:
-        report_frequency = (num_epochs // 10)
-
-    assert isinstance(model, ConditionalLogitModel) or isinstance(model, NestedLogitModel), \
-        f'A model of type {type(model)} is not supported by this runner.'
-    model = deepcopy(model)  # do not modify the model outside.
-    trained_model = deepcopy(model)  # create another copy for returning.
-    data_loader = data_utils.create_data_loader(dataset, batch_size=batch_size, shuffle=True)
-    optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
-    print('=' * 20, 'received model', '=' * 20)
-    print(model)
-    print('=' * 20, 'received dataset', '=' * 20)
-    print(dataset)
-    print('=' * 20, 'training the model', '=' * 20)
-    # fit the model.
-    for e in range(1, num_epochs + 1):
-        # track the log-likelihood to minimize.
-        ll, count = 0.0, 0.0
-        for batch in data_loader:
-            item_index = batch['item'].item_index if isinstance(model, NestedLogitModel) else batch.item_index
-            # the model.loss returns negative log-likelihood + regularization term.
-            loss = model.loss(batch, item_index)
-
-            if (e % report_frequency) == 0:
-                # record log-likelihood.
-                ll -= model.negative_log_likelihood(batch, item_index).detach().item() # * len(batch)
-                count += len(batch)
-
-            optimizer.zero_grad()
-            loss.backward()
-            optimizer.step()
-
-        # ll /= count
-        if (e % report_frequency) == 0:
-            print(f'Epoch {e}: Log-likelihood={ll}')
-
-    if dataset_test is not None:
-        test_ll = - model.negative_log_likelihood(dataset_test, dataset_test.item_index).detach().item()
-        print('Test set log-likelihood: ', test_ll)
-
-    # current methods of computing standard deviation will corrupt the model, load weights into another model for returning.
-    state_dict = deepcopy(model.state_dict())
-    trained_model.load_state_dict(state_dict)
-
-    # get mean of estimation.
-    mean_dict = dict()
-    for k, v in model.named_parameters():
-        mean_dict[k] = v.clone()
-
-    # estimate the standard error of the model.
-    if isinstance(model, ConditionalLogitModel):
-        def nll_loss(model):
-            y_pred = model(dataset)
-            return F.cross_entropy(y_pred, dataset.item_index, reduction='sum')
-    elif isinstance(model, NestedLogitModel):
-        def nll_loss(model):
-            d = dataset[torch.arange(len(dataset))]
-            return model.negative_log_likelihood(d, d['item'].item_index)
-
-    std_dict = parameter_std(model, nll_loss)
-
-    print('=' * 20, 'model results', '=' * 20)
-    report = list()
-    for coef_name, std in std_dict.items():
-        std = std.cpu().detach().numpy()
-        mean = mean_dict[coef_name].cpu().detach().numpy()
-        coef_name = coef_name.replace('coef_dict.', '').replace('.coef', '')
-        for i in range(mean.size):
-            report.append({'Coefficient': coef_name + f'_{i}',
-                           'Estimation': float(mean[i]),
-                           'Std. Err.': float(std[i])})
-    report = pd.DataFrame(report).set_index('Coefficient')
-    print(f'Training Epochs: {num_epochs}\n')
-    print(f'Learning Rate: {learning_rate}\n')
-    print(f'Batch Size: {batch_size if batch_size != -1 else len(dataset)} out of {len(dataset)} observations in total\n')
-    print(f'Final Log-likelihood: {ll}\n')
-    print('Coefficients:\n')
-    print(report.to_markdown())
-    return trained_model
-
+        return getattr(torch.optim, self.optimizer_class_string)(self.parameters(), lr=self.learning_rate)
 
 def section_print(input_text):
     """Helper function for printing"""
     print('=' * 20, input_text, '=' * 20)
 
 
-def run_on_lightning(lightning_model: LightningModelWrapper,
-                     dataset_list: List[ChoiceDataset],
-                     batch_size: int=-1,
-                     num_epochs: int=10,
-                     num_workers: int=8,
-                     **kwargs) -> LightningModelWrapper:
-    """A standard pipeline of model training and evaluation.
+def run(model: Union [ConditionalLogitModel, NestedLogitModel],
+        dataset_train: ChoiceDataset,
+        dataset_val: Optional[ChoiceDataset]=None,
+        dataset_test: Optional[ChoiceDataset]=None,
+        model_optimizer: str='Adam',
+        batch_size: int=-1,
+        learning_rate: float=0.01,
+        num_epochs: int=10,
+        num_workers: int=0,
+        device: Optional[str]=None,
+        **kwargs) -> Union[ConditionalLogitModel, NestedLogitModel]:
+    """_summary_
 
     Args:
-        model (LitBEMBFlex): the initialized pytorch-lightning wrapper of bemb.
-        dataset_list (List[ChoiceDataset]): train_dataset, validation_test, and test_dataset in a list of length 3.
-        batch_size (int, optional): batch_size for training and evaluation. Defaults to -1, which indicates full-batch training.
-        num_epochs (int, optional): number of epochs for training. Defaults to 10.
-        **kwargs: additional keyword argument for the pytorch-lightning Trainer.
+        model (Union[ConditionalLogitModel, NestedLogitModel]): the constructed model.
+        dataset_train (ChoiceDataset): the dataset for training.
+        dataset_val (ChoiceDataset): an optional dataset for validation.
+        dataset_test (ChoiceDataset): an optional dataset for testing.
+        batch_size (int, optional): batch size for model training. Defaults to -1.
+        learning_rate (float, optional): learning rate for model training. Defaults to 0.01.
+        num_epochs (int, optional): number of epochs for the training. Defaults to 10.
+        num_workers (int, optional): number of parallel workers for data loading. Defaults to 0.
+        device (Optional[str], optional): the device that trains the model, if None is specified, the function will
+            use the current device of the provided model. Defaults to None.
+        **kwargs: other keyword arguments for the pytorch lightning trainer, this is for users with experience in
+            pytorch lightning and wish to customize the training process.
 
     Returns:
-        LitBEMBFlex: the trained bemb model.
+        Union[ConditionalLogitModel, NestedLogitModel]: the trained model.
     """
-    # present a summary of the model received.
-    model = lightning_model.model
-    model_clone = deepcopy(model)  # create another copy for returning.
+    # ==================================================================================================================
+    # Setup the lightning wrapper.
+    # ==================================================================================================================
+    lightning_model = LightningModelWrapper(model,
+                                            learning_rate=learning_rate,
+                                            model_optimizer=model_optimizer)
+    if device is None:
+        # infer from the model device.
+        device = str(model.device)
+    # the cloned model will be used for standard error calculation later.
+    model_clone = deepcopy(model)
     section_print('model received')
     print(model)
 
+    # ==================================================================================================================
+    # Prepare the data.
+    # ==================================================================================================================
     # present a summary of datasets received.
     section_print('data set received')
-    print('[Training dataset]', dataset_list[0])
-    print('[Validation dataset]', dataset_list[1])
-    print('[Testing dataset]', dataset_list[2])
+    print('[Train dataset]', dataset_train)
+    print('[Validation dataset]', dataset_val)
+    print('[Test dataset]', dataset_test)
 
     # create pytorch dataloader objects.
-    train = create_data_loader(dataset_list[0], batch_size=batch_size, shuffle=True, num_workers=num_workers)
-    if dataset_list[1] is not None:
-        validation = create_data_loader(dataset_list[1], batch_size=batch_size, shuffle=False, num_workers=num_workers)
+    train_dataloader = create_data_loader(dataset_train.to(device), batch_size=batch_size, shuffle=True, num_workers=num_workers)
+
+    if dataset_val is not None:
+        val_dataloader = create_data_loader(dataset_val.to(device), batch_size=batch_size, shuffle=False, num_workers=num_workers)
     else:
-        validation = None
-    # WARNING: the test step takes extensive memory cost since it computes likelihood for all items.
-    # we run the test step with a much smaller batch_size.
-    if dataset_list[2] is not None:
-        test = create_data_loader(dataset_list[2], batch_size=batch_size // 10, shuffle=False, num_workers=num_workers)
+        val_dataloader = None
+
+    if dataset_test is not None:
+        test_dataloader = create_data_loader(dataset_test.to(device), batch_size=batch_size, shuffle=False, num_workers=num_workers)
     else:
-        test = None
+        test_dataloader = None
 
-    section_print('train the model')
-    trainer = pl.Trainer(gpus=1 if ('cuda' in str(model.device)) else 0,  # use GPU if the model is currently on the GPU.
+    # ==================================================================================================================
+    # Training the model.
+    # ==================================================================================================================
+    # if the validation dataset is provided, do early stopping.
+    callbacks = [EarlyStopping(monitor="val_ll", mode="max", patience=10, min_delta=0.001)] if val_dataloader is not None else []
+
+    trainer = pl.Trainer(accelerator="cuda" if "cuda" in device else device,  # note: "cuda:0" is not a accelerator name.
+                         devices="auto",
                          max_epochs=num_epochs,
-                         check_val_every_n_epoch=1,
-                         log_every_n_steps=1,
+                         check_val_every_n_epoch=num_epochs // 100,
+                         log_every_n_steps=num_epochs // 100,
+                         callbacks=callbacks,
                          **kwargs)
     start_time = time.time()
-    trainer.fit(model, train_dataloaders=train, val_dataloaders=validation)
-    print(f'time taken: {time.time() - start_time}')
+    trainer.fit(lightning_model, train_dataloaders=train_dataloader, val_dataloaders=val_dataloader)
+    print(f'Time taken for training: {time.time() - start_time}')
+    if test_dataloader is not None:
+        trainer.test(lightning_model, test_dataloaders=test_dataloader)
+    else:
+        print('Skip testing, no test dataset is provided.')
 
+    # ==================================================================================================================
+    # Construct standard error, z-value, and p-value of coefficients.
+    # ==================================================================================================================
     # current methods of computing standard deviation will corrupt the model, load weights into another model for returning.
-    state_dict = deepcopy(model.state_dict())
+    state_dict = deepcopy(lightning_model.model.state_dict())
     model_clone.load_state_dict(state_dict)
 
     # get mean of estimation.
     mean_dict = dict()
-    for k, v in model.named_parameters():
+    for k, v in lightning_model.model.named_parameters():
         mean_dict[k] = v.clone()
 
     # estimate the standard error of the model.
-    dataset_for_std = dataset_list[0]
+    dataset_for_std = dataset_train.clone()
+
     if isinstance(model, ConditionalLogitModel):
         def nll_loss(model):
             y_pred = model(dataset_for_std)
             return F.cross_entropy(y_pred, dataset_for_std.item_index, reduction='sum')
     elif isinstance(model, NestedLogitModel):
         def nll_loss(model):
             d = dataset_for_std[torch.arange(len(dataset_for_std))]
             return model.negative_log_likelihood(d, d['item'].item_index)
+    std_dict = parameter_std(model_clone, nll_loss)
 
-    std_dict = parameter_std(model, nll_loss)
-
-    # TODO: continue working here.
     print('=' * 20, 'model results', '=' * 20)
     report = list()
     for coef_name, std in std_dict.items():
         std = std.cpu().detach().numpy()
         mean = mean_dict[coef_name].cpu().detach().numpy()
         coef_name = coef_name.replace('coef_dict.', '').replace('.coef', '')
         for i in range(mean.size):
             report.append({'Coefficient': coef_name + f'_{i}',
                            'Estimation': float(mean[i]),
                            'Std. Err.': float(std[i])})
     report = pd.DataFrame(report).set_index('Coefficient')
-    print(f'Training Epochs: {num_epochs}\n')
-    print(f'Learning Rate: {learning_rate}\n')
-    print(f'Batch Size: {batch_size if batch_size != -1 else len(dataset)} out of {len(dataset)} observations in total\n')
-    print(f'Final Log-likelihood: {ll}\n')
-    print('Coefficients:\n')
-    print(report.to_markdown())
 
-    if test is not None:
-        section_print('test performance')
-        trainer.test(model, dataloaders=test)
+    # Compute z-value
+    report['z-value'] = report['Estimation'] / report['Std. Err.']
+
+    # Compute p-value (two tails).
+    report['Pr(>|z|)'] = (1 - norm.cdf(abs(report['z-value']))) * 2
+
+    # Compute significance stars
+    report['Significance'] = ''
+    report.loc[report['Pr(>|z|)'] < 0.001, 'Significance'] = '***'
+    report.loc[(report['Pr(>|z|)'] >= 0.001) & (report['Pr(>|z|)'] < 0.01), 'Significance'] = '**'
+    report.loc[(report['Pr(>|z|)'] >= 0.01) & (report['Pr(>|z|)'] < 0.05), 'Significance'] = '*'
+
+    # Compute log-likelihood on the final model on all splits of datasets.
+    lightning_model.model.to(device)
+    is_nested = isinstance(lightning_model.model, NestedLogitModel)
+
+    train_ll = - lightning_model.model.negative_log_likelihood(dataset_train.datasets if is_nested else dataset_train,
+                                                               dataset_train.item_index).detach().item()
+
+    if dataset_val is not None:
+        val_ll = - lightning_model.model.negative_log_likelihood(dataset_val.datasets if is_nested else dataset_val,
+                                                                 dataset_val.item_index).detach().item()
+    else:
+        val_ll = 'N/A'
+
+    if dataset_test is not None:
+        test_ll = - lightning_model.model.negative_log_likelihood(dataset_test.datasets if is_nested else dataset_test,
+                                                                  dataset_test.item_index).detach().item()
     else:
-        print('No test dataset provided.')
-    return model
+        test_ll = 'N/A'
+
+    print(f'Log-likelihood: [Training] {train_ll}, [Validation] {val_ll}, [Test] {test_ll}\n')
+    print(report.to_markdown())
+    print("Significance codes: 0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
+    return model
```

### Comparing `torch_choice-1.0.1/torch_choice/utils/std.py` & `torch_choice-1.0.2/torch_choice/utils/std.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.1/torch_choice.egg-info/SOURCES.txt` & `torch_choice-1.0.2/torch_choice.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 torch_choice/__init__.py
 torch_choice.egg-info/PKG-INFO
 torch_choice.egg-info/SOURCES.txt
 torch_choice.egg-info/dependency_links.txt
 torch_choice.egg-info/top_level.txt
 torch_choice/data/__init__.py
 torch_choice/data/choice_dataset.py
+torch_choice/data/example_datasets.py
 torch_choice/data/joint_dataset.py
 torch_choice/data/utils.py
 torch_choice/model/__init__.py
 torch_choice/model/coefficient.py
 torch_choice/model/conditional_logit_model.py
 torch_choice/model/formula_parser.py
 torch_choice/model/nested_logit_model.py
 torch_choice/utils/__init__.py
 torch_choice/utils/easy_data_wrapper.py
 torch_choice/utils/run_helper.py
-torch_choice/utils/run_helper_temp.py
+torch_choice/utils/run_helper_lightning.py
 torch_choice/utils/std.py
```

