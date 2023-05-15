# Comparing `tmp/OmniEvent-0.1.5.tar.gz` & `tmp/OmniEvent-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/ph/OpenEE/dist/tmpgohqtnl1/OmniEvent-0.1.5.tar", last modified: Tue Sep 13 09:51:36 2022, max compression
+gzip compressed data, was "OmniEvent-0.1.6.tar", last modified: Mon May 15 04:53:37 2023, max compression
```

## Comparing `OmniEvent-0.1.5.tar` & `OmniEvent-0.1.6.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/
--rw-rw-r--   0 ph        (1004) ph        (1004)     1049 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/LICENSE
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/__init__.py
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent/aggregation/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/aggregation/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    17701 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/aggregation/aggregation.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    10484 2022-09-10 13:52:37.000000 OmniEvent-0.1.5/OmniEvent/arguments.py
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent/backbone/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/backbone/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    14018 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/backbone/backbone.py
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent/evaluation/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/evaluation/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    23433 2022-09-10 13:52:37.000000 OmniEvent-0.1.5/OmniEvent/evaluation/convert_format.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    16899 2022-09-10 13:52:37.000000 OmniEvent-0.1.5/OmniEvent/evaluation/dump_result.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    13663 2022-09-10 13:52:37.000000 OmniEvent-0.1.5/OmniEvent/evaluation/metric.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    20598 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/evaluation/utils.py
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent/head/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/head/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     2115 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/head/classification.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    13128 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/head/crf.py
--rw-rw-r--   0 ph        (1004) ph        (1004)      508 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/head/head.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     5036 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/infer.py
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent/infer_module/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/infer_module/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     1755 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/infer_module/io_format.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     9776 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/infer_module/seq2seq.py
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    21268 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/base_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    17559 2022-09-10 13:52:37.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/input_utils.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    11199 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/mrc_converter.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    14961 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/mrc_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    14945 2022-09-10 13:52:37.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/seq2seq_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    13811 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/sequence_labeling_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    14221 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/token_classification_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    11756 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/tokenizer.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    12996 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/input_engineering/whitespace_tokenizer.py
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent/model/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/model/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    12627 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/model/constraint_decoding.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     2342 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/model/label_smoother_sum.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    11539 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/model/model.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    10211 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/trainer.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    18172 2022-09-10 13:52:23.000000 OmniEvent-0.1.5/OmniEvent/trainer_seq2seq.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     2297 2022-09-13 09:41:11.000000 OmniEvent-0.1.5/OmniEvent/utils.py
-drwxrwxr-x   0 ph        (1004) ph        (1004)        0 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent.egg-info/
--rw-rw-r--   0 ph        (1004) ph        (1004)    22817 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent.egg-info/PKG-INFO
--rw-rw-r--   0 ph        (1004) ph        (1004)     1453 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent.egg-info/SOURCES.txt
--rw-rw-r--   0 ph        (1004) ph        (1004)        1 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent.egg-info/dependency_links.txt
--rw-rw-r--   0 ph        (1004) ph        (1004)      153 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent.egg-info/requires.txt
--rw-rw-r--   0 ph        (1004) ph        (1004)       10 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/OmniEvent.egg-info/top_level.txt
--rw-rw-r--   0 ph        (1004) ph        (1004)    22817 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/PKG-INFO
--rw-rw-r--   0 ph        (1004) ph        (1004)    21255 2022-09-13 09:14:39.000000 OmniEvent-0.1.5/README.md
--rw-rw-r--   0 ph        (1004) ph        (1004)      926 2022-09-13 09:50:59.000000 OmniEvent-0.1.5/pyproject.toml
--rw-rw-r--   0 ph        (1004) ph        (1004)       38 2022-09-13 09:51:36.000000 OmniEvent-0.1.5/setup.cfg
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/
+-rw-rw-r--   0 ph        (1004) ph        (1004)     1049 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/LICENSE
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.582532 OmniEvent-0.1.6/OmniEvent/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/__init__.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/aggregation/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/aggregation/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    20012 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/aggregation/aggregation.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    13142 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/arguments.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/backbone/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/backbone/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    14972 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/backbone/backbone.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/evaluation/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    27628 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/convert_format.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    15442 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/dump_result.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    18870 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/metric.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    20868 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/utils.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/head/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/head/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     2297 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/head/classification.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    13128 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/head/crf.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)      508 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/head/head.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     5354 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/infer.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/infer_module/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/infer_module/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     1755 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/infer_module/io_format.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     9832 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/infer_module/seq2seq.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/OmniEvent/input_engineering/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    21674 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/base_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    18195 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/input_utils.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    11310 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/mrc_converter.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    20815 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/mrc_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    14875 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/seq2seq_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    13751 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/sequence_labeling_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    18459 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/token_classification_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    11756 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/tokenizer.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    12996 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/whitespace_tokenizer.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/OmniEvent/model/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/model/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    12627 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/model/constraint_decoding.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     2342 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/model/label_smoother_sum.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    12488 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/model/model.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    10211 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/trainer.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    18172 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/trainer_seq2seq.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     2300 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/utils.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent.egg-info/
+-rw-rw-r--   0 ph        (1004) ph        (1004)    22831 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/PKG-INFO
+-rw-rw-r--   0 ph        (1004) ph        (1004)     1473 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/SOURCES.txt
+-rw-rw-r--   0 ph        (1004) ph        (1004)        1 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/dependency_links.txt
+-rw-rw-r--   0 ph        (1004) ph        (1004)      153 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/requires.txt
+-rw-rw-r--   0 ph        (1004) ph        (1004)       10 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/top_level.txt
+-rw-rw-r--   0 ph        (1004) ph        (1004)    22831 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/PKG-INFO
+-rw-rw-r--   0 ph        (1004) ph        (1004)    21269 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/README.md
+-rw-rw-r--   0 ph        (1004) ph        (1004)      926 2023-05-15 04:52:34.000000 OmniEvent-0.1.6/pyproject.toml
+-rw-rw-r--   0 ph        (1004) ph        (1004)       38 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/setup.cfg
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/tests/
+-rw-rw-r--   0 ph        (1004) ph        (1004)      780 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/tests/test_infer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `OmniEvent-0.1.5/LICENSE` & `OmniEvent-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/aggregation/aggregation.py` & `OmniEvent-0.1.6/OmniEvent/aggregation/aggregation.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,18 +31,20 @@
     else:
         raise ValueError("Invaild %s aggregation method" % config.aggregation)
 
 
 def aggregate(config,
               method,
               hidden_states: torch.Tensor,
+              attention_mask: torch.Tensor,
               trigger_left: torch.Tensor,
               trigger_right: torch.Tensor,
               argument_left: torch.Tensor,
-              argument_right: torch.Tensor):
+              argument_right: torch.Tensor,
+              embeddings: Optional[torch.Tensor]=None):
     """Aggregates information to each position.
 
     Aggregates information to each position. The aggregation methods include selecting the "cls"s' representations,
     selecting the markers' representations, max-pooling, and dynamic multi-pooling.
 
     Args:
         config:
@@ -67,15 +69,15 @@
         if argument_left is not None:
             return method(hidden_states, argument_left, argument_right)
         else:
             return method(hidden_states, trigger_left, trigger_right)
     elif config.aggregation == "max_pooling":
         return method(hidden_states)
     elif config.aggregation == "dynamic_pooling":
-        return method(hidden_states, trigger_left, argument_left)
+        return method(hidden_states, attention_mask, trigger_left, embeddings, argument_left, argument_right)
     else:
         raise ValueError("Invaild %s aggregation method" % config.aggregation)
 
 
 def max_pooling(hidden_states: torch.Tensor) -> torch.Tensor:
     """Applies the max-pooling operation over the sentence representation.
 
@@ -158,15 +160,15 @@
     """
     def __init__(self,
                  config) -> None:
         """Constructs a `DynamicPooling`."""
         super(DynamicPooling, self).__init__()
         self.dense = nn.Linear(config.hidden_size*config.head_scale, config.hidden_size*config.head_scale)
         self.activation = nn.Tanh()
-        self.dropout = nn.Dropout()
+        self.dropout = nn.Dropout(p=0.2)
     
     def get_mask(self,
                  position: torch.Tensor,
                  batch_size: int,
                  seq_length: int,
                  device: str) -> torch.Tensor:
         """Returns the mask indicating whether the token is padded or not."""
@@ -174,52 +176,89 @@
         for i in range(batch_size):
             mask = torch.zeros((seq_length), dtype=torch.int16, device=device)
             mask[:int(position[i])] = 1 
             all_masks.append(mask.to(torch.bool))
         all_masks = torch.stack(all_masks, dim=0)
         return all_masks
 
+    def get_lexical_level_features(self, embeddings, position, max_seq_length):
+        llf_idx = torch.stack([position-1, position, position+1], dim=0).to(torch.long)
+        llf_idx[0] = llf_idx[0] * (llf_idx[0] != -1) + (position+2) * (llf_idx[0] == -1)
+        llf_idx[2] = llf_idx[2] * (llf_idx[2] != max_seq_length) + (position-2) * (llf_idx[2] == max_seq_length)
+        features = []
+        for i in range(3):
+            features.append(embeddings[torch.arange(embeddings.shape[0]), llf_idx[i]])
+        features = torch.cat(features, dim=-1)
+        return features
+
+    def get_argument_lexical_features(self, embeddings, start, end, max_seq_length):
+        mid_features = []
+        for i in range(start.shape[0]):
+            mid_features.append(torch.mean(embeddings[i, start[i]:end[i]+1], dim=0))
+        mid_features = torch.stack(mid_features, dim=0)
+        
+        llf_idx = torch.stack([start-1, end+1], dim=0).to(torch.long)
+        llf_idx[0] = llf_idx[0] * (llf_idx[0] != -1) + (end+2) * (llf_idx[0] == -1)
+        llf_idx[1] = llf_idx[1] * (llf_idx[1] != max_seq_length) + (start-2) * (llf_idx[1] == max_seq_length)
+        features = [mid_features]
+        for i in range(2):
+            features.append(embeddings[torch.arange(embeddings.shape[0]), llf_idx[i]])
+        features = torch.cat(features, dim=-1)
+        return features
+
     def max_pooling(self,
                     hidden_states: torch.Tensor,
                     mask: torch.Tensor) -> torch.Tensor:
         """Conducts the max-pooling operation on the hidden states."""
+        # import pdb; pdb.set_trace()
         batch_size, seq_length, hidden_size = hidden_states.size()
-        conved = hidden_states.transpose(1, 2)
-        conved = conved.transpose(0, 1)
-        states = (conved * mask).transpose(0, 1)
-        states += torch.ones_like(states)
-        pooled_states = F.max_pool1d(input=states, kernel_size=seq_length).contiguous().view(batch_size, hidden_size)
-        pooled_states -= torch.ones_like(pooled_states)
+        mask = mask.unsqueeze(2)
+        states = hidden_states * mask + mask * 100
+        pooled_states = torch.max(states, dim=1)[0]
+        pooled_states -= 100
         return pooled_states
 
     def forward(self, 
                 hidden_states: torch.Tensor, 
+                attention_mask: torch.Tensor,
                 trigger_position: torch.Tensor, 
-                argument_position: Optional[torch.Tensor] = None) -> torch.Tensor:
+                embeddings: Optional[torch.Tensor] = None,
+                argument_left: Optional[torch.Tensor] = None,
+                argument_right: Optional[torch.Tensor] = None,) -> torch.Tensor:
         """Conducts the dynamic multi-pooling process on the hidden states."""
         batch_size, seq_length = hidden_states.size()[:2]
         trigger_mask = self.get_mask(trigger_position, batch_size, seq_length, hidden_states.device)
-        if argument_position is not None:
-            argument_mask = self.get_mask(argument_position, batch_size, seq_length, hidden_states.device)
-            left_mask = torch.logical_and(trigger_mask, argument_mask).to(torch.float32) 
-            middle_mask = torch.logical_xor(trigger_mask, argument_mask).to(torch.float32) 
-            right_mask = 1 - torch.logical_or(trigger_mask, argument_mask).to(torch.float32)
+        if embeddings is not None:
+            lexical_features = self.get_lexical_level_features(embeddings, trigger_position, hidden_states.size(1))
+        if argument_left is not None:
+            if embeddings is not None:
+                lexical_features = self.get_argument_lexical_features(embeddings, argument_left, argument_right, hidden_states.size(1))
+                # lexical_features = self.get_lexical_level_features(embeddings, argument_left, hidden_states.size(1))
+            argument_mask = self.get_mask(argument_left, batch_size, seq_length, hidden_states.device)
+            left_mask = torch.logical_and(trigger_mask, argument_mask).to(torch.float32) * attention_mask
+            middle_mask = torch.logical_xor(trigger_mask, argument_mask).to(torch.float32) * attention_mask
+            right_mask = (1 - torch.logical_or(trigger_mask, argument_mask).to(torch.float32)) * attention_mask
+            # import pdb; pdb.set_trace()
             # pooling 
             left_states = self.max_pooling(hidden_states, left_mask)
             middle_states = self.max_pooling(hidden_states, middle_mask)
             right_states = self.max_pooling(hidden_states, right_mask)
             pooled_output = torch.cat((left_states, middle_states, right_states), dim=-1)
         else:
-            left_mask = trigger_mask.to(torch.float32)
-            right_mask = 1 - left_mask
+            left_mask = trigger_mask.to(torch.float32) * attention_mask
+            right_mask = (1 - left_mask) * attention_mask
             left_states = self.max_pooling(hidden_states, left_mask)
             right_states = self.max_pooling(hidden_states, right_mask)
             pooled_output = torch.cat((left_states, right_states), dim=-1)
-
-        return pooled_output
+        if embeddings is not None:
+            final_output = torch.cat([pooled_output, lexical_features], dim=-1)
+        else:
+            final_output = pooled_output
+        final_output = self.dropout(final_output)
+        return final_output
 
 
 # To do 
 # - Test MOGANED
 class MOGCN(nn.Module):
     """Multi-order Graph Convolutional Network (MOGAN).
```

### Comparing `OmniEvent-0.1.5/OmniEvent/arguments.py` & `OmniEvent-0.1.6/OmniEvent/arguments.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import yaml 
+import json
 import dataclasses
 
+from enum import Enum
 from pathlib import Path 
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, asdict
 from typing import Optional
 from transformers import TrainingArguments, HfArgumentParser
 
 from .utils import check_web_and_convert_path
 
 
 @dataclass
@@ -126,14 +128,53 @@
     )
     mrc_template_id: int = field(
         default=0,
         metadata={
             "help": "Mrc template, 0: role_name, 1: role_name in [trigger], 2: guidelines, 3: guidelines in [trigger]"
         }
     )
