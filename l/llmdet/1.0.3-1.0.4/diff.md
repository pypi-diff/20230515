# Comparing `tmp/llmdet-1.0.3.tar.gz` & `tmp/llmdet-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmdet-1.0.3.tar", last modified: Thu May  4 08:44:36 2023, max compression
+gzip compressed data, was "llmdet-1.0.4.tar", last modified: Mon May 15 15:09:55 2023, max compression
```

## Comparing `llmdet-1.0.3.tar` & `llmdet-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:44:36.493380 llmdet-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-05-03 11:43:47.000000 llmdet-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3598 2023-05-04 08:44:36.493380 llmdet-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3151 2023-05-03 11:43:47.000000 llmdet-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:44:36.489380 llmdet-1.0.3/llmdet/
--rw-r--r--   0 root         (0) root         (0)     1224 2023-05-04 07:59:29.000000 llmdet-1.0.3/llmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6002 2023-05-03 11:43:48.000000 llmdet-1.0.3/llmdet/arguments.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-05-03 11:43:48.000000 llmdet-1.0.3/llmdet/classifier.py
--rw-r--r--   0 root         (0) root         (0)     7702 2023-05-04 08:43:28.000000 llmdet-1.0.3/llmdet/detector.py
--rw-r--r--   0 root         (0) root         (0)    25372 2023-05-03 11:43:48.000000 llmdet-1.0.3/llmdet/new_proxy_perplexity.py
--rw-r--r--   0 root         (0) root         (0)    16061 2023-05-03 11:43:48.000000 llmdet-1.0.3/llmdet/run_main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:44:36.489380 llmdet-1.0.3/llmdet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3598 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 08:44:36.000000 llmdet-1.0.3/llmdet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 08:44:36.493380 llmdet-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      888 2023-05-04 08:43:56.000000 llmdet-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:09:55.425925 llmdet-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-05-15 15:09:55.425925 llmdet-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3368 2023-05-15 15:01:34.000000 llmdet-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:09:55.425925 llmdet-1.0.4/llmdet/
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-05-15 15:01:34.000000 llmdet-1.0.4/llmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-05-15 15:01:34.000000 llmdet-1.0.4/llmdet/arguments.py
+-rw-r--r--   0 root         (0) root         (0)     3676 2023-05-15 15:01:34.000000 llmdet-1.0.4/llmdet/classifier.py
+-rw-r--r--   0 root         (0) root         (0)     9413 2023-05-15 15:01:34.000000 llmdet-1.0.4/llmdet/detector.py
+-rw-r--r--   0 root         (0) root         (0)    25372 2023-05-15 15:01:34.000000 llmdet-1.0.4/llmdet/new_proxy_perplexity.py
+-rw-r--r--   0 root         (0) root         (0)    20319 2023-05-15 15:01:34.000000 llmdet-1.0.4/llmdet/run_main.py
+-rw-r--r--   0 root         (0) root         (0)     3873 2023-05-15 15:01:34.000000 llmdet-1.0.4/llmdet/train_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     5289 2023-05-15 15:01:34.000000 llmdet-1.0.4/llmdet/truth_perplexity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:09:55.425925 llmdet-1.0.4/llmdet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-05-15 15:09:55.000000 llmdet-1.0.4/llmdet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-15 15:09:55.000000 llmdet-1.0.4/llmdet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 15:09:55.000000 llmdet-1.0.4/llmdet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-15 15:09:55.000000 llmdet-1.0.4/llmdet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-15 15:09:55.000000 llmdet-1.0.4/llmdet.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 15:09:55.429925 llmdet-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 15:01:34.000000 llmdet-1.0.4/setup.py
```

### Comparing `llmdet-1.0.3/LICENSE` & `llmdet-1.0.4/llmdet/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-MIT License
-
-Copyright (c) 2023 Kangxi Wu, Liang Pang, TryMore Group
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+# Copyright 2023 Kangxi Wu, Liang Pang, TryMore Group.
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+__version__ = "1.0.4"
+
+from .detector import load_probability
+from .detector import detect
```

### Comparing `llmdet-1.0.3/PKG-INFO` & `llmdet-1.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 Metadata-Version: 2.1
 Name: llmdet
-Version: 1.0.3
-Summary: LLMDet：A Large Language Models Detection Tool
+Version: 1.0.4
+Summary: LLMDet: A Large Language Models Detection Tool
 Home-page: https://github.com/cansee5/LLMDet
 Author: Kangxi Wu, Liang Pang
 Author-email: wukx0901@gmail.com
