# Comparing `tmp/hi-ml-cpath-0.3.0.tar.gz` & `tmp/hi-ml-cpath-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hi-ml-cpath-0.3.0.tar", last modified: Sun May  7 19:21:48 2023, max compression
+gzip compressed data, was "hi-ml-cpath-0.3.1.tar", last modified: Mon May 15 10:35:46 2023, max compression
```

## Comparing `hi-ml-cpath-0.3.0.tar` & `hi-ml-cpath-0.3.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3562 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/configs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/
--rw-r--r--   0 runner    (1001) docker     (122)    17055 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/BaseMIL.py
--rw-r--r--   0 runner    (1001) docker     (122)     4326 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILECrck.py
--rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILEPanda.py
--rw-r--r--   0 runner    (1001) docker     (122)     7824 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILESlidesPandaBenchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/configs/run_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/
--rw-r--r--   0 runner    (1001) docker     (122)    17147 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/base_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     2885 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/panda_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/panda_module_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datamodules/tcga_crck_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)    13476 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/dataset_return_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/default_paths.py
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/panda_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5579 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/panda_tiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/tcga_crck_tiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/datasets/tcga_prad_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/models/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/models/deepmil.py
--rw-r--r--   0 runner    (1001) docker     (122)    22673 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/models/encoders.py
--rw-r--r--   0 runner    (1001) docker     (122)    17693 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/models/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)    10310 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/create_panda_tiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    15042 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/create_tiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    19956 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/loading.py
--rw-r--r--   0 runner    (1001) docker     (122)    13827 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/tiff_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6353 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/tiling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.445846 hi-ml-cpath-0.3.0/src/health_cpath/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     4594 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/aggregate_metrics_crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/create_montage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/generate_checkpoint_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    15779 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/generate_crossval_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/mount_azure_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/scripts/tcga_dataset_prep.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/src/health_cpath/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14187 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/analysis_plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    27643 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)    13078 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/deepmil_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    25803 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/girder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/heatmap_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/montage.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/montage_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (122)    21122 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/output_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/package_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    21647 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/plots_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    14679 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/tcga_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6717 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/tiff_conversion_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    17727 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/tiles_selection_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    14170 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5868 2023-05-07 19:21:28.000000 hi-ml-cpath-0.3.0/src/health_cpath/utils/wsi_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:21:48.449846 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-07 19:21:48.000000 hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.750237 hi-ml-cpath-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-15 10:35:46.750237 hi-ml-cpath-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3562 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 10:35:46.750237 hi-ml-cpath-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.742236 hi-ml-cpath-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.742236 hi-ml-cpath-0.3.1/src/health_cpath/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.742236 hi-ml-cpath-0.3.1/src/health_cpath/configs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.746236 hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)    17055 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/BaseMIL.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4326 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/DeepSMILECrck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/DeepSMILEPanda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7824 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/DeepSMILESlidesPandaBenchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/configs/run_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.746236 hi-ml-cpath-0.3.1/src/health_cpath/datamodules/
+-rw-r--r--   0 runner    (1001) docker     (122)    17147 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datamodules/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2885 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datamodules/panda_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datamodules/panda_module_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datamodules/tcga_crck_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.746236 hi-ml-cpath-0.3.1/src/health_cpath/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)    13476 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datasets/dataset_return_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datasets/default_paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datasets/panda_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5579 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datasets/panda_tiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datasets/tcga_crck_tiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/datasets/tcga_prad_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.746236 hi-ml-cpath-0.3.1/src/health_cpath/models/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/models/deepmil.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22673 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/models/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17693 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/models/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.746236 hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)    10310 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/create_panda_tiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15042 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/create_tiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19956 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/loading.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13827 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/tiff_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6353 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/tiling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.746236 hi-ml-cpath-0.3.1/src/health_cpath/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     4594 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/scripts/aggregate_metrics_crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/scripts/create_montage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/scripts/generate_checkpoint_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15779 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/scripts/generate_crossval_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/scripts/mount_azure_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/scripts/tcga_dataset_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.750237 hi-ml-cpath-0.3.1/src/health_cpath/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14187 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/analysis_plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27643 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13078 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/deepmil_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25803 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/girder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/heatmap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/montage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/montage_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21122 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/package_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21647 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/plots_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14679 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/tcga_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6717 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/tiff_conversion_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17727 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/tiles_selection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14170 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5868 2023-05-15 10:35:34.000000 hi-ml-cpath-0.3.1/src/health_cpath/utils/wsi_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 10:35:46.750237 hi-ml-cpath-0.3.1/src/hi_ml_cpath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-15 10:35:46.000000 hi-ml-cpath-0.3.1/src/hi_ml_cpath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-05-15 10:35:46.000000 hi-ml-cpath-0.3.1/src/hi_ml_cpath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 10:35:46.000000 hi-ml-cpath-0.3.1/src/hi_ml_cpath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-15 10:35:46.000000 hi-ml-cpath-0.3.1/src/hi_ml_cpath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-15 10:35:46.000000 hi-ml-cpath-0.3.1/src/hi_ml_cpath.egg-info/top_level.txt
```

### Comparing `hi-ml-cpath-0.3.0/PKG-INFO` & `hi-ml-cpath-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-cpath
-Version: 0.3.0
+Version: 0.3.1
 Summary: Microsoft Health Futures package for deep learning on histopathology images
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Keywords: Health Futures,Health Intelligence,Computational Pathology,AzureML
 Platform: UNKNOWN
