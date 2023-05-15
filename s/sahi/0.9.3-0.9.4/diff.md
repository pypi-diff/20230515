# Comparing `tmp/sahi-0.9.3.tar.gz` & `tmp/sahi-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sahi-0.9.3.tar", last modified: Sun May  8 01:14:31 2022, max compression
+gzip compressed data, was "sahi-0.9.4.tar", last modified: Sat May 28 18:18:24 2022, max compression
```

## Comparing `sahi-0.9.3.tar` & `sahi-0.9.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:31.755852 sahi-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-05-08 01:14:22.000000 sahi-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-08 01:14:22.000000 sahi-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11701 2022-05-08 01:14:31.755852 sahi-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10833 2022-05-08 01:14:22.000000 sahi-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-05-08 01:14:22.000000 sahi-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-08 01:14:22.000000 sahi-0.9.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:31.751851 sahi-0.9.3/sahi/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22633 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    26729 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:31.751851 sahi-0.9.3/sahi/postprocess/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22111 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/postprocess/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:31.751851 sahi-0.9.3/sahi/postprocess/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/postprocess/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7758 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/postprocess/legacy/combine.py
--rw-r--r--   0 runner    (1001) docker     (121)     7409 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/postprocess/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    34382 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/predict.py
--rw-r--r--   0 runner    (1001) docker     (121)     7742 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:31.751851 sahi-0.9.3/sahi/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/scripts/coco2fiftyone.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/scripts/coco2yolov5.py
--rw-r--r--   0 runner    (1001) docker     (121)    16180 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/scripts/coco_error_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    16343 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/scripts/coco_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/scripts/predict.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/scripts/predict_fiftyone.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/scripts/slice_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)    17217 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/slicing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:31.755852 sahi-0.9.3/sahi/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    80778 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/coco.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)    20291 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/cv.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/fiftyone.py
--rw-r--r--   0 runner    (1001) docker     (121)     6729 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/mmdet.py
--rw-r--r--   0 runner    (1001) docker     (121)    14510 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/mot.py
--rw-r--r--   0 runner    (1001) docker     (121)    11097 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/shapely.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-05-08 01:14:22.000000 sahi-0.9.3/sahi/utils/yolov5.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 01:14:31.751851 sahi-0.9.3/sahi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11701 2022-05-08 01:14:31.000000 sahi-0.9.3/sahi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-05-08 01:14:31.000000 sahi-0.9.3/sahi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-08 01:14:31.000000 sahi-0.9.3/sahi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-08 01:14:31.000000 sahi-0.9.3/sahi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-08 01:14:31.000000 sahi-0.9.3/sahi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-08 01:14:31.000000 sahi-0.9.3/sahi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-08 01:14:31.755852 sahi-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-05-08 01:14:22.000000 sahi-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:24.333589 sahi-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-05-28 18:18:09.000000 sahi-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-28 18:18:09.000000 sahi-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    11780 2022-05-28 18:18:24.333589 sahi-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10912 2022-05-28 18:18:09.000000 sahi-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-05-28 18:18:09.000000 sahi-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-28 18:18:09.000000 sahi-0.9.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:24.325589 sahi-0.9.4/sahi/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22633 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26729 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:24.325589 sahi-0.9.4/sahi/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22111 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/postprocess/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:24.325589 sahi-0.9.4/sahi/postprocess/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/postprocess/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7758 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/postprocess/legacy/combine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7409 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/postprocess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35001 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7742 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:24.329589 sahi-0.9.4/sahi/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/scripts/coco2fiftyone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/scripts/coco2yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16180 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/scripts/coco_error_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16343 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/scripts/coco_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/scripts/predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/scripts/predict_fiftyone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/scripts/slice_coco.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17364 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:24.333589 sahi-0.9.4/sahi/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    80778 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/coco.py
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20291 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/cv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/fiftyone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6839 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14510 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/mot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11097 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/shapely.py
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-05-28 18:18:09.000000 sahi-0.9.4/sahi/utils/yolov5.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 18:18:24.325589 sahi-0.9.4/sahi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11780 2022-05-28 18:18:24.000000 sahi-0.9.4/sahi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-05-28 18:18:24.000000 sahi-0.9.4/sahi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-28 18:18:24.000000 sahi-0.9.4/sahi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-28 18:18:24.000000 sahi-0.9.4/sahi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-28 18:18:24.000000 sahi-0.9.4/sahi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-28 18:18:24.000000 sahi-0.9.4/sahi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-28 18:18:24.333589 sahi-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-05-28 18:18:09.000000 sahi-0.9.4/setup.py
```

### Comparing `sahi-0.9.3/LICENSE` & `sahi-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/PKG-INFO` & `sahi-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sahi
-Version: 0.9.3
+Version: 0.9.4
 Summary: A vision library for performing sliced inference on large images/small objects
 Home-page: https://github.com/obss/sahi
 Author: OBSS
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -224,31 +224,32 @@
 - Reformat with black and isort:
 
 ```bash
 black . --config pyproject.toml
 isort .
 ```
 
