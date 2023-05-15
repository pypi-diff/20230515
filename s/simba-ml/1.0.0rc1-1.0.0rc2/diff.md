# Comparing `tmp/simba_ml-1.0.0rc1.tar.gz` & `tmp/simba_ml-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simba_ml-1.0.0rc1.tar", last modified: Fri Mar  3 17:26:32 2023, max compression
+gzip compressed data, was "simba_ml-1.0.0rc2.tar", last modified: Mon May 15 07:09:41 2023, max compression
```

## Comparing `simba_ml-1.0.0rc1.tar` & `simba_ml-1.0.0rc2.tar`

### file list

```diff
@@ -1,178 +1,176 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/
--rw-r--r--   0 max       (1000) max       (1000)       50 2023-02-10 13:34:20.000000 simba_ml-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)     5141 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     4553 2023-03-03 16:39:55.000000 simba_ml-1.0.0rc1/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.505150 simba_ml-1.0.0rc1/man/
--rw-r--r--   0 max       (1000) max       (1000)      681 2023-03-03 17:26:32.000000 simba_ml-1.0.0rc1/man/simba_ml.1
--rw-r--r--   0 max       (1000) max       (1000)      119 2023-02-10 13:34:20.000000 simba_ml-1.0.0rc1/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)     1464 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)     1505 2023-03-03 09:54:37.000000 simba_ml-1.0.0rc1/setup.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/
--rw-r--r--   0 max       (1000) max       (1000)      178 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      500 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/_version.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.505150 simba_ml-1.0.0rc1/simba_ml/cli/
--rw-r--r--   0 max       (1000) max       (1000)       23 2023-03-03 07:53:39.000000 simba_ml-1.0.0rc1/simba_ml/cli/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      488 2023-03-03 09:43:52.000000 simba_ml-1.0.0rc1/simba_ml/cli/__main__.py
--rw-r--r--   0 max       (1000) max       (1000)     1573 2023-03-03 15:22:57.000000 simba_ml-1.0.0rc1/simba_ml/cli/generate_data.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/cli/problem_viewer/
--rw-r--r--   0 max       (1000) max       (1000)       45 2023-03-03 11:00:00.000000 simba_ml-1.0.0rc1/simba_ml/cli/problem_viewer/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     2297 2023-03-03 07:53:39.000000 simba_ml-1.0.0rc1/simba_ml/cli/problem_viewer/problem_viewer.py
--rwxr-xr-x   0 max       (1000) max       (1000)      693 2023-03-03 11:00:00.000000 simba_ml-1.0.0rc1/simba_ml/cli/problem_viewer/run_problem_viewer.py
--rw-r--r--   0 max       (1000) max       (1000)     1595 2023-03-03 11:00:00.000000 simba_ml-1.0.0rc1/simba_ml/cli/start_prediction.py
--rw-r--r--   0 max       (1000) max       (1000)     4644 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/error_handler.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/example_problems/
--rw-r--r--   0 max       (1000) max       (1000)       71 2022-12-05 22:19:42.000000 simba_ml-1.0.0rc1/simba_ml/example_problems/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1013 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/example_problems/constant_function.py
--rw-r--r--   0 max       (1000) max       (1000)     1714 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/example_problems/salt_and_brine_tanks.py
--rw-r--r--   0 max       (1000) max       (1000)     2500 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/example_problems/sir.py
--rw-r--r--   0 max       (1000) max       (1000)     2395 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/example_problems/sird.py
--rw-r--r--   0 max       (1000) max       (1000)     1870 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/example_problems/trigonometry.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/
--rw-r--r--   0 max       (1000) max       (1000)       42 2023-02-14 12:44:58.000000 simba_ml-1.0.0rc1/simba_ml/prediction/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/logging/
--rw-r--r--   0 max       (1000) max       (1000)       36 2023-02-14 12:44:58.000000 simba_ml-1.0.0rc1/simba_ml/prediction/logging/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      176 2023-02-25 17:12:45.000000 simba_ml-1.0.0rc1/simba_ml/prediction/logging/logging_config.py
--rw-r--r--   0 max       (1000) max       (1000)     1659 2023-02-25 17:12:45.000000 simba_ml-1.0.0rc1/simba_ml/prediction/logging/wandb_logger.py
--rw-r--r--   0 max       (1000) max       (1000)     2307 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/normalizer.py
--rw-r--r--   0 max       (1000) max       (1000)      870 2023-02-14 12:44:58.000000 simba_ml-1.0.0rc1/simba_ml/prediction/plugin_loader.py
--rw-r--r--   0 max       (1000) max       (1000)     3069 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/prediction/preprocessing.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/
--rw-r--r--   0 max       (1000) max       (1000)       43 2023-02-20 10:54:12.000000 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/config/
--rw-r--r--   0 max       (1000) max       (1000)       63 2023-02-20 10:54:12.000000 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      408 2023-02-23 11:43:59.000000 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/config/steady_state_data_config.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/data_loader/
--rw-r--r--   0 max       (1000) max       (1000)       41 2023-02-20 10:54:12.000000 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/data_loader/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1611 2023-02-23 11:43:59.000000 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/data_loader/dataset_generator.py
--rw-r--r--   0 max       (1000) max       (1000)     4857 2023-02-23 11:43:59.000000 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py
--rw-r--r--   0 max       (1000) max       (1000)     1902 2023-02-22 18:30:18.000000 simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/data_loader/splits.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/
--rw-r--r--   0 max       (1000) max       (1000)       44 2023-02-14 12:44:58.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/
--rw-r--r--   0 max       (1000) max       (1000)      397 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/mixed_data_pipeline/
--rw-r--r--   0 max       (1000) max       (1000)      400 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/mixed_data_pipeline/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      552 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/mixed_data_pipeline/mixed_data_config.py
--rw-r--r--   0 max       (1000) max       (1000)     1096 2023-02-25 17:12:45.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/synthetic_data_pipeline/
--rw-r--r--   0 max       (1000) max       (1000)      413 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/synthetic_data_pipeline/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1117 2023-02-25 17:12:45.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py
--rw-r--r--   0 max       (1000) max       (1000)      493 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/synthetic_data_pipeline/synthetic_data_config.py
--rw-r--r--   0 max       (1000) max       (1000)      242 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/time_series_config.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/transfer_learning_pipeline/
--rw-r--r--   0 max       (1000) max       (1000)      445 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/transfer_learning_pipeline/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      466 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/transfer_learning_pipeline/transfer_learning_data_config.py
--rw-r--r--   0 max       (1000) max       (1000)     1136 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/transfer_learning_pipeline/transfer_learning_pipeline_config.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/
--rw-r--r--   0 max       (1000) max       (1000)       66 2023-02-14 12:44:58.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4209 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py
--rw-r--r--   0 max       (1000) max       (1000)     2663 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/splits.py
--rw-r--r--   0 max       (1000) max       (1000)     3370 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py
--rw-r--r--   0 max       (1000) max       (1000)     4268 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py
--rw-r--r--   0 max       (1000) max       (1000)     2129 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/window_generator.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/metrics/
--rw-r--r--   0 max       (1000) max       (1000)       31 2023-02-14 12:44:58.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/metrics/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1573 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/metrics/factory.py
--rw-r--r--   0 max       (1000) max       (1000)     9267 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/metrics/metrics.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/
--rw-r--r--   0 max       (1000) max       (1000)      403 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3090 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/average_predictor.py
--rw-r--r--   0 max       (1000) max       (1000)     3136 2023-02-25 15:51:06.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/factory.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/keras/
--rw-r--r--   0 max       (1000) max       (1000)      916 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/keras/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1689 2023-02-25 17:12:45.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/keras/dense_neural_network.py
--rw-r--r--   0 max       (1000) max       (1000)     4919 2023-02-28 10:55:45.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/keras/keras_model.py
--rw-r--r--   0 max       (1000) max       (1000)     2426 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/last_value_predictor.py
--rw-r--r--   0 max       (1000) max       (1000)     2656 2023-02-25 15:40:47.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/model.py
--rw-r--r--   0 max       (1000) max       (1000)     1999 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/pytorch_lightning/
--rw-r--r--   0 max       (1000) max       (1000)      472 2023-02-26 19:32:11.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3120 2023-02-25 15:40:47.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py
--rw-r--r--   0 max       (1000) max       (1000)     5164 2023-02-25 15:40:47.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/
--rw-r--r--   0 max       (1000) max       (1000)      923 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     2811 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py
--rw-r--r--   0 max       (1000) max       (1000)     1904 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py
--rw-r--r--   0 max       (1000) max       (1000)     2160 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py
--rw-r--r--   0 max       (1000) max       (1000)     3228 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py
--rw-r--r--   0 max       (1000) max       (1000)     3480 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py
--rw-r--r--   0 max       (1000) max       (1000)     1978 2023-02-25 10:48:51.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py
--rw-r--r--   0 max       (1000) max       (1000)     2490 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/transfer_learning_factory.py
--rw-r--r--   0 max       (1000) max       (1000)     2756 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/transfer_learning_model.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/pipelines/
--rw-r--r--   0 max       (1000) max       (1000)       31 2023-02-14 12:44:58.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/pipelines/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3931 2023-02-25 17:12:45.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py
--rw-r--r--   0 max       (1000) max       (1000)     3795 2023-03-03 07:53:39.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py
--rw-r--r--   0 max       (1000) max       (1000)     3937 2023-02-26 19:32:14.000000 simba_ml-1.0.0rc1/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/simulation/
--rw-r--r--   0 max       (1000) max       (1000)       61 2022-12-05 22:19:42.000000 simba_ml-1.0.0rc1/simba_ml/simulation/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.508484 simba_ml-1.0.0rc1/simba_ml/simulation/constraints/
--rw-r--r--   0 max       (1000) max       (1000)      537 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/constraints/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3265 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/constraints/constraint.py
--rw-r--r--   0 max       (1000) max       (1000)     2106 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/constraints/keep_species_sum.py
--rw-r--r--   0 max       (1000) max       (1000)     2465 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/constraints/species_value_in_range.py
--rw-r--r--   0 max       (1000) max       (1000)     2157 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/constraints/species_value_truncator.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/
--rw-r--r--   0 max       (1000) max       (1000)      961 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1562 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)      789 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/derivative_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)     1419 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)     1635 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)      699 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)     1315 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/
--rw-r--r--   0 max       (1000) max       (1000)     1120 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1953 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/beta_distribution.py
--rw-r--r--   0 max       (1000) max       (1000)     1072 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/constant.py
--rw-r--r--   0 max       (1000) max       (1000)     2049 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/continuous_uniform_distribution.py
--rw-r--r--   0 max       (1000) max       (1000)      950 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/distribution.py
--rw-r--r--   0 max       (1000) max       (1000)     1084 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/helper_functions.py
--rw-r--r--   0 max       (1000) max       (1000)     1921 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/lognormal_distribution.py
--rw-r--r--   0 max       (1000) max       (1000)     1918 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/normal_distribution.py
--rw-r--r--   0 max       (1000) max       (1000)     1621 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/distributions/vector_distribution.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/simulation/generators/
--rw-r--r--   0 max       (1000) max       (1000)      675 2023-03-03 07:53:39.000000 simba_ml-1.0.0rc1/simba_ml/simulation/generators/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      789 2023-03-03 07:53:39.000000 simba_ml-1.0.0rc1/simba_ml/simulation/generators/generator_interface.py
--rw-r--r--   0 max       (1000) max       (1000)     7886 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/generators/pertubation_generator.py
--rw-r--r--   0 max       (1000) max       (1000)     5138 2023-03-03 11:00:00.000000 simba_ml-1.0.0rc1/simba_ml/simulation/generators/steady_state_generator.py
--rw-r--r--   0 max       (1000) max       (1000)     1915 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/generators/time_points_generator.py
--rw-r--r--   0 max       (1000) max       (1000)     2768 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/generators/time_series_generator.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/
--rw-r--r--   0 max       (1000) max       (1000)      684 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     2804 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py
--rw-r--r--   0 max       (1000) max       (1000)     1837 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py
--rw-r--r--   0 max       (1000) max       (1000)     1482 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py
--rw-r--r--   0 max       (1000) max       (1000)      759 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/
--rw-r--r--   0 max       (1000) max       (1000)      917 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1066 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/additive_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)     2392 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/adjusting_mean_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)     2056 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/column_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)     2773 2023-02-23 11:43:59.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/elastic_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)      930 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/multi_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)     1082 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/multiplicative_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)      469 2022-12-15 19:50:19.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/no_noiser.py
--rw-r--r--   0 max       (1000) max       (1000)      358 2023-01-31 10:05:48.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/noiser.py
--rw-r--r--   0 max       (1000) max       (1000)      852 2023-01-31 10:05:48.000000 simba_ml-1.0.0rc1/simba_ml/simulation/noisers/sequential_noiser.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/
--rw-r--r--   0 max       (1000) max       (1000)      945 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4029 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/constant_suffix_remover.py
--rw-r--r--   0 max       (1000) max       (1000)     4470 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/interval_sparsifier.py
--rw-r--r--   0 max       (1000) max       (1000)     4029 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py
--rw-r--r--   0 max       (1000) max       (1000)      553 2023-01-31 10:05:48.000000 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/no_sparsifier.py
--rw-r--r--   0 max       (1000) max       (1000)     1302 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/random_sample_sparsifier.py
--rw-r--r--   0 max       (1000) max       (1000)      903 2023-01-31 10:05:48.000000 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/sequential_sparsifier.py
--rw-r--r--   0 max       (1000) max       (1000)      455 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/sparsifier.py
--rw-r--r--   0 max       (1000) max       (1000)     2563 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/species.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.511817 simba_ml-1.0.0rc1/simba_ml/simulation/system_model/
--rw-r--r--   0 max       (1000) max       (1000)      207 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/system_model/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    11740 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/system_model/system_model.py
--rw-r--r--   0 max       (1000) max       (1000)     1956 2023-02-17 15:15:40.000000 simba_ml-1.0.0rc1/simba_ml/simulation/system_model/system_model_interface.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-03-03 17:26:32.505150 simba_ml-1.0.0rc1/simba_ml.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     5141 2023-03-03 17:26:32.000000 simba_ml-1.0.0rc1/simba_ml.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     7559 2023-03-03 17:26:32.000000 simba_ml-1.0.0rc1/simba_ml.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2023-03-03 17:26:32.000000 simba_ml-1.0.0rc1/simba_ml.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       56 2023-03-03 17:26:32.000000 simba_ml-1.0.0rc1/simba_ml.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       72 2023-03-03 17:26:32.000000 simba_ml-1.0.0rc1/simba_ml.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        9 2023-03-03 17:26:32.000000 simba_ml-1.0.0rc1/simba_ml.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)    83607 2023-02-10 13:34:20.000000 simba_ml-1.0.0rc1/versioneer.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.730448 simba_ml-1.0.0rc2/
+-rw-r--r--   0 max       (1000) max       (1000)       50 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)     4962 2023-05-15 07:09:41.730448 simba_ml-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     4272 2023-05-14 12:38:51.000000 simba_ml-1.0.0rc2/README.md
+-rw-r--r--   0 max       (1000) max       (1000)      119 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)     1451 2023-05-15 07:09:41.730448 simba_ml-1.0.0rc2/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)     1498 2023-05-14 12:38:51.000000 simba_ml-1.0.0rc2/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.730448 simba_ml-1.0.0rc2/simba_ml/
+-rw-r--r--   0 max       (1000) max       (1000)      178 2023-05-15 06:45:57.000000 simba_ml-1.0.0rc2/simba_ml/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      500 2023-05-15 07:09:41.730448 simba_ml-1.0.0rc2/simba_ml/_version.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/cli/
+-rw-r--r--   0 max       (1000) max       (1000)       23 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/cli/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      488 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/cli/__main__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1573 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/cli/generate_data.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/cli/problem_viewer/
+-rw-r--r--   0 max       (1000) max       (1000)       45 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/cli/problem_viewer/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2297 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/cli/problem_viewer/problem_viewer.py
+-rwxr-xr-x   0 max       (1000) max       (1000)      693 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/cli/problem_viewer/run_problem_viewer.py
+-rw-r--r--   0 max       (1000) max       (1000)     1650 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/cli/start_prediction.py
+-rw-r--r--   0 max       (1000) max       (1000)     4644 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/error_handler.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/example_problems/
+-rw-r--r--   0 max       (1000) max       (1000)       71 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/example_problems/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1013 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/example_problems/constant_function.py
+-rw-r--r--   0 max       (1000) max       (1000)     1714 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/example_problems/salt_and_brine_tanks.py
+-rw-r--r--   0 max       (1000) max       (1000)     2500 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/example_problems/sir.py
+-rw-r--r--   0 max       (1000) max       (1000)     2395 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/example_problems/sird.py
+-rw-r--r--   0 max       (1000) max       (1000)     1870 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/example_problems/trigonometry.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/
+-rw-r--r--   0 max       (1000) max       (1000)       42 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/logging/
+-rw-r--r--   0 max       (1000) max       (1000)       36 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/logging/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      176 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/logging/logging_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     1659 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/logging/wandb_logger.py
+-rw-r--r--   0 max       (1000) max       (1000)     3246 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/normalizer.py
+-rw-r--r--   0 max       (1000) max       (1000)      924 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/plugin_loader.py
+-rw-r--r--   0 max       (1000) max       (1000)     3152 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/preprocessing.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/
+-rw-r--r--   0 max       (1000) max       (1000)       43 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/config/
+-rw-r--r--   0 max       (1000) max       (1000)       63 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      408 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/config/steady_state_data_config.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/data_loader/
+-rw-r--r--   0 max       (1000) max       (1000)       41 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/data_loader/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1611 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/data_loader/dataset_generator.py
+-rw-r--r--   0 max       (1000) max       (1000)     4857 2023-05-15 06:45:36.000000 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py
+-rw-r--r--   0 max       (1000) max       (1000)     1902 2023-05-15 06:45:36.000000 simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/data_loader/splits.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/
+-rw-r--r--   0 max       (1000) max       (1000)       44 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/
+-rw-r--r--   0 max       (1000) max       (1000)      387 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/mixed_data_pipeline/
+-rw-r--r--   0 max       (1000) max       (1000)      394 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/mixed_data_pipeline/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      588 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/mixed_data_pipeline/data_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     1103 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/synthetic_data_pipeline/
+-rw-r--r--   0 max       (1000) max       (1000)      402 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/synthetic_data_pipeline/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      485 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/synthetic_data_pipeline/data_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     1116 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py
+-rw-r--r--   0 max       (1000) max       (1000)      278 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/time_series_config.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/transfer_learning_pipeline/
+-rw-r--r--   0 max       (1000) max       (1000)      408 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/transfer_learning_pipeline/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      379 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/transfer_learning_pipeline/data_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     1119 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/
+-rw-r--r--   0 max       (1000) max       (1000)       66 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3965 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py
+-rw-r--r--   0 max       (1000) max       (1000)     2646 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/splits.py
+-rw-r--r--   0 max       (1000) max       (1000)     3041 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py
+-rw-r--r--   0 max       (1000) max       (1000)     3969 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py
+-rw-r--r--   0 max       (1000) max       (1000)     3125 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/window_generator.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/metrics/
+-rw-r--r--   0 max       (1000) max       (1000)       31 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/metrics/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1825 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/metrics/factory.py
+-rw-r--r--   0 max       (1000) max       (1000)    14058 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/metrics/metrics.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/
+-rw-r--r--   0 max       (1000) max       (1000)      403 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3335 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/average_predictor.py
+-rw-r--r--   0 max       (1000) max       (1000)     3136 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/factory.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/keras/
+-rw-r--r--   0 max       (1000) max       (1000)      915 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/keras/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1698 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/keras/dense_neural_network.py
+-rw-r--r--   0 max       (1000) max       (1000)     5145 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/keras/keras_model.py
+-rw-r--r--   0 max       (1000) max       (1000)     2700 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/last_value_predictor.py
+-rw-r--r--   0 max       (1000) max       (1000)     2835 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/model.py
+-rw-r--r--   0 max       (1000) max       (1000)     1999 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/pytorch_lightning/
+-rw-r--r--   0 max       (1000) max       (1000)      932 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3146 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py
+-rw-r--r--   0 max       (1000) max       (1000)     5457 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/
+-rw-r--r--   0 max       (1000) max       (1000)      923 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2811 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py
+-rw-r--r--   0 max       (1000) max       (1000)     1904 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py
+-rw-r--r--   0 max       (1000) max       (1000)     2160 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py
+-rw-r--r--   0 max       (1000) max       (1000)     3228 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py
+-rw-r--r--   0 max       (1000) max       (1000)     3695 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py
+-rw-r--r--   0 max       (1000) max       (1000)     1978 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py
+-rw-r--r--   0 max       (1000) max       (1000)     2490 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/transfer_learning_factory.py
+-rw-r--r--   0 max       (1000) max       (1000)     2756 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/transfer_learning_model.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/pipelines/
+-rw-r--r--   0 max       (1000) max       (1000)       31 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/pipelines/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4133 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py
+-rw-r--r--   0 max       (1000) max       (1000)     3886 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py
+-rw-r--r--   0 max       (1000) max       (1000)     4044 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/simulation/
+-rw-r--r--   0 max       (1000) max       (1000)       61 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/simulation/constraints/
+-rw-r--r--   0 max       (1000) max       (1000)      537 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/constraints/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3265 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/constraints/constraint.py
+-rw-r--r--   0 max       (1000) max       (1000)     2106 2023-05-15 06:45:36.000000 simba_ml-1.0.0rc2/simba_ml/simulation/constraints/keep_species_sum.py
+-rw-r--r--   0 max       (1000) max       (1000)     2465 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/constraints/species_value_in_range.py
+-rw-r--r--   0 max       (1000) max       (1000)     2164 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/constraints/species_value_truncator.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/
+-rw-r--r--   0 max       (1000) max       (1000)      961 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1562 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)      789 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/derivative_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)     1419 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)     1635 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)      699 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)     1315 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/
+-rw-r--r--   0 max       (1000) max       (1000)     1120 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1953 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/beta_distribution.py
+-rw-r--r--   0 max       (1000) max       (1000)     1072 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/constant.py
+-rw-r--r--   0 max       (1000) max       (1000)     2049 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/continuous_uniform_distribution.py
+-rw-r--r--   0 max       (1000) max       (1000)      950 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/distribution.py
+-rw-r--r--   0 max       (1000) max       (1000)     1084 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/helper_functions.py
+-rw-r--r--   0 max       (1000) max       (1000)     1921 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/lognormal_distribution.py
+-rw-r--r--   0 max       (1000) max       (1000)     1918 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/normal_distribution.py
+-rw-r--r--   0 max       (1000) max       (1000)     1621 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/distributions/vector_distribution.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/simulation/generators/
+-rw-r--r--   0 max       (1000) max       (1000)      675 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/generators/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      789 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/generators/generator_interface.py
+-rw-r--r--   0 max       (1000) max       (1000)     7886 2023-05-15 06:41:40.000000 simba_ml-1.0.0rc2/simba_ml/simulation/generators/pertubation_generator.py
+-rw-r--r--   0 max       (1000) max       (1000)     5138 2023-05-15 06:41:40.000000 simba_ml-1.0.0rc2/simba_ml/simulation/generators/steady_state_generator.py
+-rw-r--r--   0 max       (1000) max       (1000)     1915 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/generators/time_points_generator.py
+-rw-r--r--   0 max       (1000) max       (1000)     2768 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/generators/time_series_generator.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/
+-rw-r--r--   0 max       (1000) max       (1000)      684 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2804 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py
+-rw-r--r--   0 max       (1000) max       (1000)     1837 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py
+-rw-r--r--   0 max       (1000) max       (1000)     1482 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py
+-rw-r--r--   0 max       (1000) max       (1000)      759 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.730448 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/
+-rw-r--r--   0 max       (1000) max       (1000)      917 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1066 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/additive_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)     2392 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/adjusting_mean_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)     2056 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/column_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)     2773 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/elastic_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)      930 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/multi_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)     1082 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/multiplicative_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)      469 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/no_noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)      358 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/noiser.py
+-rw-r--r--   0 max       (1000) max       (1000)      852 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/noisers/sequential_noiser.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.730448 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/
+-rw-r--r--   0 max       (1000) max       (1000)      945 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4029 2023-05-15 06:45:36.000000 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/constant_suffix_remover.py
+-rw-r--r--   0 max       (1000) max       (1000)     4470 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/interval_sparsifier.py
+-rw-r--r--   0 max       (1000) max       (1000)     4029 2023-05-15 06:45:36.000000 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py
+-rw-r--r--   0 max       (1000) max       (1000)      553 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/no_sparsifier.py
+-rw-r--r--   0 max       (1000) max       (1000)     1302 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/random_sample_sparsifier.py
+-rw-r--r--   0 max       (1000) max       (1000)      903 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/sequential_sparsifier.py
+-rw-r--r--   0 max       (1000) max       (1000)      455 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/sparsifier.py
+-rw-r--r--   0 max       (1000) max       (1000)     2563 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/species.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.730448 simba_ml-1.0.0rc2/simba_ml/simulation/system_model/
+-rw-r--r--   0 max       (1000) max       (1000)      207 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/system_model/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    11740 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/system_model/system_model.py
+-rw-r--r--   0 max       (1000) max       (1000)     1956 2023-05-10 14:24:11.000000 simba_ml-1.0.0rc2/simba_ml/simulation/system_model/system_model_interface.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-15 07:09:41.727115 simba_ml-1.0.0rc2/simba_ml.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     4962 2023-05-15 07:09:41.000000 simba_ml-1.0.0rc2/simba_ml.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     7492 2023-05-15 07:09:41.000000 simba_ml-1.0.0rc2/simba_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-05-15 07:09:41.000000 simba_ml-1.0.0rc2/simba_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       57 2023-05-15 07:09:41.000000 simba_ml-1.0.0rc2/simba_ml.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       72 2023-05-15 07:09:41.000000 simba_ml-1.0.0rc2/simba_ml.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        9 2023-05-15 07:09:41.000000 simba_ml-1.0.0rc2/simba_ml.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)    83607 2023-05-14 13:09:26.000000 simba_ml-1.0.0rc2/versioneer.py
```

### Comparing `simba_ml-1.0.0rc1/PKG-INFO` & `simba_ml-1.0.0rc2/simba_ml.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: simba_ml
-Version: 1.0.0rc1
+Name: simba-ml
+Version: 1.0.0rc2
 Summary: Simulation-Based Machine Learning
