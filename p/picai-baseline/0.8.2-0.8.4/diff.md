# Comparing `tmp/picai_baseline-0.8.2.tar.gz` & `tmp/picai_baseline-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picai_baseline-0.8.2.tar", last modified: Thu Mar  2 16:43:05 2023, max compression
+gzip compressed data, was "picai_baseline-0.8.4.tar", last modified: Mon May 15 16:55:07 2023, max compression
```

## Comparing `picai_baseline-0.8.2.tar` & `picai_baseline-0.8.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.954009 picai_baseline-0.8.2/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2022-12-13 09:52:15.000000 picai_baseline-0.8.2/LICENSE
--rw-r--r--   0 joeranbosma   (501) staff       (20)    12609 2023-03-02 16:43:05.954084 picai_baseline-0.8.2/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11814 2023-01-12 14:14:37.000000 picai_baseline-0.8.2/README.md
--rw-r--r--   0 joeranbosma   (501) staff       (20)      472 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/pyproject.toml
--rw-r--r--   0 joeranbosma   (501) staff       (20)      870 2023-03-02 16:43:05.954450 picai_baseline-0.8.2/setup.cfg
--rw-r--r--   0 joeranbosma   (501) staff       (20)      727 2023-03-02 16:38:33.000000 picai_baseline-0.8.2/setup.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.938212 picai_baseline-0.8.2/src/
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.940247 picai_baseline-0.8.2/src/picai_baseline/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      856 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5232 2023-01-12 14:14:37.000000 picai_baseline-0.8.2/src/picai_baseline/__main__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.941723 picai_baseline-0.8.2/src/picai_baseline/nnunet/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-08-31 20:12:51.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    10618 2022-12-21 09:40:52.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/eval.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5686 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/nnunet_baseline.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    10820 2022-08-31 20:12:51.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/softmax_export.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.942858 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/__init__.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     6708 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/focal_loss.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     3692 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/io.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     2490 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_CE_checkpoints.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     7957 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_FL_and_CE.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     6302 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_focalLoss.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    22335 2023-03-01 08:52:59.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/nnunet_wrapper.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    12650 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/run_training.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     8937 2023-02-28 11:37:27.000000 picai_baseline-0.8.2/src/picai_baseline/prepare_data.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    10485 2023-02-28 11:36:42.000000 picai_baseline-0.8.2/src/picai_baseline/prepare_data_semi_supervised.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.942977 picai_baseline-0.8.2/src/picai_baseline/splits/
--rw-r--r--   0 joeranbosma   (501) staff       (20)   202261 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/__init__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.944774 picai_baseline-0.8.2/src/picai_baseline/splits/picai/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1304 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      333 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    30030 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    30080 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    29980 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    29930 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    30130 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7530 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7480 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7580 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7630 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7430 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   217842 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.946420 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1304 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      345 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      180 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-train-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-train-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-train-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-train-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      205 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-train-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      130 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      105 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1792 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.946798 picai_baseline-0.8.2/src/picai_baseline/splits/picai_nnunet/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1705 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_nnunet/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      347 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_nnunet/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)   188117 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_nnunet/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.949162 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     3126 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      349 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)   181905 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   182355 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   182230 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   182080 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   182280 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45830 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45380 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45505 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45655 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45455 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)  1320857 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.950174 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv_nnunet/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1761 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv_nnunet/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      419 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv_nnunet/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)  1191517 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv_nnunet/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.951172 picai_baseline-0.8.2/src/picai_baseline/unet/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5647 2022-12-20 10:42:09.000000 picai_baseline-0.8.2/src/picai_baseline/unet/plan_overview.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     8439 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/unet/train.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.952401 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/__init__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.953149 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11063 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/multi_threaded_augmenter.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     9507 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/nnUNet_DA.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1806 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/single_threaded_augmenter.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      667 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/test_time_augmentations.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    10425 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/callbacks.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1192 2022-08-15 08:53:24.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/compute_spec.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5840 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/data_generator.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1501 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/default_hyperparam.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5146 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/image_reader.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.953421 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/loss_functions/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/loss_functions/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1789 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/loss_functions/focal.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1287 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/neural_network_selector.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.953714 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/neural_networks/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/neural_networks/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    14022 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/neural_networks/unets.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      852 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/poly_lr.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1644 2022-07-03 16:12:55.000000 picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/preprocess_utils.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.941218 picai_baseline-0.8.2/src/picai_baseline.egg-info/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    12609 2023-03-02 16:43:05.000000 picai_baseline-0.8.2/src/picai_baseline.egg-info/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5131 2023-03-02 16:43:05.000000 picai_baseline-0.8.2/src/picai_baseline.egg-info/SOURCES.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-03-02 16:43:05.000000 picai_baseline-0.8.2/src/picai_baseline.egg-info/dependency_links.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-01-11 10:53:56.000000 picai_baseline-0.8.2/src/picai_baseline.egg-info/not-zip-safe
--rw-r--r--   0 joeranbosma   (501) staff       (20)      149 2023-03-02 16:43:05.000000 picai_baseline-0.8.2/src/picai_baseline.egg-info/requires.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)       15 2023-03-02 16:43:05.000000 picai_baseline-0.8.2/src/picai_baseline.egg-info/top_level.txt
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-03-02 16:43:05.953864 picai_baseline-0.8.2/tests/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     4719 2022-12-12 13:16:27.000000 picai_baseline-0.8.2/tests/test_splits.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.422766 picai_baseline-0.8.4/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2022-12-13 09:52:15.000000 picai_baseline-0.8.4/LICENSE
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    12928 2023-05-15 16:55:07.422936 picai_baseline-0.8.4/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    12133 2023-04-04 06:58:41.000000 picai_baseline-0.8.4/README.md
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      472 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/pyproject.toml
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      870 2023-05-15 16:55:07.423324 picai_baseline-0.8.4/setup.cfg
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      727 2023-05-15 14:35:12.000000 picai_baseline-0.8.4/setup.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.390154 picai_baseline-0.8.4/src/
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.393066 picai_baseline-0.8.4/src/picai_baseline/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      856 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5232 2023-01-12 14:14:37.000000 picai_baseline-0.8.4/src/picai_baseline/__main__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.395628 picai_baseline-0.8.4/src/picai_baseline/nnunet/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-08-31 20:12:51.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    10618 2022-12-21 09:40:52.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/eval.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5686 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/nnunet_baseline.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    10820 2022-08-31 20:12:51.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/softmax_export.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.397801 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/__init__.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     6708 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/focal_loss.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     3692 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/io.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     2490 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_CE_checkpoints.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     7957 2023-03-25 11:22:48.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_FL_and_CE.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     6302 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_focalLoss.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    23090 2023-05-02 09:49:54.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnunet_wrapper.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    12650 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/run_training.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     8937 2023-02-28 11:37:27.000000 picai_baseline-0.8.4/src/picai_baseline/prepare_data.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    10485 2023-02-28 11:36:42.000000 picai_baseline-0.8.4/src/picai_baseline/prepare_data_semi_supervised.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.397954 picai_baseline-0.8.4/src/picai_baseline/splits/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   202261 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/__init__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.402204 picai_baseline-0.8.4/src/picai_baseline/splits/picai/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1304 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      333 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    30030 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    30080 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    29980 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    29930 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    30130 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7530 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7480 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7580 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7630 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7430 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   217842 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.404792 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1304 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      345 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      180 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      205 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      130 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      105 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1792 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.405230 picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1705 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      347 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   188117 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.409610 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     3126 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      349 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   181905 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   182355 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   182230 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   182080 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   182280 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45830 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45380 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45505 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45655 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45455 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)  1320857 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.411924 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1761 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      419 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)  1191517 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.417561 picai_baseline-0.8.4/src/picai_baseline/unet/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5647 2022-12-20 10:42:09.000000 picai_baseline-0.8.4/src/picai_baseline/unet/plan_overview.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     8439 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/unet/train.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.420665 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/__init__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.421491 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11063 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/multi_threaded_augmenter.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     9507 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/nnUNet_DA.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1806 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/single_threaded_augmenter.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      667 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/test_time_augmentations.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    10436 2023-05-15 14:35:12.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/callbacks.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1192 2022-08-15 08:53:24.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/compute_spec.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5856 2023-05-15 14:35:12.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/data_generator.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1501 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/default_hyperparam.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5146 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/image_reader.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.421802 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1765 2023-05-15 14:34:37.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/focal.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1287 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_network_selector.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.422232 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    14022 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/unets.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      852 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/poly_lr.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/preprocess_utils.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.394174 picai_baseline-0.8.4/src/picai_baseline.egg-info/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    12928 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5131 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/SOURCES.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/dependency_links.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-01-11 10:53:56.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/not-zip-safe
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      149 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/requires.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       15 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/top_level.txt
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.422400 picai_baseline-0.8.4/tests/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     4719 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/tests/test_splits.py
```

### Comparing `picai_baseline-0.8.2/LICENSE` & `picai_baseline-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/PKG-INFO` & `picai_baseline-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picai_baseline
-Version: 0.8.2
+Version: 0.8.4
 Summary: PICAI Baselines
 Home-page: https://github.com/DIAGNijmegen/picai_baseline
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/picai_baseline/issues
 Platform: unix
