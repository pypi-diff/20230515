# Comparing `tmp/pai-easycv-0.8.0.tar.gz` & `tmp/pai-easycv-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pai-easycv-0.8.0.tar", last modified: Tue Dec  6 03:04:31 2022, max compression
+gzip compressed data, was "dist/pai-easycv-0.9.0.tar", last modified: Tue Jan 17 02:44:07 2023, max compression
```

## Comparing `pai-easycv-0.8.0.tar` & `pai-easycv-0.9.0.tar`

### file list

```diff
@@ -1,1016 +1,1070 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)    12734 2022-12-06 03:04:30.000000 pai-easycv-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    15463 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      181 2022-12-06 03:04:30.000000 pai-easycv-0.8.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/
--rw-r--r--   0 runner    (1001) docker     (122)     2282 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/selfsup/
--rw-r--r--   0 runner    (1001) docker     (122)     3528 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/simclr.py
--rw-r--r--   0 runner    (1001) docker     (122)    10485 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/moby.py
--rw-r--r--   0 runner    (1001) docker     (122)     2731 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/mae.py
--rw-r--r--   0 runner    (1001) docker     (122)    14559 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/dino.py
--rw-r--r--   0 runner    (1001) docker     (122)     8571 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/swav.py
--rw-r--r--   0 runner    (1001) docker     (122)      259 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8312 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/moco.py
--rw-r--r--   0 runner    (1001) docker     (122)     3540 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/byol.py
--rw-r--r--   0 runner    (1001) docker     (122)     3724 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/mixco.py
--rw-r--r--   0 runner    (1001) docker     (122)    20903 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/selfsup/necks.py
--rw-r--r--   0 runner    (1001) docker     (122)      657 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)    18522 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/modelzoo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/face/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3532 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/face/face_keypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/face/head/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/face/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1639 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/face/head/face_keypoint_pose_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/face/head/face_keypoint_head.py
--rw-r--r--   0 runner    (1001) docker     (122)      468 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (122)    16230 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/mask2former.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13523 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/segmentation/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      233 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/utils/shape_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7453 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     4313 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/utils/point_rend.py
--rw-r--r--   0 runner    (1001) docker     (122)    12316 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/utils/embed.py
--rw-r--r--   0 runner    (1001) docker     (122)    14284 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/utils/criterion.py
--rw-r--r--   0 runner    (1001) docker     (122)     3069 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/utils/panoptic_gt_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/
--rw-r--r--   0 runner    (1001) docker     (122)    18696 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/transformer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     3462 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     6819 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/segformer_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/mask2former_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    17151 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/pixel_decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)      271 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6499 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/uper_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    11026 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/segmentation/heads/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/pose/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8627 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/pose/top_down.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/pose/heads/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/pose/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13007 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/pose/heads/topdown_heatmap_simple_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/pose/heads/topdown_heatmap_base_head.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/loss/
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    12544 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/iou_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/loss/set_criterion/
--rw-r--r--   0 runner    (1001) docker     (122)    26009 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/set_criterion/set_criterion.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/set_criterion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5046 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/set_criterion/matcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     3853 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/ocr_rec_multi_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    13973 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     8685 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1388 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3454 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9157 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/pytorch_metric_learning.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/face_keypoint_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     7657 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/det_db_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    16221 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/loss/focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/dense_heads/
--rw-r--r--   0 runner    (1001) docker     (122)     8513 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/dense_heads/dense_test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/dense_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14069 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/dense_heads/anchor_free_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    23284 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/dense_heads/base_dense_head.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/necks/
--rw-r--r--   0 runner    (1001) docker     (122)     8849 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4714 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/necks/sfp.py
--rw-r--r--   0 runner    (1001) docker     (122)       42 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/detr/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/detr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5823 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/detr/detr_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    13710 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/detr/detr_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/fcos/
--rw-r--r--   0 runner    (1001) docker     (122)    37216 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/fcos/fcos_head.py
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/fcos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dino/
--rw-r--r--   0 runner    (1001) docker     (122)    24332 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dino/dino_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    48085 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dino/deformable_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8062 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dino/cdn_components.py
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/
--rw-r--r--   0 runner    (1001) docker     (122)    25373 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/yolo_head_template.py
--rw-r--r--   0 runner    (1001) docker     (122)    11675 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/yolo_pafpn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4616 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/yolo_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     6950 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/asff.py
--rw-r--r--   0 runner    (1001) docker     (122)     7900 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/yolox.py
--rw-r--r--   0 runner    (1001) docker     (122)     9205 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/tood_head.py
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5145 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/detection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox_edge/
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox_edge/yolox_edge.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/yolox_edge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/
--rw-r--r--   0 runner    (1001) docker     (122)    11710 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/dab_detr_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     7522 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/dn_components.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21005 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/attention.py
--rw-r--r--   0 runner    (1001) docker     (122)    19793 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/dab_detr_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (122)    17199 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/utils/boxes.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9364 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/utils/generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6568 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/utils/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     8843 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/ocr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/ocr/postprocess/
--rw-r--r--   0 runner    (1001) docker     (122)     7561 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/postprocess/rec_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7148 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/postprocess/db_postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/ocr/necks/
--rw-r--r--   0 runner    (1001) docker     (122)    10417 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/necks/db_fpn.py
--rw-r--r--   0 runner    (1001) docker     (122)     6963 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/necks/squence_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      248 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/ocr/cls/
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/cls/text_classifier.py
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/cls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/ocr/backbones/
--rw-r--r--   0 runner    (1001) docker     (122)    18720 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/backbones/rec_svtrnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     6904 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/backbones/rec_mv1_enhance.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5186 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/backbones/rec_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (122)     8753 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/backbones/det_resnet_vd.py
--rw-r--r--   0 runner    (1001) docker     (122)    10728 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/backbones/det_mobilenet_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/ocr/rec/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/rec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/rec/ocr_rec.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/ocr/det/
--rw-r--r--   0 runner    (1001) docker     (122)     5119 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/det/db_net.py
--rw-r--r--   0 runner    (1001) docker     (122)       76 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/det/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/ocr/heads/
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/heads/db_head.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16723 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/ocr/heads/rec_head.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (122)    12926 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/inceptionv3.py
--rw-r--r--   0 runner    (1001) docker     (122)      890 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/benchmark_mlp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/mae_vit_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)    35873 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/swin_transformer_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (122)    14289 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/conv_vitdet.py
--rw-r--r--   0 runner    (1001) docker     (122)    20443 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    27124 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)    12540 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6118 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (122)    13098 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/resnet_jit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11084 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/vit_transformer_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (122)    17626 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/shuffle_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6921 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (122)      982 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14519 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/edgevit.py
--rw-r--r--   0 runner    (1001) docker     (122)    57326 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/genet.py
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/face_keypoint_backbone.py
--rw-r--r--   0 runner    (1001) docker     (122)    17270 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/mit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6937 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/darknet.py
--rw-r--r--   0 runner    (1001) docker     (122)    17039 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/vitdet.py
--rw-r--r--   0 runner    (1001) docker     (122)    16886 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/conv_mae_vit.py
--rw-r--r--   0 runner    (1001) docker     (122)    15666 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/efficientformer.py
--rw-r--r--   0 runner    (1001) docker     (122)    29413 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    12473 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/repvgg_yolox_backbone.py
--rw-r--r--   0 runner    (1001) docker     (122)    36277 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/lighthrnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     6072 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/mnasnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     9935 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/network_blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)    46977 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/bninception.py
--rw-r--r--   0 runner    (1001) docker     (122)    22322 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/xcit_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8314 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/pytorch_image_models_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    20173 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/backbones/resnest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection3d/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/
--rw-r--r--   0 runner    (1001) docker     (122)    34758 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/bevformer_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    40003 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)      898 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/attentions/
--rw-r--r--   0 runner    (1001) docker     (122)    14781 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/attentions/multi_scale_deformable_attention.py
--rw-r--r--   0 runner    (1001) docker     (122)    11808 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/attentions/temporal_self_attention.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/attentions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7132 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/attentions/spatial_cross_attention.py
--rw-r--r--   0 runner    (1001) docker     (122)    18171 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/bevformer.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20990 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/mvx_two_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     4919 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/detection3d/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/detection3d/utils/grid_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11367 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (122)    11813 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/classification/necks.py
--rw-r--r--   0 runner    (1001) docker     (122)     7260 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      867 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/sobel.py
--rw-r--r--   0 runner    (1001) docker     (122)     3819 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/norm.py
--rw-r--r--   0 runner    (1001) docker     (122)    29286 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1385 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (122)     7779 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/face_keypoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4002 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3233 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6240 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (122)      364 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/scale.py
--rw-r--r--   0 runner    (1001) docker     (122)     3360 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/multi_pooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/init_weights.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/activation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3261 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (122)      676 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/utils/gather_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/models/heads/
--rw-r--r--   0 runner    (1001) docker     (122)     9252 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/heads/mp_metric_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     2754 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/heads/multi_cls_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/heads/cls_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/heads/latent_pred_head.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/models/heads/contrastive_head.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/points/
--rw-r--r--   0 runner    (1001) docker     (122)     2525 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/points/cam_points.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/points/depth_points.py
--rw-r--r--   0 runner    (1001) docker     (122)    16651 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/points/base_points.py
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/points/lidar_points.py
--rw-r--r--   0 runner    (1001) docker     (122)     9426 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/standard_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/sailfish/
--rw-r--r--   0 runner    (1001) docker     (122)     6154 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/sailfish/linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     7831 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/sailfish/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/sailfish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5663 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/sailfish/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/sailfish/activation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10298 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/sailfish/function.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/bbox/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/bbox/coders/
--rw-r--r--   0 runner    (1001) docker     (122)      187 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/coders/nms_free_coder.py
--rw-r--r--   0 runner    (1001) docker     (122)      546 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/coders/base_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (122)      601 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/
--rw-r--r--   0 runner    (1001) docker     (122)    13795 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/cam_box3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     7215 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/box_3d_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)    10850 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/depth_box3d.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11833 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8164 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/lidar_box3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     9189 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/coord_3d_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)    21406 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/structures/base_box3d.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/bbox/assigners/
--rw-r--r--   0 runner    (1001) docker     (122)      429 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/assigners/base_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/assigners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7812 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/assigners/assign_result.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6398 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/assigners/hungarian_assigner_3d.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/bbox/match_costs/
--rw-r--r--   0 runner    (1001) docker     (122)      336 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/match_costs/builder.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5862 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/match_costs/match_cost.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/match_costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13901 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/bbox_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/bbox/iou_calculators/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/iou_calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7373 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/iou_calculators/iou2d_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/bbox/samplers/
--rw-r--r--   0 runner    (1001) docker     (122)     3974 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1532 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/samplers/pseudo_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5440 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/bbox/samplers/sampling_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)    11386 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (122)      180 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4879 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/visualization/image_3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    18442 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/visualization/open3d_vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/anchor/
--rw-r--r--   0 runner    (1001) docker     (122)      644 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/anchor/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)    10789 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/anchor/point_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/anchor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/optimizer/
--rw-r--r--   0 runner    (1001) docker     (122)      202 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     8589 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/optimizer/ranger.py
--rw-r--r--   0 runner    (1001) docker     (122)      374 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4792 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/optimizer/adam.py
--rw-r--r--   0 runner    (1001) docker     (122)     3853 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/optimizer/layer_decay_optimizer_constructor.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (122)     4510 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/optimizer/lars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/face_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)    39521 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/coco_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)      589 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)    22075 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/top_down_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/evaluation/custom_cocotools/
--rw-r--r--   0 runner    (1001) docker     (122)    42040 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/custom_cocotools/cocoeval.py
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/custom_cocotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/auc_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     4716 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/keypoint_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     4945 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/wholebody_keypoint_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6056 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/classification_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     8252 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/faceid_pair_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     7480 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    51790 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/coco_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (122)    11165 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/segmentation_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/base_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (122)     9679 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/ocr_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     1815 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/mse_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     7840 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/retrival_topk_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)    33656 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/nuscenes_eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     1815 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/evaluation/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/utils/
--rw-r--r--   0 runner    (1001) docker     (122)    13267 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/utils/array_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3944 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/core/post_processing/
--rw-r--r--   0 runner    (1001) docker     (122)     6820 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/post_processing/merge_augs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10780 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/post_processing/box3d_nms.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/post_processing/nms.py
--rw-r--r--   0 runner    (1001) docker     (122)    12225 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/core/post_processing/pose_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mocov2/
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_tfrecord.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/swav/
--rw-r--r--   0 runner    (1001) docker     (122)     3078 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/swav/swav_genet_8xb32_200e_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/swav/swav_rn50_8xb32_200e_tfrecord.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/fast_convmae/
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/fast_convmae/fast_convmae_vit_base_patch16_8xb64_50e.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/dino/
--rw-r--r--   0 runner    (1001) docker     (122)     5236 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     4028 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_tfrecord.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/simclr/
--rw-r--r--   0 runner    (1001) docker     (122)     2364 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/simclr/simclr_rn50_mocov2_neck_8xb32_200e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2400 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mixco/
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mixco/mixco_genet_8xb32_200e_tfrecord_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mixco/mixco_rn50_4xb64_200e_tfrecord_oss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/moby/
--rw-r--r--   0 runner    (1001) docker     (122)     2432 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/moby/moby_dynamic_swin_tiny_8xb64_300e_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/moby/moby_rn50_4xb128_100e_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     3202 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/moby/moby_deit_small_p16_4xb128_300e_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     2603 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/moby/moby_deit_small_4xb32_100e_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/byol/
--rw-r--r--   0 runner    (1001) docker     (122)     3512 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/byol/byol_rn50_8xb32_200e.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mae/
--rw-r--r--   0 runner    (1001) docker     (122)       88 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mae/mae_vit_base_patch16_8xb64_400e.py
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mae/mae_vit_base_patch16_8xb64_1600e.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/selfsup/mae/mae_vit_large_patch16_8xb32_1600e.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/edge_models/
--rw-r--r--   0 runner    (1001) docker     (122)     5487 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/edge_models/yolox_m.py
--rw-r--r--   0 runner    (1001) docker     (122)     5485 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/edge_models/yolox_l.py
--rw-r--r--   0 runner    (1001) docker     (122)     5339 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/edge_models/yolox_nano.py
--rw-r--r--   0 runner    (1001) docker     (122)     5340 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/edge_models/yolox_tiny.py
--rw-r--r--   0 runner    (1001) docker     (122)     6055 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/edge_models/yolox_edge.py
--rw-r--r--   0 runner    (1001) docker     (122)     5485 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/edge_models/yolox_s.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/face/
--rw-r--r--   0 runner    (1001) docker     (122)     8821 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/face/face_96x96_wingloss.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/segmentation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/segmentation/mask2former/
--rw-r--r--   0 runner    (1001) docker     (122)     8058 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_instance.py
--rw-r--r--   0 runner    (1001) docker     (122)     9875 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e127_semantic.py
--rw-r--r--   0 runner    (1001) docker     (122)    10421 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_panoptic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/segmentation/segformer/
--rw-r--r--   0 runner    (1001) docker     (122)    10276 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/segformer/segformer_b0_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     1842 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/segformer/segformer_b5_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      347 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/segformer/segformer_b2_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      348 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/segformer/segformer_b3_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      348 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/segformer/segformer_b4_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/segformer/segformer_b1_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/segmentation/upernet/
--rw-r--r--   0 runner    (1001) docker     (122)     5278 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/upernet/upernet_r50_512x512_8xb4_60e_voc12aug.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/segmentation/fcn/
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/segmentation/fcn/fcn_r50-d8_512x512_8xb4_60e_voc12aug.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/pose/
--rw-r--r--   0 runner    (1001) docker     (122)     5990 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/pose/hrnet_w48_coco_256x192_udp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5483 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/pose/litehrnet_30_coco_384x288.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/pose/hand/
--rw-r--r--   0 runner    (1001) docker     (122)     5866 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/pose/hand/hrnet_w18_coco_wholebody_hand_256x256_dark.py
--rw-r--r--   0 runner    (1001) docker     (122)     5359 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/pose/hand/litehrnet_30_coco_wholebody_hand_256x256.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/pose/wholebody/
--rw-r--r--   0 runner    (1001) docker     (122)     5807 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/pose/wholebody/hrnet_w48_coco_wholebody_384x288_dark_plus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/detr/
--rw-r--r--   0 runner    (1001) docker     (122)     1085 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/detr/detr.py
--rw-r--r--   0 runner    (1001) docker     (122)      519 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/detr/detr_r50_8x2_150e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/fcos/
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/fcos/fcos.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/fcos/coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/fcos/fcos_r50_caffe_1x_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      642 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/fcos/fcos_r50_torch_1x_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_swinl_36e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      119 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_r50_24e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_r50_36e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     2991 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_r50.py
--rw-r--r--   0 runner    (1001) docker     (122)      245 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_swinl.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_swinl_center_iou_memoryreduce_18e_obj2coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      121 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_swinl_24e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_schedule_1x.py
--rw-r--r--   0 runner    (1001) docker     (122)      798 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_swinl_center_iou_memoryreduce_26e_obj365.py
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_r50_36e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_swinl_36e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      119 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_r50_24e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      121 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_swinl_24e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      115 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_swinl_12e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_r50_12e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     3152 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_swinl.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_r50.py
--rw-r--r--   0 runner    (1001) docker     (122)      115 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_swinl_12e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_r50_12e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (122)     4178 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_tiny_8xb16_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     5611 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/pai_yoloxs_8xb16_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_m_8xb16_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     5609 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/pai_yoloxs_asff_8xb16_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_nano_8xb16_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco_pai.py
--rw-r--r--   0 runner    (1001) docker     (122)     5805 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      256 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_l_8xb8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     2612 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_voc.py
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/pai_yoloxs_asff_tood3_8xb16_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      256 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_x_8xb8_300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/common/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/common/dataset/
--rw-r--r--   0 runner    (1001) docker     (122)     5111 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/common/dataset/autoaug_coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     8826 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/common/dataset/autoaug_obj365_val5k_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     5138 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/common/dataset/autoaug_obj2coco_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_mask_rcnn_100e.py
--rw-r--r--   0 runner    (1001) docker     (122)     4280 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4199 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/lsj_coco_instance.py
--rw-r--r--   0 runner    (1001) docker     (122)      660 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_schedule_100e.py
--rw-r--r--   0 runner    (1001) docker     (122)     4868 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_mask_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4112 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/lsj_coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7931 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_cascade_mask_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_cascade_mask_rcnn_100e.py
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_faster_rcnn_100e.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/mask_rcnn/
--rw-r--r--   0 runner    (1001) docker     (122)     4675 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/mask_rcnn/mask_rcnn_r50_fpn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection/dab_detr/
--rw-r--r--   0 runner    (1001) docker     (122)      185 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dab_detr/dn_detr_r50_8x2_50e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dab_detr/dab_detr_r50_8x2_50e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dab_detr/dn_detr_r50_dc5_8x2_50e_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection/dab_detr/dab_detr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/ocr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/ocr/direction/
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/direction/direction_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_te.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_en.py
--rw-r--r--   0 runner    (1001) docker     (122)     3913 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_ch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_devanagari.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_ka.py
--rw-r--r--   0 runner    (1001) docker     (122)     1615 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_cyrillic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_chinese_cht.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_latin.py
--rw-r--r--   0 runner    (1001) docker     (122)     3797 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_arabic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_japan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_ta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1559 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_korean.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/ocr/detection/
--rw-r--r--   0 runner    (1001) docker     (122)     4108 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/detection/det_model_en.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/detection/det_model_ch_r50.py
--rw-r--r--   0 runner    (1001) docker     (122)     3991 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/detection/det_model_ch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/ocr/detection/det_model_en_r50.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/config_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     5679 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/yolox_itag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/swav_r50_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/topdown_litehrnet_30.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/yolox_edge.py
--rw-r--r--   0 runner    (1001) docker     (122)     2814 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/moco_r50_tfrecord_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     6149 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/yolox.py
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/moco_r50_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/mae_vit_base_patch16.py
--rw-r--r--   0 runner    (1001) docker     (122)     3071 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/dino_timm.py
--rw-r--r--   0 runner    (1001) docker     (122)     6301 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/topdown_hrnet_w48_udp.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/moco_timm_tfrecord_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     3494 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/moby_timm_tfrecord_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     9578 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/classification.py
--rw-r--r--   0 runner    (1001) docker     (122)    10447 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/classification_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)    10057 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/classification_tfrecord_oss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/config_templates/metric_learning/
--rw-r--r--   0 runner    (1001) docker     (122)     5972 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/metric_learning/softmaxbased_tfrecord_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/metric_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5697 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/metric_learning/modelparallel_softmaxbased_tfrecord_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/dino_timm_tfrecord_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2511 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/moco_timm_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     3521 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/swav_r50_tfrecord_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     5411 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/yolox_edge_itag.py
--rw-r--r--   0 runner    (1001) docker     (122)     4236 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/config_templates/dino_rn50_tfrecord_oss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection3d/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/detection3d/bevformer/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection3d/bevformer/bevformer_tiny_r50_nuscenes_fp16.py
--rw-r--r--   0 runner    (1001) docker     (122)    11256 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (122)    11556 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection3d/bevformer/bevformer_tiny_r50_nuscenes.py
--rw-r--r--   0 runner    (1001) docker     (122)    11391 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/imagenet_resnet50_1000kid_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/common/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/common/metriclearning_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/common/dataset/
--rw-r--r--   0 runner    (1001) docker     (122)     9358 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/common/dataset/imagenet_metriclearning.py
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/imagenet_timm_softmaxbased_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/cub_resnet50_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/imagenet_resnet50_1000kid_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     4480 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/sop_timm_swinb_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/metric_learning/imagenet_timm_modelparallel_softmaxbased_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/mlp-mixer/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/mlp-mixer/mixer_l16_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/mlp-mixer/mixer_b16_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/twins/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/twins/twins_svt_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/twins/twins_svt_large.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/twins/twins_svt_small.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/resmlp/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/resmlp/resmlp_12_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/resmlp/resmlp_big_24_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/resmlp/resmlp_24_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/resmlp/resmlp_36_distilled_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/deit/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/deit/deit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      121 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/deit/deit_base_distilled_patch16_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/shuffle_transformer/
--rw-r--r--   0 runner    (1001) docker     (122)      118 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/shuffle_transformer/shuffletrans_small_p4_w7_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/shuffle_transformer/shuffletrans_tiny_p4_w7_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/shuffle_transformer/shuffletrans_base_p4_w7_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/gmlp/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/gmlp/gmlp_s16_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/poolformer/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_m48.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_m36.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_s24.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_s12.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_s36.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/pit/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/pit/pit_s_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      109 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/pit/pit_b_distilled_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/nest/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/nest/jx_nest_tiny.py
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/nest/jx_nest_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/nest/jx_nest_small.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/xcit/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/xcit/xcit_medium_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/xcit/xcit_medium_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      115 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/xcit/xcit_large_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/xcit/xcit_large_24_p8_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/coat/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/coat/coat_tiny.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/coat/coat_mini.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/tnt/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/tnt/tnt_s_patch16_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convnext/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convnext/convnext_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convnext/convnext_small.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convnext/convnext_large.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convnext/convnext_tiny.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/gmixer/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/gmixer/gmixer_24_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/sequencer/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/sequencer/sequencer2d_l.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/sequencer/sequencer2d_s.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/sequencer/sequencer2d_m.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/levit/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/levit/levit_256.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/levit/levit_192.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/levit/levit_128.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/cait/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/cait/cait_xxs36_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/cait/cait_s24_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/cait/cait_xxs24_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/swint/
--rw-r--r--   0 runner    (1001) docker     (122)      118 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/swint/dynamic_swin_small_p4_w7_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/swint/dynamic_swin_tiny_p4_w7_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/swint/swin_base_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      119 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/swint/swin_large_patch4_window7_224.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/vit/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/vit/vit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/vit/vit_large_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (122)     2814 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/timm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/crossvit/
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/crossvit/crossvit_small_240.py
--rw-r--r--   0 runner    (1001) docker     (122)      107 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/crossvit/crossvit_base_240.py
--rw-r--r--   0 runner    (1001) docker     (122)      107 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/crossvit/crossvit_tiny_240.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convmixer/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convmixer/convmixer_1536_20.py
--rw-r--r--   0 runner    (1001) docker     (122)      115 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convmixer/convmixer_1024_20_ks9_p14.py
--rw-r--r--   0 runner    (1001) docker     (122)      106 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convmixer/convmixer_768_32.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/mobilevit/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/mobilevit/mobilevit_xxs.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/mobilevit/mobilevit_s.py
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/mobilevit/mobilevit_xs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convit/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convit/convit_small.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convit/convit_tiny.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/convit/convit_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/
--rw-r--r--   0 runner    (1001) docker     (122)      758 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/deit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/imagenet_deit_base_hydra_layer8_patch16_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/deit_schedule.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/imagenet_deit_base_patch16_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/imagenet_deit_base_hydra_layer12_patch16_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2557 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/randaug_imagenet_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnext/
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnext/imagenet_resnext101-32x4d_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnext/imagenet_resnext50-32x4d_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnext/resnext50-32x4d_b32x8_100e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnext/imagenet_resnext152-32x4d_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnext/imagenet_resnext101-32x8d_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/
--rw-r--r--   0 runner    (1001) docker     (122)      924 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/deitiii_base_patch16_192.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/imagenet_deitiii_large_patch16_192_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/threeaug_imagenet_classification_224.py
--rw-r--r--   0 runner    (1001) docker     (122)      435 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/imagenet_deitiii_small_patch16_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/threeaug_imagenet_classification_192.py
--rw-r--r--   0 runner    (1001) docker     (122)      952 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/deitiii_schedule.py
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/imagenet_deitiii_base_patch16_192_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/
--rw-r--r--   0 runner    (1001) docker     (122)     2728 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/EdgeVit_b512x8_300e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_xxs_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_xs_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_s_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/common/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/common/dataset/
--rw-r--r--   0 runner    (1001) docker     (122)     8996 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/common/dataset/imagenet_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)      587 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/common/classification_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnet/
--rw-r--r--   0 runner    (1001) docker     (122)     1786 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet50_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet101_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      729 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnet/resnet50_b32x8_100e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet152_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet50_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw30_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw32_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/hrnetw18_b32x8_100e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw40_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw44_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw48_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw64_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw18_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/
--rw-r--r--   0 runner    (1001) docker     (122)      263 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/imagenet_swin_small_patch4_window7_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/imagenet_swin_large_patch4_window7_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/imagenet_swin_base_patch4_window7_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/imagenet_swin_tiny_patch4_window7_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2327 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/swin_tiny_patch4_window7_224_b64x16_300e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/imagenet_swin_tiny_patch4_window7_224_jpg_torchacc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/vit/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/vit/imagenet_vit_large_patch16_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/vit/vit_base_patch16_224_b64x64_300e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/vit/imagenet_vit_base_patch32_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/vit/imagenet_vit_base_patch16_224_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      221 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/vit/imagenet_vit_large_patch32_224_jpg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/efficientformer/
--rw-r--r--   0 runner    (1001) docker     (122)      159 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/efficientformer/efficientformer_l3.py
--rw-r--r--   0 runner    (1001) docker     (122)     2731 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/efficientformer/efficientformer_l1.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/imagenet/efficientformer/efficientformer_l7.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/configs/classification/cifar10/
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/cifar10/r50_b128_300e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)     3142 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/classification/cifar10/swintiny_b64_5e_jpg.py
--rw-r--r--   0 runner    (1001) docker     (122)      419 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/predictors/
--rw-r--r--   0 runner    (1001) docker     (122)     9296 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/classifier.py
--rw-r--r--   0 runner    (1001) docker     (122)    10461 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/ocr.py
--rw-r--r--   0 runner    (1001) docker     (122)      262 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4902 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/face_keypoints_predictor.py
--rw-r--r--   0 runner    (1001) docker     (122)    22047 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)      976 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3842 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/interface.py
--rw-r--r--   0 runner    (1001) docker     (122)    19741 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/detector.py
--rw-r--r--   0 runner    (1001) docker     (122)    12732 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/wholebody_keypoints_predictor.py
--rw-r--r--   0 runner    (1001) docker     (122)     7844 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/hand_keypoints_predictor.py
--rw-r--r--   0 runner    (1001) docker     (122)    19069 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/pose_predictor.py
--rw-r--r--   0 runner    (1001) docker     (122)    13357 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10144 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/predictors/bevformer_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/runner/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9548 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/runner/ev_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/framework/
--rw-r--r--   0 runner    (1001) docker     (122)     3693 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/framework/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)     6996 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/eval_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)      903 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/show_time_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)      221 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4815 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/oss_sync_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)      119 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/yolox_lr_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/dino_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/collate_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1616 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/yolox_mode_switch_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/export_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1847 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/swav_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/sync_norm_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/throughput_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/wandb.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/best_ckpt_saver_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1865 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/sync_random_size_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/optimizer_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     3246 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/lr_update_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/hooks/byol_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/file/
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/file/image.py
--rw-r--r--   0 runner    (1001) docker     (122)       66 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2906 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/file/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    30023 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/file/file_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     6729 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/file/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/toolkit/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/toolkit/prune/
--rw-r--r--   0 runner    (1001) docker     (122)       88 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/prune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3276 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/prune/prune_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/toolkit/torchacc/
--rw-r--r--   0 runner    (1001) docker     (122)    12687 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/torchacc/convert_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)      642 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/torchacc/initilization.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/torchacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/toolkit/blade/
--rw-r--r--   0 runner    (1001) docker     (122)     5156 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/blade/trt_plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/blade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11404 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/blade/cv_blade_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/toolkit/quantize/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/quantize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6299 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/toolkit/quantize/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/apis/
--rw-r--r--   0 runner    (1001) docker     (122)      239 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11904 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18447 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/apis/train.py
--rw-r--r--   0 runner    (1001) docker     (122)    26128 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/apis/export.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/apis/train_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/u2sod/
--rw-r--r--   0 runner    (1001) docker     (122)    15169 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/u2sod/u2net_models.py
--rw-r--r--   0 runner    (1001) docker     (122)      427 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/u2sod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4809 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/u2sod/u2net_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     7103 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/u2sod/sodpredictor.py
--rw-r--r--   0 runner    (1001) docker     (122)      580 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/face_align.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/mtcnn/
--rw-r--r--   0 runner    (1001) docker     (122)     6482 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/mtcnn/get_nets.py
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/mtcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8777 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/mtcnn/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9129 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/mtcnn/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4873 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/functions/
--rw-r--r--   0 runner    (1001) docker     (122)     5730 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/functions/ms_deform_attn_func.py
--rw-r--r--   0 runner    (1001) docker     (122)      733 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/modules/
--rw-r--r--   0 runner    (1001) docker     (122)      720 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8229 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/modules/ms_deform_attn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cpu/
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.h
--rw-r--r--   0 runner    (1001) docker     (122)     1434 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/vision.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1981 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/ms_deform_attn.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cuda/
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.h
--rw-r--r--   0 runner    (1001) docker     (122)     7459 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (122)    54837 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_im2col_cuda.cuh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/resource/
--rw-r--r--   0 runner    (1001) docker     (122) 10044356 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/resource/simhei.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1805 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)      280 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6225 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)      181 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     3656 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/data_sources/imagenet_feature.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2851 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/selfsup/data_sources/image_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/shared/
--rw-r--r--   0 runner    (1001) docker     (122)     5978 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/dali_tfrecord_imagenet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/shared/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)     2426 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/pipelines/third_transforms_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     6220 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/pipelines/dali_transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)      401 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8099 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/pipelines/format.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)     5791 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/dali_tfrecord_multi_view.py
--rw-r--r--   0 runner    (1001) docker     (122)      903 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8586 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/odps_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      570 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/raw.py
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/dataset_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/shared/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1441 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/data_sources/concat.py
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/data_sources/image_npy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/shared/multi_view.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/face/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/face/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)    15330 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/face/pipelines/face_keypoint_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)      242 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/face/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/face/face_keypoint_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/face/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/face/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6625 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/face/data_sources/face_keypoint_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      634 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6098 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)      221 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2826 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)    14836 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/coco_stuff.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4898 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/raw.py
--rw-r--r--   0 runner    (1001) docker     (122)     7220 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    13022 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/voc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8206 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/pose/
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/hand_coco_wholebody_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1877 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/wholebody_topdown_coco_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/pose/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)      800 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    33432 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)      449 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/top_down.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/hand/
--rw-r--r--   0 runner    (1001) docker     (122)       98 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/hand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9671 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/hand/coco_hand.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/wholebody/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/wholebody/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    35725 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/wholebody/wholebody_coco_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      636 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12530 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/mpii.py
--rw-r--r--   0 runner    (1001) docker     (122)    13060 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/top_down.py
--rw-r--r--   0 runner    (1001) docker     (122)     5855 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/crowd_pose.py
--rw-r--r--   0 runner    (1001) docker     (122)    12204 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/oc_human.py
--rw-r--r--   0 runner    (1001) docker     (122)    10864 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/pose/data_sources/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/detection/
--rw-r--r--   0 runner    (1001) docker     (122)     8964 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/mix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/detection/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)      752 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    88688 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/pipelines/mm_transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7770 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/fruit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5241 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/pet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5370 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/pai_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     3847 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/artaxor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5139 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/wider_person.py
--rw-r--r--   0 runner    (1001) docker     (122)    16723 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/coco_panoptic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1177 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4553 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/raw.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/african_wildlife.py
--rw-r--r--   0 runner    (1001) docker     (122)     4871 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/coco_livs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4063 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/crowd_human.py
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/objects365.py
--rw-r--r--   0 runner    (1001) docker     (122)     6531 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5374 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/wider_face.py
--rw-r--r--   0 runner    (1001) docker     (122)    10917 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/voc.py
--rw-r--r--   0 runner    (1001) docker     (122)    15325 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection/data_sources/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/ocr/
--rw-r--r--   0 runner    (1001) docker     (122)      857 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/ocr_det_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/ocr_cls_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/ocr/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)    22195 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/pipelines/rec_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)      327 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21717 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/pipelines/det_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     7443 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/pipelines/label_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)      250 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/ocr_raw_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/ocr/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/data_sources/ocr_cls_datasource.py
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/data_sources/ocr_det_datasource.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6358 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/data_sources/ocr_rec_datasource.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/ocr/ocr_rec_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)    17576 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/transforms_3d.py
--rw-r--r--   0 runner    (1001) docker     (122)      860 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23107 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/test_aug.py
--rw-r--r--   0 runner    (1001) docker     (122)    11467 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/format.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/functional.py
--rw-r--r--   0 runner    (1001) docker     (122)      213 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    20136 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/nuscenes_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11857 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/data_sources/nuscenes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9182 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/detection3d/data_sources/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/classification/
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/odps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/classification/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)    43526 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/pipelines/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6260 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/pipelines/transform.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3400 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     1905 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/imagenet_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/fashiongen_h5.py
--rw-r--r--   0 runner    (1001) docker     (122)     7512 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/cub.py
--rw-r--r--   0 runner    (1001) docker     (122)     2582 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (122)     1588 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/mnist.py
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/cifar.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/flower.py
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/class_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     9335 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/image_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3457 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/classification/data_sources/caltech.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/loader/
--rw-r--r--   0 runner    (1001) docker     (122)    20702 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/loader/sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)      469 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7763 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/loader/build_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/loader/loader_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/loader/collate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      235 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/utils/type_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     4594 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/utils/tfrecord_util.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/utils/transform_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/datasets/utils/download_data/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/utils/download_data/download_voc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2298 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/utils/download_data/download_coco.py
--rw-r--r--   0 runner    (1001) docker     (122)      129 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/utils/download_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1722 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/datasets/utils/download_data/commont.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     9034 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/quantize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/tools/analyze_tools/
--rw-r--r--   0 runner    (1001) docker     (122)     3012 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/analyze_tools/measure_inference_time.py
--rw-r--r--   0 runner    (1001) docker     (122)     1844 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/analyze_tools/count_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/analyze_tools/count_flops.py
--rw-r--r--   0 runner    (1001) docker     (122)     8412 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/prune.py
--rw-r--r--   0 runner    (1001) docker     (122)     9937 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/eval.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/tools/prepare_data/
--rw-r--r--   0 runner    (1001) docker     (122)     7701 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/prepare_data/create_voc_data_files.py
--rw-r--r--   0 runner    (1001) docker     (122)    29869 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/prepare_data/prepare_nuscenes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5228 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/prepare_data/coco_stuff164k.py
--rw-r--r--   0 runner    (1001) docker     (122)     4701 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/prepare_data/create_voc_low_shot_challenge_samples.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/prepare_data/convert_subset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2348 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/commands_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    11695 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (122)    15577 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)     3423 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/launch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/tools/export.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/easycv/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/gather.py
--rw-r--r--   0 runner    (1001) docker     (122)    14714 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/mmlab_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/metric_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/alias_multinomial.py
--rw-r--r--   0 runner    (1001) docker     (122)      591 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/py_util.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/parse_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)     3762 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3712 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      951 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2585 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     6803 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/preprocess_function.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      704 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5866 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1981 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     4304 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (122)     6949 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2429 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (122)    12790 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/test_util.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/constant.py
--rw-r--r--   0 runner    (1001) docker     (122)    22342 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/config_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    15438 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (122)     5468 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/ms_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      888 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/user_config_params_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/torchacc_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3534 2022-12-06 03:04:27.000000 pai-easycv-0.8.0/easycv/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/pai_easycv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 03:04:30.000000 pai-easycv-0.8.0/pai_easycv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-12-06 03:04:30.000000 pai-easycv-0.8.0/pai_easycv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 03:04:30.000000 pai-easycv-0.8.0/pai_easycv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)    39935 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/pai_easycv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)    15463 2022-12-06 03:04:30.000000 pai-easycv-0.8.0/pai_easycv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      282 2022-12-06 03:04:30.000000 pai-easycv-0.8.0/pai_easycv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-06 03:04:31.000000 pai-easycv-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/runner/
+-rw-r--r--   0 runner    (1001) docker     (122)     9548 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/runner/ev_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/framework/
+-rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/framework/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/commands_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8412 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/prune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3423 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/launch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11695 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/export.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/tools/analyze_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/analyze_tools/count_flops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/analyze_tools/measure_inference_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/analyze_tools/count_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9034 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9937 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/eval.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/tools/prepare_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/prepare_data/convert_subset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5228 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/prepare_data/coco_stuff164k.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4701 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/prepare_data/create_voc_low_shot_challenge_samples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7701 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/prepare_data/create_voc_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29869 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/prepare_data/prepare_nuscenes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16742 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/tools/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)    18447 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/apis/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26359 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/apis/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/apis/train_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11904 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/apis/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/face_align.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/u2sod/
+-rw-r--r--   0 runner    (1001) docker     (122)     7103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/u2sod/sodpredictor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/u2sod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4809 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/u2sod/u2net_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15169 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/u2sod/u2net_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/mtcnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     9129 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mtcnn/detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6482 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mtcnn/get_nets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mtcnn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mtcnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     8229 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/modules/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/functions/ms_deform_attn_func.py
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/ms_deform_attn.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/vision.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cuda/
+-rw-r--r--   0 runner    (1001) docker     (122)    54837 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_im2col_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7459 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cpu/
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/
+-rw-r--r--   0 runner    (1001) docker     (122)     4286 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/demo_mot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/bytetrack/
+-rw-r--r--   0 runner    (1001) docker     (122)    10671 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/bytetrack/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7842 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/bytetrack/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/bytetrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13316 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/bytetrack/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/bytetrack/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6065 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/thirdparty/mot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/face/
+-rw-r--r--   0 runner    (1001) docker     (122)     8821 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/face/face_96x96_wingloss.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/ocr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/ocr/direction/
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/direction/direction_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/ocr/detection/
+-rw-r--r--   0 runner    (1001) docker     (122)     4108 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/detection/det_model_en.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3991 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/detection/det_model_ch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/detection/det_model_ch_r50.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/detection/det_model_en_r50.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_te.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3797 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_arabic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_ka.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_ta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_ch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_korean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_cyrillic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_en.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_chinese_cht.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_devanagari.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_japan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_latin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/x3d/
+-rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/x3d/x3d_l.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/x3d/x3d_xs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/x3d/x3d_m.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/clipbert/
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/clipbert/clipbert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5060 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/clipbert/clipbert_multilabel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/swin/
+-rw-r--r--   0 runner    (1001) docker     (122)     4136 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/swin/video_swin_s.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4138 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/swin/video_swin_b.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4134 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/video_recognition/swin/video_swin_tiny.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/fast_convmae/
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/fast_convmae/fast_convmae_vit_base_patch16_8xb64_50e.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mae/
+-rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mae/mae_vit_base_patch16_8xb64_1600e.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mae/mae_vit_large_patch16_8xb32_1600e.py
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mae/mae_vit_base_patch16_8xb64_400e.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/simclr/
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/simclr/simclr_rn50_mocov2_neck_8xb32_200e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/dino/
+-rw-r--r--   0 runner    (1001) docker     (122)     4028 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5236 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/byol/
+-rw-r--r--   0 runner    (1001) docker     (122)     3512 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/byol/byol_rn50_8xb32_200e.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/swav/
+-rw-r--r--   0 runner    (1001) docker     (122)     3078 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/swav/swav_genet_8xb32_200e_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/swav/swav_rn50_8xb32_200e_tfrecord.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/moby/
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/moby/moby_rn50_4xb128_100e_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/moby/moby_dynamic_swin_tiny_8xb64_300e_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2603 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/moby/moby_deit_small_4xb32_100e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/moby/moby_deit_small_p16_4xb128_300e_tfrecord.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mocov2/
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_tfrecord.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mixco/
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mixco/mixco_genet_8xb32_200e_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/selfsup/mixco/mixco_rn50_4xb64_200e_tfrecord_oss.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection3d/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/
+-rw-r--r--   0 runner    (1001) docker     (122)    11285 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11556 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/bevformer_tiny_r50_nuscenes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11391 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/bevformer_tiny_r50_nuscenes_fp16.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11285 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes_blancehybrid.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/cifar10/swintiny_b64_5e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/cifar10/r50_b128_300e_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/inception/
+-rw-r--r--   0 runner    (1001) docker     (122)    10008 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/inception/inceptionv3_b32x8_100e.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/sequencer/sequencer2d_s.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/sequencer/sequencer2d_m.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/sequencer/sequencer2d_l.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convmixer/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convmixer/convmixer_1024_20_ks9_p14.py
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convmixer/convmixer_768_32.py
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convmixer/convmixer_1536_20.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/shuffle_transformer/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/shuffle_transformer/shuffletrans_small_p4_w7_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/shuffle_transformer/shuffletrans_base_p4_w7_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/shuffle_transformer/shuffletrans_tiny_p4_w7_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/levit/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/levit/levit_128.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/levit/levit_256.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/levit/levit_192.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/xcit/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/xcit/xcit_large_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/xcit/xcit_medium_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/xcit/xcit_medium_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/xcit/xcit_large_24_p8_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/twins/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/twins/twins_svt_small.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/twins/twins_svt_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/twins/twins_svt_large.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convit/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convit/convit_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convit/convit_small.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convit/convit_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/deit/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/deit/deit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/deit/deit_base_distilled_patch16_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/cait/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/cait/cait_xxs36_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/cait/cait_xxs24_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/cait/cait_s24_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/vit/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/vit/vit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/vit/vit_large_patch16_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/mlp-mixer/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/mlp-mixer/mixer_b16_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/mlp-mixer/mixer_l16_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/poolformer/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_s12.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_s36.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_m36.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_m48.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/poolformer/poolformer_s24.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/mobilevit/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/mobilevit/mobilevit_s.py
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/mobilevit/mobilevit_xs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/mobilevit/mobilevit_xxs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/coat/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/coat/coat_mini.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/coat/coat_tiny.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/tnt/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/tnt/tnt_s_patch16_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/swint/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/swint/swin_base_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/swint/swin_large_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/swint/dynamic_swin_small_p4_w7_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/swint/dynamic_swin_tiny_p4_w7_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/gmlp/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/gmlp/gmlp_s16_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/pit/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/pit/pit_s_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/pit/pit_b_distilled_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convnext/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convnext/convnext_large.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convnext/convnext_small.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convnext/convnext_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/convnext/convnext_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/resmlp/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/resmlp/resmlp_12_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/resmlp/resmlp_big_24_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/resmlp/resmlp_36_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/resmlp/resmlp_24_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/timm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/gmixer/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/gmixer/gmixer_24_224.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/crossvit/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/crossvit/crossvit_base_240.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/crossvit/crossvit_small_240.py
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/crossvit/crossvit_tiny_240.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/nest/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/nest/jx_nest_small.py
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/nest/jx_nest_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/nest/jx_nest_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnet/
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet50_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet152_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1786 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet50_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnet/resnet50_b32x8_100e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet101_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/imagenet_deit_base_patch16_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/deit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/imagenet_deit_base_hydra_layer12_patch16_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/imagenet_deit_base_hydra_layer8_patch16_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/deit_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2557 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/randaug_imagenet_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/vit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/vit/vit_base_patch16_224_b64x64_300e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/vit/imagenet_vit_large_patch32_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/vit/imagenet_vit_base_patch16_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/vit/imagenet_vit_large_patch16_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/vit/imagenet_vit_base_patch32_224_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/hrnetw18_b32x8_100e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw48_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw30_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw64_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw18_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw44_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw32_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw40_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/common/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)     8996 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/common/dataset/imagenet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/common/classification_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_s_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_xxs_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_xs_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2728 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/EdgeVit_b512x8_300e_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/imagenet_deitiii_base_patch16_192_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/deitiii_base_patch16_192.py
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/deitiii_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/imagenet_deitiii_large_patch16_192_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/threeaug_imagenet_classification_192.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/threeaug_imagenet_classification_224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/imagenet_deitiii_small_patch16_224_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/imagenet_swin_tiny_patch4_window7_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/imagenet_swin_tiny_patch4_window7_224_jpg_torchacc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/swin_tiny_patch4_window7_224_b64x16_300e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/imagenet_swin_large_patch4_window7_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/imagenet_swin_base_patch4_window7_224_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/imagenet_swin_small_patch4_window7_224_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnext/
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnext/imagenet_resnext101-32x4d_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnext/imagenet_resnext50-32x4d_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnext/resnext50-32x4d_b32x8_100e_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnext/imagenet_resnext101-32x8d_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnext/imagenet_resnext152-32x4d_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/efficientformer/
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/efficientformer/efficientformer_l3.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/efficientformer/efficientformer_l7.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/classification/imagenet/efficientformer/efficientformer_l1.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/fcos/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/fcos/fcos_r50_torch_1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/fcos/fcos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/fcos/coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/fcos/fcos_r50_caffe_1x_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_schedule_1x.py
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_r50_36e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_r50_24e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_swinl_center_iou_memoryreduce_26e_obj365.py
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_r50_24e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3152 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_swinl.py
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_swinl_24e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_swinl_center_iou_memoryreduce_18e_obj2coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_swinl_36e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_r50_36e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_swinl_24e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_swinl_12e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_r50.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2991 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_r50.py
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_swinl.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_swinl_36e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_swinl_12e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_r50_12e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_r50_12e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (122)     5609 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/pai_yoloxs_asff_8xb16_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_x_8xb8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_nano_8xb16_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/pai_yoloxs_asff_tood3_8xb16_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_m_8xb16_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_l_8xb8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4178 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_tiny_8xb16_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5611 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/pai_yoloxs_8xb16_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5831 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_voc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco_pai.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/common/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)     5111 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/common/dataset/autoaug_coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/common/dataset/autoaug_obj2coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8826 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/common/dataset/autoaug_obj365_val5k_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/
+-rw-r--r--   0 runner    (1001) docker     (122)     4868 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_mask_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4112 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/lsj_coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7931 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_cascade_mask_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_mask_rcnn_100e.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4199 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/lsj_coco_instance.py
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_faster_rcnn_100e.py
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_schedule_100e.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4280 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_cascade_mask_rcnn_100e.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/dab_detr/
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dab_detr/dab_detr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dab_detr/dn_detr_r50_dc5_8x2_50e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dab_detr/dab_detr_r50_8x2_50e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/dab_detr/dn_detr_r50_8x2_50e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/detr/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/detr/detr_r50_8x2_150e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/detr/detr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/detection/mask_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     4675 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/detection/mask_rcnn/mask_rcnn_r50_fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/segmentation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/segmentation/upernet/
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/upernet/upernet_r50_512x512_8xb4_60e_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/upernet/upernet_r50_512x512_8xb4_60e_voc12aug.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/segmentation/segformer/
+-rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/segformer/segformer_b5_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10276 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/segformer/segformer_b0_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/segformer/segformer_b3_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/segformer/segformer_b4_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/segformer/segformer_b1_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/segformer/segformer_b2_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/segmentation/fcn/
+-rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/fcn/fcn_r50-d8_512x512_8xb4_60e_voc12aug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/fcn/fcn_r50-d8_512x512_8xb4_60e_voc12.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/segmentation/mask2former/
+-rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e127_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8058 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_instance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10421 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_panoptic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/config_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     6301 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/topdown_hrnet_w48_udp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4236 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/dino_rn50_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/topdown_litehrnet_30.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10447 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/classification_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/swav_r50_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/moco_r50_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3521 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/swav_r50_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2511 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/moco_timm_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5411 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/yolox_edge_itag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/yolox_edge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/dino_timm_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/moco_timm_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5679 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/yolox_itag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3494 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/moby_timm_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9578 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10057 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/classification_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6149 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/yolox.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3071 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/dino_timm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/config_templates/metric_learning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/metric_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/metric_learning/softmaxbased_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5697 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/metric_learning/modelparallel_softmaxbased_tfrecord_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/mae_vit_base_patch16.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/config_templates/moco_r50_tfrecord.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/pose/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/pose/hand/
+-rw-r--r--   0 runner    (1001) docker     (122)     5359 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/pose/hand/litehrnet_30_coco_wholebody_hand_256x256.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/pose/hand/hrnet_w18_coco_wholebody_hand_256x256_dark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5990 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/pose/hrnet_w48_coco_256x192_udp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/pose/wholebody/
+-rw-r--r--   0 runner    (1001) docker     (122)     5807 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/pose/wholebody/hrnet_w48_coco_wholebody_384x288_dark_plus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5483 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/pose/litehrnet_30_coco_384x288.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/imagenet_timm_modelparallel_softmaxbased_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4480 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/sop_timm_swinb_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/cub_resnet50_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/common/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)     9358 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/common/dataset/imagenet_metriclearning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/common/metriclearning_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/imagenet_resnet50_1000kid_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/imagenet_resnet50_1000kid_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/metric_learning/imagenet_timm_softmaxbased_jpg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/configs/edge_models/
+-rw-r--r--   0 runner    (1001) docker     (122)     5485 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/edge_models/yolox_s.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/edge_models/yolox_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6055 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/edge_models/yolox_edge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5485 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/edge_models/yolox_l.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5339 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/edge_models/yolox_nano.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5487 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/configs/edge_models/yolox_m.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/face/
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/face/face_keypoint_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/face/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     6630 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/face/data_sources/face_keypoint_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/face/data_sources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/face/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/face/pipelines/face_keypoint_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/face/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/face/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/ocr/
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/ocr_det_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/ocr/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/data_sources/ocr_cls_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/data_sources/ocr_det_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6358 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/data_sources/ocr_rec_datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/ocr/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)    21717 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/pipelines/det_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22195 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/pipelines/rec_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7443 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/pipelines/label_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/ocr_rec_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/ocr_cls_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/ocr_raw_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/loader/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/loader/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20702 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/loader/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/loader/loader_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7763 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/loader/build_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1805 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/data_sources/video_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/data_sources/video_text_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)    14771 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/pipelines/text_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69689 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/pipelines/transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/video_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/data_sources/imagenet_feature.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/data_sources/image_list.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     6225 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/selfsup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     9182 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/data_sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11857 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/data_sources/nuscenes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/data_sources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)    23107 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/test_aug.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/functional.py
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11467 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/format.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17576 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/transforms_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20136 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection3d/nuscenes_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/classification/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     3672 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/class_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3457 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/caltech.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7512 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/cub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1905 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/imagenet_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8937 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/image_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/flower.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/fashiongen_h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/data_sources/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3400 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/classification/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)    43526 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/pipelines/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6260 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/pipelines/transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/classification/odps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/detection/
+-rw-r--r--   0 runner    (1001) docker     (122)     8964 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/mix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     6531 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5374 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/wider_face.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4063 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/crowd_human.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15325 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5370 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/pai_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4553 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/raw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/fruit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/wider_person.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16723 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/coco_panoptic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/african_wildlife.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10917 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/voc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3847 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/artaxor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/objects365.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/pet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/data_sources/coco_livs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7770 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/detection/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)    88688 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/pipelines/mm_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     7173 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8206 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14785 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/coco_stuff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4898 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/raw.py
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13022 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/voc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     6098 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/pose/
+-rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/wholebody_topdown_coco_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/top_down.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)    12204 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/oc_human.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/crowd_pose.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10864 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/coco.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/hand/
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/hand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9671 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/hand/coco_hand.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13060 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/top_down.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12530 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/mpii.py
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/wholebody/
+-rw-r--r--   0 runner    (1001) docker     (122)    35725 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/wholebody/wholebody_coco_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/data_sources/wholebody/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/pose/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)    33432 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      449 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/pose/hand_coco_wholebody_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/utils/transform_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/utils/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/utils/download_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/utils/download_data/commont.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/utils/download_data/download_voc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/utils/download_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/utils/download_data/download_coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4594 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/utils/tfrecord_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/shared/
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/multi_view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/shared/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/data_sources/concat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/data_sources/image_npy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/raw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/dali_tfrecord_multi_view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/datasets/shared/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     2426 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/pipelines/third_transforms_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8099 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/pipelines/format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6220 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/pipelines/dali_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5978 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/dali_tfrecord_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8586 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/datasets/shared/odps_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/file/
+-rw-r--r--   0 runner    (1001) docker     (122)     6729 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/file/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30311 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/file/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/file/image.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/resource/
+-rw-r--r--   0 runner    (1001) docker     (122) 10044356 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/resource/simhei.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/post_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)    12225 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/post_processing/pose_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10780 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/post_processing/box3d_nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6820 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/post_processing/merge_augs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/post_processing/nms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/sailfish/
+-rw-r--r--   0 runner    (1001) docker     (122)    10298 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/sailfish/function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6154 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/sailfish/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/sailfish/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7831 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/sailfish/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/sailfish/activation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/sailfish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/bbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/
+-rw-r--r--   0 runner    (1001) docker     (122)    13795 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/cam_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21406 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/base_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/box_3d_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9189 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/coord_3d_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10850 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/depth_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/lidar_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11833 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/bbox/coders/
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/coders/base_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/coders/nms_free_coder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/coders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/bbox/match_costs/
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/match_costs/builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5862 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/match_costs/match_cost.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/match_costs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/bbox/assigners/
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/assigners/base_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7812 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/assigners/assign_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/assigners/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6398 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/assigners/hungarian_assigner_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13901 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/bbox_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/bbox/iou_calculators/
+-rw-r--r--   0 runner    (1001) docker     (122)     7373 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/iou_calculators/iou2d_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/iou_calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/bbox/samplers/
+-rw-r--r--   0 runner    (1001) docker     (122)     3974 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5440 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/samplers/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/bbox/samplers/pseudo_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)    39521 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/coco_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7840 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/retrival_topk_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11165 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/segmentation_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4716 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/keypoint_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22075 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/top_down_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9351 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/classification_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33656 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/nuscenes_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/face_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/evaluation/custom_cocotools/
+-rw-r--r--   0 runner    (1001) docker     (122)    42040 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/custom_cocotools/cocoeval.py
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/custom_cocotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9679 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/ocr_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7480 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4945 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/wholebody_keypoint_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51790 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/coco_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/metric_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/auc_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8252 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/faceid_pair_eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/evaluation/mse_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)     4879 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/visualization/image_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18442 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/visualization/open3d_vis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/visualization/image.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/anchor/
+-rw-r--r--   0 runner    (1001) docker     (122)    10789 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/anchor/point_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/anchor/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/anchor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9426 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/standard_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (122)     3853 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/optimizer/layer_decay_optimizer_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4792 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/optimizer/adam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8589 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/optimizer/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4510 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/optimizer/lars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)    13267 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/utils/array_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/core/points/
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/points/depth_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16651 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/points/base_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/points/cam_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/core/points/lidar_points.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/optimizer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/throughput_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/yolox_lr_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/collate_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/yolox_mode_switch_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1865 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/show_time_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4815 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/oss_sync_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/swav_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/lr_update_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/byol_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6996 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/eval_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/dino_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/export_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/sync_random_size_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/sync_norm_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/hooks/best_ckpt_saver_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/toolkit/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/toolkit/torchacc/
+-rw-r--r--   0 runner    (1001) docker     (122)    12687 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/torchacc/convert_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/torchacc/initilization.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/torchacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/toolkit/blade/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/blade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11404 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/blade/cv_blade_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5156 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/blade/trt_plugin_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/toolkit/quantize/
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/quantize/quantize_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/quantize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/toolkit/prune/
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/prune/prune_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/prune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     7260 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/face/
+-rw-r--r--   0 runner    (1001) docker     (122)     3532 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/face/face_keypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/face/head/
+-rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/face/head/face_keypoint_pose_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/face/head/face_keypoint_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/face/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/face/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/ocr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/ocr/backbones/
+-rw-r--r--   0 runner    (1001) docker     (122)    10728 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/backbones/det_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8753 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/backbones/det_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18720 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/backbones/rec_svtrnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5186 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/backbones/rec_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/backbones/rec_mv1_enhance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/ocr/cls/
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/cls/text_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/cls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/ocr/rec/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/rec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/rec/ocr_rec.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/ocr/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/postprocess/db_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7561 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/postprocess/rec_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/postprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/ocr/heads/
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/heads/db_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16723 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/heads/rec_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/ocr/necks/
+-rw-r--r--   0 runner    (1001) docker     (122)     6963 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/necks/squence_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10417 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/necks/db_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/necks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/ocr/det/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/det/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/ocr/det/db_net.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2282 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18522 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/modelzoo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/video_recognition/
+-rw-r--r--   0 runner    (1001) docker     (122)     9680 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/video_recognition/recognizer3d.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/video_recognition/heads/
+-rw-r--r--   0 runner    (1001) docker     (122)     6100 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/video_recognition/heads/x3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4489 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/video_recognition/heads/base_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/video_recognition/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2460 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/video_recognition/heads/i3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/video_recognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4980 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/video_recognition/ClipBertTwoStream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (122)    11084 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/vit_transformer_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13098 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/resnet_jit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36277 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/lighthrnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12540 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35873 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/swin_transformer_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11798 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/x3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57326 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/genet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16886 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/conv_mae_vit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12473 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/repvgg_yolox_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12926 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/inceptionv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15666 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/efficientformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6118 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/mobilenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4617 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/mae_vit_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20173 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17626 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/shuffle_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29413 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17270 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/mit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6072 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/mnasnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6921 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14289 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/conv_vitdet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46977 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/bninception.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27124 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/benchmark_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22322 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/xcit_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6937 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/darknet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17039 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/vitdet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14519 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/edgevit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22438 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/clip_bert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8314 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/pytorch_image_models_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9935 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/network_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20443 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28658 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/swin_transformer3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/backbones/face_keypoint_backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/selfsup/
+-rw-r--r--   0 runner    (1001) docker     (122)     3724 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/mixco.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20872 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/necks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8312 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/moco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/mae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3528 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10485 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/moby.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14559 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/dino.py
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3540 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/byol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8571 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/selfsup/swav.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection3d/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)     4919 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/
+-rw-r--r--   0 runner    (1001) docker     (122)    40003 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34797 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/bevformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18171 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/bevformer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/attentions/
+-rw-r--r--   0 runner    (1001) docker     (122)    14781 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/attentions/multi_scale_deformable_attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7132 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/attentions/spatial_cross_attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/attentions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11808 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/attentions/temporal_self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)      898 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20990 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/mvx_two_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/utils/grid_mask.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection3d/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)    11813 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/classification/necks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11367 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/dense_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)     8513 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/dense_heads/dense_test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14069 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/dense_heads/anchor_free_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23284 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/dense_heads/base_dense_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/dense_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/fcos/
+-rw-r--r--   0 runner    (1001) docker     (122)    37216 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/fcos/fcos_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/fcos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dino/
+-rw-r--r--   0 runner    (1001) docker     (122)     8062 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dino/cdn_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24332 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dino/dino_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48085 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dino/deformable_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/
+-rw-r--r--   0 runner    (1001) docker     (122)     6950 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/asff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11675 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/yolo_pafpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25373 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/yolo_head_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7900 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/yolox.py
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9205 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/tood_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4616 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/yolo_head.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox_edge/
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox_edge/yolox_edge.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/yolox_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/
+-rw-r--r--   0 runner    (1001) docker     (122)     7522 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/dn_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21005 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19793 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/dab_detr_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11710 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/dab_detr_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/detection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/detr/
+-rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/detr/detr_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/detr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13710 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/detectors/detr/detr_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/necks/
+-rw-r--r--   0 runner    (1001) docker     (122)     4714 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/necks/sfp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8849 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/necks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     6568 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/utils/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17199 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/utils/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9364 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/utils/generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8843 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/detection/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (122)    16230 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/mask2former.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/
+-rw-r--r--   0 runner    (1001) docker     (122)    11026 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6499 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/uper_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18696 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6819 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/segformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17151 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/pixel_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3462 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/heads/mask2former_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13523 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/segmentation/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/utils/point_rend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/utils/shape_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3069 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/utils/panoptic_gt_processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14284 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/utils/criterion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12316 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/utils/embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/segmentation/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/pose/
+-rw-r--r--   0 runner    (1001) docker     (122)     8627 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/pose/top_down.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/pose/heads/
+-rw-r--r--   0 runner    (1001) docker     (122)    13007 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/pose/heads/topdown_heatmap_simple_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/pose/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/pose/heads/topdown_heatmap_base_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/pose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/heads/
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/heads/latent_pred_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/heads/contrastive_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/heads/cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2754 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/heads/multi_cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9252 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/heads/mp_metric_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/loss/
+-rw-r--r--   0 runner    (1001) docker     (122)     7657 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/det_db_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16221 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8685 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/face_keypoint_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15688 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/cross_entropy_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/loss/set_criterion/
+-rw-r--r--   0 runner    (1001) docker     (122)     5046 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/set_criterion/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26009 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/set_criterion/set_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/set_criterion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9157 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/pytorch_metric_learning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3853 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/ocr_rec_multi_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1388 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12544 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/loss/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7779 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/face_keypoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29286 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/scale.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6462 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/video_model_stem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3261 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6240 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/activation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/sobel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25758 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/x3d_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3233 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4002 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/gather_layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/norm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/init_weights.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/models/utils/multi_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/easycv/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/alias_multinomial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/parse_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14714 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/mmlab_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/constant.py
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/preprocess_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23083 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/config_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/user_config_params_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5468 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/ms_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/py_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/metric_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15438 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6949 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12790 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/torchacc_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/gather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/easycv/predictors/
+-rw-r--r--   0 runner    (1001) docker     (122)    13357 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/video_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19069 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/pose_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12732 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9296 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19604 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3842 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/wholebody_keypoints_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10144 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/bevformer_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22047 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10461 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/hand_keypoints_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4902 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/face_keypoints_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-01-17 02:44:01.000000 pai-easycv-0.9.0/easycv/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/pai_easycv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/pai_easycv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/pai_easycv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    42083 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/pai_easycv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/pai_easycv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    15644 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/pai_easycv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/pai_easycv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    12867 2023-01-17 02:44:06.000000 pai-easycv-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    15644 2023-01-17 02:44:07.000000 pai-easycv-0.9.0/PKG-INFO
```

### Comparing `pai-easycv-0.8.0/README.md` & `pai-easycv-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,20 @@
 
 - **Efficiency**
 
   EasyCV supports multi-gpu and multi-worker training. EasyCV uses [DALI](https://github.com/NVIDIA/DALI) to accelerate data io and preprocessing process, and uses [TorchAccelerator](https://github.com/alibaba/EasyCV/tree/master/docs/source/tutorials/torchacc.md) and fp16 to accelerate training process. For inference optimization, EasyCV exports model using jit script, which can be optimized by [PAI-Blade](https://help.aliyun.com/document_detail/205134.html)
 
 
 ## What's New
+[🔥 2023.01.17]
+
+* 17/01/2023 EasyCV v0.9.0 was released.
+- Support Single-lens MOT
+- Support video recognition (X3D, SWIN-video)
+
 [🔥 2022.12.02]
 
 * 02/12/2022 EasyCV v0.8.0 was released.
 - bevformer-base NDS increased by 0.8 on nuscenes val, training speed increased by 10%, and inference speed increased by 40%.
 - Support Objects365 pretrain and Adding the DINO++ model can achieve an accuracy of 63.4mAP at a model scale of 200M(Under the same scale, the accuracy is the best).
 
 [🔥 2022.08.31] We have released our YOLOX-PAI that achieves SOTA results within 40~50 mAP (less than 1ms). And we also provide a convenient and fast export/predictor api for end2end object detection. To get a quick start of YOLOX-PAI, click [here](docs/source/tutorials/yolox.md)!
@@ -89,15 +95,15 @@
 * [image classification](docs/source/tutorials/cls.md)
 * [metric learning](docs/source/tutorials/metric_learning.md)
 * [object detection with yolox-pai](docs/source/tutorials/yolox.md)
 * [model compression with yolox](docs/source/tutorials/compression.md)
 * [using torchacc](docs/source/tutorials/torchacc.md)
 * [file io for local and oss files](docs/source/tutorials/file.md)
 * [using mmdetection model in EasyCV](docs/source/tutorials/mmdet_models_usage_guide.md)
-* [batch prediction tools][docs/source/tutorials/predict.md]
+* [batch prediction tools](docs/source/tutorials/predict.md)
 
 
 
 notebook
 * [self-supervised learning](docs/source/tutorials/EasyCV图像自监督训练-MAE.ipynb)
 * [image classification](docs/source/tutorials/EasyCV图像分类resnet50.ipynb)
 * [object detection with yolox-pai](docs/source/tutorials/EasyCV图像检测YoloX.ipynb)
```

### Comparing `pai-easycv-0.8.0/PKG-INFO` & `pai-easycv-0.9.0/pai_easycv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pai-easycv
-Version: 0.8.0
+Version: 0.9.0
 Summary: An all-in-one toolkit for computer vision
 Home-page: https://github.com/alibaba/EasyCV.git
 Author: Alibaba PAI team
 Author-email: easycv@list.alibaba-inc.com
 License: Apache License 2.0
 Description: 
         <div align="center">
@@ -50,14 +50,20 @@
         
         - **Efficiency**
         
           EasyCV supports multi-gpu and multi-worker training. EasyCV uses [DALI](https://github.com/NVIDIA/DALI) to accelerate data io and preprocessing process, and uses [TorchAccelerator](https://github.com/alibaba/EasyCV/tree/master/docs/source/tutorials/torchacc.md) and fp16 to accelerate training process. For inference optimization, EasyCV exports model using jit script, which can be optimized by [PAI-Blade](https://help.aliyun.com/document_detail/205134.html)
         
         
         ## What's New
+        [🔥 2023.01.17]
+        
+        * 17/01/2023 EasyCV v0.9.0 was released.
+        - Support Single-lens MOT
+        - Support video recognition (X3D, SWIN-video)
+        
         [🔥 2022.12.02]
         
         * 02/12/2022 EasyCV v0.8.0 was released.
         - bevformer-base NDS increased by 0.8 on nuscenes val, training speed increased by 10%, and inference speed increased by 40%.
         - Support Objects365 pretrain and Adding the DINO++ model can achieve an accuracy of 63.4mAP at a model scale of 200M(Under the same scale, the accuracy is the best).
         
         [🔥 2022.08.31] We have released our YOLOX-PAI that achieves SOTA results within 40~50 mAP (less than 1ms). And we also provide a convenient and fast export/predictor api for end2end object detection. To get a quick start of YOLOX-PAI, click [here](docs/source/tutorials/yolox.md)!
@@ -97,15 +103,15 @@
         * [image classification](docs/source/tutorials/cls.md)
         * [metric learning](docs/source/tutorials/metric_learning.md)
         * [object detection with yolox-pai](docs/source/tutorials/yolox.md)
         * [model compression with yolox](docs/source/tutorials/compression.md)
         * [using torchacc](docs/source/tutorials/torchacc.md)
         * [file io for local and oss files](docs/source/tutorials/file.md)
         * [using mmdetection model in EasyCV](docs/source/tutorials/mmdet_models_usage_guide.md)
-        * [batch prediction tools][docs/source/tutorials/predict.md]
+        * [batch prediction tools](docs/source/tutorials/predict.md)
         
         
         
         notebook
         * [self-supervised learning](docs/source/tutorials/EasyCV图像自监督训练-MAE.ipynb)
         * [image classification](docs/source/tutorials/EasyCV图像分类resnet50.ipynb)
         * [object detection with yolox-pai](docs/source/tutorials/EasyCV图像检测YoloX.ipynb)
```

### Comparing `pai-easycv-0.8.0/easycv/models/builder.py` & `pai-easycv-0.9.0/easycv/models/builder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/simclr.py` & `pai-easycv-0.9.0/easycv/models/selfsup/simclr.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/moby.py` & `pai-easycv-0.9.0/easycv/models/selfsup/moby.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/mae.py` & `pai-easycv-0.9.0/easycv/models/selfsup/mae.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/dino.py` & `pai-easycv-0.9.0/easycv/models/selfsup/dino.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/swav.py` & `pai-easycv-0.9.0/easycv/models/selfsup/swav.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/moco.py` & `pai-easycv-0.9.0/easycv/models/selfsup/moco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/byol.py` & `pai-easycv-0.9.0/easycv/models/selfsup/byol.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/mixco.py` & `pai-easycv-0.9.0/easycv/models/selfsup/mixco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/selfsup/necks.py` & `pai-easycv-0.9.0/easycv/models/selfsup/necks.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,14 @@
 
         self.decoder_blocks = nn.ModuleList([
             Block(
                 decoder_embed_dim,
                 decoder_num_heads,
                 mlp_ratio,
                 qkv_bias=True,
-                qk_scale=None,
                 norm_layer=norm_layer) for _ in range(decoder_depth)
         ])
 
         self.decoder_norm = norm_layer(decoder_embed_dim)
         self.decoder_pred = nn.Linear(
             decoder_embed_dim, patch_size**2 * in_chans, bias=True)
```

### Comparing `pai-easycv-0.8.0/easycv/models/registry.py` & `pai-easycv-0.9.0/easycv/models/registry.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/modelzoo.py` & `pai-easycv-0.9.0/easycv/models/modelzoo.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/face/face_keypoint.py` & `pai-easycv-0.9.0/easycv/models/face/face_keypoint.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/face/head/face_keypoint_pose_head.py` & `pai-easycv-0.9.0/easycv/models/face/head/face_keypoint_pose_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/face/head/face_keypoint_head.py` & `pai-easycv-0.9.0/easycv/models/face/head/face_keypoint_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/mask2former.py` & `pai-easycv-0.9.0/easycv/models/segmentation/mask2former.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/encoder_decoder.py` & `pai-easycv-0.9.0/easycv/models/segmentation/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/utils/shape_convert.py` & `pai-easycv-0.9.0/easycv/models/segmentation/utils/shape_convert.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/utils/matcher.py` & `pai-easycv-0.9.0/easycv/models/segmentation/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/utils/point_rend.py` & `pai-easycv-0.9.0/easycv/models/segmentation/utils/point_rend.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/utils/embed.py` & `pai-easycv-0.9.0/easycv/models/segmentation/utils/embed.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/utils/criterion.py` & `pai-easycv-0.9.0/easycv/models/segmentation/utils/criterion.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/utils/panoptic_gt_processing.py` & `pai-easycv-0.9.0/easycv/models/segmentation/utils/panoptic_gt_processing.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/heads/transformer_decoder.py` & `pai-easycv-0.9.0/easycv/models/segmentation/heads/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/heads/fcn_head.py` & `pai-easycv-0.9.0/easycv/models/segmentation/heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/heads/segformer_head.py` & `pai-easycv-0.9.0/easycv/models/segmentation/heads/segformer_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/heads/mask2former_head.py` & `pai-easycv-0.9.0/easycv/models/segmentation/heads/mask2former_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/heads/pixel_decoder.py` & `pai-easycv-0.9.0/easycv/models/segmentation/heads/pixel_decoder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/heads/uper_head.py` & `pai-easycv-0.9.0/easycv/models/segmentation/heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/segmentation/heads/base.py` & `pai-easycv-0.9.0/easycv/models/segmentation/heads/base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/pose/top_down.py` & `pai-easycv-0.9.0/easycv/models/pose/top_down.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/pose/heads/topdown_heatmap_simple_head.py` & `pai-easycv-0.9.0/easycv/models/pose/heads/topdown_heatmap_simple_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/pose/heads/topdown_heatmap_base_head.py` & `pai-easycv-0.9.0/easycv/models/pose/heads/topdown_heatmap_base_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/mse_loss.py` & `pai-easycv-0.9.0/easycv/models/loss/mse_loss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/iou_loss.py` & `pai-easycv-0.9.0/easycv/models/loss/iou_loss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/set_criterion/set_criterion.py` & `pai-easycv-0.9.0/easycv/models/loss/set_criterion/set_criterion.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/set_criterion/matcher.py` & `pai-easycv-0.9.0/easycv/models/loss/set_criterion/matcher.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/ocr_rec_multi_loss.py` & `pai-easycv-0.9.0/easycv/models/loss/ocr_rec_multi_loss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/cross_entropy_loss.py` & `pai-easycv-0.9.0/easycv/models/loss/cross_entropy_loss.py`

 * *Files 5% similar despite different names*

```diff
@@ -341,7 +341,61 @@
         included into the backward graph, `loss_` must be the prefix of the
         name.
 
         Returns:
             str: The name of this loss item.
         """
         return self._loss_name
+
+
+@LOSSES.register_module()
+class AsymmetricLoss(nn.Module):
+
+    def __init__(self,
+                 gamma_neg=4,
+                 gamma_pos=1,
+                 clip=0.05,
+                 eps=1e-8,
+                 disable_torch_grad_focal_loss=True):
+        super(AsymmetricLoss, self).__init__()
+
+        self.gamma_neg = gamma_neg
+        self.gamma_pos = gamma_pos
+        self.clip = clip
+        self.disable_torch_grad_focal_loss = disable_torch_grad_focal_loss
+        self.eps = eps
+
+    def forward(self, x, y):
+        """"
+        Parameters
+        ----------
+        x: input logits
+        y: targets (multi-label binarized vector)
+        """
+
+        # Calculating Probabilities
+        x_sigmoid = torch.sigmoid(x)
+        xs_pos = x_sigmoid
+        xs_neg = 1 - x_sigmoid
+
+        # Asymmetric Clipping
+        if self.clip is not None and self.clip > 0:
+            xs_neg = (xs_neg + self.clip).clamp(max=1)
+
+        # Basic CE calculation
+        los_pos = y * torch.log(xs_pos.clamp(min=self.eps))
+        los_neg = (1 - y) * torch.log(xs_neg.clamp(min=self.eps))
+        loss = los_pos + los_neg
+
+        # Asymmetric Focusing
+        if self.gamma_neg > 0 or self.gamma_pos > 0:
+            if self.disable_torch_grad_focal_loss:
+                torch.set_grad_enabled(False)
+            pt0 = xs_pos * y
+            pt1 = xs_neg * (1 - y)  # pt = p if t > 0 else 1-p
+            pt = pt0 + pt1
+            one_sided_gamma = self.gamma_pos * y + self.gamma_neg * (1 - y)
+            one_sided_w = torch.pow(1 - pt, one_sided_gamma)
+            if self.disable_torch_grad_focal_loss:
+                torch.set_grad_enabled(True)
+            loss *= one_sided_w
+        return -loss.sum()
```

### Comparing `pai-easycv-0.8.0/easycv/models/loss/l1_loss.py` & `pai-easycv-0.9.0/easycv/models/loss/l1_loss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/__init__.py` & `pai-easycv-0.9.0/easycv/models/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/utils.py` & `pai-easycv-0.9.0/easycv/models/loss/utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/pytorch_metric_learning.py` & `pai-easycv-0.9.0/easycv/models/loss/pytorch_metric_learning.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/face_keypoint_loss.py` & `pai-easycv-0.9.0/easycv/models/loss/face_keypoint_loss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/det_db_loss.py` & `pai-easycv-0.9.0/easycv/models/loss/det_db_loss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/loss/focal_loss.py` & `pai-easycv-0.9.0/easycv/models/loss/focal_loss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/dense_heads/dense_test_mixins.py` & `pai-easycv-0.9.0/easycv/models/detection/dense_heads/dense_test_mixins.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/dense_heads/anchor_free_head.py` & `pai-easycv-0.9.0/easycv/models/detection/dense_heads/anchor_free_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/dense_heads/base_dense_head.py` & `pai-easycv-0.9.0/easycv/models/detection/dense_heads/base_dense_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/necks/fpn.py` & `pai-easycv-0.9.0/easycv/models/detection/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/necks/sfp.py` & `pai-easycv-0.9.0/easycv/models/detection/necks/sfp.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/detr/detr_head.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/detr/detr_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/detr/detr_transformer.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/detr/detr_transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/fcos/fcos_head.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/fcos/fcos_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/dino/dino_head.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/dino/dino_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/dino/deformable_transformer.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/dino/deformable_transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/dino/cdn_components.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/dino/cdn_components.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/__init__.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/yolo_head_template.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/yolo_head_template.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/yolo_pafpn.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/yolo_head.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/yolo_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/asff.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/asff.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/yolox.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/yolox.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/yolox/tood_head.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/yolox/tood_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/detection.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/detection.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/yolox_edge/yolox_edge.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/yolox_edge/yolox_edge.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/dab_detr_head.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/dab_detr_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/dn_components.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/dn_components.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/attention.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/attention.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/detectors/dab_detr/dab_detr_transformer.py` & `pai-easycv-0.9.0/easycv/models/detection/detectors/dab_detr/dab_detr_transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/utils/boxes.py` & `pai-easycv-0.9.0/easycv/models/detection/utils/boxes.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/utils/__init__.py` & `pai-easycv-0.9.0/easycv/models/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/utils/generator.py` & `pai-easycv-0.9.0/easycv/models/detection/utils/generator.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/utils/postprocess.py` & `pai-easycv-0.9.0/easycv/models/detection/utils/postprocess.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection/utils/misc.py` & `pai-easycv-0.9.0/easycv/models/detection/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/postprocess/rec_postprocess.py` & `pai-easycv-0.9.0/easycv/models/ocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/postprocess/db_postprocess.py` & `pai-easycv-0.9.0/easycv/models/ocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/necks/db_fpn.py` & `pai-easycv-0.9.0/easycv/models/ocr/necks/db_fpn.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/necks/squence_encoder.py` & `pai-easycv-0.9.0/easycv/models/ocr/necks/squence_encoder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/cls/text_classifier.py` & `pai-easycv-0.9.0/easycv/models/ocr/cls/text_classifier.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/backbones/rec_svtrnet.py` & `pai-easycv-0.9.0/easycv/models/ocr/backbones/rec_svtrnet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/backbones/rec_mv1_enhance.py` & `pai-easycv-0.9.0/easycv/models/ocr/backbones/rec_mv1_enhance.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/backbones/rec_mobilenet_v3.py` & `pai-easycv-0.9.0/easycv/models/ocr/backbones/rec_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/backbones/det_resnet_vd.py` & `pai-easycv-0.9.0/easycv/models/ocr/backbones/det_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/backbones/det_mobilenet_v3.py` & `pai-easycv-0.9.0/easycv/models/ocr/backbones/det_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/rec/ocr_rec.py` & `pai-easycv-0.9.0/easycv/models/ocr/rec/ocr_rec.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/det/db_net.py` & `pai-easycv-0.9.0/easycv/models/ocr/det/db_net.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/heads/db_head.py` & `pai-easycv-0.9.0/easycv/models/ocr/heads/db_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/ocr/heads/rec_head.py` & `pai-easycv-0.9.0/easycv/models/ocr/heads/rec_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/inceptionv3.py` & `pai-easycv-0.9.0/easycv/models/backbones/inceptionv3.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/benchmark_mlp.py` & `pai-easycv-0.9.0/easycv/models/backbones/benchmark_mlp.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/mae_vit_transformer.py` & `pai-easycv-0.9.0/easycv/models/backbones/mae_vit_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
             requires_grad=False)  # fixed sin-cos embedding
         self.blocks = nn.ModuleList([
             Block(
                 embed_dim,
                 num_heads,
                 mlp_ratio,
                 qkv_bias=True,
-                qk_scale=None,
                 norm_layer=norm_layer) for i in range(depth)
         ])
         self.norm = norm_layer(embed_dim)
 
     def init_weights(self):
         w = self.patch_embed.proj.weight.data
         torch.nn.init.xavier_uniform_(w.view([w.shape[0], -1]))
```

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/swin_transformer_dynamic.py` & `pai-easycv-0.9.0/easycv/models/backbones/swin_transformer_dynamic.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/conv_vitdet.py` & `pai-easycv-0.9.0/easycv/models/backbones/conv_vitdet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/resnet.py` & `pai-easycv-0.9.0/easycv/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/swin_transformer.py` & `pai-easycv-0.9.0/easycv/models/backbones/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/vision_transformer.py` & `pai-easycv-0.9.0/easycv/models/backbones/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/mobilenetv2.py` & `pai-easycv-0.9.0/easycv/models/backbones/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/resnet_jit.py` & `pai-easycv-0.9.0/easycv/models/backbones/resnet_jit.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/vit_transformer_dynamic.py` & `pai-easycv-0.9.0/easycv/models/backbones/vit_transformer_dynamic.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/shuffle_transformer.py` & `pai-easycv-0.9.0/easycv/models/backbones/shuffle_transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/resnext.py` & `pai-easycv-0.9.0/easycv/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/__init__.py` & `pai-easycv-0.9.0/easycv/models/backbones/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 from .benchmark_mlp import BenchMarkMLP
 from .bninception import BNInception
+from .clip_bert import ClipBertClassification
 from .conv_mae_vit import FastConvMAEViT
 from .conv_vitdet import ConvViTDet
 from .edgevit import EdgeVit
 from .efficientformer import EfficientFormer
 from .face_keypoint_backbone import FaceKeypointBackbone
 from .genet import PlainNet
 from .hrnet import HRNet
@@ -18,9 +19,11 @@
 from .repvgg_yolox_backbone import RepVGGYOLOX
 from .resnest import ResNeSt
 from .resnet import ResNet
 from .resnet_jit import ResNetJIT
 from .resnext import ResNeXt
 from .shuffle_transformer import ShuffleTransformer
 from .swin_transformer import SwinTransformer
+from .swin_transformer3d import SwinTransformer3D
 from .vision_transformer import VisionTransformer
 from .vitdet import ViTDet
+from .x3d import X3D
```

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/edgevit.py` & `pai-easycv-0.9.0/easycv/models/backbones/edgevit.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/genet.py` & `pai-easycv-0.9.0/easycv/models/backbones/genet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/face_keypoint_backbone.py` & `pai-easycv-0.9.0/easycv/models/backbones/face_keypoint_backbone.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/mit.py` & `pai-easycv-0.9.0/easycv/models/backbones/mit.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/darknet.py` & `pai-easycv-0.9.0/easycv/models/backbones/darknet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/vitdet.py` & `pai-easycv-0.9.0/easycv/models/backbones/vitdet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/conv_mae_vit.py` & `pai-easycv-0.9.0/easycv/models/backbones/conv_mae_vit.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/efficientformer.py` & `pai-easycv-0.9.0/easycv/models/backbones/efficientformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/hrnet.py` & `pai-easycv-0.9.0/easycv/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/repvgg_yolox_backbone.py` & `pai-easycv-0.9.0/easycv/models/backbones/repvgg_yolox_backbone.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/lighthrnet.py` & `pai-easycv-0.9.0/easycv/models/backbones/lighthrnet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/mnasnet.py` & `pai-easycv-0.9.0/easycv/models/backbones/mnasnet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/network_blocks.py` & `pai-easycv-0.9.0/easycv/models/backbones/network_blocks.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/bninception.py` & `pai-easycv-0.9.0/easycv/models/backbones/bninception.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/xcit_transformer.py` & `pai-easycv-0.9.0/easycv/models/backbones/xcit_transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/pytorch_image_models_wrapper.py` & `pai-easycv-0.9.0/easycv/models/backbones/pytorch_image_models_wrapper.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/backbones/resnest.py` & `pai-easycv-0.9.0/easycv/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/bevformer_head.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/bevformer_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,28 +642,30 @@
         # for one2many task
         if 'all_cls_scores_aux' in preds_dicts and self.one2many_gt_mul:
             all_cls_scores_aux = preds_dicts['all_cls_scores_aux']
             all_bbox_preds_aux = preds_dicts['all_bbox_preds_aux']
 
             gt_bboxes_list_aux = []
             gt_labels_list_aux = []
-            for gt_bboxes, gt_labels in zip(gt_bboxes_list, gt_labels_list):
-                gt_bboxes_list_aux.append(
-                    gt_bboxes.repeat(self.one2many_gt_mul, 1))
-                gt_labels_list_aux.append(
-                    gt_labels.repeat(self.one2many_gt_mul))
+            # for gt_bboxes, gt_labels in zip(gt_bboxes_list, gt_labels_list):
+            #     gt_bboxes_list_aux.append(
+            #         gt_bboxes.repeat(self.one2many_gt_mul, 1))
+            #     gt_labels_list_aux.append(
+            #         gt_labels.repeat(self.one2many_gt_mul))
             # for classwise multiply
-            # for gt_bboxes, gt_labels in zip(gt_bboxes_list,gt_labels_list):
-            #     gt_bboxes_aux = []
-            #     gt_labels_aux = []
-            #     for gt_bbox, gt_label in zip(gt_bboxes, gt_labels):
-            #         gt_bboxes_aux += [gt_bbox]*self.one2many_gt_mul[gt_label]
-            #         gt_labels_aux += [gt_label]*self.one2many_gt_mul[gt_label]
-            #     gt_bboxes_list_aux.append(torch.stack(gt_bboxes_aux))
-            #     gt_labels_list_aux.append(torch.stack(gt_labels_aux))
+            for gt_bboxes, gt_labels in zip(gt_bboxes_list, gt_labels_list):
+                gt_bboxes_aux = []
+                gt_labels_aux = []
+                for gt_bbox, gt_label in zip(gt_bboxes, gt_labels):
+                    gt_bboxes_aux += [gt_bbox] * self.one2many_gt_mul[gt_label]
+                    gt_labels_aux += [gt_label
+                                      ] * self.one2many_gt_mul[gt_label]
+                gt_bboxes_list_aux.append(torch.stack(gt_bboxes_aux))
+                gt_labels_list_aux.append(torch.stack(gt_labels_aux))
+
             all_gt_bboxes_list_aux = [
                 gt_bboxes_list_aux for _ in range(num_dec_layers)
             ]
             all_gt_labels_list_aux = [
                 gt_labels_list_aux for _ in range(num_dec_layers)
             ]
             losses_cls_aux, losses_bbox_aux = multi_apply(
```

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/transformer.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/__init__.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/attentions/multi_scale_deformable_attention.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/attentions/multi_scale_deformable_attention.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/attentions/temporal_self_attention.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/attentions/temporal_self_attention.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/attentions/spatial_cross_attention.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/attentions/spatial_cross_attention.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/bevformer/bevformer.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/bevformer/bevformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/mvx_two_stage.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/mvx_two_stage.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/detectors/base.py` & `pai-easycv-0.9.0/easycv/models/detection3d/detectors/base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/detection3d/utils/grid_mask.py` & `pai-easycv-0.9.0/easycv/models/detection3d/utils/grid_mask.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/classification/classification.py` & `pai-easycv-0.9.0/easycv/models/classification/classification.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/classification/necks.py` & `pai-easycv-0.9.0/easycv/models/classification/necks.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/base.py` & `pai-easycv-0.9.0/easycv/models/base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/sobel.py` & `pai-easycv-0.9.0/easycv/models/utils/sobel.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/norm.py` & `pai-easycv-0.9.0/easycv/models/utils/norm.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/transformer.py` & `pai-easycv-0.9.0/easycv/models/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/conv_ws.py` & `pai-easycv-0.9.0/easycv/models/utils/conv_ws.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/face_keypoint_utils.py` & `pai-easycv-0.9.0/easycv/models/utils/face_keypoint_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/pos_embed.py` & `pai-easycv-0.9.0/easycv/models/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/__init__.py` & `pai-easycv-0.9.0/easycv/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/dist_utils.py` & `pai-easycv-0.9.0/easycv/models/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/conv_module.py` & `pai-easycv-0.9.0/easycv/models/utils/conv_module.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/ops.py` & `pai-easycv-0.9.0/easycv/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/multi_pooling.py` & `pai-easycv-0.9.0/easycv/models/utils/multi_pooling.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/init_weights.py` & `pai-easycv-0.9.0/easycv/models/utils/init_weights.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/activation.py` & `pai-easycv-0.9.0/easycv/models/utils/activation.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/res_layer.py` & `pai-easycv-0.9.0/easycv/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/utils/gather_layer.py` & `pai-easycv-0.9.0/easycv/models/utils/gather_layer.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/heads/mp_metric_head.py` & `pai-easycv-0.9.0/easycv/models/heads/mp_metric_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/heads/multi_cls_head.py` & `pai-easycv-0.9.0/easycv/models/heads/multi_cls_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/heads/cls_head.py` & `pai-easycv-0.9.0/easycv/models/heads/cls_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/heads/latent_pred_head.py` & `pai-easycv-0.9.0/easycv/models/heads/latent_pred_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/models/heads/contrastive_head.py` & `pai-easycv-0.9.0/easycv/models/heads/contrastive_head.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/points/cam_points.py` & `pai-easycv-0.9.0/easycv/core/points/cam_points.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/points/__init__.py` & `pai-easycv-0.9.0/easycv/core/points/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/points/depth_points.py` & `pai-easycv-0.9.0/easycv/core/points/depth_points.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/points/base_points.py` & `pai-easycv-0.9.0/easycv/core/points/base_points.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/points/lidar_points.py` & `pai-easycv-0.9.0/easycv/core/points/lidar_points.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/standard_fields.py` & `pai-easycv-0.9.0/easycv/core/standard_fields.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/sailfish/linear.py` & `pai-easycv-0.9.0/easycv/core/sailfish/linear.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/sailfish/loss.py` & `pai-easycv-0.9.0/easycv/core/sailfish/loss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/sailfish/__init__.py` & `pai-easycv-0.9.0/easycv/core/sailfish/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/sailfish/util.py` & `pai-easycv-0.9.0/easycv/core/sailfish/util.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/sailfish/activation.py` & `pai-easycv-0.9.0/easycv/core/sailfish/activation.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/sailfish/function.py` & `pai-easycv-0.9.0/easycv/core/sailfish/function.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/coders/nms_free_coder.py` & `pai-easycv-0.9.0/easycv/core/bbox/coders/nms_free_coder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/coders/base_bbox_coder.py` & `pai-easycv-0.9.0/easycv/core/bbox/coders/base_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/builder.py` & `pai-easycv-0.9.0/easycv/core/bbox/builder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/structures/cam_box3d.py` & `pai-easycv-0.9.0/easycv/core/bbox/structures/cam_box3d.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/structures/box_3d_mode.py` & `pai-easycv-0.9.0/easycv/core/bbox/structures/box_3d_mode.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/structures/depth_box3d.py` & `pai-easycv-0.9.0/easycv/core/bbox/structures/depth_box3d.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/structures/__init__.py` & `pai-easycv-0.9.0/easycv/core/bbox/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/structures/utils.py` & `pai-easycv-0.9.0/easycv/core/bbox/structures/utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/structures/lidar_box3d.py` & `pai-easycv-0.9.0/easycv/core/bbox/structures/lidar_box3d.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/structures/coord_3d_mode.py` & `pai-easycv-0.9.0/easycv/core/bbox/structures/coord_3d_mode.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/structures/base_box3d.py` & `pai-easycv-0.9.0/easycv/core/bbox/structures/base_box3d.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/assigners/assign_result.py` & `pai-easycv-0.9.0/easycv/core/bbox/assigners/assign_result.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/assigners/hungarian_assigner_3d.py` & `pai-easycv-0.9.0/easycv/core/bbox/assigners/hungarian_assigner_3d.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/__init__.py` & `pai-easycv-0.9.0/easycv/core/bbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/match_costs/match_cost.py` & `pai-easycv-0.9.0/easycv/core/bbox/match_costs/match_cost.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/bbox_util.py` & `pai-easycv-0.9.0/easycv/core/bbox/bbox_util.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/iou_calculators/iou2d_calculator.py` & `pai-easycv-0.9.0/easycv/core/bbox/iou_calculators/iou2d_calculator.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/samplers/base_sampler.py` & `pai-easycv-0.9.0/easycv/core/bbox/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/samplers/pseudo_sampler.py` & `pai-easycv-0.9.0/easycv/core/bbox/samplers/pseudo_sampler.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/bbox/samplers/sampling_result.py` & `pai-easycv-0.9.0/easycv/core/bbox/samplers/sampling_result.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/visualization/image.py` & `pai-easycv-0.9.0/easycv/core/visualization/image.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/visualization/image_3d.py` & `pai-easycv-0.9.0/easycv/core/visualization/image_3d.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/visualization/open3d_vis.py` & `pai-easycv-0.9.0/easycv/core/visualization/open3d_vis.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/anchor/builder.py` & `pai-easycv-0.9.0/easycv/core/anchor/builder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/anchor/point_generator.py` & `pai-easycv-0.9.0/easycv/core/anchor/point_generator.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/optimizer/ranger.py` & `pai-easycv-0.9.0/easycv/core/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/optimizer/adam.py` & `pai-easycv-0.9.0/easycv/core/optimizer/adam.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/optimizer/layer_decay_optimizer_constructor.py` & `pai-easycv-0.9.0/easycv/core/optimizer/layer_decay_optimizer_constructor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/optimizer/lamb.py` & `pai-easycv-0.9.0/easycv/core/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/optimizer/lars.py` & `pai-easycv-0.9.0/easycv/core/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/face_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/face_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/coco_tools.py` & `pai-easycv-0.9.0/easycv/core/evaluation/coco_tools.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/builder.py` & `pai-easycv-0.9.0/easycv/core/evaluation/builder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/top_down_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/top_down_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/custom_cocotools/cocoeval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/custom_cocotools/cocoeval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/auc_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/auc_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/keypoint_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/keypoint_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/wholebody_keypoint_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/wholebody_keypoint_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/__init__.py` & `pai-easycv-0.9.0/easycv/core/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/faceid_pair_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/faceid_pair_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/metrics.py` & `pai-easycv-0.9.0/easycv/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/coco_evaluation.py` & `pai-easycv-0.9.0/easycv/core/evaluation/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/segmentation_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/segmentation_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/base_evaluator.py` & `pai-easycv-0.9.0/easycv/core/evaluation/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/ocr_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/ocr_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/mse_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/mse_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/retrival_topk_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/retrival_topk_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/nuscenes_eval.py` & `pai-easycv-0.9.0/easycv/core/evaluation/nuscenes_eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/evaluation/metric_registry.py` & `pai-easycv-0.9.0/easycv/core/evaluation/metric_registry.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/utils/array_converter.py` & `pai-easycv-0.9.0/easycv/core/utils/array_converter.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/utils/misc.py` & `pai-easycv-0.9.0/easycv/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/post_processing/merge_augs.py` & `pai-easycv-0.9.0/easycv/core/post_processing/merge_augs.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/post_processing/box3d_nms.py` & `pai-easycv-0.9.0/easycv/core/post_processing/box3d_nms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/post_processing/__init__.py` & `pai-easycv-0.9.0/easycv/core/post_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/post_processing/nms.py` & `pai-easycv-0.9.0/easycv/core/post_processing/nms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/core/post_processing/pose_transforms.py` & `pai-easycv-0.9.0/easycv/core/post_processing/pose_transforms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/swav/swav_genet_8xb32_200e_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/swav/swav_genet_8xb32_200e_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/swav/swav_rn50_8xb32_200e_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/swav/swav_rn50_8xb32_200e_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/fast_convmae/fast_convmae_vit_base_patch16_8xb64_50e.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/fast_convmae/fast_convmae_vit_base_patch16_8xb64_50e.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/simclr/simclr_rn50_mocov2_neck_8xb32_200e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/simclr/simclr_rn50_mocov2_neck_8xb32_200e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/mixco/mixco_genet_8xb32_200e_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/mixco/mixco_genet_8xb32_200e_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/mixco/mixco_rn50_4xb64_200e_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/mixco/mixco_rn50_4xb64_200e_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/moby/moby_dynamic_swin_tiny_8xb64_300e_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/moby/moby_dynamic_swin_tiny_8xb64_300e_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/moby/moby_rn50_4xb128_100e_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/moby/moby_rn50_4xb128_100e_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/moby/moby_deit_small_p16_4xb128_300e_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/moby/moby_deit_small_p16_4xb128_300e_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/moby/moby_deit_small_4xb32_100e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/moby/moby_deit_small_4xb32_100e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/byol/byol_rn50_8xb32_200e.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/byol/byol_rn50_8xb32_200e.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/mae/mae_vit_base_patch16_8xb64_1600e.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/mae/mae_vit_base_patch16_8xb64_1600e.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/selfsup/mae/mae_vit_large_patch16_8xb32_1600e.py` & `pai-easycv-0.9.0/easycv/configs/selfsup/mae/mae_vit_large_patch16_8xb32_1600e.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/edge_models/yolox_m.py` & `pai-easycv-0.9.0/easycv/configs/edge_models/yolox_m.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/edge_models/yolox_l.py` & `pai-easycv-0.9.0/easycv/configs/edge_models/yolox_l.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/edge_models/yolox_nano.py` & `pai-easycv-0.9.0/easycv/configs/edge_models/yolox_nano.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/edge_models/yolox_tiny.py` & `pai-easycv-0.9.0/easycv/configs/edge_models/yolox_tiny.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/edge_models/yolox_edge.py` & `pai-easycv-0.9.0/easycv/configs/edge_models/yolox_edge.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/edge_models/yolox_s.py` & `pai-easycv-0.9.0/easycv/configs/edge_models/yolox_s.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/face/face_96x96_wingloss.py` & `pai-easycv-0.9.0/easycv/configs/face/face_96x96_wingloss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_instance.py` & `pai-easycv-0.9.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_instance.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e127_semantic.py` & `pai-easycv-0.9.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e127_semantic.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_panoptic.py` & `pai-easycv-0.9.0/easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_panoptic.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/segmentation/segformer/segformer_b0_coco.py` & `pai-easycv-0.9.0/easycv/configs/segmentation/segformer/segformer_b0_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/segmentation/segformer/segformer_b5_coco.py` & `pai-easycv-0.9.0/easycv/configs/segmentation/segformer/segformer_b5_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/segmentation/upernet/upernet_r50_512x512_8xb4_60e_voc12aug.py` & `pai-easycv-0.9.0/easycv/configs/segmentation/upernet/upernet_r50_512x512_8xb4_60e_voc12aug.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,17 @@
     'background', 'aeroplane', 'bicycle', 'bird', 'boat', 'bottle', 'bus',
     'car', 'cat', 'chair', 'cow', 'diningtable', 'dog', 'horse', 'motorbike',
     'person', 'pottedplant', 'sheep', 'sofa', 'train', 'tvmonitor'
 ]
 
 # model settings
 num_classes = 21
-norm_cfg = dict(type='SyncBN', requires_grad=True)
+# norm_cfg = dict(type='SyncBN', requires_grad=True)  # multi gpus
+norm_cfg = dict(type='BN', requires_grad=True)
+
 model = dict(
     type='EncoderDecoder',
     pretrained='open-mmlab://resnet50_v1c',
     backbone=dict(
         type='ResNetV1c',
         depth=50,
         num_stages=4,
@@ -52,14 +54,31 @@
     # model training and testing settings
     train_cfg=dict(),
     test_cfg=dict(mode='whole'))
 
 # dataset settings
 dataset_type = 'SegDataset'
 data_root = 'data/VOCdevkit/VOC2012/'
+
+train_img_root = data_root + 'JPEGImages'
+train_label_root = data_root + 'SegmentationClass'
+train_list_file = data_root + 'ImageSets/Segmentation/train.txt'
+
+train_aug_img_root = data_root + 'JPEGImages'
+train_aug_label_root = data_root + 'SegmentationClassAug'
+train_aug_list_file = data_root + 'ImageSets/Segmentation/aug.txt'
+
+val_img_root = data_root + 'JPEGImages'
+val_label_root = data_root + 'SegmentationClass'
+val_list_file = data_root + 'ImageSets/Segmentation/val.txt'
+
+test_img_root = data_root + 'JPEGImages'
+test_label_root = data_root + 'SegmentationClass'
+test_list_file = data_root + 'ImageSets/Segmentation/test.txt'
+
 img_norm_cfg = dict(
     mean=[123.675, 116.28, 103.53], std=[58.395, 57.12, 57.375], to_rgb=True)
 crop_size = (512, 512)
 train_pipeline = [
     dict(type='MMResize', img_scale=(2048, 512), ratio_range=(0.5, 2.0)),
     dict(type='SegRandomCrop', crop_size=crop_size, cat_max_ratio=0.75),
     dict(type='MMRandomFlip', flip_ratio=0.5),
@@ -100,45 +119,45 @@
         type=dataset_type,
         ignore_index=255,
         data_source=dict(
             type='SourceConcat',
             data_source_list=[
                 dict(
                     type='SegSourceRaw',
-                    img_root=data_root + 'JPEGImages',
-                    label_root=data_root + 'SegmentationClass',
-                    split=data_root + 'ImageSets/Segmentation/train.txt',
+                    img_root=train_img_root,
+                    label_root=train_label_root,
+                    split=train_list_file,
                     classes=CLASSES),
                 dict(
                     type='SegSourceRaw',
-                    img_root=data_root + 'JPEGImages',
-                    label_root=data_root + 'SegmentationClassAug',
-                    split=data_root + 'ImageSets/Segmentation/aug.txt',
+                    img_root=train_aug_img_root,
+                    label_root=train_aug_label_root,
+                    split=train_aug_list_file,
                     classes=CLASSES),
             ]),
         pipeline=train_pipeline),
     val=dict(
         imgs_per_gpu=1,
         ignore_index=255,
         type=dataset_type,
         data_source=dict(
             type='SegSourceRaw',
-            img_root=data_root + 'JPEGImages',
-            label_root=data_root + 'SegmentationClass',
-            split=data_root + 'ImageSets/Segmentation/val.txt',
+            img_root=val_img_root,
+            label_root=val_label_root,
+            split=val_list_file,
             classes=CLASSES,
         ),
         pipeline=test_pipeline),
     test=dict(
         type=dataset_type,
         data_source=dict(
             type='SegSourceRaw',
-            img_root=data_root + 'JPEGImages',
-            label_root=data_root + 'SegmentationClass',
-            split=data_root + 'ImageSets/Segmentation/test.txt',
+            img_root=test_img_root,
+            label_root=test_label_root,
+            split=test_list_file,
             classes=CLASSES,
         ),
         pipeline=test_pipeline))
 
 # optimizer
 optimizer = dict(type='SGD', lr=0.01, momentum=0.9, weight_decay=0.0005)
 optimizer_config = dict()
```

### Comparing `pai-easycv-0.8.0/easycv/configs/segmentation/fcn/fcn_r50-d8_512x512_8xb4_60e_voc12aug.py` & `pai-easycv-0.9.0/easycv/configs/segmentation/fcn/fcn_r50-d8_512x512_8xb4_60e_voc12aug.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,18 @@
     'background', 'aeroplane', 'bicycle', 'bird', 'boat', 'bottle', 'bus',
     'car', 'cat', 'chair', 'cow', 'diningtable', 'dog', 'horse', 'motorbike',
     'person', 'pottedplant', 'sheep', 'sofa', 'train', 'tvmonitor'
 ]
 
 # model settings
 num_classes = 21
-norm_cfg = dict(type='SyncBN', requires_grad=True)
+
+# norm_cfg = dict(type='SyncBN', requires_grad=True)  # multi gpus
+norm_cfg = dict(type='BN', requires_grad=True)
+
 model = dict(
     type='EncoderDecoder',
     pretrained='open-mmlab://resnet50_v1c',
     backbone=dict(
         type='ResNetV1c',
         depth=50,
         num_stages=4,
@@ -53,14 +56,31 @@
     # model training and testing settings
     train_cfg=dict(),
     test_cfg=dict(mode='whole'))
 
 # dataset settings
 dataset_type = 'SegDataset'
 data_root = 'data/VOCdevkit/VOC2012'
+
+train_img_root = data_root + 'JPEGImages'
+train_label_root = data_root + 'SegmentationClass'
+train_list_file = data_root + 'ImageSets/Segmentation/train.txt'
+
+train_aug_img_root = data_root + 'JPEGImages'
+train_aug_label_root = data_root + 'SegmentationClassAug'
+train_aug_list_file = data_root + 'ImageSets/Segmentation/aug.txt'
+
+val_img_root = data_root + 'JPEGImages'
+val_label_root = data_root + 'SegmentationClass'
+val_list_file = data_root + 'ImageSets/Segmentation/val.txt'
+
+test_img_root = data_root + 'JPEGImages'
+test_label_root = data_root + 'SegmentationClass'
+test_list_file = data_root + 'ImageSets/Segmentation/test.txt'
+
 img_norm_cfg = dict(
     mean=[123.675, 116.28, 103.53], std=[58.395, 57.12, 57.375], to_rgb=True)
 crop_size = (512, 512)
 train_pipeline = [
     dict(type='MMResize', img_scale=(2048, 512), ratio_range=(0.5, 2.0)),
     dict(type='SegRandomCrop', crop_size=crop_size, cat_max_ratio=0.75),
     dict(type='MMRandomFlip', flip_ratio=0.5),
@@ -101,45 +121,45 @@
         type=dataset_type,
         ignore_index=255,
         data_source=dict(
             type='SourceConcat',
             data_source_list=[
                 dict(
                     type='SegSourceRaw',
-                    img_root=data_root + 'JPEGImages',
-                    label_root=data_root + 'SegmentationClass',
-                    split=data_root + 'ImageSets/Segmentation/train.txt',
+                    img_root=train_img_root,
+                    label_root=train_label_root,
+                    split=train_list_file,
                     classes=CLASSES),
                 dict(
                     type='SegSourceRaw',
-                    img_root=data_root + 'JPEGImages',
-                    label_root=data_root + 'SegmentationClassAug',
-                    split=data_root + 'ImageSets/Segmentation/aug.txt',
+                    img_root=train_aug_img_root,
+                    label_root=train_aug_label_root,
+                    split=train_aug_list_file,
                     classes=CLASSES),
             ]),
         pipeline=train_pipeline),
     val=dict(
         imgs_per_gpu=1,
         ignore_index=255,
         type=dataset_type,
         data_source=dict(
             type='SegSourceRaw',
-            img_root=data_root + 'JPEGImages',
-            label_root=data_root + 'SegmentationClass',
-            split=data_root + 'ImageSets/Segmentation/val.txt',
+            img_root=val_img_root,
+            label_root=val_label_root,
+            split=val_list_file,
             classes=CLASSES,
         ),
         pipeline=test_pipeline),
     test=dict(
         type=dataset_type,
         data_source=dict(
             type='SegSourceRaw',
-            img_root=data_root + 'JPEGImages',
-            label_root=data_root + 'SegmentationClass',
-            split=data_root + 'ImageSets/Segmentation/test.txt',
+            img_root=test_img_root,
+            label_root=test_label_root,
+            split=test_list_file,
             classes=CLASSES,
         ),
         pipeline=test_pipeline))
 
 # optimizer
 optimizer = dict(type='SGD', lr=0.01, momentum=0.9, weight_decay=0.0005)
 optimizer_config = dict()
```

### Comparing `pai-easycv-0.8.0/easycv/configs/pose/hrnet_w48_coco_256x192_udp.py` & `pai-easycv-0.9.0/easycv/configs/pose/hrnet_w48_coco_256x192_udp.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/pose/litehrnet_30_coco_384x288.py` & `pai-easycv-0.9.0/easycv/configs/pose/litehrnet_30_coco_384x288.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/pose/hand/hrnet_w18_coco_wholebody_hand_256x256_dark.py` & `pai-easycv-0.9.0/easycv/configs/pose/hand/hrnet_w18_coco_wholebody_hand_256x256_dark.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/pose/hand/litehrnet_30_coco_wholebody_hand_256x256.py` & `pai-easycv-0.9.0/easycv/configs/pose/hand/litehrnet_30_coco_wholebody_hand_256x256.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/pose/wholebody/hrnet_w48_coco_wholebody_384x288_dark_plus.py` & `pai-easycv-0.9.0/easycv/configs/pose/wholebody/hrnet_w48_coco_wholebody_384x288_dark_plus.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/detr/detr.py` & `pai-easycv-0.9.0/easycv/configs/detection/detr/detr.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/detr/detr_r50_8x2_150e_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/detr/detr_r50_8x2_150e_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/fcos/fcos.py` & `pai-easycv-0.9.0/easycv/configs/detection/fcos/fcos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # model settings
+num_classes = 80
 model = dict(
     type='Detection',
     pretrained=True,
     backbone=dict(
         type='ResNet',
         depth=50,
         num_stages=4,
@@ -17,15 +18,15 @@
         out_channels=256,
         start_level=1,
         add_extra_convs='on_output',  # use P5
         num_outs=5,
         relu_before_extra_convs=True),
     head=dict(
         type='FCOSHead',
-        num_classes=80,
+        num_classes=num_classes,
         in_channels=256,
         stacked_convs=4,
         feat_channels=256,
         strides=[8, 16, 32, 64, 128],
         center_sampling=True,
         center_sample_radius=1.5,
         norm_on_bbox=True,
```

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/fcos/coco_detection.py` & `pai-easycv-0.9.0/easycv/configs/detection/vitdet/lsj_coco_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,37 +15,51 @@
 ]
 
 # dataset settings
 data_root = 'data/coco/'
 img_norm_cfg = dict(
     mean=[123.675, 116.28, 103.53], std=[58.395, 57.12, 57.375], to_rgb=True)
 
+image_size = (1024, 1024)
 train_pipeline = [
-    dict(type='MMResize', img_scale=(1333, 800), keep_ratio=True),
+    # large scale jittering
+    dict(
+        type='MMResize',
+        img_scale=image_size,
+        ratio_range=(0.1, 2.0),
+        multiscale_mode='range',
+        keep_ratio=True),
+    dict(
+        type='MMRandomCrop',
+        crop_type='absolute_range',
+        crop_size=image_size,
+        recompute_bbox=False,
+        allow_negative_crop=True),
+    dict(type='MMFilterAnnotations', min_gt_bbox_wh=(1e-2, 1e-2)),
     dict(type='MMRandomFlip', flip_ratio=0.5),
     dict(type='MMNormalize', **img_norm_cfg),
-    dict(type='MMPad', size_divisor=32),
+    dict(type='MMPad', size=image_size),
     dict(type='DefaultFormatBundle'),
     dict(
         type='Collect',
         keys=['img', 'gt_bboxes', 'gt_labels'],
         meta_keys=('filename', 'ori_filename', 'ori_shape', 'ori_img_shape',
                    'img_shape', 'pad_shape', 'scale_factor', 'flip',
                    'flip_direction', 'img_norm_cfg'))
 ]
 test_pipeline = [
     dict(
         type='MMMultiScaleFlipAug',
-        img_scale=(1333, 800),
+        img_scale=image_size,
         flip=False,
         transforms=[
             dict(type='MMResize', keep_ratio=True),
             dict(type='MMRandomFlip'),
             dict(type='MMNormalize', **img_norm_cfg),
-            dict(type='MMPad', size_divisor=32),
+            dict(type='MMPad', size_divisor=1024),
             dict(type='ImageToTensor', keys=['img']),
             dict(
                 type='Collect',
                 keys=['img'],
                 meta_keys=('filename', 'ori_filename', 'ori_shape',
                            'ori_img_shape', 'img_shape', 'pad_shape',
                            'scale_factor', 'flip', 'flip_direction',
@@ -83,19 +97,21 @@
         classes=CLASSES,
         test_mode=True,
         filter_empty_gt=False,
         iscrowd=True),
     pipeline=test_pipeline)
 
 data = dict(
-    imgs_per_gpu=2, workers_per_gpu=2, train=train_dataset, val=val_dataset)
+    imgs_per_gpu=4, workers_per_gpu=2, train=train_dataset, val=val_dataset
+)  # 64(total batch size) = 4 (batch size/per gpu) x 8 (gpu num) x 2(node)
 
 # evaluation
-eval_config = dict(interval=1, gpu_collect=False)
+eval_config = dict(initial=False, interval=1, gpu_collect=False)
 eval_pipelines = [
     dict(
         mode='test',
+        # dist_eval=True,
         evaluators=[
             dict(type='CocoDetectionEvaluator', classes=CLASSES),
         ],
     )
 ]
```

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/fcos/fcos_r50_caffe_1x_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/fcos/fcos_r50_caffe_1x_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/fcos/fcos_r50_torch_1x_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/fcos/fcos_r50_torch_1x_coco.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 optimizer_config = dict(grad_clip=None)
 # learning policy
 lr_config = dict(
     policy='step',
     warmup='linear',
     warmup_iters=500,
     warmup_ratio=1.0 / 3,
+    warmup_by_epoch=False,
     step=[8, 11])
 
 total_epochs = 12
 
 find_unused_parameters = False
```

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_r50.py` & `pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_r50.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_swinl_center_iou_memoryreduce_18e_obj2coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_swinl_center_iou_memoryreduce_18e_obj2coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/dino/dino_5sc_swinl_center_iou_memoryreduce_26e_obj365.py` & `pai-easycv-0.9.0/easycv/configs/detection/dino/dino_5sc_swinl_center_iou_memoryreduce_26e_obj365.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/dino/dino_4sc_swinl.py` & `pai-easycv-0.9.0/easycv/configs/detection/dino/dino_4sc_swinl.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_tiny_8xb16_300e_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_tiny_8xb16_300e_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/yolox/pai_yoloxs_8xb16_300e_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/yolox/pai_yoloxs_8xb16_300e_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/yolox/pai_yoloxs_asff_8xb16_300e_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/yolox/pai_yoloxs_asff_8xb16_300e_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco_pai.py` & `pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco_pai.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 _base_ = '../../base.py'
 
+num_classes = 80
 # model settings s m l x
 model = dict(
     type='YOLOX',
     test_conf=0.01,
     nms_thre=0.65,
     backbone='CSPDarknet',
     model_type='s',  # s m l x tiny nano
     head=dict(
         type='YOLOXHead',
         model_type='s',
         obj_loss_type='BCE',
         reg_loss_type='giou',
-        num_classes=80,
+        num_classes=num_classes,
         decode_in_inference=True))
 
 # s m l x
 img_scale = (640, 640)
 random_size = (14, 26)
 scale_ratio = (0.1, 2)
```

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_voc.py` & `pai-easycv-0.9.0/easycv/configs/detection/yolox/yolox_s_8xb16_300e_voc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/yolox/pai_yoloxs_asff_tood3_8xb16_300e_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/yolox/pai_yoloxs_asff_tood3_8xb16_300e_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/common/dataset/autoaug_coco_detection.py` & `pai-easycv-0.9.0/easycv/configs/detection/common/dataset/autoaug_coco_detection.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/common/dataset/autoaug_obj365_val5k_detection.py` & `pai-easycv-0.9.0/easycv/configs/detection/common/dataset/autoaug_obj365_val5k_detection.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/common/dataset/autoaug_obj2coco_detection.py` & `pai-easycv-0.9.0/easycv/configs/detection/common/dataset/autoaug_obj2coco_detection.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_faster_rcnn.py` & `pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/vitdet/lsj_coco_instance.py` & `pai-easycv-0.9.0/easycv/configs/detection/vitdet/lsj_coco_instance.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_schedule_100e.py` & `pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_schedule_100e.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_mask_rcnn.py` & `pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_mask_rcnn.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/vitdet/lsj_coco_detection.py` & `pai-easycv-0.9.0/easycv/configs/detection/fcos/coco_detection.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,54 +12,45 @@
     'keyboard', 'cell phone', 'microwave', 'oven', 'toaster', 'sink',
     'refrigerator', 'book', 'clock', 'vase', 'scissors', 'teddy bear',
     'hair drier', 'toothbrush'
 ]
 
 # dataset settings
 data_root = 'data/coco/'
+train_ann_file = data_root + 'annotations/instances_train2017.json'
+train_img_prefix = data_root + 'train2017/'
+val_ann_file = data_root + 'annotations/instances_val2017.json'
+val_img_prefix = data_root + 'val2017/'
+
 img_norm_cfg = dict(
     mean=[123.675, 116.28, 103.53], std=[58.395, 57.12, 57.375], to_rgb=True)
 
-image_size = (1024, 1024)
 train_pipeline = [
-    # large scale jittering
-    dict(
-        type='MMResize',
-        img_scale=image_size,
-        ratio_range=(0.1, 2.0),
-        multiscale_mode='range',
-        keep_ratio=True),
-    dict(
-        type='MMRandomCrop',
-        crop_type='absolute_range',
-        crop_size=image_size,
-        recompute_bbox=False,
-        allow_negative_crop=True),
-    dict(type='MMFilterAnnotations', min_gt_bbox_wh=(1e-2, 1e-2)),
+    dict(type='MMResize', img_scale=(1333, 800), keep_ratio=True),
     dict(type='MMRandomFlip', flip_ratio=0.5),
     dict(type='MMNormalize', **img_norm_cfg),
-    dict(type='MMPad', size=image_size),
+    dict(type='MMPad', size_divisor=32),
     dict(type='DefaultFormatBundle'),
     dict(
         type='Collect',
         keys=['img', 'gt_bboxes', 'gt_labels'],
         meta_keys=('filename', 'ori_filename', 'ori_shape', 'ori_img_shape',
                    'img_shape', 'pad_shape', 'scale_factor', 'flip',
                    'flip_direction', 'img_norm_cfg'))
 ]
 test_pipeline = [
     dict(
         type='MMMultiScaleFlipAug',
-        img_scale=image_size,
+        img_scale=(1333, 800),
         flip=False,
         transforms=[
             dict(type='MMResize', keep_ratio=True),
             dict(type='MMRandomFlip'),
             dict(type='MMNormalize', **img_norm_cfg),
-            dict(type='MMPad', size_divisor=1024),
+            dict(type='MMPad', size_divisor=32),
             dict(type='ImageToTensor', keys=['img']),
             dict(
                 type='Collect',
                 keys=['img'],
                 meta_keys=('filename', 'ori_filename', 'ori_shape',
                            'ori_img_shape', 'img_shape', 'pad_shape',
                            'scale_factor', 'flip', 'flip_direction',
@@ -67,16 +58,16 @@
         ])
 ]
 
 train_dataset = dict(
     type='DetDataset',
     data_source=dict(
         type='DetSourceCoco',
-        ann_file=data_root + 'annotations/instances_train2017.json',
-        img_prefix=data_root + 'train2017/',
+        ann_file=train_ann_file,
+        img_prefix=train_img_prefix,
         pipeline=[
             dict(type='LoadImageFromFile'),
             dict(type='LoadAnnotations', with_bbox=True)
         ],
         classes=CLASSES,
         test_mode=False,
         filter_empty_gt=True,
@@ -84,34 +75,32 @@
     pipeline=train_pipeline)
 
 val_dataset = dict(
     type='DetDataset',
     imgs_per_gpu=1,
     data_source=dict(
         type='DetSourceCoco',
-        ann_file=data_root + 'annotations/instances_val2017.json',
-        img_prefix=data_root + 'val2017/',
+        ann_file=val_ann_file,
+        img_prefix=val_img_prefix,
         pipeline=[
             dict(type='LoadImageFromFile'),
             dict(type='LoadAnnotations', with_bbox=True)
         ],
         classes=CLASSES,
         test_mode=True,
         filter_empty_gt=False,
         iscrowd=True),
     pipeline=test_pipeline)
 
 data = dict(
-    imgs_per_gpu=4, workers_per_gpu=2, train=train_dataset, val=val_dataset
-)  # 64(total batch size) = 4 (batch size/per gpu) x 8 (gpu num) x 2(node)
+    imgs_per_gpu=2, workers_per_gpu=2, train=train_dataset, val=val_dataset)
 
 # evaluation
-eval_config = dict(initial=False, interval=1, gpu_collect=False)
+eval_config = dict(interval=1, gpu_collect=False)
 eval_pipelines = [
     dict(
         mode='test',
-        # dist_eval=True,
         evaluators=[
             dict(type='CocoDetectionEvaluator', classes=CLASSES),
         ],
     )
 ]
```

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/vitdet/vitdet_cascade_mask_rcnn.py` & `pai-easycv-0.9.0/easycv/configs/detection/vitdet/vitdet_cascade_mask_rcnn.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/mask_rcnn/mask_rcnn_r50_fpn.py` & `pai-easycv-0.9.0/easycv/configs/detection/mask_rcnn/mask_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/dab_detr/dab_detr_r50_8x2_50e_coco.py` & `pai-easycv-0.9.0/easycv/configs/detection/dab_detr/dab_detr_r50_8x2_50e_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection/dab_detr/dab_detr.py` & `pai-easycv-0.9.0/easycv/configs/detection/dab_detr/dab_detr.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/direction/direction_model.py` & `pai-easycv-0.9.0/easycv/configs/ocr/direction/direction_model.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_te.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_te.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_en.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_en.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_ch.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_ch.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_devanagari.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_devanagari.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_ka.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_ka.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_cyrillic.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_cyrillic.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_chinese_cht.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_chinese_cht.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_latin.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_latin.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_arabic.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_arabic.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_japan.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_japan.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_ta.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_ta.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/recognition/rec_model_korean.py` & `pai-easycv-0.9.0/easycv/configs/ocr/recognition/rec_model_korean.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/detection/det_model_en.py` & `pai-easycv-0.9.0/easycv/configs/ocr/detection/det_model_en.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/detection/det_model_ch_r50.py` & `pai-easycv-0.9.0/easycv/configs/ocr/detection/det_model_ch_r50.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/detection/det_model_ch.py` & `pai-easycv-0.9.0/easycv/configs/ocr/detection/det_model_ch.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/ocr/detection/det_model_en_r50.py` & `pai-easycv-0.9.0/easycv/configs/ocr/detection/det_model_en_r50.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/yolox_itag.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/yolox_itag.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/swav_r50_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/swav_r50_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/topdown_litehrnet_30.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/topdown_litehrnet_30.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/yolox_edge.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/yolox_edge.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/moco_r50_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/moco_r50_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/yolox.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/yolox.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/moco_r50_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/moco_r50_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/mae_vit_base_patch16.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/mae_vit_base_patch16.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/dino_timm.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/dino_timm.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/topdown_hrnet_w48_udp.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/topdown_hrnet_w48_udp.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/moco_timm_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/moco_timm_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/moby_timm_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/moby_timm_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/classification.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/classification.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/classification_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/classification_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/classification_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/classification_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/metric_learning/softmaxbased_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/metric_learning/softmaxbased_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/metric_learning/modelparallel_softmaxbased_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/metric_learning/modelparallel_softmaxbased_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/dino_timm_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/dino_timm_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/moco_timm_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/moco_timm_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/swav_r50_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/swav_r50_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/yolox_edge_itag.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/yolox_edge_itag.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/config_templates/dino_rn50_tfrecord_oss.py` & `pai-easycv-0.9.0/easycv/configs/config_templates/dino_rn50_tfrecord_oss.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes_hybrid.py` & `pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes_blancehybrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         relu_before_extra_convs=True),
     pts_bbox_head=dict(
         type='BEVFormerHead',
         bev_h=bev_h,
         bev_w=bev_w,
         num_query=900,
         num_query_one2many=1800,
-        one2many_gt_mul=4,
+        one2many_gt_mul=[2, 3, 7, 7, 9, 6, 7, 6, 2, 5],
         num_classes=10,
         in_channels=embed_dim,
         sync_cls_avg_factor=True,
         with_box_refine=True,
         as_two_stage=False,
         transformer=dict(
             type='PerceptionTransformer',
```

### Comparing `pai-easycv-0.8.0/easycv/configs/detection3d/bevformer/bevformer_tiny_r50_nuscenes.py` & `pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/bevformer_tiny_r50_nuscenes.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes.py` & `pai-easycv-0.9.0/easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/metric_learning/imagenet_resnet50_1000kid_jpg.py` & `pai-easycv-0.9.0/easycv/configs/metric_learning/imagenet_resnet50_1000kid_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/metric_learning/common/dataset/imagenet_metriclearning.py` & `pai-easycv-0.9.0/easycv/configs/metric_learning/common/dataset/imagenet_metriclearning.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/metric_learning/imagenet_timm_softmaxbased_jpg.py` & `pai-easycv-0.9.0/easycv/configs/metric_learning/imagenet_timm_softmaxbased_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/metric_learning/cub_resnet50_jpg.py` & `pai-easycv-0.9.0/easycv/configs/metric_learning/cub_resnet50_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/metric_learning/imagenet_resnet50_1000kid_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/metric_learning/imagenet_resnet50_1000kid_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/metric_learning/sop_timm_swinb_local.py` & `pai-easycv-0.9.0/easycv/configs/metric_learning/sop_timm_swinb_local.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/metric_learning/imagenet_timm_modelparallel_softmaxbased_jpg.py` & `pai-easycv-0.9.0/easycv/configs/metric_learning/imagenet_timm_modelparallel_softmaxbased_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/timm/timm_config.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/timm/timm_config.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/deit_base_patch16_224.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/deit_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/deit_schedule.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/deit_schedule.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/deit/randaug_imagenet_classification.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/deit/randaug_imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnext/resnext50-32x4d_b32x8_100e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnext/resnext50-32x4d_b32x8_100e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/deitiii_base_patch16_192.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/deitiii_base_patch16_192.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/threeaug_imagenet_classification_224.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/threeaug_imagenet_classification_224.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/threeaug_imagenet_classification_192.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/threeaug_imagenet_classification_192.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/deitiii/deitiii_schedule.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/deitiii/deitiii_schedule.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/EdgeVit_b512x8_300e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/EdgeVit_b512x8_300e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_xxs_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_xxs_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_xs_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_xs_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_s_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/edgevit/imagenet_edgeVIT_s_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/common/dataset/imagenet_classification.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/common/dataset/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/common/classification_base.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/common/classification_base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet50_tfrecord.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnet/imagenet_resnet50_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/resnet/resnet50_b32x8_100e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/resnet/resnet50_b32x8_100e_jpg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 _base_ = '../common/dataset/imagenet_classification.py'
 
+num_classes = 1000
 # model settings
 model = dict(
     type='Classification',
     backbone=dict(
         type='ResNet',
         depth=50,
         out_indices=[4],  # 0: conv-1, x: stage-x
@@ -12,15 +13,15 @@
         type='ClsHead',
         with_avg_pool=True,
         in_channels=2048,
         loss_config=dict(
             type='CrossEntropyLossWithLabelSmooth',
             label_smooth=0,
         ),
-        num_classes=1000))
+        num_classes=num_classes))
 
 # optimizer
 optimizer = dict(type='SGD', lr=0.1, momentum=0.9, weight_decay=0.0001)
 
 # learning policy
 lr_config = dict(policy='step', step=[30, 60, 90])
 checkpoint_config = dict(interval=10)
```

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/hrnet/hrnetw18_b32x8_100e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/hrnet/hrnetw18_b32x8_100e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/swin_tiny_patch4_window7_224_b64x16_300e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/swin_tiny_patch4_window7_224_b64x16_300e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/swint/imagenet_swin_tiny_patch4_window7_224_jpg_torchacc.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/swint/imagenet_swin_tiny_patch4_window7_224_jpg_torchacc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/vit/vit_base_patch16_224_b64x64_300e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/vit/vit_base_patch16_224_b64x64_300e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/imagenet/efficientformer/efficientformer_l1.py` & `pai-easycv-0.9.0/easycv/configs/classification/imagenet/efficientformer/efficientformer_l1.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/cifar10/r50_b128_300e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/cifar10/r50_b128_300e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/configs/classification/cifar10/swintiny_b64_5e_jpg.py` & `pai-easycv-0.9.0/easycv/configs/classification/cifar10/swintiny_b64_5e_jpg.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/classifier.py` & `pai-easycv-0.9.0/easycv/predictors/classifier.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/ocr.py` & `pai-easycv-0.9.0/easycv/predictors/ocr.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/face_keypoints_predictor.py` & `pai-easycv-0.9.0/easycv/predictors/face_keypoints_predictor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/feature_extractor.py` & `pai-easycv-0.9.0/easycv/predictors/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/__init__.py` & `pai-easycv-0.9.0/easycv/predictors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,9 @@
                                 TorchFeatureExtractor)
 from .hand_keypoints_predictor import HandKeypointsPredictor
 from .ocr import (OCRClsPredictor, OCRDetPredictor, OCRPredictor,
                   OCRRecPredictor)
 from .pose_predictor import (TorchPoseTopDownPredictor,
                              TorchPoseTopDownPredictorWithDetector)
 from .segmentation import Mask2formerPredictor, SegmentationPredictor
+from .video_classifier import VideoClassificationPredictor
 from .wholebody_keypoints_predictor import WholeBodyKeypointsPredictor
```

### Comparing `pai-easycv-0.8.0/easycv/predictors/interface.py` & `pai-easycv-0.9.0/easycv/predictors/interface.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/detector.py` & `pai-easycv-0.9.0/easycv/predictors/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,14 @@
             font_size=18,
             thickness=2,
             font_scale=0.0,
             show=show,
             out_file=out_file)
 
 
-@deprecated(reason='Please use DetectionPredictor.')
-@PREDICTORS.register_module()
-class DetrPredictor(DetectionPredictor):
-    """"""
-
-
 class _JitProcessorWrapper:
 
     def __init__(self, processor, device) -> None:
         self.processor = processor
         self.device = device
 
     def __call__(self, results):
```

### Comparing `pai-easycv-0.8.0/easycv/predictors/segmentation.py` & `pai-easycv-0.9.0/easycv/predictors/segmentation.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/wholebody_keypoints_predictor.py` & `pai-easycv-0.9.0/easycv/predictors/wholebody_keypoints_predictor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/hand_keypoints_predictor.py` & `pai-easycv-0.9.0/easycv/predictors/hand_keypoints_predictor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/pose_predictor.py` & `pai-easycv-0.9.0/easycv/predictors/pose_predictor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/base.py` & `pai-easycv-0.9.0/easycv/predictors/base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/predictors/bevformer_predictor.py` & `pai-easycv-0.9.0/easycv/predictors/bevformer_predictor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/runner/ev_runner.py` & `pai-easycv-0.9.0/easycv/runner/ev_runner.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/framework/errors.py` & `pai-easycv-0.9.0/easycv/framework/errors.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/eval_hook.py` & `pai-easycv-0.9.0/easycv/hooks/eval_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/show_time_hook.py` & `pai-easycv-0.9.0/easycv/hooks/show_time_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/oss_sync_hook.py` & `pai-easycv-0.9.0/easycv/hooks/oss_sync_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/yolox_lr_hook.py` & `pai-easycv-0.9.0/easycv/hooks/yolox_lr_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/__init__.py` & `pai-easycv-0.9.0/easycv/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/dino_hook.py` & `pai-easycv-0.9.0/easycv/hooks/dino_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/collate_hook.py` & `pai-easycv-0.9.0/easycv/hooks/collate_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/logger.py` & `pai-easycv-0.9.0/easycv/hooks/logger.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/yolox_mode_switch_hook.py` & `pai-easycv-0.9.0/easycv/hooks/yolox_mode_switch_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/export_hook.py` & `pai-easycv-0.9.0/easycv/hooks/export_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/swav_hook.py` & `pai-easycv-0.9.0/easycv/hooks/swav_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/sync_norm_hook.py` & `pai-easycv-0.9.0/easycv/hooks/sync_norm_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/throughput_hook.py` & `pai-easycv-0.9.0/easycv/hooks/throughput_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/wandb.py` & `pai-easycv-0.9.0/easycv/hooks/wandb.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/best_ckpt_saver_hook.py` & `pai-easycv-0.9.0/easycv/hooks/best_ckpt_saver_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/extractor.py` & `pai-easycv-0.9.0/easycv/hooks/extractor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/sync_random_size_hook.py` & `pai-easycv-0.9.0/easycv/hooks/sync_random_size_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/optimizer_hook.py` & `pai-easycv-0.9.0/easycv/hooks/optimizer_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/tensorboard.py` & `pai-easycv-0.9.0/easycv/hooks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/ema_hook.py` & `pai-easycv-0.9.0/easycv/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/lr_update_hook.py` & `pai-easycv-0.9.0/easycv/hooks/lr_update_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/hooks/byol_hook.py` & `pai-easycv-0.9.0/easycv/hooks/byol_hook.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/file/image.py` & `pai-easycv-0.9.0/easycv/file/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 import io
-import logging
-import time
 
 import cv2
 import numpy as np
 from cv2 import IMREAD_COLOR
 from PIL import Image
 
 from easycv import file
-from easycv.framework.errors import IOError, KeyError, ValueError
-from easycv.utils.constant import MAX_READ_IMAGE_TRY_TIMES
-from .utils import is_oss_path, is_url_path
+from easycv.framework.errors import KeyError, ValueError
+from .utils import is_url_path
 
 try:
     from turbojpeg import TurboJPEG, TJCS_RGB, TJPF_BGR
     turbo_jpeg = TurboJPEG()
     turbo_jpeg_mode = {'RGB': TJCS_RGB, 'BGR': TJPF_BGR}
 except:
     turbo_jpeg = None
@@ -77,28 +74,23 @@
         img = load_image_with_cv2(fp, mode=mode, dtype=dtype)
     else:
         raise KeyError(
             'Only support backend in ["pillow", "turbojpeg", "cv2"]')
     return img
 
 
-def load_image(img_path,
-               mode='BGR',
-               dtype=np.uint8,
-               backend='pillow',
-               max_try_times=MAX_READ_IMAGE_TRY_TIMES):
+def load_image(img_path, mode='BGR', dtype=np.uint8, backend='pillow'):
     """Load image file, return np.ndarray.
 
     Args:
         img_path (str): Image file path.
         mode (str): Order of channel, candidates are `bgr` and `rgb`.
         dtype : Output data type.
         backend (str): The image decoding backend type. Options are `cv2`, `pillow`, `turbojpeg`.
     """
-    # TODO: functions of multi tries should be in the `io.open`
     img = None
     if is_url_path(img_path):
         from mmcv.fileio.file_client import HTTPBackend
         client = HTTPBackend()
         img_bytes = client.get(img_path)
         img = _load_image(img_bytes, mode=mode, dtype=dtype, backend=backend)
     else:
```

### Comparing `pai-easycv-0.8.0/easycv/file/utils.py` & `pai-easycv-0.9.0/easycv/file/utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/file/file_io.py` & `pai-easycv-0.9.0/easycv/file/file_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,25 @@
     """
     IO module to support both local and oss io.
     If access oss file, you need to authorize OSS, please refer to `IO.access_oss`.
     """
 
     __name__ = 'IO'
 
-    def __init__(self, max_retry=10):
+    def __init__(self, max_retry=10, retry_wait=0.1, max_retry_wait=30):
 
         super(IO, self).__init__()
 
         self.oss_pattern = re.compile(r'oss://([^/]+)/(.+)')
         self.buckets_map = {}
         self.auth = None
         self.oss_config = None
         self.max_retry = max_retry
+        self.retry_wait = retry_wait
+        self.max_retry_wait = max_retry_wait
 
         if self._is_oss_env_prepared():
             self.access_oss(
                 ak_id=os.environ.get('OSS_ACCESS_KEY_ID'),
                 ak_secret=os.environ.get('OSS_ACCESS_KEY_SECRET'),
                 hosts=[
                     i.strip()
@@ -169,14 +171,16 @@
     def _read_oss(self, full_path, mode):
         assert mode in ['r', 'rb']
         path_exists = self.exists(full_path)
         if not path_exists:
             raise FileNotFoundError(full_path)
         bucket, path = self._get_bucket_obj_and_path(full_path)
         num_retry = 0
+        retry_wait = self.retry_wait
+
         data = None
         while num_retry < self.max_retry:
             try:
                 obj = bucket.get_object(path)
                 # auto cache large files to avoid memory issues
                 if obj.content_length > 200 * 1024**2:  # 200M
                     with tqdm(
@@ -191,17 +195,19 @@
                         data = obj.read()
                 else:
                     data = obj.read()
                 break
             except Exception as e:
                 num_retry += 1
                 logging.warning(
-                    f'read exception occur, sleep 3s to retry num_retry/max_retry {num_retry}/{self.max_retry}\n {e}'
+                    f'read exception occur, sleep {retry_wait}s to retry num_retry/max_retry {num_retry}/{self.max_retry}\n {e}'
                 )
-                time.sleep(3)
+                if retry_wait > 0:
+                    time.sleep(retry_wait)
+                    retry_wait = min(retry_wait * 2, self.max_retry_wait)
 
         if data is None:
             raise IOError('Read file error: %s!' % full_path)
 
         if mode == 'rb':
             return NullContextWrapper(BytesIO(data))
         else:
```

### Comparing `pai-easycv-0.8.0/easycv/file/base.py` & `pai-easycv-0.9.0/easycv/file/base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/toolkit/prune/prune_utils.py` & `pai-easycv-0.9.0/easycv/toolkit/prune/prune_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/toolkit/torchacc/convert_ops.py` & `pai-easycv-0.9.0/easycv/toolkit/torchacc/convert_ops.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/toolkit/torchacc/initilization.py` & `pai-easycv-0.9.0/easycv/toolkit/torchacc/initilization.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/toolkit/blade/trt_plugin_utils.py` & `pai-easycv-0.9.0/easycv/toolkit/blade/trt_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/toolkit/blade/cv_blade_utils.py` & `pai-easycv-0.9.0/easycv/toolkit/blade/cv_blade_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/toolkit/quantize/quantize_utils.py` & `pai-easycv-0.9.0/easycv/toolkit/quantize/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/apis/test.py` & `pai-easycv-0.9.0/easycv/apis/test.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/apis/train.py` & `pai-easycv-0.9.0/easycv/apis/train.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/apis/export.py` & `pai-easycv-0.9.0/easycv/apis/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,15 @@
         export_cfg = dict(export_neck=False)
     export_neck = export_cfg.get('export_neck', False)
 
     tbackbone = replace_syncbn(cfg.model.backbone)
 
     model_config = dict(
         type='Classification',
+        pretrained=False,  # avoid loading default pretrained backbone model
         backbone=tbackbone,
     )
 
     if export_neck and hasattr(cfg.model, 'neck'):
         cfg.model.neck.export = True
         cfg.model.neck.with_avg_pool = True
         model_config['neck'] = cfg.model.neck
@@ -422,14 +423,15 @@
         export_cfg = cfg.export
     else:
         export_cfg = dict(export_neck=False)
     export_neck = export_cfg.get('export_neck', False)
 
     model_config = dict(
         type='Classification',
+        pretrained=False,  # avoid loading default pretrained backbone model
         backbone=replace_syncbn(cfg.model.backbone),
         head=dict(
             type='ClsHead',
             with_avg_pool=True,
             in_channels=2048,
             num_classes=1000,
         ),
@@ -477,14 +479,15 @@
         export_cfg = cfg.export
     else:
         export_cfg = dict(export_neck=False)
     export_neck = export_cfg.get('export_neck', False)
 
     model_config = dict(
         type='Classification',
+        pretrained=False,  # avoid loading default pretrained backbone model
         backbone=replace_syncbn(cfg.model.backbone),
         head=dict(
             type='ClsHead',
             with_avg_pool=True,
             in_channels=2048,
             num_classes=1000,
         ),
```

### Comparing `pai-easycv-0.8.0/easycv/apis/train_misc.py` & `pai-easycv-0.9.0/easycv/apis/train_misc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/u2sod/u2net_models.py` & `pai-easycv-0.9.0/easycv/thirdparty/u2sod/u2net_models.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/u2sod/u2net_transform.py` & `pai-easycv-0.9.0/easycv/thirdparty/u2sod/u2net_transform.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/u2sod/sodpredictor.py` & `pai-easycv-0.9.0/easycv/thirdparty/u2sod/sodpredictor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/__init__.py` & `pai-easycv-0.9.0/easycv/thirdparty/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/face_align.py` & `pai-easycv-0.9.0/easycv/thirdparty/face_align.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/mtcnn/get_nets.py` & `pai-easycv-0.9.0/easycv/thirdparty/mtcnn/get_nets.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/mtcnn/utils.py` & `pai-easycv-0.9.0/easycv/thirdparty/mtcnn/utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/mtcnn/detector.py` & `pai-easycv-0.9.0/easycv/thirdparty/mtcnn/detector.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/setup.py` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/setup.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/test.py` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/test.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/functions/ms_deform_attn_func.py` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/functions/ms_deform_attn_func.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/functions/__init__.py` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/modules/__init__.py` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/modules/ms_deform_attn.py` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/modules/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.cpp` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.cpp`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.h` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.h`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/vision.cpp` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/vision.cpp`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/ms_deform_attn.h` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/ms_deform_attn.h`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.h` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.h`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.cu` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.cu`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_im2col_cuda.cuh` & `pai-easycv-0.9.0/easycv/thirdparty/deformable_attention/src/cuda/ms_deform_im2col_cuda.cuh`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/resource/simhei.ttf` & `pai-easycv-0.9.0/easycv/resource/simhei.ttf`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/builder.py` & `pai-easycv-0.9.0/easycv/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/selfsup/pipelines/transforms.py` & `pai-easycv-0.9.0/easycv/datasets/selfsup/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/selfsup/data_sources/imagenet_feature.py` & `pai-easycv-0.9.0/easycv/datasets/selfsup/data_sources/imagenet_feature.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/selfsup/data_sources/image_list.py` & `pai-easycv-0.9.0/easycv/datasets/selfsup/data_sources/image_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import time
 
 from PIL import Image, ImageFile
 
 from easycv.datasets.registry import DATASOURCES
 from easycv.file import io
+from easycv.file.image import load_image
 from easycv.framework.errors import ValueError
 
 
 @DATASOURCES.register_module
 class SSLSourceImageList(object):
     """ datasource for classification
 
@@ -62,27 +63,14 @@
 
         return fns
 
     def __len__(self):
         return len(self.fns)
 
     def __getitem__(self, idx):
-        img = None
-        try_idx = 0
-
-        while img is None and try_idx < self.max_try:
-            try:
-                img = Image.open(io.open(self.fns[idx], 'rb'))
-                if img.mode != 'RGB':
-                    img = img.convert('RGB')
-            except:
-                # frequent access to oss will cause error, sleep can aviod it
-                time.sleep(1)
-                logging.warning('Try read file fault, %s' % self.fns[idx])
-                img = None
-
-            try_idx += 1
-
+        img = load_image(self.fns[idx], mode='RGB')
         if img is None:
             return self[(idx + 1) % len(self.fns)]
 
+        img = Image.fromarray(img)
+
         return {'img': img}
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/dali_tfrecord_imagenet.py` & `pai-easycv-0.9.0/easycv/datasets/shared/dali_tfrecord_imagenet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/pipelines/third_transforms_wrapper.py` & `pai-easycv-0.9.0/easycv/datasets/shared/pipelines/third_transforms_wrapper.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/pipelines/dali_transforms.py` & `pai-easycv-0.9.0/easycv/datasets/shared/pipelines/dali_transforms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/pipelines/format.py` & `pai-easycv-0.9.0/easycv/datasets/shared/pipelines/format.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/pipelines/transforms.py` & `pai-easycv-0.9.0/easycv/datasets/shared/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/dali_tfrecord_multi_view.py` & `pai-easycv-0.9.0/easycv/datasets/shared/dali_tfrecord_multi_view.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/__init__.py` & `pai-easycv-0.9.0/easycv/datasets/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/odps_reader.py` & `pai-easycv-0.9.0/easycv/datasets/shared/odps_reader.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/raw.py` & `pai-easycv-0.9.0/easycv/datasets/shared/raw.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/dataset_wrappers.py` & `pai-easycv-0.9.0/easycv/datasets/shared/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/data_sources/concat.py` & `pai-easycv-0.9.0/easycv/datasets/shared/data_sources/concat.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/data_sources/image_npy.py` & `pai-easycv-0.9.0/easycv/datasets/shared/data_sources/image_npy.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/base.py` & `pai-easycv-0.9.0/easycv/datasets/shared/base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/shared/multi_view.py` & `pai-easycv-0.9.0/easycv/datasets/shared/multi_view.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/face/pipelines/face_keypoint_transform.py` & `pai-easycv-0.9.0/easycv/datasets/face/pipelines/face_keypoint_transform.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/face/face_keypoint_dataset.py` & `pai-easycv-0.9.0/easycv/datasets/face/face_keypoint_dataset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/face/data_sources/face_keypoint_source.py` & `pai-easycv-0.9.0/easycv/datasets/face/data_sources/face_keypoint_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import cv2
 import numpy as np
 import torch
 
 from easycv.datasets.face.pipelines.face_keypoint_transform import (
     FaceKeypointNorm, FaceKeypointRandomAugmentation, normal)
 from easycv.datasets.registry import DATASOURCES
-from easycv.datasets.shared.base import BaseDataset
+from easycv.file.image import load_image
 
 FACE_KEYPOINT_DATASET_INFO = dict(
     real_list_file_dir='real_face_list.txt',
     data_info_dir='infos/merge/',
     data_image_dir='images/merge/',
     data_overlay_dir='images/overlay/',
 )
@@ -152,15 +152,16 @@
                 'target_pose_mask':
                 torch.tensor(pose_mask.astype(np.float32))
             })
 
     def __getitem__(self, index):
         img_path, points, points_mask, pose, pose_mask = copy.deepcopy(
             self.points_and_pose_datas[index])