-
 ## <div align="center">Contributors</div>
 
 <div align="center">
 
 <a align="left" href="https://github.com/fcakyon" target="_blank">Fatih Cagatay Akyon</a>
 
 <a align="left" href="https://github.com/sinanonur" target="_blank">Sinan Onur Altinuc</a>
 
-<a align="left" href="https://github.com/kadirnar" target="_blank">Kadir Nar</a>
+<a align="left" href="https://github.com/devrimcavusoglu" target="_blank">Devrim Cavusoglu</a>
 
 <a align="left" href="https://github.com/cemilcengiz" target="_blank">Cemil Cengiz</a>
 
+<a align="left" href="https://github.com/oulcan" target="_blank">Ogulcan Eryuksel</a>
+
+<a align="left" href="https://github.com/kadirnar" target="_blank">Kadir Nar</a>
+
+<a align="left" href="https://github.com/madenburak" target="_blank">Burak Maden</a>
+
 <a align="left" href="https://github.com/ssahinnkadir" target="_blank">Kadir Sahin</a>
-  
-<a align="left" href="https://github.com/devrimcavusoglu" target="_blank">Devrim Cavusoglu</a>
-  
+
 <a align="left" href="https://github.com/weiji14" target="_blank">Wei Ji</a>
-  
-<a align="left" href="https://github.com/oulcan" target="_blank">Ogulcan Eryuksel</a>
 
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sahi Version: 0.9.3 Summary: A vision library for
+Metadata-Version: 2.1 Name: sahi Version: 0.9.4 Summary: A vision library for
 performing sliced inference on large images/small objects Home-page: https://
 github.com/obss/sahi Author: OBSS License: MIT Platform: UNKNOWN Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -109,9 +109,9 @@
 21ecb285aa6bf93c2a00605dfb9b138f19d8d62d/sahi/model.py#L177) or [YOLOv5
 wrapper](https://github.com/obss/sahi/blob/
 21ecb285aa6bf93c2a00605dfb9b138f19d8d62d/sahi/model.py#L388) as a reference.
 Before opening a PR: - Install required development packages: ```bash pip
 install -e ."[dev]" ``` - Reformat with black and isort: ```bash black . --
 config pyproject.toml isort . ``` ##
                                  Contributors
-   Fatih_Cagatay_Akyon Sinan_Onur_Altinuc Kadir_Nar Cemil_Cengiz Kadir_Sahin
-                   Devrim_Cavusoglu Wei_Ji Ogulcan_Eryuksel
+ Fatih_Cagatay_Akyon Sinan_Onur_Altinuc Devrim_Cavusoglu Cemil_Cengiz Ogulcan
+               Eryuksel Kadir_Nar Burak_Maden Kadir_Sahin Wei_Ji
```

### Comparing `sahi-0.9.3/README.md` & `sahi-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -200,29 +200,30 @@
 - Reformat with black and isort:
 
 ```bash
 black . --config pyproject.toml
 isort .
 ```
 
-
 ## <div align="center">Contributors</div>
 
 <div align="center">
 
 <a align="left" href="https://github.com/fcakyon" target="_blank">Fatih Cagatay Akyon</a>
 
 <a align="left" href="https://github.com/sinanonur" target="_blank">Sinan Onur Altinuc</a>
 
-<a align="left" href="https://github.com/kadirnar" target="_blank">Kadir Nar</a>
+<a align="left" href="https://github.com/devrimcavusoglu" target="_blank">Devrim Cavusoglu</a>
 
 <a align="left" href="https://github.com/cemilcengiz" target="_blank">Cemil Cengiz</a>
 
+<a align="left" href="https://github.com/oulcan" target="_blank">Ogulcan Eryuksel</a>
+
+<a align="left" href="https://github.com/kadirnar" target="_blank">Kadir Nar</a>
+
+<a align="left" href="https://github.com/madenburak" target="_blank">Burak Maden</a>
+
 <a align="left" href="https://github.com/ssahinnkadir" target="_blank">Kadir Sahin</a>
-  
-<a align="left" href="https://github.com/devrimcavusoglu" target="_blank">Devrim Cavusoglu</a>
-  
+
 <a align="left" href="https://github.com/weiji14" target="_blank">Wei Ji</a>
-  
-<a align="left" href="https://github.com/oulcan" target="_blank">Ogulcan Eryuksel</a>
 
 </div>
```

#### html2text {}

```diff
@@ -97,9 +97,9 @@
 21ecb285aa6bf93c2a00605dfb9b138f19d8d62d/sahi/model.py#L177) or [YOLOv5
 wrapper](https://github.com/obss/sahi/blob/
 21ecb285aa6bf93c2a00605dfb9b138f19d8d62d/sahi/model.py#L388) as a reference.
 Before opening a PR: - Install required development packages: ```bash pip
 install -e ."[dev]" ``` - Reformat with black and isort: ```bash black . --
 config pyproject.toml isort . ``` ##
                                  Contributors
-   Fatih_Cagatay_Akyon Sinan_Onur_Altinuc Kadir_Nar Cemil_Cengiz Kadir_Sahin
-                   Devrim_Cavusoglu Wei_Ji Ogulcan_Eryuksel
+ Fatih_Cagatay_Akyon Sinan_Onur_Altinuc Devrim_Cavusoglu Cemil_Cengiz Ogulcan
+               Eryuksel Kadir_Nar Burak_Maden Kadir_Sahin Wei_Ji
```

### Comparing `sahi-0.9.3/sahi/annotation.py` & `sahi-0.9.4/sahi/annotation.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/cli.py` & `sahi-0.9.4/sahi/cli.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/model.py` & `sahi-0.9.4/sahi/model.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/postprocess/combine.py` & `sahi-0.9.4/sahi/postprocess/combine.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/postprocess/legacy/combine.py` & `sahi-0.9.4/sahi/postprocess/legacy/combine.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/postprocess/utils.py` & `sahi-0.9.4/sahi/postprocess/utils.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/predict.py` & `sahi-0.9.4/sahi/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     overlap_width_ratio: float = 0.2,
     perform_standard_pred: bool = True,
     postprocess_type: str = "GREEDYNMM",
     postprocess_match_metric: str = "IOS",
     postprocess_match_threshold: float = 0.5,
     postprocess_class_agnostic: bool = False,
     verbose: int = 1,
+    merge_buffer_length: int = None,
 ) -> PredictionResult:
     """
     Function for slice image + get predicion for each slice + combine predictions in full image.
 
     Args:
         image: str or np.ndarray
             Location of image or numpy image matrix to slice
@@ -175,14 +176,18 @@
             postprocessed after sliced prediction.
         postprocess_class_agnostic: bool
             If True, postprocess will ignore category ids.
         verbose: int
             0: no print
             1: print number of slices (default)
             2: print number of slices and slice/prediction durations
+        merge_buffer_length: int
+            The length of buffer for slices to be used during sliced prediction, which is suitable for low memory.
+            It may affect the AP if it is specified. The higher the amount, the closer results to the non-buffered.
+            scenario. See [the discussion](https://github.com/obss/sahi/pull/445).
 
     Returns:
         A Dict with fields:
             object_prediction_list: a list of sahi.prediction.ObjectPrediction
             durations_in_seconds: a dict containing elapsed times for profiling
     """
     if image_size is not None:
@@ -246,29 +251,31 @@
                 slice_image_result.original_image_width,
             ],
         )
         # convert sliced predictions to full predictions
         for object_prediction in prediction_result.object_prediction_list:
             if object_prediction:  # if not empty
                 object_prediction_list.append(object_prediction.get_shifted_object_prediction())
+
+        # merge matching predictions during sliced prediction
+        if merge_buffer_length is not None and len(object_prediction_list) > merge_buffer_length:
+            object_prediction_list = postprocess(object_prediction_list)
+
     # perform standard prediction
     if num_slices > 1 and perform_standard_pred:
         prediction_result = get_prediction(
             image=image,
             detection_model=detection_model,
             image_size=image_size,
             shift_amount=[0, 0],
             full_shape=None,
             postprocess=None,
         )
         object_prediction_list.extend(prediction_result.object_prediction_list)
 
-    time_end = time.time() - time_start
-    durations_in_seconds["prediction"] = time_end
-
     if verbose == 2:
         print(
             "Slicing performed in",
             durations_in_seconds["slice"],
             "seconds.",
         )
         print(
@@ -277,14 +284,17 @@
             "seconds.",
         )
 
     # merge matching predictions
     if len(object_prediction_list) > 1:
         object_prediction_list = postprocess(object_prediction_list)
 
