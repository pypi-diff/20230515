# Comparing `tmp/sarus-0.6.2.tar.gz` & `tmp/sarus-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.6.2.tar", last modified: Fri May 12 10:42:30 2023, max compression
+gzip compressed data, was "sarus-0.6.3.tar", last modified: Mon May 15 09:43:35 2023, max compression
```

## Comparing `sarus-0.6.2.tar` & `sarus-0.6.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.2/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-12 10:42:30.124224 sarus-0.6.2/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.2/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.2/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.104224 sarus-0.6.2/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-12 10:41:41.000000 sarus-0.6.2/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13051 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.104224 sarus-0.6.2/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13713 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.104224 sarus-0.6.2/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.108224 sarus-0.6.2/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.108224 sarus-0.6.2/sarus/legacy/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.2/sarus/legacy/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.2/sarus/legacy/pandas/dataframe.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.112224 sarus-0.6.2/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.2/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.112224 sarus-0.6.2/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5351 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1925 2023-05-10 18:35:08.000000 sarus-0.6.2/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1239 2023-05-10 18:35:08.000000 sarus-0.6.2/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3734 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6201 2023-05-10 13:10:09.000000 sarus-0.6.2/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.112224 sarus-0.6.2/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3352 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    19506 2023-05-12 10:35:52.000000 sarus-0.6.2/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2556 2023-05-04 12:45:45.000000 sarus-0.6.2/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4591 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1572 2023-05-10 18:35:08.000000 sarus-0.6.2/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.116224 sarus-0.6.2/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.116224 sarus-0.6.2/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.116224 sarus-0.6.2/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.116224 sarus-0.6.2/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    55942 2023-05-10 13:10:09.000000 sarus-0.6.2/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.120224 sarus-0.6.2/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4618 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1112 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1569 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1074 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/storage/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.2/sarus/storage/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.2/sarus/storage/legacy_local.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1780 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11037 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      755 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.104224 sarus-0.6.2/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-12 10:42:29.000000 sarus-0.6.2/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-12 10:42:30.000000 sarus-0.6.2/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-12 10:42:29.000000 sarus-0.6.2/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.2/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      349 2023-05-12 10:42:29.000000 sarus-0.6.2/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-12 10:42:29.000000 sarus-0.6.2/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1306 2023-05-12 10:42:30.124224 sarus-0.6.2/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-12 10:42:04.000000 sarus-0.6.2/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.2/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.770840 sarus-0.6.3/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.3/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-15 09:43:35.770840 sarus-0.6.3/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.3/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.3/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.754840 sarus-0.6.3/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-15 09:43:15.000000 sarus-0.6.3/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    12834 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.754840 sarus-0.6.3/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-15 07:50:17.000000 sarus-0.6.3/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-15 07:50:17.000000 sarus-0.6.3/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13731 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.3/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.754840 sarus-0.6.3/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.754840 sarus-0.6.3/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.754840 sarus-0.6.3/sarus/legacy/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.3/sarus/legacy/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.3/sarus/legacy/pandas/dataframe.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.758839 sarus-0.6.3/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.3/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.758839 sarus-0.6.3/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7609 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.758839 sarus-0.6.3/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.3/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    21049 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2556 2023-05-04 12:45:45.000000 sarus-0.6.3/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.762839 sarus-0.6.3/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.762839 sarus-0.6.3/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.3/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.762839 sarus-0.6.3/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-15 07:50:17.000000 sarus-0.6.3/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.762839 sarus-0.6.3/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    55850 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.762839 sarus-0.6.3/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.3/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.766839 sarus-0.6.3/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.3/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-15 07:50:17.000000 sarus-0.6.3/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-15 07:50:17.000000 sarus-0.6.3/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-15 07:50:17.000000 sarus-0.6.3/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.3/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.3/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.766839 sarus-0.6.3/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.766839 sarus-0.6.3/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1074 2022-11-29 13:03:29.000000 sarus-0.6.3/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.766839 sarus-0.6.3/sarus/storage/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.3/sarus/storage/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.3/sarus/storage/legacy_local.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.770840 sarus-0.6.3/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1780 2023-05-15 07:50:17.000000 sarus-0.6.3/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10972 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.3/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.770840 sarus-0.6.3/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.3/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-15 09:41:41.000000 sarus-0.6.3/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.754840 sarus-0.6.3/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-15 09:43:35.000000 sarus-0.6.3/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-15 09:43:35.000000 sarus-0.6.3/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-15 09:43:35.000000 sarus-0.6.3/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.3/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      349 2023-05-15 09:43:35.000000 sarus-0.6.3/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-15 09:43:35.000000 sarus-0.6.3/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1306 2023-05-15 09:43:35.770840 sarus-0.6.3/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-15 09:43:07.000000 sarus-0.6.3/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-15 09:43:35.770840 sarus-0.6.3/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.3/tests/test_sanity.py
```

### Comparing `sarus-0.6.2/PKG-INFO` & `sarus-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.2/README.rst` & `sarus-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/__init__.py` & `sarus-0.6.3/sarus/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.6.2"
+VERSION = "0.6.3"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.6.2/sarus/config.yaml` & `sarus-0.6.3/sarus/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
           __eq__: pandas.PD_EQ
           abs: pandas.PD_ABS
           add: pandas.PD_ADD
           agg: pandas.PD_AGG
           any: pandas.PD_ANY
           append: pandas.PD_APPEND
           astype: pandas.PD_ASTYPE