-        image = cv2.imread(img_path)
+
+        image = load_image(img_path, backend='cv2')
 
         return {
             'img': image,
             'target_point': points,
             'target_point_mask': points_mask,
             'target_pose': pose,
             'target_pose_mask': pose_mask,
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/__init__.py` & `pai-easycv-0.9.0/easycv/datasets/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 # isort:skip_file
 from easycv.utils.import_utils import check_numpy
 check_numpy()
 from . import (classification, detection, detection3d, face, ocr, pose,
-               segmentation, selfsup, shared)
+               segmentation, selfsup, shared, video_recognition)
 from .builder import (build_dali_dataset, build_dataset, build_datasource,
                       build_sampler)
 from .loader import (DistributedGivenIterationSampler, DistributedGroupSampler,
                      DistributedMPSampler, DistributedSampler, GroupSampler,
                      RASampler, build_dataloader)
 from .registry import DATASETS, DATASOURCES, PIPELINES, SAMPLERS
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/segmentation/pipelines/transforms.py` & `pai-easycv-0.9.0/easycv/datasets/segmentation/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/segmentation/raw.py` & `pai-easycv-0.9.0/easycv/datasets/segmentation/raw.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/coco_stuff.py` & `pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/coco_stuff.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,15 @@
             gt_semantic_seg[gt_semantic_seg == 0] = 255
             gt_semantic_seg = gt_semantic_seg - 1
             gt_semantic_seg[gt_semantic_seg == 254] = 255
 
         return {'gt_semantic_seg': gt_semantic_seg}
 
     def load_image(self, img_path):
