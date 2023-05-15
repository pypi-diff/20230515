# Comparing `tmp/express-pascal-voc-tools-0.7.0.tar.gz` & `tmp/express-pascal-voc-tools-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.7.0.tar", last modified: Fri May 12 04:44:56 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.7.1.tar", last modified: Mon May 15 16:32:45 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.7.0.tar` & `express-pascal-voc-tools-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 04:44:56.946051 express-pascal-voc-tools-0.7.0/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     4900 2023-05-12 04:44:56.942059 express-pascal-voc-tools-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     4416 2023-05-11 13:01:05.000000 express-pascal-voc-tools-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 04:44:56.892233 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0     4900 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 04:44:56.947051 express-pascal-voc-tools-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-12 04:28:46.000000 express-pascal-voc-tools-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 04:44:56.927125 express-pascal-voc-tools-0.7.0/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.7.0/voc_tools/__init__.py
--rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.7.0/voc_tools/constants.py
--rw-rw-rw-   0        0        0     5096 2023-05-12 04:28:20.000000 express-pascal-voc-tools-0.7.0/voc_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-12 04:44:56.935124 express-pascal-voc-tools-0.7.0/voc_tools/unittest/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.7.0/voc_tools/unittest/__init__.py
--rw-rw-rw-   0        0        0     3745 2023-05-12 04:43:55.000000 express-pascal-voc-tools-0.7.0/voc_tools/unittest/reader_test.py
--rw-rw-rw-   0        0        0     8858 2023-05-11 12:09:35.000000 express-pascal-voc-tools-0.7.0/voc_tools/utils.py
--rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.7.0/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.7.0/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:32:45.383434 express-pascal-voc-tools-0.7.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     4900 2023-05-15 16:32:45.372765 express-pascal-voc-tools-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4416 2023-05-11 13:01:05.000000 express-pascal-voc-tools-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 16:32:45.247692 express-pascal-voc-tools-0.7.1/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0     4900 2023-05-15 16:32:43.000000 express-pascal-voc-tools-0.7.1/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-15 16:32:44.000000 express-pascal-voc-tools-0.7.1/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 16:32:43.000000 express-pascal-voc-tools-0.7.1/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-15 16:32:43.000000 express-pascal-voc-tools-0.7.1/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 16:32:43.000000 express-pascal-voc-tools-0.7.1/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 16:32:45.384280 express-pascal-voc-tools-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-15 16:31:57.000000 express-pascal-voc-tools-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:32:45.326753 express-pascal-voc-tools-0.7.1/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.7.1/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.7.1/voc_tools/constants.py
+-rw-rw-rw-   0        0        0     5146 2023-05-15 16:30:16.000000 express-pascal-voc-tools-0.7.1/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:32:45.354410 express-pascal-voc-tools-0.7.1/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.7.1/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     3745 2023-05-12 04:43:55.000000 express-pascal-voc-tools-0.7.1/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0     8974 2023-05-15 16:30:16.000000 express-pascal-voc-tools-0.7.1/voc_tools/utils.py
+-rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.7.1/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.7.1/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.7.0/LICENSE` & `express-pascal-voc-tools-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.7.0/PKG-INFO` & `express-pascal-voc-tools-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.7.0
+Version: 0.7.1
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `express-pascal-voc-tools-0.7.0/README.md` & `express-pascal-voc-tools-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/PKG-INFO` & `express-pascal-voc-tools-0.7.1/express_pascal_voc_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.7.0
+Version: 0.7.1
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `express-pascal-voc-tools-0.7.0/setup.py` & `express-pascal-voc-tools-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['lxml', 'numpy', 'opencv-python'],
     version_config=True,
-    version="0.7.0"
+    version="0.7.1"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.7.0/voc_tools/reader.py` & `express-pascal-voc-tools-0.7.1/voc_tools/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pathlib
 import xml.etree.ElementTree as ET
 
 from voc_tools.constants import VOC_XMLS, VOC_IMAGES, VOC_CAPTIONS
-from voc_tools.utils import Annotation, Caption
+from voc_tools.utils import Annotation, Caption, Dataset
 
 
 def from_file(file: str):
     """
     Generate a list of Annotation objects for a given image or xml of a PASCAL VOC dataset.
     It also supports captions .txt files
     """
@@ -22,26 +22,26 @@
 
 
 def from_caption(txt_file: str):
     """
     Generate a list of Annotation objects for a given caption of a PASCAL VOC dataset
     """
     txt_file = pathlib.Path(txt_file)
