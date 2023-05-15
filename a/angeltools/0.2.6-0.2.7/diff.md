# Comparing `tmp/angeltools-0.2.6.tar.gz` & `tmp/angeltools-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angeltools-0.2.6.tar", last modified: Fri Mar 31 00:53:09 2023, max compression
+gzip compressed data, was "angeltools-0.2.7.tar", last modified: Mon May 15 09:06:42 2023, max compression
```

## Comparing `angeltools-0.2.6.tar` & `angeltools-0.2.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-03-31 00:53:09.424180 angeltools-0.2.6/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.2.6/LICENSE
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-03-31 00:53:09.424180 angeltools-0.2.6/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.2.6/README.md
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-03-31 00:53:09.420180 angeltools-0.2.6/angeltools/
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-03-31 00:53:09.424180 angeltools-0.2.6/angeltools/Db/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.2.6/angeltools/Db/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3289 2022-04-21 02:57:31.000000 angeltools-0.2.6/angeltools/Db/redis_connector.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     4862 2022-04-25 02:13:03.000000 angeltools-0.2.6/angeltools/ImageTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.2.6/angeltools/MathTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8113 2023-03-31 00:52:10.000000 angeltools-0.2.6/angeltools/Slavers.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    13732 2023-03-30 08:27:56.000000 angeltools-0.2.6/angeltools/StrTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     1405 2022-04-21 02:57:09.000000 angeltools-0.2.6/angeltools/TimeTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.2.6/angeltools/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6425 2023-03-30 08:28:51.000000 angeltools-0.2.6/angeltools/commands.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-03-31 00:53:09.424180 angeltools-0.2.6/angeltools/fdfs/
--rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.2.6/angeltools/fdfs/__init__.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-03-31 00:53:09.424180 angeltools-0.2.6/angeltools/fdfs/fdfs_client/
--rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/connection.py
--rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/exceptions.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/fdfs_protol.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/fdfs_test.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/storage_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/tracker_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_client/utils.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.2.6/angeltools/fdfs/fdfs_operator.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-03-31 00:53:09.424180 angeltools-0.2.6/angeltools.egg-info/
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-03-31 00:53:09.000000 angeltools-0.2.6/angeltools.egg-info/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-03-31 00:53:09.000000 angeltools-0.2.6/angeltools.egg-info/SOURCES.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-03-31 00:53:09.000000 angeltools-0.2.6/angeltools.egg-info/dependency_links.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-03-31 00:53:09.000000 angeltools-0.2.6/angeltools.egg-info/entry_points.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.2.6/angeltools.egg-info/not-zip-safe
--rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-03-31 00:53:09.000000 angeltools-0.2.6/angeltools.egg-info/requires.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-03-31 00:53:09.000000 angeltools-0.2.6/angeltools.egg-info/top_level.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-03-31 00:53:09.424180 angeltools-0.2.6/setup.cfg
--rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-03-31 00:52:21.000000 angeltools-0.2.6/setup.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.2.7/LICENSE
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-15 09:06:42.418693 angeltools-0.2.7/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.2.7/README.md
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools/
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools/Db/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.2.7/angeltools/Db/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3289 2022-04-21 02:57:31.000000 angeltools-0.2.7/angeltools/Db/redis_connector.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.2.7/angeltools/ImageTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.2.7/angeltools/MathTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.2.7/angeltools/Slavers.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    14085 2023-05-15 08:54:56.000000 angeltools-0.2.7/angeltools/StrTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.2.7/angeltools/TimeTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.2.7/angeltools/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.2.7/angeltools/commands.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools/fdfs/
+-rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.2.7/angeltools/fdfs/__init__.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools/fdfs/fdfs_client/
+-rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/connection.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/exceptions.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/fdfs_protol.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/fdfs_test.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/storage_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/tracker_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/utils.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_operator.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools.egg-info/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/entry_points.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.2.7/angeltools.egg-info/not-zip-safe
+-rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/requires.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/top_level.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-05-15 09:06:42.418693 angeltools-0.2.7/setup.cfg
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-05-15 09:06:08.000000 angeltools-0.2.7/setup.py
```

### Comparing `angeltools-0.2.6/LICENSE` & `angeltools-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/PKG-INFO` & `angeltools-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.2.6
+Version: 0.2.7
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.2.6/README.md` & `angeltools-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/Db/__init__.py` & `angeltools-0.2.7/angeltools/Db/__init__.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/Db/redis_connector.py` & `angeltools-0.2.7/angeltools/Db/redis_connector.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/ImageTool.py` & `angeltools-0.2.7/angeltools/ImageTool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 # -*- coding: utf-8 -*-
 import io
 import os
 import sys
 from pathlib import Path
 