+    insert_marker: bool = field(
+        default=True,
+        metadata={
+            "help": "whether insert marker"
+        }
+    )
+    consider_event_type: bool = field(
+        default=False,
+        metadata={
+            "help": "Consider event type as type ids"
+        }
+    )
+    type_marker: bool = field(
+        default=True,
+        metadata={
+            "help": "Whether type specific marker"
+        }
+    )
+
+    def to_dict(self):
+        """
+        Serializes this instance while replace `Enum` by their values (for JSON serialization support). It obfuscates
+        the token values by removing their value.
+        """
+        d = asdict(self)
+        for k, v in d.items():
+            if isinstance(v, Enum):
+                d[k] = v.value
+            if isinstance(v, list) and len(v) > 0 and isinstance(v[0], Enum):
+                d[k] = [x.value for x in v]
+            if k.endswith("_token"):
+                d[k] = f"<{k.upper()}>"
+        return d
+
+    def to_json_string(self):
+        """
+        Serializes this instance to a JSON string.
+        """
+        return json.dumps(self.to_dict(), indent=2)
 
 
 @dataclass
 class ModelArguments:
     """Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
 
     Arguments pertaining to which model/config/tokenizer we are going to fine-tune from, such as the model type, model
@@ -141,15 +182,19 @@
     """
     model_type: str = field(
         metadata={"help": "Model type."}
     )
     model_name_or_path: str = field(
         metadata={"help": "Path to pretrained model or model identifier from huggingface.co/models"}
     )
-    checkpoint_path: str = field(
+    backbone_checkpoint_path: str = field(
+        default=None,
+        metadata={"help": "Path to pretrained model or model identifier"}
+    )
+    model_checkpoint_path: str = field(
         default=None,
         metadata={"help": "Path to pretrained model or model identifier"}
     )
     hidden_size: int = field(
         default=768,
         metadata={"help": "Hidden size"}
     )
@@ -207,14 +252,20 @@
     )
     position_embedding_dim: int = field(
         default=20,
         metadata={
             "help": "Position embedding dimension for tranditional word vector."
         }
     )
+    type_embedding_dim: int = field(
+        default=5,
+        metadata={
+            "help": "Type embedding dimension for tranditional word vector."
+        }
+    )
     num_position_embeddings: int = field(
         default=512,
         metadata={
             "help": "Number of position embeddings."
         }
     )
     hidden_dropout_prob: float = field(
@@ -225,15 +276,53 @@
     )
     vocab_file: float = field(
         default=None,
         metadata={
             "help": "Path to vocab file."
         }
     )
+    has_type_embeddings: bool = field(
+        default=False,
+        metadata={
+            "help": "type embeddings"
+        }
+    )
+    dropout_after_wordvec: bool = field(
+        default=False,
+        metadata={
+            "help": "Whether dropout after word embedding"
+        }
+    )
+    dropout_after_encoder: bool = field(
+        default=False,
+        metadata={
+            "help": "Whether dropout after PLM encoder"
+        }
+    )
 
+    def to_dict(self):
+        """
+        Serializes this instance while replace `Enum` by their values (for JSON serialization support). It obfuscates
+        the token values by removing their value.
+        """
+        d = asdict(self)
+        for k, v in d.items():
+            if isinstance(v, Enum):
+                d[k] = v.value
+            if isinstance(v, list) and len(v) > 0 and isinstance(v[0], Enum):
+                d[k] = [x.value for x in v]
+            if k.endswith("_token"):
+                d[k] = f"<{k.upper()}>"
+        return d
+
+    def to_json_string(self):
+        """
+        Serializes this instance to a JSON string.
+        """
+        return json.dumps(self.to_dict(), indent=2)
 
 
 @dataclass 
 class TrainingArguments(TrainingArguments):
     """Arguments pertaining to the configurations in the training process.
 
     Arguments pertaining to the configurations in the training process, such as the random seed, task name,
```

### Comparing `OmniEvent-0.1.5/OmniEvent/backbone/backbone.py` & `OmniEvent-0.1.6/OmniEvent/backbone/backbone.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 from transformers import RobertaModel, RobertaTokenizerFast
 from transformers import T5ForConditionalGeneration, T5TokenizerFast
 from transformers import MT5ForConditionalGeneration
 from transformers import BartForConditionalGeneration, BartTokenizerFast
 from transformers.utils import ModelOutput
 
 from ..input_engineering.whitespace_tokenizer import WordLevelTokenizer, load_vocab, VOCAB_FILES_NAMES
-
+from ..arguments import ModelArguments
 
 def get_backbone(model_type: str,
                  model_name_or_path: str,
                  tokenizer_name: str,
                  markers: List[str],
-                 model_args: Optional = None,
+                 model_args: Optional[ModelArguments] = None,
                  new_tokens: Optional[List[str]] = []):
     """Obtains the backbone model and tokenizer.
 
     Obtains the backbone model and tokenizer. The backbone model is selected from BERT, RoBERTa, T5, MT5, CNN, and LSTM,
     corresponding to a distinct tokenizer.
 
     Args:
@@ -110,14 +110,18 @@
         else:
             embeddings = np.load(os.path.join(config.vocab_file, VOCAB_FILES_NAMES["vocab_file"].replace("txt", "npy")))
         self.word_embeddings = nn.Embedding.from_pretrained(torch.tensor(embeddings), freeze=False, padding_idx=0)
         self.position_embeddings = nn.Embedding(config.num_position_embeddings, config.position_embedding_dim)
         self.register_buffer("position_ids", torch.arange(config.num_position_embeddings).expand((1, -1)))
         self.dropout = nn.Dropout(config.hidden_dropout_prob)
         self.resize_token_embeddings(vocab_size)
+        self.config = config
+        # event type embeddings
+        if config.has_type_embeddings:
+            self.type_embeddings = nn.Embedding(config.num_types, config.type_embedding_dim)
 
     def resize_token_embeddings(self,
                                 vocab_size: int) -> None:
         """Resizes the embeddings from the pre-trained embedding dimension to pre-defined embedding size."""
         if len(self.word_embeddings.weight) > vocab_size:
             raise ValueError("Invalid vocab_size %d < original vocab size." % vocab_size)
         elif len(self.word_embeddings.weight) == vocab_size:
@@ -131,25 +135,30 @@
                     self.word_embeddings.weight.data,
                     average_embedding.expand(num_added_token, embedding_dim)
                 )
             ))
 
     def forward(self,
                 input_ids: torch.Tensor,
-                position_ids: Optional[torch.Tensor] = None) -> torch.Tensor:
+                token_type_ids: Optional[torch.Tensor] = None,
+                position: Optional[torch.Tensor] = None) -> torch.Tensor:
         """Generates word embeddings and position embeddings and concatenates them together."""
         input_shape = input_ids.size()
         batch_size, seq_length = input_shape[0], input_shape[1]
-        if position_ids is None:
-            position_ids = self.position_ids[:, :seq_length].expand(batch_size, seq_length)
+        position_ids = self.position_ids[:, :seq_length].expand(batch_size, seq_length)
+        if position is not None:
+            position_ids = torch.abs(position_ids - position.unsqueeze(1)).to(torch.long)
         # input embeddings & position embeddings 
         inputs_embeds = self.word_embeddings(input_ids)
         position_embeds = self.position_embeddings(position_ids)
         embeds = torch.cat((inputs_embeds, position_embeds), dim=-1)
-        embeds = self.dropout(embeds)
+        if token_type_ids is not None and self.config.has_type_embeddings:
+            embeds = torch.cat((embeds, self.type_embeddings(token_type_ids)), dim=-1)
+        if self.config.dropout_after_wordvec:
+            embeds = self.dropout(embeds)
         return embeds
 
 
 class Output(ModelOutput):
     """A class for the model's output, containing the hidden states of the sequence."""
     last_hidden_state: torch.Tensor = None
 
@@ -175,35 +184,38 @@
                  vocab_size: int,
                  kernel_size: Optional[int] = 3,
                  padding_size: Optional[int] = 1) -> None:
         """Constructs a `CNN`."""
         super(CNN, self).__init__()
         self.config = config
         self.embedding = WordEmbedding(config, vocab_size)
