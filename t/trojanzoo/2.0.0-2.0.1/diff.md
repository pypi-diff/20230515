# Comparing `tmp/trojanzoo-2.0.0.tar.gz` & `tmp/trojanzoo-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trojanzoo-2.0.0.tar", last modified: Sun May 14 09:58:21 2023, max compression
+gzip compressed data, was "trojanzoo-2.0.1.tar", last modified: Sun May 14 23:51:34 2023, max compression
```

## Comparing `trojanzoo-2.0.0.tar` & `trojanzoo-2.0.1.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9623 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8712 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.820679 trojanzoo-2.0.0/docs/
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.820679 trojanzoo-2.0.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.820679 trojanzoo-2.0.0/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)     4286 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.820679 trojanzoo-2.0.0/docs/source/images/logo/
--rw-r--r--   0 root         (0) root         (0)     8520 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo-dark.svg
--rw-r--r--   0 root         (0) root         (0)     5671 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo-icon.svg
--rw-r--r--   0 root         (0) root         (0)     7587 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo.svg
--rw-r--r--   0 root         (0) root         (0)   570067 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/screenshot.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/images/trojanvision/
--rw-r--r--   0 root         (0) root         (0)    83160 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/center_cropped.png
--rw-r--r--   0 root         (0) root         (0)    16840 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/grad_cam.png
--rw-r--r--   0 root         (0) root         (0)    79679 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/grad_cam_impose.png
--rw-r--r--   0 root         (0) root         (0)    51879 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/saliency_map.png
--rw-r--r--   0 root         (0) root         (0)    92604 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/saliency_map_impose.png
--rw-r--r--   0 root         (0) root         (0)    68027 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanzoo-logo-readme.svg
--rw-r--r--   0 root         (0) root         (0)      507 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/attacks/
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/adv.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/clean_label.rst
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/dynamic.rst
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/index.rst
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/normal.rst
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/index.rst
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/configs.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/datasets/
--rw-r--r--   0 root         (0) root         (0)      317 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/datasets/folder.rst
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/datasets/index.rst
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/datasets/normal.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/defenses/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/adv.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/attack_agnostic.rst
--rw-r--r--   0 root         (0) root         (0)      209 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/index.rst
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/input_filtering.rst
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/model_inspection.rst
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/training_filtering.rst
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/index.rst
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/environ.rst
--rw-r--r--   0 root         (0) root         (0)      206 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/index.rst
--rw-r--r--   0 root         (0) root         (0)      174 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/marks.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/trojanvision/models/
--rw-r--r--   0 root         (0) root         (0)      283 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/models/index.rst
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/models/nas.rst
--rw-r--r--   0 root         (0) root         (0)      129 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/models/others.rst
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/models/torchvision.rst
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/optim.rst
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/trainer.rst
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/utils.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/trojanzoo/
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/attacks.rst
--rw-r--r--   0 root         (0) root         (0)      127 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/configs.rst
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/datasets.rst
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/defenses.rst
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/environ.rst
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/index.rst
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/models.rst
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/optim.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/trainer.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/trojanzoo/utils/
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/data.rst
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/fim.rst
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/index.rst
--rw-r--r--   0 root         (0) root         (0)      213 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/logger.rst
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/model.rst
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/module.rst
--rw-r--r--   0 root         (0) root         (0)      206 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/tensor.rst
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/train.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/tutorials/
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/tutorials/basic.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/examples/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/adv_attack.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/adv_defense.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/adv_validate.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/backdoor_attack.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/backdoor_defense.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/backdoor_validate.py
--rw-r--r--   0 root         (0) root         (0)     1013 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/heatmap.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/test.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/train.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/validate.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/
--rw-r--r--   0 root         (0) root         (0)     3584 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18456 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/adv/
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/adv/__init__.py
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/adv/pgd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/__init__.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/clean_label.py
--rw-r--r--   0 root         (0) root         (0)    11700 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/invisible_poison.py
--rw-r--r--   0 root         (0) root         (0)    16740 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/label_consistent.py
--rw-r--r--   0 root         (0) root         (0)    26368 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/refool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/dynamic/
--rw-r--r--   0 root         (0) root         (0)      248 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/dynamic/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30304 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/dynamic/input_aware_dynamic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/
--rw-r--r--   0 root         (0) root         (0)      474 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/__init__.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/badnet.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/imc.py
--rw-r--r--   0 root         (0) root         (0)    10777 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/latent_backdoor.py
--rw-r--r--   0 root         (0) root         (0)    15353 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/trojannet.py
--rw-r--r--   0 root         (0) root         (0)    11063 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/trojannn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/others/
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/others/unlearn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/attacks/poison/
--rw-r--r--   0 root         (0) root         (0)      373 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/poison/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8430 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/poison/imc_poison.py
--rw-r--r--   0 root         (0) root         (0)     7186 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/poison/poison_basic.py
--rw-r--r--   0 root         (0) root         (0)     4085 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/poison/poison_random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/configs/
--rw-r--r--   0 root         (0) root         (0)     1057 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/configs/attack/
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/bypass_embed.yml
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/clean_label.yml
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/hidden_trigger.yml
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/pgd.yml
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/reflection_backdoor.yml
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/dataset.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/configs/defense/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/abs.yml
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/activation_clustering.yml
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/advmind.yml
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/fine_pruning.yml
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/image_transform.yml
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/neo.yml
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/neuron_inspect.yml
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/spectral_signature.yml
--rw-r--r--   0 root         (0) root         (0)      261 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/model.yml
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/trainer.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.816679 trojanzoo-2.0.0/trojanvision/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/data/cub200/
--rw-r--r--   0 root         (0) root         (0)   174592 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/cub200/test.txt
--rw-r--r--   0 root         (0) root         (0)   168954 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/cub200/train.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/cub200_2011/
--rw-r--r--   0 root         (0) root         (0)   682287 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/cub200_2011/images.txt
--rw-r--r--   0 root         (0) root         (0)    83198 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/cub200_2011/train_test_split.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/isic2018/
--rw-r--r--   0 root         (0) root         (0)   410650 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/isic2018/train.csv
--rw-r--r--   0 root         (0) root         (0)     7948 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/isic2018/valid.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/refool/
--rw-r--r--   0 root         (0) root         (0)     8680 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/refool/insert_reflection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/sample_imagenet/
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/sample_imagenet/class_dict.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/stl10/
--rw-r--r--   0 root         (0) root         (0)   100000 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/stl10/unlabeled_y.bin
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/datasets/
--rw-r--r--   0 root         (0) root         (0)     2911 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/datasets/folder/
--rw-r--r--   0 root         (0) root         (0)      679 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5558 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/cub200.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/gtsrb.py
--rw-r--r--   0 root         (0) root         (0)     4814 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/imagenet.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/isic.py
--rw-r--r--   0 root         (0) root         (0)     1655 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/vggface2.py
--rw-r--r--   0 root         (0) root         (0)    14991 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/imagefolder.py
--rw-r--r--   0 root         (0) root         (0)    10615 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/imageset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/datasets/normal/
--rw-r--r--   0 root         (0) root         (0)      592 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1262 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/celeba.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/cifar.py
--rw-r--r--   0 root         (0) root         (0)     4314 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/downsampled_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/mnist.py
--rw-r--r--   0 root         (0) root         (0)     4725 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/stl10.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/defenses/
--rw-r--r--   0 root         (0) root         (0)     1560 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23436 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/adv/
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/adv/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17940 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/adv/advmind.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/adv/curvature.py
--rw-r--r--   0 root         (0) root         (0)     2603 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/adv/grad_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/
--rw-r--r--   0 root         (0) root         (0)      532 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5981 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/adv_train.py
--rw-r--r--   0 root         (0) root         (0)     4215 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/fine_pruning.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/magnet.py
--rw-r--r--   0 root         (0) root         (0)      287 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/randomized_smooth.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/recompress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/neo.py
--rw-r--r--   0 root         (0) root         (0)     3610 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/strip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/
--rw-r--r--   0 root         (0) root         (0)      504 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14370 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/abs.py
--rw-r--r--   0 root         (0) root         (0)     6652 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/deep_inspect.py
--rw-r--r--   0 root         (0) root         (0)     5908 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/neural_cleanse.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/neuron_inspect.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/tabor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/
--rw-r--r--   0 root         (0) root         (0)      387 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10901 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/activation_clustering.py
--rw-r--r--   0 root         (0) root         (0)     7870 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/spectral_signature.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/environ.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/marks/
--rw-r--r--   0 root         (0) root         (0)    22268 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3602 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/apple_black.png
--rw-r--r--   0 root         (0) root         (0)     3595 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/apple_white.png
--rw-r--r--   0 root         (0) root         (0)      756 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/square_black.png
--rw-r--r--   0 root         (0) root         (0)      675 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/square_white.png
--rw-r--r--   0 root         (0) root         (0)     9850 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/tag_black.png
--rw-r--r--   0 root         (0) root         (0)     9823 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/tag_white.png
--rw-r--r--   0 root         (0) root         (0)    26522 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/watermark_black.png
--rw-r--r--   0 root         (0) root         (0)    26281 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/watermark_white.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/
--rw-r--r--   0 root         (0) root         (0)     4128 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29817 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/imagemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/nas/
--rw-r--r--   0 root         (0) root         (0)      524 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20990 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/darts.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/enas.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/lanet.py
--rw-r--r--   0 root         (0) root         (0)     8069 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/natsbench.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/pnasnet.py
--rw-r--r--   0 root         (0) root         (0)     3494 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/proxylessnas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/normal/
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9448 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/bit.py
--rw-r--r--   0 root         (0) root         (0)     3928 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/dla.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/dpn.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/net.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/others/
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7219 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/others/magnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/torchvision/
--rw-r--r--   0 root         (0) root         (0)      724 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/alexnet.py
--rw-r--r--   0 root         (0) root         (0)     3648 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/densenet.py
--rw-r--r--   0 root         (0) root         (0)     4174 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/efficientnet.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/mnasnet.py
--rw-r--r--   0 root         (0) root         (0)     3530 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/mobilenet.py
--rw-r--r--   0 root         (0) root         (0)     8284 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/resnet.py
--rw-r--r--   0 root         (0) root         (0)     4247 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/shufflenetv2.py
--rw-r--r--   0 root         (0) root         (0)     3699 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/vgg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/shortcut/
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/shortcut/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13302 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/shortcut/pgd.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/
--rw-r--r--   0 root         (0) root         (0)     2641 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9275 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/datasets/
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6102 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/datasets/downsampled_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/model_archs/
--rw-r--r--   0 root         (0) root         (0)      885 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/bit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4593 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/features.py
--rw-r--r--   0 root         (0) root         (0)    10884 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/genotypes.py
--rw-r--r--   0 root         (0) root         (0)     5945 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/operations.py
--rw-r--r--   0 root         (0) root         (0)     6067 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/search.py
--rw-r--r--   0 root         (0) root         (0)    11910 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/sgas.py
--rw-r--r--   0 root         (0) root         (0)    10085 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/dla.py
--rw-r--r--   0 root         (0) root         (0)     8661 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/dpn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/macro.py
--rw-r--r--   0 root         (0) root         (0)    14031 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/mutables.py
--rw-r--r--   0 root         (0) root         (0)     3400 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/ops.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/lanet.py
--rw-r--r--   0 root         (0) root         (0)     4285 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/pnasnet.py
--rw-r--r--   0 root         (0) root         (0)     5806 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/resnet_ap.py
--rw-r--r--   0 root         (0) root         (0)     1933 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/resnet_s.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/sgm.py
--rw-r--r--   0 root         (0) root         (0)    11205 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanzoo/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6739 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/attacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo/configs/
--rw-r--r--   0 root         (0) root         (0)    10382 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/__init__.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/attack.yml
--rw-r--r--   0 root         (0) root         (0)      125 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/dataset.yml
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/defense.yml
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/env.yml
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/model.yml
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/trainer.yml
--rw-r--r--   0 root         (0) root         (0)    22356 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/datasets.py
--rw-r--r--   0 root         (0) root         (0)     6064 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/defenses.py
--rw-r--r--   0 root         (0) root         (0)     7468 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/environ.py
--rw-r--r--   0 root         (0) root         (0)    66195 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo/optim/
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10815 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/optim/optimizer.py
--rw-r--r--   0 root         (0) root         (0)    13659 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/optim/pgd.py
--rw-r--r--   0 root         (0) root         (0)     4831 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/optim/uname.py
--rw-r--r--   0 root         (0) root         (0)    14367 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo/utils/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7818 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo/utils/fim/
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/fim/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12525 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/fim/ekfac.py
--rw-r--r--   0 root         (0) root         (0)     3897 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/fim/fim.py
--rw-r--r--   0 root         (0) root         (0)    15646 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/fim/kfac.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/lock.py
--rw-r--r--   0 root         (0) root         (0)    14626 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/memory.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/metric.py
--rw-r--r--   0 root         (0) root         (0)    25201 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/trojanzoo/utils/module/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6231 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/module/param.py
--rw-r--r--   0 root         (0) root         (0)     6545 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/module/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/trojanzoo/utils/ntk/
--rw-r--r--   0 root         (0) root         (0)     1918 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/ntk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3795 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/output.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/tensor.py
--rw-r--r--   0 root         (0) root         (0)    13800 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/train.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9623 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10615 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.726260 trojanzoo-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9623 2023-05-14 23:51:34.726260 trojanzoo-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8712 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.678260 trojanzoo-2.0.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.678260 trojanzoo-2.0.1/docs/source/
+-rw-r--r--   0 root         (0) root         (0)     4069 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.682260 trojanzoo-2.0.1/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.682260 trojanzoo-2.0.1/docs/source/images/logo/
+-rw-r--r--   0 root         (0) root         (0)     8520 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/logo/trojanzoo-logo-dark.svg
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/logo/trojanzoo-logo-icon.svg
+-rw-r--r--   0 root         (0) root         (0)     7587 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/logo/trojanzoo-logo.svg
+-rw-r--r--   0 root         (0) root         (0)   570067 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/screenshot.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.682260 trojanzoo-2.0.1/docs/source/images/trojanvision/
+-rw-r--r--   0 root         (0) root         (0)    83160 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/trojanvision/center_cropped.png
+-rw-r--r--   0 root         (0) root         (0)    16840 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/trojanvision/grad_cam.png
+-rw-r--r--   0 root         (0) root         (0)    79679 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/trojanvision/grad_cam_impose.png
+-rw-r--r--   0 root         (0) root         (0)    51879 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/trojanvision/saliency_map.png
+-rw-r--r--   0 root         (0) root         (0)    92604 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/trojanvision/saliency_map_impose.png
+-rw-r--r--   0 root         (0) root         (0)    68027 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/images/trojanzoo-logo-readme.svg
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.682260 trojanzoo-2.0.1/docs/source/trojanvision/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.682260 trojanzoo-2.0.1/docs/source/trojanvision/attacks/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/attacks/adv.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.686260 trojanzoo-2.0.1/docs/source/trojanvision/attacks/backdoor/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/attacks/backdoor/clean_label.rst
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/attacks/backdoor/dynamic.rst
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/attacks/backdoor/index.rst
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/attacks/backdoor/normal.rst
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/attacks/index.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/configs.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.686260 trojanzoo-2.0.1/docs/source/trojanvision/datasets/
+-rw-r--r--   0 root         (0) root         (0)      317 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/datasets/folder.rst
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/datasets/index.rst
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/datasets/normal.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.686260 trojanzoo-2.0.1/docs/source/trojanvision/defenses/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/defenses/adv.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.686260 trojanzoo-2.0.1/docs/source/trojanvision/defenses/backdoor/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/defenses/backdoor/attack_agnostic.rst
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/defenses/backdoor/index.rst
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/defenses/backdoor/input_filtering.rst
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/defenses/backdoor/model_inspection.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/defenses/backdoor/training_filtering.rst
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/defenses/index.rst
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/environ.rst
+-rw-r--r--   0 root         (0) root         (0)      206 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/index.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/marks.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.686260 trojanzoo-2.0.1/docs/source/trojanvision/models/
+-rw-r--r--   0 root         (0) root         (0)      283 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/models/index.rst
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/models/nas.rst
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/models/others.rst
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/models/torchvision.rst
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/optim.rst
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/trainer.rst
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanvision/utils.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.686260 trojanzoo-2.0.1/docs/source/trojanzoo/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/attacks.rst
+-rw-r--r--   0 root         (0) root         (0)      127 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/configs.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/datasets.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/defenses.rst
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/environ.rst
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/index.rst
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/models.rst
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/optim.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/trainer.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.690260 trojanzoo-2.0.1/docs/source/trojanzoo/utils/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/utils/data.rst
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/utils/fim.rst
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/utils/index.rst
+-rw-r--r--   0 root         (0) root         (0)      213 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/utils/logger.rst
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/utils/model.rst
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/utils/module.rst
+-rw-r--r--   0 root         (0) root         (0)      206 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/utils/tensor.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/trojanzoo/utils/train.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.690260 trojanzoo-2.0.1/docs/source/tutorials/
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/docs/source/tutorials/basic.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.690260 trojanzoo-2.0.1/examples/
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/adv_attack.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/adv_defense.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/adv_validate.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/backdoor_attack.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/backdoor_defense.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/backdoor_validate.py
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/heatmap.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/test.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/train.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/examples/validate.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-14 23:51:34.726260 trojanzoo-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.690260 trojanzoo-2.0.1/trojanvision/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.690260 trojanzoo-2.0.1/trojanvision/attacks/
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18456 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.694260 trojanzoo-2.0.1/trojanvision/attacks/adv/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/adv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/adv/pgd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.694260 trojanzoo-2.0.1/trojanvision/attacks/backdoor/
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.694260 trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/clean_label.py
+-rw-r--r--   0 root         (0) root         (0)    11700 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/invisible_poison.py
+-rw-r--r--   0 root         (0) root         (0)    16740 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/label_consistent.py
+-rw-r--r--   0 root         (0) root         (0)    26368 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/refool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.694260 trojanzoo-2.0.1/trojanvision/attacks/backdoor/dynamic/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/dynamic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30304 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/dynamic/input_aware_dynamic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.694260 trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/
+-rw-r--r--   0 root         (0) root         (0)      474 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/badnet.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/imc.py
+-rw-r--r--   0 root         (0) root         (0)    10777 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/latent_backdoor.py
+-rw-r--r--   0 root         (0) root         (0)    15353 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/trojannet.py
+-rw-r--r--   0 root         (0) root         (0)    11063 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/trojannn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.694260 trojanzoo-2.0.1/trojanvision/attacks/backdoor/others/
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/backdoor/others/unlearn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.694260 trojanzoo-2.0.1/trojanvision/attacks/poison/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/poison/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8430 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/poison/imc_poison.py
+-rw-r--r--   0 root         (0) root         (0)     7186 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/poison/poison_basic.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/attacks/poison/poison_random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.698260 trojanzoo-2.0.1/trojanvision/configs/
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.698260 trojanzoo-2.0.1/trojanvision/configs/attack/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/attack/bypass_embed.yml
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/attack/clean_label.yml
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/attack/hidden_trigger.yml
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/attack/pgd.yml
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/attack/reflection_backdoor.yml
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/dataset.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.698260 trojanzoo-2.0.1/trojanvision/configs/defense/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/defense/abs.yml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/defense/activation_clustering.yml
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/defense/advmind.yml
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/defense/fine_pruning.yml
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/defense/image_transform.yml
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/defense/neo.yml
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/defense/neuron_inspect.yml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/defense/spectral_signature.yml
+-rw-r--r--   0 root         (0) root         (0)      261 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/model.yml
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/configs/trainer.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.674260 trojanzoo-2.0.1/trojanvision/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.698260 trojanzoo-2.0.1/trojanvision/data/cub200/
+-rw-r--r--   0 root         (0) root         (0)   174592 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/cub200/test.txt
+-rw-r--r--   0 root         (0) root         (0)   168954 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/cub200/train.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.702260 trojanzoo-2.0.1/trojanvision/data/cub200_2011/
+-rw-r--r--   0 root         (0) root         (0)   682287 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/cub200_2011/images.txt
+-rw-r--r--   0 root         (0) root         (0)    83198 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/cub200_2011/train_test_split.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.702260 trojanzoo-2.0.1/trojanvision/data/isic2018/
+-rw-r--r--   0 root         (0) root         (0)   410650 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/isic2018/train.csv
+-rw-r--r--   0 root         (0) root         (0)     7948 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/isic2018/valid.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.702260 trojanzoo-2.0.1/trojanvision/data/refool/
+-rw-r--r--   0 root         (0) root         (0)     8680 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/refool/insert_reflection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.702260 trojanzoo-2.0.1/trojanvision/data/sample_imagenet/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/sample_imagenet/class_dict.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.702260 trojanzoo-2.0.1/trojanvision/data/stl10/
+-rw-r--r--   0 root         (0) root         (0)   100000 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/data/stl10/unlabeled_y.bin
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.702260 trojanzoo-2.0.1/trojanvision/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.702260 trojanzoo-2.0.1/trojanvision/datasets/folder/
+-rw-r--r--   0 root         (0) root         (0)      679 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/folder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/folder/cub200.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/folder/gtsrb.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/folder/imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/folder/isic.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/folder/vggface2.py
+-rw-r--r--   0 root         (0) root         (0)    14991 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/imagefolder.py
+-rw-r--r--   0 root         (0) root         (0)    10615 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/imageset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.706260 trojanzoo-2.0.1/trojanvision/datasets/normal/
+-rw-r--r--   0 root         (0) root         (0)      592 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/normal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/normal/celeba.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/normal/cifar.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/normal/downsampled_imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/normal/mnist.py
+-rw-r--r--   0 root         (0) root         (0)     4725 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/datasets/normal/stl10.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.706260 trojanzoo-2.0.1/trojanvision/defenses/
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23436 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.706260 trojanzoo-2.0.1/trojanvision/defenses/adv/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/adv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17940 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/adv/advmind.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/adv/curvature.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/adv/grad_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.706260 trojanzoo-2.0.1/trojanvision/defenses/backdoor/
+-rw-r--r--   0 root         (0) root         (0)      532 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.706260 trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/adv_train.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/fine_pruning.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/magnet.py
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/randomized_smooth.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/recompress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.706260 trojanzoo-2.0.1/trojanvision/defenses/backdoor/input_filtering/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/input_filtering/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/input_filtering/neo.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/input_filtering/strip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.706260 trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14370 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/abs.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/deep_inspect.py
+-rw-r--r--   0 root         (0) root         (0)     5908 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/neural_cleanse.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/neuron_inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/tabor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.710260 trojanzoo-2.0.1/trojanvision/defenses/backdoor/training_filtering/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/training_filtering/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10901 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/training_filtering/activation_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     7870 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/defenses/backdoor/training_filtering/spectral_signature.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/environ.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.710260 trojanzoo-2.0.1/trojanvision/marks/
+-rw-r--r--   0 root         (0) root         (0)    22268 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/apple_black.png
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/apple_white.png
+-rw-r--r--   0 root         (0) root         (0)      756 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/square_black.png
+-rw-r--r--   0 root         (0) root         (0)      675 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/square_white.png
+-rw-r--r--   0 root         (0) root         (0)     9850 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/tag_black.png
+-rw-r--r--   0 root         (0) root         (0)     9823 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/tag_white.png
+-rw-r--r--   0 root         (0) root         (0)    26522 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/watermark_black.png
+-rw-r--r--   0 root         (0) root         (0)    26281 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/marks/watermark_white.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.710260 trojanzoo-2.0.1/trojanvision/models/
+-rw-r--r--   0 root         (0) root         (0)     4128 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29817 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/imagemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.710260 trojanzoo-2.0.1/trojanvision/models/nas/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/nas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20990 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/nas/darts.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/nas/enas.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/nas/lanet.py
+-rw-r--r--   0 root         (0) root         (0)     8069 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/nas/natsbench.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/nas/pnasnet.py
+-rw-r--r--   0 root         (0) root         (0)     3494 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/nas/proxylessnas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.714259 trojanzoo-2.0.1/trojanvision/models/normal/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/normal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9480 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/normal/bit.py
+-rw-r--r--   0 root         (0) root         (0)     3928 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/normal/dla.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/normal/dpn.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/normal/net.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.714259 trojanzoo-2.0.1/trojanvision/models/others/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/others/magnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.714259 trojanzoo-2.0.1/trojanvision/models/torchvision/
+-rw-r--r--   0 root         (0) root         (0)      724 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/alexnet.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/densenet.py
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/efficientnet.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/mnasnet.py
+-rw-r--r--   0 root         (0) root         (0)     3530 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/mobilenet.py
+-rw-r--r--   0 root         (0) root         (0)     8284 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/resnet.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/shufflenetv2.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/models/torchvision/vgg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.714259 trojanzoo-2.0.1/trojanvision/shortcut/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/shortcut/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13302 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/shortcut/pgd.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.714259 trojanzoo-2.0.1/trojanvision/utils/
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9275 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.714259 trojanzoo-2.0.1/trojanvision/utils/datasets/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6102 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/datasets/downsampled_imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.718259 trojanzoo-2.0.1/trojanvision/utils/model_archs/
+-rw-r--r--   0 root         (0) root         (0)      918 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/bit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.718259 trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4593 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/features.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/genotypes.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/operations.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/search.py
+-rw-r--r--   0 root         (0) root         (0)    11910 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/sgas.py
+-rw-r--r--   0 root         (0) root         (0)    10085 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/dla.py
+-rw-r--r--   0 root         (0) root         (0)     8661 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/dpn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.718259 trojanzoo-2.0.1/trojanvision/utils/model_archs/enas/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/enas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/enas/macro.py
+-rw-r--r--   0 root         (0) root         (0)    14031 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/enas/mutables.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/enas/ops.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/lanet.py
+-rw-r--r--   0 root         (0) root         (0)     4285 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/pnasnet.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/resnet_ap.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/model_archs/resnet_s.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/sgm.py
+-rw-r--r--   0 root         (0) root         (0)    11205 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanvision/utils/transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.718259 trojanzoo-2.0.1/trojanzoo/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6739 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/attacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.722259 trojanzoo-2.0.1/trojanzoo/configs/
+-rw-r--r--   0 root         (0) root         (0)    10382 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/configs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/configs/attack.yml
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/configs/dataset.yml
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/configs/defense.yml
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/configs/env.yml
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/configs/model.yml
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/configs/trainer.yml
+-rw-r--r--   0 root         (0) root         (0)    22356 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6064 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/defenses.py
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/environ.py
+-rw-r--r--   0 root         (0) root         (0)    66218 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.722259 trojanzoo-2.0.1/trojanzoo/optim/
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/optim/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    13659 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/optim/pgd.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/optim/uname.py
+-rw-r--r--   0 root         (0) root         (0)    14367 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.722259 trojanzoo-2.0.1/trojanzoo/utils/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7818 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.726260 trojanzoo-2.0.1/trojanzoo/utils/fim/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/fim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/fim/ekfac.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/fim/fim.py
+-rw-r--r--   0 root         (0) root         (0)    15646 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/fim/kfac.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/lock.py
+-rw-r--r--   0 root         (0) root         (0)    14536 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/memory.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/metric.py
+-rw-r--r--   0 root         (0) root         (0)    25201 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.726260 trojanzoo-2.0.1/trojanzoo/utils/module/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6301 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/module/param.py
+-rw-r--r--   0 root         (0) root         (0)     6545 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/module/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.726260 trojanzoo-2.0.1/trojanzoo/utils/ntk/
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/ntk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/output.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/tensor.py
+-rw-r--r--   0 root         (0) root         (0)    13800 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/utils/train.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 23:51:26.000000 trojanzoo-2.0.1/trojanzoo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 23:51:34.722259 trojanzoo-2.0.1/trojanzoo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9623 2023-05-14 23:51:34.000000 trojanzoo-2.0.1/trojanzoo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10615 2023-05-14 23:51:34.000000 trojanzoo-2.0.1/trojanzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 23:51:34.000000 trojanzoo-2.0.1/trojanzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 23:51:34.000000 trojanzoo-2.0.1/trojanzoo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-14 23:51:34.000000 trojanzoo-2.0.1/trojanzoo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-14 23:51:34.000000 trojanzoo-2.0.1/trojanzoo.egg-info/top_level.txt
```

### Comparing `trojanzoo-2.0.0/LICENSE` & `trojanzoo-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/PKG-INFO` & `trojanzoo-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo
-Version: 2.0.0
+Version: 2.0.1
 Summary: a universal pytorch platform to conduct security researches
 Home-page: https://github.com/ain-soph/trojanzoo
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Keywords: pytorch,image classification,backdoor attack/defense
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
@@ -12,25 +12,25 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TrojanZoo
 ![logo](https://github.com/ain-soph/trojanzoo/raw/main/docs/source/images/trojanzoo-logo-readme.svg)
 
 [![contact](https://img.shields.io/badge/contact-rbp5354@psu.edu-yellow)](mailto:rbp5354@psu.edu)
 [![License](https://img.shields.io/github/license/ain-soph/trojanzoo)](https://opensource.org/licenses/GPL-3.0)
 
-![python>=3.10](https://img.shields.io/badge/python->=3.10-informational.svg)
+![python>=3.11](https://img.shields.io/badge/python->=3.11-informational.svg)
 [![docs](https://github.com/ain-soph/trojanzoo/workflows/docs/badge.svg)](https://ain-soph.github.io/trojanzoo/)
 
 [![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo)](https://github.com/ain-soph/trojanzoo/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo)](https://pypi.org/project/trojanzoo/)
 [![docker](https://img.shields.io/pypi/v/trojanzoo?label=docker)](https://hub.docker.com/r/local0state/trojanzoo)
 <!-- [![conda](https://img.shields.io/pypi/v/trojanzoo?label=conda)](https://anaconda.org/anaconda/trojanzoo) -->
```

### Comparing `trojanzoo-2.0.0/README.md` & `trojanzoo-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # TrojanZoo
 ![logo](https://github.com/ain-soph/trojanzoo/raw/main/docs/source/images/trojanzoo-logo-readme.svg)
 
 [![contact](https://img.shields.io/badge/contact-rbp5354@psu.edu-yellow)](mailto:rbp5354@psu.edu)
 [![License](https://img.shields.io/github/license/ain-soph/trojanzoo)](https://opensource.org/licenses/GPL-3.0)
 
-![python>=3.10](https://img.shields.io/badge/python->=3.10-informational.svg)
+![python>=3.11](https://img.shields.io/badge/python->=3.11-informational.svg)
 [![docs](https://github.com/ain-soph/trojanzoo/workflows/docs/badge.svg)](https://ain-soph.github.io/trojanzoo/)
 
 [![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo)](https://github.com/ain-soph/trojanzoo/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo)](https://pypi.org/project/trojanzoo/)
 [![docker](https://img.shields.io/pypi/v/trojanzoo?label=docker)](https://hub.docker.com/r/local0state/trojanzoo)
 <!-- [![conda](https://img.shields.io/pypi/v/trojanzoo?label=conda)](https://anaconda.org/anaconda/trojanzoo) -->
```

### Comparing `trojanzoo-2.0.0/docs/make.bat` & `trojanzoo-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/conf.py` & `trojanzoo-2.0.1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
 
 # autodoc options
 autodoc_docstring_signature = True
 autodoc_inherit_docstrings = False
 autodoc_preserve_defaults = True
 autodoc_typehints = 'none'
 
+toc_object_entries = True
+toc_object_entries_show_parents = "hide"
 # autoapi_type = 'python'
 # autoapi_generate_api_docs = False
 
 # autosectionlabel options
 # autosectionlabel throws warnings if section names are duplicated.
 # The following tells autosectionlabel to not throw a warning for
 # duplicated section names that are in different documents.
```

### Comparing `trojanzoo-2.0.0/docs/source/images/favicon.ico` & `trojanzoo-2.0.1/docs/source/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo-dark.svg` & `trojanzoo-2.0.1/docs/source/images/logo/trojanzoo-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo-icon.svg` & `trojanzoo-2.0.1/docs/source/images/logo/trojanzoo-logo-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo.svg` & `trojanzoo-2.0.1/docs/source/images/logo/trojanzoo-logo.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/screenshot.png` & `trojanzoo-2.0.1/docs/source/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/trojanvision/center_cropped.png` & `trojanzoo-2.0.1/docs/source/images/trojanvision/center_cropped.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/trojanvision/grad_cam.png` & `trojanzoo-2.0.1/docs/source/images/trojanvision/grad_cam.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/trojanvision/grad_cam_impose.png` & `trojanzoo-2.0.1/docs/source/images/trojanvision/grad_cam_impose.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/trojanvision/saliency_map.png` & `trojanzoo-2.0.1/docs/source/images/trojanvision/saliency_map.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/trojanvision/saliency_map_impose.png` & `trojanzoo-2.0.1/docs/source/images/trojanvision/saliency_map_impose.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/images/trojanzoo-logo-readme.svg` & `trojanzoo-2.0.1/docs/source/images/trojanzoo-logo-readme.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/docs/source/tutorials/basic.rst` & `trojanzoo-2.0.1/docs/source/tutorials/basic.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/adv_attack.py` & `trojanzoo-2.0.1/examples/adv_attack.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/adv_defense.py` & `trojanzoo-2.0.1/examples/adv_defense.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/adv_validate.py` & `trojanzoo-2.0.1/examples/adv_validate.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/backdoor_attack.py` & `trojanzoo-2.0.1/examples/backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/backdoor_defense.py` & `trojanzoo-2.0.1/examples/backdoor_defense.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/backdoor_validate.py` & `trojanzoo-2.0.1/examples/backdoor_validate.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/heatmap.py` & `trojanzoo-2.0.1/examples/heatmap.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/train.py` & `trojanzoo-2.0.1/examples/train.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/examples/validate.py` & `trojanzoo-2.0.1/examples/validate.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/setup.cfg` & `trojanzoo-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	matplotlib>=3.4.2
 	scikit-image>=0.19.2
 	scikit-learn>=0.24.0
 	scipy>=1.5.4
 	pyyaml>=5.3.1
 	pandas>=1.1.5
 	tqdm>=4.54.1
-python_requires = >=3.10
+python_requires = >=3.11
 
 [options.package_data]
 * = *.yml
 trojanvision = data/*/*, marks/*.png
 
 [options.packages.find]
 include = trojan*
```

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/__init__.py` & `trojanzoo-2.0.1/trojanvision/attacks/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/abstract.py` & `trojanzoo-2.0.1/trojanvision/attacks/abstract.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/clean_label.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/clean_label.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/invisible_poison.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/invisible_poison.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/label_consistent.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/label_consistent.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/refool.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/clean_label/refool.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/dynamic/input_aware_dynamic.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/dynamic/input_aware_dynamic.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/badnet.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/badnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/imc.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/imc.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/latent_backdoor.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/latent_backdoor.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/trojannet.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/trojannet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/trojannn.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/normal/trojannn.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/backdoor/others/unlearn.py` & `trojanzoo-2.0.1/trojanvision/attacks/backdoor/others/unlearn.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/poison/imc_poison.py` & `trojanzoo-2.0.1/trojanvision/attacks/poison/imc_poison.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/poison/poison_basic.py` & `trojanzoo-2.0.1/trojanvision/attacks/poison/poison_basic.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/attacks/poison/poison_random.py` & `trojanzoo-2.0.1/trojanvision/attacks/poison/poison_random.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/configs/__init__.py` & `trojanzoo-2.0.1/trojanvision/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/data/cub200/test.txt` & `trojanzoo-2.0.1/trojanvision/data/cub200/test.txt`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/data/cub200/train.txt` & `trojanzoo-2.0.1/trojanvision/data/cub200/train.txt`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/data/cub200_2011/images.txt` & `trojanzoo-2.0.1/trojanvision/data/cub200_2011/images.txt`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/data/cub200_2011/train_test_split.txt` & `trojanzoo-2.0.1/trojanvision/data/cub200_2011/train_test_split.txt`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/data/isic2018/train.csv` & `trojanzoo-2.0.1/trojanvision/data/isic2018/train.csv`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/data/isic2018/valid.csv` & `trojanzoo-2.0.1/trojanvision/data/isic2018/valid.csv`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/data/refool/insert_reflection.py` & `trojanzoo-2.0.1/trojanvision/data/refool/insert_reflection.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/data/stl10/unlabeled_y.bin` & `trojanzoo-2.0.1/trojanvision/data/stl10/unlabeled_y.bin`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/__init__.py` & `trojanzoo-2.0.1/trojanvision/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/folder/__init__.py` & `trojanzoo-2.0.1/trojanvision/datasets/folder/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/folder/cub200.py` & `trojanzoo-2.0.1/trojanvision/datasets/folder/cub200.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/folder/gtsrb.py` & `trojanzoo-2.0.1/trojanvision/datasets/folder/gtsrb.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/folder/imagenet.py` & `trojanzoo-2.0.1/trojanvision/datasets/folder/imagenet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/folder/isic.py` & `trojanzoo-2.0.1/trojanvision/datasets/folder/isic.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/folder/vggface2.py` & `trojanzoo-2.0.1/trojanvision/datasets/folder/vggface2.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/imagefolder.py` & `trojanzoo-2.0.1/trojanvision/datasets/imagefolder.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/imageset.py` & `trojanzoo-2.0.1/trojanvision/datasets/imageset.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/normal/__init__.py` & `trojanzoo-2.0.1/trojanvision/datasets/normal/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/normal/celeba.py` & `trojanzoo-2.0.1/trojanvision/datasets/normal/celeba.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/normal/cifar.py` & `trojanzoo-2.0.1/trojanvision/datasets/normal/cifar.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/normal/downsampled_imagenet.py` & `trojanzoo-2.0.1/trojanvision/datasets/normal/downsampled_imagenet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/normal/mnist.py` & `trojanzoo-2.0.1/trojanvision/datasets/normal/mnist.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/datasets/normal/stl10.py` & `trojanzoo-2.0.1/trojanvision/datasets/normal/stl10.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/__init__.py` & `trojanzoo-2.0.1/trojanvision/defenses/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/abstract.py` & `trojanzoo-2.0.1/trojanvision/defenses/abstract.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/adv/advmind.py` & `trojanzoo-2.0.1/trojanvision/defenses/adv/advmind.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/adv/curvature.py` & `trojanzoo-2.0.1/trojanvision/defenses/adv/curvature.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/adv/grad_train.py` & `trojanzoo-2.0.1/trojanvision/defenses/adv/grad_train.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/__init__.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/__init__.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/adv_train.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/adv_train.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/fine_pruning.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/fine_pruning.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/magnet.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/magnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/recompress.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/attack_agnostic/recompress.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/neo.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/input_filtering/neo.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/strip.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/input_filtering/strip.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/abs.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/abs.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/deep_inspect.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/deep_inspect.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/neural_cleanse.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/neural_cleanse.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/neuron_inspect.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/neuron_inspect.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/tabor.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/model_inspection/tabor.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/activation_clustering.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/training_filtering/activation_clustering.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/spectral_signature.py` & `trojanzoo-2.0.1/trojanvision/defenses/backdoor/training_filtering/spectral_signature.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/environ.py` & `trojanzoo-2.0.1/trojanvision/environ.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/__init__.py` & `trojanzoo-2.0.1/trojanvision/marks/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/apple_black.png` & `trojanzoo-2.0.1/trojanvision/marks/apple_black.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/apple_white.png` & `trojanzoo-2.0.1/trojanvision/marks/apple_white.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/square_black.png` & `trojanzoo-2.0.1/trojanvision/marks/square_black.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/square_white.png` & `trojanzoo-2.0.1/trojanvision/marks/square_white.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/tag_black.png` & `trojanzoo-2.0.1/trojanvision/marks/tag_black.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/tag_white.png` & `trojanzoo-2.0.1/trojanvision/marks/tag_white.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/watermark_black.png` & `trojanzoo-2.0.1/trojanvision/marks/watermark_black.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/marks/watermark_white.png` & `trojanzoo-2.0.1/trojanvision/marks/watermark_white.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/__init__.py` & `trojanzoo-2.0.1/trojanvision/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/imagemodel.py` & `trojanzoo-2.0.1/trojanvision/models/imagemodel.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/nas/__init__.py` & `trojanzoo-2.0.1/trojanvision/models/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/nas/darts.py` & `trojanzoo-2.0.1/trojanvision/models/nas/darts.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/nas/enas.py` & `trojanzoo-2.0.1/trojanvision/models/nas/enas.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/nas/lanet.py` & `trojanzoo-2.0.1/trojanvision/models/nas/lanet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/nas/natsbench.py` & `trojanzoo-2.0.1/trojanvision/models/nas/natsbench.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/nas/pnasnet.py` & `trojanzoo-2.0.1/trojanvision/models/nas/pnasnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/nas/proxylessnas.py` & `trojanzoo-2.0.1/trojanvision/models/nas/proxylessnas.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/normal/bit.py` & `trojanzoo-2.0.1/trojanvision/models/normal/bit.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import torch
 import torch.nn as nn
 import torch.hub
 import numpy as np
 import os
 from collections import OrderedDict
+from typing import Self
 
 
 class _BiT(_ImageModel):
     def __init__(self, name: str = 'bit-m-r50x1', **kwargs):
         model_name = name.split('_')[0].upper().replace('BIT', 'BiT').replace('X', 'x')
         _model = KNOWN_MODELS[model_name](head_size=1)
         root, head = _model.root, _model.head
@@ -160,15 +161,15 @@
                     _dict[dict_prefix + 'downsample.weight'] = weight
         _dict['features.gn.weight'] = tf2th(weights['resnet/group_norm/gamma'])
         _dict['features.gn.bias'] = tf2th(weights['resnet/group_norm/beta'])
         _dict['classifier.fc.weight'] = tf2th(weights['resnet/head/conv2d/kernel']).flatten(1)
         _dict['classifier.fc.bias'] = tf2th(weights['resnet/head/conv2d/bias'])
         return _dict
 
-    def parametrize_(self, parametrize: bool = True):
+    def parametrize_(self, parametrize: bool = True) -> Self:
         for mod in self.modules():
             if isinstance(mod, StdConv2d):
                 mod.parametrize_(parametrize)
         return self
 
     def load(self, *args, **kwargs) -> OrderedDict[str, torch.Tensor]:
         self.parametrize_(False)
```

### Comparing `trojanzoo-2.0.0/trojanvision/models/normal/dla.py` & `trojanzoo-2.0.1/trojanvision/models/normal/dla.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/normal/dpn.py` & `trojanzoo-2.0.1/trojanvision/models/normal/dpn.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/normal/net.py` & `trojanzoo-2.0.1/trojanvision/models/normal/net.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/others/magnet.py` & `trojanzoo-2.0.1/trojanvision/models/others/magnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/__init__.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/alexnet.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/alexnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/densenet.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/densenet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/efficientnet.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/efficientnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/mnasnet.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/mnasnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/mobilenet.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/mobilenet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/resnet.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/resnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/shufflenetv2.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/models/torchvision/vgg.py` & `trojanzoo-2.0.1/trojanvision/models/torchvision/vgg.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/shortcut/pgd.py` & `trojanzoo-2.0.1/trojanvision/shortcut/pgd.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/trainer.py` & `trojanzoo-2.0.1/trojanvision/trainer.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/__init__.py` & `trojanzoo-2.0.1/trojanvision/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/dataset.py` & `trojanzoo-2.0.1/trojanvision/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/datasets/downsampled_imagenet.py` & `trojanzoo-2.0.1/trojanvision/utils/datasets/downsampled_imagenet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model.py` & `trojanzoo-2.0.1/trojanvision/utils/model.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/__init__.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #!/usr/bin/env python3
 
 import torch
 import torch.nn as nn
 import torch.nn.utils.parametrize as P
 
+from typing import Self
+
 
 class Std(nn.Module):
     def forward(self, X: torch.Tensor):
         v, m = torch.var_mean(X, dim=[1, 2, 3], keepdim=True, unbiased=False)
         return (X - m) / torch.sqrt(v + 1e-10)
 
 
 class StdConv2d(nn.Conv2d):
     def __init__(self, *args, parametrize: bool = True, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.parametrize = parametrize
         if parametrize:
             P.register_parametrization(self, 'weight', Std())
 
-    def parametrize_(self, parametrize: bool = True):
+    def parametrize_(self, parametrize: bool = True) -> Self:
         if parametrize:
             if not self.parametrize:
                 P.register_parametrization(self, 'weight', Std())
         elif self.parametrize:
             P.remove_parametrizations(self, 'weight')
         self.parametrize = parametrize
         return self
```

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/bit.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/bit.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/features.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/features.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/genotypes.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/genotypes.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/operations.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/operations.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/search.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/search.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/sgas.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/darts/sgas.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/dla.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/dla.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/dpn.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/dpn.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/macro.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/enas/macro.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/mutables.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/enas/mutables.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/ops.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/enas/ops.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/lanet.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/lanet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/pnasnet.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/pnasnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/resnet_ap.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/resnet_ap.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/model_archs/resnet_s.py` & `trojanzoo-2.0.1/trojanvision/utils/model_archs/resnet_s.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/sgm.py` & `trojanzoo-2.0.1/trojanvision/utils/sgm.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanvision/utils/transform.py` & `trojanzoo-2.0.1/trojanvision/utils/transform.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/attacks.py` & `trojanzoo-2.0.1/trojanzoo/attacks.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/configs/__init__.py` & `trojanzoo-2.0.1/trojanzoo/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/datasets.py` & `trojanzoo-2.0.1/trojanzoo/datasets.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/defenses.py` & `trojanzoo-2.0.1/trojanzoo/defenses.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/environ.py` & `trojanzoo-2.0.1/trojanzoo/environ.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/models.py` & `trojanzoo-2.0.1/trojanzoo/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import numpy as np
 import os
 from collections import OrderedDict
 from collections.abc import Iterable
 
 from typing import TYPE_CHECKING
 # TODO: python 3.10
-from typing import Generator, Iterator, Mapping
-from trojanzoo.configs import Config    # TODO: python 3.10
+from typing import Generator, Iterator, Mapping, Self
+from trojanzoo.configs import Config
 from trojanzoo.utils.model import ExponentialMovingAverage
 from torch.optim.optimizer import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 from torchvision.models._api import WeightsEnum
 import argparse
 from collections.abc import Callable
 if TYPE_CHECKING:
@@ -1162,55 +1162,55 @@
             depth = 1
         summary(self._model, depth=depth, verbose=verbose,
                 indent=indent + 10, **kwargs)
         prints('-' * 20, indent=indent + 10)
 
     # -------------------------------Reload---------------------------- #
 
-    def train(self, mode: bool = True):
+    def train(self, mode: bool = True) -> Self:
         r"""Sets the module in training mode.
 
         See Also:
             :any:`torch.nn.Module.train`.
         """
         self._model.train(mode=mode)
         self.model.train(mode=mode)
         return self
 
-    def eval(self):
+    def eval(self) -> Self:
         r"""Sets the module in evaluation mode.
 
         See Also:
             :any:`torch.nn.Module.eval`.
         """
         self._model.eval()
         self.model.eval()
         return self
 
-    def cpu(self):
+    def cpu(self) -> Self:
         r"""Moves all model parameters and buffers to the CPU.
 
         See Also:
             :any:`torch.nn.Module.cpu`.
         """
         self._model.cpu()
         self.model.cpu()
         return self
 
-    def cuda(self, device: None | int | torch.device = None):
+    def cuda(self, device: None | int | torch.device = None) -> Self:
         r"""Moves all model parameters and buffers to the GPU.
 
         See Also:
             :any:`torch.nn.Module.cuda`.
         """
         self._model.cuda(device=device)
         self.model.cuda(device=device)
         return self
 
-    def zero_grad(self, set_to_none: bool = False):
+    def zero_grad(self, set_to_none: bool = False) -> Self:
         r"""Sets gradients of all model parameters to zero.
 
         See Also:
             :any:`torch.nn.Module.zero_grad`.
         """
         return self._model.zero_grad(set_to_none=set_to_none)
```

### Comparing `trojanzoo-2.0.0/trojanzoo/optim/optimizer.py` & `trojanzoo-2.0.1/trojanzoo/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/optim/pgd.py` & `trojanzoo-2.0.1/trojanzoo/optim/pgd.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/optim/uname.py` & `trojanzoo-2.0.1/trojanzoo/optim/uname.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/trainer.py` & `trojanzoo-2.0.1/trojanzoo/trainer.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/data.py` & `trojanzoo-2.0.1/trojanzoo/utils/data.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/fim/ekfac.py` & `trojanzoo-2.0.1/trojanzoo/utils/fim/ekfac.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/fim/fim.py` & `trojanzoo-2.0.1/trojanzoo/utils/fim/fim.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/fim/kfac.py` & `trojanzoo-2.0.1/trojanzoo/utils/fim/kfac.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/lock.py` & `trojanzoo-2.0.1/trojanzoo/utils/lock.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/logger.py` & `trojanzoo-2.0.1/trojanzoo/utils/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import statistics
 import time
 from collections import defaultdict, deque
 from tqdm import tqdm as tqdm_class
 
 
-from typing import Generator, Iterable, TypeVar    # TODO: python 3.10
+from typing import Generator, Iterable, Self, TypeVar
 _T = TypeVar("_T")
 
 __all__ = ['SmoothedValue', 'MetricLogger', 'AverageMeter']
 
 MB = 1 << 20
 
 
@@ -50,15 +50,15 @@
     def __init__(self, name: str = '', window_size: int = None, fmt: str = '{global_avg:.3f}'):
         self.name = name
         self.deque: deque[float] = deque(maxlen=window_size)
         self.count: int = 0
         self.total: float = 0.0
         self.fmt = fmt
 
-    def update(self, value: float, n: int = 1) -> 'SmoothedValue':
+    def update(self, value: float, n: int = 1) -> Self:
         r"""Update :attr:`n` pieces of data with same :attr:`value`.
 
         .. code-block:: python
 
             self.deque.append(value)
             self.total += value * n
             self.count += n
@@ -71,15 +71,15 @@
             SmoothedValue: return ``self`` for stream usage.
         """
         self.deque.append(value)
         self.total += value * n
         self.count += n
         return self
 
-    def update_list(self, value_list: list[float]) -> 'SmoothedValue':
+    def update_list(self, value_list: list[float]) -> Self:
         r"""Update :attr:`value_list`.
 
         .. code-block:: python
 
             for value in value_list:
                 self.deque.append(value)
                 self.total += value
@@ -93,15 +93,15 @@
         """
         for value in value_list:
             self.deque.append(value)
             self.total += value
         self.count += len(value_list)
         return self
 
-    def reset(self) -> 'SmoothedValue':
+    def reset(self) -> Self:
         r"""Reset ``deque``, ``count`` and ``total`` to be empty.
 
         Returns:
             SmoothedValue: return ``self`` for stream usage.
         """
         self.deque = deque(maxlen=self.deque.maxlen)
         self.count = 0
@@ -217,30 +217,30 @@
         self.tqdm = tqdm
         self.indent = indent
 
         self.iter_time = SmoothedValue()
         self.data_time = SmoothedValue()
         self.memory = SmoothedValue(fmt='{max:.0f}')
 
-    def create_meters(self, **kwargs: str) -> 'MetricLogger':
+    def create_meters(self, **kwargs: str) -> Self:
         r"""Create meters with specific ``fmt`` in :attr:`self.meters`.
 
         ``self.meters[meter_name] = SmoothedValue(fmt=fmt)``
 
         Args:
             **kwargs: ``(meter_name: fmt)``
 
         Returns:
             MetricLogger: return ``self`` for stream usage.
         """
         for k, v in kwargs.items():
             self.meters[k] = SmoothedValue(fmt='{global_avg:.3f}' if v is None else v)
         return self
 
-    def update(self, n: int = 1, **kwargs: float) -> 'MetricLogger':
+    def update(self, n: int = 1, **kwargs: float) -> Self:
         r"""Update values to :attr:`self.meters` by calling :meth:`SmoothedValue.update()`.
 
         ``self.meters[meter_name].update(float(value), n=n)``
 
         Args:
             n (int): the number of data with same value.
             **kwargs: ``{meter_name: value}``.
@@ -248,30 +248,30 @@
         Returns:
             MetricLogger: return ``self`` for stream usage.
         """
         for k, v in kwargs.items():
             self.meters[k].update(float(v), n=n)
         return self
 
-    def update_list(self, **kwargs: list) -> 'MetricLogger':
+    def update_list(self, **kwargs: list) -> Self:
         r"""Update values to :attr:`self.meters` by calling :meth:`SmoothedValue.update_list()`.
 
         ``self.meters[meter_name].update_list(value_list)``
 
         Args:
             **kwargs: ``{meter_name: value_list}``.
 
         Returns:
             MetricLogger: return ``self`` for stream usage.
         """
         for k, v in kwargs.items():
             self.meters[k].update_list(v)
         return self
 
-    def reset(self) -> 'MetricLogger':
+    def reset(self) -> Self:
         r"""Reset meter in :attr:`self.meters` by calling :meth:`SmoothedValue.reset()`.
 
         Returns:
             MetricLogger: return ``self`` for stream usage.
         """
         for meter in self.meters.values():
             meter.reset()
```

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/memory.py` & `trojanzoo-2.0.1/trojanzoo/utils/memory.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/metric.py` & `trojanzoo-2.0.1/trojanzoo/utils/metric.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/model.py` & `trojanzoo-2.0.1/trojanzoo/utils/model.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/module/__init__.py` & `trojanzoo-2.0.1/trojanzoo/utils/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/module/param.py` & `trojanzoo-2.0.1/trojanzoo/utils/module/param.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 from trojanzoo.utils.output import prints
 
-from typing import Generic, MutableMapping, TypeVar
+from typing import Generic, MutableMapping, Self, TypeVar
 _KT = TypeVar("_KT")  # Key type.
 _VT = TypeVar("_VT")  # Value type.
 
 
 # TODO: issue 3 why need Generic
 class Module(MutableMapping[_KT, _VT], Generic[_KT, _VT]):
     r"""A dict-like class which supports attribute-like view as well.
@@ -26,15 +26,15 @@
 
     def __init__(self, *args: MutableMapping[_KT, _VT], **kwargs: _VT):
         self.__data: dict[_KT, _VT] = {}
         if len(args) == 1 and args[0] is None:
             return
         self.update(*args, **kwargs)
 
-    def update(self, *args: MutableMapping[_KT, _VT], **kwargs: _VT):
+    def update(self, *args: MutableMapping[_KT, _VT], **kwargs: _VT) -> Self:
         r"""update values.
 
         Args:
             *args: Positional dict-like arguments.
                 All keys will be merged together.
             **kwargs: Keyword arguments that compose a dict.
                 All keys will be merged together.
@@ -45,30 +45,30 @@
         args: list = list(args)     # TODO: issue 2 pylance issue
         args.append(kwargs)
         for module in args:
             self._update(module)
         return self
 
     # TODO: issue 4 dict | Module
-    def _update(self, module: MutableMapping[_KT, _VT]):
+    def _update(self, module: MutableMapping[_KT, _VT]) -> Self:
         for key, value in module.items():
             if value is None:
                 continue
             if key in self.keys() and isinstance(self[key], Module):
                 sub_module: Module = self[key]
                 sub_module.update(value)
             elif key in self.keys() and isinstance(value, Module):
                 self[key] = type(value)(self[key]).update(value)
             elif isinstance(value, Module):
                 self[key] = value.copy()
             else:
                 self[key] = value
         return self
 
-    def remove_none(self):
+    def remove_none(self) -> Self:
         r"""Remove the parameters whose values are ``None``.
 
         Returns:
             Module: return :attr:`self` for stream usage.
         """
         for key in self.__data.keys():
             if self.__data[key] is None:
@@ -79,15 +79,15 @@
         r"""Deepcopy of :attr:`self`.
 
         Returns:
             Module: return the deepcopy of :attr:`self`.
         """
         return type(self)(self)
 
-    def clear(self):
+    def clear(self) -> Self:
         r"""Remove all keys.
 
         Returns:
             Module: return :attr:`self` for stream usage.
         """
         self.__data = {}
         return self
@@ -160,29 +160,29 @@
         _marker (str): The marker of the class,
             which is shown in ``str(self)``.
             Defaults to ``'P'``.
         default (Any): The default value of unknown keys.
     """
     _marker = 'P'
 
-    def update(self, *args: dict[_KT, _VT], **kwargs: _VT):
+    def update(self, *args: dict[_KT, _VT], **kwargs: _VT) -> Self:
         if len(kwargs) == 0 and len(args) == 1 and \
                 not isinstance(args[0], (dict, Module)):
             self.default = args[0]
             return self
         return super().update(*args, **kwargs)
 
-    def _update(self, module: dict[_KT, _VT]):
+    def _update(self, module: dict[_KT, _VT]) -> Self:
         for key, value in module.items():
             if key == 'default':
                 self.default = value
         super()._update(module)
         return self     # For linting purpose
 
-    def remove_none(self):
+    def remove_none(self) -> Self:
         for key in list(self.__data.keys()):
             if self.__data[key] is None and \
                     not (isinstance(key, str) and key == 'default'):
                 del self.__data[key]
         return self
 
     def __getattr__(self, name: str) -> _VT:
@@ -197,11 +197,11 @@
         if key not in self.keys():
             key = 'default'
             if 'default' not in self.keys():
                 print(self)
                 raise KeyError(key)
         return super().__getitem__(key)
 
-    def clear(self):
+    def clear(self) -> Self:
         super().clear()
         self.default = None
         return self
```

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/module/process.py` & `trojanzoo-2.0.1/trojanzoo/utils/module/process.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/ntk/__init__.py` & `trojanzoo-2.0.1/trojanzoo/utils/ntk/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/output.py` & `trojanzoo-2.0.1/trojanzoo/utils/output.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/tensor.py` & `trojanzoo-2.0.1/trojanzoo/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo/utils/train.py` & `trojanzoo-2.0.1/trojanzoo/utils/train.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-2.0.0/trojanzoo.egg-info/PKG-INFO` & `trojanzoo-2.0.1/trojanzoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo
-Version: 2.0.0
+Version: 2.0.1
 Summary: a universal pytorch platform to conduct security researches
 Home-page: https://github.com/ain-soph/trojanzoo
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Keywords: pytorch,image classification,backdoor attack/defense
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
@@ -12,25 +12,25 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TrojanZoo
 ![logo](https://github.com/ain-soph/trojanzoo/raw/main/docs/source/images/trojanzoo-logo-readme.svg)
 
 [![contact](https://img.shields.io/badge/contact-rbp5354@psu.edu-yellow)](mailto:rbp5354@psu.edu)
 [![License](https://img.shields.io/github/license/ain-soph/trojanzoo)](https://opensource.org/licenses/GPL-3.0)
 
-![python>=3.10](https://img.shields.io/badge/python->=3.10-informational.svg)
+![python>=3.11](https://img.shields.io/badge/python->=3.11-informational.svg)
 [![docs](https://github.com/ain-soph/trojanzoo/workflows/docs/badge.svg)](https://ain-soph.github.io/trojanzoo/)
 
 [![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo)](https://github.com/ain-soph/trojanzoo/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo)](https://pypi.org/project/trojanzoo/)
 [![docker](https://img.shields.io/pypi/v/trojanzoo?label=docker)](https://hub.docker.com/r/local0state/trojanzoo)
 <!-- [![conda](https://img.shields.io/pypi/v/trojanzoo?label=conda)](https://anaconda.org/anaconda/trojanzoo) -->
```

### Comparing `trojanzoo-2.0.0/trojanzoo.egg-info/SOURCES.txt` & `trojanzoo-2.0.1/trojanzoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

