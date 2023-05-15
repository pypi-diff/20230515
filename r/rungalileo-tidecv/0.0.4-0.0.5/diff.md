# Comparing `tmp/rungalileo-tidecv-0.0.4.tar.gz` & `tmp/rungalileo-tidecv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rungalileo-tidecv-0.0.4.tar", last modified: Wed May  3 16:30:01 2023, max compression
+gzip compressed data, was "rungalileo-tidecv-0.0.5.tar", last modified: Mon May 15 17:21:02 2023, max compression
```

## Comparing `rungalileo-tidecv-0.0.4.tar` & `rungalileo-tidecv-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-03 16:30:01.252567 rungalileo-tidecv-0.0.4/
--rw-r--r--   0 benepstein   (501) staff       (20)     1055 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.4/LICENSE
--rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-05-03 16:30:01.252232 rungalileo-tidecv-0.0.4/PKG-INFO
--rw-r--r--   0 benepstein   (501) staff       (20)     3431 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.4/README.md
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-03 16:30:01.242320 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/
--rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/PKG-INFO
--rw-r--r--   0 benepstein   (501) staff       (20)      434 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/SOURCES.txt
--rw-r--r--   0 benepstein   (501) staff       (20)        1 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/dependency_links.txt
--rw-r--r--   0 benepstein   (501) staff       (20)       33 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/requires.txt
--rw-r--r--   0 benepstein   (501) staff       (20)        7 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/top_level.txt
--rw-r--r--   0 benepstein   (501) staff       (20)       38 2023-05-03 16:30:01.252698 rungalileo-tidecv-0.0.4/setup.cfg
--rw-r--r--   0 benepstein   (501) staff       (20)     1214 2023-05-03 16:28:29.000000 rungalileo-tidecv-0.0.4/setup.py
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-03 16:30:01.248431 rungalileo-tidecv-0.0.4/tidecv/
--rw-r--r--   0 benepstein   (501) staff       (20)      103 2023-05-03 16:28:43.000000 rungalileo-tidecv-0.0.4/tidecv/__init__.py
--rw-r--r--   0 benepstein   (501) staff       (20)    11096 2023-05-03 16:29:39.000000 rungalileo-tidecv-0.0.4/tidecv/ap.py
--rw-r--r--   0 benepstein   (501) staff       (20)     4733 2023-04-13 14:56:12.000000 rungalileo-tidecv-0.0.4/tidecv/data.py
--rw-r--r--   0 benepstein   (501) staff       (20)    11375 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.4/tidecv/datasets.py
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-03 16:30:01.251300 rungalileo-tidecv-0.0.4/tidecv/errors/
--rw-r--r--   0 benepstein   (501) staff       (20)     2927 2023-04-05 13:33:29.000000 rungalileo-tidecv-0.0.4/tidecv/errors/error.py
--rw-r--r--   0 benepstein   (501) staff       (20)     3081 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.4/tidecv/errors/main_errors.py
--rw-r--r--   0 benepstein   (501) staff       (20)     1329 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.4/tidecv/errors/qualifiers.py
--rw-r--r--   0 benepstein   (501) staff       (20)     3010 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.4/tidecv/functions.py
--rw-r--r--   0 benepstein   (501) staff       (20)     1116 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.4/tidecv/plotting.py
--rw-r--r--   0 benepstein   (501) staff       (20)    27034 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.4/tidecv/quantify.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-15 17:21:02.941452 rungalileo-tidecv-0.0.5/
+-rw-r--r--   0 benepstein   (501) staff       (20)     1055 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.5/LICENSE
+-rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-05-15 17:21:02.941082 rungalileo-tidecv-0.0.5/PKG-INFO
+-rw-r--r--   0 benepstein   (501) staff       (20)     3431 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.5/README.md
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-15 17:21:02.915749 rungalileo-tidecv-0.0.5/rungalileo_tidecv.egg-info/
+-rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-05-15 17:21:02.000000 rungalileo-tidecv-0.0.5/rungalileo_tidecv.egg-info/PKG-INFO
+-rw-r--r--   0 benepstein   (501) staff       (20)      452 2023-05-15 17:21:02.000000 rungalileo-tidecv-0.0.5/rungalileo_tidecv.egg-info/SOURCES.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)        1 2023-05-15 17:21:02.000000 rungalileo-tidecv-0.0.5/rungalileo_tidecv.egg-info/dependency_links.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)       33 2023-05-15 17:21:02.000000 rungalileo-tidecv-0.0.5/rungalileo_tidecv.egg-info/requires.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)        7 2023-05-15 17:21:02.000000 rungalileo-tidecv-0.0.5/rungalileo_tidecv.egg-info/top_level.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)       38 2023-05-15 17:21:02.941578 rungalileo-tidecv-0.0.5/setup.cfg
+-rw-r--r--   0 benepstein   (501) staff       (20)     1214 2023-05-15 17:20:22.000000 rungalileo-tidecv-0.0.5/setup.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-15 17:21:02.938317 rungalileo-tidecv-0.0.5/tidecv/
+-rw-r--r--   0 benepstein   (501) staff       (20)      103 2023-05-15 17:18:30.000000 rungalileo-tidecv-0.0.5/tidecv/__init__.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    12655 2023-05-15 17:18:30.000000 rungalileo-tidecv-0.0.5/tidecv/ap.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     4751 2023-05-15 17:18:30.000000 rungalileo-tidecv-0.0.5/tidecv/data.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    11375 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.5/tidecv/datasets.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-15 17:21:02.940394 rungalileo-tidecv-0.0.5/tidecv/errors/
+-rw-r--r--   0 benepstein   (501) staff       (20)     3437 2023-05-15 17:18:30.000000 rungalileo-tidecv-0.0.5/tidecv/errors/error.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     3081 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.5/tidecv/errors/main_errors.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     1329 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.5/tidecv/errors/qualifiers.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     3010 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.5/tidecv/functions.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     7343 2023-05-15 17:18:30.000000 rungalileo-tidecv-0.0.5/tidecv/helpers.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     1116 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.5/tidecv/plotting.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    29298 2023-05-15 17:18:30.000000 rungalileo-tidecv-0.0.5/tidecv/quantify.py
```

### Comparing `rungalileo-tidecv-0.0.4/LICENSE` & `rungalileo-tidecv-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.4/PKG-INFO` & `rungalileo-tidecv-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rungalileo-tidecv
-Version: 0.0.4
+Version: 0.0.5
 Summary: A General Toolbox for Identifying ObjectDetection Errors
 Home-page: https://github.com/rungalileo/tide
 Author: Galileo
 Author-email: galileo@rungalileo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rungalileo-tidecv-0.0.4/README.md` & `rungalileo-tidecv-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/PKG-INFO` & `rungalileo-tidecv-0.0.5/rungalileo_tidecv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rungalileo-tidecv