-        self.conv = nn.Conv1d(config.word_embedding_dim + config.position_embedding_dim,
+        in_channels = config.word_embedding_dim + config.position_embedding_dim + config.type_embedding_dim if config.has_type_embeddings else \
+                        config.word_embedding_dim + config.position_embedding_dim
+        self.conv = nn.Conv1d(in_channels,
                               config.hidden_size,
                               kernel_size,
                               padding=padding_size)
         self.dropout = nn.Dropout(config.hidden_dropout_prob)
 
     def resize_token_embeddings(self,
                                 vocab_size: int) -> None:
         """Resizes the embeddings from the pre-trained embedding dimension to pre-defined embedding size."""
         self.embedding.resize_token_embeddings(vocab_size)
 
     def forward(self,
                 input_ids: torch.Tensor,
                 attention_mask: torch.Tensor,
-                token_type_ids: torch.Tensor,
+                token_type_ids: Optional[torch.Tensor] = None,
+                position: Optional[torch.Tensor] = None,
                 return_dict: Optional[bool] = True) -> Union[Output, Tuple[torch.Tensor]]:
         """Conducts the convolution operations on the input tokens."""
-        x = self.embedding(input_ids)  # (B, L, H)
+        x = self.embedding(input_ids, token_type_ids, position)  # (B, L, H)
         x = x.transpose(1, 2)  # (B, H, L)
         x = F.relu(self.conv(x).transpose(1, 2))  # (B, H, L)
-        x = self.dropout(x)
+        # x = self.dropout(x)
         if return_dict:
             return Output(last_hidden_state=x)
         else:
             return x
 
 
 class LSTM(nn.Module):
@@ -254,25 +266,26 @@
         sorted_input_ids = input_ids[indices]
         return sorted_input_ids, sorted_input_lengths, desorted_indices
 
     def forward(self,
                 input_ids: torch.Tensor,
                 attention_mask: torch.Tensor,
                 token_type_ids: torch.Tensor,
+                position: Optional[torch.Tensor] = None,
                 return_dict: Optional[bool] = True):
         """Forward propagation of a LSTM network."""
         # add a pseudo input of max_length
         add_pseudo = max(torch.sum(attention_mask, dim=-1).tolist()) != input_ids.shape[1]
         if add_pseudo:
             input_ids = torch.cat((torch.zeros_like(input_ids[0]).unsqueeze(0), input_ids), dim=0)
             attention_mask = torch.cat((torch.ones_like(attention_mask[0]).unsqueeze(0), attention_mask), dim=0)
         input_length = torch.sum(attention_mask, dim=-1).to(torch.long)
         sorted_input_ids, sorted_seq_length, desorted_indices = self.prepare_pack_padded_sequence(input_ids,
                                                                                                   input_length)
-        x = self.embedding(sorted_input_ids)  # (B, L, H)
+        x = self.embedding(sorted_input_ids, position)  # (B, L, H)
         packed_embedded = nn.utils.rnn.pack_padded_sequence(x, sorted_seq_length.cpu(), batch_first=True)
         self.rnn.flatten_parameters()
         packed_output, (hidden, cell) = self.rnn(packed_embedded)
         output, _ = nn.utils.rnn.pad_packed_sequence(packed_output, batch_first=True)
         x = output[desorted_indices]
         if add_pseudo:
             x = self.dropout(x)[1:, :, :]  # remove the pseudo input
```

### Comparing `OmniEvent-0.1.5/OmniEvent/evaluation/convert_format.py` & `OmniEvent-0.1.6/OmniEvent/evaluation/convert_format.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import numpy as np
 
 from typing import List, Dict, Union, Tuple
 from sklearn.metrics import f1_score
-from .metric import select_start_position, compute_unified_micro_f1
+from .metric import select_start_position, compute_unified_micro_f1, f1_score_overall_with_type
 from ..input_engineering.input_utils import (
     get_left_and_right_pos,
     check_pred_len,
     get_ed_candidates,
     get_eae_candidates,
     get_event_preds,
     get_plain_label,
@@ -19,15 +19,16 @@
 def get_pred_per_mention(pos_start: int,
                          pos_end: int,
                          preds: List[Union[str, Tuple[str, str]]],
                          id2label: Dict[int, str] = None,
                          label: str = None,
                          label2id: Dict[str, int] = None,
                          text: str = None,
-                         paradigm: str = "sl") -> str:
+                         paradigm: str = "sl",
+                         task: str = "EAE") -> str:
     """Get the predicted event type or argument role for each mention via the predictions of different paradigms.
 
     The predictions of Sequence Labeling, Seq2Seq, MRC paradigms are not aligned to each word. We need to convert the
     paradigm-dependent predictions to word-level for the unified evaluation. This function is designed to get the
     prediction for each single mention, given the paradigm-dependent predictions.
 
     Args:
@@ -54,14 +55,20 @@
     if paradigm == "sl":
         # sequence labeling paradigm
         if pos_start == pos_end or\
                 pos_end > len(preds) or \
                 id2label[int(preds[pos_start])] == "O" or \
                 id2label[int(preds[pos_start])].split("-")[0] != "B":
             return "NA"
+        if pos_end < len(preds):
+            if id2label[int(preds[pos_end-1])] == id2label[int(preds[pos_end])]:
+                return "NA"
+        for pos in range(pos_start+1, pos_end):
+            if id2label[int(preds[pos])][0] != "I":
+                return "NA"
 
         predictions = set()
         for pos in range(pos_start, pos_end):
             _pred = id2label[int(preds[pos])][2:]
             predictions.add(_pred)
 
         if len(predictions) > 1:
@@ -87,24 +94,44 @@
         if (word, pred_label) in preds:
             preds.remove((word, pred_label))
 
         return pred_label
 
     elif paradigm == "mrc":
         # mrc paradigm
-        predictions = []
-        for pred in preds:
-            if pred[1] == (pos_start, pos_end - 1):
-                pred_role = pred[0].split("_")[-1]
-                predictions.append(pred_role)
-
-        if label in predictions:
-            return label
+        if task == "EAE":
+            # select the pred with the lowest non_na_prob
+            filtered_preds = []
+            for pred in preds:
+                assert pred[0].split("_")[0] == label
+                if pred[0].split("_")[0] == label:
+                    filtered_preds.append(pred)
+            if len(filtered_preds) == 0:
+                return "NA"
+            filtered_preds = sorted(filtered_preds, key=lambda item: item[2])
+            for pred in filtered_preds:
+                if pred[1] == (pos_start, pos_end - 1):
+                    pred_role = pred[0].split("_")[-1]
+                    return pred_role
+            return "NA"
+        elif task == "ED":
+            # sequence labeling paradigm
+            if pos_start == pos_end or \
+                    pos_end > len(preds):
+                return "NA"
+            predictions = set()
+            for pos in range(pos_start, pos_end):
+                _pred = id2label[int(preds[pos])]
+                predictions.add(_pred)
+            if len(predictions) > 1:
+                return "NA"
+            else:
+                return list(predictions)[0]
         else:
-            return predictions[0] if predictions else "NA"
+            raise NotImplementedError
     else:
         raise NotImplementedError
 
 
 def get_ace2005_trigger_detection_sl(preds: np.array,
                                      labels: np.array,
                                      data_file: str,
@@ -151,16 +178,16 @@
             # loop for converting
             for candidate in candidates:
                 left_pos, right_pos = get_left_and_right_pos(text=item["text"], trigger=candidate, language=language)
                 pred = get_pred_per_mention(left_pos, right_pos, preds[i], data_args.id2type)
                 results.append(pred)
 
     if "events" in item:
-        micro_f1 = compute_unified_micro_f1(label_names=label_names, results=results)
-        logger.info("{} test performance after converting: {}".format(data_args.dataset_name, micro_f1))
+        metric_results = compute_unified_micro_f1(label_names=label_names, results=results)
+        logger.info("{} test performance after converting: {}".format(data_args.dataset_name, metric_results))
 
     return results
 
 
 def get_ace2005_argument_extraction_sl(preds: np.array,
                                        labels: np.array,
                                        data_file: str,
@@ -195,14 +222,15 @@
     golden_trigger = data_args.golden_trigger
 
     # pred events
     event_preds = get_event_preds(pred_file=data_args.test_pred_file)
 
     # get per-word predictions
     preds, labels = select_start_position(preds, labels, False)
+    golden_types, pred_types = [], []
     results = []
     label_names = []
     with open(data_file, "r", encoding="utf-8") as f:
         trigger_idx = 0
         eae_instance_idx = 0
         lines = f.readlines()
         for line in lines:
@@ -222,21 +250,20 @@
                         check_pred_len(pred=preds[eae_instance_idx], item=item, language=language)
 
                     candidates, label_names_per_trigger = get_eae_candidates(item=item, trigger=trigger)
                     label_names.extend(label_names_per_trigger)
 
                     # loop for converting
                     for candi in candidates:
-                        if true_type == pred_type:
-                            # get word positions
-                            left_pos, right_pos = get_left_and_right_pos(text=text, trigger=candi, language=language)
-                            # get predictions
-                            pred = get_pred_per_mention(left_pos, right_pos, preds[eae_instance_idx], data_args.id2role)
-                        else:
-                            pred = "NA"
+                        golden_types.append(true_type)
+                        pred_types.append(pred_type)
+                        # get word positions
+                        left_pos, right_pos = get_left_and_right_pos(text=text, trigger=candi, language=language)
+                        # get predictions
+                        pred = get_pred_per_mention(left_pos, right_pos, preds[eae_instance_idx], data_args.id2role)
                         # record results
                         results.append(pred)
                     eae_instance_idx += 1
 
             # negative triggers
             for trigger in item["negative_triggers"]:
                 true_type = "NA"
@@ -249,31 +276,93 @@
                             check_pred_len(pred=preds[eae_instance_idx], item=item, language=language)
 
                         candidates, label_names_per_trigger = get_eae_candidates(item=item, trigger=trigger)
                         label_names.extend(label_names_per_trigger)
 
                         # loop for converting
                         for candi in candidates:
+                            golden_types.append(true_type)
+                            pred_types.append(pred_type)
                             # get word positions
                             left_pos, right_pos = get_left_and_right_pos(text=text, trigger=candi, language=language)
                             # get predictions
                             pred = get_pred_per_mention(left_pos, right_pos, preds[eae_instance_idx], data_args.id2role)
                             # record results
                             results.append(pred)
 
                         eae_instance_idx += 1
 
         assert len(preds) == eae_instance_idx
         
-    pos_labels = list(set(label_names))
-    pos_labels.remove("NA")
-    micro_f1 = f1_score(label_names, results, labels=pos_labels, average="micro") * 100.0
-
+    P, R, F1 = f1_score_overall_with_type(results, label_names, pred_types, golden_types)
+    metric_results = {
+        "precision": P * 100,
+        "recall": R * 100,
+        "micro_f1": F1 * 100
+    }
     logger.info('Number of Instances: {}'.format(eae_instance_idx))
-    logger.info("{} test performance after converting: {}".format(data_args.dataset_name, micro_f1))
+    logger.info("{} test performance after converting: {}".format(data_args.dataset_name, metric_results))
+    return results
+
+
+def get_ace2005_trigger_detection_mrc(preds: np.array,
+                                     labels: np.array,
+                                     data_file: str,
+                                     data_args,
+                                     is_overflow) -> List[str]:
+    """Obtains the event detection prediction results of the ACE2005 dataset based on the sequence labeling paradigm.
+
+    Obtains the event detection prediction results of the ACE2005 dataset based on the sequence labeling paradigm,
+    predicting the labels and calculating the micro F1 score based on the predictions and labels.
+
+    Args:
+        preds (`np.array`):
+            A list of strings indicating the predicted types of the instances.
+        labels (`np.array`):
+            A list of strings indicating the actual labels of the instances.
+        data_file (`str`):
+            A string indicating the path of the testing data file.
+        data_args:
+            The pre-defined arguments for data processing.
+        is_overflow:
+
+
+    Returns:
+        results (`List[str]`):
+            A list of strings indicating the prediction results of event triggers.
+    """
+    # get per-word predictions
+    preds, _ = select_start_position(preds, labels, False)
+    results = []
+    label_names = []
+    language = data_args.language
+
+    with open(data_file, "r", encoding='utf-8') as f:
+        lines = f.readlines()
+        for i, line in enumerate(lines):
+            item = json.loads(line.strip())
+
+            if not is_overflow[i]:
+                check_pred_len(pred=preds[i], item=item, language=language)
+
+            candidates, label_names_per_item = get_ed_candidates(item=item)
+            label_names.extend(label_names_per_item)
+
+            # loop for converting
+            for candidate in candidates:
+                left_pos, right_pos = get_left_and_right_pos(text=item["text"], trigger=candidate, language=language)
+                pred = get_pred_per_mention(left_pos, right_pos, preds[i], data_args.id2type, 
+                                            paradigm="mrc", task="ED")
+                results.append(pred)
+
+    if "events" in item:
+        metric_results = compute_unified_micro_f1(label_names=label_names, results=results)
+        logger.info("{} test performance after converting: {}".format(data_args.dataset_name, metric_results))
+
+
     return results
 
 
 def get_ace2005_argument_extraction_mrc(preds, labels, data_file, data_args, is_overflow):
     """Obtains the event argument extraction results of the ACE2005 dataset based on the MRC paradigm.
 
     Obtains the event argument extraction prediction results of the ACE2005 dataset based on the MRC paradigm,
@@ -301,90 +390,99 @@
     golden_trigger = data_args.golden_trigger
     language = data_args.language
 
     # pred events
     event_preds = get_event_preds(pred_file=data_args.test_pred_file)
 
     # get per-word predictions
+    golden_types, pred_types = [], []
     results = []
     all_labels = []
     with open(data_args.test_file, "r", encoding="utf-8") as f:
         trigger_idx = 0
         eae_instance_idx = 0
         lines = f.readlines()
-        for line in lines:
+        for idx, line in enumerate(lines):
             item = json.loads(line.strip())
             text = item["text"]
 
-            # preds per index 
-            preds_per_idx = []
-            for pred in preds:
-                if pred[-1] == trigger_idx:
-                    preds_per_idx.append(pred)
-
             for event in item["events"]:
                 for trigger in event["triggers"]:
                     true_type = event["type"]
                     pred_type = true_type if golden_trigger or event_preds is None else event_preds[trigger_idx]
                     trigger_idx += 1
+                    # preds per index
+                    preds_per_idx = []
+                    for pred in preds:
+                        if pred[-1] == trigger_idx - 1:
+                            preds_per_idx.append(pred)
 
                     if eval_mode in ['default', 'loose']:
                         if pred_type == "NA":
                             continue
 
                     # get candidates 
                     candidates, labels_per_idx = get_eae_candidates(item, trigger)
                     all_labels.extend(labels_per_idx)
 
                     # loop for converting
                     for cid, candi in enumerate(candidates):
-                        label = labels_per_idx[cid]
-                        if pred_type == true_type:
-                            # get word positions
-                            left_pos, right_pos = get_left_and_right_pos(text=text, trigger=candi, language=language)
-                            # get predictions
-                            pred_role = get_pred_per_mention(pos_start=left_pos, pos_end=right_pos, preds=preds_per_idx,
-                                                             label=label, paradigm='mrc')
-                        else:
-                            pred_role = "NA"
+                        golden_types.append(true_type)
+                        pred_types.append(pred_type)
+                        label = pred_type
+                        # get word positions
+                        left_pos, right_pos = get_left_and_right_pos(text=text, trigger=candi, language=language)
+                        # get predictions
+                        pred_role = get_pred_per_mention(pos_start=left_pos, pos_end=right_pos, preds=preds_per_idx,
+                                                            label=label, paradigm='mrc')
                         # record results
                         results.append(pred_role)
                     eae_instance_idx += 1
 
             # negative triggers
             for trigger in item["negative_triggers"]:
                 true_type = "NA"
                 pred_type = true_type if golden_trigger or event_preds is None else event_preds[trigger_idx]
                 trigger_idx += 1
 
+                # preds per index 
+                preds_per_idx = []
+                for pred in preds:
+                    if pred[-1] == trigger_idx - 1:
+                        preds_per_idx.append(pred)
+
                 if eval_mode in ['default', 'strict']:  # loose mode has no neg
                     if pred_type != "NA":
                         # get candidates
                         candidates, labels_per_idx = get_eae_candidates(item, trigger)
                         all_labels.extend(labels_per_idx)
 
                         # loop for converting
                         for candi in candidates:
-                            label = "NA"
+                            golden_types.append(true_type)
+                            pred_types.append(pred_type)
+                            label = pred_type
                             # get word positions
                             left_pos, right_pos = get_left_and_right_pos(text=text, trigger=candi, language=language)
                             # get predictions
                             pred_role = get_pred_per_mention(pos_start=left_pos, pos_end=right_pos, preds=preds_per_idx,
                                                              label=label, paradigm='mrc')
                             # record results
                             results.append(pred_role)
 
                         eae_instance_idx += 1
         
-    pos_labels = list(data_args.role2id.keys())
-    pos_labels.remove("NA")
-    micro_f1 = f1_score(all_labels, results, labels=pos_labels, average="micro") * 100.0
-
+    P, R, F1 = f1_score_overall_with_type(results, all_labels, pred_types, golden_types)
+    metric_results = {
+        "precision": P * 100,
+        "recall": R * 100,
+        "micro_f1": F1 * 100
+    }
     logger.info('Number of Instances: {}'.format(eae_instance_idx))
-    logger.info("{} test performance after converting: {}".format(data_args.dataset_name, micro_f1))
+    logger.info("{} test performance after converting: {}".format(data_args.dataset_name, metric_results))
     return results
 
 
 def get_ace2005_trigger_detection_s2s(preds, labels, data_file, data_args, is_overflow):
     """Obtains the event detection prediction results of the ACE2005 dataset based on the Seq2Seq paradigm.
 
     Obtains the event detection prediction results of the ACE2005 dataset based on the Seq2Seq paradigm,
```

### Comparing `OmniEvent-0.1.5/OmniEvent/evaluation/dump_result.py` & `OmniEvent-0.1.6/OmniEvent/evaluation/dump_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,53 +5,14 @@
 from collections import defaultdict
 from typing import List, Dict, Union, Tuple
 from .convert_format import get_pred_per_mention
 from .metric import select_start_position
 from ..input_engineering.input_utils import check_pred_len, get_left_and_right_pos
 
 
-<<<<<<< HEAD
-def get_pred_per_mention(pos_start: int,
-                         pos_end: int,
-                         preds: List[str],
-                         id2label: Dict[int, str]) -> str:
-    """Get the predicted event type or argument role for each mention in Sequence Labeling (SL) paradigm.
-
-    The predictions of Sequence Labeling (SL) paradigm are sequences of tokens. This function is get the prediction for
-    each single mention, given the sequence predictions.
-
-    Args:
-        pos_start (`int`):
-            The start position of the mention in the sequence of tokens.
-        pos_end (`int`):
-            The end position of the mention in the sequence of tokens.
-        preds (`List[str]`):
-            The predictions of the sequence of tokens.
-        id2label (`Dict[int, str]`):
-            A dictionary that contains the mapping from id to textual label.
-
-    Returns:
-        A string which represents the predicted label.
-    """
-    if pos_start == pos_end or \
-            pos_end > len(preds) or \
-            id2label[int(preds[pos_start])] == "O" or \
-            id2label[int(preds[pos_start])].split("-")[0] != "B":
-        return "NA"
-    predictions = set()
-    for pos in range(pos_start, pos_end):
-        _pred = id2label[int(preds[pos])][2:]
-        predictions.add(_pred)
-    if len(predictions) > 1:
-        return "NA"
-    return list(predictions)[0]
-
-
-=======
->>>>>>> 849862bafe3342e60077401272ebc44f7ce2ddd8
 def get_sentence_arguments(input_sentence: List[Dict[str, str]]) -> List[Dict[str, str]]:
     """Get the predicted arguments from a sentence in the Sequence Labeling paradigm.
 
     Args:
         input_sentence (`List[Dict[str, str]]`):
             A list of dictionaries each of which contains the word and the corresponding bio-role.
     Returns:
```

### Comparing `OmniEvent-0.1.5/OmniEvent/evaluation/metric.py` & `OmniEvent-0.1.6/OmniEvent/evaluation/metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 
 import torch
 import numpy as np
 
-from sklearn.metrics import f1_score
+from sklearn.metrics import f1_score, precision_score, recall_score
 from seqeval.metrics import f1_score as span_f1_score
+from seqeval.metrics import precision_score as span_precision_score
+from seqeval.metrics import recall_score as span_recall_score
 from seqeval.scheme import IOB2
 from typing import Tuple, Dict, List, Optional, Union
 
 from ..input_engineering.mrc_converter import make_predictions, compute_mrc_F1_cls
 from ..input_engineering.seq2seq_processor import extract_argument
 
 
@@ -25,16 +27,22 @@
 
     Returns:
         micro_f1 (`float`):
             The computation results of F1 score.
     """
     pos_labels = list(set(label_names))
     pos_labels.remove("NA")
+    precision = precision_score(label_names, results, labels=pos_labels, average="micro") * 100.0
+    recall = recall_score(label_names, results, labels=pos_labels, average="micro") * 100.0
     micro_f1 = f1_score(label_names, results, labels=pos_labels, average="micro") * 100.0
-    return micro_f1
+    return {
+        "precision": precision,
+        "recall": recall,
+        "micro_f1": micro_f1
+    }
 
 
 def f1_score_overall(preds: Union[List[str], List[tuple]],
                      labels: Union[List[str], List[tuple]]) -> Tuple[float, float, float]:
     """Computes the overall F1 score of the predictions.
 
     Computes the overall F1 score of the predictions based on the calculation of the overall precision and recall after
@@ -58,14 +66,67 @@
             label_stack.remove(pred)  # one prediction can only be matched to one ground truth.
     precision = true_pos / (len(preds)+1e-10)
     recall = true_pos / (len(labels)+1e-10)
     f1 = 2 * precision * recall / (precision + recall + 1e-10)
     return precision, recall, f1
 
 
+def f1_score_overall_with_type(preds: Union[List[str], List[tuple]],
+                               labels: Union[List[str], List[tuple]],
+                               pred_types: Union[List[str], List[tuple]],
+                               golden_types: Union[List[str], List[tuple]]) -> Tuple[float, float, float]:
+    """Computes the overall F1 score of the predictions.
+
+    Computes the overall F1 score of the predictions based on the calculation of the overall precision and recall after
+    counting the true predictions, in which both the prediction of mention and type are correct.
+
+    Args:
+        preds (`Union[List[str], List[tuple]]`):
+            A list of strings indicating the prediction of labels from the model.
+        labels (`Union[List[str], List[tuple]]`):
+            A list of strings indicating the actual labels obtained from the annotated dataset.
+
+    Returns:
+        precision (`float`), recall (`float`), and f1 (`float`):
+            Three float variables representing the computation results of precision, recall, and F1 score, respectively.
+    """
+    assert len(preds) == len(pred_types)
+    assert len(pred_types) == len(golden_types)
+    def is_NA(x):
+        if isinstance(x,tuple):
+            return (0 in x) or ("NA" in x) or ("None" in x)
+        raise ValueError
+
+    TP, TN, FP, FN = 0, 0, 0, 0
+    for i in range(len(preds)):
+        pred = (pred_types[i], preds[i])
+        golden = (golden_types[i], labels[i])
+        if pred == golden and not is_NA(pred):
+            TP += 1
+        elif pred != golden:
+            if is_NA(pred) and not is_NA(golden):
+                FN += 1
+            elif is_NA(golden) and not is_NA(pred):
+                FP += 1
+            elif (not is_NA(golden)) and (not is_NA(pred)):
+                FN += 1
+                FP += 1
+            else:
+                TN += 1
+        else:
+            TN += 1
+    P = TP / (TP + FP)
+    R = TP / (TP + FN)
+    if P + R == 0:
+        return 0, 0, 0
+    else:
+        F1 = 2 * P * R / (P + R)
+        return P, R, F1
+
+
 def compute_seq_F1(logits: np.ndarray,
                    labels: np.ndarray,
                    **kwargs) -> Dict[str, float]:
     """Computes the F1 score of the Sequence-to-Sequence (Seq2Seq) paradigm.
 
     Computes the F1 score of the  Sequence-to-Sequence (Seq2Seq) paradigm. The predictions of the model are firstly
     decoded into strings, then the overall F1 score of the prediction could be calculated.
@@ -210,20 +271,38 @@
     # if the type is wrongly predicted, set arguments NA
     if training_args.task_name == "EAE":
         pred_types = training_args.data_for_evaluation["pred_types"]
         true_types = training_args.data_for_evaluation["true_types"]
         assert len(pred_types) == len(true_types)
         assert len(pred_types) == len(final_labels)
         for i, (pred, true) in enumerate(zip(pred_types, true_types)):
-            if pred != true:
-                final_preds[i] = [id2label[0]] * len(final_preds[i])  # set to NA
+            if pred in [0, "NA", "None"] or true in [0, "NA", "None"]:
+                if pred in [0, "NA", "None"]:
+                    final_preds[i] = [id2label[0]] * len(final_preds[i])
+                if true in [0, "NA", "None"]:
+                    final_labels[i] = [id2label[0]] * len(final_labels[i])
+            else:
+                if pred != true:
+                    seq_pred = []
+                    for j in range(len(final_preds[i])):
+                        if final_preds[i][j] != id2label[0]:
+                            seq_pred.append(final_preds[i][j]+"-Error")
+                        else:
+                            seq_pred.append(id2label[0])
+                    final_preds[i] = seq_pred
 
+    precision = span_precision_score(final_labels, final_preds, mode='strict', scheme=IOB2) * 100.0
+    recall = span_recall_score(final_labels, final_preds, mode='strict', scheme=IOB2) * 100.0
     micro_f1 = span_f1_score(final_labels, final_preds, mode='strict', scheme=IOB2) * 100.0
-    return {"micro_f1": micro_f1}
-    
+    return {
+        "precision": precision,
+        "recall": recall,
+        "micro_f1": micro_f1
+    }
+
 
 def compute_F1(logits: np.ndarray,
                labels: np.ndarray,
                **kwargs) -> Dict[str, float]:
     """Computes the F1 score of the Token Classification (TC) paradigm.
 
     Computes the F1 score of the Token Classification (TC) paradigm. The prediction of the model is converted into
@@ -243,23 +322,31 @@
     training_args = kwargs["training_args"]
     # if the type is wrongly predicted, set arguments NA
     if training_args.task_name == "EAE":
         pred_types = training_args.data_for_evaluation["pred_types"]
         true_types = training_args.data_for_evaluation["true_types"]
         assert len(pred_types) == len(true_types)
         assert len(pred_types) == len(predictions)
-        for i, (pred, true) in enumerate(zip(pred_types, true_types)):
-            if pred != true:
-                predictions[i] = 0 # set to NA
-        pos_labels = list(set(training_args.role2id.values()))
+        P, R, F1 = f1_score_overall_with_type(predictions, labels, pred_types, true_types)
+        return {
+            "precision": P * 100,
+            "recall": R * 100,
+            "micro_f1": F1 * 100
+        }
     else:
         pos_labels = list(set(training_args.type2id.values()))
-    pos_labels.remove(0)
-    micro_f1 = f1_score(labels, predictions, labels=pos_labels, average="micro") * 100.0
-    return {"micro_f1": micro_f1}
+        pos_labels.remove(0)
+        precision = precision_score(labels, predictions, labels=pos_labels, average="micro") * 100.0
+        recall = recall_score(labels, predictions, labels=pos_labels, average="micro") * 100.0
+        micro_f1 = f1_score(labels, predictions, labels=pos_labels, average="micro") * 100.0
+        return {
+            "precision": precision,
+            "recall": recall,
+            "micro_f1": micro_f1
+        }
 
 
 def softmax(logits: np.ndarray,
             dim: Optional[int] = -1) -> np.ndarray:
     """Conducts the softmax operation on the last dimension.
 
     Conducts the softmax operation on the last dimension and returns a numpy array.
@@ -297,14 +384,48 @@
             A dictionary containing the calculation result of the accuracy.
     """
     predictions = np.argmax(softmax(logits), axis=-1)
     accuracy = (predictions == labels).sum() / labels.shape[0]
     return {"accuracy": accuracy}
 
 
+def compute_mrc_trigger_F1(logits: np.ndarray,
+                    labels: np.ndarray,
+                    **kwargs) -> Dict[str, int]:
+    """Computes the F1 score of the Sequence Labeling (SL) paradigm.
+
+    Computes the F1 score of the Sequence Labeling (SL) paradigm. The prediction of the model is converted into strings,
+    then the overall F1 score of the prediction could be calculated.
+
+    Args:
+        logits (`np.ndarray`):
+            An numpy array of integers containing the predictions from the model to be decoded.
+        labels (`np.ndarray`):
+            An numpy array of integers containing the actual labels obtained from the annotated dataset.
+
+    Returns:
+        `Dict[str: float]`:
+            A dictionary containing the calculation result of F1 score.
+    """
+
+    preds = np.argmax(logits, axis=-1) if len(logits.shape) == 3 else logits
+    training_args = kwargs["training_args"]
+    predictions, labels = select_start_position(preds, labels, True)
+    pos_labels = list(set(training_args.type2id.values()))
+    pos_labels.remove(0)
+    precision = precision_score(labels, predictions, labels=pos_labels, average="micro") * 100.0
+    recall = recall_score(labels, predictions, labels=pos_labels, average="micro") * 100.0
+    micro_f1 = f1_score(labels, predictions, labels=pos_labels, average="micro") * 100.0
+    return {
+        "precision": precision,
+        "recall": recall,
+        "micro_f1": micro_f1
+    }
+
+
 def compute_mrc_F1(logits: np.ndarray,
                    labels: np.ndarray,
                    **kwargs) -> Dict[str, float]:
     """Computes the F1 score of the Machine Reading Comprehension (MRC) method.
 
     Computes the F1 score of the Machine Reading Comprehension (MRC) method. The prediction of the model is firstly
     decoded into strings, then the overall F1 score of the prediction could be calculated.
@@ -317,9 +438,14 @@
 
     Returns:
         `Dict[str: float]`:
             A dictionary containing the calculation result of F1 score.
     """
     start_logits, end_logits = np.split(logits, 2, axis=-1)
     all_predictions, all_labels = make_predictions(start_logits, end_logits, kwargs["training_args"])
-    micro_f1 = compute_mrc_F1_cls(all_predictions, all_labels)
-    return {"micro_f1": micro_f1}
+    precision, recall, micro_f1 = compute_mrc_F1_cls(all_predictions, all_labels)
+    return {
+        "precision": precision,
+        "recall": recall,
+        "micro_f1": micro_f1
+    }
+
```

### Comparing `OmniEvent-0.1.5/OmniEvent/evaluation/utils.py` & `OmniEvent-0.1.6/OmniEvent/evaluation/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from ..trainer import Trainer
 from ..trainer_seq2seq import Seq2SeqTrainer
 from ..arguments import DataArguments, ModelArguments, TrainingArguments
 from ..input_engineering.seq2seq_processor import extract_argument
 from ..input_engineering.base_processor import EDDataProcessor, EAEDataProcessor
 from ..input_engineering.mrc_converter import make_predictions, find_best_thresh
 
-from .convert_format import get_ace2005_trigger_detection_sl, get_ace2005_trigger_detection_s2s
+from .convert_format import (
+    get_ace2005_trigger_detection_sl, 
+    get_ace2005_trigger_detection_s2s,
+    get_ace2005_trigger_detection_mrc
+)
 
 logger = logging.getLogger(__name__)
 
 
 def dump_preds(trainer: Union[Trainer, Seq2SeqTrainer],
                tokenizer: PreTrainedTokenizer,
                data_class: type,
@@ -74,14 +78,16 @@
 
     preds = get_pred_s2s(logits, tokenizer) if model_args.paradigm == "seq2seq" else np.argmax(logits, axis=-1)
 
     if model_args.paradigm == "token_classification":
         pred_labels = [data_args.id2type[pred] for pred in preds]
     elif model_args.paradigm == "sequence_labeling":
         pred_labels = get_ace2005_trigger_detection_sl(preds, labels, data_file, data_args, dataset.is_overflow)
+    elif model_args.paradigm == "mrc":
+        pred_labels = get_ace2005_trigger_detection_mrc(preds, labels, data_file, data_args, dataset.is_overflow)
     elif model_args.paradigm == "seq2seq":
         pred_labels = get_ace2005_trigger_detection_s2s(preds, labels, data_file, data_args, None)
     else:
         raise NotImplementedError
 
     save_path = os.path.join(output_dir, "{}_preds.json".format(mode))
 
@@ -149,24 +155,25 @@
     Returns:
         preds (`List[List[Tuple[str, str]]]`):
             The textual predictions of the Event Type or Argument Role.
             A list of tuple lists, in which each tuple is (argument, role) or (trigger, event_type)
     """
 
     start_logits, end_logits = np.split(logits, 2, axis=-1)
-    all_preds, all_labels = make_predictions(start_logits, end_logits, training_args)
+    all_preds, all_labels = make_predictions(start_logits, end_logits, training_args, use_example_id=False)
 
     all_preds = sorted(all_preds, key=lambda x: x[-2])
     best_na_thresh = find_best_thresh(all_preds, all_labels)
     logger.info("Best thresh founded. %.6f" % best_na_thresh)
 
     final_preds = []
     for argument in all_preds:
         if argument[-2] < best_na_thresh:
-            final_preds.append(argument[:-2] + argument[-1:])  # no na_prob
+            # final_preds.append(argument[:-2] + argument[-1:])  # no na_prob
+            final_preds.append(argument)
 
     return final_preds
 
 
 def predict(trainer: Union[Trainer, Seq2SeqTrainer],
             tokenizer: PreTrainedTokenizer,
             data_class: type,
```

### Comparing `OmniEvent-0.1.5/OmniEvent/head/classification.py` & `OmniEvent-0.1.6/OmniEvent/head/classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
     Attributes:
         classifier (`nn.Linear`):
             An `nn.Linear` layer classifying each logit into its corresponding label.
     """
     def __init__(self, config):
         super(LinearHead, self).__init__()
-        self.classifier = nn.Linear(config.hidden_size*config.head_scale, config.num_labels)
+        if config.model_type == "cnn":
+            self.classifier = nn.Linear(config.hidden_size*config.head_scale+config.word_embedding_dim*3, config.num_labels)
+        else:
+            self.classifier = nn.Linear(config.hidden_size*config.head_scale, config.num_labels)
 
     def forward(self,
                 hidden_state: torch.Tensor) -> torch.Tensor:
         """Classifies hidden states to label distribution."""
         logits = self.classifier(hidden_state)
         return logits
```

### Comparing `OmniEvent-0.1.5/OmniEvent/head/crf.py` & `OmniEvent-0.1.6/OmniEvent/head/crf.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/infer.py` & `OmniEvent-0.1.6/OmniEvent/infer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import os 
-import json 
+import os
+import json
+
+import torch.cuda
+
 from .arguments import (
-    ArgumentParser, 
+    ArgumentParser,
     ModelArguments,
     DataArguments,
     TrainingArguments
 )
 from .model.model import get_model_cls
 from .input_engineering.whitespace_tokenizer import WhitespaceTokenizer
 from .utils import check_web_and_convert_path
@@ -13,22 +16,23 @@
     BertTokenizerFast,
     RobertaTokenizerFast,
     T5TokenizerFast,
     MT5TokenizerFast,
     BartTokenizerFast
 )
 from .infer_module.seq2seq import (
-    do_event_detection, 
+    do_event_detection,
     do_event_argument_extraction,
     get_ed_result,
     get_eae_result,
     prepare_for_eae_from_input,
     prepare_for_eae_from_pred
 )
 
+
 class AttrDict(dict):
     def __init__(self, *args, **kwargs):
         super(AttrDict, self).__init__(*args, **kwargs)
         self.__dict__ = self
 
 
 TOKENIZER_NAME_TO_CLS = {
@@ -48,34 +52,35 @@
     return tokenizer
 
 
 def get_model(model_args, model_name_or_path):
     path = check_web_and_convert_path(model_name_or_path, "model")
     model = get_model_cls(model_args).from_pretrained(path)
     return model
-    
 
-def get_pretrained(model_name_or_path):
+
+def get_pretrained(model_name_or_path, device):
     # config 
     # parser = ArgumentParser((ModelArguments, DataArguments, TrainingArguments))
     # model_args, data_args, training_args = parser.from_pretrained(model_name_or_path)
     # model
     model_args = AttrDict({
         "paradigm": "seq2seq",
         "model_type": "mt5"
     })
     model = get_model(model_args, model_name_or_path)
-    model.cuda()
+    model = model.to(device)
+    # model.cuda()
     # tokenizer 
     tokenizer = get_tokenizer(model_name_or_path)
 
     return model, tokenizer
 
 
-def infer(text, model=None, tokenizer=None, triggers=None, schema="ace", task="ED"):
+def infer(text, model=None, tokenizer=None, triggers=None, schema="ace", task="ED", device='auto'):
     """Infer method.
 
     Args:
         text (`str`): Input plain text.
         triggers (`List[List]`, *optional*): List of triggers in the text. Only useful for EAE. Examples: [(moving, 2, 8), ...]
         schema (`str`): Schema used for ED and EAE. Selected in ['ace', 'kbp', 'ere', 'maven', 'leven', 'duee', 'fewfc']
         task (`str`): Task type. Selected in ['ED', 'EAE', 'EE']
@@ -101,41 +106,49 @@
                 ]
             } 
         ]
     """
     assert schema in ['ace', 'kbp', 'ere', 'maven', 'leven', 'duee', 'fewfc']
     assert task in ['ED', 'EAE', 'EE']
     schema = f"<{schema}>"
+    # get device.
+    if device == 'auto':
+        device = torch.device("cpu")
+        if torch.cuda.is_available():
+            device = 'cuda'
+    else:
+        device = torch.device(device)
+
     if task == "ED":
         if model is None or tokenizer is None:
-            ed_model, ed_tokenizer = get_pretrained("s2s-mt5-ed")
+            ed_model, ed_tokenizer = get_pretrained("s2s-mt5-ed", device)
         else:
             ed_model, ed_tokenizer = model, tokenizer
-        events = do_event_detection(ed_model, ed_tokenizer, [text], [schema])
+        events = do_event_detection(ed_model, ed_tokenizer, [text], [schema], device)
         results = get_ed_result([text], events)
     elif task == "EAE":
         if model is None or tokenizer is None:
-            eae_model, eae_tokenizer = get_pretrained("s2s-mt5-eae")
+            eae_model, eae_tokenizer = get_pretrained("s2s-mt5-eae", device)
         else:
             eae_model, eae_tokenizer = model, tokenizer
         instances = prepare_for_eae_from_input([text], [triggers], [schema])
         arguments = do_event_argument_extraction(eae_model, eae_tokenizer, instances)
         results = get_eae_result(instances, arguments)
     elif task == "EE":
         if model is None or tokenizer is None:
-            ed_model, ed_tokenizer = get_pretrained("s2s-mt5-ed")
-            eae_model, eae_tokenizer = get_pretrained("s2s-mt5-eae")
+            ed_model, ed_tokenizer = get_pretrained("s2s-mt5-ed", device)
+            eae_model, eae_tokenizer = get_pretrained("s2s-mt5-eae", device)
         else:
             ed_model, ed_tokenizer = model[0], tokenizer[0]
             eae_model, eae_tokenizer = model[1], tokenizer[1]
-        events = do_event_detection(ed_model, ed_tokenizer, [text], [schema])
+        events = do_event_detection(ed_model, ed_tokenizer, [text], [schema], device)
         instances = prepare_for_eae_from_pred([text], events, [schema])
         if len(instances[0]["triggers"]) == 0:
             results = [{
                 "text": instances[0]["text"],
                 "events": []
             }]
             return results
-        arguments = do_event_argument_extraction(eae_model, eae_tokenizer, instances)
+        arguments = do_event_argument_extraction(eae_model, eae_tokenizer, instances, device)
         results = get_eae_result(instances, arguments)
     print(results)
     return results
```

### Comparing `OmniEvent-0.1.5/OmniEvent/infer_module/io_format.py` & `OmniEvent-0.1.6/OmniEvent/infer_module/io_format.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/infer_module/seq2seq.py` & `OmniEvent-0.1.6/OmniEvent/infer_module/seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,28 @@
                                        is_split_into_words=True)
         return dict(
             input_ids=torch.tensor(input_context["input_ids"], dtype=torch.long),
             attention_mask=torch.tensor(input_context["attention_mask"], dtype=torch.float32)
         )
 
 
-    def tokenize(self, texts, schemas):
+    def tokenize(self, texts, schemas, device):
         batch = []
         for text, schema in zip(texts, schemas):
             batch.append(self.tokenize_per_instance(text, schema))
         # output batch features 
         output_batch = defaultdict(list)
         for key in batch[0].keys():
             output_batch[key] = torch.stack([x[key] for x in batch], dim=0)
         # truncate
         input_length = int(output_batch["attention_mask"].sum(-1).max())
         for key in ["input_ids", "attention_mask", "token_type_ids"]:
             if key not in output_batch:
                 continue
-            output_batch[key] = output_batch[key][:, :input_length].cuda()
+            output_batch[key] = output_batch[key][:, :input_length].to(device)
         return output_batch
 
 
 class EAEProcessor():
     def __init__(self, tokenizer, max_seq_length=160):
         self.tokenizer = tokenizer 
         self.max_seq_length = max_seq_length
@@ -89,29 +89,29 @@
                                        max_length=self.max_seq_length,
                                        is_split_into_words=True)
         return dict(
             input_ids=torch.tensor(input_context["input_ids"], dtype=torch.long),
             attention_mask=torch.tensor(input_context["attention_mask"], dtype=torch.float32)
         )
 