+License: UNKNOWN
+Description: # 🪬 LLMDet：A Large Language Models Detection Tool
+        
+        LLMDet is a text detection tool that can identify which generated sources the text came from (e.g. large language model or human-write). The core idea of the detection algorithm is to use the n-grams probability sampled from specified language model to calculate proxy perplexity of large language models, and use the proxy perplexity as a feature to train a text classifier.
+        
+        ### Features
+        We believe that a practical LLM detection tool needs to have the following capabilities, which is also the goal of our LLMDet.
+        
+        1. **Specificity**: Our project aims to distinguish between different large-scale language models and human-generated text. For example, LLMDet can tell you whether the text is generated by GPT-2 or OPT or a human, and give each a specific probability.
+        2. **Safty**: Our project does not need to require running large language models locally. That is, we can act as a third-party authentication agent without maintaining large language models, which may be fixed assets or sensitive information for large companies.
+        3. **Efficiency**: Our method detects very fast. This is because we don't need to infer from large language models.
+        4. **Extendibility**: Our project can easily adapt to newly proposed large language models. 
+        
+        
+        ### Installation Notes
+        A package for large language model-generated text detection tool.
+        
+        Code is compatible with Python >=3.8
+          * Fully automatic installation: `pip install llmdet`
+          * Semi-automatic installation: First download http://pypi.python.org/pypi/llmdet/ , decompress and run `python setup.py install`
+          * See `requirements.txt` for dependent python packages.
+        
+        ### Main Functions
+        
+        Currently, it is supported to determine whether the text comes from GPT-2, OPT, UniLM or Human-write.
+        
+        #### Examples
+        ```python
+        import llmdet
+        
+        llmdet.load_probability()
+        
+        text = "The actress was honoured for her role in 'The Reader' at the annual ceremony, which was held at the Royal Albert Hall. The film, which is based on the novel by the same name by Philip Roth, tells the story of a New York Times reporter who returns to his hometown to cover the death of his brother-in-law. Winslet plays his wife, with whom he has been divided since the death of their son.\nIn the film, Winslet plays the mother of the grieving brother-in-law.\nThe actress also won a Golden Globe for her role in the film at the ceremony in November.\nWinslet was also nominated for an Oscar for her role in 'The Reader'.\nThe 63-year-old Winslet was seen accepting her awards at the ceremony, where she was joined by her husband, John Krasinski, who has been nominated for best supporting actor in the film.\nWinslet and Krasinski met while"
+        
+        # Detect, `text` is a string or string list
+        result = llmdet.detect(text)
+        print(result)
+        ```
+        #### Detection Results
+        ```json
+        [{
+            'OPT': 0.5451331013247862,
+            'GPT-2': 0.4393605735865629, 
+            'UniLM': 0.012642800848279893, 
+            'T5': 0.0022592730436008556, 
+            'Bloom': 0.00025873253035729044, 
+            'GPT-neo': 0.0002520776780109571, 
+            'LLaMA': 6.0459794454546154e-05, 
+            'Human_write': 1.9576671778802474e-05, 
+            'BART': 1.3404522168622544e-05
+        }]
+        ```
+        
+        ### TODO List
+          - [ ] Extend the detection models to LLaMA, T5, Bart and Vicuna.
+          - [ ] Compress the project.
+          - [ ] Add more experimental performnce results.
+        
+        ### Citation
+        ```bibtex
+        
+        ```
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 🪬 LLMDet：A Large Language Models Detection Tool
-
-LLMDet is a text detection tool that can identify which generated sources the text came from (e.g. large language model or human-write). The core idea of the detection algorithm is to use the n-grams probability sampled from specified language model to calculate proxy perplexity of large language models, and use the proxy perplexity as a feature to train a text classifier.
-
-### Features
-We believe that a practical LLM detection tool needs to have the following capabilities, which is also the goal of our LLMDet.
-
-1. **Specificity**: Our project aims to distinguish between different large-scale language models and human-generated text. For example, LLMDet can tell you whether the text is generated by GPT-2 or OPT or a human, and give each a specific probability.
-2. **Safty**: Our project does not need to require running large language models locally. That is, we can act as a third-party authentication agent without maintaining large language models, which may be fixed assets or sensitive information for large companies.
-3. **Efficiency**: Our method detects very fast. This is because we don't need to infer from large language models.
-4. **Extendibility**: Our project can easily adapt to newly proposed large language models. 
-
-
-### Installation Notes
-A package for large language model-generated text detection tool.
-
-Code is compatible with Python >=3.8
-  * Fully automatic installation: `pip install llmdet`
-  * Semi-automatic installation: First download http://pypi.python.org/pypi/llmdet/ , decompress and run `python setup.py install`
-  * See `requirements.txt` for dependent python packages.
-
-### Main Functions
-
-Currently, it is supported to determine whether the text comes from GPT-2, OPT, UniLM or Human-write.
-
-#### Examples
-```python
-from llmdet import detect
-
-text = "The actress was honoured for her role in 'The Reader' at the annual ceremony, which was held at the Royal Albert Hall. The film, which is based on the novel by the same name by Philip Roth, tells the story of a New York Times reporter who returns to his hometown to cover the death of his brother-in-law. Winslet plays his wife, with whom he has been divided since the death of their son.\nIn the film, Winslet plays the mother of the grieving brother-in-law.\nThe actress also won a Golden Globe for her role in the film at the ceremony in November.\nWinslet was also nominated for an Oscar for her role in 'The Reader'.\nThe 63-year-old Winslet was seen accepting her awards at the ceremony, where she was joined by her husband, John Krasinski, who has been nominated for best supporting actor in the film.\nWinslet and Krasinski met while"
-
-# Detect, `text` is a string or string list
-result = detect(text)
-print(result)
-```
-#### Detection Results
-```json
-[{
- "Human_write": 0.00034990044262862392 , 
- "GPT-2": 0.003904839900808308, 
- "OPT": 0.6458330377453642, 
- "UniLM": 0.34991221792754135
-}]
-```
-
-### TODO List
-  - [ ] Extend the detection models to LLaMA, T5, Bart and Vicuna.
-  - [ ] Compress the project.
-  - [ ] Add more experimental performnce results.
-
-### Citation
-```bibtex
-
-```
-
-
```

### Comparing `llmdet-1.0.3/README.md` & `llmdet-1.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -21,29 +21,36 @@
 
 ### Main Functions
 
 Currently, it is supported to determine whether the text comes from GPT-2, OPT, UniLM or Human-write.
 
 #### Examples
 ```python
-from llmdet import detect
+import llmdet
+
+llmdet.load_probability()
 
 text = "The actress was honoured for her role in 'The Reader' at the annual ceremony, which was held at the Royal Albert Hall. The film, which is based on the novel by the same name by Philip Roth, tells the story of a New York Times reporter who returns to his hometown to cover the death of his brother-in-law. Winslet plays his wife, with whom he has been divided since the death of their son.\nIn the film, Winslet plays the mother of the grieving brother-in-law.\nThe actress also won a Golden Globe for her role in the film at the ceremony in November.\nWinslet was also nominated for an Oscar for her role in 'The Reader'.\nThe 63-year-old Winslet was seen accepting her awards at the ceremony, where she was joined by her husband, John Krasinski, who has been nominated for best supporting actor in the film.\nWinslet and Krasinski met while"
 
 # Detect, `text` is a string or string list
-result = detect(text)
+result = llmdet.detect(text)
 print(result)
 ```
 #### Detection Results
 ```json
 [{
- "Human_write": 0.00034990044262862392 , 
- "GPT-2": 0.003904839900808308, 
- "OPT": 0.6458330377453642, 
- "UniLM": 0.34991221792754135
+    'OPT': 0.5451331013247862,
+    'GPT-2': 0.4393605735865629, 
+    'UniLM': 0.012642800848279893, 
+    'T5': 0.0022592730436008556, 
+    'Bloom': 0.00025873253035729044, 
+    'GPT-neo': 0.0002520776780109571, 
+    'LLaMA': 6.0459794454546154e-05, 
+    'Human_write': 1.9576671778802474e-05, 
+    'BART': 1.3404522168622544e-05
 }]
 ```
 
 ### TODO List
   - [ ] Extend the detection models to LLaMA, T5, Bart and Vicuna.
   - [ ] Compress the project.
   - [ ] Add more experimental performnce results.
```

### Comparing `llmdet-1.0.3/llmdet/arguments.py` & `llmdet-1.0.4/llmdet/arguments.py`

 * *Files identical despite different names*

### Comparing `llmdet-1.0.3/llmdet/classifier.py` & `llmdet-1.0.4/llmdet/classifier.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from lightgbm import LGBMClassifier, Booster
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import accuracy_score
 from sklearn.metrics import accuracy_score, f1_score, precision_recall_fscore_support
 import json
 import numpy as np
+import torch
 
-def construct_data(perplexity_file):
+def construct_data():
+    model_name = ["gpt2", "opt", "unilm", "llama", "bart", "t5", "bloom", "neo", "vicuna", "gpt2_large", "opt_3b"]
+    # model_name = ["gpt2", "opt", "unilm"]
+    labels_to_number = {"human": 0, "gpt2": 1, "opt": 2, "unilm": 3, "llama": 4, "bart": 5, "t5": 6, "bloom": 7,"neo": 8, "vicuna":9}
+    # labels_to_number = {"human": 0, "gpt2": 1, "opt": 2, "unilm": 3}
     perplexity = []
