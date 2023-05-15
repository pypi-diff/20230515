# Comparing `tmp/s2aff-0.25.tar.gz` & `tmp/s2aff-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.25.tar", last modified: Mon May 15 17:00:19 2023, max compression
+gzip compressed data, was "s2aff-0.26.tar", last modified: Mon May 15 17:16:25 2023, max compression
```

## Comparing `s2aff-0.25.tar` & `s2aff-0.26.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:00:19.829498 s2aff-0.25/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.25/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 17:00:19.829375 s2aff-0.25/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.25/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:00:19.821571 s2aff-0.25/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.25/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.25/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.25/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:00:19.821845 s2aff-0.25/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.25/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:00:19.824970 s2aff-0.25/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8045 2023-05-15 14:58:57.000000 s2aff-0.25/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.25/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.25/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.25/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.25/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.25/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    14211 2023-05-15 16:54:57.000000 s2aff-0.25/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.25/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.25/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:00:19.826958 s2aff-0.25/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.25/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.25/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5287 2023-05-15 04:30:43.000000 s2aff-0.25/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:00:19.826271 s2aff-0.25/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 17:00:19.000000 s2aff-0.25/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 17:00:19.000000 s2aff-0.25/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 17:00:19.000000 s2aff-0.25/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 17:00:19.000000 s2aff-0.25/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 17:00:19.000000 s2aff-0.25/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:00:19.829120 s2aff-0.25/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.25/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3039 2023-05-15 04:35:10.000000 s2aff-0.25/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4490 2023-05-15 04:35:10.000000 s2aff-0.25/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6350 2023-05-15 04:35:10.000000 s2aff-0.25/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.25/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.25/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.25/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 17:00:19.829542 s2aff-0.25/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 17:00:15.000000 s2aff-0.25/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:16:25.417744 s2aff-0.26/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.26/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 17:16:25.417621 s2aff-0.26/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.26/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:16:25.409831 s2aff-0.26/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.26/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.26/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.26/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:16:25.410033 s2aff-0.26/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.26/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:16:25.413510 s2aff-0.26/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8045 2023-05-15 14:58:57.000000 s2aff-0.26/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.26/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.26/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.26/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.26/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.26/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    14299 2023-05-15 17:15:34.000000 s2aff-0.26/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.26/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.26/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:16:25.415250 s2aff-0.26/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.26/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.26/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5287 2023-05-15 04:30:43.000000 s2aff-0.26/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:16:25.414594 s2aff-0.26/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 17:16:25.000000 s2aff-0.26/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 17:16:25.000000 s2aff-0.26/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 17:16:25.000000 s2aff-0.26/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 17:16:25.000000 s2aff-0.26/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 17:16:25.000000 s2aff-0.26/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 17:16:25.417360 s2aff-0.26/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.26/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3039 2023-05-15 04:35:10.000000 s2aff-0.26/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4490 2023-05-15 04:35:10.000000 s2aff-0.26/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6350 2023-05-15 04:35:10.000000 s2aff-0.26/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.26/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.26/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.26/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 17:16:25.417788 s2aff-0.26/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 17:16:02.000000 s2aff-0.26/setup.py
```

### Comparing `s2aff-0.25/LICENSE` & `s2aff-0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/README.md` & `s2aff-0.26/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/data/combine_gold.py` & `s2aff-0.26/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/data/download_latest_ror.py` & `s2aff-0.26/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/__init__.py` & `s2aff-0.26/s2aff/__init__.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/consts.py` & `s2aff-0.26/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/data.py` & `s2aff-0.26/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/features.py` & `s2aff-0.26/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/file_cache.py` & `s2aff-0.26/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/lightgbm_helpers.py` & `s2aff-0.26/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/model.py` & `s2aff-0.26/s2aff/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 from blingfire import text_to_words
 from s2aff.consts import PATHS
 from s2aff.text import fix_text, CERTAINLY_MAIN
 
 
 FEATURE_NAMES = list(FEATURE_NAMES)
 
+process_cnt = 0
+
 def process_item(item, self_ror_index, self_lm, fixed_affiliation_str):
+    print(f"RUNNING PROCESS ITEM: {process_cnt}")
+    process_cnt += 1
     ror_entry = parse_ror_entry_into_single_string_lightgbm(item[0], self_ror_index)
     x = make_lightgbm_features(fixed_affiliation_str, ror_entry, self_lm)
     x[-3:] = [item[1], int(item[1] == -0.15), int(item[1] == -0.1)]
     return x
 
 def parse_ner_prediction(ner_prediction, ror_index):
     """Parse the NER prediction that comes out of a NERPredictor
```

### Comparing `s2aff-0.25/s2aff/ror.py` & `s2aff-0.26/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/text.py` & `s2aff-0.26/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/timo/integration_test.py` & `s2aff-0.26/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff/timo/interface.py` & `s2aff-0.26/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/s2aff.egg-info/SOURCES.txt` & `s2aff-0.26/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.26/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.26/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/scripts/generate_lightgbm_training_data.py` & `s2aff-0.26/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/scripts/train_lightgbm_reranker.py` & `s2aff-0.26/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/scripts/train_ner_model.py` & `s2aff-0.26/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/scripts/update_openalex_works_counts.py` & `s2aff-0.26/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.25/setup.py` & `s2aff-0.26/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.25",
+    version="0.26",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

