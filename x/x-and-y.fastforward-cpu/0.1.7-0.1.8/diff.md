# Comparing `tmp/x-and-y.fastforward-cpu-0.1.7.tar.gz` & `tmp/x-and-y.fastforward-cpu-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-and-y.fastforward-cpu-0.1.7.tar", last modified: Thu Sep  1 18:49:56 2022, max compression
+gzip compressed data, was "x-and-y.fastforward-cpu-0.1.8.tar", last modified: Mon May 15 11:27:48 2023, max compression
```

## Comparing `x-and-y.fastforward-cpu-0.1.7.tar` & `x-and-y.fastforward-cpu-0.1.8.tar`

### file list

```diff
@@ -1,114 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.282778 x-and-y.fastforward-cpu-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.262777 x-and-y.fastforward-cpu-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.266778 x-and-y.fastforward-cpu-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/.github/workflows/push-to-pip.yml
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    11383 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-09-01 18:49:56.282778 x-and-y.fastforward-cpu-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.270778 x-and-y.fastforward-cpu-0.1.7/fastforward/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.270778 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.270778 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/dummy/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/dummy/config.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/dummy/info.json
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/dummy/model.onnx
--rw-r--r--   0 runner    (1001) docker     (121)   466248 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/dummy/tokenizer.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.274778 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/metric/
--rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/metric/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/metric/profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_classification_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_cross_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_question_answering_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_sequence_similarity_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4473 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_summarization_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.274778 x-and-y.fastforward-cpu-0.1.7/fastforward/engine/
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/engine/abstract_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.274778 x-and-y.fastforward-cpu-0.1.7/fastforward/engine/listener/
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/engine/listener/onnx_listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     2982 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/engine/onnx_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.274778 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12046 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generation_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8893 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generation_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.274778 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/abstract_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/bart_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/marian_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/pegasus_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/t5_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.274778 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.278778 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/
--rw-r--r--   0 runner    (1001) docker     (121)     4658 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4340 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/abstract_logits_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/encoder_no_repeat_ngram.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/forced_bos_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/forced_eos_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/hamming_diversity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/inf_nan_remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/min_length.py
--rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/no_bad_words.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/no_repeat_ngram.py
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/prefix_constrained.py
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/repetition_penalty.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.278778 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/abstract_stopping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/max_length_criteria.py
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/max_new_tokens_criteria.py
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/max_time_criteria.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/abstract_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.278778 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/beam/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/beam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7402 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/beam/beam_search.py
--rw-r--r--   0 runner    (1001) docker     (121)    12028 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/beam/beam_search_scorer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/beam_gen_mode_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.278778 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/greedy/
--rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/greedy/greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/greedy_gen_mode_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.278778 x-and-y.fastforward-cpu-0.1.7/fastforward/mixin/
--rw-r--r--   0 runner    (1001) docker     (121)     5816 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/mixin/registry_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_cross_encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)     3035 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_question_answering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_sequence_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_sequence_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_summarization.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.278778 x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/
--rw-r--r--   0 runner    (1001) docker     (121)     7308 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/qa_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     9000 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/qa_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3065 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/squad_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/squad_features.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.278778 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/abstract_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.282778 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9058 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/fast_tokenizer_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/prefix_tokenizer_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/type_tokenizer_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6138 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/marian_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.282778 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/mixin/
--rw-r--r--   0 runner    (1001) docker     (121)     4764 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/mixin/special_tokens_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/tokenizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.282778 x-and-y.fastforward-cpu-0.1.7/fastforward/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/fastforward/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-01 18:49:56.282778 x-and-y.fastforward-cpu-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-09-01 18:49:44.000000 x-and-y.fastforward-cpu-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 18:49:56.282778 x-and-y.fastforward-cpu-0.1.7/x_and_y.fastforward_cpu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-09-01 18:49:55.000000 x-and-y.fastforward-cpu-0.1.7/x_and_y.fastforward_cpu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4261 2022-09-01 18:49:56.000000 x-and-y.fastforward-cpu-0.1.7/x_and_y.fastforward_cpu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 18:49:55.000000 x-and-y.fastforward-cpu-0.1.7/x_and_y.fastforward_cpu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-01 18:49:55.000000 x-and-y.fastforward-cpu-0.1.7/x_and_y.fastforward_cpu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-01 18:49:55.000000 x-and-y.fastforward-cpu-0.1.7/x_and_y.fastforward_cpu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.397502 x-and-y.fastforward-cpu-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.401502 x-and-y.fastforward-cpu-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/.github/workflows/push-to-pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.401502 x-and-y.fastforward-cpu-0.1.8/fastforward/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.401502 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.405502 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/dummy/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/dummy/info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/dummy/model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)   466248 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/dummy/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/lo_951_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.405502 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/metric/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/metric/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_cross_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_question_answering_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_sequence_similarity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_summarization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.405502 x-and-y.fastforward-cpu-0.1.8/fastforward/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/engine/abstract_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.405502 x-and-y.fastforward-cpu-0.1.8/fastforward/engine/listener/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/engine/listener/onnx_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/engine/onnx_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.405502 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generation_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.405502 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/abstract_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/bart_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/marian_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/pegasus_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/t5_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.405502 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.405502 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/abstract_logits_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/encoder_no_repeat_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/forced_bos_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/forced_eos_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/hamming_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/inf_nan_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/min_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/no_bad_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/no_repeat_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/prefix_constrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/repetition_penalty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/abstract_stopping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/max_length_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/max_new_tokens_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/max_time_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/abstract_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/beam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/beam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/beam/beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/beam/beam_search_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/beam_gen_mode_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/greedy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/greedy/greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/greedy_gen_mode_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/mixin/registry_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_cross_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_sequence_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_sequence_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/qa_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/qa_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/squad_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/squad_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/abstract_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/fast_tokenizer_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/prefix_tokenizer_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/type_tokenizer_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/marian_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/mixin/special_tokens_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/tokenizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/fastforward/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/fastforward/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-15 11:27:43.000000 x-and-y.fastforward-cpu-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:27:48.409502 x-and-y.fastforward-cpu-0.1.8/x_and_y.fastforward_cpu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-15 11:27:48.000000 x-and-y.fastforward-cpu-0.1.8/x_and_y.fastforward_cpu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-15 11:27:48.000000 x-and-y.fastforward-cpu-0.1.8/x_and_y.fastforward_cpu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:27:48.000000 x-and-y.fastforward-cpu-0.1.8/x_and_y.fastforward_cpu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:27:48.000000 x-and-y.fastforward-cpu-0.1.8/x_and_y.fastforward_cpu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 11:27:48.000000 x-and-y.fastforward-cpu-0.1.8/x_and_y.fastforward_cpu.egg-info/top_level.txt
```

### Comparing `x-and-y.fastforward-cpu-0.1.7/.github/workflows/build-and-test.yml` & `x-and-y.fastforward-cpu-0.1.8/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/.github/workflows/push-to-pip.yml` & `x-and-y.fastforward-cpu-0.1.8/.github/workflows/push-to-pip.yml`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/LICENSE.txt` & `x-and-y.fastforward-cpu-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/PKG-INFO` & `x-and-y.fastforward-cpu-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: x-and-y.fastforward-cpu
-Version: 0.1.7
+Version: 0.1.8
 Summary: Fastforward is an inference engine for efficient AI models.
 Home-page: https://github.com/c7nw3r/fastforward
 Author: x-and-y
 Author-email: christian.weber@leftshift.one
 License: Apache Software License
-Download-URL: https://github.com/c7nw3r/fastforward/archive/refs/tags/v0.1.6.tar.gz
+Download-URL: https://github.com/c7nw3r/fastforward/archive/refs/tags/v0.1.8.tar.gz
 Description: *fastforward*
         
         Fastforward is an inference engine for efficient AI models.
 Keywords: onnx-engine,machine-learning,artificial-intelligence
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/dummy/tokenizer.json` & `x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/dummy/tokenizer.json`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/metric/benchmark.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/metric/benchmark.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_cross_encoding_test.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_cross_encoding_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import unittest
+import os
 
 from fastforward.model_for_cross_encoding import ModelForCrossEncoding
 
 
 class ModelForCrossEncodingTest(unittest.TestCase):
 
