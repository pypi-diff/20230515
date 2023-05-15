# Comparing `tmp/cubetools-0.3.0.tar.gz` & `tmp/cubetools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.3.0.tar", last modified: Thu Apr  6 06:17:35 2023, max compression
+gzip compressed data, was "dist/cubetools-0.3.1.tar", last modified: Mon May 15 01:21:33 2023, max compression
```

## Comparing `cubetools-0.3.0.tar` & `cubetools-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-06 06:17:35.000000 cubetools-0.3.0/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2109 2023-04-06 06:17:35.000000 cubetools-0.3.0/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1033 2023-04-03 13:20:28.000000 cubetools-0.3.0/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-06 06:17:35.000000 cubetools-0.3.0/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.0/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9881 2023-03-31 00:50:39.000000 cubetools-0.3.0/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.0/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.0/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 06:17:33.000000 cubetools-0.3.0/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.0/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.0/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.0/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-06 06:17:35.000000 cubetools-0.3.0/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2109 2023-04-06 06:17:35.000000 cubetools-0.3.0/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      439 2023-04-06 06:17:35.000000 cubetools-0.3.0/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-04-06 06:17:35.000000 cubetools-0.3.0/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-04-06 06:17:35.000000 cubetools-0.3.0/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-04-06 06:17:35.000000 cubetools-0.3.0/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-04-06 06:17:35.000000 cubetools-0.3.0/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-04-06 06:17:35.000000 cubetools-0.3.0/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-04-06 06:17:33.000000 cubetools-0.3.0/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 01:21:33.000000 cubetools-0.3.1/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2109 2023-05-15 01:21:33.000000 cubetools-0.3.1/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1033 2023-04-03 13:20:28.000000 cubetools-0.3.1/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 01:21:33.000000 cubetools-0.3.1/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.1/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:20:55.000000 cubetools-0.3.1/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.1/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.1/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.1/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.1/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.1/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.1/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 01:21:33.000000 cubetools-0.3.1/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2109 2023-05-15 01:21:33.000000 cubetools-0.3.1/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      439 2023-05-15 01:21:33.000000 cubetools-0.3.1/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-15 01:21:33.000000 cubetools-0.3.1/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-15 01:21:33.000000 cubetools-0.3.1/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-15 01:21:33.000000 cubetools-0.3.1/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-15 01:21:33.000000 cubetools-0.3.1/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-15 01:21:33.000000 cubetools-0.3.1/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-15 01:21:29.000000 cubetools-0.3.1/setup.py
```

### Comparing `cubetools-0.3.0/PKG-INFO` & `cubetools-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.0
+Version: 0.3.1
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.3.0/README.md` & `cubetools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.0/cubetools/image_tools.py` & `cubetools-0.3.1/cubetools/image_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,27 @@
 from PIL import Image, ExifTags, ImageDraw, ImageFont
 
 
 def read_img(img):
     """
     从输入参数读取图像，转换成二进制字节流格式
     :param img:
-        存在5种可能形式：
+        存在6种可能形式：
+            - PIL Image
             - np.ndarray格式的图像数据（默认为RGB格式）
             - 图像文件路径名
             - 图像文件二进制字节流
             - 图像文件二进制字节流的base64编码字符串
             - 图像文件二进制字节流的base64编码URL字符串
     :return: (PIL.Image格式的图像对象, np.ndarray格式的图像数据(RGB格式))
     """
     try:
+        if isinstance(img, Image.Image):
+            return img, np.asarray(img)
+
         if isinstance(img, np.ndarray):
             return np2pil(img), img
 
         if isinstance(img, bytes):
             img_pil = bin2pil(img)
             img = np.asarray(img_pil)
             return img_pil, img
```

### Comparing `cubetools-0.3.0/cubetools/mindspore_lite_predict.py` & `cubetools-0.3.1/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.0/cubetools/onnx_predict.py` & `cubetools-0.3.1/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.0/cubetools/openvino_predict.py` & `cubetools-0.3.1/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.0/cubetools/paddle_predict.py` & `cubetools-0.3.1/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.0/cubetools/video_capture.py` & `cubetools-0.3.1/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.0/cubetools/video_predict.py` & `cubetools-0.3.1/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.0/cubetools.egg-info/PKG-INFO` & `cubetools-0.3.1/cubetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.0
+Version: 0.3.1
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.3.0/setup.py` & `cubetools-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.3.0',
+    version='0.3.1',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