-    def tokenize(self, instances):
+    def tokenize(self, instances, device):
         batch = []
         for i, instance in enumerate(instances):
             for trigger in instance["triggers"]:
                 batch.append(self.tokenize_per_instance(instance["text"], trigger, instance["schema"]))
         # output batch features 
         output_batch = defaultdict(list)
         for key in batch[0].keys():
             output_batch[key] = torch.stack([x[key] for x in batch], dim=0)
         # truncate
         input_length = int(output_batch["attention_mask"].sum(-1).max())
         for key in ["input_ids", "attention_mask", "token_type_ids"]:
             if key not in output_batch:
                 continue
-            output_batch[key] = output_batch[key][:, :input_length].cuda()
+            output_batch[key] = output_batch[key][:, :input_length].to(device)
         return output_batch
 
 
 def find_position(mention, text):
     char_start = text.index(mention)
     char_end = char_start + len(mention)
     return [char_start, char_end]
@@ -248,32 +248,32 @@
     generated_tokens = model.generate(
         generation_inputs,
         **gen_kwargs,
     )
     return tokenizer.batch_decode(generated_tokens, skip_special_tokens=False)
 
 
-def do_event_detection(model, tokenizer, texts, schemas):
+def do_event_detection(model, tokenizer, texts, schemas, device):
     data_processor = EDProcessor(tokenizer)