```

### Comparing `hi-ml-cpath-0.3.0/README.md` & `hi-ml-cpath-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/setup.py` & `hi-ml-cpath-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/BaseMIL.py` & `hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/BaseMIL.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILECrck.py` & `hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/DeepSMILECrck.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILEPanda.py` & `hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/DeepSMILEPanda.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/configs/classification/DeepSMILESlidesPandaBenchmark.py` & `hi-ml-cpath-0.3.1/src/health_cpath/configs/classification/DeepSMILESlidesPandaBenchmark.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datamodules/base_module.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datamodules/base_module.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datamodules/panda_module.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datamodules/panda_module.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datamodules/panda_module_benchmark.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datamodules/panda_module_benchmark.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datamodules/tcga_crck_module.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datamodules/tcga_crck_module.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datasets/base_dataset.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datasets/dataset_return_index.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datasets/dataset_return_index.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datasets/default_paths.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datasets/default_paths.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datasets/panda_dataset.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datasets/panda_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datasets/panda_tiles_dataset.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datasets/panda_tiles_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datasets/tcga_crck_tiles_dataset.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datasets/tcga_crck_tiles_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/datasets/tcga_prad_dataset.py` & `hi-ml-cpath-0.3.1/src/health_cpath/datasets/tcga_prad_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/models/deepmil.py` & `hi-ml-cpath-0.3.1/src/health_cpath/models/deepmil.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/models/encoders.py` & `hi-ml-cpath-0.3.1/src/health_cpath/models/encoders.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/models/transforms.py` & `hi-ml-cpath-0.3.1/src/health_cpath/models/transforms.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/create_panda_tiles_dataset.py` & `hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/create_panda_tiles_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/create_tiles_dataset.py` & `hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/create_tiles_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/loading.py` & `hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/loading.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/tiff_conversion.py` & `hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/tiff_conversion.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/preprocessing/tiling.py` & `hi-ml-cpath-0.3.1/src/health_cpath/preprocessing/tiling.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/scripts/aggregate_metrics_crossvalidation.py` & `hi-ml-cpath-0.3.1/src/health_cpath/scripts/aggregate_metrics_crossvalidation.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/scripts/create_montage.py` & `hi-ml-cpath-0.3.1/src/health_cpath/scripts/create_montage.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/scripts/generate_checkpoint_url.py` & `hi-ml-cpath-0.3.1/src/health_cpath/scripts/generate_checkpoint_url.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/scripts/generate_crossval_report.py` & `hi-ml-cpath-0.3.1/src/health_cpath/scripts/generate_crossval_report.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/scripts/mount_azure_dataset.py` & `hi-ml-cpath-0.3.1/src/health_cpath/scripts/mount_azure_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/scripts/tcga_dataset_prep.py` & `hi-ml-cpath-0.3.1/src/health_cpath/scripts/tcga_dataset_prep.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/analysis_plot_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/analysis_plot_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/callbacks.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/deepmil_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/deepmil_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/download_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/girder.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/girder.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/heatmap_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/layer_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/montage.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/montage.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/montage_config.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/montage_config.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/naming.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/naming.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/output_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/package_setup.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/package_setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/plots_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/plots_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/report_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/tcga_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/tcga_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/tiff_conversion_config.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/tiff_conversion_config.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/tiles_selection_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/tiles_selection_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/viz_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/viz_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/health_cpath/utils/wsi_utils.py` & `hi-ml-cpath-0.3.1/src/health_cpath/utils/wsi_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/PKG-INFO` & `hi-ml-cpath-0.3.1/src/hi_ml_cpath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-cpath
-Version: 0.3.0
+Version: 0.3.1
 Summary: Microsoft Health Futures package for deep learning on histopathology images
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Keywords: Health Futures,Health Intelligence,Computational Pathology,AzureML
 Platform: UNKNOWN
```

### Comparing `hi-ml-cpath-0.3.0/src/hi_ml_cpath.egg-info/SOURCES.txt` & `hi-ml-cpath-0.3.1/src/hi_ml_cpath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

