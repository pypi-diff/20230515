# Comparing `tmp/yolov5-7.0.8.tar.gz` & `tmp/yolov5-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov5-7.0.8.tar", last modified: Tue Jan 31 20:54:00 2023, max compression
+gzip compressed data, was "yolov5-7.0.9.tar", last modified: Sun Feb 12 19:38:49 2023, max compression
```

## Comparing `yolov5-7.0.8.tar` & `yolov5-7.0.9.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.962799 yolov5-7.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35126 2023-01-31 20:53:51.000000 yolov5-7.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-31 20:53:51.000000 yolov5-7.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-01-31 20:54:00.962799 yolov5-7.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-01-31 20:53:51.000000 yolov5-7.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:54:00.962799 yolov5-7.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-01-31 20:53:51.000000 yolov5-7.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.954799 yolov5-7.0.8/yolov5/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.954799 yolov5-7.0.8/yolov5/classify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/classify/val.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.954799 yolov5-7.0.8/yolov5/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18871 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/coco128.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.954799 yolov5-7.0.8/yolov5/data/hyps/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/hyps/hyp.Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/hyps/hyp.VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/hyps/hyp.no-augmentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/hyps/hyp.scratch-high.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/hyps/hyp.scratch-low.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/hyps/hyp.scratch-med.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.958799 yolov5-7.0.8/yolov5/data/images/
--rw-r--r--   0 runner    (1001) docker     (123)   487438 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/images/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   168949 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/images/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.958799 yolov5-7.0.8/yolov5/data/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/scripts/download_weights.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1566 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/scripts/get_coco.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/scripts/get_coco128.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/scripts/get_imagenet.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/data/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    32064 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/hubconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.958799 yolov5-7.0.8/yolov5/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41762 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.958799 yolov5-7.0.8/yolov5/models/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/anchors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5-bifpn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5-fpn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5-p34.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5-p7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5-panet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5l6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5m6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5n6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5s-LeakyReLU.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5s-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5s-transformer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5s6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/hub/yolov5x6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.958799 yolov5-7.0.8/yolov5/models/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/segment/yolov5l-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/segment/yolov5m-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/segment/yolov5n-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/segment/yolov5s-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/segment/yolov5x-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27044 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/yolov5m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/yolov5n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/yolov5s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/models/yolov5x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.958799 yolov5-7.0.8/yolov5/segment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    36012 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    24320 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/segment/val.py
--rw-r--r--   0 runner    (1001) docker     (123)    37557 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.962799 yolov5-7.0.8/yolov5/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    56639 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    46776 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.962799 yolov5-7.0.8/yolov5/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.962799 yolov5-7.0.8/yolov5/utils/loggers/clearml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/clearml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/clearml/clearml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/clearml/hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.962799 yolov5-7.0.8/yolov5/utils/loggers/comet/
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/comet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/comet/comet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/comet/hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.962799 yolov5-7.0.8/yolov5/utils/loggers/neptune/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/neptune/neptune_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.962799 yolov5-7.0.8/yolov5/utils/loggers/wandb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/wandb/log_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/wandb/sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loggers/wandb/wandb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24571 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/roboflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.962799 yolov5-7.0.8/yolov5/utils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/segment/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/segment/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/segment/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/segment/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/segment/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/segment/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-01-31 20:53:51.000000 yolov5-7.0.8/yolov5/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:54:00.954799 yolov5-7.0.8/yolov5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-01-31 20:54:00.000000 yolov5-7.0.8/yolov5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-01-31 20:54:00.000000 yolov5-7.0.8/yolov5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:54:00.000000 yolov5-7.0.8/yolov5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-31 20:54:00.000000 yolov5-7.0.8/yolov5.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-31 20:54:00.000000 yolov5-7.0.8/yolov5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-31 20:54:00.000000 yolov5-7.0.8/yolov5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.965976 yolov5-7.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35126 2023-02-12 19:38:39.000000 yolov5-7.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-12 19:38:39.000000 yolov5-7.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-02-12 19:38:49.965976 yolov5-7.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-02-12 19:38:39.000000 yolov5-7.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 19:38:49.965976 yolov5-7.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-02-12 19:38:39.000000 yolov5-7.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.953976 yolov5-7.0.9/yolov5/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.957976 yolov5-7.0.9/yolov5/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/classify/val.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.957976 yolov5-7.0.9/yolov5/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18871 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/coco128.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.957976 yolov5-7.0.9/yolov5/data/hyps/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/hyps/hyp.Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/hyps/hyp.VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/hyps/hyp.no-augmentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/hyps/hyp.scratch-high.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/hyps/hyp.scratch-low.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/hyps/hyp.scratch-med.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.957976 yolov5-7.0.9/yolov5/data/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   487438 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/images/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   168949 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/images/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.957976 yolov5-7.0.9/yolov5/data/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/scripts/download_weights.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1566 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/scripts/get_coco.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/scripts/get_coco128.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/scripts/get_imagenet.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/data/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32064 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/hubconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.961976 yolov5-7.0.9/yolov5/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41762 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.961976 yolov5-7.0.9/yolov5/models/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/anchors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5-bifpn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5-fpn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5-p34.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5-p7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5-panet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5l6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5m6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5n6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5s-LeakyReLU.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5s-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5s-transformer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5s6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/hub/yolov5x6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.961976 yolov5-7.0.9/yolov5/models/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/segment/yolov5l-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/segment/yolov5m-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/segment/yolov5n-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/segment/yolov5s-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/segment/yolov5x-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27044 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/yolov5m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/yolov5n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/yolov5s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/models/yolov5x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.961976 yolov5-7.0.9/yolov5/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36012 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24320 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/segment/val.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37557 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.961976 yolov5-7.0.9/yolov5/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56639 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46762 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.961976 yolov5-7.0.9/yolov5/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.965976 yolov5-7.0.9/yolov5/utils/loggers/clearml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/clearml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/clearml/clearml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/clearml/hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.965976 yolov5-7.0.9/yolov5/utils/loggers/comet/
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/comet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/comet/comet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/comet/hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.965976 yolov5-7.0.9/yolov5/utils/loggers/neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/neptune/neptune_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.965976 yolov5-7.0.9/yolov5/utils/loggers/wandb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/wandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/wandb/log_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/wandb/sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loggers/wandb/wandb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24571 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/roboflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.965976 yolov5-7.0.9/yolov5/utils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/segment/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/segment/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/segment/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/segment/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/segment/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/segment/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-02-12 19:38:39.000000 yolov5-7.0.9/yolov5/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 19:38:49.957976 yolov5-7.0.9/yolov5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-02-12 19:38:49.000000 yolov5-7.0.9/yolov5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-02-12 19:38:49.000000 yolov5-7.0.9/yolov5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 19:38:49.000000 yolov5-7.0.9/yolov5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-12 19:38:49.000000 yolov5-7.0.9/yolov5.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-12 19:38:49.000000 yolov5-7.0.9/yolov5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-12 19:38:49.000000 yolov5-7.0.9/yolov5.egg-info/top_level.txt
```

### Comparing `yolov5-7.0.8/LICENSE` & `yolov5-7.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/PKG-INFO` & `yolov5-7.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5
-Version: 7.0.8
+Version: 7.0.9
 Summary: Packaged version of the Yolov5 object detector
 Home-page: https://github.com/fcakyon/yolov5-pip
 Author: 
 License: GPL
 Keywords: machine-learning,deep-learning,ml,pytorch,YOLO,object-detection,vision,YOLOv5,YOLOv7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yolov5 Version: 7.0.8 Summary: Packaged version of
