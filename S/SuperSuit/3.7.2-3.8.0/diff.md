# Comparing `tmp/SuperSuit-3.7.2.tar.gz` & `tmp/SuperSuit-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SuperSuit-3.7.2.tar", last modified: Mon Mar 20 14:50:16 2023, max compression
+gzip compressed data, was "SuperSuit-3.8.0.tar", last modified: Mon May 15 21:03:05 2023, max compression
```

## Comparing `SuperSuit-3.7.2.tar` & `SuperSuit-3.8.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.220735 SuperSuit-3.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-20 14:50:16.220735 SuperSuit-3.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.212735 SuperSuit-3.7.2/SuperSuit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-20 14:50:16.000000 SuperSuit-3.7.2/SuperSuit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-20 14:50:16.000000 SuperSuit-3.7.2/SuperSuit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 14:50:16.000000 SuperSuit-3.7.2/SuperSuit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-20 14:50:16.000000 SuperSuit-3.7.2/SuperSuit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-20 14:50:16.000000 SuperSuit-3.7.2/SuperSuit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 14:50:16.220735 SuperSuit-3.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.212735 SuperSuit-3.7.2/supersuit/
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.212735 SuperSuit-3.7.2/supersuit/aec_vector/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/aec_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/aec_vector/async_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/aec_vector/base_aec_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/aec_vector/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/aec_vector/vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.212735 SuperSuit-3.7.2/supersuit/generic_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/basic_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/delay_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/frame_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/max_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/nan_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/sticky_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.212735 SuperSuit-3.7.2/supersuit/generic_wrappers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/utils/base_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/generic_wrappers/utils/shared_wrapper_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.212735 SuperSuit-3.7.2/supersuit/lambda_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/lambda_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/lambda_wrappers/action_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/lambda_wrappers/observation_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/lambda_wrappers/reward_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.216735 SuperSuit-3.7.2/supersuit/multiagent_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/multiagent_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/multiagent_wrappers/agent_indication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/multiagent_wrappers/black_death.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/multiagent_wrappers/padding_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.216735 SuperSuit-3.7.2/supersuit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/accumulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.216735 SuperSuit-3.7.2/supersuit/utils/action_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/action_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/action_transforms/homogenize_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/agent_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/base_aec_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.216735 SuperSuit-3.7.2/supersuit/utils/basic_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/basic_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/basic_transforms/color_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/basic_transforms/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/basic_transforms/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/basic_transforms/normalize_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/basic_transforms/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/basic_transforms/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/convert_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/frame_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/make_defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/obs_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/utils/wrapper_chooser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.216735 SuperSuit-3.7.2/supersuit/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/concat_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/markov_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/multiproc_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/sb3_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/sb_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/single_vec_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.216735 SuperSuit-3.7.2/supersuit/vector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/utils/shared_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/utils/space_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/supersuit/vector/vector_constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.220735 SuperSuit-3.7.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/aec_mock_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/aec_unwrapped_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/dummy_aec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/dummy_gym_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/generated_agents_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/gym_mock_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/gym_unwrapped_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/parallel_env_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/pettingzoo_api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_autodep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:16.220735 SuperSuit-3.7.2/test/test_vector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_vector/test_aec_vector_identity_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_vector/test_aec_vector_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_vector/test_env_is_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_vector/test_gym_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_vector/test_pettingzoo_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_vector/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/test_vector/test_vector_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-20 14:50:11.000000 SuperSuit-3.7.2/test/vec_env_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.030030 SuperSuit-3.8.0/SuperSuit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 21:03:05.000000 SuperSuit-3.8.0/SuperSuit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.030030 SuperSuit-3.8.0/supersuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.030030 SuperSuit-3.8.0/supersuit/aec_vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/async_vector_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/base_aec_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/aec_vector/vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/generic_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/basic_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/delay_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/frame_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/frame_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/max_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/nan_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/sticky_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/generic_wrappers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/utils/base_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/generic_wrappers/utils/shared_wrapper_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/lambda_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/lambda_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/lambda_wrappers/action_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/lambda_wrappers/observation_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/lambda_wrappers/reward_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/multiagent_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/multiagent_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/multiagent_wrappers/agent_indication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/multiagent_wrappers/black_death.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/multiagent_wrappers/padding_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/accumulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/utils/action_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/action_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/action_transforms/homogenize_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/agent_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/base_aec_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.034030 SuperSuit-3.8.0/supersuit/utils/basic_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/color_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/normalize_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/basic_transforms/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/convert_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/frame_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/frame_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/make_defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/obs_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/utils/wrapper_chooser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/supersuit/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/concat_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/markov_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/multiproc_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/sb3_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/sb_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/single_vec_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/supersuit/vector/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/utils/shared_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/utils/space_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/supersuit/vector/vector_constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/aec_mock_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/aec_unwrapped_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/dummy_aec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/dummy_gym_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/generated_agents_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/gym_mock_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/gym_unwrapped_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/parallel_env_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/pettingzoo_api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_autodep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.038030 SuperSuit-3.8.0/test/test_vector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_aec_vector_identity_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_aec_vector_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_env_is_wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_gym_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_pettingzoo_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/test_vector/test_vector_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-15 21:03:02.000000 SuperSuit-3.8.0/test/vec_env_test.py
```

### Comparing `SuperSuit-3.7.2/LICENSE.txt` & `SuperSuit-3.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/PKG-INFO` & `SuperSuit-3.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperSuit
-Version: 3.7.2
+Version: 3.8.0
 Summary: Wrappers for Gymnasium and PettingZoo
 Home-page: https://github.com/Farama-Foundation/SuperSuit
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI,gymnasium
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `SuperSuit-3.7.2/README.md` & `SuperSuit-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/SuperSuit.egg-info/PKG-INFO` & `SuperSuit-3.8.0/SuperSuit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperSuit
-Version: 3.7.2
+Version: 3.8.0
 Summary: Wrappers for Gymnasium and PettingZoo
 Home-page: https://github.com/Farama-Foundation/SuperSuit
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI,gymnasium
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `SuperSuit-3.7.2/SuperSuit.egg-info/SOURCES.txt` & `SuperSuit-3.8.0/SuperSuit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/setup.py` & `SuperSuit-3.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     url="https://github.com/Farama-Foundation/SuperSuit",
     license_files=("LICENSE.txt",),
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["Reinforcement Learning", "game", "RL", "AI", "gymnasium"],
     python_requires=">=3.7, <3.12",
     packages=find_packages(),