-    label = []
-    with open(perplexity_file, "r", encoding="utf-8") as f:
-        for line in f:
-            try:
-                data = json.loads(line)
-                for i, j in data.items():
-                    perplexity.append(j)
-                    if i == "human_write":
-                        label.append(0)
-                    elif i == "gpt2":
-                        label.append(1)
-                    elif i == "opt":
-                        label.append(2)
-                    elif i == "unilm":
-                        label.append(3)
-            except Exception as e:
-                print(e, line)
-
+    for model in model_name:
+        perplexity_file = f'result/{model}.json'
+        model_perplexity = []
+        label = []
+        with open(perplexity_file, "r", encoding="utf-8") as f:
+            for line in f:
+                try:
+                    data = json.loads(line)
+                    for i, j in data.items():
+                        if i in labels_to_number.keys():
+                            model_perplexity.append(j)
+                            label.append(labels_to_number[i])
+                except Exception as e:
+                    print(e, line)
+        perplexity.append(model_perplexity)
     return perplexity, label
 
 def LightGBM_Classification(X, y, n):
     # Load train dataset
     X = np.array(X)
     y = np.array(y)
-    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=12343)
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=12343)
 
     model = LGBMClassifier(
         max_depth=3,
         learning_rate=0.1,
         n_estimators=200,
         objective='multiclass',
         num_class=n,
@@ -45,36 +47,52 @@
         colsample_bytree=0.8,
         reg_alpha=0,
         reg_lambda=1,
         seed=0)
 
     model.fit(X_train, y_train, eval_set=[(X_train, y_train), (X_test, y_test)], verbose=100, early_stopping_rounds=50)
 
+    y_pred = model.predict(X_test)
+    # y_pred = [np.argmax(i) for i in y_pred]
+    p_class, r_class, f_class, support_micro = precision_recall_fscore_support(y_test, y_pred, labels=[i for i in range(10)])
+    print(p_class, r_class)
+    print(f_class)
     # Save model
-    model.booster_.save_model("LightGBM_model.txt")
+    model.booster_.save_model("nine_LightGBM_model.txt")
 
     return X_test,  y_test
 
 if __name__ == "__main__":
-    GPT_perplexity, label_1 = construct_data("new_gpt_ppl.json")
-    OPT_perplexity, label_2 = construct_data("new_opt_ppl.json")
-    UniLM_perplexity, label_3 = construct_data("new_unilm_ppl.json")
-    perplexity = [[i, j, k] for i, j, k in zip(GPT_perplexity, OPT_perplexity, UniLM_perplexity)]
-
-    # Ground truth label
-    ground_label = []
-    for i, j, k in zip(label_1, label_2, label_3):
-        if i == j and i == k and j == k:
-            ground_label.append(i)
+    perplexity, label = construct_data()
+    number = len(perplexity)
+    lenght = len(label)
+    perplexity = [[perplexity[i][j] for i in range(number)] for j in range(lenght)]
+
 
     # Train classification model and return test data
-    X_test, y_test = LightGBM_Classification(perplexity, ground_label, 4)
+    X_test, y_test = LightGBM_Classification(perplexity, label, 10)
+    for i in range(len(y_test)):
+        if y_test[i] == 9:
+            y_test[i] = 4
 
     # Load trained model
-    model = Booster(model_file='LightGBM_model.txt')
+    model = Booster(model_file='nine_LightGBM_model.txt')
     # Make predictions on the test setMake predictions on the test set
     y_pred = model.predict(X_test)
+    sum_num = len(y_test)
+    R2 = 0
+    for i in range(sum_num):
+        values, indics = torch.topk(torch.tensor(y_pred[i]), 3, -1)
+        if y_test[i] in indics:
+            R2 += 1
+    R2 = R2/sum_num
     y_pred = [np.argmax(i) for i in y_pred]
+    for i in range(len(y_pred)):
+        if y_pred[i] == 9:
+            y_pred[i] = 4
     # Calculate accuracy, recall, f1 value
-    p_class, r_class, f_class, support_micro = precision_recall_fscore_support(y_test, y_pred, labels=[i for i in range(4)])
+    p_class, r_class, f_class, support_micro = precision_recall_fscore_support(y_test, y_pred, labels=[i for i in range(9)])
+    print(p_class, r_class)
     print(f_class)
+    print(R2)
 
+    np.savez("matrix.npz", y_test=np.array(y_test), y_pred=np.array(y_pred))
```

### Comparing `llmdet-1.0.3/llmdet/detector.py` & `llmdet-1.0.4/llmdet/detector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import numpy as np
 import datasets
 from tqdm import tqdm
 import math
 import json
-from transformers import AutoTokenizer
+from transformers import AutoTokenizer,  LlamaTokenizer, BartTokenizer, T5Tokenizer
 from unilm import UniLMTokenizer
 from lightgbm import Booster
 
 
 def load_probability():
     dm = datasets.DownloadManager()
-    files = dm.download_and_extract('https://huggingface.co/datasets/wukx/n-grams_sample_probability/resolve/main/new_n_grams.zip')
-    n_grams = np.load(f'{files}/new_n_grams.npz' , allow_pickle=True)
-    global gpt_n_grams_probability, opt_n_grams_probability, unilm_n_grams_probability
-    gpt_n_grams_probability = n_grams["gpt"]
-    opt_n_grams_probability = n_grams["opt"]
-    unilm_n_grams_probability = n_grams["unilm"]
+    files = dm.download_and_extract('https://huggingface.co/datasets/TryMore/n_grams_probability/resolve/main/n-grams_probability.tar.gz')
+    model = ["gpt2", "opt", "unilm", "llama", "bart", "t5", "bloom", "neo", "vicuna" , "gpt2_large", "opt_3b"]
+    global_vars = globals()
+    for item in model:
+        n_grams = np.load(f'{files}/npz/{item}.npz', allow_pickle=True)
+        global_vars[item] = n_grams["t5"]
 
 # Calculate the perplexity of text.
 def perplexity(text_set_token_ids, n_grams_probability, vocab_size):
 
     # Calculate proxy perplexity value for test text set
     test_perplexity = []
 
@@ -64,15 +64,15 @@
                 else:
                     top_k = len(n_grams_probability[0][tuple([text_token_ids[i]])])
                     sum_probs = sum(n_grams_probability[1][tuple([text_token_ids[i]])])
                     if (1 - sum_probs) > 0:
                         ppl = ppl + math.log2((1 - sum_probs) / (vocab_size - top_k))
                 number_2_grams = number_2_grams + 1
 
-        perplexity = round(ppl / (number_2_grams + number_3_grams + number_4_grams + 1), 2)
+        perplexity = ppl / (number_2_grams + number_3_grams + number_4_grams + 1)
         test_perplexity.append(-perplexity)
 
     return test_perplexity
 
 # Detect function
 def detect(text):
     # Determine whether the input is a single text or a collection of text.