+    base_path = os.path.dirname(os.path.abspath(__file__))
+
     def test_encode(self):
-        encoder = ModelForCrossEncoding("./dummy", use_sigmoid=True)
+        encoder = ModelForCrossEncoding(
+            f"{self.base_path}/dummy", use_sigmoid=True)
         self.assertTrue(encoder(("A", "B")) is not None)
         self.assertTrue(encoder(("A", "B")) is not None)
 
     def test_encode_batch(self):
-        encoder = ModelForCrossEncoding("./dummy", use_sigmoid=True)
+        encoder = ModelForCrossEncoding(
+            f"{self.base_path}/dummy", use_sigmoid=True)
         self.assertEqual(len(encoder([("A", "B"), ("A", "B")])), 2)
         self.assertEqual(len(encoder([("A", "B"), ("A", "B")])), 2)
 
     def test_encode_batch_with_different_sequence_lengths(self):
-        encoder = ModelForCrossEncoding("./dummy", use_sigmoid=True)
+        encoder = ModelForCrossEncoding(
+            f"{self.base_path}/dummy", use_sigmoid=True)
         self.assertEqual(len(encoder([("A", "B"), ("A", "B")])), 2)
-        self.assertEqual(len(encoder([("A", "B C"), ("A", "B C D E")])), 2)
+        self.assertEqual(len(encoder([("A", "B C"), ("A", "B C D E")])), 2)
```

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_question_answering_test.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_question_answering_test.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/__test__/model_for_summarization_test.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/__test__/model_for_summarization_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
-
+import pytest
 from fastforward.__test__.metric.benchmark import benchmark
 from fastforward.__test__.metric.profiler import Profiler
 from fastforward.engine.listener.onnx_listener import OnnxListener
 from fastforward.model_for_summarization import ModelForSummarization
 
-
+@pytest.mark.skip(reason="no way of currently testing this")
 class ModelForSummarizationTest(unittest.TestCase):
 
     def test_gpu(self):
         text = """Computer Space is a space-combat arcade game released in 1971. Created by Nolan Bushnell and 
         Ted Dabney in partnership as Syzygy Engineering, it was the first arcade video game and the first commercially 
         available video game. In the game the player controls a rocket engaged in a missile battle against a pair of 
         hardware-controlled flying saucers set against a starfield background."""
```

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/config.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/config.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/engine/abstract_engine.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/engine/listener/onnx_listener.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/engine/listener/onnx_listener.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/engine/onnx_engine.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/engine/onnx_engine.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generation_config.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generation_config.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generation_mixin.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generation_mixin.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/__init__.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/abstract_generator.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/abstract_generator.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/bart_generator.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/bart_generator.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/marian_generator.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/marian_generator.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/pegasus_generator.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/pegasus_generator.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/generator/t5_generator.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/generator/t5_generator.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/__init__.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/__init__.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/abstract_logits_processor.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/abstract_logits_processor.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/encoder_no_repeat_ngram.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/encoder_no_repeat_ngram.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/forced_bos_token.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/forced_bos_token.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/forced_eos_token.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/forced_eos_token.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/hamming_diversity.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/hamming_diversity.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/inf_nan_remove.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/inf_nan_remove.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/min_length.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/min_length.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/no_bad_words.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/no_bad_words.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/no_repeat_ngram.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/no_repeat_ngram.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/prefix_constrained.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/prefix_constrained.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_logits_processor/repetition_penalty.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_logits_processor/repetition_penalty.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/__init__.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/abstract_stopping_criteria.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/abstract_stopping_criteria.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/max_length_criteria.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/max_length_criteria.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/max_new_tokens_criteria.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/max_new_tokens_criteria.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/_stopping_criteria/max_time_criteria.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/_stopping_criteria/max_time_criteria.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/abstract_strategy.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/abstract_strategy.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/beam/beam_search.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/beam/beam_search.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/beam/beam_search_scorer.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/beam/beam_search_scorer.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/beam_gen_mode_strategy.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/beam_gen_mode_strategy.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/greedy/greedy_search.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/greedy/greedy_search.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/generation/strategy/greedy_gen_mode_strategy.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/generation/strategy/greedy_gen_mode_strategy.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/mixin/registry_mixin.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/mixin/registry_mixin.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_cross_encoding.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_cross_encoding.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_encoding.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_encoding.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_generic.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_generic.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_question_answering.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_sequence_classification.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_sequence_similarity.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_sequence_similarity.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_summarization.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_summarization.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/model_for_translation.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/model_for_translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 class ModelForTranslation(GenerationMixin, FastForwardModel):
 
     def __init__(self, config_path: str, listeners: EngineListeners = None):
         super().__init__(config_path, listeners)
 
     def __call__(self, text: Union[str, List[str]], **kwargs):
         batch = self.sequence_to_ids(text)