-    inputs = data_processor.tokenize(texts, schemas)
+    inputs = data_processor.tokenize(texts, schemas, device)
     decoded_preds = generate(model, tokenizer, inputs)
     def clean_str(x_str):
         for to_remove_token in [tokenizer.eos_token, tokenizer.pad_token]:
             x_str = x_str.replace(to_remove_token, '')
         return x_str.strip()
     pred_triggers = []
     for i, pred in enumerate(decoded_preds):
         pred = clean_str(pred)
         pred_triggers.extend(extract_argument(pred, i))
     return pred_triggers
 
 
-def do_event_argument_extraction(model, tokenizer, instances):
+def do_event_argument_extraction(model, tokenizer, instances, device):
     data_processor = EAEProcessor(tokenizer)
-    inputs = data_processor.tokenize(instances)
+    inputs = data_processor.tokenize(instances, device)
     decoded_preds = generate(model, tokenizer, inputs)
     def clean_str(x_str):
         for to_remove_token in [tokenizer.eos_token, tokenizer.pad_token]:
             x_str = x_str.replace(to_remove_token, '')
         return x_str.strip()
     pred_triggers = []
     for i, pred in enumerate(decoded_preds):
```

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/base_processor.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/base_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def __init__(self,
                  example_id: Union[int, str],
                  input_ids: List[int],
                  attention_mask: List[int],
                  token_type_ids: Optional[List[int]] = None,
                  trigger_left: Optional[int] = None,
                  trigger_right: Optional[int] = None,
-                 labels: Optional[List[str]] = None) -> None:
+                 labels: Optional[List[int]] = None) -> None:
         """Constructs an `EDInputFeatures`."""
         self.example_id = example_id
         self.input_ids = input_ids
         self.attention_mask = attention_mask
         self.token_type_ids = token_type_ids
         self.trigger_left = trigger_left
         self.trigger_right = trigger_right
@@ -128,27 +128,29 @@
     """
 
     def __init__(self,
                  example_id: Union[int, str],
                  text: Union[str, List[str]],
                  pred_type: str,
                  true_type: str,
-                 input_template: Optional = None,
+                 trigger_id: Union[int, str] = None,
+                 input_template: Optional[str] = None,
                  trigger_left: Optional[int] = None,
                  trigger_right: Optional[int] = None,
                  argument_left: Optional[int] = None,
                  argument_right: Optional[int] = None,
                  argument_role: Optional[str] = None,
                  labels: Optional[Union[str, List[str]]] = None,
                  **kwargs):
         """Constructs a `EAEInputExample`."""
         self.example_id = example_id
         self.text = text
         self.pred_type = pred_type
         self.true_type = true_type
+        self.trigger_id = trigger_id
         self.input_template = input_template
         self.trigger_left = trigger_left
         self.trigger_right = trigger_right
         self.argument_left = argument_left
         self.argument_right = argument_right
         self.argument_role = argument_role
         self.labels = labels
@@ -368,14 +370,16 @@
         raise NotImplementedError
 
     def get_data_for_evaluation(self) -> Dict[str, Union[int, List[str]]]:
         """Obtains the data for evaluation."""
         self.data_for_evaluation["pred_types"] = self.get_pred_types()
         self.data_for_evaluation["true_types"] = self.get_true_types()
         self.data_for_evaluation["ids"] = self.get_ids()
+        self.data_for_evaluation["trigger_ids"] = self.get_trigger_ids()
+        self.data_for_evaluation["examples"] = self.examples
         if self.examples[0].argument_role is not None:
             self.data_for_evaluation["roles"] = self.get_roles()
         return self.data_for_evaluation
 
     def get_pred_types(self) -> List[str]:
         """Obtains the event type predicted by the model."""
         pred_types = []
@@ -413,14 +417,20 @@
 
     def get_ids(self) -> List[Union[int, str]]:
         """Returns the id of the examples."""
         ids = []
         for example in self.examples:
             ids.append(example.example_id)
         return ids
+    
+    def get_trigger_ids(self):
+        trigger_ids = []
+        for example in self.examples:
+            trigger_ids.append(example.trigger_id)
+        return trigger_ids
 
     def get_single_pred(self, trigger_idx, input_file, true_type):
         if self.is_training or "train" in input_file or self.config.golden_trigger or self.event_preds is None:
             pred_type = true_type
         else:
             pred_type = self.event_preds[trigger_idx]
         return pred_type
```

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/input_utils.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/input_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -160,14 +160,29 @@
         left_pos = trigger["position"][0] if keep_space else len("".join(text[:trigger["position"][0]].split()))
         right_pos = trigger["position"][1] if keep_space else len("".join(text[:trigger["position"][1]].split()))
     else:
         raise NotImplementedError
     return left_pos, right_pos
 
 
+def char_pos_to_word_pos(text: str,
+                           char_pos: List[int],
+                           language: str = "English",
+                           keep_space: bool = False) -> Tuple[int, int]:
+    if language == "English":
+        left_pos = len(text[:char_pos[0]].split())
+        right_pos = len(text[:char_pos[1]].split())
+    elif language == "Chinese":
+        left_pos = char_pos[0] if keep_space else len("".join(text[:char_pos[0]].split()))
+        right_pos = char_pos[1] if keep_space else len("".join(text[:char_pos[1]].split()))
+    else:
+        raise NotImplementedError
+    return left_pos, right_pos
+
+
 def get_word_ids(tokenizer: PreTrainedTokenizer,
                  outputs: BatchEncoding,
                  word_list: List[str]) -> List[int]:
     """Return a list mapping the tokens to their actual word in the initial sentence for a tokenizer.
 
     Return a list indicating the word corresponding to each token. Special tokens added by the tokenizer are mapped to
     None and other tokens are mapped to the index of their corresponding word (several tokens will be mapped to the same
```

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/mrc_converter.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/mrc_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     Returns:
         An integer indicating the word-level position of the mention.
     """
     return len(text[:position].split())
 
 
-def make_predictions(all_start_logits, all_end_logits, training_args):
+def make_predictions(all_start_logits, all_end_logits, training_args, use_example_id=True):
     """Obtains the prediction from the Machine Reading Comprehension (MRC) model."""
     data_for_evaluation = training_args.data_for_evaluation
     assert len(all_start_logits) == len(data_for_evaluation["ids"])
     # all golden labels
     final_all_labels = []
     for arguments in data_for_evaluation["golden_arguments"]:
         arguments_per_trigger = []
@@ -169,15 +169,15 @@
         prelim_predictions = sorted(prelim_predictions, key=lambda x: (x.start_logit + x.end_logit), reverse=True)
         # get final pred in format: [event_type_offset_argument_type, [start_offset, end_offset]]
         max_num_pred_per_arg = 1
         predictions_per_query = []
         for _, pred in enumerate(prelim_predictions[:max_num_pred_per_arg]):
             na_prob = (start_logits[0] + end_logits[0]) - (pred.start_logit + pred.end_logit)
             predictions_per_query.append((event_argument_type, (pred.start_index, pred.end_index), na_prob,
-                                          data_for_evaluation["ids"][example_id]))
+                                          data_for_evaluation["ids"][example_id] if use_example_id else data_for_evaluation["trigger_ids"][example_id]))
         final_all_predictions.extend(predictions_per_query)
 
     logger.info("\nAll predictions and labels generated. %d %d\n" % (len(final_all_predictions), len(final_all_labels)))
     return final_all_predictions, final_all_labels
 
 
 def find_best_thresh(new_preds, new_all_gold):
@@ -252,9 +252,9 @@
     else:
         recall_c = 0
     if prec_c or recall_c:
         f1_c = 2 * prec_c * recall_c / (prec_c + recall_c)
     else:
         f1_c = 0
 
