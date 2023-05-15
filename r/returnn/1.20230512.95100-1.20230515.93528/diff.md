# Comparing `tmp/returnn-1.20230512.95100.tar.gz` & `tmp/returnn-1.20230515.93528.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230512.95100.tar", last modified: Fri May 12 08:07:35 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230515.93528.tar", last modified: Mon May 15 08:06:02 2023, max compression
```

## Comparing `returnn-1.20230512.95100.tar` & `returnn-1.20230515.93528.tar`

### file list

```diff
@@ -1,444 +1,444 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 08:07:10.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-12 08:07:12.000000 returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39412 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99004 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157297 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151443 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37861 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   585402 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67246 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551354 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/dump-pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/export_to_onnx.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:07:35.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-12 08:07:08.000000 returnn-1.20230512.95100/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 08:05:38.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-15 08:05:40.000000 returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39412 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157297 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151443 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37861 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   585402 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67314 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551354 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/dump-pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/export_to_onnx.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:06:02.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-15 08:05:37.000000 returnn-1.20230515.93528/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230512.95100/.gitignore` & `returnn-1.20230515.93528/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/.gitmodules` & `returnn-1.20230515.93528/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/CHANGELOG.md` & `returnn-1.20230515.93528/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/CODEOWNERS` & `returnn-1.20230515.93528/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/CONTRIBUTING.md` & `returnn-1.20230515.93528/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/LICENSE` & `returnn-1.20230515.93528/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/MANIFEST.in` & `returnn-1.20230515.93528/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/PKG-INFO` & `returnn-1.20230515.93528/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230512.95100
+Version: 1.20230515.93528
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230512.95100/README.rst` & `returnn-1.20230515.93528/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/__init__.py` & `returnn-1.20230515.93528/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/12AX.cluster_map` & `returnn-1.20230515.93528/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-fwd.config` & `returnn-1.20230515.93528/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-horovod-mpi.py` & `returnn-1.20230515.93528/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230515.93528/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-hyper-param-tuning.config` & `returnn-1.20230515.93528/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-iter-dataset.py` & `returnn-1.20230515.93528/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-list-devices.py` & `returnn-1.20230515.93528/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-lua-torch-layer.config` & `returnn-1.20230515.93528/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230515.93528/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-returnn-as-framework.py` & `returnn-1.20230515.93528/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-rf.config` & `returnn-1.20230515.93528/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-rhn-enwik8.config` & `returnn-1.20230515.93528/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-sprint-interface.py` & `returnn-1.20230515.93528/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-att-copy.config` & `returnn-1.20230515.93528/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-attention.config` & `returnn-1.20230515.93528/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230515.93528/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230515.93528/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-enc-dec.config` & `returnn-1.20230515.93528/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230515.93528/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230515.93528/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230515.93528/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230515.93528/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230515.93528/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230515.93528/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230515.93528/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230515.93528/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230515.93528/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230515.93528/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-rec-self-att.config` & `returnn-1.20230515.93528/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230515.93528/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230515.93528/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230515.93528/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-torch.config` & `returnn-1.20230515.93528/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230515.93528/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/demo.sh` & `returnn-1.20230515.93528/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230515.93528/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230515.93528/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230515.93528/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/README.txt` & `returnn-1.20230515.93528/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/config_demo` & `returnn-1.20230515.93528/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230515.93528/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/config_real` & `returnn-1.20230515.93528/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230515.93528/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/decode.py` & `returnn-1.20230515.93528/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230515.93528/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230515.93528/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230515.93528/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230515.93528/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230515.93528/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230515.93528/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230515.93528/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230515.93528/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230515.93528/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230515.93528/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/__init__.py` & `returnn-1.20230515.93528/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/__main__.py` & `returnn-1.20230515.93528/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/__old_mod_loader__.py` & `returnn-1.20230515.93528/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/__setup__.py` & `returnn-1.20230515.93528/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/config.py` & `returnn-1.20230515.93528/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/audio.py` & `returnn-1.20230515.93528/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/basic.py` & `returnn-1.20230515.93528/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/bundle_file.py` & `returnn-1.20230515.93528/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/cached.py` & `returnn-1.20230515.93528/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/cached2.py` & `returnn-1.20230515.93528/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/generating.py` & `returnn-1.20230515.93528/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/hdf.py` & `returnn-1.20230515.93528/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/lm.py` & `returnn-1.20230515.93528/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/map.py` & `returnn-1.20230515.93528/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/meta.py` & `returnn-1.20230515.93528/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/multi_proc.py` & `returnn-1.20230515.93528/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/normalization_data.py` & `returnn-1.20230515.93528/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/numpy_dump.py` & `returnn-1.20230515.93528/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/raw_wav.py` & `returnn-1.20230515.93528/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/sprint.py` & `returnn-1.20230515.93528/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/stereo.py` & `returnn-1.20230515.93528/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230515.93528/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/datasets/util/vocabulary.py` & `returnn-1.20230515.93528/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/engine/base.py` & `returnn-1.20230515.93528/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/engine/batch.py` & `returnn-1.20230515.93528/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230515.93528/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230515.93528/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230515.93528/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230515.93528/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/graph_editor/edit.py` & `returnn-1.20230515.93528/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230515.93528/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/graph_editor/select.py` & `returnn-1.20230515.93528/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230515.93528/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/graph_editor/transform.py` & `returnn-1.20230515.93528/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/extern/graph_editor/util.py` & `returnn-1.20230515.93528/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/__init__.py` & `returnn-1.20230515.93528/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/_backend.py` & `returnn-1.20230515.93528/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/_numpy_backend.py` & `returnn-1.20230515.93528/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/_utils.py` & `returnn-1.20230515.93528/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/array_.py` & `returnn-1.20230515.93528/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/attention.py` & `returnn-1.20230515.93528/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/cond.py` & `returnn-1.20230515.93528/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/const.py` & `returnn-1.20230515.93528/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/container.py` & `returnn-1.20230515.93528/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/conv.py` & `returnn-1.20230515.93528/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/device.py` & `returnn-1.20230515.93528/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/dims.py` & `returnn-1.20230515.93528/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/dropout.py` & `returnn-1.20230515.93528/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/dtype.py` & `returnn-1.20230515.93528/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/encoder/base.py` & `returnn-1.20230515.93528/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/encoder/conformer.py` & `returnn-1.20230515.93528/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/init.py` & `returnn-1.20230515.93528/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/linear.py` & `returnn-1.20230515.93528/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/loop.py` & `returnn-1.20230515.93528/returnn/frontend/loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,19 +77,19 @@
 def scan(
     *,
     spatial_dim: Optional[Dim] = None,
     cond_dims: Optional[Sequence[Dim]] = None,
     initial: S = None,
     xs: X = None,
     ys: Y = None,
-    cond: Optional[Callable[[S, X], Tensor]] = None,
-    body: Callable[[S, X], Tuple[S, Y]],
+    cond: Optional[Callable[[X, S], Tensor]] = None,
+    body: Callable[[X, S], Tuple[Y, S]],
     max_seq_len: Optional[int] = None,
     return_tensor_arrays: bool = False,
-) -> Tuple[S, Y, Dim]:
+) -> Tuple[Y, S, Dim]:
     """
     Extended variant of :func:`while_loop`.
 
     Supports iterating over a given axis (spatial_dim),
     supports iterating over some input tensors (xs: X) on the given axis,
     and supports returning some frame-accumulated output tensors (ys: Y).
 
@@ -109,15 +109,15 @@
     :param body:
     :param max_seq_len: If given, it is checked in addition to `cond`, and when reached, it stops the loop.
     :param return_tensor_arrays: if True, will return TensorArray instead of Tensor for ys.
         Internally, we work with TensorArray anyway, so this avoids the final stack().
         In case of beam search, it might make more sense
         to perform some post-processing on the TensorArray per entry,
         like selecting the right beam entries.
-    :return: final state, outputs ys, and the new spatial_dim
+    :return: outputs ys, final state, and the new spatial_dim
     """
     if spatial_dim is None or not spatial_dim.is_dim_known():
         assert cond is not None, f"scan: spatial_dim {spatial_dim} is None/unknown, need to provide `end`"
         assert xs is None, f"scan: spatial_dim {spatial_dim} is None/unknown, cannot use input `xs` {xs}"
         if spatial_dim is None:
             spatial_dim = Dim(None, name="scan_dim")
 
@@ -127,22 +127,22 @@
             if max_seq_len is not None:
                 c = rf.logical_and(c, i < max_seq_len)
             return c
 
         def _body(_s: Tuple[Tensor, Tensor, Tensor, S, Y]) -> Tuple[Tensor, Tensor, Tensor, S, Y]:
             i, seq_len_, prev_cond, s, ys_ = _s
             seq_len_ = seq_len_ + rf.cast(prev_cond, dtype=seq_len_.dtype)
-            s, y = body(s, None)
+            y, s = body(None, s)
             tree.assert_same_structure(ys_, y)
             ys_ = tree.map_structure(lambda ys__, y_: ys__.push_back(y_), ys_, y)
-            c = cond(s, None)
+            c = cond(None, s)
             c = rf.logical_and(c, prev_cond)
             return i + 1, seq_len_, c, s, ys_
 
-        initial_cond = cond(initial, None)
+        initial_cond = cond(None, initial)
         assert (
             isinstance(initial_cond, Tensor)
             and initial_cond.dtype == "bool"
             and initial_cond.dims_set == set(cond_dims)
         )
         _, seq_len, _, final_s, ys = while_loop(
             _cond,
@@ -166,15 +166,15 @@
 
         def _cond(_s: Tuple[Tensor, S, Y]) -> Tensor:
             i, *_ = _s
             return i < spatial_dim.get_dim_value_tensor()
 
         def _body(_s: Tuple[Tensor, S, Y]) -> Tuple[Tensor, S, Y]:
             i, s, ys_ = _s
-            s, y = body(s, tree.map_structure(lambda x: x[i], xs))
+            y, s = body(tree.map_structure(lambda x: x[i], xs), s)
             tree.assert_same_structure(ys_, y)
             ys_ = tree.map_structure(lambda ys__, y_: ys__.push_back(y_), ys_, y)
             return i + 1, s, ys_
 
         _, final_s, ys = while_loop(
             _cond,
             _body,
@@ -183,8 +183,8 @@
                 initial,  # state
                 tree.map_structure(lambda y: TensorArray(y), ys),
             ),
         )
 
     if not return_tensor_arrays:
         ys = tree.map_structure(lambda ys_: ys_.stack(axis=spatial_dim), ys)
-    return final_s, ys, spatial_dim
+    return ys, final_s, spatial_dim
```

### Comparing `returnn-1.20230512.95100/returnn/frontend/loss.py` & `returnn-1.20230515.93528/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/math_.py` & `returnn-1.20230515.93528/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/matmul.py` & `returnn-1.20230515.93528/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/module.py` & `returnn-1.20230515.93528/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/normalization.py` & `returnn-1.20230515.93528/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/parameter.py` & `returnn-1.20230515.93528/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/rand.py` & `returnn-1.20230515.93528/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/reduce.py` & `returnn-1.20230515.93528/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/run_ctx.py` & `returnn-1.20230515.93528/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/signal.py` & `returnn-1.20230515.93528/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/state.py` & `returnn-1.20230515.93528/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/tensor_array.py` & `returnn-1.20230515.93528/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/frontend/types.py` & `returnn-1.20230515.93528/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/import_/common.py` & `returnn-1.20230515.93528/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/import_/git.py` & `returnn-1.20230515.93528/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/import_/import_.py` & `returnn-1.20230515.93528/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/learning_rate_control.py` & `returnn-1.20230515.93528/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/log.py` & `returnn-1.20230515.93528/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/native_op.cpp` & `returnn-1.20230515.93528/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/native_op.py` & `returnn-1.20230515.93528/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/pretrain.py` & `returnn-1.20230515.93528/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/sprint/cache.py` & `returnn-1.20230515.93528/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/sprint/control.py` & `returnn-1.20230515.93528/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/sprint/error_signals.py` & `returnn-1.20230515.93528/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/sprint/extern_interface.py` & `returnn-1.20230515.93528/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/sprint/interface.py` & `returnn-1.20230515.93528/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/_dim_extra.py` & `returnn-1.20230515.93528/returnn/tensor/_dim_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -2381,3808 +2381,3841 @@
 000094c0: 206e 6f74 2073 697a 655f 6474 7970 653a   not size_dtype:
 000094d0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
 000094e0: 655f 6474 7970 6520 3d20 5f74 2e54 656e  e_dtype = _t.Ten
 000094f0: 736f 722e 7369 7a65 5f64 7479 7065 0a0a  sor.size_dtype..
 00009500: 2020 2020 2020 2020 696d 706f 7274 206e          import n
 00009510: 756d 7079 0a20 2020 2020 2020 2069 6d70  umpy.        imp
 00009520: 6f72 7420 7265 7475 726e 6e2e 6672 6f6e  ort returnn.fron
-00009530: 7465 6e64 2061 7320 7266 0a20 2020 2020  tend as rf.     
-00009540: 2020 2066 726f 6d20 7265 7475 726e 6e2e     from returnn.
-00009550: 7465 6e73 6f72 2069 6d70 6f72 7420 5465  tensor import Te
-00009560: 6e73 6f72 0a0a 2020 2020 2020 2020 7466  nsor..        tf
-00009570: 203d 2074 665f 7574 696c 203d 2074 656e   = tf_util = ten
-00009580: 736f 725f 7574 696c 203d 204e 6f6e 650a  sor_util = None.
-00009590: 2020 2020 2020 2020 6966 2062 6163 6b65          if backe
-000095a0: 6e64 2061 6e64 2062 6163 6b65 6e64 2e69  nd and backend.i
-000095b0: 735f 7465 6e73 6f72 666c 6f77 3a0a 2020  s_tensorflow:.  
-000095c0: 2020 2020 2020 2020 2020 696d 706f 7274            import
-000095d0: 2074 656e 736f 7266 6c6f 7720 6173 2074   tensorflow as t
-000095e0: 660a 0a20 2020 2020 2020 2020 2020 2069  f..            i
-000095f0: 6620 6261 636b 656e 642e 5261 7754 656e  f backend.RawTen
-00009600: 736f 7254 7970 6520 3d3d 2074 662e 5465  sorType == tf.Te
-00009610: 6e73 6f72 3a0a 2020 2020 2020 2020 2020  nsor:.          
-00009620: 2020 2020 2020 6672 6f6d 2072 6574 7572        from retur
-00009630: 6e6e 2e74 662e 7574 696c 2069 6d70 6f72  nn.tf.util impor
-00009640: 7420 6261 7369 6320 6173 2074 665f 7574  t basic as tf_ut
-00009650: 696c 0a20 2020 2020 2020 2020 2020 2020  il.             
-00009660: 2020 2066 726f 6d20 7465 6e73 6f72 666c     from tensorfl
-00009670: 6f77 2e70 7974 686f 6e2e 6672 616d 6577  ow.python.framew
-00009680: 6f72 6b20 696d 706f 7274 2074 656e 736f  ork import tenso
-00009690: 725f 7574 696c 0a20 2020 2020 2020 2020  r_util.         
-000096a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000096b0: 2020 2020 2020 2020 2074 6620 3d20 4e6f           tf = No
-000096c0: 6e65 0a0a 2020 2020 2020 2020 6b69 6e64  ne..        kind
-000096d0: 203d 206f 702e 6b69 6e64 0a20 2020 2020   = op.kind.     
-000096e0: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
-000096f0: 6974 6828 225f 7269 6768 7422 293a 0a20  ith("_right"):. 
-00009700: 2020 2020 2020 2020 2020 206b 696e 6420             kind 
-00009710: 3d20 6b69 6e64 5b3a 202d 6c65 6e28 225f  = kind[: -len("_
-00009720: 7269 6768 7422 295d 2020 2320 6f72 6465  right")]  # orde
-00009730: 7220 646f 6573 206e 6f74 206d 6174 7465  r does not matte
-00009740: 7220 6865 7265 0a20 2020 2020 2020 2069  r here.        i
-00009750: 6620 6b69 6e64 2e65 6e64 7377 6974 6828  f kind.endswith(
-00009760: 225f 6c65 6674 2229 3a0a 2020 2020 2020  "_left"):.      
-00009770: 2020 2020 2020 6b69 6e64 203d 206b 696e        kind = kin
-00009780: 645b 3a20 2d6c 656e 2822 5f6c 6566 7422  d[: -len("_left"
-00009790: 295d 0a0a 2020 2020 2020 2020 6465 6620  )]..        def 
-000097a0: 5f69 735f 6e65 6761 7469 7665 2878 5f5f  _is_negative(x__
-000097b0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-000097c0: 6620 6973 696e 7374 616e 6365 2878 5f5f  f isinstance(x__
-000097d0: 2c20 6e75 6d70 792e 6e64 6172 7261 7929  , numpy.ndarray)
-000097e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000097f0: 2020 7265 7475 726e 2028 785f 5f20 3c20    return (x__ < 
-00009800: 3029 2e61 6e79 2829 0a20 2020 2020 2020  0).any().       
-00009810: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00009820: 6365 2878 5f5f 2c20 2869 6e74 2c20 666c  ce(x__, (int, fl
-00009830: 6f61 742c 206e 756d 7079 2e6e 756d 6265  oat, numpy.numbe
-00009840: 7229 293a 0a20 2020 2020 2020 2020 2020  r)):.           
-00009850: 2020 2020 2072 6574 7572 6e20 785f 5f20       return x__ 
-00009860: 3c20 300a 2020 2020 2020 2020 2020 2020  < 0.            
-00009870: 6966 206e 6f74 2074 663a 0a20 2020 2020  if not tf:.     
-00009880: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009890: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-000098a0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-000098b0: 7461 6e63 6528 785f 5f2c 2074 662e 5465  tance(x__, tf.Te
-000098c0: 6e73 6f72 290a 2020 2020 2020 2020 2020  nsor).          
-000098d0: 2020 785f 5f20 3d20 7465 6e73 6f72 5f75    x__ = tensor_u
-000098e0: 7469 6c2e 636f 6e73 7461 6e74 5f76 616c  til.constant_val
-000098f0: 7565 2878 5f5f 290a 2020 2020 2020 2020  ue(x__).        
-00009900: 2020 2020 6966 2078 5f5f 2069 7320 6e6f      if x__ is no
-00009910: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00009920: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00009930: 6973 5f6e 6567 6174 6976 6528 785f 5f29  is_negative(x__)
-00009940: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00009950: 7572 6e20 4661 6c73 650a 0a20 2020 2020  urn False..     
-00009960: 2020 2064 6566 205f 6269 6e5f 6f70 5f74     def _bin_op_t
-00009970: 6628 612c 2062 293a 0a20 2020 2020 2020  f(a, b):.       
-00009980: 2020 2020 2069 6620 7465 6d70 6c61 7465       if template
-00009990: 5f6f 6e6c 793a 0a20 2020 2020 2020 2020  _only:.         
-000099a0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-000099b0: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
-000099c0: 6620 6120 6973 204e 6f6e 6520 6f72 2062  f a is None or b
-000099d0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000099e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000099f0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00009a00: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00009a10: 6e63 6528 612c 2074 662e 5465 6e73 6f72  nce(a, tf.Tensor
-00009a20: 2920 616e 6420 6973 696e 7374 616e 6365  ) and isinstance
-00009a30: 2862 2c20 2869 6e74 2c20 7466 2e54 656e  (b, (int, tf.Ten
-00009a40: 736f 7229 290a 2020 2020 2020 2020 2020  sor)).          
-00009a50: 2020 7769 7468 2074 665f 7574 696c 2e73    with tf_util.s
-00009a60: 616d 655f 636f 6e74 726f 6c5f 666c 6f77  ame_control_flow
-00009a70: 5f63 7478 285b 612c 2062 5d29 3a0a 2020  _ctx([a, b]):.  
-00009a80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00009a90: 206b 696e 6420 3d3d 2022 6164 6422 3a0a   kind == "add":.
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 7573 655f 7265 6c75 203d 205f      use_relu = _
-00009ac0: 6973 5f6e 6567 6174 6976 6528 6129 206f  is_negative(a) o
-00009ad0: 7220 5f69 735f 6e65 6761 7469 7665 2862  r _is_negative(b
-00009ae0: 2920 2023 2066 6f72 2064 796e 616d 6963  )  # for dynamic
-00009af0: 2074 656e 736f 7273 2c20 6173 7375 6d65   tensors, assume
-00009b00: 2061 6c6c 2070 6f73 6974 6976 650a 2020   all positive.  
-00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b20: 2020 6966 2075 7365 5f72 656c 753a 0a20    if use_relu:. 
-00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b40: 2020 2020 2020 2072 6574 7572 6e20 7466         return tf
-00009b50: 2e63 6f6e 7665 7274 5f74 6f5f 7465 6e73  .convert_to_tens
-00009b60: 6f72 2874 665f 7574 696c 2e73 696d 706c  or(tf_util.simpl
-00009b70: 6966 795f 6e6f 6e5f 6e65 6761 7469 7665  ify_non_negative
-00009b80: 5f73 6571 5f6c 656e 6774 6828 6120 2b20  _seq_length(a + 
-00009b90: 6229 290a 2020 2020 2020 2020 2020 2020  b)).            
-00009ba0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00009bb0: 202b 2062 0a20 2020 2020 2020 2020 2020   + b.           
-00009bc0: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
-00009bd0: 3d20 2273 7562 223a 0a20 2020 2020 2020  = "sub":.       
-00009be0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00009bf0: 7572 6e20 7466 2e63 6f6e 7665 7274 5f74  urn tf.convert_t
-00009c00: 6f5f 7465 6e73 6f72 2874 665f 7574 696c  o_tensor(tf_util
-00009c10: 2e73 696d 706c 6966 795f 6e6f 6e5f 6e65  .simplify_non_ne
-00009c20: 6761 7469 7665 5f73 6571 5f6c 656e 6774  gative_seq_lengt
-00009c30: 6828 6120 2d20 6229 290a 2020 2020 2020  h(a - b)).      
-00009c40: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
-00009c50: 696e 6420 3d3d 2022 6d75 6c22 3a0a 2020  ind == "mul":.  
-00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c70: 2020 7265 7475 726e 2061 202a 2062 0a20    return a * b. 
-00009c80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00009c90: 6c69 6620 6b69 6e64 2069 6e20 2822 666c  lif kind in ("fl
-00009ca0: 6f6f 7264 6976 222c 2022 7472 7565 6469  oordiv", "truedi
-00009cb0: 7622 293a 2020 2320 7472 7565 6469 7620  v"):  # truediv 
-00009cc0: 6173 7375 6d65 7320 7468 6572 6520 6973  assumes there is
-00009cd0: 206e 6f20 7265 6d61 696e 6465 720a 2020   no remainder.  
-00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cf0: 2020 7265 7475 726e 2061 202f 2f20 620a    return a // b.
+00009530: 7465 6e64 2061 7320 7266 0a0a 2020 2020  tend as rf..    
+00009540: 2020 2020 7466 203d 2074 665f 7574 696c      tf = tf_util
+00009550: 203d 2074 656e 736f 725f 7574 696c 203d   = tensor_util =
+00009560: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+00009570: 2062 6163 6b65 6e64 2061 6e64 2062 6163   backend and bac
+00009580: 6b65 6e64 2e69 735f 7465 6e73 6f72 666c  kend.is_tensorfl
+00009590: 6f77 3a0a 2020 2020 2020 2020 2020 2020  ow:.            
+000095a0: 696d 706f 7274 2074 656e 736f 7266 6c6f  import tensorflo
+000095b0: 7720 6173 2074 660a 0a20 2020 2020 2020  w as tf..       
+000095c0: 2020 2020 2069 6620 6261 636b 656e 642e       if backend.
+000095d0: 5261 7754 656e 736f 7254 7970 6520 3d3d  RawTensorType ==
+000095e0: 2074 662e 5465 6e73 6f72 3a0a 2020 2020   tf.Tensor:.    
+000095f0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
+00009600: 2072 6574 7572 6e6e 2e74 662e 7574 696c   returnn.tf.util
+00009610: 2069 6d70 6f72 7420 6261 7369 6320 6173   import basic as
+00009620: 2074 665f 7574 696c 0a20 2020 2020 2020   tf_util.       
+00009630: 2020 2020 2020 2020 2066 726f 6d20 7465           from te
+00009640: 6e73 6f72 666c 6f77 2e70 7974 686f 6e2e  nsorflow.python.
+00009650: 6672 616d 6577 6f72 6b20 696d 706f 7274  framework import
+00009660: 2074 656e 736f 725f 7574 696c 0a20 2020   tensor_util.   
+00009670: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00009680: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00009690: 6620 3d20 4e6f 6e65 0a0a 2020 2020 2020  f = None..      
+000096a0: 2020 6b69 6e64 203d 206f 702e 6b69 6e64    kind = op.kind
+000096b0: 0a20 2020 2020 2020 2069 6620 6b69 6e64  .        if kind
+000096c0: 2e65 6e64 7377 6974 6828 225f 7269 6768  .endswith("_righ
+000096d0: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
+000096e0: 206b 696e 6420 3d20 6b69 6e64 5b3a 202d   kind = kind[: -
+000096f0: 6c65 6e28 225f 7269 6768 7422 295d 2020  len("_right")]  
+00009700: 2320 6f72 6465 7220 646f 6573 206e 6f74  # order does not
+00009710: 206d 6174 7465 7220 6865 7265 0a20 2020   matter here.   
+00009720: 2020 2020 2069 6620 6b69 6e64 2e65 6e64       if kind.end
+00009730: 7377 6974 6828 225f 6c65 6674 2229 3a0a  swith("_left"):.
+00009740: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
+00009750: 203d 206b 696e 645b 3a20 2d6c 656e 2822   = kind[: -len("
+00009760: 5f6c 6566 7422 295d 0a0a 2020 2020 2020  _left")]..      
+00009770: 2020 6465 6620 5f69 735f 6e65 6761 7469    def _is_negati
+00009780: 7665 2878 5f5f 293a 0a20 2020 2020 2020  ve(x__):.       
+00009790: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000097a0: 6365 2878 5f5f 2c20 6e75 6d70 792e 6e64  ce(x__, numpy.nd
+000097b0: 6172 7261 7929 3a0a 2020 2020 2020 2020  array):.        
+000097c0: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+000097d0: 785f 5f20 3c20 3029 2e61 6e79 2829 0a20  x__ < 0).any(). 
+000097e0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000097f0: 696e 7374 616e 6365 2878 5f5f 2c20 2869  instance(x__, (i
+00009800: 6e74 2c20 666c 6f61 742c 206e 756d 7079  nt, float, numpy
+00009810: 2e6e 756d 6265 7229 293a 0a20 2020 2020  .number)):.     
+00009820: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009830: 6e20 785f 5f20 3c20 300a 2020 2020 2020  n x__ < 0.      
+00009840: 2020 2020 2020 6966 206e 6f74 2074 663a        if not tf:
+00009850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009860: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00009870: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00009880: 2069 7369 6e73 7461 6e63 6528 785f 5f2c   isinstance(x__,
+00009890: 2074 662e 5465 6e73 6f72 290a 2020 2020   tf.Tensor).    
+000098a0: 2020 2020 2020 2020 785f 5f20 3d20 7465          x__ = te
+000098b0: 6e73 6f72 5f75 7469 6c2e 636f 6e73 7461  nsor_util.consta
+000098c0: 6e74 5f76 616c 7565 2878 5f5f 290a 2020  nt_value(x__).  
+000098d0: 2020 2020 2020 2020 2020 6966 2078 5f5f            if x__
+000098e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000098f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00009900: 7475 726e 205f 6973 5f6e 6567 6174 6976  turn _is_negativ
+00009910: 6528 785f 5f29 0a20 2020 2020 2020 2020  e(x__).         
+00009920: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00009930: 0a20 2020 2020 2020 2064 6566 205f 6269  .        def _bi
+00009940: 6e5f 6f70 5f74 6628 612c 2062 293a 0a20  n_op_tf(a, b):. 
+00009950: 2020 2020 2020 2020 2020 2069 6620 7465             if te
+00009960: 6d70 6c61 7465 5f6f 6e6c 793a 0a20 2020  mplate_only:.   
+00009970: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00009980: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+00009990: 2020 2020 2069 6620 6120 6973 204e 6f6e       if a is Non
+000099a0: 6520 6f72 2062 2069 7320 4e6f 6e65 3a0a  e or b is None:.
+000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099c0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+000099d0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+000099e0: 7369 6e73 7461 6e63 6528 612c 2074 662e  sinstance(a, tf.
+000099f0: 5465 6e73 6f72 2920 616e 6420 6973 696e  Tensor) and isin
+00009a00: 7374 616e 6365 2862 2c20 2869 6e74 2c20  stance(b, (int, 
+00009a10: 7466 2e54 656e 736f 7229 290a 2020 2020  tf.Tensor)).    
+00009a20: 2020 2020 2020 2020 7769 7468 2074 665f          with tf_
+00009a30: 7574 696c 2e73 616d 655f 636f 6e74 726f  util.same_contro
+00009a40: 6c5f 666c 6f77 5f63 7478 285b 612c 2062  l_flow_ctx([a, b
+00009a50: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00009a60: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
+00009a70: 6164 6422 3a0a 2020 2020 2020 2020 2020  add":.          
+00009a80: 2020 2020 2020 2020 2020 7573 655f 7265            use_re
+00009a90: 6c75 203d 205f 6973 5f6e 6567 6174 6976  lu = _is_negativ
+00009aa0: 6528 6129 206f 7220 5f69 735f 6e65 6761  e(a) or _is_nega
+00009ab0: 7469 7665 2862 2920 2023 2066 6f72 2064  tive(b)  # for d
+00009ac0: 796e 616d 6963 2074 656e 736f 7273 2c20  ynamic tensors, 
+00009ad0: 6173 7375 6d65 2061 6c6c 2070 6f73 6974  assume all posit
+00009ae0: 6976 650a 2020 2020 2020 2020 2020 2020  ive.            
+00009af0: 2020 2020 2020 2020 6966 2075 7365 5f72          if use_r
+00009b00: 656c 753a 0a20 2020 2020 2020 2020 2020  elu:.           
+00009b10: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00009b20: 7572 6e20 7466 2e63 6f6e 7665 7274 5f74  urn tf.convert_t
+00009b30: 6f5f 7465 6e73 6f72 2874 665f 7574 696c  o_tensor(tf_util
+00009b40: 2e73 696d 706c 6966 795f 6e6f 6e5f 6e65  .simplify_non_ne
+00009b50: 6761 7469 7665 5f73 6571 5f6c 656e 6774  gative_seq_lengt
+00009b60: 6828 6120 2b20 6229 290a 2020 2020 2020  h(a + b)).      
+00009b70: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00009b80: 7475 726e 2061 202b 2062 0a20 2020 2020  turn a + b.     
+00009b90: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00009ba0: 6b69 6e64 203d 3d20 2273 7562 223a 0a20  kind == "sub":. 
+00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bc0: 2020 2072 6574 7572 6e20 7466 2e63 6f6e     return tf.con
+00009bd0: 7665 7274 5f74 6f5f 7465 6e73 6f72 2874  vert_to_tensor(t
+00009be0: 665f 7574 696c 2e73 696d 706c 6966 795f  f_util.simplify_
+00009bf0: 6e6f 6e5f 6e65 6761 7469 7665 5f73 6571  non_negative_seq
+00009c00: 5f6c 656e 6774 6828 6120 2d20 6229 290a  _length(a - b)).
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c20: 656c 6966 206b 696e 6420 3d3d 2022 6d75  elif kind == "mu
+00009c30: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+00009c40: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00009c50: 202a 2062 0a20 2020 2020 2020 2020 2020   * b.           
+00009c60: 2020 2020 2065 6c69 6620 6b69 6e64 2069       elif kind i
+00009c70: 6e20 2822 666c 6f6f 7264 6976 222c 2022  n ("floordiv", "
+00009c80: 7472 7565 6469 7622 293a 2020 2320 7472  truediv"):  # tr
+00009c90: 7565 6469 7620 6173 7375 6d65 7320 7468  uediv assumes th
+00009ca0: 6572 6520 6973 206e 6f20 7265 6d61 696e  ere is no remain
+00009cb0: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
+00009cc0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00009cd0: 202f 2f20 620a 2020 2020 2020 2020 2020   // b.          
+00009ce0: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
+00009cf0: 3d3d 2022 6365 696c 6469 7622 3a0a 2020  == "ceildiv":.  
 00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d10: 656c 6966 206b 696e 6420 3d3d 2022 6365  elif kind == "ce
-00009d20: 696c 6469 7622 3a0a 2020 2020 2020 2020  ildiv":.        
-00009d30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009d40: 726e 202d 282d 6120 2f2f 2062 290a 2020  rn -(-a // b).  
-00009d50: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00009d60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00009d70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00009d80: 6c75 6545 7272 6f72 2822 756e 6b6e 6f77  lueError("unknow
-00009d90: 6e20 6f70 206b 696e 6420 2572 2220 2520  n op kind %r" % 
-00009da0: 6f70 2e6b 696e 6429 0a0a 2020 2020 2020  op.kind)..      
-00009db0: 2020 6465 6620 5f62 696e 5f6f 7028 612c    def _bin_op(a,
-00009dc0: 2062 293a 0a20 2020 2020 2020 2020 2020   b):.           
-00009dd0: 2069 6620 7465 6d70 6c61 7465 5f6f 6e6c   if template_onl
-00009de0: 7920 6f72 206e 6f74 2062 6163 6b65 6e64  y or not backend
-00009df0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009e00: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00009e10: 612c 205f 742e 5465 6e73 6f72 2920 616e  a, _t.Tensor) an
-00009e20: 6420 6973 696e 7374 616e 6365 2862 2c20  d isinstance(b, 
-00009e30: 5f74 2e54 656e 736f 7229 3a0a 2020 2020  _t.Tensor):.    
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 7265 7475 726e 205f 742e 5465 6e73 6f72  return _t.Tensor
-00009e60: 2e67 6574 5f63 6f6d 6d6f 6e5f 6461 7461  .get_common_data
-00009e70: 285b 612c 2062 5d2c 2061 6c6c 6f77 5f62  ([a, b], allow_b
-00009e80: 726f 6164 6361 7374 5f61 6c6c 5f73 6f75  roadcast_all_sou
-00009e90: 7263 6573 3d54 7275 6529 0a20 2020 2020  rces=True).     
-00009ea0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00009eb0: 696e 7374 616e 6365 2861 2c20 5f74 2e54  instance(a, _t.T
-00009ec0: 656e 736f 7229 3a0a 2020 2020 2020 2020  ensor):.        
-00009ed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009ee0: 726e 2061 0a20 2020 2020 2020 2020 2020  rn a.           
-00009ef0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00009f00: 6365 2862 2c20 5f74 2e54 656e 736f 7229  ce(b, _t.Tensor)
-00009f10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009f20: 2020 2020 2020 7265 7475 726e 2062 0a20        return b. 
-00009f30: 2020 2020 2020 2020 2020 2069 6620 6b69             if ki
-00009f40: 6e64 203d 3d20 2261 6464 223a 0a20 2020  nd == "add":.   
-00009f50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00009f60: 7572 6e20 6120 2b20 620a 2020 2020 2020  urn a + b.      
-00009f70: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
-00009f80: 3d3d 2022 7375 6222 3a0a 2020 2020 2020  == "sub":.      
-00009f90: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009fa0: 2061 202d 2062 0a20 2020 2020 2020 2020   a - b.         
-00009fb0: 2020 2065 6c69 6620 6b69 6e64 203d 3d20     elif kind == 
-00009fc0: 226d 756c 223a 0a20 2020 2020 2020 2020  "mul":.         
-00009fd0: 2020 2020 2020 2072 6574 7572 6e20 6120         return a 
-00009fe0: 2a20 620a 2020 2020 2020 2020 2020 2020  * b.            
-00009ff0: 656c 6966 206b 696e 6420 696e 2028 2266  elif kind in ("f
-0000a000: 6c6f 6f72 6469 7622 2c20 2274 7275 6564  loordiv", "trued
-0000a010: 6976 2229 3a20 2023 2074 7275 6564 6976  iv"):  # truediv
-0000a020: 2061 7373 756d 6573 2074 6865 7265 2069   assumes there i
-0000a030: 7320 6e6f 2072 656d 6169 6e64 6572 0a20  s no remainder. 
-0000a040: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a050: 6574 7572 6e20 6120 2f2f 2062 0a20 2020  eturn a // b.   
-0000a060: 2020 2020 2020 2020 2065 6c69 6620 6b69           elif ki
-0000a070: 6e64 203d 3d20 2263 6569 6c64 6976 223a  nd == "ceildiv":
-0000a080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a090: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
-0000a0a0: 2c20 5465 6e73 6f72 293a 0a20 2020 2020  , Tensor):.     
-0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a0c0: 6574 7572 6e20 7266 2e63 6569 6c5f 6469  eturn rf.ceil_di
-0000a0d0: 7669 6465 2861 2c20 6229 0a20 2020 2020  vide(a, b).     
-0000a0e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000a0f0: 6e20 2d28 2d61 202f 2f20 6229 0a20 2020  n -(-a // b).   
-0000a100: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000a110: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a120: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000a130: 2275 6e6b 6e6f 776e 206f 7020 6b69 6e64  "unknown op kind
-0000a140: 2025 7222 2025 206f 702e 6b69 6e64 290a   %r" % op.kind).
-0000a150: 0a20 2020 2020 2020 2079 5f6e 616d 6520  .        y_name 
-0000a160: 3d20 7365 6c66 2e64 6573 6372 6970 7469  = self.descripti
-0000a170: 6f6e 202b 2022 3a73 6571 2d6c 656e 6774  on + ":seq-lengt
-0000a180: 6822 0a20 2020 2020 2020 2079 3a20 4f70  h".        y: Op
-0000a190: 7469 6f6e 616c 5b5f 742e 5465 6e73 6f72  tional[_t.Tensor
-0000a1a0: 5d20 3d20 4e6f 6e65 2020 2320 7265 7375  ] = None  # resu
-0000a1b0: 6c74 696e 6720 6479 6e20 7369 7a65 0a20  lting dyn size. 
-0000a1c0: 2020 2020 2020 2069 6e70 7574 7320 3d20         inputs = 
-0000a1d0: 6c69 7374 286f 702e 696e 7075 7473 290a  list(op.inputs).
-0000a1e0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-0000a1f0: 6e70 7574 730a 2020 2020 2020 2020 7768  nputs.        wh
-0000a200: 696c 6520 696e 7075 7473 3a0a 2020 2020  ile inputs:.    
-0000a210: 2020 2020 2020 2020 7820 3d20 696e 7075          x = inpu
-0000a220: 7473 2e70 6f70 2830 290a 2020 2020 2020  ts.pop(0).      
-0000a230: 2020 2020 2020 6966 206e 6f74 2078 2e69        if not x.i
-0000a240: 735f 6479 6e61 6d69 6328 293a 2020 2320  s_dynamic():  # 
-0000a250: 7374 6174 6963 0a20 2020 2020 2020 2020  static.         
-0000a260: 2020 2020 2020 2061 7373 6572 7420 782e         assert x.
-0000a270: 6469 6d65 6e73 696f 6e20 6973 206e 6f74  dimension is not
-0000a280: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000a290: 2020 2020 2020 6966 2079 2069 7320 4e6f        if y is No
-0000a2a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a2b0: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
-0000a2c0: 656d 706c 6174 655f 6f6e 6c79 2061 6e64  emplate_only and
-0000a2d0: 2062 6163 6b65 6e64 2061 6e64 206e 6f74   backend and not
-0000a2e0: 2074 663a 0a20 2020 2020 2020 2020 2020   tf:.           
-0000a2f0: 2020 2020 2020 2020 2020 2020 2079 203d               y =
-0000a300: 2062 6163 6b65 6e64 2e63 6f6e 7665 7274   backend.convert
-0000a310: 5f74 6f5f 7465 6e73 6f72 2878 2e64 696d  _to_tensor(x.dim
-0000a320: 656e 7369 6f6e 2c20 6469 6d73 3d5b 5d2c  ension, dims=[],
-0000a330: 2064 7479 7065 3d73 697a 655f 6474 7970   dtype=size_dtyp
-0000a340: 652c 206e 616d 653d 795f 6e61 6d65 290a  e, name=y_name).
+00009d10: 2020 7265 7475 726e 202d 282d 6120 2f2f    return -(-a //
+00009d20: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
+00009d30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009d40: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00009d50: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00009d60: 756e 6b6e 6f77 6e20 6f70 206b 696e 6420  unknown op kind 
+00009d70: 2572 2220 2520 6f70 2e6b 696e 6429 0a0a  %r" % op.kind)..
+00009d80: 2020 2020 2020 2020 6465 6620 5f62 696e          def _bin
+00009d90: 5f6f 7028 612c 2062 293a 0a20 2020 2020  _op(a, b):.     
+00009da0: 2020 2020 2020 2069 6620 7465 6d70 6c61         if templa
+00009db0: 7465 5f6f 6e6c 7920 6f72 206e 6f74 2062  te_only or not b
+00009dc0: 6163 6b65 6e64 3a0a 2020 2020 2020 2020  ackend:.        
+00009dd0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00009de0: 7461 6e63 6528 612c 205f 742e 5465 6e73  tance(a, _t.Tens
+00009df0: 6f72 2920 616e 6420 6973 696e 7374 616e  or) and isinstan
+00009e00: 6365 2862 2c20 5f74 2e54 656e 736f 7229  ce(b, _t.Tensor)
+00009e10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009e20: 2020 2020 2020 7265 7475 726e 205f 742e        return _t.
+00009e30: 5465 6e73 6f72 2e67 6574 5f63 6f6d 6d6f  Tensor.get_commo
+00009e40: 6e5f 6461 7461 285b 612c 2062 5d2c 2061  n_data([a, b], a
+00009e50: 6c6c 6f77 5f62 726f 6164 6361 7374 5f61  llow_broadcast_a
+00009e60: 6c6c 5f73 6f75 7263 6573 3d54 7275 6529  ll_sources=True)
+00009e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009e80: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+00009e90: 2c20 5f74 2e54 656e 736f 7229 3a0a 2020  , _t.Tensor):.  
+00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009eb0: 2020 7265 7475 726e 2061 0a20 2020 2020    return a.     
+00009ec0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00009ed0: 696e 7374 616e 6365 2862 2c20 5f74 2e54  instance(b, _t.T
+00009ee0: 656e 736f 7229 3a0a 2020 2020 2020 2020  ensor):.        
+00009ef0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009f00: 726e 2062 0a20 2020 2020 2020 2020 2020  rn b.           
+00009f10: 2069 6620 6b69 6e64 203d 3d20 2261 6464   if kind == "add
+00009f20: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00009f30: 2020 2072 6574 7572 6e20 5f72 656c 7528     return _relu(
+00009f40: 6120 2b20 6229 0a20 2020 2020 2020 2020  a + b).         
+00009f50: 2020 2065 6c69 6620 6b69 6e64 203d 3d20     elif kind == 
+00009f60: 2273 7562 223a 0a20 2020 2020 2020 2020  "sub":.         
+00009f70: 2020 2020 2020 2072 6574 7572 6e20 5f72         return _r
+00009f80: 656c 7528 6120 2d20 6229 0a20 2020 2020  elu(a - b).     
+00009f90: 2020 2020 2020 2065 6c69 6620 6b69 6e64         elif kind
+00009fa0: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
+00009fb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009fc0: 6e20 6120 2a20 620a 2020 2020 2020 2020  n a * b.        
+00009fd0: 2020 2020 656c 6966 206b 696e 6420 696e      elif kind in
+00009fe0: 2028 2266 6c6f 6f72 6469 7622 2c20 2274   ("floordiv", "t
+00009ff0: 7275 6564 6976 2229 3a20 2023 2074 7275  ruediv"):  # tru
+0000a000: 6564 6976 2061 7373 756d 6573 2074 6865  ediv assumes the
+0000a010: 7265 2069 7320 6e6f 2072 656d 6169 6e64  re is no remaind
+0000a020: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+0000a030: 2020 2072 6574 7572 6e20 6120 2f2f 2062     return a // b
+0000a040: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000a050: 6620 6b69 6e64 203d 3d20 2263 6569 6c64  f kind == "ceild
+0000a060: 6976 223a 0a20 2020 2020 2020 2020 2020  iv":.           
+0000a070: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0000a080: 6365 2861 2c20 5f74 2e54 656e 736f 7229  ce(a, _t.Tensor)
+0000a090: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a0a0: 2020 2020 2020 7265 7475 726e 2072 662e        return rf.
+0000a0b0: 6365 696c 5f64 6976 6964 6528 612c 2062  ceil_divide(a, b
+0000a0c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a0d0: 2020 7265 7475 726e 202d 282d 6120 2f2f    return -(-a //
+0000a0e0: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
+0000a0f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000a100: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0000a110: 6545 7272 6f72 2822 756e 6b6e 6f77 6e20  eError("unknown 
+0000a120: 6f70 206b 696e 6420 2572 2220 2520 6f70  op kind %r" % op
+0000a130: 2e6b 696e 6429 0a0a 2020 2020 2020 2020  .kind)..        
+0000a140: 6465 6620 5f72 656c 7528 6129 3a0a 2020  def _relu(a):.  
+0000a150: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000a160: 6e73 7461 6e63 6528 612c 205f 742e 5465  nstance(a, _t.Te
+0000a170: 6e73 6f72 293a 0a20 2020 2020 2020 2020  nsor):.         
+0000a180: 2020 2020 2020 2072 6574 7572 6e20 7266         return rf
+0000a190: 2e72 656c 7528 6129 0a20 2020 2020 2020  .relu(a).       
+0000a1a0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+0000a1b0: 616e 6365 2861 2c20 696e 7429 3a0a 2020  ance(a, int):.  
+0000a1c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000a1d0: 7475 726e 206d 6178 2861 2c20 3029 0a20  turn max(a, 0). 
+0000a1e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000a1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a200: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+0000a210: 2866 2263 6f6d 706c 6574 655f 6479 6e5f  (f"complete_dyn_
+0000a220: 7369 7a65 3a20 5f72 656c 753a 2075 6e65  size: _relu: une
+0000a230: 7870 6563 7465 6420 7479 7065 207b 7479  xpected type {ty
+0000a240: 7065 2861 297d 2229 0a0a 2020 2020 2020  pe(a)}")..      
+0000a250: 2020 795f 6e61 6d65 203d 2073 656c 662e    y_name = self.
+0000a260: 6465 7363 7269 7074 696f 6e20 2b20 223a  description + ":
+0000a270: 7365 712d 6c65 6e67 7468 220a 2020 2020  seq-length".    
+0000a280: 2020 2020 793a 204f 7074 696f 6e61 6c5b      y: Optional[
+0000a290: 5f74 2e54 656e 736f 725d 203d 204e 6f6e  _t.Tensor] = Non
+0000a2a0: 6520 2023 2072 6573 756c 7469 6e67 2064  e  # resulting d
+0000a2b0: 796e 2073 697a 650a 2020 2020 2020 2020  yn size.        
+0000a2c0: 696e 7075 7473 203d 206c 6973 7428 6f70  inputs = list(op
+0000a2d0: 2e69 6e70 7574 7329 0a20 2020 2020 2020  .inputs).       
+0000a2e0: 2061 7373 6572 7420 696e 7075 7473 0a20   assert inputs. 
+0000a2f0: 2020 2020 2020 2077 6869 6c65 2069 6e70         while inp
+0000a300: 7574 733a 0a20 2020 2020 2020 2020 2020  uts:.           
+0000a310: 2078 203d 2069 6e70 7574 732e 706f 7028   x = inputs.pop(
+0000a320: 3029 0a20 2020 2020 2020 2020 2020 2069  0).            i
+0000a330: 6620 6e6f 7420 782e 6973 5f64 796e 616d  f not x.is_dynam
+0000a340: 6963 2829 3a20 2023 2073 7461 7469 630a  ic():  # static.
 0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a360: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a380: 2020 7920 3d20 5f74 2e54 656e 736f 7228    y = _t.Tensor(
-0000a390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a3a0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-0000a3b0: 653d 795f 6e61 6d65 2c0a 2020 2020 2020  e=y_name,.      
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3d0: 2020 2020 2020 6469 6d5f 7461 6773 3d5b        dim_tags=[
-0000a3e0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000a400: 7479 7065 3d73 697a 655f 6474 7970 652c  type=size_dtype,
-0000a410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a420: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a440: 2020 2069 6620 6e6f 7420 7465 6d70 6c61     if not templa
-0000a450: 7465 5f6f 6e6c 7920 616e 6420 7466 3a0a  te_only and tf:.
-0000a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a470: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000a480: 2074 662e 636f 6e74 726f 6c5f 6465 7065   tf.control_depe
-0000a490: 6e64 656e 6369 6573 284e 6f6e 6529 3a20  ndencies(None): 
-0000a4a0: 2023 2074 6869 7320 7769 6c6c 2072 6573   # this will res
-0000a4b0: 6574 2074 6865 2063 6f6e 7465 7874 0a20  et the context. 
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0000a4e0: 2e72 6177 5f74 656e 736f 7220 3d20 7466  .raw_tensor = tf
-0000a4f0: 2e63 6f6e 7374 616e 7428 782e 6469 6d65  .constant(x.dime
-0000a500: 6e73 696f 6e29 0a20 2020 2020 2020 2020  nsion).         
-0000a510: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000a520: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-0000a530: 2020 2020 6966 2074 663a 0a20 2020 2020      if tf:.     
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0000a550: 2e70 6c61 6365 686f 6c64 6572 203d 205f  .placeholder = _
-0000a560: 6269 6e5f 6f70 5f74 6628 792e 706c 6163  bin_op_tf(y.plac
-0000a570: 6568 6f6c 6465 722c 2078 2e64 696d 656e  eholder, x.dimen
-0000a580: 7369 6f6e 290a 2020 2020 2020 2020 2020  sion).          
-0000a590: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5b0: 7920 3d20 5f62 696e 5f6f 7028 792c 2078  y = _bin_op(y, x
-0000a5c0: 2e64 696d 656e 7369 6f6e 290a 2020 2020  .dimension).    
-0000a5d0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000a5e0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-0000a5f0: 2069 6620 7365 6c66 2e62 6174 6368 3a0a   if self.batch:.
+0000a360: 6173 7365 7274 2078 2e64 696d 656e 7369  assert x.dimensi
+0000a370: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 0a20  on is not None. 
+0000a380: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000a390: 6620 7920 6973 204e 6f6e 653a 0a20 2020  f y is None:.   
+0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3b0: 2069 6620 6e6f 7420 7465 6d70 6c61 7465   if not template
+0000a3c0: 5f6f 6e6c 7920 616e 6420 6261 636b 656e  _only and backen
+0000a3d0: 6420 616e 6420 6e6f 7420 7466 3a0a 2020  d and not tf:.  
+0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3f0: 2020 2020 2020 7920 3d20 6261 636b 656e        y = backen
+0000a400: 642e 636f 6e76 6572 745f 746f 5f74 656e  d.convert_to_ten
+0000a410: 736f 7228 782e 6469 6d65 6e73 696f 6e2c  sor(x.dimension,
+0000a420: 2064 696d 733d 5b5d 2c20 6474 7970 653d   dims=[], dtype=
+0000a430: 7369 7a65 5f64 7479 7065 2c20 6e61 6d65  size_dtype, name
+0000a440: 3d79 5f6e 616d 6529 0a20 2020 2020 2020  =y_name).       
+0000a450: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000a460: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000a470: 2020 2020 2020 2020 2020 2079 203d 205f             y = _
+0000a480: 742e 5465 6e73 6f72 280a 2020 2020 2020  t.Tensor(.      
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 2020 6e61 6d65 3d79 5f6e 616d        name=y_nam
+0000a4b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000a4d0: 696d 5f74 6167 733d 5b5d 2c0a 2020 2020  im_tags=[],.    
+0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4f0: 2020 2020 2020 2020 6474 7970 653d 7369          dtype=si
+0000a500: 7a65 5f64 7479 7065 2c0a 2020 2020 2020  ze_dtype,.      
+0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a520: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000a530: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000a540: 6f74 2074 656d 706c 6174 655f 6f6e 6c79  ot template_only
+0000a550: 2061 6e64 2074 663a 0a20 2020 2020 2020   and tf:.       
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2020 2020 2077 6974 6820 7466 2e63 6f6e       with tf.con
+0000a580: 7472 6f6c 5f64 6570 656e 6465 6e63 6965  trol_dependencie
+0000a590: 7328 4e6f 6e65 293a 2020 2320 7468 6973  s(None):  # this
+0000a5a0: 2077 696c 6c20 7265 7365 7420 7468 6520   will reset the 
+0000a5b0: 636f 6e74 6578 740a 2020 2020 2020 2020  context.        
+0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5d0: 2020 2020 2020 2020 792e 7261 775f 7465          y.raw_te
+0000a5e0: 6e73 6f72 203d 2074 662e 636f 6e73 7461  nsor = tf.consta
+0000a5f0: 6e74 2878 2e64 696d 656e 7369 6f6e 290a  nt(x.dimension).
 0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a610: 7820 3d20 782e 6765 745f 666f 725f 6261  x = x.get_for_ba
-0000a620: 7463 685f 6374 7828 7365 6c66 2e62 6174  tch_ctx(self.bat
-0000a630: 6368 2c20 7365 6c66 2e63 6f6e 7472 6f6c  ch, self.control
-0000a640: 5f66 6c6f 775f 6374 7829 0a20 2020 2020  _flow_ctx).     
-0000a650: 2020 2020 2020 2078 2e63 6f6d 706c 6574         x.complet
-0000a660: 655f 6479 6e5f 7369 7a65 2874 656d 706c  e_dyn_size(templ
-0000a670: 6174 655f 6f6e 6c79 3d74 656d 706c 6174  ate_only=templat
-0000a680: 655f 6f6e 6c79 290a 2020 2020 2020 2020  e_only).        
-0000a690: 2020 2020 6966 206e 6f74 2078 2e64 796e      if not x.dyn
-0000a6a0: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-0000a6b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000a6c0: 6e0a 2020 2020 2020 2020 2020 2020 7820  n.            x 
-0000a6d0: 3d20 782e 6479 6e5f 7369 7a65 5f65 7874  = x.dyn_size_ext
-0000a6e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000a6f0: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
-0000a700: 2020 2020 2020 2020 2020 2079 203d 2078             y = x
-0000a710: 2e63 6f70 7928 6e61 6d65 3d79 5f6e 616d  .copy(name=y_nam
-0000a720: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000a730: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-0000a740: 2020 2020 2020 2020 6966 2078 2e64 696d          if x.dim
-0000a750: 5f74 6167 7320 213d 2079 2e64 696d 5f74  _tags != y.dim_t
-0000a760: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
-0000a770: 2020 2020 2063 6f6d 6d6f 6e20 3d20 5f74       common = _t
-0000a780: 2e54 656e 736f 722e 6765 745f 636f 6d6d  .Tensor.get_comm
-0000a790: 6f6e 5f64 6174 6128 5b78 2c20 795d 2c20  on_data([x, y], 
-0000a7a0: 616c 6c6f 775f 6272 6f61 6463 6173 745f  allow_broadcast_
-0000a7b0: 616c 6c5f 736f 7572 6365 733d 5472 7565  all_sources=True
-0000a7c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a7d0: 2020 785f 203d 2078 2e63 6f70 795f 636f    x_ = x.copy_co
-0000a7e0: 6d70 6174 6962 6c65 5f74 6f28 636f 6d6d  mpatible_to(comm
-0000a7f0: 6f6e 2920 6966 2078 2e64 696d 5f74 6167  on) if x.dim_tag
-0000a800: 7320 656c 7365 2078 0a20 2020 2020 2020  s else x.       
-0000a810: 2020 2020 2020 2020 2079 5f20 3d20 792e           y_ = y.
-0000a820: 636f 7079 5f63 6f6d 7061 7469 626c 655f  copy_compatible_
-0000a830: 746f 2863 6f6d 6d6f 6e29 2069 6620 792e  to(common) if y.
-0000a840: 6469 6d5f 7461 6773 2065 6c73 6520 790a  dim_tags else y.
-0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a860: 7920 3d20 636f 6d6d 6f6e 0a20 2020 2020  y = common.     
-0000a870: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000a880: 2020 2020 2020 2020 2020 2020 2078 5f2c               x_,
-0000a890: 2079 5f20 3d20 782c 2079 0a20 2020 2020   y_ = x, y.     
-0000a8a0: 2020 2020 2020 2069 6620 7466 3a0a 2020         if tf:.  
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 792e                y.
-0000a8c0: 706c 6163 6568 6f6c 6465 7220 3d20 5f62  placeholder = _b
-0000a8d0: 696e 5f6f 705f 7466 2879 5f2e 706c 6163  in_op_tf(y_.plac
-0000a8e0: 6568 6f6c 6465 722c 2078 5f2e 706c 6163  eholder, x_.plac
-0000a8f0: 6568 6f6c 6465 7229 0a20 2020 2020 2020  eholder).       
-0000a900: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a910: 2020 2020 2020 2020 2020 2079 203d 205f             y = _
-0000a920: 6269 6e5f 6f70 2879 5f2c 2078 5f29 0a20  bin_op(y_, x_). 
-0000a930: 2020 2020 2020 2061 7373 6572 7420 792c         assert y,
-0000a940: 2066 226f 7020 7b6f 707d 3f22 0a20 2020   f"op {op}?".   
-0000a950: 2020 2020 2069 6620 7365 6c66 2e64 796e       if self.dyn
-0000a960: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-0000a970: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-0000a980: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-0000a990: 6469 6d5f 7461 6773 203d 3d20 792e 6469  dim_tags == y.di
-0000a9a0: 6d5f 7461 6773 0a20 2020 2020 2020 2069  m_tags.        i
-0000a9b0: 6620 792e 6261 7463 683a 0a20 2020 2020  f y.batch:.     
-0000a9c0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0000a9d0: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
-0000a9e0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-0000a9f0: 662e 6261 7463 6820 3d3d 2079 2e62 6174  f.batch == y.bat
-0000aa00: 6368 0a20 2020 2020 2020 2020 2020 2065  ch.            e
-0000aa10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000aa20: 2020 2020 2073 656c 662e 6261 7463 6820       self.batch 
-0000aa30: 3d20 792e 6261 7463 680a 2020 2020 2020  = y.batch.      
-0000aa40: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-0000aa50: 6578 7420 3d20 790a 2020 2020 2020 2020  ext = y.        
-0000aa60: 6966 2074 6620 616e 6420 792e 706c 6163  if tf and y.plac
-0000aa70: 6568 6f6c 6465 7220 6973 206e 6f74 204e  eholder is not N
-0000aa80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000aa90: 2073 656c 662e 7365 745f 7461 675f 6f6e   self.set_tag_on
-0000aaa0: 5f73 697a 655f 7465 6e73 6f72 2879 2e70  _size_tensor(y.p
-0000aab0: 6c61 6365 686f 6c64 6572 290a 0a20 2020  laceholder)..   
-0000aac0: 2064 6566 2069 735f 6571 7561 6c28 0a20   def is_equal(. 
-0000aad0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000aae0: 2020 2020 206f 7468 6572 2c0a 2020 2020       other,.    
-0000aaf0: 2020 2020 6967 6e6f 7265 5f66 6561 7475      ignore_featu
-0000ab00: 7265 5f64 696d 3d46 616c 7365 2c0a 2020  re_dim=False,.  
-0000ab10: 2020 2020 2020 616c 6c6f 775f 7361 6d65        allow_same
-0000ab20: 5f66 6561 7475 7265 5f64 696d 3d46 616c  _feature_dim=Fal
-0000ab30: 7365 2c0a 2020 2020 2020 2020 616c 6c6f  se,.        allo
-0000ab40: 775f 7361 6d65 5f73 7061 7469 616c 5f64  w_same_spatial_d
-0000ab50: 696d 3d4e 6f6e 652c 0a20 2020 2020 2020  im=None,.       
-0000ab60: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
-0000ab70: 735f 7370 6174 6961 6c3d 4661 6c73 652c  s_spatial=False,
-0000ab80: 0a20 2020 2020 2020 2062 726f 6164 6361  .        broadca
-0000ab90: 7374 5f6d 6174 6368 6573 3d46 616c 7365  st_matches=False
-0000aba0: 2c0a 2020 2020 2020 2020 756e 6b6e 6f77  ,.        unknow
-0000abb0: 6e5f 7370 6174 6961 6c5f 6d61 7463 6865  n_spatial_matche
-0000abc0: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
-0000abd0: 2075 6e64 6566 696e 6564 5f6d 6174 6368   undefined_match
-0000abe0: 6573 3d46 616c 7365 2c0a 2020 2020 2020  es=False,.      
-0000abf0: 2020 6465 7269 7665 645f 6d61 7463 6865    derived_matche
-0000ac00: 733d 4661 6c73 652c 0a20 2020 2029 3a0a  s=False,.    ):.
-0000ac10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000ac20: 2020 2020 436f 6d70 6172 6573 2073 656c      Compares sel
-0000ac30: 6620 746f 206f 7468 6572 2066 6f72 2065  f to other for e
-0000ac40: 7175 616c 6974 792e 0a0a 2020 2020 2020  quality...      
-0000ac50: 2020 4e6f 7465 2074 6861 7420 7468 6520    Note that the 
-0000ac60: 6465 6661 756c 7420 6265 6861 7669 6f72  default behavior
-0000ac70: 2069 7320 7665 7279 2072 6573 7472 6963   is very restric
-0000ac80: 7469 7665 2e0a 2020 2020 2020 2020 5573  tive..        Us
-0000ac90: 6520 6675 6e63 7469 6f6e 7320 7375 6368  e functions such
-0000aca0: 2061 7320 3a66 756e 633a 6067 6574 5f61   as :func:`get_a
-0000acb0: 6c6c 5f64 696d 656e 7369 6f6e 5f74 6167  ll_dimension_tag
-0000acc0: 7360 206f 7220 3a66 756e 633a 6067 6574  s` or :func:`get
-0000acd0: 5f65 7869 7374 696e 675f 7461 675f 6672  _existing_tag_fr
-0000ace0: 6f6d 5f63 6f6c 6c65 6374 696f 6e60 0a20  om_collection`. 
-0000acf0: 2020 2020 2020 2074 6f20 6578 706c 6963         to explic
-0000ad00: 6974 6c79 2073 7065 6369 6679 2074 6865  itly specify the
-0000ad10: 2062 6568 6176 696f 7220 666f 7220 7468   behavior for th
-0000ad20: 6520 636f 6d70 6172 6973 6f6e 2e0a 0a20  e comparison... 
-0000ad30: 2020 2020 2020 2041 6c73 6f20 6e6f 7465         Also note
-0000ad40: 2074 6861 7420 7468 6520 6465 6669 6e69   that the defini
-0000ad50: 7469 6f6e 2069 7320 736c 6967 6874 6c79  tion is slightly
-0000ad60: 2061 642d 686f 6320 666f 7220 736f 6d65   ad-hoc for some
-0000ad70: 2063 6173 6573 2c0a 2020 2020 2020 2020   cases,.        
-0000ad80: 616e 6420 6d69 6768 7420 706f 7465 6e74  and might potent
-0000ad90: 6961 6c6c 7920 6368 616e 6765 2069 6e20  ially change in 
-0000ada0: 7468 6520 6675 7475 7265 2e0a 2020 2020  the future..    
-0000adb0: 2020 2020 2020 6874 7470 733a 2f2f 6769        https://gi
-0000adc0: 7468 7562 2e63 6f6d 2f72 7774 682d 6936  thub.com/rwth-i6
-0000add0: 2f72 6574 7572 6e6e 2f69 7373 7565 732f  /returnn/issues/
-0000ade0: 3633 340a 0a20 2020 2020 2020 203a 7061  634..        :pa
-0000adf0: 7261 6d20 4469 6d20 6f74 6865 723a 0a20  ram Dim other:. 
-0000ae00: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
-0000ae10: 6f6c 2069 676e 6f72 655f 6665 6174 7572  ol ignore_featur
-0000ae20: 655f 6469 6d3a 0a20 2020 2020 2020 203a  e_dim:.        :
-0000ae30: 7061 7261 6d20 626f 6f6c 2061 6c6c 6f77  param bool allow
-0000ae40: 5f73 616d 655f 6665 6174 7572 655f 6469  _same_feature_di
-0000ae50: 6d3a 0a20 2020 2020 2020 203a 7061 7261  m:.        :para
-0000ae60: 6d20 626f 6f6c 7c4e 6f6e 6520 616c 6c6f  m bool|None allo
-0000ae70: 775f 7361 6d65 5f73 7061 7469 616c 5f64  w_same_spatial_d
-0000ae80: 696d 3a0a 2020 2020 2020 2020 3a70 6172  im:.        :par
-0000ae90: 616d 2062 6f6f 6c20 7472 6561 745f 6665  am bool treat_fe
-0000aea0: 6174 7572 655f 6173 5f73 7061 7469 616c  ature_as_spatial
-0000aeb0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-0000aec0: 2062 6f6f 6c20 6272 6f61 6463 6173 745f   bool broadcast_
-0000aed0: 6d61 7463 6865 733a 0a20 2020 2020 2020  matches:.       
-0000aee0: 203a 7061 7261 6d20 626f 6f6c 2075 6e6b   :param bool unk
-0000aef0: 6e6f 776e 5f73 7061 7469 616c 5f6d 6174  nown_spatial_mat
-0000af00: 6368 6573 3a0a 2020 2020 2020 2020 3a70  ches:.        :p
-0000af10: 6172 616d 2062 6f6f 6c20 756e 6465 6669  aram bool undefi
-0000af20: 6e65 645f 6d61 7463 6865 733a 0a20 2020  ned_matches:.   
-0000af30: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
-0000af40: 2064 6572 6976 6564 5f6d 6174 6368 6573   derived_matches
-0000af50: 3a0a 2020 2020 2020 2020 3a72 7479 7065  :.        :rtype
-0000af60: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-0000af70: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
-0000af80: 7265 7475 726e 6e2e 7574 696c 2069 6d70  returnn.util imp
-0000af90: 6f72 7420 4265 6861 7669 6f72 5665 7273  ort BehaviorVers
-0000afa0: 696f 6e0a 0a20 2020 2020 2020 2069 6620  ion..        if 
-0000afb0: 7365 6c66 2069 7320 6f74 6865 723a 2020  self is other:  
-0000afc0: 2320 6669 7273 7420 736f 6d65 2066 6173  # first some fas
-0000afd0: 7420 7061 7468 2063 6865 636b 0a20 2020  t path check.   
-0000afe0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000aff0: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
-0000b000: 7365 6c66 2e73 7065 6369 616c 206f 7220  self.special or 
-0000b010: 6f74 6865 722e 7370 6563 6961 6c3a 0a20  other.special:. 
-0000b020: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b030: 6e20 4661 6c73 6520 2023 206f 6e6c 7920  n False  # only 
-0000b040: 7472 7565 2069 6620 7361 6d65 2069 6e73  true if same ins
-0000b050: 7461 6e63 652c 2063 6865 636b 2061 626f  tance, check abo
-0000b060: 7665 0a20 2020 2020 2020 2069 6620 616c  ve.        if al
-0000b070: 6c6f 775f 7361 6d65 5f73 7061 7469 616c  low_same_spatial
-0000b080: 5f64 696d 2069 7320 4e6f 6e65 3a0a 2020  _dim is None:.  
-0000b090: 2020 2020 2020 2020 2020 616c 6c6f 775f            allow_
-0000b0a0: 7361 6d65 5f73 7061 7469 616c 5f64 696d  same_spatial_dim
-0000b0b0: 203d 2061 6c6c 6f77 5f73 616d 655f 6665   = allow_same_fe
-0000b0c0: 6174 7572 655f 6469 6d0a 2020 2020 2020  ature_dim.      
-0000b0d0: 2020 7365 6c66 5f62 6173 6520 3d20 7365    self_base = se
-0000b0e0: 6c66 2e67 6574 5f73 616d 655f 6465 7269  lf.get_same_deri
-0000b0f0: 7665 645f 6261 7365 2829 2069 6620 6465  ved_base() if de
-0000b100: 7269 7665 645f 6d61 7463 6865 7320 656c  rived_matches el
-0000b110: 7365 2073 656c 662e 6765 745f 7361 6d65  se self.get_same
-0000b120: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
-0000b130: 6f74 6865 725f 6261 7365 203d 206f 7468  other_base = oth
-0000b140: 6572 2e67 6574 5f73 616d 655f 6465 7269  er.get_same_deri
-0000b150: 7665 645f 6261 7365 2829 2069 6620 6465  ved_base() if de
-0000b160: 7269 7665 645f 6d61 7463 6865 7320 656c  rived_matches el
-0000b170: 7365 206f 7468 6572 2e67 6574 5f73 616d  se other.get_sam
-0000b180: 655f 6261 7365 2829 0a20 2020 2020 2020  e_base().       
-0000b190: 2069 6620 7365 6c66 5f62 6173 6520 6973   if self_base is
-0000b1a0: 206f 7468 6572 5f62 6173 653a 0a20 2020   other_base:.   
-0000b1b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000b1c0: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
-0000b1d0: 7365 6c66 5f62 6173 652e 6465 7269 7665  self_base.derive
-0000b1e0: 645f 6672 6f6d 5f6f 7020 616e 6420 6f74  d_from_op and ot
-0000b1f0: 6865 725f 6261 7365 2e64 6572 6976 6564  her_base.derived
-0000b200: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
-0000b210: 2020 2020 2020 6966 2073 656c 665f 6261        if self_ba
-0000b220: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
-0000b230: 6f70 203d 3d20 6f74 6865 725f 6261 7365  op == other_base
-0000b240: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-0000b250: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b260: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000b270: 2020 2020 2020 7365 6c66 5f6b 696e 6420        self_kind 
-0000b280: 3d20 7365 6c66 2e6b 696e 640a 2020 2020  = self.kind.    
-0000b290: 2020 2020 6f74 6865 725f 6b69 6e64 203d      other_kind =
-0000b2a0: 206f 7468 6572 2e6b 696e 640a 2020 2020   other.kind.    
-0000b2b0: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
-0000b2c0: 203d 3d20 6f74 6865 725f 6b69 6e64 203d   == other_kind =
-0000b2d0: 3d20 4469 6d54 7970 6573 2e46 6561 7475  = DimTypes.Featu
-0000b2e0: 7265 2061 6e64 2069 676e 6f72 655f 6665  re and ignore_fe
-0000b2f0: 6174 7572 655f 6469 6d3a 0a20 2020 2020  ature_dim:.     
-0000b300: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000b310: 7565 0a20 2020 2020 2020 2069 6620 7472  ue.        if tr
-0000b320: 6561 745f 6665 6174 7572 655f 6173 5f73  eat_feature_as_s
-0000b330: 7061 7469 616c 3a0a 2020 2020 2020 2020  patial:.        
-0000b340: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
-0000b350: 203d 3d20 4469 6d54 7970 6573 2e46 6561   == DimTypes.Fea
-0000b360: 7475 7265 3a0a 2020 2020 2020 2020 2020  ture:.          
-0000b370: 2020 2020 2020 7365 6c66 5f6b 696e 6420        self_kind 
-0000b380: 3d20 4469 6d54 7970 6573 2e53 7061 7469  = DimTypes.Spati
-0000b390: 616c 0a20 2020 2020 2020 2020 2020 2069  al.            i
-0000b3a0: 6620 6f74 6865 725f 6b69 6e64 203d 3d20  f other_kind == 
-0000b3b0: 4469 6d54 7970 6573 2e46 6561 7475 7265  DimTypes.Feature
-0000b3c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b3d0: 2020 6f74 6865 725f 6b69 6e64 203d 2044    other_kind = D
-0000b3e0: 696d 5479 7065 732e 5370 6174 6961 6c0a  imTypes.Spatial.
-0000b3f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b400: 6469 6d65 6e73 696f 6e20 213d 206f 7468  dimension != oth
-0000b410: 6572 2e64 696d 656e 7369 6f6e 3a0a 2020  er.dimension:.  
-0000b420: 2020 2020 2020 2020 2020 6966 2062 726f            if bro
-0000b430: 6164 6361 7374 5f6d 6174 6368 6573 2061  adcast_matches a
-0000b440: 6e64 2028 7365 6c66 2e64 696d 656e 7369  nd (self.dimensi
-0000b450: 6f6e 203d 3d20 3120 6f72 206f 7468 6572  on == 1 or other
-0000b460: 2e64 696d 656e 7369 6f6e 203d 3d20 3129  .dimension == 1)
-0000b470: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b480: 2020 7061 7373 2020 2320 7061 7373 206f    pass  # pass o
-0000b490: 6e0a 2020 2020 2020 2020 2020 2020 656c  n.            el
-0000b4a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000b4b0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0000b4c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000b4d0: 5f6b 696e 6420 213d 206f 7468 6572 5f6b  _kind != other_k
-0000b4e0: 696e 643a 0a20 2020 2020 2020 2020 2020  ind:.           
-0000b4f0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-0000b500: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
-0000b510: 6e64 203d 3d20 6f74 6865 725f 6b69 6e64  nd == other_kind
-0000b520: 203d 3d20 4469 6d54 7970 6573 2e42 6174   == DimTypes.Bat
-0000b530: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-0000b540: 2320 4e6f 7465 3a20 5468 6973 206d 6967  # Note: This mig
-0000b550: 6874 2062 6520 696e 636f 7272 6563 7420  ht be incorrect 
-0000b560: 696e 2073 6f6d 6520 6361 7365 732c 0a20  in some cases,. 
-0000b570: 2020 2020 2020 2020 2020 2023 2065 2e67             # e.g
-0000b580: 2e20 666f 7220 6265 616d 2073 6561 7263  . for beam searc
-0000b590: 6820 7768 656e 2077 6520 6861 7665 2074  h when we have t
-0000b5a0: 6865 2062 6561 6d20 6869 6464 656e 2069  he beam hidden i
-0000b5b0: 6e20 7468 6520 6261 7463 6820 6469 6d2c  n the batch dim,
-0000b5c0: 0a20 2020 2020 2020 2020 2020 2023 206f  .            # o
-0000b5d0: 7220 7768 656e 2077 6520 7573 6564 204d  r when we used M
-0000b5e0: 6572 6765 4469 6d73 4c61 7965 7220 6f6e  ergeDimsLayer on
-0000b5f0: 2074 6865 2062 6174 6368 2061 7869 732c   the batch axis,
-0000b600: 206f 7220 736f 2e0a 2020 2020 2020 2020   or so..        
-0000b610: 2020 2020 2320 5765 206d 6967 6874 206e      # We might n
-0000b620: 6565 6420 746f 2065 7874 656e 6420 7468  eed to extend th
-0000b630: 6520 6c6f 6769 6320 6865 7265 206c 6174  e logic here lat
-0000b640: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-0000b650: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000b660: 2020 2020 6966 2042 6568 6176 696f 7256      if BehaviorV
-0000b670: 6572 7369 6f6e 2e67 6574 2829 203e 3d20  ersion.get() >= 
-0000b680: 3136 3a0a 2020 2020 2020 2020 2020 2020  16:.            
-0000b690: 2320 4569 7468 6572 2073 656c 6620 6f72  # Either self or
-0000b6a0: 206f 7468 6572 2069 7320 736f 6d65 2064   other is some d
-0000b6b0: 696d 2074 6167 2065 7870 6c69 6369 746c  im tag explicitl
-0000b6c0: 7920 6372 6561 7465 6420 6279 2074 6865  y created by the
-0000b6d0: 2075 7365 722c 0a20 2020 2020 2020 2020   user,.         
-0000b6e0: 2020 2023 2061 6e64 2074 6865 7920 6172     # and they ar
-0000b6f0: 6520 6e6f 7420 7468 6520 7361 6d65 2c20  e not the same, 
-0000b700: 736f 2077 6520 6e65 7665 7220 7472 6561  so we never trea
-0000b710: 7420 7468 656d 2061 7320 6571 7561 6c2e  t them as equal.
-0000b720: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b730: 6e6f 7420 7365 6c66 2e61 7574 6f5f 6765  not self.auto_ge
-0000b740: 6e65 7261 7465 6420 6f72 206e 6f74 206f  nerated or not o
-0000b750: 7468 6572 2e61 7574 6f5f 6765 6e65 7261  ther.auto_genera
-0000b760: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
-0000b770: 2020 2020 2069 6620 6272 6f61 6463 6173       if broadcas
-0000b780: 745f 6d61 7463 6865 7320 616e 6420 280a  t_matches and (.
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7a0: 2020 2020 2873 656c 662e 6469 6d65 6e73      (self.dimens
-0000b7b0: 696f 6e20 3d3d 2031 2061 6e64 2073 656c  ion == 1 and sel
-0000b7c0: 662e 6175 746f 5f67 656e 6572 6174 6564  f.auto_generated
-0000b7d0: 2920 6f72 2028 6f74 6865 722e 6469 6d65  ) or (other.dime
-0000b7e0: 6e73 696f 6e20 3d3d 2031 2061 6e64 206f  nsion == 1 and o
-0000b7f0: 7468 6572 2e61 7574 6f5f 6765 6e65 7261  ther.auto_genera
-0000b800: 7465 6429 0a20 2020 2020 2020 2020 2020  ted).           
-0000b810: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-0000b820: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0000b830: 2020 2320 6578 6365 7074 696f 6e2c 2061    # exception, a
-0000b840: 6c6c 6f77 2062 726f 6164 6361 7374 206c  llow broadcast l
-0000b850: 6f67 6963 0a20 2020 2020 2020 2020 2020  ogic.           
-0000b860: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000b870: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000b880: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-0000b890: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
-0000b8a0: 203d 3d20 6f74 6865 725f 6b69 6e64 203d   == other_kind =
-0000b8b0: 3d20 4469 6d54 7970 6573 2e46 6561 7475  = DimTypes.Featu
-0000b8c0: 7265 3a0a 2020 2020 2020 2020 2020 2020  re:.            
-0000b8d0: 6966 2061 6c6c 6f77 5f73 616d 655f 6665  if allow_same_fe
-0000b8e0: 6174 7572 655f 6469 6d3a 0a20 2020 2020  ature_dim:.     
-0000b8f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b900: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
-0000b910: 6620 7365 6c66 5f6b 696e 6420 3d3d 206f  f self_kind == o
-0000b920: 7468 6572 5f6b 696e 6420 3d3d 2044 696d  ther_kind == Dim
-0000b930: 5479 7065 732e 5370 6174 6961 6c3a 0a20  Types.Spatial:. 
-0000b940: 2020 2020 2020 2020 2020 2069 6620 616c             if al
-0000b950: 6c6f 775f 7361 6d65 5f73 7061 7469 616c  low_same_spatial
-0000b960: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
-0000b970: 2020 2020 2020 6966 2073 656c 662e 6469        if self.di
-0000b980: 6d65 6e73 696f 6e20 6973 206e 6f74 204e  mension is not N
-0000b990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000b9a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000b9b0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000b9c0: 2020 2020 2069 6620 6272 6f61 6463 6173       if broadcas
-0000b9d0: 745f 6d61 7463 6865 7320 616e 6420 2873  t_matches and (s
-0000b9e0: 656c 662e 6469 6d65 6e73 696f 6e20 3d3d  elf.dimension ==
-0000b9f0: 2031 206f 7220 6f74 6865 722e 6469 6d65   1 or other.dime
-0000ba00: 6e73 696f 6e20 3d3d 2031 293a 0a20 2020  nsion == 1):.   
+0000a610: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+0000a620: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000a630: 7466 3a0a 2020 2020 2020 2020 2020 2020  tf:.            
+0000a640: 2020 2020 2020 2020 792e 706c 6163 6568          y.placeh
+0000a650: 6f6c 6465 7220 3d20 5f62 696e 5f6f 705f  older = _bin_op_
+0000a660: 7466 2879 2e70 6c61 6365 686f 6c64 6572  tf(y.placeholder
+0000a670: 2c20 782e 6469 6d65 6e73 696f 6e29 0a20  , x.dimension). 
+0000a680: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000a690: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000a6a0: 2020 2020 2020 2020 2079 203d 205f 6269           y = _bi
+0000a6b0: 6e5f 6f70 2879 2c20 782e 6469 6d65 6e73  n_op(y, x.dimens
+0000a6c0: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+0000a6d0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+0000a6e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000a6f0: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
+0000a700: 2020 2020 2020 2020 2078 203d 2078 2e67           x = x.g
+0000a710: 6574 5f66 6f72 5f62 6174 6368 5f63 7478  et_for_batch_ctx
+0000a720: 2873 656c 662e 6261 7463 682c 2073 656c  (self.batch, sel
+0000a730: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+0000a740: 7478 290a 2020 2020 2020 2020 2020 2020  tx).            
+0000a750: 782e 636f 6d70 6c65 7465 5f64 796e 5f73  x.complete_dyn_s
+0000a760: 697a 6528 7465 6d70 6c61 7465 5f6f 6e6c  ize(template_onl
+0000a770: 793d 7465 6d70 6c61 7465 5f6f 6e6c 7929  y=template_only)
+0000a780: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000a790: 6e6f 7420 782e 6479 6e5f 7369 7a65 5f65  not x.dyn_size_e
+0000a7a0: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+0000a7b0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000a7c0: 2020 2020 2020 2078 203d 2078 2e64 796e         x = x.dyn
+0000a7d0: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
+0000a7e0: 2020 2020 2020 6966 2079 2069 7320 4e6f        if y is No
+0000a7f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000a800: 2020 2020 7920 3d20 782e 636f 7079 286e      y = x.copy(n
+0000a810: 616d 653d 795f 6e61 6d65 290a 2020 2020  ame=y_name).    
+0000a820: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000a830: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000a840: 2069 6620 782e 6469 6d5f 7461 6773 2021   if x.dim_tags !
+0000a850: 3d20 792e 6469 6d5f 7461 6773 3a0a 2020  = y.dim_tags:.  
+0000a860: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000a870: 6d6d 6f6e 203d 205f 742e 5465 6e73 6f72  mmon = _t.Tensor
+0000a880: 2e67 6574 5f63 6f6d 6d6f 6e5f 6461 7461  .get_common_data
+0000a890: 285b 782c 2079 5d2c 2061 6c6c 6f77 5f62  ([x, y], allow_b
+0000a8a0: 726f 6164 6361 7374 5f61 6c6c 5f73 6f75  roadcast_all_sou
+0000a8b0: 7263 6573 3d54 7275 6529 0a20 2020 2020  rces=True).     
+0000a8c0: 2020 2020 2020 2020 2020 2078 5f20 3d20             x_ = 
+0000a8d0: 782e 636f 7079 5f63 6f6d 7061 7469 626c  x.copy_compatibl
+0000a8e0: 655f 746f 2863 6f6d 6d6f 6e29 2069 6620  e_to(common) if 
+0000a8f0: 782e 6469 6d5f 7461 6773 2065 6c73 6520  x.dim_tags else 
+0000a900: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+0000a910: 2020 795f 203d 2079 2e63 6f70 795f 636f    y_ = y.copy_co
+0000a920: 6d70 6174 6962 6c65 5f74 6f28 636f 6d6d  mpatible_to(comm
+0000a930: 6f6e 2920 6966 2079 2e64 696d 5f74 6167  on) if y.dim_tag
+0000a940: 7320 656c 7365 2079 0a20 2020 2020 2020  s else y.       
+0000a950: 2020 2020 2020 2020 2079 203d 2063 6f6d           y = com
+0000a960: 6d6f 6e0a 2020 2020 2020 2020 2020 2020  mon.            
+0000a970: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000a980: 2020 2020 2020 785f 2c20 795f 203d 2078        x_, y_ = x
+0000a990: 2c20 790a 2020 2020 2020 2020 2020 2020  , y.            
+0000a9a0: 6966 2074 663a 0a20 2020 2020 2020 2020  if tf:.         
+0000a9b0: 2020 2020 2020 2079 2e70 6c61 6365 686f         y.placeho
+0000a9c0: 6c64 6572 203d 205f 6269 6e5f 6f70 5f74  lder = _bin_op_t
+0000a9d0: 6628 795f 2e70 6c61 6365 686f 6c64 6572  f(y_.placeholder
+0000a9e0: 2c20 785f 2e70 6c61 6365 686f 6c64 6572  , x_.placeholder
+0000a9f0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000aa00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000aa10: 2020 2020 7920 3d20 5f62 696e 5f6f 7028      y = _bin_op(
+0000aa20: 795f 2c20 785f 290a 2020 2020 2020 2020  y_, x_).        
+0000aa30: 6173 7365 7274 2079 2c20 6622 6f70 207b  assert y, f"op {
+0000aa40: 6f70 7d3f 220a 2020 2020 2020 2020 6966  op}?".        if
+0000aa50: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+0000aa60: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+0000aa70: 6173 7365 7274 2073 656c 662e 6479 6e5f  assert self.dyn_
+0000aa80: 7369 7a65 5f65 7874 2e64 696d 5f74 6167  size_ext.dim_tag
+0000aa90: 7320 3d3d 2079 2e64 696d 5f74 6167 730a  s == y.dim_tags.
+0000aaa0: 2020 2020 2020 2020 6966 2079 2e62 6174          if y.bat
+0000aab0: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+0000aac0: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
+0000aad0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000aae0: 7373 6572 7420 7365 6c66 2e62 6174 6368  ssert self.batch
+0000aaf0: 203d 3d20 792e 6261 7463 680a 2020 2020   == y.batch.    
+0000ab00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ab10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ab20: 6c66 2e62 6174 6368 203d 2079 2e62 6174  lf.batch = y.bat
+0000ab30: 6368 0a20 2020 2020 2020 2073 656c 662e  ch.        self.
+0000ab40: 6479 6e5f 7369 7a65 5f65 7874 203d 2079  dyn_size_ext = y
+0000ab50: 0a20 2020 2020 2020 2069 6620 7466 2061  .        if tf a
+0000ab60: 6e64 2079 2e70 6c61 6365 686f 6c64 6572  nd y.placeholder
+0000ab70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000ab80: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000ab90: 6574 5f74 6167 5f6f 6e5f 7369 7a65 5f74  et_tag_on_size_t
+0000aba0: 656e 736f 7228 792e 706c 6163 6568 6f6c  ensor(y.placehol
+0000abb0: 6465 7229 0a0a 2020 2020 6465 6620 6973  der)..    def is
+0000abc0: 5f65 7175 616c 280a 2020 2020 2020 2020  _equal(.        
+0000abd0: 7365 6c66 2c0a 2020 2020 2020 2020 6f74  self,.        ot
+0000abe0: 6865 722c 0a20 2020 2020 2020 2069 676e  her,.        ign
+0000abf0: 6f72 655f 6665 6174 7572 655f 6469 6d3d  ore_feature_dim=
+0000ac00: 4661 6c73 652c 0a20 2020 2020 2020 2061  False,.        a
+0000ac10: 6c6c 6f77 5f73 616d 655f 6665 6174 7572  llow_same_featur
+0000ac20: 655f 6469 6d3d 4661 6c73 652c 0a20 2020  e_dim=False,.   
+0000ac30: 2020 2020 2061 6c6c 6f77 5f73 616d 655f       allow_same_
+0000ac40: 7370 6174 6961 6c5f 6469 6d3d 4e6f 6e65  spatial_dim=None
+0000ac50: 2c0a 2020 2020 2020 2020 7472 6561 745f  ,.        treat_
+0000ac60: 6665 6174 7572 655f 6173 5f73 7061 7469  feature_as_spati
+0000ac70: 616c 3d46 616c 7365 2c0a 2020 2020 2020  al=False,.      
+0000ac80: 2020 6272 6f61 6463 6173 745f 6d61 7463    broadcast_matc
+0000ac90: 6865 733d 4661 6c73 652c 0a20 2020 2020  hes=False,.     
+0000aca0: 2020 2075 6e6b 6e6f 776e 5f73 7061 7469     unknown_spati
+0000acb0: 616c 5f6d 6174 6368 6573 3d46 616c 7365  al_matches=False
+0000acc0: 2c0a 2020 2020 2020 2020 756e 6465 6669  ,.        undefi
+0000acd0: 6e65 645f 6d61 7463 6865 733d 4661 6c73  ned_matches=Fals
+0000ace0: 652c 0a20 2020 2020 2020 2064 6572 6976  e,.        deriv
+0000acf0: 6564 5f6d 6174 6368 6573 3d46 616c 7365  ed_matches=False
+0000ad00: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0000ad10: 2022 2222 0a20 2020 2020 2020 2043 6f6d   """.        Com
+0000ad20: 7061 7265 7320 7365 6c66 2074 6f20 6f74  pares self to ot
+0000ad30: 6865 7220 666f 7220 6571 7561 6c69 7479  her for equality
+0000ad40: 2e0a 0a20 2020 2020 2020 204e 6f74 6520  ...        Note 
+0000ad50: 7468 6174 2074 6865 2064 6566 6175 6c74  that the default
+0000ad60: 2062 6568 6176 696f 7220 6973 2076 6572   behavior is ver
+0000ad70: 7920 7265 7374 7269 6374 6976 652e 0a20  y restrictive.. 
+0000ad80: 2020 2020 2020 2055 7365 2066 756e 6374         Use funct
+0000ad90: 696f 6e73 2073 7563 6820 6173 203a 6675  ions such as :fu
+0000ada0: 6e63 3a60 6765 745f 616c 6c5f 6469 6d65  nc:`get_all_dime
+0000adb0: 6e73 696f 6e5f 7461 6773 6020 6f72 203a  nsion_tags` or :
+0000adc0: 6675 6e63 3a60 6765 745f 6578 6973 7469  func:`get_existi
+0000add0: 6e67 5f74 6167 5f66 726f 6d5f 636f 6c6c  ng_tag_from_coll
+0000ade0: 6563 7469 6f6e 600a 2020 2020 2020 2020  ection`.        
+0000adf0: 746f 2065 7870 6c69 6369 746c 7920 7370  to explicitly sp
+0000ae00: 6563 6966 7920 7468 6520 6265 6861 7669  ecify the behavi
+0000ae10: 6f72 2066 6f72 2074 6865 2063 6f6d 7061  or for the compa
+0000ae20: 7269 736f 6e2e 0a0a 2020 2020 2020 2020  rison...        
+0000ae30: 416c 736f 206e 6f74 6520 7468 6174 2074  Also note that t
+0000ae40: 6865 2064 6566 696e 6974 696f 6e20 6973  he definition is
+0000ae50: 2073 6c69 6768 746c 7920 6164 2d68 6f63   slightly ad-hoc
+0000ae60: 2066 6f72 2073 6f6d 6520 6361 7365 732c   for some cases,
+0000ae70: 0a20 2020 2020 2020 2061 6e64 206d 6967  .        and mig
+0000ae80: 6874 2070 6f74 656e 7469 616c 6c79 2063  ht potentially c
+0000ae90: 6861 6e67 6520 696e 2074 6865 2066 7574  hange in the fut
+0000aea0: 7572 652e 0a20 2020 2020 2020 2020 2068  ure..          h
+0000aeb0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000aec0: 6d2f 7277 7468 2d69 362f 7265 7475 726e  m/rwth-i6/return
+0000aed0: 6e2f 6973 7375 6573 2f36 3334 0a0a 2020  n/issues/634..  
+0000aee0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+0000aef0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+0000af00: 3a70 6172 616d 2062 6f6f 6c20 6967 6e6f  :param bool igno
+0000af10: 7265 5f66 6561 7475 7265 5f64 696d 3a0a  re_feature_dim:.
+0000af20: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+0000af30: 6f6f 6c20 616c 6c6f 775f 7361 6d65 5f66  ool allow_same_f
+0000af40: 6561 7475 7265 5f64 696d 3a0a 2020 2020  eature_dim:.    
+0000af50: 2020 2020 3a70 6172 616d 2062 6f6f 6c7c      :param bool|
+0000af60: 4e6f 6e65 2061 6c6c 6f77 5f73 616d 655f  None allow_same_
+0000af70: 7370 6174 6961 6c5f 6469 6d3a 0a20 2020  spatial_dim:.   
+0000af80: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
+0000af90: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
+0000afa0: 735f 7370 6174 6961 6c3a 0a20 2020 2020  s_spatial:.     
+0000afb0: 2020 203a 7061 7261 6d20 626f 6f6c 2062     :param bool b
+0000afc0: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
+0000afd0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+0000afe0: 2062 6f6f 6c20 756e 6b6e 6f77 6e5f 7370   bool unknown_sp
+0000aff0: 6174 6961 6c5f 6d61 7463 6865 733a 0a20  atial_matches:. 
+0000b000: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
+0000b010: 6f6c 2075 6e64 6566 696e 6564 5f6d 6174  ol undefined_mat
+0000b020: 6368 6573 3a0a 2020 2020 2020 2020 3a70  ches:.        :p
+0000b030: 6172 616d 2062 6f6f 6c20 6465 7269 7665  aram bool derive
+0000b040: 645f 6d61 7463 6865 733a 0a20 2020 2020  d_matches:.     
+0000b050: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+0000b060: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b070: 2020 2020 6672 6f6d 2072 6574 7572 6e6e      from returnn
+0000b080: 2e75 7469 6c20 696d 706f 7274 2042 6568  .util import Beh
+0000b090: 6176 696f 7256 6572 7369 6f6e 0a0a 2020  aviorVersion..  
+0000b0a0: 2020 2020 2020 6966 2073 656c 6620 6973        if self is
+0000b0b0: 206f 7468 6572 3a20 2023 2066 6972 7374   other:  # first
+0000b0c0: 2073 6f6d 6520 6661 7374 2070 6174 6820   some fast path 
+0000b0d0: 6368 6563 6b0a 2020 2020 2020 2020 2020  check.          
+0000b0e0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000b0f0: 2020 2020 2020 6966 2073 656c 662e 7370        if self.sp
+0000b100: 6563 6961 6c20 6f72 206f 7468 6572 2e73  ecial or other.s
+0000b110: 7065 6369 616c 3a0a 2020 2020 2020 2020  pecial:.        
+0000b120: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0000b130: 2020 2320 6f6e 6c79 2074 7275 6520 6966    # only true if
+0000b140: 2073 616d 6520 696e 7374 616e 6365 2c20   same instance, 
+0000b150: 6368 6563 6b20 6162 6f76 650a 2020 2020  check above.    
+0000b160: 2020 2020 6966 2061 6c6c 6f77 5f73 616d      if allow_sam
+0000b170: 655f 7370 6174 6961 6c5f 6469 6d20 6973  e_spatial_dim is
+0000b180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000b190: 2020 2061 6c6c 6f77 5f73 616d 655f 7370     allow_same_sp
+0000b1a0: 6174 6961 6c5f 6469 6d20 3d20 616c 6c6f  atial_dim = allo
+0000b1b0: 775f 7361 6d65 5f66 6561 7475 7265 5f64  w_same_feature_d
+0000b1c0: 696d 0a20 2020 2020 2020 2073 656c 665f  im.        self_
+0000b1d0: 6261 7365 203d 2073 656c 662e 6765 745f  base = self.get_
+0000b1e0: 7361 6d65 5f64 6572 6976 6564 5f62 6173  same_derived_bas
+0000b1f0: 6528 2920 6966 2064 6572 6976 6564 5f6d  e() if derived_m
+0000b200: 6174 6368 6573 2065 6c73 6520 7365 6c66  atches else self
+0000b210: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
+0000b220: 0a20 2020 2020 2020 206f 7468 6572 5f62  .        other_b
+0000b230: 6173 6520 3d20 6f74 6865 722e 6765 745f  ase = other.get_
+0000b240: 7361 6d65 5f64 6572 6976 6564 5f62 6173  same_derived_bas
+0000b250: 6528 2920 6966 2064 6572 6976 6564 5f6d  e() if derived_m
+0000b260: 6174 6368 6573 2065 6c73 6520 6f74 6865  atches else othe
+0000b270: 722e 6765 745f 7361 6d65 5f62 6173 6528  r.get_same_base(
+0000b280: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000b290: 665f 6261 7365 2069 7320 6f74 6865 725f  f_base is other_
+0000b2a0: 6261 7365 3a0a 2020 2020 2020 2020 2020  base:.          
+0000b2b0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000b2c0: 2020 2020 2020 6966 2073 656c 665f 6261        if self_ba
+0000b2d0: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
+0000b2e0: 6f70 2061 6e64 206f 7468 6572 5f62 6173  op and other_bas
+0000b2f0: 652e 6465 7269 7665 645f 6672 6f6d 5f6f  e.derived_from_o
+0000b300: 703a 0a20 2020 2020 2020 2020 2020 2069  p:.            i
+0000b310: 6620 7365 6c66 5f62 6173 652e 6465 7269  f self_base.deri
+0000b320: 7665 645f 6672 6f6d 5f6f 7020 3d3d 206f  ved_from_op == o
+0000b330: 7468 6572 5f62 6173 652e 6465 7269 7665  ther_base.derive
+0000b340: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
+0000b350: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000b360: 6e20 5472 7565 0a20 2020 2020 2020 2073  n True.        s
+0000b370: 656c 665f 6b69 6e64 203d 2073 656c 662e  elf_kind = self.
+0000b380: 6b69 6e64 0a20 2020 2020 2020 206f 7468  kind.        oth
+0000b390: 6572 5f6b 696e 6420 3d20 6f74 6865 722e  er_kind = other.
+0000b3a0: 6b69 6e64 0a20 2020 2020 2020 2069 6620  kind.        if 
+0000b3b0: 7365 6c66 5f6b 696e 6420 3d3d 206f 7468  self_kind == oth
+0000b3c0: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
+0000b3d0: 7065 732e 4665 6174 7572 6520 616e 6420  pes.Feature and 
+0000b3e0: 6967 6e6f 7265 5f66 6561 7475 7265 5f64  ignore_feature_d
+0000b3f0: 696d 3a0a 2020 2020 2020 2020 2020 2020  im:.            
+0000b400: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
+0000b410: 2020 2020 6966 2074 7265 6174 5f66 6561      if treat_fea
+0000b420: 7475 7265 5f61 735f 7370 6174 6961 6c3a  ture_as_spatial:
+0000b430: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
+0000b440: 6f74 653a 204e 6f20 6b69 6e64 2061 7420  ote: No kind at 
+0000b450: 616c 6c3a 2052 6569 6e74 6572 7072 6574  all: Reinterpret
+0000b460: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
+0000b470: 735f 7370 6174 6961 6c20 6120 6269 743a  s_spatial a bit:
+0000b480: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
+0000b490: 7373 756d 6520 7468 6174 2077 6520 7761  ssume that we wa
+0000b4a0: 6e74 2074 6865 6d20 616c 6c20 746f 2062  nt them all to b
+0000b4b0: 6520 6861 6e64 6c65 6420 7468 6520 7361  e handled the sa
+0000b4c0: 6d65 2c20 6e6f 206d 6174 7465 7220 7468  me, no matter th
+0000b4d0: 6520 6b69 6e64 2e0a 2020 2020 2020 2020  e kind..        
+0000b4e0: 2020 2020 2320 2845 7863 6570 7420 6f66      # (Except of
+0000b4f0: 2062 6174 6368 2064 696d 206b 696e 642c   batch dim kind,
+0000b500: 2077 6869 6368 2069 7320 7374 696c 6c20   which is still 
+0000b510: 6578 636c 7564 6564 2068 6572 652e 290a  excluded here.).
+0000b520: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000b530: 656c 665f 6b69 6e64 203d 3d20 4469 6d54  elf_kind == DimT
+0000b540: 7970 6573 2e46 6561 7475 7265 206f 7220  ypes.Feature or 
+0000b550: 6e6f 7420 7365 6c66 5f6b 696e 643a 0a20  not self_kind:. 
+0000b560: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b570: 656c 665f 6b69 6e64 203d 2044 696d 5479  elf_kind = DimTy
+0000b580: 7065 732e 5370 6174 6961 6c0a 2020 2020  pes.Spatial.    
+0000b590: 2020 2020 2020 2020 6966 206f 7468 6572          if other
+0000b5a0: 5f6b 696e 6420 3d3d 2044 696d 5479 7065  _kind == DimType
+0000b5b0: 732e 4665 6174 7572 6520 6f72 206e 6f74  s.Feature or not
+0000b5c0: 206f 7468 6572 5f6b 696e 643a 0a20 2020   other_kind:.   
+0000b5d0: 2020 2020 2020 2020 2020 2020 206f 7468               oth
+0000b5e0: 6572 5f6b 696e 6420 3d20 4469 6d54 7970  er_kind = DimTyp
+0000b5f0: 6573 2e53 7061 7469 616c 0a20 2020 2020  es.Spatial.     
+0000b600: 2020 2069 6620 7365 6c66 2e64 696d 656e     if self.dimen
+0000b610: 7369 6f6e 2021 3d20 6f74 6865 722e 6469  sion != other.di
+0000b620: 6d65 6e73 696f 6e3a 0a20 2020 2020 2020  mension:.       
+0000b630: 2020 2020 2069 6620 6272 6f61 6463 6173       if broadcas
+0000b640: 745f 6d61 7463 6865 7320 616e 6420 2873  t_matches and (s
+0000b650: 656c 662e 6469 6d65 6e73 696f 6e20 3d3d  elf.dimension ==
+0000b660: 2031 206f 7220 6f74 6865 722e 6469 6d65   1 or other.dime
+0000b670: 6e73 696f 6e20 3d3d 2031 293a 0a20 2020  nsion == 1):.   
+0000b680: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+0000b690: 7320 2023 2070 6173 7320 6f6e 0a20 2020  s  # pass on.   
+0000b6a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b6c0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+0000b6d0: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
+0000b6e0: 2021 3d20 6f74 6865 725f 6b69 6e64 3a0a   != other_kind:.
+0000b6f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b700: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0000b710: 2069 6620 7365 6c66 5f6b 696e 6420 3d3d   if self_kind ==
+0000b720: 206f 7468 6572 5f6b 696e 6420 3d3d 2044   other_kind == D
+0000b730: 696d 5479 7065 732e 4261 7463 683a 0a20  imTypes.Batch:. 
+0000b740: 2020 2020 2020 2020 2020 2023 204e 6f74             # Not
+0000b750: 653a 2054 6869 7320 6d69 6768 7420 6265  e: This might be
+0000b760: 2069 6e63 6f72 7265 6374 2069 6e20 736f   incorrect in so
+0000b770: 6d65 2063 6173 6573 2c0a 2020 2020 2020  me cases,.      
+0000b780: 2020 2020 2020 2320 652e 672e 2066 6f72        # e.g. for
+0000b790: 2062 6561 6d20 7365 6172 6368 2077 6865   beam search whe
+0000b7a0: 6e20 7765 2068 6176 6520 7468 6520 6265  n we have the be
+0000b7b0: 616d 2068 6964 6465 6e20 696e 2074 6865  am hidden in the
+0000b7c0: 2062 6174 6368 2064 696d 2c0a 2020 2020   batch dim,.    
+0000b7d0: 2020 2020 2020 2020 2320 6f72 2077 6865          # or whe
+0000b7e0: 6e20 7765 2075 7365 6420 4d65 7267 6544  n we used MergeD
+0000b7f0: 696d 734c 6179 6572 206f 6e20 7468 6520  imsLayer on the 
+0000b800: 6261 7463 6820 6178 6973 2c20 6f72 2073  batch axis, or s
+0000b810: 6f2e 0a20 2020 2020 2020 2020 2020 2023  o..            #
+0000b820: 2057 6520 6d69 6768 7420 6e65 6564 2074   We might need t
+0000b830: 6f20 6578 7465 6e64 2074 6865 206c 6f67  o extend the log
+0000b840: 6963 2068 6572 6520 6c61 7465 722e 0a20  ic here later.. 
+0000b850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000b860: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
+0000b870: 6620 4265 6861 7669 6f72 5665 7273 696f  f BehaviorVersio
+0000b880: 6e2e 6765 7428 2920 3e3d 2031 363a 0a20  n.get() >= 16:. 
+0000b890: 2020 2020 2020 2020 2020 2023 2045 6974             # Eit
+0000b8a0: 6865 7220 7365 6c66 206f 7220 6f74 6865  her self or othe
+0000b8b0: 7220 6973 2073 6f6d 6520 6469 6d20 7461  r is some dim ta
+0000b8c0: 6720 6578 706c 6963 6974 6c79 2063 7265  g explicitly cre
+0000b8d0: 6174 6564 2062 7920 7468 6520 7573 6572  ated by the user
+0000b8e0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+0000b8f0: 616e 6420 7468 6579 2061 7265 206e 6f74  and they are not
+0000b900: 2074 6865 2073 616d 652c 2073 6f20 7765   the same, so we
+0000b910: 206e 6576 6572 2074 7265 6174 2074 6865   never treat the
+0000b920: 6d20 6173 2065 7175 616c 2e0a 2020 2020  m as equal..    
+0000b930: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+0000b940: 656c 662e 6175 746f 5f67 656e 6572 6174  elf.auto_generat
+0000b950: 6564 206f 7220 6e6f 7420 6f74 6865 722e  ed or not other.
+0000b960: 6175 746f 5f67 656e 6572 6174 6564 3a0a  auto_generated:.
+0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b980: 6966 2062 726f 6164 6361 7374 5f6d 6174  if broadcast_mat
+0000b990: 6368 6573 2061 6e64 2028 0a20 2020 2020  ches and (.     
+0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0000b9b0: 7365 6c66 2e64 696d 656e 7369 6f6e 203d  self.dimension =
+0000b9c0: 3d20 3120 616e 6420 7365 6c66 2e61 7574  = 1 and self.aut
+0000b9d0: 6f5f 6765 6e65 7261 7465 6429 206f 7220  o_generated) or 
+0000b9e0: 286f 7468 6572 2e64 696d 656e 7369 6f6e  (other.dimension
+0000b9f0: 203d 3d20 3120 616e 6420 6f74 6865 722e   == 1 and other.
+0000ba00: 6175 746f 5f67 656e 6572 6174 6564 290a  auto_generated).
 0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba20: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-0000ba30: 2020 2020 2020 2020 2069 6620 756e 6b6e           if unkn
-0000ba40: 6f77 6e5f 7370 6174 6961 6c5f 6d61 7463  own_spatial_matc
-0000ba50: 6865 7320 616e 6420 2828 7365 6c66 2e64  hes and ((self.d
-0000ba60: 796e 5f73 697a 6520 6973 204e 6f6e 6529  yn_size is None)
-0000ba70: 206f 7220 286f 7468 6572 2e64 796e 5f73   or (other.dyn_s
-0000ba80: 697a 6520 6973 204e 6f6e 6529 293a 0a20  ize is None)):. 
-0000ba90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000baa0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-0000bab0: 2020 2020 2020 2069 6620 756e 6465 6669         if undefi
-0000bac0: 6e65 645f 6d61 7463 6865 7320 616e 6420  ned_matches and 
-0000bad0: 2873 656c 662e 756e 6465 6669 6e65 6420  (self.undefined 
-0000bae0: 6f72 206f 7468 6572 2e75 6e64 6566 696e  or other.undefin
-0000baf0: 6564 293a 0a20 2020 2020 2020 2020 2020  ed):.           
-0000bb00: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-0000bb10: 0a20 2020 2020 2020 2023 2049 6e20 7072  .        # In pr
-0000bb20: 696e 6369 706c 652c 2077 6520 776f 756c  inciple, we woul
-0000bb30: 6420 7761 6e74 2074 6f20 6368 6563 6b20  d want to check 
-0000bb40: 666f 7220 6964 656e 7469 7479 2028 7365  for identity (se
-0000bb50: 6c66 2069 7320 6f74 6865 7229 2e0a 2020  lf is other)..  
-0000bb60: 2020 2020 2020 2320 5765 2063 7572 7265        # We curre
-0000bb70: 6e74 6c79 2075 7365 2074 6865 2064 6573  ntly use the des
-0000bb80: 6372 6970 7469 6f6e 2062 6563 6175 7365  cription because
-0000bb90: 2074 6865 2069 6465 6e74 6974 7920 776f   the identity wo
-0000bba0: 756c 6420 6e6f 7420 6265 2074 6865 2073  uld not be the s
-0000bbb0: 616d 650a 2020 2020 2020 2020 2320 696e  ame.        # in
-0000bbc0: 2063 6173 6520 6f66 2074 656d 706c 6174   case of templat
-0000bbd0: 6520 636f 6e73 7472 7563 7469 6f6e 2077  e construction w
-0000bbe0: 6865 7265 2061 2064 696d 2074 6167 2069  here a dim tag i
-0000bbf0: 7320 6f6e 6365 2063 7265 6174 6564 2066  s once created f
-0000bc00: 6f72 2061 2074 656d 706c 6174 6520 6c61  or a template la
-0000bc10: 7965 722c 0a20 2020 2020 2020 2023 2061  yer,.        # a
-0000bc20: 6e64 2074 6865 6e20 6c61 7465 7220 6167  nd then later ag
-0000bc30: 6169 6e20 666f 7220 7468 6520 7265 616c  ain for the real
-0000bc40: 206c 6179 6572 2e0a 2020 2020 2020 2020   layer..        
-0000bc50: 6966 2073 656c 662e 6175 746f 5f67 656e  if self.auto_gen
-0000bc60: 6572 6174 6564 2061 6e64 206f 7468 6572  erated and other
-0000bc70: 2e61 7574 6f5f 6765 6e65 7261 7465 6420  .auto_generated 
-0000bc80: 616e 6420 7365 6c66 2e64 6573 6372 6970  and self.descrip
-0000bc90: 7469 6f6e 203d 3d20 6f74 6865 722e 6465  tion == other.de
-0000bca0: 7363 7269 7074 696f 6e3a 0a20 2020 2020  scription:.     
-0000bcb0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000bcc0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-0000bcd0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-0000bce0: 205f 5f65 715f 5f28 7365 6c66 2c20 6f74   __eq__(self, ot
-0000bcf0: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
-0000bd00: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-0000bd10: 2044 696d 206f 7468 6572 3a0a 2020 2020   Dim other:.    
-0000bd20: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-0000bd30: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0000bd40: 3a20 3a66 756e 633a 6069 735f 6571 7561  : :func:`is_equa
-0000bd50: 6c60 2077 6974 6820 6465 6661 756c 7420  l` with default 
-0000bd60: 6f70 7469 6f6e 730a 2020 2020 2020 2020  options.        
-0000bd70: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-0000bd80: 6f74 2069 7369 6e73 7461 6e63 6528 6f74  ot isinstance(ot
-0000bd90: 6865 722c 205f 642e 4469 6d29 3a0a 2020  her, _d.Dim):.  
-0000bda0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000bdb0: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
-0000bdc0: 6574 7572 6e20 7365 6c66 2e69 735f 6571  eturn self.is_eq
-0000bdd0: 7561 6c28 6f74 6865 7229 0a0a 2020 2020  ual(other)..    
-0000bde0: 6465 6620 5f5f 6e65 5f5f 2873 656c 663a  def __ne__(self:
-0000bdf0: 2044 696d 2c20 6f74 6865 723a 2044 696d   Dim, other: Dim
-0000be00: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000be10: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
-0000be20: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
-0000be30: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-0000be40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000be50: 2020 7265 7475 726e 206e 6f74 2028 7365    return not (se
-0000be60: 6c66 203d 3d20 6f74 6865 7229 0a0a 2020  lf == other)..  
-0000be70: 2020 6465 6620 5f5f 6861 7368 5f5f 2873    def __hash__(s
-0000be80: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000be90: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
-0000bea0: 3a20 696e 740a 2020 2020 2020 2020 3a72  : int.        :r
-0000beb0: 6574 7572 6e3a 2068 6173 682c 206d 6174  eturn: hash, mat
-0000bec0: 6368 696e 6720 746f 203a 6675 6e63 3a60  ching to :func:`
-0000bed0: 5f5f 6571 5f5f 600a 2020 2020 2020 2020  __eq__`.        
-0000bee0: 2222 220a 2020 2020 2020 2020 2320 5468  """.        # Th
-0000bef0: 6973 206d 7573 7420 6d61 7463 6820 7468  is must match th
-0000bf00: 6520 6265 6861 7669 6f72 2069 6e20 5f5f  e behavior in __
-0000bf10: 6571 5f5f 2c20 7768 6963 6820 6973 2069  eq__, which is i
-0000bf20: 735f 6571 7561 6c20 7769 7468 2064 6566  s_equal with def
-0000bf30: 6175 6c74 206f 7074 696f 6e73 2e0a 2020  ault options..  
-0000bf40: 2020 2020 2020 2320 492e 652e 2064 6966        # I.e. dif
-0000bf50: 6665 7265 6e74 2068 6173 6820 696d 706c  ferent hash impl
-0000bf60: 6965 7320 6e6f 7420 6571 7561 6c20 2862  ies not equal (b
-0000bf70: 7574 2073 616d 6520 6861 7368 206e 6f74  ut same hash not
-0000bf80: 206e 6563 6573 7361 7269 6c79 2065 7175   necessarily equ
-0000bf90: 616c 292e 0a20 2020 2020 2020 2069 6620  al)..        if 
-0000bfa0: 7365 6c66 2e73 7065 6369 616c 3a0a 2020  self.special:.  
-0000bfb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000bfc0: 2068 6173 6828 6964 2873 656c 6629 290a   hash(id(self)).
-0000bfd0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000bfe0: 6973 5f62 6174 6368 5f64 696d 2829 3a0a  is_batch_dim():.
-0000bff0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c000: 726e 2068 6173 6828 2829 290a 2020 2020  rn hash(()).    
-0000c010: 2020 2020 7769 7468 2075 7469 6c2e 6775      with util.gu
-0000c020: 6172 645f 696e 6669 6e69 7465 5f72 6563  ard_infinite_rec
-0000c030: 7572 7369 6f6e 285f 642e 4469 6d2e 5f5f  ursion(_d.Dim.__
-0000c040: 6861 7368 5f5f 2c20 7365 6c66 293a 0a20  hash__, self):. 
-0000c050: 2020 2020 2020 2020 2020 2062 6173 6520             base 
-0000c060: 3d20 7365 6c66 2e67 6574 5f73 616d 655f  = self.get_same_
-0000c070: 6261 7365 2829 0a20 2020 2020 2020 2020  base().         
-0000c080: 2020 2069 6620 6261 7365 2069 7320 6e6f     if base is no
-0000c090: 7420 7365 6c66 3a0a 2020 2020 2020 2020  t self:.        
-0000c0a0: 2020 2020 2020 2020 7265 7475 726e 2068          return h
-0000c0b0: 6173 6828 6261 7365 290a 2020 2020 2020  ash(base).      
-0000c0c0: 2020 2020 2020 6966 2073 656c 662e 6465        if self.de
-0000c0d0: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000c0f0: 6574 7572 6e20 6861 7368 2873 656c 662e  eturn hash(self.
-0000c100: 6465 7269 7665 645f 6672 6f6d 5f6f 7029  derived_from_op)
-0000c110: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c120: 7365 6c66 2e61 7574 6f5f 6765 6e65 7261  self.auto_genera
-0000c130: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
-0000c140: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
-0000c150: 2828 6261 7365 2e6b 696e 642c 2062 6173  ((base.kind, bas
-0000c160: 652e 6469 6d65 6e73 696f 6e2c 2062 6173  e.dimension, bas
-0000c170: 652e 6465 7363 7269 7074 696f 6e29 290a  e.description)).
-0000c180: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c190: 726e 2068 6173 6828 6964 2862 6173 6529  rn hash(id(base)
-0000c1a0: 290a 0a20 2020 2064 6566 205f 5f6c 745f  )..    def __lt_
-0000c1b0: 5f28 7365 6c66 3a20 4469 6d2c 206f 7468  _(self: Dim, oth
-0000c1c0: 6572 3a20 4469 6d29 3a0a 2020 2020 2020  er: Dim):.      
-0000c1d0: 2020 2222 220a 2020 2020 2020 2020 4465    """.        De
-0000c1e0: 6669 6e65 2073 6f6d 6520 6f72 6465 722e  fine some order.
-0000c1f0: 2054 6869 7320 6973 206a 7573 7420 7375   This is just su
-0000c200: 6368 2074 6861 7420 6073 6f72 7465 6460  ch that `sorted`
-0000c210: 2077 6f72 6b73 2c20 6f72 2073 6f6d 6520   works, or some 
-0000c220: 6469 6666 2072 6570 6f72 7469 6e67 2c20  diff reporting, 
-0000c230: 6f72 2073 6f2e 0a20 2020 2020 2020 2049  or so..        I
-0000c240: 7420 6973 206f 6e20 7379 6d62 6f6c 6963  t is on symbolic
-0000c250: 206c 6576 656c 2c20 692e 652e 2069 7420   level, i.e. it 
-0000c260: 646f 6573 206e 6f74 2063 6f6e 7369 6465  does not conside
-0000c270: 7220 7468 6520 6163 7475 616c 2064 696d  r the actual dim
-0000c280: 656e 7369 6f6e 2076 616c 7565 2e0a 2020  ension value..  
-0000c290: 2020 2020 2020 5468 6520 6465 6669 6e65        The define
-0000c2a0: 6420 6f72 6465 7220 736f 6d65 7768 6174  d order somewhat
-0000c2b0: 2061 7262 6974 7261 7279 2c20 736f 2064   arbitrary, so d
-0000c2c0: 6f20 6e6f 7420 7265 6c79 206f 6e20 7468  o not rely on th
-0000c2d0: 6520 6578 6163 7420 6265 6861 7669 6f72  e exact behavior
-0000c2e0: 2c0a 2020 2020 2020 2020 6173 2074 6869  ,.        as thi
-0000c2f0: 7320 6d69 6768 7420 6368 616e 6765 2061  s might change a
-0000c300: 7420 736f 6d65 206c 6174 6572 2070 6f69  t some later poi
-0000c310: 6e74 2e0a 2020 2020 2020 2020 4375 7272  nt..        Curr
-0000c320: 656e 746c 792c 2069 7420 6465 7065 6e64  ently, it depend
-0000c330: 7320 6f6e 2074 6865 2063 7265 6174 696f  s on the creatio
-0000c340: 6e20 696e 6465 782e 0a0a 2020 2020 2020  n index...      
-0000c350: 2020 3a70 6172 616d 2044 696d 206f 7468    :param Dim oth
-0000c360: 6572 3a0a 2020 2020 2020 2020 3a72 7479  er:.        :rty
-0000c370: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-0000c380: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-0000c390: 6e6f 7420 6973 696e 7374 616e 6365 286f  not isinstance(o
-0000c3a0: 7468 6572 2c20 285f 642e 4469 6d2c 205f  ther, (_d.Dim, _
-0000c3b0: 6d2e 4d61 726b 6564 4469 6d29 293a 0a20  m.MarkedDim)):. 
-0000c3c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000c3d0: 2054 7970 6545 7272 6f72 2822 6361 6e6e   TypeError("cann
-0000c3e0: 6f74 2063 6f6d 7061 7265 2025 7220 7769  ot compare %r wi
-0000c3f0: 7468 2025 7222 2025 2028 7365 6c66 2c20  th %r" % (self, 
-0000c400: 6f74 6865 7229 290a 2020 2020 2020 2020  other)).        
-0000c410: 6966 2073 656c 6620 3d3d 206f 7468 6572  if self == other
-0000c420: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000c430: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-0000c440: 2020 2072 6574 7572 6e20 6469 6d5f 636d     return dim_cm
-0000c450: 705f 7661 6c75 6528 7365 6c66 2920 3c20  p_value(self) < 
-0000c460: 6469 6d5f 636d 705f 7661 6c75 6528 6f74  dim_cmp_value(ot
-0000c470: 6865 7229 0a0a 2020 2020 6465 6620 5f5f  her)..    def __
-0000c480: 6774 5f5f 2873 656c 662c 206f 7468 6572  gt__(self, other
-0000c490: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000c4a0: 2020 2020 2020 2053 6565 203a 6675 6e63         See :func
-0000c4b0: 3a60 5f5f 6c74 5f5f 602e 0a0a 2020 2020  :`__lt__`...    
-0000c4c0: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
-0000c4d0: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
-0000c4e0: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
-0000c4f0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000c500: 6574 7572 6e20 6f74 6865 7220 3c20 7365  eturn other < se
-0000c510: 6c66 0a0a 2020 2020 6465 6620 5f5f 6765  lf..    def __ge
-0000c520: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-0000c530: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c540: 6e6f 7420 7365 6c66 203c 206f 7468 6572  not self < other
-0000c550: 0a0a 2020 2020 6465 6620 5f5f 6c65 5f5f  ..    def __le__
-0000c560: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
-0000c570: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
-0000c580: 7420 7365 6c66 203e 206f 7468 6572 0a0a  t self > other..
-0000c590: 2020 2020 6465 6620 6765 745f 7361 6d65      def get_same
-0000c5a0: 5f62 6173 6528 7365 6c66 3a20 5f64 2e44  _base(self: _d.D
-0000c5b0: 696d 2920 2d3e 205f 642e 4469 6d3a 0a20  im) -> _d.Dim:. 
-0000c5c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c5d0: 2020 203a 7265 7475 726e 3a20 7361 6d65     :return: same
-0000c5e0: 2062 6173 650a 2020 2020 2020 2020 2222   base.        ""
-0000c5f0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-0000c600: 2073 656c 662e 5f65 7874 7261 3a0a 2020   self._extra:.  
-0000c610: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c620: 2073 656c 660a 2020 2020 2020 2020 6261   self.        ba
-0000c630: 7365 203d 2073 656c 660a 2020 2020 2020  se = self.      
-0000c640: 2020 7768 696c 6520 6261 7365 2e73 616d    while base.sam
-0000c650: 655f 6173 3a0a 2020 2020 2020 2020 2020  e_as:.          
-0000c660: 2020 6261 7365 203d 2062 6173 652e 7361    base = base.sa
-0000c670: 6d65 5f61 730a 2020 2020 2020 2020 7265  me_as.        re
-0000c680: 7475 726e 2062 6173 650a 0a20 2020 2064  turn base..    d
-0000c690: 6566 2067 6574 5f73 616d 655f 6465 7269  ef get_same_deri
-0000c6a0: 7665 645f 6261 7365 2873 656c 663a 205f  ved_base(self: _
-0000c6b0: 642e 4469 6d29 202d 3e20 5f64 2e44 696d  d.Dim) -> _d.Dim
-0000c6c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000c6d0: 2020 2020 2020 3a72 6574 7572 6e3a 2073        :return: s
-0000c6e0: 616d 6520 6261 7365 2c20 6275 7420 616c  ame base, but al
-0000c6f0: 736f 2063 6f6e 7369 6465 7220 6465 7269  so consider deri
-0000c700: 7665 645f 6672 6f6d 5f2e 2e2e 0a20 2020  ved_from_....   
-0000c710: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c720: 2062 6173 6520 3d20 7365 6c66 0a20 2020   base = self.   
-0000c730: 2020 2020 2076 6973 6974 6564 203d 207b       visited = {
-0000c740: 7d0a 2020 2020 2020 2020 7768 696c 6520  }.        while 
-0000c750: 6261 7365 2e73 616d 655f 6173 206f 7220  base.same_as or 
-0000c760: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
-0000c770: 6d5f 7461 673a 0a20 2020 2020 2020 2020  m_tag:.         
-0000c780: 2020 2061 7373 6572 7420 6964 2862 6173     assert id(bas
-0000c790: 6529 206e 6f74 2069 6e20 7669 7369 7465  e) not in visite
-0000c7a0: 6420 2023 2073 686f 756c 6420 6e6f 7420  d  # should not 
-0000c7b0: 6861 7665 2063 7963 6c65 732e 206e 6f72  have cycles. nor
-0000c7c0: 6d61 6c6c 7920 7468 6973 2073 686f 756c  mally this shoul
-0000c7d0: 6420 6e65 7665 7220 6265 2074 7269 6767  d never be trigg
-0000c7e0: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
-0000c7f0: 2076 6973 6974 6564 5b69 6428 6261 7365   visited[id(base
-0000c800: 295d 203d 2062 6173 650a 2020 2020 2020  )] = base.      
-0000c810: 2020 2020 2020 6966 2062 6173 652e 7361        if base.sa
-0000c820: 6d65 5f61 733a 0a20 2020 2020 2020 2020  me_as:.         
-0000c830: 2020 2020 2020 2062 6173 6520 3d20 6261         base = ba
-0000c840: 7365 2e73 616d 655f 6173 0a20 2020 2020  se.same_as.     
-0000c850: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000c860: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-0000c870: 6261 7365 203d 2062 6173 652e 6465 7269  base = base.deri
-0000c880: 7665 645f 6672 6f6d 5f74 6167 0a20 2020  ved_from_tag.   
-0000c890: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000c8a0: 6261 7365 0a20 2020 2020 2020 2072 6574  base.        ret
-0000c8b0: 7572 6e20 6261 7365 0a0a 2020 2020 6465  urn base..    de
-0000c8c0: 6620 6765 745f 6465 7269 7665 645f 6261  f get_derived_ba
-0000c8d0: 7365 735f 7365 7428 7365 6c66 293a 0a20  ses_set(self):. 
-0000c8e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c8f0: 2020 203a 7274 7970 653a 2073 6574 5b44     :rtype: set[D
-0000c900: 696d 5d0a 2020 2020 2020 2020 2222 220a  im].        """.
-0000c910: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-0000c920: 7428 290a 2020 2020 2020 2020 7175 6575  t().        queu
-0000c930: 6520 3d20 5b73 656c 665d 0a20 2020 2020  e = [self].     
-0000c940: 2020 2076 6973 6974 6564 203d 207b 7d20     visited = {} 
-0000c950: 2023 2074 7970 653a 2044 6963 745b 696e   # type: Dict[in
-0000c960: 742c 5f64 2e44 696d 5d20 2023 2062 7920  t,_d.Dim]  # by 
-0000c970: 6964 0a20 2020 2020 2020 2077 6869 6c65  id.        while
-0000c980: 2071 7565 7565 3a0a 2020 2020 2020 2020   queue:.        
-0000c990: 2020 2020 6261 7365 203d 2071 7565 7565      base = queue
-0000c9a0: 2e70 6f70 282d 3129 0a20 2020 2020 2020  .pop(-1).       
-0000c9b0: 2020 2020 2069 6620 6261 7365 2e73 616d       if base.sam
-0000c9c0: 655f 6173 3a0a 2020 2020 2020 2020 2020  e_as:.          
-0000c9d0: 2020 2020 2020 6261 7365 203d 2062 6173        base = bas
-0000c9e0: 652e 7361 6d65 5f61 730a 2020 2020 2020  e.same_as.      
-0000c9f0: 2020 2020 2020 6966 2069 6428 6261 7365        if id(base
-0000ca00: 2920 696e 2076 6973 6974 6564 3a0a 2020  ) in visited:.  
-0000ca10: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000ca20: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-0000ca30: 2020 2076 6973 6974 6564 5b69 6428 6261     visited[id(ba
-0000ca40: 7365 295d 203d 2062 6173 650a 2020 2020  se)] = base.    
-0000ca50: 2020 2020 2020 2020 7265 732e 6164 6428          res.add(
-0000ca60: 6261 7365 290a 2020 2020 2020 2020 2020  base).          
-0000ca70: 2020 6966 2062 6173 652e 6465 7269 7665    if base.derive
-0000ca80: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
-0000ca90: 2020 2020 2020 2020 2020 2071 7565 7565             queue
-0000caa0: 2e65 7874 656e 6428 6261 7365 2e64 6572  .extend(base.der
-0000cab0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-0000cac0: 7574 7329 0a20 2020 2020 2020 2020 2020  uts).           
-0000cad0: 2065 6c69 6620 6261 7365 2e64 6572 6976   elif base.deriv
-0000cae0: 6564 5f66 726f 6d5f 7461 673a 0a20 2020  ed_from_tag:.   
-0000caf0: 2020 2020 2020 2020 2020 2020 2071 7565               que
-0000cb00: 7565 2e61 7070 656e 6428 6261 7365 2e64  ue.append(base.d
-0000cb10: 6572 6976 6564 5f66 726f 6d5f 7461 6729  erived_from_tag)
-0000cb20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000cb30: 7265 730a 0a20 2020 2040 7072 6f70 6572  res..    @proper
-0000cb40: 7479 0a20 2020 2064 6566 2075 6e64 6566  ty.    def undef
-0000cb50: 696e 6564 2873 656c 663a 205f 642e 4469  ined(self: _d.Di
-0000cb60: 6d29 202d 3e20 626f 6f6c 3a0a 2020 2020  m) -> bool:.    
-0000cb70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000cb80: 3a72 6574 7572 6e3a 2077 6865 7468 6572  :return: whether
-0000cb90: 2074 6865 2075 6e64 6566 696e 6564 2066   the undefined f
-0000cba0: 6c61 6720 6973 2073 6574 2c20 696e 2073  lag is set, in s
-0000cbb0: 656c 662c 2062 6173 6573 2c20 6f72 2061  elf, bases, or a
-0000cbc0: 6e79 2064 6572 6976 6564 2062 6173 6573  ny derived bases
-0000cbd0: 2e20 616c 736f 2073 6565 203a 6675 6e63  . also see :func
-0000cbe0: 3a60 6973 5f64 696d 5f6b 6e6f 776e 600a  :`is_dim_known`.
-0000cbf0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000cc00: 2020 2020 6261 7365 203d 2073 656c 660a      base = self.
-0000cc10: 2020 2020 2020 2020 7669 7369 7465 6420          visited 
-0000cc20: 3d20 7b7d 0a20 2020 2020 2020 2077 6869  = {}.        whi
-0000cc30: 6c65 2062 6173 652e 7361 6d65 5f61 7320  le base.same_as 
-0000cc40: 6f72 2062 6173 652e 6465 7269 7665 645f  or base.derived_
-0000cc50: 6672 6f6d 5f74 6167 3a0a 2020 2020 2020  from_tag:.      
-0000cc60: 2020 2020 2020 6173 7365 7274 2069 6428        assert id(
-0000cc70: 6261 7365 2920 6e6f 7420 696e 2076 6973  base) not in vis
-0000cc80: 6974 6564 2020 2320 7368 6f75 6c64 206e  ited  # should n
-0000cc90: 6f74 2068 6176 6520 6379 636c 6573 2e20  ot have cycles. 
-0000cca0: 6e6f 726d 616c 6c79 2074 6869 7320 7368  normally this sh
-0000ccb0: 6f75 6c64 206e 6576 6572 2062 6520 7472  ould never be tr
-0000ccc0: 6967 6765 7265 640a 2020 2020 2020 2020  iggered.        
-0000ccd0: 2020 2020 7669 7369 7465 645b 6964 2862      visited[id(b
-0000cce0: 6173 6529 5d20 3d20 6261 7365 0a20 2020  ase)] = base.   
-0000ccf0: 2020 2020 2020 2020 2023 206e 6f69 6e73           # noins
-0000cd00: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
-0000cd10: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
-0000cd20: 2020 2020 2020 6966 2062 6173 652e 5f65        if base._e
-0000cd30: 7874 7261 2061 6e64 2062 6173 652e 5f65  xtra and base._e
-0000cd40: 7874 7261 2e75 6e64 6566 696e 6564 3a0a  xtra.undefined:.
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd60: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000cd70: 2020 2020 2020 2020 6966 2062 6173 652e          if base.
-0000cd80: 7361 6d65 5f61 733a 0a20 2020 2020 2020  same_as:.       
-0000cd90: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0000cda0: 6261 7365 2e73 616d 655f 6173 0a20 2020  base.same_as.   
-0000cdb0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000cdc0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-0000cdd0: 2020 6261 7365 203d 2062 6173 652e 6465    base = base.de
-0000cde0: 7269 7665 645f 6672 6f6d 5f74 6167 0a20  rived_from_tag. 
-0000cdf0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000ce00: 7420 6261 7365 0a20 2020 2020 2020 2023  t base.        #
-0000ce10: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-0000ce20: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
-0000ce30: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-0000ce40: 6173 652e 5f65 7874 7261 2061 6e64 2062  ase._extra and b
-0000ce50: 6173 652e 5f65 7874 7261 2e75 6e64 6566  ase._extra.undef
-0000ce60: 696e 6564 0a0a 2020 2020 6465 6620 6465  ined..    def de
-0000ce70: 636c 6172 655f 7361 6d65 5f61 7328 7365  clare_same_as(se
-0000ce80: 6c66 3a20 5f64 2e44 696d 2c20 6f74 6865  lf: _d.Dim, othe
-0000ce90: 723a 205f 642e 4469 6d29 3a0a 2020 2020  r: _d.Dim):.    
-0000cea0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ceb0: 3a70 6172 616d 206f 7468 6572 3a0a 2020  :param other:.  
-0000cec0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000ced0: 2020 6173 7365 7274 2073 656c 662e 6361    assert self.ca
-0000cee0: 6e5f 6265 5f75 7365 645f 6173 5f64 696d  n_be_used_as_dim
-0000cef0: 2829 2061 6e64 206f 7468 6572 2e63 616e  () and other.can
-0000cf00: 5f62 655f 7573 6564 5f61 735f 6469 6d28  _be_used_as_dim(
-0000cf10: 2920 2023 2064 6563 6c61 7265 5f73 616d  )  # declare_sam
-0000cf20: 655f 6173 2064 6f65 7320 6e6f 7420 6d61  e_as does not ma
-0000cf30: 6b65 2073 656e 7365 206f 7468 6572 7769  ke sense otherwi
-0000cf40: 7365 0a20 2020 2020 2020 2023 204e 6f74  se.        # Not
-0000cf50: 653a 2043 6865 636b 2060 6973 602c 206e  e: Check `is`, n
-0000cf60: 6f74 2060 3d3d 602e 2060 3d3d 6020 6361  ot `==`. `==` ca
-0000cf70: 6e20 6265 2074 7275 6520 6576 656e 2074  n be true even t
-0000cf80: 686f 7567 6820 7361 6d65 5f61 7320 6172  hough same_as ar
-0000cf90: 6520 6e6f 7420 7468 6520 7361 6d65 2069  e not the same i
-0000cfa0: 6e73 7461 6e63 652c 0a20 2020 2020 2020  nstance,.       
-0000cfb0: 2023 2065 2e67 2e20 7669 6120 6175 746f   # e.g. via auto
-0000cfc0: 5f67 656e 6572 6174 6564 2e0a 2020 2020  _generated..    
-0000cfd0: 2020 2020 6966 2073 656c 6620 6973 206f      if self is o
-0000cfe0: 7468 6572 3a0a 2020 2020 2020 2020 2020  ther:.          
-0000cff0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000d000: 2073 656c 662e 5f6d 6179 6265 5f75 7064   self._maybe_upd
-0000d010: 6174 6528 290a 2020 2020 2020 2020 7365  ate().        se
-0000d020: 6c66 2e5f 7661 6c69 6461 7465 5f69 6e5f  lf._validate_in_
-0000d030: 6375 7272 656e 745f 6772 6170 6828 290a  current_graph().
-0000d040: 2020 2020 2020 2020 6f74 6865 722e 5f76          other._v
-0000d050: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
-0000d060: 6e74 5f67 7261 7068 2829 0a20 2020 2020  nt_graph().     
-0000d070: 2020 206f 7468 6572 5f73 616d 655f 6261     other_same_ba
-0000d080: 7365 203d 206f 7468 6572 2e67 6574 5f73  se = other.get_s
-0000d090: 616d 655f 6261 7365 2829 0a20 2020 2020  ame_base().     
-0000d0a0: 2020 2069 6620 7365 6c66 2069 7320 6f74     if self is ot
-0000d0b0: 6865 725f 7361 6d65 5f62 6173 6520 6f72  her_same_base or
-0000d0c0: 2073 656c 662e 7361 6d65 5f61 7320 6973   self.same_as is
-0000d0d0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000d0e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000d0f0: 7475 726e 0a20 2020 2020 2020 2073 656c  turn.        sel
-0000d100: 665f 7361 6d65 5f61 7320 3d20 7365 6c66  f_same_as = self
-0000d110: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
-0000d120: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000d130: 5f73 616d 655f 6173 2069 7320 6f74 6865  _same_as is othe
-0000d140: 725f 7361 6d65 5f62 6173 653a 0a20 2020  r_same_base:.   
-0000d150: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000d160: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-0000d170: 5f73 616d 655f 6261 7365 2e67 6574 5f73  _same_base.get_s
-0000d180: 616d 655f 6465 7269 7665 645f 6261 7365  ame_derived_base
-0000d190: 2829 2069 7320 7365 6c66 5f73 616d 655f  () is self_same_
-0000d1a0: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
-0000d1b0: 2320 5765 2061 6374 7561 6c6c 7920 7761  # We actually wa
-0000d1c0: 6e74 2069 7420 746f 2062 6520 7468 6520  nt it to be the 
-0000d1d0: 6f74 6865 7220 7761 7920 6172 6f75 6e64  other way around
-0000d1e0: 2e0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-0000d1f0: 7468 2075 7469 6c2e 6775 6172 645f 696e  th util.guard_in
-0000d200: 6669 6e69 7465 5f72 6563 7572 7369 6f6e  finite_recursion
-0000d210: 285f 642e 4469 6d2e 6465 636c 6172 655f  (_d.Dim.declare_
-0000d220: 7361 6d65 5f61 732c 206f 7468 6572 2c20  same_as, other, 
-0000d230: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
-0000d240: 2020 2020 2020 2072 6574 7572 6e20 6f74         return ot
-0000d250: 6865 722e 6465 636c 6172 655f 7361 6d65  her.declare_same
-0000d260: 5f61 7328 7365 6c66 290a 2020 2020 2020  _as(self).      
-0000d270: 2020 6966 2073 656c 662e 6261 7463 683a    if self.batch:
-0000d280: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
-0000d290: 6620 7365 6c66 2069 7320 6465 6669 6e65  f self is define
-0000d2a0: 6420 2873 656c 662e 6973 5f64 696d 5f6b  d (self.is_dim_k
-0000d2b0: 6e6f 776e 292c 2062 6520 6661 6972 2074  nown), be fair t
-0000d2c0: 6f20 6f74 6865 722c 2061 6e64 2061 6461  o other, and ada
-0000d2d0: 7074 2069 7420 746f 2074 6865 2072 6967  pt it to the rig
-0000d2e0: 6874 2062 6174 6368 2c0a 2020 2020 2020  ht batch,.      
-0000d2f0: 2020 2020 2020 2320 7375 6368 2074 6861        # such tha
-0000d300: 7420 6f74 6865 722e 6973 5f64 696d 5f6b  t other.is_dim_k
-0000d310: 6e6f 776e 2069 7320 636f 7272 6563 742c  nown is correct,
-0000d320: 2062 7920 706f 7465 6e74 6961 6c6c 7920   by potentially 
-0000d330: 636f 6d70 6c65 7469 6e67 2069 742e 0a20  completing it.. 
-0000d340: 2020 2020 2020 2020 2020 206f 7468 6572             other
-0000d350: 5f20 3d20 6f74 6865 722e 6765 745f 666f  _ = other.get_fo
-0000d360: 725f 6261 7463 685f 6374 7828 7365 6c66  r_batch_ctx(self
-0000d370: 2e62 6174 6368 2c20 6374 783d 7365 6c66  .batch, ctx=self
-0000d380: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000d390: 7829 0a20 2020 2020 2020 2065 6c73 653a  x).        else:
-0000d3a0: 0a20 2020 2020 2020 2020 2020 206f 7468  .            oth
-0000d3b0: 6572 5f20 3d20 6f74 6865 720a 2020 2020  er_ = other.    
-0000d3c0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-0000d3d0: 2020 2020 2028 7365 6c66 2e69 735f 6469       (self.is_di
-0000d3e0: 6d5f 6b6e 6f77 6e28 2920 616e 6420 6e6f  m_known() and no
-0000d3f0: 7420 6f74 6865 725f 2e69 735f 6469 6d5f  t other_.is_dim_
-0000d400: 6b6e 6f77 6e28 2929 0a20 2020 2020 2020  known()).       
-0000d410: 2020 2020 206f 720a 2020 2020 2020 2020       or.        
-0000d420: 2020 2020 2320 4c69 6b65 2069 735f 6469      # Like is_di
-0000d430: 6d5f 6b6e 6f77 6e20 6275 7420 666f 7220  m_known but for 
-0000d440: 7374 6174 6963 2064 696d 732c 2077 6520  static dims, we 
-0000d450: 6d69 6768 7420 6b6e 6f77 2062 6f74 682c  might know both,
-0000d460: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
-0000d470: 7574 2074 6865 2064 6572 6976 6564 5f66  ut the derived_f
-0000d480: 726f 6d5f 6f70 2073 7469 6c6c 2077 6f75  rom_op still wou
-0000d490: 6c64 2070 726f 7669 6465 206d 6f72 6520  ld provide more 
-0000d4a0: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
-0000d4b0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-0000d4c0: 2020 2020 2020 2020 2020 2073 656c 665f             self_
-0000d4d0: 7361 6d65 5f61 732e 6465 7269 7665 645f  same_as.derived_
-0000d4e0: 6672 6f6d 5f6f 700a 2020 2020 2020 2020  from_op.        
-0000d4f0: 2020 2020 2020 2020 616e 6420 6e6f 7420          and not 
-0000d500: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
-0000d510: 6465 7269 7665 645f 6672 6f6d 5f6f 700a  derived_from_op.
-0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d530: 616e 6420 6f74 6865 7220 6e6f 7420 696e  and other not in
-0000d540: 2073 656c 662e 6765 745f 6465 7269 7665   self.get_derive
-0000d550: 645f 6261 7365 735f 7365 7428 290a 2020  d_bases_set().  
-0000d560: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d570: 2020 2020 2020 2020 6f72 2028 6e6f 7420          or (not 
-0000d580: 7365 6c66 2e75 6e64 6566 696e 6564 2061  self.undefined a
-0000d590: 6e64 206f 7468 6572 5f2e 756e 6465 6669  nd other_.undefi
-0000d5a0: 6e65 6429 0a20 2020 2020 2020 2029 3a0a  ned).        ):.
-0000d5b0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000d5c0: 2075 7469 6c2e 6775 6172 645f 696e 6669   util.guard_infi
-0000d5d0: 6e69 7465 5f72 6563 7572 7369 6f6e 285f  nite_recursion(_
-0000d5e0: 642e 4469 6d2e 6465 636c 6172 655f 7361  d.Dim.declare_sa
-0000d5f0: 6d65 5f61 732c 206f 7468 6572 2c20 7365  me_as, other, se
-0000d600: 6c66 293a 0a20 2020 2020 2020 2020 2020  lf):.           
-0000d610: 2020 2020 2072 6574 7572 6e20 6f74 6865       return othe
-0000d620: 722e 6465 636c 6172 655f 7361 6d65 5f61  r.declare_same_a
-0000d630: 7328 7365 6c66 290a 2020 2020 2020 2020  s(self).        
-0000d640: 6f74 6865 725f 6465 7269 7665 645f 6261  other_derived_ba
-0000d650: 7365 7320 3d20 6f74 6865 722e 6765 745f  ses = other.get_
-0000d660: 6465 7269 7665 645f 6261 7365 735f 7365  derived_bases_se
-0000d670: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-0000d680: 5f64 6572 6976 6564 5f62 6173 6573 203d  _derived_bases =
-0000d690: 2073 656c 662e 6765 745f 6465 7269 7665   self.get_derive
-0000d6a0: 645f 6261 7365 735f 7365 7428 290a 2020  d_bases_set().  
-0000d6b0: 2020 2020 2020 6966 206f 7468 6572 5f64        if other_d
-0000d6c0: 6572 6976 6564 5f62 6173 6573 2021 3d20  erived_bases != 
-0000d6d0: 7365 6c66 5f64 6572 6976 6564 5f62 6173  self_derived_bas
-0000d6e0: 6573 2061 6e64 2073 656c 665f 6465 7269  es and self_deri
-0000d6f0: 7665 645f 6261 7365 732e 6973 7375 6273  ved_bases.issubs
-0000d700: 6574 286f 7468 6572 5f64 6572 6976 6564  et(other_derived
-0000d710: 5f62 6173 6573 293a 0a20 2020 2020 2020  _bases):.       
-0000d720: 2020 2020 2023 2041 766f 6964 2063 7963       # Avoid cyc
-0000d730: 6c65 7320 6f6e 2064 6572 6976 6564 5f66  les on derived_f
-0000d740: 726f 6d5f 7461 672e 2068 7474 7073 3a2f  rom_tag. https:/
-0000d750: 2f67 6974 6875 622e 636f 6d2f 7277 7468  /github.com/rwth
-0000d760: 2d69 362f 7265 7475 726e 6e2f 6973 7375  -i6/returnn/issu
-0000d770: 6573 2f31 3035 340a 2020 2020 2020 2020  es/1054.        
-0000d780: 2020 2020 7769 7468 2075 7469 6c2e 6775      with util.gu
-0000d790: 6172 645f 696e 6669 6e69 7465 5f72 6563  ard_infinite_rec
-0000d7a0: 7572 7369 6f6e 285f 642e 4469 6d2e 6465  ursion(_d.Dim.de
-0000d7b0: 636c 6172 655f 7361 6d65 5f61 732c 206f  clare_same_as, o
-0000d7c0: 7468 6572 2c20 7365 6c66 293a 0a20 2020  ther, self):.   
-0000d7d0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000d7e0: 7572 6e20 6f74 6865 722e 6465 636c 6172  urn other.declar
-0000d7f0: 655f 7361 6d65 5f61 7328 7365 6c66 290a  e_same_as(self).
-0000d800: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d810: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
-0000d820: 2020 2020 7365 6c66 2e5f 6578 7472 612e      self._extra.
-0000d830: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-0000d840: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0000d850: 2020 2073 656c 662e 5f65 7874 7261 2e64     self._extra.d
-0000d860: 6572 6976 6564 5f66 726f 6d5f 7461 6720  erived_from_tag 
-0000d870: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-0000d880: 6620 7365 6c66 5f73 616d 655f 6173 2069  f self_same_as i
-0000d890: 7320 6e6f 7420 7365 6c66 3a0a 2020 2020  s not self:.    
-0000d8a0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-0000d8b0: 6f74 2073 656c 665f 7361 6d65 5f61 732e  ot self_same_as.
-0000d8c0: 7361 6d65 5f61 730a 2020 2020 2020 2020  same_as.        
-0000d8d0: 2020 2020 6966 2073 656c 665f 7361 6d65      if self_same
-0000d8e0: 5f61 7320 6973 206f 7468 6572 5f73 616d  _as is other_sam
-0000d8f0: 655f 6261 7365 3a0a 2020 2020 2020 2020  e_base:.        
-0000d900: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000d910: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000d920: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
-0000d930: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
-0000d940: 2e44 696d 2e64 6563 6c61 7265 5f73 616d  .Dim.declare_sam
-0000d950: 655f 6173 2c20 7365 6c66 5f73 616d 655f  e_as, self_same_
-0000d960: 6173 2c20 6f74 6865 725f 7361 6d65 5f62  as, other_same_b
-0000d970: 6173 6529 3a0a 2020 2020 2020 2020 2020  ase):.          
-0000d980: 2020 2020 2020 7365 6c66 5f73 616d 655f        self_same_
-0000d990: 6173 2e64 6563 6c61 7265 5f73 616d 655f  as.declare_same_
-0000d9a0: 6173 286f 7468 6572 5f73 616d 655f 6261  as(other_same_ba
-0000d9b0: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-0000d9c0: 6966 2028 7365 6c66 2e64 796e 5f73 697a  if (self.dyn_siz
-0000d9d0: 655f 6578 7420 6973 204e 6f6e 6520 6f72  e_ext is None or
-0000d9e0: 206e 6f74 2073 656c 662e 5f76 616c 6964   not self._valid
-0000d9f0: 6174 655f 696e 5f63 7572 7265 6e74 5f67  ate_in_current_g
-0000da00: 7261 7068 2829 2920 616e 6420 7365 6c66  raph()) and self
-0000da10: 5f73 616d 655f 6173 2e64 796e 5f73 697a  _same_as.dyn_siz
-0000da20: 655f 6578 743a 0a20 2020 2020 2020 2020  e_ext:.         
-0000da30: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
-0000da40: 7369 7a65 5f65 7874 203d 2073 656c 665f  size_ext = self_
-0000da50: 7361 6d65 5f61 732e 6765 745f 6479 6e5f  same_as.get_dyn_
-0000da60: 7369 7a65 5f65 7874 5f66 6f72 5f62 6174  size_ext_for_bat
-0000da70: 6368 5f63 7478 280a 2020 2020 2020 2020  ch_ctx(.        
-0000da80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000da90: 2e62 6174 6368 2c20 7365 6c66 2e63 6f6e  .batch, self.con
-0000daa0: 7472 6f6c 5f66 6c6f 775f 6374 782c 2074  trol_flow_ctx, t
-0000dab0: 656d 706c 6174 655f 6f6e 6c79 3d54 7275  emplate_only=Tru
-0000dac0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000dad0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
-0000dae0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000daf0: 2073 656c 662e 5f65 7874 7261 3a0a 2020   self._extra:.  
-0000db00: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000db10: 7220 6469 6d5f 2069 6e20 7365 6c66 2e5f  r dim_ in self._
-0000db20: 6578 7472 612e 7361 6d65 5f66 6f72 5f62  extra.same_for_b
-0000db30: 6174 6368 5f63 7478 2e76 616c 7565 7328  atch_ctx.values(
-0000db40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000db50: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
-0000db60: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
-0000db70: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
-0000db80: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0000db90: 696d 5f2e 5f65 7874 7261 3a0a 2020 2020  im_._extra:.    
-0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbb0: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
-0000dbc0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
-0000dbd0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-0000dbe0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-0000dbf0: 5f2e 5f65 7874 7261 2e64 6572 6976 6564  _._extra.derived
-0000dc00: 5f66 726f 6d5f 6f70 203d 204e 6f6e 650a  _from_op = None.
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
-0000dc30: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
-0000dc40: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
-0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc60: 2064 696d 5f2e 5f65 7874 7261 2e64 6572   dim_._extra.der
-0000dc70: 6976 6564 5f66 726f 6d5f 7461 6720 3d20  ived_from_tag = 
-0000dc80: 4e6f 6e65 0a20 2020 2020 2020 2023 204e  None.        # N
-0000dc90: 6f77 206d 6572 6765 2065 7869 7374 696e  ow merge existin
-0000dca0: 6720 7661 7269 616e 7473 2e20 4275 7420  g variants. But 
-0000dcb0: 6f6e 6c79 2069 6620 6e6f 7420 6465 7269  only if not deri
-0000dcc0: 7665 6420 7669 6120 6f70 2c20 6265 6361  ved via op, beca
-0000dcd0: 7573 6520 696e 2074 6861 7420 6361 7365  use in that case
-0000dce0: 2c20 7765 2063 616e 2028 616e 6420 7368  , we can (and sh
-0000dcf0: 6f75 6c64 2129 0a20 2020 2020 2020 2023  ould!).        #
-0000dd00: 2061 7574 6f6d 6174 6963 616c 6c79 2069   automatically i
-0000dd10: 6e66 6572 2069 742e 204e 6f74 6520 7468  nfer it. Note th
-0000dd20: 6174 2077 6520 6f6e 6c79 2067 6f74 2068  at we only got h
-0000dd30: 6572 6520 7768 656e 2074 6865 206f 7468  ere when the oth
-0000dd40: 6572 2069 7320 6e6f 7420 7468 6520 7361  er is not the sa
-0000dd50: 6d65 2064 696d 2c20 736f 2069 7420 6d65  me dim, so it me
-0000dd60: 616e 7320 7468 6174 0a20 2020 2020 2020  ans that.       
-0000dd70: 2023 2074 6865 206f 7468 6572 2069 7320   # the other is 
-0000dd80: 7265 616c 6c79 2064 6966 6665 7265 6e74  really different
-0000dd90: 2c20 7468 6520 7369 7a65 7320 6172 6520  , the sizes are 
-0000dda0: 706f 7465 6e74 6961 6c6c 7920 6469 6666  potentially diff
-0000ddb0: 6572 656e 742c 2062 7574 2077 6520 7761  erent, but we wa
-0000ddc0: 6e74 2074 6f20 6f76 6572 7461 6b65 2074  nt to overtake t
-0000ddd0: 6865 206f 7468 6572 2e0a 2020 2020 2020  he other..      
-0000dde0: 2020 6966 206f 7468 6572 5f73 616d 655f    if other_same_
-0000ddf0: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
-0000de00: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
-0000de10: 2020 2320 436c 6561 6e75 7020 6576 6572    # Cleanup ever
-0000de20: 7974 6869 6e67 2c20 6573 7020 706f 7465  ything, esp pote
-0000de30: 6e74 6961 6c20 616c 7265 6164 7920 636f  ntial already co
-0000de40: 6d70 7574 6564 2073 697a 6573 2c20 6173  mputed sizes, as
-0000de50: 2074 6865 7365 206d 6967 6874 2062 6520   these might be 
-0000de60: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
-0000de70: 2020 2020 2066 6f72 2064 696d 5f20 696e       for dim_ in
-0000de80: 205b 7365 6c66 5f73 616d 655f 6173 2c20   [self_same_as, 
-0000de90: 7365 6c66 5d20 2b20 286c 6973 7428 7365  self] + (list(se
-0000dea0: 6c66 2e5f 6578 7472 612e 7361 6d65 5f66  lf._extra.same_f
-0000deb0: 6f72 5f62 6174 6368 5f63 7478 2e76 616c  or_batch_ctx.val
-0000dec0: 7565 7328 2929 2069 6620 7365 6c66 2e5f  ues()) if self._
-0000ded0: 6578 7472 6120 656c 7365 205b 5d29 3a0a  extra else []):.
-0000dee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000def0: 6966 2064 696d 5f2e 6479 6e5f 7369 7a65  if dim_.dyn_size
-0000df00: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
-0000df10: 2020 2020 2020 2020 2020 6469 6d5f 2e64            dim_.d
-0000df20: 796e 5f73 697a 655f 6578 742e 706c 6163  yn_size_ext.plac
-0000df30: 6568 6f6c 6465 7220 3d20 4e6f 6e65 0a20  eholder = None. 
-0000df40: 2020 2020 2020 206f 7468 6572 5f73 616d         other_sam
-0000df50: 655f 6261 7365 2e5f 6d65 7267 655f 7361  e_base._merge_sa
-0000df60: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
-0000df70: 5f64 6963 7428 7365 6c66 290a 2020 2020  _dict(self).    
-0000df80: 2020 2020 6f74 6865 722e 5f6d 6179 6265      other._maybe
-0000df90: 5f75 7064 6174 6528 290a 2020 2020 2020  _update().      
-0000dfa0: 2020 7365 6c66 2e73 616d 655f 6173 203d    self.same_as =
-0000dfb0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000dfc0: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
-0000dfd0: 6179 6265 5f75 7064 6174 6528 290a 2020  aybe_update().  
-0000dfe0: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
-0000dff0: 6e5f 7369 7a65 2069 7320 6e6f 7420 4e6f  n_size is not No
-0000e000: 6e65 2061 6e64 206f 7468 6572 5f73 616d  ne and other_sam
-0000e010: 655f 6261 7365 2e64 796e 5f73 697a 6520  e_base.dyn_size 
-0000e020: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000e030: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000e040: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
-0000e050: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000e060: 2e64 796e 5f73 697a 653a 0a20 2020 2020  .dyn_size:.     
-0000e070: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000e080: 6c66 2e62 6174 6368 203d 3d20 6f74 6865  lf.batch == othe
-0000e090: 725f 7361 6d65 5f62 6173 652e 6261 7463  r_same_base.batc
-0000e0a0: 6820 616e 6420 7365 6c66 2e63 6f6e 7472  h and self.contr
-0000e0b0: 6f6c 5f66 6c6f 775f 6374 7820 3d3d 206f  ol_flow_ctx == o
-0000e0c0: 7468 6572 5f73 616d 655f 6261 7365 2e63  ther_same_base.c
-0000e0d0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 783a  ontrol_flow_ctx:
-0000e0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e0f0: 2020 2020 2023 204e 6f74 653a 2049 6e73       # Note: Ins
-0000e100: 7465 6164 206f 6620 6d61 6b69 6e67 2074  tead of making t
-0000e110: 6869 7320 6120 7761 726e 696e 672c 2077  his a warning, w
-0000e120: 6520 636f 756c 6420 616c 736f 2065 6e66  e could also enf
-0000e130: 6f72 6365 2074 6869 7320 6174 2073 6f6d  orce this at som
-0000e140: 6520 706f 696e 742e 0a20 2020 2020 2020  e point..       
-0000e150: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-0000e160: 2054 6865 2075 7365 7220 7368 6f75 6c64   The user should
-0000e170: 2062 6520 6162 6c65 2074 6f20 6669 7820   be able to fix 
-0000e180: 6065 7874 6572 6e5f 6461 7461 6020 696e  `extern_data` in
-0000e190: 2074 6865 2063 6f6e 6669 670a 2020 2020   the config.    
-0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1b0: 2320 2020 7375 6368 2074 6861 7420 7468  #   such that th
-0000e1c0: 6973 2069 7320 636f 7272 6563 7420 696e  is is correct in
-0000e1d0: 2074 6865 2066 6972 7374 2070 6c61 6365   the first place
-0000e1e0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e1f0: 2020 2020 2020 2320 2020 416c 736f 2c20        #   Also, 
-0000e200: 696e 2061 6464 6974 696f 6e20 746f 2074  in addition to t
-0000e210: 6869 7320 7761 726e 696e 672c 0a20 2020  his warning,.   
-0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e230: 2023 2020 2077 6520 6d69 6768 7420 7761   #   we might wa
-0000e240: 6e74 2074 6f20 6164 6420 736f 6d65 2072  nt to add some r
-0000e250: 756e 7469 6d65 2063 6865 636b 206f 6e20  untime check on 
-0000e260: 7468 6520 6571 206f 6620 7468 6520 6479  the eq of the dy
-0000e270: 6e20 7369 7a65 732e 0a20 2020 2020 2020  n sizes..       
-0000e280: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000e290: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-0000e2a0: 2020 2020 2020 2020 2020 2020 2257 6172              "War
-0000e2b0: 6e69 6e67 3a20 6173 7375 6d69 6e67 2064  ning: assuming d
-0000e2c0: 696d 2074 6167 7320 6172 6520 7361 6d65  im tags are same
-0000e2d0: 2077 6974 6820 6469 6666 6572 656e 7420   with different 
-0000e2e0: 7369 7a65 2070 6c61 6365 686f 6c64 6572  size placeholder
-0000e2f0: 733a 2025 7220 7673 2025 7222 0a20 2020  s: %r vs %r".   
-0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e310: 2020 2020 2025 2028 7365 6c66 2e64 796e       % (self.dyn
-0000e320: 5f73 697a 652c 206f 7468 6572 5f73 616d  _size, other_sam
-0000e330: 655f 6261 7365 2e64 796e 5f73 697a 6529  e_base.dyn_size)
-0000e340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e350: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
-0000e360: 2049 6620 7765 2068 6176 6520 6120 6465   If we have a de
-0000e370: 6669 6e65 6420 736f 7572 6365 2c20 616e  fined source, an
-0000e380: 6420 7468 6973 2069 7320 6120 6479 6e61  d this is a dyna
-0000e390: 6d69 6320 7370 6174 6961 6c20 6178 6973  mic spatial axis
-0000e3a0: 2c20 616e 6420 6974 2077 6173 2075 6e64  , and it was und
-0000e3b0: 6566 696e 6564 2062 6566 6f72 652c 0a20  efined before,. 
-0000e3c0: 2020 2020 2020 2023 206d 6179 6265 2077         # maybe w
-0000e3d0: 6520 6361 6e20 6f76 6572 7461 6b65 2074  e can overtake t
-0000e3e0: 6865 2073 697a 655f 706c 6163 6568 6f6c  he size_placehol
-0000e3f0: 6465 7220 6e6f 772e 0a20 2020 2020 2020  der now..       
-0000e400: 2069 6620 6f74 6865 725f 7361 6d65 5f62   if other_same_b
-0000e410: 6173 652e 6479 6e5f 7369 7a65 2069 7320  ase.dyn_size is 
-0000e420: 6e6f 7420 4e6f 6e65 2061 6e64 2073 656c  not None and sel
-0000e430: 662e 5f65 7874 7261 2061 6e64 2073 656c  f._extra and sel
-0000e440: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
-0000e450: 613a 0a20 2020 2020 2020 2020 2020 2061  a:.            a
-0000e460: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-0000e470: 2873 656c 662e 5f65 7874 7261 2e73 7263  (self._extra.src
-0000e480: 5f61 7869 732c 2069 6e74 290a 2020 2020  _axis, int).    
-0000e490: 2020 2020 2020 2020 2320 4d61 7962 6520          # Maybe 
-0000e4a0: 6974 2063 6861 6e67 6564 2069 6e20 7468  it changed in th
-0000e4b0: 6520 6d65 616e 7768 696c 652c 2073 6f20  e meanwhile, so 
-0000e4c0: 6368 6563 6b2e 0a20 2020 2020 2020 2020  check..         
-0000e4d0: 2020 2074 6167 203d 2073 656c 662e 5f65     tag = self._e
-0000e4e0: 7874 7261 2e73 7263 5f64 6174 612e 6765  xtra.src_data.ge
-0000e4f0: 745f 6469 6d5f 7461 6728 7365 6c66 2e5f  t_dim_tag(self._
-0000e500: 6578 7472 612e 7372 635f 6178 6973 290a  extra.src_axis).
-0000e510: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0000e520: 6167 2e64 6573 6372 6970 7469 6f6e 203d  ag.description =
-0000e530: 3d20 7365 6c66 2e64 6573 6372 6970 7469  = self.descripti
-0000e540: 6f6e 2061 6e64 2028 6e6f 7420 7461 672e  on and (not tag.
-0000e550: 6479 6e5f 7369 7a65 5f65 7874 206f 7220  dyn_size_ext or 
-0000e560: 6e6f 7420 7461 672e 5f76 616c 6964 6174  not tag._validat
-0000e570: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
-0000e580: 7068 2829 293a 0a20 2020 2020 2020 2020  ph()):.         
-0000e590: 2020 2020 2020 2074 6167 2e64 796e 5f73         tag.dyn_s
-0000e5a0: 697a 655f 6578 7420 3d20 7365 6c66 2e67  ize_ext = self.g
-0000e5b0: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
-0000e5c0: 666f 725f 6261 7463 685f 6374 7828 0a20  for_batch_ctx(. 
-0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5e0: 2020 2074 6167 2e62 6174 6368 2c20 7461     tag.batch, ta
-0000e5f0: 672e 636f 6e74 726f 6c5f 666c 6f77 5f63  g.control_flow_c
-0000e600: 7478 2c20 7465 6d70 6c61 7465 5f6f 6e6c  tx, template_onl
-0000e610: 793d 5472 7565 0a20 2020 2020 2020 2020  y=True.         
-0000e620: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e630: 2020 2020 2020 2020 2074 6167 2e5f 6d61           tag._ma
-0000e640: 7962 655f 7570 6461 7465 2829 0a20 2020  ybe_update().   
-0000e650: 2020 2020 2023 2049 6620 6f74 6865 7273       # If others
-0000e660: 2064 796e 5f73 697a 6520 6973 204e 6f6e   dyn_size is Non
-0000e670: 6520 6275 7420 7765 2068 6176 6520 6120  e but we have a 
-0000e680: 6479 6e5f 7369 7a65 2c20 6d61 7962 6520  dyn_size, maybe 
-0000e690: 7570 6461 7465 206f 7468 6572 7320 6479  update others dy
-0000e6a0: 6e5f 7369 7a65 2e0a 2020 2020 2020 2020  n_size..        
-0000e6b0: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
-0000e6c0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000e6d0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000e6e0: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
-0000e6f0: 2073 656c 662e 6479 6e5f 7369 7a65 3a0a   self.dyn_size:.
-0000e700: 2020 2020 2020 2020 2020 2020 2320 436f              # Co
-0000e710: 756c 6420 6265 2075 6e73 6574 2069 6620  uld be unset if 
-0000e720: 6974 2063 6f6d 6573 2066 726f 6d20 7468  it comes from th
-0000e730: 6520 636f 6e66 6967 2c20 6f72 2066 726f  e config, or fro
-0000e740: 6d20 7072 6576 2067 7261 7068 2063 7265  m prev graph cre
-0000e750: 6174 696f 6e2e 0a20 2020 2020 2020 2020  ation..         
-0000e760: 2020 2023 2054 6869 7320 6973 2069 6d70     # This is imp
-0000e770: 6f72 7461 6e74 2073 7563 6820 7468 6174  ortant such that
-0000e780: 2073 656c 662e 6361 6e5f 636f 6d70 6172   self.can_compar
-0000e790: 6528 2920 6973 2073 616e 652e 0a20 2020  e() is sane..   
-0000e7a0: 2020 2020 2020 2020 2069 6620 6f74 6865           if othe
-0000e7b0: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
-0000e7c0: 7369 7a65 2069 7320 4e6f 6e65 206f 7220  size is None or 
-0000e7d0: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
-0000e7e0: 6173 652e 5f76 616c 6964 6174 655f 696e  ase._validate_in
-0000e7f0: 5f63 7572 7265 6e74 5f67 7261 7068 2829  _current_graph()
-0000e800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e810: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
-0000e820: 652e 6479 6e5f 7369 7a65 5f65 7874 203d  e.dyn_size_ext =
-0000e830: 2073 656c 662e 6765 745f 6479 6e5f 7369   self.get_dyn_si
-0000e840: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
-0000e850: 5f63 7478 280a 2020 2020 2020 2020 2020  _ctx(.          
-0000e860: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
-0000e870: 7361 6d65 5f62 6173 652e 6261 7463 682c  same_base.batch,
-0000e880: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000e890: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000e8a0: 782c 2074 656d 706c 6174 655f 6f6e 6c79  x, template_only
-0000e8b0: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
-0000e8c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000e8d0: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
-0000e8e0: 6d65 5f62 6173 652e 5f6d 6179 6265 5f75  me_base._maybe_u
-0000e8f0: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
-0000e900: 6966 206e 6f74 2073 656c 662e 6479 6e5f  if not self.dyn_
-0000e910: 7369 7a65 5f65 7874 206f 7220 6e6f 7420  size_ext or not 
-0000e920: 7365 6c66 2e5f 7661 6c69 6461 7465 5f69  self._validate_i
-0000e930: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
-0000e940: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000e950: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-0000e960: 203d 206f 7468 6572 5f73 616d 655f 6261   = other_same_ba
-0000e970: 7365 2e67 6574 5f64 796e 5f73 697a 655f  se.get_dyn_size_
-0000e980: 6578 745f 666f 725f 6261 7463 685f 6374  ext_for_batch_ct
-0000e990: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
-0000e9a0: 2020 2073 656c 662e 6261 7463 682c 2073     self.batch, s
-0000e9b0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-0000e9c0: 5f63 7478 2c20 7465 6d70 6c61 7465 5f6f  _ctx, template_o
-0000e9d0: 6e6c 793d 5472 7565 0a20 2020 2020 2020  nly=True.       
-0000e9e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000e9f0: 2020 2073 656c 662e 5f6d 6179 6265 5f75     self._maybe_u
-0000ea00: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
-0000ea10: 656c 6966 206f 7468 6572 5f73 616d 655f  elif other_same_
-0000ea20: 6261 7365 2e64 796e 5f73 697a 655f 6578  base.dyn_size_ex
-0000ea30: 7420 6973 204e 6f6e 6520 6f72 206e 6f74  t is None or not
-0000ea40: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000ea50: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
-0000ea60: 7272 656e 745f 6772 6170 6828 293a 0a20  rrent_graph():. 
-0000ea70: 2020 2020 2020 2020 2020 206f 7468 6572             other
-0000ea80: 5f73 616d 655f 6261 7365 2e64 796e 5f73  _same_base.dyn_s
-0000ea90: 697a 655f 6578 7420 3d20 7365 6c66 2e67  ize_ext = self.g
-0000eaa0: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
-0000eab0: 666f 725f 6261 7463 685f 6374 7828 0a20  for_batch_ctx(. 
-0000eac0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000ead0: 7468 6572 5f73 616d 655f 6261 7365 2e62  ther_same_base.b
-0000eae0: 6174 6368 2c20 6f74 6865 725f 7361 6d65  atch, other_same
-0000eaf0: 5f62 6173 652e 636f 6e74 726f 6c5f 666c  _base.control_fl
-0000eb00: 6f77 5f63 7478 2c20 7465 6d70 6c61 7465  ow_ctx, template
-0000eb10: 5f6f 6e6c 793d 5472 7565 0a20 2020 2020  _only=True.     
-0000eb20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000eb30: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
-0000eb40: 6261 7365 2e5f 6d61 7962 655f 7570 6461  base._maybe_upda
-0000eb50: 7465 2829 0a20 2020 2020 2020 2069 6620  te().        if 
-0000eb60: 7365 6c66 2e69 735f 6469 6d5f 6b6e 6f77  self.is_dim_know
-0000eb70: 6e28 2920 616e 6420 6f74 6865 722e 6973  n() and other.is
-0000eb80: 5f64 696d 5f6b 6e6f 776e 2829 3a0a 2020  _dim_known():.  
-0000eb90: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000eba0: 2073 656c 662e 6469 6d65 6e73 696f 6e20   self.dimension 
-0000ebb0: 3d3d 206f 7468 6572 2e64 696d 656e 7369  == other.dimensi
-0000ebc0: 6f6e 0a20 2020 2020 2020 2065 6c69 6620  on.        elif 
-0000ebd0: 7365 6c66 2e69 735f 6469 6d5f 6b6e 6f77  self.is_dim_know
-0000ebe0: 6e28 2920 616e 6420 6e6f 7420 6f74 6865  n() and not othe
-0000ebf0: 722e 6973 5f64 696d 5f6b 6e6f 776e 2829  r.is_dim_known()
-0000ec00: 3a0a 2020 2020 2020 2020 2020 2020 6f74  :.            ot
-0000ec10: 6865 722e 6361 7061 6369 7479 203d 2073  her.capacity = s
-0000ec20: 656c 662e 6361 7061 6369 7479 0a20 2020  elf.capacity.   
-0000ec30: 2020 2020 2020 2020 206f 7468 6572 2e73           other.s
-0000ec40: 697a 6520 3d20 7365 6c66 2e73 697a 650a  ize = self.size.
-0000ec50: 2020 2020 2020 2020 656c 6966 206e 6f74          elif not
-0000ec60: 2073 656c 662e 6973 5f64 696d 5f6b 6e6f   self.is_dim_kno
-0000ec70: 776e 2829 2061 6e64 206f 7468 6572 2e69  wn() and other.i
-0000ec80: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
-0000ec90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000eca0: 6361 7061 6369 7479 203d 206f 7468 6572  capacity = other
-0000ecb0: 2e63 6170 6163 6974 790a 2020 2020 2020  .capacity.      
-0000ecc0: 2020 2020 2020 7365 6c66 2e73 697a 6520        self.size 
-0000ecd0: 3d20 6f74 6865 722e 7369 7a65 0a20 2020  = other.size.   
-0000ece0: 2020 2020 2069 6620 7365 6c66 2e76 6f63       if self.voc
-0000ecf0: 6162 2061 6e64 206e 6f74 206f 7468 6572  ab and not other
-0000ed00: 5f73 616d 655f 6261 7365 2e76 6f63 6162  _same_base.vocab
-0000ed10: 3a0a 2020 2020 2020 2020 2020 2020 6f74  :.            ot
-0000ed20: 6865 725f 7361 6d65 5f62 6173 652e 766f  her_same_base.vo
-0000ed30: 6361 6220 3d20 7365 6c66 2e76 6f63 6162  cab = self.vocab
-0000ed40: 0a20 2020 2020 2020 2065 6c69 6620 6f74  .        elif ot
-0000ed50: 6865 725f 7361 6d65 5f62 6173 652e 766f  her_same_base.vo
-0000ed60: 6361 6220 616e 6420 6e6f 7420 7365 6c66  cab and not self
-0000ed70: 2e76 6f63 6162 3a0a 2020 2020 2020 2020  .vocab:.        
-0000ed80: 2020 2020 7365 6c66 2e76 6f63 6162 203d      self.vocab =
-0000ed90: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000eda0: 2e76 6f63 6162 0a20 2020 2020 2020 2073  .vocab.        s
-0000edb0: 656c 662e 5f6d 616b 655f 6578 7472 6128  elf._make_extra(
-0000edc0: 290a 2020 2020 2020 2020 7365 6c66 5f73  ).        self_s
-0000edd0: 616d 655f 6173 2e5f 6d61 6b65 5f65 7874  ame_as._make_ext
-0000ede0: 7261 2829 0a20 2020 2020 2020 2023 206e  ra().        # n
-0000edf0: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
-0000ee00: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
-0000ee10: 2020 2020 2020 7365 6c66 2e5f 6578 7472        self._extr
-0000ee20: 612e 6175 746f 5f67 656e 6572 6174 6564  a.auto_generated
-0000ee30: 203d 2073 656c 665f 7361 6d65 5f61 732e   = self_same_as.
-0000ee40: 5f65 7874 7261 2e61 7574 6f5f 6765 6e65  _extra.auto_gene
-0000ee50: 7261 7465 6420 3d20 6f74 6865 725f 7361  rated = other_sa
-0000ee60: 6d65 5f62 6173 652e 6175 746f 5f67 656e  me_base.auto_gen
-0000ee70: 6572 6174 6564 0a20 2020 2020 2020 2023  erated.        #
-0000ee80: 2054 616b 6520 6f76 6572 2064 6572 6976   Take over deriv
-0000ee90: 6564 5f66 726f 6d5f 6f70 2e20 486f 7765  ed_from_op. Howe
-0000eea0: 7665 722c 206f 6e6c 7920 6966 2074 6869  ver, only if thi
-0000eeb0: 7320 776f 756c 6420 6e6f 7420 696e 7472  s would not intr
-0000eec0: 6f64 7563 6520 6379 636c 6573 210a 2020  oduce cycles!.  
-0000eed0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0000eee0: 665f 6465 7269 7665 645f 6261 7365 732e  f_derived_bases.
-0000eef0: 6973 7375 7065 7273 6574 286f 7468 6572  issuperset(other
-0000ef00: 5f64 6572 6976 6564 5f62 6173 6573 293a  _derived_bases):
-0000ef10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000ef20: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
-0000ef30: 6d5f 6f70 2061 6e64 206e 6f74 206f 7468  m_op and not oth
-0000ef40: 6572 5f73 616d 655f 6261 7365 2e64 6572  er_same_base.der
-0000ef50: 6976 6564 5f66 726f 6d5f 6f70 3a0a 2020  ived_from_op:.  
-0000ef60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000ef70: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-0000ef80: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-0000ef90: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000efa0: 7468 6572 5f73 616d 655f 6261 7365 2e5f  ther_same_base._
-0000efb0: 6d61 6b65 5f65 7874 7261 2829 2e64 6572  make_extra().der
-0000efc0: 6976 6564 5f66 726f 6d5f 6f70 203d 2073  ived_from_op = s
-0000efd0: 656c 662e 6465 7269 7665 645f 6672 6f6d  elf.derived_from
-0000efe0: 5f6f 700a 2020 2020 2020 2020 2020 2020  _op.            
-0000eff0: 656c 6966 206f 7468 6572 5f73 616d 655f  elif other_same_
-0000f000: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
-0000f010: 6d5f 6f70 2061 6e64 206e 6f74 2073 656c  m_op and not sel
-0000f020: 662e 6465 7269 7665 645f 6672 6f6d 5f6f  f.derived_from_o
-0000f030: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-0000f040: 2020 2073 656c 662e 5f6d 616b 655f 6578     self._make_ex
-0000f050: 7472 6128 292e 6465 7269 7665 645f 6672  tra().derived_fr
-0000f060: 6f6d 5f6f 7020 3d20 6f74 6865 725f 7361  om_op = other_sa
-0000f070: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
-0000f080: 6672 6f6d 5f6f 700a 2020 2020 2020 2020  from_op.        
-0000f090: 6966 2073 656c 662e 5f65 7874 7261 2061  if self._extra a
-0000f0a0: 6e64 206e 6f74 206f 7468 6572 5f73 616d  nd not other_sam
-0000f0b0: 655f 6261 7365 2e69 735f 6479 6e61 6d69  e_base.is_dynami
-0000f0c0: 6328 293a 0a20 2020 2020 2020 2020 2020  c():.           
-0000f0d0: 2023 2054 686f 7365 206d 6967 6874 2062   # Those might b
-0000f0e0: 6520 7365 7420 7669 6120 6765 745f 6261  e set via get_ba
-0000f0f0: 7463 685f 666f 725f 6374 7820 666f 7220  tch_for_ctx for 
-0000f100: 616e 2075 6e64 6566 696e 6564 2064 696d  an undefined dim
-0000f110: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-0000f120: 7768 6963 6820 6e6f 7720 6265 636f 6d65  which now become
-0000f130: 7320 7374 6174 6963 2064 7565 2074 6f20  s static due to 
-0000f140: 606f 7468 6572 602e 0a20 2020 2020 2020  `other`..       
-0000f150: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
-0000f160: 2e62 6174 6368 203d 204e 6f6e 650a 2020  .batch = None.  
-0000f170: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000f180: 6578 7472 612e 636f 6e74 726f 6c5f 666c  extra.control_fl
-0000f190: 6f77 5f63 7478 203d 204e 6f6e 650a 2020  ow_ctx = None.  
-0000f1a0: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
-0000f1b0: 792c 2064 696d 5f20 696e 2073 656c 662e  y, dim_ in self.
-0000f1c0: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
-0000f1d0: 6261 7463 685f 6374 782e 6974 656d 7328  batch_ctx.items(
-0000f1e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000f1f0: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
-0000f200: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
-0000f210: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
-0000f220: 2020 2020 6469 6d5f 6578 7472 6120 3d20      dim_extra = 
-0000f230: 6469 6d5f 2e5f 6578 7472 610a 2020 2020  dim_._extra.    
-0000f240: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0000f250: 696d 5f65 7874 7261 3a0a 2020 2020 2020  im_extra:.      
-0000f260: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0000f270: 6d5f 6578 7472 612e 6261 7463 6820 3d20  m_extra.batch = 
-0000f280: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0000f290: 2020 2020 2020 2020 2064 696d 5f65 7874           dim_ext
-0000f2a0: 7261 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  ra.control_flow_
-0000f2b0: 6374 7820 3d20 4e6f 6e65 0a20 2020 2020  ctx = None.     
-0000f2c0: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
-0000f2d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000f2e0: 6c66 5f20 3d20 7365 6c66 2e67 6574 5f66  lf_ = self.get_f
-0000f2f0: 6f72 5f62 6174 6368 5f63 7478 2862 6174  or_batch_ctx(bat
-0000f300: 6368 3d73 656c 662e 6261 7463 682c 2063  ch=self.batch, c
-0000f310: 7478 3d73 656c 662e 636f 6e74 726f 6c5f  tx=self.control_
-0000f320: 666c 6f77 5f63 7478 290a 2020 2020 2020  flow_ctx).      
-0000f330: 2020 2020 2020 6966 2073 656c 665f 2069        if self_ i
-0000f340: 7320 6e6f 7420 7365 6c66 3a0a 2020 2020  s not self:.    
-0000f350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f360: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000f370: 7820 3d20 7365 6c66 5f2e 636f 6e74 726f  x = self_.contro
-0000f380: 6c5f 666c 6f77 5f63 7478 2020 2320 6d69  l_flow_ctx  # mi
-0000f390: 6768 7420 6265 2064 6966 6665 7265 6e74  ght be different
-0000f3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f3b0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-0000f3c0: 7874 203d 2073 656c 665f 2e64 796e 5f73  xt = self_.dyn_s
-0000f3d0: 697a 655f 6578 7420 2023 206d 6967 6874  ize_ext  # might
-0000f3e0: 2062 6520 756e 7365 740a 0a20 2020 2064   be unset..    d
-0000f3f0: 6566 205f 6d65 7267 655f 7361 6d65 5f66  ef _merge_same_f
-0000f400: 6f72 5f62 6174 6368 5f63 7478 5f64 6963  or_batch_ctx_dic
-0000f410: 7428 7365 6c66 3a20 5f64 2e44 696d 2c20  t(self: _d.Dim, 
-0000f420: 6f74 6865 723a 205f 642e 4469 6d29 3a0a  other: _d.Dim):.
-0000f430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f440: 2020 2020 3a70 6172 616d 206f 7468 6572      :param other
-0000f450: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000f460: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-0000f470: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-0000f480: 4d65 6d62 6572 0a20 2020 2020 2020 2069  Member.        i
-0000f490: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
-0000f4a0: 6120 616e 6420 6e6f 7420 6f74 6865 722e  a and not other.
-0000f4b0: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
-0000f4c0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000f4d0: 2020 2073 656c 662e 5f76 616c 6964 6174     self._validat
-0000f4e0: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
-0000f4f0: 7068 2829 0a20 2020 2020 2020 2069 6620  ph().        if 
-0000f500: 7365 6c66 2e5f 6578 7472 613a 0a20 2020  self._extra:.   
-0000f510: 2020 2020 2020 2020 2066 6f72 205f 2c20           for _, 
-0000f520: 6469 6d20 696e 206c 6973 7428 7365 6c66  dim in list(self
-0000f530: 2e5f 6578 7472 612e 7361 6d65 5f66 6f72  ._extra.same_for
-0000f540: 5f62 6174 6368 5f63 7478 2e69 7465 6d73  _batch_ctx.items
-0000f550: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
-0000f560: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
-0000f570: 7374 616e 6365 2864 696d 2c20 5f64 2e44  stance(dim, _d.D
-0000f580: 696d 290a 2020 2020 2020 2020 2020 2020  im).            
-0000f590: 2020 2020 6469 6d2e 5f76 616c 6964 6174      dim._validat
-0000f5a0: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
-0000f5b0: 7068 2829 0a20 2020 2020 2020 2023 206e  ph().        # n
-0000f5c0: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
-0000f5d0: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
-0000f5e0: 2020 2020 2020 6966 206f 7468 6572 2e5f        if other._
-0000f5f0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
-0000f600: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
-0000f610: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
-0000f620: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
-0000f630: 666f 7220 6b65 792c 2064 696d 2069 6e20  for key, dim in 
-0000f640: 6f74 6865 722e 5f65 7874 7261 2e73 616d  other._extra.sam
-0000f650: 655f 666f 725f 6261 7463 685f 6374 782e  e_for_batch_ctx.
-0000f660: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-0000f670: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000f680: 6469 6d2e 5f76 616c 6964 6174 655f 696e  dim._validate_in
-0000f690: 5f63 7572 7265 6e74 5f67 7261 7068 2829  _current_graph()
-0000f6a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f6b0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f6d0: 656c 665f 6469 6d20 3d20 7365 6c66 2e5f  elf_dim = self._
-0000f6e0: 6d61 6b65 5f65 7874 7261 2829 2e73 616d  make_extra().sam
-0000f6f0: 655f 666f 725f 6261 7463 685f 6374 782e  e_for_batch_ctx.
-0000f700: 6765 7428 6b65 792c 204e 6f6e 6529 0a20  get(key, None). 
-0000f710: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f720: 6620 7365 6c66 5f64 696d 2061 6e64 2028  f self_dim and (
-0000f730: 7365 6c66 5f64 696d 2e64 796e 5f73 697a  self_dim.dyn_siz
-0000f740: 655f 6578 7420 6f72 206e 6f74 2064 696d  e_ext or not dim
-0000f750: 2e64 796e 5f73 697a 655f 6578 7429 3a0a  .dyn_size_ext):.
+0000ba20: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000ba30: 2020 2020 2020 2070 6173 7320 2023 2065         pass  # e
+0000ba40: 7863 6570 7469 6f6e 2c20 616c 6c6f 7720  xception, allow 
+0000ba50: 6272 6f61 6463 6173 7420 6c6f 6769 630a  broadcast logic.
+0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000ba80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ba90: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
+0000baa0: 6620 7365 6c66 5f6b 696e 6420 3d3d 206f  f self_kind == o
+0000bab0: 7468 6572 5f6b 696e 6420 3d3d 2044 696d  ther_kind == Dim
+0000bac0: 5479 7065 732e 4665 6174 7572 653a 0a20  Types.Feature:. 
+0000bad0: 2020 2020 2020 2020 2020 2069 6620 616c             if al
+0000bae0: 6c6f 775f 7361 6d65 5f66 6561 7475 7265  low_same_feature
+0000baf0: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
+0000bb00: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000bb10: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0000bb20: 665f 6b69 6e64 203d 3d20 6f74 6865 725f  f_kind == other_
+0000bb30: 6b69 6e64 203d 3d20 4469 6d54 7970 6573  kind == DimTypes
+0000bb40: 2e53 7061 7469 616c 3a0a 2020 2020 2020  .Spatial:.      
+0000bb50: 2020 2020 2020 6966 2061 6c6c 6f77 5f73        if allow_s
+0000bb60: 616d 655f 7370 6174 6961 6c5f 6469 6d3a  ame_spatial_dim:
+0000bb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bb80: 2069 6620 7365 6c66 2e64 696d 656e 7369   if self.dimensi
+0000bb90: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbb0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbd0: 6966 2062 726f 6164 6361 7374 5f6d 6174  if broadcast_mat
+0000bbe0: 6368 6573 2061 6e64 2028 7365 6c66 2e64  ches and (self.d
+0000bbf0: 696d 656e 7369 6f6e 203d 3d20 3120 6f72  imension == 1 or
+0000bc00: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
+0000bc10: 203d 3d20 3129 3a0a 2020 2020 2020 2020   == 1):.        
+0000bc20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000bc30: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+0000bc40: 2020 2020 6966 2075 6e6b 6e6f 776e 5f73      if unknown_s
+0000bc50: 7061 7469 616c 5f6d 6174 6368 6573 2061  patial_matches a
+0000bc60: 6e64 2028 2873 656c 662e 6479 6e5f 7369  nd ((self.dyn_si
+0000bc70: 7a65 2069 7320 4e6f 6e65 2920 6f72 2028  ze is None) or (
+0000bc80: 6f74 6865 722e 6479 6e5f 7369 7a65 2069  other.dyn_size i
+0000bc90: 7320 4e6f 6e65 2929 3a0a 2020 2020 2020  s None)):.      
+0000bca0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000bcb0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+0000bcc0: 2020 6966 2075 6e64 6566 696e 6564 5f6d    if undefined_m
+0000bcd0: 6174 6368 6573 2061 6e64 2028 7365 6c66  atches and (self
+0000bce0: 2e75 6e64 6566 696e 6564 206f 7220 6f74  .undefined or ot
+0000bcf0: 6865 722e 756e 6465 6669 6e65 6429 3a0a  her.undefined):.
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd10: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
+0000bd20: 2020 2020 2320 496e 2070 7269 6e63 6970      # In princip
+0000bd30: 6c65 2c20 7765 2077 6f75 6c64 2077 616e  le, we would wan
+0000bd40: 7420 746f 2063 6865 636b 2066 6f72 2069  t to check for i
+0000bd50: 6465 6e74 6974 7920 2873 656c 6620 6973  dentity (self is
+0000bd60: 206f 7468 6572 292e 0a20 2020 2020 2020   other)..       
+0000bd70: 2023 2057 6520 6375 7272 656e 746c 7920   # We currently 
+0000bd80: 7573 6520 7468 6520 6465 7363 7269 7074  use the descript
+0000bd90: 696f 6e20 6265 6361 7573 6520 7468 6520  ion because the 
+0000bda0: 6964 656e 7469 7479 2077 6f75 6c64 206e  identity would n
+0000bdb0: 6f74 2062 6520 7468 6520 7361 6d65 0a20  ot be the same. 
+0000bdc0: 2020 2020 2020 2023 2069 6e20 6361 7365         # in case
+0000bdd0: 206f 6620 7465 6d70 6c61 7465 2063 6f6e   of template con
+0000bde0: 7374 7275 6374 696f 6e20 7768 6572 6520  struction where 
+0000bdf0: 6120 6469 6d20 7461 6720 6973 206f 6e63  a dim tag is onc
+0000be00: 6520 6372 6561 7465 6420 666f 7220 6120  e created for a 
+0000be10: 7465 6d70 6c61 7465 206c 6179 6572 2c0a  template layer,.
+0000be20: 2020 2020 2020 2020 2320 616e 6420 7468          # and th
+0000be30: 656e 206c 6174 6572 2061 6761 696e 2066  en later again f
+0000be40: 6f72 2074 6865 2072 6561 6c20 6c61 7965  or the real laye
+0000be50: 722e 0a20 2020 2020 2020 2069 6620 7365  r..        if se
+0000be60: 6c66 2e61 7574 6f5f 6765 6e65 7261 7465  lf.auto_generate
+0000be70: 6420 616e 6420 6f74 6865 722e 6175 746f  d and other.auto
+0000be80: 5f67 656e 6572 6174 6564 2061 6e64 2073  _generated and s
+0000be90: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
+0000bea0: 3d3d 206f 7468 6572 2e64 6573 6372 6970  == other.descrip
+0000beb0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+0000bec0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000bed0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0000bee0: 7365 0a0a 2020 2020 6465 6620 5f5f 6571  se..    def __eq
+0000bef0: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
+0000bf00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000bf10: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
+0000bf20: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+0000bf30: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+0000bf40: 2020 2020 3a72 6574 7572 6e3a 203a 6675      :return: :fu
+0000bf50: 6e63 3a60 6973 5f65 7175 616c 6020 7769  nc:`is_equal` wi
+0000bf60: 7468 2064 6566 6175 6c74 206f 7074 696f  th default optio
+0000bf70: 6e73 0a20 2020 2020 2020 2022 2222 0a20  ns.        """. 
+0000bf80: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+0000bf90: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
+0000bfa0: 5f64 2e44 696d 293a 0a20 2020 2020 2020  _d.Dim):.       
+0000bfb0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+0000bfc0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0000bfd0: 2073 656c 662e 6973 5f65 7175 616c 286f   self.is_equal(o
+0000bfe0: 7468 6572 290a 0a20 2020 2064 6566 205f  ther)..    def _
+0000bff0: 5f6e 655f 5f28 7365 6c66 3a20 4469 6d2c  _ne__(self: Dim,
+0000c000: 206f 7468 6572 3a20 4469 6d29 3a0a 2020   other: Dim):.  
+0000c010: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c020: 2020 3a70 6172 616d 2044 696d 206f 7468    :param Dim oth
+0000c030: 6572 3a0a 2020 2020 2020 2020 3a72 7479  er:.        :rty
+0000c040: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
+0000c050: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+0000c060: 7572 6e20 6e6f 7420 2873 656c 6620 3d3d  urn not (self ==
+0000c070: 206f 7468 6572 290a 0a20 2020 2064 6566   other)..    def
+0000c080: 205f 5f68 6173 685f 5f28 7365 6c66 293a   __hash__(self):
+0000c090: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c0a0: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
+0000c0b0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000c0c0: 3a20 6861 7368 2c20 6d61 7463 6869 6e67  : hash, matching
+0000c0d0: 2074 6f20 3a66 756e 633a 605f 5f65 715f   to :func:`__eq_
+0000c0e0: 5f60 0a20 2020 2020 2020 2022 2222 0a20  _`.        """. 
+0000c0f0: 2020 2020 2020 2023 2054 6869 7320 6d75         # This mu
+0000c100: 7374 206d 6174 6368 2074 6865 2062 6568  st match the beh
+0000c110: 6176 696f 7220 696e 205f 5f65 715f 5f2c  avior in __eq__,
+0000c120: 2077 6869 6368 2069 7320 6973 5f65 7175   which is is_equ
+0000c130: 616c 2077 6974 6820 6465 6661 756c 7420  al with default 
+0000c140: 6f70 7469 6f6e 732e 0a20 2020 2020 2020  options..       
+0000c150: 2023 2049 2e65 2e20 6469 6666 6572 656e   # I.e. differen
+0000c160: 7420 6861 7368 2069 6d70 6c69 6573 206e  t hash implies n
+0000c170: 6f74 2065 7175 616c 2028 6275 7420 7361  ot equal (but sa
+0000c180: 6d65 2068 6173 6820 6e6f 7420 6e65 6365  me hash not nece
+0000c190: 7373 6172 696c 7920 6571 7561 6c29 2e0a  ssarily equal)..
+0000c1a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000c1b0: 7370 6563 6961 6c3a 0a20 2020 2020 2020  special:.       
+0000c1c0: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
+0000c1d0: 2869 6428 7365 6c66 2929 0a20 2020 2020  (id(self)).     
+0000c1e0: 2020 2069 6620 7365 6c66 2e69 735f 6261     if self.is_ba
+0000c1f0: 7463 685f 6469 6d28 293a 0a20 2020 2020  tch_dim():.     
+0000c200: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
+0000c210: 7368 2828 2929 0a20 2020 2020 2020 2077  sh(()).        w
+0000c220: 6974 6820 7574 696c 2e67 7561 7264 5f69  ith util.guard_i
+0000c230: 6e66 696e 6974 655f 7265 6375 7273 696f  nfinite_recursio
+0000c240: 6e28 5f64 2e44 696d 2e5f 5f68 6173 685f  n(_d.Dim.__hash_
+0000c250: 5f2c 2073 656c 6629 3a0a 2020 2020 2020  _, self):.      
+0000c260: 2020 2020 2020 6261 7365 203d 2073 656c        base = sel
+0000c270: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
+0000c280: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000c290: 2062 6173 6520 6973 206e 6f74 2073 656c   base is not sel
+0000c2a0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+0000c2b0: 2020 2072 6574 7572 6e20 6861 7368 2862     return hash(b
+0000c2c0: 6173 6529 0a20 2020 2020 2020 2020 2020  ase).           
+0000c2d0: 2069 6620 7365 6c66 2e64 6572 6976 6564   if self.derived
+0000c2e0: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
+0000c2f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000c300: 2068 6173 6828 7365 6c66 2e64 6572 6976   hash(self.deriv
+0000c310: 6564 5f66 726f 6d5f 6f70 290a 2020 2020  ed_from_op).    
+0000c320: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000c330: 6175 746f 5f67 656e 6572 6174 6564 3a0a  auto_generated:.
+0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c350: 7265 7475 726e 2068 6173 6828 2862 6173  return hash((bas
+0000c360: 652e 6b69 6e64 2c20 6261 7365 2e64 696d  e.kind, base.dim
+0000c370: 656e 7369 6f6e 2c20 6261 7365 2e64 6573  ension, base.des
+0000c380: 6372 6970 7469 6f6e 2929 0a20 2020 2020  cription)).     
+0000c390: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
+0000c3a0: 7368 2869 6428 6261 7365 2929 0a0a 2020  sh(id(base))..  
+0000c3b0: 2020 6465 6620 5f5f 6c74 5f5f 2873 656c    def __lt__(sel
+0000c3c0: 663a 2044 696d 2c20 6f74 6865 723a 2044  f: Dim, other: D
+0000c3d0: 696d 293a 0a20 2020 2020 2020 2022 2222  im):.        """
+0000c3e0: 0a20 2020 2020 2020 2044 6566 696e 6520  .        Define 
+0000c3f0: 736f 6d65 206f 7264 6572 2e20 5468 6973  some order. This
+0000c400: 2069 7320 6a75 7374 2073 7563 6820 7468   is just such th
+0000c410: 6174 2060 736f 7274 6564 6020 776f 726b  at `sorted` work
+0000c420: 732c 206f 7220 736f 6d65 2064 6966 6620  s, or some diff 
+0000c430: 7265 706f 7274 696e 672c 206f 7220 736f  reporting, or so
+0000c440: 2e0a 2020 2020 2020 2020 4974 2069 7320  ..        It is 
+0000c450: 6f6e 2073 796d 626f 6c69 6320 6c65 7665  on symbolic leve
+0000c460: 6c2c 2069 2e65 2e20 6974 2064 6f65 7320  l, i.e. it does 
+0000c470: 6e6f 7420 636f 6e73 6964 6572 2074 6865  not consider the
+0000c480: 2061 6374 7561 6c20 6469 6d65 6e73 696f   actual dimensio
+0000c490: 6e20 7661 6c75 652e 0a20 2020 2020 2020  n value..       
+0000c4a0: 2054 6865 2064 6566 696e 6564 206f 7264   The defined ord
+0000c4b0: 6572 2073 6f6d 6577 6861 7420 6172 6269  er somewhat arbi
+0000c4c0: 7472 6172 792c 2073 6f20 646f 206e 6f74  trary, so do not
+0000c4d0: 2072 656c 7920 6f6e 2074 6865 2065 7861   rely on the exa
+0000c4e0: 6374 2062 6568 6176 696f 722c 0a20 2020  ct behavior,.   
+0000c4f0: 2020 2020 2061 7320 7468 6973 206d 6967       as this mig
+0000c500: 6874 2063 6861 6e67 6520 6174 2073 6f6d  ht change at som
+0000c510: 6520 6c61 7465 7220 706f 696e 742e 0a20  e later point.. 
+0000c520: 2020 2020 2020 2043 7572 7265 6e74 6c79         Currently
+0000c530: 2c20 6974 2064 6570 656e 6473 206f 6e20  , it depends on 
+0000c540: 7468 6520 6372 6561 7469 6f6e 2069 6e64  the creation ind
+0000c550: 6578 2e0a 0a20 2020 2020 2020 203a 7061  ex...        :pa
+0000c560: 7261 6d20 4469 6d20 6f74 6865 723a 0a20  ram Dim other:. 
+0000c570: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
+0000c580: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
+0000c590: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+0000c5a0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
+0000c5b0: 2028 5f64 2e44 696d 2c20 5f6d 2e4d 6172   (_d.Dim, _m.Mar
+0000c5c0: 6b65 6444 696d 2929 3a0a 2020 2020 2020  kedDim)):.      
+0000c5d0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+0000c5e0: 4572 726f 7228 2263 616e 6e6f 7420 636f  Error("cannot co
+0000c5f0: 6d70 6172 6520 2572 2077 6974 6820 2572  mpare %r with %r
+0000c600: 2220 2520 2873 656c 662c 206f 7468 6572  " % (self, other
+0000c610: 2929 0a20 2020 2020 2020 2069 6620 7365  )).        if se
+0000c620: 6c66 203d 3d20 6f74 6865 723a 0a20 2020  lf == other:.   
+0000c630: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c640: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
+0000c650: 7475 726e 2064 696d 5f63 6d70 5f76 616c  turn dim_cmp_val
+0000c660: 7565 2873 656c 6629 203c 2064 696d 5f63  ue(self) < dim_c
+0000c670: 6d70 5f76 616c 7565 286f 7468 6572 290a  mp_value(other).
+0000c680: 0a20 2020 2064 6566 205f 5f67 745f 5f28  .    def __gt__(
+0000c690: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+0000c6a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c6b0: 2020 5365 6520 3a66 756e 633a 605f 5f6c    See :func:`__l
+0000c6c0: 745f 5f60 2e0a 0a20 2020 2020 2020 203a  t__`...        :
+0000c6d0: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
+0000c6e0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000c6f0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
+0000c700: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+0000c710: 206f 7468 6572 203c 2073 656c 660a 0a20   other < self.. 
+0000c720: 2020 2064 6566 205f 5f67 655f 5f28 7365     def __ge__(se
+0000c730: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+0000c740: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+0000c750: 656c 6620 3c20 6f74 6865 720a 0a20 2020  elf < other..   
+0000c760: 2064 6566 205f 5f6c 655f 5f28 7365 6c66   def __le__(self
+0000c770: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+0000c780: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
+0000c790: 6620 3e20 6f74 6865 720a 0a20 2020 2064  f > other..    d
+0000c7a0: 6566 2067 6574 5f73 616d 655f 6261 7365  ef get_same_base
+0000c7b0: 2873 656c 663a 205f 642e 4469 6d29 202d  (self: _d.Dim) -
+0000c7c0: 3e20 5f64 2e44 696d 3a0a 2020 2020 2020  > _d.Dim:.      
+0000c7d0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+0000c7e0: 6574 7572 6e3a 2073 616d 6520 6261 7365  eturn: same base
+0000c7f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c800: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0000c810: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
+0000c820: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000c830: 0a20 2020 2020 2020 2062 6173 6520 3d20  .        base = 
+0000c840: 7365 6c66 0a20 2020 2020 2020 2077 6869  self.        whi
+0000c850: 6c65 2062 6173 652e 7361 6d65 5f61 733a  le base.same_as:
+0000c860: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+0000c870: 6520 3d20 6261 7365 2e73 616d 655f 6173  e = base.same_as
+0000c880: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000c890: 6261 7365 0a0a 2020 2020 6465 6620 6765  base..    def ge
+0000c8a0: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
+0000c8b0: 6173 6528 7365 6c66 3a20 5f64 2e44 696d  ase(self: _d.Dim
+0000c8c0: 2920 2d3e 205f 642e 4469 6d3a 0a20 2020  ) -> _d.Dim:.   
+0000c8d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c8e0: 203a 7265 7475 726e 3a20 7361 6d65 2062   :return: same b
+0000c8f0: 6173 652c 2062 7574 2061 6c73 6f20 636f  ase, but also co
+0000c900: 6e73 6964 6572 2064 6572 6976 6564 5f66  nsider derived_f
+0000c910: 726f 6d5f 2e2e 2e0a 2020 2020 2020 2020  rom_....        
+0000c920: 2222 220a 2020 2020 2020 2020 6261 7365  """.        base
+0000c930: 203d 2073 656c 660a 2020 2020 2020 2020   = self.        
+0000c940: 7669 7369 7465 6420 3d20 7b7d 0a20 2020  visited = {}.   
+0000c950: 2020 2020 2077 6869 6c65 2062 6173 652e       while base.
+0000c960: 7361 6d65 5f61 7320 6f72 2062 6173 652e  same_as or base.
+0000c970: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
+0000c980: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
+0000c990: 7365 7274 2069 6428 6261 7365 2920 6e6f  sert id(base) no
+0000c9a0: 7420 696e 2076 6973 6974 6564 2020 2320  t in visited  # 
+0000c9b0: 7368 6f75 6c64 206e 6f74 2068 6176 6520  should not have 
+0000c9c0: 6379 636c 6573 2e20 6e6f 726d 616c 6c79  cycles. normally
+0000c9d0: 2074 6869 7320 7368 6f75 6c64 206e 6576   this should nev
+0000c9e0: 6572 2062 6520 7472 6967 6765 7265 640a  er be triggered.
+0000c9f0: 2020 2020 2020 2020 2020 2020 7669 7369              visi
+0000ca00: 7465 645b 6964 2862 6173 6529 5d20 3d20  ted[id(base)] = 
+0000ca10: 6261 7365 0a20 2020 2020 2020 2020 2020  base.           
+0000ca20: 2069 6620 6261 7365 2e73 616d 655f 6173   if base.same_as
+0000ca30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ca40: 2020 6261 7365 203d 2062 6173 652e 7361    base = base.sa
+0000ca50: 6d65 5f61 730a 2020 2020 2020 2020 2020  me_as.          
+0000ca60: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+0000ca70: 2020 2020 2020 2020 2020 2062 6173 6520             base 
+0000ca80: 3d20 6261 7365 2e64 6572 6976 6564 5f66  = base.derived_f
+0000ca90: 726f 6d5f 7461 670a 2020 2020 2020 2020  rom_tag.        
+0000caa0: 2020 2020 6173 7365 7274 2062 6173 650a      assert base.
+0000cab0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+0000cac0: 6173 650a 0a20 2020 2064 6566 2067 6574  ase..    def get
+0000cad0: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
+0000cae0: 6574 2873 656c 6629 3a0a 2020 2020 2020  et(self):.      
+0000caf0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+0000cb00: 7479 7065 3a20 7365 745b 4469 6d5d 0a20  type: set[Dim]. 
+0000cb10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000cb20: 2020 2072 6573 203d 2073 6574 2829 0a20     res = set(). 
+0000cb30: 2020 2020 2020 2071 7565 7565 203d 205b         queue = [
+0000cb40: 7365 6c66 5d0a 2020 2020 2020 2020 7669  self].        vi
+0000cb50: 7369 7465 6420 3d20 7b7d 2020 2320 7479  sited = {}  # ty
+0000cb60: 7065 3a20 4469 6374 5b69 6e74 2c5f 642e  pe: Dict[int,_d.
+0000cb70: 4469 6d5d 2020 2320 6279 2069 640a 2020  Dim]  # by id.  
+0000cb80: 2020 2020 2020 7768 696c 6520 7175 6575        while queu
+0000cb90: 653a 0a20 2020 2020 2020 2020 2020 2062  e:.            b
+0000cba0: 6173 6520 3d20 7175 6575 652e 706f 7028  ase = queue.pop(
+0000cbb0: 2d31 290a 2020 2020 2020 2020 2020 2020  -1).            
+0000cbc0: 6966 2062 6173 652e 7361 6d65 5f61 733a  if base.same_as:
+0000cbd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cbe0: 2062 6173 6520 3d20 6261 7365 2e73 616d   base = base.sam
+0000cbf0: 655f 6173 0a20 2020 2020 2020 2020 2020  e_as.           
+0000cc00: 2069 6620 6964 2862 6173 6529 2069 6e20   if id(base) in 
+0000cc10: 7669 7369 7465 643a 0a20 2020 2020 2020  visited:.       
+0000cc20: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0000cc30: 650a 2020 2020 2020 2020 2020 2020 7669  e.            vi
+0000cc40: 7369 7465 645b 6964 2862 6173 6529 5d20  sited[id(base)] 
+0000cc50: 3d20 6261 7365 0a20 2020 2020 2020 2020  = base.         
+0000cc60: 2020 2072 6573 2e61 6464 2862 6173 6529     res.add(base)
+0000cc70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000cc80: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000cc90: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
+0000cca0: 2020 2020 2020 7175 6575 652e 6578 7465        queue.exte
+0000ccb0: 6e64 2862 6173 652e 6465 7269 7665 645f  nd(base.derived_
+0000ccc0: 6672 6f6d 5f6f 702e 696e 7075 7473 290a  from_op.inputs).
+0000ccd0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000cce0: 2062 6173 652e 6465 7269 7665 645f 6672   base.derived_fr
+0000ccf0: 6f6d 5f74 6167 3a0a 2020 2020 2020 2020  om_tag:.        
+0000cd00: 2020 2020 2020 2020 7175 6575 652e 6170          queue.ap
+0000cd10: 7065 6e64 2862 6173 652e 6465 7269 7665  pend(base.derive
+0000cd20: 645f 6672 6f6d 5f74 6167 290a 2020 2020  d_from_tag).    
+0000cd30: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
+0000cd40: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000cd50: 2020 6465 6620 756e 6465 6669 6e65 6428    def undefined(
+0000cd60: 7365 6c66 3a20 5f64 2e44 696d 2920 2d3e  self: _d.Dim) ->
+0000cd70: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+0000cd80: 2222 0a20 2020 2020 2020 203a 7265 7475  "".        :retu
+0000cd90: 726e 3a20 7768 6574 6865 7220 7468 6520  rn: whether the 
+0000cda0: 756e 6465 6669 6e65 6420 666c 6167 2069  undefined flag i
+0000cdb0: 7320 7365 742c 2069 6e20 7365 6c66 2c20  s set, in self, 
+0000cdc0: 6261 7365 732c 206f 7220 616e 7920 6465  bases, or any de
+0000cdd0: 7269 7665 6420 6261 7365 732e 2061 6c73  rived bases. als
+0000cde0: 6f20 7365 6520 3a66 756e 633a 6069 735f  o see :func:`is_
+0000cdf0: 6469 6d5f 6b6e 6f77 6e60 0a20 2020 2020  dim_known`.     
+0000ce00: 2020 2022 2222 0a20 2020 2020 2020 2062     """.        b
+0000ce10: 6173 6520 3d20 7365 6c66 0a20 2020 2020  ase = self.     
+0000ce20: 2020 2076 6973 6974 6564 203d 207b 7d0a     visited = {}.
+0000ce30: 2020 2020 2020 2020 7768 696c 6520 6261          while ba
+0000ce40: 7365 2e73 616d 655f 6173 206f 7220 6261  se.same_as or ba
+0000ce50: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
+0000ce60: 7461 673a 0a20 2020 2020 2020 2020 2020  tag:.           
+0000ce70: 2061 7373 6572 7420 6964 2862 6173 6529   assert id(base)
+0000ce80: 206e 6f74 2069 6e20 7669 7369 7465 6420   not in visited 
+0000ce90: 2023 2073 686f 756c 6420 6e6f 7420 6861   # should not ha
+0000cea0: 7665 2063 7963 6c65 732e 206e 6f72 6d61  ve cycles. norma
+0000ceb0: 6c6c 7920 7468 6973 2073 686f 756c 6420  lly this should 
+0000cec0: 6e65 7665 7220 6265 2074 7269 6767 6572  never be trigger
+0000ced0: 6564 0a20 2020 2020 2020 2020 2020 2076  ed.            v
+0000cee0: 6973 6974 6564 5b69 6428 6261 7365 295d  isited[id(base)]
+0000cef0: 203d 2062 6173 650a 2020 2020 2020 2020   = base.        
+0000cf00: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+0000cf10: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+0000cf20: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+0000cf30: 2069 6620 6261 7365 2e5f 6578 7472 6120   if base._extra 
+0000cf40: 616e 6420 6261 7365 2e5f 6578 7472 612e  and base._extra.
+0000cf50: 756e 6465 6669 6e65 643a 0a20 2020 2020  undefined:.     
+0000cf60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000cf70: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
+0000cf80: 2020 2069 6620 6261 7365 2e73 616d 655f     if base.same_
+0000cf90: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
+0000cfa0: 2020 2020 6261 7365 203d 2062 6173 652e      base = base.
+0000cfb0: 7361 6d65 5f61 730a 2020 2020 2020 2020  same_as.        
+0000cfc0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000cfd0: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+0000cfe0: 6520 3d20 6261 7365 2e64 6572 6976 6564  e = base.derived
+0000cff0: 5f66 726f 6d5f 7461 670a 2020 2020 2020  _from_tag.      
+0000d000: 2020 2020 2020 6173 7365 7274 2062 6173        assert bas
+0000d010: 650a 2020 2020 2020 2020 2320 6e6f 696e  e.        # noin
+0000d020: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+0000d030: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+0000d040: 2020 2072 6574 7572 6e20 6261 7365 2e5f     return base._
+0000d050: 6578 7472 6120 616e 6420 6261 7365 2e5f  extra and base._
+0000d060: 6578 7472 612e 756e 6465 6669 6e65 640a  extra.undefined.
+0000d070: 0a20 2020 2064 6566 2064 6563 6c61 7265  .    def declare
+0000d080: 5f73 616d 655f 6173 2873 656c 663a 205f  _same_as(self: _
+0000d090: 642e 4469 6d2c 206f 7468 6572 3a20 5f64  d.Dim, other: _d
+0000d0a0: 2e44 696d 293a 0a20 2020 2020 2020 2022  .Dim):.        "
+0000d0b0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+0000d0c0: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
+0000d0d0: 2022 2222 0a20 2020 2020 2020 2061 7373   """.        ass
+0000d0e0: 6572 7420 7365 6c66 2e63 616e 5f62 655f  ert self.can_be_
+0000d0f0: 7573 6564 5f61 735f 6469 6d28 2920 616e  used_as_dim() an
+0000d100: 6420 6f74 6865 722e 6361 6e5f 6265 5f75  d other.can_be_u
+0000d110: 7365 645f 6173 5f64 696d 2829 2020 2320  sed_as_dim()  # 
+0000d120: 6465 636c 6172 655f 7361 6d65 5f61 7320  declare_same_as 
+0000d130: 646f 6573 206e 6f74 206d 616b 6520 7365  does not make se
+0000d140: 6e73 6520 6f74 6865 7277 6973 650a 2020  nse otherwise.  
+0000d150: 2020 2020 2020 2320 4e6f 7465 3a20 4368        # Note: Ch
+0000d160: 6563 6b20 6069 7360 2c20 6e6f 7420 603d  eck `is`, not `=
+0000d170: 3d60 2e20 603d 3d60 2063 616e 2062 6520  =`. `==` can be 
+0000d180: 7472 7565 2065 7665 6e20 7468 6f75 6768  true even though
+0000d190: 2073 616d 655f 6173 2061 7265 206e 6f74   same_as are not
+0000d1a0: 2074 6865 2073 616d 6520 696e 7374 616e   the same instan
+0000d1b0: 6365 2c0a 2020 2020 2020 2020 2320 652e  ce,.        # e.
+0000d1c0: 672e 2076 6961 2061 7574 6f5f 6765 6e65  g. via auto_gene
+0000d1d0: 7261 7465 642e 0a20 2020 2020 2020 2069  rated..        i
+0000d1e0: 6620 7365 6c66 2069 7320 6f74 6865 723a  f self is other:
+0000d1f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000d200: 7572 6e0a 2020 2020 2020 2020 7365 6c66  urn.        self
+0000d210: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
+0000d220: 0a20 2020 2020 2020 2073 656c 662e 5f76  .        self._v
+0000d230: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
+0000d240: 6e74 5f67 7261 7068 2829 0a20 2020 2020  nt_graph().     
+0000d250: 2020 206f 7468 6572 2e5f 7661 6c69 6461     other._valida
+0000d260: 7465 5f69 6e5f 6375 7272 656e 745f 6772  te_in_current_gr
+0000d270: 6170 6828 290a 2020 2020 2020 2020 6f74  aph().        ot
+0000d280: 6865 725f 7361 6d65 5f62 6173 6520 3d20  her_same_base = 
+0000d290: 6f74 6865 722e 6765 745f 7361 6d65 5f62  other.get_same_b
+0000d2a0: 6173 6528 290a 2020 2020 2020 2020 6966  ase().        if
+0000d2b0: 2073 656c 6620 6973 206f 7468 6572 5f73   self is other_s
+0000d2c0: 616d 655f 6261 7365 206f 7220 7365 6c66  ame_base or self
+0000d2d0: 2e73 616d 655f 6173 2069 7320 6f74 6865  .same_as is othe
+0000d2e0: 725f 7361 6d65 5f62 6173 653a 0a20 2020  r_same_base:.   
+0000d2f0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000d300: 2020 2020 2020 2020 7365 6c66 5f73 616d          self_sam
+0000d310: 655f 6173 203d 2073 656c 662e 6765 745f  e_as = self.get_
+0000d320: 7361 6d65 5f62 6173 6528 290a 2020 2020  same_base().    
+0000d330: 2020 2020 6966 2073 656c 665f 7361 6d65      if self_same
+0000d340: 5f61 7320 6973 206f 7468 6572 5f73 616d  _as is other_sam
+0000d350: 655f 6261 7365 3a0a 2020 2020 2020 2020  e_base:.        
+0000d360: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000d370: 2020 2069 6620 6f74 6865 725f 7361 6d65     if other_same
+0000d380: 5f62 6173 652e 6765 745f 7361 6d65 5f64  _base.get_same_d
+0000d390: 6572 6976 6564 5f62 6173 6528 2920 6973  erived_base() is
+0000d3a0: 2073 656c 665f 7361 6d65 5f61 733a 0a20   self_same_as:. 
+0000d3b0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
+0000d3c0: 6163 7475 616c 6c79 2077 616e 7420 6974  actually want it
+0000d3d0: 2074 6f20 6265 2074 6865 206f 7468 6572   to be the other
+0000d3e0: 2077 6179 2061 726f 756e 642e 0a20 2020   way around..   
+0000d3f0: 2020 2020 2020 2020 2077 6974 6820 7574           with ut
+0000d400: 696c 2e67 7561 7264 5f69 6e66 696e 6974  il.guard_infinit
+0000d410: 655f 7265 6375 7273 696f 6e28 5f64 2e44  e_recursion(_d.D
+0000d420: 696d 2e64 6563 6c61 7265 5f73 616d 655f  im.declare_same_
+0000d430: 6173 2c20 6f74 6865 722c 2073 656c 6629  as, other, self)
+0000d440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d450: 2020 7265 7475 726e 206f 7468 6572 2e64    return other.d
+0000d460: 6563 6c61 7265 5f73 616d 655f 6173 2873  eclare_same_as(s
+0000d470: 656c 6629 0a20 2020 2020 2020 2069 6620  elf).        if 
+0000d480: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
+0000d490: 2020 2020 2020 2020 2320 4966 2073 656c          # If sel
+0000d4a0: 6620 6973 2064 6566 696e 6564 2028 7365  f is defined (se
+0000d4b0: 6c66 2e69 735f 6469 6d5f 6b6e 6f77 6e29  lf.is_dim_known)
+0000d4c0: 2c20 6265 2066 6169 7220 746f 206f 7468  , be fair to oth
+0000d4d0: 6572 2c20 616e 6420 6164 6170 7420 6974  er, and adapt it
+0000d4e0: 2074 6f20 7468 6520 7269 6768 7420 6261   to the right ba
+0000d4f0: 7463 682c 0a20 2020 2020 2020 2020 2020  tch,.           
+0000d500: 2023 2073 7563 6820 7468 6174 206f 7468   # such that oth
+0000d510: 6572 2e69 735f 6469 6d5f 6b6e 6f77 6e20  er.is_dim_known 
+0000d520: 6973 2063 6f72 7265 6374 2c20 6279 2070  is correct, by p
+0000d530: 6f74 656e 7469 616c 6c79 2063 6f6d 706c  otentially compl
+0000d540: 6574 696e 6720 6974 2e0a 2020 2020 2020  eting it..      
+0000d550: 2020 2020 2020 6f74 6865 725f 203d 206f        other_ = o
+0000d560: 7468 6572 2e67 6574 5f66 6f72 5f62 6174  ther.get_for_bat
+0000d570: 6368 5f63 7478 2873 656c 662e 6261 7463  ch_ctx(self.batc
+0000d580: 682c 2063 7478 3d73 656c 662e 636f 6e74  h, ctx=self.cont
+0000d590: 726f 6c5f 666c 6f77 5f63 7478 290a 2020  rol_flow_ctx).  
+0000d5a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000d5b0: 2020 2020 2020 2020 6f74 6865 725f 203d          other_ =
+0000d5c0: 206f 7468 6572 0a20 2020 2020 2020 2069   other.        i
+0000d5d0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+0000d5e0: 2873 656c 662e 6973 5f64 696d 5f6b 6e6f  (self.is_dim_kno
+0000d5f0: 776e 2829 2061 6e64 206e 6f74 206f 7468  wn() and not oth
+0000d600: 6572 5f2e 6973 5f64 696d 5f6b 6e6f 776e  er_.is_dim_known
+0000d610: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+0000d620: 6f72 0a20 2020 2020 2020 2020 2020 2023  or.            #
+0000d630: 204c 696b 6520 6973 5f64 696d 5f6b 6e6f   Like is_dim_kno
+0000d640: 776e 2062 7574 2066 6f72 2073 7461 7469  wn but for stati
+0000d650: 6320 6469 6d73 2c20 7765 206d 6967 6874  c dims, we might
+0000d660: 206b 6e6f 7720 626f 7468 2c0a 2020 2020   know both,.    
+0000d670: 2020 2020 2020 2020 2320 6275 7420 7468          # but th
+0000d680: 6520 6465 7269 7665 645f 6672 6f6d 5f6f  e derived_from_o
+0000d690: 7020 7374 696c 6c20 776f 756c 6420 7072  p still would pr
+0000d6a0: 6f76 6964 6520 6d6f 7265 2069 6e66 6f72  ovide more infor
+0000d6b0: 6d61 7469 6f6e 2e0a 2020 2020 2020 2020  mation..        
+0000d6c0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+0000d6d0: 2020 2020 2020 7365 6c66 5f73 616d 655f        self_same_
+0000d6e0: 6173 2e64 6572 6976 6564 5f66 726f 6d5f  as.derived_from_
+0000d6f0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
+0000d700: 2020 2061 6e64 206e 6f74 206f 7468 6572     and not other
+0000d710: 5f73 616d 655f 6261 7365 2e64 6572 6976  _same_base.deriv
+0000d720: 6564 5f66 726f 6d5f 6f70 0a20 2020 2020  ed_from_op.     
+0000d730: 2020 2020 2020 2020 2020 2061 6e64 206f             and o
+0000d740: 7468 6572 206e 6f74 2069 6e20 7365 6c66  ther not in self
+0000d750: 2e67 6574 5f64 6572 6976 6564 5f62 6173  .get_derived_bas
+0000d760: 6573 5f73 6574 2829 0a20 2020 2020 2020  es_set().       
+0000d770: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000d780: 2020 206f 7220 286e 6f74 2073 656c 662e     or (not self.
+0000d790: 756e 6465 6669 6e65 6420 616e 6420 6f74  undefined and ot
+0000d7a0: 6865 725f 2e75 6e64 6566 696e 6564 290a  her_.undefined).
+0000d7b0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+0000d7c0: 2020 2020 2020 2077 6974 6820 7574 696c         with util
+0000d7d0: 2e67 7561 7264 5f69 6e66 696e 6974 655f  .guard_infinite_
+0000d7e0: 7265 6375 7273 696f 6e28 5f64 2e44 696d  recursion(_d.Dim
+0000d7f0: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
+0000d800: 2c20 6f74 6865 722c 2073 656c 6629 3a0a  , other, self):.
+0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d820: 7265 7475 726e 206f 7468 6572 2e64 6563  return other.dec
+0000d830: 6c61 7265 5f73 616d 655f 6173 2873 656c  lare_same_as(sel
+0000d840: 6629 0a20 2020 2020 2020 206f 7468 6572  f).        other
+0000d850: 5f64 6572 6976 6564 5f62 6173 6573 203d  _derived_bases =
+0000d860: 206f 7468 6572 2e67 6574 5f64 6572 6976   other.get_deriv
+0000d870: 6564 5f62 6173 6573 5f73 6574 2829 0a20  ed_bases_set(). 
+0000d880: 2020 2020 2020 2073 656c 665f 6465 7269         self_deri
+0000d890: 7665 645f 6261 7365 7320 3d20 7365 6c66  ved_bases = self
+0000d8a0: 2e67 6574 5f64 6572 6976 6564 5f62 6173  .get_derived_bas
+0000d8b0: 6573 5f73 6574 2829 0a20 2020 2020 2020  es_set().       
+0000d8c0: 2069 6620 6f74 6865 725f 6465 7269 7665   if other_derive
+0000d8d0: 645f 6261 7365 7320 213d 2073 656c 665f  d_bases != self_
+0000d8e0: 6465 7269 7665 645f 6261 7365 7320 616e  derived_bases an
+0000d8f0: 6420 7365 6c66 5f64 6572 6976 6564 5f62  d self_derived_b
+0000d900: 6173 6573 2e69 7373 7562 7365 7428 6f74  ases.issubset(ot
+0000d910: 6865 725f 6465 7269 7665 645f 6261 7365  her_derived_base
+0000d920: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000d930: 2320 4176 6f69 6420 6379 636c 6573 206f  # Avoid cycles o
+0000d940: 6e20 6465 7269 7665 645f 6672 6f6d 5f74  n derived_from_t
+0000d950: 6167 2e20 6874 7470 733a 2f2f 6769 7468  ag. https://gith
+0000d960: 7562 2e63 6f6d 2f72 7774 682d 6936 2f72  ub.com/rwth-i6/r
+0000d970: 6574 7572 6e6e 2f69 7373 7565 732f 3130  eturnn/issues/10
+0000d980: 3534 0a20 2020 2020 2020 2020 2020 2077  54.            w
+0000d990: 6974 6820 7574 696c 2e67 7561 7264 5f69  ith util.guard_i
+0000d9a0: 6e66 696e 6974 655f 7265 6375 7273 696f  nfinite_recursio
+0000d9b0: 6e28 5f64 2e44 696d 2e64 6563 6c61 7265  n(_d.Dim.declare
+0000d9c0: 5f73 616d 655f 6173 2c20 6f74 6865 722c  _same_as, other,
+0000d9d0: 2073 656c 6629 3a0a 2020 2020 2020 2020   self):.        
+0000d9e0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+0000d9f0: 7468 6572 2e64 6563 6c61 7265 5f73 616d  ther.declare_sam
+0000da00: 655f 6173 2873 656c 6629 0a20 2020 2020  e_as(self).     
+0000da10: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
+0000da20: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
+0000da30: 656c 662e 5f65 7874 7261 2e64 6572 6976  elf._extra.deriv
+0000da40: 6564 5f66 726f 6d5f 6f70 203d 204e 6f6e  ed_from_op = Non
+0000da50: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+0000da60: 6c66 2e5f 6578 7472 612e 6465 7269 7665  lf._extra.derive
+0000da70: 645f 6672 6f6d 5f74 6167 203d 204e 6f6e  d_from_tag = Non
+0000da80: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0000da90: 665f 7361 6d65 5f61 7320 6973 206e 6f74  f_same_as is not
+0000daa0: 2073 656c 663a 0a20 2020 2020 2020 2020   self:.         
+0000dab0: 2020 2061 7373 6572 7420 6e6f 7420 7365     assert not se
+0000dac0: 6c66 5f73 616d 655f 6173 2e73 616d 655f  lf_same_as.same_
+0000dad0: 6173 0a20 2020 2020 2020 2020 2020 2069  as.            i
+0000dae0: 6620 7365 6c66 5f73 616d 655f 6173 2069  f self_same_as i
+0000daf0: 7320 6f74 6865 725f 7361 6d65 5f62 6173  s other_same_bas
+0000db00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000db10: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000db20: 2020 2020 2020 7769 7468 2075 7469 6c2e        with util.
+0000db30: 6775 6172 645f 696e 6669 6e69 7465 5f72  guard_infinite_r
+0000db40: 6563 7572 7369 6f6e 285f 642e 4469 6d2e  ecursion(_d.Dim.
+0000db50: 6465 636c 6172 655f 7361 6d65 5f61 732c  declare_same_as,
+0000db60: 2073 656c 665f 7361 6d65 5f61 732c 206f   self_same_as, o
+0000db70: 7468 6572 5f73 616d 655f 6261 7365 293a  ther_same_base):
+0000db80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000db90: 2073 656c 665f 7361 6d65 5f61 732e 6465   self_same_as.de
+0000dba0: 636c 6172 655f 7361 6d65 5f61 7328 6f74  clare_same_as(ot
+0000dbb0: 6865 725f 7361 6d65 5f62 6173 6529 0a20  her_same_base). 
+0000dbc0: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
+0000dbd0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+0000dbe0: 2069 7320 4e6f 6e65 206f 7220 6e6f 7420   is None or not 
+0000dbf0: 7365 6c66 2e5f 7661 6c69 6461 7465 5f69  self._validate_i
+0000dc00: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000dc10: 2929 2061 6e64 2073 656c 665f 7361 6d65  )) and self_same
+0000dc20: 5f61 732e 6479 6e5f 7369 7a65 5f65 7874  _as.dyn_size_ext
+0000dc30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000dc40: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
+0000dc50: 6578 7420 3d20 7365 6c66 5f73 616d 655f  ext = self_same_
+0000dc60: 6173 2e67 6574 5f64 796e 5f73 697a 655f  as.get_dyn_size_
+0000dc70: 6578 745f 666f 725f 6261 7463 685f 6374  ext_for_batch_ct
+0000dc80: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
+0000dc90: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
+0000dca0: 682c 2073 656c 662e 636f 6e74 726f 6c5f  h, self.control_
+0000dcb0: 666c 6f77 5f63 7478 2c20 7465 6d70 6c61  flow_ctx, templa
+0000dcc0: 7465 5f6f 6e6c 793d 5472 7565 0a20 2020  te_only=True.   
+0000dcd0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000dce0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000dcf0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000dd00: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
+0000dd10: 2020 2020 2020 2020 2066 6f72 2064 696d           for dim
+0000dd20: 5f20 696e 2073 656c 662e 5f65 7874 7261  _ in self._extra
+0000dd30: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
+0000dd40: 6374 782e 7661 6c75 6573 2829 3a0a 2020  ctx.values():.  
+0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd60: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
+0000dd70: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
+0000dd80: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+0000dd90: 2020 2020 2020 2069 6620 6469 6d5f 2e5f         if dim_._
+0000dda0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
+0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000ddc0: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+0000ddd0: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddf0: 2020 2020 2020 2020 6469 6d5f 2e5f 6578          dim_._ex
+0000de00: 7472 612e 6465 7269 7665 645f 6672 6f6d  tra.derived_from
+0000de10: 5f6f 7020 3d20 4e6f 6e65 0a20 2020 2020  _op = None.     
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
+0000de40: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
+0000de50: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
+0000de60: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
+0000de70: 2e5f 6578 7472 612e 6465 7269 7665 645f  ._extra.derived_
+0000de80: 6672 6f6d 5f74 6167 203d 204e 6f6e 650a  from_tag = None.
+0000de90: 2020 2020 2020 2020 2320 4e6f 7720 6d65          # Now me
+0000dea0: 7267 6520 6578 6973 7469 6e67 2076 6172  rge existing var
+0000deb0: 6961 6e74 732e 2042 7574 206f 6e6c 7920  iants. But only 
+0000dec0: 6966 206e 6f74 2064 6572 6976 6564 2076  if not derived v
+0000ded0: 6961 206f 702c 2062 6563 6175 7365 2069  ia op, because i
+0000dee0: 6e20 7468 6174 2063 6173 652c 2077 6520  n that case, we 
+0000def0: 6361 6e20 2861 6e64 2073 686f 756c 6421  can (and should!
+0000df00: 290a 2020 2020 2020 2020 2320 6175 746f  ).        # auto
+0000df10: 6d61 7469 6361 6c6c 7920 696e 6665 7220  matically infer 
+0000df20: 6974 2e20 4e6f 7465 2074 6861 7420 7765  it. Note that we
+0000df30: 206f 6e6c 7920 676f 7420 6865 7265 2077   only got here w
+0000df40: 6865 6e20 7468 6520 6f74 6865 7220 6973  hen the other is
+0000df50: 206e 6f74 2074 6865 2073 616d 6520 6469   not the same di
+0000df60: 6d2c 2073 6f20 6974 206d 6561 6e73 2074  m, so it means t
+0000df70: 6861 740a 2020 2020 2020 2020 2320 7468  hat.        # th
+0000df80: 6520 6f74 6865 7220 6973 2072 6561 6c6c  e other is reall
+0000df90: 7920 6469 6666 6572 656e 742c 2074 6865  y different, the
+0000dfa0: 2073 697a 6573 2061 7265 2070 6f74 656e   sizes are poten
+0000dfb0: 7469 616c 6c79 2064 6966 6665 7265 6e74  tially different
+0000dfc0: 2c20 6275 7420 7765 2077 616e 7420 746f  , but we want to
+0000dfd0: 206f 7665 7274 616b 6520 7468 6520 6f74   overtake the ot
+0000dfe0: 6865 722e 0a20 2020 2020 2020 2069 6620  her..        if 
+0000dff0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000e000: 6465 7269 7665 645f 6672 6f6d 5f6f 703a  derived_from_op:
+0000e010: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+0000e020: 6c65 616e 7570 2065 7665 7279 7468 696e  leanup everythin
+0000e030: 672c 2065 7370 2070 6f74 656e 7469 616c  g, esp potential
+0000e040: 2061 6c72 6561 6479 2063 6f6d 7075 7465   already compute
+0000e050: 6420 7369 7a65 732c 2061 7320 7468 6573  d sizes, as thes
+0000e060: 6520 6d69 6768 7420 6265 2069 6e76 616c  e might be inval
+0000e070: 6964 2e0a 2020 2020 2020 2020 2020 2020  id..            
+0000e080: 666f 7220 6469 6d5f 2069 6e20 5b73 656c  for dim_ in [sel
+0000e090: 665f 7361 6d65 5f61 732c 2073 656c 665d  f_same_as, self]
+0000e0a0: 202b 2028 6c69 7374 2873 656c 662e 5f65   + (list(self._e
+0000e0b0: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
+0000e0c0: 7463 685f 6374 782e 7661 6c75 6573 2829  tch_ctx.values()
+0000e0d0: 2920 6966 2073 656c 662e 5f65 7874 7261  ) if self._extra
+0000e0e0: 2065 6c73 6520 5b5d 293a 0a20 2020 2020   else []):.     
+0000e0f0: 2020 2020 2020 2020 2020 2069 6620 6469             if di
+0000e100: 6d5f 2e64 796e 5f73 697a 655f 6578 743a  m_.dyn_size_ext:
+0000e110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e120: 2020 2020 2064 696d 5f2e 6479 6e5f 7369       dim_.dyn_si
+0000e130: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
+0000e140: 6572 203d 204e 6f6e 650a 2020 2020 2020  er = None.      
+0000e150: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
+0000e160: 652e 5f6d 6572 6765 5f73 616d 655f 666f  e._merge_same_fo
+0000e170: 725f 6261 7463 685f 6374 785f 6469 6374  r_batch_ctx_dict
+0000e180: 2873 656c 6629 0a20 2020 2020 2020 206f  (self).        o
+0000e190: 7468 6572 2e5f 6d61 7962 655f 7570 6461  ther._maybe_upda
+0000e1a0: 7465 2829 0a20 2020 2020 2020 2073 656c  te().        sel
+0000e1b0: 662e 7361 6d65 5f61 7320 3d20 6f74 6865  f.same_as = othe
+0000e1c0: 725f 7361 6d65 5f62 6173 650a 2020 2020  r_same_base.    
+0000e1d0: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
+0000e1e0: 7570 6461 7465 2829 0a20 2020 2020 2020  update().       
+0000e1f0: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
+0000e200: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
+0000e210: 6420 6f74 6865 725f 7361 6d65 5f62 6173  d other_same_bas
+0000e220: 652e 6479 6e5f 7369 7a65 2069 7320 6e6f  e.dyn_size is no
+0000e230: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000e240: 2020 2020 6966 2073 656c 662e 6479 6e5f      if self.dyn_
+0000e250: 7369 7a65 2069 7320 6e6f 7420 6f74 6865  size is not othe
+0000e260: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
+0000e270: 7369 7a65 3a0a 2020 2020 2020 2020 2020  size:.          
+0000e280: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
+0000e290: 7463 6820 3d3d 206f 7468 6572 5f73 616d  tch == other_sam
+0000e2a0: 655f 6261 7365 2e62 6174 6368 2061 6e64  e_base.batch and
+0000e2b0: 2073 656c 662e 636f 6e74 726f 6c5f 666c   self.control_fl
+0000e2c0: 6f77 5f63 7478 203d 3d20 6f74 6865 725f  ow_ctx == other_
+0000e2d0: 7361 6d65 5f62 6173 652e 636f 6e74 726f  same_base.contro
+0000e2e0: 6c5f 666c 6f77 5f63 7478 3a0a 2020 2020  l_flow_ctx:.    
+0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e300: 2320 4e6f 7465 3a20 496e 7374 6561 6420  # Note: Instead 
+0000e310: 6f66 206d 616b 696e 6720 7468 6973 2061  of making this a
+0000e320: 2077 6172 6e69 6e67 2c20 7765 2063 6f75   warning, we cou
+0000e330: 6c64 2061 6c73 6f20 656e 666f 7263 6520  ld also enforce 
+0000e340: 7468 6973 2061 7420 736f 6d65 2070 6f69  this at some poi
+0000e350: 6e74 2e0a 2020 2020 2020 2020 2020 2020  nt..            
+0000e360: 2020 2020 2020 2020 2320 2020 5468 6520          #   The 
+0000e370: 7573 6572 2073 686f 756c 6420 6265 2061  user should be a
+0000e380: 626c 6520 746f 2066 6978 2060 6578 7465  ble to fix `exte
+0000e390: 726e 5f64 6174 6160 2069 6e20 7468 6520  rn_data` in the 
+0000e3a0: 636f 6e66 6967 0a20 2020 2020 2020 2020  config.         
+0000e3b0: 2020 2020 2020 2020 2020 2023 2020 2073             #   s
+0000e3c0: 7563 6820 7468 6174 2074 6869 7320 6973  uch that this is
+0000e3d0: 2063 6f72 7265 6374 2069 6e20 7468 6520   correct in the 
+0000e3e0: 6669 7273 7420 706c 6163 652e 0a20 2020  first place..   
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e400: 2023 2020 2041 6c73 6f2c 2069 6e20 6164   #   Also, in ad
+0000e410: 6469 7469 6f6e 2074 6f20 7468 6973 2077  dition to this w
+0000e420: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
+0000e430: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0000e440: 7765 206d 6967 6874 2077 616e 7420 746f  we might want to
+0000e450: 2061 6464 2073 6f6d 6520 7275 6e74 696d   add some runtim
+0000e460: 6520 6368 6563 6b20 6f6e 2074 6865 2065  e check on the e
+0000e470: 7120 6f66 2074 6865 2064 796e 2073 697a  q of the dyn siz
+0000e480: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+0000e490: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
+0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4b0: 2020 2020 2020 2022 5761 726e 696e 673a         "Warning:
+0000e4c0: 2061 7373 756d 696e 6720 6469 6d20 7461   assuming dim ta
+0000e4d0: 6773 2061 7265 2073 616d 6520 7769 7468  gs are same with
+0000e4e0: 2064 6966 6665 7265 6e74 2073 697a 6520   different size 
+0000e4f0: 706c 6163 6568 6f6c 6465 7273 3a20 2572  placeholders: %r
+0000e500: 2076 7320 2572 220a 2020 2020 2020 2020   vs %r".        
+0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e520: 2520 2873 656c 662e 6479 6e5f 7369 7a65  % (self.dyn_size
+0000e530: 2c20 6f74 6865 725f 7361 6d65 5f62 6173  , other_same_bas
+0000e540: 652e 6479 6e5f 7369 7a65 290a 2020 2020  e.dyn_size).    
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e560: 290a 2020 2020 2020 2020 2320 4966 2077  ).        # If w
+0000e570: 6520 6861 7665 2061 2064 6566 696e 6564  e have a defined
+0000e580: 2073 6f75 7263 652c 2061 6e64 2074 6869   source, and thi
+0000e590: 7320 6973 2061 2064 796e 616d 6963 2073  s is a dynamic s
+0000e5a0: 7061 7469 616c 2061 7869 732c 2061 6e64  patial axis, and
+0000e5b0: 2069 7420 7761 7320 756e 6465 6669 6e65   it was undefine
+0000e5c0: 6420 6265 666f 7265 2c0a 2020 2020 2020  d before,.      
+0000e5d0: 2020 2320 6d61 7962 6520 7765 2063 616e    # maybe we can
+0000e5e0: 206f 7665 7274 616b 6520 7468 6520 7369   overtake the si
+0000e5f0: 7a65 5f70 6c61 6365 686f 6c64 6572 206e  ze_placeholder n
+0000e600: 6f77 2e0a 2020 2020 2020 2020 6966 206f  ow..        if o
+0000e610: 7468 6572 5f73 616d 655f 6261 7365 2e64  ther_same_base.d
+0000e620: 796e 5f73 697a 6520 6973 206e 6f74 204e  yn_size is not N
+0000e630: 6f6e 6520 616e 6420 7365 6c66 2e5f 6578  one and self._ex
+0000e640: 7472 6120 616e 6420 7365 6c66 2e5f 6578  tra and self._ex
+0000e650: 7472 612e 7372 635f 6461 7461 3a0a 2020  tra.src_data:.  
+0000e660: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000e670: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
+0000e680: 2e5f 6578 7472 612e 7372 635f 6178 6973  ._extra.src_axis
+0000e690: 2c20 696e 7429 0a20 2020 2020 2020 2020  , int).         
+0000e6a0: 2020 2023 204d 6179 6265 2069 7420 6368     # Maybe it ch
+0000e6b0: 616e 6765 6420 696e 2074 6865 206d 6561  anged in the mea
+0000e6c0: 6e77 6869 6c65 2c20 736f 2063 6865 636b  nwhile, so check
+0000e6d0: 2e0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
+0000e6e0: 6720 3d20 7365 6c66 2e5f 6578 7472 612e  g = self._extra.
+0000e6f0: 7372 635f 6461 7461 2e67 6574 5f64 696d  src_data.get_dim
+0000e700: 5f74 6167 2873 656c 662e 5f65 7874 7261  _tag(self._extra
+0000e710: 2e73 7263 5f61 7869 7329 0a20 2020 2020  .src_axis).     
+0000e720: 2020 2020 2020 2069 6620 7461 672e 6465         if tag.de
+0000e730: 7363 7269 7074 696f 6e20 3d3d 2073 656c  scription == sel
+0000e740: 662e 6465 7363 7269 7074 696f 6e20 616e  f.description an
+0000e750: 6420 286e 6f74 2074 6167 2e64 796e 5f73  d (not tag.dyn_s
+0000e760: 697a 655f 6578 7420 6f72 206e 6f74 2074  ize_ext or not t
+0000e770: 6167 2e5f 7661 6c69 6461 7465 5f69 6e5f  ag._validate_in_
+0000e780: 6375 7272 656e 745f 6772 6170 6828 2929  current_graph())
+0000e790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e7a0: 2020 7461 672e 6479 6e5f 7369 7a65 5f65    tag.dyn_size_e
+0000e7b0: 7874 203d 2073 656c 662e 6765 745f 6479  xt = self.get_dy
+0000e7c0: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
+0000e7d0: 6174 6368 5f63 7478 280a 2020 2020 2020  atch_ctx(.      
+0000e7e0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+0000e7f0: 672e 6261 7463 682c 2074 6167 2e63 6f6e  g.batch, tag.con
+0000e800: 7472 6f6c 5f66 6c6f 775f 6374 782c 2074  trol_flow_ctx, t
+0000e810: 656d 706c 6174 655f 6f6e 6c79 3d54 7275  emplate_only=Tru
+0000e820: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000e830: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000e840: 2020 2020 7461 672e 5f6d 6179 6265 5f75      tag._maybe_u
+0000e850: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
+0000e860: 2320 4966 206f 7468 6572 7320 6479 6e5f  # If others dyn_
+0000e870: 7369 7a65 2069 7320 4e6f 6e65 2062 7574  size is None but
+0000e880: 2077 6520 6861 7665 2061 2064 796e 5f73   we have a dyn_s
+0000e890: 697a 652c 206d 6179 6265 2075 7064 6174  ize, maybe updat
+0000e8a0: 6520 6f74 6865 7273 2064 796e 5f73 697a  e others dyn_siz
+0000e8b0: 652e 0a20 2020 2020 2020 2069 6620 7365  e..        if se
+0000e8c0: 6c66 2e64 796e 5f73 697a 6520 6973 206e  lf.dyn_size is n
+0000e8d0: 6f74 204e 6f6e 6520 616e 6420 6f74 6865  ot None and othe
+0000e8e0: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
+0000e8f0: 7369 7a65 2069 7320 6e6f 7420 7365 6c66  size is not self
+0000e900: 2e64 796e 5f73 697a 653a 0a20 2020 2020  .dyn_size:.     
+0000e910: 2020 2020 2020 2023 2043 6f75 6c64 2062         # Could b
+0000e920: 6520 756e 7365 7420 6966 2069 7420 636f  e unset if it co
+0000e930: 6d65 7320 6672 6f6d 2074 6865 2063 6f6e  mes from the con
+0000e940: 6669 672c 206f 7220 6672 6f6d 2070 7265  fig, or from pre
+0000e950: 7620 6772 6170 6820 6372 6561 7469 6f6e  v graph creation
+0000e960: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000e970: 5468 6973 2069 7320 696d 706f 7274 616e  This is importan
+0000e980: 7420 7375 6368 2074 6861 7420 7365 6c66  t such that self
+0000e990: 2e63 616e 5f63 6f6d 7061 7265 2829 2069  .can_compare() i
+0000e9a0: 7320 7361 6e65 2e0a 2020 2020 2020 2020  s sane..        
+0000e9b0: 2020 2020 6966 206f 7468 6572 5f73 616d      if other_sam
+0000e9c0: 655f 6261 7365 2e64 796e 5f73 697a 6520  e_base.dyn_size 
+0000e9d0: 6973 204e 6f6e 6520 6f72 206e 6f74 206f  is None or not o
+0000e9e0: 7468 6572 5f73 616d 655f 6261 7365 2e5f  ther_same_base._
+0000e9f0: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
+0000ea00: 656e 745f 6772 6170 6828 293a 0a20 2020  ent_graph():.   
+0000ea10: 2020 2020 2020 2020 2020 2020 206f 7468               oth
+0000ea20: 6572 5f73 616d 655f 6261 7365 2e64 796e  er_same_base.dyn
+0000ea30: 5f73 697a 655f 6578 7420 3d20 7365 6c66  _size_ext = self
+0000ea40: 2e67 6574 5f64 796e 5f73 697a 655f 6578  .get_dyn_size_ex
+0000ea50: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
+0000ea60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea70: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
+0000ea80: 6261 7365 2e62 6174 6368 2c20 6f74 6865  base.batch, othe
+0000ea90: 725f 7361 6d65 5f62 6173 652e 636f 6e74  r_same_base.cont
+0000eaa0: 726f 6c5f 666c 6f77 5f63 7478 2c20 7465  rol_flow_ctx, te
+0000eab0: 6d70 6c61 7465 5f6f 6e6c 793d 5472 7565  mplate_only=True
+0000eac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ead0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000eae0: 2020 206f 7468 6572 5f73 616d 655f 6261     other_same_ba
+0000eaf0: 7365 2e5f 6d61 7962 655f 7570 6461 7465  se._maybe_update
+0000eb00: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
+0000eb10: 7420 7365 6c66 2e64 796e 5f73 697a 655f  t self.dyn_size_
+0000eb20: 6578 7420 6f72 206e 6f74 2073 656c 662e  ext or not self.
+0000eb30: 5f76 616c 6964 6174 655f 696e 5f63 7572  _validate_in_cur
+0000eb40: 7265 6e74 5f67 7261 7068 2829 3a0a 2020  rent_graph():.  
+0000eb50: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000eb60: 796e 5f73 697a 655f 6578 7420 3d20 6f74  yn_size_ext = ot
+0000eb70: 6865 725f 7361 6d65 5f62 6173 652e 6765  her_same_base.ge
+0000eb80: 745f 6479 6e5f 7369 7a65 5f65 7874 5f66  t_dyn_size_ext_f
+0000eb90: 6f72 5f62 6174 6368 5f63 7478 280a 2020  or_batch_ctx(.  
+0000eba0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ebb0: 6c66 2e62 6174 6368 2c20 7365 6c66 2e63  lf.batch, self.c
+0000ebc0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 782c  ontrol_flow_ctx,
+0000ebd0: 2074 656d 706c 6174 655f 6f6e 6c79 3d54   template_only=T
+0000ebe0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000ebf0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000ec00: 6c66 2e5f 6d61 7962 655f 7570 6461 7465  lf._maybe_update
+0000ec10: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
+0000ec20: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000ec30: 6479 6e5f 7369 7a65 5f65 7874 2069 7320  dyn_size_ext is 
+0000ec40: 4e6f 6e65 206f 7220 6e6f 7420 6f74 6865  None or not othe
+0000ec50: 725f 7361 6d65 5f62 6173 652e 5f76 616c  r_same_base._val
+0000ec60: 6964 6174 655f 696e 5f63 7572 7265 6e74  idate_in_current
+0000ec70: 5f67 7261 7068 2829 3a0a 2020 2020 2020  _graph():.      
+0000ec80: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
+0000ec90: 5f62 6173 652e 6479 6e5f 7369 7a65 5f65  _base.dyn_size_e
+0000eca0: 7874 203d 2073 656c 662e 6765 745f 6479  xt = self.get_dy
+0000ecb0: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
+0000ecc0: 6174 6368 5f63 7478 280a 2020 2020 2020  atch_ctx(.      
+0000ecd0: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
+0000ece0: 7361 6d65 5f62 6173 652e 6261 7463 682c  same_base.batch,
+0000ecf0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000ed00: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000ed10: 782c 2074 656d 706c 6174 655f 6f6e 6c79  x, template_only
+0000ed20: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
+0000ed30: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000ed40: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000ed50: 5f6d 6179 6265 5f75 7064 6174 6528 290a  _maybe_update().
+0000ed60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ed70: 6973 5f64 696d 5f6b 6e6f 776e 2829 2061  is_dim_known() a
+0000ed80: 6e64 206f 7468 6572 2e69 735f 6469 6d5f  nd other.is_dim_
+0000ed90: 6b6e 6f77 6e28 293a 0a20 2020 2020 2020  known():.       
+0000eda0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+0000edb0: 2e64 696d 656e 7369 6f6e 203d 3d20 6f74  .dimension == ot
+0000edc0: 6865 722e 6469 6d65 6e73 696f 6e0a 2020  her.dimension.  
+0000edd0: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+0000ede0: 6973 5f64 696d 5f6b 6e6f 776e 2829 2061  is_dim_known() a
+0000edf0: 6e64 206e 6f74 206f 7468 6572 2e69 735f  nd not other.is_
+0000ee00: 6469 6d5f 6b6e 6f77 6e28 293a 0a20 2020  dim_known():.   
+0000ee10: 2020 2020 2020 2020 206f 7468 6572 2e63           other.c
+0000ee20: 6170 6163 6974 7920 3d20 7365 6c66 2e63  apacity = self.c
+0000ee30: 6170 6163 6974 790a 2020 2020 2020 2020  apacity.        
+0000ee40: 2020 2020 6f74 6865 722e 7369 7a65 203d      other.size =
+0000ee50: 2073 656c 662e 7369 7a65 0a20 2020 2020   self.size.     
+0000ee60: 2020 2065 6c69 6620 6e6f 7420 7365 6c66     elif not self
+0000ee70: 2e69 735f 6469 6d5f 6b6e 6f77 6e28 2920  .is_dim_known() 
+0000ee80: 616e 6420 6f74 6865 722e 6973 5f64 696d  and other.is_dim
+0000ee90: 5f6b 6e6f 776e 2829 3a0a 2020 2020 2020  _known():.      
+0000eea0: 2020 2020 2020 7365 6c66 2e63 6170 6163        self.capac
+0000eeb0: 6974 7920 3d20 6f74 6865 722e 6361 7061  ity = other.capa
+0000eec0: 6369 7479 0a20 2020 2020 2020 2020 2020  city.           
+0000eed0: 2073 656c 662e 7369 7a65 203d 206f 7468   self.size = oth
+0000eee0: 6572 2e73 697a 650a 2020 2020 2020 2020  er.size.        
+0000eef0: 6966 2073 656c 662e 766f 6361 6220 616e  if self.vocab an
+0000ef00: 6420 6e6f 7420 6f74 6865 725f 7361 6d65  d not other_same
+0000ef10: 5f62 6173 652e 766f 6361 623a 0a20 2020  _base.vocab:.   
+0000ef20: 2020 2020 2020 2020 206f 7468 6572 5f73           other_s
+0000ef30: 616d 655f 6261 7365 2e76 6f63 6162 203d  ame_base.vocab =
+0000ef40: 2073 656c 662e 766f 6361 620a 2020 2020   self.vocab.    
+0000ef50: 2020 2020 656c 6966 206f 7468 6572 5f73      elif other_s
+0000ef60: 616d 655f 6261 7365 2e76 6f63 6162 2061  ame_base.vocab a
+0000ef70: 6e64 206e 6f74 2073 656c 662e 766f 6361  nd not self.voca
+0000ef80: 623a 0a20 2020 2020 2020 2020 2020 2073  b:.            s
+0000ef90: 656c 662e 766f 6361 6220 3d20 6f74 6865  elf.vocab = othe
+0000efa0: 725f 7361 6d65 5f62 6173 652e 766f 6361  r_same_base.voca
+0000efb0: 620a 2020 2020 2020 2020 7365 6c66 2e5f  b.        self._
+0000efc0: 6d61 6b65 5f65 7874 7261 2829 0a20 2020  make_extra().   
+0000efd0: 2020 2020 2073 656c 665f 7361 6d65 5f61       self_same_a
+0000efe0: 732e 5f6d 616b 655f 6578 7472 6128 290a  s._make_extra().
+0000eff0: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
+0000f000: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
+0000f010: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
+0000f020: 2073 656c 662e 5f65 7874 7261 2e61 7574   self._extra.aut
+0000f030: 6f5f 6765 6e65 7261 7465 6420 3d20 7365  o_generated = se
+0000f040: 6c66 5f73 616d 655f 6173 2e5f 6578 7472  lf_same_as._extr
+0000f050: 612e 6175 746f 5f67 656e 6572 6174 6564  a.auto_generated
+0000f060: 203d 206f 7468 6572 5f73 616d 655f 6261   = other_same_ba
+0000f070: 7365 2e61 7574 6f5f 6765 6e65 7261 7465  se.auto_generate
+0000f080: 640a 2020 2020 2020 2020 2320 5461 6b65  d.        # Take
+0000f090: 206f 7665 7220 6465 7269 7665 645f 6672   over derived_fr
+0000f0a0: 6f6d 5f6f 702e 2048 6f77 6576 6572 2c20  om_op. However, 
+0000f0b0: 6f6e 6c79 2069 6620 7468 6973 2077 6f75  only if this wou
+0000f0c0: 6c64 206e 6f74 2069 6e74 726f 6475 6365  ld not introduce
+0000f0d0: 2063 7963 6c65 7321 0a20 2020 2020 2020   cycles!.       
+0000f0e0: 2069 6620 6e6f 7420 7365 6c66 5f64 6572   if not self_der
+0000f0f0: 6976 6564 5f62 6173 6573 2e69 7373 7570  ived_bases.issup
+0000f100: 6572 7365 7428 6f74 6865 725f 6465 7269  erset(other_deri
+0000f110: 7665 645f 6261 7365 7329 3a0a 2020 2020  ved_bases):.    
+0000f120: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f130: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
+0000f140: 616e 6420 6e6f 7420 6f74 6865 725f 7361  and not other_sa
+0000f150: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
+0000f160: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
+0000f170: 2020 2020 2020 2020 2023 206e 6f69 6e73           # noins
+0000f180: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
+0000f190: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
+0000f1a0: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
+0000f1b0: 7361 6d65 5f62 6173 652e 5f6d 616b 655f  same_base._make_
+0000f1c0: 6578 7472 6128 292e 6465 7269 7665 645f  extra().derived_
+0000f1d0: 6672 6f6d 5f6f 7020 3d20 7365 6c66 2e64  from_op = self.d
+0000f1e0: 6572 6976 6564 5f66 726f 6d5f 6f70 0a20  erived_from_op. 
+0000f1f0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0000f200: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000f210: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
+0000f220: 616e 6420 6e6f 7420 7365 6c66 2e64 6572  and not self.der
+0000f230: 6976 6564 5f66 726f 6d5f 6f70 3a0a 2020  ived_from_op:.  
+0000f240: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f250: 6c66 2e5f 6d61 6b65 5f65 7874 7261 2829  lf._make_extra()
+0000f260: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+0000f270: 203d 206f 7468 6572 5f73 616d 655f 6261   = other_same_ba
+0000f280: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
+0000f290: 6f70 0a20 2020 2020 2020 2069 6620 7365  op.        if se
+0000f2a0: 6c66 2e5f 6578 7472 6120 616e 6420 6e6f  lf._extra and no
+0000f2b0: 7420 6f74 6865 725f 7361 6d65 5f62 6173  t other_same_bas
+0000f2c0: 652e 6973 5f64 796e 616d 6963 2829 3a0a  e.is_dynamic():.
+0000f2d0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+0000f2e0: 6f73 6520 6d69 6768 7420 6265 2073 6574  ose might be set
+0000f2f0: 2076 6961 2067 6574 5f62 6174 6368 5f66   via get_batch_f
+0000f300: 6f72 5f63 7478 2066 6f72 2061 6e20 756e  or_ctx for an un
+0000f310: 6465 6669 6e65 6420 6469 6d2c 0a20 2020  defined dim,.   
+0000f320: 2020 2020 2020 2020 2023 2077 6869 6368           # which
+0000f330: 206e 6f77 2062 6563 6f6d 6573 2073 7461   now becomes sta
+0000f340: 7469 6320 6475 6520 746f 2060 6f74 6865  tic due to `othe
+0000f350: 7260 2e0a 2020 2020 2020 2020 2020 2020  r`..            
+0000f360: 7365 6c66 2e5f 6578 7472 612e 6261 7463  self._extra.batc
+0000f370: 6820 3d20 4e6f 6e65 0a20 2020 2020 2020  h = None.       
+0000f380: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
+0000f390: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000f3a0: 7820 3d20 4e6f 6e65 0a20 2020 2020 2020  x = None.       
+0000f3b0: 2020 2020 2066 6f72 206b 6579 2c20 6469       for key, di
+0000f3c0: 6d5f 2069 6e20 7365 6c66 2e5f 6578 7472  m_ in self._extr
+0000f3d0: 612e 7361 6d65 5f66 6f72 5f62 6174 6368  a.same_for_batch
+0000f3e0: 5f63 7478 2e69 7465 6d73 2829 3a0a 2020  _ctx.items():.  
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000f400: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+0000f410: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
+0000f420: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000f430: 696d 5f65 7874 7261 203d 2064 696d 5f2e  im_extra = dim_.
+0000f440: 5f65 7874 7261 0a20 2020 2020 2020 2020  _extra.         
+0000f450: 2020 2020 2020 2069 6620 6469 6d5f 6578         if dim_ex
+0000f460: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+0000f470: 2020 2020 2020 2020 2064 696d 5f65 7874           dim_ext
+0000f480: 7261 2e62 6174 6368 203d 204e 6f6e 650a  ra.batch = None.
+0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4a0: 2020 2020 6469 6d5f 6578 7472 612e 636f      dim_extra.co
+0000f4b0: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
+0000f4c0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+0000f4d0: 2073 656c 662e 6261 7463 683a 0a20 2020   self.batch:.   
+0000f4e0: 2020 2020 2020 2020 2073 656c 665f 203d           self_ =
+0000f4f0: 2073 656c 662e 6765 745f 666f 725f 6261   self.get_for_ba
+0000f500: 7463 685f 6374 7828 6261 7463 683d 7365  tch_ctx(batch=se
+0000f510: 6c66 2e62 6174 6368 2c20 6374 783d 7365  lf.batch, ctx=se
+0000f520: 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  lf.control_flow_
+0000f530: 6374 7829 0a20 2020 2020 2020 2020 2020  ctx).           
+0000f540: 2069 6620 7365 6c66 5f20 6973 206e 6f74   if self_ is not
+0000f550: 2073 656c 663a 0a20 2020 2020 2020 2020   self:.         
+0000f560: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+0000f570: 726f 6c5f 666c 6f77 5f63 7478 203d 2073  rol_flow_ctx = s
+0000f580: 656c 665f 2e63 6f6e 7472 6f6c 5f66 6c6f  elf_.control_flo
+0000f590: 775f 6374 7820 2023 206d 6967 6874 2062  w_ctx  # might b
+0000f5a0: 6520 6469 6666 6572 656e 740a 2020 2020  e different.    
+0000f5b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f5c0: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
+0000f5d0: 7365 6c66 5f2e 6479 6e5f 7369 7a65 5f65  self_.dyn_size_e
+0000f5e0: 7874 2020 2320 6d69 6768 7420 6265 2075  xt  # might be u
+0000f5f0: 6e73 6574 0a0a 2020 2020 6465 6620 5f6d  nset..    def _m
+0000f600: 6572 6765 5f73 616d 655f 666f 725f 6261  erge_same_for_ba
+0000f610: 7463 685f 6374 785f 6469 6374 2873 656c  tch_ctx_dict(sel
+0000f620: 663a 205f 642e 4469 6d2c 206f 7468 6572  f: _d.Dim, other
+0000f630: 3a20 5f64 2e44 696d 293a 0a20 2020 2020  : _d.Dim):.     
+0000f640: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+0000f650: 7061 7261 6d20 6f74 6865 723a 0a20 2020  param other:.   
+0000f660: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f670: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
+0000f680: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
+0000f690: 720a 2020 2020 2020 2020 6966 206e 6f74  r.        if not
+0000f6a0: 2073 656c 662e 5f65 7874 7261 2061 6e64   self._extra and
+0000f6b0: 206e 6f74 206f 7468 6572 2e5f 6578 7472   not other._extr
+0000f6c0: 613a 0a20 2020 2020 2020 2020 2020 2072  a:.            r
+0000f6d0: 6574 7572 6e0a 2020 2020 2020 2020 7365  eturn.        se
+0000f6e0: 6c66 2e5f 7661 6c69 6461 7465 5f69 6e5f  lf._validate_in_
+0000f6f0: 6375 7272 656e 745f 6772 6170 6828 290a  current_graph().
+0000f700: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f710: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
+0000f720: 2020 2020 666f 7220 5f2c 2064 696d 2069      for _, dim i
+0000f730: 6e20 6c69 7374 2873 656c 662e 5f65 7874  n list(self._ext
+0000f740: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+0000f750: 685f 6374 782e 6974 656d 7328 2929 3a0a  h_ctx.items()):.
 0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f770: 2020 2020 636f 6e74 696e 7565 2020 2320      continue  # 
-0000f780: 6b65 6570 206f 7572 730a 2020 2020 2020  keep ours.      
-0000f790: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000f7a0: 2064 696d 2e64 796e 5f73 697a 655f 6578   dim.dyn_size_ex
-0000f7b0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000f7c0: 2020 2020 2020 2063 6f6e 7469 6e75 6520         continue 
-0000f7d0: 2023 2075 6e64 6566 696e 6564 2c20 646f   # undefined, do
-0000f7e0: 206e 6f74 206f 7665 7274 616b 650a 2020   not overtake.  
-0000f7f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f800: 6c66 2e5f 6578 7472 612e 7361 6d65 5f66  lf._extra.same_f
-0000f810: 6f72 5f62 6174 6368 5f63 7478 5b6b 6579  or_batch_ctx[key
-0000f820: 5d20 3d20 6469 6d0a 2020 2020 2020 2020  ] = dim.        
-0000f830: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
-0000f840: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
-0000f850: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-0000f860: 206f 7468 6572 2e5f 6578 7472 612e 7361   other._extra.sa
-0000f870: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
-0000f880: 2e63 6c65 6172 2829 2020 2320 7765 206f  .clear()  # we o
-0000f890: 6e6c 7920 7761 6e74 2074 6f20 6861 7665  nly want to have
-0000f8a0: 2069 7420 6f6e 6365 0a0a 2020 2020 2320   it once..    # 
-0000f8b0: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-0000f8c0: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-0000f8d0: 2020 2064 6566 2064 6572 6976 655f 6672     def derive_fr
-0000f8e0: 6f6d 2873 656c 663a 205f 642e 4469 6d2c  om(self: _d.Dim,
-0000f8f0: 2062 6173 653a 205f 642e 4469 6d2c 2073   base: _d.Dim, s
-0000f900: 6574 5f64 6572 6976 6564 5f66 726f 6d5f  et_derived_from_
-0000f910: 666c 6167 3a20 626f 6f6c 203d 2054 7275  flag: bool = Tru
-0000f920: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
-0000f930: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
-0000f940: 6173 653a 2064 696d 0a20 2020 2020 2020  ase: dim.       
-0000f950: 203a 7061 7261 6d20 7365 745f 6465 7269   :param set_deri
-0000f960: 7665 645f 6672 6f6d 5f66 6c61 673a 0a20  ved_from_flag:. 
-0000f970: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000f980: 2020 2073 656c 665f 6261 7365 203d 2073     self_base = s
-0000f990: 656c 662e 6765 745f 7361 6d65 5f62 6173  elf.get_same_bas
-0000f9a0: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-0000f9b0: 5f62 6173 655f 6578 7472 6120 3d20 7365  _base_extra = se
-0000f9c0: 6c66 5f62 6173 652e 5f6d 616b 655f 6578  lf_base._make_ex
-0000f9d0: 7472 6128 290a 2020 2020 2020 2020 6966  tra().        if
-0000f9e0: 2073 6574 5f64 6572 6976 6564 5f66 726f   set_derived_fro
-0000f9f0: 6d5f 666c 6167 3a0a 2020 2020 2020 2020  m_flag:.        
-0000fa00: 2020 2020 6966 2073 656c 665f 6261 7365      if self_base
-0000fa10: 5f65 7874 7261 2e64 6572 6976 6564 5f66  _extra.derived_f
-0000fa20: 726f 6d5f 7461 673a 0a20 2020 2020 2020  rom_tag:.       
-0000fa30: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000fa40: 7365 6c66 5f62 6173 655f 6578 7472 612e  self_base_extra.
-0000fa50: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
-0000fa60: 203d 3d20 6261 7365 0a20 2020 2020 2020   == base.       
-0000fa70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000fa80: 2020 2020 2020 2020 2020 2073 656c 665f             self_
-0000fa90: 6261 7365 5f65 7874 7261 2e64 6572 6976  base_extra.deriv
-0000faa0: 6564 5f66 726f 6d5f 7461 6720 3d20 6261  ed_from_tag = ba
-0000fab0: 7365 0a20 2020 2020 2020 2069 6620 6e6f  se.        if no
-0000fac0: 7420 7365 6c66 2e62 6174 6368 2061 6e64  t self.batch and
-0000fad0: 2062 6173 652e 6261 7463 683a 0a20 2020   base.batch:.   
-0000fae0: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
-0000faf0: 7463 6820 3d20 6261 7365 2e62 6174 6368  tch = base.batch
-0000fb00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fb10: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
-0000fb20: 7478 203d 2062 6173 652e 636f 6e74 726f  tx = base.contro
-0000fb30: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
-0000fb40: 2020 2020 2020 206b 6579 203d 2062 6173         key = bas
-0000fb50: 652e 6261 7463 682c 2062 6173 652e 636f  e.batch, base.co
-0000fb60: 6e74 726f 6c5f 666c 6f77 5f63 7478 0a20  ntrol_flow_ctx. 
-0000fb70: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000fb80: 7420 6b65 7920 6e6f 7420 696e 2073 656c  t key not in sel
-0000fb90: 665f 6261 7365 5f65 7874 7261 2e73 616d  f_base_extra.sam
-0000fba0: 655f 666f 725f 6261 7463 685f 6374 780a  e_for_batch_ctx.
-0000fbb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fbc0: 5f62 6173 655f 6578 7472 612e 7361 6d65  _base_extra.same
-0000fbd0: 5f66 6f72 5f62 6174 6368 5f63 7478 5b6b  _for_batch_ctx[k
-0000fbe0: 6579 5d20 3d20 7365 6c66 0a20 2020 2020  ey] = self.     
-0000fbf0: 2020 2069 6620 7365 6c66 2e69 735f 6479     if self.is_dy
-0000fc00: 6e61 6d69 6328 2920 6f72 206e 6f74 2073  namic() or not s
-0000fc10: 656c 662e 6973 5f64 696d 5f6b 6e6f 776e  elf.is_dim_known
-0000fc20: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000fc30: 6966 206e 6f74 2073 656c 662e 6479 6e5f  if not self.dyn_
-0000fc40: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-0000fc50: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
-0000fc60: 652e 6479 6e5f 7369 7a65 5f65 7874 3a0a  e.dyn_size_ext:.
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2020 2020 6966 2062 6173 652e 6261 7463      if base.batc
-0000fc90: 6820 616e 6420 6261 7365 2e62 6174 6368  h and base.batch
-0000fca0: 203d 3d20 7365 6c66 2e62 6174 6368 2061   == self.batch a
-0000fcb0: 6e64 2062 6173 652e 636f 6e74 726f 6c5f  nd base.control_
-0000fcc0: 666c 6f77 5f63 7478 203d 3d20 7365 6c66  flow_ctx == self
-0000fcd0: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000fce0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-0000fcf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fd00: 6479 6e5f 7369 7a65 5f65 7874 203d 2062  dyn_size_ext = b
-0000fd10: 6173 652e 6479 6e5f 7369 7a65 5f65 7874  ase.dyn_size_ext
-0000fd20: 2e63 6f70 795f 7465 6d70 6c61 7465 286e  .copy_template(n
-0000fd30: 616d 653d 2225 733a 7369 7a65 2220 2520  ame="%s:size" % 
-0000fd40: 7365 6c66 5f62 6173 652e 6465 7363 7269  self_base.descri
-0000fd50: 7074 696f 6e29 0a20 2020 2020 2020 2020  ption).         
-0000fd60: 2020 2020 2020 2065 6c69 6620 6261 7365         elif base
-0000fd70: 2e69 735f 6261 7463 685f 6469 6d28 293a  .is_batch_dim():
-0000fd80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd90: 2020 2020 2073 656c 662e 6479 6e5f 7369       self.dyn_si
-0000fda0: 7a65 5f65 7874 203d 205f 742e 5465 6e73  ze_ext = _t.Tens
-0000fdb0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000fdc0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000fdd0: 3d22 2573 3a62 6174 6368 2220 2520 7365  ="%s:batch" % se
-0000fde0: 6c66 5f62 6173 652e 6465 7363 7269 7074  lf_base.descript
-0000fdf0: 696f 6e2c 2073 6861 7065 3d28 292c 2064  ion, shape=(), d
-0000fe00: 7479 7065 3d22 696e 7433 3222 2c20 6261  type="int32", ba
-0000fe10: 7463 685f 6469 6d5f 6178 6973 3d4e 6f6e  tch_dim_axis=Non
-0000fe20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000fe30: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0000fe40: 2063 6f70 795f 6672 6f6d 2873 656c 663a   copy_from(self:
-0000fe50: 2044 696d 2c20 6f74 6865 723a 2044 696d   Dim, other: Dim
-0000fe60: 293a 0a20 2020 2020 2020 2022 2222 6465  ):.        """de
-0000fe70: 6669 6e65 2222 220a 2020 2020 2020 2020  fine""".        
-0000fe80: 7365 6c66 2e73 697a 6520 3d20 6f74 6865  self.size = othe
-0000fe90: 722e 7369 7a65 0a20 2020 2020 2020 2073  r.size.        s
-0000fea0: 656c 662e 6361 7061 6369 7479 203d 206f  elf.capacity = o
-0000feb0: 7468 6572 2e63 6170 6163 6974 790a 2020  ther.capacity.  
-0000fec0: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-0000fed0: 697a 655f 6578 7420 3d20 6f74 6865 722e  ize_ext = other.
-0000fee0: 6479 6e5f 7369 7a65 5f65 7874 0a20 2020  dyn_size_ext.   
-0000fef0: 2020 2020 2073 656c 662e 6465 7269 7665       self.derive
-0000ff00: 5f66 726f 6d28 6f74 6865 7229 0a0a 2020  _from(other)..  
-0000ff10: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-0000ff20: 2020 2064 6566 2067 6574 5f65 7869 7374     def get_exist
-0000ff30: 696e 675f 7461 675f 6672 6f6d 5f63 6f6c  ing_tag_from_col
-0000ff40: 6c65 6374 696f 6e28 636c 732c 206f 7468  lection(cls, oth
-0000ff50: 6572 2c20 7461 6773 2c20 6973 5f65 7175  er, tags, is_equ
-0000ff60: 616c 5f6f 7074 733d 4e6f 6e65 293a 0a20  al_opts=None):. 
-0000ff70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ff80: 2020 203a 7061 7261 6d20 4469 6d20 6f74     :param Dim ot
-0000ff90: 6865 723a 0a20 2020 2020 2020 203a 7061  her:.        :pa
-0000ffa0: 7261 6d20 6c69 7374 5b44 696d 5d7c 7475  ram list[Dim]|tu
-0000ffb0: 706c 655b 4469 6d5d 7c73 6574 5b44 696d  ple[Dim]|set[Dim
-0000ffc0: 5d20 7461 6773 3a0a 2020 2020 2020 2020  ] tags:.        
-0000ffd0: 3a70 6172 616d 2064 6963 745b 7374 725d  :param dict[str]
-0000ffe0: 7c4e 6f6e 6520 6973 5f65 7175 616c 5f6f  |None is_equal_o
-0000fff0: 7074 733a 2070 6173 7365 6420 746f 2044  pts: passed to D
-00010000: 696d 2e69 735f 6571 7561 6c0a 2020 2020  im.is_equal.    
-00010010: 2020 2020 3a72 7479 7065 3a20 4469 6d7c      :rtype: Dim|
-00010020: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00010030: 0a20 2020 2020 2020 2069 6620 6973 5f65  .        if is_e
-00010040: 7175 616c 5f6f 7074 7320 6973 204e 6f6e  qual_opts is Non
-00010050: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00010060: 735f 6571 7561 6c5f 6f70 7473 203d 207b  s_equal_opts = {
-00010070: 7d0a 2020 2020 2020 2020 2320 5765 2064  }.        # We d
-00010080: 6f20 706f 7465 6e74 6961 6c20 6d75 6c74  o potential mult
-00010090: 6970 6c65 2072 6f75 6e64 732c 2073 7563  iple rounds, suc
-000100a0: 6820 7468 6174 2077 6520 7072 6566 6572  h that we prefer
-000100b0: 2022 6d6f 7265 2065 7175 616c 2220 2875   "more equal" (u
-000100c0: 7369 6e67 206c 6573 7320 6973 5f65 7175  sing less is_equ
-000100d0: 616c 5f6f 7074 7329 2e0a 2020 2020 2020  al_opts)..      
-000100e0: 2020 726f 756e 6473 203d 205b 7b7d 5d0a    rounds = [{}].
-000100f0: 2020 2020 2020 2020 6966 2069 735f 6571          if is_eq
-00010100: 7561 6c5f 6f70 7473 3a0a 2020 2020 2020  ual_opts:.      
-00010110: 2020 2020 2020 6966 2022 6272 6f61 6463        if "broadc
-00010120: 6173 745f 6d61 7463 6865 7322 2069 6e20  ast_matches" in 
-00010130: 6973 5f65 7175 616c 5f6f 7074 733a 0a20  is_equal_opts:. 
-00010140: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00010150: 6f75 6e64 732e 6170 7065 6e64 287b 6b3a  ounds.append({k:
-00010160: 2076 2066 6f72 2028 6b2c 2076 2920 696e   v for (k, v) in
-00010170: 2069 735f 6571 7561 6c5f 6f70 7473 2e69   is_equal_opts.i
-00010180: 7465 6d73 2829 2069 6620 6b20 213d 2022  tems() if k != "
-00010190: 6272 6f61 6463 6173 745f 6d61 7463 6865  broadcast_matche
-000101a0: 7322 7d29 0a20 2020 2020 2020 2020 2020  s"}).           
-000101b0: 2072 6f75 6e64 732e 6170 7065 6e64 2869   rounds.append(i
-000101c0: 735f 6571 7561 6c5f 6f70 7473 290a 2020  s_equal_opts).  
-000101d0: 2020 2020 2020 666f 7220 5f69 735f 6571        for _is_eq
-000101e0: 7561 6c5f 6f70 7473 2069 6e20 726f 756e  ual_opts in roun
-000101f0: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-00010200: 666f 7220 5f74 6167 2069 6e20 7461 6773  for _tag in tags
-00010210: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010220: 2020 6966 205f 7461 672e 6973 5f65 7175    if _tag.is_equ
-00010230: 616c 286f 7468 6572 2c20 2a2a 5f69 735f  al(other, **_is_
-00010240: 6571 7561 6c5f 6f70 7473 293a 0a20 2020  equal_opts):.   
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2072 6574 7572 6e20 5f74 6167 0a20 2020   return _tag.   
-00010270: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00010280: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00010290: 6f64 0a20 2020 2064 6566 2067 6574 5f61  od.    def get_a
-000102a0: 6c6c 5f64 696d 656e 7369 6f6e 5f74 6167  ll_dimension_tag
-000102b0: 7328 636c 732c 2064 6174 615f 6c69 7374  s(cls, data_list
-000102c0: 2c20 6973 5f65 7175 616c 5f6f 7074 733d  , is_equal_opts=
-000102d0: 4e6f 6e65 2c20 756e 6971 7565 5f73 6570  None, unique_sep
-000102e0: 6172 6174 655f 6178 6573 3d54 7275 6529  arate_axes=True)
-000102f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010300: 2020 2020 2020 3a70 6172 616d 206c 6973        :param lis
-00010310: 745b 5f74 2e54 656e 736f 725d 2064 6174  t[_t.Tensor] dat
-00010320: 615f 6c69 7374 3a0a 2020 2020 2020 2020  a_list:.        
-00010330: 3a70 6172 616d 2064 6963 745b 7374 725d  :param dict[str]
-00010340: 7c4e 6f6e 6520 6973 5f65 7175 616c 5f6f  |None is_equal_o
-00010350: 7074 733a 2070 6173 7365 6420 746f 2044  pts: passed to D
-00010360: 696d 2e69 735f 6571 7561 6c0a 2020 2020  im.is_equal.    
-00010370: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00010380: 756e 6971 7565 5f73 6570 6172 6174 655f  unique_separate_
-00010390: 6178 6573 3a20 652e 672e 2064 6174 615f  axes: e.g. data_
-000103a0: 6c69 7374 3d5b 4461 7461 2077 6974 6820  list=[Data with 
-000103b0: 7368 6170 6520 2842 2c35 2c35 2c31 3029  shape (B,5,5,10)
-000103c0: 5d20 7265 7375 6c74 7320 696e 2034 2064  ] results in 4 d
-000103d0: 696d 2074 6167 732c 206e 6f74 2033 2e0a  im tags, not 3..
-000103e0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-000103f0: 206c 6973 7420 6f66 2064 696d 656e 7369   list of dimensi
-00010400: 6f6e 2074 6167 732c 2064 6963 7420 666f  on tags, dict fo
-00010410: 7220 6461 7461 202d 3e20 6c69 7374 206f  r data -> list o
-00010420: 6620 6469 6d65 6e73 696f 6e20 7461 6773  f dimension tags
-00010430: 2028 666f 7220 6561 6368 2061 7869 7329   (for each axis)
-00010440: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00010450: 2028 6c69 7374 5b44 696d 5d2c 2075 7469   (list[Dim], uti
-00010460: 6c2e 4469 6374 5265 664b 6579 735b 5f74  l.DictRefKeys[_t
-00010470: 2e54 656e 736f 722c 206c 6973 745b 4469  .Tensor, list[Di
-00010480: 6d5d 5d29 0a20 2020 2020 2020 2022 2222  m]]).        """
-00010490: 0a20 2020 2020 2020 2074 6167 7320 3d20  .        tags = 
-000104a0: 5b5d 0a20 2020 2020 2020 2064 6174 615f  [].        data_
-000104b0: 6178 6573 5f64 6963 7420 3d20 7574 696c  axes_dict = util
-000104c0: 2e44 6963 7452 6566 4b65 7973 2829 2020  .DictRefKeys()  
-000104d0: 2320 7479 7065 3a20 7574 696c 2e44 6963  # type: util.Dic
-000104e0: 7452 6566 4b65 7973 5b5f 742e 5465 6e73  tRefKeys[_t.Tens
-000104f0: 6f72 2c20 4c69 7374 5b44 696d 5d5d 0a20  or, List[Dim]]. 
-00010500: 2020 2020 2020 2066 6f72 2064 6174 6120         for data 
-00010510: 696e 2064 6174 615f 6c69 7374 3a0a 2020  in data_list:.  
-00010520: 2020 2020 2020 2020 2020 6461 7461 5f61            data_a
-00010530: 7865 735f 6469 6374 5b64 6174 615d 203d  xes_dict[data] =
-00010540: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-00010550: 6578 6973 7469 6e67 5f74 6167 5f63 6f6c  existing_tag_col
-00010560: 6c65 6374 696f 6e5f 666f 725f 6461 7461  lection_for_data
-00010570: 203d 206c 6973 7428 7461 6773 2920 6966   = list(tags) if
-00010580: 2075 6e69 7175 655f 7365 7061 7261 7465   unique_separate
-00010590: 5f61 7865 7320 656c 7365 2074 6167 730a  _axes else tags.
-000105a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000105b0: 6178 6973 2069 6e20 7261 6e67 6528 6461  axis in range(da
-000105c0: 7461 2e62 6174 6368 5f6e 6469 6d29 3a0a  ta.batch_ndim):.
-000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 7461 6720 3d20 6461 7461 2e67 6574 5f64  tag = data.get_d
-000105f0: 696d 5f74 6167 2861 7869 7329 0a20 2020  im_tag(axis).   
-00010600: 2020 2020 2020 2020 2020 2020 2065 7869               exi
-00010610: 7374 696e 675f 7461 6720 3d20 636c 732e  sting_tag = cls.
-00010620: 6765 745f 6578 6973 7469 6e67 5f74 6167  get_existing_tag
-00010630: 5f66 726f 6d5f 636f 6c6c 6563 7469 6f6e  _from_collection
-00010640: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010650: 2020 2020 2020 7461 672c 2074 6167 733d        tag, tags=
-00010660: 6578 6973 7469 6e67 5f74 6167 5f63 6f6c  existing_tag_col
-00010670: 6c65 6374 696f 6e5f 666f 725f 6461 7461  lection_for_data
-00010680: 2c20 6973 5f65 7175 616c 5f6f 7074 733d  , is_equal_opts=
-00010690: 6973 5f65 7175 616c 5f6f 7074 730a 2020  is_equal_opts.  
-000106a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 6966 2065 7869 7374 696e 675f 7461 673a  if existing_tag:
-000106d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106e0: 2020 2020 2069 6620 756e 6971 7565 5f73       if unique_s
-000106f0: 6570 6172 6174 655f 6178 6573 3a0a 2020  eparate_axes:.  
-00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010710: 2020 2020 2020 6578 6973 7469 6e67 5f74        existing_t
-00010720: 6167 5f63 6f6c 6c65 6374 696f 6e5f 666f  ag_collection_fo
-00010730: 725f 6461 7461 2e72 656d 6f76 6528 6578  r_data.remove(ex
-00010740: 6973 7469 6e67 5f74 6167 2920 2023 2064  isting_tag)  # d
-00010750: 6f6e 2774 2074 616b 6520 6974 2061 6761  on't take it aga
-00010760: 696e 2066 6f72 2074 6869 7320 6461 7461  in for this data
-00010770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010780: 2020 2020 2072 6570 6c61 6365 5f65 7869       replace_exi
-00010790: 7374 696e 6720 3d20 280a 2020 2020 2020  sting = (.      
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 6578 6973 7469 6e67 5f74 6167 2e75    existing_tag.u
-000107c0: 6e64 6566 696e 6564 2061 6e64 206e 6f74  ndefined and not
-000107d0: 2074 6167 2e75 6e64 6566 696e 6564 2061   tag.undefined a
-000107e0: 6e64 2074 6167 2e64 696d 656e 7369 6f6e  nd tag.dimension
-000107f0: 203d 3d20 6578 6973 7469 6e67 5f74 6167   == existing_tag
-00010800: 2e64 696d 656e 7369 6f6e 0a20 2020 2020  .dimension.     
-00010810: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00010820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010830: 2020 2020 2069 6620 7265 706c 6163 655f       if replace_
-00010840: 6578 6973 7469 6e67 3a20 2023 2052 6570  existing:  # Rep
-00010850: 6c61 6365 2074 6865 2065 7869 7374 696e  lace the existin
-00010860: 6720 6279 2074 6865 206e 6577 2074 6167  g by the new tag
-00010870: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010880: 2020 2020 2020 2020 2020 7461 6773 5b74            tags[t
-00010890: 6167 732e 696e 6465 7828 6578 6973 7469  ags.index(existi
-000108a0: 6e67 5f74 6167 295d 203d 2074 6167 0a20  ng_tag)] = tag. 
-000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108c0: 2020 2020 2020 2066 6f72 205f 2c20 6469         for _, di
-000108d0: 6d73 5f20 696e 2064 6174 615f 6178 6573  ms_ in data_axes
-000108e0: 5f64 6963 742e 6974 656d 7328 293a 0a20  _dict.items():. 
-000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010900: 2020 2020 2020 2020 2020 2064 696d 735f             dims_
-00010910: 5b3a 5d20 3d20 5b74 6167 2069 6620 6420  [:] = [tag if d 
-00010920: 3d3d 2065 7869 7374 696e 675f 7461 6720  == existing_tag 
-00010930: 656c 7365 2064 2066 6f72 2064 2069 6e20  else d for d in 
-00010940: 6469 6d73 5f5d 0a20 2020 2020 2020 2020  dims_].         
-00010950: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00010960: 7869 7374 696e 675f 7461 6720 3d20 7461  xisting_tag = ta
-00010970: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00010980: 2020 656c 7365 3a20 2023 206e 6f20 6578    else:  # no ex
-00010990: 6973 7469 6e67 2074 6167 0a20 2020 2020  isting tag.     
-000109a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000109b0: 6167 732e 6170 7065 6e64 2874 6167 290a  ags.append(tag).
-000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109d0: 6461 7461 5f61 7865 735f 6469 6374 5b64  data_axes_dict[d
-000109e0: 6174 615d 2e61 7070 656e 6428 6578 6973  ata].append(exis
-000109f0: 7469 6e67 5f74 6167 206f 7220 7461 6729  ting_tag or tag)
-00010a00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010a10: 7461 6773 2c20 6461 7461 5f61 7865 735f  tags, data_axes_
-00010a20: 6469 6374 0a0a 2020 2020 4063 6c61 7373  dict..    @class
-00010a30: 6d65 7468 6f64 0a20 2020 2064 6566 2067  method.    def g
-00010a40: 6574 5f75 6e69 715f 636f 6c6c 6563 7469  et_uniq_collecti
-00010a50: 6f6e 2863 6c73 2c20 7461 6773 2c20 6973  on(cls, tags, is
-00010a60: 5f65 7175 616c 5f6f 7074 733d 4e6f 6e65  _equal_opts=None
-00010a70: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00010a80: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
-00010a90: 7374 5b44 696d 5d7c 7475 706c 655b 4469  st[Dim]|tuple[Di
-00010aa0: 6d5d 7c73 6574 5b44 696d 5d20 7461 6773  m]|set[Dim] tags
-00010ab0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-00010ac0: 2064 6963 745b 7374 725d 7c4e 6f6e 6520   dict[str]|None 
-00010ad0: 6973 5f65 7175 616c 5f6f 7074 733a 2070  is_equal_opts: p
-00010ae0: 6173 7365 6420 746f 2044 696d 2e69 735f  assed to Dim.is_
-00010af0: 6571 7561 6c0a 2020 2020 2020 2020 3a72  equal.        :r
-00010b00: 7479 7065 3a20 6c69 7374 5b44 696d 5d0a  type: list[Dim].
-00010b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010b20: 2020 2020 7265 7320 3d20 5b5d 0a20 2020      res = [].   
-00010b30: 2020 2020 2066 6f72 2074 6167 2069 6e20       for tag in 
-00010b40: 7461 6773 3a0a 2020 2020 2020 2020 2020  tags:.          
-00010b50: 2020 6578 203d 2063 6c73 2e67 6574 5f65    ex = cls.get_e
-00010b60: 7869 7374 696e 675f 7461 675f 6672 6f6d  xisting_tag_from
-00010b70: 5f63 6f6c 6c65 6374 696f 6e28 7461 672c  _collection(tag,
-00010b80: 2072 6573 2c20 6973 5f65 7175 616c 5f6f   res, is_equal_o
-00010b90: 7074 733d 6973 5f65 7175 616c 5f6f 7074  pts=is_equal_opt
-00010ba0: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
-00010bb0: 6620 6e6f 7420 6578 3a0a 2020 2020 2020  f not ex:.      
-00010bc0: 2020 2020 2020 2020 2020 7265 732e 6170            res.ap
-00010bd0: 7065 6e64 2874 6167 290a 2020 2020 2020  pend(tag).      
-00010be0: 2020 7265 7475 726e 2072 6573 0a0a 2020    return res..  
-00010bf0: 2020 6465 6620 6765 745f 7369 7a65 5f74    def get_size_t
-00010c00: 656e 736f 7228 7365 6c66 2920 2d3e 205f  ensor(self) -> _
-00010c10: 742e 5465 6e73 6f72 3a0a 2020 2020 2020  t.Tensor:.      
-00010c20: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
-00010c30: 6574 7572 6e3a 2073 697a 6520 7465 6e73  eturn: size tens
-00010c40: 6f72 2c20 6f72 2064 796e 5f73 697a 655f  or, or dyn_size_
-00010c50: 6578 7420 6966 2064 6566 696e 6564 0a20  ext if defined. 
-00010c60: 2020 2020 2020 203a 7274 7970 653a 205f         :rtype: _
-00010c70: 742e 5465 6e73 6f72 0a20 2020 2020 2020  t.Tensor.       
-00010c80: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00010c90: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00010ca0: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-00010cb0: 6574 7572 6e20 7365 6c66 2e64 796e 5f73  eturn self.dyn_s
-00010cc0: 697a 655f 6578 740a 0a20 2020 2020 2020  ize_ext..       
-00010cd0: 2069 6d70 6f72 7420 7265 7475 726e 6e2e   import returnn.
-00010ce0: 6672 6f6e 7465 6e64 2061 7320 7266 0a0a  frontend as rf..
-00010cf0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00010d00: 656c 662e 7369 7a65 2069 7320 6e6f 7420  elf.size is not 
-00010d10: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
-00010d20: 7572 6e20 7266 2e63 6f6e 7665 7274 5f74  urn rf.convert_t
-00010d30: 6f5f 7465 6e73 6f72 2873 656c 662e 7369  o_tensor(self.si
-00010d40: 7a65 2c20 6e61 6d65 3d22 2573 3a73 697a  ze, name="%s:siz
-00010d50: 6522 2025 2073 656c 662e 6465 7363 7269  e" % self.descri
-00010d60: 7074 696f 6e29 0a0a 2020 2020 6465 6620  ption)..    def 
-00010d70: 6765 745f 6469 6d5f 7661 6c75 6528 7365  get_dim_value(se
-00010d80: 6c66 2920 2d3e 2055 6e69 6f6e 5b69 6e74  lf) -> Union[int
-00010d90: 2c20 5f74 2e52 6177 5465 6e73 6f72 5479  , _t.RawTensorTy
-00010da0: 7065 5d3a 0a20 2020 2020 2020 2022 2222  pe]:.        """
-00010db0: 0a20 2020 2020 2020 2049 6e66 6572 7320  .        Infers 
-00010dc0: 7468 6520 6469 6d20 7468 6973 2061 7869  the dim this axi
-00010dd0: 7320 7368 6f75 6c64 2068 6176 6520 6966  s should have if
-00010de0: 2075 6e62 726f 6164 6361 7374 6564 2e0a   unbroadcasted..
-00010df0: 2020 2020 2020 2020 4966 2060 7365 6c66          If `self
-00010e00: 2e73 7263 5f64 6174 6160 2068 6173 2061  .src_data` has a
-00010e10: 2070 6c61 6365 686f 6c64 6572 2c20 7769   placeholder, wi
-00010e20: 6c6c 2075 7365 2074 6865 2073 6861 7065  ll use the shape
-00010e30: 2066 726f 6d20 7468 6572 652e 0a20 2020   from there..   
-00010e40: 2020 2020 204f 7468 6572 7769 7365 2c20       Otherwise, 
-00010e50: 7573 6573 2060 7365 6c66 2e64 696d 656e  uses `self.dimen
-00010e60: 7369 6f6e 6020 2869 6620 7374 6174 6963  sion` (if static
-00010e70: 2920 6f72 2060 7365 6c66 2e64 796e 5f73  ) or `self.dyn_s
-00010e80: 697a 6560 2028 6966 2064 796e 616d 6963  ize` (if dynamic
-00010e90: 292e 0a0a 2020 2020 2020 2020 3a72 6574  )...        :ret
-00010ea0: 7572 6e3a 206d 6178 2873 697a 6520 6f72  urn: max(size or
-00010eb0: 2064 796e 5f73 697a 6529 0a20 2020 2020   dyn_size).     
-00010ec0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00010ed0: 6573 203d 2073 656c 662e 6765 745f 6469  es = self.get_di
-00010ee0: 6d5f 7661 6c75 655f 7465 6e73 6f72 2829  m_value_tensor()
-00010ef0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00010f00: 7374 616e 6365 2872 6573 2c20 5f74 2e54  stance(res, _t.T
-00010f10: 656e 736f 7229 3a0a 2020 2020 2020 2020  ensor):.        
-00010f20: 2020 2020 6173 7365 7274 2072 6573 2e64      assert res.d
-00010f30: 696d 7320 3d3d 2028 290a 2020 2020 2020  ims == ().      
-00010f40: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00010f50: 2e72 6177 5f74 656e 736f 720a 2020 2020  .raw_tensor.    
-00010f60: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-00010f70: 7461 6e63 6528 7265 732c 2069 6e74 290a  tance(res, int).
-00010f80: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00010f90: 6573 0a0a 2020 2020 6465 6620 6765 745f  es..    def get_
-00010fa0: 6469 6d5f 7661 6c75 655f 7465 6e73 6f72  dim_value_tensor
-00010fb0: 2873 656c 6629 202d 3e20 556e 696f 6e5b  (self) -> Union[
-00010fc0: 696e 742c 205f 742e 5465 6e73 6f72 5d3a  int, _t.Tensor]:
-00010fd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010fe0: 2020 2020 2049 6e66 6572 7320 7468 6520       Infers the 
-00010ff0: 6469 6d20 7468 6973 2061 7869 7320 7368  dim this axis sh
-00011000: 6f75 6c64 2068 6176 6520 6966 2075 6e62  ould have if unb
-00011010: 726f 6164 6361 7374 6564 2e0a 2020 2020  roadcasted..    
-00011020: 2020 2020 4966 2060 7365 6c66 2e73 7263      If `self.src
-00011030: 5f64 6174 6160 2068 6173 2061 2070 6c61  _data` has a pla
-00011040: 6365 686f 6c64 6572 2c20 7769 6c6c 2075  ceholder, will u
-00011050: 7365 2074 6865 2073 6861 7065 2066 726f  se the shape fro
-00011060: 6d20 7468 6572 652e 0a20 2020 2020 2020  m there..       
-00011070: 204f 7468 6572 7769 7365 2c20 7573 6573   Otherwise, uses
-00011080: 2060 7365 6c66 2e64 696d 656e 7369 6f6e   `self.dimension
-00011090: 6020 2869 6620 7374 6174 6963 2920 6f72  ` (if static) or
-000110a0: 2060 7365 6c66 2e64 796e 5f73 697a 6560   `self.dyn_size`
-000110b0: 2028 6966 2064 796e 616d 6963 292e 0a0a   (if dynamic)...
-000110c0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-000110d0: 206d 6178 2873 697a 6520 6f72 2064 796e   max(size or dyn
-000110e0: 5f73 697a 6529 0a20 2020 2020 2020 2022  _size).        "
-000110f0: 2222 0a20 2020 2020 2020 2069 6d70 6f72  "".        impor
-00011100: 7420 7265 7475 726e 6e2e 6672 6f6e 7465  t returnn.fronte
-00011110: 6e64 2061 7320 7266 0a0a 2020 2020 2020  nd as rf..      
-00011120: 2020 6966 2073 656c 662e 6469 6d65 6e73    if self.dimens
-00011130: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-00011140: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00011150: 7572 6e20 7365 6c66 2e64 696d 656e 7369  urn self.dimensi
-00011160: 6f6e 0a20 2020 2020 2020 2069 6620 7365  on.        if se
-00011170: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
-00011180: 616e 6420 7365 6c66 2e64 796e 5f73 697a  and self.dyn_siz
-00011190: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
-000111a0: 7220 6973 206e 6f74 204e 6f6e 653a 2020  r is not None:  
-000111b0: 2320 6661 7374 2070 6174 680a 2020 2020  # fast path.    
-000111c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000111d0: 6479 6e5f 7369 7a65 5f65 7874 2e62 6174  dyn_size_ext.bat
-000111e0: 6368 5f6e 6469 6d20 3e20 303a 0a20 2020  ch_ndim > 0:.   
-000111f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00011200: 7572 6e20 7266 2e72 6564 7563 655f 6d61  urn rf.reduce_ma
-00011210: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
-00011220: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
-00011230: 7369 7a65 5f65 7874 2c0a 2020 2020 2020  size_ext,.      
-00011240: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-00011250: 6973 3d73 656c 662e 6479 6e5f 7369 7a65  is=self.dyn_size
-00011260: 5f65 7874 2e64 696d 5f74 6167 732c 0a20  _ext.dim_tags,. 
-00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011280: 2020 2023 204d 6173 6b69 6e67 2069 7320     # Masking is 
-00011290: 6e6f 7420 616c 7761 7973 2070 6f73 7369  not always possi
-000112a0: 626c 6520 6865 7265 2c20 652e 672e 0a20  ble here, e.g.. 
-000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112c0: 2020 2023 2073 656c 6620 3d20 4469 6d7b     # self = Dim{
-000112d0: 2773 656c 662d 6174 742d 6b65 7973 275b  'self-att-keys'[
-000112e0: 2774 696d 653a 7661 723a 6578 7465 726e  'time:var:extern
-000112f0: 5f64 6174 613a 636c 6173 7365 7327 5b42  _data:classes'[B
-00011300: 5d5d 7d2e 0a20 2020 2020 2020 2020 2020  ]]}..           
-00011310: 2020 2020 2020 2020 2075 7365 5f6d 6173           use_mas
-00011320: 6b3d 4661 6c73 652c 0a20 2020 2020 2020  k=False,.       
-00011330: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00011340: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00011350: 6c66 2e64 796e 5f73 697a 655f 6578 740a  lf.dyn_size_ext.
-00011360: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011370: 6973 5f62 6174 6368 5f64 696d 2829 3a0a  is_batch_dim():.
-00011380: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00011390: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-000113a0: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
-000113b0: 6120 616e 6420 7365 6c66 2e5f 6578 7472  a and self._extr
-000113c0: 612e 7372 635f 6461 7461 3a0a 2020 2020  a.src_data:.    
-000113d0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-000113e0: 3d20 7365 6c66 2e5f 6578 7472 612e 7372  = self._extra.sr
-000113f0: 635f 6461 7461 2e67 6574 5f62 6174 6368  c_data.get_batch
-00011400: 5f64 696d 2829 0a20 2020 2020 2020 2020  _dim().         
-00011410: 2020 2065 6c69 6620 7365 6c66 2e62 6174     elif self.bat
-00011420: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-00011430: 2020 2020 7265 7320 3d20 7365 6c66 2e62      res = self.b
-00011440: 6174 6368 2e64 696d 0a20 2020 2020 2020  atch.dim.       
-00011450: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00011460: 6365 2872 6573 2c20 696e 7429 3a0a 2020  ce(res, int):.  
-00011470: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00011480: 7475 726e 2072 6573 0a20 2020 2020 2020  turn res.       
-00011490: 2020 2020 2069 6620 7265 7320 6973 206e       if res is n
-000114a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000114b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000114c0: 5f74 2e54 656e 736f 7228 2262 6174 6368  _t.Tensor("batch
-000114d0: 222c 2064 696d 733d 2829 2c20 6474 7970  ", dims=(), dtyp
-000114e0: 653d 7266 2e67 6574 5f64 6566 6175 6c74  e=rf.get_default
-000114f0: 5f61 7272 6179 5f69 6e64 6578 5f64 7479  _array_index_dty
-00011500: 7065 2829 2c20 7261 775f 7465 6e73 6f72  pe(), raw_tensor
-00011510: 3d72 6573 290a 2020 2020 2020 2020 6966  =res).        if
-00011520: 2028 0a20 2020 2020 2020 2020 2020 2073   (.            s
-00011530: 656c 662e 5f65 7874 7261 0a20 2020 2020  elf._extra.     
-00011540: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
-00011550: 5f65 7874 7261 2e73 7263 5f64 6174 6120  _extra.src_data 
-00011560: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-00011570: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
-00011580: 2e5f 6578 7472 612e 7372 635f 6178 6973  ._extra.src_axis
-00011590: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-000115a0: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
-000115b0: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
-000115c0: 612e 706c 6163 6568 6f6c 6465 7220 6973  a.placeholder is
-000115d0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-000115e0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-000115f0: 2072 6573 203d 2073 656c 662e 5f65 7874   res = self._ext
-00011600: 7261 2e73 7263 5f64 6174 612e 6765 745f  ra.src_data.get_
-00011610: 6469 6d28 7365 6c66 2e5f 6578 7472 612e  dim(self._extra.
-00011620: 7372 635f 6178 6973 290a 2020 2020 2020  src_axis).      
-00011630: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00011640: 6e63 6528 7265 732c 2069 6e74 293a 0a20  nce(res, int):. 
-00011650: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011660: 6574 7572 6e20 7265 730a 2020 2020 2020  eturn res.      
-00011670: 2020 2020 2020 7265 7475 726e 205f 742e        return _t.
-00011680: 5465 6e73 6f72 2822 6261 7463 6822 2c20  Tensor("batch", 
-00011690: 6469 6d73 3d28 292c 2064 7479 7065 3d72  dims=(), dtype=r
-000116a0: 662e 6765 745f 6465 6661 756c 745f 6172  f.get_default_ar
-000116b0: 7261 795f 696e 6465 785f 6474 7970 6528  ray_index_dtype(
-000116c0: 292c 2072 6177 5f74 656e 736f 723d 7265  ), raw_tensor=re
-000116d0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-000116e0: 636f 6d70 6c65 7465 5f64 796e 5f73 697a  complete_dyn_siz
-000116f0: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
-00011700: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00011710: 2061 6e64 2073 656c 662e 6479 6e5f 7369   and self.dyn_si
-00011720: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
-00011730: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00011740: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00011750: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00011760: 2e62 6174 6368 5f6e 6469 6d20 3e20 303a  .batch_ndim > 0:
-00011770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011780: 2072 6574 7572 6e20 7266 2e72 6564 7563   return rf.reduc
-00011790: 655f 6d61 7828 7365 6c66 2e64 796e 5f73  e_max(self.dyn_s
-000117a0: 697a 655f 6578 742c 2061 7869 733d 7365  ize_ext, axis=se
-000117b0: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-000117c0: 6469 6d5f 7461 6773 290a 2020 2020 2020  dim_tags).      
-000117d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000117e0: 662e 6479 6e5f 7369 7a65 5f65 7874 0a20  f.dyn_size_ext. 
-000117f0: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
-00011800: 6570 7469 6f6e 2822 2573 3a20 6e65 6564  eption("%s: need
-00011810: 2070 6c61 6365 686f 6c64 6572 2c20 7365   placeholder, se
-00011820: 6c66 2e64 696d 656e 7369 6f6e 206f 7220  lf.dimension or 
-00011830: 7365 6c66 2e64 796e 5f73 697a 6520 666f  self.dyn_size fo
-00011840: 7220 6469 6d20 7661 6c75 6522 2025 2073  r dim value" % s
-00011850: 656c 6629 0a0a 2020 2020 6465 6620 6178  elf)..    def ax
-00011860: 6973 5f73 706c 6974 5f69 6e66 6f28 7365  is_split_info(se
-00011870: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00011880: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00011890: 3a20 6178 6973 2073 706c 6974 2069 6e66  : axis split inf
-000118a0: 6f2e 2073 6565 203a 6675 6e63 3a60 6765  o. see :func:`ge
-000118b0: 745f 7061 7261 6d5f 6178 6573 5f73 706c  t_param_axes_spl
-000118c0: 6974 5f69 6e66 6f60 2061 6e64 2075 7361  it_info` and usa
-000118d0: 6765 2028 652e 672e 2070 7265 7472 6169  ge (e.g. pretrai
-000118e0: 6e69 6e67 290a 2020 2020 2020 2020 3a72  ning).        :r
-000118f0: 7479 7065 3a20 6c69 7374 5b69 6e74 7c4e  type: list[int|N
-00011900: 6f6e 655d 0a20 2020 2020 2020 2022 2222  one].        """
-00011910: 0a20 2020 2020 2020 2073 616d 655f 6261  .        same_ba
-00011920: 7365 203d 2073 656c 662e 6765 745f 7361  se = self.get_sa
-00011930: 6d65 5f62 6173 6528 290a 2020 2020 2020  me_base().      
-00011940: 2020 6f70 203d 2073 656c 662e 6465 7269    op = self.deri
-00011950: 7665 645f 6672 6f6d 5f6f 7020 6f72 2073  ved_from_op or s
-00011960: 616d 655f 6261 7365 2e64 6572 6976 6564  ame_base.derived
-00011970: 5f66 726f 6d5f 6f70 0a20 2020 2020 2020  _from_op.       
-00011980: 2069 6620 6e6f 7420 6f70 3a0a 2020 2020   if not op:.    
-00011990: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-000119a0: 7365 6c66 2e64 696d 656e 7369 6f6e 5d0a  self.dimension].
-000119b0: 2020 2020 2020 2020 6966 206f 702e 6b69          if op.ki
-000119c0: 6e64 203d 3d20 2261 6464 223a 0a20 2020  nd == "add":.   
-000119d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000119e0: 7375 6d28 5b78 2e61 7869 735f 7370 6c69  sum([x.axis_spli
-000119f0: 745f 696e 666f 2829 2066 6f72 2078 2069  t_info() for x i
-00011a00: 6e20 6f70 2e69 6e70 7574 735d 2c20 5b5d  n op.inputs], []
-00011a10: 2920 2023 2066 6c61 7474 656e 0a20 2020  )  # flatten.   
-00011a20: 2020 2020 2069 6620 6f70 2e6b 696e 6420       if op.kind 
-00011a30: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
-00011a40: 2020 2020 2020 7265 7320 3d20 5b31 5d0a        res = [1].
-00011a50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00011a60: 7820 696e 206f 702e 696e 7075 7473 3a0a  x in op.inputs:.
-00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a80: 7265 7320 3d20 7375 6d28 5b6e 202a 2078  res = sum([n * x
-00011a90: 2e61 7869 735f 7370 6c69 745f 696e 666f  .axis_split_info
-00011aa0: 2829 2069 6620 6e20 6973 206e 6f74 204e  () if n is not N
-00011ab0: 6f6e 6520 656c 7365 204e 6f6e 6520 666f  one else None fo
-00011ac0: 7220 6e20 696e 2072 6573 5d2c 205b 5d29  r n in res], [])
-00011ad0: 2020 2320 666c 6174 7465 6e0a 2020 2020    # flatten.    
-00011ae0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00011af0: 6573 0a20 2020 2020 2020 2072 6574 7572  es.        retur
-00011b00: 6e20 5b73 656c 662e 6469 6d65 6e73 696f  n [self.dimensio
-00011b10: 6e5d 0a0a 2020 2020 6465 6620 5f67 6574  n]..    def _get
-00011b20: 5f73 616d 655f 6261 7365 5f65 7874 7261  _same_base_extra
-00011b30: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
-00011b40: 616c 5b5f 4469 6d45 7874 7261 5d3a 0a20  al[_DimExtra]:. 
-00011b50: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00011b60: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
-00011b70: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00011b80: 6e65 0a20 2020 2020 2020 2062 6173 6520  ne.        base 
-00011b90: 3d20 7365 6c66 2e67 6574 5f73 616d 655f  = self.get_same_
-00011ba0: 6261 7365 2829 0a20 2020 2020 2020 2023  base().        #
-00011bb0: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-00011bc0: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
-00011bd0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-00011be0: 6173 652e 5f65 7874 7261 0a0a 2020 2020  ase._extra..    
-00011bf0: 6465 6620 5f6d 616b 655f 6578 7472 6128  def _make_extra(
-00011c00: 7365 6c66 3a20 5f64 2e44 696d 2920 2d3e  self: _d.Dim) ->
-00011c10: 205f 4469 6d45 7874 7261 3a0a 2020 2020   _DimExtra:.    
-00011c20: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00011c30: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
-00011c40: 2020 2020 7365 6c66 2e5f 6578 7472 6120      self._extra 
-00011c50: 3d20 5f44 696d 4578 7472 6128 6469 6d3d  = _DimExtra(dim=
-00011c60: 7365 6c66 290a 2020 2020 2020 2020 7265  self).        re
-00011c70: 7475 726e 2073 656c 662e 5f65 7874 7261  turn self._extra
-00011c80: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00011c90: 2020 2020 6465 6620 766f 6361 6228 7365      def vocab(se
-00011ca0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00011cb0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00011cc0: 2072 6574 7572 6e6e 2e64 6174 6173 6574   returnn.dataset
-00011cd0: 732e 7574 696c 2e76 6f63 6162 756c 6172  s.util.vocabular
-00011ce0: 792e 566f 6361 6275 6c61 7279 7c4e 6f6e  y.Vocabulary|Non
-00011cf0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-00011d00: 2020 2020 2020 6578 7472 6120 3d20 7365        extra = se
-00011d10: 6c66 2e5f 6765 745f 7361 6d65 5f62 6173  lf._get_same_bas
-00011d20: 655f 6578 7472 6128 290a 2020 2020 2020  e_extra().      
-00011d30: 2020 6966 2065 7874 7261 3a0a 2020 2020    if extra:.    
-00011d40: 2020 2020 2020 2020 7265 7475 726e 2065          return e
-00011d50: 7874 7261 2e76 6f63 6162 0a20 2020 2020  xtra.vocab.     
-00011d60: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00011d70: 2020 2020 4076 6f63 6162 2e73 6574 7465      @vocab.sette
-00011d80: 720a 2020 2020 6465 6620 766f 6361 6228  r.    def vocab(
-00011d90: 7365 6c66 2c20 766f 6361 6229 3a0a 2020  self, vocab):.  
-00011da0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011db0: 2020 3a70 6172 616d 2072 6574 7572 6e6e    :param returnn
-00011dc0: 2e64 6174 6173 6574 732e 7574 696c 2e76  .datasets.util.v
-00011dd0: 6f63 6162 756c 6172 792e 566f 6361 6275  ocabulary.Vocabu
-00011de0: 6c61 7279 7c4e 6f6e 6520 766f 6361 623a  lary|None vocab:
-00011df0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011e00: 2020 2020 2069 6620 766f 6361 6220 6973       if vocab is
-00011e10: 2073 656c 662e 766f 6361 623a 0a20 2020   self.vocab:.   
-00011e20: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00011e30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011e40: 7361 6d65 5f61 733a 0a20 2020 2020 2020  same_as:.       
-00011e50: 2020 2020 2073 656c 662e 6765 745f 7361       self.get_sa
-00011e60: 6d65 5f62 6173 6528 292e 766f 6361 6220  me_base().vocab 
-00011e70: 3d20 766f 6361 620a 2020 2020 2020 2020  = vocab.        
-00011e80: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00011e90: 2020 2065 7874 7261 203d 2073 656c 662e     extra = self.
-00011ea0: 5f67 6574 5f73 616d 655f 6261 7365 5f65  _get_same_base_e
-00011eb0: 7874 7261 2829 0a20 2020 2020 2020 2069  xtra().        i
-00011ec0: 6620 6578 7472 613a 0a20 2020 2020 2020  f extra:.       
-00011ed0: 2020 2020 2065 7874 7261 2e76 6f63 6162       extra.vocab
-00011ee0: 203d 2076 6f63 6162 0a0a 2020 2020 2320   = vocab..    # 
-00011ef0: 5468 6520 6b69 6e64 206f 6620 6f70 6572  The kind of oper
-00011f00: 6174 696f 6e73 2077 6520 6861 7665 3a0a  ations we have:.
-00011f10: 2020 2020 2320 6120 2b20 623a 2070 6164      # a + b: pad
-00011f20: 6469 6e67 2c20 636f 6e63 6174 0a20 2020  ding, concat.   
-00011f30: 2023 2061 202d 2062 3a20 7769 6e64 6f77   # a - b: window
-00011f40: 2077 6974 6820 7661 6c69 6420 6672 616d   with valid fram
-00011f50: 6573 206f 6e6c 790a 2020 2020 2320 6120  es only.    # a 
-00011f60: 2a20 623a 206d 6572 6765 2064 696d 732c  * b: merge dims,
-00011f70: 2075 7073 616d 706c 652c 2074 7261 6e73   upsample, trans
-00011f80: 706f 7365 6420 636f 6e76 2077 6974 6820  posed conv with 
-00011f90: 7374 7269 6469 6e67 0a20 2020 2023 2061  striding.    # a
-00011fa0: 202f 2062 2028 7768 656e 2061 2025 2062   / b (when a % b
-00011fb0: 203d 3d20 3029 3a20 7370 6c69 7420 6469   == 0): split di
-00011fc0: 6d73 2c20 646f 776e 7361 6d70 6c65 2c20  ms, downsample, 
-00011fd0: 636f 6e76 2077 6974 6820 7374 7269 6469  conv with stridi
-00011fe0: 6e67 0a20 2020 2023 2063 6569 6c64 6976  ng.    # ceildiv
-00011ff0: 2861 2c20 6229 3a20 636f 6e76 2077 6974  (a, b): conv wit
-00012000: 6820 7374 7269 6469 6e67 0a20 2020 2023  h striding.    #
-00012010: 2063 7573 746f 6d3a 2072 6570 6561 742c   custom: repeat,
-00012020: 2072 656d 6f76 652c 206d 6173 6b2c 206c   remove, mask, l
-00012030: 6f6f 7020 7769 7468 2064 796e 2065 6e64  oop with dyn end
-00012040: 0a20 2020 2023 204e 6f74 6520 7468 6174  .    # Note that
-00012050: 2077 6520 6469 6666 6572 656e 7469 6174   we differentiat
-00012060: 6520 6265 7477 6565 6e20 7468 6520 6f72  e between the or
-00012070: 6465 722c 2069 2e65 2e20 6120 2b20 6220  der, i.e. a + b 
-00012080: 213d 2062 202b 2061 2e0a 2020 2020 2320  != b + a..    # 
-00012090: 4e6f 7465 2074 6861 7420 7765 2061 6c77  Note that we alw
-000120a0: 6179 7320 6861 7665 2074 6865 2061 7373  ays have the ass
-000120b0: 756d 7074 696f 6e20 7468 6174 2061 2064  umption that a d
-000120c0: 696d 656e 7369 6f6e 2069 7320 6e6f 6e2d  imension is non-
-000120d0: 6e65 6761 7469 7665 2e0a 2020 2020 2320  negative..    # 
-000120e0: 5468 6973 2061 7373 756d 7074 696f 6e20  This assumption 
-000120f0: 6973 206e 6563 6573 7361 7279 2066 6f72  is necessary for
-00012100: 2073 6f6d 6520 7369 6d70 6c69 6669 6361   some simplifica
-00012110: 7469 6f6e 732e 0a20 2020 2023 2068 7474  tions..    # htt
-00012120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00012130: 7277 7468 2d69 362f 7265 7475 726e 6e2f  rwth-i6/returnn/
-00012140: 7075 6c6c 2f38 3533 0a0a 2020 2020 6465  pull/853..    de
-00012150: 6620 5f5f 6164 645f 5f28 7365 6c66 3a20  f __add__(self: 
-00012160: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
-00012170: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012180: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012190: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-000121a0: 7265 7475 726e 3a20 7365 6c66 202b 206f  return: self + o
-000121b0: 7468 6572 2e20 6e6f 7465 2074 6861 7420  ther. note that 
-000121c0: 7468 6973 2069 7320 6e6f 7420 636f 6d6d  this is not comm
-000121d0: 7574 6174 6976 652c 2069 2e65 2e20 6469  utative, i.e. di
-000121e0: 6666 6572 656e 7420 6672 6f6d 206f 7468  fferent from oth
-000121f0: 6572 202b 2073 656c 662e 0a20 2020 2020  er + self..     
-00012200: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-00012210: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012220: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
-00012230: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
-00012240: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
-00012250: 6572 6d2e 6578 7465 6e64 5f61 6464 5f73  erm.extend_add_s
-00012260: 7562 5f28 6f74 6865 722c 206b 696e 643d  ub_(other, kind=
-00012270: 2261 6464 222c 2072 6967 6874 3d54 7275  "add", right=Tru
-00012280: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-00012290: 6e20 7465 726d 2e61 735f 6469 6d28 290a  n term.as_dim().
-000122a0: 0a20 2020 2064 6566 205f 5f72 6164 645f  .    def __radd_
-000122b0: 5f28 7365 6c66 3a20 4469 6d2c 206f 7468  _(self: Dim, oth
-000122c0: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
-000122d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000122e0: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-000122f0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00012300: 6f74 6865 7220 2b20 7365 6c66 0a20 2020  other + self.   
-00012310: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00012320: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012330: 2020 2020 2074 6572 6d20 3d20 5f4f 704c       term = _OpL
-00012340: 696e 6561 7254 6572 6d2e 6672 6f6d 5f64  inearTerm.from_d
-00012350: 696d 2873 656c 6629 0a20 2020 2020 2020  im(self).       
-00012360: 2074 6572 6d2e 6578 7465 6e64 5f61 6464   term.extend_add
-00012370: 5f73 7562 5f28 6f74 6865 722c 206b 696e  _sub_(other, kin
-00012380: 643d 2261 6464 222c 2072 6967 6874 3d46  d="add", right=F
-00012390: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
-000123a0: 7475 726e 2074 6572 6d2e 6173 5f64 696d  turn term.as_dim
-000123b0: 2829 0a0a 2020 2020 6465 6620 5f5f 7375  ()..    def __su
-000123c0: 625f 5f28 7365 6c66 2c20 6f74 6865 7229  b__(self, other)
-000123d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000123e0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-000123f0: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
-00012400: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00012410: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012420: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00012430: 7375 625f 7269 6768 7428 6f74 6865 7229  sub_right(other)
-00012440: 0a0a 2020 2020 6465 6620 7375 625f 7269  ..    def sub_ri
-00012450: 6768 7428 7365 6c66 3a20 4469 6d2c 206f  ght(self: Dim, o
-00012460: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
-00012470: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00012480: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
-00012490: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000124a0: 3a20 7365 6c66 202d 206f 7468 6572 0a20  : self - other. 
-000124b0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-000124c0: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-000124d0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-000124e0: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-000124f0: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00012500: 2020 2074 6572 6d2e 6578 7465 6e64 5f61     term.extend_a
-00012510: 6464 5f73 7562 5f28 6f74 6865 722c 206b  dd_sub_(other, k
-00012520: 696e 643d 2273 7562 222c 2072 6967 6874  ind="sub", right
-00012530: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
-00012540: 6574 7572 6e20 7465 726d 2e61 735f 6469  eturn term.as_di
-00012550: 6d28 290a 0a20 2020 2064 6566 2073 7562  m()..    def sub
-00012560: 5f6c 6566 7428 7365 6c66 3a20 4469 6d2c  _left(self: Dim,
-00012570: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00012580: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00012590: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-000125a0: 723a 0a20 2020 2020 2020 203a 7265 7475  r:.        :retu
-000125b0: 726e 3a20 282d 6f74 6865 7229 202b 2073  rn: (-other) + s
-000125c0: 656c 660a 2020 2020 2020 2020 3a72 7479  elf.        :rty
-000125d0: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
-000125e0: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
-000125f0: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
-00012600: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
-00012610: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
-00012620: 656e 645f 6164 645f 7375 625f 286f 7468  end_add_sub_(oth
-00012630: 6572 2c20 6b69 6e64 3d22 7375 6222 2c20  er, kind="sub", 
-00012640: 7269 6768 743d 4661 6c73 6529 0a20 2020  right=False).   
-00012650: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
-00012660: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
-00012670: 6566 205f 5f6d 756c 5f5f 2873 656c 663a  ef __mul__(self:
-00012680: 2044 696d 2c20 6f74 6865 7229 3a0a 2020   Dim, other):.  
-00012690: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000126a0: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
-000126b0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
-000126c0: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
-000126d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000126e0: 7465 726d 203d 205f 4f70 4c69 6e65 6172  term = _OpLinear
-000126f0: 5465 726d 2e66 726f 6d5f 6469 6d28 7365  Term.from_dim(se
-00012700: 6c66 290a 2020 2020 2020 2020 7465 726d  lf).        term
-00012710: 2e65 7874 656e 645f 6d75 6c5f 6469 765f  .extend_mul_div_
-00012720: 286f 7468 6572 2c20 6b69 6e64 3d22 6d75  (other, kind="mu
-00012730: 6c22 2c20 7269 6768 743d 5472 7565 290a  l", right=True).
-00012740: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00012750: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
-00012760: 2020 6465 6620 5f5f 726d 756c 5f5f 2873    def __rmul__(s
-00012770: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
-00012780: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012790: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-000127a0: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
-000127b0: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-000127c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000127d0: 2020 2020 7465 726d 203d 205f 4f70 4c69      term = _OpLi
-000127e0: 6e65 6172 5465 726d 2e66 726f 6d5f 6469  nearTerm.from_di
-000127f0: 6d28 7365 6c66 290a 2020 2020 2020 2020  m(self).        
-00012800: 7465 726d 2e65 7874 656e 645f 6d75 6c5f  term.extend_mul_
-00012810: 6469 765f 286f 7468 6572 2c20 6b69 6e64  div_(other, kind
-00012820: 3d22 6d75 6c22 2c20 7269 6768 743d 4661  ="mul", right=Fa
-00012830: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
-00012840: 7572 6e20 7465 726d 2e61 735f 6469 6d28  urn term.as_dim(
-00012850: 290a 0a20 2020 2064 6566 205f 5f66 6c6f  )..    def __flo
-00012860: 6f72 6469 765f 5f28 7365 6c66 3a20 4469  ordiv__(self: Di
-00012870: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
-00012880: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00012890: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
-000128a0: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
-000128b0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
-000128c0: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
-000128d0: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
-000128e0: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
-000128f0: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
-00012900: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
-00012910: 6865 722c 206b 696e 643d 2266 6c6f 6f72  her, kind="floor
-00012920: 6469 7622 2c20 7269 6768 743d 5472 7565  div", right=True
-00012930: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00012940: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
-00012950: 2020 2020 6465 6620 5f5f 7472 7565 6469      def __truedi
-00012960: 765f 5f28 7365 6c66 2c20 6f74 6865 7229  v__(self, other)
-00012970: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012980: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00012990: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
-000129a0: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-000129b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000129c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000129d0: 6469 765f 7269 6768 7428 6f74 6865 7229  div_right(other)
-000129e0: 0a0a 2020 2020 6465 6620 6469 765f 6c65  ..    def div_le
-000129f0: 6674 2873 656c 663a 2044 696d 2c20 6f74  ft(self: Dim, ot
-00012a00: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
-00012a10: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00012a20: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
-00012a30: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00012a40: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00012a50: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
-00012a60: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
-00012a70: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
-00012a80: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
-00012a90: 6d75 6c5f 6469 765f 286f 7468 6572 2c20  mul_div_(other, 
-00012aa0: 6b69 6e64 3d22 7472 7565 6469 7622 2c20  kind="truediv", 
-00012ab0: 7269 6768 743d 4661 6c73 6529 0a20 2020  right=False).   
-00012ac0: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
-00012ad0: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
-00012ae0: 6566 2064 6976 5f72 6967 6874 2873 656c  ef div_right(sel
-00012af0: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
-00012b00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012b10: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
-00012b20: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
-00012b30: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
-00012b40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012b50: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
-00012b60: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
-00012b70: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
-00012b80: 726d 2e65 7874 656e 645f 6d75 6c5f 6469  rm.extend_mul_di
-00012b90: 765f 286f 7468 6572 2c20 6b69 6e64 3d22  v_(other, kind="
-00012ba0: 7472 7565 6469 7622 2c20 7269 6768 743d  truediv", right=
-00012bb0: 5472 7565 290a 2020 2020 2020 2020 7265  True).        re
-00012bc0: 7475 726e 2074 6572 6d2e 6173 5f64 696d  turn term.as_dim
-00012bd0: 2829 0a0a 2020 2020 6465 6620 6365 696c  ()..    def ceil
-00012be0: 6469 765f 6c65 6674 2873 656c 663a 2044  div_left(self: D
-00012bf0: 696d 2c20 6f74 6865 7229 3a0a 2020 2020  im, other):.    
-00012c00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012c10: 3a70 6172 616d 2044 696d 7c69 6e74 206f  :param Dim|int o
-00012c20: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
-00012c30: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
-00012c40: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
-00012c50: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
-00012c60: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
-00012c70: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
-00012c80: 7874 656e 645f 6d75 6c5f 6469 765f 286f  xtend_mul_div_(o
-00012c90: 7468 6572 2c20 6b69 6e64 3d22 6365 696c  ther, kind="ceil
-00012ca0: 6469 7622 2c20 7269 6768 743d 4661 6c73  div", right=Fals
-00012cb0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-00012cc0: 6e20 7465 726d 2e61 735f 6469 6d28 290a  n term.as_dim().
-00012cd0: 0a20 2020 2064 6566 2063 6569 6c64 6976  .    def ceildiv
-00012ce0: 5f72 6967 6874 2873 656c 663a 2044 696d  _right(self: Dim
-00012cf0: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00012d00: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00012d10: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
-00012d20: 6572 3a0a 2020 2020 2020 2020 3a72 7479  er:.        :rty
-00012d30: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
-00012d40: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
-00012d50: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
-00012d60: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
-00012d70: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
-00012d80: 656e 645f 6d75 6c5f 6469 765f 286f 7468  end_mul_div_(oth
-00012d90: 6572 2c20 6b69 6e64 3d22 6365 696c 6469  er, kind="ceildi
-00012da0: 7622 2c20 7269 6768 743d 5472 7565 290a  v", right=True).
-00012db0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00012dc0: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
-00012dd0: 2020 6465 6620 5f5f 6e65 675f 5f28 7365    def __neg__(se
-00012de0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00012df0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00012e00: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
-00012e10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012e20: 2d31 202a 2073 656c 660a 0a20 2020 2064  -1 * self..    d
-00012e30: 6566 2069 735f 636f 6e73 7461 6e74 5f73  ef is_constant_s
-00012e40: 7461 7469 635f 6469 6d28 7365 6c66 2920  tatic_dim(self) 
-00012e50: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00012e60: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
-00012e70: 7475 726e 3a20 6465 7269 7665 6420 6f70  turn: derived op
-00012e80: 206f 6620 7479 7065 2063 6f6e 7374 616e   of type constan
-00012e90: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
-00012ea0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00012eb0: 662e 6465 7269 7665 645f 6672 6f6d 5f6f  f.derived_from_o
-00012ec0: 7020 616e 6420 7365 6c66 2e64 6572 6976  p and self.deriv
-00012ed0: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
-00012ee0: 3d3d 2022 636f 6e73 7461 6e74 220a 0a0a  == "constant"...
-00012ef0: 6465 6620 5f6d 616b 655f 636f 6e73 7461  def _make_consta
-00012f00: 6e74 5f73 7461 7469 635f 6469 6d28 7661  nt_static_dim(va
-00012f10: 6c75 652c 206b 696e 643d 4e6f 6e65 293a  lue, kind=None):
-00012f20: 0a20 2020 2022 2222 0a20 2020 203a 7061  .    """.    :pa
-00012f30: 7261 6d20 696e 7420 7661 6c75 653a 0a20  ram int value:. 
-00012f40: 2020 203a 7061 7261 6d20 456e 7469 7479     :param Entity
-00012f50: 7c4e 6f6e 6520 6b69 6e64 3a0a 2020 2020  |None kind:.    
-00012f60: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
-00012f70: 2222 220a 2020 2020 7265 7475 726e 205f  """.    return _
-00012f80: 642e 4469 6d28 0a20 2020 2020 2020 2064  d.Dim(.        d
-00012f90: 696d 656e 7369 6f6e 3d76 616c 7565 2c0a  imension=value,.
-00012fa0: 2020 2020 2020 2020 6b69 6e64 3d6b 696e          kind=kin
-00012fb0: 6420 6f72 2044 696d 5479 7065 732e 556e  d or DimTypes.Un
-00012fc0: 7370 6563 6966 6965 642c 0a20 2020 2020  specified,.     
-00012fd0: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
-00012fe0: 756e 6e61 6d65 645f 2573 6469 6d5f 2569  unnamed_%sdim_%i
-00012ff0: 2220 2520 286b 696e 642e 6e61 6d65 202b  " % (kind.name +
-00013000: 2022 5f22 2069 6620 6b69 6e64 2065 6c73   "_" if kind els
-00013010: 6520 2222 2c20 7661 6c75 6529 2c0a 2020  e "", value),.  
-00013020: 2020 2020 2020 6465 7269 7665 645f 6672        derived_fr
-00013030: 6f6d 5f6f 703d 4f70 286b 696e 643d 2263  om_op=Op(kind="c
-00013040: 6f6e 7374 616e 7422 2c20 696e 7075 7473  onstant", inputs
-00013050: 3d5b 5d2c 2061 7474 7269 6273 3d7b 2276  =[], attribs={"v
-00013060: 616c 7565 223a 2076 616c 7565 7d29 2c0a  alue": value}),.
-00013070: 2020 2020 2020 2020 6175 746f 5f67 656e          auto_gen
-00013080: 6572 6174 6564 3d54 7275 652c 0a20 2020  erated=True,.   
-00013090: 2029 0a0a 0a63 6c61 7373 204f 703a 0a20   )...class Op:. 
-000130a0: 2020 2022 2222 0a20 2020 204f 7020 6f6e     """.    Op on
-000130b0: 203a 636c 6173 733a 6044 696d 6020 7768   :class:`Dim` wh
-000130c0: 6963 6820 7265 7375 6c74 7320 696e 2061  ich results in a
-000130d0: 2064 6572 6976 6564 203a 636c 6173 733a   derived :class:
-000130e0: 6044 696d 602e 0a20 2020 2022 2222 0a0a  `Dim`..    """..
-000130f0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00013100: 2873 656c 662c 206b 696e 642c 2069 6e70  (self, kind, inp
-00013110: 7574 732c 2061 7474 7269 6273 3d4e 6f6e  uts, attribs=Non
-00013120: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
-00013130: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00013140: 7472 206b 696e 643a 2022 6164 6422 2c20  tr kind: "add", 
-00013150: 2273 7562 222c 2022 6d75 6c22 2c20 2263  "sub", "mul", "c
-00013160: 6569 6c64 6976 220a 2020 2020 2020 2020  eildiv".        
-00013170: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
-00013180: 2069 6e70 7574 733a 0a20 2020 2020 2020   inputs:.       
-00013190: 203a 7061 7261 6d20 6469 6374 5b73 7472   :param dict[str
-000131a0: 5d7c 4e6f 6e65 2061 7474 7269 6273 3a0a  ]|None attribs:.
-000131b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000131c0: 2020 2020 7365 6c66 2e6b 696e 6420 3d20      self.kind = 
-000131d0: 6b69 6e64 0a20 2020 2020 2020 2073 656c  kind.        sel
-000131e0: 662e 696e 7075 7473 203d 2069 6e70 7574  f.inputs = input
-000131f0: 730a 2020 2020 2020 2020 7365 6c66 2e6f  s.        self.o
-00013200: 7574 7075 7420 3d20 4e6f 6e65 2020 2320  utput = None  # 
-00013210: 7479 7065 3a20 4f70 7469 6f6e 616c 5b5f  type: Optional[_
-00013220: 642e 4469 6d5d 0a20 2020 2020 2020 2073  d.Dim].        s
-00013230: 656c 662e 6174 7472 6962 7320 3d20 6174  elf.attribs = at
-00013240: 7472 6962 730a 0a20 2020 2064 6566 205f  tribs..    def _
-00013250: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
-00013260: 2020 2020 2020 2061 7474 7269 6273 203d         attribs =
-00013270: 2028 2220 2572 2220 2520 7365 6c66 2e61   (" %r" % self.a
-00013280: 7474 7269 6273 2920 6966 2073 656c 662e  ttribs) if self.
-00013290: 6174 7472 6962 7320 656c 7365 2022 220a  attribs else "".
-000132a0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-000132b0: 3c44 696d 2e4f 7020 2572 2025 7325 733e  <Dim.Op %r %s%s>
-000132c0: 2220 2520 2873 656c 662e 6b69 6e64 2c20  " % (self.kind, 
-000132d0: 7365 6c66 2e69 6e70 7574 732c 2061 7474  self.inputs, att
-000132e0: 7269 6273 290a 0a20 2020 2064 6566 205f  ribs)..    def _
-000132f0: 7661 6c75 6528 7365 6c66 293a 0a20 2020  value(self):.   
-00013300: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00013310: 2e6b 696e 642c 2074 7570 6c65 2873 656c  .kind, tuple(sel
-00013320: 662e 696e 7075 7473 292c 2066 726f 7a65  f.inputs), froze
-00013330: 6e73 6574 2873 656c 662e 6174 7472 6962  nset(self.attrib
-00013340: 732e 6974 656d 7328 2929 2069 6620 7365  s.items()) if se
-00013350: 6c66 2e61 7474 7269 6273 2065 6c73 6520  lf.attribs else 
-00013360: 4e6f 6e65 0a0a 2020 2020 6465 6620 5f5f  None..    def __
-00013370: 6861 7368 5f5f 2873 656c 6629 3a0a 2020  hash__(self):.  
-00013380: 2020 2020 2020 7265 7475 726e 2068 6173        return has
-00013390: 6828 7365 6c66 2e5f 7661 6c75 6528 2929  h(self._value())
-000133a0: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
-000133b0: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
-000133c0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000133d0: 616e 6365 286f 7468 6572 2c20 4f70 293a  ance(other, Op):
-000133e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000133f0: 7572 6e20 7365 6c66 2e5f 7661 6c75 6528  urn self._value(
-00013400: 2920 3d3d 206f 7468 6572 2e5f 7661 6c75  ) == other._valu
-00013410: 6528 290a 2020 2020 2020 2020 7265 7475  e().        retu
-00013420: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
-00013430: 6620 5f5f 6e65 5f5f 2873 656c 662c 206f  f __ne__(self, o
-00013440: 7468 6572 293a 0a20 2020 2020 2020 2072  ther):.        r
-00013450: 6574 7572 6e20 6e6f 7420 7365 6c66 2e5f  eturn not self._
-00013460: 5f65 715f 5f28 6f74 6865 7229 0a0a 0a64  _eq__(other)...d
-00013470: 6566 205f 6765 745f 6465 7363 7269 7074  ef _get_descript
-00013480: 696f 6e28 6469 6d2c 2062 7261 636b 6574  ion(dim, bracket
-00013490: 733d 5472 7565 293a 0a20 2020 2022 2222  s=True):.    """
-000134a0: 0a20 2020 203a 7061 7261 6d20 4469 6d20  .    :param Dim 
-000134b0: 6469 6d3a 0a20 2020 203a 7061 7261 6d20  dim:.    :param 
-000134c0: 626f 6f6c 2062 7261 636b 6574 733a 2061  bool brackets: a
-000134d0: 6464 2062 7261 636b 6574 7320 7768 656e  dd brackets when
-000134e0: 206e 6563 6573 7361 7279 0a20 2020 203a   necessary.    :
-000134f0: 7274 7970 653a 2073 7472 0a20 2020 2022  rtype: str.    "
-00013500: 2222 0a20 2020 2069 6620 6469 6d2e 6465  "".    if dim.de
-00013510: 7363 7269 7074 696f 6e20 616e 6420 6469  scription and di
-00013520: 6d2e 6465 7363 7269 7074 696f 6e2e 7374  m.description.st
-00013530: 6172 7473 7769 7468 2822 756e 6e61 6d65  artswith("unname
-00013540: 645f 2229 2061 6e64 2064 696d 2e64 696d  d_") and dim.dim
-00013550: 656e 7369 6f6e 2069 7320 6e6f 7420 4e6f  ension is not No
-00013560: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
-00013570: 726e 2073 7472 2864 696d 2e64 696d 656e  rn str(dim.dimen
-00013580: 7369 6f6e 290a 2020 2020 6966 2064 696d  sion).    if dim
-00013590: 2e64 6573 6372 6970 7469 6f6e 3a0a 2020  .description:.  
-000135a0: 2020 2020 2020 6966 2062 7261 636b 6574        if bracket
-000135b0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-000135c0: 6d70 6f72 7420 7265 0a0a 2020 2020 2020  mport re..      
-000135d0: 2020 2020 2020 6966 2072 652e 7365 6172        if re.sear
-000135e0: 6368 2822 5b2b 5c5c 2d2f 205d 222c 2064  ch("[+\\-/ ]", d
-000135f0: 696d 2e64 6573 6372 6970 7469 6f6e 293a  im.description):
-00013600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013610: 2072 6574 7572 6e20 2228 2573 2922 2025   return "(%s)" %
-00013620: 2064 696d 2e64 6573 6372 6970 7469 6f6e   dim.description
-00013630: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013640: 6469 6d2e 6465 7363 7269 7074 696f 6e0a  dim.description.
-00013650: 2020 2020 7265 7475 726e 2022 756e 6e61      return "unna
-00013660: 6d65 645f 2573 5f64 696d 2573 2220 2520  med_%s_dim%s" % 
-00013670: 2864 696d 2e6b 696e 642c 2064 696d 2e64  (dim.kind, dim.d
-00013680: 696d 656e 7369 6f6e 2069 6620 6469 6d2e  imension if dim.
-00013690: 6469 6d65 6e73 696f 6e20 6973 206e 6f74  dimension is not
-000136a0: 204e 6f6e 6520 656c 7365 2022 3f22 290a   None else "?").
-000136b0: 0a0a 636c 6173 7320 5f4f 704d 756c 7454  ..class _OpMultT
-000136c0: 6572 6d3a 0a20 2020 2022 2222 0a20 2020  erm:.    """.   
-000136d0: 2072 6570 7265 7365 6e74 7320 7374 6820   represents sth 
-000136e0: 6c69 6b65 2061 202a 2062 202a 2063 0a20  like a * b * c. 
-000136f0: 2020 2022 2222 0a0a 2020 2020 4063 6c61     """..    @cla
-00013700: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00013710: 2066 726f 6d5f 6469 6d28 636c 732c 2064   from_dim(cls, d
-00013720: 696d 3a20 5f64 2e44 696d 2920 2d3e 205f  im: _d.Dim) -> _
-00013730: 4f70 4d75 6c74 5465 726d 3a0a 2020 2020  OpMultTerm:.    
-00013740: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00013750: 3a70 6172 616d 2064 696d 3a0a 2020 2020  :param dim:.    
-00013760: 2020 2020 3a72 6574 7572 6e3a 206f 7020      :return: op 
-00013770: 6d75 6c74 2074 6572 6d0a 2020 2020 2020  mult term.      
-00013780: 2020 2222 220a 2020 2020 2020 2020 6469    """.        di
-00013790: 6d20 3d20 6469 6d2e 6765 745f 7361 6d65  m = dim.get_same
-000137a0: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
-000137b0: 6966 2064 696d 2e64 696d 656e 7369 6f6e  if dim.dimension
-000137c0: 203d 3d20 3120 616e 6420 6469 6d2e 6973   == 1 and dim.is
-000137d0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-000137e0: 5f64 696d 2829 3a0a 2020 2020 2020 2020  _dim():.        
-000137f0: 2020 2020 7265 7475 726e 2063 6c73 2e6f      return cls.o
-00013800: 6e65 2829 0a20 2020 2020 2020 2069 6620  ne().        if 
-00013810: 6469 6d2e 6465 7269 7665 645f 6672 6f6d  dim.derived_from
-00013820: 5f6f 7020 616e 6420 6469 6d2e 6465 7269  _op and dim.deri
-00013830: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
-00013840: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
-00013850: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00013860: 7328 6c69 7374 2864 696d 2e64 6572 6976  s(list(dim.deriv
-00013870: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
-00013880: 7329 290a 2020 2020 2020 2020 7265 7475  s)).        retu
-00013890: 726e 2063 6c73 285b 6469 6d5d 290a 0a20  rn cls([dim]).. 
-000138a0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-000138b0: 2020 2020 6465 6620 6672 6f6d 5f64 696d      def from_dim
-000138c0: 5f66 6163 746f 7273 2863 6c73 2c20 6469  _factors(cls, di
-000138d0: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
-000138e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000138f0: 6c69 7374 5b44 696d 5d20 6469 6d73 3a0a  list[Dim] dims:.
-00013900: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00013910: 4469 6d2e 5f4f 704d 756c 7454 6572 6d0a  Dim._OpMultTerm.
-00013920: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013930: 2020 2020 7265 7320 3d20 636c 732e 6f6e      res = cls.on
-00013940: 6528 290a 2020 2020 2020 2020 666f 7220  e().        for 
-00013950: 6420 696e 2064 696d 733a 0a20 2020 2020  d in dims:.     
-00013960: 2020 2020 2020 2072 6573 2e65 7874 656e         res.exten
-00013970: 645f 6d75 6c5f 6469 765f 2864 2c20 6b69  d_mul_div_(d, ki
-00013980: 6e64 3d22 6d75 6c22 2c20 7269 6768 743d  nd="mul", right=
-00013990: 5472 7565 290a 2020 2020 2020 2020 7265  True).        re
-000139a0: 7475 726e 2072 6573 0a0a 2020 2020 4063  turn res..    @c
-000139b0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-000139c0: 6566 206f 6e65 2863 6c73 293a 0a20 2020  ef one(cls):.   
-000139d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000139e0: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
-000139f0: 4d75 6c74 5465 726d 0a20 2020 2020 2020  MultTerm.       
-00013a00: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00013a10: 7572 6e20 636c 7328 5b5d 290a 0a20 2020  urn cls([])..   
-00013a20: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00013a30: 6c66 2c20 7465 726d 7329 3a0a 2020 2020  lf, terms):.    
-00013a40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00013a50: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
-00013a60: 2074 6572 6d73 3a0a 2020 2020 2020 2020   terms:.        
-00013a70: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-00013a80: 2e74 6572 6d73 203d 2074 6572 6d73 0a0a  .terms = terms..
-00013a90: 2020 2020 6465 6620 5f5f 6861 7368 5f5f      def __hash__
-00013aa0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00013ab0: 7265 7475 726e 2068 6173 6828 7475 706c  return hash(tupl
-00013ac0: 6528 7365 6c66 2e74 6572 6d73 2929 0a0a  e(self.terms))..
-00013ad0: 2020 2020 6465 6620 5f5f 6571 5f5f 2873      def __eq__(s
-00013ae0: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-00013af0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013b00: 203a 7061 7261 6d20 4469 6d7c 4469 6d2e   :param Dim|Dim.
-00013b10: 5f4f 704d 756c 7454 6572 6d20 6f74 6865  _OpMultTerm othe
-00013b20: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
-00013b30: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00013b40: 616e 6365 286f 7468 6572 2c20 5f4f 704d  ance(other, _OpM
-00013b50: 756c 7454 6572 6d29 3a0a 2020 2020 2020  ultTerm):.      
-00013b60: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00013b70: 662e 7465 726d 7320 3d3d 206f 7468 6572  f.terms == other
-00013b80: 2e74 6572 6d73 0a20 2020 2020 2020 2072  .terms.        r
-00013b90: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-00013ba0: 2064 6566 205f 5f6e 655f 5f28 7365 6c66   def __ne__(self
-00013bb0: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00013bc0: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
-00013bd0: 662e 5f5f 6571 5f5f 286f 7468 6572 290a  f.__eq__(other).
-00013be0: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
-00013bf0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00013c00: 2072 6574 7572 6e20 2244 696d 2e5f 4f70   return "Dim._Op
-00013c10: 4d75 6c74 5465 726d 2825 7229 2220 2520  MultTerm(%r)" % 
-00013c20: 2873 656c 662e 7465 726d 732c 290a 0a20  (self.terms,).. 
-00013c30: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00013c40: 2064 6566 2064 696d 656e 7369 6f6e 2873   def dimension(s
-00013c50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00013c60: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
-00013c70: 3a20 696e 747c 4e6f 6e65 0a20 2020 2020  : int|None.     
-00013c80: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-00013c90: 696d 203d 2031 0a20 2020 2020 2020 2066  im = 1.        f
-00013ca0: 6f72 2070 6172 7420 696e 2073 656c 662e  or part in self.
-00013cb0: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
-00013cc0: 2020 2069 6620 7061 7274 2e64 696d 656e     if part.dimen
-00013cd0: 7369 6f6e 2069 7320 4e6f 6e65 3a0a 2020  sion is None:.  
-00013ce0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00013cf0: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00013d00: 2020 2020 2020 6469 6d20 2a3d 2070 6172        dim *= par
-00013d10: 742e 6469 6d65 6e73 696f 6e0a 2020 2020  t.dimension.    
-00013d20: 2020 2020 7265 7475 726e 2064 696d 0a0a      return dim..
-00013d30: 2020 2020 6465 6620 6261 7365 5f74 6572      def base_ter
-00013d40: 6d28 7365 6c66 293a 0a20 2020 2020 2020  m(self):.       
-00013d50: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
-00013d60: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
-00013d70: 2022 2222 0a20 2020 2020 2020 2061 7373   """.        ass
-00013d80: 6572 7420 7365 6c66 2e74 6572 6d73 0a20  ert self.terms. 
-00013d90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00013da0: 6c66 2e74 6572 6d73 5b2d 315d 0a0a 2020  lf.terms[-1]..  
-00013db0: 2020 6465 6620 6973 5f6f 6e65 2873 656c    def is_one(sel
-00013dc0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00013dd0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00013de0: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
-00013df0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013e00: 6e6f 7420 7365 6c66 2e74 6572 6d73 0a0a  not self.terms..
-00013e10: 2020 2020 6465 6620 6973 5f63 6f6e 7374      def is_const
-00013e20: 616e 745f 7374 6174 6963 5f64 696d 2873  ant_static_dim(s
-00013e30: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00013e40: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
-00013e50: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-00013e60: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-00013e70: 7420 7365 6c66 2e74 6572 6d73 3a0a 2020  t self.terms:.  
-00013e80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00013e90: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
-00013ea0: 7475 726e 2061 6c6c 2874 6572 6d2e 6973  turn all(term.is
-00013eb0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00013ec0: 5f64 696d 2829 2066 6f72 2074 6572 6d20  _dim() for term 
-00013ed0: 696e 2073 656c 662e 7465 726d 7329 0a0a  in self.terms)..
-00013ee0: 2020 2020 6465 6620 636f 7079 2873 656c      def copy(sel
-00013ef0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00013f00: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00013f10: 4469 6d2e 5f4f 704d 756c 7454 6572 6d0a  Dim._OpMultTerm.
-00013f20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013f30: 2020 2020 7265 7475 726e 205f 4f70 4d75      return _OpMu
-00013f40: 6c74 5465 726d 286c 6973 7428 7365 6c66  ltTerm(list(self
-00013f50: 2e74 6572 6d73 2929 0a0a 2020 2020 6465  .terms))..    de
-00013f60: 6620 6e65 6761 7469 7665 2873 656c 6629  f negative(self)
-00013f70: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00013f80: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
-00013f90: 6d2e 5f4f 704d 756c 7454 6572 6d0a 2020  m._OpMultTerm.  
-00013fa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013fb0: 2020 6966 2073 656c 662e 7465 726d 7320    if self.terms 
-00013fc0: 616e 6420 7365 6c66 2e74 6572 6d73 5b30  and self.terms[0
-00013fd0: 5d2e 6973 5f63 6f6e 7374 616e 745f 7374  ].is_constant_st
-00013fe0: 6174 6963 5f64 696d 2829 2061 6e64 2073  atic_dim() and s
-00013ff0: 656c 662e 7465 726d 735b 305d 2e64 696d  elf.terms[0].dim
-00014000: 656e 7369 6f6e 203d 3d20 2d31 3a0a 2020  ension == -1:.  
-00014010: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014020: 205f 4f70 4d75 6c74 5465 726d 2873 656c   _OpMultTerm(sel
-00014030: 662e 7465 726d 735b 313a 5d29 0a20 2020  f.terms[1:]).   
-00014040: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-00014050: 636f 7079 2829 0a20 2020 2020 2020 2072  copy().        r
-00014060: 6573 2e65 7874 656e 645f 6d75 6c5f 6469  es.extend_mul_di
-00014070: 765f 285f 6d61 6b65 5f63 6f6e 7374 616e  v_(_make_constan
-00014080: 745f 7374 6174 6963 5f64 696d 282d 3129  t_static_dim(-1)
-00014090: 2c20 6b69 6e64 3d22 6d75 6c22 2c20 7269  , kind="mul", ri
-000140a0: 6768 743d 4661 6c73 6529 0a20 2020 2020  ght=False).     
-000140b0: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
-000140c0: 2020 2064 6566 2064 6976 6973 6962 6c65     def divisible
-000140d0: 2873 656c 662c 206f 7468 6572 2c20 7269  (self, other, ri
-000140e0: 6768 7429 3a0a 2020 2020 2020 2020 2222  ght):.        ""
-000140f0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00014100: 2044 696d 206f 7468 6572 3a0a 2020 2020   Dim other:.    
-00014110: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00014120: 7269 6768 743a 0a20 2020 2020 2020 203a  right:.        :
-00014130: 7265 7475 726e 3a20 7768 6574 6865 7220  return: whether 
-00014140: 7765 2063 616e 2064 6976 6964 6520 6f74  we can divide ot
-00014150: 6865 722c 2077 6974 686f 7574 2072 656d  her, without rem
-00014160: 6169 6e64 6572 0a20 2020 2020 2020 203a  ainder.        :
-00014170: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-00014180: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00014190: 6966 206e 6f74 2073 656c 662e 7465 726d  if not self.term
-000141a0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-000141b0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-000141c0: 2020 2020 6966 206f 7468 6572 2e64 6572      if other.der
-000141d0: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
-000141e0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
-000141f0: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-00014200: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
-00014210: 2020 746d 7020 3d20 7365 6c66 2e63 6f70    tmp = self.cop
-00014220: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-00014230: 666f 7220 7465 726d 2069 6e20 6f74 6865  for term in othe
-00014240: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00014250: 702e 696e 7075 7473 2069 6620 7269 6768  p.inputs if righ
-00014260: 7420 656c 7365 2072 6576 6572 7365 6428  t else reversed(
-00014270: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00014280: 6f6d 5f6f 702e 696e 7075 7473 293a 0a20  om_op.inputs):. 
-00014290: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000142a0: 6620 6e6f 7420 746d 702e 6469 7669 7369  f not tmp.divisi
-000142b0: 626c 6528 7465 726d 2c20 7269 6768 743d  ble(term, right=
-000142c0: 7269 6768 7429 3a0a 2020 2020 2020 2020  right):.        
-000142d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000142e0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-000142f0: 2020 2020 2020 2020 2074 6d70 2e65 7874           tmp.ext
-00014300: 656e 645f 6d75 6c5f 6469 765f 2874 6572  end_mul_div_(ter
-00014310: 6d2c 206b 696e 643d 2274 7275 6564 6976  m, kind="truediv
-00014320: 222c 2072 6967 6874 3d72 6967 6874 290a  ", right=right).
-00014330: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014340: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00014350: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
-00014360: 203d 2073 656c 662e 7465 726d 735b 2d31   = self.terms[-1
-00014370: 2069 6620 7269 6768 7420 656c 7365 2030   if right else 0
-00014380: 5d0a 2020 2020 2020 2020 6966 206f 7468  ].        if oth
-00014390: 6572 203d 3d20 6d6f 7374 5f72 6563 656e  er == most_recen
-000143a0: 745f 7465 726d 3a0a 2020 2020 2020 2020  t_term:.        
-000143b0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-000143c0: 2020 2020 2020 2020 6966 206d 6f73 745f          if most_
-000143d0: 7265 6365 6e74 5f74 6572 6d2e 6469 6d65  recent_term.dime
-000143e0: 6e73 696f 6e20 6973 206e 6f74 204e 6f6e  nsion is not Non
-000143f0: 6520 616e 6420 6f74 6865 722e 6469 6d65  e and other.dime
-00014400: 6e73 696f 6e20 6973 206e 6f74 204e 6f6e  nsion is not Non
-00014410: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00014420: 6620 6d6f 7374 5f72 6563 656e 745f 7465  f most_recent_te
-00014430: 726d 2e64 696d 656e 7369 6f6e 2025 206f  rm.dimension % o
-00014440: 7468 6572 2e64 696d 656e 7369 6f6e 203d  ther.dimension =
-00014450: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00014460: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00014470: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014480: 4661 6c73 650a 0a20 2020 2064 6566 2063  False..    def c
-00014490: 616e 5f73 696d 706c 6966 7928 7365 6c66  an_simplify(self
-000144a0: 2c20 6f74 6865 722c 206b 696e 642c 2072  , other, kind, r
-000144b0: 6967 6874 293a 0a20 2020 2020 2020 2022  ight):.        "
-000144c0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-000144d0: 6d20 4469 6d20 6f74 6865 723a 0a20 2020  m Dim other:.   
-000144e0: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
-000144f0: 6b69 6e64 3a0a 2020 2020 2020 2020 3a70  kind:.        :p
-00014500: 6172 616d 2062 6f6f 6c20 7269 6768 743a  aram bool right:
-00014510: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00014520: 3a20 7768 6574 6865 7220 7765 2063 616e  : whether we can
-00014530: 2073 696d 706c 6966 7920 7768 656e 2061   simplify when a
-00014540: 7070 6c79 696e 6720 7468 6973 206f 7065  pplying this ope
-00014550: 7261 7469 6f6e 0a20 2020 2020 2020 203a  ration.        :
-00014560: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-00014570: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00014580: 6966 206f 7468 6572 2e64 6572 6976 6564  if other.derived
-00014590: 5f66 726f 6d5f 6f70 2061 6e64 206f 7468  _from_op and oth
-000145a0: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
-000145b0: 6f70 2e6b 696e 6420 3d3d 2022 6d75 6c22  op.kind == "mul"
-000145c0: 3a0a 2020 2020 2020 2020 2020 2020 746d  :.            tm
-000145d0: 7020 3d20 7365 6c66 2e63 6f70 7928 290a  p = self.copy().
-000145e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000145f0: 7465 726d 2069 6e20 6f74 6865 722e 6465  term in other.de
-00014600: 7269 7665 645f 6672 6f6d 5f6f 702e 696e  rived_from_op.in
-00014610: 7075 7473 2069 6620 7269 6768 7420 656c  puts if right el
-00014620: 7365 2072 6576 6572 7365 6428 6f74 6865  se reversed(othe
-00014630: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00014640: 702e 696e 7075 7473 293a 0a20 2020 2020  p.inputs):.     
-00014650: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00014660: 7420 746d 702e 6361 6e5f 7369 6d70 6c69  t tmp.can_simpli
-00014670: 6679 2874 6572 6d2c 206b 696e 643d 6b69  fy(term, kind=ki
-00014680: 6e64 2c20 7269 6768 743d 7269 6768 7429  nd, right=right)
-00014690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000146a0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000146b0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-000146c0: 2020 2074 6d70 2e65 7874 656e 645f 6d75     tmp.extend_mu
-000146d0: 6c5f 6469 765f 2874 6572 6d2c 206b 696e  l_div_(term, kin
-000146e0: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
-000146f0: 6768 7429 0a20 2020 2020 2020 2020 2020  ght).           
-00014700: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00014710: 2020 2020 2069 6478 203d 2073 656c 662e       idx = self.
-00014720: 5f73 696d 706c 6966 795f 7465 726d 5f69  _simplify_term_i
-00014730: 6478 286f 7468 6572 2c20 6b69 6e64 3d6b  dx(other, kind=k
-00014740: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
-00014750: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00014760: 2069 6478 2069 7320 6e6f 7420 4e6f 6e65   idx is not None
-00014770: 0a0a 2020 2020 6465 6620 5f73 696d 706c  ..    def _simpl
-00014780: 6966 795f 7465 726d 5f69 6478 2873 656c  ify_term_idx(sel
-00014790: 662c 206f 7468 6572 2c20 6b69 6e64 2c20  f, other, kind, 
-000147a0: 7269 6768 7429 3a0a 2020 2020 2020 2020  right):.        
-000147b0: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-000147c0: 616d 2044 696d 206f 7468 6572 3a0a 2020  am Dim other:.  
-000147d0: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
-000147e0: 206b 696e 643a 0a20 2020 2020 2020 203a   kind:.        :
-000147f0: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
-00014800: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-00014810: 6e3a 2069 6e64 6578 206f 6620 7465 726d  n: index of term
-00014820: 2074 6f20 7369 6d70 6c69 6679 0a20 2020   to simplify.   
-00014830: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-00014840: 7c4e 6f6e 650a 2020 2020 2020 2020 2222  |None.        ""
-00014850: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-00014860: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
-00014870: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00014880: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-00014890: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
-000148a0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
-000148b0: 7761 6e74 2028 6220 2a20 6129 202f 2f20  want (b * a) // 
-000148c0: 6220 213d 2061 2e0a 2020 2020 2020 2020  b != a..        
-000148d0: 2020 2020 2320 486f 7765 7665 722c 2077      # However, w
-000148e0: 6520 7761 6e74 2068 202a 2028 3220 2a20  e want h * (2 * 
-000148f0: 6120 2f2f 2068 2920 3d3d 2032 202a 2061  a // h) == 2 * a
-00014900: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00014910: 536f 2c20 666f 7220 606d 756c 602c 2061  So, for `mul`, a
-00014920: 6e64 206f 6e6c 7920 666f 7220 606d 756c  nd only for `mul
-00014930: 602c 2063 6865 636b 2061 6c6c 2074 6572  `, check all ter
-00014940: 6d73 2c20 7768 6574 6865 7220 7765 2063  ms, whether we c
-00014950: 616e 2073 696d 706c 6966 7920 736f 6d65  an simplify some
-00014960: 2064 6976 6973 696f 6e2d 7465 726d 2e0a   division-term..
-00014970: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00014980: 692c 2074 6572 6d20 696e 2072 6576 6572  i, term in rever
-00014990: 7365 6428 6c69 7374 2865 6e75 6d65 7261  sed(list(enumera
-000149a0: 7465 2873 656c 662e 7465 726d 7329 2929  te(self.terms)))
-000149b0: 2069 6620 7269 6768 7420 656c 7365 2065   if right else e
-000149c0: 6e75 6d65 7261 7465 2873 656c 662e 7465  numerate(self.te
-000149d0: 726d 7329 3a0a 2020 2020 2020 2020 2020  rms):.          
-000149e0: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-000149f0: 6e73 7461 6e63 6528 7465 726d 2c20 5f64  nstance(term, _d
-00014a00: 2e44 696d 290a 2020 2020 2020 2020 2020  .Dim).          
-00014a10: 2020 2020 2020 6966 2074 6572 6d2e 6465        if term.de
-00014a20: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a40: 2020 2069 6620 7465 726d 2e64 6572 6976     if term.deriv
-00014a50: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
-00014a60: 3d3d 2022 7472 7565 6469 765f 2220 2b20  == "truediv_" + 
-00014a70: 2822 7269 6768 7422 2069 6620 7269 6768  ("right" if righ
-00014a80: 7420 656c 7365 2022 6c65 6674 2229 3a0a  t else "left"):.
-00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014aa0: 2020 2020 2020 2020 6966 2074 6572 6d2e          if term.
-00014ab0: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-00014ac0: 696e 7075 7473 5b2d 315d 203d 3d20 6f74  inputs[-1] == ot
-00014ad0: 6865 723a 0a20 2020 2020 2020 2020 2020  her:.           
-00014ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014af0: 2072 6574 7572 6e20 690a 2020 2020 2020   return i.      
-00014b00: 2020 2020 2020 2020 2020 6966 206f 7468            if oth
-00014b10: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
-00014b20: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
-00014b30: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-00014b40: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00014b50: 2e6b 696e 6420 3d3d 2022 7472 7565 6469  .kind == "truedi
-00014b60: 765f 2220 2b20 2822 7269 6768 7422 2069  v_" + ("right" i
-00014b70: 6620 6e6f 7420 7269 6768 7420 656c 7365  f not right else
-00014b80: 2022 6c65 6674 2229 3a0a 2020 2020 2020   "left"):.      
-00014b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ba0: 2020 6966 206f 7468 6572 2e64 6572 6976    if other.deriv
-00014bb0: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
-00014bc0: 735b 2d31 5d20 3d3d 2074 6572 6d3a 0a20  s[-1] == term:. 
-00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014be0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014bf0: 6e20 690a 2020 2020 2020 2020 2020 2020  n i.            
-00014c00: 2020 2020 6966 2074 6572 6d2e 6973 5f63      if term.is_c
-00014c10: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
-00014c20: 696d 2829 2061 6e64 206f 7468 6572 2e69  im() and other.i
-00014c30: 735f 636f 6e73 7461 6e74 5f73 7461 7469  s_constant_stati
-00014c40: 635f 6469 6d28 293a 0a20 2020 2020 2020  c_dim():.       
-00014c50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00014c60: 7572 6e20 690a 2020 2020 2020 2020 2320  urn i.        # 
-00014c70: 466f 7220 7468 6520 6c61 7374 2f66 6972  For the last/fir
-00014c80: 7374 2074 6572 6d2c 2065 7874 7261 2063  st term, extra c
-00014c90: 6865 636b 732e 0a20 2020 2020 2020 2069  hecks..        i
-00014ca0: 203d 206c 656e 2873 656c 662e 7465 726d   = len(self.term
-00014cb0: 7329 202d 2031 2069 6620 7269 6768 7420  s) - 1 if right 
-00014cc0: 656c 7365 2030 0a20 2020 2020 2020 2074  else 0.        t
-00014cd0: 6572 6d20 3d20 7365 6c66 2e74 6572 6d73  erm = self.terms
-00014ce0: 5b69 5d0a 2020 2020 2020 2020 6966 206b  [i].        if k
-00014cf0: 696e 642e 656e 6473 7769 7468 2822 6469  ind.endswith("di
-00014d00: 7622 2920 616e 6420 6f74 6865 7220 3d3d  v") and other ==
-00014d10: 2074 6572 6d3a 0a20 2020 2020 2020 2020   term:.         
-00014d20: 2020 2072 6574 7572 6e20 690a 2020 2020     return i.    
-00014d30: 2020 2020 6f70 5f6b 696e 6420 3d20 6b69      op_kind = ki
-00014d40: 6e64 202b 2022 5f22 202b 2028 2272 6967  nd + "_" + ("rig
-00014d50: 6874 2220 6966 2072 6967 6874 2065 6c73  ht" if right els
-00014d60: 6520 226c 6566 7422 290a 2020 2020 2020  e "left").      
-00014d70: 2020 6966 2074 6572 6d2e 6465 7269 7665    if term.derive
-00014d80: 645f 6672 6f6d 5f6f 7020 616e 6420 7465  d_from_op and te
-00014d90: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
-00014da0: 6f70 2e6b 696e 6420 3d3d 206f 705f 6b69  op.kind == op_ki
-00014db0: 6e64 3a0a 2020 2020 2020 2020 2020 2020  nd:.            
-00014dc0: 7265 7475 726e 2069 0a20 2020 2020 2020  return i.       
-00014dd0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00014de0: 2020 6465 6620 6578 7465 6e64 5f6d 756c    def extend_mul
-00014df0: 5f64 6976 5f28 7365 6c66 2c20 6f74 6865  _div_(self, othe
-00014e00: 722c 206b 696e 642c 2072 6967 6874 293a  r, kind, right):
-00014e10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014e20: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
-00014e30: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00014e40: 7061 7261 6d20 7374 7220 6b69 6e64 3a0a  param str kind:.
-00014e50: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
-00014e60: 6f6f 6c20 7269 6768 743a 0a20 2020 2020  ool right:.     
-00014e70: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
-00014e80: 7373 6572 7420 6b69 6e64 2069 6e20 7b22  ssert kind in {"
-00014e90: 6d75 6c22 2c20 2266 6c6f 6f72 6469 7622  mul", "floordiv"
-00014ea0: 2c20 2274 7275 6564 6976 222c 2022 6365  , "truediv", "ce
-00014eb0: 696c 6469 7622 7d0a 2020 2020 2020 2020  ildiv"}.        
-00014ec0: 6966 206f 7468 6572 2e69 735f 636f 6e73  if other.is_cons
-00014ed0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-00014ee0: 2920 616e 6420 6f74 6865 722e 6469 6d65  ) and other.dime
-00014ef0: 6e73 696f 6e20 3d3d 2031 3a0a 2020 2020  nsion == 1:.    
-00014f00: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00014f10: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00014f20: 6c66 2e74 6572 6d73 3a0a 2020 2020 2020  lf.terms:.      
-00014f30: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
-00014f40: 2022 6d75 6c22 3a0a 2020 2020 2020 2020   "mul":.        
-00014f50: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00014f60: 6d73 2e61 7070 656e 6428 6f74 6865 7229  ms.append(other)
-00014f70: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00014f80: 6620 6b69 6e64 2e65 6e64 7377 6974 6828  f kind.endswith(
-00014f90: 2264 6976 2229 3a0a 2020 2020 2020 2020  "div"):.        
-00014fa0: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00014fb0: 6d73 203d 205b 5f4f 704d 756c 7454 6572  ms = [_OpMultTer
-00014fc0: 6d2e 6e65 775f 6469 765f 6469 6d28 7365  m.new_div_dim(se
-00014fd0: 6c66 2e61 735f 6469 6d28 292c 206f 7468  lf.as_dim(), oth
-00014fe0: 6572 2c20 6b69 6e64 3d6b 696e 642c 2072  er, kind=kind, r
-00014ff0: 6967 6874 3d72 6967 6874 295d 0a20 2020  ight=right)].   
-00015000: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00015010: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-00015020: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00015030: 2061 6e64 206f 7468 6572 2e64 6572 6976   and other.deriv
-00015040: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
-00015050: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
-00015060: 2020 2020 2020 666f 7220 7465 726d 2069        for term i
-00015070: 6e20 6f74 6865 722e 6465 7269 7665 645f  n other.derived_
-00015080: 6672 6f6d 5f6f 702e 696e 7075 7473 2069  from_op.inputs i
-00015090: 6620 7269 6768 7420 656c 7365 2072 6576  f right else rev
-000150a0: 6572 7365 6428 6f74 6865 722e 6465 7269  ersed(other.deri
-000150b0: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-000150c0: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
-000150d0: 2020 2020 2073 656c 662e 6578 7465 6e64       self.extend
-000150e0: 5f6d 756c 5f64 6976 5f28 7465 726d 2c20  _mul_div_(term, 
-000150f0: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00015100: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
-00015110: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00015120: 2020 2069 6478 203d 2073 656c 662e 5f73     idx = self._s
-00015130: 696d 706c 6966 795f 7465 726d 5f69 6478  implify_term_idx
-00015140: 286f 7468 6572 2c20 6b69 6e64 3d6b 696e  (other, kind=kin
-00015150: 642c 2072 6967 6874 3d72 6967 6874 290a  d, right=right).
-00015160: 2020 2020 2020 2020 6966 2069 6478 2069          if idx i
-00015170: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00015180: 2020 2020 2020 2020 7465 726d 203d 2073          term = s
-00015190: 656c 662e 7465 726d 735b 6964 785d 0a20  elf.terms[idx]. 
-000151a0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-000151b0: 7420 6973 696e 7374 616e 6365 2874 6572  t isinstance(ter
-000151c0: 6d2c 205f 642e 4469 6d29 0a20 2020 2020  m, _d.Dim).     
-000151d0: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-000151e0: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
-000151f0: 6e64 206f 7468 6572 203d 3d20 7465 726d  nd other == term
-00015200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015210: 2020 7365 6c66 2e74 6572 6d73 2e70 6f70    self.terms.pop
-00015220: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
-00015230: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00015240: 2020 2020 2020 2020 2069 6620 6b69 6e64           if kind
-00015250: 203d 3d20 226d 756c 2220 616e 6420 7465   == "mul" and te
-00015260: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
-00015270: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
-00015280: 2020 2020 6966 2074 6572 6d2e 6465 7269      if term.deri
-00015290: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
-000152a0: 203d 3d20 2274 7275 6564 6976 5f22 202b   == "truediv_" +
-000152b0: 2028 2272 6967 6874 2220 6966 2072 6967   ("right" if rig
-000152c0: 6874 2065 6c73 6520 226c 6566 7422 293a  ht else "left"):
-000152d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000152e0: 2020 2020 2069 6620 7465 726d 2e64 6572       if term.der
-000152f0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-00015300: 7574 735b 2d31 5d20 3d3d 206f 7468 6572  uts[-1] == other
-00015310: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015320: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00015330: 6572 6d73 5b69 6478 5d20 3d20 7465 726d  erms[idx] = term
-00015340: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00015350: 2e69 6e70 7574 735b 305d 0a20 2020 2020  .inputs[0].     
-00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015370: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00015380: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
-00015390: 2022 6d75 6c22 2061 6e64 206f 7468 6572   "mul" and other
-000153a0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-000153b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000153c0: 2020 6966 206f 7468 6572 2e64 6572 6976    if other.deriv
-000153d0: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
-000153e0: 3d3d 2022 7472 7565 6469 765f 2220 2b20  == "truediv_" + 
-000153f0: 2822 7269 6768 7422 2069 6620 6e6f 7420  ("right" if not 
-00015400: 7269 6768 7420 656c 7365 2022 6c65 6674  right else "left
-00015410: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00015420: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-00015430: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00015440: 2e69 6e70 7574 735b 2d31 5d20 3d3d 2074  .inputs[-1] == t
-00015450: 6572 6d3a 0a20 2020 2020 2020 2020 2020  erm:.           
-00015460: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015470: 662e 7465 726d 735b 6964 785d 203d 206f  f.terms[idx] = o
-00015480: 7468 6572 2e64 6572 6976 6564 5f66 726f  ther.derived_fro
-00015490: 6d5f 6f70 2e69 6e70 7574 735b 305d 0a20  m_op.inputs[0]. 
-000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154b0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-000154c0: 2020 2020 2020 2020 2020 6966 2074 6572            if ter
-000154d0: 6d2e 6973 5f63 6f6e 7374 616e 745f 7374  m.is_constant_st
-000154e0: 6174 6963 5f64 696d 2829 2061 6e64 206f  atic_dim() and o
-000154f0: 7468 6572 2e69 735f 636f 6e73 7461 6e74  ther.is_constant
-00015500: 5f73 7461 7469 635f 6469 6d28 293a 0a20  _static_dim():. 
-00015510: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015520: 6620 6b69 6e64 203d 3d20 226d 756c 223a  f kind == "mul":
-00015530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015540: 2020 2020 2069 6620 7465 726d 2e64 696d       if term.dim
-00015550: 656e 7369 6f6e 202a 206f 7468 6572 2e64  ension * other.d
-00015560: 696d 656e 7369 6f6e 203d 3d20 313a 0a20  imension == 1:. 
-00015570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015580: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
-00015590: 732e 706f 7028 6964 7829 0a20 2020 2020  s.pop(idx).     
-000155a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155b0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000155c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000155d0: 6c66 2e74 6572 6d73 5b69 6478 5d20 3d20  lf.terms[idx] = 
-000155e0: 5f6d 616b 655f 636f 6e73 7461 6e74 5f73  _make_constant_s
-000155f0: 7461 7469 635f 6469 6d28 7465 726d 2e64  tatic_dim(term.d
-00015600: 696d 656e 7369 6f6e 202a 206f 7468 6572  imension * other
-00015610: 2e64 696d 656e 7369 6f6e 2c20 6b69 6e64  .dimension, kind
-00015620: 3d74 6572 6d2e 6b69 6e64 290a 2020 2020  =term.kind).    
-00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015640: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-00015650: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-00015660: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
-00015670: 6e64 2074 6572 6d2e 6469 6d65 6e73 696f  nd term.dimensio
-00015680: 6e20 2520 6f74 6865 722e 6469 6d65 6e73  n % other.dimens
-00015690: 696f 6e20 3d3d 2030 3a0a 2020 2020 2020  ion == 0:.      
-000156a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000156b0: 6c66 2e74 6572 6d73 5b69 6478 5d20 3d20  lf.terms[idx] = 
-000156c0: 5f6d 616b 655f 636f 6e73 7461 6e74 5f73  _make_constant_s
-000156d0: 7461 7469 635f 6469 6d28 7465 726d 2e64  tatic_dim(term.d
-000156e0: 696d 656e 7369 6f6e 202f 2f20 6f74 6865  imension // othe
-000156f0: 722e 6469 6d65 6e73 696f 6e2c 206b 696e  r.dimension, kin
-00015700: 643d 7465 726d 2e6b 696e 6429 0a20 2020  d=term.kind).   
-00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015720: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00015730: 2020 2020 2020 2020 2320 4661 6c6c 6261          # Fallba
-00015740: 636b 2077 6974 6820 6765 6e65 7269 6320  ck with generic 
-00015750: 6861 6e64 6c69 6e67 2e0a 2020 2020 2020  handling..      
-00015760: 2020 2020 2020 6f70 5f6b 696e 6420 3d20        op_kind = 
-00015770: 6b69 6e64 202b 2022 5f22 202b 2028 2272  kind + "_" + ("r
-00015780: 6967 6874 2220 6966 2072 6967 6874 2065  ight" if right e
-00015790: 6c73 6520 226c 6566 7422 290a 2020 2020  lse "left").    
-000157a0: 2020 2020 2020 2020 6966 206b 696e 642e          if kind.
-000157b0: 656e 6473 7769 7468 2822 6469 7622 2920  endswith("div") 
-000157c0: 616e 6420 7465 726d 2e64 6572 6976 6564  and term.derived
-000157d0: 5f66 726f 6d5f 6f70 2061 6e64 2074 6572  _from_op and ter
-000157e0: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
-000157f0: 702e 6b69 6e64 203d 3d20 6f70 5f6b 696e  p.kind == op_kin
-00015800: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
-00015810: 2020 206e 756d 6572 6174 6f72 203d 2074     numerator = t
-00015820: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
-00015830: 5f6f 702e 696e 7075 7473 5b30 5d0a 2020  _op.inputs[0].  
-00015840: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00015850: 6e6f 6d69 6e61 746f 7220 3d20 7465 726d  nominator = term
-00015860: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00015870: 2e69 6e70 7574 735b 315d 0a20 2020 2020  .inputs[1].     
-00015880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015890: 7465 726d 735b 6964 785d 203d 205f 4f70  terms[idx] = _Op
-000158a0: 4d75 6c74 5465 726d 2e6e 6577 5f64 6976  MultTerm.new_div
-000158b0: 5f64 696d 286e 756d 6572 6174 6f72 2c20  _dim(numerator, 
-000158c0: 6465 6e6f 6d69 6e61 746f 7220 2a20 6f74  denominator * ot
-000158d0: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
-000158e0: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
-000158f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00015900: 7572 6e0a 2020 2020 2020 2020 6966 206b  urn.        if k
-00015910: 696e 642e 656e 6473 7769 7468 2822 6469  ind.endswith("di
-00015920: 7622 293a 0a20 2020 2020 2020 2020 2020  v"):.           
-00015930: 2073 656c 662e 7465 726d 7320 3d20 5b5f   self.terms = [_
-00015940: 4f70 4d75 6c74 5465 726d 2e6e 6577 5f64  OpMultTerm.new_d
-00015950: 6976 5f64 696d 2873 656c 662e 6173 5f64  iv_dim(self.as_d
-00015960: 696d 2829 2c20 6f74 6865 722c 206b 696e  im(), other, kin
-00015970: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
-00015980: 6768 7429 5d0a 2020 2020 2020 2020 2020  ght)].          
-00015990: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-000159a0: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
-000159b0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
-000159c0: 6620 7269 6768 743a 0a20 2020 2020 2020  f right:.       
-000159d0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-000159e0: 726d 732e 6170 7065 6e64 286f 7468 6572  rms.append(other
-000159f0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00015a00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00015a10: 2020 2020 7365 6c66 2e74 6572 6d73 2e69      self.terms.i
-00015a20: 6e73 6572 7428 302c 206f 7468 6572 290a  nsert(0, other).
-00015a30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015a40: 726e 0a20 2020 2020 2020 2061 7373 6572  rn.        asser
-00015a50: 7420 4661 6c73 650a 0a20 2020 2040 636c  t False..    @cl
-00015a60: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00015a70: 6620 6e65 775f 6469 765f 6469 6d28 636c  f new_div_dim(cl
-00015a80: 732c 206e 756d 6572 6174 6f72 2c20 6465  s, numerator, de
-00015a90: 6e6f 6d69 6e61 746f 722c 206b 696e 642c  nominator, kind,
-00015aa0: 2072 6967 6874 293a 0a20 2020 2020 2020   right):.       
-00015ab0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00015ac0: 7261 6d20 4469 6d20 6e75 6d65 7261 746f  ram Dim numerato
-00015ad0: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
-00015ae0: 6d20 4469 6d20 6465 6e6f 6d69 6e61 746f  m Dim denominato
-00015af0: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
-00015b00: 6d20 7374 7220 6b69 6e64 3a20 2266 6c6f  m str kind: "flo
-00015b10: 6f72 6469 7622 206f 7220 2263 6569 6c64  ordiv" or "ceild
-00015b20: 6976 2220 6f72 2022 7472 7565 6469 7622  iv" or "truediv"
-00015b30: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00015b40: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
-00015b50: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00015b60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015b70: 2020 2020 6469 6d5f 7661 6c75 6520 3d20      dim_value = 
-00015b80: 4e6f 6e65 0a20 2020 2020 2020 2061 203d  None.        a =
-00015b90: 206e 756d 6572 6174 6f72 2e64 696d 656e   numerator.dimen
-00015ba0: 7369 6f6e 0a20 2020 2020 2020 2062 203d  sion.        b =
-00015bb0: 2064 656e 6f6d 696e 6174 6f72 2e64 696d   denominator.dim
-00015bc0: 656e 7369 6f6e 0a20 2020 2020 2020 2069  ension.        i
-00015bd0: 6620 6120 6973 206e 6f74 204e 6f6e 6520  f a is not None 
-00015be0: 616e 6420 6220 6973 206e 6f74 204e 6f6e  and b is not Non
-00015bf0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00015c00: 6620 6b69 6e64 203d 3d20 2266 6c6f 6f72  f kind == "floor
-00015c10: 6469 7622 3a0a 2020 2020 2020 2020 2020  div":.          
-00015c20: 2020 2020 2020 6469 6d5f 7661 6c75 6520        dim_value 
-00015c30: 3d20 6120 2f2f 2062 0a20 2020 2020 2020  = a // b.       
-00015c40: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
-00015c50: 3d20 2263 6569 6c64 6976 223a 0a20 2020  = "ceildiv":.   
-00015c60: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-00015c70: 5f76 616c 7565 203d 202d 282d 6120 2f2f  _value = -(-a //
-00015c80: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
-00015c90: 2020 2020 6966 2061 2025 2062 203d 3d20      if a % b == 
-00015ca0: 3020 616e 6420 7269 6768 743a 0a20 2020  0 and right:.   
-00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cc0: 206b 696e 6420 3d20 2266 6c6f 6f72 6469   kind = "floordi
-00015cd0: 7622 2020 2320 666f 7220 6e69 6365 7220  v"  # for nicer 
-00015ce0: 6465 7363 7269 7074 696f 6e2c 2061 6e64  description, and
-00015cf0: 2064 6f65 7320 6e6f 7420 6d61 7474 6572   does not matter
-00015d00: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00015d10: 6620 6b69 6e64 203d 3d20 2274 7275 6564  f kind == "trued
-00015d20: 6976 223a 0a20 2020 2020 2020 2020 2020  iv":.           
-00015d30: 2020 2020 2069 6620 6120 2520 6220 213d       if a % b !=
-00015d40: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00015d50: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00015d60: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-00015d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d80: 2020 2225 7320 7472 7565 6469 7620 2573    "%s truediv %s
-00015d90: 206f 6e6c 7920 616c 6c6f 7765 6420 6966   only allowed if
-00015da0: 2074 6865 2072 6573 756c 7420 6973 2061   the result is a
-00015db0: 6e20 696e 7465 6765 7222 2025 2028 6e75  n integer" % (nu
-00015dc0: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
-00015dd0: 6174 6f72 290a 2020 2020 2020 2020 2020  ator).          
-00015de0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00015df0: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
-00015e00: 7661 6c75 6520 3d20 6120 2f2f 2062 0a20  value = a // b. 
-00015e10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015e20: 6620 7269 6768 743a 0a20 2020 2020 2020  f right:.       
-00015e30: 2020 2020 2020 2020 2020 2020 206b 696e               kin
-00015e40: 6420 3d20 2266 6c6f 6f72 6469 7622 2020  d = "floordiv"  
-00015e50: 2320 666f 7220 6e69 6365 7220 6465 7363  # for nicer desc
-00015e60: 7269 7074 696f 6e2c 2061 6e64 2064 6f65  ription, and doe
-00015e70: 7320 6e6f 7420 6d61 7474 6572 0a20 2020  s not matter.   
-00015e80: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00015e90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00015ea0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00015eb0: 2269 6e76 616c 6964 206b 696e 6420 2572  "invalid kind %r
-00015ec0: 2220 2520 286b 696e 642c 2929 0a20 2020  " % (kind,)).   
-00015ed0: 2020 2020 2069 6620 6b69 6e64 203d 3d20       if kind == 
-00015ee0: 2266 6c6f 6f72 6469 7622 2061 6e64 2072  "floordiv" and r
-00015ef0: 6967 6874 3a0a 2020 2020 2020 2020 2020  ight:.          
-00015f00: 2020 6465 7363 7269 7074 696f 6e20 3d20    description = 
-00015f10: 2225 732f 2f25 7322 2025 2028 5f67 6574  "%s//%s" % (_get
-00015f20: 5f64 6573 6372 6970 7469 6f6e 286e 756d  _description(num
-00015f30: 6572 6174 6f72 292c 205f 6765 745f 6465  erator), _get_de
-00015f40: 7363 7269 7074 696f 6e28 6465 6e6f 6d69  scription(denomi
-00015f50: 6e61 746f 7229 290a 2020 2020 2020 2020  nator)).        
-00015f60: 656c 6966 206b 696e 6420 3d3d 2022 6365  elif kind == "ce
-00015f70: 696c 6469 7622 2061 6e64 2072 6967 6874  ildiv" and right
-00015f80: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-00015f90: 7363 7269 7074 696f 6e20 3d20 22e2 8c88  scription = "...
-00015fa0: 2573 2f25 73e2 8c89 2220 2520 285f 6765  %s/%s..." % (_ge
-00015fb0: 745f 6465 7363 7269 7074 696f 6e28 6e75  t_description(nu
-00015fc0: 6d65 7261 746f 7229 2c20 5f67 6574 5f64  merator), _get_d
-00015fd0: 6573 6372 6970 7469 6f6e 2864 656e 6f6d  escription(denom
-00015fe0: 696e 6174 6f72 2929 0a20 2020 2020 2020  inator)).       
-00015ff0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00016000: 2020 2064 6573 6372 6970 7469 6f6e 203d     description =
-00016010: 2022 2573 5f25 7328 2573 2c20 2573 2922   "%s_%s(%s, %s)"
-00016020: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
-00016030: 2020 2020 206b 696e 642c 0a20 2020 2020       kind,.     
-00016040: 2020 2020 2020 2020 2020 2022 7269 6768             "righ
-00016050: 7422 2069 6620 7269 6768 7420 656c 7365  t" if right else
-00016060: 2022 6c65 6674 222c 0a20 2020 2020 2020   "left",.       
-00016070: 2020 2020 2020 2020 205f 6765 745f 6465           _get_de
-00016080: 7363 7269 7074 696f 6e28 6e75 6d65 7261  scription(numera
-00016090: 746f 722c 2062 7261 636b 6574 733d 4661  tor, brackets=Fa
-000160a0: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
-000160b0: 2020 2020 2020 5f67 6574 5f64 6573 6372        _get_descr
-000160c0: 6970 7469 6f6e 2864 656e 6f6d 696e 6174  iption(denominat
-000160d0: 6f72 2c20 6272 6163 6b65 7473 3d46 616c  or, brackets=Fal
-000160e0: 7365 292c 0a20 2020 2020 2020 2020 2020  se),.           
-000160f0: 2029 0a20 2020 2020 2020 206f 705f 6b69   ).        op_ki
-00016100: 6e64 203d 206b 696e 640a 2020 2020 2020  nd = kind.      
-00016110: 2020 6966 2061 2069 7320 6e6f 7420 4e6f    if a is not No
-00016120: 6e65 2061 6e64 2062 2069 7320 6e6f 7420  ne and b is not 
-00016130: 4e6f 6e65 2061 6e64 2061 2025 2062 203d  None and a % b =
-00016140: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00016150: 206f 705f 6b69 6e64 203d 2022 7472 7565   op_kind = "true
-00016160: 6469 7622 2020 2320 6d61 6b65 7320 736f  div"  # makes so
-00016170: 6d65 206f 7468 6572 2063 6865 636b 7320  me other checks 
-00016180: 7369 6d70 6c65 720a 2020 2020 2020 2020  simpler.        
-00016190: 6f70 5f6b 696e 6420 2b3d 2022 5f22 202b  op_kind += "_" +
-000161a0: 2028 2272 6967 6874 2220 6966 2072 6967   ("right" if rig
-000161b0: 6874 2065 6c73 6520 226c 6566 7422 290a  ht else "left").
-000161c0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000161d0: 642e 4469 6d28 0a20 2020 2020 2020 2020  d.Dim(.         
-000161e0: 2020 2064 6573 6372 6970 7469 6f6e 3d64     description=d
-000161f0: 6573 6372 6970 7469 6f6e 2c0a 2020 2020  escription,.    
-00016200: 2020 2020 2020 2020 6b69 6e64 3d6e 756d          kind=num
-00016210: 6572 6174 6f72 2e6b 696e 642c 0a20 2020  erator.kind,.   
-00016220: 2020 2020 2020 2020 2064 696d 656e 7369           dimensi
-00016230: 6f6e 3d64 696d 5f76 616c 7565 2c0a 2020  on=dim_value,.  
-00016240: 2020 2020 2020 2020 2020 6465 7269 7665            derive
-00016250: 645f 6672 6f6d 5f6f 703d 4f70 286b 696e  d_from_op=Op(kin
-00016260: 643d 6f70 5f6b 696e 642c 2069 6e70 7574  d=op_kind, input
-00016270: 733d 5b6e 756d 6572 6174 6f72 2c20 6465  s=[numerator, de
-00016280: 6e6f 6d69 6e61 746f 725d 292c 0a20 2020  nominator]),.   
-00016290: 2020 2020 2020 2020 2064 6572 6976 6564           derived
-000162a0: 5f66 726f 6d5f 7461 673d 6e75 6d65 7261  _from_tag=numera
-000162b0: 746f 722c 0a20 2020 2020 2020 2029 0a0a  tor,.        )..
-000162c0: 2020 2020 6465 6620 6173 5f64 696d 2873      def as_dim(s
-000162d0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000162e0: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
-000162f0: 3a20 4469 6d0a 2020 2020 2020 2020 2222  : Dim.        ""
-00016300: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00016310: 662e 6973 5f6f 6e65 2829 3a0a 2020 2020  f.is_one():.    
-00016320: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00016330: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
-00016340: 6174 6963 5f64 696d 2831 290a 2020 2020  atic_dim(1).    
-00016350: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
-00016360: 7465 726d 7329 203d 3d20 313a 0a20 2020  terms) == 1:.   
-00016370: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00016380: 7365 6c66 2e74 6572 6d73 5b30 5d0a 2020  self.terms[0].  
-00016390: 2020 2020 2020 6469 6d5f 6b69 6e64 203d        dim_kind =
-000163a0: 205f 6765 745f 6d65 7267 6564 5f64 696d   _get_merged_dim
-000163b0: 5f6b 696e 6428 7365 6c66 2e74 6572 6d73  _kind(self.terms
-000163c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000163d0: 205f 642e 4469 6d28 0a20 2020 2020 2020   _d.Dim(.       
-000163e0: 2020 2020 206b 696e 643d 6469 6d5f 6b69       kind=dim_ki
-000163f0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-00016400: 6465 7363 7269 7074 696f 6e3d 222a 222e  description="*".
-00016410: 6a6f 696e 286d 6170 285f 6765 745f 6465  join(map(_get_de
-00016420: 7363 7269 7074 696f 6e2c 2073 656c 662e  scription, self.
-00016430: 7465 726d 7329 292c 0a20 2020 2020 2020  terms)),.       
-00016440: 2020 2020 2064 696d 656e 7369 6f6e 3d73       dimension=s
-00016450: 656c 662e 6469 6d65 6e73 696f 6e2c 0a20  elf.dimension,. 
-00016460: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
-00016470: 6564 5f66 726f 6d5f 6f70 3d4f 7028 6b69  ed_from_op=Op(ki
-00016480: 6e64 3d22 6d75 6c22 2c20 696e 7075 7473  nd="mul", inputs
-00016490: 3d6c 6973 7428 7365 6c66 2e74 6572 6d73  =list(self.terms
-000164a0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-000164b0: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
-000164c0: 3d73 656c 662e 7265 7072 6573 656e 7461  =self.representa
-000164d0: 7469 7665 5f74 6167 2829 2c0a 2020 2020  tive_tag(),.    
-000164e0: 2020 2020 290a 0a20 2020 2064 6566 2072      )..    def r
-000164f0: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
-00016500: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
-00016510: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
-00016520: 7970 653a 2044 696d 7c4e 6f6e 650a 2020  ype: Dim|None.  
-00016530: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00016540: 2020 2320 416c 736f 2073 6565 2044 696d    # Also see Dim
-00016550: 2e5f 4f70 4c69 6e65 6172 5465 726d 2e72  ._OpLinearTerm.r
-00016560: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
-00016570: 6728 292e 0a20 2020 2020 2020 2023 2046  g()..        # F
-00016580: 6972 7374 2066 696e 6420 616e 7920 6479  irst find any dy
-00016590: 6e61 6d69 632e 0a20 2020 2020 2020 2066  namic..        f
-000165a0: 6f72 2074 6572 6d5f 2069 6e20 7365 6c66  or term_ in self
-000165b0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-000165c0: 2020 2020 6966 2074 6572 6d5f 2e69 735f      if term_.is_
-000165d0: 6479 6e61 6d69 6328 293a 0a20 2020 2020  dynamic():.     
-000165e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000165f0: 6e20 7465 726d 5f0a 2020 2020 2020 2020  n term_.        
-00016600: 2320 4e6f 7720 6669 6e64 206e 6f6e 2d75  # Now find non-u
-00016610: 6e73 7065 6369 6669 6564 2e0a 2020 2020  nspecified..    
-00016620: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
-00016630: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
-00016640: 2020 2020 2020 2020 2069 6620 7465 726d           if term
-00016650: 5f2e 6b69 6e64 2021 3d20 4469 6d54 7970  _.kind != DimTyp
-00016660: 6573 2e55 6e73 7065 6369 6669 6564 3a0a  es.Unspecified:.
-00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016680: 7265 7475 726e 2074 6572 6d5f 0a20 2020  return term_.   
-00016690: 2020 2020 2023 204e 6f77 2066 696e 6420       # Now find 
-000166a0: 616e 792e 0a20 2020 2020 2020 2066 6f72  any..        for
-000166b0: 2074 6572 6d5f 2069 6e20 7365 6c66 2e74   term_ in self.t
-000166c0: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
-000166d0: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
-000166e0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-000166f0: 6e65 0a0a 0a63 6c61 7373 205f 4f70 4c69  ne...class _OpLi
-00016700: 6e65 6172 5465 726d 3a0a 2020 2020 2222  nearTerm:.    ""
-00016710: 220a 2020 2020 7265 7072 6573 656e 7473  ".    represents
-00016720: 2073 7468 206c 696b 6520 6120 2a20 6220   sth like a * b 
-00016730: 2b20 630a 2020 2020 2222 220a 0a20 2020  + c.    """..   
-00016740: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00016750: 2020 6465 6620 6672 6f6d 5f64 696d 2863    def from_dim(c
-00016760: 6c73 2c20 6469 6d29 3a0a 2020 2020 2020  ls, dim):.      
-00016770: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00016780: 6172 616d 2044 696d 2064 696d 3a0a 2020  aram Dim dim:.  
-00016790: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
-000167a0: 6d2e 5f4f 704c 696e 6561 7254 6572 6d0a  m._OpLinearTerm.
-000167b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000167c0: 2020 2020 7265 7320 3d20 636c 732e 7a65      res = cls.ze
-000167d0: 726f 2829 0a20 2020 2020 2020 2072 6573  ro().        res
-000167e0: 2e65 7874 656e 645f 6164 645f 7375 625f  .extend_add_sub_
-000167f0: 2864 696d 2c20 6b69 6e64 3d22 6164 6422  (dim, kind="add"
-00016800: 2c20 7269 6768 743d 5472 7565 290a 2020  , right=True).  
-00016810: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00016820: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00016830: 6f64 0a20 2020 2064 6566 207a 6572 6f28  od.    def zero(
-00016840: 636c 7329 3a0a 2020 2020 2020 2020 2222  cls):.        ""
-00016850: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
-00016860: 3a20 4469 6d2e 5f4f 704c 696e 6561 7254  : Dim._OpLinearT
-00016870: 6572 6d0a 2020 2020 2020 2020 2222 220a  erm.        """.
-00016880: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00016890: 4f70 4c69 6e65 6172 5465 726d 285b 5d29  OpLinearTerm([])
-000168a0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000168b0: 5f5f 2873 656c 662c 2074 6572 6d73 293a  __(self, terms):
-000168c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000168d0: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
-000168e0: 5b44 696d 2e5f 4f70 4d75 6c74 5465 726d  [Dim._OpMultTerm
-000168f0: 5d20 7465 726d 733a 0a20 2020 2020 2020  ] terms:.       
-00016900: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-00016910: 662e 7465 726d 7320 3d20 7465 726d 730a  f.terms = terms.
-00016920: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
-00016930: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00016940: 2072 6574 7572 6e20 6861 7368 2874 7570   return hash(tup
-00016950: 6c65 2873 656c 662e 7465 726d 7329 290a  le(self.terms)).
-00016960: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
-00016970: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
-00016980: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00016990: 6e63 6528 6f74 6865 722c 205f 4f70 4c69  nce(other, _OpLi
-000169a0: 6e65 6172 5465 726d 293a 0a20 2020 2020  nearTerm):.     
-000169b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000169c0: 6c66 2e74 6572 6d73 203d 3d20 6f74 6865  lf.terms == othe
-000169d0: 722e 7465 726d 730a 2020 2020 2020 2020  r.terms.        
-000169e0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-000169f0: 2020 6465 6620 5f5f 6e65 5f5f 2873 656c    def __ne__(sel
-00016a00: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
-00016a10: 2020 2072 6574 7572 6e20 6e6f 7420 7365     return not se
-00016a20: 6c66 2e5f 5f65 715f 5f28 6f74 6865 7229  lf.__eq__(other)
-00016a30: 0a0a 2020 2020 6465 6620 6173 5f64 696d  ..    def as_dim
-00016a40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00016a50: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
-00016a60: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
-00016a70: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00016a80: 656c 662e 6973 5f7a 6572 6f28 293a 0a20  elf.is_zero():. 
-00016a90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00016aa0: 6e20 5f6d 616b 655f 636f 6e73 7461 6e74  n _make_constant
-00016ab0: 5f73 7461 7469 635f 6469 6d28 3029 0a20  _static_dim(0). 
-00016ac0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-00016ad0: 6c66 2e74 6572 6d73 2920 3d3d 2031 3a0a  lf.terms) == 1:.
-00016ae0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00016af0: 726e 2073 656c 662e 7465 726d 735b 305d  rn self.terms[0]
-00016b00: 2e61 735f 6469 6d28 290a 2020 2020 2020  .as_dim().      
-00016b10: 2020 6164 645f 7061 7274 7320 3d20 5b5d    add_parts = []
-00016b20: 0a20 2020 2020 2020 2064 6573 635f 7061  .        desc_pa
-00016b30: 7274 7320 3d20 5b5d 0a20 2020 2020 2020  rts = [].       
-00016b40: 2064 696d 203d 2030 0a20 2020 2020 2020   dim = 0.       
-00016b50: 2066 6f72 2074 6572 6d20 696e 2073 656c   for term in sel
-00016b60: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
-00016b70: 2020 2020 2073 203d 2074 6572 6d2e 6173       s = term.as
-00016b80: 5f64 696d 2829 0a20 2020 2020 2020 2020  _dim().         
-00016b90: 2020 2061 6464 5f70 6172 7473 2e61 7070     add_parts.app
-00016ba0: 656e 6428 7329 0a20 2020 2020 2020 2020  end(s).         
-00016bb0: 2020 2064 6573 635f 7061 7274 732e 6170     desc_parts.ap
-00016bc0: 7065 6e64 285f 6765 745f 6465 7363 7269  pend(_get_descri
-00016bd0: 7074 696f 6e28 7329 290a 2020 2020 2020  ption(s)).      
-00016be0: 2020 2020 2020 6966 2064 696d 2069 7320        if dim is 
-00016bf0: 6e6f 7420 4e6f 6e65 2061 6e64 2073 2e64  not None and s.d
-00016c00: 696d 656e 7369 6f6e 2069 7320 6e6f 7420  imension is not 
-00016c10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00016c20: 2020 2020 2020 6469 6d20 2b3d 2073 2e64        dim += s.d
-00016c30: 696d 656e 7369 6f6e 0a20 2020 2020 2020  imension.       
-00016c40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00016c50: 2020 2020 2020 2020 2020 2064 696d 203d             dim =
-00016c60: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-00016c70: 206c 656e 2861 6464 5f70 6172 7473 2920   len(add_parts) 
-00016c80: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00016c90: 2020 7265 7475 726e 2061 6464 5f70 6172    return add_par
-00016ca0: 7473 5b30 5d0a 2020 2020 2020 2020 7265  ts[0].        re
-00016cb0: 7475 726e 205f 642e 4469 6d28 0a20 2020  turn _d.Dim(.   
-00016cc0: 2020 2020 2020 2020 206b 696e 643d 5f67           kind=_g
-00016cd0: 6574 5f6d 6572 6765 645f 6469 6d5f 6b69  et_merged_dim_ki
-00016ce0: 6e64 2861 6464 5f70 6172 7473 292c 0a20  nd(add_parts),. 
-00016cf0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00016d00: 6970 7469 6f6e 3d22 2b22 2e6a 6f69 6e28  iption="+".join(
-00016d10: 6465 7363 5f70 6172 7473 292c 0a20 2020  desc_parts),.   
-00016d20: 2020 2020 2020 2020 2064 696d 656e 7369           dimensi
-00016d30: 6f6e 3d64 696d 2c0a 2020 2020 2020 2020  on=dim,.        
-00016d40: 2020 2020 6465 7269 7665 645f 6672 6f6d      derived_from
-00016d50: 5f6f 703d 4f70 286b 696e 643d 2261 6464  _op=Op(kind="add
-00016d60: 222c 2069 6e70 7574 733d 6164 645f 7061  ", inputs=add_pa
-00016d70: 7274 7329 2c0a 2020 2020 2020 2020 2020  rts),.          
-00016d80: 2020 6465 7269 7665 645f 6672 6f6d 5f74    derived_from_t
-00016d90: 6167 3d73 656c 662e 7265 7072 6573 656e  ag=self.represen
-00016da0: 7461 7469 7665 5f74 6167 2829 2c0a 2020  tative_tag(),.  
-00016db0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00016dc0: 205f 5f72 6570 725f 5f28 7365 6c66 293a   __repr__(self):
-00016dd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00016de0: 2244 696d 2e5f 4f70 4c69 6e65 6172 5465  "Dim._OpLinearTe
-00016df0: 726d 2825 7229 2220 2520 2873 656c 662e  rm(%r)" % (self.
-00016e00: 7465 726d 732c 290a 0a20 2020 2064 6566  terms,)..    def
-00016e10: 2069 735f 7a65 726f 2873 656c 6629 3a0a   is_zero(self):.
-00016e20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00016e30: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-00016e40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016e50: 2020 2020 2072 6574 7572 6e20 6e6f 7420       return not 
-00016e60: 7365 6c66 2e74 6572 6d73 0a0a 2020 2020  self.terms..    
-00016e70: 6465 6620 6578 7465 6e64 5f61 6464 5f73  def extend_add_s
-00016e80: 7562 5f28 7365 6c66 2c20 6f74 6865 722c  ub_(self, other,
-00016e90: 206b 696e 642c 2072 6967 6874 293a 0a20   kind, right):. 
-00016ea0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016eb0: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
-00016ec0: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
-00016ed0: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
-00016ee0: 3a20 2261 6464 2220 6f72 2022 7375 6222  : "add" or "sub"
-00016ef0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00016f00: 626f 6f6c 2072 6967 6874 3a20 6f72 206c  bool right: or l
-00016f10: 6566 742e 2072 6967 6874 206d 6561 6e73  eft. right means
-00016f20: 2073 656c 6620 2b20 6f74 6865 722c 206c   self + other, l
-00016f30: 6566 7420 6d65 616e 7320 6f74 6865 7220  eft means other 
-00016f40: 2b20 7365 6c66 0a20 2020 2020 2020 2022  + self.        "
-00016f50: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
-00016f60: 7420 6b69 6e64 2069 6e20 7b22 6164 6422  t kind in {"add"
-00016f70: 2c20 2273 7562 227d 0a20 2020 2020 2020  , "sub"}.       
-00016f80: 206f 7468 6572 203d 2073 656c 662e 5f6d   other = self._m
-00016f90: 616b 655f 6469 6d28 6f74 6865 722c 206b  ake_dim(other, k
-00016fa0: 696e 643d 6b69 6e64 290a 2020 2020 2020  ind=kind).      
-00016fb0: 2020 6966 206f 7468 6572 2e69 735f 636f    if other.is_co
-00016fc0: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
-00016fd0: 6d28 2920 616e 6420 6f74 6865 722e 6469  m() and other.di
-00016fe0: 6d65 6e73 696f 6e20 3d3d 2030 3a0a 2020  mension == 0:.  
-00016ff0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017000: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-00017010: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00017020: 7020 616e 6420 6f74 6865 722e 6465 7269  p and other.deri
-00017030: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
-00017040: 203d 3d20 2261 6464 223a 0a20 2020 2020   == "add":.     
-00017050: 2020 2020 2020 2066 6f72 206f 7468 6572         for other
-00017060: 5f20 696e 206f 7468 6572 2e64 6572 6976  _ in other.deriv
-00017070: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
-00017080: 7320 6966 2072 6967 6874 2065 6c73 6520  s if right else 
-00017090: 7265 7665 7273 6564 286f 7468 6572 2e64  reversed(other.d
-000170a0: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
-000170b0: 6e70 7574 7329 3a0a 2020 2020 2020 2020  nputs):.        
-000170c0: 2020 2020 2020 2020 7365 6c66 2e65 7874          self.ext
-000170d0: 656e 645f 6164 645f 7375 625f 286f 7468  end_add_sub_(oth
-000170e0: 6572 5f2c 206b 696e 643d 6b69 6e64 2c20  er_, kind=kind, 
-000170f0: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
-00017100: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00017110: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
-00017120: 4f70 4d75 6c74 5465 726d 2e66 726f 6d5f  OpMultTerm.from_
-00017130: 6469 6d28 6f74 6865 7229 0a20 2020 2020  dim(other).     
-00017140: 2020 206e 6567 5f74 6572 6d20 3d20 7465     neg_term = te
-00017150: 726d 2e6e 6567 6174 6976 6528 290a 2020  rm.negative().  
-00017160: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
-00017170: 2022 7375 6222 3a0a 2020 2020 2020 2020   "sub":.        
-00017180: 2020 2020 7465 726d 2c20 6e65 675f 7465      term, neg_te
-00017190: 726d 203d 206e 6567 5f74 6572 6d2c 2074  rm = neg_term, t
-000171a0: 6572 6d0a 2020 2020 2020 2020 6d6f 7374  erm.        most
-000171b0: 5f72 6563 656e 745f 7465 726d 203d 2073  _recent_term = s
-000171c0: 656c 662e 7465 726d 735b 2d31 2069 6620  elf.terms[-1 if 
-000171d0: 7269 6768 7420 656c 7365 2030 5d20 6966  right else 0] if
-000171e0: 2073 656c 662e 7465 726d 7320 656c 7365   self.terms else
-000171f0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-00017200: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
-00017210: 6d3a 0a20 2020 2020 2020 2020 2020 2069  m:.            i
-00017220: 6620 6d6f 7374 5f72 6563 656e 745f 7465  f most_recent_te
-00017230: 726d 203d 3d20 6e65 675f 7465 726d 3a0a  rm == neg_term:.
-00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017250: 7365 6c66 2e74 6572 6d73 2e70 6f70 282d  self.terms.pop(-
-00017260: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
-00017270: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-00017280: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00017290: 2020 2020 2020 6966 206d 6f73 745f 7265        if most_re
-000172a0: 6365 6e74 5f74 6572 6d2e 6973 5f63 6f6e  cent_term.is_con
-000172b0: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-000172c0: 2829 2061 6e64 2074 6572 6d2e 6973 5f63  () and term.is_c
-000172d0: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
-000172e0: 696d 2829 3a0a 2020 2020 2020 2020 2020  im():.          
-000172f0: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00017300: 5b2d 3120 6966 2072 6967 6874 2065 6c73  [-1 if right els
-00017310: 6520 305d 203d 205f 4f70 4d75 6c74 5465  e 0] = _OpMultTe
-00017320: 726d 2e66 726f 6d5f 6469 6d28 0a20 2020  rm.from_dim(.   
-00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017340: 205f 6d61 6b65 5f63 6f6e 7374 616e 745f   _make_constant_
-00017350: 7374 6174 6963 5f64 696d 286d 6f73 745f  static_dim(most_
-00017360: 7265 6365 6e74 5f74 6572 6d2e 6469 6d65  recent_term.dime
-00017370: 6e73 696f 6e20 2b20 7465 726d 2e64 696d  nsion + term.dim
-00017380: 656e 7369 6f6e 2c20 6b69 6e64 3d6f 7468  ension, kind=oth
-00017390: 6572 2e6b 696e 6429 0a20 2020 2020 2020  er.kind).       
-000173a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000173b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000173c0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-000173d0: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
-000173e0: 6d2e 7465 726d 7320 616e 6420 7465 726d  m.terms and term
-000173f0: 2e74 6572 6d73 2061 6e64 206d 6f73 745f  .terms and most_
-00017400: 7265 6365 6e74 5f74 6572 6d2e 7465 726d  recent_term.term
-00017410: 735b 2d31 5d20 3d3d 2074 6572 6d2e 7465  s[-1] == term.te
-00017420: 726d 735b 2d31 5d3a 0a20 2020 2020 2020  rms[-1]:.       
-00017430: 2020 2020 2020 2020 2023 204d 6572 6765           # Merge
-00017440: 2074 6572 6d73 0a20 2020 2020 2020 2020   terms.         
-00017450: 2020 2020 2020 2061 203d 205f 4f70 4d75         a = _OpMu
-00017460: 6c74 5465 726d 2e66 726f 6d5f 6469 6d5f  ltTerm.from_dim_
-00017470: 6661 6374 6f72 7328 6d6f 7374 5f72 6563  factors(most_rec
-00017480: 656e 745f 7465 726d 2e74 6572 6d73 5b3a  ent_term.terms[:
-00017490: 2d31 5d29 2e61 735f 6469 6d28 290a 2020  -1]).as_dim().  
-000174a0: 2020 2020 2020 2020 2020 2020 2020 6220                b 
-000174b0: 3d20 5f4f 704d 756c 7454 6572 6d2e 6672  = _OpMultTerm.fr
-000174c0: 6f6d 5f64 696d 5f66 6163 746f 7273 2874  om_dim_factors(t
-000174d0: 6572 6d2e 7465 726d 735b 3a2d 315d 292e  erm.terms[:-1]).
-000174e0: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
-000174f0: 2020 2020 2020 2020 2072 6573 203d 205f           res = _
-00017500: 4f70 4d75 6c74 5465 726d 2e66 726f 6d5f  OpMultTerm.from_
-00017510: 6469 6d28 2861 202b 2062 2920 6966 2072  dim((a + b) if r
-00017520: 6967 6874 2065 6c73 6520 2862 202b 2061  ight else (b + a
-00017530: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00017540: 2020 2072 6573 2e65 7874 656e 645f 6d75     res.extend_mu
-00017550: 6c5f 6469 765f 2874 6572 6d2e 7465 726d  l_div_(term.term
-00017560: 735b 2d31 5d2c 206b 696e 643d 226d 756c  s[-1], kind="mul
-00017570: 222c 2072 6967 6874 3d54 7275 6529 0a20  ", right=True). 
-00017580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017590: 656c 662e 7465 726d 735b 2d31 2069 6620  elf.terms[-1 if 
-000175a0: 7269 6768 7420 656c 7365 2030 5d20 3d20  right else 0] = 
-000175b0: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
-000175c0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000175d0: 2020 2069 6620 7269 6768 743a 0a20 2020     if right:.   
-000175e0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-000175f0: 726d 732e 6170 7065 6e64 2874 6572 6d29  rms.append(term)
-00017600: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00017610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017620: 7465 726d 732e 696e 7365 7274 2830 2c20  terms.insert(0, 
-00017630: 7465 726d 290a 0a20 2020 2064 6566 2065  term)..    def e
-00017640: 7874 656e 645f 6d75 6c5f 6469 765f 2873  xtend_mul_div_(s
-00017650: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
-00017660: 2c20 7269 6768 7429 3a0a 2020 2020 2020  , right):.      
-00017670: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00017680: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
-00017690: 6572 3a0a 2020 2020 2020 2020 3a70 6172  er:.        :par
-000176a0: 616d 2073 7472 206b 696e 643a 2022 6d75  am str kind: "mu
-000176b0: 6c22 206f 7220 2263 6569 6c64 6976 220a  l" or "ceildiv".
-000176c0: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
-000176d0: 6f6f 6c20 7269 6768 743a 206f 7220 6c65  ool right: or le
-000176e0: 6674 2e20 7269 6768 7420 6d65 616e 7320  ft. right means 
-000176f0: 7365 6c66 202a 206f 7468 6572 2c20 6c65  self * other, le
-00017700: 6674 206d 6561 6e73 206f 7468 6572 202a  ft means other *
-00017710: 2073 656c 660a 2020 2020 2020 2020 2222   self.        ""
-00017720: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00017730: 206b 696e 6420 696e 207b 226d 756c 222c   kind in {"mul",
-00017740: 2022 666c 6f6f 7264 6976 222c 2022 7472   "floordiv", "tr
-00017750: 7565 6469 7622 2c20 2263 6569 6c64 6976  uediv", "ceildiv
-00017760: 227d 0a20 2020 2020 2020 206f 7468 6572  "}.        other
-00017770: 203d 2073 656c 662e 5f6d 616b 655f 6469   = self._make_di
-00017780: 6d28 6f74 6865 722c 206b 696e 643d 6b69  m(other, kind=ki
-00017790: 6e64 290a 2020 2020 2020 2020 6966 206b  nd).        if k
-000177a0: 696e 6420 3d3d 2022 6d75 6c22 2061 6e64  ind == "mul" and
-000177b0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-000177c0: 2020 2020 6966 206e 6f74 2061 6c6c 2874      if not all(t
-000177d0: 6572 6d2e 6361 6e5f 7369 6d70 6c69 6679  erm.can_simplify
-000177e0: 286f 7468 6572 2c20 6b69 6e64 3d6b 696e  (other, kind=kin
-000177f0: 642c 2072 6967 6874 3d72 6967 6874 2920  d, right=right) 
-00017800: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
-00017810: 2e74 6572 6d73 293a 0a20 2020 2020 2020  .terms):.       
-00017820: 2020 2020 2020 2020 2023 2044 6f20 6974           # Do it
-00017830: 2074 6865 206f 7468 6572 2077 6179 2061   the other way a
-00017840: 726f 756e 640a 2020 2020 2020 2020 2020  round.          
-00017850: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00017860: 2c20 6f74 6865 7220 3d20 5f4f 704c 696e  , other = _OpLin
-00017870: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
-00017880: 286f 7468 6572 292e 7465 726d 732c 2073  (other).terms, s
-00017890: 656c 662e 6173 5f64 696d 2829 0a20 2020  elf.as_dim().   
-000178a0: 2020 2020 2020 2020 2020 2020 2072 6967               rig
-000178b0: 6874 203d 2046 616c 7365 0a20 2020 2020  ht = False.     
-000178c0: 2020 2069 6620 6f74 6865 722e 6973 5f63     if other.is_c
-000178d0: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
-000178e0: 696d 2829 2061 6e64 206f 7468 6572 2e64  im() and other.d
-000178f0: 696d 656e 7369 6f6e 203d 3d20 313a 0a20  imension == 1:. 
-00017900: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00017910: 6e0a 2020 2020 2020 2020 6966 206b 696e  n.        if kin
-00017920: 642e 656e 6473 7769 7468 2822 6469 7622  d.endswith("div"
-00017930: 2920 616e 6420 6c65 6e28 7365 6c66 2e74  ) and len(self.t
-00017940: 6572 6d73 2920 3e3d 2032 3a0a 2020 2020  erms) >= 2:.    
-00017950: 2020 2020 2020 2020 6966 2061 6e79 286e          if any(n
-00017960: 6f74 2074 6572 6d2e 6469 7669 7369 626c  ot term.divisibl
-00017970: 6528 6f74 6865 722c 2072 6967 6874 3d72  e(other, right=r
-00017980: 6967 6874 2920 666f 7220 7465 726d 2069  ight) for term i
-00017990: 6e20 7365 6c66 2e74 6572 6d73 293a 0a20  n self.terms):. 
-000179a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000179b0: 656c 662e 7465 726d 7320 3d20 5b0a 2020  elf.terms = [.  
-000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179d0: 2020 5f4f 704d 756c 7454 6572 6d2e 6672    _OpMultTerm.fr
-000179e0: 6f6d 5f64 696d 285f 4f70 4d75 6c74 5465  om_dim(_OpMultTe
-000179f0: 726d 2e6e 6577 5f64 6976 5f64 696d 2873  rm.new_div_dim(s
-00017a00: 656c 662e 6173 5f64 696d 2829 2c20 6f74  elf.as_dim(), ot
-00017a10: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
-00017a20: 7269 6768 743d 7269 6768 7429 290a 2020  right=right)).  
-00017a30: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00017a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a50: 7265 7475 726e 0a20 2020 2020 2020 2066  return.        f
-00017a60: 6f72 2074 6572 6d20 696e 2073 656c 662e  or term in self.
-00017a70: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
-00017a80: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
-00017a90: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
-00017aa0: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
-00017ab0: 7269 6768 7429 0a0a 2020 2020 6465 6620  right)..    def 
-00017ac0: 5f6d 616b 655f 6469 6d28 7365 6c66 2c20  _make_dim(self, 
-00017ad0: 6f74 6865 722c 206b 696e 6429 3a0a 2020  other, kind):.  
-00017ae0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00017af0: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
-00017b00: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
-00017b10: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
-00017b20: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00017b30: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
-00017b40: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00017b50: 7374 616e 6365 286f 7468 6572 2c20 696e  stance(other, in
-00017b60: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00017b70: 6261 7365 5f74 6167 203d 2073 656c 662e  base_tag = self.
-00017b80: 7265 7072 6573 656e 7461 7469 7665 5f74  representative_t
-00017b90: 6167 2829 0a20 2020 2020 2020 2020 2020  ag().           
-00017ba0: 2072 6574 7572 6e20 5f6d 616b 655f 636f   return _make_co
-00017bb0: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
-00017bc0: 6d28 6f74 6865 722c 206b 696e 643d 6261  m(other, kind=ba
-00017bd0: 7365 5f74 6167 2e6b 696e 6420 6966 2062  se_tag.kind if b
-00017be0: 6173 655f 7461 6720 656c 7365 204e 6f6e  ase_tag else Non
-00017bf0: 6529 0a20 2020 2020 2020 2065 6c69 6620  e).        elif 
-00017c00: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
-00017c10: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
-00017c20: 2020 2020 2020 2072 6574 7572 6e20 6f74         return ot
-00017c30: 6865 722e 6765 745f 7361 6d65 5f62 6173  her.get_same_bas
-00017c40: 6528 290a 2020 2020 2020 2020 656c 7365  e().        else
-00017c50: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00017c60: 6973 6520 5479 7065 4572 726f 7228 2225  ise TypeError("%
-00017c70: 7320 2573 2025 7320 696e 7661 6c69 6420  s %s %s invalid 
-00017c80: 666f 7220 7479 7065 2025 7322 2025 2028  for type %s" % (
-00017c90: 7365 6c66 2c20 6b69 6e64 2c20 6f74 6865  self, kind, othe
-00017ca0: 722c 2074 7970 6528 6f74 6865 7229 2929  r, type(other)))
-00017cb0: 0a0a 2020 2020 6465 6620 7265 7072 6573  ..    def repres
-00017cc0: 656e 7461 7469 7665 5f74 6167 2873 656c  entative_tag(sel
-00017cd0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00017ce0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00017cf0: 4469 6d7c 4e6f 6e65 0a20 2020 2020 2020  Dim|None.       
-00017d00: 2022 2222 0a20 2020 2020 2020 2023 2046   """.        # F
-00017d10: 6972 7374 2066 696e 6420 616e 7920 6479  irst find any dy
-00017d20: 6e61 6d69 632e 0a20 2020 2020 2020 2066  namic..        f
-00017d30: 6f72 2074 6572 6d20 696e 2073 656c 662e  or term in self.
-00017d40: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
-00017d50: 2020 2066 6f72 2074 6572 6d5f 2069 6e20     for term_ in 
-00017d60: 7465 726d 2e74 6572 6d73 3a0a 2020 2020  term.terms:.    
-00017d70: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00017d80: 6572 6d5f 2e69 735f 6479 6e61 6d69 6328  erm_.is_dynamic(
-00017d90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017da0: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
-00017db0: 726d 5f0a 2020 2020 2020 2020 2320 4e6f  rm_.        # No
-00017dc0: 7720 6669 6e64 206e 6f6e 2d75 6e73 7065  w find non-unspe
-00017dd0: 6369 6669 6564 2e0a 2020 2020 2020 2020  cified..        
-00017de0: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
-00017df0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00017e00: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
-00017e10: 2074 6572 6d2e 7465 726d 733a 0a20 2020   term.terms:.   
-00017e20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00017e30: 7465 726d 5f2e 6b69 6e64 2021 3d20 4469  term_.kind != Di
-00017e40: 6d54 7970 6573 2e55 6e73 7065 6369 6669  mTypes.Unspecifi
-00017e50: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00017e60: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00017e70: 6572 6d5f 0a20 2020 2020 2020 2023 204e  erm_.        # N
-00017e80: 6f77 2066 696e 6420 616e 792e 0a20 2020  ow find any..   
-00017e90: 2020 2020 2066 6f72 2074 6572 6d20 696e       for term in
-00017ea0: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
-00017eb0: 2020 2020 2020 2020 2066 6f72 2074 6572           for ter
-00017ec0: 6d5f 2069 6e20 7465 726d 2e74 6572 6d73  m_ in term.terms
-00017ed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017ee0: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
-00017ef0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00017f00: 6e65 0a0a 0a64 6566 205f 6765 745f 6d65  ne...def _get_me
-00017f10: 7267 6564 5f64 696d 5f6b 696e 6428 6469  rged_dim_kind(di
-00017f20: 6d5f 7461 6773 293a 0a20 2020 2022 2222  m_tags):.    """
-00017f30: 0a20 2020 203a 7061 7261 6d20 6c69 7374  .    :param list
-00017f40: 5b44 696d 5d7c 7475 706c 655b 4469 6d5d  [Dim]|tuple[Dim]
-00017f50: 2064 696d 5f74 6167 733a 0a20 2020 203a   dim_tags:.    :
-00017f60: 7265 7475 726e 3a20 6469 6d20 6b69 6e64  return: dim kind
-00017f70: 0a20 2020 203a 7274 7970 653a 2045 6e74  .    :rtype: Ent
-00017f80: 6974 790a 2020 2020 2222 220a 2020 2020  ity.    """.    
-00017f90: 6966 2061 6e79 2874 6167 2e69 735f 6261  if any(tag.is_ba
-00017fa0: 7463 685f 6469 6d28 2920 666f 7220 7461  tch_dim() for ta
-00017fb0: 6720 696e 2064 696d 5f74 6167 7329 3a0a  g in dim_tags):.
-00017fc0: 2020 2020 2020 2020 7265 7475 726e 2044          return D
-00017fd0: 696d 5479 7065 732e 4261 7463 680a 2020  imTypes.Batch.  
-00017fe0: 2020 656c 6966 2061 6e79 2874 6167 2e69    elif any(tag.i
-00017ff0: 735f 6665 6174 7572 655f 6469 6d28 2920  s_feature_dim() 
-00018000: 666f 7220 7461 6720 696e 2064 696d 5f74  for tag in dim_t
-00018010: 6167 7329 3a0a 2020 2020 2020 2020 7265  ags):.        re
-00018020: 7475 726e 2044 696d 5479 7065 732e 4665  turn DimTypes.Fe
-00018030: 6174 7572 650a 2020 2020 656c 7365 3a0a  ature.    else:.
-00018040: 2020 2020 2020 2020 7265 7475 726e 2044          return D
-00018050: 696d 5479 7065 732e 5370 6174 6961 6c0a  imTypes.Spatial.
-00018060: 0a0a 6465 6620 6469 6d5f 636d 705f 7661  ..def dim_cmp_va
-00018070: 6c75 6528 6f62 6a29 3a0a 2020 2020 2222  lue(obj):.    ""
-00018080: 220a 2020 2020 3a70 6172 616d 2044 696d  ".    :param Dim
-00018090: 7c5f 4d61 726b 6564 4469 6d20 6f62 6a3a  |_MarkedDim obj:
-000180a0: 0a20 2020 203a 7265 7475 726e 3a20 616e  .    :return: an
-000180b0: 7974 6869 6e67 2077 6869 6368 2063 616e  ything which can
-000180c0: 2062 6520 636f 6d70 6172 6564 0a20 2020   be compared.   
-000180d0: 2022 2222 0a20 2020 2023 204d 616b 6520   """.    # Make 
-000180e0: 4469 6d20 616e 6420 5f4d 6172 6b65 6444  Dim and _MarkedD
-000180f0: 696d 2063 6f6d 7061 7261 626c 6520 746f  im comparable to
-00018100: 2065 6163 6820 6f74 6865 722e 0a20 2020   each other..   
-00018110: 2023 204e 6f74 6520 7468 6174 2074 6865   # Note that the
-00018120: 206f 7264 6572 2069 7320 7265 616c 6c79   order is really
-00018130: 2061 7262 6974 7261 7279 2061 6e64 2064   arbitrary and d
-00018140: 6f65 7320 6e6f 7420 6d61 7474 6572 2e0a  oes not matter..
-00018150: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00018160: 6528 6f62 6a2c 205f 642e 4469 6d29 3a0a  e(obj, _d.Dim):.
-00018170: 2020 2020 2020 2020 6f62 6a20 3d20 6f62          obj = ob
-00018180: 6a2e 6765 745f 7361 6d65 5f62 6173 6528  j.get_same_base(
-00018190: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000181a0: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
-000181b0: 222c 0a20 2020 2020 2020 2020 2020 206f  ",.            o
-000181c0: 626a 2e64 6573 6372 6970 7469 6f6e 2c0a  bj.description,.
-000181d0: 2020 2020 2020 2020 2020 2020 6f62 6a2e              obj.
-000181e0: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
-000181f0: 2020 6f62 6a2e 6469 6d65 6e73 696f 6e2c    obj.dimension,
-00018200: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
-00018210: 2e64 796e 5f73 697a 655f 6578 742e 6469  .dyn_size_ext.di
-00018220: 6d73 2069 6620 6f62 6a2e 6479 6e5f 7369  ms if obj.dyn_si
-00018230: 7a65 5f65 7874 2069 7320 6e6f 7420 4e6f  ze_ext is not No
-00018240: 6e65 2065 6c73 6520 4e6f 6e65 2c0a 2020  ne else None,.  
-00018250: 2020 2020 2020 290a 2020 2020 6966 2069        ).    if i
-00018260: 7369 6e73 7461 6e63 6528 6f62 6a2c 205f  sinstance(obj, _
-00018270: 6d2e 4d61 726b 6564 4469 6d29 3a0a 2020  m.MarkedDim):.  
-00018280: 2020 2020 2020 7265 7475 726e 206f 626a        return obj
-00018290: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-000182a0: 655f 5f2c 206f 626a 2e74 6167 0a20 2020  e__, obj.tag.   
-000182b0: 2072 6574 7572 6e20 6f62 6a0a             return obj.
+0000f770: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+0000f780: 6528 6469 6d2c 205f 642e 4469 6d29 0a20  e(dim, _d.Dim). 
+0000f790: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000f7a0: 696d 2e5f 7661 6c69 6461 7465 5f69 6e5f  im._validate_in_
+0000f7b0: 6375 7272 656e 745f 6772 6170 6828 290a  current_graph().
+0000f7c0: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
+0000f7d0: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
+0000f7e0: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
+0000f7f0: 2069 6620 6f74 6865 722e 5f65 7874 7261   if other._extra
+0000f800: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000f810: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+0000f820: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
+0000f830: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+0000f840: 6579 2c20 6469 6d20 696e 206f 7468 6572  ey, dim in other
+0000f850: 2e5f 6578 7472 612e 7361 6d65 5f66 6f72  ._extra.same_for
+0000f860: 5f62 6174 6368 5f63 7478 2e69 7465 6d73  _batch_ctx.items
+0000f870: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000f880: 2020 2020 6966 206e 6f74 2064 696d 2e5f      if not dim._
+0000f890: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
+0000f8a0: 656e 745f 6772 6170 6828 293a 0a20 2020  ent_graph():.   
+0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8c0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+0000f8d0: 2020 2020 2020 2020 2020 7365 6c66 5f64            self_d
+0000f8e0: 696d 203d 2073 656c 662e 5f6d 616b 655f  im = self._make_
+0000f8f0: 6578 7472 6128 292e 7361 6d65 5f66 6f72  extra().same_for
+0000f900: 5f62 6174 6368 5f63 7478 2e67 6574 286b  _batch_ctx.get(k
+0000f910: 6579 2c20 4e6f 6e65 290a 2020 2020 2020  ey, None).      
+0000f920: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000f930: 665f 6469 6d20 616e 6420 2873 656c 665f  f_dim and (self_
+0000f940: 6469 6d2e 6479 6e5f 7369 7a65 5f65 7874  dim.dyn_size_ext
+0000f950: 206f 7220 6e6f 7420 6469 6d2e 6479 6e5f   or not dim.dyn_
+0000f960: 7369 7a65 5f65 7874 293a 0a20 2020 2020  size_ext):.     
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f980: 6f6e 7469 6e75 6520 2023 206b 6565 7020  ontinue  # keep 
+0000f990: 6f75 7273 0a20 2020 2020 2020 2020 2020  ours.           
+0000f9a0: 2020 2020 2069 6620 6e6f 7420 6469 6d2e       if not dim.
+0000f9b0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9d0: 2020 636f 6e74 696e 7565 2020 2320 756e    continue  # un
+0000f9e0: 6465 6669 6e65 642c 2064 6f20 6e6f 7420  defined, do not 
+0000f9f0: 6f76 6572 7461 6b65 0a20 2020 2020 2020  overtake.       
+0000fa00: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+0000fa10: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
+0000fa20: 7463 685f 6374 785b 6b65 795d 203d 2064  tch_ctx[key] = d
+0000fa30: 696d 0a20 2020 2020 2020 2020 2020 2023  im.            #
+0000fa40: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+0000fa50: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+0000fa60: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+0000fa70: 722e 5f65 7874 7261 2e73 616d 655f 666f  r._extra.same_fo
+0000fa80: 725f 6261 7463 685f 6374 782e 636c 6561  r_batch_ctx.clea
+0000fa90: 7228 2920 2023 2077 6520 6f6e 6c79 2077  r()  # we only w
+0000faa0: 616e 7420 746f 2068 6176 6520 6974 206f  ant to have it o
+0000fab0: 6e63 650a 0a20 2020 2023 206e 6f69 6e73  nce..    # noins
+0000fac0: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
+0000fad0: 7465 644d 656d 6265 720a 2020 2020 6465  tedMember.    de
+0000fae0: 6620 6465 7269 7665 5f66 726f 6d28 7365  f derive_from(se
+0000faf0: 6c66 3a20 5f64 2e44 696d 2c20 6261 7365  lf: _d.Dim, base
+0000fb00: 3a20 5f64 2e44 696d 2c20 7365 745f 6465  : _d.Dim, set_de
+0000fb10: 7269 7665 645f 6672 6f6d 5f66 6c61 673a  rived_from_flag:
+0000fb20: 2062 6f6f 6c20 3d20 5472 7565 293a 0a20   bool = True):. 
+0000fb30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000fb40: 2020 203a 7061 7261 6d20 6261 7365 3a20     :param base: 
+0000fb50: 6469 6d0a 2020 2020 2020 2020 3a70 6172  dim.        :par
+0000fb60: 616d 2073 6574 5f64 6572 6976 6564 5f66  am set_derived_f
+0000fb70: 726f 6d5f 666c 6167 3a0a 2020 2020 2020  rom_flag:.      
+0000fb80: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+0000fb90: 6c66 5f62 6173 6520 3d20 7365 6c66 2e67  lf_base = self.g
+0000fba0: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
+0000fbb0: 2020 2020 2020 2073 656c 665f 6261 7365         self_base
+0000fbc0: 5f65 7874 7261 203d 2073 656c 665f 6261  _extra = self_ba
+0000fbd0: 7365 2e5f 6d61 6b65 5f65 7874 7261 2829  se._make_extra()
+0000fbe0: 0a20 2020 2020 2020 2069 6620 7365 745f  .        if set_
+0000fbf0: 6465 7269 7665 645f 6672 6f6d 5f66 6c61  derived_from_fla
+0000fc00: 673a 0a20 2020 2020 2020 2020 2020 2069  g:.            i
+0000fc10: 6620 7365 6c66 5f62 6173 655f 6578 7472  f self_base_extr
+0000fc20: 612e 6465 7269 7665 645f 6672 6f6d 5f74  a.derived_from_t
+0000fc30: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+0000fc40: 2020 2020 6173 7365 7274 2073 656c 665f      assert self_
+0000fc50: 6261 7365 5f65 7874 7261 2e64 6572 6976  base_extra.deriv
+0000fc60: 6564 5f66 726f 6d5f 7461 6720 3d3d 2062  ed_from_tag == b
+0000fc70: 6173 650a 2020 2020 2020 2020 2020 2020  ase.            
+0000fc80: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000fc90: 2020 2020 2020 7365 6c66 5f62 6173 655f        self_base_
+0000fca0: 6578 7472 612e 6465 7269 7665 645f 6672  extra.derived_fr
+0000fcb0: 6f6d 5f74 6167 203d 2062 6173 650a 2020  om_tag = base.  
+0000fcc0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+0000fcd0: 662e 6261 7463 6820 616e 6420 6261 7365  f.batch and base
+0000fce0: 2e62 6174 6368 3a0a 2020 2020 2020 2020  .batch:.        
+0000fcf0: 2020 2020 7365 6c66 2e62 6174 6368 203d      self.batch =
+0000fd00: 2062 6173 652e 6261 7463 680a 2020 2020   base.batch.    
+0000fd10: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000fd20: 7472 6f6c 5f66 6c6f 775f 6374 7820 3d20  trol_flow_ctx = 
+0000fd30: 6261 7365 2e63 6f6e 7472 6f6c 5f66 6c6f  base.control_flo
+0000fd40: 775f 6374 780a 2020 2020 2020 2020 2020  w_ctx.          
+0000fd50: 2020 6b65 7920 3d20 6261 7365 2e62 6174    key = base.bat
+0000fd60: 6368 2c20 6261 7365 2e63 6f6e 7472 6f6c  ch, base.control
+0000fd70: 5f66 6c6f 775f 6374 780a 2020 2020 2020  _flow_ctx.      
+0000fd80: 2020 2020 2020 6173 7365 7274 206b 6579        assert key
+0000fd90: 206e 6f74 2069 6e20 7365 6c66 5f62 6173   not in self_bas
+0000fda0: 655f 6578 7472 612e 7361 6d65 5f66 6f72  e_extra.same_for
+0000fdb0: 5f62 6174 6368 5f63 7478 0a20 2020 2020  _batch_ctx.     
+0000fdc0: 2020 2020 2020 2073 656c 665f 6261 7365         self_base
+0000fdd0: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000fde0: 6261 7463 685f 6374 785b 6b65 795d 203d  batch_ctx[key] =
+0000fdf0: 2073 656c 660a 2020 2020 2020 2020 6966   self.        if
+0000fe00: 2073 656c 662e 6973 5f64 796e 616d 6963   self.is_dynamic
+0000fe10: 2829 206f 7220 6e6f 7420 7365 6c66 2e69  () or not self.i
+0000fe20: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
+0000fe30: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000fe40: 7420 7365 6c66 2e64 796e 5f73 697a 655f  t self.dyn_size_
+0000fe50: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
+0000fe60: 2020 2020 2069 6620 6261 7365 2e64 796e       if base.dyn
+0000fe70: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
+0000fe80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000fe90: 6620 6261 7365 2e62 6174 6368 2061 6e64  f base.batch and
+0000fea0: 2062 6173 652e 6261 7463 6820 3d3d 2073   base.batch == s
+0000feb0: 656c 662e 6261 7463 6820 616e 6420 6261  elf.batch and ba
+0000fec0: 7365 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  se.control_flow_
+0000fed0: 6374 7820 3d3d 2073 656c 662e 636f 6e74  ctx == self.cont
+0000fee0: 726f 6c5f 666c 6f77 5f63 7478 3a0a 2020  rol_flow_ctx:.  
+0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff00: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
+0000ff10: 697a 655f 6578 7420 3d20 6261 7365 2e64  ize_ext = base.d
+0000ff20: 796e 5f73 697a 655f 6578 742e 636f 7079  yn_size_ext.copy
+0000ff30: 5f74 656d 706c 6174 6528 6e61 6d65 3d22  _template(name="
+0000ff40: 2573 3a73 697a 6522 2025 2073 656c 665f  %s:size" % self_
+0000ff50: 6261 7365 2e64 6573 6372 6970 7469 6f6e  base.description
+0000ff60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ff70: 2020 656c 6966 2062 6173 652e 6973 5f62    elif base.is_b
+0000ff80: 6174 6368 5f64 696d 2829 3a0a 2020 2020  atch_dim():.    
+0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffa0: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+0000ffb0: 7420 3d20 5f74 2e54 656e 736f 7228 0a20  t = _t.Tensor(. 
+0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffd0: 2020 2020 2020 206e 616d 653d 2225 733a         name="%s:
+0000ffe0: 6261 7463 6822 2025 2073 656c 665f 6261  batch" % self_ba
+0000fff0: 7365 2e64 6573 6372 6970 7469 6f6e 2c20  se.description, 
+00010000: 7368 6170 653d 2829 2c20 6474 7970 653d  shape=(), dtype=
+00010010: 2269 6e74 3332 222c 2062 6174 6368 5f64  "int32", batch_d
+00010020: 696d 5f61 7869 733d 4e6f 6e65 0a20 2020  im_axis=None.   
+00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010040: 2029 0a0a 2020 2020 6465 6620 636f 7079   )..    def copy
+00010050: 5f66 726f 6d28 7365 6c66 3a20 4469 6d2c  _from(self: Dim,
+00010060: 206f 7468 6572 3a20 4469 6d29 3a0a 2020   other: Dim):.  
+00010070: 2020 2020 2020 2222 2264 6566 696e 6522        """define"
+00010080: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00010090: 7369 7a65 203d 206f 7468 6572 2e73 697a  size = other.siz
+000100a0: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
+000100b0: 6170 6163 6974 7920 3d20 6f74 6865 722e  apacity = other.
+000100c0: 6361 7061 6369 7479 0a20 2020 2020 2020  capacity.       
+000100d0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+000100e0: 7874 203d 206f 7468 6572 2e64 796e 5f73  xt = other.dyn_s
+000100f0: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
+00010100: 7365 6c66 2e64 6572 6976 655f 6672 6f6d  self.derive_from
+00010110: 286f 7468 6572 290a 0a20 2020 2040 636c  (other)..    @cl
+00010120: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00010130: 6620 6765 745f 6578 6973 7469 6e67 5f74  f get_existing_t
+00010140: 6167 5f66 726f 6d5f 636f 6c6c 6563 7469  ag_from_collecti
+00010150: 6f6e 2863 6c73 2c20 6f74 6865 722c 2074  on(cls, other, t
+00010160: 6167 732c 2069 735f 6571 7561 6c5f 6f70  ags, is_equal_op
+00010170: 7473 3d4e 6f6e 6529 3a0a 2020 2020 2020  ts=None):.      
+00010180: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00010190: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
+000101a0: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
+000101b0: 6973 745b 4469 6d5d 7c74 7570 6c65 5b44  ist[Dim]|tuple[D
+000101c0: 696d 5d7c 7365 745b 4469 6d5d 2074 6167  im]|set[Dim] tag
+000101d0: 733a 0a20 2020 2020 2020 203a 7061 7261  s:.        :para
+000101e0: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
+000101f0: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
+00010200: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
+00010210: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
+00010220: 7274 7970 653a 2044 696d 7c4e 6f6e 650a  rtype: Dim|None.
+00010230: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010240: 2020 2020 6966 2069 735f 6571 7561 6c5f      if is_equal_
+00010250: 6f70 7473 2069 7320 4e6f 6e65 3a0a 2020  opts is None:.  
+00010260: 2020 2020 2020 2020 2020 6973 5f65 7175            is_equ
+00010270: 616c 5f6f 7074 7320 3d20 7b7d 0a20 2020  al_opts = {}.   
+00010280: 2020 2020 2023 2057 6520 646f 2070 6f74       # We do pot
+00010290: 656e 7469 616c 206d 756c 7469 706c 6520  ential multiple 
+000102a0: 726f 756e 6473 2c20 7375 6368 2074 6861  rounds, such tha
+000102b0: 7420 7765 2070 7265 6665 7220 226d 6f72  t we prefer "mor
+000102c0: 6520 6571 7561 6c22 2028 7573 696e 6720  e equal" (using 
+000102d0: 6c65 7373 2069 735f 6571 7561 6c5f 6f70  less is_equal_op
+000102e0: 7473 292e 0a20 2020 2020 2020 2072 6f75  ts)..        rou
+000102f0: 6e64 7320 3d20 5b7b 7d5d 0a20 2020 2020  nds = [{}].     
+00010300: 2020 2069 6620 6973 5f65 7175 616c 5f6f     if is_equal_o
+00010310: 7074 733a 0a20 2020 2020 2020 2020 2020  pts:.           
+00010320: 2069 6620 2262 726f 6164 6361 7374 5f6d   if "broadcast_m
+00010330: 6174 6368 6573 2220 696e 2069 735f 6571  atches" in is_eq
+00010340: 7561 6c5f 6f70 7473 3a0a 2020 2020 2020  ual_opts:.      
+00010350: 2020 2020 2020 2020 2020 726f 756e 6473            rounds
+00010360: 2e61 7070 656e 6428 7b6b 3a20 7620 666f  .append({k: v fo
+00010370: 7220 286b 2c20 7629 2069 6e20 6973 5f65  r (k, v) in is_e
+00010380: 7175 616c 5f6f 7074 732e 6974 656d 7328  qual_opts.items(
+00010390: 2920 6966 206b 2021 3d20 2262 726f 6164  ) if k != "broad
+000103a0: 6361 7374 5f6d 6174 6368 6573 227d 290a  cast_matches"}).
+000103b0: 2020 2020 2020 2020 2020 2020 726f 756e              roun
+000103c0: 6473 2e61 7070 656e 6428 6973 5f65 7175  ds.append(is_equ
+000103d0: 616c 5f6f 7074 7329 0a20 2020 2020 2020  al_opts).       
+000103e0: 2066 6f72 205f 6973 5f65 7175 616c 5f6f   for _is_equal_o
+000103f0: 7074 7320 696e 2072 6f75 6e64 733a 0a20  pts in rounds:. 
+00010400: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
+00010410: 7461 6720 696e 2074 6167 733a 0a20 2020  tag in tags:.   
+00010420: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010430: 5f74 6167 2e69 735f 6571 7561 6c28 6f74  _tag.is_equal(ot
+00010440: 6865 722c 202a 2a5f 6973 5f65 7175 616c  her, **_is_equal
+00010450: 5f6f 7074 7329 3a0a 2020 2020 2020 2020  _opts):.        
+00010460: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00010470: 726e 205f 7461 670a 2020 2020 2020 2020  rn _tag.        
+00010480: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00010490: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+000104a0: 2020 6465 6620 6765 745f 616c 6c5f 6469    def get_all_di
+000104b0: 6d65 6e73 696f 6e5f 7461 6773 2863 6c73  mension_tags(cls
+000104c0: 2c20 6461 7461 5f6c 6973 742c 2069 735f  , data_list, is_
+000104d0: 6571 7561 6c5f 6f70 7473 3d4e 6f6e 652c  equal_opts=None,
+000104e0: 2075 6e69 7175 655f 7365 7061 7261 7465   unique_separate
+000104f0: 5f61 7865 733d 5472 7565 293a 0a20 2020  _axes=True):.   
+00010500: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00010510: 203a 7061 7261 6d20 6c69 7374 5b5f 742e   :param list[_t.
+00010520: 5465 6e73 6f72 5d20 6461 7461 5f6c 6973  Tensor] data_lis
+00010530: 743a 0a20 2020 2020 2020 203a 7061 7261  t:.        :para
+00010540: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
+00010550: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
+00010560: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
+00010570: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
+00010580: 7061 7261 6d20 626f 6f6c 2075 6e69 7175  param bool uniqu
+00010590: 655f 7365 7061 7261 7465 5f61 7865 733a  e_separate_axes:
+000105a0: 2065 2e67 2e20 6461 7461 5f6c 6973 743d   e.g. data_list=
+000105b0: 5b44 6174 6120 7769 7468 2073 6861 7065  [Data with shape
+000105c0: 2028 422c 352c 352c 3130 295d 2072 6573   (B,5,5,10)] res
+000105d0: 756c 7473 2069 6e20 3420 6469 6d20 7461  ults in 4 dim ta
+000105e0: 6773 2c20 6e6f 7420 332e 0a20 2020 2020  gs, not 3..     
+000105f0: 2020 203a 7265 7475 726e 3a20 6c69 7374     :return: list
+00010600: 206f 6620 6469 6d65 6e73 696f 6e20 7461   of dimension ta
+00010610: 6773 2c20 6469 6374 2066 6f72 2064 6174  gs, dict for dat
+00010620: 6120 2d3e 206c 6973 7420 6f66 2064 696d  a -> list of dim
+00010630: 656e 7369 6f6e 2074 6167 7320 2866 6f72  ension tags (for
+00010640: 2065 6163 6820 6178 6973 290a 2020 2020   each axis).    
+00010650: 2020 2020 3a72 7479 7065 3a20 286c 6973      :rtype: (lis
+00010660: 745b 4469 6d5d 2c20 7574 696c 2e44 6963  t[Dim], util.Dic
+00010670: 7452 6566 4b65 7973 5b5f 742e 5465 6e73  tRefKeys[_t.Tens
+00010680: 6f72 2c20 6c69 7374 5b44 696d 5d5d 290a  or, list[Dim]]).
+00010690: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000106a0: 2020 2020 7461 6773 203d 205b 5d0a 2020      tags = [].  
+000106b0: 2020 2020 2020 6461 7461 5f61 7865 735f        data_axes_
+000106c0: 6469 6374 203d 2075 7469 6c2e 4469 6374  dict = util.Dict
+000106d0: 5265 664b 6579 7328 2920 2023 2074 7970  RefKeys()  # typ
+000106e0: 653a 2075 7469 6c2e 4469 6374 5265 664b  e: util.DictRefK
+000106f0: 6579 735b 5f74 2e54 656e 736f 722c 204c  eys[_t.Tensor, L
+00010700: 6973 745b 4469 6d5d 5d0a 2020 2020 2020  ist[Dim]].      
+00010710: 2020 666f 7220 6461 7461 2069 6e20 6461    for data in da
+00010720: 7461 5f6c 6973 743a 0a20 2020 2020 2020  ta_list:.       
+00010730: 2020 2020 2064 6174 615f 6178 6573 5f64       data_axes_d
+00010740: 6963 745b 6461 7461 5d20 3d20 5b5d 0a20  ict[data] = []. 
+00010750: 2020 2020 2020 2020 2020 2065 7869 7374             exist
+00010760: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
+00010770: 6f6e 5f66 6f72 5f64 6174 6120 3d20 6c69  on_for_data = li
+00010780: 7374 2874 6167 7329 2069 6620 756e 6971  st(tags) if uniq
+00010790: 7565 5f73 6570 6172 6174 655f 6178 6573  ue_separate_axes
+000107a0: 2065 6c73 6520 7461 6773 0a20 2020 2020   else tags.     
+000107b0: 2020 2020 2020 2066 6f72 2061 7869 7320         for axis 
+000107c0: 696e 2072 616e 6765 2864 6174 612e 6261  in range(data.ba
+000107d0: 7463 685f 6e64 696d 293a 0a20 2020 2020  tch_ndim):.     
+000107e0: 2020 2020 2020 2020 2020 2074 6167 203d             tag =
+000107f0: 2064 6174 612e 6765 745f 6469 6d5f 7461   data.get_dim_ta
+00010800: 6728 6178 6973 290a 2020 2020 2020 2020  g(axis).        
+00010810: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
+00010820: 5f74 6167 203d 2063 6c73 2e67 6574 5f65  _tag = cls.get_e
+00010830: 7869 7374 696e 675f 7461 675f 6672 6f6d  xisting_tag_from
+00010840: 5f63 6f6c 6c65 6374 696f 6e28 0a20 2020  _collection(.   
+00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010860: 2074 6167 2c20 7461 6773 3d65 7869 7374   tag, tags=exist
+00010870: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
+00010880: 6f6e 5f66 6f72 5f64 6174 612c 2069 735f  on_for_data, is_
+00010890: 6571 7561 6c5f 6f70 7473 3d69 735f 6571  equal_opts=is_eq
+000108a0: 7561 6c5f 6f70 7473 0a20 2020 2020 2020  ual_opts.       
+000108b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000108c0: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
+000108d0: 6973 7469 6e67 5f74 6167 3a0a 2020 2020  isting_tag:.    
+000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108f0: 6966 2075 6e69 7175 655f 7365 7061 7261  if unique_separa
+00010900: 7465 5f61 7865 733a 0a20 2020 2020 2020  te_axes:.       
+00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010920: 2065 7869 7374 696e 675f 7461 675f 636f   existing_tag_co
+00010930: 6c6c 6563 7469 6f6e 5f66 6f72 5f64 6174  llection_for_dat
+00010940: 612e 7265 6d6f 7665 2865 7869 7374 696e  a.remove(existin
+00010950: 675f 7461 6729 2020 2320 646f 6e27 7420  g_tag)  # don't 
+00010960: 7461 6b65 2069 7420 6167 6169 6e20 666f  take it again fo
+00010970: 7220 7468 6973 2064 6174 610a 2020 2020  r this data.    
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 7265 706c 6163 655f 6578 6973 7469 6e67  replace_existing
+000109a0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000109b0: 2020 2020 2020 2020 2020 2020 2065 7869               exi
+000109c0: 7374 696e 675f 7461 672e 756e 6465 6669  sting_tag.undefi
+000109d0: 6e65 6420 616e 6420 6e6f 7420 7461 672e  ned and not tag.
+000109e0: 756e 6465 6669 6e65 6420 616e 6420 7461  undefined and ta
+000109f0: 672e 6469 6d65 6e73 696f 6e20 3d3d 2065  g.dimension == e
+00010a00: 7869 7374 696e 675f 7461 672e 6469 6d65  xisting_tag.dime
+00010a10: 6e73 696f 6e0a 2020 2020 2020 2020 2020  nsion.          
+00010a20: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a40: 6966 2072 6570 6c61 6365 5f65 7869 7374  if replace_exist
+00010a50: 696e 673a 2020 2320 5265 706c 6163 6520  ing:  # Replace 
+00010a60: 7468 6520 6578 6973 7469 6e67 2062 7920  the existing by 
+00010a70: 7468 6520 6e65 7720 7461 672e 0a20 2020  the new tag..   
+00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a90: 2020 2020 2074 6167 735b 7461 6773 2e69       tags[tags.i
+00010aa0: 6e64 6578 2865 7869 7374 696e 675f 7461  ndex(existing_ta
+00010ab0: 6729 5d20 3d20 7461 670a 2020 2020 2020  g)] = tag.      
+00010ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ad0: 2020 666f 7220 5f2c 2064 696d 735f 2069    for _, dims_ i
+00010ae0: 6e20 6461 7461 5f61 7865 735f 6469 6374  n data_axes_dict
+00010af0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b10: 2020 2020 2020 6469 6d73 5f5b 3a5d 203d        dims_[:] =
+00010b20: 205b 7461 6720 6966 2064 203d 3d20 6578   [tag if d == ex
+00010b30: 6973 7469 6e67 5f74 6167 2065 6c73 6520  isting_tag else 
+00010b40: 6420 666f 7220 6420 696e 2064 696d 735f  d for d in dims_
+00010b50: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00010b60: 2020 2020 2020 2020 2020 6578 6973 7469            existi
+00010b70: 6e67 5f74 6167 203d 2074 6167 0a20 2020  ng_tag = tag.   
+00010b80: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00010b90: 653a 2020 2320 6e6f 2065 7869 7374 696e  e:  # no existin
+00010ba0: 6720 7461 670a 2020 2020 2020 2020 2020  g tag.          
+00010bb0: 2020 2020 2020 2020 2020 7461 6773 2e61            tags.a
+00010bc0: 7070 656e 6428 7461 6729 0a20 2020 2020  ppend(tag).     
+00010bd0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+00010be0: 6178 6573 5f64 6963 745b 6461 7461 5d2e  axes_dict[data].
+00010bf0: 6170 7065 6e64 2865 7869 7374 696e 675f  append(existing_
+00010c00: 7461 6720 6f72 2074 6167 290a 2020 2020  tag or tag).    
+00010c10: 2020 2020 7265 7475 726e 2074 6167 732c      return tags,
+00010c20: 2064 6174 615f 6178 6573 5f64 6963 740a   data_axes_dict.
+00010c30: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00010c40: 640a 2020 2020 6465 6620 6765 745f 756e  d.    def get_un
+00010c50: 6971 5f63 6f6c 6c65 6374 696f 6e28 636c  iq_collection(cl
+00010c60: 732c 2074 6167 732c 2069 735f 6571 7561  s, tags, is_equa
+00010c70: 6c5f 6f70 7473 3d4e 6f6e 6529 3a0a 2020  l_opts=None):.  
+00010c80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010c90: 2020 3a70 6172 616d 206c 6973 745b 4469    :param list[Di
+00010ca0: 6d5d 7c74 7570 6c65 5b44 696d 5d7c 7365  m]|tuple[Dim]|se
+00010cb0: 745b 4469 6d5d 2074 6167 733a 0a20 2020  t[Dim] tags:.   
+00010cc0: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
+00010cd0: 5b73 7472 5d7c 4e6f 6e65 2069 735f 6571  [str]|None is_eq
+00010ce0: 7561 6c5f 6f70 7473 3a20 7061 7373 6564  ual_opts: passed
+00010cf0: 2074 6f20 4469 6d2e 6973 5f65 7175 616c   to Dim.is_equal
+00010d00: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00010d10: 206c 6973 745b 4469 6d5d 0a20 2020 2020   list[Dim].     
+00010d20: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00010d30: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
+00010d40: 666f 7220 7461 6720 696e 2074 6167 733a  for tag in tags:
+00010d50: 0a20 2020 2020 2020 2020 2020 2065 7820  .            ex 
+00010d60: 3d20 636c 732e 6765 745f 6578 6973 7469  = cls.get_existi
+00010d70: 6e67 5f74 6167 5f66 726f 6d5f 636f 6c6c  ng_tag_from_coll
+00010d80: 6563 7469 6f6e 2874 6167 2c20 7265 732c  ection(tag, res,
+00010d90: 2069 735f 6571 7561 6c5f 6f70 7473 3d69   is_equal_opts=i
+00010da0: 735f 6571 7561 6c5f 6f70 7473 290a 2020  s_equal_opts).  
+00010db0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00010dc0: 2065 783a 0a20 2020 2020 2020 2020 2020   ex:.           
+00010dd0: 2020 2020 2072 6573 2e61 7070 656e 6428       res.append(
+00010de0: 7461 6729 0a20 2020 2020 2020 2072 6574  tag).        ret
+00010df0: 7572 6e20 7265 730a 0a20 2020 2064 6566  urn res..    def
+00010e00: 2067 6574 5f73 697a 655f 7465 6e73 6f72   get_size_tensor
+00010e10: 2873 656c 6629 202d 3e20 5f74 2e54 656e  (self) -> _t.Ten
+00010e20: 736f 723a 0a20 2020 2020 2020 2022 2222  sor:.        """
+00010e30: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00010e40: 3a20 7369 7a65 2074 656e 736f 722c 206f  : size tensor, o
+00010e50: 7220 6479 6e5f 7369 7a65 5f65 7874 2069  r dyn_size_ext i
+00010e60: 6620 6465 6669 6e65 640a 2020 2020 2020  f defined.      
+00010e70: 2020 3a72 7479 7065 3a20 5f74 2e54 656e    :rtype: _t.Ten
+00010e80: 736f 720a 2020 2020 2020 2020 2222 220a  sor.        """.
+00010e90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010ea0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+00010eb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010ec0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+00010ed0: 7874 0a0a 2020 2020 2020 2020 696d 706f  xt..        impo
+00010ee0: 7274 2072 6574 7572 6e6e 2e66 726f 6e74  rt returnn.front
+00010ef0: 656e 6420 6173 2072 660a 0a20 2020 2020  end as rf..     
+00010f00: 2020 2061 7373 6572 7420 7365 6c66 2e73     assert self.s
+00010f10: 697a 6520 6973 206e 6f74 204e 6f6e 650a  ize is not None.
+00010f20: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00010f30: 662e 636f 6e76 6572 745f 746f 5f74 656e  f.convert_to_ten
+00010f40: 736f 7228 7365 6c66 2e73 697a 652c 206e  sor(self.size, n
+00010f50: 616d 653d 2225 733a 7369 7a65 2220 2520  ame="%s:size" % 
+00010f60: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
+00010f70: 290a 0a20 2020 2064 6566 2067 6574 5f64  )..    def get_d
+00010f80: 696d 5f76 616c 7565 2873 656c 6629 202d  im_value(self) -
+00010f90: 3e20 556e 696f 6e5b 696e 742c 205f 742e  > Union[int, _t.
+00010fa0: 5261 7754 656e 736f 7254 7970 655d 3a0a  RawTensorType]:.
+00010fb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010fc0: 2020 2020 496e 6665 7273 2074 6865 2064      Infers the d
+00010fd0: 696d 2074 6869 7320 6178 6973 2073 686f  im this axis sho
+00010fe0: 756c 6420 6861 7665 2069 6620 756e 6272  uld have if unbr
+00010ff0: 6f61 6463 6173 7465 642e 0a20 2020 2020  oadcasted..     
+00011000: 2020 2049 6620 6073 656c 662e 7372 635f     If `self.src_
+00011010: 6461 7461 6020 6861 7320 6120 706c 6163  data` has a plac
+00011020: 6568 6f6c 6465 722c 2077 696c 6c20 7573  eholder, will us
+00011030: 6520 7468 6520 7368 6170 6520 6672 6f6d  e the shape from
+00011040: 2074 6865 7265 2e0a 2020 2020 2020 2020   there..        
+00011050: 4f74 6865 7277 6973 652c 2075 7365 7320  Otherwise, uses 
+00011060: 6073 656c 662e 6469 6d65 6e73 696f 6e60  `self.dimension`
+00011070: 2028 6966 2073 7461 7469 6329 206f 7220   (if static) or 
+00011080: 6073 656c 662e 6479 6e5f 7369 7a65 6020  `self.dyn_size` 
+00011090: 2869 6620 6479 6e61 6d69 6329 2e0a 0a20  (if dynamic)... 
+000110a0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000110b0: 6d61 7828 7369 7a65 206f 7220 6479 6e5f  max(size or dyn_
+000110c0: 7369 7a65 290a 2020 2020 2020 2020 2222  size).        ""
+000110d0: 220a 2020 2020 2020 2020 7265 7320 3d20  ".        res = 
+000110e0: 7365 6c66 2e67 6574 5f64 696d 5f76 616c  self.get_dim_val
+000110f0: 7565 5f74 656e 736f 7228 290a 2020 2020  ue_tensor().    
+00011100: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00011110: 6528 7265 732c 205f 742e 5465 6e73 6f72  e(res, _t.Tensor
+00011120: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+00011130: 7373 6572 7420 7265 732e 6469 6d73 203d  ssert res.dims =
+00011140: 3d20 2829 0a20 2020 2020 2020 2020 2020  = ().           
+00011150: 2072 6574 7572 6e20 7265 732e 7261 775f   return res.raw_
+00011160: 7465 6e73 6f72 0a20 2020 2020 2020 2061  tensor.        a
+00011170: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+00011180: 2872 6573 2c20 696e 7429 0a20 2020 2020  (res, int).     
+00011190: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
+000111a0: 2020 2064 6566 2067 6574 5f64 696d 5f76     def get_dim_v
+000111b0: 616c 7565 5f74 656e 736f 7228 7365 6c66  alue_tensor(self
+000111c0: 2920 2d3e 2055 6e69 6f6e 5b69 6e74 2c20  ) -> Union[int, 
+000111d0: 5f74 2e54 656e 736f 725d 3a0a 2020 2020  _t.Tensor]:.    
+000111e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000111f0: 496e 6665 7273 2074 6865 2064 696d 2074  Infers the dim t
+00011200: 6869 7320 6178 6973 2073 686f 756c 6420  his axis should 
+00011210: 6861 7665 2069 6620 756e 6272 6f61 6463  have if unbroadc
+00011220: 6173 7465 642e 0a20 2020 2020 2020 2049  asted..        I
+00011230: 6620 6073 656c 662e 7372 635f 6461 7461  f `self.src_data
+00011240: 6020 6861 7320 6120 706c 6163 6568 6f6c  ` has a placehol
+00011250: 6465 722c 2077 696c 6c20 7573 6520 7468  der, will use th
+00011260: 6520 7368 6170 6520 6672 6f6d 2074 6865  e shape from the
+00011270: 7265 2e0a 2020 2020 2020 2020 4f74 6865  re..        Othe
+00011280: 7277 6973 652c 2075 7365 7320 6073 656c  rwise, uses `sel
+00011290: 662e 6469 6d65 6e73 696f 6e60 2028 6966  f.dimension` (if
+000112a0: 2073 7461 7469 6329 206f 7220 6073 656c   static) or `sel
+000112b0: 662e 6479 6e5f 7369 7a65 6020 2869 6620  f.dyn_size` (if 
+000112c0: 6479 6e61 6d69 6329 2e0a 0a20 2020 2020  dynamic)...     
+000112d0: 2020 203a 7265 7475 726e 3a20 6d61 7828     :return: max(
+000112e0: 7369 7a65 206f 7220 6479 6e5f 7369 7a65  size or dyn_size
+000112f0: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
+00011300: 2020 2020 2020 696d 706f 7274 2072 6574        import ret
+00011310: 7572 6e6e 2e66 726f 6e74 656e 6420 6173  urnn.frontend as
+00011320: 2072 660a 0a20 2020 2020 2020 2069 6620   rf..        if 
+00011330: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
+00011340: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00011350: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011360: 656c 662e 6469 6d65 6e73 696f 6e0a 2020  elf.dimension.  
+00011370: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
+00011380: 6e5f 7369 7a65 5f65 7874 2061 6e64 2073  n_size_ext and s
+00011390: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+000113a0: 2e70 6c61 6365 686f 6c64 6572 2069 7320  .placeholder is 
+000113b0: 6e6f 7420 4e6f 6e65 3a20 2023 2066 6173  not None:  # fas
+000113c0: 7420 7061 7468 0a20 2020 2020 2020 2020  t path.         
+000113d0: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
+000113e0: 697a 655f 6578 742e 6261 7463 685f 6e64  ize_ext.batch_nd
+000113f0: 696d 203e 2030 3a0a 2020 2020 2020 2020  im > 0:.        
+00011400: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00011410: 662e 7265 6475 6365 5f6d 6178 280a 2020  f.reduce_max(.  
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
+00011440: 6578 742c 0a20 2020 2020 2020 2020 2020  ext,.           
+00011450: 2020 2020 2020 2020 2061 7869 733d 7365           axis=se
+00011460: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
+00011470: 6469 6d5f 7461 6773 2c0a 2020 2020 2020  dim_tags,.      
+00011480: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00011490: 4d61 736b 696e 6720 6973 206e 6f74 2061  Masking is not a
+000114a0: 6c77 6179 7320 706f 7373 6962 6c65 2068  lways possible h
+000114b0: 6572 652c 2065 2e67 2e0a 2020 2020 2020  ere, e.g..      
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000114d0: 7365 6c66 203d 2044 696d 7b27 7365 6c66  self = Dim{'self
+000114e0: 2d61 7474 2d6b 6579 7327 5b27 7469 6d65  -att-keys'['time
+000114f0: 3a76 6172 3a65 7874 6572 6e5f 6461 7461  :var:extern_data
+00011500: 3a63 6c61 7373 6573 275b 425d 5d7d 2e0a  :classes'[B]]}..
+00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011520: 2020 2020 7573 655f 6d61 736b 3d46 616c      use_mask=Fal
+00011530: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00011540: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00011550: 2020 7265 7475 726e 2073 656c 662e 6479    return self.dy
+00011560: 6e5f 7369 7a65 5f65 7874 0a20 2020 2020  n_size_ext.     
+00011570: 2020 2069 6620 7365 6c66 2e69 735f 6261     if self.is_ba
+00011580: 7463 685f 6469 6d28 293a 0a20 2020 2020  tch_dim():.     
+00011590: 2020 2020 2020 2072 6573 203d 204e 6f6e         res = Non
+000115a0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+000115b0: 2073 656c 662e 5f65 7874 7261 2061 6e64   self._extra and
+000115c0: 2073 656c 662e 5f65 7874 7261 2e73 7263   self._extra.src
+000115d0: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
+000115e0: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
+000115f0: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
+00011600: 612e 6765 745f 6261 7463 685f 6469 6d28  a.get_batch_dim(
+00011610: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00011620: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
+00011630: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00011640: 6573 203d 2073 656c 662e 6261 7463 682e  es = self.batch.
+00011650: 6469 6d0a 2020 2020 2020 2020 2020 2020  dim.            
+00011660: 6966 2069 7369 6e73 7461 6e63 6528 7265  if isinstance(re
+00011670: 732c 2069 6e74 293a 0a20 2020 2020 2020  s, int):.       
+00011680: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011690: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
+000116a0: 6966 2072 6573 2069 7320 6e6f 7420 4e6f  if res is not No
+000116b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000116c0: 2020 2020 7265 7475 726e 205f 742e 5465      return _t.Te
+000116d0: 6e73 6f72 2822 6261 7463 6822 2c20 6469  nsor("batch", di
+000116e0: 6d73 3d28 292c 2064 7479 7065 3d72 662e  ms=(), dtype=rf.
+000116f0: 6765 745f 6465 6661 756c 745f 6172 7261  get_default_arra
+00011700: 795f 696e 6465 785f 6474 7970 6528 292c  y_index_dtype(),
+00011710: 2072 6177 5f74 656e 736f 723d 7265 7329   raw_tensor=res)
+00011720: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
+00011730: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00011740: 6578 7472 610a 2020 2020 2020 2020 2020  extra.          
+00011750: 2020 616e 6420 7365 6c66 2e5f 6578 7472    and self._extr
+00011760: 612e 7372 635f 6461 7461 2069 7320 6e6f  a.src_data is no
+00011770: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
+00011780: 2020 2061 6e64 2073 656c 662e 5f65 7874     and self._ext
+00011790: 7261 2e73 7263 5f61 7869 7320 6973 206e  ra.src_axis is n
+000117a0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+000117b0: 2020 2020 616e 6420 7365 6c66 2e5f 6578      and self._ex
+000117c0: 7472 612e 7372 635f 6461 7461 2e70 6c61  tra.src_data.pla
+000117d0: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
+000117e0: 4e6f 6e65 0a20 2020 2020 2020 2029 3a0a  None.        ):.
+000117f0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00011800: 3d20 7365 6c66 2e5f 6578 7472 612e 7372  = self._extra.sr
+00011810: 635f 6461 7461 2e67 6574 5f64 696d 2873  c_data.get_dim(s
+00011820: 656c 662e 5f65 7874 7261 2e73 7263 5f61  elf._extra.src_a
+00011830: 7869 7329 0a20 2020 2020 2020 2020 2020  xis).           
+00011840: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
+00011850: 6573 2c20 696e 7429 3a0a 2020 2020 2020  es, int):.      
+00011860: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011870: 2072 6573 0a20 2020 2020 2020 2020 2020   res.           
+00011880: 2072 6574 7572 6e20 5f74 2e54 656e 736f   return _t.Tenso
+00011890: 7228 2262 6174 6368 222c 2064 696d 733d  r("batch", dims=
+000118a0: 2829 2c20 6474 7970 653d 7266 2e67 6574  (), dtype=rf.get
+000118b0: 5f64 6566 6175 6c74 5f61 7272 6179 5f69  _default_array_i
+000118c0: 6e64 6578 5f64 7479 7065 2829 2c20 7261  ndex_dtype(), ra
+000118d0: 775f 7465 6e73 6f72 3d72 6573 290a 2020  w_tensor=res).  
+000118e0: 2020 2020 2020 7365 6c66 2e63 6f6d 706c        self.compl
+000118f0: 6574 655f 6479 6e5f 7369 7a65 2829 0a20  ete_dyn_size(). 
+00011900: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+00011910: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
+00011920: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00011930: 742e 706c 6163 6568 6f6c 6465 7220 6973  t.placeholder is
+00011940: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011950: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+00011960: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
+00011970: 685f 6e64 696d 203e 2030 3a0a 2020 2020  h_ndim > 0:.    
+00011980: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011990: 726e 2072 662e 7265 6475 6365 5f6d 6178  rn rf.reduce_max
+000119a0: 2873 656c 662e 6479 6e5f 7369 7a65 5f65  (self.dyn_size_e
+000119b0: 7874 2c20 6178 6973 3d73 656c 662e 6479  xt, axis=self.dy
+000119c0: 6e5f 7369 7a65 5f65 7874 2e64 696d 5f74  n_size_ext.dim_t
+000119d0: 6167 7329 0a20 2020 2020 2020 2020 2020  ags).           
+000119e0: 2072 6574 7572 6e20 7365 6c66 2e64 796e   return self.dyn
+000119f0: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
+00011a00: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+00011a10: 6e28 2225 733a 206e 6565 6420 706c 6163  n("%s: need plac
+00011a20: 6568 6f6c 6465 722c 2073 656c 662e 6469  eholder, self.di
+00011a30: 6d65 6e73 696f 6e20 6f72 2073 656c 662e  mension or self.
+00011a40: 6479 6e5f 7369 7a65 2066 6f72 2064 696d  dyn_size for dim
+00011a50: 2076 616c 7565 2220 2520 7365 6c66 290a   value" % self).
+00011a60: 0a20 2020 2064 6566 2061 7869 735f 7370  .    def axis_sp
+00011a70: 6c69 745f 696e 666f 2873 656c 6629 3a0a  lit_info(self):.
+00011a80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011a90: 2020 2020 3a72 6574 7572 6e3a 2061 7869      :return: axi
+00011aa0: 7320 7370 6c69 7420 696e 666f 2e20 7365  s split info. se
+00011ab0: 6520 3a66 756e 633a 6067 6574 5f70 6172  e :func:`get_par
+00011ac0: 616d 5f61 7865 735f 7370 6c69 745f 696e  am_axes_split_in
+00011ad0: 666f 6020 616e 6420 7573 6167 6520 2865  fo` and usage (e
+00011ae0: 2e67 2e20 7072 6574 7261 696e 696e 6729  .g. pretraining)
+00011af0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00011b00: 206c 6973 745b 696e 747c 4e6f 6e65 5d0a   list[int|None].
+00011b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011b20: 2020 2020 7361 6d65 5f62 6173 6520 3d20      same_base = 
+00011b30: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
+00011b40: 7365 2829 0a20 2020 2020 2020 206f 7020  se().        op 
+00011b50: 3d20 7365 6c66 2e64 6572 6976 6564 5f66  = self.derived_f
+00011b60: 726f 6d5f 6f70 206f 7220 7361 6d65 5f62  rom_op or same_b
+00011b70: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
+00011b80: 5f6f 700a 2020 2020 2020 2020 6966 206e  _op.        if n
+00011b90: 6f74 206f 703a 0a20 2020 2020 2020 2020  ot op:.         
+00011ba0: 2020 2072 6574 7572 6e20 5b73 656c 662e     return [self.
+00011bb0: 6469 6d65 6e73 696f 6e5d 0a20 2020 2020  dimension].     
+00011bc0: 2020 2069 6620 6f70 2e6b 696e 6420 3d3d     if op.kind ==
+00011bd0: 2022 6164 6422 3a0a 2020 2020 2020 2020   "add":.        
+00011be0: 2020 2020 7265 7475 726e 2073 756d 285b      return sum([
+00011bf0: 782e 6178 6973 5f73 706c 6974 5f69 6e66  x.axis_split_inf
+00011c00: 6f28 2920 666f 7220 7820 696e 206f 702e  o() for x in op.
+00011c10: 696e 7075 7473 5d2c 205b 5d29 2020 2320  inputs], [])  # 
+00011c20: 666c 6174 7465 6e0a 2020 2020 2020 2020  flatten.        
+00011c30: 6966 206f 702e 6b69 6e64 203d 3d20 226d  if op.kind == "m
+00011c40: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
+00011c50: 2072 6573 203d 205b 315d 0a20 2020 2020   res = [1].     
+00011c60: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
+00011c70: 6f70 2e69 6e70 7574 733a 0a20 2020 2020  op.inputs:.     
+00011c80: 2020 2020 2020 2020 2020 2072 6573 203d             res =
+00011c90: 2073 756d 285b 6e20 2a20 782e 6178 6973   sum([n * x.axis
+00011ca0: 5f73 706c 6974 5f69 6e66 6f28 2920 6966  _split_info() if
+00011cb0: 206e 2069 7320 6e6f 7420 4e6f 6e65 2065   n is not None e
+00011cc0: 6c73 6520 4e6f 6e65 2066 6f72 206e 2069  lse None for n i
+00011cd0: 6e20 7265 735d 2c20 5b5d 2920 2023 2066  n res], [])  # f
+00011ce0: 6c61 7474 656e 0a20 2020 2020 2020 2020  latten.         
+00011cf0: 2020 2072 6574 7572 6e20 7265 730a 2020     return res.  
+00011d00: 2020 2020 2020 7265 7475 726e 205b 7365        return [se
+00011d10: 6c66 2e64 696d 656e 7369 6f6e 5d0a 0a20  lf.dimension].. 
+00011d20: 2020 2064 6566 205f 6765 745f 7361 6d65     def _get_same
+00011d30: 5f62 6173 655f 6578 7472 6128 7365 6c66  _base_extra(self
+00011d40: 2920 2d3e 204f 7074 696f 6e61 6c5b 5f44  ) -> Optional[_D
+00011d50: 696d 4578 7472 615d 3a0a 2020 2020 2020  imExtra]:.      
+00011d60: 2020 6966 206e 6f74 2073 656c 662e 5f65    if not self._e
+00011d70: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
+00011d80: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+00011d90: 2020 2020 2020 6261 7365 203d 2073 656c        base = sel
+00011da0: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
+00011db0: 290a 2020 2020 2020 2020 2320 6e6f 696e  ).        # noin
+00011dc0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+00011dd0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+00011de0: 2020 2072 6574 7572 6e20 6261 7365 2e5f     return base._
+00011df0: 6578 7472 610a 0a20 2020 2064 6566 205f  extra..    def _
+00011e00: 6d61 6b65 5f65 7874 7261 2873 656c 663a  make_extra(self:
+00011e10: 205f 642e 4469 6d29 202d 3e20 5f44 696d   _d.Dim) -> _Dim
+00011e20: 4578 7472 613a 0a20 2020 2020 2020 2069  Extra:.        i
+00011e30: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
+00011e40: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
+00011e50: 656c 662e 5f65 7874 7261 203d 205f 4469  elf._extra = _Di
+00011e60: 6d45 7874 7261 2864 696d 3d73 656c 6629  mExtra(dim=self)
+00011e70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011e80: 7365 6c66 2e5f 6578 7472 610a 0a20 2020  self._extra..   
+00011e90: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00011ea0: 6566 2076 6f63 6162 2873 656c 6629 3a0a  ef vocab(self):.
+00011eb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011ec0: 2020 2020 3a72 7479 7065 3a20 7265 7475      :rtype: retu
+00011ed0: 726e 6e2e 6461 7461 7365 7473 2e75 7469  rnn.datasets.uti
+00011ee0: 6c2e 766f 6361 6275 6c61 7279 2e56 6f63  l.vocabulary.Voc
+00011ef0: 6162 756c 6172 797c 4e6f 6e65 0a20 2020  abulary|None.   
+00011f00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011f10: 2065 7874 7261 203d 2073 656c 662e 5f67   extra = self._g
+00011f20: 6574 5f73 616d 655f 6261 7365 5f65 7874  et_same_base_ext
+00011f30: 7261 2829 0a20 2020 2020 2020 2069 6620  ra().        if 
+00011f40: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
+00011f50: 2020 2072 6574 7572 6e20 6578 7472 612e     return extra.
+00011f60: 766f 6361 620a 2020 2020 2020 2020 7265  vocab.        re
+00011f70: 7475 726e 204e 6f6e 650a 0a20 2020 2040  turn None..    @
+00011f80: 766f 6361 622e 7365 7474 6572 0a20 2020  vocab.setter.   
+00011f90: 2064 6566 2076 6f63 6162 2873 656c 662c   def vocab(self,
+00011fa0: 2076 6f63 6162 293a 0a20 2020 2020 2020   vocab):.       
+00011fb0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+00011fc0: 7261 6d20 7265 7475 726e 6e2e 6461 7461  ram returnn.data
+00011fd0: 7365 7473 2e75 7469 6c2e 766f 6361 6275  sets.util.vocabu
+00011fe0: 6c61 7279 2e56 6f63 6162 756c 6172 797c  lary.Vocabulary|
+00011ff0: 4e6f 6e65 2076 6f63 6162 3a0a 2020 2020  None vocab:.    
+00012000: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012010: 6966 2076 6f63 6162 2069 7320 7365 6c66  if vocab is self
+00012020: 2e76 6f63 6162 3a0a 2020 2020 2020 2020  .vocab:.        
+00012030: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00012040: 2020 2069 6620 7365 6c66 2e73 616d 655f     if self.same_
+00012050: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
+00012060: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
+00012070: 7365 2829 2e76 6f63 6162 203d 2076 6f63  se().vocab = voc
+00012080: 6162 0a20 2020 2020 2020 2020 2020 2072  ab.            r
+00012090: 6574 7572 6e0a 2020 2020 2020 2020 6578  eturn.        ex
+000120a0: 7472 6120 3d20 7365 6c66 2e5f 6765 745f  tra = self._get_
+000120b0: 7361 6d65 5f62 6173 655f 6578 7472 6128  same_base_extra(
+000120c0: 290a 2020 2020 2020 2020 6966 2065 7874  ).        if ext
+000120d0: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
+000120e0: 6578 7472 612e 766f 6361 6220 3d20 766f  extra.vocab = vo
+000120f0: 6361 620a 0a20 2020 2023 2054 6865 206b  cab..    # The k
+00012100: 696e 6420 6f66 206f 7065 7261 7469 6f6e  ind of operation
+00012110: 7320 7765 2068 6176 653a 0a20 2020 2023  s we have:.    #
+00012120: 2061 202b 2062 3a20 7061 6464 696e 672c   a + b: padding,
+00012130: 2063 6f6e 6361 740a 2020 2020 2320 6120   concat.    # a 
+00012140: 2d20 623a 2077 696e 646f 7720 7769 7468  - b: window with
+00012150: 2076 616c 6964 2066 7261 6d65 7320 6f6e   valid frames on
+00012160: 6c79 0a20 2020 2023 2061 202a 2062 3a20  ly.    # a * b: 
+00012170: 6d65 7267 6520 6469 6d73 2c20 7570 7361  merge dims, upsa
+00012180: 6d70 6c65 2c20 7472 616e 7370 6f73 6564  mple, transposed
+00012190: 2063 6f6e 7620 7769 7468 2073 7472 6964   conv with strid
+000121a0: 696e 670a 2020 2020 2320 6120 2f20 6220  ing.    # a / b 
+000121b0: 2877 6865 6e20 6120 2520 6220 3d3d 2030  (when a % b == 0
+000121c0: 293a 2073 706c 6974 2064 696d 732c 2064  ): split dims, d
+000121d0: 6f77 6e73 616d 706c 652c 2063 6f6e 7620  ownsample, conv 
+000121e0: 7769 7468 2073 7472 6964 696e 670a 2020  with striding.  
+000121f0: 2020 2320 6365 696c 6469 7628 612c 2062    # ceildiv(a, b
+00012200: 293a 2063 6f6e 7620 7769 7468 2073 7472  ): conv with str
+00012210: 6964 696e 670a 2020 2020 2320 6375 7374  iding.    # cust
+00012220: 6f6d 3a20 7265 7065 6174 2c20 7265 6d6f  om: repeat, remo
+00012230: 7665 2c20 6d61 736b 2c20 6c6f 6f70 2077  ve, mask, loop w
+00012240: 6974 6820 6479 6e20 656e 640a 2020 2020  ith dyn end.    
+00012250: 2320 4e6f 7465 2074 6861 7420 7765 2064  # Note that we d
+00012260: 6966 6665 7265 6e74 6961 7465 2062 6574  ifferentiate bet
+00012270: 7765 656e 2074 6865 206f 7264 6572 2c20  ween the order, 
+00012280: 692e 652e 2061 202b 2062 2021 3d20 6220  i.e. a + b != b 
+00012290: 2b20 612e 0a20 2020 2023 204e 6f74 6520  + a..    # Note 
+000122a0: 7468 6174 2077 6520 616c 7761 7973 2068  that we always h
+000122b0: 6176 6520 7468 6520 6173 7375 6d70 7469  ave the assumpti
+000122c0: 6f6e 2074 6861 7420 6120 6469 6d65 6e73  on that a dimens
+000122d0: 696f 6e20 6973 206e 6f6e 2d6e 6567 6174  ion is non-negat
+000122e0: 6976 652e 0a20 2020 2023 2054 6869 7320  ive..    # This 
+000122f0: 6173 7375 6d70 7469 6f6e 2069 7320 6e65  assumption is ne
+00012300: 6365 7373 6172 7920 666f 7220 736f 6d65  cessary for some
+00012310: 2073 696d 706c 6966 6963 6174 696f 6e73   simplifications
+00012320: 2e0a 2020 2020 2320 6874 7470 733a 2f2f  ..    # https://
+00012330: 6769 7468 7562 2e63 6f6d 2f72 7774 682d  github.com/rwth-
+00012340: 6936 2f72 6574 7572 6e6e 2f70 756c 6c2f  i6/returnn/pull/
+00012350: 3835 330a 0a20 2020 2064 6566 205f 5f61  853..    def __a
+00012360: 6464 5f5f 2873 656c 663a 2044 696d 2c20  dd__(self: Dim, 
+00012370: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00012380: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+00012390: 616d 2044 696d 7c69 6e74 206f 7468 6572  am Dim|int other
+000123a0: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
+000123b0: 6e3a 2073 656c 6620 2b20 6f74 6865 722e  n: self + other.
+000123c0: 206e 6f74 6520 7468 6174 2074 6869 7320   note that this 
+000123d0: 6973 206e 6f74 2063 6f6d 6d75 7461 7469  is not commutati
+000123e0: 7665 2c20 692e 652e 2064 6966 6665 7265  ve, i.e. differe
+000123f0: 6e74 2066 726f 6d20 6f74 6865 7220 2b20  nt from other + 
+00012400: 7365 6c66 2e0a 2020 2020 2020 2020 3a72  self..        :r
+00012410: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+00012420: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
+00012430: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
+00012440: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
+00012450: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
+00012460: 7874 656e 645f 6164 645f 7375 625f 286f  xtend_add_sub_(o
+00012470: 7468 6572 2c20 6b69 6e64 3d22 6164 6422  ther, kind="add"
+00012480: 2c20 7269 6768 743d 5472 7565 290a 2020  , right=True).  
+00012490: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
+000124a0: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
+000124b0: 6465 6620 5f5f 7261 6464 5f5f 2873 656c  def __radd__(sel
+000124c0: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
+000124d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000124e0: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
+000124f0: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
+00012500: 2020 3a72 6574 7572 6e3a 206f 7468 6572    :return: other
+00012510: 202b 2073 656c 660a 2020 2020 2020 2020   + self.        
+00012520: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
+00012530: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012540: 7465 726d 203d 205f 4f70 4c69 6e65 6172  term = _OpLinear
+00012550: 5465 726d 2e66 726f 6d5f 6469 6d28 7365  Term.from_dim(se
+00012560: 6c66 290a 2020 2020 2020 2020 7465 726d  lf).        term
+00012570: 2e65 7874 656e 645f 6164 645f 7375 625f  .extend_add_sub_
+00012580: 286f 7468 6572 2c20 6b69 6e64 3d22 6164  (other, kind="ad
+00012590: 6422 2c20 7269 6768 743d 4661 6c73 6529  d", right=False)
+000125a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000125b0: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
+000125c0: 2020 2064 6566 205f 5f73 7562 5f5f 2873     def __sub__(s
+000125d0: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
+000125e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000125f0: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
+00012600: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+00012610: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
+00012620: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00012630: 6574 7572 6e20 7365 6c66 2e73 7562 5f72  eturn self.sub_r
+00012640: 6967 6874 286f 7468 6572 290a 0a20 2020  ight(other)..   
+00012650: 2064 6566 2073 7562 5f72 6967 6874 2873   def sub_right(s
+00012660: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
+00012670: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012680: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00012690: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
+000126a0: 2020 2020 3a72 6574 7572 6e3a 2073 656c      :return: sel
+000126b0: 6620 2d20 6f74 6865 720a 2020 2020 2020  f - other.      
+000126c0: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
+000126d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000126e0: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
+000126f0: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
+00012700: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
+00012710: 726d 2e65 7874 656e 645f 6164 645f 7375  rm.extend_add_su
+00012720: 625f 286f 7468 6572 2c20 6b69 6e64 3d22  b_(other, kind="
+00012730: 7375 6222 2c20 7269 6768 743d 5472 7565  sub", right=True
+00012740: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00012750: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
+00012760: 2020 2020 6465 6620 7375 625f 6c65 6674      def sub_left
+00012770: 2873 656c 663a 2044 696d 2c20 6f74 6865  (self: Dim, othe
+00012780: 7229 3a0a 2020 2020 2020 2020 2222 220a  r):.        """.
+00012790: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
+000127a0: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
+000127b0: 2020 2020 2020 3a72 6574 7572 6e3a 2028        :return: (
+000127c0: 2d6f 7468 6572 2920 2b20 7365 6c66 0a20  -other) + self. 
+000127d0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+000127e0: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
+000127f0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
+00012800: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
+00012810: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
+00012820: 2020 2074 6572 6d2e 6578 7465 6e64 5f61     term.extend_a
+00012830: 6464 5f73 7562 5f28 6f74 6865 722c 206b  dd_sub_(other, k
+00012840: 696e 643d 2273 7562 222c 2072 6967 6874  ind="sub", right
+00012850: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00012860: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
+00012870: 696d 2829 0a0a 2020 2020 6465 6620 5f5f  im()..    def __
+00012880: 6d75 6c5f 5f28 7365 6c66 3a20 4469 6d2c  mul__(self: Dim,
+00012890: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+000128a0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+000128b0: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
+000128c0: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
+000128d0: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
+000128e0: 2222 0a20 2020 2020 2020 2074 6572 6d20  "".        term 
+000128f0: 3d20 5f4f 704c 696e 6561 7254 6572 6d2e  = _OpLinearTerm.
+00012900: 6672 6f6d 5f64 696d 2873 656c 6629 0a20  from_dim(self). 
+00012910: 2020 2020 2020 2074 6572 6d2e 6578 7465         term.exte
+00012920: 6e64 5f6d 756c 5f64 6976 5f28 6f74 6865  nd_mul_div_(othe
+00012930: 722c 206b 696e 643d 226d 756c 222c 2072  r, kind="mul", r
+00012940: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
+00012950: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
+00012960: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
+00012970: 205f 5f72 6d75 6c5f 5f28 7365 6c66 3a20   __rmul__(self: 
+00012980: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
+00012990: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000129a0: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
+000129b0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+000129c0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
+000129d0: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
+000129e0: 6572 6d20 3d20 5f4f 704c 696e 6561 7254  erm = _OpLinearT
+000129f0: 6572 6d2e 6672 6f6d 5f64 696d 2873 656c  erm.from_dim(sel
+00012a00: 6629 0a20 2020 2020 2020 2074 6572 6d2e  f).        term.
+00012a10: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
+00012a20: 6f74 6865 722c 206b 696e 643d 226d 756c  other, kind="mul
+00012a30: 222c 2072 6967 6874 3d46 616c 7365 290a  ", right=False).
+00012a40: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00012a50: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
+00012a60: 2020 6465 6620 5f5f 666c 6f6f 7264 6976    def __floordiv
+00012a70: 5f5f 2873 656c 663a 2044 696d 2c20 6f74  __(self: Dim, ot
+00012a80: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
+00012a90: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00012aa0: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
+00012ab0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00012ac0: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
+00012ad0: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
+00012ae0: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
+00012af0: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
+00012b00: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
+00012b10: 6d75 6c5f 6469 765f 286f 7468 6572 2c20  mul_div_(other, 
+00012b20: 6b69 6e64 3d22 666c 6f6f 7264 6976 222c  kind="floordiv",
+00012b30: 2072 6967 6874 3d54 7275 6529 0a20 2020   right=True).   
+00012b40: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
+00012b50: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
+00012b60: 6566 205f 5f74 7275 6564 6976 5f5f 2873  ef __truediv__(s
+00012b70: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
+00012b80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012b90: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
+00012ba0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+00012bb0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
+00012bc0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00012bd0: 6574 7572 6e20 7365 6c66 2e64 6976 5f72  eturn self.div_r
+00012be0: 6967 6874 286f 7468 6572 290a 0a20 2020  ight(other)..   
+00012bf0: 2064 6566 2064 6976 5f6c 6566 7428 7365   def div_left(se
+00012c00: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
+00012c10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012c20: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
+00012c30: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
+00012c40: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
+00012c50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012c60: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
+00012c70: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
+00012c80: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
+00012c90: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
+00012ca0: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
+00012cb0: 2274 7275 6564 6976 222c 2072 6967 6874  "truediv", right
+00012cc0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00012cd0: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
+00012ce0: 696d 2829 0a0a 2020 2020 6465 6620 6469  im()..    def di
+00012cf0: 765f 7269 6768 7428 7365 6c66 3a20 4469  v_right(self: Di
+00012d00: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
+00012d10: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00012d20: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+00012d30: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
+00012d40: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00012d50: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
+00012d60: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
+00012d70: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
+00012d80: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
+00012d90: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
+00012da0: 6865 722c 206b 696e 643d 2274 7275 6564  her, kind="trued
+00012db0: 6976 222c 2072 6967 6874 3d54 7275 6529  iv", right=True)
+00012dc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012dd0: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
+00012de0: 2020 2064 6566 2063 6569 6c64 6976 5f6c     def ceildiv_l
+00012df0: 6566 7428 7365 6c66 3a20 4469 6d2c 206f  eft(self: Dim, o
+00012e00: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012e10: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012e20: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00012e30: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00012e40: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00012e50: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
+00012e60: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
+00012e70: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
+00012e80: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
+00012e90: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
+00012ea0: 206b 696e 643d 2263 6569 6c64 6976 222c   kind="ceildiv",
+00012eb0: 2072 6967 6874 3d46 616c 7365 290a 2020   right=False).  
+00012ec0: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
+00012ed0: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
+00012ee0: 6465 6620 6365 696c 6469 765f 7269 6768  def ceildiv_righ
+00012ef0: 7428 7365 6c66 3a20 4469 6d2c 206f 7468  t(self: Dim, oth
+00012f00: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
+00012f10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00012f20: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
+00012f30: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+00012f40: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
+00012f50: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
+00012f60: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
+00012f70: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
+00012f80: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
+00012f90: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
+00012fa0: 696e 643d 2263 6569 6c64 6976 222c 2072  ind="ceildiv", r
+00012fb0: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
+00012fc0: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
+00012fd0: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
+00012fe0: 205f 5f6e 6567 5f5f 2873 656c 6629 3a0a   __neg__(self):.
+00012ff0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013000: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
+00013010: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013020: 2020 2020 7265 7475 726e 202d 3120 2a20      return -1 * 
+00013030: 7365 6c66 0a0a 2020 2020 6465 6620 6973  self..    def is
+00013040: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+00013050: 5f64 696d 2873 656c 6629 202d 3e20 626f  _dim(self) -> bo
+00013060: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
+00013070: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00013080: 2064 6572 6976 6564 206f 7020 6f66 2074   derived op of t
+00013090: 7970 6520 636f 6e73 7461 6e74 0a20 2020  ype constant.   
+000130a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000130b0: 2072 6574 7572 6e20 7365 6c66 2e64 6572   return self.der
+000130c0: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
+000130d0: 2073 656c 662e 6465 7269 7665 645f 6672   self.derived_fr
+000130e0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2263  om_op.kind == "c
+000130f0: 6f6e 7374 616e 7422 0a0a 0a64 6566 205f  onstant"...def _
+00013100: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
+00013110: 6174 6963 5f64 696d 2876 616c 7565 2c20  atic_dim(value, 
+00013120: 6b69 6e64 3d4e 6f6e 6529 3a0a 2020 2020  kind=None):.    
+00013130: 2222 220a 2020 2020 3a70 6172 616d 2069  """.    :param i
+00013140: 6e74 2076 616c 7565 3a0a 2020 2020 3a70  nt value:.    :p
+00013150: 6172 616d 2045 6e74 6974 797c 4e6f 6e65  aram Entity|None
+00013160: 206b 696e 643a 0a20 2020 203a 7274 7970   kind:.    :rtyp
+00013170: 653a 2044 696d 0a20 2020 2022 2222 0a20  e: Dim.    """. 
+00013180: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
+00013190: 280a 2020 2020 2020 2020 6469 6d65 6e73  (.        dimens
+000131a0: 696f 6e3d 7661 6c75 652c 0a20 2020 2020  ion=value,.     
+000131b0: 2020 206b 696e 643d 6b69 6e64 206f 7220     kind=kind or 
+000131c0: 4469 6d54 7970 6573 2e55 6e73 7065 6369  DimTypes.Unspeci
+000131d0: 6669 6564 2c0a 2020 2020 2020 2020 6465  fied,.        de
+000131e0: 7363 7269 7074 696f 6e3d 2275 6e6e 616d  scription="unnam
+000131f0: 6564 5f25 7364 696d 5f25 6922 2025 2028  ed_%sdim_%i" % (
+00013200: 6b69 6e64 2e6e 616d 6520 2b20 225f 2220  kind.name + "_" 
+00013210: 6966 206b 696e 6420 656c 7365 2022 222c  if kind else "",
+00013220: 2076 616c 7565 292c 0a20 2020 2020 2020   value),.       
+00013230: 2064 6572 6976 6564 5f66 726f 6d5f 6f70   derived_from_op
+00013240: 3d4f 7028 6b69 6e64 3d22 636f 6e73 7461  =Op(kind="consta
+00013250: 6e74 222c 2069 6e70 7574 733d 5b5d 2c20  nt", inputs=[], 
+00013260: 6174 7472 6962 733d 7b22 7661 6c75 6522  attribs={"value"
+00013270: 3a20 7661 6c75 657d 292c 0a20 2020 2020  : value}),.     
+00013280: 2020 2061 7574 6f5f 6765 6e65 7261 7465     auto_generate
+00013290: 643d 5472 7565 2c0a 2020 2020 290a 0a0a  d=True,.    )...
+000132a0: 636c 6173 7320 4f70 3a0a 2020 2020 2222  class Op:.    ""
+000132b0: 220a 2020 2020 4f70 206f 6e20 3a63 6c61  ".    Op on :cla
+000132c0: 7373 3a60 4469 6d60 2077 6869 6368 2072  ss:`Dim` which r
+000132d0: 6573 756c 7473 2069 6e20 6120 6465 7269  esults in a deri
+000132e0: 7665 6420 3a63 6c61 7373 3a60 4469 6d60  ved :class:`Dim`
+000132f0: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+00013300: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00013310: 2c20 6b69 6e64 2c20 696e 7075 7473 2c20  , kind, inputs, 
+00013320: 6174 7472 6962 733d 4e6f 6e65 293a 0a20  attribs=None):. 
+00013330: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013340: 2020 203a 7061 7261 6d20 7374 7220 6b69     :param str ki
+00013350: 6e64 3a20 2261 6464 222c 2022 7375 6222  nd: "add", "sub"
+00013360: 2c20 226d 756c 222c 2022 6365 696c 6469  , "mul", "ceildi
+00013370: 7622 0a20 2020 2020 2020 203a 7061 7261  v".        :para
+00013380: 6d20 6c69 7374 5b44 696d 5d20 696e 7075  m list[Dim] inpu
+00013390: 7473 3a0a 2020 2020 2020 2020 3a70 6172  ts:.        :par
+000133a0: 616d 2064 6963 745b 7374 725d 7c4e 6f6e  am dict[str]|Non
+000133b0: 6520 6174 7472 6962 733a 0a20 2020 2020  e attribs:.     
+000133c0: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+000133d0: 656c 662e 6b69 6e64 203d 206b 696e 640a  elf.kind = kind.
+000133e0: 2020 2020 2020 2020 7365 6c66 2e69 6e70          self.inp
+000133f0: 7574 7320 3d20 696e 7075 7473 0a20 2020  uts = inputs.   
+00013400: 2020 2020 2073 656c 662e 6f75 7470 7574       self.output
+00013410: 203d 204e 6f6e 6520 2023 2074 7970 653a   = None  # type:
+00013420: 204f 7074 696f 6e61 6c5b 5f64 2e44 696d   Optional[_d.Dim
+00013430: 5d0a 2020 2020 2020 2020 7365 6c66 2e61  ].        self.a
+00013440: 7474 7269 6273 203d 2061 7474 7269 6273  ttribs = attribs
+00013450: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+00013460: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00013470: 2020 6174 7472 6962 7320 3d20 2822 2025    attribs = (" %
+00013480: 7222 2025 2073 656c 662e 6174 7472 6962  r" % self.attrib
+00013490: 7329 2069 6620 7365 6c66 2e61 7474 7269  s) if self.attri
+000134a0: 6273 2065 6c73 6520 2222 0a20 2020 2020  bs else "".     
+000134b0: 2020 2072 6574 7572 6e20 223c 4469 6d2e     return "<Dim.
+000134c0: 4f70 2025 7220 2573 2573 3e22 2025 2028  Op %r %s%s>" % (
+000134d0: 7365 6c66 2e6b 696e 642c 2073 656c 662e  self.kind, self.
+000134e0: 696e 7075 7473 2c20 6174 7472 6962 7329  inputs, attribs)
+000134f0: 0a0a 2020 2020 6465 6620 5f76 616c 7565  ..    def _value
+00013500: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00013510: 7265 7475 726e 2073 656c 662e 6b69 6e64  return self.kind
+00013520: 2c20 7475 706c 6528 7365 6c66 2e69 6e70  , tuple(self.inp
+00013530: 7574 7329 2c20 6672 6f7a 656e 7365 7428  uts), frozenset(
+00013540: 7365 6c66 2e61 7474 7269 6273 2e69 7465  self.attribs.ite
+00013550: 6d73 2829 2920 6966 2073 656c 662e 6174  ms()) if self.at
+00013560: 7472 6962 7320 656c 7365 204e 6f6e 650a  tribs else None.
+00013570: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
+00013580: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00013590: 2072 6574 7572 6e20 6861 7368 2873 656c   return hash(sel
+000135a0: 662e 5f76 616c 7565 2829 290a 0a20 2020  f._value())..   
+000135b0: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
+000135c0: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+000135d0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000135e0: 6f74 6865 722c 204f 7029 3a0a 2020 2020  other, Op):.    
+000135f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00013600: 656c 662e 5f76 616c 7565 2829 203d 3d20  elf._value() == 
+00013610: 6f74 6865 722e 5f76 616c 7565 2829 0a20  other._value(). 
+00013620: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00013630: 6c73 650a 0a20 2020 2064 6566 205f 5f6e  lse..    def __n
+00013640: 655f 5f28 7365 6c66 2c20 6f74 6865 7229  e__(self, other)
+00013650: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00013660: 206e 6f74 2073 656c 662e 5f5f 6571 5f5f   not self.__eq__
+00013670: 286f 7468 6572 290a 0a0a 6465 6620 5f67  (other)...def _g
+00013680: 6574 5f64 6573 6372 6970 7469 6f6e 2864  et_description(d
+00013690: 696d 2c20 6272 6163 6b65 7473 3d54 7275  im, brackets=Tru
+000136a0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+000136b0: 3a70 6172 616d 2044 696d 2064 696d 3a0a  :param Dim dim:.
+000136c0: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+000136d0: 6272 6163 6b65 7473 3a20 6164 6420 6272  brackets: add br
+000136e0: 6163 6b65 7473 2077 6865 6e20 6e65 6365  ackets when nece
+000136f0: 7373 6172 790a 2020 2020 3a72 7479 7065  ssary.    :rtype
+00013700: 3a20 7374 720a 2020 2020 2222 220a 2020  : str.    """.  
+00013710: 2020 6966 2064 696d 2e64 6573 6372 6970    if dim.descrip
+00013720: 7469 6f6e 2061 6e64 2064 696d 2e64 6573  tion and dim.des
+00013730: 6372 6970 7469 6f6e 2e73 7461 7274 7377  cription.startsw
+00013740: 6974 6828 2275 6e6e 616d 6564 5f22 2920  ith("unnamed_") 
+00013750: 616e 6420 6469 6d2e 6469 6d65 6e73 696f  and dim.dimensio
+00013760: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00013770: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+00013780: 7228 6469 6d2e 6469 6d65 6e73 696f 6e29  r(dim.dimension)
+00013790: 0a20 2020 2069 6620 6469 6d2e 6465 7363  .    if dim.desc
+000137a0: 7269 7074 696f 6e3a 0a20 2020 2020 2020  ription:.       
+000137b0: 2069 6620 6272 6163 6b65 7473 3a0a 2020   if brackets:.  
+000137c0: 2020 2020 2020 2020 2020 696d 706f 7274            import
+000137d0: 2072 650a 0a20 2020 2020 2020 2020 2020   re..           
+000137e0: 2069 6620 7265 2e73 6561 7263 6828 225b   if re.search("[
+000137f0: 2b5c 5c2d 2f20 5d22 2c20 6469 6d2e 6465  +\\-/ ]", dim.de
+00013800: 7363 7269 7074 696f 6e29 3a0a 2020 2020  scription):.    
+00013810: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013820: 726e 2022 2825 7329 2220 2520 6469 6d2e  rn "(%s)" % dim.
+00013830: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
+00013840: 2020 2020 7265 7475 726e 2064 696d 2e64      return dim.d
+00013850: 6573 6372 6970 7469 6f6e 0a20 2020 2072  escription.    r
+00013860: 6574 7572 6e20 2275 6e6e 616d 6564 5f25  eturn "unnamed_%
+00013870: 735f 6469 6d25 7322 2025 2028 6469 6d2e  s_dim%s" % (dim.
+00013880: 6b69 6e64 2c20 6469 6d2e 6469 6d65 6e73  kind, dim.dimens
+00013890: 696f 6e20 6966 2064 696d 2e64 696d 656e  ion if dim.dimen
+000138a0: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+000138b0: 2065 6c73 6520 223f 2229 0a0a 0a63 6c61   else "?")...cla
+000138c0: 7373 205f 4f70 4d75 6c74 5465 726d 3a0a  ss _OpMultTerm:.
+000138d0: 2020 2020 2222 220a 2020 2020 7265 7072      """.    repr
+000138e0: 6573 656e 7473 2073 7468 206c 696b 6520  esents sth like 
+000138f0: 6120 2a20 6220 2a20 630a 2020 2020 2222  a * b * c.    ""
+00013900: 220a 0a20 2020 2040 636c 6173 736d 6574  "..    @classmet
+00013910: 686f 640a 2020 2020 6465 6620 6672 6f6d  hod.    def from
+00013920: 5f64 696d 2863 6c73 2c20 6469 6d3a 205f  _dim(cls, dim: _
+00013930: 642e 4469 6d29 202d 3e20 5f4f 704d 756c  d.Dim) -> _OpMul
+00013940: 7454 6572 6d3a 0a20 2020 2020 2020 2022  tTerm:.        "
+00013950: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00013960: 6d20 6469 6d3a 0a20 2020 2020 2020 203a  m dim:.        :
+00013970: 7265 7475 726e 3a20 6f70 206d 756c 7420  return: op mult 
+00013980: 7465 726d 0a20 2020 2020 2020 2022 2222  term.        """
+00013990: 0a20 2020 2020 2020 2064 696d 203d 2064  .        dim = d
+000139a0: 696d 2e67 6574 5f73 616d 655f 6261 7365  im.get_same_base
+000139b0: 2829 0a20 2020 2020 2020 2069 6620 6469  ().        if di
+000139c0: 6d2e 6469 6d65 6e73 696f 6e20 3d3d 2031  m.dimension == 1
+000139d0: 2061 6e64 2064 696d 2e69 735f 636f 6e73   and dim.is_cons
+000139e0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
+000139f0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00013a00: 6574 7572 6e20 636c 732e 6f6e 6528 290a  eturn cls.one().
+00013a10: 2020 2020 2020 2020 6966 2064 696d 2e64          if dim.d
+00013a20: 6572 6976 6564 5f66 726f 6d5f 6f70 2061  erived_from_op a
+00013a30: 6e64 2064 696d 2e64 6572 6976 6564 5f66  nd dim.derived_f
+00013a40: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
+00013a50: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
+00013a60: 2020 7265 7475 726e 2063 6c73 286c 6973    return cls(lis
+00013a70: 7428 6469 6d2e 6465 7269 7665 645f 6672  t(dim.derived_fr
+00013a80: 6f6d 5f6f 702e 696e 7075 7473 2929 0a20  om_op.inputs)). 
+00013a90: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
+00013aa0: 7328 5b64 696d 5d29 0a0a 2020 2020 4063  s([dim])..    @c
+00013ab0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00013ac0: 6566 2066 726f 6d5f 6469 6d5f 6661 6374  ef from_dim_fact
+00013ad0: 6f72 7328 636c 732c 2064 696d 7329 3a0a  ors(cls, dims):.
+00013ae0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013af0: 2020 2020 3a70 6172 616d 206c 6973 745b      :param list[
+00013b00: 4469 6d5d 2064 696d 733a 0a20 2020 2020  Dim] dims:.     
+00013b10: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
+00013b20: 4f70 4d75 6c74 5465 726d 0a20 2020 2020  OpMultTerm.     
+00013b30: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00013b40: 6573 203d 2063 6c73 2e6f 6e65 2829 0a20  es = cls.one(). 
+00013b50: 2020 2020 2020 2066 6f72 2064 2069 6e20         for d in 
+00013b60: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
+00013b70: 2020 7265 732e 6578 7465 6e64 5f6d 756c    res.extend_mul
+00013b80: 5f64 6976 5f28 642c 206b 696e 643d 226d  _div_(d, kind="m
+00013b90: 756c 222c 2072 6967 6874 3d54 7275 6529  ul", right=True)
+00013ba0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013bb0: 7265 730a 0a20 2020 2040 636c 6173 736d  res..    @classm
+00013bc0: 6574 686f 640a 2020 2020 6465 6620 6f6e  ethod.    def on
+00013bd0: 6528 636c 7329 3a0a 2020 2020 2020 2020  e(cls):.        
+00013be0: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
+00013bf0: 7065 3a20 4469 6d2e 5f4f 704d 756c 7454  pe: Dim._OpMultT
+00013c00: 6572 6d0a 2020 2020 2020 2020 2222 220a  erm.        """.
+00013c10: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00013c20: 6c73 285b 5d29 0a0a 2020 2020 6465 6620  ls([])..    def 
+00013c30: 5f5f 696e 6974 5f5f 2873 656c 662c 2074  __init__(self, t
+00013c40: 6572 6d73 293a 0a20 2020 2020 2020 2022  erms):.        "
+00013c50: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00013c60: 6d20 6c69 7374 5b44 696d 5d20 7465 726d  m list[Dim] term
+00013c70: 733a 0a20 2020 2020 2020 2022 2222 0a20  s:.        """. 
+00013c80: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
+00013c90: 7320 3d20 7465 726d 730a 0a20 2020 2064  s = terms..    d
+00013ca0: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
+00013cb0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00013cc0: 6e20 6861 7368 2874 7570 6c65 2873 656c  n hash(tuple(sel
+00013cd0: 662e 7465 726d 7329 290a 0a20 2020 2064  f.terms))..    d
+00013ce0: 6566 205f 5f65 715f 5f28 7365 6c66 2c20  ef __eq__(self, 
+00013cf0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00013d00: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+00013d10: 616d 2044 696d 7c44 696d 2e5f 4f70 4d75  am Dim|Dim._OpMu
+00013d20: 6c74 5465 726d 206f 7468 6572 3a0a 2020  ltTerm other:.  
+00013d30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013d40: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00013d50: 6f74 6865 722c 205f 4f70 4d75 6c74 5465  other, _OpMultTe
+00013d60: 726d 293a 0a20 2020 2020 2020 2020 2020  rm):.           
+00013d70: 2072 6574 7572 6e20 7365 6c66 2e74 6572   return self.ter
+00013d80: 6d73 203d 3d20 6f74 6865 722e 7465 726d  ms == other.term
+00013d90: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+00013da0: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
+00013db0: 5f5f 6e65 5f5f 2873 656c 662c 206f 7468  __ne__(self, oth
+00013dc0: 6572 293a 0a20 2020 2020 2020 2072 6574  er):.        ret
+00013dd0: 7572 6e20 6e6f 7420 7365 6c66 2e5f 5f65  urn not self.__e
+00013de0: 715f 5f28 6f74 6865 7229 0a0a 2020 2020  q__(other)..    
+00013df0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+00013e00: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00013e10: 726e 2022 4469 6d2e 5f4f 704d 756c 7454  rn "Dim._OpMultT
+00013e20: 6572 6d28 2572 2922 2025 2028 7365 6c66  erm(%r)" % (self
+00013e30: 2e74 6572 6d73 2c29 0a0a 2020 2020 4070  .terms,)..    @p
+00013e40: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00013e50: 6469 6d65 6e73 696f 6e28 7365 6c66 293a  dimension(self):
+00013e60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013e70: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
+00013e80: 7c4e 6f6e 650a 2020 2020 2020 2020 2222  |None.        ""
+00013e90: 220a 2020 2020 2020 2020 6469 6d20 3d20  ".        dim = 
+00013ea0: 310a 2020 2020 2020 2020 666f 7220 7061  1.        for pa
+00013eb0: 7274 2069 6e20 7365 6c66 2e74 6572 6d73  rt in self.terms
+00013ec0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00013ed0: 2070 6172 742e 6469 6d65 6e73 696f 6e20   part.dimension 
+00013ee0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00013ef0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013f00: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00013f10: 2064 696d 202a 3d20 7061 7274 2e64 696d   dim *= part.dim
+00013f20: 656e 7369 6f6e 0a20 2020 2020 2020 2072  ension.        r
+00013f30: 6574 7572 6e20 6469 6d0a 0a20 2020 2064  eturn dim..    d
+00013f40: 6566 2062 6173 655f 7465 726d 2873 656c  ef base_term(sel
+00013f50: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00013f60: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00013f70: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
+00013f80: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+00013f90: 656c 662e 7465 726d 730a 2020 2020 2020  elf.terms.      
+00013fa0: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
+00013fb0: 726d 735b 2d31 5d0a 0a20 2020 2064 6566  rms[-1]..    def
+00013fc0: 2069 735f 6f6e 6528 7365 6c66 293a 0a20   is_one(self):. 
+00013fd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013fe0: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+00013ff0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014000: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+00014010: 656c 662e 7465 726d 730a 0a20 2020 2064  elf.terms..    d
+00014020: 6566 2069 735f 636f 6e73 7461 6e74 5f73  ef is_constant_s
+00014030: 7461 7469 635f 6469 6d28 7365 6c66 293a  tatic_dim(self):
+00014040: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014050: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00014060: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
+00014070: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00014080: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
+00014090: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+000140a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000140b0: 616c 6c28 7465 726d 2e69 735f 636f 6e73  all(term.is_cons
+000140c0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
+000140d0: 2920 666f 7220 7465 726d 2069 6e20 7365  ) for term in se
+000140e0: 6c66 2e74 6572 6d73 290a 0a20 2020 2064  lf.terms)..    d
+000140f0: 6566 2063 6f70 7928 7365 6c66 293a 0a20  ef copy(self):. 
+00014100: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014110: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
+00014120: 4f70 4d75 6c74 5465 726d 0a20 2020 2020  OpMultTerm.     
+00014130: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00014140: 6574 7572 6e20 5f4f 704d 756c 7454 6572  eturn _OpMultTer
+00014150: 6d28 6c69 7374 2873 656c 662e 7465 726d  m(list(self.term
+00014160: 7329 290a 0a20 2020 2064 6566 206e 6567  s))..    def neg
+00014170: 6174 6976 6528 7365 6c66 293a 0a20 2020  ative(self):.   
+00014180: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014190: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
+000141a0: 4d75 6c74 5465 726d 0a20 2020 2020 2020  MultTerm.       
+000141b0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+000141c0: 7365 6c66 2e74 6572 6d73 2061 6e64 2073  self.terms and s
+000141d0: 656c 662e 7465 726d 735b 305d 2e69 735f  elf.terms[0].is_
+000141e0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+000141f0: 6469 6d28 2920 616e 6420 7365 6c66 2e74  dim() and self.t
+00014200: 6572 6d73 5b30 5d2e 6469 6d65 6e73 696f  erms[0].dimensio
+00014210: 6e20 3d3d 202d 313a 0a20 2020 2020 2020  n == -1:.       
+00014220: 2020 2020 2072 6574 7572 6e20 5f4f 704d       return _OpM
+00014230: 756c 7454 6572 6d28 7365 6c66 2e74 6572  ultTerm(self.ter
+00014240: 6d73 5b31 3a5d 290a 2020 2020 2020 2020  ms[1:]).        
+00014250: 7265 7320 3d20 7365 6c66 2e63 6f70 7928  res = self.copy(
+00014260: 290a 2020 2020 2020 2020 7265 732e 6578  ).        res.ex
+00014270: 7465 6e64 5f6d 756c 5f64 6976 5f28 5f6d  tend_mul_div_(_m
+00014280: 616b 655f 636f 6e73 7461 6e74 5f73 7461  ake_constant_sta
+00014290: 7469 635f 6469 6d28 2d31 292c 206b 696e  tic_dim(-1), kin
+000142a0: 643d 226d 756c 222c 2072 6967 6874 3d46  d="mul", right=F
+000142b0: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
+000142c0: 7475 726e 2072 6573 0a0a 2020 2020 6465  turn res..    de
+000142d0: 6620 6469 7669 7369 626c 6528 7365 6c66  f divisible(self
+000142e0: 2c20 6f74 6865 722c 2072 6967 6874 293a  , other, right):
+000142f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014300: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
+00014310: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+00014320: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
+00014330: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
+00014340: 6e3a 2077 6865 7468 6572 2077 6520 6361  n: whether we ca
+00014350: 6e20 6469 7669 6465 206f 7468 6572 2c20  n divide other, 
+00014360: 7769 7468 6f75 7420 7265 6d61 696e 6465  without remainde
+00014370: 720a 2020 2020 2020 2020 3a72 7479 7065  r.        :rtype
+00014380: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
+00014390: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+000143a0: 7420 7365 6c66 2e74 6572 6d73 3a0a 2020  t self.terms:.  
+000143b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000143c0: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
+000143d0: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
+000143e0: 6672 6f6d 5f6f 7020 616e 6420 6f74 6865  from_op and othe
+000143f0: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00014400: 702e 6b69 6e64 203d 3d20 226d 756c 223a  p.kind == "mul":
+00014410: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
+00014420: 203d 2073 656c 662e 636f 7079 2829 0a20   = self.copy(). 
+00014430: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+00014440: 6572 6d20 696e 206f 7468 6572 2e64 6572  erm in other.der
+00014450: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
+00014460: 7574 7320 6966 2072 6967 6874 2065 6c73  uts if right els
+00014470: 6520 7265 7665 7273 6564 286f 7468 6572  e reversed(other
+00014480: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00014490: 2e69 6e70 7574 7329 3a0a 2020 2020 2020  .inputs):.      
+000144a0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000144b0: 2074 6d70 2e64 6976 6973 6962 6c65 2874   tmp.divisible(t
+000144c0: 6572 6d2c 2072 6967 6874 3d72 6967 6874  erm, right=right
+000144d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000144e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000144f0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00014500: 2020 2020 746d 702e 6578 7465 6e64 5f6d      tmp.extend_m
+00014510: 756c 5f64 6976 5f28 7465 726d 2c20 6b69  ul_div_(term, ki
+00014520: 6e64 3d22 7472 7565 6469 7622 2c20 7269  nd="truediv", ri
+00014530: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
+00014540: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00014550: 7565 0a20 2020 2020 2020 206d 6f73 745f  ue.        most_
+00014560: 7265 6365 6e74 5f74 6572 6d20 3d20 7365  recent_term = se
+00014570: 6c66 2e74 6572 6d73 5b2d 3120 6966 2072  lf.terms[-1 if r
+00014580: 6967 6874 2065 6c73 6520 305d 0a20 2020  ight else 0].   
+00014590: 2020 2020 2069 6620 6f74 6865 7220 3d3d       if other ==
+000145a0: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
+000145b0: 6d3a 0a20 2020 2020 2020 2020 2020 2072  m:.            r
+000145c0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+000145d0: 2020 2069 6620 6d6f 7374 5f72 6563 656e     if most_recen
+000145e0: 745f 7465 726d 2e64 696d 656e 7369 6f6e  t_term.dimension
+000145f0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00014600: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
+00014610: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00014620: 2020 2020 2020 2020 2020 6966 206d 6f73            if mos
+00014630: 745f 7265 6365 6e74 5f74 6572 6d2e 6469  t_recent_term.di
+00014640: 6d65 6e73 696f 6e20 2520 6f74 6865 722e  mension % other.
+00014650: 6469 6d65 6e73 696f 6e20 3d3d 2030 3a0a  dimension == 0:.
+00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014670: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
+00014680: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00014690: 0a0a 2020 2020 6465 6620 6361 6e5f 7369  ..    def can_si
+000146a0: 6d70 6c69 6679 2873 656c 662c 206f 7468  mplify(self, oth
+000146b0: 6572 2c20 6b69 6e64 2c20 7269 6768 7429  er, kind, right)
+000146c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000146d0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+000146e0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+000146f0: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
+00014700: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00014710: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
+00014720: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
+00014730: 7468 6572 2077 6520 6361 6e20 7369 6d70  ther we can simp
+00014740: 6c69 6679 2077 6865 6e20 6170 706c 7969  lify when applyi
+00014750: 6e67 2074 6869 7320 6f70 6572 6174 696f  ng this operatio
+00014760: 6e0a 2020 2020 2020 2020 3a72 7479 7065  n.        :rtype
+00014770: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
+00014780: 2222 0a20 2020 2020 2020 2069 6620 6f74  "".        if ot
+00014790: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+000147a0: 5f6f 7020 616e 6420 6f74 6865 722e 6465  _op and other.de
+000147b0: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
+000147c0: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
+000147d0: 2020 2020 2020 2020 2074 6d70 203d 2073           tmp = s
+000147e0: 656c 662e 636f 7079 2829 0a20 2020 2020  elf.copy().     
+000147f0: 2020 2020 2020 2066 6f72 2074 6572 6d20         for term 
+00014800: 696e 206f 7468 6572 2e64 6572 6976 6564  in other.derived
+00014810: 5f66 726f 6d5f 6f70 2e69 6e70 7574 7320  _from_op.inputs 
+00014820: 6966 2072 6967 6874 2065 6c73 6520 7265  if right else re
+00014830: 7665 7273 6564 286f 7468 6572 2e64 6572  versed(other.der
+00014840: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
+00014850: 7574 7329 3a0a 2020 2020 2020 2020 2020  uts):.          
+00014860: 2020 2020 2020 6966 206e 6f74 2074 6d70        if not tmp
+00014870: 2e63 616e 5f73 696d 706c 6966 7928 7465  .can_simplify(te
+00014880: 726d 2c20 6b69 6e64 3d6b 696e 642c 2072  rm, kind=kind, r
+00014890: 6967 6874 3d72 6967 6874 293a 0a20 2020  ight=right):.   
+000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148b0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+000148c0: 2020 2020 2020 2020 2020 2020 2020 746d                tm
+000148d0: 702e 6578 7465 6e64 5f6d 756c 5f64 6976  p.extend_mul_div
+000148e0: 5f28 7465 726d 2c20 6b69 6e64 3d6b 696e  _(term, kind=kin
+000148f0: 642c 2072 6967 6874 3d72 6967 6874 290a  d, right=right).
+00014900: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014910: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+00014920: 6964 7820 3d20 7365 6c66 2e5f 7369 6d70  idx = self._simp
+00014930: 6c69 6679 5f74 6572 6d5f 6964 7828 6f74  lify_term_idx(ot
+00014940: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
+00014950: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
+00014960: 2020 2020 2072 6574 7572 6e20 6964 7820       return idx 
+00014970: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
+00014980: 2064 6566 205f 7369 6d70 6c69 6679 5f74   def _simplify_t
+00014990: 6572 6d5f 6964 7828 7365 6c66 2c20 6f74  erm_idx(self, ot
+000149a0: 6865 722c 206b 696e 642c 2072 6967 6874  her, kind, right
+000149b0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000149c0: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+000149d0: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
+000149e0: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
+000149f0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00014a00: 2062 6f6f 6c20 7269 6768 743a 0a20 2020   bool right:.   
+00014a10: 2020 2020 203a 7265 7475 726e 3a20 696e       :return: in
+00014a20: 6465 7820 6f66 2074 6572 6d20 746f 2073  dex of term to s
+00014a30: 696d 706c 6966 790a 2020 2020 2020 2020  implify.        
+00014a40: 3a72 7479 7065 3a20 696e 747c 4e6f 6e65  :rtype: int|None
+00014a50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014a60: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00014a70: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00014a80: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00014a90: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
+00014aa0: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
+00014ab0: 2020 2020 2020 2320 5765 2077 616e 7420        # We want 
+00014ac0: 2862 202a 2061 2920 2f2f 2062 2021 3d20  (b * a) // b != 
+00014ad0: 612e 0a20 2020 2020 2020 2020 2020 2023  a..            #
+00014ae0: 2048 6f77 6576 6572 2c20 7765 2077 616e   However, we wan
+00014af0: 7420 6820 2a20 2832 202a 2061 202f 2f20  t h * (2 * a // 
+00014b00: 6829 203d 3d20 3220 2a20 612e 0a20 2020  h) == 2 * a..   
+00014b10: 2020 2020 2020 2020 2023 2053 6f2c 2066           # So, f
+00014b20: 6f72 2060 6d75 6c60 2c20 616e 6420 6f6e  or `mul`, and on
+00014b30: 6c79 2066 6f72 2060 6d75 6c60 2c20 6368  ly for `mul`, ch
+00014b40: 6563 6b20 616c 6c20 7465 726d 732c 2077  eck all terms, w
+00014b50: 6865 7468 6572 2077 6520 6361 6e20 7369  hether we can si
+00014b60: 6d70 6c69 6679 2073 6f6d 6520 6469 7669  mplify some divi
+00014b70: 7369 6f6e 2d74 6572 6d2e 0a20 2020 2020  sion-term..     
+00014b80: 2020 2020 2020 2066 6f72 2069 2c20 7465         for i, te
+00014b90: 726d 2069 6e20 7265 7665 7273 6564 286c  rm in reversed(l
+00014ba0: 6973 7428 656e 756d 6572 6174 6528 7365  ist(enumerate(se
+00014bb0: 6c66 2e74 6572 6d73 2929 2920 6966 2072  lf.terms))) if r
+00014bc0: 6967 6874 2065 6c73 6520 656e 756d 6572  ight else enumer
+00014bd0: 6174 6528 7365 6c66 2e74 6572 6d73 293a  ate(self.terms):
+00014be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014bf0: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
+00014c00: 6365 2874 6572 6d2c 205f 642e 4469 6d29  ce(term, _d.Dim)
+00014c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c20: 2069 6620 7465 726d 2e64 6572 6976 6564   if term.derived
+00014c30: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
+00014c40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014c50: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
+00014c60: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
+00014c70: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
+00014c80: 6874 2220 6966 2072 6967 6874 2065 6c73  ht" if right els
+00014c90: 6520 226c 6566 7422 293a 0a20 2020 2020  e "left"):.     
+00014ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cb0: 2020 2069 6620 7465 726d 2e64 6572 6976     if term.deriv
+00014cc0: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
+00014cd0: 735b 2d31 5d20 3d3d 206f 7468 6572 3a0a  s[-1] == other:.
+00014ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014d00: 726e 2069 0a20 2020 2020 2020 2020 2020  rn i.           
+00014d10: 2020 2020 2069 6620 6f74 6865 722e 6465       if other.de
+00014d20: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
+00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d40: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
+00014d50: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+00014d60: 203d 3d20 2274 7275 6564 6976 5f22 202b   == "truediv_" +
+00014d70: 2028 2272 6967 6874 2220 6966 206e 6f74   ("right" if not
+00014d80: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
+00014d90: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
+00014da0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014db0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00014dc0: 6f6d 5f6f 702e 696e 7075 7473 5b2d 315d  om_op.inputs[-1]
+00014dd0: 203d 3d20 7465 726d 3a0a 2020 2020 2020   == term:.      
+00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014df0: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
+00014e00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014e10: 6620 7465 726d 2e69 735f 636f 6e73 7461  f term.is_consta
+00014e20: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
+00014e30: 616e 6420 6f74 6865 722e 6973 5f63 6f6e  and other.is_con
+00014e40: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
+00014e50: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014e60: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00014e70: 0a20 2020 2020 2020 2023 2046 6f72 2074  .        # For t
+00014e80: 6865 206c 6173 742f 6669 7273 7420 7465  he last/first te
+00014e90: 726d 2c20 6578 7472 6120 6368 6563 6b73  rm, extra checks
+00014ea0: 2e0a 2020 2020 2020 2020 6920 3d20 6c65  ..        i = le
+00014eb0: 6e28 7365 6c66 2e74 6572 6d73 2920 2d20  n(self.terms) - 
+00014ec0: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
+00014ed0: 300a 2020 2020 2020 2020 7465 726d 203d  0.        term =
+00014ee0: 2073 656c 662e 7465 726d 735b 695d 0a20   self.terms[i]. 
+00014ef0: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
+00014f00: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
+00014f10: 6e64 206f 7468 6572 203d 3d20 7465 726d  nd other == term
+00014f20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00014f30: 7475 726e 2069 0a20 2020 2020 2020 206f  turn i.        o
+00014f40: 705f 6b69 6e64 203d 206b 696e 6420 2b20  p_kind = kind + 
+00014f50: 225f 2220 2b20 2822 7269 6768 7422 2069  "_" + ("right" i
+00014f60: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
+00014f70: 6674 2229 0a20 2020 2020 2020 2069 6620  ft").        if 
+00014f80: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
+00014f90: 6d5f 6f70 2061 6e64 2074 6572 6d2e 6465  m_op and term.de
+00014fa0: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
+00014fb0: 6e64 203d 3d20 6f70 5f6b 696e 643a 0a20  nd == op_kind:. 
+00014fc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00014fd0: 6e20 690a 2020 2020 2020 2020 7265 7475  n i.        retu
+00014fe0: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
+00014ff0: 2065 7874 656e 645f 6d75 6c5f 6469 765f   extend_mul_div_
+00015000: 2873 656c 662c 206f 7468 6572 2c20 6b69  (self, other, ki
+00015010: 6e64 2c20 7269 6768 7429 3a0a 2020 2020  nd, right):.    
+00015020: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00015030: 3a70 6172 616d 2044 696d 206f 7468 6572  :param Dim other
+00015040: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00015050: 2073 7472 206b 696e 643a 0a20 2020 2020   str kind:.     
+00015060: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
+00015070: 6967 6874 3a0a 2020 2020 2020 2020 2222  ight:.        ""
+00015080: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
+00015090: 206b 696e 6420 696e 207b 226d 756c 222c   kind in {"mul",
+000150a0: 2022 666c 6f6f 7264 6976 222c 2022 7472   "floordiv", "tr
+000150b0: 7565 6469 7622 2c20 2263 6569 6c64 6976  uediv", "ceildiv
+000150c0: 227d 0a20 2020 2020 2020 2069 6620 6f74  "}.        if ot
+000150d0: 6865 722e 6973 5f63 6f6e 7374 616e 745f  her.is_constant_
+000150e0: 7374 6174 6963 5f64 696d 2829 2061 6e64  static_dim() and
+000150f0: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
+00015100: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+00015110: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00015120: 2020 6966 206e 6f74 2073 656c 662e 7465    if not self.te
+00015130: 726d 733a 0a20 2020 2020 2020 2020 2020  rms:.           
+00015140: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
+00015150: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00015160: 2020 2073 656c 662e 7465 726d 732e 6170     self.terms.ap
+00015170: 7065 6e64 286f 7468 6572 290a 2020 2020  pend(other).    
+00015180: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
+00015190: 642e 656e 6473 7769 7468 2822 6469 7622  d.endswith("div"
+000151a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000151b0: 2020 2073 656c 662e 7465 726d 7320 3d20     self.terms = 
+000151c0: 5b5f 4f70 4d75 6c74 5465 726d 2e6e 6577  [_OpMultTerm.new
+000151d0: 5f64 6976 5f64 696d 2873 656c 662e 6173  _div_dim(self.as
+000151e0: 5f64 696d 2829 2c20 6f74 6865 722c 206b  _dim(), other, k
+000151f0: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
+00015200: 7269 6768 7429 5d0a 2020 2020 2020 2020  right)].        
+00015210: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00015220: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
+00015230: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
+00015240: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00015250: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 226d  om_op.kind == "m
+00015260: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
+00015270: 2066 6f72 2074 6572 6d20 696e 206f 7468   for term in oth
+00015280: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
+00015290: 6f70 2e69 6e70 7574 7320 6966 2072 6967  op.inputs if rig
+000152a0: 6874 2065 6c73 6520 7265 7665 7273 6564  ht else reversed
+000152b0: 286f 7468 6572 2e64 6572 6976 6564 5f66  (other.derived_f
+000152c0: 726f 6d5f 6f70 2e69 6e70 7574 7329 3a0a  rom_op.inputs):.
+000152d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152e0: 7365 6c66 2e65 7874 656e 645f 6d75 6c5f  self.extend_mul_
+000152f0: 6469 765f 2874 6572 6d2c 206b 696e 643d  div_(term, kind=
+00015300: 6b69 6e64 2c20 7269 6768 743d 7269 6768  kind, right=righ
+00015310: 7429 0a20 2020 2020 2020 2020 2020 2072  t).            r
+00015320: 6574 7572 6e0a 2020 2020 2020 2020 6964  eturn.        id
+00015330: 7820 3d20 7365 6c66 2e5f 7369 6d70 6c69  x = self._simpli
+00015340: 6679 5f74 6572 6d5f 6964 7828 6f74 6865  fy_term_idx(othe
+00015350: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
+00015360: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
+00015370: 2020 2069 6620 6964 7820 6973 206e 6f74     if idx is not
+00015380: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00015390: 2020 2074 6572 6d20 3d20 7365 6c66 2e74     term = self.t
+000153a0: 6572 6d73 5b69 6478 5d0a 2020 2020 2020  erms[idx].      
+000153b0: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+000153c0: 6e73 7461 6e63 6528 7465 726d 2c20 5f64  nstance(term, _d
+000153d0: 2e44 696d 290a 2020 2020 2020 2020 2020  .Dim).          
+000153e0: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
+000153f0: 7468 2822 6469 7622 2920 616e 6420 6f74  th("div") and ot
+00015400: 6865 7220 3d3d 2074 6572 6d3a 0a20 2020  her == term:.   
+00015410: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015420: 662e 7465 726d 732e 706f 7028 6964 7829  f.terms.pop(idx)
+00015430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015440: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00015450: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
+00015460: 6d75 6c22 2061 6e64 2074 6572 6d2e 6465  mul" and term.de
+00015470: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
+00015480: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015490: 6620 7465 726d 2e64 6572 6976 6564 5f66  f term.derived_f
+000154a0: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
+000154b0: 7472 7565 6469 765f 2220 2b20 2822 7269  truediv_" + ("ri
+000154c0: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
+000154d0: 7365 2022 6c65 6674 2229 3a0a 2020 2020  se "left"):.    
+000154e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154f0: 6966 2074 6572 6d2e 6465 7269 7665 645f  if term.derived_
+00015500: 6672 6f6d 5f6f 702e 696e 7075 7473 5b2d  from_op.inputs[-
+00015510: 315d 203d 3d20 6f74 6865 723a 0a20 2020  1] == other:.   
+00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015530: 2020 2020 2073 656c 662e 7465 726d 735b       self.terms[
+00015540: 6964 785d 203d 2074 6572 6d2e 6465 7269  idx] = term.deri
+00015550: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
+00015560: 7473 5b30 5d0a 2020 2020 2020 2020 2020  ts[0].          
+00015570: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00015580: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00015590: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
+000155a0: 2220 616e 6420 6f74 6865 722e 6465 7269  " and other.deri
+000155b0: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
+000155c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000155d0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+000155e0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
+000155f0: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
+00015600: 6874 2220 6966 206e 6f74 2072 6967 6874  ht" if not right
+00015610: 2065 6c73 6520 226c 6566 7422 293a 0a20   else "left"):. 
+00015620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015630: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
+00015640: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
+00015650: 7473 5b2d 315d 203d 3d20 7465 726d 3a0a  ts[-1] == term:.
+00015660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015670: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
+00015680: 6d73 5b69 6478 5d20 3d20 6f74 6865 722e  ms[idx] = other.
+00015690: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+000156a0: 696e 7075 7473 5b30 5d0a 2020 2020 2020  inputs[0].      
+000156b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156c0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+000156d0: 2020 2020 2069 6620 7465 726d 2e69 735f       if term.is_
+000156e0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+000156f0: 6469 6d28 2920 616e 6420 6f74 6865 722e  dim() and other.
+00015700: 6973 5f63 6f6e 7374 616e 745f 7374 6174  is_constant_stat
+00015710: 6963 5f64 696d 2829 3a0a 2020 2020 2020  ic_dim():.      
+00015720: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
+00015730: 6420 3d3d 2022 6d75 6c22 3a0a 2020 2020  d == "mul":.    
+00015740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015750: 6966 2074 6572 6d2e 6469 6d65 6e73 696f  if term.dimensio
+00015760: 6e20 2a20 6f74 6865 722e 6469 6d65 6e73  n * other.dimens
+00015770: 696f 6e20 3d3d 2031 3a0a 2020 2020 2020  ion == 1:.      
+00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015790: 2020 7365 6c66 2e74 6572 6d73 2e70 6f70    self.terms.pop
+000157a0: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
+000157b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000157c0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+000157d0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+000157e0: 726d 735b 6964 785d 203d 205f 6d61 6b65  rms[idx] = _make
+000157f0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+00015800: 5f64 696d 2874 6572 6d2e 6469 6d65 6e73  _dim(term.dimens
+00015810: 696f 6e20 2a20 6f74 6865 722e 6469 6d65  ion * other.dime
+00015820: 6e73 696f 6e2c 206b 696e 643d 7465 726d  nsion, kind=term
+00015830: 2e6b 696e 6429 0a20 2020 2020 2020 2020  .kind).         
+00015840: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00015850: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00015860: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
+00015870: 7468 2822 6469 7622 2920 616e 6420 7465  th("div") and te
+00015880: 726d 2e64 696d 656e 7369 6f6e 2025 206f  rm.dimension % o
+00015890: 7468 6572 2e64 696d 656e 7369 6f6e 203d  ther.dimension =
+000158a0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+000158b0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+000158c0: 726d 735b 6964 785d 203d 205f 6d61 6b65  rms[idx] = _make
+000158d0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+000158e0: 5f64 696d 2874 6572 6d2e 6469 6d65 6e73  _dim(term.dimens
+000158f0: 696f 6e20 2f2f 206f 7468 6572 2e64 696d  ion // other.dim
+00015900: 656e 7369 6f6e 2c20 6b69 6e64 3d74 6572  ension, kind=ter
+00015910: 6d2e 6b69 6e64 290a 2020 2020 2020 2020  m.kind).        
+00015920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015930: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
+00015940: 2020 2023 2046 616c 6c62 6163 6b20 7769     # Fallback wi
+00015950: 7468 2067 656e 6572 6963 2068 616e 646c  th generic handl
+00015960: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
+00015970: 206f 705f 6b69 6e64 203d 206b 696e 6420   op_kind = kind 
+00015980: 2b20 225f 2220 2b20 2822 7269 6768 7422  + "_" + ("right"
+00015990: 2069 6620 7269 6768 7420 656c 7365 2022   if right else "
+000159a0: 6c65 6674 2229 0a20 2020 2020 2020 2020  left").         
+000159b0: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
+000159c0: 6974 6828 2264 6976 2229 2061 6e64 2074  ith("div") and t
+000159d0: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
+000159e0: 5f6f 7020 616e 6420 7465 726d 2e64 6572  _op and term.der
+000159f0: 6976 6564 5f66 726f 6d5f 6f70 2e6b 696e  ived_from_op.kin
+00015a00: 6420 3d3d 206f 705f 6b69 6e64 3a0a 2020  d == op_kind:.  
+00015a10: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00015a20: 6d65 7261 746f 7220 3d20 7465 726d 2e64  merator = term.d
+00015a30: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
+00015a40: 6e70 7574 735b 305d 0a20 2020 2020 2020  nputs[0].       
+00015a50: 2020 2020 2020 2020 2064 656e 6f6d 696e           denomin
+00015a60: 6174 6f72 203d 2074 6572 6d2e 6465 7269  ator = term.deri
+00015a70: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
+00015a80: 7473 5b31 5d0a 2020 2020 2020 2020 2020  ts[1].          
+00015a90: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
+00015aa0: 5b69 6478 5d20 3d20 5f4f 704d 756c 7454  [idx] = _OpMultT
+00015ab0: 6572 6d2e 6e65 775f 6469 765f 6469 6d28  erm.new_div_dim(
+00015ac0: 6e75 6d65 7261 746f 722c 2064 656e 6f6d  numerator, denom
+00015ad0: 696e 6174 6f72 202a 206f 7468 6572 2c20  inator * other, 
+00015ae0: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
+00015af0: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
+00015b00: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00015b10: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
+00015b20: 6e64 7377 6974 6828 2264 6976 2229 3a0a  ndswith("div"):.
+00015b30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015b40: 2e74 6572 6d73 203d 205b 5f4f 704d 756c  .terms = [_OpMul
+00015b50: 7454 6572 6d2e 6e65 775f 6469 765f 6469  tTerm.new_div_di
+00015b60: 6d28 7365 6c66 2e61 735f 6469 6d28 292c  m(self.as_dim(),
+00015b70: 206f 7468 6572 2c20 6b69 6e64 3d6b 696e   other, kind=kin
+00015b80: 642c 2072 6967 6874 3d72 6967 6874 295d  d, right=right)]
+00015b90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015ba0: 7572 6e0a 2020 2020 2020 2020 6966 206b  urn.        if k
+00015bb0: 696e 6420 3d3d 2022 6d75 6c22 3a0a 2020  ind == "mul":.  
+00015bc0: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
+00015bd0: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
+00015be0: 2020 2020 7365 6c66 2e74 6572 6d73 2e61      self.terms.a
+00015bf0: 7070 656e 6428 6f74 6865 7229 0a20 2020  ppend(other).   
+00015c00: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00015c10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015c20: 656c 662e 7465 726d 732e 696e 7365 7274  elf.terms.insert
+00015c30: 2830 2c20 6f74 6865 7229 0a20 2020 2020  (0, other).     
+00015c40: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00015c50: 2020 2020 2020 6173 7365 7274 2046 616c        assert Fal
+00015c60: 7365 0a0a 2020 2020 4063 6c61 7373 6d65  se..    @classme
+00015c70: 7468 6f64 0a20 2020 2064 6566 206e 6577  thod.    def new
+00015c80: 5f64 6976 5f64 696d 2863 6c73 2c20 6e75  _div_dim(cls, nu
+00015c90: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
+00015ca0: 6174 6f72 2c20 6b69 6e64 2c20 7269 6768  ator, kind, righ
+00015cb0: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
+00015cc0: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
+00015cd0: 696d 206e 756d 6572 6174 6f72 3a0a 2020  im numerator:.  
+00015ce0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00015cf0: 2064 656e 6f6d 696e 6174 6f72 3a0a 2020   denominator:.  
+00015d00: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+00015d10: 206b 696e 643a 2022 666c 6f6f 7264 6976   kind: "floordiv
+00015d20: 2220 6f72 2022 6365 696c 6469 7622 206f  " or "ceildiv" o
+00015d30: 7220 2274 7275 6564 6976 220a 2020 2020  r "truediv".    
+00015d40: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+00015d50: 7269 6768 743a 0a20 2020 2020 2020 203a  right:.        :
+00015d60: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
+00015d70: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
+00015d80: 696d 5f76 616c 7565 203d 204e 6f6e 650a  im_value = None.
+00015d90: 2020 2020 2020 2020 6120 3d20 6e75 6d65          a = nume
+00015da0: 7261 746f 722e 6469 6d65 6e73 696f 6e0a  rator.dimension.
+00015db0: 2020 2020 2020 2020 6220 3d20 6465 6e6f          b = deno
+00015dc0: 6d69 6e61 746f 722e 6469 6d65 6e73 696f  minator.dimensio
+00015dd0: 6e0a 2020 2020 2020 2020 6966 2061 2069  n.        if a i
+00015de0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2062  s not None and b
+00015df0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00015e00: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
+00015e10: 6420 3d3d 2022 666c 6f6f 7264 6976 223a  d == "floordiv":
+00015e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e30: 2064 696d 5f76 616c 7565 203d 2061 202f   dim_value = a /
+00015e40: 2f20 620a 2020 2020 2020 2020 2020 2020  / b.            
+00015e50: 656c 6966 206b 696e 6420 3d3d 2022 6365  elif kind == "ce
+00015e60: 696c 6469 7622 3a0a 2020 2020 2020 2020  ildiv":.        
+00015e70: 2020 2020 2020 2020 6469 6d5f 7661 6c75          dim_valu
+00015e80: 6520 3d20 2d28 2d61 202f 2f20 6229 0a20  e = -(-a // b). 
+00015e90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015ea0: 6620 6120 2520 6220 3d3d 2030 2061 6e64  f a % b == 0 and
+00015eb0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
+00015ec0: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
+00015ed0: 203d 2022 666c 6f6f 7264 6976 2220 2023   = "floordiv"  #
+00015ee0: 2066 6f72 206e 6963 6572 2064 6573 6372   for nicer descr
+00015ef0: 6970 7469 6f6e 2c20 616e 6420 646f 6573  iption, and does
+00015f00: 206e 6f74 206d 6174 7465 720a 2020 2020   not matter.    
+00015f10: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
+00015f20: 6420 3d3d 2022 7472 7565 6469 7622 3a0a  d == "truediv":.
+00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f40: 6966 2061 2025 2062 2021 3d20 303a 0a20  if a % b != 0:. 
+00015f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f60: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00015f70: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00015f80: 2020 2020 2020 2020 2020 2020 2022 2573               "%s
+00015f90: 2074 7275 6564 6976 2025 7320 6f6e 6c79   truediv %s only
+00015fa0: 2061 6c6c 6f77 6564 2069 6620 7468 6520   allowed if the 
+00015fb0: 7265 7375 6c74 2069 7320 616e 2069 6e74  result is an int
+00015fc0: 6567 6572 2220 2520 286e 756d 6572 6174  eger" % (numerat
+00015fd0: 6f72 2c20 6465 6e6f 6d69 6e61 746f 7229  or, denominator)
+00015fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015ff0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00016000: 2020 2020 2020 2064 696d 5f76 616c 7565         dim_value
+00016010: 203d 2061 202f 2f20 620a 2020 2020 2020   = a // b.      
+00016020: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
+00016030: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
+00016040: 2020 2020 2020 2020 6b69 6e64 203d 2022          kind = "
+00016050: 666c 6f6f 7264 6976 2220 2023 2066 6f72  floordiv"  # for
+00016060: 206e 6963 6572 2064 6573 6372 6970 7469   nicer descripti
+00016070: 6f6e 2c20 616e 6420 646f 6573 206e 6f74  on, and does not
+00016080: 206d 6174 7465 720a 2020 2020 2020 2020   matter.        
+00016090: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000160a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000160b0: 5661 6c75 6545 7272 6f72 2822 696e 7661  ValueError("inva
+000160c0: 6c69 6420 6b69 6e64 2025 7222 2025 2028  lid kind %r" % (
+000160d0: 6b69 6e64 2c29 290a 2020 2020 2020 2020  kind,)).        
+000160e0: 6966 206b 696e 6420 3d3d 2022 666c 6f6f  if kind == "floo
+000160f0: 7264 6976 2220 616e 6420 7269 6768 743a  rdiv" and right:
+00016100: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00016110: 6372 6970 7469 6f6e 203d 2022 2573 2f2f  cription = "%s//
+00016120: 2573 2220 2520 285f 6765 745f 6465 7363  %s" % (_get_desc
+00016130: 7269 7074 696f 6e28 6e75 6d65 7261 746f  ription(numerato
+00016140: 7229 2c20 5f67 6574 5f64 6573 6372 6970  r), _get_descrip
+00016150: 7469 6f6e 2864 656e 6f6d 696e 6174 6f72  tion(denominator
+00016160: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
+00016170: 6b69 6e64 203d 3d20 2263 6569 6c64 6976  kind == "ceildiv
+00016180: 2220 616e 6420 7269 6768 743a 0a20 2020  " and right:.   
+00016190: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+000161a0: 7469 6f6e 203d 2022 e28c 8825 732f 2573  tion = "...%s/%s
+000161b0: e28c 8922 2025 2028 5f67 6574 5f64 6573  ..." % (_get_des
+000161c0: 6372 6970 7469 6f6e 286e 756d 6572 6174  cription(numerat
+000161d0: 6f72 292c 205f 6765 745f 6465 7363 7269  or), _get_descri
+000161e0: 7074 696f 6e28 6465 6e6f 6d69 6e61 746f  ption(denominato
+000161f0: 7229 290a 2020 2020 2020 2020 656c 7365  r)).        else
+00016200: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+00016210: 7363 7269 7074 696f 6e20 3d20 2225 735f  scription = "%s_
+00016220: 2573 2825 732c 2025 7329 2220 2520 280a  %s(%s, %s)" % (.
+00016230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016240: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
+00016250: 2020 2020 2020 2272 6967 6874 2220 6966        "right" if
+00016260: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
+00016270: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00016280: 2020 2020 5f67 6574 5f64 6573 6372 6970      _get_descrip
+00016290: 7469 6f6e 286e 756d 6572 6174 6f72 2c20  tion(numerator, 
+000162a0: 6272 6163 6b65 7473 3d46 616c 7365 292c  brackets=False),
+000162b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000162c0: 205f 6765 745f 6465 7363 7269 7074 696f   _get_descriptio
+000162d0: 6e28 6465 6e6f 6d69 6e61 746f 722c 2062  n(denominator, b
+000162e0: 7261 636b 6574 733d 4661 6c73 6529 2c0a  rackets=False),.
+000162f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00016300: 2020 2020 2020 6f70 5f6b 696e 6420 3d20        op_kind = 
+00016310: 6b69 6e64 0a20 2020 2020 2020 2069 6620  kind.        if 
+00016320: 6120 6973 206e 6f74 204e 6f6e 6520 616e  a is not None an
+00016330: 6420 6220 6973 206e 6f74 204e 6f6e 6520  d b is not None 
+00016340: 616e 6420 6120 2520 6220 3d3d 2030 3a0a  and a % b == 0:.
+00016350: 2020 2020 2020 2020 2020 2020 6f70 5f6b              op_k
+00016360: 696e 6420 3d20 2274 7275 6564 6976 2220  ind = "truediv" 
+00016370: 2023 206d 616b 6573 2073 6f6d 6520 6f74   # makes some ot
+00016380: 6865 7220 6368 6563 6b73 2073 696d 706c  her checks simpl
+00016390: 6572 0a20 2020 2020 2020 206f 705f 6b69  er.        op_ki
+000163a0: 6e64 202b 3d20 225f 2220 2b20 2822 7269  nd += "_" + ("ri
+000163b0: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
+000163c0: 7365 2022 6c65 6674 2229 0a20 2020 2020  se "left").     
+000163d0: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
+000163e0: 280a 2020 2020 2020 2020 2020 2020 6465  (.            de
+000163f0: 7363 7269 7074 696f 6e3d 6465 7363 7269  scription=descri
+00016400: 7074 696f 6e2c 0a20 2020 2020 2020 2020  ption,.         
+00016410: 2020 206b 696e 643d 6e75 6d65 7261 746f     kind=numerato
+00016420: 722e 6b69 6e64 2c0a 2020 2020 2020 2020  r.kind,.        
+00016430: 2020 2020 6469 6d65 6e73 696f 6e3d 6469      dimension=di
+00016440: 6d5f 7661 6c75 652c 0a20 2020 2020 2020  m_value,.       
+00016450: 2020 2020 2064 6572 6976 6564 5f66 726f       derived_fro
+00016460: 6d5f 6f70 3d4f 7028 6b69 6e64 3d6f 705f  m_op=Op(kind=op_
+00016470: 6b69 6e64 2c20 696e 7075 7473 3d5b 6e75  kind, inputs=[nu
+00016480: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
+00016490: 6174 6f72 5d29 2c0a 2020 2020 2020 2020  ator]),.        
+000164a0: 2020 2020 6465 7269 7665 645f 6672 6f6d      derived_from
+000164b0: 5f74 6167 3d6e 756d 6572 6174 6f72 2c0a  _tag=numerator,.
+000164c0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+000164d0: 6566 2061 735f 6469 6d28 7365 6c66 293a  ef as_dim(self):
+000164e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000164f0: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00016500: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016510: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+00016520: 6f6e 6528 293a 0a20 2020 2020 2020 2020  one():.         
+00016530: 2020 2072 6574 7572 6e20 5f6d 616b 655f     return _make_
+00016540: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+00016550: 6469 6d28 3129 0a20 2020 2020 2020 2069  dim(1).        i
+00016560: 6620 6c65 6e28 7365 6c66 2e74 6572 6d73  f len(self.terms
+00016570: 2920 3d3d 2031 3a0a 2020 2020 2020 2020  ) == 1:.        
+00016580: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00016590: 7465 726d 735b 305d 0a20 2020 2020 2020  terms[0].       
+000165a0: 2064 696d 5f6b 696e 6420 3d20 5f67 6574   dim_kind = _get
+000165b0: 5f6d 6572 6765 645f 6469 6d5f 6b69 6e64  _merged_dim_kind
+000165c0: 2873 656c 662e 7465 726d 7329 0a20 2020  (self.terms).   
+000165d0: 2020 2020 2072 6574 7572 6e20 5f64 2e44       return _d.D
+000165e0: 696d 280a 2020 2020 2020 2020 2020 2020  im(.            
+000165f0: 6b69 6e64 3d64 696d 5f6b 696e 642c 0a20  kind=dim_kind,. 
+00016600: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00016610: 6970 7469 6f6e 3d22 2a22 2e6a 6f69 6e28  iption="*".join(
+00016620: 6d61 7028 5f67 6574 5f64 6573 6372 6970  map(_get_descrip
+00016630: 7469 6f6e 2c20 7365 6c66 2e74 6572 6d73  tion, self.terms
+00016640: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00016650: 6469 6d65 6e73 696f 6e3d 7365 6c66 2e64  dimension=self.d
+00016660: 696d 656e 7369 6f6e 2c0a 2020 2020 2020  imension,.      
+00016670: 2020 2020 2020 6465 7269 7665 645f 6672        derived_fr
+00016680: 6f6d 5f6f 703d 4f70 286b 696e 643d 226d  om_op=Op(kind="m
+00016690: 756c 222c 2069 6e70 7574 733d 6c69 7374  ul", inputs=list
+000166a0: 2873 656c 662e 7465 726d 7329 292c 0a20  (self.terms)),. 
+000166b0: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
+000166c0: 6564 5f66 726f 6d5f 7461 673d 7365 6c66  ed_from_tag=self
+000166d0: 2e72 6570 7265 7365 6e74 6174 6976 655f  .representative_
+000166e0: 7461 6728 292c 0a20 2020 2020 2020 2029  tag(),.        )
+000166f0: 0a0a 2020 2020 6465 6620 7265 7072 6573  ..    def repres
+00016700: 656e 7461 7469 7665 5f74 6167 2873 656c  entative_tag(sel
+00016710: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00016720: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00016730: 4469 6d7c 4e6f 6e65 0a20 2020 2020 2020  Dim|None.       
+00016740: 2022 2222 0a20 2020 2020 2020 2023 2041   """.        # A
+00016750: 6c73 6f20 7365 6520 4469 6d2e 5f4f 704c  lso see Dim._OpL
+00016760: 696e 6561 7254 6572 6d2e 7265 7072 6573  inearTerm.repres
+00016770: 656e 7461 7469 7665 5f74 6167 2829 2e0a  entative_tag()..
+00016780: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
+00016790: 6669 6e64 2061 6e79 2064 796e 616d 6963  find any dynamic
+000167a0: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
+000167b0: 726d 5f20 696e 2073 656c 662e 7465 726d  rm_ in self.term
+000167c0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+000167d0: 6620 7465 726d 5f2e 6973 5f64 796e 616d  f term_.is_dynam
+000167e0: 6963 2829 3a0a 2020 2020 2020 2020 2020  ic():.          
+000167f0: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
+00016800: 6d5f 0a20 2020 2020 2020 2023 204e 6f77  m_.        # Now
+00016810: 2066 696e 6420 6e6f 6e2d 756e 7370 6563   find non-unspec
+00016820: 6966 6965 642e 0a20 2020 2020 2020 2066  ified..        f
+00016830: 6f72 2074 6572 6d5f 2069 6e20 7365 6c66  or term_ in self
+00016840: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00016850: 2020 2020 6966 2074 6572 6d5f 2e6b 696e      if term_.kin
+00016860: 6420 213d 2044 696d 5479 7065 732e 556e  d != DimTypes.Un
+00016870: 7370 6563 6966 6965 643a 0a20 2020 2020  specified:.     
+00016880: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016890: 6e20 7465 726d 5f0a 2020 2020 2020 2020  n term_.        
+000168a0: 2320 4e6f 7720 6669 6e64 2061 6e79 2e0a  # Now find any..
+000168b0: 2020 2020 2020 2020 666f 7220 7465 726d          for term
+000168c0: 5f20 696e 2073 656c 662e 7465 726d 733a  _ in self.terms:
+000168d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000168e0: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
+000168f0: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
+00016900: 636c 6173 7320 5f4f 704c 696e 6561 7254  class _OpLinearT
+00016910: 6572 6d3a 0a20 2020 2022 2222 0a20 2020  erm:.    """.   
+00016920: 2072 6570 7265 7365 6e74 7320 7374 6820   represents sth 
+00016930: 6c69 6b65 2061 202a 2062 202b 2063 0a20  like a * b + c. 
+00016940: 2020 2022 2222 0a0a 2020 2020 4063 6c61     """..    @cla
+00016950: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00016960: 2066 726f 6d5f 6469 6d28 636c 732c 2064   from_dim(cls, d
+00016970: 696d 293a 0a20 2020 2020 2020 2022 2222  im):.        """
+00016980: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00016990: 4469 6d20 6469 6d3a 0a20 2020 2020 2020  Dim dim:.       
+000169a0: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
+000169b0: 4c69 6e65 6172 5465 726d 0a20 2020 2020  LinearTerm.     
+000169c0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+000169d0: 6573 203d 2063 6c73 2e7a 6572 6f28 290a  es = cls.zero().
+000169e0: 2020 2020 2020 2020 7265 732e 6578 7465          res.exte
+000169f0: 6e64 5f61 6464 5f73 7562 5f28 6469 6d2c  nd_add_sub_(dim,
+00016a00: 206b 696e 643d 2261 6464 222c 2072 6967   kind="add", rig
+00016a10: 6874 3d54 7275 6529 0a20 2020 2020 2020  ht=True).       
+00016a20: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
+00016a30: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00016a40: 2020 6465 6620 7a65 726f 2863 6c73 293a    def zero(cls):
+00016a50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016a60: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00016a70: 2e5f 4f70 4c69 6e65 6172 5465 726d 0a20  ._OpLinearTerm. 
+00016a80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016a90: 2020 2072 6574 7572 6e20 5f4f 704c 696e     return _OpLin
+00016aa0: 6561 7254 6572 6d28 5b5d 290a 0a20 2020  earTerm([])..   
+00016ab0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00016ac0: 6c66 2c20 7465 726d 7329 3a0a 2020 2020  lf, terms):.    
+00016ad0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00016ae0: 3a70 6172 616d 206c 6973 745b 4469 6d2e  :param list[Dim.
+00016af0: 5f4f 704d 756c 7454 6572 6d5d 2074 6572  _OpMultTerm] ter
+00016b00: 6d73 3a0a 2020 2020 2020 2020 2222 220a  ms:.        """.
+00016b10: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
+00016b20: 6d73 203d 2074 6572 6d73 0a0a 2020 2020  ms = terms..    
+00016b30: 6465 6620 5f5f 6861 7368 5f5f 2873 656c  def __hash__(sel
+00016b40: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00016b50: 726e 2068 6173 6828 7475 706c 6528 7365  rn hash(tuple(se
+00016b60: 6c66 2e74 6572 6d73 2929 0a0a 2020 2020  lf.terms))..    
+00016b70: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
+00016b80: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+00016b90: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
+00016ba0: 7468 6572 2c20 5f4f 704c 696e 6561 7254  ther, _OpLinearT
+00016bb0: 6572 6d29 3a0a 2020 2020 2020 2020 2020  erm):.          
+00016bc0: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
+00016bd0: 726d 7320 3d3d 206f 7468 6572 2e74 6572  rms == other.ter
+00016be0: 6d73 0a20 2020 2020 2020 2072 6574 7572  ms.        retur
+00016bf0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00016c00: 205f 5f6e 655f 5f28 7365 6c66 2c20 6f74   __ne__(self, ot
+00016c10: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
+00016c20: 7475 726e 206e 6f74 2073 656c 662e 5f5f  turn not self.__
+00016c30: 6571 5f5f 286f 7468 6572 290a 0a20 2020  eq__(other)..   
+00016c40: 2064 6566 2061 735f 6469 6d28 7365 6c66   def as_dim(self
+00016c50: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00016c60: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+00016c70: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
+00016c80: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00016c90: 735f 7a65 726f 2829 3a0a 2020 2020 2020  s_zero():.      
+00016ca0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00016cb0: 6b65 5f63 6f6e 7374 616e 745f 7374 6174  ke_constant_stat
+00016cc0: 6963 5f64 696d 2830 290a 2020 2020 2020  ic_dim(0).      
+00016cd0: 2020 6966 206c 656e 2873 656c 662e 7465    if len(self.te
+00016ce0: 726d 7329 203d 3d20 313a 0a20 2020 2020  rms) == 1:.     
+00016cf0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00016d00: 6c66 2e74 6572 6d73 5b30 5d2e 6173 5f64  lf.terms[0].as_d
+00016d10: 696d 2829 0a20 2020 2020 2020 2061 6464  im().        add
+00016d20: 5f70 6172 7473 203d 205b 5d0a 2020 2020  _parts = [].    
+00016d30: 2020 2020 6465 7363 5f70 6172 7473 203d      desc_parts =
+00016d40: 205b 5d0a 2020 2020 2020 2020 6469 6d20   [].        dim 
+00016d50: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
+00016d60: 7465 726d 2069 6e20 7365 6c66 2e74 6572  term in self.ter
+00016d70: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+00016d80: 7320 3d20 7465 726d 2e61 735f 6469 6d28  s = term.as_dim(
+00016d90: 290a 2020 2020 2020 2020 2020 2020 6164  ).            ad
+00016da0: 645f 7061 7274 732e 6170 7065 6e64 2873  d_parts.append(s
+00016db0: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
+00016dc0: 7363 5f70 6172 7473 2e61 7070 656e 6428  sc_parts.append(
+00016dd0: 5f67 6574 5f64 6573 6372 6970 7469 6f6e  _get_description
+00016de0: 2873 2929 0a20 2020 2020 2020 2020 2020  (s)).           
+00016df0: 2069 6620 6469 6d20 6973 206e 6f74 204e   if dim is not N
+00016e00: 6f6e 6520 616e 6420 732e 6469 6d65 6e73  one and s.dimens
+00016e10: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+00016e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016e30: 2064 696d 202b 3d20 732e 6469 6d65 6e73   dim += s.dimens
+00016e40: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00016e50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00016e60: 2020 2020 2020 6469 6d20 3d20 4e6f 6e65        dim = None
+00016e70: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00016e80: 6164 645f 7061 7274 7329 203d 3d20 313a  add_parts) == 1:
+00016e90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00016ea0: 7572 6e20 6164 645f 7061 7274 735b 305d  urn add_parts[0]
+00016eb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00016ec0: 5f64 2e44 696d 280a 2020 2020 2020 2020  _d.Dim(.        
+00016ed0: 2020 2020 6b69 6e64 3d5f 6765 745f 6d65      kind=_get_me
+00016ee0: 7267 6564 5f64 696d 5f6b 696e 6428 6164  rged_dim_kind(ad
+00016ef0: 645f 7061 7274 7329 2c0a 2020 2020 2020  d_parts),.      
+00016f00: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00016f10: 6e3d 222b 222e 6a6f 696e 2864 6573 635f  n="+".join(desc_
+00016f20: 7061 7274 7329 2c0a 2020 2020 2020 2020  parts),.        
+00016f30: 2020 2020 6469 6d65 6e73 696f 6e3d 6469      dimension=di
+00016f40: 6d2c 0a20 2020 2020 2020 2020 2020 2064  m,.            d
+00016f50: 6572 6976 6564 5f66 726f 6d5f 6f70 3d4f  erived_from_op=O
+00016f60: 7028 6b69 6e64 3d22 6164 6422 2c20 696e  p(kind="add", in
+00016f70: 7075 7473 3d61 6464 5f70 6172 7473 292c  puts=add_parts),
+00016f80: 0a20 2020 2020 2020 2020 2020 2064 6572  .            der
+00016f90: 6976 6564 5f66 726f 6d5f 7461 673d 7365  ived_from_tag=se
+00016fa0: 6c66 2e72 6570 7265 7365 6e74 6174 6976  lf.representativ
+00016fb0: 655f 7461 6728 292c 0a20 2020 2020 2020  e_tag(),.       
+00016fc0: 2029 0a0a 2020 2020 6465 6620 5f5f 7265   )..    def __re
+00016fd0: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
+00016fe0: 2020 2020 7265 7475 726e 2022 4469 6d2e      return "Dim.
+00016ff0: 5f4f 704c 696e 6561 7254 6572 6d28 2572  _OpLinearTerm(%r
+00017000: 2922 2025 2028 7365 6c66 2e74 6572 6d73  )" % (self.terms
+00017010: 2c29 0a0a 2020 2020 6465 6620 6973 5f7a  ,)..    def is_z
+00017020: 6572 6f28 7365 6c66 293a 0a20 2020 2020  ero(self):.     
+00017030: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00017040: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+00017050: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00017060: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
+00017070: 7465 726d 730a 0a20 2020 2064 6566 2065  terms..    def e
+00017080: 7874 656e 645f 6164 645f 7375 625f 2873  xtend_add_sub_(s
+00017090: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
+000170a0: 2c20 7269 6768 7429 3a0a 2020 2020 2020  , right):.      
+000170b0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+000170c0: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
+000170d0: 6572 3a0a 2020 2020 2020 2020 3a70 6172  er:.        :par
+000170e0: 616d 2073 7472 206b 696e 643a 2022 6164  am str kind: "ad
+000170f0: 6422 206f 7220 2273 7562 220a 2020 2020  d" or "sub".    
+00017100: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+00017110: 7269 6768 743a 206f 7220 6c65 6674 2e20  right: or left. 
+00017120: 7269 6768 7420 6d65 616e 7320 7365 6c66  right means self
+00017130: 202b 206f 7468 6572 2c20 6c65 6674 206d   + other, left m
+00017140: 6561 6e73 206f 7468 6572 202b 2073 656c  eans other + sel
+00017150: 660a 2020 2020 2020 2020 2222 220a 2020  f.        """.  
+00017160: 2020 2020 2020 6173 7365 7274 206b 696e        assert kin
+00017170: 6420 696e 207b 2261 6464 222c 2022 7375  d in {"add", "su
+00017180: 6222 7d0a 2020 2020 2020 2020 6f74 6865  b"}.        othe
+00017190: 7220 3d20 7365 6c66 2e5f 6d61 6b65 5f64  r = self._make_d
+000171a0: 696d 286f 7468 6572 2c20 6b69 6e64 3d6b  im(other, kind=k
+000171b0: 696e 6429 0a20 2020 2020 2020 2069 6620  ind).        if 
+000171c0: 6f74 6865 722e 6973 5f63 6f6e 7374 616e  other.is_constan
+000171d0: 745f 7374 6174 6963 5f64 696d 2829 2061  t_static_dim() a
+000171e0: 6e64 206f 7468 6572 2e64 696d 656e 7369  nd other.dimensi
+000171f0: 6f6e 203d 3d20 303a 0a20 2020 2020 2020  on == 0:.       
+00017200: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00017210: 2020 2020 6966 206f 7468 6572 2e64 6572      if other.der
+00017220: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
+00017230: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
+00017240: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
+00017250: 6164 6422 3a0a 2020 2020 2020 2020 2020  add":.          
+00017260: 2020 666f 7220 6f74 6865 725f 2069 6e20    for other_ in 
+00017270: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00017280: 6f6d 5f6f 702e 696e 7075 7473 2069 6620  om_op.inputs if 
+00017290: 7269 6768 7420 656c 7365 2072 6576 6572  right else rever
+000172a0: 7365 6428 6f74 6865 722e 6465 7269 7665  sed(other.derive
+000172b0: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
+000172c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000172d0: 2020 2073 656c 662e 6578 7465 6e64 5f61     self.extend_a
+000172e0: 6464 5f73 7562 5f28 6f74 6865 725f 2c20  dd_sub_(other_, 
+000172f0: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
+00017300: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
+00017310: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00017320: 2020 2074 6572 6d20 3d20 5f4f 704d 756c     term = _OpMul
+00017330: 7454 6572 6d2e 6672 6f6d 5f64 696d 286f  tTerm.from_dim(o
+00017340: 7468 6572 290a 2020 2020 2020 2020 6e65  ther).        ne
+00017350: 675f 7465 726d 203d 2074 6572 6d2e 6e65  g_term = term.ne
+00017360: 6761 7469 7665 2829 0a20 2020 2020 2020  gative().       
+00017370: 2069 6620 6b69 6e64 203d 3d20 2273 7562   if kind == "sub
+00017380: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
+00017390: 6572 6d2c 206e 6567 5f74 6572 6d20 3d20  erm, neg_term = 
+000173a0: 6e65 675f 7465 726d 2c20 7465 726d 0a20  neg_term, term. 
+000173b0: 2020 2020 2020 206d 6f73 745f 7265 6365         most_rece
+000173c0: 6e74 5f74 6572 6d20 3d20 7365 6c66 2e74  nt_term = self.t
+000173d0: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
+000173e0: 2065 6c73 6520 305d 2069 6620 7365 6c66   else 0] if self
+000173f0: 2e74 6572 6d73 2065 6c73 6520 4e6f 6e65  .terms else None
+00017400: 0a20 2020 2020 2020 2069 6620 6d6f 7374  .        if most
+00017410: 5f72 6563 656e 745f 7465 726d 3a0a 2020  _recent_term:.  
+00017420: 2020 2020 2020 2020 2020 6966 206d 6f73            if mos
+00017430: 745f 7265 6365 6e74 5f74 6572 6d20 3d3d  t_recent_term ==
+00017440: 206e 6567 5f74 6572 6d3a 0a20 2020 2020   neg_term:.     
+00017450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017460: 7465 726d 732e 706f 7028 2d31 2069 6620  terms.pop(-1 if 
+00017470: 7269 6768 7420 656c 7365 2030 290a 2020  right else 0).  
+00017480: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00017490: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+000174a0: 2069 6620 6d6f 7374 5f72 6563 656e 745f   if most_recent_
+000174b0: 7465 726d 2e69 735f 636f 6e73 7461 6e74  term.is_constant
+000174c0: 5f73 7461 7469 635f 6469 6d28 2920 616e  _static_dim() an
+000174d0: 6420 7465 726d 2e69 735f 636f 6e73 7461  d term.is_consta
+000174e0: 6e74 5f73 7461 7469 635f 6469 6d28 293a  nt_static_dim():
+000174f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017500: 2073 656c 662e 7465 726d 735b 2d31 2069   self.terms[-1 i
+00017510: 6620 7269 6768 7420 656c 7365 2030 5d20  f right else 0] 
+00017520: 3d20 5f4f 704d 756c 7454 6572 6d2e 6672  = _OpMultTerm.fr
+00017530: 6f6d 5f64 696d 280a 2020 2020 2020 2020  om_dim(.        
+00017540: 2020 2020 2020 2020 2020 2020 5f6d 616b              _mak
+00017550: 655f 636f 6e73 7461 6e74 5f73 7461 7469  e_constant_stati
+00017560: 635f 6469 6d28 6d6f 7374 5f72 6563 656e  c_dim(most_recen
+00017570: 745f 7465 726d 2e64 696d 656e 7369 6f6e  t_term.dimension
+00017580: 202b 2074 6572 6d2e 6469 6d65 6e73 696f   + term.dimensio
+00017590: 6e2c 206b 696e 643d 6f74 6865 722e 6b69  n, kind=other.ki
+000175a0: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
+000175b0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000175c0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000175d0: 2020 2020 2020 2020 2069 6620 6d6f 7374           if most
+000175e0: 5f72 6563 656e 745f 7465 726d 2e74 6572  _recent_term.ter
+000175f0: 6d73 2061 6e64 2074 6572 6d2e 7465 726d  ms and term.term
+00017600: 7320 616e 6420 6d6f 7374 5f72 6563 656e  s and most_recen
+00017610: 745f 7465 726d 2e74 6572 6d73 5b2d 315d  t_term.terms[-1]
+00017620: 203d 3d20 7465 726d 2e74 6572 6d73 5b2d   == term.terms[-
+00017630: 315d 3a0a 2020 2020 2020 2020 2020 2020  1]:.            
+00017640: 2020 2020 2320 4d65 7267 6520 7465 726d      # Merge term
+00017650: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00017660: 2020 6120 3d20 5f4f 704d 756c 7454 6572    a = _OpMultTer
+00017670: 6d2e 6672 6f6d 5f64 696d 5f66 6163 746f  m.from_dim_facto
+00017680: 7273 286d 6f73 745f 7265 6365 6e74 5f74  rs(most_recent_t
+00017690: 6572 6d2e 7465 726d 735b 3a2d 315d 292e  erm.terms[:-1]).
+000176a0: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
+000176b0: 2020 2020 2020 2020 2062 203d 205f 4f70           b = _Op
+000176c0: 4d75 6c74 5465 726d 2e66 726f 6d5f 6469  MultTerm.from_di
+000176d0: 6d5f 6661 6374 6f72 7328 7465 726d 2e74  m_factors(term.t
+000176e0: 6572 6d73 5b3a 2d31 5d29 2e61 735f 6469  erms[:-1]).as_di
+000176f0: 6d28 290a 2020 2020 2020 2020 2020 2020  m().            
+00017700: 2020 2020 7265 7320 3d20 5f4f 704d 756c      res = _OpMul
+00017710: 7454 6572 6d2e 6672 6f6d 5f64 696d 2828  tTerm.from_dim((
+00017720: 6120 2b20 6229 2069 6620 7269 6768 7420  a + b) if right 
+00017730: 656c 7365 2028 6220 2b20 6129 290a 2020  else (b + a)).  
+00017740: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00017750: 732e 6578 7465 6e64 5f6d 756c 5f64 6976  s.extend_mul_div
+00017760: 5f28 7465 726d 2e74 6572 6d73 5b2d 315d  _(term.terms[-1]
+00017770: 2c20 6b69 6e64 3d22 6d75 6c22 2c20 7269  , kind="mul", ri
+00017780: 6768 743d 5472 7565 290a 2020 2020 2020  ght=True).      
+00017790: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+000177a0: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
+000177b0: 2065 6c73 6520 305d 203d 2072 6573 0a20   else 0] = res. 
+000177c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000177d0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+000177e0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
+000177f0: 2020 2020 7365 6c66 2e74 6572 6d73 2e61      self.terms.a
+00017800: 7070 656e 6428 7465 726d 290a 2020 2020  ppend(term).    
+00017810: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00017820: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
+00017830: 2e69 6e73 6572 7428 302c 2074 6572 6d29  .insert(0, term)
+00017840: 0a0a 2020 2020 6465 6620 6578 7465 6e64  ..    def extend
+00017850: 5f6d 756c 5f64 6976 5f28 7365 6c66 2c20  _mul_div_(self, 
+00017860: 6f74 6865 722c 206b 696e 642c 2072 6967  other, kind, rig
+00017870: 6874 293a 0a20 2020 2020 2020 2022 2222  ht):.        """
+00017880: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00017890: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
+000178a0: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
+000178b0: 7220 6b69 6e64 3a20 226d 756c 2220 6f72  r kind: "mul" or
+000178c0: 2022 6365 696c 6469 7622 0a20 2020 2020   "ceildiv".     
+000178d0: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
+000178e0: 6967 6874 3a20 6f72 206c 6566 742e 2072  ight: or left. r
+000178f0: 6967 6874 206d 6561 6e73 2073 656c 6620  ight means self 
+00017900: 2a20 6f74 6865 722c 206c 6566 7420 6d65  * other, left me
+00017910: 616e 7320 6f74 6865 7220 2a20 7365 6c66  ans other * self
+00017920: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00017930: 2020 2020 2061 7373 6572 7420 6b69 6e64       assert kind
+00017940: 2069 6e20 7b22 6d75 6c22 2c20 2266 6c6f   in {"mul", "flo
+00017950: 6f72 6469 7622 2c20 2274 7275 6564 6976  ordiv", "truediv
+00017960: 222c 2022 6365 696c 6469 7622 7d0a 2020  ", "ceildiv"}.  
+00017970: 2020 2020 2020 6f74 6865 7220 3d20 7365        other = se
+00017980: 6c66 2e5f 6d61 6b65 5f64 696d 286f 7468  lf._make_dim(oth
+00017990: 6572 2c20 6b69 6e64 3d6b 696e 6429 0a20  er, kind=kind). 
+000179a0: 2020 2020 2020 2069 6620 6b69 6e64 203d         if kind =
+000179b0: 3d20 226d 756c 2220 616e 6420 7269 6768  = "mul" and righ
+000179c0: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
+000179d0: 6620 6e6f 7420 616c 6c28 7465 726d 2e63  f not all(term.c
+000179e0: 616e 5f73 696d 706c 6966 7928 6f74 6865  an_simplify(othe
+000179f0: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
+00017a00: 6768 743d 7269 6768 7429 2066 6f72 2074  ght=right) for t
+00017a10: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
+00017a20: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00017a30: 2020 2020 2320 446f 2069 7420 7468 6520      # Do it the 
+00017a40: 6f74 6865 7220 7761 7920 6172 6f75 6e64  other way around
+00017a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017a60: 2073 656c 662e 7465 726d 732c 206f 7468   self.terms, oth
+00017a70: 6572 203d 205f 4f70 4c69 6e65 6172 5465  er = _OpLinearTe
+00017a80: 726d 2e66 726f 6d5f 6469 6d28 6f74 6865  rm.from_dim(othe
+00017a90: 7229 2e74 6572 6d73 2c20 7365 6c66 2e61  r).terms, self.a
+00017aa0: 735f 6469 6d28 290a 2020 2020 2020 2020  s_dim().        
+00017ab0: 2020 2020 2020 2020 7269 6768 7420 3d20          right = 
+00017ac0: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
+00017ad0: 206f 7468 6572 2e69 735f 636f 6e73 7461   other.is_consta
+00017ae0: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
+00017af0: 616e 6420 6f74 6865 722e 6469 6d65 6e73  and other.dimens
+00017b00: 696f 6e20 3d3d 2031 3a0a 2020 2020 2020  ion == 1:.      
+00017b10: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00017b20: 2020 2020 2069 6620 6b69 6e64 2e65 6e64       if kind.end
+00017b30: 7377 6974 6828 2264 6976 2229 2061 6e64  swith("div") and
+00017b40: 206c 656e 2873 656c 662e 7465 726d 7329   len(self.terms)
+00017b50: 203e 3d20 323a 0a20 2020 2020 2020 2020   >= 2:.         
+00017b60: 2020 2069 6620 616e 7928 6e6f 7420 7465     if any(not te
+00017b70: 726d 2e64 6976 6973 6962 6c65 286f 7468  rm.divisible(oth
+00017b80: 6572 2c20 7269 6768 743d 7269 6768 7429  er, right=right)
+00017b90: 2066 6f72 2074 6572 6d20 696e 2073 656c   for term in sel
+00017ba0: 662e 7465 726d 7329 3a0a 2020 2020 2020  f.terms):.      
+00017bb0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00017bc0: 6572 6d73 203d 205b 0a20 2020 2020 2020  erms = [.       
+00017bd0: 2020 2020 2020 2020 2020 2020 205f 4f70               _Op
+00017be0: 4d75 6c74 5465 726d 2e66 726f 6d5f 6469  MultTerm.from_di
+00017bf0: 6d28 5f4f 704d 756c 7454 6572 6d2e 6e65  m(_OpMultTerm.ne
+00017c00: 775f 6469 765f 6469 6d28 7365 6c66 2e61  w_div_dim(self.a
+00017c10: 735f 6469 6d28 292c 206f 7468 6572 2c20  s_dim(), other, 
+00017c20: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
+00017c30: 3d72 6967 6874 2929 0a20 2020 2020 2020  =right)).       
+00017c40: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00017c50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00017c60: 6e0a 2020 2020 2020 2020 666f 7220 7465  n.        for te
+00017c70: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
+00017c80: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00017c90: 726d 2e65 7874 656e 645f 6d75 6c5f 6469  rm.extend_mul_di
+00017ca0: 765f 286f 7468 6572 2c20 6b69 6e64 3d6b  v_(other, kind=k
+00017cb0: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
+00017cc0: 290a 0a20 2020 2064 6566 205f 6d61 6b65  )..    def _make
+00017cd0: 5f64 696d 2873 656c 662c 206f 7468 6572  _dim(self, other
+00017ce0: 2c20 6b69 6e64 293a 0a20 2020 2020 2020  , kind):.       
+00017cf0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+00017d00: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
+00017d10: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
+00017d20: 6d20 7374 7220 6b69 6e64 3a0a 2020 2020  m str kind:.    
+00017d30: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
+00017d40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00017d50: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00017d60: 6528 6f74 6865 722c 2069 6e74 293a 0a20  e(other, int):. 
+00017d70: 2020 2020 2020 2020 2020 2062 6173 655f             base_
+00017d80: 7461 6720 3d20 7365 6c66 2e72 6570 7265  tag = self.repre
+00017d90: 7365 6e74 6174 6976 655f 7461 6728 290a  sentative_tag().
+00017da0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017db0: 726e 205f 6d61 6b65 5f63 6f6e 7374 616e  rn _make_constan
+00017dc0: 745f 7374 6174 6963 5f64 696d 286f 7468  t_static_dim(oth
+00017dd0: 6572 2c20 6b69 6e64 3d62 6173 655f 7461  er, kind=base_ta
+00017de0: 672e 6b69 6e64 2069 6620 6261 7365 5f74  g.kind if base_t
+00017df0: 6167 2065 6c73 6520 4e6f 6e65 290a 2020  ag else None).  
+00017e00: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00017e10: 7461 6e63 6528 6f74 6865 722c 205f 642e  tance(other, _d.
+00017e20: 4469 6d29 3a0a 2020 2020 2020 2020 2020  Dim):.          
+00017e30: 2020 7265 7475 726e 206f 7468 6572 2e67    return other.g
+00017e40: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
+00017e50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00017e60: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00017e70: 7970 6545 7272 6f72 2822 2573 2025 7320  ypeError("%s %s 
+00017e80: 2573 2069 6e76 616c 6964 2066 6f72 2074  %s invalid for t
+00017e90: 7970 6520 2573 2220 2520 2873 656c 662c  ype %s" % (self,
+00017ea0: 206b 696e 642c 206f 7468 6572 2c20 7479   kind, other, ty
+00017eb0: 7065 286f 7468 6572 2929 290a 0a20 2020  pe(other)))..   
+00017ec0: 2064 6566 2072 6570 7265 7365 6e74 6174   def representat
+00017ed0: 6976 655f 7461 6728 7365 6c66 293a 0a20  ive_tag(self):. 
+00017ee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00017ef0: 2020 203a 7274 7970 653a 2044 696d 7c4e     :rtype: Dim|N
+00017f00: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
+00017f10: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
+00017f20: 6669 6e64 2061 6e79 2064 796e 616d 6963  find any dynamic
+00017f30: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
+00017f40: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
+00017f50: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00017f60: 7220 7465 726d 5f20 696e 2074 6572 6d2e  r term_ in term.
+00017f70: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+00017f80: 2020 2020 2020 2069 6620 7465 726d 5f2e         if term_.
+00017f90: 6973 5f64 796e 616d 6963 2829 3a0a 2020  is_dynamic():.  
+00017fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fb0: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
+00017fc0: 2020 2020 2020 2023 204e 6f77 2066 696e         # Now fin
+00017fd0: 6420 6e6f 6e2d 756e 7370 6563 6966 6965  d non-unspecifie
+00017fe0: 642e 0a20 2020 2020 2020 2066 6f72 2074  d..        for t
+00017ff0: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
+00018000: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00018010: 6f72 2074 6572 6d5f 2069 6e20 7465 726d  or term_ in term
+00018020: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00018030: 2020 2020 2020 2020 6966 2074 6572 6d5f          if term_
+00018040: 2e6b 696e 6420 213d 2044 696d 5479 7065  .kind != DimType
+00018050: 732e 556e 7370 6563 6966 6965 643a 0a20  s.Unspecified:. 
+00018060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018070: 2020 2072 6574 7572 6e20 7465 726d 5f0a     return term_.
+00018080: 2020 2020 2020 2020 2320 4e6f 7720 6669          # Now fi
+00018090: 6e64 2061 6e79 2e0a 2020 2020 2020 2020  nd any..        
+000180a0: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
+000180b0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+000180c0: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
+000180d0: 2074 6572 6d2e 7465 726d 733a 0a20 2020   term.terms:.   
+000180e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000180f0: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
+00018100: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
+00018110: 6465 6620 5f67 6574 5f6d 6572 6765 645f  def _get_merged_
+00018120: 6469 6d5f 6b69 6e64 2864 696d 5f74 6167  dim_kind(dim_tag
+00018130: 7329 3a0a 2020 2020 2222 220a 2020 2020  s):.    """.    
+00018140: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
+00018150: 7c74 7570 6c65 5b44 696d 5d20 6469 6d5f  |tuple[Dim] dim_
+00018160: 7461 6773 3a0a 2020 2020 3a72 6574 7572  tags:.    :retur
+00018170: 6e3a 2064 696d 206b 696e 640a 2020 2020  n: dim kind.    
+00018180: 3a72 7479 7065 3a20 456e 7469 7479 0a20  :rtype: Entity. 
+00018190: 2020 2022 2222 0a20 2020 2069 6620 616e     """.    if an
+000181a0: 7928 7461 672e 6973 5f62 6174 6368 5f64  y(tag.is_batch_d
+000181b0: 696d 2829 2066 6f72 2074 6167 2069 6e20  im() for tag in 
+000181c0: 6469 6d5f 7461 6773 293a 0a20 2020 2020  dim_tags):.     
+000181d0: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
+000181e0: 6573 2e42 6174 6368 0a20 2020 2065 6c69  es.Batch.    eli
+000181f0: 6620 616e 7928 7461 672e 6973 5f66 6561  f any(tag.is_fea
+00018200: 7475 7265 5f64 696d 2829 2066 6f72 2074  ture_dim() for t
+00018210: 6167 2069 6e20 6469 6d5f 7461 6773 293a  ag in dim_tags):
+00018220: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00018230: 4469 6d54 7970 6573 2e46 6561 7475 7265  DimTypes.Feature
+00018240: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00018250: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
+00018260: 6573 2e53 7061 7469 616c 0a0a 0a64 6566  es.Spatial...def
+00018270: 2064 696d 5f63 6d70 5f76 616c 7565 286f   dim_cmp_value(o
+00018280: 626a 293a 0a20 2020 2022 2222 0a20 2020  bj):.    """.   
+00018290: 203a 7061 7261 6d20 4469 6d7c 5f4d 6172   :param Dim|_Mar
+000182a0: 6b65 6444 696d 206f 626a 3a0a 2020 2020  kedDim obj:.    
+000182b0: 3a72 6574 7572 6e3a 2061 6e79 7468 696e  :return: anythin
+000182c0: 6720 7768 6963 6820 6361 6e20 6265 2063  g which can be c
+000182d0: 6f6d 7061 7265 640a 2020 2020 2222 220a  ompared.    """.
+000182e0: 2020 2020 2320 4d61 6b65 2044 696d 2061      # Make Dim a
+000182f0: 6e64 205f 4d61 726b 6564 4469 6d20 636f  nd _MarkedDim co
+00018300: 6d70 6172 6162 6c65 2074 6f20 6561 6368  mparable to each
+00018310: 206f 7468 6572 2e0a 2020 2020 2320 4e6f   other..    # No
+00018320: 7465 2074 6861 7420 7468 6520 6f72 6465  te that the orde
+00018330: 7220 6973 2072 6561 6c6c 7920 6172 6269  r is really arbi
+00018340: 7472 6172 7920 616e 6420 646f 6573 206e  trary and does n
+00018350: 6f74 206d 6174 7465 722e 0a20 2020 2069  ot matter..    i
+00018360: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
+00018370: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
+00018380: 2020 206f 626a 203d 206f 626a 2e67 6574     obj = obj.get
+00018390: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
+000183a0: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
+000183b0: 2020 2020 2020 2020 2020 2222 2c0a 2020            "",.  
+000183c0: 2020 2020 2020 2020 2020 6f62 6a2e 6465            obj.de
+000183d0: 7363 7269 7074 696f 6e2c 0a20 2020 2020  scription,.     
+000183e0: 2020 2020 2020 206f 626a 2e6b 696e 642c         obj.kind,
+000183f0: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
+00018400: 2e64 696d 656e 7369 6f6e 2c0a 2020 2020  .dimension,.    
+00018410: 2020 2020 2020 2020 6f62 6a2e 6479 6e5f          obj.dyn_
+00018420: 7369 7a65 5f65 7874 2e64 696d 7320 6966  size_ext.dims if
+00018430: 206f 626a 2e64 796e 5f73 697a 655f 6578   obj.dyn_size_ex
+00018440: 7420 6973 206e 6f74 204e 6f6e 6520 656c  t is not None el
+00018450: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
+00018460: 2029 0a20 2020 2069 6620 6973 696e 7374   ).    if isinst
+00018470: 616e 6365 286f 626a 2c20 5f6d 2e4d 6172  ance(obj, _m.Mar
+00018480: 6b65 6444 696d 293a 0a20 2020 2020 2020  kedDim):.       
+00018490: 2072 6574 7572 6e20 6f62 6a2e 5f5f 636c   return obj.__cl
+000184a0: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20  ass__.__name__, 
+000184b0: 6f62 6a2e 7461 670a 2020 2020 7265 7475  obj.tag.    retu
+000184c0: 726e 206f 626a 0a                        rn obj.
```

### Comparing `returnn-1.20230512.95100/returnn/tensor/_tensor_extra.py` & `returnn-1.20230515.93528/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230515.93528/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230515.93528/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230515.93528/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/dim.py` & `returnn-1.20230515.93528/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/marked_dim.py` & `returnn-1.20230515.93528/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/tensor.py` & `returnn-1.20230515.93528/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/tensor_dict.py` & `returnn-1.20230515.93528/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tensor/utils.py` & `returnn-1.20230515.93528/returnn/tensor/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,62 +10,74 @@
 
 
 def tensor_dict_fill_random_numpy_(
     tensor_dict: TensorDict,
     *,
     rnd: Union[int, numpy.random.RandomState] = 42,
     dyn_dim_max_sizes: Optional[Dict[Dim, int]] = None,
+    dyn_dim_min_sizes: Optional[Dict[Dim, int]] = None,
 ):
     """
     Random fill with NumPy arrays.
 
     :param tensor_dict:
     :param rnd:
     :param dyn_dim_max_sizes: you can specify max sizes for dim tags with dynamic sizes.
         The fill random code makes sure that there is at least one entry where we reach the max size,
         so that the dim value will be the max size.
+    :param dyn_dim_min_sizes:
     """
     if not isinstance(rnd, numpy.random.RandomState):
         rnd = numpy.random.RandomState(rnd)
     for v in tensor_dict.data.values():
-        tensor_fill_random_numpy_(v, rnd=rnd, dyn_dim_max_sizes=dyn_dim_max_sizes)
+        tensor_fill_random_numpy_(v, rnd=rnd, dyn_dim_max_sizes=dyn_dim_max_sizes, dyn_dim_min_sizes=dyn_dim_min_sizes)
 
 
 def tensor_fill_random_numpy_(
     x: Tensor,
     *,
     min_val: int = 0,
     max_val: Optional[int] = None,
     rnd: numpy.random.RandomState,
     dyn_dim_max_sizes: Optional[Dict[Dim, int]] = None,
+    dyn_dim_min_sizes: Optional[Dict[Dim, int]] = None,
 ) -> bool:
     """fill. return whether sth was filled"""
     if dyn_dim_max_sizes is None:
         dyn_dim_max_sizes = {}
+    if dyn_dim_min_sizes is None:
+        dyn_dim_min_sizes = {}
     filled = False
     while True:
         have_unfilled = False
         filled_this_round = False
 
         for dim in x.dims:
             if dim.is_batch_dim() and not dim.dyn_size_ext:
                 dim.dyn_size_ext = Tensor("batch", [], dtype="int32")
             if not dim.dyn_size_ext:
                 continue
             if tensor_fill_random_numpy_(
                 dim.dyn_size_ext,
-                min_val=2,
+                min_val=dyn_dim_min_sizes.get(dim, 2),
                 max_val=dyn_dim_max_sizes.get(dim, None),
                 rnd=rnd,
                 dyn_dim_max_sizes=dyn_dim_max_sizes,
             ):
                 if dim in dyn_dim_max_sizes:
                     # Make sure at least one of the dyn sizes matches the max size.
                     i = rnd.randint(0, dim.dyn_size_ext.raw_tensor.size)
                     dim.dyn_size_ext.raw_tensor.flat[i] = dyn_dim_max_sizes[dim]
+                    if dim in dyn_dim_min_sizes:
+                        j = rnd.randint(0, dim.dyn_size_ext.raw_tensor.size - 1)
+                        if j >= i:
+                            j += 1
+                        dim.dyn_size_ext.raw_tensor.flat[j] = dyn_dim_min_sizes[dim]
+                elif dim in dyn_dim_min_sizes:
+                    raise Exception(f"also define {dim} in dyn_dim_max_sizes, not just dyn_dim_min_sizes")
                 filled = True
                 filled_this_round = True
             if dim.dyn_size_ext.raw_tensor is None:
                 have_unfilled = True
             elif not isinstance(dim.dyn_size_ext.raw_tensor, numpy.ndarray):
                 have_unfilled = True
```

### Comparing `returnn-1.20230512.95100/returnn/tf/compat.py` & `returnn-1.20230515.93528/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/data_pipeline.py` & `returnn-1.20230515.93528/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/distributed.py` & `returnn-1.20230515.93528/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/engine.py` & `returnn-1.20230515.93528/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230515.93528/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230515.93528/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/horovod.py` & `returnn-1.20230515.93528/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230515.93528/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/layers/base.py` & `returnn-1.20230515.93528/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/layers/basic.py` & `returnn-1.20230515.93528/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/layers/rec.py` & `returnn-1.20230515.93528/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/layers/segmental_model.py` & `returnn-1.20230515.93528/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/layers/signal_processing.py` & `returnn-1.20230515.93528/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/layers/variable.py` & `returnn-1.20230515.93528/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/native_op.py` & `returnn-1.20230515.93528/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/network.py` & `returnn-1.20230515.93528/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/sprint.py` & `returnn-1.20230515.93528/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/updater.py` & `returnn-1.20230515.93528/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/util/basic.py` & `returnn-1.20230515.93528/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/util/data.py` & `returnn-1.20230515.93528/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/util/ken_lm.py` & `returnn-1.20230515.93528/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/tf/util/open_fst.py` & `returnn-1.20230515.93528/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/torch/data/pipeline.py` & `returnn-1.20230515.93528/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230515.93528/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/torch/data/tensor_utils.py` & `returnn-1.20230515.93528/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/torch/engine.py` & `returnn-1.20230515.93528/returnn/torch/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Main engine for PyTorch
 """
 
 from __future__ import annotations
 from typing import Optional, Union, Callable, Dict
+from contextlib import nullcontext
 
 import os
 import torch
 import torch.utils.data.datapipes as dp
+from torch import autocast
+from torch.cuda import amp
 from torchdata.dataloader2 import DataLoader2
 from random import random
 
 from returnn.config import Config
 from returnn.log import log
 from returnn.engine.base import EngineBase
 import returnn.frontend as rf
@@ -49,14 +52,17 @@
         self._final_epoch = None  # type: Optional[int]
         self._orig_model = None  # type: Optional[Union[rf.Module, torch.nn.Module]]
         self._pt_model = None  # type: Optional[torch.nn.Module]
         self._train_step_func = None  # type: Optional[Callable]
         self._save_model_epoch_interval = 1
         self._updater = None  # type: Optional[Updater]
 
+        self._amp_dtype = None  # type: Optional[str]
+        self._grad_scaler = None  # type: Optional[amp.GradScaler]
+
         self._device = _get_device_from_config(config)
         print("Using device:", self._device, file=log.v2)
 
     def init_train_from_config(
         self,
         config: Optional[Config] = None,
         train_data: Optional[Dataset] = None,
@@ -100,14 +106,20 @@
         self._updater.create_optimizer()
         if self._start_epoch > 1:
             self._load_optimizer(self._start_epoch)
 
         self._train_step_func = self.config.typed_value("train_step")
         assert self._train_step_func, "train_step not defined"
 
+        amp_options = self.config.typed_value("torch_amp_options")
+        if amp_options is not None:
+            assert isinstance(amp_options, dict)
+            self._amp_dtype = amp_options.get("dtype")
+            self._grad_scaler = amp.GradScaler()
+
     def train(self):
         """
         Main training loop.
         """
 
         print("Starting training at epoch {}.".format(self._start_epoch), file=log.v3)
         assert self._pt_model is not None, "Model not initialized, call init_train_from_config()."
@@ -140,31 +152,37 @@
 
         self._pt_model.train()
 
         accumulated_losses_dict = NumbersDict()
         accumulated_inv_norm_factors_dict = NumbersDict()
         step_idx = 0
         for data in self._train_dataloader:
-            self._run_step(data, train_flag=True)
+            self._updater.get_optimizer().zero_grad()
+            with autocast(device_type=self._device, dtype=self._amp_dtype) if self._amp_dtype else nullcontext():
+                self._run_step(data, train_flag=True)
 
             train_ctx = rf.get_run_ctx()
             total_loss = train_ctx.total_loss()
             losses_dict = NumbersDict(
                 {
                     name: float(loss.get_summed_loss().raw_tensor.detach().cpu().numpy())
                     for name, loss in train_ctx.losses.items()
                 }
             )
             inv_norm_factors_dict = NumbersDict(
                 {name: float(_to_raw(loss.get_inv_norm_factor())) for name, loss in train_ctx.losses.items()}
             )
 
-            self._updater.get_optimizer().zero_grad()
-            total_loss.raw_tensor.backward()
-            self._updater.get_optimizer().step()
+            if self._amp_dtype:
+                self._grad_scaler.scale(total_loss).backward()
+                self._grad_scaler.step(self._updater.get_optimizer())
+                self._grad_scaler.update()
+            else:
+                total_loss.raw_tensor.backward()
+                self._updater.get_optimizer().step()
 
             accumulated_losses_dict += losses_dict
             accumulated_inv_norm_factors_dict += inv_norm_factors_dict
             _print_process(
                 f"ep {self.epoch} train",
                 step=step_idx,
                 eval_info=dict(losses_dict / inv_norm_factors_dict),
@@ -207,15 +225,18 @@
             accumulated_losses_dict = NumbersDict()
             accumulated_inv_norm_factors_dict = NumbersDict()
             step_idx = 0
 
             with torch.no_grad():
                 for data in data_loader:
 
-                    self._run_step(data)
+                    with autocast(
+                        device_type=self._device, dtype=self._amp_dtype
+                    ) if self._amp_dtype else nullcontext():
+                        self._run_step(data)
                     train_ctx = rf.get_run_ctx()
 
                     if score_keys is None:
                         score_keys = [name for name, loss in train_ctx.losses.items() if not loss.as_error]
                         error_keys = [name for name, loss in train_ctx.losses.items() if loss.as_error]
 
                     losses_dict = NumbersDict(
```

### Comparing `returnn-1.20230512.95100/returnn/torch/frontend/_backend.py` & `returnn-1.20230515.93528/returnn/torch/frontend/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,29 +363,30 @@
         out_dims: Sequence[Dim],
         mode: str = "constant",
         value: Optional[Union[rf.RawTensorTypes, Tensor]] = None,
     ) -> Tensor:
         """pad"""
         assert len(out_dims) == len(axes) == len(padding)
         out = source.copy_template_new_dim_tags(
-            [out_dims[axes.index(dim)] if dim in axes else dim for dim in source.dim_tags]
+            [out_dims[axes.index(dim)] if dim in axes else dim for dim in source.dim_tags], keep_special_axes=True
         )
         remaining_dims = set(axes)
         raw_pad = []
         for dim in reversed(source.dims):
             if dim not in remaining_dims:
+                raw_pad += [0, 0]
                 continue
             remaining_dims.remove(dim)
             pad_ = padding[axes.index(dim)]
-            raw_pad.extend(
-                (
-                    pad_[0].get_dim_value() if isinstance(pad_[0], Dim) else pad_[0],
-                    pad_[1].get_dim_value() if isinstance(pad_[1], Dim) else pad_[1],
-                )
-            )
+            raw_pad += [
+                pad_[0].get_dim_value() if isinstance(pad_[0], Dim) else pad_[0],
+                pad_[1].get_dim_value() if isinstance(pad_[1], Dim) else pad_[1],
+            ]
+            if not remaining_dims:
+                break
         if isinstance(value, Tensor):
             assert value.dims == (), f"value {value} must be a scalar"
             value = value.raw_tensor
         out.raw_tensor = torch.nn.functional.pad(source.raw_tensor, pad=raw_pad, mode=mode, value=value)
         return out
 
     @staticmethod
```

### Comparing `returnn-1.20230512.95100/returnn/torch/frontend/_rand.py` & `returnn-1.20230515.93528/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/torch/frontend/bridge.py` & `returnn-1.20230515.93528/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/torch/updater.py` & `returnn-1.20230515.93528/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/basic.py` & `returnn-1.20230515.93528/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/better_exchook.py` & `returnn-1.20230515.93528/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/bpe.py` & `returnn-1.20230515.93528/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/debug.py` & `returnn-1.20230515.93528/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/debug_helpers.py` & `returnn-1.20230515.93528/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/fsa.py` & `returnn-1.20230515.93528/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230515.93528/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/pprint.py` & `returnn-1.20230515.93528/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/py-to-pickle.cpp` & `returnn-1.20230515.93528/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/sig_proc.py` & `returnn-1.20230515.93528/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn/util/task_system.py` & `returnn-1.20230515.93528/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/returnn.egg-info/PKG-INFO` & `returnn-1.20230515.93528/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230512.95100
+Version: 1.20230515.93528
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230512.95100/returnn.egg-info/SOURCES.txt` & `returnn-1.20230515.93528/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/setup.py` & `returnn-1.20230515.93528/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/DummySprintExec.py` & `returnn-1.20230515.93528/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230515.93528/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230515.93528/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230515.93528/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/_set_num_threads1.py` & `returnn-1.20230515.93528/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/_setup_test_env.py` & `returnn-1.20230515.93528/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/bpe-unicode-demo.codes` & `returnn-1.20230515.93528/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/bpe-unicode-demo.vocab` & `returnn-1.20230515.93528/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/lexicon_opt.isyms` & `returnn-1.20230515.93528/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/lexicon_opt.jpg` & `returnn-1.20230515.93528/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/lint_common.py` & `returnn-1.20230515.93528/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/pycharm-inspect.py` & `returnn-1.20230515.93528/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/pylint.py` & `returnn-1.20230515.93528/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/returnn-as-framework.py` & `returnn-1.20230515.93528/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/rf_utils.py` & `returnn-1.20230515.93528/tests/rf_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,23 @@
 
 def run_model(
     extern_data: TensorDict,
     get_model: rf.GetModelFunc,
     forward_step: rf.StepFunc,
     *,
     dyn_dim_max_sizes: Optional[Dict[Dim, int]] = None,
+    dyn_dim_min_sizes: Optional[Dict[Dim, int]] = None,
     test_tensorflow: bool = True,
 ) -> TensorDict:
     """run"""
     print(f"* run_model with dyn_dim_max_sizes={dyn_dim_max_sizes!r}")
     extern_data.reset_content()
-    tensor_dict_fill_random_numpy_(extern_data, dyn_dim_max_sizes=dyn_dim_max_sizes)
+    tensor_dict_fill_random_numpy_(
+        extern_data, dyn_dim_max_sizes=dyn_dim_max_sizes, dyn_dim_min_sizes=dyn_dim_min_sizes
+    )
 
     print("** run with PyTorch backend")
     with rft.TorchBackend.random_journal_record() as random_journal:
         out_pt = run_model_torch(extern_data, get_model, forward_step)
         _pad_mask_zeros(out_pt)
         # get the values now because dims might get overwritten
         out_pt_raw = out_pt.as_raw_tensor_dict(include_const_sizes=True)
```

### Comparing `returnn-1.20230512.95100/tests/spelling.dic` & `returnn-1.20230515.93528/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_Config.py` & `returnn-1.20230515.93528/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_Dataset.py` & `returnn-1.20230515.93528/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_Fsa.py` & `returnn-1.20230515.93528/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_GeneratingDataset.py` & `returnn-1.20230515.93528/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_HDFDataset.py` & `returnn-1.20230515.93528/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_LearningRateControl.py` & `returnn-1.20230515.93528/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_Log.py` & `returnn-1.20230515.93528/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_MultiProcDataset.py` & `returnn-1.20230515.93528/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_PTDataset.py` & `returnn-1.20230515.93528/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_Pretrain.py` & `returnn-1.20230515.93528/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_ResNet.py` & `returnn-1.20230515.93528/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_SprintDataset.py` & `returnn-1.20230515.93528/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_SprintInterface.py` & `returnn-1.20230515.93528/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TFEngine.py` & `returnn-1.20230515.93528/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TFNativeOp.py` & `returnn-1.20230515.93528/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TFNetworkLayer.py` & `returnn-1.20230515.93528/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230515.93528/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230515.93528/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TFUpdater.py` & `returnn-1.20230515.93528/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TFUtil.py` & `returnn-1.20230515.93528/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TF_determinism.py` & `returnn-1.20230515.93528/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TaskSystem.py` & `returnn-1.20230515.93528/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230515.93528/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_TranslationDataset.py` & `returnn-1.20230515.93528/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_Util.py` & `returnn-1.20230515.93528/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_demos.py` & `returnn-1.20230515.93528/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_fork_exec.py` & `returnn-1.20230515.93528/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_hdf_dump.py` & `returnn-1.20230515.93528/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_rf_array.py` & `returnn-1.20230515.93528/tests/test_rf_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,36 @@
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         out, (new_time, new_feat) = model(extern_data["data"])
         out.mark_as_default_output(shape=(batch_dim, new_time, new_feat))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
 
 
+def test_pad_time():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __call__(self, x: Tensor) -> Tuple[Tensor, Tuple[Dim, Dim]]:
+            pack, (new_time,) = rf.pad(x, axes=[time_dim], padding=[(1, 0)], value=0)
+            return pack, (new_time,)
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out, (new_time,) = model(extern_data["data"])
+        out.mark_as_default_output(shape=(batch_dim, new_time, in_dim))
+
+    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
+
+
 def test_gather():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
     in_dim = Dim(7, name="in")
     extern_data = TensorDict(
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
```

### Comparing `returnn-1.20230512.95100/tests/test_rf_attention.py` & `returnn-1.20230515.93528/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_rf_base.py` & `returnn-1.20230515.93528/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_rf_cond.py` & `returnn-1.20230515.93528/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_rf_container.py` & `returnn-1.20230515.93528/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_rf_conv.py` & `returnn-1.20230515.93528/tests/test_rf_conv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 RETURNN frontend (returnn.frontend) tests
 """
 
 from __future__ import annotations
 from typing import Tuple
+import numpy
 import _setup_test_env  # noqa
 import returnn.frontend as rf
 from returnn.tensor import Tensor, Dim, TensorDict, batch_dim
 from rf_utils import run_model
 
 
 def test_conv1d():
@@ -278,7 +279,44 @@
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         out, out_spatial_dim = model(extern_data["data"], in_spatial_dim=time_dim)
         out.mark_as_default_output(shape=(batch_dim, out_spatial_dim, in_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 7})
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step, dyn_dim_max_sizes={time_dim: 9})
+
+
+def test_maxpool1d_stride_border_cond():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __call__(self, x: rf.Tensor, *, in_spatial_dim: Dim) -> Tuple[Tensor, Dim]:
+            return rf.max_pool1d(x, pool_size=6, strides=3, padding="valid", in_spatial_dim=in_spatial_dim)
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out, out_spatial_dim = model(extern_data["data"], in_spatial_dim=time_dim)
+        out.mark_as_default_output(shape=(batch_dim, out_spatial_dim, in_dim))
+
+    out = run_model(
+        extern_data,
+        lambda *, epoch, step: _Net(),
+        _forward_step,
+        dyn_dim_max_sizes={time_dim: 9},
+        # 2 means we get: ceildiv(2 - 6 + 1, 3) == -1.
+        # So this checks that there is correctly a relu on the size.
+        dyn_dim_min_sizes={time_dim: 2},
+    )
+    out = out["output"]
+    (out_spatial_dim,) = out.get_dyn_size_tags()
+    assert isinstance(out_spatial_dim, Dim)
+    out_sizes = out_spatial_dim.dyn_size_ext.raw_tensor
+    print("out sizes:", out_sizes)
+    assert isinstance(out_sizes, numpy.ndarray)
+    assert min(out_sizes) != max(out_sizes)  # not all the same
+    assert min(out_sizes) == 0
```

### Comparing `returnn-1.20230512.95100/tests/test_rf_encoder_conformer.py` & `returnn-1.20230515.93528/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_rf_loop.py` & `returnn-1.20230515.93528/tests/test_rf_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,26 +53,26 @@
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
     )
 
     class _Net(rf.Module):
         def __call__(self, x: Tensor) -> Tuple[Tensor, Dim]:
-            def _cond(s: Tuple[Tensor, Tensor], _):
+            def _cond(_, s: Tuple[Tensor, Tensor]):
                 t, s_ = s
                 if t.raw_tensor.__class__.__module__.startswith("torch"):
                     print("**", t.raw_tensor, rf.reduce_sum(s_, axis=in_dim).raw_tensor)
                 return rf.logical_and(rf.reduce_sum(s_, axis=in_dim) < 20, t < time_dim.get_dim_value_tensor())
 
-            def _body(s, _):
+            def _body(_, s):
                 t, s_ = s
                 y_ = s_ + rf.abs(rf.gather(x, indices=t, axis=time_dim))
-                return (t + 1, y_), y_
+                return y_, (t + 1, y_)
 
-            _, y, out_time_dim = rf.scan(
+            y, _, out_time_dim = rf.scan(
                 cond=_cond,
                 body=_body,
                 cond_dims=[batch_dim],
                 initial=(rf.zeros((), dtype=rf.get_default_array_index_dtype()), rf.zeros((batch_dim, in_dim))),
                 ys=Tensor("y", dims=(batch_dim, in_dim), dtype=x.dtype),
             )
 
@@ -93,19 +93,19 @@
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
     )
 
     class _Net(rf.Module):
         def __call__(self, x: Tensor) -> Tensor:
-            def _body(s, x_):
+            def _body(x_, s):
                 y_ = s + x_
                 return y_, y_
 
-            _, y, _ = rf.scan(
+            y, _, _ = rf.scan(
                 spatial_dim=time_dim,
                 body=_body,
                 initial=rf.zeros((batch_dim, in_dim)),
                 xs=x,
                 ys=Tensor("y", dims=(batch_dim, in_dim), dtype=x.dtype),
             )
```

### Comparing `returnn-1.20230512.95100/tests/test_rf_math.py` & `returnn-1.20230515.93528/tests/test_rf_math.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,7 +67,28 @@
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         out = model(extern_data["data"])
         out.mark_as_default_output(shape=(batch_dim, time_dim, in_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
+
+
+def test_relu():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __call__(self, x: Tensor) -> Tensor:
+            return rf.relu(x)
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out = model(extern_data["data"])
+        out.mark_as_default_output(shape=(batch_dim, time_dim, in_dim))
+
+    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
```

### Comparing `returnn-1.20230512.95100/tests/test_rf_normalization.py` & `returnn-1.20230515.93528/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_rf_signal.py` & `returnn-1.20230515.93528/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_tensor.py` & `returnn-1.20230515.93528/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_tools.py` & `returnn-1.20230515.93528/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_torch_frontend.py` & `returnn-1.20230515.93528/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tests/test_torch_internal_frontend.py` & `returnn-1.20230515.93528/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/analyze-dataset-batches.py` & `returnn-1.20230515.93528/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/bliss-collect-seq-lens.py` & `returnn-1.20230515.93528/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/bliss-dump-text.py` & `returnn-1.20230515.93528/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/bliss-get-segment-names.py` & `returnn-1.20230515.93528/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/bliss-to-ogg-zip.py` & `returnn-1.20230515.93528/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/bpe-create-lexicon.py` & `returnn-1.20230515.93528/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/calculate-word-error-rate.py` & `returnn-1.20230515.93528/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/cleanup-old-models.py` & `returnn-1.20230515.93528/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/collect-orth-symbols.py` & `returnn-1.20230515.93528/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/collect-words.py` & `returnn-1.20230515.93528/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/compile_native_op.py` & `returnn-1.20230515.93528/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/compile_tf_graph.py` & `returnn-1.20230515.93528/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/debug-dump-search-scores.py` & `returnn-1.20230515.93528/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/debug-plot-search-scores.py` & `returnn-1.20230515.93528/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/dump-dataset-raw-strings.py` & `returnn-1.20230515.93528/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/dump-dataset.py` & `returnn-1.20230515.93528/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/dump-forward-stats.py` & `returnn-1.20230515.93528/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/dump-forward.py` & `returnn-1.20230515.93528/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/dump-network-json.py` & `returnn-1.20230515.93528/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/dump-pickle.py` & `returnn-1.20230515.93528/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/export_to_onnx.py` & `returnn-1.20230515.93528/tools/export_to_onnx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230515.93528/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/get-attention-weights.py` & `returnn-1.20230515.93528/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/get-best-model-epoch.py` & `returnn-1.20230515.93528/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/hdf_dump.py` & `returnn-1.20230515.93528/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230515.93528/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/import-blocks-mt-model.py` & `returnn-1.20230515.93528/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/import-t2t-mt-model.py` & `returnn-1.20230515.93528/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/Makefile` & `returnn-1.20230515.93528/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/README.md` & `returnn-1.20230515.93528/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/example/README.md` & `returnn-1.20230515.93528/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230515.93528/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230515.93528/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230515.93528/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/file.h` & `returnn-1.20230515.93528/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230515.93528/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230515.93528/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/main.cc` & `returnn-1.20230515.93528/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230515.93528/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230515.93528/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230515.93528/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/tf_avg_checkpoints.py` & `returnn-1.20230515.93528/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/tf_inspect_checkpoint.py` & `returnn-1.20230515.93528/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230512.95100/tools/tf_inspect_summary_log.py` & `returnn-1.20230515.93528/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

