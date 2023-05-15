# Comparing `tmp/s2aff-0.28.tar.gz` & `tmp/s2aff-0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.28.tar", last modified: Mon May 15 17:29:51 2023, max compression
+gzip compressed data, was "s2aff-0.29.tar", last modified: Mon May 15 18:05:45 2023, max compression
```

## Comparing `s2aff-0.28.tar` & `s2aff-0.29.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:29:51.993292 s2aff-0.28/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.28/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 17:29:51.993110 s2aff-0.28/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.28/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:29:51.982886 s2aff-0.28/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.28/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.28/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.28/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:29:51.983175 s2aff-0.28/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.28/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:29:51.986499 s2aff-0.28/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8097 2023-05-15 17:25:26.000000 s2aff-0.28/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.28/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.28/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.28/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.28/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.28/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13675 2023-05-15 17:29:38.000000 s2aff-0.28/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.28/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.28/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:29:51.988154 s2aff-0.28/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.28/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.28/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5287 2023-05-15 04:30:43.000000 s2aff-0.28/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:29:51.987536 s2aff-0.28/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 17:29:51.000000 s2aff-0.28/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 17:29:51.000000 s2aff-0.28/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 17:29:51.000000 s2aff-0.28/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 17:29:51.000000 s2aff-0.28/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 17:29:51.000000 s2aff-0.28/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:29:51.990618 s2aff-0.28/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.28/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3039 2023-05-15 04:35:10.000000 s2aff-0.28/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4490 2023-05-15 04:35:10.000000 s2aff-0.28/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6350 2023-05-15 04:35:10.000000 s2aff-0.28/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.28/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.28/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.28/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 17:29:51.993394 s2aff-0.28/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 17:29:43.000000 s2aff-0.28/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.552203 s2aff-0.29/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.29/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 18:05:45.552073 s2aff-0.29/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.29/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.544734 s2aff-0.29/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.29/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.29/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.29/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.544993 s2aff-0.29/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.29/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.548384 s2aff-0.29/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8093 2023-05-15 18:04:35.000000 s2aff-0.29/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.29/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.29/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.29/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.549974 s2aff-0.29/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.29/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.549469 s2aff-0.29/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.551782 s2aff-0.29/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.29/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.29/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.29/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.29/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.29/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.29/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.29/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 18:05:45.552249 s2aff-0.29/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 18:05:28.000000 s2aff-0.29/setup.py
```

### Comparing `s2aff-0.28/LICENSE` & `s2aff-0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/README.md` & `s2aff-0.29/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/data/combine_gold.py` & `s2aff-0.29/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/data/download_latest_ror.py` & `s2aff-0.29/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/s2aff/__init__.py` & `s2aff-0.29/s2aff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,20 +53,20 @@
         no_candidates_output_text="NO_CANDIDATES_FOUND",
         number_of_top_candidates_to_return=1,
         look_for_grid_and_isni=True,
     ):
         self.ner_predictor = ner_predictor
         self.ror_index = ror_index
         self.pairwise_model = pairwise_model
-        self.top_k_first_stage = 20
+        self.top_k_first_stage = top_k_first_stage
         self.pairwise_model_threshold = pairwise_model_threshold
         self.pairwise_model_delta_threshold = pairwise_model_delta_threshold
         self.no_ror_output_text = no_ror_output_text
         self.no_candidates_output_text = no_candidates_output_text