+Home-page: UNKNOWN
 Author: Maximilian Kleissl, Björn Heyder, Julian Zabbarov, Lukas Drews
 Author-email: maximilian.kleissl@student.hpi.de,bjoern.heyder@student.hpi.de,julian.zabbarov@student.hpi.de,lukas.drews@student.hpi.de
-Project-URL: Bug Tracker, https://gitlab.hpi.de/mpws2022br1/simba_ml/issues
-Project-URL: Source Code, https://gitlab.hpi.de/mpws2022br1/simba_ml/
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/DILiS-lab/SimbaML/issues
+Project-URL: Source Code, https://github.com/DILiS-lab/SimbaML
+Project-URL: Documentation, https://simbaml.readthedocs.io
 Keywords: python,machine learning,simulation,ordinary differential equations,ode,simba,simba-ml
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-[![pipeline status](https://gitlab.hpi.de/mpws2022br1/simba_ml/badges/main/pipeline.svg)](https://gitlab.hpi.de/mpws2022br1/simba_ml/-/commits/main)
-[![coverage report](https://gitlab.hpi.de/mpws2022br1/simba_ml/badges/main/coverage.svg)](https://gitlab.hpi.de/mpws2022br1/simba_ml/-/commits/main)
-
 # SimbaML
 
 ![Overview of the SimbaML framework](docs/source/_static/visualabstract.png)
 
 SimbaML is an all-in-one framework for integrating prior knowledge of ODE models into the ML process by synthetic data augmentation. It allows for the convenient generation of realistic synthetic data by sparsifying and adding noise. Furthermore, our framework provides customizable pipelines for various ML experiments, such as identifying needs for data collection and transfer learning.
 
 # Installation
@@ -165,8 +166,10 @@
 ```
 from simba_ml.prediction.time_series.pipelines import synthetic_data_pipeline
 result_df = synthetic_data_pipeline.main("ml_config.toml")
 ```
 
 # Documentation
 
-Comming soon!
+https://simbaml.readthedocs.io/
+
+
```

### Comparing `simba_ml-1.0.0rc1/README.md` & `simba_ml-1.0.0rc2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-[![pipeline status](https://gitlab.hpi.de/mpws2022br1/simba_ml/badges/main/pipeline.svg)](https://gitlab.hpi.de/mpws2022br1/simba_ml/-/commits/main)
-[![coverage report](https://gitlab.hpi.de/mpws2022br1/simba_ml/badges/main/coverage.svg)](https://gitlab.hpi.de/mpws2022br1/simba_ml/-/commits/main)
-
 # SimbaML
 
 ![Overview of the SimbaML framework](docs/source/_static/visualabstract.png)
 
 SimbaML is an all-in-one framework for integrating prior knowledge of ODE models into the ML process by synthetic data augmentation. It allows for the convenient generation of realistic synthetic data by sparsifying and adding noise. Furthermore, our framework provides customizable pipelines for various ML experiments, such as identifying needs for data collection and transfer learning.
 
 # Installation
@@ -154,8 +151,8 @@
 ```
 from simba_ml.prediction.time_series.pipelines import synthetic_data_pipeline
 result_df = synthetic_data_pipeline.main("ml_config.toml")
 ```
 
 # Documentation
 
-Comming soon!
+https://simbaml.readthedocs.io/
```

### Comparing `simba_ml-1.0.0rc1/setup.cfg` & `simba_ml-1.0.0rc2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 	"Operating System :: OS Independent",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.10",
 	"Topic :: Scientific/Engineering"]
 
 [project.urls]
-Bug Tracker = https://gitlab.hpi.de/mpws2022br1/simba_ml/issues
-Source Code = https://gitlab.hpi.de/mpws2022br1/simba_ml/
+Bug Tracker = https://github.com/DILiS-lab/SimbaML/issues
+Source Code = https://github.com/DILiS-lab/SimbaML
 
 [versioneer]
 VCS = git
 style = pep440
 versionfile_source = simba_ml/_version.py
 versionfile_build = simba_ml/_version.py
 tag_prefix = v
```

### Comparing `simba_ml-1.0.0rc1/setup.py` & `simba_ml-1.0.0rc2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 setup(
     name="simba_ml",
     version=VERSION,
     cmdclass=versioneer.get_cmdclass(),
     author="Maximilian Kleissl, Björn Heyder, Julian Zabbarov, Lukas Drews",
     author_email="maximilian.kleissl@student.hpi.de,bjoern.heyder@student.hpi.de,julian.zabbarov@student.hpi.de,lukas.drews@student.hpi.de",
     project_urls={
-        "Bug Tracker": "https://gitlab.hpi.de/mpws2022br1/simba_ml/issues",
-        "Source Code": "https://gitlab.hpi.de/mpws2022br1/simba_ml/",
+        "Bug Tracker": "https://github.com/DILiS-lab/SimbaML/issues",
+        "Source Code": "https://github.com/DILiS-lab/SimbaML",
+        "Documentation": "https://simbaml.readthedocs.io"
     },
     description=DESCRIPTION,
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "streamlit",
@@ -46,10 +47,9 @@
     ],
     classifiers=[],
     entry_points={
         "console_scripts": [
             "simba_ml = simba_ml.cli.__main__:main",
         ],
     },
-    license_files=("LICENSE.txt",),
-    data_files=[("man/man1", ["man/simba_ml.1"])],
+    license_files=("LICENSE.txt",)
 )
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/cli/generate_data.py` & `simba_ml-1.0.0rc2/simba_ml/cli/generate_data.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/cli/problem_viewer/problem_viewer.py` & `simba_ml-1.0.0rc2/simba_ml/cli/problem_viewer/problem_viewer.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/cli/problem_viewer/run_problem_viewer.py` & `simba_ml-1.0.0rc2/simba_ml/cli/problem_viewer/run_problem_viewer.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/cli/start_prediction.py` & `simba_ml-1.0.0rc2/simba_ml/cli/start_prediction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Module for starting a prediction pipeline."""
+import os
+import sys
+
 import typing
 import logging
 import datetime
 
 import pandas as pd
 import click
 
@@ -50,9 +53,10 @@
     """Start a prediction pipeline.
 
     Args:
         pipeline: name of the pipeline.
         output_path: path to the output file.
         config_path: path to the config file.
     """
+    sys.path.append(os.getcwd())
     results = PIPELINES[pipeline](config_path)
     results.to_csv(output_path)
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/error_handler.py` & `simba_ml-1.0.0rc2/simba_ml/error_handler.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/example_problems/constant_function.py` & `simba_ml-1.0.0rc2/simba_ml/example_problems/constant_function.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/example_problems/salt_and_brine_tanks.py` & `simba_ml-1.0.0rc2/simba_ml/example_problems/salt_and_brine_tanks.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/example_problems/sir.py` & `simba_ml-1.0.0rc2/simba_ml/example_problems/sir.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/example_problems/sird.py` & `simba_ml-1.0.0rc2/simba_ml/example_problems/sird.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/example_problems/trigonometry.py` & `simba_ml-1.0.0rc2/simba_ml/example_problems/trigonometry.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/logging/wandb_logger.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/logging/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/plugin_loader.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/plugin_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """A simple plugin loader."""
+import os
+import sys
 import importlib
 
 
 class PluginInterface:
     """Represents a plugin interface.
 
     A plugin has a single register function.
@@ -28,10 +30,11 @@
 
 def load_plugins(plugins: list[str]) -> None:
     """Loads the plugins defined in the plugins list.
 
     Args:
         plugins: A list of plugins (complete names) to load.
     """
+    sys.path.append(os.getcwd())
     for plugin_file in plugins:
         plugin = import_module(plugin_file)
         plugin.register()
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/preprocessing.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/preprocessing.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     Raises:
         ValueError: if the given directory is empty.
         ValueError: if the given directory contains no csvs.
 
     Returns:
         data: numpy array containing the data.
     """
+    path_to_csvs = path_to_csvs if path_to_csvs[-1] == "/" else f"{path_to_csvs}/"
     if len(os.listdir(path_to_csvs)) == 0:
         raise ValueError("The given directory is empty.")
     if data_list := [
         pd.read_csv(path_to_csvs + file, header=0)
         for file in os.listdir(path_to_csvs)
         if file.endswith(".csv")
     ]:
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/data_loader/dataset_generator.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/data_loader/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/steady_state/data_loader/splits.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/steady_state/data_loader/splits.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Provides the configuration for the pipeline."""
 import typing
 import dataclasses
 
 from simba_ml.prediction.time_series.config.mixed_data_pipeline import (
-    mixed_data_config,
+    data_config,
 )
 from simba_ml.prediction.logging import logging_config
 from simba_ml.prediction.time_series.metrics import factory as metrics_factory
 from simba_ml.prediction.time_series.metrics import metrics as metrics_module
 
 
 @dataclasses.dataclass
 class PipelineConfig:
     """Config for the Pipeline."""
 
     models: list[dict[str, object]]
     metrics: list[str]
-    data: mixed_data_config.DataConfig
+    data: data_config.DataConfig
     plugins: list[str] = dataclasses.field(default_factory=list)
     metric_functions: dict[str, metrics_module.Metric] = dataclasses.field(init=False)
     logging: typing.Optional[logging_config.LoggingConfig] = None
+    seed: int = 42
 
     def __post_init__(self) -> None:
         """Inits the PipelineConfig.
 
         Creates a dict mapping the given metric_ids to their respective functions.
         """
         self.metric_functions = {
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Provides the configuration for the pipeline."""
 import typing
 import dataclasses
 
 from simba_ml.prediction.time_series.config.synthetic_data_pipeline import (
-    synthetic_data_config,
+    data_config,
 )
 from simba_ml.prediction.logging import (
     logging_config,
 )
 from simba_ml.prediction.time_series.metrics import factory as metrics_factory
 from simba_ml.prediction.time_series.metrics import metrics as metrics_module
 
 
 @dataclasses.dataclass
 class PipelineConfig:
     """Config for the Pipeline."""
 
     models: list[dict[str, object]]
     metrics: list[str]
-    data: synthetic_data_config.DataConfig
+    data: data_config.DataConfig
     plugins: list[str] = dataclasses.field(default_factory=list)
     metric_functions: dict[str, metrics_module.Metric] = dataclasses.field(init=False)
     logging: typing.Optional[logging_config.LoggingConfig] = None
+    seed: int = 42
 
     def __post_init__(self) -> None:
         """Inits the PipelineConfig.
 
         Creates a dict mapping the given metric_ids to their respective functions.
         """
         self.metric_functions = {
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/config/transfer_learning_pipeline/transfer_learning_pipeline_config.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Provides the configuration for the pipeline."""
 import dataclasses
 import typing
 
 from simba_ml.prediction.time_series.config.transfer_learning_pipeline import (
-    transfer_learning_data_config,
+    data_config,
 )
 from simba_ml.prediction.logging import (
     logging_config,
 )
 from simba_ml.prediction.time_series.metrics import factory as metrics_factory
 from simba_ml.prediction.time_series.metrics import metrics as metrics_module
 
 
 @dataclasses.dataclass
 class PipelineConfig:
     """Config for the Pipeline."""
 
     models: list[dict[str, object]]
     metrics: list[str]
-    data: transfer_learning_data_config.DataConfig
+    data: data_config.DataConfig
     logging: typing.Optional[logging_config.LoggingConfig] = None
     plugins: list[str] = dataclasses.field(default_factory=list)
     metric_functions: dict[str, metrics_module.Metric] = dataclasses.field(init=False)
+    seed: int = 42
 
     def __post_init__(self) -> None:
         """Inits the PipelineConfig.
 
         Creates a dict mapping the given metric_ids to their respective functions.
         """
         self.metric_functions = {
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 import os
 from typing import Optional, Tuple
 
 import pandas as pd
 import numpy as np
 from numpy import typing as npt
 
-from simba_ml.prediction.time_series.config.mixed_data_pipeline import (
-    mixed_data_config,
+from simba_ml.prediction.time_series.config.transfer_learning_pipeline import (
+    data_config,
 )
 from simba_ml.prediction import preprocessing
 from simba_ml.prediction.time_series.data_loader import window_generator, splits
 
 
-class MixedDataLoader:
+class TransferLearningDataLoader:
     """Loads and preprocesses the data.
 
     Attributes:
         X_test: the input of the test data
         y_test: the labels for the test data
         train_validation_sets: list of validations sets, one for each ratio of
             synthethic to observed data
     """
 
-    config: mixed_data_config.DataConfig
+    config: data_config.DataConfig
     __X_test: Optional[npt.NDArray[np.float64]] = None
     __y_test: Optional[npt.NDArray[np.float64]] = None
-    __train_sets: Optional[dict[float, list[npt.NDArray[np.float64]]]] = None
+    __train_observed: Optional[list[npt.NDArray[np.float64]]] = None
+    __train_synthetic: Optional[list[npt.NDArray[np.float64]]] = None
 
-    def __init__(self, config: mixed_data_config.DataConfig) -> None:
+    def __init__(self, config: data_config.DataConfig) -> None:
         """Inits the DataLoader.
 
         Args:
             config: the data configuration.
         """
         self.config = config
 
@@ -58,46 +59,25 @@
         )
         return synthetic, observed
 
     def prepare_data(self) -> None:
         """This function preprocesses the data."""
         if self.__X_test is not None:  # pragma: no cover
             return  # pragma: no cover
-
-        self.__train_sets = {}
         synthethic_data, observed_data = self.load_data()
-
-        synthetic_train, _ = splits.train_test_split(
-            data=synthethic_data,
-            test_split=self.config.test_split,
-            input_length=self.config.time_series.input_length,
-            split_axis=self.config.split_axis,
-        )
         observed_train, observed_test = splits.train_test_split(
             data=observed_data,
             test_split=self.config.test_split,
             input_length=self.config.time_series.input_length,
             split_axis=self.config.split_axis,
         )
-
-        for ratio in self.config.ratios:
-            train = preprocessing.convert_dataframe_to_numpy(
-                preprocessing.mix_data(
-                    synthetic_data=synthetic_train,
-                    observed_data=observed_train,
-                    ratio=ratio,
-                )
-            )
-            self.__train_sets[ratio] = train
-
-        test = preprocessing.convert_dataframe_to_numpy(observed_test)
+        self.__train_synthetic = synthethic_data
+        self.__train_observed = observed_train
         self.__X_test, self.__y_test = window_generator.create_window_dataset(
-            test,
-            self.config.time_series.input_length,
-            self.config.time_series.output_length,
+            observed_test, self.config.time_series
         )
 
     # sourcery skip: snake-case-functions
     @property
     def X_test(self) -> npt.NDArray[np.float64]:
         """The input of the test dataset.
 
@@ -118,21 +98,37 @@
         """
         if self.__y_test is None:
             self.prepare_data()
             return self.y_test
         return self.__y_test
 
     @property
-    def train_sets(
+    def train_observed(
+        self,
+    ) -> list[npt.NDArray[np.float64]]:
+        """Lists of train sets.
+
+        One set for each ratio.
+
+        Returns:
+            A dict containing the train sets.
+        """
+        if not self.__train_observed:
+            self.prepare_data()
+            return self.train_observed
+        return self.__train_observed
+
+    @property
+    def train_synthetic(
         self,
-    ) -> dict[float, list[npt.NDArray[np.float64]]]:
+    ) -> list[npt.NDArray[np.float64]]:
         """Lists of train sets.
 
         One set for each ratio.
 
         Returns:
             A dict containing the train sets.
         """
-        if not self.__train_sets:
+        if not self.__train_synthetic:
             self.prepare_data()
-            return self.train_sets
-        return self.__train_sets
+            return self.train_synthetic
+        return self.__train_synthetic
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/splits.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/splits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Module containing splitting functionalities."""
 import random
 
 import pandas as pd
 
-random.seed(42)
-
 
 def train_test_split_vertical(
     data: list[pd.DataFrame], test_split: float, input_length: float
 ) -> tuple[list[pd.DataFrame], list[pd.DataFrame]]:
     """Splits a given dataframe in train, test and validations split.
 
     Args:
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 import pandas as pd
 import numpy as np
 from numpy import typing as npt
 
 from simba_ml.prediction.time_series.config.synthetic_data_pipeline import (
-    synthetic_data_config,
+    data_config,
 )
 from simba_ml.prediction import preprocessing
 from simba_ml.prediction.time_series.data_loader import window_generator, splits
 
 
 class SyntheticDataLoader:
     """Loads and preprocesses the data.
@@ -19,39 +19,35 @@
     Attributes:
         X_test: the input of the test data
         y_test: the labels for the test data
         train_validation_sets: list of validations sets, one for each ratio of
             synthethic to observed data
     """
 
-    config: synthetic_data_config.DataConfig
+    config: data_config.DataConfig
     __X_test: Optional[npt.NDArray[np.float64]] = None
     __y_test: Optional[npt.NDArray[np.float64]] = None
     __train: Optional[list[npt.NDArray[np.float64]]] = None
 
-    def __init__(self, config: synthetic_data_config.DataConfig) -> None:
+    def __init__(self, config: data_config.DataConfig) -> None:
         """Inits the DataLoader.
 
         Args:
             config: the data configuration.
         """
         self.config = config
 
     def load_data(self) -> list[pd.DataFrame]:
         """Loads the data.
 
         Returns:
             A list of dataframes.
         """
-        return (
-            []
-            if self.config.synthetic is None
-            else preprocessing.read_dataframes_from_csvs(
-                os.getcwd() + self.config.synthetic
-            )
+        return preprocessing.read_dataframes_from_csvs(
+            os.getcwd() + self.config.synthetic
         )
 
     def prepare_data(self) -> None:
         """This function preprocesses the data."""
         if self.__X_test is not None:  # pragma: no cover
             return  # pragma: no cover
 
@@ -61,21 +57,17 @@
         synthetic_train, synthetic_test = splits.train_test_split(
             data=synthetic_data,
             test_split=self.config.test_split,
             input_length=self.config.time_series.input_length,
             split_axis=self.config.split_axis,
         )
 
-        self.__train = preprocessing.convert_dataframe_to_numpy(synthetic_train)
-
-        synthetic_test = preprocessing.convert_dataframe_to_numpy(synthetic_test)
+        self.__train = synthetic_train
         self.__X_test, self.__y_test = window_generator.create_window_dataset(
-            synthetic_test,
-            self.config.time_series.input_length,
-            self.config.time_series.output_length,
+            synthetic_test, self.config.time_series
         )
 
     # sourcery skip: snake-case-functions
     @property
     def X_test(self) -> npt.NDArray[np.float64]:
         """The input of the test dataset.
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 import os
 from typing import Optional, Tuple
 
 import pandas as pd
 import numpy as np
 from numpy import typing as npt
 
-from simba_ml.prediction.time_series.config.transfer_learning_pipeline import (
-    transfer_learning_data_config,
+from simba_ml.prediction.time_series.config.mixed_data_pipeline import (
+    data_config,
 )
 from simba_ml.prediction import preprocessing
 from simba_ml.prediction.time_series.data_loader import window_generator, splits
 
 
-class TransferLearningDataLoader:
+class MixedDataLoader:
     """Loads and preprocesses the data.
 
     Attributes:
         X_test: the input of the test data
         y_test: the labels for the test data
         train_validation_sets: list of validations sets, one for each ratio of
             synthethic to observed data
     """
 
-    config: transfer_learning_data_config.DataConfig
+    config: data_config.DataConfig
     __X_test: Optional[npt.NDArray[np.float64]] = None
     __y_test: Optional[npt.NDArray[np.float64]] = None
-    __train_observed: Optional[list[npt.NDArray[np.float64]]] = None
-    __train_synthetic: Optional[list[npt.NDArray[np.float64]]] = None
+    __train_sets: Optional[dict[float, list[npt.NDArray[np.float64]]]] = None
 
-    def __init__(self, config: transfer_learning_data_config.DataConfig) -> None:
+    def __init__(self, config: data_config.DataConfig) -> None:
         """Inits the DataLoader.
 
         Args:
             config: the data configuration.
         """
         self.config = config
 
@@ -59,30 +58,42 @@
         )
         return synthetic, observed
 
     def prepare_data(self) -> None:
         """This function preprocesses the data."""
         if self.__X_test is not None:  # pragma: no cover
             return  # pragma: no cover
+
+        self.__train_sets = {}
         synthethic_data, observed_data = self.load_data()
+
+        synthetic_train, _ = splits.train_test_split(
+            data=synthethic_data,
+            test_split=self.config.test_split,
+            input_length=self.config.time_series.input_length,
+            split_axis=self.config.split_axis,
+        )
         observed_train, observed_test = splits.train_test_split(
             data=observed_data,
             test_split=self.config.test_split,
             input_length=self.config.time_series.input_length,
             split_axis=self.config.split_axis,
         )
-        self.__train_synthetic = preprocessing.convert_dataframe_to_numpy(
-            synthethic_data
-        )
-        self.__train_observed = preprocessing.convert_dataframe_to_numpy(observed_train)
-        test = preprocessing.convert_dataframe_to_numpy(observed_test)
+
+        for ratio in self.config.ratios:
+            train = preprocessing.mix_data(
+                synthetic_data=synthetic_train,
+                observed_data=observed_train,
+                ratio=ratio,
+            )
+
+            self.__train_sets[ratio] = train
+
         self.__X_test, self.__y_test = window_generator.create_window_dataset(
-            test,
-            self.config.time_series.input_length,
-            self.config.time_series.output_length,
+            observed_test, self.config.time_series
         )
 
     # sourcery skip: snake-case-functions
     @property
     def X_test(self) -> npt.NDArray[np.float64]:
         """The input of the test dataset.
 
@@ -103,37 +114,21 @@
         """
         if self.__y_test is None:
             self.prepare_data()
             return self.y_test
         return self.__y_test
 
     @property
-    def train_observed(
-        self,
-    ) -> list[npt.NDArray[np.float64]]:
-        """Lists of train sets.
-
-        One set for each ratio.
-
-        Returns:
-            A dict containing the train sets.
-        """
-        if not self.__train_observed:
-            self.prepare_data()
-            return self.train_observed
-        return self.__train_observed
-
-    @property
-    def train_synthetic(
+    def train_sets(
         self,
-    ) -> list[npt.NDArray[np.float64]]:
+    ) -> dict[float, list[npt.NDArray[np.float64]]]:
         """Lists of train sets.
 
         One set for each ratio.
 
         Returns:
             A dict containing the train sets.
         """
-        if not self.__train_synthetic:
+        if not self.__train_sets:
             self.prepare_data()
-            return self.train_synthetic
-        return self.__train_synthetic
+            return self.train_sets
+        return self.__train_sets
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/metrics/factory.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/metrics/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,15 +44,19 @@
     try:
         metric = metric_funcs[metric_id]
     except KeyError as e:
         raise MetricNotFoundError(f"Metric {metric_id} not found") from e
     return metric
 
 
+register("mean_directional_accuracy", metrics.mean_directional_accuracy)
 register("r_square", metrics.r_square)
 register("mean_absolute_error", metrics.mean_absolute_error)
 register("mean_squared_error", metrics.mean_squared_error)
 register("mean_absolute_percentage_error", metrics.mean_absolute_percentage_error)
 register("root_mean_squared_error", metrics.root_mean_squared_error)
+register("root_mean_squared_log_error", metrics.rmsle)
+register("mean_squared_log_error", metrics.msle)
 register(
     "normalized_root_mean_squared_error", metrics.normalized_root_mean_squared_error
 )
+register("mean_absolute_scaled_error", metrics.mean_absolute_scaled_error)
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/metrics/metrics.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/metrics/metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -276,14 +276,43 @@
         >>> metrics.mean_absolute_percentage_error(y_true, y_pred)
         1.0
     """
     test_input(y_true, y_pred)
     return np.average(mean_absolute_percentage_error_matrix(y_true, y_pred))
 
 
+def __mean_directional_accuracy_matrix(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64]
+) -> npt.NDArray[np.float64]:
+    return np.array(
+        [
+            np.mean(
+                (np.sign(y_true[i, 1:] - y_true[i, :-1]))
+                == np.sign(y_pred[i, 1:] - y_pred[i, :-1])
+            )
+            for i in range(y_true.shape[0])
+        ]
+    )
+
+
+def mean_directional_accuracy(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64]
+) -> np.float64:
+    """Calculates the mean directional accuracy.
+
+    Args:
+        y_true: The ground truth labels.
+        y_pred: The predicted labels.
+
+    Returns:
+        The mean directional accuracy.
+    """
+    return np.average(__mean_directional_accuracy_matrix(y_true, y_pred))
+
+
 def root_mean_squared_error(
     y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64]
 ) -> np.float64:
     """Calculates the root mean squared error.
 
     Args:
         y_true: The ground truth labels.
@@ -304,7 +333,163 @@
         y_true: The ground truth labels.
         y_pred: The predicted labels.
 
     Returns:
         The normalized root mean squared error.
     """
     return root_mean_squared_error(y_true, y_pred) / np.mean(y_true)
+
+
+def __rmsle_matrix(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64]
+) -> npt.NDArray[np.float64]:
+    return np.array(
+        [
+            sk_metrics.mean_squared_log_error(
+                y_true[:, i, :],
+                y_pred[:, i, :],
+                multioutput="raw_values",
+                squared=False,
+            )
+            for i in range(y_true.shape[1])
+        ]
+    )
+
+
+def rmsle(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64]
+) -> np.float64:
+    """Calculates the root mean squared log error.
+
+    Args:
+        y_true: The ground truth labels.
+        y_pred: The predicted labels.
+
+    Returns:
+            The root mean squared log error.
+    """
+    return np.average(__rmsle_matrix(y_true, y_pred))
+
+
+def __msle_matrix(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64]
+) -> npt.NDArray[np.float64]:
+    return np.array(
+        [
+            sk_metrics.mean_squared_log_error(
+                y_true[:, i, :], y_pred[:, i, :], multioutput="raw_values", squared=True
+            )
+            for i in range(y_true.shape[1])
+        ]
+    )
+
+
+def msle(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64]
+) -> np.float64:
+    """Calculates the mean squared log error.
+
+    Args:
+        y_true: The ground truth labels.
+        y_pred: The predicted labels.
+
+    Returns:
+        The mean squared log error.
+    """
+    return np.average(__msle_matrix(y_true, y_pred))
+
+
+def mean_absolute_scaled_error(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64]
+) -> np.float64:
+    """Calculates the mean absolute scaled error.
+
+    Args:
+        y_true: The ground truth labels.
+        y_pred: The predicted labels.
+
+    Returns:
+        The the mean absolute scaled error.
+    """
+    test_input(y_true, y_pred)
+
+    return mean_absolute_error(y_true, y_pred) / mean_absolute_error(
+        y_true[:, 1:], y_true[:, :-1]
+    )
+
+
+def __mean_average_precision_matrix(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64], treshold: float
+) -> npt.NDArray[np.float64]:
+    test_input(y_true, y_pred)
+
+    return np.array(
+        [
+            np.average(np.abs(y_true[i] - y_pred[i]) <= treshold)
+            for i in range(y_true.shape[0])
+        ]
+    )
+
+
+def mean_average_precision(
+    y_true: npt.NDArray[np.float64], y_pred: npt.NDArray[np.float64], treshold: float
+) -> np.float64:
+    """Calculates the mean average precision with a given treshold.
+
+    Args:
+        y_true: The ground truth labels.
+        y_pred: The predicted labels.
+        treshold: The maximal absolute error, which is considered correct.
+
+    Returns:
+        The the mean average precision.
+    """
+    test_input(y_true, y_pred)
+    return np.average(__mean_average_precision_matrix(y_true, y_pred, treshold))
+
+
+def mean_average_precision_0_1(
+    y_true: npt.NDArray[np.float64],
+    y_pred: npt.NDArray[np.float64],
+) -> np.float64:
+    """Calculates the mean average precision with treshold=0.1.
+
+    Args:
+        y_true: The ground truth labels.
+        y_pred: The predicted labels.
+
+    Returns:
+        The the mean average precision.
+    """
+    return mean_average_precision(y_true, y_pred, 0.1)
+
+
+def mean_average_precision_1(
+    y_true: npt.NDArray[np.float64],
+    y_pred: npt.NDArray[np.float64],
+) -> np.float64:
+    """Calculates the mean average precision with treshold=1.
+
+    Args:
+        y_true: The ground truth labels.
+        y_pred: The predicted labels.
+
+    Returns:
+        The the mean average precision.
+    """
+    return mean_average_precision(y_true, y_pred, 1)
+
+
+def mean_average_precision_10(
+    y_true: npt.NDArray[np.float64],
+    y_pred: npt.NDArray[np.float64],
+) -> np.float64:
+    """Calculates the mean average precision with treshold=10.
+
+    Args:
+        y_true: The ground truth labels.
+        y_pred: The predicted labels.
+
+    Returns:
+        The the mean average precision.
+    """
+    return mean_average_precision(y_true, y_pred, 10)
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/average_predictor.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/average_predictor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Provides a model, which predicts the average of the train data."""
 import dataclasses
 import statistics
 
+import pandas as pd
 import numpy as np
 import numpy.typing as npt
 
 from simba_ml.prediction.time_series.models import model
 from simba_ml.prediction.time_series.config import (
     time_series_config,
 )
@@ -32,15 +33,22 @@
             time_series_params: parameters of the time series that influence
                 the training and archicture of the model.
             model_params: configuration for the model.
         """
         super().__init__(time_series_params, model_params)
         self.avg = 0.0
 