@@ -59,15 +59,15 @@
 We define setup steps that are shared between the different baseline algorithms. To follow the baseline algorithm tutorials, this setup must be completed first.
 
 
 ### Folder Structure
 We define three main folders that must be prepared apriori:
 - `/input/` contains one of the [PI-CAI datasets](https://pi-cai.grand-challenge.org/DATA/). This can be the Public Training and Development Dataset, the Private Training Dataset, the Hidden Validation and Tuning Cohort, or the Hidden Testing Cohort.
   - `/input/images/` contains the imaging files. For the Public Training and Development Dataset, these can be retrieved [here](https://zenodo.org/record/6624726).
-  - `/input/labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
+  - `/input/picai_labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
 - `/workdir/` stores intermediate results, such as preprocessed images and annotations.
   - `/workdir/results/[model name]/` stores model checkpoints/weights during training (enables the ability to pause/resume training).    
 - `/output/` stores training output, such as trained model weights and preprocessing plan.
 
 
 ### Data Preparation
 Unless specified otherwise, this tutorial assumes that the [PI-CAI: Public Training and Development Dataset](https://pi-cai.grand-challenge.org/DATA/) will be downloaded and unpacked. Before downloading the dataset, read its [documentation](https://zenodo.org/record/6624726) and [dedicated forum post](https://grand-challenge.org/forums/forum/pi-cai-607/topic/public-training-and-development-dataset-updates-and-fixes-631/) (for all updates/fixes, if any). To download and unpack the dataset, run the following commands:
@@ -96,18 +96,31 @@
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold2.zip -d /input/images/
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold3.zip -d /input/images/
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold4.zip -d /input/images/
 ```
 
 Please follow the [instructions here](nnunet_baseline.md#nnu-net---docker-setup) to set up the Docker container.
 
-Also, collect the training annotations via the following command:
+Also, collect the training annotations. This can be done via the following command:
 
 ```bash
-git clone https://github.com/DIAGNijmegen/picai_labels /input/labels/
+cd /input
+git clone https://github.com/DIAGNijmegen/picai_labels
+```
+
+After cloning the repository with annotations, you should have a folder structure like this:
+
+```bash
+/input/picai_labels
+├── anatomical_delineations
+│   ├── ...
+├── clinical_information
+│   └── marksheet.csv
+└── csPCa_lesion_delineations
+    ├── ...
 ```
 
 
 ### Cross-Validation Splits
 We have prepared 5-fold cross-validation splits of all 1500 cases in the [PI-CAI: Public Training and Development Dataset](https://pi-cai.grand-challenge.org/DATA/). We have ensured there is no patient overlap between training/validation splits. You can load these splits as follows:
 
 ```python
```

### Comparing `picai_baseline-0.8.2/README.md` & `picai_baseline-0.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 We define setup steps that are shared between the different baseline algorithms. To follow the baseline algorithm tutorials, this setup must be completed first.
 
 
 ### Folder Structure
 We define three main folders that must be prepared apriori:
 - `/input/` contains one of the [PI-CAI datasets](https://pi-cai.grand-challenge.org/DATA/). This can be the Public Training and Development Dataset, the Private Training Dataset, the Hidden Validation and Tuning Cohort, or the Hidden Testing Cohort.
   - `/input/images/` contains the imaging files. For the Public Training and Development Dataset, these can be retrieved [here](https://zenodo.org/record/6624726).
-  - `/input/labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
+  - `/input/picai_labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
 - `/workdir/` stores intermediate results, such as preprocessed images and annotations.
   - `/workdir/results/[model name]/` stores model checkpoints/weights during training (enables the ability to pause/resume training).    
 - `/output/` stores training output, such as trained model weights and preprocessing plan.
 
 
 ### Data Preparation
 Unless specified otherwise, this tutorial assumes that the [PI-CAI: Public Training and Development Dataset](https://pi-cai.grand-challenge.org/DATA/) will be downloaded and unpacked. Before downloading the dataset, read its [documentation](https://zenodo.org/record/6624726) and [dedicated forum post](https://grand-challenge.org/forums/forum/pi-cai-607/topic/public-training-and-development-dataset-updates-and-fixes-631/) (for all updates/fixes, if any). To download and unpack the dataset, run the following commands:
@@ -71,18 +71,31 @@
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold2.zip -d /input/images/
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold3.zip -d /input/images/
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold4.zip -d /input/images/
 ```
 
 Please follow the [instructions here](nnunet_baseline.md#nnu-net---docker-setup) to set up the Docker container.
 
-Also, collect the training annotations via the following command:
+Also, collect the training annotations. This can be done via the following command:
 
 ```bash
-git clone https://github.com/DIAGNijmegen/picai_labels /input/labels/
+cd /input
+git clone https://github.com/DIAGNijmegen/picai_labels
+```
+
+After cloning the repository with annotations, you should have a folder structure like this:
+
+```bash
+/input/picai_labels
+├── anatomical_delineations
+│   ├── ...
+├── clinical_information
+│   └── marksheet.csv
+└── csPCa_lesion_delineations
+    ├── ...
 ```
 
 
 ### Cross-Validation Splits
 We have prepared 5-fold cross-validation splits of all 1500 cases in the [PI-CAI: Public Training and Development Dataset](https://pi-cai.grand-challenge.org/DATA/). We have ensured there is no patient overlap between training/validation splits. You can load these splits as follows:
 
 ```python
```

### Comparing `picai_baseline-0.8.2/setup.cfg` & `picai_baseline-0.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/setup.py` & `picai_baseline-0.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
-        version='0.8.2',
+        version='0.8.4',
         author_email='Joeran.Bosma@radboudumc.nl',
         long_description=long_description,
         long_description_content_type="text/markdown",
         url='https://github.com/DIAGNijmegen/picai_baseline',
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/picai_baseline/issues"
         },
```

### Comparing `picai_baseline-0.8.2/src/picai_baseline/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/__main__.py` & `picai_baseline-0.8.4/src/picai_baseline/__main__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/eval.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/eval.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/nnunet_baseline.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/nnunet_baseline.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/softmax_export.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/softmax_export.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/focal_loss.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/focal_loss.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/io.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/io.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_CE_checkpoints.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_CE_checkpoints.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_FL_and_CE.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_FL_and_CE.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_focalLoss.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_focalLoss.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/nnunet_wrapper.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnunet_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 
 def plan_train(argv):
     # Plan experiment, then train network
     parser = argparse.ArgumentParser()
     parser.add_argument('task', type=str)
     parser.add_argument('data', type=str)
     parser.add_argument('--results', type=str, required=False)
+    parser.add_argument('--prepdir', type=str, default=os.environ.get('prepdir', '/home/user/data'))
     parser.add_argument('--network', type=str, default='3d_fullres')
     parser.add_argument('--trainer', type=str, default='nnUNetTrainerV2')
     parser.add_argument('--trainer_kwargs', required=False, default="{}",
                         help="Use a dictionary in string format to specify keyword arguments. This will get"
                              " parsed into a dictionary, the values get correctly parsed to the data format"
                              " and passed to the trainer. Example (backslash included): \n"
                              r"--trainer_kwargs='{\"class_weights\":[0,2.00990337,1.42540704,2.13387239,0.85529504,0.592059,0.30040984,8.26874351],"
@@ -200,22 +201,25 @@
                         help='Export probability maps for ensembling during the final validation')
     parser.add_argument('--use_compressed_data', action='store_true',
                         help='Disable unpacking of compressed training data, use with caution')
     parser.add_argument('--plan_2d', action='store_true', help='Enable planning of 2D experiments')
     parser.add_argument('--dont_plan_3d', action='store_true', help='Disable planning of 3D experiments')
     parser.add_argument('--carbontracker', action='store_true', help='Enables tracking of energy consumption')
     parser.add_argument('--pretrained_weights', type=str, required=False, default=None)
+    parser.add_argument('--disable_validation_inference', required=False, action='store_true', 
+                        help="If set nnU-Net will not run inference on the validation set. This is useful if you are only interested in the test set results and want to save some disk space and time.")
+    parser.add_argument('--dont_copy_preprocessed_data', action='store_true', help="Don't copy preprocessed data to datadir")
     args = parser.parse_args(argv)
 
     # aid type hinting
     args.task = str(args.task)
 
     # Set environment variables
     datadir = Path(args.data)
-    prepdir = Path(os.environ.get('prepdir', '/home/user/data'))
+    prepdir = Path(args.prepdir)
 
     splits_file = prepdir / args.task / 'splits_final.pkl'
 
     os.environ['nnUNet_raw_data_base'] = str(datadir)
     os.environ['nnUNet_preprocessed'] = str(prepdir)
     os.environ['RESULTS_FOLDER'] = args.results if args.results else str(datadir / 'results')
 
@@ -255,35 +259,34 @@
                 '-tl', os.environ.get("nnUNet_tl", '8'), '-tf', os.environ.get("nnUNet_tf", '8'),
                 '--verify_dataset_integrity'
             ]
             if not args.plan_2d and '2d' not in args.network:
                 cmd.extend(['--planner2d', 'None'])  # disable 2D planning to speed up the preprocessing phase
             if args.dont_plan_3d and '3d' not in args.network:
                 cmd.extend(['--planner3d', 'None'])
-            if args.pretrained_weights is not None:
-                cmd.extend(['-pretrained_weights', args.pretrained_weights])
             subprocess.check_call(cmd)
 
             # Use a custom data split?
             if args.custom_split:
                 splits = []
                 for split in read_json(args.custom_split):
                     splits.append(OrderedDict([
                         ('train', np.array(split['train'])),
                         ('val', np.array(split['val']))
                     ]))
 
                 splits_file.parent.mkdir(parents=True, exist_ok=True)
                 with splits_file.open('wb') as fp:
                     pickle.dump(splits, fp)
-                shutil_sol.copyfile(args.custom_split, splits_file.with_suffix('.json'))
+                atomic_file_copy(args.custom_split, splits_file.with_suffix('.json'))
 
-            if (prepdir / args.task).absolute() != taskdir.absolute():
+            if (prepdir / args.task).absolute() != taskdir.absolute() and not args.dont_copy_preprocessed_data:
                 # Copy preprocessed data to storage server
-                print('[#] Copying plans and preprocessed data from compute node to storage server')
+                print('[#] Copying plans and preprocessed data from compute node to storage server' +
+                      f' ({taskdir} -> {prepdir / args.task})')
                 taskdir.parent.mkdir(parents=True, exist_ok=True)
                 shutil_sol.copytree(prepdir / args.task, taskdir)
 
         if args.plan_only:
             return
 
         # Run training
@@ -301,33 +304,38 @@
 
         if args.validation_only:
             print('[#] Running validation step only')
             cmd.append('--validation_only')
         elif path_exists(outdir) and any(outdir.glob("*.model")):
             print('[#] Resuming network training')
             cmd.append('-c')
+        elif args.pretrained_weights is not None:
+            print("Load pre-trained_model")
+            cmd.extend(['-pretrained_weights', args.pretrained_weights])
         else:
             print('[#] Starting network training')
 
         if args.trainer_kwargs:
             cmd.append('--trainer_kwargs=%s' % args.trainer_kwargs)
         if args.use_compressed_data:
             cmd.append('--use_compressed_data')
         if args.ensembling:
             cmd.append('--npz')
         if args.kwargs is not None:
             cmd.extend(args.kwargs.split(" "))
+        if args.disable_validation_inference:
+            cmd.append('--disable_validation_inference')
         print(f'[#] Running {" ".join(cmd)}')
 
         subprocess.check_call(cmd)
 
         # Copy split file since that is for sure available now (nnUNet_train has created
         # it if the file did not exist already - unless training with "all", so still check)
-        if splits_file.exists() and splits_file.parent.absolute() != taskdir.absolute():
-            shutil_sol.copyfile(splits_file, taskdir)
+        if splits_file.exists() and splits_file.parent.absolute() != taskdir.absolute() and taskdir.is_dir():
+            atomic_file_copy(splits_file, taskdir)
 
 
 def reveal_split(argv):
     # Print out the 5-fold cross validation split
     parser = argparse.ArgumentParser()
     parser.add_argument('task', type=str)
     parser.add_argument('data', type=str)
```

### Comparing `picai_baseline-0.8.2/src/picai_baseline/nnunet/training_docker/run_training.py` & `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/run_training.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/prepare_data.py` & `picai_baseline-0.8.4/src/picai_baseline/prepare_data.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/prepare_data_semi_supervised.py` & `picai_baseline-0.8.4/src/picai_baseline/prepare_data_semi_supervised.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-0.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-0.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-1.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-1.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-2.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-2.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-3.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-3.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-train-fold-4.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-4.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-0.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-0.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-1.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-1.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-2.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-2.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-3.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-3.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/ds-config-valid-fold-4.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-4.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai/splits.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_debug/splits.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_nnunet/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_nnunet/splits.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-0.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-0.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-1.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-1.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-2.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-2.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-3.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-3.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-4.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-4.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-0.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-0.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-1.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-1.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-2.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-2.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-3.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-3.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-4.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-4.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv/splits.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv_nnunet/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/splits/picai_pubpriv_nnunet/splits.json` & `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/plan_overview.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/plan_overview.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/train.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/train.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/multi_threaded_augmenter.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/multi_threaded_augmenter.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/nnUNet_DA.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/nnUNet_DA.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/single_threaded_augmenter.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/single_threaded_augmenter.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/augmentations/test_time_augmentations.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/test_time_augmentations.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/callbacks.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 import os
 import time
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import torch
-from picai_baseline.unet.training_setup.poly_lr import poly_lr
-from picai_eval import evaluate
+from picai_eval import Metrics
+from picai_eval.eval import evaluate_case
 from report_guided_annotation import extract_lesion_candidates
 from scipy.ndimage import gaussian_filter
 
+from picai_baseline.unet.training_setup.poly_lr import poly_lr
+
 
 def resume_or_restart_training(model, optimizer, device, args, fold_id):
     """Resume/restart training, based on whether checkpoint exists"""
 
     weights_file = Path(args.weights_dir) / f"{args.model_type}_F{fold_id}.pt"
     metrics_file = Path(args.weights_dir) / f"{args.model_type}_F{fold_id}_metrics.xlsx"
 
@@ -110,24 +112,24 @@
         try:
             inputs = batch_data['data'].to(device)
             labels = batch_data['seg'].to(device)
         except Exception:
             inputs = torch.from_numpy(batch_data['data']).to(device)
             labels = torch.from_numpy(batch_data['seg']).to(device)
         outputs = model(inputs)
-        loss = loss_func(outputs, labels[:, 0, ...].long())
+        loss = loss_func(outputs, labels)
         train_loss += loss.item()
 
         # backpropagate + optimize
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
 
         # define each training epoch == 100 steps (note: nnU-Net uses 250 steps)
-        if step >= 100: 
+        if step >= 100:
             break
 
     # update learning rate
     updated_lr = poly_lr(epoch+1, args.num_epochs, args.base_lr, 0.95)
     optimizer.param_groups[0]['lr'] = updated_lr
     print("Learning Rate Updated! New Value: "+str(np.round(updated_lr, 10)), flush=True)
 
@@ -141,26 +143,26 @@
 
     return model, optimizer, train_gen, tracking_metrics, writer
 
 
 def validate_model(model, optimizer, valid_gen, args, tracking_metrics, device, writer):
     """Validate model per N epoch + export model weights"""
 
-    all_valid_preds, all_valid_labels = [], []
     epoch, f = tracking_metrics['epoch'], tracking_metrics['fold_id']
 
     # for each validation sample
+    lesion_results = []
     for valid_data in valid_gen:
 
         try:
             valid_images = valid_data['data'].to(device)
             valid_labels = valid_data['seg']
         except Exception:
             valid_images = torch.from_numpy(valid_data['data']).to(device)
-            valid_labels = torch.from_numpy(valid_data['seg'])
+            valid_labels = valid_data['seg']
 
         # test-time augmentation
         valid_images = [valid_images, torch.flip(valid_images, [4]).to(device)]
 
         # aggregate all validation predictions
         # gaussian blur to counteract checkerboard artifacts in
         # predictions from the use of transposed conv. in the U-Net
@@ -170,31 +172,41 @@
         ]
 
         # revert horizontally flipped tta image
         preds[1] = np.flip(preds[1], [3])
 
         # gaussian blur to counteract checkerboard artifacts in
         # predictions from the use of transposed conv. in the U-Net
-        all_valid_preds += [
-            np.mean([
-                gaussian_filter(x, sigma=1.5)
-                for x in preds
-            ], axis=0)
+        preds = np.mean([
+            gaussian_filter(x, sigma=1.5)
+            for x in preds
+        ], axis=0)
+    
+        # extract lesion candidates
+        preds = [
+            extract_lesion_candidates(x)[0] 
+            for x in preds
         ]
-        all_valid_labels += [valid_labels.numpy()[:, 0, ...]]
+
+        # evaluate detection maps of batch
+        for y_det, y_true in zip(preds, valid_labels):
+            y_list, *_ = evaluate_case(
+                y_det=y_det,
+                y_true=y_true.squeeze(),
+            )
+
+            # aggregate all validation evaluations
+            lesion_results.append(y_list)
 
     # track validation metrics
-    valid_metrics = evaluate(y_det=iter(np.concatenate([x for x in np.array(all_valid_preds)], axis=0)),
-                             y_true=iter(np.concatenate([x for x in np.array(all_valid_labels)], axis=0)),
-                             y_det_postprocess_func=lambda pred: extract_lesion_candidates(pred)[0])
-
-    num_pos = int(np.sum([np.max(y) for y in np.concatenate(
-        [x for x in np.array(all_valid_labels)], axis=0)]))
-    num_neg = int(len(np.concatenate([x for x in
-                                      np.array(all_valid_labels)], axis=0)) - num_pos)
+    lesion_results = {idx: result for idx, result in enumerate(lesion_results)}
+    valid_metrics = Metrics(lesion_results)
+
+    num_pos = sum([y == 1 for y in valid_metrics.case_target.values()])
+    num_neg = sum([y == 0 for y in valid_metrics.case_target.values()])
 
     tracking_metrics['all_epochs'].append(epoch+1)
     tracking_metrics['all_train_loss'].append(tracking_metrics['train_loss'])
     tracking_metrics['all_valid_metrics_auroc'].append(valid_metrics.auroc)
     tracking_metrics['all_valid_metrics_ap'].append(valid_metrics.AP)
     tracking_metrics['all_valid_metrics_ranking'].append(valid_metrics.score)
 
@@ -206,15 +218,15 @@
                                         tracking_metrics['all_valid_metrics_ranking'])),
                                columns=['epoch', 'train_loss', 'valid_auroc', 'valid_ap', 'valid_ranking'])
 
     # create target folder and save exports sheet
     os.makedirs(args.weights_dir, exist_ok=True)
 
     metrics_file = Path(args.weights_dir) / f"{args.model_type}_F{f}_metrics.xlsx"
-    metricsData.to_excel(metrics_file, encoding='utf-8', index=False)
+    metricsData.to_excel(metrics_file, index=False)
 
     writer.add_scalar("valid_auroc",   valid_metrics.auroc, epoch+1)
     writer.add_scalar("valid_ap",      valid_metrics.AP,    epoch+1)
     writer.add_scalar("valid_ranking", valid_metrics.score, epoch+1)
 
     print(f"Valid. Performance [Benign or Indolent PCa (n={num_neg}) \
         vs. csPCa (n={num_pos})]:\nRanking Score = {valid_metrics.score:.3f},\
```

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/compute_spec.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/compute_spec.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/data_generator.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/data_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 
 import monai
 import numpy as np
 import torch
 from batchgenerators.dataloading.data_loader import DataLoader
 from monai.transforms import Compose, EnsureType
+
 from picai_baseline.unet.training_setup.image_reader import SimpleITKDataset
 
 
 def default_collate(batch):
     """collate multiple samples into batches, if needed"""
 
     if isinstance(batch[0], np.ndarray):
@@ -117,10 +118,10 @@
     train_ds = SimpleITKDataset(image_files=train_data[0], seg_files=train_data[1],
                                 transform=Compose(pretx),  seg_transform=Compose(pretx))
     valid_ds = SimpleITKDataset(image_files=valid_data[0], seg_files=valid_data[1],
                                 transform=Compose(pretx),  seg_transform=Compose(pretx))
     train_ldr = DataLoaderFromDataset(train_ds, 
         batch_size=args.batch_size, num_threads=args.num_threads, infinite=True, shuffle=True)
     valid_ldr = DataLoaderFromDataset(valid_ds, 
-        batch_size=args.batch_size, num_threads=1, infinite=False, shuffle=False)
+        batch_size=args.batch_size, num_threads=args.num_threads, infinite=False, shuffle=False)
 
     return train_ldr, valid_ldr, class_weights.astype(np.float32)
```

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/default_hyperparam.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/default_hyperparam.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/image_reader.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/image_reader.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/loss_functions/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/loss_functions/focal.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/focal.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,19 +28,19 @@
         self.reduction = reduction
 
     def forward(self, inputs, targets):
         inputs = torch.sigmoid(inputs)
         targets = F.one_hot(targets, num_classes=self.num_classes).float()
         targets = torch.moveaxis(targets, (0, 1, 2, 3, 4), (0, 2, 3, 4, 1))
         ce_loss = F.binary_cross_entropy(inputs, targets, reduction="none")
-        p_t = (inputs[-1] * targets[-1]) + ((1 - inputs[-1]) * (1 - targets[-1]))
+        p_t = (inputs * targets) + ((1 - inputs) * (1 - targets))
         loss = ce_loss * ((1 - p_t) ** self.gamma)
 
         if self.alpha >= 0:
-            alpha_t = self.alpha * targets[-1] + (1 - self.alpha) * (1 - targets[-1])
+            alpha_t = self.alpha * targets + (1 - self.alpha) * (1 - targets)
             loss = alpha_t * loss
 
         if self.reduction == "mean":
             loss = loss.mean()
         elif self.reduction == "sum":
             loss = loss.sum()
```

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/neural_network_selector.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_network_selector.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/neural_networks/__init__.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/neural_networks/unets.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/unets.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/poly_lr.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/poly_lr.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline/unet/training_setup/preprocess_utils.py` & `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/preprocess_utils.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/src/picai_baseline.egg-info/PKG-INFO` & `picai_baseline-0.8.4/src/picai_baseline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picai-baseline
-Version: 0.8.2
+Version: 0.8.4
 Summary: PICAI Baselines
 Home-page: https://github.com/DIAGNijmegen/picai_baseline
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/picai_baseline/issues
 Platform: unix
@@ -59,15 +59,15 @@
 We define setup steps that are shared between the different baseline algorithms. To follow the baseline algorithm tutorials, this setup must be completed first.
 
 
 ### Folder Structure
 We define three main folders that must be prepared apriori:
 - `/input/` contains one of the [PI-CAI datasets](https://pi-cai.grand-challenge.org/DATA/). This can be the Public Training and Development Dataset, the Private Training Dataset, the Hidden Validation and Tuning Cohort, or the Hidden Testing Cohort.
   - `/input/images/` contains the imaging files. For the Public Training and Development Dataset, these can be retrieved [here](https://zenodo.org/record/6624726).
-  - `/input/labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
+  - `/input/picai_labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
 - `/workdir/` stores intermediate results, such as preprocessed images and annotations.
   - `/workdir/results/[model name]/` stores model checkpoints/weights during training (enables the ability to pause/resume training).    
 - `/output/` stores training output, such as trained model weights and preprocessing plan.
 
 
 ### Data Preparation
 Unless specified otherwise, this tutorial assumes that the [PI-CAI: Public Training and Development Dataset](https://pi-cai.grand-challenge.org/DATA/) will be downloaded and unpacked. Before downloading the dataset, read its [documentation](https://zenodo.org/record/6624726) and [dedicated forum post](https://grand-challenge.org/forums/forum/pi-cai-607/topic/public-training-and-development-dataset-updates-and-fixes-631/) (for all updates/fixes, if any). To download and unpack the dataset, run the following commands:
@@ -96,18 +96,31 @@
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold2.zip -d /input/images/
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold3.zip -d /input/images/
 docker run --cpus=2 --memory=8gb --rm -v /path/to/input:/input joeranbosma/picai_nnunet:latest unzip /input/picai_public_images_fold4.zip -d /input/images/
 ```
 
 Please follow the [instructions here](nnunet_baseline.md#nnu-net---docker-setup) to set up the Docker container.
 
-Also, collect the training annotations via the following command:
+Also, collect the training annotations. This can be done via the following command:
 
 ```bash
-git clone https://github.com/DIAGNijmegen/picai_labels /input/labels/
+cd /input
+git clone https://github.com/DIAGNijmegen/picai_labels
+```
+
+After cloning the repository with annotations, you should have a folder structure like this:
+
+```bash
+/input/picai_labels
+├── anatomical_delineations
+│   ├── ...
+├── clinical_information
+│   └── marksheet.csv
+└── csPCa_lesion_delineations
+    ├── ...
 ```
 
 
 ### Cross-Validation Splits
 We have prepared 5-fold cross-validation splits of all 1500 cases in the [PI-CAI: Public Training and Development Dataset](https://pi-cai.grand-challenge.org/DATA/). We have ensured there is no patient overlap between training/validation splits. You can load these splits as follows:
 
 ```python
```

### Comparing `picai_baseline-0.8.2/src/picai_baseline.egg-info/SOURCES.txt` & `picai_baseline-0.8.4/src/picai_baseline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.2/tests/test_splits.py` & `picai_baseline-0.8.4/tests/test_splits.py`

 * *Files identical despite different names*

