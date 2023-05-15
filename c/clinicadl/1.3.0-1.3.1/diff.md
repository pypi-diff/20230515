# Comparing `tmp/clinicadl-1.3.0.tar.gz` & `tmp/clinicadl-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinicadl-1.3.0.tar", max compression
+gzip compressed data, was "clinicadl-1.3.1.tar", max compression
```

## Comparing `clinicadl-1.3.0.tar` & `clinicadl-1.3.1.tar`

### file list

```diff
@@ -1,141 +1,138 @@
--rw-r--r--   0        0        0     1093 2023-04-13 12:16:19.852665 clinicadl-1.3.0/LICENSE.txt
--rwxr-xr-x   0        0        0     3737 2023-04-13 12:16:19.852665 clinicadl-1.3.0/README.md
--rw-r--r--   0        0        0      162 2023-04-13 12:16:19.852665 clinicadl-1.3.0/clinicadl/__init__.py
--rw-r--r--   0        0        0     1608 2023-04-13 12:16:19.852665 clinicadl-1.3.0/clinicadl/cmdline.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.852665 clinicadl-1.3.0/clinicadl/generate/__init__.py
--rw-r--r--   0        0        0    21940 2023-04-13 12:16:19.852665 clinicadl-1.3.0/clinicadl/generate/generate.py
--rw-r--r--   0        0        0      797 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_cli.py
--rw-r--r--   0        0        0     1760 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_hypometabolic_cli.py
--rw-r--r--   0        0        0     1569 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_random_cli.py
--rw-r--r--   0        0        0     1637 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_shepplogan_cli.py
--rw-r--r--   0        0        0     1759 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_trivial_cli.py
--rwxr-xr-x   0        0        0     9883 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/interpret/__init__.py
--rw-r--r--   0        0        0     4210 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/interpret/gradients.py
--rw-r--r--   0        0        0     3524 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/interpret/interpret.py
--rw-r--r--   0        0        0     3568 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/interpret/interpret_cli.py
--rw-r--r--   0        0        0     2816 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/mlflow_test.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/predict/__init__.py
--rw-r--r--   0        0        0     3089 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/predict/predict.py
--rw-r--r--   0        0        0     3301 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/predict/predict_cli.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/prepare_data/__init__.py
--rw-r--r--   0        0        0     7512 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/prepare_data/prepare_data.py
--rw-r--r--   0        0        0     8624 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/prepare_data/prepare_data_cli.py
--rw-r--r--   0        0        0    17717 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/prepare_data/prepare_data_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/__init__.py
--rw-r--r--   0        0        0     1504 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/pet_linear/cli.py
--rw-r--r--   0        0        0     4484 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/pet_linear/quality_check.py
--rw-r--r--   0        0        0     1044 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/pet_linear/utils.py
--rw-r--r--   0        0        0      747 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/qc_cli.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/__init__.py
--rwxr-xr-x   0        0        0     1787 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/cli.py
--rw-r--r--   0        0        0    22989 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/models.py
--rwxr-xr-x   0        0        0     5435 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/quality_check.py
--rwxr-xr-x   0        0        0     8355 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/utils.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_volume/__init__.py
--rw-r--r--   0        0        0      842 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_volume/cli.py
--rw-r--r--   0        0        0     1823 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_volume/quality_check.py
--rw-r--r--   0        0        0     4622 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_volume/utils.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/random_search/__init__.py
--rwxr-xr-x   0        0        0      723 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/random_search/random_search.py
--rw-r--r--   0        0        0      628 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/random_search/random_search_cli.py
--rw-r--r--   0        0        0     6558 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/random_search/random_search_utils.py
--rw-r--r--   0        0        0     1324 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/config/train_config.toml
--rw-r--r--   0        0        0      101 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/masks/README.md
--rwxr-xr-x   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/masks/__init__.py
--rw-r--r--   0        0        0      117 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/models/README.md
--rwxr-xr-x   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/models/__init__.py
--rwxr-xr-x   0        0        0       25 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/__init__.py
--rw-r--r--   0        0        0     1251 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/from_json_cli.py
--rw-r--r--   0        0        0      773 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/list_models_cli.py
--rw-r--r--   0        0        0     2057 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/resume.py
--rw-r--r--   0        0        0      526 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/resume_cli.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/__init__.py
--rw-r--r--   0        0        0     2354 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/classification_cli.py
--rw-r--r--   0        0        0     2190 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/reconstruction_cli.py
--rw-r--r--   0        0        0     2203 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/regression_cli.py
--rw-r--r--   0        0        0     3589 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/task_utils.py
--rw-r--r--   0        0        0      377 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/train.py
--rw-r--r--   0        0        0      707 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/train_cli.py
--rw-r--r--   0        0        0     8541 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/train_option.py
--rw-r--r--   0        0        0     6102 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/train_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/adapt/__init__.py
--rw-r--r--   0        0        0     3692 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/adapt/adapt.py
--rw-r--r--   0        0        0     1136 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/adapt/adapt_cli.py
--rw-r--r--   0        0        0       44 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/analysis/__init__.py
--rw-r--r--   0        0        0     7885 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/analysis/analysis.py
--rw-r--r--   0        0        0      670 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/analysis/analysis_cli.py
--rw-r--r--   0        0        0     1268 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/cli.py
--rw-r--r--   0        0        0       60 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_labels/__init__.py
--rw-r--r--   0        0        0    16143 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_labels/get_labels.py
--rw-r--r--   0        0        0     2479 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_labels/get_labels_cli.py
--rw-r--r--   0        0        0     2509 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_labels/old_get_labels_cli.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/__init__.py
--rw-r--r--   0        0        0     2465 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/get_metadata.py
--rw-r--r--   0        0        0      964 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/get_metadata_cli.py
--rw-r--r--   0        0        0       45 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_progression/__init__.py
--rw-r--r--   0        0        0     7525 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_progression/get_progression.py
--rw-r--r--   0        0        0      811 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_progression/get_progression_cli.py
--rw-r--r--   0        0        0    23294 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/getlabels/getlabels.py
--rw-r--r--   0        0        0       35 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/kfold/__init__.py
--rw-r--r--   0        0        0     6369 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/kfold/kfold.py
--rw-r--r--   0        0        0     1170 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/kfold/kfold_cli.py
--rw-r--r--   0        0        0     3997 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py
--rw-r--r--   0        0        0       35 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/split/__init__.py
--rw-r--r--   0        0        0    12006 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/split/split.py
--rw-r--r--   0        0        0     2470 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/split/split_cli.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/utils/caps_dataset/__init__.py
--rw-r--r--   0        0        0    39601 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/utils/caps_dataset/data.py
--rw-r--r--   0        0        0       45 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/utils/cli_param/__init__.py
--rw-r--r--   0        0        0     1378 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/cli_param/argument.py
--rw-r--r--   0        0        0     5309 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/cli_param/option.py
--rw-r--r--   0        0        0      897 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/cli_param/option_group.py
--rw-r--r--   0        0        0      264 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/cmdline_utils.py
--rw-r--r--   0        0        0      803 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/descriptors.py
--rw-r--r--   0        0        0     1264 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/early_stopping.py
--rw-r--r--   0        0        0      755 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/exceptions.py
--rw-r--r--   0        0        0     2362 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/logger.py
--rw-r--r--   0        0        0      192 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/__init__.py
--rw-r--r--   0        0        0    11591 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/iotools.py
--rw-r--r--   0        0        0     4480 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/logwriter.py
--rw-r--r--   0        0        0    86481 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/maps_manager.py
--rw-r--r--   0        0        0     8725 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/maps_manager_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/meta_maps/__init__.py
--rw-r--r--   0        0        0     2412 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/meta_maps/getter.py
--rw-r--r--   0        0        0    10173 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/metric_module.py
--rw-r--r--   0        0        0      354 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/autoencoder/__init__.py
--rw-r--r--   0        0        0     4751 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/autoencoder/cnn_transformer.py
--rw-r--r--   0        0        0     1496 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/autoencoder/models.py
--rw-r--r--   0        0        0     4491 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/SECNN.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/__init__.py
--rw-r--r--   0        0        0    10360 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/models.py
--rw-r--r--   0        0        0     8632 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/random.py
--rw-r--r--   0        0        0     2394 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/resnet.py
--rw-r--r--   0        0        0     3033 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/resnet3D.py
--rw-r--r--   0        0        0     2822 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/network.py
--rw-r--r--   0        0        0     4065 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/network_utils.py
--rw-r--r--   0        0        0     4377 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/sub_network.py
--rw-r--r--   0        0        0        0 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/vae/__init__.py
--rw-r--r--   0        0        0     2238 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/vae/base_vae.py
--rw-r--r--   0        0        0    10052 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/vae/vae_utils.py
--rw-r--r--   0        0        0    12099 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/vae/vanilla_vae.py
--rw-r--r--   0        0        0     1280 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/preprocessing.py
--rw-r--r--   0        0        0     3661 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/seed.py
--rw-r--r--   0        0        0       68 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/__init__.py
--rw-r--r--   0        0        0     1133 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/kfold.py
--rw-r--r--   0        0        0     7204 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/out.txt
--rw-r--r--   0        0        0     7801 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/ref.txt
--rw-r--r--   0        0        0      798 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/single_split.py
--rw-r--r--   0        0        0     9703 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/split_manager.py
--rw-r--r--   0        0        0     5059 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/test.txt
--rw-r--r--   0        0        0      142 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/__init__.py
--rw-r--r--   0        0        0     7162 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/classification.py
--rw-r--r--   0        0        0     3540 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/reconstruction.py
--rw-r--r--   0        0        0     5471 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/regression.py
--rw-r--r--   0        0        0     6976 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/task_manager.py
--rw-r--r--   0        0        0     9402 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/tsvtools_utils.py
--rw-r--r--   0        0        0     2068 2023-04-13 12:16:19.868665 clinicadl-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5356 1970-01-01 00:00:00.000000 clinicadl-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-15 15:50:37.044849 clinicadl-1.3.1/LICENSE.txt
+-rwxr-xr-x   0        0        0     3737 2023-05-15 15:50:37.044849 clinicadl-1.3.1/README.md
+-rw-r--r--   0        0        0      162 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/cmdline.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/__init__.py
+-rw-r--r--   0        0        0    21940 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate.py
+-rw-r--r--   0        0        0      797 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_cli.py
+-rw-r--r--   0        0        0     1760 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_hypometabolic_cli.py
+-rw-r--r--   0        0        0     1569 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_random_cli.py
+-rw-r--r--   0        0        0     1637 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_shepplogan_cli.py
+-rw-r--r--   0        0        0     1759 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_trivial_cli.py
+-rwxr-xr-x   0        0        0     9883 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/generate/generate_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/interpret/__init__.py
+-rw-r--r--   0        0        0     4210 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/interpret/gradients.py
+-rw-r--r--   0        0        0     3524 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/interpret/interpret.py
+-rw-r--r--   0        0        0     3568 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/interpret/interpret_cli.py
+-rw-r--r--   0        0        0     2816 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/mlflow_test.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/predict/__init__.py
+-rw-r--r--   0        0        0     3089 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/predict/predict.py
+-rw-r--r--   0        0        0     3301 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/predict/predict_cli.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/prepare_data/__init__.py
+-rw-r--r--   0        0        0     7512 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/prepare_data/prepare_data.py
+-rw-r--r--   0        0        0     8624 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/prepare_data/prepare_data_cli.py
+-rw-r--r--   0        0        0    17717 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/prepare_data/prepare_data_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/__init__.py
+-rw-r--r--   0        0        0     1504 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/pet_linear/cli.py
+-rw-r--r--   0        0        0     4484 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/pet_linear/quality_check.py
+-rw-r--r--   0        0        0     1044 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/pet_linear/utils.py
+-rw-r--r--   0        0        0      747 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/qc_cli.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/__init__.py
+-rwxr-xr-x   0        0        0     1787 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/cli.py
+-rw-r--r--   0        0        0    22989 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/models.py
+-rwxr-xr-x   0        0        0     5435 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/quality_check.py
+-rwxr-xr-x   0        0        0     8355 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_linear/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_volume/__init__.py
+-rw-r--r--   0        0        0      842 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_volume/cli.py
+-rw-r--r--   0        0        0     1823 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_volume/quality_check.py
+-rw-r--r--   0        0        0     4622 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/quality_check/t1_volume/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/random_search/__init__.py
+-rwxr-xr-x   0        0        0      723 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/random_search/random_search.py
+-rw-r--r--   0        0        0      628 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/random_search/random_search_cli.py
+-rw-r--r--   0        0        0     6558 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/random_search/random_search_utils.py
+-rw-r--r--   0        0        0     1324 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/config/train_config.toml
+-rw-r--r--   0        0        0      101 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/masks/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/masks/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/models/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/resources/models/__init__.py
+-rwxr-xr-x   0        0        0       25 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/__init__.py
+-rw-r--r--   0        0        0     1251 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/from_json_cli.py
+-rw-r--r--   0        0        0      773 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/list_models_cli.py
+-rw-r--r--   0        0        0     2057 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/resume.py
+-rw-r--r--   0        0        0      526 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/resume_cli.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/__init__.py
+-rw-r--r--   0        0        0     2354 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/classification_cli.py
+-rw-r--r--   0        0        0     2190 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/reconstruction_cli.py
+-rw-r--r--   0        0        0     2203 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/regression_cli.py
+-rw-r--r--   0        0        0     3589 2023-05-15 15:50:37.044849 clinicadl-1.3.1/clinicadl/train/tasks/task_utils.py
+-rw-r--r--   0        0        0      377 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/train/train.py
+-rw-r--r--   0        0        0      707 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/train/train_cli.py
+-rw-r--r--   0        0        0     8541 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/train/train_option.py
+-rw-r--r--   0        0        0     6102 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/train/train_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/adapt/__init__.py
+-rw-r--r--   0        0        0     3692 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/adapt/adapt.py
+-rw-r--r--   0        0        0     1136 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/adapt/adapt_cli.py
+-rw-r--r--   0        0        0       44 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/analysis/__init__.py
+-rw-r--r--   0        0        0     7885 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/analysis/analysis.py
+-rw-r--r--   0        0        0      670 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/analysis/analysis_cli.py
+-rw-r--r--   0        0        0     1268 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/cli.py
+-rw-r--r--   0        0        0       60 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_labels/__init__.py
+-rw-r--r--   0        0        0    15681 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_labels/get_labels.py
+-rw-r--r--   0        0        0     2571 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_labels/get_labels_cli.py
+-rw-r--r--   0        0        0     2601 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_labels/old_get_labels_cli.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/__init__.py
+-rw-r--r--   0        0        0     2465 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/get_metadata.py
+-rw-r--r--   0        0        0      964 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/get_metadata_cli.py
+-rw-r--r--   0        0        0       45 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_progression/__init__.py
+-rw-r--r--   0        0        0     7525 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_progression/get_progression.py
+-rw-r--r--   0        0        0      811 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/get_progression/get_progression_cli.py
+-rw-r--r--   0        0        0    23294 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/getlabels/getlabels.py
+-rw-r--r--   0        0        0       35 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/kfold/__init__.py
+-rw-r--r--   0        0        0     6369 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/kfold/kfold.py
+-rw-r--r--   0        0        0     1170 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/kfold/kfold_cli.py
+-rw-r--r--   0        0        0     3997 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py
+-rw-r--r--   0        0        0       35 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/split/__init__.py
+-rw-r--r--   0        0        0    12006 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/split/split.py
+-rw-r--r--   0        0        0     2470 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/tsvtools/split/split_cli.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/caps_dataset/__init__.py
+-rw-r--r--   0        0        0    39601 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/caps_dataset/data.py
+-rw-r--r--   0        0        0       45 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cli_param/__init__.py
+-rw-r--r--   0        0        0     1465 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cli_param/argument.py
+-rw-r--r--   0        0        0     5309 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cli_param/option.py
+-rw-r--r--   0        0        0      897 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cli_param/option_group.py
+-rw-r--r--   0        0        0      264 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/cmdline_utils.py
+-rw-r--r--   0        0        0      803 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/descriptors.py
+-rw-r--r--   0        0        0     1264 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/early_stopping.py
+-rw-r--r--   0        0        0      755 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/exceptions.py
+-rw-r--r--   0        0        0     2362 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/logger.py
+-rw-r--r--   0        0        0      192 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/__init__.py
+-rw-r--r--   0        0        0    11591 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/iotools.py
+-rw-r--r--   0        0        0     4480 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/logwriter.py
+-rw-r--r--   0        0        0    86481 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/maps_manager.py
+-rw-r--r--   0        0        0     8725 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/maps_manager/maps_manager_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/meta_maps/__init__.py
+-rw-r--r--   0        0        0     2412 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/meta_maps/getter.py
+-rw-r--r--   0        0        0    10173 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/metric_module.py
+-rw-r--r--   0        0        0      354 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/autoencoder/__init__.py
+-rw-r--r--   0        0        0     4751 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/autoencoder/cnn_transformer.py
+-rw-r--r--   0        0        0     1496 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/autoencoder/models.py
+-rw-r--r--   0        0        0     4491 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/SECNN.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/__init__.py
+-rw-r--r--   0        0        0    10360 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/models.py
+-rw-r--r--   0        0        0     8632 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/random.py
+-rw-r--r--   0        0        0     2394 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/resnet.py
+-rw-r--r--   0        0        0     3033 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/cnn/resnet3D.py
+-rw-r--r--   0        0        0     2822 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/network.py
+-rw-r--r--   0        0        0     4065 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/network_utils.py
+-rw-r--r--   0        0        0     4377 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/sub_network.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/vae/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-15 15:50:37.048849 clinicadl-1.3.1/clinicadl/utils/network/vae/base_vae.py
+-rw-r--r--   0        0        0    10052 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/network/vae/vae_utils.py
+-rw-r--r--   0        0        0    12099 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/network/vae/vanilla_vae.py
+-rw-r--r--   0        0        0     1280 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/preprocessing.py
+-rw-r--r--   0        0        0     3661 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/seed.py
+-rw-r--r--   0        0        0       68 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/split_manager/__init__.py
+-rw-r--r--   0        0        0     1133 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/split_manager/kfold.py
+-rw-r--r--   0        0        0      798 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/split_manager/single_split.py
+-rw-r--r--   0        0        0     9703 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/split_manager/split_manager.py
+-rw-r--r--   0        0        0      142 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/__init__.py
+-rw-r--r--   0        0        0     7162 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/classification.py
+-rw-r--r--   0        0        0     3540 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/reconstruction.py
+-rw-r--r--   0        0        0     5471 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/regression.py
+-rw-r--r--   0        0        0     6976 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/task_manager/task_manager.py
+-rw-r--r--   0        0        0     9396 2023-05-15 15:50:37.052850 clinicadl-1.3.1/clinicadl/utils/tsvtools_utils.py
+-rw-r--r--   0        0        0     2068 2023-05-15 15:50:37.060850 clinicadl-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5356 1970-01-01 00:00:00.000000 clinicadl-1.3.1/PKG-INFO
```

### Comparing `clinicadl-1.3.0/LICENSE.txt` & `clinicadl-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/README.md` & `clinicadl-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/cmdline.py` & `clinicadl-1.3.1/clinicadl/cmdline.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/generate/generate.py` & `clinicadl-1.3.1/clinicadl/generate/generate.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/generate/generate_cli.py` & `clinicadl-1.3.1/clinicadl/generate/generate_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/generate/generate_hypometabolic_cli.py` & `clinicadl-1.3.1/clinicadl/generate/generate_hypometabolic_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/generate/generate_random_cli.py` & `clinicadl-1.3.1/clinicadl/generate/generate_random_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/generate/generate_shepplogan_cli.py` & `clinicadl-1.3.1/clinicadl/generate/generate_shepplogan_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/generate/generate_trivial_cli.py` & `clinicadl-1.3.1/clinicadl/generate/generate_trivial_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/generate/generate_utils.py` & `clinicadl-1.3.1/clinicadl/generate/generate_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/interpret/gradients.py` & `clinicadl-1.3.1/clinicadl/interpret/gradients.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/interpret/interpret.py` & `clinicadl-1.3.1/clinicadl/interpret/interpret.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/interpret/interpret_cli.py` & `clinicadl-1.3.1/clinicadl/interpret/interpret_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/mlflow_test.py` & `clinicadl-1.3.1/clinicadl/mlflow_test.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/predict/predict.py` & `clinicadl-1.3.1/clinicadl/predict/predict.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/predict/predict_cli.py` & `clinicadl-1.3.1/clinicadl/predict/predict_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/prepare_data/prepare_data.py` & `clinicadl-1.3.1/clinicadl/prepare_data/prepare_data.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/prepare_data/prepare_data_cli.py` & `clinicadl-1.3.1/clinicadl/prepare_data/prepare_data_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/prepare_data/prepare_data_utils.py` & `clinicadl-1.3.1/clinicadl/prepare_data/prepare_data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     return parameters
 
 
 def compute_extract_json(extract_json: str) -> str:
     if extract_json is None:
         return f"extract_{int(time())}.json"