-        img = _load_img(img_path, mode='RGB')
-        img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
+        img = _load_img(img_path, mode='BGR')
         result = {
             'img': img.astype(np.float32),
             'img_shape': img.shape,  # h, w, c
             'ori_shape': img.shape,
         }
         return result
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/raw.py` & `pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/raw.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/base.py` & `pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 from easycv.datasets.registry import DATASOURCES
 from easycv.file.image import load_image as _load_img
 from easycv.framework.errors import NotImplementedError, ValueError
 
 
 def load_image(img_path):
-    img = _load_img(img_path, mode='RGB')
-    img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
+    img = _load_img(img_path, mode='BGR')
     result = {
         'img': img.astype(np.float32),
         'img_shape': img.shape,  # h, w, c
         'ori_shape': img.shape,
     }
     return result
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/voc.py` & `pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/voc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/segmentation/data_sources/coco.py` & `pai-easycv-0.9.0/easycv/datasets/segmentation/data_sources/coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/hand_coco_wholebody_dataset.py` & `pai-easycv-0.9.0/easycv/datasets/pose/hand_coco_wholebody_dataset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/wholebody_topdown_coco_dataset.py` & `pai-easycv-0.9.0/easycv/datasets/pose/wholebody_topdown_coco_dataset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/pipelines/__init__.py` & `pai-easycv-0.9.0/easycv/datasets/pose/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/pipelines/transforms.py` & `pai-easycv-0.9.0/easycv/datasets/pose/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/top_down.py` & `pai-easycv-0.9.0/easycv/datasets/pose/top_down.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/data_sources/hand/coco_hand.py` & `pai-easycv-0.9.0/easycv/datasets/pose/data_sources/hand/coco_hand.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/data_sources/wholebody/wholebody_coco_source.py` & `pai-easycv-0.9.0/easycv/datasets/pose/data_sources/wholebody/wholebody_coco_source.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/data_sources/__init__.py` & `pai-easycv-0.9.0/easycv/datasets/pose/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/data_sources/mpii.py` & `pai-easycv-0.9.0/easycv/datasets/pose/data_sources/mpii.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/data_sources/top_down.py` & `pai-easycv-0.9.0/easycv/datasets/pose/data_sources/top_down.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/data_sources/crowd_pose.py` & `pai-easycv-0.9.0/easycv/datasets/pose/data_sources/crowd_pose.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/data_sources/oc_human.py` & `pai-easycv-0.9.0/easycv/datasets/pose/data_sources/oc_human.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/pose/data_sources/coco.py` & `pai-easycv-0.9.0/easycv/datasets/pose/data_sources/coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/mix.py` & `pai-easycv-0.9.0/easycv/datasets/detection/mix.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/pipelines/__init__.py` & `pai-easycv-0.9.0/easycv/datasets/detection/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/pipelines/mm_transforms.py` & `pai-easycv-0.9.0/easycv/datasets/detection/pipelines/mm_transforms.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/raw.py` & `pai-easycv-0.9.0/easycv/datasets/detection/raw.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/fruit.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/fruit.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/pet.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/pet.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/pai_format.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/pai_format.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/artaxor.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/artaxor.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/wider_person.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/wider_person.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/coco_panoptic.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/__init__.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/utils.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/raw.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/raw.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/african_wildlife.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/african_wildlife.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/coco_livs.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/coco_livs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 import os
 from pathlib import Path
 
 from torchvision.datasets.utils import download_and_extract_archive
 from xtcocotools.coco import COCO
 
 from easycv.datasets.detection.data_sources.coco import DetSourceCoco