-        self.number_of_top_candidates_to_return = 1
+        self.number_of_top_candidates_to_return = number_of_top_candidates_to_return
         self.look_for_grid_and_isni = True
 
     def predict(self, raw_affiliations):
         """Predict function for raw affiliation strings
 
         :param raw_affiliations: a list of raw affiliation strings
 
@@ -92,15 +92,14 @@
         outputs = []
         for counter, (raw_affiliation, ner_prediction) in enumerate(zip(raw_affiliations, ner_predictions)):
             print(
                 f"Getting ROR candidates and reranking for: '{raw_affiliation}' ({counter+1}/{len(raw_affiliations)})",
                 end="\r",
             )
             main, child, address, early_candidates = parse_ner_prediction(ner_prediction, self.ror_index)
-            print("Parse NER prediction finished!")
             # sometimes the affiliation strings just contain GRID or ISNI ids
             # todo: some time in the future the strings may contain ROR ids too
             if self.look_for_grid_and_isni:
                 ror_from_grid = self.ror_index.extract_grid_and_map_to_ror(raw_affiliation)
                 ror_from_isni = self.ror_index.extract_isni_and_map_to_ror(raw_affiliation)
                 ror_from_grid_or_isni = ror_from_grid or ror_from_isni
                 found_early = ror_from_grid_or_isni is not None
```

### Comparing `s2aff-0.28/s2aff/consts.py` & `s2aff-0.29/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/s2aff/data.py` & `s2aff-0.29/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/s2aff/features.py` & `s2aff-0.29/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/s2aff/file_cache.py` & `s2aff-0.29/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/s2aff/lightgbm_helpers.py` & `s2aff-0.29/s2aff/lightgbm_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         label_gain_max=1000,
         eval_at="1,2,3,4,5,100",
         n_estimators=5000,
         hyperopt_evals=25,
         device="cpu",
         tree_learner="data",
         random_seed=0,
-        threads=16,
+        threads=10,
         feval=None,
     ):
 
         super().__init__()
 
         if learning_task == "classification":
             assert metric in {"binary", "multiclass", "multiclassova"}
```

### Comparing `s2aff-0.28/s2aff/model.py` & `s2aff-0.29/s2aff/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import torch
-import time
 
 # have to do this to avoid weird bugs
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 torch.multiprocessing.set_sharing_strategy("file_system")
 
 import gc
 import numpy as np
@@ -151,35 +150,35 @@
     """Named Entity Recognition for affiliation strings.
     Uses SimpleTransformers under the hood.
     """
 
     def __init__(self, model_path=PATHS["ner_model"], model_type="roberta", use_cuda=True):
         self.model_path = model_path
         self.model_type = model_type
-        self.use_cuda = True
+        self.use_cuda = use_cuda
         if self.model_path is not None:
             self.load_model(self.model_path, self.model_type)
 
     def load_model(self, model_path=PATHS["ner_model"], model_type="roberta"):
         """Load a model from disk.
 
         model_path (str, optional): Location of the saved NER model.
             Should be what is saved by SimpleTransformers NERModel. Defaults to PATHS["ner_model"].
         model_type (str, optional): Model type such as roberta or bert.
             If you don't know, check the config.json in the model directory. Defaults to "roberta".
         """
         self.model = NERModel(
             model_type,
             model_path,
-            use_cuda=True,
+            use_cuda=self.use_cuda,
             args={
-                "use_multiprocessing": True,
-                "use_multiprocessing_for_evaluation": True,
+                "use_multiprocessing": False,
+                "use_multiprocessing_for_evaluation": False,
                 "process_count": 1,
-                "eval_batch_size": 16,
+                "eval_batch_size": 8,
             },
         )
 
     def save_model(self, model_path=PATHS["ner_model"]):
         """Save model to disk
 
         Args:
@@ -229,21 +228,21 @@
         model_args.attention_probs_dropout_prob = 0.3
         model_args.evaluate_during_training = False
         model_args.reprocess_input_data = True
         model_args.overwrite_output_dir = True
         model_args.manual_seed = 4
         model_args.train_batch_size = 32
         model_args.eval_batch_size = 128
-        model_args.use_multiprocessing = True
-        model_args.use_multiprocessing_for_evaluation = True
+        model_args.use_multiprocessing = False
+        model_args.use_multiprocessing_for_evaluation = False
         model_args.process_count = 1
 
         # train and save model
         custom_labels = list(set(df_train.labels))
-        model = NERModel(model_type, model_name, labels=custom_labels, args=model_args, use_cuda=True)
+        model = NERModel(model_type, model_name, labels=custom_labels, args=model_args, use_cuda=self.use_cuda)
         model.train_model(df_train)
         self.model = model.model
 
         if df_validation is not None:
             result_vl, _ = self.eval(df_validation)
         else:
             result_vl = None
@@ -284,15 +283,15 @@
             return predictions[0]
         else:
             return predictions
 
 
 class PairwiseRORLightGBMReranker:
     def __init__(
-        self, ror_index, model_path=PATHS["lightgbm_model"], kenlm_model_path=PATHS["kenlm_model"], num_threads=16
+        self, ror_index, model_path=PATHS["lightgbm_model"], kenlm_model_path=PATHS["kenlm_model"], num_threads=0
     ):
         self.ror_index = ror_index
         self.model_path = model_path
         self.kenlm_model_path = kenlm_model_path
         self.load_model(model_path)
         self.lm = kenlm.LanguageModel(kenlm_model_path)
         self.num_threads = num_threads
