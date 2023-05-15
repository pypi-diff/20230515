# Comparing `tmp/geolibs-0.0.4.tar.gz` & `tmp/geolibs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolibs-0.0.4.tar", max compression
+gzip compressed data, was "geolibs-0.0.5.tar", max compression
```

## Comparing `geolibs-0.0.4.tar` & `geolibs-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      566 2023-05-06 21:58:44.569227 geolibs-0.0.4/README.rst
--rwxr-xr-x   0        0        0      512 2023-05-06 22:05:37.281858 geolibs-0.0.4/geolibs/__init__.py
--rwxr-xr-x   0        0        0     5514 2023-05-06 20:36:53.288107 geolibs-0.0.4/geolibs/engine_cocoext.py
--rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.4/geolibs/engine_cocometric.py
--rwxr-xr-x   0        0        0     4167 2023-05-06 21:58:44.616807 geolibs-0.0.4/geolibs/engine_csv.py
--rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.4/geolibs/enginelogger_hook.py
--rwxr-xr-x   0        0        0    12304 2023-05-06 20:53:44.332058 geolibs-0.0.4/geolibs/loading.py
--rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.4/geolibs/misc.py
--rwxr-xr-x   0        0        0     1066 2023-05-06 22:05:37.276852 geolibs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 geolibs-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      566 2023-05-06 21:58:44.569227 geolibs-0.0.5/README.rst
+-rwxr-xr-x   0        0        0      512 2023-05-15 18:43:38.073114 geolibs-0.0.5/geolibs/__init__.py
+-rwxr-xr-x   0        0        0    12027 2023-05-15 18:42:52.449796 geolibs-0.0.5/geolibs/engine_cocoext.py
+-rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.5/geolibs/engine_cocometric.py
+-rwxr-xr-x   0        0        0     4167 2023-05-06 21:58:44.616807 geolibs-0.0.5/geolibs/engine_csv.py
+-rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.5/geolibs/enginelogger_hook.py
+-rwxr-xr-x   0        0        0    12170 2023-05-15 18:42:52.457794 geolibs-0.0.5/geolibs/loading.py
+-rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.5/geolibs/misc.py
+-rwxr-xr-x   0        0        0     1066 2023-05-15 18:43:38.066115 geolibs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 geolibs-0.0.5/PKG-INFO
```

### Comparing `geolibs-0.0.4/README.rst` & `geolibs-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.4/geolibs/__init__.py` & `geolibs-0.0.5/geolibs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from .engine_cocoext import EngineCocoExt
 from .engine_csv import EngineCSV
 from .loading import LoadBandsFromFile, LoadVariableSizedBandsFromFile, LoadMasks
 from .engine_cocometric import EngineCocoMetric
 
 __author__ = """Sagar Verma"""
 __email__ = 'sagar@granular.ai'
-__version__ = 'v0.0.4'
+__version__ = 'v0.0.5'
 
 __all__ = ["EngineLoggerHook", "EngineCocoExt", "EngineCocoMetric",
            "EngineCSV", "LoadBandsFromFile", "LoadVariableSizedBandsFromFile",
            "LoadMasks"]