+Metadata-Version: 2.1 Name: yolov5 Version: 7.0.9 Summary: Packaged version of
 the Yolov5 object detector Home-page: https://github.com/fcakyon/yolov5-pip
 Author: License: GPL Keywords: machine-learning,deep-
 learning,ml,pytorch,YOLO,object-detection,vision,YOLOv5,YOLOv7 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License (GPL) Classifier: Operating System :: OS
 Independent Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Programming Language :: Python :: 3
```

### Comparing `yolov5-7.0.8/README.md` & `yolov5-7.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/setup.py` & `yolov5-7.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/benchmarks.py` & `yolov5-7.0.9/yolov5/benchmarks.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/classify/predict.py` & `yolov5-7.0.9/yolov5/classify/predict.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/classify/train.py` & `yolov5-7.0.9/yolov5/classify/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     # Save run settings
     yaml_save(save_dir / 'opt.yaml', vars(opt))
 
     # Logger
     logger = GenericLogger(opt=opt, console_logger=LOGGER) if RANK in {-1, 0} else None
 
     # Download Dataset
-    with torch_distributed_zero_first(LOCAL_RANK), WorkingDirectory(ROOT):
+    with torch_distributed_zero_first(LOCAL_RANK):
         data_dir = data if data.is_dir() else (DATASETS_DIR / data)
         if not data_dir.is_dir():
             LOGGER.info(f'\nDataset not found ⚠️, missing path {data_dir}, attempting download...')
             t = time.time()
             if str(data) == 'imagenet':
                 subprocess.run(f"bash {ROOT / 'data/scripts/get_imagenet.sh'}", shell=True, check=True)
             else:
```

### Comparing `yolov5-7.0.8/yolov5/classify/val.py` & `yolov5-7.0.9/yolov5/classify/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/cli.py` & `yolov5-7.0.9/yolov5/cli.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/Argoverse.yaml` & `yolov5-7.0.9/yolov5/data/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/GlobalWheat2020.yaml` & `yolov5-7.0.9/yolov5/data/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/ImageNet.yaml` & `yolov5-7.0.9/yolov5/data/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/Objects365.yaml` & `yolov5-7.0.9/yolov5/data/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/SKU-110K.yaml` & `yolov5-7.0.9/yolov5/data/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/VOC.yaml` & `yolov5-7.0.9/yolov5/data/VOC.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/VisDrone.yaml` & `yolov5-7.0.9/yolov5/data/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/coco.yaml` & `yolov5-7.0.9/yolov5/data/coco.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/coco128-seg.yaml` & `yolov5-7.0.9/yolov5/data/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/coco128.yaml` & `yolov5-7.0.9/yolov5/data/coco128.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/hyps/hyp.Objects365.yaml` & `yolov5-7.0.9/yolov5/data/hyps/hyp.Objects365.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/hyps/hyp.VOC.yaml` & `yolov5-7.0.9/yolov5/data/hyps/hyp.VOC.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/hyps/hyp.no-augmentation.yaml` & `yolov5-7.0.9/yolov5/data/hyps/hyp.no-augmentation.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/hyps/hyp.scratch-high.yaml` & `yolov5-7.0.9/yolov5/data/hyps/hyp.scratch-high.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/hyps/hyp.scratch-low.yaml` & `yolov5-7.0.9/yolov5/data/hyps/hyp.scratch-low.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/hyps/hyp.scratch-med.yaml` & `yolov5-7.0.9/yolov5/data/hyps/hyp.scratch-med.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/images/bus.jpg` & `yolov5-7.0.9/yolov5/data/images/bus.jpg`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/images/zidane.jpg` & `yolov5-7.0.9/yolov5/data/images/zidane.jpg`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/scripts/download_weights.sh` & `yolov5-7.0.9/yolov5/data/scripts/download_weights.sh`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/scripts/get_coco.sh` & `yolov5-7.0.9/yolov5/data/scripts/get_coco.sh`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/scripts/get_coco128.sh` & `yolov5-7.0.9/yolov5/data/scripts/get_coco128.sh`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/scripts/get_imagenet.sh` & `yolov5-7.0.9/yolov5/data/scripts/get_imagenet.sh`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/data/xView.yaml` & `yolov5-7.0.9/yolov5/data/xView.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/detect.py` & `yolov5-7.0.9/yolov5/detect.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/export.py` & `yolov5-7.0.9/yolov5/export.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/helpers.py` & `yolov5-7.0.9/yolov5/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,18 +394,24 @@
     if has_yolo_s3_data_dir and opt.upload_dataset:
         raise ValueError(
             "'--upload_dataset' argument cannot be passed when 'yolo_s3_data_dir' field is not empty in 'data.yaml'."
         )
 
     if is_coco_data:
         from sahi.utils.coco import export_coco_as_yolov5_via_yml
-
-        data = export_coco_as_yolov5_via_yml(
-            yml_path=opt.data, output_dir=save_dir / "data"
-        )
+        from sahi.utils.file import is_colab
+        
+        if is_colab():
+            data = export_coco_as_yolov5_via_yml(
+            yml_path=opt.data, output_dir=save_dir / "data", disable_symlink=True
+        )   
+        else:     
+            data = export_coco_as_yolov5_via_yml(
+                yml_path=opt.data, output_dir=save_dir / "data"
+            )
         opt.data = data
 
         # add coco fields to data.yaml
         with open(data, errors="ignore") as f:
             updated_data_info = yaml.safe_load(f)  # load data dict
             updated_data_info["train_json_path"] = data_info["train_json_path"]
             updated_data_info["val_json_path"] = data_info["val_json_path"]