-          corr: pandas.PD_CORR
+          corr: pandas.PD_CORR_SERIES
           count: pandas.PD_COUNT
           describe: pandas.PD_DESCRIBE
           drop: pandas.PD_DROP
           dropna: pandas.PD_DROPNA
           drop_duplicates: pandas.PD_DROP_DUPLICATES
           droplevel: pandas.PD_DROPLEVEL
           fillna: pandas.PD_FILLNA
@@ -170,15 +170,15 @@
           quantile: pandas.PD_QUANTILE
           reindex: pandas.PD_REINDEX
           rename: pandas.PD_RENAME
           replace: pandas.PD_REPLACE
           reset_index: pandas.PD_RESET_INDEX
           round: pandas.PD_ROUND
           skew: pandas.PD_SKEW
-          sort_values: pandas.PD_SORT_VALUES
+          sort_values: pandas.PD_SORT_VALUES_SERIES
           std: pandas.PD_STD
           sub: pandas.PD_SUB
           sum: pandas.PD_SUM
           to_dict: pandas.PD_TO_DICT
           nunique: pandas.PD_NUNIQUE
           unique: pandas.PD_UNIQUE
           value_counts: pandas.PD_VALUE_COUNTS
@@ -205,21 +205,14 @@
         LinearRegression:
           predict: sklearn.SK_PREDICT
           score: sklearn.SK_SCORE
     model_selection:
       sarus_functions:
         cross_val_score: sklearn.SK_CROSS_VAL_SCORE
         train_test_split: sklearn.SK_TRAIN_TEST_SPLIT
-      # classes:
-      # RepeatedStratifiedKFold:
-      #   get_n_splits: sklearn.SK_GET_N_SPLITS
-      #   split: sklearn.SK_SPLIT
-      # KFold:
-      #   get_n_splits: sklearn.SK_GET_N_SPLITS
-      #   split: sklearn.SK_SPLIT
     metrics:
       sarus_functions:
         accuracy_score: sklearn.SK_ACCURACY_SCORE
         auc: sklearn.SK_AUC
         average_precision_score: sklearn.SK_AVERAGE_PRECISION_SCORE
         classification_report: sklearn.SK_CLASSIFICATION_REPORT
         confusion_matrix: sklearn.SK_CONFUSION_MATRIX
@@ -393,9 +386,9 @@
     express:
       explicit_eval:
         - histogram
   xgboost:
     xgboost:
       classes:
         XGBClassifier:
-          predict: xgboost.XGB_PREDICT
-          predict_proba: xgboost.XGB_PREDICT_PROBA
+          predict: sklearn.SK_PREDICT
+          predict_proba: sklearn.SK_PREDICT_PROBA
```

### Comparing `sarus-0.6.2/sarus/context/local_sdk.py` & `sarus-0.6.3/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/dataspec_wrapper.py` & `sarus-0.6.3/sarus/dataspec_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from sarus.utils import register_ops
 
 logger = logging.getLogger(__name__)
 
 
 IGNORE_WARNING = [
     "_ipython_canary_method_should_not_exist_",
+    "_repr_png_",
 ]
 
 T = TypeVar("T")
 
 
 class MetaWrapper(type):
     """Metaclass to delegate some class attributes to the wrapped class."""
```

### Comparing `sarus-0.6.2/sarus/debug.py` & `sarus-0.6.3/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/imblearn/over_sampling.py` & `sarus-0.6.3/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/imblearn/pipeline.py` & `sarus-0.6.3/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/imblearn/under_sampling.py` & `sarus-0.6.3/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/legacy/pandas/dataframe.py` & `sarus-0.6.3/sarus/legacy/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/legacy/tensorflow/dataset.py` & `sarus-0.6.3/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/legacy/tensorflow/model.py` & `sarus-0.6.3/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/manager/arrow_local.py` & `sarus-0.6.3/sarus/manager/arrow_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import time
 import traceback
 import typing as t
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
@@ -33,14 +34,15 @@
         super().__init__(computing_manager)
         self.parquet_computation = parquet_computation
         self.remote_arrow = arrow_remote
 
     async def prepare(self, dataspec: st.DataSpec) -> None:
         try:
             logger.debug(f'STARTED LOCAL ARROW {dataspec.uuid()}')
+            start = time.perf_counter()
             # Only prepare parents since calling `to_arrow` will require the
             # computation of the scalars in the ancestry.
             dataset = t.cast(st.Dataset, dataspec)
 
             if self.computing_manager().is_cached(dataspec):
                 await self.parquet_computation.complete_task(dataspec)
 
@@ -69,15 +71,18 @@
                 properties={
                     "message": traceback.format_exc(),
                     'relaunch': str(False),
                 },
             )
             raise stt.DataSpecErrorStatus((False, traceback.format_exc()))
         else:
-            logger.debug(f'FINISHED LOCAL ARROW {dataspec.uuid()}')
+            end = time.perf_counter()
+            logger.debug(
+                f'FINISHED LOCAL ARROW {dataspec.uuid()} ({end-start:.2f}s)'
+            )
             stt.ready(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
             )
 
     async def result_from_stage_properties(
```

### Comparing `sarus-0.6.2/sarus/manager/arrow_remote.py` & `sarus-0.6.3/sarus/manager/arrow_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import pyarrow as pa
 import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import ARROW_TASK
 from sarus_data_spec.manager.computations.base import (
     ErrorCatchingAsyncIterator,
 )
+
 from sarus.manager.base_remote import RemoteComputation
+
 from .dataspec_api import dataset_result, dataspec_status, launch_dataspec
 
 
 class ToArrowComputationOnServer(
     RemoteComputation[t.AsyncIterator[pa.RecordBatch]]
 ):
     """ToArrowComputation on the Sarus server through the REST API."""
```

### Comparing `sarus-0.6.2/sarus/manager/base_remote.py` & `sarus-0.6.3/sarus/manager/base_remote.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
+from sarus_data_spec.manager.computations.base import status_error_policy
 from sarus_data_spec.manager.computations.remote.base import (
     RemoteComputation as BaseRemote,
-    T,
 )
-from sarus_data_spec.manager.computations.base import status_error_policy
+from sarus_data_spec.manager.computations.remote.base import T
+
 from .dataspec_api import launch_dataspec
 
 
 class RemoteComputation(BaseRemote[T]):
     async def error(
         self,
         dataspec: st.DataSpec,
```

### Comparing `sarus-0.6.2/sarus/manager/cache_scalar_local.py` & `sarus-0.6.3/sarus/manager/cache_scalar_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import pickle as pkl
+import time
 import traceback
 import typing as t
 
 import sarus_data_spec.protobuf as sp
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import (
     CACHE_PATH,
@@ -33,14 +34,15 @@
         self, computing_manager: Base, remote_scalar: ValueComputationOnServer
     ) -> None:
         super().__init__(computing_manager)
         self.remote_scalar = remote_scalar
 
     async def prepare(self, dataspec: st.DataSpec) -> None:
         logger.debug(f'STARTING CACHE_SCALAR {dataspec.uuid()}')
+        start = time.perf_counter()
         try:
             if self.computing_manager().is_computation_remote(dataspec):
                 value = await self.remote_scalar.task_result(dataspec)
             else:
                 value = await self.computing_manager().async_value_op(
                     scalar=t.cast(Scalar, dataspec)
                 )
@@ -79,15 +81,18 @@
                     "message": traceback.format_exc(),
                     'relaunch': str(False),
                 },
             )
 
             raise DataSpecErrorStatus((False, traceback.format_exc()))
         else:
-            logger.debug(f'FINISHED CACHE_SCALAR {dataspec.uuid()}')
+            end = time.perf_counter()
+            logger.debug(
+                f'FINISHED CACHE_SCALAR {dataspec.uuid()} ({end-start:.2f}s)'
+            )
             ready(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
                 properties=properties,
             )
```

### Comparing `sarus-0.6.2/sarus/manager/dataspec_api.py` & `sarus-0.6.3/sarus/manager/dataspec_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import io
 import json
+import logging
 import pickle as pkl
+import time
 import typing as t
 from http import HTTPStatus
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 from requests import Response
 from sarus_data_spec.constants import (
     BEST_ALTERNATIVE,
     CONSTRAINT_KIND,
     PRIVACY_LIMIT,
 )
-from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
+from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.protobuf.utilities import dict_deserialize, dict_serialize
 
 from sarus.typing import Client
 
+logger = logging.getLogger(__name__)
+
 
 def raise_response(resp: Response) -> None:
     """Raise exception with message encapsulated in the response JSON data."""
     if resp.status_code >= HTTPStatus.INTERNAL_SERVER_ERROR:
         resp.raise_for_status()
     if resp.status_code >= HTTPStatus.BAD_REQUEST:
         try:
@@ -35,48 +39,63 @@
     resp.raise_for_status()
 
 
 def get_dataspec(
     client: Client, uuid: str
 ) -> t.Tuple[t.Optional[st.DataSpec], float]:
     """Fetch a single Dataspec from the server."""
+    start = time.perf_counter()
     resp: Response = client.session().get(
         f"{client.url()}/dataspecs/{uuid}",
     )
+    end = time.perf_counter()
+    logger.debug(
+        f"GET /dataspecs/{uuid} {resp.status_code} ({end-start:.2f}s)"
+    )
     if resp.status_code == HTTPStatus.NOT_FOUND:
         return None, 0.0
 
     raise_response(resp)
 
     proto = dict_deserialize(resp.json()["dataspec"])
     epsilon = resp.json()["epsilon"]
     return client.context().factory().create(proto), epsilon
 
 
 def pull_dataspec_graph(client: Client, uuid: str) -> None:
     """Fetch a dataspec's computation graph and store it."""
+    start = time.perf_counter()
     resp: Response = client.session().get(
         f"{client.url()}/dataspecs/{uuid}/graph",
     )
+    end = time.perf_counter()
+    logger.debug(
+        f"GET /dataspecs/{uuid}/graph {resp.status_code} ({end-start:.2f}s)"
+    )
     raise_response(resp)
 
     protos = [dict_deserialize(msg) for msg in resp.json()]
     referrables = [
         client.context().factory().create(proto, store=False)
         for proto in protos
     ]
     client.context().storage().batch_store(referrables)
 
 
 def push_dataspec_graph(client: Client, graph: t.List[st.Referrable]) -> None:
     """Push a list of referrables to the server."""
+    start = time.perf_counter()
     resp: Response = client.session().post(
         f"{client.url()}/dataspecs/graph",
         json=[dict_serialize(ref.protobuf()) for ref in graph],
     )