-import requests
-from numpy import array
-from tqdm import tqdm
-
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
-import pygame
 
 
 def image2chars(image_path, width=120, k=1.0, reverse=False, outfile=None, chart_list=None):
     """
     照片转为字符，默认120个字符宽度
     """
     from PIL import Image
@@ -51,14 +46,15 @@
     :param size:
     :param font_color:
     :param back_color:
     :param save_path:
     :param font_path:
     :return:
     """
+    import pygame
 
     font_path = check_font_path(font_path)
     size = int(size) if size else 50
     font_color = tuple(font_color) if font_color else (0, 0, 0)
     back_color = tuple(back_color) if back_color else (255, 255, 255)
 
     if save_path:
@@ -73,15 +69,15 @@
     font = pygame.font.Font(font_path, size)
     render_text = font.render(text, True, font_color, back_color)
 
     pygame.image.save(render_text, save_path)
     return save_path
 
 
-def strip_empty_line(arr: array):
+def strip_empty_line(arr):
 
     r_temp = [sum(r) for r in arr]
     rs = get_empty_line_start(r_temp)
     re = get_empty_line_start(r_temp[::-1])
     re = len(r_temp) - re
 
     r_temp_t = [sum(r) for r in arr.T]
@@ -101,14 +97,17 @@
             has_empty = True
         else:
             break
     return rs + 1 if has_empty else rs
 
 
 def check_font_path(font_path):
+    from tqdm import tqdm
+    import requests
+
     if font_path and os.path.exists(font_path):
         return font_path
     base_path = Path(__file__).parent
     local_font_dir = base_path / 'fonts'
     local_msyh_font_path = local_font_dir / 'msyh-B.ttf'
     if os.path.exists(local_msyh_font_path.absolute()):
         return local_msyh_font_path
```

### Comparing `angeltools-0.2.6/angeltools/MathTool.py` & `angeltools-0.2.7/angeltools/MathTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/Slavers.py` & `angeltools-0.2.7/angeltools/Slavers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import logging
 import os
 import sys
 import threading
 import time
 import random
 import traceback
-from multiprocessing import Pool as Mpp
-from multiprocessing.dummy import Pool as ThreadPool
-
-import tqdm
-from tqdm.contrib.concurrent import process_map, thread_map
 
 
 class MWT(threading.Thread):
     def __init__(self, function, params):
         threading.Thread.__init__(self)
         self.func = function
         self.params = params
@@ -49,14 +44,16 @@
 
     def work(self, func, params_list: list, default=None, list_flat=False, remove_item_if_empty=False):
         start_time = time.time()
         func_name = func.__name__
         self._say_name(func_name=func_name)
         try:
             if self.with_tq:
+                import tqdm
+
                 tq = tqdm.tqdm(total=len(params_list))
                 res_data = self.map_list(func, params_list, tq=tq)
                 tq.close()
             else:
                 res_data = self.map_list(func, params_list)
 
             if list_flat and isinstance(res_data, list) and isinstance(res_data[0], list):
@@ -104,17 +101,16 @@
 
     def __init__(self, workers=None, with_tq=False, name=None):
         """
         :param workers:     线程数
         :param with_tq:     使用tqdm
         :param name:        任务名称
         """
-        self.pool = ThreadPool(workers if workers else 10)
         self.with_tq = with_tq
-        self.workers = workers
+        self.workers = workers if workers else 10
         self.name = name
 
     def _say_name(self, func_name=None):
         if self.name:
             if isinstance(self.name, str):
                 mission_name = self.name
             else:
@@ -124,17 +120,22 @@
     def work(self, func, params_list: list, default=None, list_flat=False, remove_item_if_empty=False):
         start_time = time.time()
         func_name = func.__name__
         self._say_name(func_name=func_name)
         try:
 
             if self.with_tq:
+                from tqdm.contrib.concurrent import thread_map
+
                 res_data = thread_map(func, params_list, max_workers=self.workers)
             else:
-                res_data = self.pool.map(func, params_list)
+                from multiprocessing.dummy import Pool as ThreadPool
+
+                pool = ThreadPool(self.workers)
+                res_data = pool.map(func, params_list)
             if list_flat and isinstance(res_data, list) and isinstance(res_data[0], list):
                 if remove_item_if_empty:
                     res_data = [item for sublist in res_data for item in sublist if item]
                 else:
                     res_data = [item for sublist in res_data for item in sublist]
 
             end_time = time.time()
@@ -184,16 +185,20 @@
     def work(self, func, params_list: list, default=None, list_flat=False, remove_item_if_empty=False):
         start_time = time.time()
         func_name = func.__name__
         self._say_name(func_name=func_name)
 
         try:
             if self.with_tq:
+                from tqdm.contrib.concurrent import process_map
+
                 res_data = process_map(func, params_list, max_workers=self.workers, chunksize=1000)
             else:
+                from multiprocessing import Pool as Mpp
+
                 pool = Mpp(self.workers)
                 res_data = pool.map(func, params_list)
 
             if list_flat and isinstance(res_data, list) and isinstance(res_data[0], list):
                 if remove_item_if_empty:
                     res_data = [item for sublist in res_data for item in sublist if item]
                 else:
```

### Comparing `angeltools-0.2.6/angeltools/StrTool.py` & `angeltools-0.2.7/angeltools/StrTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,19 @@
 import os
 import random
 import re
 import sys
 import time
 import uuid
 from pathlib import Path
-from urllib.parse import quote, urlparse, unquote
-
-import urllib3
-from BaseColor.base_colors import hgreen, hred
-from pypinyin import lazy_pinyin
-from scrapy import Selector
-from scrapy.http import HtmlResponse
-
-from angeltools.Slavers import Slaves
 
 
 def get_domain(url):
+    import urllib3
+
     domain = urllib3.get_host(url)[1]
     if domain.startswith('www.'):
         domain = domain.lstrip('www.')
     return domain
 
 
 def hash_str(data):
@@ -42,27 +35,32 @@
 
 
 class ScrapyXpath:
     """
     包装 scrapy response 的xpath方法，不用每次都 extract 再判断结果，使爬虫更整洁
     也可以传入由 requests 获取的 response text 和 url，变成 scrapy selector 对象方便提取
     """
+    from scrapy import Selector
+
     def __init__(self, scrapy_selector: Selector = None, url=None, html_content=None):
         """
         :param scrapy_selector:     response.xpath('//div[@class="xxx"]')
         """
+        from scrapy.http import HtmlResponse
+
+        self.HtmlResponse = HtmlResponse
         if scrapy_selector:
             self.raw = scrapy_selector
         elif url and html_content:
             self.raw = self.response_selector(url, html_content)
         else:
             raise ValueError('scrapy_selector or url and html_content required!')
 
     def scrapy_response(self, url, html_content):
-        return HtmlResponse(url=url, body=html_content, encoding="utf-8")
+        return self.HtmlResponse(url=url, body=html_content, encoding="utf-8")
 
     def response_selector(self, url, html_content):
         return self.scrapy_response(url, html_content).xpath('//html')
 
     def __map_str(self, map_dic, raw_str):
         if map_dic:
             n_res = ""
@@ -115,34 +113,39 @@
                     nw = sep.join(nw)
                 return nw
         return default
 
 
 class UrlFormat:
     def __init__(self, url=None):
+        from urllib.parse import quote, urlparse, unquote
+
+        self.quote = quote
+        self.urlparse = urlparse
+        self.unquote = unquote
         self.url = url
 
     def quote_str(self, s):
-        res = quote(str(s).encode())
+        res = self.quote(str(s).encode())
         return res
 
     def unquote_str(self, s):
-        res = unquote(s)
+        res = self.unquote(s)
         return res
 
     def make_url(self, base, params_add_dic, quote_param=True):
         new_url = base
         new_url += f'?{"&".join([f"{k}={self.quote_str(v) if quote_param else v}" for k, v in params_add_dic.items()])}'
         return new_url
 
     def split_url(self):
         url_data = dict()
         if self.url:
-            temp_data = urlparse(unquote(self.url))
-            url_data["queries"] = {x.split("=")[0]: unquote("=".join(x.split("=")[1:])) for x in temp_data.query.split("&")}
+            temp_data = self.urlparse(self.unquote(self.url))
+            url_data["queries"] = {x.split("=")[0]: self.unquote("=".join(x.split("=")[1:])) for x in temp_data.query.split("&")}
             url_data["host"] = temp_data.netloc
             url_data["protocol"] = temp_data.scheme
             url_data["path"] = temp_data.path
             url_data["require_params"] = temp_data.params
             url_data["fragment"] = temp_data.fragment
         return url_data
 
@@ -338,31 +341,35 @@
         self.__exit_lock()
         return lock_time
 
 
 class SortedWithFirstPinyin(object):
 
     def __init__(self, file_path, save_path=None, full_match=False, reverse=False):
+        from BaseColor.base_colors import hred
+        from pypinyin import lazy_pinyin
+
         file_path = Path(file_path)
         if not os.path.exists(str(file_path.absolute())):
             print(f"No such file: {hred(file_path.absolute())}")
             sys.exit(1)
         self.file_path = file_path
+        self.lazy_pinyin = lazy_pinyin
 
         if not save_path:
             save_path_split = self.file_path.name.split('.')
             file_name = '.'.join(save_path_split[:-1])
             sub = save_path_split[-1]
             save_path = self.file_path.parent / f"{file_name}_sorted.{sub}"
         self.save_path = str(Path(save_path).absolute())
         self.full_match = full_match
         self.reverse = reverse
 
     def get_pinyin_first(self, text):
-        return lazy_pinyin(text)[0][0] if not self.full_match else lazy_pinyin(text)[0]
+        return self.lazy_pinyin(text)[0][0] if not self.full_match else self.lazy_pinyin(text)[0]
 
     def get_pinyin(self, text):
         if not re.findall(r'[\ue4e00-\u9fa5]', text):
             return text
 
         n_line = ''
         for i in text:
@@ -370,14 +377,16 @@
                 lt = self.get_pinyin_first(i)
             else:
                 lt = i
             n_line += lt
         return ''.join(n_line)
 
     def run(self):
+        from angeltools.Slavers import Slaves
+        from BaseColor.base_colors import hgreen
 
         with open(self.file_path, 'r') as rf:
             lines = rf.readlines()
         lines = [x for x in lines if x.strip()]
         py_raw_lines_map = {}
         py_lines = Slaves().work(self.get_pinyin, lines)
         for raw, py in zip(lines, py_lines):
@@ -411,12 +420,12 @@
     #
     # BigSlaves(7).work(do_job, [x for x in "ABCDEFGHIJKLMN"])
 
     # uf = UrlFormat('http://www.baidu.com?page=1&user=me&name=%E5%BC%A0%E4%B8%89')
     # print(uf.split_url())
 
     SortedWithFirstPinyin(
-        file_path='/home/ga/words.txt',
+        file_path='/home/ga/Guardian/For-Python/AngelTools/angeltools/testfiles/res.txt',
         # save_path=save_path,
         full_match=True,
         reverse=False,
     ).run()
```

### Comparing `angeltools-0.2.6/angeltools/TimeTool.py` & `angeltools-0.2.7/angeltools/TimeTool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import random
 import time
 from datetime import datetime, timedelta
 
-from angeltools.StrTool import get_domain, FileLock
-
 
 def tell_timestamp(time_str=None, str_format="%Y-%m-%d %H:%M:%S"):
     if not time_str:
         return int(time.time())
     return int(time.mktime(time.strptime(time_str, str_format)))
 
 
@@ -24,14 +22,16 @@
 
 def wait(url, time_range: list = None):
     """
     用文件锁实现异步等待器，用于爬虫爬取等待
     :param url: https://api.github.com
     :param time_range: 随机时间列表 [start, end]
     """
+    from angeltools.StrTool import get_domain, FileLock
+
     time_range = [10, 30] if not time_range else time_range
     domain = get_domain(url)
 
     wait_time = random.choice([x/100 for x in range(*[int(i*100) for i in time_range], 1)])
 
     flock = FileLock(lock_id=domain)
     while time.time() < wait_time + flock.lock_time():
```

### Comparing `angeltools-0.2.6/angeltools/commands.py` & `angeltools-0.2.7/angeltools/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import argparse
 import json
 import os.path
 from pathlib import Path
 
-from angeltools.StrTool import SortedWithFirstPinyin
-from angeltools.ImageTool import text2chars, image2chars
-
 
 def txt2chars(args=None):
     dp = ' *** 文字转字符块小工具'
     da = "--->   "
     parser = argparse.ArgumentParser(description=dp, add_help=True)
     parser.add_argument("text", type=str, default='Hello', help=f'{da} 任何文字')
     parser.add_argument("-f", "--font_path", type=str, dest="font_path",
@@ -57,14 +54,15 @@
         except:
             raise ValueError(f'无法在此路径创建文件: {outfile_path.parent.absolute()}')
     if chart_list:
         try:
             chart_list = json.loads(chart_list)
         except:
             raise ValueError("-c chart_list 参数不正确")
+    from angeltools.ImageTool import text2chars
 
     text2chars(
         text,
         font_path=font_path,
         width=width,
         k=aspect_ratio,
         outfile=outfile,
@@ -122,14 +120,15 @@
         except:
             raise ValueError(f'无法在此路径创建文件: {outfile_path.parent.absolute()}')
     if chart_list:
         try:
             chart_list = json.loads(chart_list)
         except:
             raise ValueError("-c chart_list 参数不正确")
+    from angeltools.ImageTool import image2chars
 
     image2chars(
         image_path=image,
         width=width,
         k=aspect_ratio,
         outfile=outfile,
         reverse=reverse,
@@ -148,14 +147,16 @@
 
     parser.add_argument("-f", "--full_match", type=bool, dest="full_match", nargs='?', default=False,
                         help=f'{da} match all pinyin letters')
 
     parser.add_argument("-r", "--reverse", type=bool, dest="reverse", nargs='?', default=False,
                         help=f'{da} 反转')
 
+    from angeltools.StrTool import SortedWithFirstPinyin
+
     args = parser.parse_args()
 
     file_path = args.file_path
     save_path = args.save_path
     reverse = True if args.reverse else False
     full_match = True if args.full_match else False
     SortedWithFirstPinyin(
```

### Comparing `angeltools-0.2.6/angeltools/fdfs/fdfs_client/client.py` & `angeltools-0.2.7/angeltools/fdfs/fdfs_client/client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/fdfs/fdfs_client/connection.py` & `angeltools-0.2.7/angeltools/fdfs/fdfs_client/connection.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/fdfs/fdfs_client/fdfs_protol.py` & `angeltools-0.2.7/angeltools/fdfs/fdfs_client/fdfs_protol.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/fdfs/fdfs_client/fdfs_test.py` & `angeltools-0.2.7/angeltools/fdfs/fdfs_client/fdfs_test.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/fdfs/fdfs_client/storage_client.py` & `angeltools-0.2.7/angeltools/fdfs/fdfs_client/storage_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/fdfs/fdfs_client/tracker_client.py` & `angeltools-0.2.7/angeltools/fdfs/fdfs_client/tracker_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/fdfs/fdfs_client/utils.py` & `angeltools-0.2.7/angeltools/fdfs/fdfs_client/utils.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools/fdfs/fdfs_operator.py` & `angeltools-0.2.7/angeltools/fdfs/fdfs_operator.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/angeltools.egg-info/PKG-INFO` & `angeltools-0.2.7/angeltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.2.6
+Version: 0.2.7
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.2.6/angeltools.egg-info/SOURCES.txt` & `angeltools-0.2.7/angeltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.6/setup.py` & `angeltools-0.2.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 using_setuptools = True
 
 setup_args = {
     "name": "angeltools",
-    "version": "0.2.6",
+    "version": "0.2.7",
     "url": "https://github.com/ga1008/angeltools",
     "description": "personal python small tools collection",
     "long_description": long_description,
     "author": "Guardian",
     "author_email": "zhling2012@live.com",
     "maintainer": "Guardian",
     "maintainer_email": "zhling2012@live.com",
```