-from easycv.datasets.registry import DATASOURCES, PIPELINES
-from easycv.datasets.shared.pipelines import Compose
-from easycv.framework.errors import TypeError
-from easycv.utils.registry import build_from_cfg
+from easycv.datasets.registry import DATASOURCES
 
 
 @DATASOURCES.register_module
 class DetSourceLvis(DetSourceCoco):
     """
     lvis data source
     """
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/crowd_human.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/crowd_human.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/objects365.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/objects365.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/base.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/wider_face.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/wider_face.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/voc.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/voc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection/data_sources/coco.py` & `pai-easycv-0.9.0/easycv/datasets/detection/data_sources/coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/ocr_det_dataset.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/ocr_det_dataset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/ocr_cls_dataset.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/ocr_cls_dataset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/pipelines/rec_transform.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/pipelines/rec_transform.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/pipelines/det_transform.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/pipelines/det_transform.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/pipelines/label_ops.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/pipelines/label_ops.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/ocr_raw_dataset.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/ocr_raw_dataset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/data_sources/ocr_cls_datasource.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/data_sources/ocr_cls_datasource.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/data_sources/ocr_det_datasource.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/data_sources/ocr_det_datasource.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/data_sources/ocr_rec_datasource.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/data_sources/ocr_rec_datasource.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/ocr/ocr_rec_dataset.py` & `pai-easycv-0.9.0/easycv/datasets/ocr/ocr_rec_dataset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/transforms_3d.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/transforms_3d.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/__init__.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/loading.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/test_aug.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/test_aug.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/format.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/format.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/pipelines/functional.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/pipelines/functional.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/utils.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/nuscenes_dataset.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/nuscenes_dataset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/data_sources/nuscenes.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/data_sources/nuscenes.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/detection3d/data_sources/base.py` & `pai-easycv-0.9.0/easycv/datasets/detection3d/data_sources/base.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/odps.py` & `pai-easycv-0.9.0/easycv/datasets/classification/odps.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/pipelines/auto_augment.py` & `pai-easycv-0.9.0/easycv/datasets/classification/pipelines/auto_augment.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/pipelines/transform.py` & `pai-easycv-0.9.0/easycv/datasets/classification/pipelines/transform.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/raw.py` & `pai-easycv-0.9.0/easycv/datasets/classification/raw.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/imagenet_tfrecord.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/imagenet_tfrecord.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/fashiongen_h5.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/fashiongen_h5.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/cub.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/cub.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/imagenet.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/imagenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 
 import os
 
