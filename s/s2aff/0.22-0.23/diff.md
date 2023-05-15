# Comparing `tmp/s2aff-0.22.tar.gz` & `tmp/s2aff-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.22.tar", last modified: Fri May 12 15:53:20 2023, max compression
+gzip compressed data, was "s2aff-0.23.tar", last modified: Mon May 15 04:41:07 2023, max compression
```

## Comparing `s2aff-0.22.tar` & `s2aff-0.23.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 15:53:20.366566 s2aff-0.22/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.22/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-12 15:53:20.366431 s2aff-0.22/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.22/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 15:53:20.359891 s2aff-0.22/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.22/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.22/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.22/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 15:53:20.360266 s2aff-0.22/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.22/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 15:53:20.363286 s2aff-0.22/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8094 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.22/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.22/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-12 15:50:06.000000 s2aff-0.22/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 15:53:20.364516 s2aff-0.22/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-08 19:46:34.000000 s2aff-0.22/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 15:53:20.363983 s2aff-0.22/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-12 15:53:20.000000 s2aff-0.22/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-12 15:53:20.000000 s2aff-0.22/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-12 15:53:20.000000 s2aff-0.22/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-12 15:53:20.000000 s2aff-0.22/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-12 15:53:20.000000 s2aff-0.22/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 15:53:20.366110 s2aff-0.22/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.22/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-08 19:46:34.000000 s2aff-0.22/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-08 19:46:34.000000 s2aff-0.22/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-08 19:46:34.000000 s2aff-0.22/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.22/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.22/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.22/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-12 15:53:20.366614 s2aff-0.22/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-12 15:53:13.000000 s2aff-0.22/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.456303 s2aff-0.23/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.23/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 04:41:07.456187 s2aff-0.23/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.23/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.449497 s2aff-0.23/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.23/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.23/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.23/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.449733 s2aff-0.23/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.23/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.452675 s2aff-0.23/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8094 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.23/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.23/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13564 2023-05-15 04:32:44.000000 s2aff-0.23/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.454006 s2aff-0.23/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5287 2023-05-15 04:30:43.000000 s2aff-0.23/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.453566 s2aff-0.23/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.455940 s2aff-0.23/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.23/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3039 2023-05-15 04:35:10.000000 s2aff-0.23/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4490 2023-05-15 04:35:10.000000 s2aff-0.23/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6350 2023-05-15 04:35:10.000000 s2aff-0.23/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.23/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.23/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.23/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 04:41:07.456347 s2aff-0.23/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 04:41:05.000000 s2aff-0.23/setup.py
```

### Comparing `s2aff-0.22/LICENSE` & `s2aff-0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/README.md` & `s2aff-0.23/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/data/combine_gold.py` & `s2aff-0.23/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/data/download_latest_ror.py` & `s2aff-0.23/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/__init__.py` & `s2aff-0.23/s2aff/__init__.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/consts.py` & `s2aff-0.23/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/data.py` & `s2aff-0.23/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/features.py` & `s2aff-0.23/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/file_cache.py` & `s2aff-0.23/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/lightgbm_helpers.py` & `s2aff-0.23/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/model.py` & `s2aff-0.23/s2aff/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,30 +150,30 @@
     """Named Entity Recognition for affiliation strings.
     Uses SimpleTransformers under the hood.
     """
 
     def __init__(self, model_path=PATHS["ner_model"], model_type="roberta", use_cuda=True):
         self.model_path = model_path
         self.model_type = model_type
-        self.use_cuda = use_cuda
+        self.use_cuda = True
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
-            use_cuda=self.use_cuda,
+            use_cuda=True,
             args={
                 "use_multiprocessing": True,
                 "use_multiprocessing_for_evaluation": True,
                 "process_count": 1,
                 "eval_batch_size": 16,
             },
         )
@@ -228,21 +228,21 @@
         model_args.attention_probs_dropout_prob = 0.3
         model_args.evaluate_during_training = False
         model_args.reprocess_input_data = True
         model_args.overwrite_output_dir = True
         model_args.manual_seed = 4
         model_args.train_batch_size = 32
         model_args.eval_batch_size = 128
-        model_args.use_multiprocessing = False
-        model_args.use_multiprocessing_for_evaluation = False
+        model_args.use_multiprocessing = True
+        model_args.use_multiprocessing_for_evaluation = True
         model_args.process_count = 1
 
         # train and save model
         custom_labels = list(set(df_train.labels))
