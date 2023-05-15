# Comparing `tmp/savant_rs-0.1.3.tar.gz` & `tmp/savant_rs-0.1.4.tar.gz`

## Comparing `savant_rs-0.1.3.tar` & `savant_rs-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 savant_rs-0.1.3/Cargo.toml
--rw-r--r--   0     1001      123     1614 2023-05-14 14:45:31.000000 savant_rs-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      466 2023-05-14 14:45:31.000000 savant_rs-0.1.3/.gitignore
--rw-r--r--   0     1001      123    11357 2023-05-14 14:45:31.000000 savant_rs-0.1.3/LICENSE
--rw-r--r--   0     1001      123      514 2023-05-14 14:45:31.000000 savant_rs-0.1.3/README.md
--rw-r--r--   0     1001      123      769 2023-05-14 14:45:31.000000 savant_rs-0.1.3/benches/batch_snapshot.rs
--rw-r--r--   0     1001      123     1197 2023-05-14 14:45:31.000000 savant_rs-0.1.3/benches/message_save_load.rs
--rw-r--r--   0     1001      123       71 2023-05-14 14:45:31.000000 savant_rs-0.1.3/build.rs
--rw-r--r--   0     1001      123      459 2023-05-14 14:45:31.000000 savant_rs-0.1.3/pyproject.toml
--rw-r--r--   0     1001      123      783 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/primitives/buf_copy.py
--rw-r--r--   0     1001      123     3741 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/primitives/frame_ops.py
--rw-r--r--   0     1001      123     1108 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/primitives/polygon_match.py
--rw-r--r--   0     1001      123      200 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_copy.py
--rw-r--r--   0     1001      123      184 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_proxy.py
--rw-r--r--   0     1001      123      407 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_pure.py
--rw-r--r--   0     1001      123      196 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_py.py
--rw-r--r--   0     1001      123      213 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_take.py
--rw-r--r--   0     1001      123      269 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/utils/fps_meter/rust_fps_meter.py
--rw-r--r--   0     1001      123     3515 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/utils/fps_meter/savant_fps_meter.py
--rw-r--r--   0     1001      123     1820 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/utils/symbol_mapper/rust_symbol_mapper.py
--rw-r--r--   0     1001      123     6394 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/utils/symbol_mapper/savant_symbol_mapper.py
--rw-r--r--   0     1001      123     1018 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/lib.rs
--rw-r--r--   0     1001      123    14168 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/attribute.rs
--rw-r--r--   0     1001      123     1221 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/bbox.rs
--rw-r--r--   0     1001      123      590 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/eos.rs
--rw-r--r--   0     1001      123     2807 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/loader.rs
--rw-r--r--   0     1001      123     2141 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/saver.rs
--rw-r--r--   0     1001      123     1932 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/video/batch.rs
--rw-r--r--   0     1001      123    28694 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/video/frame.rs
--rw-r--r--   0     1001      123    14354 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/video/object.rs
--rw-r--r--   0     1001      123       46 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/video.rs
--rw-r--r--   0     1001      123     6710 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message.rs
--rw-r--r--   0     1001      123      853 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/point.rs
--rw-r--r--   0     1001      123    13870 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/polygonal_area.rs
--rw-r--r--   0     1001      123     2558 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/segment.rs
--rw-r--r--   0     1001      123       87 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/to_json_value.rs
--rw-r--r--   0     1001      123     1628 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives.rs
--rw-r--r--   0     1001      123     5856 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/test.rs
--rw-r--r--   0     1001      123     1071 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/test_rkyv_tuple.rs
--rw-r--r--   0     1001      123     2521 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/tests_pyo3_access.rs
--rw-r--r--   0     1001      123     5968 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/utils/fps_meter.rs
--rw-r--r--   0     1001      123    20581 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/utils/symbol_mapper.rs
--rw-r--r--   0     1001      123     1818 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/utils.rs
--rw-r--r--   0     1001      123    36647 2023-05-14 14:46:46.000000 savant_rs-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 savant_rs-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      123     1614 2023-05-15 12:21:03.000000 savant_rs-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      466 2023-05-15 12:21:03.000000 savant_rs-0.1.4/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-05-15 12:21:03.000000 savant_rs-0.1.4/LICENSE
+-rw-r--r--   0     1001      123      514 2023-05-15 12:21:03.000000 savant_rs-0.1.4/README.md
+-rw-r--r--   0     1001      123      769 2023-05-15 12:21:03.000000 savant_rs-0.1.4/benches/batch_snapshot.rs
+-rw-r--r--   0     1001      123     1197 2023-05-15 12:21:03.000000 savant_rs-0.1.4/benches/message_save_load.rs
+-rw-r--r--   0     1001      123       71 2023-05-15 12:21:03.000000 savant_rs-0.1.4/build.rs
+-rw-r--r--   0     1001      123      459 2023-05-15 12:21:03.000000 savant_rs-0.1.4/pyproject.toml
+-rw-r--r--   0     1001      123     1790 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/bbox/ops.py
+-rw-r--r--   0     1001      123     2533 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/bbox/savant_scale.py
+-rw-r--r--   0     1001      123      783 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/buf_copy.py
+-rw-r--r--   0     1001      123     3741 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/frame_ops.py
+-rw-r--r--   0     1001      123     1108 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/polygon_match.py
+-rw-r--r--   0     1001      123      200 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_copy.py
+-rw-r--r--   0     1001      123      184 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_proxy.py
+-rw-r--r--   0     1001      123      407 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_pure.py
+-rw-r--r--   0     1001      123      196 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_py.py
+-rw-r--r--   0     1001      123      213 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_take.py
+-rw-r--r--   0     1001      123      269 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/utils/fps_meter/rust_fps_meter.py
+-rw-r--r--   0     1001      123     3515 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/utils/fps_meter/savant_fps_meter.py
+-rw-r--r--   0     1001      123     3386 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/utils/symbol_mapper/rust_symbol_mapper.py
+-rw-r--r--   0     1001      123     7226 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/utils/symbol_mapper/savant_symbol_mapper.py
+-rw-r--r--   0     1001      123     1018 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      123    14160 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/attribute.rs
+-rw-r--r--   0     1001      123    15513 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/bbox.rs
+-rw-r--r--   0     1001      123     1141 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/eos.rs
+-rw-r--r--   0     1001      123     2807 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/loader.rs
+-rw-r--r--   0     1001      123     2141 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/saver.rs
+-rw-r--r--   0     1001      123     1932 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/video/batch.rs
+-rw-r--r--   0     1001      123    28830 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/video/frame.rs
+-rw-r--r--   0     1001      123    14359 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/video/object.rs
+-rw-r--r--   0     1001      123       46 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/video.rs
+-rw-r--r--   0     1001      123     6710 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message.rs
+-rw-r--r--   0     1001      123      853 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/point.rs
+-rw-r--r--   0     1001      123    13870 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/polygonal_area.rs
+-rw-r--r--   0     1001      123     2558 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/segment.rs
+-rw-r--r--   0     1001      123       87 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/to_json_value.rs
+-rw-r--r--   0     1001      123     1678 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives.rs
+-rw-r--r--   0     1001      123     5863 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/test.rs
+-rw-r--r--   0     1001      123     1071 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/test_rkyv_tuple.rs
+-rw-r--r--   0     1001      123     2521 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/tests_pyo3_access.rs
+-rw-r--r--   0     1001      123        1 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/utils/bounding_box.rs
+-rw-r--r--   0     1001      123     5961 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/utils/fps_meter.rs
+-rw-r--r--   0     1001      123    21129 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/utils/symbol_mapper.rs
+-rw-r--r--   0     1001      123     2011 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/utils.rs
+-rw-r--r--   0     1001      123    36647 2023-05-15 12:22:28.000000 savant_rs-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.4/PKG-INFO
```

### Comparing `savant_rs-0.1.3/Cargo.toml` & `savant_rs-0.1.4/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "savant_rs"
-version = "0.1.3"
+version = "0.1.4"
 edition = "2021"
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Savant rust optimization library"
 homepage = "https://github.com/insight-platform/savant-rs"
 repository = "https://github.com/insight-platform/savant-rs"
 readme = "README.md"
 keywords = ["computer-vision", "video-processing"]
