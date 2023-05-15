# Comparing `tmp/chatglm-llm-1.3.3.tar.gz` & `tmp/chatglm-llm-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.3.3.tar", last modified: Sat May 13 03:02:37 2023, max compression
+gzip compressed data, was "chatglm-llm-1.3.4.tar", last modified: Mon May 15 05:57:40 2023, max compression
```

## Comparing `chatglm-llm-1.3.3.tar` & `chatglm-llm-1.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-13 03:02:37.077184 chatglm-llm-1.3.3/
--rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.3.3/MANIFEST.in
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-05-13 03:02:37.077062 chatglm-llm-1.3.3/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.3.3/README.md
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-13 03:02:37.075524 chatglm-llm-1.3.3/chatglm_llm.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-05-13 03:02:36.000000 chatglm-llm-1.3.3/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      480 2023-05-13 03:02:37.000000 chatglm-llm-1.3.3/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-13 03:02:36.000000 chatglm-llm-1.3.3/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       53 2023-05-13 03:02:36.000000 chatglm-llm-1.3.3/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.3.3/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)      226 2023-05-13 03:02:36.000000 chatglm-llm-1.3.3/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       12 2023-05-13 03:02:37.000000 chatglm-llm-1.3.3/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-13 03:02:37.076190 chatglm-llm-1.3.3/chatglm_src/
--rw-r--r--   0 mroy       (501) staff       (20)      680 2023-05-11 01:28:05.000000 chatglm-llm-1.3.3/chatglm_src/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.3.3/chatglm_src/callbacks.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-13 03:02:37.076759 chatglm-llm-1.3.3/chatglm_src/chains/
--rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.3.3/chatglm_src/chains/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.3.3/chatglm_src/chains/local_qa.py
--rw-r--r--   0 mroy       (501) staff       (20)      443 2023-05-04 01:08:28.000000 chatglm-llm-1.3.3/chatglm_src/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)     3052 2023-05-11 09:34:29.000000 chatglm-llm-1.3.3/chatglm_src/embeding.py
--rw-r--r--   0 mroy       (501) staff       (20)    24310 2023-05-13 03:01:32.000000 chatglm-llm-1.3.3/chatglm_src/llm.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-13 03:02:37.076890 chatglm-llm-1.3.3/chatglm_src/loader/
--rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.3.3/chatglm_src/loader/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-05-13 03:02:37.077224 chatglm-llm-1.3.3/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)      997 2023-05-13 03:02:29.000000 chatglm-llm-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.268688 chatglm-llm-1.3.4/
+-rw-rw-rw-   0        0        0       36 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      225 2023-05-15 05:57:40.267680 chatglm-llm-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1887 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.257685 chatglm-llm-1.3.4/chatglm_llm.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-05-15 05:57:39.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-05-15 05:57:40.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:57:39.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-15 05:57:39.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 05:57:39.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      226 2023-05-15 05:57:40.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-15 05:57:40.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.263034 chatglm-llm-1.3.4/chatglm_src/
+-rw-rw-rw-   0        0        0      680 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/__init__.py
+-rw-rw-rw-   0        0        0     4201 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.265162 chatglm-llm-1.3.4/chatglm_src/chains/
+-rw-rw-rw-   0        0        0       69 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/chains/__init__.py
+-rw-rw-rw-   0        0        0     4402 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/chains/local_qa.py
+-rw-rw-rw-   0        0        0      443 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/cmd.py
+-rw-rw-rw-   0        0        0     3052 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/embeding.py
+-rw-rw-rw-   0        0        0    24286 2023-05-15 05:53:40.000000 chatglm-llm-1.3.4/chatglm_src/llm.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.265908 chatglm-llm-1.3.4/chatglm_src/loader/
+-rw-rw-rw-   0        0        0     1403 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/loader/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:57:40.268688 chatglm-llm-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-05-15 05:56:17.000000 chatglm-llm-1.3.4/setup.py
```

### Comparing `chatglm-llm-1.3.3/README.md` & `chatglm-llm-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.3/chatglm_src/__init__.py` & `chatglm-llm-1.3.4/chatglm_src/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.3/chatglm_src/callbacks.py` & `chatglm-llm-1.3.4/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.3/chatglm_src/chains/local_qa.py` & `chatglm-llm-1.3.4/chatglm_src/chains/local_qa.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.3/chatglm_src/embeding.py` & `chatglm-llm-1.3.4/chatglm_src/embeding.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.3/chatglm_src/llm.py` & `chatglm-llm-1.3.4/chatglm_src/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 from hashlib import md5
 import time
 import numpy as np
 from aiowebsocket.converses import AioWebSocket
 from websocket import create_connection
 import websockets
 from websockets.server import serve
+from langchain.callbacks.manager import BaseCallbackManager, CallbackManagerForLLMRun
+from langchain.embeddings import HuggingFaceEmbeddings
+import gptcache
+from gptcache.processor.pre import get_prompt
+from gptcache.manager.factory import get_data_manager
+from langchain.cache import GPTCache
 
 try:
     from transformers import AutoTokenizer, AutoModel
-    from langchain.embeddings import HuggingFaceEmbeddings
     from accelerate import load_checkpoint_and_dispatch
     import torch, gc
-    import gptcache
-    from gptcache.processor.pre import get_prompt
-    from gptcache.manager.factory import get_data_manager
-    from langchain.cache import GPTCache
-    from langchain.callbacks.manager import BaseCallbackManager, CallbackManagerForLLMRun
     DEFAULT_CACHE_MAP_PATH = str(pathlib.Path.home() / ".cache" / "local_qa_cache_map")
     i = 0
 
     def init_gptcache_map(cache_obj: gptcache.Cache):
         global i
         cache_path = f'{DEFAULT_CACHE_MAP_PATH}_{i}.txt'
         cache_obj.init(
```

### Comparing `chatglm-llm-1.3.3/chatglm_src/loader/__init__.py` & `chatglm-llm-1.3.4/chatglm_src/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.3/setup.py` & `chatglm-llm-1.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.3.3',
+    version='1.3.4',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
```