-        output = self.generate(GenerationConfig(self.config, **batch, **kwargs))
+        output = self.generate(GenerationConfig(
+            self.config, **batch, **kwargs))
 
         return self.ids_to_sequence(output)
 
     def get_onnx_session(self) -> InferenceSession:
         return self.generator.decoder.onnx_session
```

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/qa_postprocessor.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/qa_postprocessor.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/qa_preprocessor.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/qa_preprocessor.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/squad_example.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/squad_example.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/questionanswering/squad_features.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/questionanswering/squad_features.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/__init__.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/abstract_tokenizer.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/abstract_tokenizer.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/__init__.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/fast_tokenizer_adapter.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/fast_tokenizer_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,42 +20,41 @@
 import numpy as np
 from tokenizers import Tokenizer
 
 from fastforward.config import ModelConfig
 from fastforward.tokenizer.abstract_tokenizer import AbstractTokenizer, NetworkInfo, EncodingConfig, Input
 from fastforward.tokenizer.tokenizer_config import TokenizerConfig, TruncationStrategy, PaddingStrategy, EncodingFast
 
+from threading import RLock
+
 
 class FastTokenizerAdapter(AbstractTokenizer):
+
     def __init__(self, config: ModelConfig, network_info: NetworkInfo):
-        self.tokenizer = Tokenizer.from_file(config.config_path + "/tokenizer.json")
+        self.tokenizer = Tokenizer.from_file(
+            config.config_path + "/tokenizer.json")
         self.network_info = network_info
+        self.lock = RLock()
 
         with open(config.config_path + "/tokenizer.json", encoding="utf-8") as config_file:
             self.config = TokenizerConfig(json.load(config_file))
 
         if isfile(config.config_path + "/tokenizer_init.json"):
             with open(config.config_path + "/tokenizer_init.json", "r", encoding="utf-8") as f:
                 config = json.load(f)
                 if "do_lower_case" in config and config["do_lower_case"]:
                     from tokenizers.normalizers import Lowercase, Sequence
                     # noinspection PyArgumentList
-                    normalizer = Sequence([Lowercase(), self.tokenizer.normalizer])
+                    normalizer = Sequence(
+                        [Lowercase(), self.tokenizer.normalizer])
                     # noinspection PyPropertyAccess
                     self.tokenizer.normalizer = normalizer
 
     def encode(self, sequence: Input, config: EncodingConfig = EncodingConfig()):
-        self.set_truncation_and_padding(config)
-
-        encodings = self.tokenizer.encode_batch(
-            sequence if isinstance(sequence, list) else [sequence],
-            add_special_tokens=config.add_special_tokens,
-            is_pretokenized=config.is_split_into_words
-        )
-
+        encodings = self._do_encode(sequence, config)
         tokens_and_encodings = [
             self._convert_encoding(
                 encoding=encoding,
                 return_token_type_ids=config.return_token_type_ids,
                 return_attention_mask=config.return_attention_mask,
                 return_overflowing_tokens=config.return_overflowing_tokens,
                 return_special_tokens_mask=config.return_special_tokens_mask,
@@ -70,33 +69,52 @@
         # (we say ~ because the number of overflow varies with the example in the batch)
         #
         # To match each overflowing sample with the original sample in the batch
         # we add an overflow_to_sample_mapping array (see below)
         sanitized_tokens = {}
         for key in tokens_and_encodings[0][0].keys():
             if key in self.network_info.get_input_names():
-                stack = [np.array(e) for item, _ in tokens_and_encodings for e in item[key]]
+                stack = [np.array(e) for item,
+                         _ in tokens_and_encodings for e in item[key]]
                 sanitized_tokens[key] = stack
-        sanitized_encodings = [e for _, item in tokens_and_encodings for e in item]
+        sanitized_encodings = [
+            e for _, item in tokens_and_encodings for e in item]
 
         # If returning overflowing tokens, we need to return a mapping
         # from the batch idx to the original sample
         if config.return_overflowing_tokens:
             overflow_to_sample_mapping = []
             for i, (toks, _) in enumerate(tokens_and_encodings):
                 overflow_to_sample_mapping += [i] * len(toks["input_ids"])
 
             # FIXME: ValueError: no node with name 'overflow_to_sample_mapping' found
             # sanitized_tokens["overflow_to_sample_mapping"] = overflow_to_sample_mapping
         return BatchEncoding(sanitized_tokens, sanitized_encodings)
 
+    def _do_encode(self, sequence: Input, config: EncodingConfig) -> Any:
+        """
+        Non ideal quickfix for:
+            https://github.com/huggingface/tokenizers/issues/537
+        """
+        with self.lock:
+            self.set_truncation_and_padding(config)
+            return self.tokenizer.encode_batch(
+                sequence if isinstance(sequence, list) else [
+                    sequence],
+                add_special_tokens=config.add_special_tokens,
+                is_pretokenized=config.is_split_into_words
+            )
+
     def decode(self, output: np.array, skip_special_token: bool = False):
         # FIXME: summarization
         output = output.astype(np.int32)
-        return self.tokenizer.decode_batch(output, skip_special_tokens=skip_special_token)
+        # quickfix: https://github.com/huggingface/tokenizers/issues/537
+        with self.lock:
+            return self.tokenizer.decode_batch(output, skip_special_tokens=skip_special_token)
+
 
     def set_truncation_and_padding(self, config: EncodingConfig):
         """
         Define the truncation and the padding strategies for fast tokenizers (provided by HuggingFace tokenizers
         library) and restore the tokenizer settings afterwards.
 
         The provided tokenizer has no padding / truncation strategy before the managed section. If your tokenizer set a
@@ -165,15 +183,16 @@
             encoding_dict["input_ids"].append(e.ids)
 
             if return_token_type_ids:
                 encoding_dict["token_type_ids"].append(e.type_ids)
             if return_attention_mask:
                 encoding_dict["attention_mask"].append(e.attention_mask)
             if return_special_tokens_mask:
-                encoding_dict["special_tokens_mask"].append(e.special_tokens_mask)
+                encoding_dict["special_tokens_mask"].append(
+                    e.special_tokens_mask)
             if return_offsets_mapping:
                 encoding_dict["offset_mapping"].append(e.offsets)
             if return_length:
                 encoding_dict["length"].append(len(e.ids))
 
         return encoding_dict, encodings
 
@@ -185,9 +204,10 @@
         self.encodings = encoding if isinstance(encoding, list) else [encoding]
 
     def sequence_ids(self, batch_index: int = 0) -> List[Optional[int]]:
         """
         Return a list mapping the tokens to the id of their original sentences:
         """
         if not self.encodings:
-            raise ValueError("sequence_ids() is not available when using Python-based tokenizers")
+            raise ValueError(
+                "sequence_ids() is not available when using Python-based tokenizers")
         return self.encodings[batch_index].sequence_ids
```

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/prefix_tokenizer_adapter.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/prefix_tokenizer_adapter.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/adapter/type_tokenizer_adapter.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/adapter/type_tokenizer_adapter.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/marian_tokenizer.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/marian_tokenizer.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/mixin/special_tokens_mixin.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/mixin/special_tokens_mixin.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/tokenizer/tokenizer_config.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/tokenizer/tokenizer_config.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/utils/__init__.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/utils/environment.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/utils/environment.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/fastforward/utils/numpy_utils.py` & `x-and-y.fastforward-cpu-0.1.8/fastforward/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `x-and-y.fastforward-cpu-0.1.7/setup.py` & `x-and-y.fastforward-cpu-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import find_packages, setup
 
 long_description = Path(__file__).with_name("README.md").read_text()
 
 setup(
     name='x-and-y.fastforward-cpu',
     packages=find_packages(exclude=("__tests__","fastforward.__tests__")),
-    version='0.1.7',
+    version='0.1.8',
     license='Apache Software License',
     description='Fastforward is an inference engine for efficient AI models.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='x-and-y',
     author_email='christian.weber@leftshift.one',
     url='https://github.com/c7nw3r/fastforward',
-    download_url='https://github.com/c7nw3r/fastforward/archive/refs/tags/v0.1.6.tar.gz',
+    download_url='https://github.com/c7nw3r/fastforward/archive/refs/tags/v0.1.8.tar.gz',
     keywords=['onnx-engine', 'machine-learning', 'artificial-intelligence'],
     setup_requires=['setuptools_scm'],
     include_package_data=True,
     install_requires=[
         str(r)
         for r in pkg_resources.parse_requirements(
             open(os.path.join(os.path.dirname(__file__), "requirements.txt"))
```