-    logger.info("Precision: %.2f, recall: %.2f" % (prec_c, recall_c))
-    return f1_c
+    # logger.info("Precision: %.2f, recall: %.2f" % (prec_c, recall_c))
+    return prec_c, recall_c, f1_c
```

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/mrc_processor.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/mrc_processor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,147 @@
 import json
 import logging
+import numpy as np
 
 from tqdm import tqdm
 from .base_processor import (
+    EDDataProcessor,
+    EDInputExample,
+    EDInputFeatures,
     EAEDataProcessor,
     EAEInputExample,
     EAEInputFeatures
 )
 from .mrc_converter import read_query_templates
 from .input_utils import get_words, get_left_and_right_pos, get_word_ids
 from collections import defaultdict
+from typing import List, Dict, Optional, Union
 
 logger = logging.getLogger(__name__)
 
 
+
+class EDMRCProcessor(EDDataProcessor):
+    """Data processor for sequence labeling for event detection.
+
+    Data processor for sequence labeling for event detection. The class is inherited from the `EDDataProcessor` class,
+    in which the undefined functions, including `read_examples()` and `convert_examples_to_features()` are  implemented;
+    a new function entitled `get_final_labels()` is defined to obtain final results, and the rest of the attributes and
+    functions are multiplexed from the `EDDataProcessor` class.
+
+    Attributes:
+        is_overflow:
+    """
+
+    def __init__(self,
+                 config,
+                 tokenizer: str,
+                 input_file: str) -> None:
+        """Constructs a EDMRCProcessor."""
+        super().__init__(config, tokenizer)
+        self.read_examples(input_file)
+        self.convert_examples_to_features()
+
+    def read_examples(self,
+                      input_file: str) -> None:
+        """Obtains a collection of `EDInputExample`s for the dataset."""
+        self.examples = []
+        language = self.config.language
+
+        with open(input_file, "r", encoding="utf-8") as f:
+            for line in tqdm(f.readlines(), desc="Reading from %s" % input_file):
+                item = json.loads(line.strip())
+                text = item["text"]
+                words = get_words(text=text, language=language)
+                labels = ["NA"] * len(words)
+
+                if "events" in item:
+                    for event in item["events"]:
+                        for trigger in event["triggers"]:
+                            left_pos, right_pos = get_left_and_right_pos(text, trigger, language, True)
+                            labels[left_pos] = f"{event['type']}"
+                            for i in range(left_pos + 1, right_pos):
+                                labels[i] = f"{event['type']}"
+                    example = EDInputExample(
+                                    example_id=item["id"], 
+                                    text=words, 
+                                    labels=labels
+                                )
+                    self.examples.append(example)
+                
+                # test set 
+                elif "candidates" in item:
+                    for candidate in item["candidates"]:
+                        example = EDInputExample(
+                            example_id=candidate["id"],
+                            text=words,
+                            labels=labels,
+                        )
+                        self.examples.append(example)
+
+
+    def get_final_labels(self,
+                         labels: List[str],
+                         word_ids_of_each_token: List[int],
+                         label_all_tokens: Optional[bool] = False) -> List[Union[str, int]]:
+        """Obtains the final label of each token."""
+        final_labels = []
+        pre_word_id = None
+        for word_id in word_ids_of_each_token:
+            if word_id is None:
+                final_labels.append(-100)
+            elif word_id != pre_word_id:  # first split token of a word
+                final_labels.append(self.config.type2id[labels[word_id]])
+            else:
+                final_labels.append(self.config.type2id[labels[word_id]] if label_all_tokens else -100)
+            pre_word_id = word_id
+
+        return final_labels
+
+    def convert_examples_to_features(self) -> None:
+        """Converts the `EDInputExample`s into `EDInputFeatures`s."""
+        self.input_features = []
+        query_question = "verb".split()
+
+        for example in tqdm(self.examples, desc="Processing features for SL"):
+            query = self.tokenizer(query_question,
+                                     truncation=False,
+                                     is_split_into_words=True)
+            max_seq_length = self.config.max_seq_length-len(query["input_ids"])
+            outputs = self.tokenizer(example.text,
+                                     padding="max_length",
+                                     truncation=False,
+                                     max_length=max_seq_length,
+                                     is_split_into_words=True)
+            # Roberta tokenizer doesn't return token_type_ids
+            if "token_type_ids" not in outputs:
+                outputs["token_type_ids"] = [0] * len(outputs["input_ids"])
+
+            outputs, is_overflow = self._truncate(outputs, max_seq_length)
+            self.is_overflow.append(is_overflow)
+
+            word_ids_of_each_token = get_word_ids(self.tokenizer, outputs, example.text)[:max_seq_length]
+            final_labels = self.get_final_labels(example.labels, word_ids_of_each_token, label_all_tokens=False)
+
+            # concat query
+            for key in ["input_ids", "attention_mask"]:
+                outputs[key] = query[key] + outputs[key]
+            outputs["token_type_ids"] = [0] * len(query["token_type_ids"]) + [1] * len(outputs["token_type_ids"])
+            final_labels = [-100] * len(query["input_ids"]) + final_labels
+
+            features = EDInputFeatures(
+                example_id=example.example_id,
+                input_ids=outputs["input_ids"],
+                attention_mask=outputs["attention_mask"],
+                token_type_ids=outputs["token_type_ids"],
+                labels=final_labels,
+            )
+            self.input_features.append(features)
+
+
 class EAEMRCProcessor(EAEDataProcessor):
     """Data processor for Machine Reading Comprehension (MRC) for event argument extraction.
 
     Data processor for Machine Reading Comprehension (MRC) for event argument extraction. The class is inherited from
     the `EAEDataProcessor` class, in which the undefined functions, including `read_examples()` and
     `convert_examples_to_features()` are implemented; a new function entitled `remove_sub_word()` is defined to remove
     the annotations whose word is a sub-word, the rest of the attributes and functions are multiplexed from the
@@ -60,15 +184,15 @@
                             # If predicted event type is NA:
                             #   in [default] and [loose] modes, we don't consider the trigger
                             #   in [strict] mode, we consider the trigger
                             if self.config.eae_eval_mode in ["default", "loose"] and pred_type == "NA":
                                 continue
 
                             # golden label for the trigger
-                            arguments_per_trigger = dict(id=trigger_idx-1,
+                            arguments_per_trigger = dict(id=idx,
                                                          arguments=[],
                                                          pred_type=pred_type,
                                                          true_type=event["type"])
                             for argument in trigger["arguments"]:
                                 arguments_per_role = dict(role=argument["role"], mentions=[])
                                 for mention in argument["mentions"]:
                                     left_pos, right_pos = get_left_and_right_pos(text, mention, language)
@@ -98,44 +222,47 @@
                                             pass
                                         if argument["role"] != role:
                                             continue
                                         no_answer = False
                                         for mention in argument["mentions"]:
                                             left_pos, right_pos = get_left_and_right_pos(text, mention, language)
                                             example = EAEInputExample(
-                                                example_id=trigger_idx-1,
+                                                example_id=idx,
+                                                trigger_id=trigger_idx-1,
                                                 text=words,
                                                 pred_type=pred_type,
                                                 true_type=event["type"],
                                                 input_template=query,
                                                 trigger_left=trigger_left,
                                                 trigger_right=trigger_right,
                                                 argument_left=left_pos,
                                                 argument_right=right_pos - 1,
                                                 argument_role=role,
                                             )
                                             self.examples.append(example)
                                     if no_answer:
                                         example = EAEInputExample(
-                                            example_id=trigger_idx-1,
+                                            example_id=idx,
+                                            trigger_id=trigger_idx-1,
                                             text=words,
                                             pred_type=pred_type,
                                             true_type=event["type"],
                                             input_template=query,
                                             trigger_left=trigger_left,
                                             trigger_right=trigger_right,
                                             argument_left=-1,
                                             argument_right=-1,
                                             argument_role=role,
                                         )
                                         self.examples.append(example)
                                 else:
                                     # one instance per query
                                     example = EAEInputExample(
-                                        example_id=trigger_idx-1,
+                                        example_id=idx,
+                                        trigger_id=trigger_idx-1,
                                         text=words,
                                         pred_type=pred_type,
                                         true_type=event["type"],
                                         input_template=query,
                                         trigger_left=trigger_left,
                                         trigger_right=trigger_right,
                                         argument_left=-1,
@@ -158,15 +285,16 @@
                             for role in query_templates[pred_type].keys():
                                 query = query_templates[pred_type][role][template_id]
                                 query = query.replace("[trigger]",
                                                       self.tokenizer.tokenize(neg_trigger["trigger_word"])[0])
                                 query = get_words(text=query, language=self.config.language)
                                 # one instance per query
                                 example = EAEInputExample(
-                                    example_id=trigger_idx-1,
+                                    example_id=idx,
+                                    trigger_id=trigger_idx-1,
                                     text=words,
                                     pred_type=pred_type,
                                     true_type="NA",
                                     input_template=query,
                                     trigger_left=trigger_left,
                                     trigger_right=trigger_right,
                                     argument_left=-1,
@@ -186,15 +314,16 @@
                         if pred_type != "NA":
                             for role in query_templates[pred_type].keys():
                                 query = query_templates[pred_type][role][template_id]
                                 query = query.replace("[trigger]", self.tokenizer.tokenize(candi["trigger_word"])[0])
                                 query = get_words(text=query, language=language)
                                 # one instance per query
                                 example = EAEInputExample(
-                                    example_id=trigger_idx-1,
+                                    example_id=idx,
+                                    trigger_id=trigger_idx-1,
                                     text=words,
                                     pred_type=pred_type,
                                     true_type="NA",
                                     input_template=query,
                                     trigger_left=trigger_left,
                                     trigger_right=trigger_right,
                                     argument_left=-1,
@@ -248,14 +377,16 @@
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 token_type_ids=token_type_ids,
                 argument_left=start_position,
                 argument_right=end_position,
             )
             self.input_features.append(features)
+            # offset
+            # example.offset = offset
 
     @staticmethod
     def remove_sub_word(tokenizer, inputs, word_list):
         """Removes the annotations whose word is a sub-word."""
         outputs = defaultdict(list)
         pre_word_id = -1
         for token_id, word_id in enumerate(get_word_ids(tokenizer, inputs, word_list)):
```

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/seq2seq_processor.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/seq2seq_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,15 @@
         words = span.strip().split(split_word)
         if len(words) != 2:
             continue
         role = words[0].strip().replace(" ", "")
         value = words[1].strip().replace(" ", "")
         if role != "" and value != "":
             arguments.append((instance_id, event_type, role, value))
-<<<<<<< HEAD
     # arguments = list(set(arguments))
-=======
->>>>>>> 849862bafe3342e60077401272ebc44f7ce2ddd8
     return arguments
 
 
 class EDSeq2SeqProcessor(EDDataProcessor):
     """Data processor for Sequence-to-Sequence (Seq2Seq) for event detection.
 
     Data processor for Sequence-to-Sequence (Seq2Seq) for event detection. The class is inherited from the
```

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/sequence_labeling_processor.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/sequence_labeling_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     def __init__(self,
                  config,
                  tokenizer: str,
                  input_file: str) -> None:
         """Constructs a EDSLProcessor."""
         super().__init__(config, tokenizer)
         self.read_examples(input_file)
-        self.is_overflow = []
         self.convert_examples_to_features()
 
     def read_examples(self,
                       input_file: str) -> None:
         """Obtains a collection of `EDInputExample`s for the dataset."""
         self.examples = []
         language = self.config.language
@@ -131,15 +130,14 @@
                  tokenizer: str,
                  input_file: str,
                  pred_file: str,
                  is_training: Optional[bool] = False) -> None:
         """Constructs an EAESLProcessor/"""
         super().__init__(config, tokenizer, pred_file, is_training)
         self.positive_candidate_indices = []
-        self.is_overflow = []
         self.config.role2id["X"] = -100
         self.read_examples(input_file)
         self.convert_examples_to_features()
 
     def read_examples(self,
                       input_file: str) -> None:
         """Obtains a collection of `EAEInputExample`s for the dataset."""
```

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/token_classification_processor.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/token_classification_processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 
 from tqdm import tqdm
 from typing import List, Optional, Dict
 
-from .input_utils import check_is_argument, get_negative_argument_candidates
+from .input_utils import check_is_argument, get_negative_argument_candidates, get_word_ids, char_pos_to_word_pos
 from .base_processor import (
     EDDataProcessor,
     EDInputExample,
     EDInputFeatures,
     EAEDataProcessor,
     EAEInputExample,
     EAEInputFeatures,
@@ -76,45 +76,70 @@
                         self.examples.append(example)
 
     def convert_examples_to_features(self) -> None:
         """Converts the `EDInputExample`s into `EDInputFeatures`s."""
         # merge and then tokenize
         self.input_features = []
         for example in tqdm(self.examples, desc="Processing features for TC"):
-            text_left = example.text[:example.trigger_left]
-            text_mid = example.text[example.trigger_left:example.trigger_right]
-            text_right = example.text[example.trigger_right:]
-
-            if self.config.language == "Chinese":
-                text = text_left + self.config.markers[0] + text_mid + self.config.markers[1] + text_right
+            if self.config.insert_marker:
+                text_left = example.text[:example.trigger_left]
+                text_mid = example.text[example.trigger_left:example.trigger_right]
+                text_right = example.text[example.trigger_right:]
+
+                if self.config.language == "Chinese":
+                    text = text_left + self.config.markers[0] + text_mid + self.config.markers[1] + text_right
+                else:
+                    text = text_left + self.config.markers[0] + " " + text_mid + " " + self.config.markers[1] + text_right
+
+                outputs = self.tokenizer(text, padding="max_length", truncation=True, max_length=self.config.max_seq_length)
+                try:
+                    left = outputs["input_ids"].index(self.tokenizer.convert_tokens_to_ids(self.config.markers[0]))
+                    right = outputs["input_ids"].index(self.tokenizer.convert_tokens_to_ids(self.config.markers[1]))
+                except:
+                    logger.warning("Markers are not in the input tokens.")
+                    left, right = 0, 0
             else:
-                text = text_left + self.config.markers[0] + " " + text_mid + " " + self.config.markers[1] + text_right
-
-            outputs = self.tokenizer(text, padding="max_length", truncation=True, max_length=self.config.max_seq_length)
-            try:
-                left = outputs["input_ids"].index(self.tokenizer.convert_tokens_to_ids(self.config.markers[0]))
-                right = outputs["input_ids"].index(self.tokenizer.convert_tokens_to_ids(self.config.markers[1]))
-            except:
-                logger.warning("Markers are not in the input tokens.")
-                left, right = 0, 0
-
+                tokens = example.text.split()
+                outputs = self.tokenizer(tokens, 
+                                        padding="max_length", 
+                                        truncation=True, 
+                                        max_length=self.config.max_seq_length,
+                                        is_split_into_words=True,
+                                        add_special_tokens=True)
+                trigger_word_left, trigger_word_right = char_pos_to_word_pos(example.text, 
+                                                                        [example.trigger_left, example.trigger_right])
+                word_ids_of_each_token = get_word_ids(self.tokenizer, outputs, tokens)[: self.config.max_seq_length]
+                left, right = -1, -1
+                for i, word_id in enumerate(word_ids_of_each_token):
+                    if word_id == trigger_word_left and left == -1:
+                        left = i
+                    if word_id == trigger_word_right-1:
+                        right = i
+
+                if left == -1:
+                    logger.warning("Overflow! %s" % example.text)
+                if right == -1:
+                    right = self.config.max_seq_length - 1
             # Roberta tokenizer doesn't return token_type_ids
             if "token_type_ids" not in outputs:
                 outputs["token_type_ids"] = [0] * len(outputs["input_ids"])
 
             features = EDInputFeatures(
                 example_id=example.example_id,
                 input_ids=outputs["input_ids"],
                 attention_mask=outputs["attention_mask"],
                 token_type_ids=outputs["token_type_ids"],
                 trigger_left=left,
                 trigger_right=right,
             )
             if example.labels is not None:
                 features.labels = self.config.type2id[example.labels]
+            if left == -1:
+                left = 0
+                features.labels = -100
             self.input_features.append(features)
 
 
 class EAETCProcessor(EAEDataProcessor):
     """Data processor for token classification for event argument extraction.
 
     Data processor for token classification for event argument extraction. The class is inherited from the
@@ -238,56 +263,103 @@
 
     def convert_examples_to_features(self) -> None:
         """Converts the `EAEInputExample`s into `EAEInputFeatures`s."""
         # merge and then tokenize
         self.input_features = []
         whitespace = True if self.config.language == "English" else False
         for example in tqdm(self.examples, desc="Processing features for TC"):
