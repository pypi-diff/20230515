# Comparing `tmp/pynocaptcha-1.4.9.tar.gz` & `tmp/pynocaptcha-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.4.9.tar", last modified: Thu May 11 08:59:31 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.5.0.tar", last modified: Mon May 15 07:35:54 2023, max compression
```

## Comparing `pynocaptcha-1.4.9.tar` & `pynocaptcha-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-11 08:59:31.000000 pynocaptcha-1.4.9/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-05-11 08:59:31.000000 pynocaptcha-1.4.9/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-11 08:59:31.000000 pynocaptcha-1.4.9/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.9/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-11 08:59:31.000000 pynocaptcha-1.4.9/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)      961 2023-05-08 09:19:50.000000 pynocaptcha-1.4.9/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4577 2023-05-11 08:54:40.000000 pynocaptcha-1.4.9/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.9/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.9/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1488 2023-04-23 14:39:24.000000 pynocaptcha-1.4.9/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.9/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-05-11 08:54:55.000000 pynocaptcha-1.4.9/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-15 07:35:54.000000 pynocaptcha-1.5.0/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-05-15 07:35:54.000000 pynocaptcha-1.5.0/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-15 07:35:54.000000 pynocaptcha-1.5.0/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      571 2023-05-15 07:30:18.000000 pynocaptcha-1.5.0/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-05-15 07:35:54.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)      961 2023-05-08 09:19:50.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4577 2023-05-11 08:54:40.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2108 2023-05-15 07:32:09.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.0/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-05-15 07:32:23.000000 pynocaptcha-1.5.0/setup.py
```

### Comparing `pynocaptcha-1.4.9/PKG-INFO` & `pynocaptcha-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.4.9
+Version: 1.5.0
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.4.9/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.5.0/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.9/pynocaptcha/crackers/base.py` & `pynocaptcha-1.5.0/pynocaptcha/crackers/base.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.9/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.5.0/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.9/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.5.0/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.9/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.5.0/pynocaptcha/crackers/incapsula.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import requests
 from .base import BaseCracker
 
 
-class IncapsulaCracker(BaseCracker):
+class IncapsulaReese84Cracker(BaseCracker):
     
     cracker_name = "incapsula"
-    cracker_version = "universal"    
+    cracker_version = "reese84"    
 
     """
     incapsula cracker
     :param href: 触发 incapsula 盾验证的首页地址
     :param user_agent: 请求流程使用 ua, 必须使用 MacOS Firefox User-Agent, 否则可能破解失败
     :param submit: 是否提交验证接口, 不提交则返回计算参数
     调用示例:
@@ -41,7 +41,35 @@
             'upgrade-insecure-requests': '1',
             'user-agent': self.user_agent,
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
             'accept-language': 'zh-CN,zh;q=0.9',
         }
         resp = requests.get("/".join(self.href.split("/")[:3])+ "/", headers=headers, cookies=cookies)
         return 'ROBOTS' not in resp.text
+
+
+class IncapsulaUtmvcCracker(BaseCracker):
+    
+    cracker_name = "incapsula"
+    cracker_version = "utmvc"    
+
+    """
+    incapsula cracker
+    :param script: Incapsula js 脚本字符串
+    :param cookies: 携带 incap_sess_xxx 的 cookies, {"incap_ses_xxx": "xaxa"}
+    调用示例:
+    cracker = IncapsulaUtmvcCracker(
+        script=script,
+        cookies={},
+        
+        user_token="xxx",
+
+        # debug=True,
+        # check_useful=True,
+        # proxy=proxy,
+        # submit=False
+    )
+    ret = cracker.crack()
+    """
+    
+    # 必传参数
+    must_check_params = ["script", "cookies"]
```

### Comparing `pynocaptcha-1.4.9/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.5.0/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.9/setup.py` & `pynocaptcha-1.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.4.9',
+    version='1.5.0',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