@@ -90,23 +90,40 @@
         raise ValueError(
             "The type of `text` which you input is not a string or list. "
             "Please enter the correct data type for `text`."
         )
     dm = datasets.DownloadManager()
     # files = dm.download_and_extract('https://huggingface.co/datasets/wukx/n-grams_sample_probability/resolve/main/n_grams.zip')
 
-    model_information = [{"model_name": "gpt2", "vocab_size": 50265, "model_probability": "gpt_n_grams_probability"},
-                         {"model_name": "facebook/opt-1.3b", "vocab_size": 50257, "model_probability": "opt_n_grams_probability"},
-                         {"model_name": "microsoft/unilm-base-cased", "vocab_size": 28996, "model_probability": "unilm_n_grams_probability"}]
+    model_information = [{"model_name": "gpt2", "vocab_size": 50265, "model_probability": "gpt2"},
+                         {"model_name": "facebook/opt-1.3b", "vocab_size": 50257, "model_probability": "opt"},
+                         {"model_name": "microsoft/unilm-base-cased", "vocab_size": 28996, "model_probability": "unilm"},
+                         {"model_name": "decapoda-research/llama-7b-hf", "vocab_size": 32000, "model_probability": "llama"},
+                         {"model_name": "facebook/bart-base", "vocab_size": 50265, "model_probability": "bart"},
+                         {"model_name": "google/flan-t5-base", "vocab_size": 32128, "model_probability": "t5"},
+                         {"model_name": "bigscience/bloom-560m", "vocab_size": 250880, "model_probability": "bloom"},
+                         {"model_name": "EleutherAI/gpt-neo-2.7B", "vocab_size": 50257, "model_probability": "neo"},
+                         {"model_name": "lmsys/vicuna-7b-delta-v1.1", "vocab_size": 32000, "model_probability": "vicuna"},
+                         {"model_name": "gpt2-large", "vocab_size": 50265, "model_probability": "gpt2_large"},
+                         {"model_name": "facebook/opt-2.7b", "vocab_size": 50257, "model_probability": "opt_3b"}]
+    #
+    # labels_to_number = {"Human_write": 0, "GPT-2": 1, "OPT": 2, "UniLM": 3, "llama": 4, "bart": 5, "t5": 6, "bloom": 7,
+    #                     "neo": 8}
 
     # Calculate the proxy perplexity
     perplexity_result = []
     for model in model_information:
         if any([(model_type in model["model_name"]) for model_type in ["unilm"]]):
             tokenizer = UniLMTokenizer.from_pretrained(model["model_name"])
+        elif any([(model_type in model["model_name"]) for model_type in ["llama", "vicuna"]]):
+            tokenizer = LlamaTokenizer.from_pretrained(model["model_name"])
+        elif any([(model_type in model["model_name"]) for model_type in ["t5"]]):
+            tokenizer = T5Tokenizer.from_pretrained(model["model_name"])
+        elif any([(model_type in model["model_name"]) for model_type in ["bart"]]):
+            tokenizer = BartTokenizer.from_pretrained(model["model_name"])
         else:
             tokenizer = AutoTokenizer.from_pretrained(model["model_name"])
 
         text_token_ids = []
         for text in test_text:
             if any([(model_type in model["model_name"]) for model_type in ["gpt"]]):
                 text_tokenize = tokenizer.tokenize(text, truncation=True)
@@ -120,18 +137,18 @@
         else:
             raise ValueError(
                 "The {} does not exist, please load n-grams probability!".format(model["model_probability"])
             )
 
     # The input features of classiffier
     features = np.stack([perplexity_result[i] for i in range(len(perplexity_result))], axis=1)
-    print(features)
 
     # Load classiffier model
-    model_files = dm.download_and_extract(
-        'https://huggingface.co/datasets/wukx/n-grams_sample_probability/resolve/main/LightGBM_model.zip')
-    model = Booster(model_file=f'{model_files}/LightGBM_model.txt')
+    model_files = dm.download_and_extract('https://huggingface.co/datasets/TryMore/n_grams_probability/resolve/main/LightGBM_model.zip')
+    model = Booster(model_file=f'{model_files}/nine_LightGBM_model.txt')
     y_pred = model.predict(features)
-    label = ["Human_write", "GPT-2", "OPT", "UniLM"]
+    label = ["Human_write", "GPT-2", "OPT", "UniLM", "LLaMA", "BART", "T5", "Bloom", "GPT-neo"]
     test_result = [{label[i]: y_pred[j][i] for i in range(len(label))} for j in range(len(y_pred))]
+    for i in range(len(test_result)):
+        test_result[i] = dict(sorted(test_result[i].items(), key=lambda x: x[1], reverse=True))
 
     return test_result
```

### Comparing `llmdet-1.0.3/llmdet/new_proxy_perplexity.py` & `llmdet-1.0.4/llmdet/new_proxy_perplexity.py`

 * *Files identical despite different names*

### Comparing `llmdet-1.0.3/llmdet/run_main.py` & `llmdet-1.0.4/llmdet/run_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import os
 import json
-import argparse
 from functools import partial
-from multiprocessing import Pool  # 多线程并行
 import tqdm
 import torch
+import torch.nn as nn
 import pickle
 import torch.nn.functional as F
 from nltk import ngrams
 from collections import Counter
 import math
 import random
+import numpy as np
 
-# mutil-GPU
-from torch.nn.parallel import DistributedDataParallel as DDP
-import torch.distributed as dist
 
-from transformers import HfArgumentParser
 from transformers import AutoTokenizer, LlamaTokenizer, AutoModelForSeq2SeqLM, AutoModelForCausalLM, LlamaForCausalLM
-
 from unilm import UniLMTokenizer, UniLMForConditionalGeneration
+from transformers import BartForConditionalGeneration, BartTokenizer, T5Tokenizer, T5ForConditionalGeneration
 
 from arguments import parse_args
 
 # Load and return model and tokenzier
 def load_model(args):
     # Load corresponding model and tokenizer according to  model name ot path
-    if args.is_seq2seq_model:
-        tokenizer = AutoTokenizer.from_pretrained(args.model_name_or_path)
-        model = AutoModelForSeq2SeqLM.from_pretrained(args.model_name_or_path)
+    if args.is_t5:
+        tokenizer = T5Tokenizer.from_pretrained(args.model_name_or_path)
+        model = T5ForConditionalGeneration.from_pretrained(args.model_name_or_path)
     elif args.is_decoder_only_model:
         tokenizer = AutoTokenizer.from_pretrained(args.model_name_or_path)
         model = AutoModelForCausalLM.from_pretrained(args.model_name_or_path)
-    elif args.is_llama:
+    elif args.is_llama or args.is_vicuna:
         tokenizer = LlamaTokenizer.from_pretrained(args.model_name_or_path)
         model = LlamaForCausalLM.from_pretrained(args.model_name_or_path, torch_dtype=torch.float16)
     elif args.is_unilm:
         tokenizer = UniLMTokenizer.from_pretrained(args.model_name_or_path)
         model = UniLMForConditionalGeneration.from_pretrained(args.model_name_or_path)