+from PIL import Image
+
 from easycv.datasets.registry import DATASOURCES
 from easycv.file.image import load_image
 
 
 def generate_label_map(label_path):
     label_txt = open(label_path).readlines()
     assert len(label_txt) > 1, f'{label_path} is None'
@@ -55,15 +57,16 @@
         self.txt_path = get_images_list(os.path.join(root, self.split))
         self.label_json = generate_label_map(
             os.path.join(root, 'meta/label_name.txt'))
 
     def read_data(self, image_path):
         img_path = os.path.join(self.root, image_path.strip())
         assert os.path.exists(img_path), f'{img_path} is not exists'
-        img = load_image(img_path)
+        img = load_image(img_path, mode='RGB')
+        img = Image.fromarray(img)
         label_key = image_path.split('/')[1]
         assert label_key in self.label_json, f'{label_key} label is not exists'
         label = self.label_json[label_key]
         return {'img': img, 'gt_labels': int(label[0].strip())}
 
     def __len__(self):
         return len(self.txt_path)
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/mnist.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/mnist.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/cifar.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/cifar.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/__init__.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/flower.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/flower.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/utils.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/class_list.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/class_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 import logging
 import os
 import random
-import time
 
 from PIL import Image, ImageFile
 
 from easycv.datasets.registry import DATASOURCES
 from easycv.file import io
