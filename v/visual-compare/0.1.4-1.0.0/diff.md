# Comparing `tmp/visual-compare-0.1.4.tar.gz` & `tmp/visual-compare-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual-compare-0.1.4.tar", last modified: Fri May 12 02:09:17 2023, max compression
+gzip compressed data, was "visual-compare-1.0.0.tar", last modified: Mon May 15 08:00:03 2023, max compression
```

## Comparing `visual-compare-0.1.4.tar` & `visual-compare-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.757008 visual-compare-0.1.4/
--rw-rw-rw-   0        0        0     2047 2023-05-12 02:09:17.757008 visual-compare-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2023-05-12 02:07:01.000000 visual-compare-0.1.4/README.md
--rw-rw-rw-   0        0        0      145 2023-05-12 02:09:17.757008 visual-compare-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-05-12 02:07:51.000000 visual-compare-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.741408 visual-compare-0.1.4/visual_compare/
--rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-0.1.4/visual_compare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.741408 visual-compare-0.1.4/visual_compare/doc/
--rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-0.1.4/visual_compare/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.741408 visual-compare-0.1.4/visual_compare/doc/image/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-0.1.4/visual_compare/doc/image/__init__.py
--rw-rw-rw-   0        0        0    29164 2023-05-11 09:04:51.000000 visual-compare-0.1.4/visual_compare/doc/image/compare_image.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 09:51:00.000000 visual-compare-0.1.4/visual_compare/doc/image/image.py
--rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-0.1.4/visual_compare/doc/image/ocr.py
--rw-rw-rw-   0        0        0     2974 2023-05-09 08:15:10.000000 visual-compare-0.1.4/visual_compare/doc/match.py
--rw-rw-rw-   0        0        0      549 2023-05-11 09:40:58.000000 visual-compare-0.1.4/visual_compare/doc/models.py
--rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-0.1.4/visual_compare/doc/pdf_test.py
--rw-rw-rw-   0        0        0    51123 2023-05-11 10:54:33.000000 visual-compare-0.1.4/visual_compare/doc/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.757008 visual-compare-0.1.4/visual_compare/tests/
--rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-0.1.4/visual_compare/tests/__init__.py
--rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-0.1.4/visual_compare/tests/conftest.py
--rw-rw-rw-   0        0        0     5322 2023-05-11 02:43:40.000000 visual-compare-0.1.4/visual_compare/tests/test_compare_image.py
--rw-rw-rw-   0        0        0     2839 2023-05-11 11:04:27.000000 visual-compare-0.1.4/visual_compare/tests/test_compare_pdf.py
--rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-0.1.4/visual_compare/tests/test_downloader.py
--rw-rw-rw-   0        0        0     1100 2023-05-11 10:06:36.000000 visual-compare-0.1.4/visual_compare/tests/test_image.py
--rw-rw-rw-   0        0        0     1599 2023-05-11 10:57:59.000000 visual-compare-0.1.4/visual_compare/tests/test_visual_test.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.757008 visual-compare-0.1.4/visual_compare/utils/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-0.1.4/visual_compare/utils/__init__.py
--rw-rw-rw-   0        0        0      639 2023-05-11 08:52:12.000000 visual-compare-0.1.4/visual_compare/utils/common.py
--rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-0.1.4/visual_compare/utils/downloader.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.741408 visual-compare-0.1.4/visual_compare.egg-info/
--rw-rw-rw-   0        0        0     2047 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      944 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-0.1.4/visual_compare.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      174 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 08:00:03.946754 visual-compare-1.0.0/
+-rw-rw-rw-   0        0        0     2023 2023-05-15 08:00:03.946754 visual-compare-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2023-05-15 07:25:08.000000 visual-compare-1.0.0/README.md
+-rw-rw-rw-   0        0        0      145 2023-05-15 08:00:03.946754 visual-compare-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-05-15 07:26:04.000000 visual-compare-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:00:03.891767 visual-compare-1.0.0/visual_compare/
+-rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-1.0.0/visual_compare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:00:03.914591 visual-compare-1.0.0/visual_compare/doc/
+-rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-1.0.0/visual_compare/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:00:03.918116 visual-compare-1.0.0/visual_compare/doc/image/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-1.0.0/visual_compare/doc/image/__init__.py
+-rw-rw-rw-   0        0        0    29164 2023-05-11 09:04:51.000000 visual-compare-1.0.0/visual_compare/doc/image/compare_image.py
+-rw-rw-rw-   0        0        0     3588 2023-05-15 02:33:50.000000 visual-compare-1.0.0/visual_compare/doc/image/image.py
+-rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-1.0.0/visual_compare/doc/image/ocr.py
+-rw-rw-rw-   0        0        0     2955 2023-05-12 09:18:28.000000 visual-compare-1.0.0/visual_compare/doc/match.py
+-rw-rw-rw-   0        0        0      568 2023-05-12 10:32:40.000000 visual-compare-1.0.0/visual_compare/doc/models.py
+-rw-rw-rw-   0        0        0     2164 2023-05-15 07:15:15.000000 visual-compare-1.0.0/visual_compare/doc/pdf.py
+-rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-1.0.0/visual_compare/doc/pdf_test.py
+-rw-rw-rw-   0        0        0    51498 2023-05-15 07:15:15.000000 visual-compare-1.0.0/visual_compare/doc/visual.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:00:03.942662 visual-compare-1.0.0/visual_compare/tests/
+-rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-1.0.0/visual_compare/tests/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-1.0.0/visual_compare/tests/conftest.py
+-rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-1.0.0/visual_compare/tests/test_downloader.py
+-rw-rw-rw-   0        0        0     1412 2023-05-15 02:03:24.000000 visual-compare-1.0.0/visual_compare/tests/test_image.py
+-rw-rw-rw-   0        0        0     3005 2023-05-12 08:28:40.000000 visual-compare-1.0.0/visual_compare/tests/test_ocr.py
+-rw-rw-rw-   0        0        0      799 2023-05-15 07:04:57.000000 visual-compare-1.0.0/visual_compare/tests/test_pdf.py
+-rw-rw-rw-   0        0        0     2139 2023-05-15 07:17:08.000000 visual-compare-1.0.0/visual_compare/tests/test_visual.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:00:03.946754 visual-compare-1.0.0/visual_compare/utils/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-1.0.0/visual_compare/utils/__init__.py
+-rw-rw-rw-   0        0        0     1002 2023-05-15 03:07:32.000000 visual-compare-1.0.0/visual_compare/utils/common.py
+-rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-1.0.0/visual_compare/utils/downloader.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:00:03.898228 visual-compare-1.0.0/visual_compare.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-05-15 08:00:03.000000 visual-compare-1.0.0/visual_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      942 2023-05-15 08:00:03.000000 visual-compare-1.0.0/visual_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 08:00:03.000000 visual-compare-1.0.0/visual_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-1.0.0/visual_compare.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      174 2023-05-15 08:00:03.000000 visual-compare-1.0.0/visual_compare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-15 08:00:03.000000 visual-compare-1.0.0/visual_compare.egg-info/top_level.txt
```

### Comparing `visual-compare-0.1.4/PKG-INFO` & `visual-compare-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 0.1.4
+Version: 1.0.0
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
@@ -30,48 +30,48 @@
 ```
 
 ## Examples
 
 ### Compare images ###
 
 ```python
