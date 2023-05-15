# Comparing `tmp/s2aff-0.23.tar.gz` & `tmp/s2aff-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.23.tar", last modified: Mon May 15 04:41:07 2023, max compression
+gzip compressed data, was "s2aff-0.24.tar", last modified: Mon May 15 16:05:22 2023, max compression
```

## Comparing `s2aff-0.23.tar` & `s2aff-0.24.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.456303 s2aff-0.23/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.23/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 04:41:07.456187 s2aff-0.23/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.23/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.449497 s2aff-0.23/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.23/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.23/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.23/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.449733 s2aff-0.23/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.23/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.452675 s2aff-0.23/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8094 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.23/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.23/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13564 2023-05-15 04:32:44.000000 s2aff-0.23/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.454006 s2aff-0.23/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.23/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5287 2023-05-15 04:30:43.000000 s2aff-0.23/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.453566 s2aff-0.23/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 04:41:07.000000 s2aff-0.23/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 04:41:07.455940 s2aff-0.23/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.23/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3039 2023-05-15 04:35:10.000000 s2aff-0.23/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4490 2023-05-15 04:35:10.000000 s2aff-0.23/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6350 2023-05-15 04:35:10.000000 s2aff-0.23/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.23/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.23/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.23/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 04:41:07.456347 s2aff-0.23/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 04:41:05.000000 s2aff-0.23/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 16:05:22.699970 s2aff-0.24/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.24/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 16:05:22.699811 s2aff-0.24/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.24/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 16:05:22.691835 s2aff-0.24/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.24/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.24/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.24/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 16:05:22.692180 s2aff-0.24/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.24/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 16:05:22.695601 s2aff-0.24/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8045 2023-05-15 14:58:57.000000 s2aff-0.24/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.24/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.24/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.24/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.24/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.24/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    14095 2023-05-15 16:02:04.000000 s2aff-0.24/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.24/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.24/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 16:05:22.697381 s2aff-0.24/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.24/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.24/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5287 2023-05-15 04:30:43.000000 s2aff-0.24/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 16:05:22.696761 s2aff-0.24/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 16:05:22.000000 s2aff-0.24/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 16:05:22.000000 s2aff-0.24/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 16:05:22.000000 s2aff-0.24/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 16:05:22.000000 s2aff-0.24/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 16:05:22.000000 s2aff-0.24/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 16:05:22.699475 s2aff-0.24/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.24/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3039 2023-05-15 04:35:10.000000 s2aff-0.24/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4490 2023-05-15 04:35:10.000000 s2aff-0.24/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6350 2023-05-15 04:35:10.000000 s2aff-0.24/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.24/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.24/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.24/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 16:05:22.700055 s2aff-0.24/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 16:05:17.000000 s2aff-0.24/setup.py
```

### Comparing `s2aff-0.23/LICENSE` & `s2aff-0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/README.md` & `s2aff-0.24/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/data/combine_gold.py` & `s2aff-0.24/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/data/download_latest_ror.py` & `s2aff-0.24/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/__init__.py` & `s2aff-0.24/s2aff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,31 +42,31 @@
     """
 
     def __init__(
         self,
         ner_predictor,
         ror_index,
         pairwise_model,
-        top_k_first_stage=100,
+        top_k_first_stage=20,
         pairwise_model_threshold=0.3,
         pairwise_model_delta_threshold=0.2,
         no_ror_output_text="NO_ROR_FOUND",
         no_candidates_output_text="NO_CANDIDATES_FOUND",
-        number_of_top_candidates_to_return=5,
+        number_of_top_candidates_to_return=1,
         look_for_grid_and_isni=True,
     ):
         self.ner_predictor = ner_predictor
         self.ror_index = ror_index
         self.pairwise_model = pairwise_model
-        self.top_k_first_stage = top_k_first_stage
+        self.top_k_first_stage = 20
         self.pairwise_model_threshold = pairwise_model_threshold
         self.pairwise_model_delta_threshold = pairwise_model_delta_threshold
         self.no_ror_output_text = no_ror_output_text
         self.no_candidates_output_text = no_candidates_output_text
-        self.number_of_top_candidates_to_return = number_of_top_candidates_to_return
+        self.number_of_top_candidates_to_return = 1
         self.look_for_grid_and_isni = True
 
     def predict(self, raw_affiliations):
         """Predict function for raw affiliation strings
 
         :param raw_affiliations: a list of raw affiliation strings