+    end = time.perf_counter()
+    logger.debug(
+        f"POST /dataspecs/graph {resp.status_code} ({end-start:.2f}s)"
+    )
     raise_response(resp)
 
 
 def compile_dataspec(
     client: Client,
     uuid: str,
     constraint_kind: t.Optional[st.ConstraintKind] = None,
@@ -87,45 +106,60 @@
     Return the compiled dataspec's UUID and the optional privacy policy name.
     """
     kind_name = constraint_kind.name if constraint_kind else BEST_ALTERNATIVE
     payload = {CONSTRAINT_KIND: kind_name}
     if privacy_limit is not None:
         payload[PRIVACY_LIMIT] = privacy_limit.delta_epsilon_dict()
 
+    start = time.perf_counter()
     resp: Response = client.session().post(
         f"{client.url()}/dataspecs/{uuid}/compile",
         json=payload,
     )
+    end = time.perf_counter()
+    logger.debug(
+        f"POST /dataspecs/{uuid}/compile {resp.status_code} ({end-start:.2f}s)"
+    )
     raise_response(resp)
 
     pp_value = resp.json()["privacy_policy"]
     privacy_policy = DataspecPrivacyPolicy(pp_value) if pp_value else None
 
     return resp.json()["uuid"], privacy_policy
 
 
 def launch_dataspec(client: Client, uuid: str) -> None:
     """Launch a Dataspec's computation on the server."""
+    start = time.perf_counter()
     resp: Response = client.session().post(
         f"{client.url()}/dataspecs/{uuid}/launch",
     )
+    end = time.perf_counter()
+    logger.debug(
+        f"POST /dataspecs/{uuid}/launch {resp.status_code} ({end-start:.2f}s)"
+    )
     raise_response(resp)
 
 
 def dataspec_status(
     client: Client, uuid: str, task_names: t.List[str]
 ) -> t.Optional[sp.Status]:
     """Get the dataspec's status on the server."""
     if type(task_names) not in [set, list, tuple]:
         raise TypeError("task_names should be a list of strings.")
 
+    start = time.perf_counter()
     resp: Response = client.session().get(
         f"{client.url()}/dataspecs/{uuid}/status",
         params={"task_names": list(task_names)},
     )
+    end = time.perf_counter()
+    logger.debug(
+        f"GET /dataspecs/{uuid}/status {resp.status_code} ({end-start:.2f}s)"
+    )
     raise_response(resp)
 
     status_proto = resp.json().get("status")
     if status_proto is None:
         return None
     else:
         return dict_deserialize(status_proto)
@@ -134,35 +168,45 @@
 def pull_dataspec_status_graph(
     client: Client, uuid: str, task_names: t.List[str]
 ) -> t.List[sp.Status]:
     """Fetch the server statuses of the computation graph's dataspecs."""
     if not type(task_names) in [list, set, tuple]:
         raise TypeError("task_names should be a list of strings.")
 
+    start = time.perf_counter()
     resp: Response = client.session().get(
         f"{client.url()}/dataspecs/{uuid}/graph/statuses",
         params={"task_names": list(task_names)},
     )
+    end = time.perf_counter()
+    logger.debug(
+        f"GET /dataspecs/{uuid}/graph/statuses {resp.status_code} ({end-start:.2f}s)"
+    )
     raise_response(resp)
 
     return [dict_deserialize(msg) for msg in resp.json()]
 
 
 def dataspec_result_response(
     client: Client, uuid: str, batch_size: t.Optional[int] = None
 ) -> Response:
     """Return the response result from the server.
 
     The response holds the dataspec's value and is read in the computation.
     """
+    start = time.perf_counter()
     resp: Response = client.session().get(
         f"{client.url()}/dataspecs/{uuid}/result",
         params={"batch_size": batch_size},
         stream=True,
     )
+    end = time.perf_counter()
+    logger.debug(
+        f"GET /dataspecs/{uuid}/result {resp.status_code} {resp.headers.get('Content-Type')} ({end-start:.2f}s)"
+    )
     raise_response(resp)
     return resp
 
 
 def dataset_result(
     client: Client, uuid: str, batch_size: int
 ) -> t.AsyncIterator[pa.RecordBatch]:
```

### Comparing `sarus-0.6.2/sarus/manager/ops/api.py` & `sarus-0.6.3/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/manager/parquet_local.py` & `sarus-0.6.3/sarus/manager/parquet_local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import time
 import traceback
 import typing as t
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import CACHE_PATH, TO_PARQUET_TASK
@@ -30,14 +31,15 @@
         self, computing_manager: Base, arrow_remote: ToArrowComputationOnServer
     ) -> None:
         super().__init__(computing_manager)
         self.remote_arrow = arrow_remote
 
     async def prepare(self, dataspec: st.DataSpec) -> None:
         logger.debug(f'STARTING LOCAL TO_PARQUET {dataspec.uuid()}')