@@ -337,24 +336,22 @@
             raw_affiliation (str): Raw affiliation string.
             candidates (list[str]): List of candidate ROR ids.
 
         Returns:
             reranked_candidates (np.array[str]): Array of candidate ROR ids
             reranked_scores (np.array[float]): Array of candidate scores
         """
-        start_time = time.time()
         fixed_affiliation_string = fix_text(raw_affiliation).lower().replace(",", "")
         X = []
         for i, s in zip(candidates, scores):
             ror_entry = parse_ror_entry_into_single_string_lightgbm(i, self.ror_index)
             x = make_lightgbm_features(fixed_affiliation_string, ror_entry, self.lm)
             x[-3:] = [s, int(s == -0.15), int(s == -0.1)]
             X.append(x)
         X = np.array(X)
-        print(f"Time to generate X: {time.time() - start_time}s")
         scores = self.model.predict(X, num_threads=self.num_threads)
         # penalty when no match across fields
         has_no_match = X[:, self.inds_to_check].sum(1) == 0
         scores -= 0.05 * has_no_match  # magic number!
         scores += 0.05 * X[:, self.city_ind]
         scores_argsort = np.argsort(scores)[::-1]
         reranked = np.vstack([np.array(candidates), scores]).T[scores_argsort]
```

### Comparing `s2aff-0.28/s2aff/ror.py` & `s2aff-0.29/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/s2aff/text.py` & `s2aff-0.29/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/s2aff/timo/integration_test.py` & `s2aff-0.29/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/s2aff/timo/interface.py` & `s2aff-0.29/s2aff/timo/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     def _load_model(self) -> None:
         """
         Perform whatever start-up operations are required to get your
         model ready for inference. This operation is performed only once
         during the application life-cycle.
         """
         ner_predictor = NERPredictor(
-            model_path=join(self._artifacts_dir, basename(PATHS["ner_model"])), use_cuda=True
+            model_path=join(self._artifacts_dir, basename(PATHS["ner_model"])), use_cuda=torch.cuda.is_available()
         )
         ror_index = RORIndex(
             ror_data_path=join(self._artifacts_dir, basename(PATHS["ror_data"])),
             country_info_path=join(self._artifacts_dir, basename(PATHS["country_info"])),
             works_counts_path=join(self._artifacts_dir, basename(PATHS["openalex_works_counts"])),
         )
         pairwise_model = PairwiseRORLightGBMReranker(
```

### Comparing `s2aff-0.28/s2aff.egg-info/SOURCES.txt` & `s2aff-0.29/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.29/scripts/approximate_runtime_and_memory_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from s2aff.consts import PATHS
 from s2aff.ror import RORIndex
 from s2aff.model import NERPredictor, PairwiseRORLightGBMReranker, parse_ner_prediction
 from s2aff.data import load_gold_affiliation_annotations
 from s2aff.text import fix_text
 from blingfire import text_to_words
 
-USE_CUDA = True
+USE_CUDA = False
 
 print(
     "Total memory footprint before loading various artifacts (in MB): ",
     psutil.Process(os.getpid()).memory_info().rss / 1024**2,
 )
 
 # fixed costs: load everything
-ner_predictor = NERPredictor(use_cuda=True)
+ner_predictor = NERPredictor(use_cuda=USE_CUDA)
 print(
     "Total memory footprint after loading NER (in MB): ",
     psutil.Process(os.getpid()).memory_info().rss / 1024**2,
 )
 ror_index = RORIndex()
 print(
     "Total memory footprint after loading inverted index (in MB): ",
```

### Comparing `s2aff-0.28/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.29/scripts/evaluate_first_stage_ranker.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import numpy as np
 from s2aff.data import load_gold_affiliation_annotations
 from s2aff.ror import RORIndex, index_min
 from s2aff.model import NERPredictor, parse_ner_prediction
 
 
-USE_CUDA = True
+USE_CUDA = False
 
 # load the gold, and subset to training data
 df = load_gold_affiliation_annotations()
 # df = df[df.split == "train"]
 
 # load the ROR index and NERPredictor
 ner_predictor = NERPredictor(use_cuda=USE_CUDA)  # defaults to models in the data directory
```

### Comparing `s2aff-0.28/scripts/generate_lightgbm_training_data.py` & `s2aff-0.29/scripts/generate_lightgbm_training_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 """
 Training set for gold data
 """
 df_gold = load_gold_affiliation_annotations()
 
 # should do this batched
-ner_predictor = NERPredictor(use_cuda=True)
+ner_predictor = NERPredictor(use_cuda=False)
 parsed_affiliations = ner_predictor.predict(df_gold.loc[:, "original_affiliation"].values)
 df_gold.loc[:, "parsed_affiliations"] = parsed_affiliations
 ner_predictor.delete_model()  # clean up to make space
 
 X_train, y_train, w_train, group_train, rors_train, qs_train = make_pairwise_data(
     df_gold,
     lm,
@@ -150,15 +150,15 @@
 
 # same but do it on the stuff with no ROR at all
 df_gold = load_gold_affiliation_annotations(keep_non_ror_gold=True)
 keep_flag = df_gold.labels.apply(lambda x: any(["ror.org" not in i for i in x]))
 df_gold = df_gold[keep_flag]
 
 # should do this batched
-ner_predictor = NERPredictor(use_cuda=True)
+ner_predictor = NERPredictor(use_cuda=False)
 parsed_affiliations = ner_predictor.predict(df_gold.loc[:, "original_affiliation"].values)
 df_gold.loc[:, "parsed_affiliations"] = parsed_affiliations
 ner_predictor.delete_model()  # clean up to make space
 
 X_none, y_none, w_none, group_none, rors_none, qs_none = make_pairwise_data(
     df_gold,
     lm,
```

### Comparing `s2aff-0.28/scripts/train_lightgbm_reranker.py` & `s2aff-0.29/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/scripts/train_ner_model.py` & `s2aff-0.29/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/scripts/update_openalex_works_counts.py` & `s2aff-0.29/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.28/setup.py` & `s2aff-0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.28",
+    version="0.29",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