-        model = NERModel(model_type, model_name, labels=custom_labels, args=model_args, use_cuda=self.use_cuda)
+        model = NERModel(model_type, model_name, labels=custom_labels, args=model_args, use_cuda=True)
         model.train_model(df_train)
         self.model = model.model
 
         if df_validation is not None:
             result_vl, _ = self.eval(df_validation)
         else:
             result_vl = None
```

### Comparing `s2aff-0.22/s2aff/ror.py` & `s2aff-0.23/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/text.py` & `s2aff-0.23/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/timo/integration_test.py` & `s2aff-0.23/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/s2aff/timo/interface.py` & `s2aff-0.23/s2aff/timo/interface.py`

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
-            model_path=join(self._artifacts_dir, basename(PATHS["ner_model"])), use_cuda=torch.cuda.is_available()
+            model_path=join(self._artifacts_dir, basename(PATHS["ner_model"])), use_cuda=True
         )
         ror_index = RORIndex(
             ror_data_path=join(self._artifacts_dir, basename(PATHS["ror_data"])),
             country_info_path=join(self._artifacts_dir, basename(PATHS["country_info"])),
             works_counts_path=join(self._artifacts_dir, basename(PATHS["openalex_works_counts"])),
         )
         pairwise_model = PairwiseRORLightGBMReranker(
```

### Comparing `s2aff-0.22/s2aff.egg-info/SOURCES.txt` & `s2aff-0.23/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.23/scripts/approximate_runtime_and_memory_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from s2aff.consts import PATHS
 from s2aff.ror import RORIndex
 from s2aff.model import NERPredictor, PairwiseRORLightGBMReranker, parse_ner_prediction
 from s2aff.data import load_gold_affiliation_annotations
 from s2aff.text import fix_text
 from blingfire import text_to_words
 
-USE_CUDA = False
+USE_CUDA = True
 
 print(
     "Total memory footprint before loading various artifacts (in MB): ",
     psutil.Process(os.getpid()).memory_info().rss / 1024**2,
 )
 
 # fixed costs: load everything
-ner_predictor = NERPredictor(use_cuda=USE_CUDA)
+ner_predictor = NERPredictor(use_cuda=True)
 print(
     "Total memory footprint after loading NER (in MB): ",
     psutil.Process(os.getpid()).memory_info().rss / 1024**2,
 )
 ror_index = RORIndex()
 print(
     "Total memory footprint after loading inverted index (in MB): ",
```

### Comparing `s2aff-0.22/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.23/scripts/evaluate_first_stage_ranker.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import numpy as np
 from s2aff.data import load_gold_affiliation_annotations
 from s2aff.ror import RORIndex, index_min
 from s2aff.model import NERPredictor, parse_ner_prediction
 
 
-USE_CUDA = False
+USE_CUDA = True
 
 # load the gold, and subset to training data
 df = load_gold_affiliation_annotations()
 # df = df[df.split == "train"]
 
 # load the ROR index and NERPredictor
 ner_predictor = NERPredictor(use_cuda=USE_CUDA)  # defaults to models in the data directory
```

### Comparing `s2aff-0.22/scripts/generate_lightgbm_training_data.py` & `s2aff-0.23/scripts/generate_lightgbm_training_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 """
 Training set for gold data
 """
 df_gold = load_gold_affiliation_annotations()
 
 # should do this batched
-ner_predictor = NERPredictor(use_cuda=False)
+ner_predictor = NERPredictor(use_cuda=True)
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
-ner_predictor = NERPredictor(use_cuda=False)
+ner_predictor = NERPredictor(use_cuda=True)
 parsed_affiliations = ner_predictor.predict(df_gold.loc[:, "original_affiliation"].values)
 df_gold.loc[:, "parsed_affiliations"] = parsed_affiliations
 ner_predictor.delete_model()  # clean up to make space
 
 X_none, y_none, w_none, group_none, rors_none, qs_none = make_pairwise_data(
     df_gold,
     lm,
```

### Comparing `s2aff-0.22/scripts/train_lightgbm_reranker.py` & `s2aff-0.23/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/scripts/train_ner_model.py` & `s2aff-0.23/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/scripts/update_openalex_works_counts.py` & `s2aff-0.23/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.22/setup.py` & `s2aff-0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.22",
+    version="0.23",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