+        start = time.perf_counter()
         try:
             if self.computing_manager().is_computation_remote(dataspec):
                 iterator = await self.remote_arrow.task_result(
                     dataspec, batch_size=BATCH_SIZE
                 )
             else:
                 iterator = await self.computing_manager().async_to_arrow_op(
@@ -69,15 +71,18 @@
                 properties={
                     "message": traceback.format_exc(),
                     'relaunch': str(False),
                 },
             )
             raise DataSpecErrorStatus((False, traceback.format_exc()))
         else:
-            logger.debug(f'FINISHED LOCAL TO_PARQUET {dataspec.uuid()}')
+            end = time.perf_counter()
+            logger.debug(
+                f'FINISHED LOCAL TO_PARQUET {dataspec.uuid()} ({end-start:.2f}s)'
+            )
             ready(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=TO_PARQUET_TASK,
                 properties={CACHE_PATH: self.cache_path(dataspec)},
             )
```

### Comparing `sarus-0.6.2/sarus/manager/sdk_manager.py` & `sarus-0.6.3/sarus/manager/sdk_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 from sarus_data_spec.manager.computations.base import BaseComputation
 from sarus_data_spec.manager.computations.local.schema import SchemaComputation
 from sarus_data_spec.manager.ops.processor.routing import (
     TransformedDataset,
     TransformedScalar,
 )
 from sarus_data_spec.manager.ops.source.routing import SourceScalar
+from sarus_data_spec.schema import schema as schema_builder
+import sarus_data_spec.type as sdt
+from sarus_data_spec.arrow.type import type_from_arrow
 
 import sarus.manager.dataspec_api as api
 import sarus.manager.ops.api as api_ops
 from sarus.typing import ADMIN_DS, MOCK, PYTHON_TYPE, Client
 
-
 from .arrow_local import ToArrowComputation
 from .arrow_remote import ToArrowComputationOnServer
 from .cache_scalar_local import CacheScalarComputation
 from .parquet_local import ToParquetComputation
 from .value_local import ValueComputation
 from .value_remote import ValueComputationOnServer
 
@@ -426,27 +428,62 @@
         if stage:
             msg = stage.properties().get("message", "").replace('"', "'")
         else:
             msg = "No status found."
         if msg:
             msg = "\n" + msg
 
-        if dataspec.is_pep():
-            label_type = f"{label_type} (PEP)"
+        try:
+            if dataspec.is_pep():
+                label_type = f"{label_type} (PEP)"
+        except NameError:
+            # the transform is not included in the public SDS
+            pass
         if self.dataspec_validator().is_dp(dataspec):
             label_type = f"{label_type} (DP)"
 
         label = f"{label_type}: {symbol}{msg}"
 
         return (
             f'"{dataspec.uuid()}"[label="{label}", '
             f'fillcolor="{fillcolor}", color="{color}", shape={shape}]'
         )
 
     async def async_schema_op(self, dataset: st.Dataset) -> st.Schema:
+        # quickfix for select sql, to be removed when there is an endpoint
+        # for schema
+        if (
+            dataset.is_transformed()
+            and dataset.transform().spec() == 'select_sql'
+        ):
+            # push dataset
+            computation_graph = self.computation_graph(dataset)
+            referrables = (
+                list(computation_graph["dataspecs"])
+                + list(computation_graph["transforms"])
+                + list(computation_graph["attributes"])
+            )
+            api.push_dataspec_graph(self._client, referrables)
+            parent_schema = await self.async_schema(dataset.parents()[0][0])
+            iterator = await self.async_to_arrow(dataset, batch_size=1000)
+            table = pa.Table.from_batches([batch async for batch in iterator])
+            fields = {
+                col: type_from_arrow(
+                    arrow_type=table.field(col).type,
+                    nullable=table.field(col).nullable,
+                )
+                for col in table.schema.names
+            }
+            schema_type = sdt.Struct(fields=fields)
+            return schema_builder(
+                dataset,
+                schema_type=schema_type,
+                name=parent_schema.name(),
+            )
+
         if dataset.is_transformed():
             return await TransformedDataset(dataset).schema()
         else:
             raise ValueError('Dataset should be transformed.')
 
     async def async_to_arrow_op(
         self, dataset: st.Dataset, batch_size: int
```

### Comparing `sarus-0.6.2/sarus/manager/typing.py` & `sarus-0.6.3/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/manager/value_local.py` & `sarus-0.6.3/sarus/manager/value_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import pickle as pkl
+import time
 import traceback
 import typing as t
 
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import SCALAR_TASK, ScalarCaching
@@ -85,15 +86,15 @@
         return await self.computing_manager().async_value_op(
             scalar=t.cast(Scalar, dataspec)
         )
 
     async def prepare(self, dataspec: st.DataSpec) -> None:
         try:
             logger.debug(f'STARTED LOCAL SCALAR {dataspec.uuid()}')
-
+            start = time.perf_counter()
             if self.computing_manager().is_cached(dataspec):
                 await self.cache_scalar_computation.task_result(dataspec)
 
             elif self.computing_manager().is_computation_remote(dataspec):
                 await self.remote_scalar.complete_task(dataspec)
             else:
                 await self.computing_manager().async_prepare_parents(dataspec)
@@ -116,13 +117,16 @@
                 properties={
                     "message": traceback.format_exc(),
                     'relaunch': str(False),
                 },
             )
             raise stt.DataSpecErrorStatus((False, traceback.format_exc()))
         else:
-            logging.debug(f'FINISHED LOCAL SCALAR {dataspec.uuid()}')
+            end = time.perf_counter()
+            logging.debug(
+                f'FINISHED LOCAL SCALAR {dataspec.uuid()} ({end-start:.2f}s)'
+            )
             stt.ready(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
             )
```

### Comparing `sarus-0.6.2/sarus/manager/value_remote.py` & `sarus-0.6.3/sarus/manager/value_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing as t
 
 import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import SCALAR_TASK
+
 from sarus.manager.base_remote import RemoteComputation
 
 from .dataspec_api import dataspec_status, launch_dataspec, scalar_result
 
 
 class ValueComputationOnServer(RemoteComputation[t.Any]):
     """ValueComputation on the Sarus server through the REST API."""
```

### Comparing `sarus-0.6.2/sarus/numpy/scalars.py` & `sarus-0.6.3/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/pandas/core.py` & `sarus-0.6.3/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/pandas/dataframe.py` & `sarus-0.6.3/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sarus.py` & `sarus-0.6.3/sarus/sarus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1405,17 +1405,15 @@
             else:
                 http_status_code = request.status_code
                 http_status_name = http.HTTPStatus(http_status_code).name
                 try:
                     error_message = request.json()["error_message"]
                     wrapped_message = textwrap.indent(error_message, "  |")
 
-                    raise Exception(
-                        f"{http_status_code} - {http_status_name}: {wrapped_message}"
-                    )
+                    raise Exception(wrapped_message)
                 except (json.JSONDecodeError, KeyError):
                     raise Exception(
                         f"Error while sending a query.\
                                                              Full Gateway answer was:{request}"
                     )
 
         task_id = request.json()["task"]