+    elif args.is_bart:
+        tokenizer = BartTokenizer.from_pretrained(args.model_name_or_path)
+        model = BartForConditionalGeneration.from_pretrained(args.model_name_or_path)
     else:
         raise ValueError(f"Unknown model type: {args.model_name_or_path}")
 
     if args.use_gpu:
         device = "cuda" if torch.cuda.is_available() else "cpu"
         model = model.to(device)
     else:
@@ -83,14 +82,36 @@
     # need to isolate the newly generated tokens
     output = output[:, tokd_input["input_ids"].shape[-1]:]
 
     decoded_output_text = tokenizer.batch_decode(output, skip_special_tokens=True)[0]
 
     return decoded_output_text
 
+def generate_seq2seq(input, args, tokenizer, model, device):
+    tokenizer_input = tokenizer(input, return_tensors="pt", add_special_tokens=True,
+                           max_length=args.prompt_max_length).to(device)
+    tokenizer_input_ids = tokenizer_input["input_ids"]
+    model = model.to(device)
+
+    outputs = model.generate(
+        inputs=tokenizer_input_ids,
+        max_length=args.max_new_tokens,
+        min_length=300,
+        num_return_sequences=1,
+        do_sample=True,
+        num_beams=args.n_beams,
+        temperature=args.sampling_temp,
+    )
+
+    # need to isolate the newly generated tokens
+    output = outputs[:, tokenizer_input_ids.shape[-1]:]
+    decoded_output_text = tokenizer.batch_decode(output, skip_special_tokens=True)[0]
+
+    return decoded_output_text
+
 # Used to count the top k n-grams  in a given text set
 def count_n_grams(text_set, n, top_k, tokenizer):
     n_grams = []
     for text in text_set:
         text_n_grams = ngrams(tokenizer.convert_tokens_to_ids(tokenizer.tokenize(text)), n)
         n_grams.extend(text_n_grams)
 
@@ -99,15 +120,16 @@
 
     if len(n_grams) < top_k:
         return n_grams
     else:
         return n_grams[:top_k]
 
 def next_token_probs(n_grams, top_k, model, tokenizer, device):
-    grams_probs = {}
+    grams_keys = {}
+    grams_probability = {}
     for i in tqdm.tqdm(range(len(n_grams))):
         prompt = tokenizer.decode(n_grams[i])
         tokd_input = tokenizer.encode(prompt, return_tensors="pt").to(device)
 
         model.to(device)
         with torch.no_grad():
             outputs = model(tokd_input)
@@ -115,19 +137,45 @@
 
         logits = predictions[0, -1, :]
 
         # probability
         probs = F.softmax(logits, dim=0)
 
         values, indices = torch.topk(probs, top_k, -1)
-        indices = indices.tolist()
-        values = values.tolist()
-        grams_probs[str(n_grams[i])] = dict(zip(indices, values))
+        indices = np.array(indices.cpu()).astype(np.uint16)
+        values = np.array(values.cpu()).astype(np.float16)
+        grams_keys[tuple(n_grams[i])] = indices
+        grams_probability[tuple(n_grams[i])] = values
+
+    return grams_keys, grams_probability
+
+def t5_next_token_probs(n_grams, top_k, model, tokenizer, device):
+    grams_keys = {}
+    grams_probability = {}
+    for i in tqdm.tqdm(range(len(n_grams))):
+        prompt = tokenizer.decode(n_grams[i])
+        tokd_input = tokenizer(prompt, return_tensors="pt").input_ids.to(device)
+        decoder_input_ids = torch.tensor([[0]]).to(device)
+        model.to(device)
+        with torch.no_grad():
+            outputs = model(tokd_input, decoder_input_ids=decoder_input_ids)
+            predictions = outputs.logits
+
+        logits = predictions[0, -1, :]
+
+        # probability
+        probs = F.softmax(logits, dim=0)
+
+        values, indices = torch.topk(probs, top_k, -1)
+        indices = np.array(indices.cpu()).astype(np.uint16)
+        values = np.array(values.cpu()).astype(np.float16)
+        grams_keys[tuple(n_grams[i])] = indices
+        grams_probability[tuple(n_grams[i])] = values
 
-    return grams_probs
+    return grams_keys, grams_probability
 
 # construct test text set with original text set and generated test set
 def construct_test_text_set(original_text_set, generated_test_set, args):
     test_set = []
     for i in generated_test_set:
         if i != "":
             test_set.append({"text": i, "label": args.model_name})
@@ -194,172 +242,208 @@
                     number_2_grams = number_2_grams + 1
             ppl = round(ppl / (number_2_grams + number_3_grams + number_4_grams + number_5_grams + 1), 2)
             ppl_result[label] = -ppl
             test_ppl.append(ppl_result)
     return test_ppl
 
 def main(args):
-    args.is_seq2seq_model = any([(model_type in args.model_name_or_path) for model_type in ["t5", "T0"]])
+    args.is_t5 = any([(model_type in args.model_name_or_path) for model_type in ["t5"]])
     args.is_decoder_only_model = any([(model_type in args.model_name_or_path) for model_type in ["gpt", "opt", "bloom"]])
     args.is_gpt = any([(model_type in args.model_name_or_path) for model_type in ["gpt"]])
     args.is_opt = any([(model_type in args.model_name_or_path) for model_type in ["opt"]])
     args.is_unilm = any([(model_type in args.model_name_or_path) for model_type in ["unilm"]])
     args.is_llama = any([(model_type in args.model_name_or_path) for model_type in ["llama"]])
+    args.is_vicuna = any([(model_type in args.model_name_or_path) for model_type in ["vicuna"]])
+    args.is_bart = any([(model_type in args.model_name_or_path) for model_type in ["bart"]])
+    args.is_bloom = any([(model_type in args.model_name_or_path) for model_type in ["bloom"]])
 
     if args.is_gpt:
         args.model_name = "gpt"
         args.vocab_length = 50257
     elif args.is_opt:
         args.model_name = "opt"
         args.vocab_length = 50265
     elif args.is_unilm:
         args.model_name = "unilm"
         args.vocab_length = 28996
     elif args.is_llama:
         args.model_name = "llama"
         args.vocab_length = 32000
+    elif args.is_vicuna:
+        args.model_name = "vicuna"
+        args.vocab_length = 32000
+    elif args.is_bart:
+        args.model_name = "bart"
+        args.vocab_length = 50265
+    elif args.is_t5:
+        args.model_name = "t5"
+        args.vocab_length = 32128
+    elif args.is_bloom:
+        args.model_name = "bloom"
+        args.vocab_length = 250880
+
+    # if args.prompt_file is not None:
+    #     extension = args.prompt_file.split(".")[-1]
+    #     assert extension in ["csv", "json", "tsv"], "`prompt_file` should be a csv or a json file."
+    #
+    # # load prompt set
+    # prompt = []
+    # with open(args.prompt_file, 'r', encoding='utf-8') as f:
+    #     for line in f:
+    #         try:
+    #             text = json.loads(line)
+    #             prompt.append(text)
+    #
+    #         except Exception as e:
+    #             print(e, line)
+    # prompt = prompt[args.prompt_set * args.n_generate_text:(args.prompt_set + 1) * args.n_generate_text]
 