-Version: 0.0.4
+Version: 0.0.5
 Summary: A General Toolbox for Identifying ObjectDetection Errors
 Home-page: https://github.com/rungalileo/tide
 Author: Galileo
 Author-email: galileo@rungalileo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rungalileo-tidecv-0.0.4/setup.py` & `rungalileo-tidecv-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.4/tidecv/ap.py` & `rungalileo-tidecv-0.0.5/tidecv/ap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,74 @@
 from collections import defaultdict
+from typing import Dict
 
 import numpy as np
 from pycocotools import mask as mask_utils
 
-from . import functions as f
 from .data import Data
 
 
 class APDataObject:
     """
     Stores all the information necessary to calculate the AP for one IoU and one class.
     Note: I type annotated this because why not.
     """
 
     def __init__(self):
-        self.data_points = {}
-        self.false_negatives = set()
-        self.num_gt_positives = 0
+        self.data_points = {}  # dict with all preds (id -> data)
+        self.false_negatives = set()  # set of FN ids (i.e., not TPs, i.e., FN + Missed)
+        self.num_gt_positives = 0  # total number of GTs
         self.curve = None
 
+    def apply_qualifier_no_check(self, kept_preds: set, kept_gts: set) -> object:
+        """
+        Makes a new data object where we only keep some of the ids in the pred
+        and gt lists.
+        We make no checks and assume that the given ids are exactly what we want.
+
+        As an example we could check that given a Pred TP, we also have the
+        associated GT making it a TP, otherwise that Pred could turn into an FP
+        in the filtered data object.
+        We do not make such checks in order to avoid unexpected effects.
+        """
+        obj = APDataObject()
+
+        if not isinstance(kept_preds, set):
+            kept_preds = set(kept_preds)
+
+        # Restrict the Preds
+        obj.data_points = {
+            pred_id: pred_vals
+            for pred_id, pred_vals in self.data_points.items()
+            if pred_id in kept_preds
+        }
+
+        # Propogate the Gts
+        obj.false_negatives = self.false_negatives.intersection(kept_gts)
+        obj.num_gt_positives = len(kept_gts)
+
+        return obj
+
     def apply_qualifier(self, kept_preds: set, kept_gts: set) -> object:
-        """Makes a new data object where we remove the ids in the pred and gt lists."""
+        """
+        Makes a new data object where we remove the ids in the preds and gts.
+        """
         obj = APDataObject()
         num_gt_removed = 0
 
+        if not isinstance(kept_preds, set):
+            kept_preds = set(kept_preds)
+
         for pred_id in self.data_points:
             score, is_true, info = self.data_points[pred_id]
 
-            # If the data point we kept was a true positive, there's a corresponding ground truth
-            # If so, we should only add that positive if the corresponding ground truth has been kept
+            # If the data point we kept was a true positive, there's a
+            # corresponding ground truth.
+            # If so, we should only add that positive if the corresponding
+            # ground truth has been kept
             if is_true and info["matched_with"] not in kept_gts:
                 num_gt_removed += 1
                 continue
 
             if pred_id in kept_preds:
                 obj.data_points[pred_id] = self.data_points[pred_id]
 
@@ -122,22 +158,26 @@
 
 class ClassedAPDataObject:
     """Stores an APDataObject for each class in the dataset."""
 
     def __init__(self):
         self.objs = defaultdict(lambda: APDataObject())
 
-    def apply_qualifier(self, pred_dict: dict, gt_dict: dict) -> object:
+    def apply_qualifier(
+        self, pred_dict: dict, gt_dict: dict, check: bool = False
+    ) -> object:
         ret = ClassedAPDataObject()
 
         for _class, obj in self.objs.items():
-            pred_list = pred_dict[_class] if _class in pred_dict else set()
-            gt_list = gt_dict[_class] if _class in gt_dict else set()
-
-            ret.objs[_class] = obj.apply_qualifier(pred_list, gt_list)
+            pred_set = pred_dict.get(_class, set())
+            gt_set = gt_dict.get(_class, set())
+            if check:
+                ret.objs[_class] = obj.apply_qualifier(pred_set, gt_set)
+            else:
+                ret.objs[_class] = obj.apply_qualifier_no_check(pred_set, gt_set)
 
         return ret
 
     def push(self, class_: int, id: int, score: float, is_true: bool, info: dict = {}):
         self.objs[class_].push(id, score, is_true, info)
 
     def push_false_negative(self, class_: int, id: int):
@@ -149,14 +189,19 @@
     def get_mAP(self) -> float:
         aps = [x.get_ap() for x in self.objs.values() if not x.is_empty()]
         # If there are no objects (no golds, no preds), then it's a perfect run
         if not aps:
             return 100.0
         return sum(aps) / len(aps)
 
+    def get_APs(self) -> Dict[int, float]:
+        return {
+            cls_id: x.get_ap() for cls_id, x in self.objs.items() if not x.is_empty()
+        }
+
     def get_gt_positives(self) -> dict:
         return {k: v.num_gt_positives for k, v in self.objs.items()}
 
     def get_pr_curve(self, cat_id: int = None) -> tuple:
         if cat_id is None:
             # Average out the curves when using all categories
             curves = [x.get_pr_curve() for x in list(self.objs.values())]
@@ -222,15 +267,14 @@
         indices.sort(key=lambda i: -preds[i]["score"])
 
         classes = [x["category_id"] for x in preds]
         gt_classes = [x["category_id"] for x in gt]
         crowd_classes = [x["category_id"] for x in gt_crowd]
 
         for _class in set(classes + gt_classes):
-            ap_per_iou = []
             num_gt_for_class = sum([1 for x in gt_classes if x == _class])
 
             for iouIdx in range(len(self.iou_thresholds)):
                 iou_threshold = self.iou_thresholds[iouIdx]
 
                 gt_used = [False] * len(gt_classes)
```

### Comparing `rungalileo-tidecv-0.0.4/tidecv/data.py` & `rungalileo-tidecv-0.0.5/tidecv/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-import os
 from collections import defaultdict
 