-    def train(self, train: list[npt.NDArray[np.float64]]) -> None:
+    def set_seed(self, seed: int) -> None:
+        """Sets the seed for the model.
+
+        Args:
+            seed: seed to set.
+        """
+
+    def train(self, train: list[pd.DataFrame]) -> None:
         """Trains the model with the given data.
 
         Args:
             train: data, that can be used for training.
         """
         self.avg = statistics.mean([df.mean().mean() for df in train])
 
@@ -61,16 +69,19 @@
             >>> from simba_ml.prediction.time_series.models import average_predictor
             >>> from simba_ml.prediction.time_series.config import time_series_config
             >>> train = np.array([[[1,2], [1,2]], [[2,5], [2,6]], [[10, 11], [12,12]]])
 
             >>> train.shape
             (3, 2, 2)
             >>> model_config = average_predictor.AveragePredictorConfig()
-            >>> ts_config = time_series_config.TimeSeriesConfig()
-            >>> ts_config.input_length = 2
+            >>> ts_config = time_series_config.TimeSeriesConfig(
+            ...     input_features=["1"],
+            ...     output_features=["1"],
+            ...     input_length=2
+            ... )
             >>> model = average_predictor.AveragePredictor(ts_config, model_config)
             >>> model.train(train=train)
             >>> model.avg
             5.5
             >>> test_input = np.array([[[10, 10], [20, 20]], [[15, 15], [15, 16]]])
             >>> print(test_input)
             [[[10 10]
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/factory.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/factory.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/keras/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/keras/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Registers the keras models as plugins."""
 
 from simba_ml.prediction.time_series.models import factory
 from simba_ml.prediction.time_series.models import transfer_learning_factory
 from simba_ml.prediction.time_series.models.keras import dense_neural_network
-
 from simba_ml.prediction.time_series.models import model_to_transfer_learning_model
 
 
 def register() -> None:
     """Registers the keras models."""
     factory.register(
         "KerasDenseNeuralNetwork",
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/keras/dense_neural_network.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/keras/dense_neural_network.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,12 +44,12 @@
             + [
                 tf.keras.layers.Dense(units=units, activation="relu")
                 for units in self.model_params.architecture_params.units
             ]
             + [
                 tf.keras.layers.Dense(
                     units=time_series_params.output_length
-                    * time_series_params.num_species
+                    * len(time_series_params.output_features)
                 ),
                 tf.keras.layers.Reshape([time_series_params.output_length, -1]),
             ]
         )
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/keras/keras_model.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/keras/keras_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Provides a model that predicts next timesteps from with a keras architecture."""
 import abc
 import dataclasses
 
 import numpy as np
 import numpy.typing as npt
+import pandas as pd
 
 from simba_ml.prediction.time_series.data_loader import window_generator
 from simba_ml.prediction.time_series.models import model
 from simba_ml.prediction.time_series.config import (
     time_series_config,
 )
 from simba_ml.prediction import normalizer
@@ -54,14 +55,15 @@
 
     architecture_params: ArchitectureParams = dataclasses.field(
         default_factory=ArchitectureParams
     )
     training_params: TrainingParams = dataclasses.field(default_factory=TrainingParams)
     name: str = "Keras Model"
     normalize: bool = True
+    seed: int = 42
 
 
 class KerasModel(model.Model):
     """Defines a Keras model to predict the next timestamps.
 
     Args:
         history: History documenting the training process of the model.
@@ -82,14 +84,15 @@
             model_params: configuration for the model.
 
 
         Raises:
             TypeError: if input_length or output_length is not an integer.
         """
         super().__init__(time_series_params, model_params)
+        self.set_seed(self.model_params.seed)
         self.history = None
         self.model_params = model_params
         self.model = self.get_model(time_series_params, model_params)
         if self.model_params.normalize:
             self.normalizer = normalizer.Normalizer()
 
     @abc.abstractmethod
@@ -102,34 +105,41 @@
 
         Args:
             time_series_params: parameters of the time series that influence
                 the training and archicture of the model.
             model_params: configuration for the model.
         """
 
-    def train(self, train: list[npt.NDArray[np.float64]]) -> None:
+    def set_seed(self, seed: int) -> None:
+        """Sets the seed for the model.
+
+        Args:
+            seed: seed to set.
+        """
+        tf.random.set_seed(seed)
+        np.random.seed(seed)
+
+    def train(self, train: list[pd.DataFrame]) -> None:
         """Trains the model with the given data.
 
         Args:
             train: training data.
         """
         early_stopping = tf.keras.callbacks.EarlyStopping(
             monitor="val_loss",
             patience=self.model_params.training_params.patience,
             mode="min",
         )
         self.model.compile(
             optimizer="adam", loss="mean_squared_error", metrics=["mean_absolute_error"]
         )
         if self.model_params.normalize:
-            train = self.normalizer.normalize_train_data(train)
+            train = self.normalizer.normalize_train_data(train, self.time_series_params)
         X_train, y_train = window_generator.create_window_dataset(
-            train,
-            self.time_series_params.input_length,
-            self.time_series_params.output_length,
+            train, self.time_series_params
         )
         self.history = self.model.fit(
             X_train,
             y_train,
             epochs=self.model_params.training_params.epochs,
             callbacks=[early_stopping],
             validation_split=self.model_params.training_params.validation_split,
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/last_value_predictor.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/last_value_predictor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 """Provides a model, which predicts the last given input value."""
 import dataclasses
 
+import pandas as pd
 import numpy as np
 import numpy.typing as npt
 
 from simba_ml.prediction.time_series.models import model
 
 
 @dataclasses.dataclass
 class LastValuePredictorConfig(model.ModelConfig):
     """Defines the configuration for the DenseNeuralNetwork."""
 
     name: str = "Last Value Predictor"
+    seed: int = 42
 
 
 class LastValuePredictor(model.Model):
     """Defines a model, which predicts the previous value."""
 
-    def train(self, train: list[npt.NDArray[np.float64]]) -> None:
+    def set_seed(self, seed: int) -> None:
+        """Sets the seed for the model.
+
+        Args:
+            seed: seed to set.
+        """
+
+    def train(self, train: list[pd.DataFrame]) -> None:
         """Trains the model with the given data.
 
         Args:
             train: data, that can be used for training.
         """
 
     def predict(self, data: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]:
@@ -40,16 +49,19 @@
             >>> import numpy as np
             >>> from simba_ml.prediction.time_series.models import last_value_predictor
             >>> from simba_ml.prediction.time_series.config import time_series_config
             >>> train = np.array([[[1,2], [1,2]], [[2,5], [2,6]], [[10, 11], [12,12]]])
             >>> train.shape
             (3, 2, 2)
             >>> model_config = last_value_predictor.LastValuePredictorConfig()
-            >>> ts_config = time_series_config.TimeSeriesConfig()
-            >>> ts_config.input_length = 2
+            >>> ts_config = time_series_config.TimeSeriesConfig(
+            ...     input_features=["1", "2"],
+            ...     output_features=["1", "2"],
+            ...     input_length=2
+            ... )
             >>> model = last_value_predictor.LastValuePredictor(ts_config, model_config)
             >>> model.train(train=train)
             >>> test_input = np.array([[[10, 10], [20, 20]], [[15, 15], [15, 16]]])
             >>> print(test_input)
             [[[10 10]
               [20 20]]
             <BLANKLINE>
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/model.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Provides an abstract Model."""
 import abc
 import dataclasses
 
+import pandas as pd
 import numpy as np
 import numpy.typing as npt
 
 from simba_ml import error_handler
 from simba_ml.prediction.time_series.config import (
     time_series_config,
 )
@@ -51,15 +52,23 @@
         error_handler.confirm_param_is_int(
             param=time_series_params.output_length, param_name="output_length"
         )
         self.time_series_params = time_series_params
         self.model_params = model_params
 
     @abc.abstractmethod
-    def train(self, train: list[npt.NDArray[np.float64]]) -> None:
+    def set_seed(self, seed: int) -> None:
+        """Sets the seed for the model.
+
+        Args:
+            seed: the seed to set.
+        """
+
+    @abc.abstractmethod
+    def train(self, train: list[pd.DataFrame]) -> None:
         """Trains the model with the given data.
 
         Args:
             train: training data.
         """
 
     @abc.abstractmethod
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,33 +57,33 @@
         super().__init__()
         self.time_series_params = time_series_params
         self.model_params = model_params
         self.model = nn.Sequential(
             nn.Flatten(),
             nn.Linear(
                 in_features=time_series_params.input_length
-                * time_series_params.num_species,
+                * len(time_series_params.input_features),
                 out_features=model_params.architecture_params.units,
             ),
             nn.ReLU(),
             nn.Linear(
                 in_features=model_params.architecture_params.units,
                 out_features=time_series_params.output_length
-                * time_series_params.num_species,
+                * len(time_series_params.output_features),
             ),
         )
 
     def forward(  # pylint: disable=arguments-differ
         self, x: torch.Tensor
     ) -> torch.Tensor:
         return self.model(x).reshape(
             (
                 x.shape[0],
                 self.time_series_params.output_length,
-                self.time_series_params.num_species,
+                len(self.time_series_params.output_features),
             )
         )
 
     def configure_optimizers(self) -> torch.optim.Adam:
         return torch.optim.Adam(self.parameters(), lr=1e-3)
 
     def training_step(  # pylint: disable=arguments-differ
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Provides a model that predicts next timesteps from with a\
      pytorch lightning architecture."""
 import abc
 import dataclasses
-import multiprocessing
 
 import torch
 from torch import utils
 import numpy as np
 import numpy.typing as npt
+import pandas as pd
 
 from simba_ml.prediction.time_series.data_loader import window_generator
 from simba_ml.prediction.time_series.models import model
 from simba_ml.prediction import normalizer
 from simba_ml.prediction.time_series.config import (
     time_series_config,
 )
@@ -48,26 +48,28 @@
     """Defines the parameters for the training."""
 
     epochs: int = 10
     patience: int = 5
     batch_size: int = 32
     validation_split: float = 0.2
     verbose: int = 0
+    accelerator: str = "auto"
 
 
 @dataclasses.dataclass
 class PytorchLightningModelConfig(model.ModelConfig):
     """Defines the configuration for the PytorchLightningModel."""
 
     name: str = "Pytorch Lightning Model"
     architecture_params: ArchitectureParams = dataclasses.field(
         default_factory=ArchitectureParams
     )
     training_params: TrainingParams = dataclasses.field(default_factory=TrainingParams)
     normalize: bool = True
+    seed: int = 42
 
 
 class PytorchLightningModel(model.Model):
     """Defines a Pytorch Lightning model to predict the next timestamps."""
 
     model_params: PytorchLightningModelConfig
 
@@ -83,14 +85,15 @@
                 influence the training and archicture of the model.
             model_params: configuration for the model.
 
         Raises:
             TypeError: if input_length or output_length is not an integer.
         """
         super().__init__(time_series_params, model_params)
+        self.set_seed(self.model_params.seed)
         if self.model_params.normalize:
             self.normalizer = normalizer.Normalizer()
         self.model_params = model_params
         self.model = self.get_model(time_series_params, model_params)
 
     @abc.abstractmethod
     def get_model(
@@ -102,58 +105,66 @@
 
         Args:
             time_series_params: configuration for the time series that
                 influence the training and archicture of the model.
             model_params: configuration for the model.
         """
 
-    def train(self, train: list[npt.NDArray[np.float64]]) -> None:
+    def set_seed(self, seed: int) -> None:
+        """Sets the seed for the model.
+
+        Args:
+            seed: seed to set.
+        """
+        torch.manual_seed(seed)
+        np.random.seed(seed)
+
+    def train(self, train: list[pd.DataFrame]) -> None:
         """Trains the model with the given data.
 
         Args:
             train: training data.
         """
         train = [array.astype(np.float32) for array in train]
 
         if self.model_params.normalize:
-            train = self.normalizer.normalize_train_data(train)
+            train = self.normalizer.normalize_train_data(train, self.time_series_params)
 
         X_train, y_train = window_generator.create_window_dataset(
-            train,
-            self.time_series_params.input_length,
-            self.time_series_params.output_length,
+            train, self.time_series_params
         )
 
         train_data = list(zip(X_train, y_train))
 
-        num_cores = multiprocessing.cpu_count()
         train_loader: utils.data.DataLoader[
             torch.FloatTensor  # pylint: disable=no-member
         ] = utils.data.DataLoader(
             train_data,  # type: ignore[arg-type]
             batch_size=self.model_params.training_params.batch_size,
             shuffle=True,
-            num_workers=num_cores,
+            num_workers=0,
         )
 
         trainer = pl.Trainer(
             max_epochs=self.model_params.training_params.epochs,
             log_every_n_steps=len(train_loader) // 2,
+            accelerator=self.model_params.training_params.accelerator,
         )
         trainer.fit(self.model, train_loader)
 
     def predict(self, data: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]:
         """Predicts the next timestamps for every row (time series).
 
         Args:
             data: np.array, where each dataframe is a time series.
 
         Returns:
             np.array, where each value is a time series.
         """
+        self.set_seed(self.model_params.seed)
         if self.model_params.normalize:
             data = self.normalizer.normalize_test_data(data)
         data_to_torch = torch.from_numpy(data).to(  # pylint: disable=no-member
             torch.float32  # pylint: disable=no-member
         )
         prediction = self.model(data_to_torch).cpu().detach().numpy()
         if self.model_params.normalize:
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Provides an arbitrary sk learn model architecture for prediction."""
 import abc
 import dataclasses
 
+import pandas as pd
 import sklearn as sk
 import numpy as np
 import numpy.typing as npt
 
 from simba_ml.prediction.time_series.models import model
 from simba_ml.prediction import normalizer
 from simba_ml.prediction.time_series.data_loader import window_generator
@@ -16,14 +17,15 @@
 
 @dataclasses.dataclass
 class SkLearnModelConfig(model.ModelConfig):
     """Defines the configuration for the SkLearnModel."""
 
     name: str = "SkLearn Model"
     normalize: bool = True
+    seed: int = 42
 
 
 class SkLearnModel(model.Model):
     """Defines a model that uses the scikit learn library for prediction.
 
     Args:
         config: configuration for the model.
@@ -44,39 +46,46 @@
             model_params: configuration for the model.
 
         """
         super().__init__(
             time_series_params,
             model_params,
         )
+        self.set_seed(self.model_params.seed)
         if self.model_params.normalize:
             self.normalizer = normalizer.Normalizer()
         self.model = self.get_model(model_params)
 
     @abc.abstractmethod
     def get_model(self, model_params: SkLearnModelConfig) -> sk.base.BaseEstimator:
         """Returns the model.
 
         Args:
             model_params: configuration for the model.
         """
 
-    def train(self, train: list[npt.NDArray[np.float64]]) -> None:
+    def set_seed(self, seed: int) -> None:
+        """Sets the seed for the model.
+
+        Args:
+            seed: seed to set.
+        """
+        np.random.seed(seed)
+
+    def train(self, train: list[pd.DataFrame]) -> None:
         """Trains the model with the train data flattened to two dimensions.
 
         Args:
             train: training data.
         """
         if self.model_params.normalize:
             self.normalizer = normalizer.Normalizer()
-            train = self.normalizer.normalize_train_data(train)
+            train = self.normalizer.normalize_train_data(train, self.time_series_params)
         X_train, y_train = window_generator.create_window_dataset(
-            train,
-            self.time_series_params.input_length,
-            self.time_series_params.output_length,
+            train, self.time_series_params
         )
         X_train = np.reshape(
             X_train, (X_train.shape[0], X_train.shape[1] * X_train.shape[2])
         )
         y_train = np.reshape(
             y_train, (y_train.shape[0], y_train.shape[1] * y_train.shape[2])
         )
@@ -103,13 +112,13 @@
         )
         prediction = self.model.predict(data)
         prediction = np.reshape(
             prediction,
             (
                 original_data_shape[0],
                 self.time_series_params.output_length,
-                original_data_shape[2],
+                len(self.time_series_params.output_features),
             ),
         )
         if self.model_params.normalize:
             prediction = self.normalizer.denormalize_prediction_data(prediction)
         return prediction
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/transfer_learning_factory.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/transfer_learning_factory.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/models/transfer_learning_model.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """Pipeline for running predictions."""
 import argparse
 import logging
+import random
 import tomli
 
+import pandas as pd
+
 import dacite
 from numpy import typing as npt
 import numpy as np
 
 from simba_ml.prediction.time_series.models import model as model_module
 from simba_ml.prediction.time_series.models import factory
 from simba_ml.prediction import plugin_loader
-from simba_ml.prediction.time_series.config.mixed_data_pipeline import pipeline_config
-from simba_ml.prediction.time_series.data_loader import mixed_data_loader
+from simba_ml.prediction.time_series.config.synthetic_data_pipeline import (
+    pipeline_config,
+)
+from simba_ml.prediction.time_series.data_loader import synthetic_data_loader
 from simba_ml.prediction.time_series.metrics import metrics as metrics_module
 from simba_ml.prediction.logging import wandb_logger as wandb
 from simba_ml.prediction.time_series.config import (
     time_series_config,
 )
 
 logger = logging.getLogger(__name__)
@@ -33,25 +38,24 @@
 
 
 def __evaluate_metrics(
     metrics: dict[str, metrics_module.Metric],
     y_test: npt.NDArray[np.float64],
     predictions: npt.NDArray[np.float64],
     experiment_logger: wandb.WandbLogger,
-    current_ratio: float,
 ) -> dict[str, np.float64]:
     evaluation = {
         metric_id: metric_function(y_true=y_test, y_pred=predictions)
         for metric_id, metric_function in metrics.items()
     }
-    experiment_logger.log(data=evaluation | {"ratio": current_ratio})
+    experiment_logger.log(data=evaluation)
     return evaluation
 
 
-def main(config_path: str) -> dict[str, dict[str, dict[str, np.float64]]]:
+def main(config_path: str) -> pd.DataFrame:
     """Starts the pipeline.
 
     Args:
         config_path: path to the config file.
 
     Returns:
         Returns a dictionary which contains the evaluation results
@@ -63,52 +67,55 @@
     config = dacite.from_dict(
         data_class=pipeline_config.PipelineConfig,
         data=config_json,
         config=dacite.Config(strict=True),
     )
     plugin_loader.load_plugins(config.plugins)
 
+    # set seed
+    np.random.seed(config.seed)
+    random.seed(config.seed)
+
     # set up wandb
     wandb_logger = wandb.WandbLogger(config.logging)
     wandb_logger.login()
 
     # instantiate models
     logging.info("Creating models...")
     models = [
         _model_config_factory(model, config.data.time_series) for model in config.models
     ]
 
     # create list of evaluation results for each ratio-run: {model, {metric, value}}
-    evaluation_results: dict[str, dict[str, dict[str, np.float64]]] = {
-        str(ratio): {} for ratio in config.data.ratios
+    evaluation_results: dict[str, dict[str, np.float64]] = {
+        model.name: {} for model in models
     }
 
     # instantiate dataloader with config file
-    dataloader = mixed_data_loader.MixedDataLoader(config.data)
+    dataloader = synthetic_data_loader.SyntheticDataLoader(config.data)
 
     # train models on all defined ratios of synthethic to observed data
-    for ratio in config.data.ratios:
-        for model in models:
-            # get timestamp for wandb run name
-            wandb_logger.init(
-                config=(config.data.__dict__ | model.model_params.__dict__),
-                name=f"{model.name}",
-            )
-            model.train(dataloader.train_sets[ratio])
-            logger.info("Running prediction for %s", model.name)
-            evaluation_results[str(ratio)][model.name] = __evaluate_metrics(
-                config.metric_functions,
-                dataloader.y_test,
-                model.predict(dataloader.X_test),
-                wandb_logger,
-                ratio,
-            )
-            wandb_logger.finish()
+    for model in models:
+        # get timestamp for wandb run name
+        wandb_logger.init(
+            config=(config.data.__dict__ | model.model_params.__dict__),
+            name=f"{model.name}",
+        )
+        logger.info("Training model %s", model.name)
+        model.train(dataloader.train)
+        logger.info("Running prediction for %s", model.name)
+        evaluation_results[model.name] = __evaluate_metrics(
+            config.metric_functions,
+            dataloader.y_test,
+            model.predict(dataloader.X_test),
+            wandb_logger,
+        )
+        wandb_logger.finish()
 
-    return evaluation_results
+    return pd.DataFrame(evaluation_results).T
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--config-path", type=str)
     args = parser.parse_args()
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """Pipeline for running predictions."""
 import argparse
 import logging
+import random
 import tomli
 
-import pandas as pd
-
 import dacite
 from numpy import typing as npt
 import numpy as np
+import pandas as pd
 
-from simba_ml.prediction.time_series.models import model as model_module
-from simba_ml.prediction.time_series.models import factory
-from simba_ml.prediction import plugin_loader
-from simba_ml.prediction.time_series.config.synthetic_data_pipeline import (
-    pipeline_config,
+from simba_ml.prediction.time_series.models import (
+    transfer_learning_factory,
+    transfer_learning_model,
 )
-from simba_ml.prediction.time_series.data_loader import synthetic_data_loader
+from simba_ml.prediction import plugin_loader
+from simba_ml.prediction.time_series.config import transfer_learning_pipeline
+from simba_ml.prediction.time_series.data_loader import transfer_learning_data_loader
 from simba_ml.prediction.time_series.metrics import metrics as metrics_module
 from simba_ml.prediction.logging import wandb_logger as wandb
 from simba_ml.prediction.time_series.config import (
     time_series_config,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def _model_config_factory(
     model_dict: dict[str, object],
     time_series_parameters: time_series_config.TimeSeriesConfig,
-) -> model_module.Model:
+) -> transfer_learning_model.TransferLearningModel:
     if not isinstance(model_dict["id"], str):
         raise TypeError("Model id must be a string.")
     model_id: str = model_dict["id"]
     del model_dict["id"]
-    return factory.create(model_id, model_dict, time_series_parameters)
+    return transfer_learning_factory.create(
+        model_id, model_dict, time_series_parameters
+    )
 
 
 def __evaluate_metrics(
     metrics: dict[str, metrics_module.Metric],
     y_test: npt.NDArray[np.float64],
     predictions: npt.NDArray[np.float64],
     experiment_logger: wandb.WandbLogger,
@@ -60,20 +62,24 @@
         Returns a dictionary which contains the evaluation results
         for each ratio for each models
     """
     # read in config and load defined plugins
     with open(config_path, mode="rb") as fp:
         config_json = tomli.load(fp)
     config = dacite.from_dict(
-        data_class=pipeline_config.PipelineConfig,
+        data_class=transfer_learning_pipeline.PipelineConfig,
         data=config_json,
         config=dacite.Config(strict=True),
     )
     plugin_loader.load_plugins(config.plugins)
 
+    # set seed
+    np.random.seed(config.seed)
+    random.seed(config.seed)
+
     # set up wandb
     wandb_logger = wandb.WandbLogger(config.logging)
     wandb_logger.login()
 
     # instantiate models
     logging.info("Creating models...")
     models = [
@@ -82,25 +88,27 @@
 
     # create list of evaluation results for each ratio-run: {model, {metric, value}}
     evaluation_results: dict[str, dict[str, np.float64]] = {
         model.name: {} for model in models
     }
 
     # instantiate dataloader with config file
-    dataloader = synthetic_data_loader.SyntheticDataLoader(config.data)
+    dataloader = transfer_learning_data_loader.TransferLearningDataLoader(config.data)
 
     # train models on all defined ratios of synthethic to observed data
     for model in models:
         # get timestamp for wandb run name
         wandb_logger.init(
             config=(config.data.__dict__ | model.model_params.__dict__),
             name=f"{model.name}",
         )
-        logger.info("Training model %s", model.name)
-        model.train(dataloader.train)
+        logger.info("Training model %s as transfer learning model", model.name)
+        model.train(
+            synthetic=dataloader.train_synthetic, observed=dataloader.train_observed
+        )
         logger.info("Running prediction for %s", model.name)
         evaluation_results[model.name] = __evaluate_metrics(
             config.metric_functions,
             dataloader.y_test,
             model.predict(dataloader.X_test),
             wandb_logger,
         )
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py` & `simba_ml-1.0.0rc2/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,116 +1,121 @@
 """Pipeline for running predictions."""
 import argparse
 import logging
+import random
 import tomli
 
 import dacite
 from numpy import typing as npt
 import numpy as np
 
-from simba_ml.prediction.time_series.models import (
-    transfer_learning_factory,
-    transfer_learning_model,
-)
+from simba_ml.prediction.time_series.models import model as model_module
+from simba_ml.prediction.time_series.models import factory
 from simba_ml.prediction import plugin_loader
-from simba_ml.prediction.time_series.config import transfer_learning_pipeline
-from simba_ml.prediction.time_series.data_loader import transfer_learning_data_loader
+from simba_ml.prediction.time_series.config.mixed_data_pipeline import pipeline_config
+from simba_ml.prediction.time_series.data_loader import mixed_data_loader
 from simba_ml.prediction.time_series.metrics import metrics as metrics_module
 from simba_ml.prediction.logging import wandb_logger as wandb
 from simba_ml.prediction.time_series.config import (
     time_series_config,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def _model_config_factory(
     model_dict: dict[str, object],
     time_series_parameters: time_series_config.TimeSeriesConfig,
-) -> transfer_learning_model.TransferLearningModel:
+) -> model_module.Model:
     if not isinstance(model_dict["id"], str):
         raise TypeError("Model id must be a string.")
     model_id: str = model_dict["id"]
     del model_dict["id"]
-    return transfer_learning_factory.create(
-        model_id, model_dict, time_series_parameters
-    )
+    return factory.create(model_id, model_dict, time_series_parameters)
 
 
 def __evaluate_metrics(
     metrics: dict[str, metrics_module.Metric],
     y_test: npt.NDArray[np.float64],
     predictions: npt.NDArray[np.float64],
     experiment_logger: wandb.WandbLogger,
+    current_ratio: float,
 ) -> dict[str, np.float64]:
     evaluation = {
         metric_id: metric_function(y_true=y_test, y_pred=predictions)
         for metric_id, metric_function in metrics.items()
     }
-    experiment_logger.log(data=evaluation)
+    experiment_logger.log(data=evaluation | {"ratio": current_ratio})
     return evaluation
 
 
-def main(config_path: str) -> dict[str, dict[str, np.float64]]:
+def main(config_path: str) -> dict[str, dict[str, dict[str, np.float64]]]:
     """Starts the pipeline.
 
     Args:
         config_path: path to the config file.
 
     Returns:
         Returns a dictionary which contains the evaluation results
         for each ratio for each models
     """
     # read in config and load defined plugins
     with open(config_path, mode="rb") as fp:
         config_json = tomli.load(fp)
     config = dacite.from_dict(
-        data_class=transfer_learning_pipeline.PipelineConfig,
+        data_class=pipeline_config.PipelineConfig,
         data=config_json,
         config=dacite.Config(strict=True),
     )
     plugin_loader.load_plugins(config.plugins)
 
+    # set seed
+    np.random.seed(config.seed)
+    random.seed(config.seed)
+
     # set up wandb
     wandb_logger = wandb.WandbLogger(config.logging)
     wandb_logger.login()
 
     # instantiate models
     logging.info("Creating models...")
     models = [
         _model_config_factory(model, config.data.time_series) for model in config.models
     ]
 
     # create list of evaluation results for each ratio-run: {model, {metric, value}}
-    evaluation_results: dict[str, dict[str, np.float64]] = {
-        model.name: {} for model in models
+    evaluation_results: dict[str, dict[str, dict[str, np.float64]]] = {
+        str(ratio): {} for ratio in config.data.ratios
     }
 
     # instantiate dataloader with config file
-    dataloader = transfer_learning_data_loader.TransferLearningDataLoader(config.data)
+    dataloader = mixed_data_loader.MixedDataLoader(config.data)
 
     # train models on all defined ratios of synthethic to observed data
-    for model in models:
-        # get timestamp for wandb run name
-        wandb_logger.init(
-            config=(config.data.__dict__ | model.model_params.__dict__),
-            name=f"{model.name}",
-        )
-        logger.info("Training model %s as transfer learning model", model.name)
-        model.train(
-            synthetic=dataloader.train_synthetic, observed=dataloader.train_observed
-        )
-        logger.info("Running prediction for %s", model.name)
-        evaluation_results[model.name] = __evaluate_metrics(
-            config.metric_functions,
-            dataloader.y_test,
-            model.predict(dataloader.X_test),
-            wandb_logger,
-        )
-        wandb_logger.finish()
+    for ratio in config.data.ratios:
+        for model in models:
+            # get timestamp for wandb run name
+            wandb_logger.init(
+                config=(
+                    config.data.__dict__
+                    | model.model_params.__dict__
+                    | {"pipeline seed": config.seed}
+                ),
+                name=f"{model.name}",
+            )
+            model.train(dataloader.train_sets[ratio])
+            logger.info("Running prediction for %s", model.name)
+            evaluation_results[str(ratio)][model.name] = __evaluate_metrics(
+                config.metric_functions,
+                dataloader.y_test,
+                model.predict(dataloader.X_test),
+                wandb_logger,
+                ratio,
+            )
+            wandb_logger.finish()
 
     return evaluation_results
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--config-path", type=str)
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/constraints/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/constraints/constraint.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/constraints/keep_species_sum.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/constraints/keep_species_sum.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/constraints/species_value_in_range.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/constraints/species_value_in_range.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/constraints/species_value_truncator.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/constraints/species_value_truncator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         Args:
             signal: (pd.DataFrame) The signal.
 
         Returns:
             pd.DataFrame: Signal with applied noise.
         """
         noised_signal = self.sm.apply_noisifier(signal)
-        noised_signal = self.__ensure_signal_is_inside_valid_range(signal)
+        noised_signal = self.__ensure_signal_is_inside_valid_range(noised_signal)
         return noised_signal
 
     def __put_value_in_valid_range(
         self, x: float, species: species_module.Species
     ) -> float:
         """Puts a value into the valid range for a given species.
```

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/derivative_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/derivative_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/beta_distribution.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/beta_distribution.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/constant.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/constant.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/continuous_uniform_distribution.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/continuous_uniform_distribution.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/distribution.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/helper_functions.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/helper_functions.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/lognormal_distribution.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/lognormal_distribution.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/normal_distribution.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/distributions/vector_distribution.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/distributions/vector_distribution.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/generators/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/generators/generator_interface.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/generators/generator_interface.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/generators/pertubation_generator.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/generators/pertubation_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/generators/steady_state_generator.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/generators/steady_state_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/generators/time_points_generator.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/generators/time_points_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/generators/time_series_generator.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/generators/time_series_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/noisers/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/noisers/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/noisers/additive_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/noisers/additive_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/noisers/adjusting_mean_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/noisers/adjusting_mean_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/noisers/column_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/noisers/column_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/noisers/elastic_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/noisers/elastic_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/noisers/multi_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/noisers/multi_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/noisers/multiplicative_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/noisers/multiplicative_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/noisers/sequential_noiser.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/noisers/sequential_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/__init__.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/constant_suffix_remover.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/constant_suffix_remover.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/interval_sparsifier.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/interval_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/no_sparsifier.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/no_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/random_sample_sparsifier.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/random_sample_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/sparsifier/sequential_sparsifier.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/sparsifier/sequential_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/species.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/species.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/system_model/system_model.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/system_model/system_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml/simulation/system_model/system_model_interface.py` & `simba_ml-1.0.0rc2/simba_ml/simulation/system_model/system_model_interface.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc1/simba_ml.egg-info/PKG-INFO` & `simba_ml-1.0.0rc2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: simba-ml
-Version: 1.0.0rc1
+Name: simba_ml
+Version: 1.0.0rc2
 Summary: Simulation-Based Machine Learning
+Home-page: UNKNOWN
 Author: Maximilian Kleissl, Björn Heyder, Julian Zabbarov, Lukas Drews
 Author-email: maximilian.kleissl@student.hpi.de,bjoern.heyder@student.hpi.de,julian.zabbarov@student.hpi.de,lukas.drews@student.hpi.de
-Project-URL: Bug Tracker, https://gitlab.hpi.de/mpws2022br1/simba_ml/issues
-Project-URL: Source Code, https://gitlab.hpi.de/mpws2022br1/simba_ml/
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/DILiS-lab/SimbaML/issues
+Project-URL: Source Code, https://github.com/DILiS-lab/SimbaML
+Project-URL: Documentation, https://simbaml.readthedocs.io
 Keywords: python,machine learning,simulation,ordinary differential equations,ode,simba,simba-ml
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-[![pipeline status](https://gitlab.hpi.de/mpws2022br1/simba_ml/badges/main/pipeline.svg)](https://gitlab.hpi.de/mpws2022br1/simba_ml/-/commits/main)
-[![coverage report](https://gitlab.hpi.de/mpws2022br1/simba_ml/badges/main/coverage.svg)](https://gitlab.hpi.de/mpws2022br1/simba_ml/-/commits/main)
-
 # SimbaML
 
 ![Overview of the SimbaML framework](docs/source/_static/visualabstract.png)
 
 SimbaML is an all-in-one framework for integrating prior knowledge of ODE models into the ML process by synthetic data augmentation. It allows for the convenient generation of realistic synthetic data by sparsifying and adding noise. Furthermore, our framework provides customizable pipelines for various ML experiments, such as identifying needs for data collection and transfer learning.
 
 # Installation
@@ -165,8 +166,10 @@
 ```
 from simba_ml.prediction.time_series.pipelines import synthetic_data_pipeline
 result_df = synthetic_data_pipeline.main("ml_config.toml")
 ```
 
 # Documentation
 
-Comming soon!
+https://simbaml.readthedocs.io/
+
+
```

### Comparing `simba_ml-1.0.0rc1/simba_ml.egg-info/SOURCES.txt` & `simba_ml-1.0.0rc2/simba_ml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
-man/simba_ml.1
 simba_ml/__init__.py
 simba_ml/_version.py
 simba_ml/error_handler.py
 simba_ml.egg-info/PKG-INFO
 simba_ml.egg-info/SOURCES.txt
 simba_ml.egg-info/dependency_links.txt
 simba_ml.egg-info/entry_points.txt
@@ -41,22 +40,22 @@
 simba_ml/prediction/steady_state/data_loader/dataset_generator.py
 simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py
 simba_ml/prediction/steady_state/data_loader/splits.py
 simba_ml/prediction/time_series/__init__.py
 simba_ml/prediction/time_series/config/__init__.py
 simba_ml/prediction/time_series/config/time_series_config.py
 simba_ml/prediction/time_series/config/mixed_data_pipeline/__init__.py
-simba_ml/prediction/time_series/config/mixed_data_pipeline/mixed_data_config.py
+simba_ml/prediction/time_series/config/mixed_data_pipeline/data_config.py
 simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py
 simba_ml/prediction/time_series/config/synthetic_data_pipeline/__init__.py
+simba_ml/prediction/time_series/config/synthetic_data_pipeline/data_config.py
 simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py
-simba_ml/prediction/time_series/config/synthetic_data_pipeline/synthetic_data_config.py
 simba_ml/prediction/time_series/config/transfer_learning_pipeline/__init__.py
-simba_ml/prediction/time_series/config/transfer_learning_pipeline/transfer_learning_data_config.py
-simba_ml/prediction/time_series/config/transfer_learning_pipeline/transfer_learning_pipeline_config.py
+simba_ml/prediction/time_series/config/transfer_learning_pipeline/data_config.py
+simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py
 simba_ml/prediction/time_series/data_loader/__init__.py
 simba_ml/prediction/time_series/data_loader/mixed_data_loader.py
 simba_ml/prediction/time_series/data_loader/splits.py
 simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py
 simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py
 simba_ml/prediction/time_series/data_loader/window_generator.py
 simba_ml/prediction/time_series/metrics/__init__.py
```

### Comparing `simba_ml-1.0.0rc1/versioneer.py` & `simba_ml-1.0.0rc2/versioneer.py`

 * *Files identical despite different names*