### Comparing `x-and-y.fastforward-cpu-0.1.7/x_and_y.fastforward_cpu.egg-info/PKG-INFO` & `x-and-y.fastforward-cpu-0.1.8/x_and_y.fastforward_cpu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: x-and-y.fastforward-cpu
-Version: 0.1.7
+Version: 0.1.8
 Summary: Fastforward is an inference engine for efficient AI models.
 Home-page: https://github.com/c7nw3r/fastforward
 Author: x-and-y
 Author-email: christian.weber@leftshift.one
 License: Apache Software License
-Download-URL: https://github.com/c7nw3r/fastforward/archive/refs/tags/v0.1.6.tar.gz
+Download-URL: https://github.com/c7nw3r/fastforward/archive/refs/tags/v0.1.8.tar.gz
 Description: *fastforward*
         
         Fastforward is an inference engine for efficient AI models.
 Keywords: onnx-engine,machine-learning,artificial-intelligence
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-and-y.fastforward-cpu-0.1.7/x_and_y.fastforward_cpu.egg-info/SOURCES.txt` & `x-and-y.fastforward-cpu-0.1.8/x_and_y.fastforward_cpu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 LICENSE.txt
 README.md
+requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/build-and-test.yml
 .github/workflows/push-to-pip.yml
 fastforward/__init__.py
 fastforward/config.py
@@ -13,14 +14,15 @@
 fastforward/model_for_encoding.py
 fastforward/model_for_generic.py
 fastforward/model_for_question_answering.py
 fastforward/model_for_sequence_classification.py
 fastforward/model_for_sequence_similarity.py
 fastforward/model_for_summarization.py
 fastforward/model_for_translation.py
+fastforward/__test__/lo_951_test.py
 fastforward/__test__/model_for_classification_test.py
 fastforward/__test__/model_for_cross_encoding_test.py
 fastforward/__test__/model_for_encoding_test.py
 fastforward/__test__/model_for_question_answering_test.py
 fastforward/__test__/model_for_sequence_similarity_test.py
 fastforward/__test__/model_for_summarization_test.py
 fastforward/__test__/dummy/config.json
```