-    parent_path = txt_file.parents[1] / "Annotations"
+    parent_path = txt_file.parents[1] / Dataset.ANNO_DIR
     file_name = txt_file.name.replace(".txt", ".xml")
     xml_file = str(parent_path / file_name)
     return from_xml(xml_file)
 
 
 def from_image(image_file: str):
     """
     Generate a list of Annotation objects for a given image of a PASCAL VOC dataset
     """
     image_file = pathlib.Path(image_file)
-    parent_path = image_file.parents[1] / "Annotations"
+    parent_path = image_file.parents[1] / Dataset.ANNO_DIR
     file_name = image_file.name.replace(".jpeg", ".xml").replace(".jpg", ".xml")
     xml_file = str(parent_path / file_name)
     return from_xml(xml_file)
 
 
 def from_xml(xml_file: str, empty_placeholder="NULL"):
     """
@@ -86,15 +86,16 @@
         images: [depreciated] use this flag to load JPEGImages directory. Use dir_flag=VOC_IMAGES instead.
         fullpath: A boolean flag indicates whether to generate full path or the filename.
     """
     dir_path = pathlib.Path(dir_path)
     if images:
         dir_flag = VOC_IMAGES
     annotations_dir = dir_path / (
-        "JPEGImages" if dir_flag == VOC_IMAGES else ("Annotations" if dir_flag == VOC_XMLS else "text"))
+        Dataset.IMAGE_DIR if dir_flag == VOC_IMAGES else (
+            Dataset.ANNO_DIR if dir_flag == VOC_XMLS else Dataset.CAPTION_DIR))
     for file_item in os.listdir(str(annotations_dir)):
         if fullpath:
             yield str(annotations_dir / file_item)
         else:
             yield (annotations_dir / file_item).name
```

### Comparing `express-pascal-voc-tools-0.7.0/voc_tools/unittest/reader_test.py` & `express-pascal-voc-tools-0.7.1/voc_tools/unittest/reader_test.py`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.7.0/voc_tools/utils.py` & `express-pascal-voc-tools-0.7.1/voc_tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     assert file.endswith(".xml") or file.endswith(".txt") or file.endswith(".jpeg") or file.endswith(".jpg"), (
         "Unsupported file format")
     assert converter_flag in [VOC_IMAGES, VOC_CAPTIONS, VOC_XMLS], "Unsupported converter_flag"
     file = pathlib.Path(file)
     filename = file.name
     parent_path = file.parents[1]
     if converter_flag == VOC_IMAGES:
-        path = parent_path / "JPEGImages" / filename
+        path = parent_path / Dataset.IMAGE_DIR / filename
     if converter_flag == VOC_XMLS:
-        path = parent_path / "Annotations" / filename
+        path = parent_path / Dataset.ANNO_DIR / filename
     if converter_flag == VOC_CAPTIONS:
-        path = parent_path / "text" / filename
+        path = parent_path / Dataset.CAPTION_DIR / filename
     return str(path)
 
 
 # ################################################
 # Python classes to hold annotation and captions #
 # ################################################
 class Atomic:
@@ -194,14 +194,18 @@
             csv_fp.write("{}\n".format(Caption.csv_header()))
             for caption in caption_from_dir(self.dataset_path, bulk=False):
                 csv_fp.write("{}\n".format(caption.csv()))
         return self
 
 
 class Dataset(ABCDataset):
+    IMAGE_DIR = "JPEGImages"
+    ANNO_DIR = "Annotations"
+    CAPTION_DIR = "captions"
+
     def __init__(self, dataset_path, caption_support=False):
         super().__init__(dataset_path)
         self.dataset_path = dataset_path
         self.caption_support = caption_support
         self.meta = np.array([], dtype='object')
         self.image_cache: JPEG = None
         self.loaded = False
@@ -225,23 +229,22 @@
         from voc_tools.reader import from_dir
         for anno in from_dir(self.dataset_path, bulk=bulk):
             if bulk:
                 yield anno, self.get_image(anno[0].filename)
             else:
                 yield anno, self.get_image(anno.filename)
 
-
     def class_names(self):
         if not self.loaded:
             self.load()
         class_name_idx = Annotation.raw_attributes().index('class_name')
         return tuple(set(self.meta[:, class_name_idx]))
 
     def get_image(self, filename):
-        return JPEG(os.path.join(self.dataset_path, "JPEGImages", filename))
+        return JPEG(os.path.join(self.dataset_path, Dataset.IMAGE_DIR, filename))
 
     def get_image_meta(self, filename):
         if self.image_cache is None or filename != self.image_cache.filename:
             # save the image
             self.image_cache = self.get_image(filename)
             # if a newer appear, re
         return self.image_cache.csv().split(",")[1:]
```