-            text = self.insert_marker(example.text,
-                                      example.pred_type,
-                                      [example.trigger_left, example.trigger_right],
-                                      [example.argument_left, example.argument_right],
-                                      self.config.markers,
-                                      whitespace)
-            outputs = self.tokenizer(text,
-                                     padding="max_length",
-                                     truncation=True,
-                                     max_length=self.config.max_seq_length)
-            is_overflow = False
-            # argument position 
-            try:
-                argument_left = outputs["input_ids"].index(
-                    self.tokenizer.convert_tokens_to_ids(self.config.markers["argument"][0]))
-                argument_right = outputs["input_ids"].index(
-                    self.tokenizer.convert_tokens_to_ids(self.config.markers["argument"][1]))
-            except:
-                argument_left, argument_right = 0, 0
-                logger.warning("Argument markers are not in the input tokens.")
-                is_overflow = True
-            # trigger position
-            try:
-                trigger_left = outputs["input_ids"].index(
-                    self.tokenizer.convert_tokens_to_ids(self.config.markers[example.pred_type][0]))
-                trigger_right = outputs["input_ids"].index(
-                    self.tokenizer.convert_tokens_to_ids(self.config.markers[example.pred_type][1]))
-            except:
-                trigger_left, trigger_right = 0, 0
-                logger.warning("Trigger markers are not in the input tokens.")
+            if self.config.insert_marker:
+                text = self.insert_marker(example.text,
+                                        example.pred_type,
+                                        [example.trigger_left, example.trigger_right],
+                                        [example.argument_left, example.argument_right],
+                                        self.config.markers,
+                                        whitespace)
+                outputs = self.tokenizer(text,
+                                        padding="max_length",
+                                        truncation=True,
+                                        max_length=self.config.max_seq_length)
+                is_overflow = False
+                # argument position 
+                try:
+                    argument_left = outputs["input_ids"].index(
+                        self.tokenizer.convert_tokens_to_ids(self.config.markers["argument"][0]))
+                    argument_right = outputs["input_ids"].index(
+                        self.tokenizer.convert_tokens_to_ids(self.config.markers["argument"][1]))
+                except:
+                    argument_left, argument_right = 0, 0
+                    logger.warning("Argument markers are not in the input tokens.")
+                    is_overflow = True
+                # trigger position
+                try:
+                    trigger_left = outputs["input_ids"].index(
+                        self.tokenizer.convert_tokens_to_ids(self.config.markers[example.pred_type][0]))
+                    trigger_right = outputs["input_ids"].index(
+                        self.tokenizer.convert_tokens_to_ids(self.config.markers[example.pred_type][1]))
+                except:
+                    trigger_left, trigger_right = 0, 0
+                    logger.warning("Trigger markers are not in the input tokens.")
+            else:
+                tokens = example.text.split()
+                outputs = self.tokenizer(tokens, 
+                                        padding="max_length", 
+                                        truncation=True, 
+                                        max_length=self.config.max_seq_length,
+                                        is_split_into_words=True,
+                                        add_special_tokens=True)
+                word_ids_of_each_token = get_word_ids(self.tokenizer, outputs, tokens)[: self.config.max_seq_length]
+                trigger_word_left, trigger_word_right = char_pos_to_word_pos(example.text, 
+                                                                        [example.trigger_left, example.trigger_right])
+                argument_word_left, argument_word_right = char_pos_to_word_pos(example.text, 
+                                                                        [example.argument_left, example.argument_right])
+                trigger_left, trigger_right = -1, -1
+                argument_left, argument_right = -1, -1
+                for i, word_id in enumerate(word_ids_of_each_token):
+                    if word_id == trigger_word_left and trigger_left == -1:
+                        trigger_left = i
+                    if word_id == trigger_word_right-1:
+                        trigger_right = i
+                    if word_id == argument_word_left and argument_left == -1:
+                        argument_left = i
+                    if word_id == argument_word_right-1:
+                        argument_right = i
+                
+                if trigger_left == -1 or argument_left == -1:
+                    logger.warning("Overflow! %s" % example.text)
+                if trigger_right == -1:
+                    trigger_right = self.config.max_seq_length - 1
+                if argument_right == -1:
+                    argument_right = self.config.max_seq_length - 1
+
             # Roberta tokenizer doesn't return token_type_ids
             if "token_type_ids" not in outputs:
                 outputs["token_type_ids"] = [0] * len(outputs["input_ids"])
+            
+            if self.config.consider_event_type:
+                token_type_ids = [0] * len(outputs["input_ids"])
+                for idx in range(trigger_left, trigger_right+1):
+                    token_type_ids[idx] = self.config.type2id[example.pred_type]
+
+                for idx in range(argument_left, argument_right):
+                    token_type_ids[idx] = self.config.type2id[example.pred_type]
+
+                outputs["token_type_ids"] = token_type_ids
 
             features = EAEInputFeatures(
                 example_id=example.example_id,
                 input_ids=outputs["input_ids"],
                 attention_mask=outputs["attention_mask"],
                 token_type_ids=outputs["token_type_ids"],
                 trigger_left=trigger_left,
                 trigger_right=trigger_right,
                 argument_left=argument_left,
                 argument_right=argument_right,
             )
             if example.labels is not None:
                 features.labels = self.config.role2id[example.labels]
-                if is_overflow:
+                if trigger_left == -1:
+                    trigger_left = 0
+                    features.labels = -100
+                if argument_left == -1:
+                    argument_left = 0
                     features.labels = -100
             self.input_features.append(features)
```

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/tokenizer.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/tokenizer.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/input_engineering/whitespace_tokenizer.py` & `OmniEvent-0.1.6/OmniEvent/input_engineering/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/model/constraint_decoding.py` & `OmniEvent-0.1.6/OmniEvent/model/constraint_decoding.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/model/label_smoother_sum.py` & `OmniEvent-0.1.6/OmniEvent/model/label_smoother_sum.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/model/model.py` & `OmniEvent-0.1.6/OmniEvent/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import torch
 import torch.nn as nn
+import torch.nn.functional as F
 
 from typing import Dict, Optional, Union
 from transformers import BartForConditionalGeneration, MT5ForConditionalGeneration, T5ForConditionalGeneration
 
 from OmniEvent.aggregation.aggregation import get_aggregation, aggregate
 from OmniEvent.head.head import get_head
 from OmniEvent.head.classification import LinearHead
@@ -14,15 +15,16 @@
     TrainingArguments,
     ArgumentParser
 )
 from OmniEvent.utils import check_web_and_convert_path
 
 
 def get_model(model_args,
-              backbone):
+              backbone,
+              task_type="EAE"):
     """Returns the model proposed to be utilized for training and prediction.
 
     Returns the model proposed to be utilized for training and prediction based on the pre-defined paradigm. The
     paradigms of training and prediction include token classification, sequence labeling, Sequence-to-Sequence
     (Seq2Seq), and Machine Reading Comprehension (MRC).
 
     Args:
@@ -37,15 +39,20 @@
     if model_args.paradigm == "token_classification":
         return ModelForTokenClassification(model_args, backbone)
     elif model_args.paradigm == "sequence_labeling":
         return ModelForSequenceLabeling(model_args, backbone)
     elif model_args.paradigm == "seq2seq":
         return backbone
     elif model_args.paradigm == "mrc":
-        return ModelForMRC(model_args, backbone)
+        if task_type == "EAE":
+            return ModelForMRC(model_args, backbone)
+        elif task_type == "ED":
+            return ModelForSequenceLabeling(model_args, backbone)
+        else:
+            raise ValueError
     else:
         raise ValueError("No such paradigm")
 
 
 def get_model_cls(model_args):
     if model_args.paradigm == "token_classification":
         return ModelForTokenClassification
@@ -65,20 +72,20 @@
     else:
         raise ValueError("No such paradigm")
 
 
 class BaseModel(nn.Module):
 
     @classmethod
-    def from_pretrained(cls, model_name_or_path: Union[str, os.PathLike], config=None, **kwargs):
-        if config is None:
+    def from_pretrained(cls, model_name_or_path: Union[str, os.PathLike], backbone=None, model_args=None, **kwargs):
+        if model_args is None:
             parser = ArgumentParser((ModelArguments, DataArguments, TrainingArguments))
             model_args, _, _ = parser.from_pretrained(model_name_or_path, **kwargs)
         path = check_web_and_convert_path(model_name_or_path, 'model')
-        model = get_model(model_args)
+        model = get_model(model_args, backbone)
         model.load_state_dict(torch.load(path), strict=False)
         return model
 
 
 class ModelForTokenClassification(BaseModel):
     """BERT model for token classification.
 
@@ -115,28 +122,37 @@
                 trigger_left: Optional[torch.Tensor] = None,
                 trigger_right: Optional[torch.Tensor] = None,
                 argument_left: Optional[torch.Tensor] = None,
                 argument_right: Optional[torch.Tensor] = None,
                 labels: Optional[torch.Tensor] = None) -> Dict[str, torch.Tensor]:
         """Manipulates the inputs through a backbone, aggregation, and classification module,
            returns the predicted logits and loss."""
-        # backbone encode 
-        outputs = self.backbone(input_ids=input_ids,
-                                attention_mask=attention_mask,
-                                token_type_ids=token_type_ids,
-                                return_dict=True)
+        # backbone encode
+        if self.config.model_type in ["cnn", "lstm"]:
+            outputs = self.backbone(input_ids=input_ids,
+                        attention_mask=attention_mask,
+                        token_type_ids=token_type_ids,
+                        position=trigger_left if argument_left is None else argument_left,
+                        return_dict=True)
+        else:
+            outputs = self.backbone(input_ids=input_ids,
+                                    attention_mask=attention_mask,
+                                    token_type_ids=token_type_ids,
+                                    return_dict=True)
         hidden_states = outputs.last_hidden_state
         # aggregation 
         hidden_state = aggregate(self.config,
                                  self.aggregation,
                                  hidden_states,
+                                 attention_mask,
                                  trigger_left,
                                  trigger_right,
                                  argument_left,
-                                 argument_right)
+                                 argument_right,
+                                 embeddings=self.backbone.embedding.word_embeddings(input_ids) if self.config.model_type=="cnn" else None)
         # classification
         logits = self.cls_head(hidden_state)
         # compute loss 
         loss = None
         if labels is not None:
             loss_fn = nn.CrossEntropyLoss()
             loss = loss_fn(logits, labels)
@@ -178,14 +194,16 @@
            returns the predicted logits and loss."""
         # backbone encode 
         outputs = self.backbone(input_ids=input_ids,
                                 attention_mask=attention_mask,
                                 token_type_ids=token_type_ids,
                                 return_dict=True)
         hidden_states = outputs.last_hidden_state
+        if self.config.dropout_after_encoder:
+            hidden_states = F.dropout(hidden_states, p=0.2)
         # classification
         logits = self.cls_head(hidden_states)  # [batch_size, seq_length, num_labels]
         # compute loss 
         loss = None
         if labels is not None:
             if self.config.head_type != "crf":
                 loss_fn = nn.CrossEntropyLoss()
```

### Comparing `OmniEvent-0.1.5/OmniEvent/trainer.py` & `OmniEvent-0.1.6/OmniEvent/trainer.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/trainer_seq2seq.py` & `OmniEvent-0.1.6/OmniEvent/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.5/OmniEvent/utils.py` & `OmniEvent-0.1.6/OmniEvent/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     os.system(f"rm {path}")
 
 
 def check_web_and_convert_path(path, load_type, base_path="~/.cache/OmniEvent_Model"): # TODO add hash
     base_path = os.path.expanduser(base_path)
     
     if not os.path.exists(base_path):
-        os.mkdir(base_path)
+        os.makedirs(base_path)
     if os.path.isdir(path):
         print(f"load from local file: {path} {load_type}")
         return path
     if os.path.isdir(os.path.join(base_path, path)):
         print(f"load from local file: {os.path.join(base_path, path)} {load_type}")
         return os.path.join(base_path, path)
```

### Comparing `OmniEvent-0.1.5/OmniEvent.egg-info/PKG-INFO` & `OmniEvent-0.1.6/OmniEvent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OmniEvent
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tookit for event extraction.
 License: Copyright (c) 2022 THUKEG
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -252,15 +252,15 @@
 
 OmniEvent evaluates models of different paradigms in a unified manner, where the predictions of different models are converted to predictions on the same candidate sets and then evaluated.
 
 ```python  
 >>> from OmniEvent.evaluation.utils import predict, get_pred_s2s
 >>> from OmniEvent.evaluation.convert_format import get_ace2005_trigger_detection_s2s
 
->>> logits, labels, metrics, test_dataset = predict(trainer=trainer, tokenizer=tokenizer, data_class=data_class,
+>>> logits, labels, metrics, test_dataset = predict(trainer=trainer, tokenizer=tokenizer, data_class=EDSeq2SeqProcessor,
                                                     data_args=data_args, data_file=data_args.test_file,
                                                     training_args=training_args)
 >>> # paradigm-dependent metrics
 >>> print("{} test performance before converting: {}".formate(test_dataset.dataset_name, metrics["test_micro_f1"]))  
 ACE2005-EN test performance before converting: 66.4215686224377
 
 >>> preds = get_pred_s2s(logits, tokenizer)
@@ -344,25 +344,28 @@
 - Aggregation
   - Select [CLS]
   - Dynamic/Max Pooling
   - Marker
   - GCN
 - Head
   - Linear / CRF / MRC heads
-'
 
 ## Contests
 OmniEvent plans to support various event extraction contest. Currently, we support the following contests and the list is continually updated!
 
 - [MAVEN Event Detection Challenge](https://codalab.lisn.upsaclay.fr/competitions/395)
 - [CAIL 2022: Event Detection Track](http://cail.cipsc.org.cn/task1.html?raceID=1&cail_tag=2022)
 - [LUGE: Information Extraction Track](https://aistudio.baidu.com/aistudio/competition/detail/46/0/task-definition)
 
 # Experiments
-We implement and evaluate state-of-the-art methods on some popular benchmarks using OmniEvent. The results of all Event Detection experiments are shown in the table below. The full results can be accessed via the links below.
+We implement and evaluate state-of-the-art methods on some popular benchmarks using OmniEvent. 
+
+The results of all Event Detection experiments are shown in the table below. 
+
+The **full results** can be accessed via the links below.
 
 - [Experiments of base models on <u>**All ED Benchmarks**</u>](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=qp276f)
 - [Experiments of base models on <u>**All EAE Benchmarks**</u>](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=b0zjme)
 - [Experiments of <u>**All ED Models**</u> on ACE-EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=odcgnh)
 - [Experiments of <u>**All EAE Models**</u> on ACE-EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=jxc1ea)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OmniEvent Version: 0.1.5 Summary: A tookit for
+Metadata-Version: 2.1 Name: OmniEvent Version: 0.1.6 Summary: A tookit for
 event extraction. License: Copyright (c) 2022 THUKEG Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -146,15 +146,15 @@
 Since the metrics in Step 4 depend on the paradigm, it is not fair to directly
 compare the performance of models in different paradigms. OmniEvent evaluates
 models of different paradigms in a unified manner, where the predictions of
 different models are converted to predictions on the same candidate sets and
 then evaluated. ```python >>> from OmniEvent.evaluation.utils import predict,
 get_pred_s2s >>> from OmniEvent.evaluation.convert_format import
 get_ace2005_trigger_detection_s2s >>> logits, labels, metrics, test_dataset =