@@ -429,14 +435,15 @@
             copyfile(data_info["train_json_path"], str(w / "train.json"))
         if "val_json_path" in data_info and Path(data_info["val_json_path"]).is_file():
             copyfile(data_info["val_json_path"], str(w / "val.json"))
 
 
 def upload_to_s3(opt, data, save_dir):
     import yaml
+    import os
     from yolov5.utils.general import colorstr
     from yolov5.utils.aws import upload_file_to_s3, upload_folder_to_s3
 
     with open(data, errors="ignore") as f:
         data_info = yaml.safe_load(f)  # load data dict
     # upload yolo formatted data to s3
     s3_folder = "s3://" + str(
```

### Comparing `yolov5-7.0.8/yolov5/hubconf.py` & `yolov5-7.0.9/yolov5/hubconf.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/common.py` & `yolov5-7.0.9/yolov5/models/common.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/experimental.py` & `yolov5-7.0.9/yolov5/models/experimental.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/anchors.yaml` & `yolov5-7.0.9/yolov5/models/hub/anchors.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov3-spp.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov3-tiny.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov3.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5-bifpn.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5-bifpn.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5-fpn.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5-fpn.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5-p2.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5-p2.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5-p34.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5-p34.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5-p6.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5-p7.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5-p7.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5-panet.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5-panet.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5l6.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5l6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5m6.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5m6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5n6.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5n6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5s-LeakyReLU.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5s-LeakyReLU.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5s-ghost.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5s-ghost.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5s-transformer.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5s-transformer.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5s6.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5s6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/hub/yolov5x6.yaml` & `yolov5-7.0.9/yolov5/models/hub/yolov5x6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/segment/yolov5l-seg.yaml` & `yolov5-7.0.9/yolov5/models/segment/yolov5l-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/segment/yolov5m-seg.yaml` & `yolov5-7.0.9/yolov5/models/segment/yolov5m-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/segment/yolov5n-seg.yaml` & `yolov5-7.0.9/yolov5/models/segment/yolov5n-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/segment/yolov5s-seg.yaml` & `yolov5-7.0.9/yolov5/models/segment/yolov5s-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/segment/yolov5x-seg.yaml` & `yolov5-7.0.9/yolov5/models/segment/yolov5x-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/tf.py` & `yolov5-7.0.9/yolov5/models/tf.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/yolo.py` & `yolov5-7.0.9/yolov5/models/yolo.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/yolov5l.yaml` & `yolov5-7.0.9/yolov5/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/yolov5m.yaml` & `yolov5-7.0.9/yolov5/models/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/yolov5n.yaml` & `yolov5-7.0.9/yolov5/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/yolov5s.yaml` & `yolov5-7.0.9/yolov5/models/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/models/yolov5x.yaml` & `yolov5-7.0.9/yolov5/models/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/segment/predict.py` & `yolov5-7.0.9/yolov5/segment/predict.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/segment/train.py` & `yolov5-7.0.9/yolov5/segment/train.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/segment/val.py` & `yolov5-7.0.9/yolov5/segment/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/train.py` & `yolov5-7.0.9/yolov5/train.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/__init__.py` & `yolov5-7.0.9/yolov5/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/activations.py` & `yolov5-7.0.9/yolov5/utils/activations.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/augmentations.py` & `yolov5-7.0.9/yolov5/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/autoanchor.py` & `yolov5-7.0.9/yolov5/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/autobatch.py` & `yolov5-7.0.9/yolov5/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/aws.py` & `yolov5-7.0.9/yolov5/utils/aws.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/callbacks.py` & `yolov5-7.0.9/yolov5/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/dataloaders.py` & `yolov5-7.0.9/yolov5/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/downloads.py` & `yolov5-7.0.9/yolov5/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/general.py` & `yolov5-7.0.9/yolov5/utils/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 FILE = Path(__file__).resolve()
 ROOT = FILE.parents[1]  # YOLOv5 root directory
 RANK = int(os.getenv('RANK', -1))
 
 # Settings
 NUM_THREADS = min(8, max(1, os.cpu_count() - 1))  # number of YOLOv5 multiprocessing threads
-DATASETS_DIR = Path(os.getenv('YOLOv5_DATASETS_DIR', ROOT.parent / 'datasets'))  # global datasets directory
+DATASETS_DIR = Path(os.getenv('YOLOv5_DATASETS_DIR', 'datasets'))  # global datasets directory
 AUTOINSTALL = str(os.getenv('YOLOv5_AUTOINSTALL', True)).lower() == 'true'  # global auto-install mode
 VERBOSE = str(os.getenv('YOLOv5_VERBOSE', True)).lower() == 'true'  # global verbose mode
 TQDM_BAR_FORMAT = '{l_bar}{bar:10}{r_bar}'  # tqdm bar format
 FONT = 'Arial.ttf'  # https://ultralytics.com/assets/Arial.ttf
 
 torch.set_printoptions(linewidth=320, precision=5, profile='long')
 np.set_printoptions(linewidth=320, formatter={'float_kind': '{:11.5g}'.format})  # format short g, %precision=5
```

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/__init__.py` & `yolov5-7.0.9/yolov5/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/clearml/clearml_utils.py` & `yolov5-7.0.9/yolov5/utils/loggers/clearml/clearml_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/clearml/hpo.py` & `yolov5-7.0.9/yolov5/utils/loggers/clearml/hpo.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/comet/__init__.py` & `yolov5-7.0.9/yolov5/utils/loggers/comet/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/comet/comet_utils.py` & `yolov5-7.0.9/yolov5/utils/loggers/comet/comet_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/comet/hpo.py` & `yolov5-7.0.9/yolov5/utils/loggers/comet/hpo.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/neptune/neptune_utils.py` & `yolov5-7.0.9/yolov5/utils/loggers/neptune/neptune_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/wandb/log_dataset.py` & `yolov5-7.0.9/yolov5/utils/loggers/wandb/log_dataset.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/wandb/sweep.py` & `yolov5-7.0.9/yolov5/utils/loggers/wandb/sweep.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loggers/wandb/wandb_utils.py` & `yolov5-7.0.9/yolov5/utils/loggers/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/loss.py` & `yolov5-7.0.9/yolov5/utils/loss.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/metrics.py` & `yolov5-7.0.9/yolov5/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/plots.py` & `yolov5-7.0.9/yolov5/utils/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/roboflow.py` & `yolov5-7.0.9/yolov5/utils/roboflow.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/segment/augmentations.py` & `yolov5-7.0.9/yolov5/utils/segment/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/segment/dataloaders.py` & `yolov5-7.0.9/yolov5/utils/segment/dataloaders.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/segment/general.py` & `yolov5-7.0.9/yolov5/utils/segment/general.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/segment/loss.py` & `yolov5-7.0.9/yolov5/utils/segment/loss.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/segment/metrics.py` & `yolov5-7.0.9/yolov5/utils/segment/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/segment/plots.py` & `yolov5-7.0.9/yolov5/utils/segment/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/torch_utils.py` & `yolov5-7.0.9/yolov5/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/utils/triton.py` & `yolov5-7.0.9/yolov5/utils/triton.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5/val.py` & `yolov5-7.0.9/yolov5/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-7.0.8/yolov5.egg-info/PKG-INFO` & `yolov5-7.0.9/yolov5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5
-Version: 7.0.8
+Version: 7.0.9
 Summary: Packaged version of the Yolov5 object detector
 Home-page: https://github.com/fcakyon/yolov5-pip
 Author: 
 License: GPL
 Keywords: machine-learning,deep-learning,ml,pytorch,YOLO,object-detection,vision,YOLOv5,YOLOv7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yolov5 Version: 7.0.8 Summary: Packaged version of
+Metadata-Version: 2.1 Name: yolov5 Version: 7.0.9 Summary: Packaged version of
 the Yolov5 object detector Home-page: https://github.com/fcakyon/yolov5-pip
 Author: License: GPL Keywords: machine-learning,deep-
 learning,ml,pytorch,YOLO,object-detection,vision,YOLOv5,YOLOv7 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License (GPL) Classifier: Operating System :: OS
 Independent Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Programming Language :: Python :: 3
```

### Comparing `yolov5-7.0.8/yolov5.egg-info/SOURCES.txt` & `yolov5-7.0.9/yolov5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