-import numpy as np
-
-from . import functions as f
-
 
 class Data:
     """
     A class to hold ground truth or predictions data in an easy to work with format.
-    Note that any time they appear, bounding boxes are [x, y, width, height] and masks
-    are either a list of polygons or pycocotools RLEs.
+    Note that any time they appear, bounding boxes are [x, y, width, height] where
+    x,y are the coordinates of the top_left corner, and masks are either a list of
+    polygons or pycocotools RLEs.
 
     Also, don't mix ground truth with predictions. Keep them in separate data objects.
 
     'max_dets' specifies the maximum number of detections the model is allowed to output for a given image.
     """
 
     def __init__(self, name: str, max_dets: int = 100):
@@ -131,8 +127,10 @@
 
     def add_image(self, id: int, name: str):
         """Register an image name/path with an image ID."""
         self.images[id]["name"] = name
 
     def get(self, image_id: int):
         """Collects all the annotations / detections for that particular image."""
-        return [self.annotations[x] for x in self.images.get(image_id, {}).get("anns", [])]
+        return [
+            self.annotations[x] for x in self.images.get(image_id, {}).get("anns", [])
+        ]
```

### Comparing `rungalileo-tidecv-0.0.4/tidecv/datasets.py` & `rungalileo-tidecv-0.0.5/tidecv/datasets.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.4/tidecv/errors/error.py` & `rungalileo-tidecv-0.0.5/tidecv/errors/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,30 @@
                     self.pred["score"],
                     False,
                     self.pred["info"],
                 )
         else:
             return None
 
+    def is_pred(self) -> bool:
+        return hasattr(self, "pred")
+
+    def is_gt(self) -> bool:
+        return hasattr(self, "gt")
+
+    def is_contained_in(self, pred_ids: set, gt_ids: set) -> bool:
+        # check if NONe
+        if not isinstance(pred_ids, set):
+            pred_ids = set(pred_ids)
+        if not isinstance(gt_ids, set):
+            gt_ids = set(gt_ids)
+        return (
+            (self.get_id() in pred_ids) if self.is_pred() else (self.get_id() in gt_ids)
+        )
+
     def get_id(self) -> int:
         if hasattr(self, "pred"):
             return self.pred["_id"]
         elif hasattr(self, "gt"):
             return self.gt["_id"]
         else:
             return -1
```

### Comparing `rungalileo-tidecv-0.0.4/tidecv/errors/main_errors.py` & `rungalileo-tidecv-0.0.5/tidecv/errors/main_errors.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.4/tidecv/errors/qualifiers.py` & `rungalileo-tidecv-0.0.5/tidecv/errors/qualifiers.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.4/tidecv/functions.py` & `rungalileo-tidecv-0.0.5/tidecv/functions.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.4/tidecv/plotting.py` & `rungalileo-tidecv-0.0.5/tidecv/plotting.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.4/tidecv/quantify.py` & `rungalileo-tidecv-0.0.5/tidecv/quantify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from collections import OrderedDict, defaultdict
+from typing import List
 
 import numpy as np
 from pycocotools import mask as mask_utils
 
 from . import functions as f
 from . import plotting as P
 from .ap import ClassedAPDataObject
 from .data import Data
 from .errors.main_errors import *
-from .errors.qualifiers import AREA, Qualifier
+from .errors.qualifiers import Qualifier
 
 
 class TIDEExample:
     """Computes all the data needed to evaluate a set of predictions and gt for a single image."""
 
     def __init__(
         self,
@@ -158,15 +159,14 @@
         run_errors: bool = True,
     ):
         self.gt = gt
         self.preds = preds
 
         self.errors = []
         self.error_dict = {_type: [] for _type in TIDE._error_types}
-        self.TP_pred_id_to_gt_id = {}
 
         self.ap_data = ClassedAPDataObject()
         self.qualifiers = {}
 
         # A list of false negatives per class
         self.false_negatives = {_id: [] for _id in self.gt.classes}
 
@@ -239,15 +239,14 @@
         preds = ex.preds  # In case the number of predictions was restricted to the max
 
         for pred_idx, pred in enumerate(preds):
 
             pred["info"] = {"iou": pred["iou"], "used": pred["used"]}
             if pred["used"]:
                 pred["info"]["matched_with"] = pred["matched_with"]