-from visual_compare.doc.visual_test import VisualTest
+from visual_compare.doc.visual import Visual
 
 def get_path(filename):
     image_base = '../../files/images/'
     return image_base + filename
 
 reference_image = get_path('123.png')
 test_image = get_path('124.png')
-vt = VisualTest()
-res = vt.compare_images(reference_image, test_image)
+vt = Visual()
+is_diff, res = vt.compare_images(reference_image, test_image)
 print(res)
-assert vt.is_different is True
+assert is_diff is True
 ```
 
  Result as follows
 
 ![1.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/1.jpg)
 
 ### Compare images with mask ###
 
 ```python
-from visual_compare.doc.visual_test import VisualTest
+from visual_compare.doc.visual import Visual
 
 def get_path(filename):
     image_base = '../../files/images/'
     return image_base + filename
 
 reference_image = get_path('123.png')
 test_image = get_path('124.png')
 mask_images = [get_path('000.png')]
-vt = VisualTest()
+vt = Visual()
 mask = vt.generate_mask(reference_image, mask_images)
-res = vt.compare_images(reference_image, test_image, mask=mask)
+is_diff, res = vt.compare_images(reference_image, test_image, mask=mask)
 print(res)
-assert vt.is_different is True
+assert is_diff is True
 ```
 
  Result as follows
 
 ![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
```