```

### Comparing `geolibs-0.0.4/geolibs/engine_cocometric.py` & `geolibs-0.0.5/geolibs/engine_cocometric.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.4/geolibs/engine_csv.py` & `geolibs-0.0.5/geolibs/engine_csv.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.4/geolibs/enginelogger_hook.py` & `geolibs-0.0.5/geolibs/enginelogger_hook.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.4/geolibs/loading.py` & `geolibs-0.0.5/geolibs/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         >>>     tif_buff = f.read()
         >>> bands = mmcv.bandsfrombytes(tif_buff, band_ids=[0, 1, 2])
     """
     with MemoryFile(content) as memfile:
         r = memfile.open()
         bands = r.read()
         metadata = r.profile
+        r.close()
         
         if not band_ids:
             return bands, metadata
         else:
             return bands[band_ids], metadata
 
 
@@ -102,40 +103,32 @@
         self.to_float32 = to_float32
         self.file_client_args = file_client_args.copy()
         self.file_client = None
         self.gray2rgb = gray2rgb
 
     def transform(self, results: dict):
         filename = results['img_path']
-        try:
-            if self.file_client_args is not None:
-                file_client = fileio.FileClient.infer_client(
-                    self.file_client_args, filename)
-                band_bytes = file_client.get(filename)
-            else:
-                band_bytes = fileio.get(
-                    filename, backend_args=self.backend_args)
-            
-            bands, metadata = bandsfrombytes(band_bytes, band_ids=self.band_ids)
-            if self.gray2rgb:
-                assert bands.shape[0] == 1, "gray2rgb is only for grayscale images"
-                bands = np.asarray([bands[0], bands[0], bands[0]])
-            bands = bands.transpose(1, 2, 0)
-
-            if "img_info" in results:
-                bands = self._make_patch(bands, results["img_info"])
-            if self.to_float32:
-                bands = bands.astype(np.float32)
-                
-        except Exception as e:
-            if self.ignore_empty:
-                return None
-            else:
-                raise e
+        if self.file_client_args is not None:
+            file_client = fileio.FileClient.infer_client(
+                self.file_client_args, filename)
+            band_bytes = file_client.get(filename)
+        else:
+            band_bytes = fileio.get(
+                filename, backend_args=self.backend_args)
+        
+        bands, metadata = bandsfrombytes(band_bytes, band_ids=self.band_ids)
+        if self.gray2rgb:
+            assert bands.shape[0] == 1, "gray2rgb is only for grayscale images"
+            bands = np.asarray([bands[0], bands[0], bands[0]])
+        bands = bands.transpose(1, 2, 0)
 
+        bands = self._make_patch(bands, results)
+        if self.to_float32:
+            bands = bands.astype(np.float32)
+                
         results["img"] = bands
         results["img_shape"] = bands.shape[:2]
         results["ori_shape"] = bands.shape[:2]
         results["img_meta"] = metadata
 
         num_channels = 1 if len(bands.shape) < 3 else bands.shape[2]
 
@@ -148,15 +141,15 @@
 
 
     def _make_patch(self, bands, img_info):
         slice_x = img_info["slice_x"]
         slice_y = img_info["slice_y"]
         slice_w = img_info["slice_w"]
         slice_h = img_info["slice_h"]
-        return bands[slice_y:slice_y+slice_h, slice_x:slice_x+slice_w, :]
+        return bands[slice_y:slice_y+slice_h, slice_x:slice_x+slice_w, :].copy()
 
 
 @TRANSFORMS.register_module()
 class LoadVariableSizedBandsFromFile(LoadImageFromFile):
     """Load variable sized bands from tar file.
     Required keys are "img_prefix" and "img_info" (a dict that must contain the
     key "filename"). Added or updated keys are "filename", "img", "img_shape",
@@ -296,28 +289,32 @@
         """
         if self.reduce_zero_label is None:
             self.reduce_zero_label = results['reduce_zero_label']
         assert self.reduce_zero_label == results['reduce_zero_label'], \
             'Initialize dataset with `reduce_zero_label` as ' \
             f'{results["reduce_zero_label"]} but when load annotation ' \
             f'the `reduce_zero_label` is {self.reduce_zero_label}'
-        h, w = results['height'], results['width']
+        h, w = results['slice_h'], results['slice_w']
         gt_semantic_seg = np.zeros((h, w), dtype=np.uint8)
         for annotation in results["instances"]:
-            pts = np.asarray(annotation['mask'][0]).reshape(-1, 1, 2).astype(np.int32)[:-1]
-            label = annotation['bbox_label'] + 1
-            gt_semantic_seg = cv2.fillPoly(gt_semantic_seg, pts=[pts], color=label)
+            for poly in annotation['mask']:
+                if len(poly):
+                    pts = np.asarray(poly).reshape(-1, 1, 2).astype(np.int32)[:-1]
+                    label = annotation['bbox_label'] + 1
+                    gt_semantic_seg = cv2.fillPoly(gt_semantic_seg, pts=[pts], color=label)
         if self.reduce_zero_label:
             # avoid using underflow conversion
             gt_semantic_seg[gt_semantic_seg == 0] = 255
             gt_semantic_seg = gt_semantic_seg - 1
             gt_semantic_seg[gt_semantic_seg == 254] = 255
 
         results['gt_seg_map'] = gt_semantic_seg
         results['seg_fields'].append('gt_seg_map')
 
+        return results
+
     def __repr__(self) -> str:
         repr_str = self.__class__.__name__
         repr_str += f'(reduce_zero_label={self.reduce_zero_label}, '
         repr_str += f"imdecode_backend='{self.imdecode_backend}', "
         repr_str += f'backend_args={self.backend_args})'
         return repr_str
```

### Comparing `geolibs-0.0.4/geolibs/misc.py` & `geolibs-0.0.5/geolibs/misc.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.4/pyproject.toml` & `geolibs-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geolibs"
-version = "v0.0.4"
+version = "v0.0.5"
 description = "A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development."
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "geolibs"}]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `geolibs-0.0.4/PKG-INFO` & `geolibs-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolibs
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development.
 Home-page: https://github.com/granularai/geolibs
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

