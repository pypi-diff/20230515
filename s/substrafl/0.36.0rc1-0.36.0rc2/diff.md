# Comparing `tmp/substrafl-0.36.0rc1.tar.gz` & `tmp/substrafl-0.36.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrafl-0.36.0rc1.tar", last modified: Thu May 11 14:30:53 2023, max compression
+gzip compressed data, was "substrafl-0.36.0rc2.tar", last modified: Thu May 11 15:07:46 2023, max compression
```

## Comparing `substrafl-0.36.0rc1.tar` & `substrafl-0.36.0rc2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.552012 substrafl-0.36.0rc1/substrafl/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.552012 substrafl-0.36.0rc1/substrafl/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23421 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/weight_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/evaluation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/index_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/index_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/index_generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/index_generator/np_index_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/model_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/aggregation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/nodes/references/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/references/local_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/references/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/test_data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/train_data_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/remote/register/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/register/generate_wheel.py
--rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/register/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/remote_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/remote/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/serializers/pickle_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/serializers/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/substratools_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/fed_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/fed_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/newton_raphson.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/single_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.552012 substrafl-0.36.0rc1/substrafl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.109447 substrafl-0.36.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 15:07:46.109447 substrafl-0.36.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:07:46.109447 substrafl-0.36.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.097447 substrafl-0.36.0rc2/substrafl/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.101447 substrafl-0.36.0rc2/substrafl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.101447 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_base_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23421 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_scaffold_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_single_organization_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/weight_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/evaluation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.101447 substrafl-0.36.0rc2/substrafl/index_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/index_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/index_generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/index_generator/np_index_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/model_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/aggregation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/nodes/references/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/references/local_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/references/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/test_data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/train_data_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/remote/register/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/register/generate_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/register/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/remote_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/remote/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/serializers/pickle_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/serializers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/substratools_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.109447 substrafl-0.36.0rc2/substrafl/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/fed_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/fed_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/newton_raphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/single_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.101447 substrafl-0.36.0rc2/substrafl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 15:07:45.000000 substrafl-0.36.0rc2/substrafl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-11 15:07:46.000000 substrafl-0.36.0rc2/substrafl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:07:45.000000 substrafl-0.36.0rc2/substrafl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-11 15:07:45.000000 substrafl-0.36.0rc2/substrafl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 15:07:45.000000 substrafl-0.36.0rc2/substrafl.egg-info/top_level.txt
```

### Comparing `substrafl-0.36.0rc1/LICENSE` & `substrafl-0.36.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/PKG-INFO` & `substrafl-0.36.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.36.0rc1
+Version: 0.36.0rc2
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.36.0rc1/README.md` & `substrafl-0.36.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/pyproject.toml` & `substrafl-0.36.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/setup.py` & `substrafl-0.36.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     packages=find_packages(exclude=["tests*", "benchmark*"]),
     # Not compatible with substratools 0.8.0 because
     # that release is private and in the Docker container
     # it has access only to the public PyPi
     install_requires=[
         "numpy>=1.20.3,!=1.24.*",
         "cloudpickle>=1.6.0",
-        "substra~=0.44.0",
+        "substra~=0.44.0rc1",
         "substratools~=0.20.0",
         "pydantic>=1.9.0",
         "pip>=21.2",
         "wheel",
         "six",
         "packaging",
     ],
```

### Comparing `substrafl-0.36.0rc1/substrafl/__init__.py` & `substrafl-0.36.0rc2/substrafl/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/algo.py` & `substrafl-0.36.0rc2/substrafl/algorithms/algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/__init__.py` & `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py` & `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_base_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py` & `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_fed_avg_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py` & `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_fed_pca_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py` & `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py` & `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_scaffold_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py` & `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_single_organization_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/weight_manager.py` & `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/weight_manager.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/dependency.py` & `substrafl-0.36.0rc2/substrafl/dependency.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/evaluation_strategy.py` & `substrafl-0.36.0rc2/substrafl/evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/exceptions.py` & `substrafl-0.36.0rc2/substrafl/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/experiment.py` & `substrafl-0.36.0rc2/substrafl/experiment.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/index_generator/base.py` & `substrafl-0.36.0rc2/substrafl/index_generator/base.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/index_generator/np_index_generator.py` & `substrafl-0.36.0rc2/substrafl/index_generator/np_index_generator.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/logger.py` & `substrafl-0.36.0rc2/substrafl/logger.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/model_loading.py` & `substrafl-0.36.0rc2/substrafl/model_loading.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/nodes/__init__.py` & `substrafl-0.36.0rc2/substrafl/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/nodes/aggregation_node.py` & `substrafl-0.36.0rc2/substrafl/nodes/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/nodes/node.py` & `substrafl-0.36.0rc2/substrafl/nodes/node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/nodes/test_data_node.py` & `substrafl-0.36.0rc2/substrafl/nodes/test_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/nodes/train_data_node.py` & `substrafl-0.36.0rc2/substrafl/nodes/train_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/remote/decorators.py` & `substrafl-0.36.0rc2/substrafl/remote/decorators.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/remote/operations.py` & `substrafl-0.36.0rc2/substrafl/remote/operations.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/remote/register/generate_wheel.py` & `substrafl-0.36.0rc2/substrafl/remote/register/generate_wheel.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/remote/register/register.py` & `substrafl-0.36.0rc2/substrafl/remote/register/register.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/remote/remote_struct.py` & `substrafl-0.36.0rc2/substrafl/remote/remote_struct.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/remote/serializers/pickle_serializer.py` & `substrafl-0.36.0rc2/substrafl/remote/serializers/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/remote/substratools_methods.py` & `substrafl-0.36.0rc2/substrafl/remote/substratools_methods.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/schemas.py` & `substrafl-0.36.0rc2/substrafl/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/strategies/fed_avg.py` & `substrafl-0.36.0rc2/substrafl/strategies/fed_avg.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/strategies/fed_pca.py` & `substrafl-0.36.0rc2/substrafl/strategies/fed_pca.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/strategies/newton_raphson.py` & `substrafl-0.36.0rc2/substrafl/strategies/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/strategies/scaffold.py` & `substrafl-0.36.0rc2/substrafl/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/strategies/single_organization.py` & `substrafl-0.36.0rc2/substrafl/strategies/single_organization.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl/strategies/strategy.py` & `substrafl-0.36.0rc2/substrafl/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc1/substrafl.egg-info/PKG-INFO` & `substrafl-0.36.0rc2/substrafl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.36.0rc1
+Version: 0.36.0rc2
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.36.0rc1/substrafl.egg-info/SOURCES.txt` & `substrafl-0.36.0rc2/substrafl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

