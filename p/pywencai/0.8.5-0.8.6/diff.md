# Comparing `tmp/pywencai-0.8.5.tar.gz` & `tmp/pywencai-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.8.5.tar", max compression
+gzip compressed data, was "pywencai-0.8.6.tar", max compression
```

## Comparing `pywencai-0.8.5.tar` & `pywencai-0.8.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-13 06:17:17.135331 pywencai-0.8.5/LICENSE
--rw-r--r--   0        0        0     2836 2023-05-13 06:17:17.135331 pywencai-0.8.5/README.md
--rw-r--r--   0        0        0      612 2023-05-13 06:17:17.135331 pywencai-0.8.5/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-13 06:17:17.135331 pywencai-0.8.5/pywencai/__init__.py
--rw-r--r--   0        0        0     4746 2023-05-13 06:17:17.135331 pywencai-0.8.5/pywencai/convert.py
--rw-r--r--   0        0        0      433 2023-05-13 06:17:17.135331 pywencai-0.8.5/pywencai/headers.py
--rw-r--r--   0        0        0    39677 2023-05-13 06:17:17.135331 pywencai-0.8.5/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4083 2023-05-13 06:17:17.135331 pywencai-0.8.5/pywencai/wencai.py
--rw-r--r--   0        0        0     3460 1970-01-01 00:00:00.000000 pywencai-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-15 02:01:42.979657 pywencai-0.8.6/LICENSE
+-rw-r--r--   0        0        0     2836 2023-05-15 02:01:42.979657 pywencai-0.8.6/README.md
+-rw-r--r--   0        0        0      612 2023-05-15 02:01:42.979657 pywencai-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-15 02:01:42.979657 pywencai-0.8.6/pywencai/__init__.py
+-rw-r--r--   0        0        0     4746 2023-05-15 02:01:42.979657 pywencai-0.8.6/pywencai/convert.py
+-rw-r--r--   0        0        0      433 2023-05-15 02:01:42.979657 pywencai-0.8.6/pywencai/headers.py
+-rw-r--r--   0        0        0    39677 2023-05-15 02:01:42.979657 pywencai-0.8.6/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4187 2023-05-15 02:01:42.983657 pywencai-0.8.6/pywencai/wencai.py
+-rw-r--r--   0        0        0     3460 1970-01-01 00:00:00.000000 pywencai-0.8.6/PKG-INFO
```

### Comparing `pywencai-0.8.5/LICENSE` & `pywencai-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.5/README.md` & `pywencai-0.8.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 ```
 > 具体参数参看：[https://requests.readthedocs.io/en/latest/api/#requests.request](https://requests.readthedocs.io/en/latest/api/#requests.request)
 
 ### 返回值
 
 当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
 
-当查询的是详情是，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
+当查询的是详情时，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
 
 ## 联系方式
 
 欢迎加入QQ群，分享量化技术！
 
 <img src="./qrcode.png" width=400>
```

### Comparing `pywencai-0.8.5/pyproject.toml` & `pywencai-0.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.8.5"
+version = "0.8.6"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.8.5/pywencai/convert.py` & `pywencai-0.8.6/pywencai/convert.py`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.5/pywencai/hexin-v.js` & `pywencai-0.8.6/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.5/pywencai/wencai.py` & `pywencai-0.8.6/pywencai/wencai.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 import pandas as pd
 import time
 import logging
 import pydash as _
 from pywencai.convert import convert
 from pywencai.headers import headers
 
-logging.basicConfig(
-    level=logging.INFO,
-    format='[pywencai] %(asctime)s - %(levelname)s - %(message)s'
-)
+handler = logging.StreamHandler()
+handler.setFormatter(logging.Formatter('[pywencai] %(asctime)s - %(levelname)s - %(message)s'))
+logger = logging.getLogger(__name__)
+logger.addHandler(handler)
+logger.setLevel(logging.INFO)
+
 
 def while_do(do, retry=10, sleep=0, log=False):
     count = 0
     while count < retry:
         time.sleep(sleep)
         try:
             return do()
         except:
-            log and logging.warning(f'{count+1}次尝试失败')
+            log and logger.warning(f'{count+1}次尝试失败')
             count += 1
     return None
 
 
 def get_robot_data(**kwargs):
     '''获取condition'''
     retry = kwargs.get('retry', 10)
@@ -38,32 +40,32 @@
         'page': 1,
         'source': 'Ths_iwencai_Xuangu',
         'secondary_intent': query_type,
         'question': question
     }
 
     count = 0
-    log and logging.info(f'获取condition开始')
+    log and logger.info(f'获取condition开始')
 
     def do():
         res = rq.request(
             method='POST',
             url='http://www.iwencai.com/customized/chart/get-robot-data',
             json=data,
             headers=headers(cookie),
             **request_params
         )
         params = convert(res)
-        log and logging.info(f'获取get_robot_data成功')
+        log and logger.info(f'获取get_robot_data成功')
         return params
 
     result = while_do(do, retry, sleep, log)
 
     if result is None:
-        log and logging.info(f'获取get_robot_data失败')
+        log and logger.info(f'获取get_robot_data失败')
 
     return result
 
 
 def replace_key(key):
     '''替换key'''
     key_map = {
@@ -85,34 +87,34 @@
     data = {
         'perpage': 100,
         'page': 1,
         'source': 'Ths_iwencai_Xuangu',
         **kwargs
     }
     count = 0
-    log and logging.info(f'第{data.get("page")}页开始')
+    log and logger.info(f'第{data.get("page")}页开始')
 
     def do():
         res = rq.request(
             method='POST',
             url='http://www.iwencai.com/gateway/urp/v7/landing/getDataList',
             data=data,
             headers=headers(cookie),
             timeout=(5, 10),
             **request_params
         )
         result = json.loads(res.text)
         list = result['answer']['components'][0]['data']['datas']
-        log and logging.info(f'第{data.get("page")}页成功')
+        log and logger.info(f'第{data.get("page")}页成功')
         return pd.DataFrame.from_dict(list)
     
     result = while_do(do, retry, sleep, log)
 
     if result is None:
-        log and logging.error(f'第{data.get("page")}页失败')
+        log and logger.error(f'第{data.get("page")}页失败')
 
     return result
 
 
 def can_loop(loop, count):
     '''是否继续循环'''
     if (loop is True):
@@ -152,8 +154,8 @@
     if condition is not None:
         kwargs = {**kwargs, **data}
         if loop:
             return loop_page(loop, **kwargs)
         else:
             return get_page(**kwargs)
     else:
-        return data
+        return data
```

### Comparing `pywencai-0.8.5/PKG-INFO` & `pywencai-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.8.5
+Version: 0.8.6
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -125,15 +125,15 @@
 ```
 > 具体参数参看：[https://requests.readthedocs.io/en/latest/api/#requests.request](https://requests.readthedocs.io/en/latest/api/#requests.request)
 
 ### 返回值
 
 当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
 
-当查询的是详情是，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
+当查询的是详情时，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
 
 ## 联系方式
 
 欢迎加入QQ群，分享量化技术！
 
 <img src="./qrcode.png" width=400>
```