-    if args.prompt_file is not None:
-        extension = args.prompt_file.split(".")[-1]
-        assert extension in ["csv", "json", "tsv"], "`prompt_file` should be a csv or a json file."
+    tokenizer, model, device = load_model(args)
 
-    # load prompt set
-    prompt = []
+    # generate_fn = partial(generate, args=args, tokenizer=tokenizer, model=model, device=device)
+
+    # out_dir = os.path.join("result", args.model_name, str(args.prompt_set))
+    # if not os.path.exists(out_dir):
+    #     os.makedirs(out_dir)
+    #
+    # save_state = os.path.join(out_dir, args.save_state)
+    #
+    # # check if there is a saved state
+    # if os.path.exists(save_state):
+    #     try:
+    #         with open(save_state, 'rb') as f:
+    #             state = pickle.load(f)
+    #             generation_text = state['generation_text']
+    #             start_batch = state['state_batch'] + 1
+    #
+    #     except Exception as e:
+    #         print(e)
+    #
+    # else:
+    #     generation_text = []
+    #     start_batch = 0
+    #
+    # for batch in tqdm.tqdm(range(start_batch, args.n_generate_text // args.batch_size)):
+    #     input = prompt[batch * args.batch_size:(batch + 1) * args.batch_size]
+    #     batch_text = []
+    #     for idx in range(len(input)):
+    #         # batch_text.append(generate_fn(input[idx]))
+    #         generated_text = generate_seq2seq(input[idx], args, tokenizer, model, device)
+    #         batch_text.append(generated_text)
+    #
+    #     # save state after each batch
+    #     generation_text.extend(batch_text)
+    #     if save_state:
+    #         state = {
+    #             "generation_text": generation_text,
+    #             "state_batch": batch
+    #         }
+    #         with open(save_state, "wb") as f:
+    #             pickle.dump(state, f)
+    #
+    # generation_text_file = os.path.join(out_dir, args.generated_text_file)
+    # with open(generation_text_file, "w", encoding='utf-8') as f:
+    #     for text in generation_text:
+    #         f.write(json.dumps(text, ensure_ascii=False))
+    #         f.write('\n')
+
+    # save final state
+    # if save_state:
+    #     state = {
+    #         'generation_text': generation_text,
+    #         'state_batch': args.n_generate_text // args.batch_size,
+    #     }
+    #     with open(save_state, 'wb') as f:
+    #         pickle.dump(state, f)
+
+    statistics_text_set = []
     with open(args.prompt_file, 'r', encoding='utf-8') as f:
         for line in f:
             try:
                 text = json.loads(line)
-                prompt.append(text)
+                statistics_text_set.append(text)
 
             except Exception as e:
                 print(e, line)