-predict(trainer=trainer, tokenizer=tokenizer, data_class=data_class,
+predict(trainer=trainer, tokenizer=tokenizer, data_class=EDSeq2SeqProcessor,
 data_args=data_args, data_file=data_args.test_file,
 training_args=training_args) >>> # paradigm-dependent metrics >>> print("{}
 test performance before converting: {}".formate(test_dataset.dataset_name,
 metrics["test_micro_f1"])) ACE2005-EN test performance before converting:
 66.4215686224377 >>> preds = get_pred_s2s(logits, tokenizer) >>> # convert to
 the unified prediction and evaluate >>> pred_labels =
 get_ace2005_trigger_detection_s2s(preds, labels, data_args.test_file,
@@ -172,24 +172,24 @@
                            Legal     ED     LEVEN
                   Chinese  General   ED EAE DuEE
                            General   ED EAE ACE-ZH
                            Financial ED EAE FewFC
 ## Models - Paradigm - Token Classification (TC) - Sequence Labeling (SL) -
 Sequence to Sequence (Seq2Seq) - Machine Reading Comprehension (MRC) - Backbone
 - CNN / LSTM - Transformers (BERT, T5, etc.) - Aggregation - Select [CLS] -
-Dynamic/Max Pooling - Marker - GCN - Head - Linear / CRF / MRC heads ' ##
+Dynamic/Max Pooling - Marker - GCN - Head - Linear / CRF / MRC heads ##
 Contests OmniEvent plans to support various event extraction contest.
 Currently, we support the following contests and the list is continually
 updated! - [MAVEN Event Detection Challenge](https://codalab.lisn.upsaclay.fr/
 competitions/395) - [CAIL 2022: Event Detection Track](http://
 cail.cipsc.org.cn/task1.html?raceID=1&cail_tag=2022) - [LUGE: Information
 Extraction Track](https://aistudio.baidu.com/aistudio/competition/detail/46/0/
 task-definition) # Experiments We implement and evaluate state-of-the-art
 methods on some popular benchmarks using OmniEvent. The results of all Event
-Detection experiments are shown in the table below. The full results can be
+Detection experiments are shown in the table below. The **full results** can be
 accessed via the links below. - [Experiments of base models on **All_ED
 Benchmarks**](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=qp276f) -
 [Experiments of base models on **All_EAE_Benchmarks**](https://docs.qq.com/
 sheet/DRW5QQU1tZ2ViZlFo?tab=b0zjme) - [Experiments of **All_ED_Models** on ACE-
 EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=odcgnh) - [Experiments of
 **All_EAE_Models** on ACE-EN+](https://docs.qq.com/sheet/
 DRW5QQU1tZ2ViZlFo?tab=jxc1ea)
```

### Comparing `OmniEvent-0.1.5/OmniEvent.egg-info/SOURCES.txt` & `OmniEvent-0.1.6/OmniEvent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 OmniEvent/input_engineering/sequence_labeling_processor.py
 OmniEvent/input_engineering/token_classification_processor.py
 OmniEvent/input_engineering/tokenizer.py
 OmniEvent/input_engineering/whitespace_tokenizer.py
 OmniEvent/model/__init__.py
 OmniEvent/model/constraint_decoding.py
 OmniEvent/model/label_smoother_sum.py
-OmniEvent/model/model.py
+OmniEvent/model/model.py
+tests/test_infer.py
```

### Comparing `OmniEvent-0.1.5/PKG-INFO` & `OmniEvent-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OmniEvent
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tookit for event extraction.
 License: Copyright (c) 2022 THUKEG
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -252,15 +252,15 @@
 
 OmniEvent evaluates models of different paradigms in a unified manner, where the predictions of different models are converted to predictions on the same candidate sets and then evaluated.
 
 ```python  
 >>> from OmniEvent.evaluation.utils import predict, get_pred_s2s
 >>> from OmniEvent.evaluation.convert_format import get_ace2005_trigger_detection_s2s
 
->>> logits, labels, metrics, test_dataset = predict(trainer=trainer, tokenizer=tokenizer, data_class=data_class,
+>>> logits, labels, metrics, test_dataset = predict(trainer=trainer, tokenizer=tokenizer, data_class=EDSeq2SeqProcessor,
                                                     data_args=data_args, data_file=data_args.test_file,
                                                     training_args=training_args)
 >>> # paradigm-dependent metrics
 >>> print("{} test performance before converting: {}".formate(test_dataset.dataset_name, metrics["test_micro_f1"]))  
 ACE2005-EN test performance before converting: 66.4215686224377
 
 >>> preds = get_pred_s2s(logits, tokenizer)
@@ -344,25 +344,28 @@
 - Aggregation
   - Select [CLS]
   - Dynamic/Max Pooling
   - Marker
   - GCN
 - Head
   - Linear / CRF / MRC heads
-'
 
 ## Contests
 OmniEvent plans to support various event extraction contest. Currently, we support the following contests and the list is continually updated!
 
 - [MAVEN Event Detection Challenge](https://codalab.lisn.upsaclay.fr/competitions/395)
 - [CAIL 2022: Event Detection Track](http://cail.cipsc.org.cn/task1.html?raceID=1&cail_tag=2022)
 - [LUGE: Information Extraction Track](https://aistudio.baidu.com/aistudio/competition/detail/46/0/task-definition)
 
 # Experiments
-We implement and evaluate state-of-the-art methods on some popular benchmarks using OmniEvent. The results of all Event Detection experiments are shown in the table below. The full results can be accessed via the links below.
+We implement and evaluate state-of-the-art methods on some popular benchmarks using OmniEvent. 
+
+The results of all Event Detection experiments are shown in the table below. 
+
+The **full results** can be accessed via the links below.
 
 - [Experiments of base models on <u>**All ED Benchmarks**</u>](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=qp276f)
 - [Experiments of base models on <u>**All EAE Benchmarks**</u>](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=b0zjme)
 - [Experiments of <u>**All ED Models**</u> on ACE-EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=odcgnh)
 - [Experiments of <u>**All EAE Models**</u> on ACE-EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=jxc1ea)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OmniEvent Version: 0.1.5 Summary: A tookit for
+Metadata-Version: 2.1 Name: OmniEvent Version: 0.1.6 Summary: A tookit for
 event extraction. License: Copyright (c) 2022 THUKEG Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -146,15 +146,15 @@
 Since the metrics in Step 4 depend on the paradigm, it is not fair to directly
 compare the performance of models in different paradigms. OmniEvent evaluates
 models of different paradigms in a unified manner, where the predictions of
 different models are converted to predictions on the same candidate sets and
 then evaluated. ```python >>> from OmniEvent.evaluation.utils import predict,
 get_pred_s2s >>> from OmniEvent.evaluation.convert_format import
 get_ace2005_trigger_detection_s2s >>> logits, labels, metrics, test_dataset =
-predict(trainer=trainer, tokenizer=tokenizer, data_class=data_class,
+predict(trainer=trainer, tokenizer=tokenizer, data_class=EDSeq2SeqProcessor,
 data_args=data_args, data_file=data_args.test_file,
 training_args=training_args) >>> # paradigm-dependent metrics >>> print("{}
 test performance before converting: {}".formate(test_dataset.dataset_name,
 metrics["test_micro_f1"])) ACE2005-EN test performance before converting:
 66.4215686224377 >>> preds = get_pred_s2s(logits, tokenizer) >>> # convert to
 the unified prediction and evaluate >>> pred_labels =
 get_ace2005_trigger_detection_s2s(preds, labels, data_args.test_file,
@@ -172,24 +172,24 @@
                            Legal     ED     LEVEN
                   Chinese  General   ED EAE DuEE
                            General   ED EAE ACE-ZH
                            Financial ED EAE FewFC
 ## Models - Paradigm - Token Classification (TC) - Sequence Labeling (SL) -
 Sequence to Sequence (Seq2Seq) - Machine Reading Comprehension (MRC) - Backbone
 - CNN / LSTM - Transformers (BERT, T5, etc.) - Aggregation - Select [CLS] -
-Dynamic/Max Pooling - Marker - GCN - Head - Linear / CRF / MRC heads ' ##
+Dynamic/Max Pooling - Marker - GCN - Head - Linear / CRF / MRC heads ##
 Contests OmniEvent plans to support various event extraction contest.
 Currently, we support the following contests and the list is continually
 updated! - [MAVEN Event Detection Challenge](https://codalab.lisn.upsaclay.fr/
 competitions/395) - [CAIL 2022: Event Detection Track](http://
 cail.cipsc.org.cn/task1.html?raceID=1&cail_tag=2022) - [LUGE: Information
 Extraction Track](https://aistudio.baidu.com/aistudio/competition/detail/46/0/
 task-definition) # Experiments We implement and evaluate state-of-the-art
 methods on some popular benchmarks using OmniEvent. The results of all Event
-Detection experiments are shown in the table below. The full results can be
+Detection experiments are shown in the table below. The **full results** can be
 accessed via the links below. - [Experiments of base models on **All_ED
 Benchmarks**](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=qp276f) -
 [Experiments of base models on **All_EAE_Benchmarks**](https://docs.qq.com/
 sheet/DRW5QQU1tZ2ViZlFo?tab=b0zjme) - [Experiments of **All_ED_Models** on ACE-
 EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=odcgnh) - [Experiments of
 **All_EAE_Models** on ACE-EN+](https://docs.qq.com/sheet/
 DRW5QQU1tZ2ViZlFo?tab=jxc1ea)
```

### Comparing `OmniEvent-0.1.5/README.md` & `OmniEvent-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
 OmniEvent evaluates models of different paradigms in a unified manner, where the predictions of different models are converted to predictions on the same candidate sets and then evaluated.
 
 ```python  
 >>> from OmniEvent.evaluation.utils import predict, get_pred_s2s
 >>> from OmniEvent.evaluation.convert_format import get_ace2005_trigger_detection_s2s
 
->>> logits, labels, metrics, test_dataset = predict(trainer=trainer, tokenizer=tokenizer, data_class=data_class,
+>>> logits, labels, metrics, test_dataset = predict(trainer=trainer, tokenizer=tokenizer, data_class=EDSeq2SeqProcessor,
                                                     data_args=data_args, data_file=data_args.test_file,
                                                     training_args=training_args)
 >>> # paradigm-dependent metrics
 >>> print("{} test performance before converting: {}".formate(test_dataset.dataset_name, metrics["test_micro_f1"]))  
 ACE2005-EN test performance before converting: 66.4215686224377
 
 >>> preds = get_pred_s2s(logits, tokenizer)
@@ -324,25 +324,28 @@
 - Aggregation
   - Select [CLS]
   - Dynamic/Max Pooling
   - Marker
   - GCN
 - Head
   - Linear / CRF / MRC heads
-'
 
 ## Contests
 OmniEvent plans to support various event extraction contest. Currently, we support the following contests and the list is continually updated!
 
 - [MAVEN Event Detection Challenge](https://codalab.lisn.upsaclay.fr/competitions/395)
 - [CAIL 2022: Event Detection Track](http://cail.cipsc.org.cn/task1.html?raceID=1&cail_tag=2022)
 - [LUGE: Information Extraction Track](https://aistudio.baidu.com/aistudio/competition/detail/46/0/task-definition)
 
 # Experiments
-We implement and evaluate state-of-the-art methods on some popular benchmarks using OmniEvent. The results of all Event Detection experiments are shown in the table below. The full results can be accessed via the links below.
+We implement and evaluate state-of-the-art methods on some popular benchmarks using OmniEvent. 
+
+The results of all Event Detection experiments are shown in the table below. 
+
+The **full results** can be accessed via the links below.
 
 - [Experiments of base models on <u>**All ED Benchmarks**</u>](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=qp276f)
 - [Experiments of base models on <u>**All EAE Benchmarks**</u>](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=b0zjme)
 - [Experiments of <u>**All ED Models**</u> on ACE-EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=odcgnh)
 - [Experiments of <u>**All EAE Models**</u> on ACE-EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=jxc1ea)
```

#### html2text {}

```diff
@@ -125,15 +125,15 @@
 Since the metrics in Step 4 depend on the paradigm, it is not fair to directly
 compare the performance of models in different paradigms. OmniEvent evaluates
 models of different paradigms in a unified manner, where the predictions of
 different models are converted to predictions on the same candidate sets and
 then evaluated. ```python >>> from OmniEvent.evaluation.utils import predict,
 get_pred_s2s >>> from OmniEvent.evaluation.convert_format import
 get_ace2005_trigger_detection_s2s >>> logits, labels, metrics, test_dataset =
-predict(trainer=trainer, tokenizer=tokenizer, data_class=data_class,
+predict(trainer=trainer, tokenizer=tokenizer, data_class=EDSeq2SeqProcessor,
 data_args=data_args, data_file=data_args.test_file,
 training_args=training_args) >>> # paradigm-dependent metrics >>> print("{}
 test performance before converting: {}".formate(test_dataset.dataset_name,
 metrics["test_micro_f1"])) ACE2005-EN test performance before converting:
 66.4215686224377 >>> preds = get_pred_s2s(logits, tokenizer) >>> # convert to
 the unified prediction and evaluate >>> pred_labels =
 get_ace2005_trigger_detection_s2s(preds, labels, data_args.test_file,
@@ -151,24 +151,24 @@
                            Legal     ED     LEVEN
                   Chinese  General   ED EAE DuEE
                            General   ED EAE ACE-ZH
                            Financial ED EAE FewFC
 ## Models - Paradigm - Token Classification (TC) - Sequence Labeling (SL) -
 Sequence to Sequence (Seq2Seq) - Machine Reading Comprehension (MRC) - Backbone
 - CNN / LSTM - Transformers (BERT, T5, etc.) - Aggregation - Select [CLS] -
-Dynamic/Max Pooling - Marker - GCN - Head - Linear / CRF / MRC heads ' ##
+Dynamic/Max Pooling - Marker - GCN - Head - Linear / CRF / MRC heads ##
 Contests OmniEvent plans to support various event extraction contest.
 Currently, we support the following contests and the list is continually
 updated! - [MAVEN Event Detection Challenge](https://codalab.lisn.upsaclay.fr/
 competitions/395) - [CAIL 2022: Event Detection Track](http://
 cail.cipsc.org.cn/task1.html?raceID=1&cail_tag=2022) - [LUGE: Information
 Extraction Track](https://aistudio.baidu.com/aistudio/competition/detail/46/0/
 task-definition) # Experiments We implement and evaluate state-of-the-art
 methods on some popular benchmarks using OmniEvent. The results of all Event
-Detection experiments are shown in the table below. The full results can be
+Detection experiments are shown in the table below. The **full results** can be
 accessed via the links below. - [Experiments of base models on **All_ED
 Benchmarks**](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=qp276f) -
 [Experiments of base models on **All_EAE_Benchmarks**](https://docs.qq.com/
 sheet/DRW5QQU1tZ2ViZlFo?tab=b0zjme) - [Experiments of **All_ED_Models** on ACE-
 EN+](https://docs.qq.com/sheet/DRW5QQU1tZ2ViZlFo?tab=odcgnh) - [Experiments of
 **All_EAE_Models** on ACE-EN+](https://docs.qq.com/sheet/
 DRW5QQU1tZ2ViZlFo?tab=jxc1ea)
```

### Comparing `OmniEvent-0.1.5/pyproject.toml` & `OmniEvent-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "OmniEvent.input_engineering",
     "OmniEvent.model"
 ]
 
 
 [project]
 name = "OmniEvent"
-version = "0.1.5"
+version = "0.1.6"
 description = "A tookit for event extraction."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