### Comparing `visual-compare-0.1.4/README.md` & `visual-compare-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,47 +8,47 @@
 ```
 
 ## Examples
 
 ### Compare images ###
 
 ```python
-from visual_compare.doc.visual_test import VisualTest
+from visual_compare.doc.visual import Visual
 
 def get_path(filename):
     image_base = '../../files/images/'
     return image_base + filename
 
 reference_image = get_path('123.png')
 test_image = get_path('124.png')
-vt = VisualTest()
-res = vt.compare_images(reference_image, test_image)
+vt = Visual()
+is_diff, res = vt.compare_images(reference_image, test_image)
 print(res)
-assert vt.is_different is True
+assert is_diff is True
 ```
 
  Result as follows
 
 ![1.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/1.jpg)
 
 ### Compare images with mask ###
 
 ```python
-from visual_compare.doc.visual_test import VisualTest
+from visual_compare.doc.visual import Visual
 
 def get_path(filename):
     image_base = '../../files/images/'
     return image_base + filename
 
 reference_image = get_path('123.png')
 test_image = get_path('124.png')
 mask_images = [get_path('000.png')]
-vt = VisualTest()
+vt = Visual()
 mask = vt.generate_mask(reference_image, mask_images)
-res = vt.compare_images(reference_image, test_image, mask=mask)
+is_diff, res = vt.compare_images(reference_image, test_image, mask=mask)
 print(res)
-assert vt.is_different is True
+assert is_diff is True
 ```
 
  Result as follows
 
 ![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
```

### Comparing `visual-compare-0.1.4/setup.py` & `visual-compare-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="visual-compare",
-    version="0.1.4",
+    version="1.0.0",
     description="Image and PDF Compare",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/visual-compare",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
```

### Comparing `visual-compare-0.1.4/visual_compare/doc/image/compare_image.py` & `visual-compare-1.0.0/visual_compare/doc/image/compare_image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.4/visual_compare/doc/image/image.py` & `visual-compare-1.0.0/visual_compare/doc/match.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,30 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 -------------------------------------------------
-   File Name：      _base
+   File Name：      match
    Description:
    Author:          dingyong.cui
-   date：           2023/5/6
+   date：           2023/5/9
 -------------------------------------------------
    Change Activity:
-                    2023/5/6
+                    2023/5/9
 -------------------------------------------------
 """
+from os.path import splitext, split
+
 import cv2
 import numpy
-import os
 
+from visual_compare.doc.image.image import Image
 from visual_compare.doc.models import Mask
-from visual_compare.utils.common import is_url
-from visual_compare.utils.downloader import download_file_from_url
-
-
-class Image:
-
-    def __init__(self, image: str):
-        if is_url(image):
-            self._image = download_file_from_url(image)
-        else:
-            self._image = str(image)
-        if os.path.isfile(image) is False:
-            raise AssertionError('The image file does not exist: {}'.format(image))
-
-    @property
-    def image(self):
-        return cv2.imread(self._image, cv2.IMREAD_UNCHANGED)
 
-    @property
-    def width(self):
-        return self.image.shape[1]
 
-    @property
-    def height(self):
-        return self.image.shape[0]
-
-
-class MatchImg:
+class Match(object):
 
     def __init__(self, threshold=0.95, match_method=cv2.TM_CCOEFF_NORMED):
         self.threshold = threshold
         self.match_method = match_method
 
     def match_temp(self, source_image, temp_image, threshold, method=cv2.TM_CCOEFF_NORMED):
         if threshold is None:
@@ -56,18 +33,57 @@
             mt = cv2.matchTemplate(source_image, temp_image, method)
             locations = numpy.where(mt >= threshold)
 
             return list(zip(locations[1], locations[0]))
         except cv2.error as e:
             print(e)
 
-    def parse_mask(self, source: str, temp: str, threshold=None, match_method=cv2.TM_CCOEFF_NORMED, mask_type='coordinates', page='all'):
+    def parse_mask(self, source: str, temp: str, threshold: float, match_method: int, mask_type: str, page: str):
+        pass
+
+
+class MatchImg(Match):
+
+    def __init__(self, threshold=0.95, match_method=cv2.TM_CCOEFF_NORMED):
+        super().__init__(threshold, match_method)
+
+    def parse_mask(self, source: str, temp: str, threshold=None, match_method=cv2.TM_CCOEFF_NORMED,
+                   mask_type='coordinates', page='all'):
         source_img = Image(source)
         temp_img = Image(temp)
 
         mask_list = []
         match_list = self.match_temp(source_img.image, temp_img.image, threshold, match_method)
         for m in match_list:
             mask = Mask(type=mask_type, page=page, x=m[0], y=m[1], width=temp_img.width, height=temp_img.height)
             mask_list.append(mask.dict())
 
         return mask_list
+
+
+class MatchPdf(Match):
+
+    def __init__(self, source, temp: str, threshold=0.05, match_method=cv2.TM_CCOEFF_NORMED):
+        super().__init__(threshold, match_method)
+        if isinstance(source, str):
+            self.source_img = Image(source).image
+        else:
+            # self.source_img = cv2.cvtColor(source, cv2.COLOR_BGR2GRAY)
+            self.source_img = source
+        self.temp_img = Image(temp).image
+        self.threshold = threshold
+
+    def parse_mask(self, match_method=cv2.TM_CCOEFF_NORMED):
+        mask_list = []
+        match_list = self.match_temp(method=match_method)
+        for m in match_list:
+            mj = {
+                'type': 'coordinates',
+                "page": "all",
+                'x': m[0],
+                'y': m[1],
+                'width': self.temp_img.width,
+                'height': self.temp_img.height
+            }
+            mask_list.append(mj)
+
+        return mask_list
```

### Comparing `visual-compare-0.1.4/visual_compare/doc/image/ocr.py` & `visual-compare-1.0.0/visual_compare/doc/image/ocr.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.4/visual_compare/doc/models.py` & `visual-compare-1.0.0/visual_compare/doc/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,17 +8,17 @@
    date：           2023/5/11
 -------------------------------------------------
    Change Activity:
                     2023/5/11
 -------------------------------------------------
 """
 from pydantic import BaseModel
-from typing import Text
+from typing import Text, Union
 
 
 class Mask(BaseModel):
     type: Text
-    page: Text
+    page: Union[int, Text]
     x: int
     y: int
     width: int
     height: int
```

### Comparing `visual-compare-0.1.4/visual_compare/doc/pdf_test.py` & `visual-compare-1.0.0/visual_compare/doc/pdf_test.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.4/visual_compare/doc/visual_test.py` & `visual-compare-1.0.0/visual_compare/doc/visual.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 import fitz
 import imutils
 import numpy as np
 import pytesseract
 from skimage import metrics
 
 from visual_compare.doc.image.compare_image import CompareImage
-from visual_compare.utils.common import is_url
+from visual_compare.utils.common import is_url, check_file_exist
 
 logger = logging.getLogger(__name__)
 
 