-    install_requires=["numpy>=1.19.0", "gymnasium>=0.26.0"],
-    extras={"dev": ["pettingzoo[butterfly]"]},
+    install_requires=["numpy>=1.19.0", "gymnasium>=0.26.0", "tinyscaler>=1.2.5"],
+    extras={"dev": ["pettingzoo[butterfly]>=1.23.0"]},
     classifiers=[
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: MIT License",
```

### Comparing `SuperSuit-3.7.2/supersuit/__init__.py` & `SuperSuit-3.8.0/supersuit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,8 +61,8 @@
                     raise DeprecatedWrapper(
                         f"{base}{version_num} is now deprecated, use {base}{act_version_num} instead"
                     )
 
     raise ImportError(f"cannot import name '{wrapper_name}' from 'supersuit'")
 
 
-__version__ = "3.7.2"
+__version__ = "3.8.0"
```

### Comparing `SuperSuit-3.7.2/supersuit/aec_vector/async_vector_env.py` & `SuperSuit-3.8.0/supersuit/aec_vector/async_vector_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/aec_vector/base_aec_vec_env.py` & `SuperSuit-3.8.0/supersuit/aec_vector/base_aec_vec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/aec_vector/create.py` & `SuperSuit-3.8.0/supersuit/aec_vector/create.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/aec_vector/vector_env.py` & `SuperSuit-3.8.0/supersuit/aec_vector/vector_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/__init__.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/basic_wrappers.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/basic_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/delay_observations.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/delay_observations.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/frame_skip.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/frame_skip.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/frame_stack.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/frame_stack.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/max_observation.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/max_observation.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/nan_wrappers.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/nan_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/sticky_actions.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/sticky_actions.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/utils/base_modifier.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/utils/base_modifier.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/generic_wrappers/utils/shared_wrapper_util.py` & `SuperSuit-3.8.0/supersuit/generic_wrappers/utils/shared_wrapper_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,23 +108,23 @@
                 if self._cur_seed is not None:
                     self._cur_seed += 1
 
     def reset(self, seed=None, options=None):
         self._cur_seed = seed
         self._cur_options = options
 
-        observations = super().reset(seed=seed, options=options)
+        observations, infos = super().reset(seed=seed, options=options)
         self.add_modifiers(self.agents)
         for agent, mod in self.modifiers.items():
             mod.reset(seed=seed, options=options)
         observations = {
             agent: self.modifiers[agent].modify_obs(obs)
             for agent, obs in observations.items()
         }
-        return observations
+        return observations, infos
 
     def step(self, actions):
         actions = {
             agent: self.modifiers[agent].modify_action(action)
             for agent, action in actions.items()
         }
         observations, rewards, terminations, truncations, infos = super().step(actions)
@@ -141,17 +141,17 @@
         super().__init__(env)
         self.modifier = modifier_class()
         self.observation_space = self.modifier.modify_obs_space(self.observation_space)
         self.action_space = self.modifier.modify_action_space(self.action_space)
 
     def reset(self, seed=None, options=None):
         self.modifier.reset(seed=seed, options=options)
-        obs = super().reset(seed=seed, options=options)
+        obs, info = super().reset(seed=seed, options=options)
         obs = self.modifier.modify_obs(obs)
-        return obs
+        return obs, info
 
     def step(self, action):
         obs, rew, term, trunc, info = super().step(self.modifier.modify_action(action))
         obs = self.modifier.modify_obs(obs)
         return obs, rew, term, trunc, info
```

### Comparing `SuperSuit-3.7.2/supersuit/lambda_wrappers/action_lambda.py` & `SuperSuit-3.8.0/supersuit/lambda_wrappers/action_lambda.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/lambda_wrappers/observation_lambda.py` & `SuperSuit-3.8.0/supersuit/lambda_wrappers/observation_lambda.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
     def step(self, action):
         observation, rew, termination, truncation, info = self.env.step(action)
         observation = self._modify_observation(observation)
         return observation, rew, termination, truncation, info
 
     def reset(self, seed=None, options=None):
-        observation = self.env.reset(seed=seed, options=options)
+        observation, infos = self.env.reset(seed=seed, options=options)
         observation = self._modify_observation(observation)
-        return observation
+        return observation, infos
 
 
 observation_lambda_v0 = WrapperChooser(
     aec_wrapper=aec_observation_lambda, gym_wrapper=gym_observation_lambda
 )
```

### Comparing `SuperSuit-3.7.2/supersuit/lambda_wrappers/reward_lambda.py` & `SuperSuit-3.8.0/supersuit/lambda_wrappers/reward_lambda.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/multiagent_wrappers/agent_indication.py` & `SuperSuit-3.8.0/supersuit/multiagent_wrappers/agent_indication.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/multiagent_wrappers/black_death.py` & `SuperSuit-3.8.0/supersuit/multiagent_wrappers/black_death.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,24 @@
         for agent in self.agents:
             space = self.observation_space(agent)
             assert isinstance(
                 space, gymnasium.spaces.Box
             ), f"observation sapces for black death must be Box spaces, is {space}"
 
     def reset(self, seed=None, options=None):
-        obss = self.env.reset(seed=seed, options=options)
+        obss, infos = self.env.reset(seed=seed, options=options)
 
         self.agents = self.env.agents[:]
         self._check_valid_for_black_death()
         black_obs = {
             agent: np.zeros_like(self.observation_space(agent).low)
             for agent in self.agents
             if agent not in obss
         }
-
-        return {**obss, **black_obs}
+        return {**obss, **black_obs}, infos
 
     def step(self, actions):
         active_actions = {agent: actions[agent] for agent in self.env.agents}
         obss, rews, terms, truncs, infos = self.env.step(active_actions)
         black_obs = {
             agent: np.zeros_like(self.observation_space(agent).low)
             for agent in self.agents
```

### Comparing `SuperSuit-3.7.2/supersuit/multiagent_wrappers/padding_wrappers.py` & `SuperSuit-3.8.0/supersuit/multiagent_wrappers/padding_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/accumulator.py` & `SuperSuit-3.8.0/supersuit/utils/accumulator.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/action_transforms/homogenize_ops.py` & `SuperSuit-3.8.0/supersuit/utils/action_transforms/homogenize_ops.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/agent_indicator.py` & `SuperSuit-3.8.0/supersuit/utils/agent_indicator.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/base_aec_wrapper.py` & `SuperSuit-3.8.0/supersuit/utils/base_aec_wrapper.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,15 +28,17 @@
         pass
 
     def reset(self, seed=None, options=None):
         super().reset(seed=seed, options=options)
         self._update_step(self.agent_selection)
 
     def observe(self, agent):
-        obs = super().observe(agent)
+        obs = super().observe(
+            agent
+        )  # problem is in this line, the obs is sometimes a different size from the obs space
         observation = self._modify_observation(agent, obs)
         return observation
 
     def step(self, action):
         agent = self.env.agent_selection
         if not self.terminations[agent] or self.truncations[agent]:
             action = self._modify_action(agent, action)
```

### Comparing `SuperSuit-3.7.2/supersuit/utils/basic_transforms/color_reduction.py` & `SuperSuit-3.8.0/supersuit/utils/basic_transforms/color_reduction.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/basic_transforms/normalize_obs.py` & `SuperSuit-3.8.0/supersuit/utils/basic_transforms/normalize_obs.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/basic_transforms/reshape.py` & `SuperSuit-3.8.0/supersuit/utils/basic_transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/basic_transforms/resize.py` & `SuperSuit-3.8.0/supersuit/utils/basic_transforms/resize.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/frame_skip.py` & `SuperSuit-3.8.0/supersuit/utils/frame_skip.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/frame_stack.py` & `SuperSuit-3.8.0/supersuit/utils/frame_stack.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/utils/wrapper_chooser.py` & `SuperSuit-3.8.0/supersuit/utils/wrapper_chooser.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/vector/concat_vec_env.py` & `SuperSuit-3.8.0/supersuit/vector/concat_vec_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,31 @@
         self.observation_space = vec_envs[0].observation_space
         self.action_space = vec_envs[0].action_space
         tot_num_envs = sum(env.num_envs for env in vec_envs)
         self.num_envs = tot_num_envs
 
     def reset(self, seed=None, options=None):
         _res_obs = []
+        _res_infos = []
 
         if seed is not None:
             for i in range(len(self.vec_envs)):
-                _obs = self.vec_envs[i].reset(seed=seed + i, options=options)
+                _obs, _info = self.vec_envs[i].reset(seed=seed + i, options=options)
                 _res_obs.append(_obs)
+                _res_infos.append(_info)
         else:
-            _res_obs = [
-                vec_env.reset(seed=None, options=options) for vec_env in self.vec_envs
-            ]
+            for i in range(len(self.vec_envs)):
+                _obs, _info = self.vec_envs[i].reset(options=options)
+                _res_obs.append(_obs)
+                _res_infos.append(_info)
+
+        # flatten infos (also done in step function)
+        flattened_infos = [info for sublist in _res_infos for info in sublist]
 
-        return self.concat_obs(_res_obs)
+        return self.concat_obs(_res_obs), flattened_infos
 
     def concat_obs(self, observations):
         return concatenate(
             self.observation_space,
             [
                 item
                 for obs in observations
@@ -82,15 +88,17 @@
             )
             idx += venv.num_envs
         observations, rewards, terminations, truncations, infos = transpose(data)
         observations = self.concat_obs(observations)
         rewards = np.concatenate(rewards, axis=0)
         terminations = np.concatenate(terminations, axis=0)
         truncations = np.concatenate(truncations, axis=0)
-        infos = sum(infos, [])
+        infos = [
+            info for sublist in infos for info in sublist
+        ]  # flatten infos from nested lists
         return observations, rewards, terminations, truncations, infos
 
     def render(self):
         return self.vec_envs[0].render()
 
     def close(self):
         for vec_env in self.vec_envs:
```

### Comparing `SuperSuit-3.7.2/supersuit/vector/constructors.py` & `SuperSuit-3.8.0/supersuit/vector/constructors.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/vector/markov_vector_wrapper.py` & `SuperSuit-3.8.0/supersuit/vector/markov_vector_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,19 @@
     def step_async(self, actions):
         self._saved_actions = actions
 
     def step_wait(self):
         return self.step(self._saved_actions)
 
     def reset(self, seed=None, options=None):
-        _observations = self.par_env.reset(seed=seed, options=options)
+        # TODO: should this be changed to infos?
+        _observations, infos = self.par_env.reset(seed=seed, options=options)
         observations = self.concat_obs(_observations)
-        return observations
+        infs = [infos.get(agent, {}) for agent in self.par_env.possible_agents]
+        return observations, infs
 
     def step(self, actions):
         actions = list(iterate(self.action_space, actions))
         agent_set = set(self.par_env.agents)
         act_dict = {
             agent: actions[i]
             for i, agent in enumerate(self.par_env.possible_agents)
@@ -85,15 +87,15 @@
         tcs = np.array(
             [truncs.get(agent, False) for agent in self.par_env.possible_agents],
             dtype=np.uint8,
         )
         infs = [infos.get(agent, {}) for agent in self.par_env.possible_agents]
 
         if env_done:
-            observations = self.reset()
+            observations, infs = self.reset()
         else:
             observations = self.concat_obs(observations)
         assert (
             self.black_death or self.par_env.agents == self.par_env.possible_agents
         ), "MarkovVectorEnv does not support environments with varying numbers of active agents unless black_death is set to True"
         return observations, rews, tms, tcs, infs
```

### Comparing `SuperSuit-3.7.2/supersuit/vector/multiproc_vec.py` & `SuperSuit-3.8.0/supersuit/vector/multiproc_vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
             if instr == "close":
                 vec_env.close()
 
             elif isinstance(instr, tuple):
                 name, data = instr
 
                 if name == "reset":
-                    observations = vec_env.reset(seed=data[0], options=data[1])
+                    observations, infos = vec_env.reset(seed=data[0], options=data[1])
+                    comp_infos = compress_info(infos)
 
                     write_observations(vec_env, env_start_idx, shared_obs, observations)
                     shared_terms.np_arr[env_start_idx:env_end_idx] = False
                     shared_truncs.np_arr[env_start_idx:env_end_idx] = False
                     shared_rews.np_arr[env_start_idx:env_end_idx] = 0.0
 
                 elif name == "step":
@@ -179,14 +180,15 @@
             if seed is not None:
                 pipe.send(("reset", (seed + i, options)))
             else:
                 pipe.send(("reset", (seed, options)))
 
         self._receive_info()
 
+        # TODO: should this include info
         return numpy_deepcopy(self.observations_buffers)
 
     def step_async(self, actions):
         actions = list(iterate(self.action_space, actions))
         for i, pipe in enumerate(self.pipes):
             start, end = self.idx_starts[i : i + 2]
             pipe.send(("step", actions[start:end]))
```

### Comparing `SuperSuit-3.7.2/supersuit/vector/sb3_vector_wrapper.py` & `SuperSuit-3.8.0/supersuit/vector/sb3_vector_wrapper.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/vector/sb_vector_wrapper.py` & `SuperSuit-3.8.0/supersuit/vector/sb_vector_wrapper.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/vector/single_vec_env.py` & `SuperSuit-3.8.0/supersuit/vector/single_vec_env.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,15 @@
         self.gym_env = gym_env_fns[0]()
         self.observation_space = self.gym_env.observation_space
         self.action_space = self.gym_env.action_space
         self.num_envs = 1
         self.metadata = self.gym_env.metadata
 
     def reset(self, seed=None, options=None):
+        # TODO: should this include info
         return np.expand_dims(self.gym_env.reset(seed=seed, options=options), 0)
 
     def step_async(self, actions):
         self._saved_actions = actions
 
     def step_wait(self):
         return self.step(self._saved_actions)
```

### Comparing `SuperSuit-3.7.2/supersuit/vector/utils/shared_array.py` & `SuperSuit-3.8.0/supersuit/vector/utils/shared_array.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/supersuit/vector/vector_constructors.py` & `SuperSuit-3.8.0/supersuit/vector/vector_constructors.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/test/aec_mock_test.py` & `SuperSuit-3.8.0/test/aec_mock_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/test/aec_unwrapped_test.py` & `SuperSuit-3.8.0/test/aec_unwrapped_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/test/dummy_aec_env.py` & `SuperSuit-3.8.0/test/dummy_aec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/test/gym_mock_test.py` & `SuperSuit-3.8.0/test/gym_mock_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 base_obs_space = Box(low=np.float32(0.0), high=np.float32(10.0), shape=[8, 8, 3])
 base_act_spaces = Discrete(5)
 
 
 def test_reshape():
     base_env = DummyEnv(base_obs, base_obs_space, base_act_spaces)
     env = reshape_v0(base_env, (64, 3))
-    obs = env.reset()
+    obs, info = env.reset()
     assert obs.shape == (64, 3)
     first_obs, _, _, _, _ = env.step(5)
     assert np.all(np.equal(first_obs, base_obs.reshape([64, 3])))
 
 
 def new_continuous_dummy():
     base_act_spaces = Box(low=np.float32(0.0), high=np.float32(10.0), shape=[3])
@@ -54,50 +54,50 @@
     supersuit.nan_random_v0(new_dummy()),
     supersuit.scale_actions_v0(new_continuous_dummy(), 0.5),
 ]
 
 
 @pytest.mark.parametrize("env", wrappers)
 def test_basic_wrappers(env):
-    obs = env.reset(seed=5)
+    obs, info = env.reset(seed=5)
     act_space = env.action_space
     obs_space = env.observation_space
     assert obs_space.contains(obs)
     assert obs.dtype == obs_space.dtype
     for i in range(10):
         env.step(act_space.sample())
 
 
 def test_lambda():
     def add1(obs, obs_space):
         return obs + 1
 
     base_env = DummyEnv(base_obs, base_obs_space, base_act_spaces)
     env = observation_lambda_v0(base_env, add1)
-    obs0 = env.reset()
+    obs0, info0 = env.reset()
     assert int(obs0[0][0][0]) == 1
     env = observation_lambda_v0(env, add1)
-    obs0 = env.reset()
+    obs0, info0 = env.reset()
     assert int(obs0[0][0][0]) == 2
 
     def tile_obs(obs, obs_space):
         shape_size = len(obs.shape)
         tile_shape = [1] * shape_size
         tile_shape[0] *= 2
         return np.tile(obs, tile_shape)
 
     env = observation_lambda_v0(env, tile_obs)
-    obs0 = env.reset()
+    obs0, info0 = env.reset()
     assert env.observation_space.shape == (16, 8, 3)
 
     def change_shape_fn(obs_space):
         return Box(low=0, high=1, shape=(32, 8, 3))
 
     env = observation_lambda_v0(env, tile_obs)
-    obs0 = env.reset()
+    obs0, info0 = env.reset()
     assert env.observation_space.shape == (32, 8, 3)
     assert obs0.shape == (32, 8, 3)
 
 
 def test_action_lambda():
     def inc1(x, space):
         return x + 1
```

### Comparing `SuperSuit-3.7.2/test/gym_unwrapped_test.py` & `SuperSuit-3.8.0/test/gym_unwrapped_test.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/test/parallel_env_test.py` & `SuperSuit-3.8.0/test/parallel_env_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             self.rewards,
             self.terminations,
             self.truncations,
             self.infos,
         )
 
     def reset(self, seed=None, options=None):
-        return self._observations
+        return self._observations, self.infos
 
     def close(self):
         pass
 
 
 base_obs = {
     f"a{idx}": np.zeros([8, 8, 3], dtype=np.float32) + np.arange(3) + idx
```

### Comparing `SuperSuit-3.7.2/test/pettingzoo_api_test.py` & `SuperSuit-3.8.0/test/pettingzoo_api_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import numpy as np
 import pytest
 from pettingzoo.butterfly import knights_archers_zombies_v10
-from pettingzoo.mpe import simple_push_v2, simple_world_comm_v2
+from pettingzoo.mpe import simple_push_v3, simple_world_comm_v3
 from pettingzoo.test import api_test, parallel_test, seed_test
 
 import supersuit
 from supersuit import (
     dtype_v0,
     frame_skip_v0,
     frame_stack_v1,
     pad_action_space_v0,
     sticky_actions_v0,
 )
 
 
 def test_pettingzoo_frame_stack():
-    _env = simple_push_v2.env()
+    _env = simple_push_v3.env()
     wrapped_env = frame_stack_v1(_env)
     api_test(wrapped_env)
 
 
 def test_pettingzoo_frame_skip():
-    env = simple_push_v2.raw_env(max_cycles=100)
+    env = simple_push_v3.raw_env(max_cycles=100)
     env = frame_skip_v0(env, 3)
     env.reset()
     x = 0
     for _ in env.agent_iter(25):
         assert env.env.steps == (x // 2) * 3
         action = env.action_space(env.agent_selection).sample()
         env.step(action)
         x += 1
 
 
 def test_pettingzoo_pad_action_space():
-    _env = simple_world_comm_v2.env()
+    _env = simple_world_comm_v3.env()
     wrapped_env = pad_action_space_v0(_env)
     api_test(wrapped_env)
-    seed_test(lambda: sticky_actions_v0(simple_world_comm_v2.env(), 0.5), 100)
+    seed_test(lambda: sticky_actions_v0(simple_world_comm_v3.env(), 0.5), 100)
 
 
 def test_pettingzoo_parallel_env():
-    _env = simple_world_comm_v2.parallel_env()
+    _env = simple_world_comm_v3.parallel_env()
     wrapped_env = pad_action_space_v0(_env)
     parallel_test.parallel_api_test(wrapped_env)
 
 
 wrappers = [
     supersuit.color_reduction_v0(
         knights_archers_zombies_v10.env(vector_state=False), "R"
@@ -65,16 +65,16 @@
     supersuit.reshape_v0(
         knights_archers_zombies_v10.env(vector_state=False), (512 * 512, 3)
     ),
     supersuit.normalize_obs_v0(
         dtype_v0(knights_archers_zombies_v10.env(), np.float32), env_min=-1, env_max=5.0
     ),
     # supersuit.frame_stack_v1(combined_arms_v6.env(), 8),
-    supersuit.pad_observations_v0(simple_world_comm_v2.env()),
-    supersuit.pad_action_space_v0(simple_world_comm_v2.env()),
+    supersuit.pad_observations_v0(simple_world_comm_v3.env()),
+    supersuit.pad_action_space_v0(simple_world_comm_v3.env()),
     # supersuit.black_death_v3(combined_arms_v6.env()),
     supersuit.agent_indicator_v0(knights_archers_zombies_v10.env(), True),
     supersuit.agent_indicator_v0(knights_archers_zombies_v10.env(), False),
     supersuit.reward_lambda_v0(knights_archers_zombies_v10.env(), lambda x: x / 10),
     # supersuit.clip_reward_v0(combined_arms_v6.env()),
     supersuit.nan_noop_v0(knights_archers_zombies_v10.env(), 0),
     supersuit.nan_zeros_v0(knights_archers_zombies_v10.env()),
@@ -90,26 +90,26 @@
 @pytest.mark.parametrize("env", wrappers)
 def test_pettingzoo_aec_api(env):
     api_test(env)
 
 
 parallel_wrappers = [
     # supersuit.frame_stack_v1(combined_arms_v6.parallel_env(), 8),
-    supersuit.frame_stack_v1(simple_push_v2.parallel_env(), 8),
+    supersuit.frame_stack_v1(simple_push_v3.parallel_env(), 8),
     # supersuit.reward_lambda_v0(combined_arms_v6.parallel_env(), lambda x: x / 10),
     # supersuit.delay_observations_v0(combined_arms_v6.parallel_env(), 3),
-    supersuit.delay_observations_v0(simple_push_v2.parallel_env(), 3),
+    supersuit.delay_observations_v0(simple_push_v3.parallel_env(), 3),
     # supersuit.dtype_v0(combined_arms_v6.parallel_env(), np.int32),
     supersuit.color_reduction_v0(
         knights_archers_zombies_v10.parallel_env(vector_state=False), "R"
     ),
     # supersuit.frame_skip_v0(combined_arms_v6.parallel_env(), 4),
-    supersuit.frame_skip_v0(simple_push_v2.parallel_env(), 4),
+    supersuit.frame_skip_v0(simple_push_v3.parallel_env(), 4),
     # supersuit.max_observation_v0(combined_arms_v6.parallel_env(), 4),
     # supersuit.black_death_v3(combined_arms_v6.parallel_env()),
-    supersuit.black_death_v3(simple_push_v2.parallel_env()),
+    supersuit.black_death_v3(simple_push_v3.parallel_env()),
 ]
 
 
 @pytest.mark.parametrize("env", parallel_wrappers)
 def test_pettingzoo_parallel_api(env):
     parallel_test.parallel_api_test(env)
```

### Comparing `SuperSuit-3.7.2/test/test_vector/test_aec_vector_identity_env.py` & `SuperSuit-3.8.0/test/test_vector/test_aec_vector_identity_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/test/test_vector/test_aec_vector_values.py` & `SuperSuit-3.8.0/test/test_vector/test_aec_vector_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
 
 import numpy as np
 from pettingzoo.butterfly import knights_archers_zombies_v10
 from pettingzoo.classic import rps_v2
-from pettingzoo.mpe import simple_world_comm_v2
+from pettingzoo.mpe import simple_world_comm_v3
 
 from supersuit import vectorize_aec_env_v0
 
 
 def test_all():
     NUM_ENVS = 5
 
@@ -75,10 +75,10 @@
         test_vec_env(
             vectorize_aec_env_v0(
                 knights_archers_zombies_v10.env(), NUM_ENVS, num_cpus=num_cpus
             )
         )
         test_vec_env(
             vectorize_aec_env_v0(
-                simple_world_comm_v2.env(), NUM_ENVS, num_cpus=num_cpus
+                simple_world_comm_v3.env(), NUM_ENVS, num_cpus=num_cpus
             )
         )
```

### Comparing `SuperSuit-3.7.2/test/test_vector/test_env_is_wrapped.py` & `SuperSuit-3.8.0/test/test_vector/test_env_is_wrapped.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import gymnasium
 import pytest
-from pettingzoo.mpe import simple_spread_v2
+from pettingzoo.mpe import simple_spread_v3
 
 from supersuit import concat_vec_envs_v1, pettingzoo_env_to_vec_env_v1
 from supersuit.generic_wrappers.frame_skip import frame_skip_gym
 
 
 def test_env_is_wrapped_true():
     env = gymnasium.make("MountainCarContinuous-v0")
@@ -29,12 +29,12 @@
     env = frame_skip_gym(env, 4)
     num_envs = 3
     venv1 = concat_vec_envs_v1(env, num_envs, num_cpus=2)
     assert venv1.env_is_wrapped(frame_skip_gym) == [True] * 3
 
 
 def test_env_is_wrapped_pettingzoo():
-    env = simple_spread_v2.parallel_env()
+    env = simple_spread_v3.parallel_env()
     venv1 = pettingzoo_env_to_vec_env_v1(env)
     num_envs = 3
     venv1 = concat_vec_envs_v1(venv1, num_envs)
     assert venv1.env_is_wrapped(frame_skip_gym) == [False] * 9
```

### Comparing `SuperSuit-3.7.2/test/test_vector/test_gym_vector.py` & `SuperSuit-3.8.0/test/test_vector/test_gym_vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 
 import gymnasium
 import numpy as np
 import pytest
-from pettingzoo.mpe import simple_spread_v2
+from pettingzoo.mpe import simple_spread_v3
 
 from supersuit import concat_vec_envs_v1, gym_vec_env_v0, pettingzoo_env_to_vec_env_v1
 
 
 def recursive_equal(info1, info2):
     try:
         if info1 == info2:
@@ -92,15 +92,15 @@
     check_vec_env_equivalency(venv1, venv2)
 
 
 @pytest.mark.skip(
     reason="Wrapper depreciated, see https://github.com/Farama-Foundation/SuperSuit/issues/188"
 )
 def test_multiagent_mutliproc_single_proc_equivalency():
-    env = simple_spread_v2.parallel_env(max_cycles=10)
+    env = simple_spread_v3.parallel_env(max_cycles=10)
     env = pettingzoo_env_to_vec_env_v1(env)
     num_envs = 3
     # uses single threaded vector environment
     venv1 = concat_vec_envs_v1(env, num_envs, num_cpus=0)
     # uses multiprocessing vector environment
     venv2 = concat_vec_envs_v1(env, num_envs, num_cpus=4)
     check_vec_env_equivalency(venv1, venv2)
```

### Comparing `SuperSuit-3.7.2/test/test_vector/test_pettingzoo_to_vec.py` & `SuperSuit-3.8.0/test/test_vector/test_pettingzoo_to_vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import copy
 
 import pytest
 from pettingzoo.butterfly import knights_archers_zombies_v10
-from pettingzoo.mpe import simple_spread_v2, simple_world_comm_v2
+from pettingzoo.mpe import simple_spread_v3, simple_world_comm_v3
 
 from supersuit import black_death_v3, concat_vec_envs_v1, pettingzoo_env_to_vec_env_v1
 
 
 def test_good_env():
-    env = simple_spread_v2.parallel_env()
+    env = simple_spread_v3.parallel_env()
     max_num_agents = len(env.possible_agents)
     env = pettingzoo_env_to_vec_env_v1(env)
     assert env.num_envs == max_num_agents
 
-    obss = env.reset()
+    obss, infos = env.reset()
     for i in range(55):
         actions = [env.action_space.sample() for i in range(env.num_envs)]
 
         # Check we're not passing a thing that gets mutated
         keep_obs = copy.deepcopy(obss)
         new_obss, rews, terms, truncs, infos = env.step(actions)
 
@@ -33,20 +33,20 @@
         if any(truncs):
             assert all(truncs)
         obss = new_obss
 
 
 def test_good_vecenv():
     num_envs = 2
-    env = simple_spread_v2.parallel_env()
+    env = simple_spread_v3.parallel_env()
     max_num_agents = len(env.possible_agents) * num_envs
     env = pettingzoo_env_to_vec_env_v1(env)
     env = concat_vec_envs_v1(env, num_envs)
 
-    obss = env.reset()
+    obss, infos = env.reset()
     for i in range(55):
         actions = [env.action_space.sample() for i in range(env.num_envs)]
 
         # Check we're not passing a thing that gets mutated
         keep_obs = copy.deepcopy(obss)
         new_obss, rews, terms, truncs, infos = env.step(actions)
 
@@ -61,15 +61,15 @@
             assert all(terms)
         if any(truncs):
             assert all(truncs)
         obss = new_obss
 
 
 def test_bad_action_spaces_env():
-    env = simple_world_comm_v2.parallel_env()
+    env = simple_world_comm_v3.parallel_env()
     with pytest.raises(AssertionError):
         env = pettingzoo_env_to_vec_env_v1(env)
 
 
 def test_env_black_death_assertion():
     env = knights_archers_zombies_v10.parallel_env(spawn_rate=50, max_cycles=2000)
     env = pettingzoo_env_to_vec_env_v1(env)
```

### Comparing `SuperSuit-3.7.2/test/test_vector/test_render.py` & `SuperSuit-3.8.0/test/test_vector/test_render.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.7.2/test/test_vector/test_vector_dict.py` & `SuperSuit-3.8.0/test/test_vector/test_vector_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     return aec_to_parallel(test_env)
 
 
 def dict_vec_env_test(env):
     # tests that environment really is a vectorized
     # version of the environment returned by make_env
 
-    obss = env.reset()
+    obss, infos = env.reset()
     for i in range(55):
         actions = [env.action_space.sample() for i in range(env.num_envs)]
         actions = concatenate(
             env.action_space,
             actions,
             create_empty_array(env.action_space, env.num_envs),
         )
```

### Comparing `SuperSuit-3.7.2/test/vec_env_test.py` & `SuperSuit-3.8.0/test/vec_env_test.py`

 * *Files identical despite different names*

