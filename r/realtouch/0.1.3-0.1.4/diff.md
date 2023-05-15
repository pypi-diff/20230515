# Comparing `tmp/realtouch-0.1.3.tar.gz` & `tmp/realtouch-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtouch-0.1.3.tar", last modified: Sun May 14 09:14:50 2023, max compression
+gzip compressed data, was "realtouch-0.1.4.tar", last modified: Sun May 14 23:20:08 2023, max compression
```

## Comparing `realtouch-0.1.3.tar` & `realtouch-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 09:14:50.849645 realtouch-0.1.3/
--rw-r--r--   0 k          (501) staff       (20)    35148 2023-05-12 00:09:36.000000 realtouch-0.1.3/LICENSE
--rw-r--r--   0 k          (501) staff       (20)      539 2023-05-14 09:14:50.849402 realtouch-0.1.3/PKG-INFO
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 09:14:50.845266 realtouch-0.1.3/realtouch/
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 09:14:50.847258 realtouch-0.1.3/realtouch/src/
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 09:14:50.848975 realtouch-0.1.3/realtouch/src/realtouch.egg-info/
--rw-r--r--   0 k          (501) staff       (20)      539 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/PKG-INFO
--rw-r--r--   0 k          (501) staff       (20)      277 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/SOURCES.txt
--rw-r--r--   0 k          (501) staff       (20)        1 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/dependency_links.txt
--rw-r--r--   0 k          (501) staff       (20)       16 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/requires.txt
--rw-r--r--   0 k          (501) staff       (20)       10 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/top_level.txt
--rw-r--r--   0 k          (501) staff       (20)    18556 2023-05-14 09:14:04.000000 realtouch-0.1.3/realtouch/src/realtouch.py
--rw-r--r--   0 k          (501) staff       (20)       38 2023-05-14 09:14:50.849728 realtouch-0.1.3/setup.cfg
--rw-r--r--   0 k          (501) staff       (20)      852 2023-05-14 09:14:31.000000 realtouch-0.1.3/setup.py
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 23:20:08.583605 realtouch-0.1.4/
+-rw-r--r--   0 k          (501) staff       (20)    35148 2023-05-12 00:09:36.000000 realtouch-0.1.4/LICENSE
+-rw-r--r--   0 k          (501) staff       (20)      539 2023-05-14 23:20:08.583015 realtouch-0.1.4/PKG-INFO
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 23:20:08.574647 realtouch-0.1.4/realtouch/
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 23:20:08.578037 realtouch-0.1.4/realtouch/src/
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 23:20:08.582245 realtouch-0.1.4/realtouch/src/realtouch.egg-info/
+-rw-r--r--   0 k          (501) staff       (20)      539 2023-05-14 23:20:08.000000 realtouch-0.1.4/realtouch/src/realtouch.egg-info/PKG-INFO
+-rw-r--r--   0 k          (501) staff       (20)      277 2023-05-14 23:20:08.000000 realtouch-0.1.4/realtouch/src/realtouch.egg-info/SOURCES.txt
+-rw-r--r--   0 k          (501) staff       (20)        1 2023-05-14 23:20:08.000000 realtouch-0.1.4/realtouch/src/realtouch.egg-info/dependency_links.txt
+-rw-r--r--   0 k          (501) staff       (20)       16 2023-05-14 23:20:08.000000 realtouch-0.1.4/realtouch/src/realtouch.egg-info/requires.txt
+-rw-r--r--   0 k          (501) staff       (20)       10 2023-05-14 23:20:08.000000 realtouch-0.1.4/realtouch/src/realtouch.egg-info/top_level.txt
+-rw-r--r--   0 k          (501) staff       (20)    20882 2023-05-14 23:14:48.000000 realtouch-0.1.4/realtouch/src/realtouch.py
+-rw-r--r--   0 k          (501) staff       (20)       38 2023-05-14 23:20:08.583806 realtouch-0.1.4/setup.cfg
+-rw-r--r--   0 k          (501) staff       (20)      852 2023-05-14 14:56:19.000000 realtouch-0.1.4/setup.py
```

### Comparing `realtouch-0.1.3/LICENSE` & `realtouch-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `realtouch-0.1.3/PKG-INFO` & `realtouch-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtouch
-Version: 0.1.3
+Version: 0.1.4
 Summary: realTouch Robot SDK
 Home-page: https://realtouch.dev
 Author: realTouch Dev
 Author-email: contact@realtouch.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `realtouch-0.1.3/realtouch/src/realtouch.egg-info/PKG-INFO` & `realtouch-0.1.4/realtouch/src/realtouch.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtouch
-Version: 0.1.3
+Version: 0.1.4
 Summary: realTouch Robot SDK
 Home-page: https://realtouch.dev
 Author: realTouch Dev
 Author-email: contact@realtouch.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `realtouch-0.1.3/realtouch/src/realtouch.py` & `realtouch-0.1.4/realtouch/src/realtouch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import hashlib
 import json
 from dataclasses import dataclass, asdict
 from enum import Enum
-from typing import Union
+from typing import Union, Any
 import requests
 from loguru import logger
 import re
+from pathlib import Path
+import base64
 
 
 @dataclass
 class ImgArea:
     start_x: float = 0
     end_x: float = 1
     start_y: float = 0
@@ -24,27 +27,52 @@
     MIDDLE = ImgArea(0, 1, 0.25, 0.75)
     HEAD = ImgArea(0, 1, 0, 0.25)
     HEADLINE = ImgArea(0, 1, 0, 0.1)
     TAIL = ImgArea(0, 1, 0.75, 1)
     FOOT = ImgArea(0, 1, 0.9, 1)
 
 
+@dataclass
+class TemplateLocation:
+    points: list[Union[tuple[int, int], list[int]]]
+    center: tuple[Union[int, float], Union[int, float]] = (-1, -1)
+    found: bool = False
+    size: int = 0
+
+
 class TextAction(Enum):
     KEYCODE_NEXT = 'KEYCODE_NEXT'
     KEYCODE_PREVIOUS = 'KEYCODE_PREVIOUS'
     KEYCODE_DONE = 'KEYCODE_DONE'
     KEYCODE_SEARCH = 'KEYCODE_SEARCH'
     KEYCODE_SEND = 'KEYCODE_SEND'
     KEYCODE_GO = 'KEYCODE_GO'
     KEYCODE_DELETE = 'KEYCODE_DELETE'
     KEYCODE_DELETE_ALL = 'KEYCODE_DELETE_ALL'
     KEYCODE_MAIN_KEYBOARD = 'KEYCODE_MAIN_KEYBOARD'
     KEYCODE_CLOSE = 'KEYCODE_CLOSE'
 
 
+def location_serialize(location: Union[
+    ImgLocation, list[ImgLocation],
+    ImgArea, list[ImgArea]] = ImgLocation.FULL):
+    try:
+        if not isinstance(location, list) and not isinstance(location, tuple):
+            location = [location]
+        result = []
+        for loc in location:
+            if isinstance(loc, ImgLocation):
+                result.append(loc.name)
+            else:
+                result.append(asdict(loc))
+        return result
+    except Exception as e:
+        logger.exception(e)
+        return location
+
 class Robot:
     def __init__(self, ip: str):
         self.ip = ip
         self._phones: dict[int, Phone] = {}
         self.__load()
 
     def __load(self):
@@ -69,16 +97,20 @@
     def phone(self, position: int) -> 'Phone':
         return self._phones.get(position)
 
     @property
     def phones(self) -> dict[int, 'Phone']:
         return self._phones
 
-    def call_func(self, position, path, **kwargs) -> Union[dict, bytes, str]:
+    def call_func(self, position, path, **kwargs) -> Any:
         phone = self.phone(position)
+
+        if 'location' in kwargs:
+            kwargs['location'] = location_serialize(kwargs['location'])
+
         if phone:
             headers = {
                 'PhonePosition': str(phone.position)
             }
         else:
             headers = {}
         result = requests.post(
@@ -255,15 +287,15 @@
         :param contain: 包含还是完全匹配
         :return:
         """
         if not isinstance(texts, list):
             texts = [texts]
         return self.phone.robot.call_func(
             self.phone.position, 'screen/has_texts', texts=list(map(str, texts)),
-            location=self.phone.location_serialize(location),
+            location=location,
             contain=contain
         )
 
     def has_any_texts(self, texts: list[str, re.Pattern], prev=False, ignore_case=True,
                       location: Union[ImgLocation, list[ImgLocation], ImgArea, list[ImgArea]] = ImgLocation.FULL,
                       contain=True, k=1):
         """
@@ -276,15 +308,15 @@
         :param k: 至少需要几个
         :return:
         """
         # self.logger.debug(f'{texts=} {prev=} {ignore_case=} {location=} {contain=} {k=}')
         return self.phone.robot.call_func(
             self.phone.position, 'screen/has_any_texts',
             texts=list(map(str, texts)),
-            location=self.phone.location_serialize(location),
+            location=location,
             contain=contain
         )
 
     def count_texts(self, texts: Union[list[str, re.Pattern], Union[str, re.Pattern]], prev=False, ignore_case=True,
                     location: Union[ImgLocation, list[ImgLocation], ImgArea, list[ImgArea]] = ImgLocation.FULL,
                     contain=True):
         """
@@ -297,15 +329,15 @@
         :return:
         """
         if not isinstance(texts, list):
             texts = [texts]
         return self.phone.robot.call_func(
             self.phone.position, 'screen/count_texts',
             texts=list(map(str, texts)),
-            location=self.phone.location_serialize(location),
+            location=location,
             contain=contain
         )
 
     def update(self, text=True):
         """
         更新屏幕图像和文字
         :param text: 是否更新文字
@@ -386,14 +418,71 @@
             'screen/clear_folder', folder=folder
         )
 
     def clear_midea(self):
         for folder in ['DCIM', 'Pictures']:
             self.clear_folder(folder)
 
+    def locate_image(
+            self, template: Union[Path, bytes],
+            image: Union[Path, bytes] = None,
+            location: Union[ImgLocation, list[ImgLocation], ImgArea, list[ImgArea]] = ImgLocation.FULL,
+            threshold=0.8
+    ) -> list[TemplateLocation]:
+        """
+        图查图. 仅作为实验用途. 如果效果可能不完美, 可以自行使用其它库去实现.
+
+        :param template: 被查找的模版路径或者bytes
+        :param image: 默认查找当前手机画面, 也可以提供被查图的路径或bytes
+        :param location: 只查找指定位置
+        :param threshold: 特征点集合阈值 , 0-∞, 越小越严格, 越大越宽松
+        :return:
+        """
+
+        def read_img(path):
+            if not path:
+                return path
+            if isinstance(path, bytes):
+                content = path
+            else:
+                with open(path, 'rb') as fin:
+                    content = fin.read()
+            return base64.b64encode(content).decode()
+
+        template_content = read_img(template)
+        img_content = read_img(image if image is not None else self.image_raw)
+
+        res = self.phone.robot.call_func(
+            self.phone.position,
+            'screen/locate-image',
+            template=template_content,
+            image=img_content,
+            location=location,
+            threshold=threshold,
+        )
+        result = []
+        for loc in res:
+            result.append(TemplateLocation(**loc))
+        return result
+
+    def show_keyboard(self):
+        """
+        显示输入法键盘
+        可以自行调用 enter_text(TextAction) 去实现其它功能
+        :return:
+        """
+        return self.enter_text(TextAction.KEYCODE_MAIN_KEYBOARD)
+
+    def hide_keyboard(self):
+        """
+        隐藏输入法键盘
+        :return:
+        """
+        return self.enter_text(TextAction.KEYCODE_CLOSE)
+
 
 class Phone:
     def __init__(
             self,
             position: int,
             robot: Robot,
             data: dict
@@ -415,22 +504,23 @@
     def calibrated(self) -> bool:
         """
         是否已经校准
         :return:
         """
         return self.robot.call_func(self.position, 'self/is-calibrated')
 
-    def upload(self, file):
+    def upload(self, file, name=None):
         """
         上传文件到手机
-        :param file:
+        :param file: 文件路径
+        :param name: 自定义文件名, 需要包含扩展名!!
         :return:
         """
         with open(file, 'rb') as f:
-            files = {'file': f}
+            files = {'file': f if not name else (name, f)}
             url = f'http://{self.robot.ip}/api/upload/{self.position}/'
             requests.post(
                 url, files=files,
                 timeout=(100, 100)
             )
 
     def touch(self, x: Union[int, float] = None, y: Union[int, float] = None, z: Union[int, float] = None,
@@ -533,28 +623,14 @@
         """
         用相机拍照
         :param move: 是否移动的对应的拍照点
         :return:
         """
         return self.robot.call_func(self.position, 'self/take_picture')
 
-    @staticmethod
-    def location_serialize(location: Union[
-        ImgLocation, list[ImgLocation],
-        ImgArea, list[ImgArea]] = ImgLocation.FULL):
-        if not isinstance(location, list) and not isinstance(location, tuple):
-            location = [location]
-        result = []
-        for loc in location:
-            if isinstance(loc, ImgLocation):
-                result.append(loc.name)
-            else:
-                result.append(asdict(location))
-        return result
-
     def touch_text(self, text: Union[str, re.Pattern],
                    index=0,
                    location: Union[
                        ImgLocation, list[ImgLocation],
                        ImgArea, list[ImgArea]] = ImgLocation.FULL,
                    contain=True,
                    offset: tuple[float, float] = (0.0, 0.0), jitter_x=True):
@@ -569,15 +645,15 @@
         :return:
         """
         return self.robot.call_func(
             self.position,
             'self/touch_text',
             text=str(text),
             index=0,
-            location=self.location_serialize(location),
+            location=location,
             contain=contain,
             offset=list(offset),
             jitter_x=jitter_x
         )
 
     def move(self, x: Union[int, float] = None, y: Union[int, float] = None, z: Union[int, float] = None,
              speed: Union[int, float] = None, raw=False, wait=False):
```

### Comparing `realtouch-0.1.3/setup.py` & `realtouch-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="realtouch",
-    version="0.1.3",
+    version="0.1.4",
     author="realTouch Dev",
     author_email="contact@realtouch.dev",
     description="realTouch Robot SDK",
     long_description="realTouch Robot SDK",
     long_description_content_type="text/markdown",
     url="https://realtouch.dev",
     packages=find_packages(),
```