-class VisualTest(object):
+class Visual(object):
     ROBOT_LIBRARY_VERSION = 0.2
     BORDER_FOR_MOVE_TOLERANCE_CHECK = 0
     DPI_DEFAULT = 200
     WATERMARK_WIDTH = 25
     WATERMARK_HEIGHT = 30
     WATERMARK_CENTER_OFFSET = 3 / 100
     FONT = cv2.FONT_HERSHEY_SIMPLEX
@@ -47,15 +47,16 @@
     LINE_TYPE = 2
     THRESHOLD = 0.95
     REFERENCE_LABEL = "Expected Result (Reference)"
     CANDIDATE_LABEL = "Actual Result (Candidate)"
     OCR_ENGINE = "tesseract"
     MOVEMENT_DETECTION = "classic"
 
-    def __init__(self, threshold: float = 0.0000, dpi: int = DPI_DEFAULT, take_screenshots: bool = False,
+    def __init__(self, threshold: float = 0.0000, dpi: int = DPI_DEFAULT,
+                 take_screenshots: bool = False,
                  show_diff: bool = False, ocr_engine: str = OCR_ENGINE, movement_detection: str = MOVEMENT_DETECTION,
                  watermark_file: str = None, screenshot_dir: str = None, screenshot_format: str = 'jpg', **kwargs):
         """
         | =Arguments= | =Description= |
         | ``take_screenshots`` | Shall screenshots be taken also for passed comparisons.   |
         | ``show_diff`` | Shall a diff screenshot be added showing differences in black and white  |
         | ``screenshot_format`` | Image format of screenshots, ``jpg`` or ``png`` |
@@ -83,20 +84,24 @@
         except TypeError:
             self.screenshot_dir = Path.cwd() / Path("screenshots/")
         if not (self.screenshot_format == 'jpg' or self.screenshot_format == 'png'):
             self.screenshot_format = 'jpg'
 
         self._is_different = False
 
+        # self.check_exist([reference_image, test_image])
+
+        self.reference_image = None
+        self.test_image = None
+
     @property
     def is_different(self):
         return self._is_different
 
-    @staticmethod
-    def generate_mask(reference_image: str, mask_images: Union[str, List[str]], threshold=THRESHOLD):
+    def generate_mask(self, reference_image: str, mask_images: Union[str, List[str]], threshold=THRESHOLD):
         """Generate mask base on ``reference_image`` and ``test_image``
 
         Result is a json for mask when matched success, otherwise None
 
         | =Arguments= | =Description= |
         | ``reference_image`` | Path or URL of the Reference Image/Document, your expected result. May be .pdf, .ps, .pcl or image files |
         | ``mask_images`` | List of the path or URL of the Reference Image/Document, your expected result. May be .pdf, .ps, .pcl or image files |
@@ -106,19 +111,26 @@
         | [{'type': 'coordinates', 'page': 'all', 'x': 724, 'y': 341, 'width': 139, 'height': 44}]
         | None
 
         """
         from visual_compare.doc.image.image import MatchImg
 
         mask = []
+
+        check_file_exist(mask_images)
+
         if isinstance(mask_images, str):
             mask_images = [mask_images]
+        ci = CompareImage(reference_image, DPI=self.DPI)
+        reference_opencv_images = ci.opencv_images
+        self.reference_image = ci.image
+
         m_img = MatchImg(threshold=threshold)
         for mi in mask_images:
-            res = m_img.parse_mask(source=reference_image, temp=mi)
+            res = m_img.parse_mask(source=reference_opencv_images, temp=mi)
             mask.extend(res)
 
         return mask if len(mask) > 0 else None
 
     def compare_images(self, reference_image: str, test_image: str, placeholder_file: Union[str, list] = None,
                        mask: Union[str, dict, list] = None, check_text_content: bool = False,
                        move_tolerance: int = None, contains_barcodes: bool = False, get_pdf_content: bool = False,
@@ -264,15 +276,15 @@
                 self._is_different = True
 
         logger.info("The compared images are equal")
 
         toc = time.perf_counter()
         logger.debug(f"Visual Image comparison performed in {toc - tic:0.4f} seconds")
 
-        return screenshot_names
+        return self._is_different, screenshot_names
 
     @staticmethod
     def get_images_with_highlighted_differences(thresh, reference, candidate, extension=10):
 
         thresh = cv2.dilate(thresh, None, iterations=extension)
         thresh = cv2.erode(thresh, None, iterations=extension)
         contours = cv2.findContours(thresh.copy(), cv2.RETR_EXTERNAL,
```

### Comparing `visual-compare-0.1.4/visual_compare/tests/test_downloader.py` & `visual-compare-1.0.0/visual_compare/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.4/visual_compare/tests/test_image.py` & `visual-compare-1.0.0/visual_compare/tests/test_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,13 +26,21 @@
     def test_parse_mask(self):
         img1 = self.get_path('123.png')
         img11 = self.get_path('000.png')
         img2 = self.get_path('124.png')
         res = self.cls().parse_mask(img1, img11)
         print(res)
 
-    def test_parse_mask(self):
+    def test_parse_mask_old(self):
         img1 = self.get_path('123.png')
         img11 = self.get_path('000.png')
         img2 = self.get_path('124.png')
         res = self.cls().parse_mask(img1, img11)
         print(res)
+
+    def test_parse_mask1(self):
+        from visual_compare.doc.image.compare_image import CompareImage
+        img = self.get_path('111.pdf')
+        img1 = CompareImage(img).opencv_images
+        img11 = self.get_path('333.png')
+        res = self.cls().parse_mask(img1, img11)
+        print(res)
```

### Comparing `visual-compare-0.1.4/visual_compare/tests/test_visual_test.py` & `visual-compare-1.0.0/visual_compare/tests/test_visual.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,67 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 -------------------------------------------------
-   File Name：      test_visual_test
+   File Name：      test_visual
    Description:
    Author:          dingyong.cui
-   date：           2023/5/11
+   date：           2023/5/12
 -------------------------------------------------
    Change Activity:
-                    2023/5/11
+                    2023/5/12
 -------------------------------------------------
 """
 
 
-class TestVisualTest:
+class TestVisual:
 
     def setup(self):
-        from visual_compare.doc.visual_test import VisualTest
-        self.cls = VisualTest
+        from visual_compare.doc.visual import Visual
+        self.cls = Visual
         self.image_base = '../../files/images/'
 
     def get_path(self, filename):
         return self.image_base + filename
 
-    def test_compare_images_with_mask(self):
+    def test_check_exist(self):
+        img1 = self.get_path('123.png')
+        img11 = self.get_path('000.png')
+        self.cls().check_exist([img1, img11])
+
+    def test_check_exist_fail(self):
+        img1 = self.get_path('123.png')
+        img11 = self.get_path('00000.png')
+        try:
+            self.cls().check_exist([img1, img11])
+        except AssertionError as e:
+            print(e)
+
+    def test_generate_mask(self):
         reference_image = self.get_path('123.png')
-        # mask_images = [self.get_path('000.png'), self.get_path('098.png')]
-        mask_images = [self.get_path('000.png')]
-        test_image = self.get_path('124.png')
+        mask_images = self.get_path('000.png')
+        res = self.cls().generate_mask(reference_image, mask_images)
+        print(res)
+
+    def test_generate_mask_pages(self):
+        reference_image = self.get_path('111.pdf')
+        mask_images = self.get_path('333.png')
+        res = self.cls().generate_mask(reference_image, mask_images)
+        print(res)
+
+    def test_compare_images(self):
+        img1 = self.get_path('123.png')
+        img2 = self.get_path('124.png')
         cls = self.cls()
-        mask = cls.generate_mask(reference_image, mask_images)
-        res = cls.compare_images(reference_image, test_image, mask=mask)
+        is_diff, res = cls.compare_images(img1, img2)
         print(res)
-        assert cls.is_different is True
+        assert is_diff is True
 
-    def test_compare_images_no_mask(self):
-        reference_image = self.get_path('123.png')
-        # mask_images = [self.get_path('000.png'), self.get_path('098.png')]
-        test_image = self.get_path('124.png')
+    def test_compare_images_with_mask(self):
+        img1 = self.get_path('123.png')
+        mask_images = self.get_path('000.png')
+        img2 = self.get_path('124.png')
         cls = self.cls()
-        # mask = cls.generate_mask(reference_image, mask_images)
-        res = cls.compare_images(reference_image, test_image)
+        mask = cls.generate_mask(img1, mask_images)
+        is_diff, res = cls.compare_images(img1, img2, mask=mask)
         print(res)
-        assert cls.is_different is False
+        assert is_diff is True
```

### Comparing `visual-compare-0.1.4/visual_compare/utils/downloader.py` & `visual-compare-1.0.0/visual_compare/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.4/visual_compare.egg-info/PKG-INFO` & `visual-compare-1.0.0/visual_compare.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 0.1.4
+Version: 1.0.0
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
@@ -30,48 +30,48 @@
 ```
 
 ## Examples
 
 ### Compare images ###
 
 ```python
-from visual_compare.doc.visual_test import VisualTest
+from visual_compare.doc.visual import Visual
 
 def get_path(filename):
     image_base = '../../files/images/'
     return image_base + filename
 
 reference_image = get_path('123.png')
 test_image = get_path('124.png')
-vt = VisualTest()
-res = vt.compare_images(reference_image, test_image)
+vt = Visual()
+is_diff, res = vt.compare_images(reference_image, test_image)
 print(res)
-assert vt.is_different is True
+assert is_diff is True
 ```
 
  Result as follows
 
 ![1.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/1.jpg)
 
 ### Compare images with mask ###
 
 ```python
-from visual_compare.doc.visual_test import VisualTest
+from visual_compare.doc.visual import Visual
 
 def get_path(filename):
     image_base = '../../files/images/'
     return image_base + filename
 
 reference_image = get_path('123.png')
 test_image = get_path('124.png')
 mask_images = [get_path('000.png')]
-vt = VisualTest()
+vt = Visual()
 mask = vt.generate_mask(reference_image, mask_images)
-res = vt.compare_images(reference_image, test_image, mask=mask)
+is_diff, res = vt.compare_images(reference_image, test_image, mask=mask)
 print(res)
-assert vt.is_different is True
+assert is_diff is True
 ```
 
  Result as follows
 
 ![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
```

### Comparing `visual-compare-0.1.4/visual_compare.egg-info/SOURCES.txt` & `visual-compare-1.0.0/visual_compare.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 visual_compare.egg-info/dependency_links.txt
 visual_compare.egg-info/not-zip-safe
 visual_compare.egg-info/requires.txt
 visual_compare.egg-info/top_level.txt
 visual_compare/doc/__init__.py
 visual_compare/doc/match.py
 visual_compare/doc/models.py
+visual_compare/doc/pdf.py
 visual_compare/doc/pdf_test.py
-visual_compare/doc/visual_test.py
+visual_compare/doc/visual.py
 visual_compare/doc/image/__init__.py
 visual_compare/doc/image/compare_image.py
 visual_compare/doc/image/image.py
 visual_compare/doc/image/ocr.py
 visual_compare/tests/__init__.py
 visual_compare/tests/conftest.py
-visual_compare/tests/test_compare_image.py
-visual_compare/tests/test_compare_pdf.py
 visual_compare/tests/test_downloader.py
 visual_compare/tests/test_image.py
-visual_compare/tests/test_visual_test.py
+visual_compare/tests/test_ocr.py
+visual_compare/tests/test_pdf.py
+visual_compare/tests/test_visual.py
 visual_compare/utils/__init__.py
 visual_compare/utils/common.py
 visual_compare/utils/downloader.py
```