-                self.TP_pred_id_to_gt_id[pred["_id"]] = pred["matched_with"]
 
             if pred["used"] is not None:
                 self.ap_data.push(
                     pred["class"],
                     pred["_id"],
                     pred["score"],
                     pred["used"],
@@ -322,30 +321,42 @@
     def fix_errors(
         self,
         condition=lambda x: False,
         transform=None,
         false_neg_dict: dict = None,
         ap_data: ClassedAPDataObject = None,
         disable_errors: bool = False,
+        pred_dict: dict = None,
+        gt_dict: dict = None,
     ) -> ClassedAPDataObject:
         """Returns a ClassedAPDataObject where all errors given the condition returns True are fixed."""
         if ap_data is None:
             ap_data = self.ap_data
 
+        if gt_dict:
+            gt_ids = set.union(*gt_dict.values())
+
         gt_pos = ap_data.get_gt_positives()
         new_ap_data = ClassedAPDataObject()
 
         # Potentially fix every error case
         for error in self.errors:
             if error.disabled:
                 continue
 
             _id = error.get_id()
             _cls, data_point = error.original
 
+            if (
+                pred_dict
+                and gt_dict
+                and not error.is_contained_in(pred_dict.get(_cls, {}), gt_ids)
+            ):
+                continue
+
             if condition(error):
                 _cls, data_point = error.fixed
 
                 if disable_errors:
                     error.disabled = True
 
                 # Specific for MissingError (or anything else that affects #GT)
@@ -376,31 +387,44 @@
         return new_ap_data
 
     def fix_main_errors(
         self,
         progressive: bool = False,
         error_types: list = None,
         qual: Qualifier = None,
+        pred_dict: dict = None,
+        gt_dict: dict = None,
     ) -> dict:
         ap_data = self.ap_data
-        last_ap = self.ap
+
+        # Restrict ids if given
+        pred_dict = pred_dict if pred_dict is not None else {}
+        gt_dict = gt_dict if gt_dict is not None else {}
+        if pred_dict or gt_dict:
+            ap_data = ap_data.apply_qualifier(pred_dict, gt_dict)
+            self.qualifiers["restricted_mAP"] = ap_data.get_mAP()
+            self.qualifiers["restricted_APs"] = ap_data.get_APs()
+
+        last_ap = ap_data.get_mAP()
 
         if qual is None:
             qual = Qualifier("", None)
 
         if error_types is None:
             error_types = TIDE._error_types
 
         errors = {}
 
         for error in error_types:
             _ap_data = self.fix_errors(
                 qual._make_error_func(error),
                 ap_data=ap_data,
                 disable_errors=progressive,
+                pred_dict=pred_dict,
+                gt_dict=gt_dict,
             )
 
             new_ap = _ap_data.get_mAP()
             # If an error is negative that means it's likely due to binning differences, so just
             # Ignore the negative by setting it to 0.
             errors[error] = max(new_ap - last_ap, 0)
 
@@ -686,19 +710,54 @@
                     ],
                 ],
                 title="Special Error",
             )
 
             print()
 
-    def get_main_errors(self):
+    def get_main_errors(
+        self, run_names: List[str] = None, pred_dict: dict = None, gt_dict: dict = None
+    ):
+        """
+        Calculates the error count and impact on mAP. To calculate it on a filtered version
+        of the data, specify the indexes to keep in the dicts pred_dict and gt_dict.
+
+        args:
+        - run_names: if specified, only return the specified runs
+        - pred_dict, gt_dict: dictionaries of the form cls_id -> set of ids
+            to keep. If specified, we restrict to the dataset whose ids are
+            contained in these sets and recalculate mAP, and impact on mAP
+            based on this filtered data.
+
+        returns:
+            dictionary error_type -> impact on mAP
+
+        side effects:
+            populates self.runs[run_name].qualifiers["restricted_mAP"] with new mAP
+            and self.runs[run_name].qualifiers["restricted_APs"] with AP per class
+        """
         errors = {}
 
-        for run_name, run in self.runs.items():
-            if run_name in self.run_main_errors:
+        if run_names is None:
+            run_names = list(self.runs)
+
+        for run_name in run_names:
+            run = self.runs[run_name]
+
+            if pred_dict or gt_dict:
+                run_name = f"filtered_errors_in_run_{run_name}"
+
+                # we recalculate it every time for filtered runs since we can't index by the filter.
+                errors[run_name] = {
+                    error.short_name: value
+                    for error, value in run.fix_main_errors(
+                        pred_dict=pred_dict, gt_dict=gt_dict
+                    ).items()
+                }
+            elif run_name in self.run_main_errors:
                 errors[run_name] = self.run_main_errors[run_name]
             else:
                 errors[run_name] = {
                     error.short_name: value
                     for error, value in run.fix_main_errors().items()
                 }
                 self.run_main_errors[run_name] = errors[run_name]
```