-
-    # load model and tokenizer
-    torch.cuda.set_device(args.local_rank)
-    dist.init_process_group(backend='nccl')
-    tokenizer, model, device = load_model(args)
-    model = DDP(model)
-
-    generate_fn = partial(generate, args=args, tokenizer=tokenizer, model=model, device=device)
-    generation_text = []
-
-    # check if there is a saved state
-    if args.save_state:
-        try:
-            with open(args.save_state, 'rb') as f:
-                state = pickle.load(f)
-                generation_text = state['generation_text']
-                start_batch = state['start_batch']
-
-        except Exception as e:
-            print(e)
-
-    else:
-        start_batch = 0
-
-    for batch in tqdm.tqdm(range(start_batch, args.n_generate_text // (args.batch_size * dist.get_world_size()))):
-        input = prompt[batch * args.batch_size * dist.get_world_size():(batch + 1) * args.batch_size * dist.get_world_size()]
-        for idx in range(len(input)):
-            generation_text.append(generate_fn(input[idx]))
-
-        # save state after each batch
-        if args.save_state:
-            state = {
-                "generateion_text": generation_text,
-                "state_batch": batch - 1
-            }
-            with open(args.save_state, "wb") as f:
-                pickle.dump(state, f)
-
-    out_dir = os.path.join("result", args.model_name)
-    if not os.path.exists(out_dir):
-        os.makedirs(out_dir)
-
-    generation_text_file = os.path.join(out_dir, args.generated_text_file)
-    with open(generation_text_file, "w", encoding='utf-8') as f:
-        for text in generation_text:
-            f.write(json.dumps(text, ensure_ascii=False))
-            f.write('\n')
-
-    # save final state
-    if args.save_state:
-        state = {
-            'generation_text': generation_text,
-            'start_batch': args.n_generate_text // args.batch_size,
-        }
-        with open(args.save_state, 'wb') as f:
-            pickle.dump(state, f)
-
-    statistics_text_set = generation_text[:int(args.n_generate_text * 0.8)]
-    generation_test_text_set = generation_text[int(args.n_generate_text * 0.8):args.n_generate_text]
-
+    # statistics_text_set = generation_text[:int(args.n_generate_text * 0.8)]
+    # generation_test_text_set = generation_text[int(args.n_generate_text * 0.8):args.n_generate_text]
+    #
     # count the number of n-grams
     one_grams = count_n_grams(statistics_text_set, 1, args.n_one_grams, tokenizer)
     two_grams = count_n_grams(statistics_text_set, 2, args.n_two_grams, tokenizer)
     three_grams = count_n_grams(statistics_text_set, 3, args.n_three_grams, tokenizer)
-    four_grams = count_n_grams(statistics_text_set, 4, args.n_four_grams, tokenizer)
-
-    # samples the next token probability of n-grams
-    two_grams_probs = next_token_probs(one_grams, args.two_grams_top_k, model, tokenizer, device)
-    three_grams_probs = next_token_probs(two_grams, args.three_grams_top_k, model, tokenizer, device)
-    four_grams_probs = next_token_probs(three_grams, args.four_grams_top_k, model, tokenizer, device)
-    five_grams_probs = next_token_probs(four_grams, args.five_grams_top_k, model, tokenizer, device)
-
-    two_grams_probs_file = os.path.join(out_dir, args.two_grams_probs_file)
-    with open(two_grams_probs_file, 'w', encoding='utf-8') as f:
-        f.write(json.dumps(two_grams_probs, ensure_ascii=False))
-
-    three_grams_probs_file = os.path.join(out_dir, args.three_grams_probs_file)
-    with open(three_grams_probs_file, 'w', encoding='utf-8') as f:
-        f.write(json.dumps(three_grams_probs, ensure_ascii=False))
-
-    four_grams_probs_file = os.path.join(out_dir, args.four_grams_probs_file)
-    with open(four_grams_probs_file, 'w', encoding='utf-8') as f:
-        f.write(json.dumps(four_grams_probs, ensure_ascii=False))
-
-    five_grams_probs_file = os.path.join(out_dir, args.five_grams_probs_file)
-    with open(five_grams_probs_file, 'w', encoding='utf-8') as f:
-        f.write(json.dumps(five_grams_probs, ensure_ascii=False))
-
-    original_text_set = []
-    with open(args.original_test_file, 'r', encoding="utf-8") as f:
-        for line in f:
-            try:
-                text = json.loads(line)
-                original_text_set.append(text)
-            except Exception as e:
-                print(e, line)
-
-    test_set = construct_test_text_set(original_text_set, generation_test_text_set, args)
+    # four_grams = count_n_grams(statistics_text_set, 4, args.n_four_grams, tokenizer)
 
-    new_test_file = os.path.join(out_dir, args.new_test_file)
-    with open(new_test_file, "w", encoding='utf-8') as f:
-        for text in test_set:
-            f.write(json.dumps(text, ensure_ascii=False))
-            f.write('\n')
-
-    test_text_tokenize_ids = []
-    for i in tqdm.tqdm(range(len(test_set))):
-        tokenize_ids = {}
-        if args.is_gpt:
-            text_tokenize = tokenizer.tokenize(test_set[i]["text"], truncation=True)
-        else:
-            text_tokenize = tokenizer.tokenize(test_set[i]["text"])
-        tokenize_ids[text[i]["label"]] = tokenizer.convert_tokens_to_ids(text_tokenize)
-        # tokens to token_ids
-        test_text_tokenize_ids.append(tokenize_ids)
-
-    test_ppl = proxy_perplexity(test_text_tokenize_ids, args, two_grams_probs, three_grams_probs, four_grams_probs, five_grams_probs)
-
-    test_ppl_file = os.path.join(out_dir, args.test_ppl_file)
-    with open(test_ppl_file, "w", encoding='utf-8') as f:
-        for ppl in test_ppl:
-            f.write(json.dumps(ppl, ensure_ascii=False))
-            f.write('\n')
+    if args.is_t5:
+        # samples the next token probability of n-grams
+        two_grams_keys, two_grams_probs = t5_next_token_probs(one_grams, args.two_grams_top_k, model, tokenizer, device)
+        three_grams_keys, three_grams_probs = t5_next_token_probs(two_grams, args.three_grams_top_k, model, tokenizer, device)
+        four_grams_keys, four_grams_probs = t5_next_token_probs(three_grams, args.four_grams_top_k, model, tokenizer, device)
+        # five_grams_probs = t5_next_token_probs(four_grams, args.five_grams_top_k, model, tokenizer, device)
+    else:
+        # samples the next token probability of n-grams
+        two_grams_keys, two_grams_probs = next_token_probs(one_grams, args.two_grams_top_k, model, tokenizer, device)
+        three_grams_keys, three_grams_probs = next_token_probs(two_grams, args.three_grams_top_k, model, tokenizer, device)
+        four_grams_keys, four_grams_probs = next_token_probs(three_grams, args.four_grams_top_k, model, tokenizer, device)
+        # five_grams_probs = next_token_probs(four_grams, args.five_grams_top_k, model, tokenizer, device)
+
+    t5 = [two_grams_keys, two_grams_probs, three_grams_keys, three_grams_probs, four_grams_keys, four_grams_probs]
+    np.savez(args.original_test_file, t5=t5)
+    # two_grams_probs_file = os.path.join(out_dir, args.two_grams_probs_file)
+    # with open(two_grams_probs_file, 'w', encoding='utf-8') as f:
+    #     f.write(json.dumps(two_grams_probs, ensure_ascii=False))
+    #
+    # three_grams_probs_file = os.path.join(out_dir, args.three_grams_probs_file)
+    # with open(three_grams_probs_file, 'w', encoding='utf-8') as f:
+    #     f.write(json.dumps(three_grams_probs, ensure_ascii=False))
+    #
+    # four_grams_probs_file = os.path.join(out_dir, args.four_grams_probs_file)
+    # with open(four_grams_probs_file, 'w', encoding='utf-8') as f:
+    #     f.write(json.dumps(four_grams_probs, ensure_ascii=False))
+    #
+    # five_grams_probs_file = os.path.join(out_dir, args.five_grams_probs_file)
+    # with open(five_grams_probs_file, 'w', encoding='utf-8') as f:
+    #     f.write(json.dumps(five_grams_probs, ensure_ascii=False))
+    #
+    # original_text_set = []
+    # with open(args.original_test_file, 'r', encoding="utf-8") as f:
+    #     for line in f:
+    #         try:
+    #             text = json.loads(line)
+    #             original_text_set.append(text)
+    #         except Exception as e:
+    #             print(e, line)
+    #
+    # test_set = construct_test_text_set(original_text_set, generation_test_text_set, args)
+    #
+    # new_test_file = os.path.join(out_dir, args.new_test_file)
+    # with open(new_test_file, "w", encoding='utf-8') as f:
+    #     for text in test_set:
+    #         f.write(json.dumps(text, ensure_ascii=False))
+    #         f.write('\n')
+    #
+    # test_text_tokenize_ids = []
+    # for i in tqdm.tqdm(range(len(test_set))):
+    #     tokenize_ids = {}
+    #     if args.is_gpt:
+    #         text_tokenize = tokenizer.tokenize(test_set[i]["text"], truncation=True)
+    #     else:
+    #         text_tokenize = tokenizer.tokenize(test_set[i]["text"])
+    #     tokenize_ids[text[i]["label"]] = tokenizer.convert_tokens_to_ids(text_tokenize)
+    #     # tokens to token_ids
+    #     test_text_tokenize_ids.append(tokenize_ids)
+    #
+    # test_ppl = proxy_perplexity(test_text_tokenize_ids, args, two_grams_probs, three_grams_probs, four_grams_probs, five_grams_probs)
+    #
+    # test_ppl_file = os.path.join(out_dir, args.test_ppl_file)
+    # with open(test_ppl_file, "w", encoding='utf-8') as f:
+    #     for ppl in test_ppl:
+    #         f.write(json.dumps(ppl, ensure_ascii=False))
+    #         f.write('\n')
 
 
 
 if __name__ == "__main__":
     args = parse_args()
-    # print(args)
-    main()
+    print(args)
+    main(args)
```

### Comparing `llmdet-1.0.3/llmdet.egg-info/PKG-INFO` & `llmdet-1.0.4/llmdet.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 Metadata-Version: 2.1
 Name: llmdet
-Version: 1.0.3
-Summary: LLMDet：A Large Language Models Detection Tool
+Version: 1.0.4
+Summary: LLMDet: A Large Language Models Detection Tool
 Home-page: https://github.com/cansee5/LLMDet
 Author: Kangxi Wu, Liang Pang
 Author-email: wukx0901@gmail.com
+License: UNKNOWN
+Description: # 🪬 LLMDet：A Large Language Models Detection Tool
+        
+        LLMDet is a text detection tool that can identify which generated sources the text came from (e.g. large language model or human-write). The core idea of the detection algorithm is to use the n-grams probability sampled from specified language model to calculate proxy perplexity of large language models, and use the proxy perplexity as a feature to train a text classifier.
+        
+        ### Features
+        We believe that a practical LLM detection tool needs to have the following capabilities, which is also the goal of our LLMDet.
+        
+        1. **Specificity**: Our project aims to distinguish between different large-scale language models and human-generated text. For example, LLMDet can tell you whether the text is generated by GPT-2 or OPT or a human, and give each a specific probability.
+        2. **Safty**: Our project does not need to require running large language models locally. That is, we can act as a third-party authentication agent without maintaining large language models, which may be fixed assets or sensitive information for large companies.
+        3. **Efficiency**: Our method detects very fast. This is because we don't need to infer from large language models.
+        4. **Extendibility**: Our project can easily adapt to newly proposed large language models. 
+        
+        
+        ### Installation Notes
+        A package for large language model-generated text detection tool.
+        
+        Code is compatible with Python >=3.8
+          * Fully automatic installation: `pip install llmdet`
+          * Semi-automatic installation: First download http://pypi.python.org/pypi/llmdet/ , decompress and run `python setup.py install`
+          * See `requirements.txt` for dependent python packages.
+        
+        ### Main Functions
+        
+        Currently, it is supported to determine whether the text comes from GPT-2, OPT, UniLM or Human-write.
+        
+        #### Examples
+        ```python
+        import llmdet
+        
+        llmdet.load_probability()
+        
+        text = "The actress was honoured for her role in 'The Reader' at the annual ceremony, which was held at the Royal Albert Hall. The film, which is based on the novel by the same name by Philip Roth, tells the story of a New York Times reporter who returns to his hometown to cover the death of his brother-in-law. Winslet plays his wife, with whom he has been divided since the death of their son.\nIn the film, Winslet plays the mother of the grieving brother-in-law.\nThe actress also won a Golden Globe for her role in the film at the ceremony in November.\nWinslet was also nominated for an Oscar for her role in 'The Reader'.\nThe 63-year-old Winslet was seen accepting her awards at the ceremony, where she was joined by her husband, John Krasinski, who has been nominated for best supporting actor in the film.\nWinslet and Krasinski met while"
+        
+        # Detect, `text` is a string or string list
+        result = llmdet.detect(text)
+        print(result)
+        ```
+        #### Detection Results
+        ```json
+        [{
+            'OPT': 0.5451331013247862,
+            'GPT-2': 0.4393605735865629, 
+            'UniLM': 0.012642800848279893, 
+            'T5': 0.0022592730436008556, 
+            'Bloom': 0.00025873253035729044, 
+            'GPT-neo': 0.0002520776780109571, 
+            'LLaMA': 6.0459794454546154e-05, 
+            'Human_write': 1.9576671778802474e-05, 
+            'BART': 1.3404522168622544e-05
+        }]
+        ```
+        
+        ### TODO List
+          - [ ] Extend the detection models to LLaMA, T5, Bart and Vicuna.
+          - [ ] Compress the project.
+          - [ ] Add more experimental performnce results.
+        
+        ### Citation
+        ```bibtex
+        
+        ```
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 🪬 LLMDet：A Large Language Models Detection Tool
-
-LLMDet is a text detection tool that can identify which generated sources the text came from (e.g. large language model or human-write). The core idea of the detection algorithm is to use the n-grams probability sampled from specified language model to calculate proxy perplexity of large language models, and use the proxy perplexity as a feature to train a text classifier.
-
-### Features
-We believe that a practical LLM detection tool needs to have the following capabilities, which is also the goal of our LLMDet.
-
-1. **Specificity**: Our project aims to distinguish between different large-scale language models and human-generated text. For example, LLMDet can tell you whether the text is generated by GPT-2 or OPT or a human, and give each a specific probability.
-2. **Safty**: Our project does not need to require running large language models locally. That is, we can act as a third-party authentication agent without maintaining large language models, which may be fixed assets or sensitive information for large companies.
-3. **Efficiency**: Our method detects very fast. This is because we don't need to infer from large language models.
-4. **Extendibility**: Our project can easily adapt to newly proposed large language models. 
-
-
-### Installation Notes
-A package for large language model-generated text detection tool.
-
-Code is compatible with Python >=3.8
-  * Fully automatic installation: `pip install llmdet`
-  * Semi-automatic installation: First download http://pypi.python.org/pypi/llmdet/ , decompress and run `python setup.py install`
-  * See `requirements.txt` for dependent python packages.
-
-### Main Functions
-
-Currently, it is supported to determine whether the text comes from GPT-2, OPT, UniLM or Human-write.
-
-#### Examples
-```python
-from llmdet import detect
-
-text = "The actress was honoured for her role in 'The Reader' at the annual ceremony, which was held at the Royal Albert Hall. The film, which is based on the novel by the same name by Philip Roth, tells the story of a New York Times reporter who returns to his hometown to cover the death of his brother-in-law. Winslet plays his wife, with whom he has been divided since the death of their son.\nIn the film, Winslet plays the mother of the grieving brother-in-law.\nThe actress also won a Golden Globe for her role in the film at the ceremony in November.\nWinslet was also nominated for an Oscar for her role in 'The Reader'.\nThe 63-year-old Winslet was seen accepting her awards at the ceremony, where she was joined by her husband, John Krasinski, who has been nominated for best supporting actor in the film.\nWinslet and Krasinski met while"
-
-# Detect, `text` is a string or string list
-result = detect(text)
-print(result)
-```
-#### Detection Results
-```json
-[{
- "Human_write": 0.00034990044262862392 , 
- "GPT-2": 0.003904839900808308, 
- "OPT": 0.6458330377453642, 
- "UniLM": 0.34991221792754135
-}]
-```
-
-### TODO List
-  - [ ] Extend the detection models to LLaMA, T5, Bart and Vicuna.
-  - [ ] Compress the project.
-  - [ ] Add more experimental performnce results.
-
-### Citation
-```bibtex
-
-```
-
-
```

### Comparing `llmdet-1.0.3/setup.py` & `llmdet-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="llmdet",
-    version="1.0.3",
+    version="1.0.4",
     author="Kangxi Wu, Liang Pang",
     author_email="wukx0901@gmail.com",
-    description="LLMDet：A Large Language Models Detection Tool",
+    description="LLMDet: A Large Language Models Detection Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cansee5/LLMDet",
     packages=setuptools.find_packages(),
     install_requires=[
-            'transformers',
+            'transformers>=4.29.0',
             'nltk',
             'lightgbm',
             'numpy',
             'sklearn',
             'tqdm',
             'argparse',
         ],
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