```

### Comparing `s2aff-0.23/s2aff/consts.py` & `s2aff-0.24/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/data.py` & `s2aff-0.24/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/features.py` & `s2aff-0.24/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/file_cache.py` & `s2aff-0.24/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/lightgbm_helpers.py` & `s2aff-0.24/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/model.py` & `s2aff-0.24/s2aff/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 import torch
+import concurrent.futures
+import functools
 
 # have to do this to avoid weird bugs
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 torch.multiprocessing.set_sharing_strategy("file_system")
 
 import gc
 import numpy as np
@@ -15,14 +17,19 @@
 from blingfire import text_to_words
 from s2aff.consts import PATHS
 from s2aff.text import fix_text, CERTAINLY_MAIN
 
 
 FEATURE_NAMES = list(FEATURE_NAMES)
 
+def process_item(item, self_ror_index, self_lm, fixed_affiliation_str):
+    ror_entry = parse_ror_entry_into_single_string_lightgbm(item[0], self_ror_index)
+    x = make_lightgbm_features(fixed_affiliation_str, ror_entry, self_lm)
+    x[-3:] = [item[1], int(item[1] == -0.15), int(item[1] == -0.1)]
+    return x
 
 def parse_ner_prediction(ner_prediction, ror_index):
     """Parse the NER prediction that comes out of a NERPredictor
     into main entity, child entities, address, and early candidates for the
     next retrieval stage.
 
     Args:
@@ -338,19 +345,24 @@
 
         Returns:
             reranked_candidates (np.array[str]): Array of candidate ROR ids
             reranked_scores (np.array[float]): Array of candidate scores
         """
         fixed_affiliation_string = fix_text(raw_affiliation).lower().replace(",", "")
         X = []
+        all_items = []
         for i, s in zip(candidates, scores):
-            ror_entry = parse_ror_entry_into_single_string_lightgbm(i, self.ror_index)
-            x = make_lightgbm_features(fixed_affiliation_string, ror_entry, self.lm)
-            x[-3:] = [s, int(s == -0.15), int(s == -0.1)]
-            X.append(x)
+            all_items.append((i,s))
+
+        process_item_with_params = functools.partial(process_item, self_ror_index=self.ror_index, self_lm=self.lm, fixed_affiliation_str=fixed_affiliation_string)
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            results = executor.map(process_item_with_params, all_items)
+            for result in results:
+                X.append(result)
+
         X = np.array(X)
         scores = self.model.predict(X, num_threads=self.num_threads)
         # penalty when no match across fields
         has_no_match = X[:, self.inds_to_check].sum(1) == 0
         scores -= 0.05 * has_no_match  # magic number!
         scores += 0.05 * X[:, self.city_ind]
         scores_argsort = np.argsort(scores)[::-1]
```

### Comparing `s2aff-0.23/s2aff/ror.py` & `s2aff-0.24/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/text.py` & `s2aff-0.24/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/timo/integration_test.py` & `s2aff-0.24/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff/timo/interface.py` & `s2aff-0.24/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/s2aff.egg-info/SOURCES.txt` & `s2aff-0.24/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.24/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.24/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/scripts/generate_lightgbm_training_data.py` & `s2aff-0.24/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/scripts/train_lightgbm_reranker.py` & `s2aff-0.24/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/scripts/train_ner_model.py` & `s2aff-0.24/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/scripts/update_openalex_works_counts.py` & `s2aff-0.24/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.23/setup.py` & `s2aff-0.24/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.23",
+    version="0.24",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