```

### Comparing `sarus-0.6.2/sarus/scripts/generate_op_list.py` & `sarus-0.6.3/sarus/scripts/generate_op_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import pandas as pd
-from sarus_data_spec.config import (
+from sarus_data_spec.config import WHITELISTED_TRANSFORMS
+from sarus_data_spec.manager.ops.processor.external import (
     DP_TRANSFORMS,
     PEP_TRANSFORMS,
-    WHITELISTED_TRANSFORMS,
 )
 
 from sarus.utils import _registered_functions, _registered_methods
 
 
 def op_list() -> pd.DataFrame:
     """Return the list of ops in a pandas DataFrame."""
```

### Comparing `sarus-0.6.2/sarus/sklearn/__init__.py` & `sarus-0.6.3/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sklearn/cluster.py` & `sarus-0.6.3/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sklearn/compose.py` & `sarus-0.6.3/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sklearn/decomposition.py` & `sarus-0.6.3/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sklearn/ensemble.py` & `sarus-0.6.3/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sklearn/impute.py` & `sarus-0.6.3/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sklearn/linear_model.py` & `sarus-0.6.3/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sklearn/model_selection.py` & `sarus-0.6.3/sarus/sklearn/model_selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sarus_data_spec.protobuf as sp
-
 from sarus.dataspec_wrapper import DataSpecWrapper
 from sarus.utils import register_ops, sarus_init
 
 try:
     import sklearn.model_selection as sk_model_selection
     from sklearn.model_selection import *
 except ModuleNotFoundError:
```

### Comparing `sarus-0.6.2/sarus/sklearn/pipeline.py` & `sarus-0.6.3/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/sklearn/preprocessing.py` & `sarus-0.6.3/sarus/sklearn/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def __init__(
         self,
         *,
         _dataspec=None,
     ):
         ...
 
-    @sarus_method("sklearn.SK_FIT", inplace=True)
+    @sarus_method("sklearn.SK_FIT_Y", inplace=True)
     def fit(self, y):
         ...
 
 
 class FunctionTransformer(
     DataSpecWrapper[sk_preprocessing.FunctionTransformer]
 ):
```

### Comparing `sarus-0.6.2/sarus/sklearn/svm.py` & `sarus-0.6.3/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/skopt/searchcv.py` & `sarus-0.6.3/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/std/types.py` & `sarus-0.6.3/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/storage/legacy_local.py` & `sarus-0.6.3/sarus/storage/legacy_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/typing.py` & `sarus-0.6.3/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/utils.py` & `sarus-0.6.3/sarus/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from functools import partial, wraps
 from typing import Any, Callable, Dict, Optional, Type
 
 import sarus_data_spec.typing as st
 import yaml
 from sarus_data_spec.context import global_context
 from sarus_data_spec.transform import external
-from sarus_data_spec.variant_constraint import public_constraint
 
 from .context.typing import LocalSDKContext
 from .typing import DataSpecVariant, DataSpecWrapper
 
 logger = logging.getLogger(__name__)
 
 config_file = os.path.join(os.path.dirname(__file__), "config.yaml")
```

### Comparing `sarus-0.6.2/sarus/wrapper_factory.py` & `sarus-0.6.3/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/sarus/xgboost/xgboost.py` & `sarus-0.6.3/sarus/xgboost/xgboost.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,13 +21,13 @@
         objective="binary:logistic",
         use_label_encoder: Optional[bool] = None,
         _dataspec=None,
         **kwargs: Any,
     ):
         ...
 
-    @sarus_method("xgboost.XGB_FIT", inplace=True)
+    @sarus_method("sklearn.SK_FIT", inplace=True)
     def fit(self, X, y, sample_weight=None):
         ...
 
 
 register_ops()
```

### Comparing `sarus-0.6.2/sarus.egg-info/PKG-INFO` & `sarus-0.6.3/sarus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.2/sarus.egg-info/SOURCES.txt` & `sarus-0.6.3/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.6.2/setup.cfg` & `sarus-0.6.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.1.2.dev0
+	sarus-data-spec-public==3.2.1.dev5
 	matplotlib>=3.1
 	cloudpickle>=1.2, <2.1
 
 [options.extras_require]
 sklearn = 
-	scikit-learn==1.1.1
+	scikit-learn==1.2.2
 	scipy==1.9.0
 imblearn = 
 	imbalanced-learn
 tensorflow = 
 	tensorflow~=2.7.0  # same as on PLL server
 pandas_profiling = 
 	pandas-profiling
```