```

### Comparing `savant_rs-0.1.3/.github/workflows/CI.yml` & `savant_rs-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/LICENSE` & `savant_rs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/README.md` & `savant_rs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/benches/batch_snapshot.rs` & `savant_rs-0.1.4/benches/batch_snapshot.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/benches/message_save_load.rs` & `savant_rs-0.1.4/benches/message_save_load.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/python/primitives/buf_copy.py` & `savant_rs-0.1.4/python/primitives/buf_copy.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/python/primitives/frame_ops.py` & `savant_rs-0.1.4/python/primitives/frame_ops.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/python/primitives/polygon_match.py` & `savant_rs-0.1.4/python/primitives/polygon_match.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/python/utils/fps_meter/savant_fps_meter.py` & `savant_rs-0.1.4/python/utils/fps_meter/savant_fps_meter.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/python/utils/symbol_mapper/savant_symbol_mapper.py` & `savant_rs-0.1.4/python/utils/symbol_mapper/savant_symbol_mapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Thread-safe singleton metaclass."""
+import threading
 from random import random
 from threading import Lock
 from typing import Any, Dict, List, Tuple, Optional
+from numba import jit
 
 
 class SingletonMeta(type):
     """Thread-safe singleton metaclass."""
 
     def __new__(cls, name, bases, attrs):
         # Assume the target class is created
@@ -155,26 +157,60 @@
 
 if __name__ == '__main__':
     from timeit import default_timer as timer
     from random import choice
     registry = ModelObjectRegistry()
     models = ["model1", "model2", "model3", "model4", "model5", "model6", "model7", "model8", "model9", "model10"]
 
+
+    @jit(nopython=True, nogil=True)
+    def plus_one() -> int:
+        return 1
+
+
+    cntr = 0
+    exit_flag = False
+
+
+    def threaded_count():
+        global cntr, exit_flag
+        while not exit_flag:
+            cntr += plus_one()
+
+    t = timer()
+    cnt = 0
+    while cnt < 1000_000:
+        cnt += plus_one()
+
+    mil_count = timer() - t
+    print(f"Time to count to million: {mil_count}")
+
     res = 0
     for m in models:
         d = dict([(id, f"object_{id}_{m}") for id in range(1000)])
         t = timer()
         registry.register_model(m, d)
         res += timer() - t
 
     print(f"Time to register: {res}")
 
-    res = 0
-    for _ in range(1000_000):
-        random_model = choice(models)
-        random_object = f"object_{choice(range(1000))}_{random_model}"
-        t = timer()
-        m = registry.get_model_uid(random_model)
-        m, o = registry.get_model_object_ids(model_name=random_model, object_label=random_object)
-        res += timer() - t
-
-    print(f"Time to get: {res}")
+    def simple_count():
+        res = 0
+        total_time = timer()
+        for _ in range(1000_000):
+            random_model = choice(models)
+            random_object = f"object_{choice(range(1000))}_{random_model}"
+            t = timer()
+            m = registry.get_model_uid(random_model)
+            m, o = registry.get_model_object_ids(model_name=random_model, object_label=random_object)
+            res += timer() - t
+        return res, timer() - total_time
+
+
+    cntr = 0
+    exit_flag = False
+    t = threading.Thread(target=threaded_count)
+    t.start()
+    res, total_time = simple_count()
+    exit_flag = True
+    t.join()
+    print(f"Time to get in individually ({total_time}): {res}, cnt: {cntr}, time spent in counter {cntr / 1_000_000 * mil_count}")
```

### Comparing `savant_rs-0.1.3/src/lib.rs` & `savant_rs-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/primitives/attribute.rs` & `savant_rs-0.1.4/src/primitives/attribute.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use crate::primitives::to_json_value::ToSerdeJsonValue;
-use crate::primitives::{BBox, Intersection, Point, PolygonalArea};
+use crate::primitives::{Intersection, Point, PolygonalArea, RBBox};
 use pyo3::{pyclass, pymethods, Py, PyAny};
 use rkyv::{Archive, Deserialize, Serialize};
 use std::collections::HashMap;
 use std::sync::{Arc, Mutex};
 
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone, Default)]
 #[archive(check_bytes)]
@@ -13,16 +13,16 @@
     StringVector(Vec<String>),
     Integer(i64),
     IntegerVector(Vec<i64>),
     Float(f64),
     FloatVector(Vec<f64>),
     Boolean(bool),
     BooleanVector(Vec<bool>),
-    BBox(BBox),
-    BBoxVector(Vec<BBox>),
+    BBox(RBBox),
+    BBoxVector(Vec<RBBox>),
     Point(Point),
     PointVector(Vec<Point>),
     Polygon(PolygonalArea),
     PolygonVector(Vec<PolygonalArea>),
     Intersection(Intersection),
     #[default]
     None,
@@ -59,27 +59,27 @@
             ValueVariant::BooleanVector(v) => serde_json::json!({
                 "boolean_vector": v,
             }),
             ValueVariant::BBox(b) => serde_json::json!({
                 "bbox": b.to_serde_json_value(),
             }),
             ValueVariant::BBoxVector(v) => serde_json::json!({
-                "bbox_vector": v.into_iter().map(|b| b.to_serde_json_value()).collect::<Vec<_>>(),
+                "bbox_vector": v.iter().map(|b| b.to_serde_json_value()).collect::<Vec<_>>(),
             }),
             ValueVariant::Point(p) => serde_json::json!({
                 "point": p.to_serde_json_value(),
             }),
             ValueVariant::PointVector(v) => serde_json::json!({
-                "point_vector": v.into_iter().map(|p| p.to_serde_json_value()).collect::<Vec<_>>(),
+                "point_vector": v.iter().map(|p| p.to_serde_json_value()).collect::<Vec<_>>(),
             }),
             ValueVariant::Polygon(p) => serde_json::json!({
                 "polygon": p.to_serde_json_value(),
             }),
             ValueVariant::PolygonVector(v) => serde_json::json!({
-                "polygon_vector": v.into_iter().map(|p| p.to_serde_json_value()).collect::<Vec<_>>(),
+                "polygon_vector": v.iter().map(|p| p.to_serde_json_value()).collect::<Vec<_>>(),
             }),
             ValueVariant::Intersection(i) => serde_json::json!({
                 "intersection": i.to_serde_json_value(),
             }),
             ValueVariant::None => serde_json::json!({
                 "none": null,
             }),
@@ -203,23 +203,23 @@
         Self {
             confidence,
             v: ValueVariant::BooleanVector(b),
         }
     }
 
     #[staticmethod]
-    pub fn bbox(bbox: BBox, confidence: Option<f64>) -> Self {
+    pub fn bbox(bbox: RBBox, confidence: Option<f64>) -> Self {
         Self {
             confidence,
             v: ValueVariant::BBox(bbox),
         }
     }
 
     #[staticmethod]
-    pub fn bboxes(bboxes: Vec<BBox>, confidence: Option<f64>) -> Self {
+    pub fn bboxes(bboxes: Vec<RBBox>, confidence: Option<f64>) -> Self {
         Self {
             confidence,
             v: ValueVariant::BBoxVector(bboxes),
         }
     }
 
     #[staticmethod]
@@ -324,22 +324,22 @@
     pub fn as_booleans(&self) -> Option<Vec<bool>> {
         match &self.v {
             ValueVariant::BooleanVector(b) => Some(b.clone()),
             _ => None,
         }
     }
 
-    pub fn as_bbox(&self) -> Option<BBox> {
+    pub fn as_bbox(&self) -> Option<RBBox> {
         match &self.v {
             ValueVariant::BBox(bbox) => Some(bbox.clone()),
             _ => None,
         }
     }
 
-    pub fn as_bboxes(&self) -> Option<Vec<BBox>> {
+    pub fn as_bboxes(&self) -> Option<Vec<RBBox>> {
         match &self.v {
             ValueVariant::BBoxVector(bbox) => Some(bbox.clone()),
             _ => None,
         }
     }
 
     pub fn as_point(&self) -> Option<Point> {
```

### Comparing `savant_rs-0.1.3/src/primitives/message/eos.rs` & `savant_rs-0.1.4/src/primitives/point.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,42 @@
+use crate::primitives::to_json_value::ToSerdeJsonValue;
 use pyo3::{pyclass, pymethods, Py, PyAny};
 use rkyv::{Archive, Deserialize, Serialize};
+use serde_json::Value;
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
-pub struct EndOfStream {
+pub struct Point {
     #[pyo3(get, set)]
-    pub source_id: String,
+    pub x: f64,
+    #[pyo3(get, set)]
+    pub y: f64,
+}
+
+impl ToSerdeJsonValue for Point {
+    fn to_serde_json_value(&self) -> Value {
+        serde_json::json!({
+            "x": self.x,
+            "y": self.y,
+        })
+    }
 }
 
 #[pymethods]
-impl EndOfStream {
+impl Point {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
     }
 
     fn __str__(&self) -> String {
         self.__repr__()
     }
 
     #[new]
-    pub fn new(source_id: String) -> Self {
-        Self { source_id }
+    pub fn new(x: f64, y: f64) -> Self {
+        Self { x, y }
     }
 }
```

### Comparing `savant_rs-0.1.3/src/primitives/message/loader.rs` & `savant_rs-0.1.4/src/primitives/message/loader.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/primitives/message/saver.rs` & `savant_rs-0.1.4/src/primitives/message/saver.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/primitives/message/video/batch.rs` & `savant_rs-0.1.4/src/primitives/message/video/batch.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/primitives/message/video/frame.rs` & `savant_rs-0.1.4/src/primitives/message/video/frame.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::primitives::attribute::{Attributive, InnerAttributes};
 use crate::primitives::message::video::object::InnerObject;
 use crate::primitives::to_json_value::ToSerdeJsonValue;
-use crate::primitives::{Attribute, Object};
+use crate::primitives::{Attribute, Message, Object};
 use pyo3::{pyclass, pymethods, Py, PyAny, PyResult, Python};
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
 use serde_json::Value;
 use std::collections::HashMap;
 use std::sync::{Arc, Mutex};
 
 #[pyclass]
@@ -315,26 +315,27 @@
     pub(crate) resident_objects: Vec<Arc<Mutex<InnerObject>>>,
 }
 
 impl ToSerdeJsonValue for InnerVideoFrame {
     fn to_serde_json_value(&self) -> Value {
         serde_json::json!(
             {
+                "type": "VideoFrame",
                 "source_id": self.source_id,
                 "framerate": self.framerate,
                 "width": self.width,
                 "height": self.height,
                 "codec": self.codec,
                 "keyframe": self.keyframe,
                 "pts": self.pts,
                 "dts": self.dts,
                 "duration": self.duration,
                 "content": self.content.to_serde_json_value(),
                 "transformations": self.transformations.iter().map(|t| t.to_serde_json_value()).collect::<Vec<_>>(),
-                "attributes": self.attributes.iter().map(|(_, v)| v.to_serde_json_value()).collect::<Vec<_>>(),
+                "attributes": self.attributes.values().map(|v| v.to_serde_json_value()).collect::<Vec<_>>(),
                 "objects": self.resident_objects.iter().map(|o| o.lock().unwrap().to_serde_json_value()).collect::<Vec<_>>(),
             }
         )
     }
 }
 
 impl InnerAttributes for Box<InnerVideoFrame> {
@@ -435,14 +436,18 @@
             content: content.inner,
             attributes: HashMap::default(),
             offline_objects: vec![],
             resident_objects: vec![],
         })
     }
 
+    pub fn to_message(&self) -> Message {
+        Message::video_frame(self.clone())
+    }
+
     #[getter]
     pub fn get_source_id(&self) -> String {
         self.inner.lock().unwrap().source_id.clone()
     }
 
     #[getter]
     pub fn get_json(&self) -> String {
```

### Comparing `savant_rs-0.1.3/src/primitives/message/video/object.rs` & `savant_rs-0.1.4/src/primitives/message/video/object.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use crate::primitives::attribute::{Attributive, InnerAttributes};
 use crate::primitives::to_json_value::ToSerdeJsonValue;
-use crate::primitives::{Attribute, BBox};
+use crate::primitives::{Attribute, RBBox};
 use pyo3::{pyclass, pymethods, Py, PyAny, Python};
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
 use std::collections::HashMap;
 use std::sync::{Arc, Mutex};
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
@@ -68,15 +68,15 @@
 
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone, derive_builder::Builder)]
 #[archive(check_bytes)]
 pub struct InnerObject {
     pub id: i64,
     pub creator: String,
     pub label: String,
-    pub bbox: BBox,
+    pub bbox: RBBox,
     pub attributes: HashMap<(String, String), Attribute>,
     pub confidence: Option<f64>,
     pub parent: Option<ParentObject>,
     pub track_id: Option<i64>,
     #[with(Skip)]
     pub modifications: Vec<Modification>,
 }
@@ -84,15 +84,15 @@
 impl ToSerdeJsonValue for InnerObject {
     fn to_serde_json_value(&self) -> serde_json::Value {
         serde_json::json!({
             "id": self.id,
             "creator": self.creator,
             "label": self.label,
             "bbox": self.bbox.to_serde_json_value(),
-            "attributes": self.attributes.iter().map(|(_, v)| v.to_serde_json_value()).collect::<Vec<_>>(),
+            "attributes": self.attributes.values().map(|v| v.to_serde_json_value()).collect::<Vec<_>>(),
             "confidence": self.confidence,
             "parent": self.parent.as_ref().map(|p| p.to_serde_json_value()),
             "track_id": self.track_id,
             "modifications": self.modifications.iter().map(|m| m.to_serde_json_value()).collect::<Vec<serde_json::Value>>(),
         })
     }
 }
@@ -153,15 +153,15 @@
 
     #[allow(clippy::too_many_arguments)]
     #[new]
     pub fn new(
         id: i64,
         creator: String,
         label: String,
-        bbox: BBox,
+        bbox: RBBox,
         attributes: HashMap<(String, String), Attribute>,
         confidence: Option<f64>,
         parent: Option<ParentObject>,
         track_id: Option<i64>,
     ) -> Self {
         let object = InnerObject {
             id,
@@ -197,15 +197,15 @@
 
     #[getter]
     pub fn get_label(&self) -> String {
         self.inner.lock().unwrap().label.clone()
     }
 
     #[getter]
-    pub fn get_bbox(&self) -> crate::primitives::BBox {
+    pub fn get_bbox(&self) -> crate::primitives::RBBox {
         self.inner.lock().unwrap().bbox.clone()
     }
 
     #[getter]
     pub fn get_confidence(&self) -> Option<f64> {
         let object = self.inner.lock().unwrap();
         object.confidence
@@ -242,15 +242,15 @@
     pub fn set_label(&mut self, label: String) {
         let mut object = self.inner.lock().unwrap();
         object.label = label;
         object.modifications.push(Modification::Label);
     }
 
     #[setter]
-    pub fn set_bbox(&mut self, bbox: BBox) {
+    pub fn set_bbox(&mut self, bbox: RBBox) {
         let mut object = self.inner.lock().unwrap();
         object.bbox = bbox;
         object.modifications.push(Modification::BoundingBox);
     }
 
     #[setter]
     pub fn set_confidence(&mut self, confidence: Option<f64>) {
@@ -341,25 +341,25 @@
     }
 }
 
 #[cfg(test)]
 mod tests {
     use crate::primitives::attribute::Attributive;
     use crate::primitives::message::video::object::InnerObjectBuilder;
-    use crate::primitives::{AttributeBuilder, BBox, Modification, Object, Value};
+    use crate::primitives::{AttributeBuilder, Modification, Object, RBBox, Value};
 
     fn get_object() -> Object {
         Object::from_inner_object(
             InnerObjectBuilder::default()
                 .id(1)
                 .track_id(None)
                 .modifications(vec![])
                 .creator("model".to_string())
                 .label("label".to_string())
-                .bbox(BBox::new(0.0, 0.0, 1.0, 1.0, None))
+                .bbox(RBBox::new(0.0, 0.0, 1.0, 1.0, None))
                 .confidence(Some(0.5))
                 .attributes(
                     vec![
                         AttributeBuilder::default()
                             .creator("creator".to_string())
                             .name("name".to_string())
                             .values(vec![Value::string("value".to_string(), None)])
@@ -458,15 +458,15 @@
     #[test]
     fn test_modifications() {
         let mut t = get_object();
         t.set_label("label2".to_string());
         assert_eq!(t.take_modifications(), vec![Modification::Label]);
         assert_eq!(t.take_modifications(), vec![]);
 
-        t.set_bbox(BBox::new(0.0, 0.0, 1.0, 1.0, None));
+        t.set_bbox(RBBox::new(0.0, 0.0, 1.0, 1.0, None));
         t.clear_attributes_py();
         assert_eq!(
             t.take_modifications(),
             vec![Modification::BoundingBox, Modification::Attributes]
         );
         assert_eq!(t.take_modifications(), vec![]);
     }
```

### Comparing `savant_rs-0.1.3/src/primitives/message.rs` & `savant_rs-0.1.4/src/primitives/message.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/primitives/point.rs` & `savant_rs-0.1.4/src/primitives/message/eos.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 use crate::primitives::to_json_value::ToSerdeJsonValue;
+use crate::primitives::Message;
 use pyo3::{pyclass, pymethods, Py, PyAny};
 use rkyv::{Archive, Deserialize, Serialize};
 use serde_json::Value;
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
-pub struct Point {
+pub struct EndOfStream {
     #[pyo3(get, set)]
-    pub x: f64,
-    #[pyo3(get, set)]
-    pub y: f64,
+    pub source_id: String,
 }
 
-impl ToSerdeJsonValue for Point {
+impl ToSerdeJsonValue for EndOfStream {
     fn to_serde_json_value(&self) -> Value {
-        serde_json::json!({
-            "x": self.x,
-            "y": self.y,
+        serde_json::json!(
+        {
+            "type": "EndOfStream",
+            "source_id": self.source_id,
         })
     }
 }
 
 #[pymethods]
-impl Point {
+impl EndOfStream {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
     }
 
     fn __str__(&self) -> String {
         self.__repr__()
     }
 
     #[new]
-    pub fn new(x: f64, y: f64) -> Self {
-        Self { x, y }
+    pub fn new(source_id: String) -> Self {
+        Self { source_id }
+    }
+
+    #[getter]
+    pub fn get_json(&self) -> String {
+        serde_json::to_string(&self.to_serde_json_value()).unwrap()
+    }
+
+    pub fn to_message(&self) -> Message {
+        Message::end_of_stream(self.clone())
     }
 }
```

### Comparing `savant_rs-0.1.3/src/primitives/polygonal_area.rs` & `savant_rs-0.1.4/src/primitives/polygonal_area.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/primitives/segment.rs` & `savant_rs-0.1.4/src/primitives/segment.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/primitives.rs` & `savant_rs-0.1.4/src/primitives.rs`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pub mod to_json_value;
 
 use crate::primitives::message::video::frame::PyFrameTransformation;
 pub use attribute::Attribute;
 pub use attribute::AttributeBuilder;
 pub use attribute::Value;
 pub use bbox::BBox;
+pub use bbox::RBBox;
 pub use message::eos::EndOfStream;
 pub use message::loader::load_message;
 pub use message::saver::save_message;
 pub use message::video::batch::VideoFrameBatch;
 pub use message::video::frame::PyVideoFrameContent;
 pub use message::video::frame::VideoFrame;
 pub use message::video::object::Modification;
@@ -32,14 +33,15 @@
 #[pymodule]
 pub fn primitives(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<Point>()?;
     m.add_class::<Segment>()?;
     m.add_class::<IntersectionKind>()?;
     m.add_class::<Intersection>()?;
     m.add_class::<PolygonalArea>()?;
+    m.add_class::<RBBox>()?;
     m.add_class::<BBox>()?;
     m.add_class::<Attribute>()?;
     m.add_class::<Value>()?;
     m.add_class::<Object>()?;
     m.add_class::<ParentObject>()?;
     m.add_class::<VideoFrame>()?;
     m.add_class::<VideoFrameBatch>()?;
```

### Comparing `savant_rs-0.1.3/src/test.rs` & `savant_rs-0.1.4/src/test.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pub mod utils {
     use crate::primitives::message::video::frame::InnerVideoFrameBuilder;
     use crate::primitives::message::video::object::InnerObjectBuilder;
     use crate::primitives::{
         AttributeBuilder, Intersection, IntersectionKind, Point, PyVideoFrameContent, Value,
     };
-    use crate::primitives::{BBox, VideoFrame};
+    use crate::primitives::{RBBox, VideoFrame};
     use pyo3::pyfunction;
     use std::collections::HashMap;
     use std::sync::{Arc, Mutex};
 
     #[pyfunction]
     pub fn gen_frame() -> VideoFrame {
         let mut f = VideoFrame::from_inner(
@@ -28,43 +28,43 @@
                 .offline_objects(Default::default())
                 .resident_objects(vec![
                     Arc::new(Mutex::new(
                         InnerObjectBuilder::default()
                             .id(0)
                             .track_id(None)
                             .modifications(Vec::default())
-                            .bbox(BBox::new(0.0, 0.0, 0.0, 0.0, None))
+                            .bbox(RBBox::new(0.0, 0.0, 0.0, 0.0, None))
                             .parent(None)
                             .attributes(HashMap::default())
                             .confidence(None)
                             .creator("test".to_string())
                             .label("test2".to_string())
                             .build()
                             .unwrap(),
                     )),
                     Arc::new(Mutex::new(
                         InnerObjectBuilder::default()
                             .id(1)
                             .track_id(None)
                             .modifications(Vec::default())
-                            .bbox(BBox::new(0.0, 0.0, 0.0, 0.0, None))
+                            .bbox(RBBox::new(0.0, 0.0, 0.0, 0.0, None))
                             .parent(None)
                             .attributes(HashMap::default())
                             .confidence(None)
                             .creator("test2".to_string())
                             .label("test".to_string())
                             .build()
                             .unwrap(),
                     )),
                     Arc::new(Mutex::new(
                         InnerObjectBuilder::default()
                             .id(2)
                             .track_id(None)
                             .modifications(Vec::default())
-                            .bbox(BBox::new(0.0, 0.0, 0.0, 0.0, None))
+                            .bbox(RBBox::new(0.0, 0.0, 0.0, 0.0, None))
                             .parent(None)
                             .attributes(HashMap::default())
                             .confidence(None)
                             .creator("test2".to_string())
                             .label("test2".to_string())
                             .build()
                             .unwrap(),
@@ -113,19 +113,19 @@
                 .values(vec![
                     Value::bytes(vec![8, 3, 8, 8], [0; 192].into(), None),
                     Value::integers([0, 1, 2, 3, 4, 5].into(), None),
                     Value::string("incoming".to_string(), Some(0.56)),
                     Value::strings(vec!["abc".into(), "cde".into()], None),
                     Value::string("outgoing".to_string(), Some(0.64)),
                     Value::none(),
-                    Value::bbox(BBox::new(0.0, 0.0, 0.0, 0.0, None), None),
+                    Value::bbox(RBBox::new(0.0, 0.0, 0.0, 0.0, None), None),
                     Value::bboxes(
                         vec![
-                            BBox::new(0.0, 0.0, 0.0, 0.0, None),
-                            BBox::new(0.0, 0.0, 0.0, 0.0, None),
+                            RBBox::new(0.0, 0.0, 0.0, 0.0, None),
+                            RBBox::new(0.0, 0.0, 0.0, 0.0, None),
                         ],
                         None,
                     ),
                     Value::float(0.0, None),
                     Value::floats(vec![0.0, 0.0, 0.0, 0.0, 0.0, 0.0], None),
                     Value::points(vec![Point::new(0.0, 0.0), Point::new(0.0, 0.0)], None),
                     Value::intersection(
```

### Comparing `savant_rs-0.1.3/src/test_rkyv_tuple.rs` & `savant_rs-0.1.4/src/test_rkyv_tuple.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/tests_pyo3_access.rs` & `savant_rs-0.1.4/src/tests_pyo3_access.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.3/src/utils/fps_meter.rs` & `savant_rs-0.1.4/src/utils/fps_meter.rs`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         let delta_time = self.delta_time();
         if self.period_passed() {
             self.reset();
         }
 
         (
             i64::try_from(delta_frames).unwrap(),
-            i64::try_from(delta_time as i64).unwrap(),
+            i64::try_from(delta_time).unwrap(),
         )
     }
 
     fn period_passed(&self) -> bool {
         match self.inner {
             MeterFlavor::CountBased(count) => self.delta_frames() >= count,
             MeterFlavor::TimeBased(seconds) => self.delta_time() >= seconds,
```

### Comparing `savant_rs-0.1.3/src/utils/symbol_mapper.rs` & `savant_rs-0.1.4/src/utils/symbol_mapper.rs`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             let mapper = SYMBOL_MAPPER.lock().unwrap();
             object_ids
                 .iter()
                 .flat_map(|object_id| {
                     mapper
                         .get_object_label(model_id, *object_id)
                         .map(|label| (*object_id, Some(label)))
-                        .or_else(|| Some((*object_id, None)))
+                        .or(Some((*object_id, None)))
                 })
                 .collect()
         })
     })
 }
 
 #[pyfunction]
@@ -184,14 +184,24 @@
         py.allow_threads(|| {
             let mapper = SYMBOL_MAPPER.lock().unwrap();
             mapper.is_object_registered(&model_name, &object_label)
         })
     })
 }
 
+#[pyfunction]
+pub fn dump_registry() -> Vec<String> {
+    Python::with_gil(|py| {
+        py.allow_threads(|| {
+            let mapper = SYMBOL_MAPPER.lock().unwrap();
+            mapper.dump_registry()
+        })
+    })
+}
+
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct SymbolMapper {
     registry: HashMap<String, (i64, Option<i64>)>,
     reverse_registry: HashMap<(i64, Option<i64>), String>,
     model_next_id: i64,
     model_object_next_ids: HashMap<String, i64>,
@@ -212,14 +222,26 @@
     pub fn clear(&mut self) {
         self.registry.clear();
         self.reverse_registry.clear();
         self.model_object_next_ids.clear();
         self.model_next_id = 0;
     }
 
+    pub fn dump_registry(&self) -> Vec<String> {
+        self.registry
+            .iter()
+            .map(|(key, (model_id, object_id))| {
+                format!(
+                    "Key={}, ModelId={}, ObjectId={:?}",
+                    key, model_id, object_id
+                )
+            })
+            .collect()
+    }
+
     pub fn build_model_object_key(model_name: &String, object_label: &String) -> String {
         format!("{}{}{}", model_name, REGISTRY_KEY_SEPARATOR, object_label)
     }
 
     pub fn get_model_id(&mut self, model_name: &String) -> anyhow::Result<i64> {
         Self::validate_base_key(model_name)?;
         match self.registry.get(model_name) {
@@ -256,15 +278,15 @@
 
         if parts.count() != 0 {
             return Err(Errors::FullyQualifiedObjectNameParseError(key.clone()).into());
         }
 
         match (model_name, object_name) {
             (Some(m), Some(o)) => {
-                if m.len() > 0 && o.len() > 0 {
+                if !m.is_empty() && !o.is_empty() {
                     Ok((m.to_string(), o.to_string()))
                 } else {
                     Err(Errors::FullyQualifiedObjectNameParseError(key.clone()).into())
                 }
             }
             _ => Err(Errors::FullyQualifiedObjectNameParseError(key.clone()).into()),
         }
@@ -285,15 +307,15 @@
     pub fn get_object_id(
         &mut self,
         model_name: &String,
         object_label: &String,
     ) -> anyhow::Result<(i64, i64)> {
         let model_id = self.get_model_id(model_name)?;
         Self::validate_base_key(object_label)?;
-        let full_key = Self::build_model_object_key(model_name, &object_label);
+        let full_key = Self::build_model_object_key(model_name, object_label);
 
         match self.registry.get(&full_key) {
             Some((model_id, Some(object_id))) => Ok((*model_id, *object_id)),
             Some((_, None)) => Err(Errors::UnexpectedModelIdObjectId(full_key).into()),
             None => {
                 let last_object_id = self
                     .model_object_next_ids
@@ -323,17 +345,17 @@
             .model_object_next_ids
             .get(model_name)
             .cloned()
             .unwrap_or(-1);
 
         for (label_id, object_label) in objects {
             Self::validate_base_key(object_label)?;
-            let key = Self::build_model_object_key(model_name, &object_label);
+            let key = Self::build_model_object_key(model_name, object_label);
             if matches!(policy, RegistrationPolicy::ErrorIfNonUnique) {
-                if self.is_object_registered(model_name, &object_label) {
+                if self.is_object_registered(model_name, object_label) {
                     return Err(Errors::DuplicateName(object_label.clone()).into());
                 }
 
                 if self
                     .reverse_registry
                     .contains_key(&(model_id, Some(*label_id)))
                 {
```

### Comparing `savant_rs-0.1.3/src/utils.rs` & `savant_rs-0.1.4/src/utils.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,41 @@
+pub mod bounding_box;
 pub mod fps_meter;
 pub mod symbol_mapper;
 
 use pyo3::prelude::*;
 
 use crate::primitives::message::loader::load_message_py;
 use crate::primitives::message::saver::save_message_py;
 use crate::test::utils::gen_frame;
 use crate::utils::symbol_mapper::RegistrationPolicy;
 use crate::utils::symbol_mapper::SymbolMapper;
 use crate::utils::symbol_mapper::{
-    build_model_object_key, clear_symbol_maps, get_model_id, get_model_name, get_object_id,
-    get_object_ids, get_object_label, get_object_labels, is_model_registered, is_object_registered,
-    parse_compound_key, register_model_objects, validate_base_key,
+    build_model_object_key, clear_symbol_maps, dump_registry, get_model_id, get_model_name,
+    get_object_id, get_object_ids, get_object_label, get_object_labels, is_model_registered,
+    is_object_registered, parse_compound_key, register_model_objects, validate_base_key,
 };
 
 pub use fps_meter::FpsMeter;
 
+#[pyfunction]
+#[inline]
+pub fn round_2_digits(v: f64) -> f64 {
+    (v * 100.0).round() / 100.0
+}
+
 #[pymodule]
 pub fn utils(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(save_message_py, m)?)?;
     m.add_function(wrap_pyfunction!(load_message_py, m)?)?;
     m.add_function(wrap_pyfunction!(gen_frame, m)?)?;
 
     m.add_function(wrap_pyfunction!(build_model_object_key, m)?)?;
     m.add_function(wrap_pyfunction!(clear_symbol_maps, m)?)?;
+    m.add_function(wrap_pyfunction!(dump_registry, m)?)?;
     m.add_function(wrap_pyfunction!(get_model_id, m)?)?;
     m.add_function(wrap_pyfunction!(get_model_name, m)?)?;
     m.add_function(wrap_pyfunction!(get_object_id, m)?)?;
     m.add_function(wrap_pyfunction!(get_object_ids, m)?)?;
     m.add_function(wrap_pyfunction!(get_object_label, m)?)?;
     m.add_function(wrap_pyfunction!(get_object_labels, m)?)?;
     m.add_function(wrap_pyfunction!(is_model_registered, m)?)?;
```

### Comparing `savant_rs-0.1.3/Cargo.lock` & `savant_rs-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -722,17 +722,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "c4ec6d5fe0b140acb27c9a0444118cf55bfbb4e0b259739429abb4521dd67c16"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -980,15 +980,15 @@
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "savant_rs"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "anyhow",
  "derive_builder",
  "env_logger",
  "geo",
  "hashbrown 0.13.2",
  "itertools",
@@ -1209,17 +1209,17 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "uuid"
-version = "1.3.2"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dad5567ad0cf5b760e5665964bec1b47dfd077ba8a2544b513f3556d3d239a2"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
```

### Comparing `savant_rs-0.1.3/PKG-INFO` & `savant_rs-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savant_rs
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Savant rust optimization library
 Keywords: computer-vision,video-processing
 Home-Page: https://github.com/insight-platform/savant-rs
```