+from easycv.file.image import load_image
 from easycv.utils.dist_utils import dist_zero_exec
 from .utils import split_listfile_byrank
 
 
 @DATASOURCES.register_module
 class ClsSourceImageListByClass(object):
     """
@@ -90,31 +90,17 @@
                              1) * image_list
 
         sample_list = random.sample(image_list, self.m_per_class)
         return_img = []
         return_label = []
 
         for path in sample_list:
-            img = None
-            try_idx = 0
-            while not img and try_idx < self.max_try:
-                try:
-                    img = Image.open(
-                        io.open(os.path.join(self.root, path), 'rb'))
-                    if img.mode != 'RGB':
-                        img = img.convert('RGB')
-                except:
-                    logging.warning('Try read file fault, %s' %
-                                    os.path.join(self.root, path))
-                    time.sleep(1)
-                    img = None
-
-                try_idx += 1
-
+            img = load_image(os.path.join(self.root, path), mode='RGB')
             if img is None:
                 return self[idx + 1]
 
+            img = Image.fromarray(img)
             return_img.append(img)
             return_label.append(label)
 
         result_dict = {'img': return_img, 'gt_labels': return_label}
         return result_dict
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/image_list.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/image_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 import json
 import logging
 import os
-import time
 
 from PIL import Image, ImageFile
 
 from easycv.datasets.registry import DATASOURCES
 from easycv.file import io
+from easycv.file.image import load_image
 from easycv.framework.errors import TypeError
 from easycv.utils.dist_utils import dist_zero_exec
 from .utils import split_listfile_byrank
 
 
 @DATASOURCES.register_module
 class ClsSourceImageList(object):
@@ -101,33 +101,19 @@
 
         return fns, labels
 
     def __len__(self):
         return len(self.fns)
 
     def __getitem__(self, idx):
-        img = None
-        try_idx = 0
-
-        while img is None and try_idx < self.max_try:
-            try:
-                img = Image.open(io.open(self.fns[idx], 'rb'))
-                if img.mode != 'RGB':
-                    img = img.convert('RGB')
-            except:
-                # frequent access to oss will cause error, sleep can aviod it
-                time.sleep(1)
-                logging.warning('Try read file fault, %s' % self.fns[idx])
-                img = None
-
-            try_idx += 1
-
+        img = load_image(self.fns[idx], mode='RGB')
         if img is None:
             return self[idx + 1]
 
+        img = Image.fromarray(img)
         label = self.labels[idx]
 
         result_dict = {'img': img, 'gt_labels': label}
         return result_dict
 
 
 @DATASOURCES.register_module
```

### Comparing `pai-easycv-0.8.0/easycv/datasets/classification/data_sources/caltech.py` & `pai-easycv-0.9.0/easycv/datasets/classification/data_sources/caltech.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/loader/sampler.py` & `pai-easycv-0.9.0/easycv/datasets/loader/sampler.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/loader/build_loader.py` & `pai-easycv-0.9.0/easycv/datasets/loader/build_loader.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/loader/loader_wrapper.py` & `pai-easycv-0.9.0/easycv/datasets/loader/loader_wrapper.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/loader/collate.py` & `pai-easycv-0.9.0/easycv/datasets/loader/collate.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/utils/tfrecord_util.py` & `pai-easycv-0.9.0/easycv/datasets/utils/tfrecord_util.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/utils/transform_util.py` & `pai-easycv-0.9.0/easycv/datasets/utils/transform_util.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/utils/download_data/download_voc.py` & `pai-easycv-0.9.0/easycv/datasets/utils/download_data/download_voc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/utils/download_data/download_coco.py` & `pai-easycv-0.9.0/easycv/datasets/utils/download_data/download_coco.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/datasets/utils/download_data/commont.py` & `pai-easycv-0.9.0/easycv/datasets/utils/download_data/commont.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/quantize.py` & `pai-easycv-0.9.0/easycv/tools/quantize.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/analyze_tools/measure_inference_time.py` & `pai-easycv-0.9.0/easycv/tools/analyze_tools/measure_inference_time.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/analyze_tools/count_parameters.py` & `pai-easycv-0.9.0/easycv/tools/analyze_tools/count_parameters.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/analyze_tools/count_flops.py` & `pai-easycv-0.9.0/easycv/tools/analyze_tools/count_flops.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/prune.py` & `pai-easycv-0.9.0/easycv/tools/prune.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/eval.py` & `pai-easycv-0.9.0/easycv/tools/eval.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/prepare_data/create_voc_data_files.py` & `pai-easycv-0.9.0/easycv/tools/prepare_data/create_voc_data_files.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/prepare_data/prepare_nuscenes.py` & `pai-easycv-0.9.0/easycv/tools/prepare_data/prepare_nuscenes.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/prepare_data/coco_stuff164k.py` & `pai-easycv-0.9.0/easycv/tools/prepare_data/coco_stuff164k.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/prepare_data/create_voc_low_shot_challenge_samples.py` & `pai-easycv-0.9.0/easycv/tools/prepare_data/create_voc_low_shot_challenge_samples.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/prepare_data/convert_subset.py` & `pai-easycv-0.9.0/easycv/tools/prepare_data/convert_subset.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/commands_wrapper.py` & `pai-easycv-0.9.0/easycv/tools/commands_wrapper.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/train.py` & `pai-easycv-0.9.0/easycv/tools/train.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/predict.py` & `pai-easycv-0.9.0/easycv/tools/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,46 +212,76 @@
     def destroy(self):
         if not self.input_empty and self.all_data_failed:
             raise RuntimeError(
                 'failed to predict all the input data, please see exception throwed above in the log'
             )
 
 
+def create_yolox_predictor_kwargs(model_dir):
+    jit_models = glob.glob('%s/**/*.jit' % model_dir, recursive=True)
+    raw_models = glob.glob('%s/**/*.pt' % model_dir, recursive=True)
+    if len(jit_models) > 0:
+        assert len(
+            jit_models
+        ) == 1, f'more than one jit script model files is found in {model_dir}'
+        config_path = jit_models[0] + '.config.json'
+        if not os.path.exists(config_path):
+            raise ValueError(
+                f'Not find config json file {config_path} for inference with jit script model'
+            )
+        return {'model_path': jit_models[0], 'config_file': config_path}
+    else:
+        assert len(raw_models) > 0, f'export model not found in {model_dir}'
+        assert len(raw_models
+                   ) == 1, f'more than one model files is found in {model_dir}'
+        return {'model_path': raw_models[0]}
+
+
+def create_default_predictor_kwargs(model_dir):
+    model_path = glob.glob('%s/**/*.pt*' % model_dir, recursive=True)
+    assert len(model_path) > 0, f'model not found in {model_dir}'
+    assert len(
+        model_path) == 1, f'more than one model file is found {model_path}'
+    model_path = model_path[0]
+    logging.info(f'model found: {model_path}')
+
+    config_path = glob.glob('%s/**/*.py' % model_dir, recursive=True)
+    if len(config_path) == 0:
+        config_path = None
+    else:
+        assert len(config_path
+                   ) == 1, f'more than one config file is found {config_path}'
+        config_path = config_path[0]
+        logging.info(f'config found: {config_path}')
+    if config_path:
+        return {'model_path': model_path, 'config_file': config_path}
+    else:
+        return {'model_path': model_path}
+
+
+def create_predictor_kwargs(model_type, model_dir):
+    if model_type == 'YoloXPredictor':
+        return create_yolox_predictor_kwargs(model_dir)
+    else:
+        return create_default_predictor_kwargs(model_dir)
+
+
 def init_predictor(args):
     model_type = args.model_type
     model_path = args.model_path
     batch_size = args.batch_size
     from easycv.predictors.builder import build_predictor
 
     ori_model_path = model_path
-    if not ori_model_path.endswith('pth') and not ori_model_path.endswith(
-            'pt'):
-        model_path = glob.glob('%s/**/*.pt*' % ori_model_path, recursive=True)
-        assert len(model_path) > 0, f'model not found in {ori_model_path}'
-        assert len(
-            model_path) == 1, f'more than one model file is found {model_path}'
-        model_path = model_path[0]
-        logging.info(f'model found: {model_path}')
-
-        config_path = glob.glob('%s/**/*.py' % ori_model_path, recursive=True)
-        if len(config_path) == 0:
-            config_path = None
-        else:
-            assert len(
-                config_path
-            ) == 1, f'more than one config file is found {config_path}'
-            config_path = config_path[0]
-            logging.info(f'config found: {config_path}')
+    if os.path.isdir(ori_model_path):
+        predictor_kwargs = create_predictor_kwargs(model_type, ori_model_path)
     else:
-        model_path = ori_model_path
-        config_path = None
+        predictor_kwargs = {'model_path': ori_model_path}
 
-    predictor_cfg = dict(type=model_type, model_path=model_path)
-    if config_path:
-        predictor_cfg['config_file'] = config_path
+    predictor_cfg = dict(type=model_type, **predictor_kwargs)
     if args.model_config != '':
         predictor_cfg['model_config'] = args.model_config
     predictor = build_predictor(predictor_cfg)
     return predictor
 
 
 def replace_oss_with_local_path(ori_file, dst_file, bucket_prefix,
```

### Comparing `pai-easycv-0.8.0/easycv/tools/launch.py` & `pai-easycv-0.9.0/easycv/tools/launch.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/tools/export.py` & `pai-easycv-0.9.0/easycv/tools/export.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/gather.py` & `pai-easycv-0.9.0/easycv/utils/gather.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/mmlab_utils.py` & `pai-easycv-0.9.0/easycv/utils/mmlab_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/metric_distance.py` & `pai-easycv-0.9.0/easycv/utils/metric_distance.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/alias_multinomial.py` & `pai-easycv-0.9.0/easycv/utils/alias_multinomial.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/py_util.py` & `pai-easycv-0.9.0/easycv/utils/py_util.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/parse_pipeline.py` & `pai-easycv-0.9.0/easycv/utils/parse_pipeline.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/collect.py` & `pai-easycv-0.9.0/easycv/utils/collect.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/util_mixins.py` & `pai-easycv-0.9.0/easycv/utils/util_mixins.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/eval_utils.py` & `pai-easycv-0.9.0/easycv/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/registry.py` & `pai-easycv-0.9.0/easycv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/preprocess_function.py` & `pai-easycv-0.9.0/easycv/utils/preprocess_function.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/import_utils.py` & `pai-easycv-0.9.0/easycv/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/dist_utils.py` & `pai-easycv-0.9.0/easycv/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/logger.py` & `pai-easycv-0.9.0/easycv/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/checkpoint.py` & `pai-easycv-0.9.0/easycv/utils/checkpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,39 +10,15 @@
 
 from easycv.file import io
 from easycv.file.utils import is_url_path
 from easycv.framework.errors import TypeError
 from easycv.utils.constant import CACHE_DIR
 
 
-def load_checkpoint(model,
-                    filename,
-                    map_location='cpu',
-                    strict=False,
-                    logger=None,
-                    revise_keys=[(r'^module\.', '')]):
-    """Load checkpoint from a file or URI.
-
-    Args:
-        model (Module): Module to load checkpoint.
-        filename (str): Accept local filepath, URL, ``torchvision://xxx``,
-            ``open-mmlab://xxx``. Please refer to ``docs/model_zoo.md`` for
-            details.
-        map_location (str): Same as :func:`torch.load`.
-        strict (bool): Whether to allow different params for the model and
-            checkpoint.
-        logger (:mod:`logging.Logger` or None): The logger for error message.
-        revise_keys (list): A list of customized keywords to modify the
-            state_dict in checkpoint. Each item is a (pattern, replacement)
-            pair of the regular expression operations. Default: strip
-            the prefix 'module.' by [(r'^module\\.', '')].
-
-    Returns:
-        dict or OrderedDict: The loaded checkpoint.
-    """
+def get_checkpoint(filename):
     if filename.startswith('oss://'):
         _, fname = os.path.split(filename)
         cache_file = os.path.join(CACHE_DIR, fname)
         if not os.path.exists(CACHE_DIR):
             os.makedirs(CACHE_DIR)
         if not os.path.exists(cache_file):
             logging.info(
@@ -63,15 +39,43 @@
             logging.info(
                 f'download checkpoint from {filename} to {cache_file}')
             download_url_to_file(filename, cache_file)
         if torch.distributed.is_available(
         ) and torch.distributed.is_initialized():
             torch.distributed.barrier()
         filename = cache_file
+    return filename
+
 
+def load_checkpoint(model,
+                    filename,
+                    map_location='cpu',
+                    strict=False,
+                    logger=None,
+                    revise_keys=[(r'^module\.', '')]):
+    """Load checkpoint from a file or URI.
+
+    Args:
+        model (Module): Module to load checkpoint.
+        filename (str): Accept local filepath, URL, ``torchvision://xxx``,
+            ``open-mmlab://xxx``. Please refer to ``docs/model_zoo.md`` for
+            details.
+        map_location (str): Same as :func:`torch.load`.
+        strict (bool): Whether to allow different params for the model and
+            checkpoint.
+        logger (:mod:`logging.Logger` or None): The logger for error message.
+        revise_keys (list): A list of customized keywords to modify the
+            state_dict in checkpoint. Each item is a (pattern, replacement)
+            pair of the regular expression operations. Default: strip
+            the prefix 'module.' by [(r'^module\\.', '')].
+
+    Returns:
+        dict or OrderedDict: The loaded checkpoint.
+    """
+    filename = get_checkpoint(filename)
     return mmcv_load_checkpoint(
         model,
         filename,
         map_location=map_location,
         strict=strict,
         logger=logger,
         revise_keys=revise_keys)
```

### Comparing `pai-easycv-0.8.0/easycv/utils/collect_env.py` & `pai-easycv-0.9.0/easycv/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/profiling.py` & `pai-easycv-0.9.0/easycv/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/json_utils.py` & `pai-easycv-0.9.0/easycv/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/setup_env.py` & `pai-easycv-0.9.0/easycv/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/test_util.py` & `pai-easycv-0.9.0/easycv/utils/test_util.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/config_tools.py` & `pai-easycv-0.9.0/easycv/utils/config_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import os.path as osp
 import platform
 import sys
 import tempfile
+import warnings
 from importlib import import_module
 
 from mmcv import Config, import_modules_from_strings
 
 import easycv
 from easycv.file import io
 from easycv.framework.errors import IOError, KeyError, ValueError
@@ -209,16 +210,16 @@
                                                     list) else [base_filename]
 
         cfg_dict_list = list()
         cfg_text_list = list()
         for f in base_filename:
             base_cfg_path = check_base_cfg_path(
                 f, ori_filename, easycv_root=easycv_root)
-            _cfg_dict, _cfg_text = mmcv_file2dict_base(base_cfg_path,
-                                                       first_order_params)
+            _cfg_dict, _cfg_text = mmcv_file2dict_base(
+                base_cfg_path, first_order_params, easycv_root=easycv_root)
             cfg_dict_list.append(_cfg_dict)
             cfg_text_list.append(_cfg_text)
 
         base_cfg_dict = dict()
         for c in cfg_dict_list:
             if len(base_cfg_dict.keys() & c.keys()) > 0:
                 raise KeyError('Duplicate key is not allowed among bases')
@@ -289,14 +290,19 @@
         hosts='oss-cn-zhangjiakou.aliyuncs.com',
         buckets=['your_bucket_2'])
     return cfg_dict
 
 
 def init_path(ori_filename):
     easycv_root = osp.dirname(easycv.__file__)  # easycv package root path
+    if not osp.exists(osp.join(easycv_root, 'configs')):
+        if osp.exists(osp.join(osp.dirname(easycv_root), 'configs')):
+            easycv_root = osp.dirname(easycv_root)
+        else:
+            raise ValueError('easycv root does not exist!')
     parse_ori_filename = ori_filename.split('/')
     if parse_ori_filename[0] == 'configs' or parse_ori_filename[
             0] == 'benchmarks':
         if osp.exists(osp.join(easycv_root, ori_filename)):
             ori_filename = osp.join(easycv_root, ori_filename)
 
     return ori_filename, easycv_root
@@ -565,8 +571,17 @@
     # edge models
     'YOLOX_EDGE': 'configs/config_templates/yolox_edge.py',
     'YOLOX_EDGE_ITAG': 'configs/config_templates/yolox_edge_itag.py',
 
     # pose
     'TOPDOWN_HRNET': 'configs/config_templates/topdown_hrnet_w48_udp.py',
     'TOPDOWN_LITEHRNET': 'configs/config_templates/topdown_litehrnet_30.py',
+
+    # video_classification
+    'X3D_XS': 'configs/video_recognition/x3d/x3d_xs.py',
+    'X3D_M': 'configs/video_recognition/x3d/x3d_m.py',
+    'X3D_L': 'configs/video_recognition/x3d/x3d_l.py',
+    'VIDEO_SWIN_T': 'configs/video_recognition/swin/video_swin_tiny.py',
+    'VIDEO_SWIN_S': 'configs/video_recognition/swin/video_swin_s.py',
+    'VIDEO_SWIN_B': 'configs/video_recognition/swin/video_swin_b.py',
+    'SWIN_BERT': 'configs/video_recognition/clipbert/clipbert_multilabel.py',
 }
```

### Comparing `pai-easycv-0.8.0/easycv/utils/flops_counter.py` & `pai-easycv-0.9.0/easycv/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/ms_utils.py` & `pai-easycv-0.9.0/easycv/utils/ms_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/user_config_params_utils.py` & `pai-easycv-0.9.0/easycv/utils/user_config_params_utils.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/easycv/utils/misc.py` & `pai-easycv-0.9.0/easycv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pai-easycv-0.8.0/pai_easycv.egg-info/SOURCES.txt` & `pai-easycv-0.9.0/pai_easycv.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw18_jpg.py
 easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw30_jpg.py
 easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw32_jpg.py
 easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw40_jpg.py
 easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw44_jpg.py
 easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw48_jpg.py
 easycv/configs/classification/imagenet/hrnet/imagenet_hrnetw64_jpg.py
+easycv/configs/classification/imagenet/inception/inceptionv3_b32x8_100e.py
 easycv/configs/classification/imagenet/resnet/imagenet_resnet101_jpg.py
 easycv/configs/classification/imagenet/resnet/imagenet_resnet152_jpg.py
 easycv/configs/classification/imagenet/resnet/imagenet_resnet50_jpg.py
 easycv/configs/classification/imagenet/resnet/imagenet_resnet50_tfrecord.py
 easycv/configs/classification/imagenet/resnet/resnet50_b32x8_100e_jpg.py
 easycv/configs/classification/imagenet/resnext/imagenet_resnext101-32x4d_jpg.py
 easycv/configs/classification/imagenet/resnext/imagenet_resnext101-32x8d_jpg.py
@@ -201,14 +202,15 @@
 easycv/configs/detection/yolox/yolox_nano_8xb16_300e_coco.py
 easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco.py
 easycv/configs/detection/yolox/yolox_s_8xb16_300e_coco_pai.py
 easycv/configs/detection/yolox/yolox_s_8xb16_300e_voc.py
 easycv/configs/detection/yolox/yolox_tiny_8xb16_300e_coco.py
 easycv/configs/detection/yolox/yolox_x_8xb8_300e_coco.py
 easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes.py
+easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes_blancehybrid.py
 easycv/configs/detection3d/bevformer/bevformer_base_r101_dcn_nuscenes_hybrid.py
 easycv/configs/detection3d/bevformer/bevformer_tiny_r50_nuscenes.py
 easycv/configs/detection3d/bevformer/bevformer_tiny_r50_nuscenes_fp16.py
 easycv/configs/edge_models/yolox_edge.py
 easycv/configs/edge_models/yolox_l.py
 easycv/configs/edge_models/yolox_m.py
 easycv/configs/edge_models/yolox_nano.py
@@ -241,24 +243,26 @@
 easycv/configs/ocr/recognition/rec_model_ta.py
 easycv/configs/ocr/recognition/rec_model_te.py
 easycv/configs/pose/hrnet_w48_coco_256x192_udp.py
 easycv/configs/pose/litehrnet_30_coco_384x288.py
 easycv/configs/pose/hand/hrnet_w18_coco_wholebody_hand_256x256_dark.py
 easycv/configs/pose/hand/litehrnet_30_coco_wholebody_hand_256x256.py
 easycv/configs/pose/wholebody/hrnet_w48_coco_wholebody_384x288_dark_plus.py
+easycv/configs/segmentation/fcn/fcn_r50-d8_512x512_8xb4_60e_voc12.py
 easycv/configs/segmentation/fcn/fcn_r50-d8_512x512_8xb4_60e_voc12aug.py
 easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e127_semantic.py
 easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_instance.py
 easycv/configs/segmentation/mask2former/mask2former_r50_8xb2_e50_panoptic.py
 easycv/configs/segmentation/segformer/segformer_b0_coco.py
 easycv/configs/segmentation/segformer/segformer_b1_coco.py
 easycv/configs/segmentation/segformer/segformer_b2_coco.py
 easycv/configs/segmentation/segformer/segformer_b3_coco.py
 easycv/configs/segmentation/segformer/segformer_b4_coco.py
 easycv/configs/segmentation/segformer/segformer_b5_coco.py
+easycv/configs/segmentation/upernet/upernet_r50_512x512_8xb4_60e_voc12.py
 easycv/configs/segmentation/upernet/upernet_r50_512x512_8xb4_60e_voc12aug.py
 easycv/configs/selfsup/byol/byol_rn50_8xb32_200e.py
 easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_jpg.py
 easycv/configs/selfsup/dino/dino_deit_small_p16_8xb32_100e_tfrecord.py
 easycv/configs/selfsup/fast_convmae/fast_convmae_vit_base_patch16_8xb64_50e.py
 easycv/configs/selfsup/mae/mae_vit_base_patch16_8xb64_1600e.py
 easycv/configs/selfsup/mae/mae_vit_base_patch16_8xb64_400e.py
@@ -272,14 +276,22 @@
 easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_jpg.py
 easycv/configs/selfsup/mocov2/mocov2_rn50_8xb32_200e_tfrecord.py
 easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_jpg.py
 easycv/configs/selfsup/simclr/simclr_rn50_8xb32_200e_tfrecord.py
 easycv/configs/selfsup/simclr/simclr_rn50_mocov2_neck_8xb32_200e_jpg.py
 easycv/configs/selfsup/swav/swav_genet_8xb32_200e_tfrecord.py
 easycv/configs/selfsup/swav/swav_rn50_8xb32_200e_tfrecord.py
+easycv/configs/video_recognition/clipbert/clipbert.py
+easycv/configs/video_recognition/clipbert/clipbert_multilabel.py
+easycv/configs/video_recognition/swin/video_swin_b.py
+easycv/configs/video_recognition/swin/video_swin_s.py
+easycv/configs/video_recognition/swin/video_swin_tiny.py
+easycv/configs/video_recognition/x3d/x3d_l.py
+easycv/configs/video_recognition/x3d/x3d_m.py
+easycv/configs/video_recognition/x3d/x3d_xs.py
 easycv/core/__init__.py
 easycv/core/standard_fields.py
 easycv/core/anchor/__init__.py
 easycv/core/anchor/builder.py
 easycv/core/anchor/point_generator.py
 easycv/core/bbox/__init__.py
 easycv/core/bbox/bbox_util.py
@@ -490,14 +502,23 @@
 easycv/datasets/utils/tfrecord_util.py
 easycv/datasets/utils/transform_util.py
 easycv/datasets/utils/type_util.py
 easycv/datasets/utils/download_data/__init__.py
 easycv/datasets/utils/download_data/commont.py
 easycv/datasets/utils/download_data/download_coco.py
 easycv/datasets/utils/download_data/download_voc.py
+easycv/datasets/video_recognition/__init__.py
+easycv/datasets/video_recognition/raw.py
+easycv/datasets/video_recognition/data_sources/__init__.py
+easycv/datasets/video_recognition/data_sources/video_datasource.py
+easycv/datasets/video_recognition/data_sources/video_text_datasource.py
+easycv/datasets/video_recognition/pipelines/__init__.py
+easycv/datasets/video_recognition/pipelines/loading.py
+easycv/datasets/video_recognition/pipelines/text_transform.py
+easycv/datasets/video_recognition/pipelines/transform.py
 easycv/file/__init__.py
 easycv/file/base.py
 easycv/file/file_io.py
 easycv/file/image.py
 easycv/file/utils.py
 easycv/framework/__init__.py
 easycv/framework/errors.py
@@ -529,14 +550,15 @@
 easycv/models/base.py
 easycv/models/builder.py
 easycv/models/modelzoo.py
 easycv/models/registry.py
 easycv/models/backbones/__init__.py
 easycv/models/backbones/benchmark_mlp.py
 easycv/models/backbones/bninception.py
+easycv/models/backbones/clip_bert.py
 easycv/models/backbones/conv_mae_vit.py
 easycv/models/backbones/conv_vitdet.py
 easycv/models/backbones/darknet.py
 easycv/models/backbones/edgevit.py
 easycv/models/backbones/efficientformer.py
 easycv/models/backbones/face_keypoint_backbone.py
 easycv/models/backbones/genet.py
@@ -552,18 +574,20 @@
 easycv/models/backbones/repvgg_yolox_backbone.py
 easycv/models/backbones/resnest.py
 easycv/models/backbones/resnet.py
 easycv/models/backbones/resnet_jit.py
 easycv/models/backbones/resnext.py
 easycv/models/backbones/shuffle_transformer.py
 easycv/models/backbones/swin_transformer.py
+easycv/models/backbones/swin_transformer3d.py
 easycv/models/backbones/swin_transformer_dynamic.py
 easycv/models/backbones/vision_transformer.py
 easycv/models/backbones/vit_transformer_dynamic.py
 easycv/models/backbones/vitdet.py
+easycv/models/backbones/x3d.py
 easycv/models/backbones/xcit_transformer.py
 easycv/models/classification/__init__.py
 easycv/models/classification/classification.py
 easycv/models/classification/necks.py
 easycv/models/detection/__init__.py
 easycv/models/detection/dense_heads/__init__.py
 easycv/models/detection/dense_heads/anchor_free_head.py
@@ -708,27 +732,37 @@
 easycv/models/utils/norm.py
 easycv/models/utils/ops.py
 easycv/models/utils/pos_embed.py
 easycv/models/utils/res_layer.py
 easycv/models/utils/scale.py
 easycv/models/utils/sobel.py
 easycv/models/utils/transformer.py
+easycv/models/utils/video_model_stem.py
+easycv/models/utils/x3d_transformer.py
+easycv/models/video_recognition/ClipBertTwoStream.py
+easycv/models/video_recognition/__init__.py
+easycv/models/video_recognition/recognizer3d.py
+easycv/models/video_recognition/heads/__init__.py
+easycv/models/video_recognition/heads/base_head.py
+easycv/models/video_recognition/heads/i3d_head.py
+easycv/models/video_recognition/heads/x3d_head.py
 easycv/predictors/__init__.py
 easycv/predictors/base.py
 easycv/predictors/bevformer_predictor.py
 easycv/predictors/builder.py
 easycv/predictors/classifier.py
 easycv/predictors/detector.py
 easycv/predictors/face_keypoints_predictor.py
 easycv/predictors/feature_extractor.py
 easycv/predictors/hand_keypoints_predictor.py
 easycv/predictors/interface.py
 easycv/predictors/ocr.py
 easycv/predictors/pose_predictor.py
 easycv/predictors/segmentation.py
+easycv/predictors/video_classifier.py
 easycv/predictors/wholebody_keypoints_predictor.py
 easycv/resource/simhei.ttf
 easycv/runner/__init__.py
 easycv/runner/ev_runner.py
 easycv/thirdparty/__init__.py
 easycv/thirdparty/face_align.py
 easycv/thirdparty/deformable_attention/__init__.py
@@ -741,14 +775,22 @@
 easycv/thirdparty/deformable_attention/src/ms_deform_attn.h
 easycv/thirdparty/deformable_attention/src/vision.cpp
 easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.cpp
 easycv/thirdparty/deformable_attention/src/cpu/ms_deform_attn_cpu.h
 easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.cu
 easycv/thirdparty/deformable_attention/src/cuda/ms_deform_attn_cuda.h
 easycv/thirdparty/deformable_attention/src/cuda/ms_deform_im2col_cuda.cuh
+easycv/thirdparty/mot/__init__.py
+easycv/thirdparty/mot/demo_mot.py
+easycv/thirdparty/mot/utils.py
+easycv/thirdparty/mot/bytetrack/__init__.py
+easycv/thirdparty/mot/bytetrack/basetrack.py
+easycv/thirdparty/mot/bytetrack/byte_tracker.py
+easycv/thirdparty/mot/bytetrack/kalman_filter.py
+easycv/thirdparty/mot/bytetrack/matching.py
 easycv/thirdparty/mtcnn/__init__.py
 easycv/thirdparty/mtcnn/detector.py
 easycv/thirdparty/mtcnn/get_nets.py
 easycv/thirdparty/mtcnn/utils.py
 easycv/thirdparty/u2sod/__init__.py
 easycv/thirdparty/u2sod/sodpredictor.py
 easycv/thirdparty/u2sod/u2net_models.py
```

### Comparing `pai-easycv-0.8.0/pai_easycv.egg-info/PKG-INFO` & `pai-easycv-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pai-easycv
-Version: 0.8.0
+Version: 0.9.0
 Summary: An all-in-one toolkit for computer vision
 Home-page: https://github.com/alibaba/EasyCV.git
 Author: Alibaba PAI team
 Author-email: easycv@list.alibaba-inc.com
 License: Apache License 2.0
 Description: 
         <div align="center">
@@ -50,14 +50,20 @@
         
         - **Efficiency**
         
           EasyCV supports multi-gpu and multi-worker training. EasyCV uses [DALI](https://github.com/NVIDIA/DALI) to accelerate data io and preprocessing process, and uses [TorchAccelerator](https://github.com/alibaba/EasyCV/tree/master/docs/source/tutorials/torchacc.md) and fp16 to accelerate training process. For inference optimization, EasyCV exports model using jit script, which can be optimized by [PAI-Blade](https://help.aliyun.com/document_detail/205134.html)
         
         
         ## What's New
+        [🔥 2023.01.17]
+        
+        * 17/01/2023 EasyCV v0.9.0 was released.
+        - Support Single-lens MOT
+        - Support video recognition (X3D, SWIN-video)
+        
         [🔥 2022.12.02]
         
         * 02/12/2022 EasyCV v0.8.0 was released.
         - bevformer-base NDS increased by 0.8 on nuscenes val, training speed increased by 10%, and inference speed increased by 40%.
         - Support Objects365 pretrain and Adding the DINO++ model can achieve an accuracy of 63.4mAP at a model scale of 200M(Under the same scale, the accuracy is the best).
         
         [🔥 2022.08.31] We have released our YOLOX-PAI that achieves SOTA results within 40~50 mAP (less than 1ms). And we also provide a convenient and fast export/predictor api for end2end object detection. To get a quick start of YOLOX-PAI, click [here](docs/source/tutorials/yolox.md)!
@@ -97,15 +103,15 @@
         * [image classification](docs/source/tutorials/cls.md)
         * [metric learning](docs/source/tutorials/metric_learning.md)
         * [object detection with yolox-pai](docs/source/tutorials/yolox.md)
         * [model compression with yolox](docs/source/tutorials/compression.md)
         * [using torchacc](docs/source/tutorials/torchacc.md)
         * [file io for local and oss files](docs/source/tutorials/file.md)
         * [using mmdetection model in EasyCV](docs/source/tutorials/mmdet_models_usage_guide.md)
-        * [batch prediction tools][docs/source/tutorials/predict.md]
+        * [batch prediction tools](docs/source/tutorials/predict.md)
         
         
         
         notebook
         * [self-supervised learning](docs/source/tutorials/EasyCV图像自监督训练-MAE.ipynb)
         * [image classification](docs/source/tutorials/EasyCV图像分类resnet50.ipynb)
         * [object detection with yolox-pai](docs/source/tutorials/EasyCV图像检测YoloX.ipynb)
```