-    elif not extract_json.suffix == ".json":
+    elif not extract_json.endswith(".json"):
         return f"{extract_json}.json"
     else:
         return extract_json
 
 
 def compute_folder_and_file_type(
     parameters: Dict[str, Any]
```

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/pet_linear/cli.py` & `clinicadl-1.3.1/clinicadl/quality_check/pet_linear/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/pet_linear/quality_check.py` & `clinicadl-1.3.1/clinicadl/quality_check/pet_linear/quality_check.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/pet_linear/utils.py` & `clinicadl-1.3.1/clinicadl/quality_check/pet_linear/utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/qc_cli.py` & `clinicadl-1.3.1/clinicadl/quality_check/qc_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/t1_linear/cli.py` & `clinicadl-1.3.1/clinicadl/quality_check/t1_linear/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/t1_linear/models.py` & `clinicadl-1.3.1/clinicadl/quality_check/t1_linear/models.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/t1_linear/quality_check.py` & `clinicadl-1.3.1/clinicadl/quality_check/t1_linear/quality_check.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/t1_linear/utils.py` & `clinicadl-1.3.1/clinicadl/quality_check/t1_linear/utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/t1_volume/cli.py` & `clinicadl-1.3.1/clinicadl/quality_check/t1_volume/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/t1_volume/quality_check.py` & `clinicadl-1.3.1/clinicadl/quality_check/t1_volume/quality_check.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/quality_check/t1_volume/utils.py` & `clinicadl-1.3.1/clinicadl/quality_check/t1_volume/utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/random_search/random_search.py` & `clinicadl-1.3.1/clinicadl/random_search/random_search.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/random_search/random_search_cli.py` & `clinicadl-1.3.1/clinicadl/random_search/random_search_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/random_search/random_search_utils.py` & `clinicadl-1.3.1/clinicadl/random_search/random_search_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/resources/config/train_config.toml` & `clinicadl-1.3.1/clinicadl/resources/config/train_config.toml`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/from_json_cli.py` & `clinicadl-1.3.1/clinicadl/train/from_json_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/list_models_cli.py` & `clinicadl-1.3.1/clinicadl/train/list_models_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/resume.py` & `clinicadl-1.3.1/clinicadl/train/resume.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/resume_cli.py` & `clinicadl-1.3.1/clinicadl/train/resume_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/tasks/classification_cli.py` & `clinicadl-1.3.1/clinicadl/train/tasks/classification_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/tasks/reconstruction_cli.py` & `clinicadl-1.3.1/clinicadl/train/tasks/reconstruction_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/tasks/regression_cli.py` & `clinicadl-1.3.1/clinicadl/train/tasks/regression_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/tasks/task_utils.py` & `clinicadl-1.3.1/clinicadl/train/tasks/task_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/train_cli.py` & `clinicadl-1.3.1/clinicadl/train/train_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/train_option.py` & `clinicadl-1.3.1/clinicadl/train/train_option.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/train/train_utils.py` & `clinicadl-1.3.1/clinicadl/train/train_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/adapt/adapt.py` & `clinicadl-1.3.1/clinicadl/tsvtools/adapt/adapt.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/adapt/adapt_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/adapt/adapt_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/analysis/analysis.py` & `clinicadl-1.3.1/clinicadl/tsvtools/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/analysis/analysis_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/analysis/analysis_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/get_labels/get_labels.py` & `clinicadl-1.3.1/clinicadl/tsvtools/get_labels/get_labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,20 +123,16 @@
     copy_bids_df: DataFrame
         Cleaned copy of the input bids_df
     """
     bids_copy_df = copy(bids_df)
     nb_subjects = 0
     if mod is not None:
         for subject, session in bids_df.index.values:
-            if len(session) == 8 and (not int(session[5]) == 1):
-                session_mod = session[:5] + session[6:8]
-            else:
-                session_mod = session
             try:
-                mod_present = missing_mods_dict[session_mod].loc[subject, mod]
+                mod_present = missing_mods_dict[session].loc[subject, mod]
                 if not mod_present:
                     bids_copy_df.drop((subject, session), inplace=True)
                     nb_subjects += 1
             except KeyError:
                 bids_copy_df.drop((subject, session), inplace=True)
                 nb_subjects += 1
     logger.info(f"Dropped sessions (mod selection): {nb_subjects}")
@@ -245,14 +241,15 @@
     restriction_path: Path = None,
     variables_of_interest: List[str] = None,
     remove_smc: bool = True,
     merged_tsv: Path = None,
     missing_mods: Path = None,
     remove_unique_session: bool = False,
     output_dir: Path = None,
+    caps_directory: Path = None,
 ):
     """
     Writes one TSV file based on merged_tsv and missing_mods.
 
 
     Parameters
     ----------
@@ -278,86 +275,80 @@
         If True, subjects with only one session are removed.
     output_dir: str (path)
         Path to the directory where the output labels.tsv will be stored.
     """
 
     from clinica.utils.inputs import check_bids_folder
 
-    if not output_dir.suffix == "tsv":
-        results_directory = bids_directory.parents[0]
-        output_tsv = results_directory / "labels.tsv"
-    else:
-        results_directory = output_dir
+    if not output_dir.is_dir():
+        output_dir.mkdir(parents=True, exist_ok=True)
 
-    output_tsv = results_directory / "labels.tsv"
+    output_tsv = output_dir / "labels.tsv"
 
     commandline_to_json(
         {
             "bids_directory": bids_directory,
-            "output_dir": results_directory,
+            "output_dir": output_dir,
             "diagnoses": diagnoses,
             "modality": modality,
             "restriction_path": restriction_path,
             "variables_of_interest": variables_of_interest,
             "remove_smc": remove_smc,
             "missing_mods": missing_mods,
             "merged_tsv": merged_tsv,
             "remove_unique_session": remove_unique_session,
+            "caps_directory": caps_directory,
         },
         filename="labels.json",
     )
 
-    # Create the results directory
-    results_directory.mkdir(parents=True, exist_ok=True)
-
     # Generating the output of `clinica iotools check-missing-modalities``
-    missing_mods_directory = results_directory / "missing_mods"
+    missing_mods_directory = output_dir / "missing_mods"
     if missing_mods is not None:
         missing_mods_directory = missing_mods
 
     if not missing_mods_directory.is_dir():
         from clinica.iotools.utils.data_handling import compute_missing_mods
 
         check_bids_folder(bids_directory)
         compute_missing_mods(bids_directory, missing_mods_directory, "missing_mods")
 
     logger.info(
         f"output of clinica iotools check-missing-modalities: {missing_mods_directory}"
     )
 
     # Generating the output of `clinica iotools merge-tsv `
-    merged_tsv_path = results_directory / "merged.tsv"
-    if merged_tsv is not None:
-        merged_tsv_path = merged_tsv
-    elif not merged_tsv_path.is_file():
+    if merged_tsv is None:
+        merged_tsv = output_dir / "merged.tsv"
+    elif not merged_tsv.is_file():
         from clinica.iotools.utils.data_handling import create_merge_file
 
         logger.info("create merge tsv")
         check_bids_folder(bids_directory)
         create_merge_file(
             bids_directory,
-            results_directory / "merged.tsv",
-            caps_dir=None,
+            merged_tsv,
+            caps_dir=caps_directory,
             pipelines=None,
             ignore_scan_files=None,
             ignore_sessions_files=None,
             volume_atlas_selection=None,
             freesurfer_atlas_selection=None,
             pvc_restriction=None,
             tsv_file=None,
             group_selection=False,
             tracers_selection=False,
         )
 
-    logger.info(f"output of clinica iotools merge-tsv: {merged_tsv_path}")
+    logger.info(f"output of clinica iotools merge-tsv: {merged_tsv}")
 
     # Reading files
-    if not merged_tsv_path.is_file():
-        raise ClinicaDLTSVError(f"{merged_tsv_path} file was not found. ")
-    bids_df = pd.read_csv(merged_tsv_path, sep="\t")
+    if not merged_tsv.is_file():
+        raise ClinicaDLTSVError(f"{merged_tsv} file was not found. ")
+    bids_df = pd.read_csv(merged_tsv, sep="\t")
     bids_df.set_index(["participant_id", "session_id"], inplace=True)
     variables_list = []
 
     if "dx1" in bids_df.columns:
         bids_df.rename(columns={"dx1": "diagnosis"}, inplace=True)
 
     try:
@@ -382,24 +373,23 @@
                 f"The variables asked by the user {variables_of_interest} do not "
                 f"exist in the data set."
             )
 
     # Loading missing modalities files
     list_files = list(missing_mods_directory.iterdir())
     missing_mods_dict = {}
-
     for file in list_files:
         fileext = file.suffix
         filename = file.stem
         if fileext == ".tsv":
             session = filename.split("_")[-1]
-            missing_mods_df = pd.read_csv(missing_mods_directory / file, sep="\t")
+            missing_mods_df = pd.read_csv(file, sep="\t")
             if len(missing_mods_df) == 0:
                 raise ClinicaDLTSVError(
-                    f"Given TSV file at {missing_mods_directory /file} loads an empty DataFrame."
+                    f"Given TSV file at {file} loads an empty DataFrame."
                 )
 
             missing_mods_df.set_index("participant_id", drop=True, inplace=True)
             missing_mods_dict[session] = missing_mods_df
 
     # Remove SMC patients
     if remove_smc:
@@ -433,8 +423,8 @@
     output_df = mod_selection(output_df, missing_mods_dict, modality)
     output_df = apply_restriction(output_df, restriction_path)
 
     output_df.reset_index()
     output_df.sort_values(by=["participant_id", "session_id"], inplace=True)
     output_df.to_csv(output_tsv, sep="\t")
 
-    logger.info(f"results are stored at {output_tsv}")
+    logger.info(f"Results are stored in {output_dir}.")
```

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/get_labels/get_labels_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/get_labels/old_get_labels_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
 
 import click
 
 from clinicadl.utils import cli_param
 
 
-@click.command(name="get-labels", no_args_is_help=True)
+@click.command(name="getlabels", no_args_is_help=True)
 @cli_param.argument.bids_directory
-@cli_param.argument.results_tsv
 @cli_param.option.diagnoses
 @cli_param.option.modality
 @cli_param.option.variables_of_interest
+@cli_param.option.caps_directory
 @click.option(
     "--restriction_tsv",
     help="Path to a TSV file containing the sessions that can be included.",
-    type=click.Path(exists=True, path_type=Path),
+    type=click.Path(exists=True),
     default=None,
 )
 @click.option(
     "--keep_smc",
     help="This flag allows to keep SMC participants, else they are removed.",
     type=bool,
     default=False,
@@ -41,51 +41,58 @@
     help="This flag allows to remove subjects with a unique session, else they are kept.",
     type=bool,
     default=False,
     is_flag=True,
 )
 def cli(
     bids_directory,
-    results_tsv,
     diagnoses,
     modality,
     restriction_tsv,
     variables_of_interest,
     keep_smc,
     missing_mods,
     merged_tsv,
     remove_unique_session,
+    caps_directory,
 ):
     """Get labels in a tsv file.
 
     This command executes the two following commands:
+
         - `clinica iotools merge-tsv`
         - `clinica iotools check-missing-modalities`
 
     BIDS_DIRECTORY is the path to the BIDS directory.
-    RESULTS_TSV is the path (including the name of the file) where the results will be save
 
     Defaults diagnoses are CN and AD.
 
     Outputs are stored in OUTPUT_TSV.
     """
+    import warnings
+
     from .get_labels import get_labels
 
+    warnings.warn(
+        "The 'tsvtools getlabels' command is deprecated and will be removed from clinicaDL in a future version. Use 'tsvtools get-labels' instead.",
+        FutureWarning,
+    )
+
     if len(variables_of_interest) == 0:
         variables_of_interest = None
 
     get_labels(
         bids_directory,
         diagnoses,
         modality=modality,
         restriction_path=restriction_tsv,
         variables_of_interest=variables_of_interest,
         remove_smc=not keep_smc,
         missing_mods=missing_mods,
         merged_tsv=merged_tsv,
         remove_unique_session=remove_unique_session,
-        output_dir=results_tsv,
+        caps_directory=caps_directory,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/get_labels/old_get_labels_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/get_labels/get_labels_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from pathlib import Path
 
 import click
 
 from clinicadl.utils import cli_param
 
 
-@click.command(name="getlabels", no_args_is_help=True)
+@click.command(name="get-labels", no_args_is_help=True)
 @cli_param.argument.bids_directory
+@cli_param.argument.output_directory
 @cli_param.option.diagnoses
 @cli_param.option.modality
 @cli_param.option.variables_of_interest
+@cli_param.option.caps_directory
 @click.option(
     "--restriction_tsv",
     help="Path to a TSV file containing the sessions that can be included.",
-    type=click.Path(exists=True),
+    type=click.Path(exists=True, path_type=Path),
     default=None,
 )
 @click.option(
     "--keep_smc",
     help="This flag allows to keep SMC participants, else they are removed.",
     type=bool,
     default=False,
@@ -40,56 +42,53 @@
     help="This flag allows to remove subjects with a unique session, else they are kept.",
     type=bool,
     default=False,
     is_flag=True,
 )
 def cli(
     bids_directory,
+    output_directory,
     diagnoses,
     modality,
     restriction_tsv,
     variables_of_interest,
     keep_smc,
     missing_mods,
     merged_tsv,
     remove_unique_session,
+    caps_directory,
 ):
     """Get labels in a tsv file.
 
     This command executes the two following commands:
-
         - `clinica iotools merge-tsv`
         - `clinica iotools check-missing-modalities`
 
     BIDS_DIRECTORY is the path to the BIDS directory.
+    TSV_DIR is the path of the directory in which the results will be saved.
 
     Defaults diagnoses are CN and AD.
 
     Outputs are stored in OUTPUT_TSV.
     """
-    import warnings
-
     from .get_labels import get_labels
 
-    warnings.warn(
-        "The 'tsvtools getlabels' command is deprecated and will be removed from clinicaDL in a future version. Use 'tsvtools get-labels' instead.",
-        FutureWarning,
-    )
-
     if len(variables_of_interest) == 0:
         variables_of_interest = None
 
     get_labels(
         bids_directory,
         diagnoses,
         modality=modality,
         restriction_path=restriction_tsv,
         variables_of_interest=variables_of_interest,
         remove_smc=not keep_smc,
         missing_mods=missing_mods,
         merged_tsv=merged_tsv,
         remove_unique_session=remove_unique_session,
+        output_dir=output_directory,
+        caps_directory=caps_directory,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/get_metadata.py` & `clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/get_metadata.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/get_metadata_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/get_metadata/get_metadata_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/get_progression/get_progression.py` & `clinicadl-1.3.1/clinicadl/tsvtools/get_progression/get_progression.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/get_progression/get_progression_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/get_progression/get_progression_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/getlabels/getlabels.py` & `clinicadl-1.3.1/clinicadl/tsvtools/getlabels/getlabels.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/kfold/kfold.py` & `clinicadl-1.3.1/clinicadl/tsvtools/kfold/kfold.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/kfold/kfold_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/kfold/kfold_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/split/split.py` & `clinicadl-1.3.1/clinicadl/tsvtools/split/split.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/tsvtools/split/split_cli.py` & `clinicadl-1.3.1/clinicadl/tsvtools/split/split_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/caps_dataset/data.py` & `clinicadl-1.3.1/clinicadl/utils/caps_dataset/data.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/cli_param/argument.py` & `clinicadl-1.3.1/clinicadl/utils/cli_param/argument.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 # TSV TOOLS
 data_tsv = click.argument("data_tsv", type=click.Path(exists=True, path_type=Path))
 old_tsv_dir = click.argument(
     "old_tsv_dir", type=click.Path(exists=True, path_type=Path)
 )
 new_tsv_dir = click.argument("new_tsv_dir", type=click.Path(path_type=Path))
+output_directory = click.argument("output_directory", type=click.Path(path_type=Path))
 dataset = click.argument("dataset", type=click.Choice(["AIBL", "OASIS"]))
 
 # GENERATE
 generated_caps = click.argument(
     "generated_caps_directory", type=click.Path(path_type=Path)
 )
```

### Comparing `clinicadl-1.3.0/clinicadl/utils/cli_param/option.py` & `clinicadl-1.3.1/clinicadl/utils/cli_param/option.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/cli_param/option_group.py` & `clinicadl-1.3.1/clinicadl/utils/cli_param/option_group.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/descriptors.py` & `clinicadl-1.3.1/clinicadl/utils/descriptors.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/early_stopping.py` & `clinicadl-1.3.1/clinicadl/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/exceptions.py` & `clinicadl-1.3.1/clinicadl/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/logger.py` & `clinicadl-1.3.1/clinicadl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/maps_manager/iotools.py` & `clinicadl-1.3.1/clinicadl/utils/maps_manager/iotools.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/maps_manager/logwriter.py` & `clinicadl-1.3.1/clinicadl/utils/maps_manager/logwriter.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/maps_manager/maps_manager.py` & `clinicadl-1.3.1/clinicadl/utils/maps_manager/maps_manager.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/maps_manager/maps_manager_utils.py` & `clinicadl-1.3.1/clinicadl/utils/maps_manager/maps_manager_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/meta_maps/getter.py` & `clinicadl-1.3.1/clinicadl/utils/meta_maps/getter.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/metric_module.py` & `clinicadl-1.3.1/clinicadl/utils/metric_module.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/autoencoder/cnn_transformer.py` & `clinicadl-1.3.1/clinicadl/utils/network/autoencoder/cnn_transformer.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/autoencoder/models.py` & `clinicadl-1.3.1/clinicadl/utils/network/autoencoder/models.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/cnn/SECNN.py` & `clinicadl-1.3.1/clinicadl/utils/network/cnn/SECNN.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/cnn/models.py` & `clinicadl-1.3.1/clinicadl/utils/network/cnn/models.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/cnn/random.py` & `clinicadl-1.3.1/clinicadl/utils/network/cnn/random.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/cnn/resnet.py` & `clinicadl-1.3.1/clinicadl/utils/network/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/cnn/resnet3D.py` & `clinicadl-1.3.1/clinicadl/utils/network/cnn/resnet3D.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/network.py` & `clinicadl-1.3.1/clinicadl/utils/network/network.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/network_utils.py` & `clinicadl-1.3.1/clinicadl/utils/network/network_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/sub_network.py` & `clinicadl-1.3.1/clinicadl/utils/network/sub_network.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/vae/base_vae.py` & `clinicadl-1.3.1/clinicadl/utils/network/vae/base_vae.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/vae/vae_utils.py` & `clinicadl-1.3.1/clinicadl/utils/network/vae/vae_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/network/vae/vanilla_vae.py` & `clinicadl-1.3.1/clinicadl/utils/network/vae/vanilla_vae.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/preprocessing.py` & `clinicadl-1.3.1/clinicadl/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/seed.py` & `clinicadl-1.3.1/clinicadl/utils/seed.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/split_manager/kfold.py` & `clinicadl-1.3.1/clinicadl/utils/split_manager/kfold.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/split_manager/single_split.py` & `clinicadl-1.3.1/clinicadl/utils/split_manager/single_split.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/split_manager/split_manager.py` & `clinicadl-1.3.1/clinicadl/utils/split_manager/split_manager.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/task_manager/classification.py` & `clinicadl-1.3.1/clinicadl/utils/task_manager/classification.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/task_manager/reconstruction.py` & `clinicadl-1.3.1/clinicadl/utils/task_manager/reconstruction.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/task_manager/regression.py` & `clinicadl-1.3.1/clinicadl/utils/task_manager/regression.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/task_manager/task_manager.py` & `clinicadl-1.3.1/clinicadl/utils/task_manager/task_manager.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.3.0/clinicadl/utils/tsvtools_utils.py` & `clinicadl-1.3.1/clinicadl/utils/tsvtools_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         row_df = diagnosis_df[diagnosis_df.participant_id == subject]
         final_df = pd.concat([final_df, row_df])
 
     return final_df
 
 
 def remove_sub_labels(
-    diagnosis_df, sub_labels, diagnosis_df_paths: list[Path], results_path: Path
+    diagnosis_df, sub_labels, diagnosis_df_paths: list, results_path: Path
 ):
     supplementary_diagnoses = []
 
     logger.debug("Before subjects removal")
     sub_df = (
         diagnosis_df.reset_index().groupby("participant_id")["session_id"].nunique()
     )
```

### Comparing `clinicadl-1.3.0/pyproject.toml` & `clinicadl-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clinicadl"
-version = "1.3.0"
+version = "1.3.1"
 description = "Framework for the reproducible processing of neuroimaging data with deep learning methods"
 license = "MIT"
 authors = ["ARAMIS Lab"]
 maintainers = ["Clinica developers <clinica-user@inria.fr>"]
 readme = "README.md"
 homepage = "https://clinicadl.readthedocs.io"
 repository = "https://github.com/aramis-lab/clinicadl.git"
```

### Comparing `clinicadl-1.3.0/PKG-INFO` & `clinicadl-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinicadl
-Version: 1.3.0
+Version: 1.3.1
 Summary: Framework for the reproducible processing of neuroimaging data with deep learning methods
 Home-page: https://clinicadl.readthedocs.io
 License: MIT
 Keywords: bids,image processing,deep learning,neuroimaging,neuroscience
 Author: ARAMIS Lab
 Maintainer: Clinica developers
 Maintainer-email: clinica-user@inria.fr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clinicadl Version: 1.3.0 Summary: Framework for the
+Metadata-Version: 2.1 Name: clinicadl Version: 1.3.1 Summary: Framework for the
 reproducible processing of neuroimaging data with deep learning methods Home-
 page: https://clinicadl.readthedocs.io License: MIT Keywords: bids,image
 processing,deep learning,neuroimaging,neuroscience Author: ARAMIS Lab
 Maintainer: Clinica developers Maintainer-email: clinica-user@inria.fr
 Requires-Python: >=3.8,<3.11 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
```