+    time_end = time.time() - time_start
+    durations_in_seconds["prediction"] = time_end
+
     return PredictionResult(
         image=image, object_prediction_list=object_prediction_list, durations_in_seconds=durations_in_seconds
     )
 
 
 def predict(
     detection_model: DetectionModel = None,
```

### Comparing `sahi-0.9.3/sahi/prediction.py` & `sahi-0.9.4/sahi/prediction.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/scripts/coco2fiftyone.py` & `sahi-0.9.4/sahi/scripts/coco2fiftyone.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/scripts/coco2yolov5.py` & `sahi-0.9.4/sahi/scripts/coco2yolov5.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/scripts/coco_error_analysis.py` & `sahi-0.9.4/sahi/scripts/coco_error_analysis.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/scripts/coco_evaluation.py` & `sahi-0.9.4/sahi/scripts/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/scripts/slice_coco.py` & `sahi-0.9.4/sahi/scripts/slice_coco.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/slicing.py` & `sahi-0.9.4/sahi/slicing.py`

 * *Files 3% similar despite different names*

```diff
@@ -304,20 +304,25 @@
 
     t0 = time.time()
     n_ims = 0
 
     # init images and annotations lists
     sliced_image_result = SliceImageResult(original_image_size=[image_height, image_width], image_dir=output_dir)
 
+    image_pil_arr = np.asarray(image_pil)
     # iterate over slices
     for slice_bbox in slice_bboxes:
         n_ims += 1
 
         # extract image
-        image_pil_slice = image_pil.crop(slice_bbox)
+        tlx = slice_bbox[0]
+        tly = slice_bbox[1]
+        brx = slice_bbox[2]
+        bry = slice_bbox[3]
+        image_pil_slice = image_pil_arr[tly:bry, tlx:brx]
 
         # process annotations if coco_annotations is given
         if coco_annotation_list is not None:
             sliced_coco_annotation_list = process_coco_annotations(coco_annotation_list, slice_bbox, min_area_ratio)
 
         # set image file suffixes
         slice_suffixes = "_".join(map(str, slice_bbox))
@@ -340,15 +345,15 @@
         # append coco annotations (if present) to coco image
         if coco_annotation_list:
             for coco_annotation in sliced_coco_annotation_list:
                 coco_image.add_annotation(coco_annotation)
 
         # create sliced image and append to sliced_image_result
         sliced_image = SlicedImage(
-            image=np.asarray(image_pil_slice),
+            image=image_pil_slice,
             coco_image=coco_image,
             starting_pixel=[slice_bbox[0], slice_bbox[1]],
         )
         sliced_image_result.add_sliced_image(sliced_image)
 
     # export slices if output directory is provided
     if output_file_name and output_dir:
```

### Comparing `sahi-0.9.3/sahi/utils/coco.py` & `sahi-0.9.4/sahi/utils/coco.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/utils/cv.py` & `sahi-0.9.4/sahi/utils/cv.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/utils/detectron2.py` & `sahi-0.9.4/sahi/utils/detectron2.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/utils/fiftyone.py` & `sahi-0.9.4/sahi/utils/fiftyone.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/utils/file.py` & `sahi-0.9.4/sahi/utils/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,22 +51,24 @@
             return float(obj)
         elif isinstance(obj, np.ndarray):
             return obj.tolist()
         else:
             return super(NumpyEncoder, self).default(obj)
 
 
-def load_json(load_path):
+def load_json(load_path: str, encoding: str = "utf-8"):
     """
     Loads json formatted data (given as "data") from load_path
+    Encoding type can be specified with 'encoding' argument
+
     Example inputs:
         load_path: "dirname/coco.json"
     """
     # read from path
-    with open(load_path) as json_file:
+    with open(load_path, encoding=encoding) as json_file:
         data = json.load(json_file)
     return data
 
 
 def list_files(
     directory: str,
     contains: list = [".json"],
```

### Comparing `sahi-0.9.3/sahi/utils/mmdet.py` & `sahi-0.9.4/sahi/utils/mmdet.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/utils/mot.py` & `sahi-0.9.4/sahi/utils/mot.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/utils/shapely.py` & `sahi-0.9.4/sahi/utils/shapely.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/utils/torch.py` & `sahi-0.9.4/sahi/utils/torch.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi/utils/yolov5.py` & `sahi-0.9.4/sahi/utils/yolov5.py`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/sahi.egg-info/PKG-INFO` & `sahi-0.9.4/sahi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sahi
-Version: 0.9.3
+Version: 0.9.4
 Summary: A vision library for performing sliced inference on large images/small objects
 Home-page: https://github.com/obss/sahi
 Author: OBSS
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -224,31 +224,32 @@
 - Reformat with black and isort:
 
 ```bash
 black . --config pyproject.toml
 isort .
 ```
 
-
 ## <div align="center">Contributors</div>
 
 <div align="center">
 
 <a align="left" href="https://github.com/fcakyon" target="_blank">Fatih Cagatay Akyon</a>
 
 <a align="left" href="https://github.com/sinanonur" target="_blank">Sinan Onur Altinuc</a>
 
-<a align="left" href="https://github.com/kadirnar" target="_blank">Kadir Nar</a>
+<a align="left" href="https://github.com/devrimcavusoglu" target="_blank">Devrim Cavusoglu</a>
 
 <a align="left" href="https://github.com/cemilcengiz" target="_blank">Cemil Cengiz</a>
 
+<a align="left" href="https://github.com/oulcan" target="_blank">Ogulcan Eryuksel</a>
+
+<a align="left" href="https://github.com/kadirnar" target="_blank">Kadir Nar</a>
+
+<a align="left" href="https://github.com/madenburak" target="_blank">Burak Maden</a>
+
 <a align="left" href="https://github.com/ssahinnkadir" target="_blank">Kadir Sahin</a>
-  
-<a align="left" href="https://github.com/devrimcavusoglu" target="_blank">Devrim Cavusoglu</a>
-  
+
 <a align="left" href="https://github.com/weiji14" target="_blank">Wei Ji</a>
-  
-<a align="left" href="https://github.com/oulcan" target="_blank">Ogulcan Eryuksel</a>
 
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sahi Version: 0.9.3 Summary: A vision library for
+Metadata-Version: 2.1 Name: sahi Version: 0.9.4 Summary: A vision library for
 performing sliced inference on large images/small objects Home-page: https://
 github.com/obss/sahi Author: OBSS License: MIT Platform: UNKNOWN Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -109,9 +109,9 @@
 21ecb285aa6bf93c2a00605dfb9b138f19d8d62d/sahi/model.py#L177) or [YOLOv5
 wrapper](https://github.com/obss/sahi/blob/
 21ecb285aa6bf93c2a00605dfb9b138f19d8d62d/sahi/model.py#L388) as a reference.
 Before opening a PR: - Install required development packages: ```bash pip
 install -e ."[dev]" ``` - Reformat with black and isort: ```bash black . --
 config pyproject.toml isort . ``` ##
                                  Contributors
-   Fatih_Cagatay_Akyon Sinan_Onur_Altinuc Kadir_Nar Cemil_Cengiz Kadir_Sahin
-                   Devrim_Cavusoglu Wei_Ji Ogulcan_Eryuksel
+ Fatih_Cagatay_Akyon Sinan_Onur_Altinuc Devrim_Cavusoglu Cemil_Cengiz Ogulcan
+               Eryuksel Kadir_Nar Burak_Maden Kadir_Sahin Wei_Ji
```

### Comparing `sahi-0.9.3/sahi.egg-info/SOURCES.txt` & `sahi-0.9.4/sahi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sahi-0.9.3/setup.py` & `sahi-0.9.4/setup.py`

 * *Files identical despite different names*

