# Comparing `tmp/chatapi-translate-0.4.tar.gz` & `tmp/chatapi-translate-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatapi-translate-0.4.tar", last modified: Wed May  3 09:32:58 2023, max compression
+gzip compressed data, was "chatapi-translate-0.5.tar", last modified: Mon May 15 03:26:52 2023, max compression
```

## Comparing `chatapi-translate-0.4.tar` & `chatapi-translate-0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:32:58.161586 chatapi-translate-0.4/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-30 17:02:13.000000 chatapi-translate-0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3518 2023-05-03 09:32:58.161586 chatapi-translate-0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:32:58.161586 chatapi-translate-0.4/chatapi_translate/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-03 06:36:13.000000 chatapi-translate-0.4/chatapi_translate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7699 2023-05-03 09:29:12.000000 chatapi-translate-0.4/chatapi_translate/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:32:58.161586 chatapi-translate-0.4/chatapi_translate/translator/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-02 07:56:47.000000 chatapi-translate-0.4/chatapi_translate/translator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3749 2023-05-01 13:57:32.000000 chatapi-translate-0.4/chatapi_translate/translator/ali.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-05-01 14:00:43.000000 chatapi-translate-0.4/chatapi_translate/translator/baidu.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-02 05:00:20.000000 chatapi-translate-0.4/chatapi_translate/translator/caiyun.py
--rw-r--r--   0 root         (0) root         (0)     2611 2023-05-02 10:29:40.000000 chatapi-translate-0.4/chatapi_translate/translator/chatgpt.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-01 13:59:38.000000 chatapi-translate-0.4/chatapi_translate/translator/deepl.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-05-01 14:10:20.000000 chatapi-translate-0.4/chatapi_translate/translator/google.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-01 14:11:07.000000 chatapi-translate-0.4/chatapi_translate/translator/tencent.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-01 14:14:00.000000 chatapi-translate-0.4/chatapi_translate/translator/utils.py
--rw-r--r--   0 root         (0) root         (0)     4993 2023-05-01 14:12:42.000000 chatapi-translate-0.4/chatapi_translate/translator/volcengine.py
--rw-r--r--   0 root         (0) root         (0)     6501 2023-05-03 09:26:06.000000 chatapi-translate-0.4/chatapi_translate/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:32:58.161586 chatapi-translate-0.4/chatapi_translate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3518 2023-05-03 09:32:58.000000 chatapi-translate-0.4/chatapi_translate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-03 09:32:58.000000 chatapi-translate-0.4/chatapi_translate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 09:32:58.000000 chatapi-translate-0.4/chatapi_translate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-03 09:32:58.000000 chatapi-translate-0.4/chatapi_translate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-03 09:32:58.000000 chatapi-translate-0.4/chatapi_translate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 09:32:58.000000 chatapi-translate-0.4/chatapi_translate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 09:32:58.161586 chatapi-translate-0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1305 2023-05-03 09:26:11.000000 chatapi-translate-0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:26:52.839746 chatapi-translate-0.5/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-30 17:02:13.000000 chatapi-translate-0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-15 03:26:52.839746 chatapi-translate-0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:26:52.835746 chatapi-translate-0.5/chatapi_translate/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-03 06:36:13.000000 chatapi-translate-0.5/chatapi_translate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7813 2023-05-15 03:25:42.000000 chatapi-translate-0.5/chatapi_translate/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:26:52.839746 chatapi-translate-0.5/chatapi_translate/translator/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-02 07:56:47.000000 chatapi-translate-0.5/chatapi_translate/translator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3749 2023-05-01 13:57:32.000000 chatapi-translate-0.5/chatapi_translate/translator/ali.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-05-01 14:00:43.000000 chatapi-translate-0.5/chatapi_translate/translator/baidu.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-02 05:00:20.000000 chatapi-translate-0.5/chatapi_translate/translator/caiyun.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-05-02 10:29:40.000000 chatapi-translate-0.5/chatapi_translate/translator/chatgpt.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-01 13:59:38.000000 chatapi-translate-0.5/chatapi_translate/translator/deepl.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-05-01 14:10:20.000000 chatapi-translate-0.5/chatapi_translate/translator/google.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-01 14:11:07.000000 chatapi-translate-0.5/chatapi_translate/translator/tencent.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-01 14:14:00.000000 chatapi-translate-0.5/chatapi_translate/translator/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-05-01 14:12:42.000000 chatapi-translate-0.5/chatapi_translate/translator/volcengine.py
+-rw-r--r--   0 root         (0) root         (0)     6501 2023-05-03 09:26:06.000000 chatapi-translate-0.5/chatapi_translate/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:26:52.835746 chatapi-translate-0.5/chatapi_translate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 03:26:52.839746 chatapi-translate-0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-05-15 03:11:47.000000 chatapi-translate-0.5/setup.py
```

### Comparing `chatapi-translate-0.4/LICENSE` & `chatapi-translate-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/PKG-INFO` & `chatapi-translate-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatapi-translate
-Version: 0.4
+Version: 0.5
 Summary: ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话
 Home-page: https://github.com/aitsc/chatapi-translate
 Author: aitsc
 License: MIT
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chatapi-translate
 ## 功能
 - ChatGPT 通常英文对话效果比较好, 但是英文水平不行的话来回翻译比较麻烦, 这个项目通过包裹 OpenAI API 接口实现自动调用翻译器来翻译你的提问和助理的回答.
+  - 英文靠谱例子：https://shareg.pt/jVBkjbD
+  - 中文不靠谱例子(最后一次回答不对)：https://shareg.pt/YfhCTDn
 - 支持流式传输, 多轮对话自动提取英文上下文用于 ChatGPT.
 
 ![chatbox](images/example.png)
 - 支持 百度翻译 / 腾讯翻译 / DeepL / 阿里翻译 / 彩云小译 / 火山翻译 / Google翻译 的API作为中转翻译器 (申请后都有免费额度)
 - 支持直接使用 ChatGPT 翻译, 不过它经常回答问题而不是翻译问题[很难控制](images/chatgpt-trans.png), 大家要能找到好的prompt可以分享一下 (见配置示例)
   - 如果肯用 gpt-4 做翻译器, 翻译效果应该还是挺好的
 - 不想使用翻译的时候可以输入 "--不翻译\n" (见配置文件)
```

### Comparing `chatapi-translate-0.4/chatapi_translate/api.py` & `chatapi-translate-0.5/chatapi_translate/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,17 @@
         except Exception as e:
             traceback.print_exc()
             raise HTTPException(status_code=500, detail=str(e))
     # 获取问题和消息
     question = ''
     for message in body["messages"][::-1]:
         if message['role'] == 'user':
-            question += message['content'] + '\n'  # 合并所有连续问题
+            question = message['content'] + '\n' + question  # 合并所有连续问题
+        elif message['role'] == 'system':
+            question = message['content'] + '\n\n' + question
         else:
             break
     question = question.strip()
     if not question:  # 没有问题
         raise HTTPException(status.HTTP_400_BAD_REQUEST, "No Question Found")
     if headers['authorization'] in get_global_config()['key_translator']:  # 翻译器
         t_name = get_global_config()['key_translator'][headers['authorization']]
```

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/__init__.py` & `chatapi-translate-0.5/chatapi_translate/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/ali.py` & `chatapi-translate-0.5/chatapi_translate/translator/ali.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/baidu.py` & `chatapi-translate-0.5/chatapi_translate/translator/baidu.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/caiyun.py` & `chatapi-translate-0.5/chatapi_translate/translator/caiyun.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/chatgpt.py` & `chatapi-translate-0.5/chatapi_translate/translator/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/deepl.py` & `chatapi-translate-0.5/chatapi_translate/translator/deepl.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/google.py` & `chatapi-translate-0.5/chatapi_translate/translator/google.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/tencent.py` & `chatapi-translate-0.5/chatapi_translate/translator/tencent.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/utils.py` & `chatapi-translate-0.5/chatapi_translate/translator/utils.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/translator/volcengine.py` & `chatapi-translate-0.5/chatapi_translate/translator/volcengine.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate/utils.py` & `chatapi-translate-0.5/chatapi_translate/utils.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/chatapi_translate.egg-info/PKG-INFO` & `chatapi-translate-0.5/chatapi_translate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatapi-translate
-Version: 0.4
+Version: 0.5
 Summary: ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话
 Home-page: https://github.com/aitsc/chatapi-translate
 Author: aitsc
 License: MIT
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chatapi-translate
 ## 功能
 - ChatGPT 通常英文对话效果比较好, 但是英文水平不行的话来回翻译比较麻烦, 这个项目通过包裹 OpenAI API 接口实现自动调用翻译器来翻译你的提问和助理的回答.
+  - 英文靠谱例子：https://shareg.pt/jVBkjbD
+  - 中文不靠谱例子(最后一次回答不对)：https://shareg.pt/YfhCTDn
 - 支持流式传输, 多轮对话自动提取英文上下文用于 ChatGPT.
 
 ![chatbox](images/example.png)
 - 支持 百度翻译 / 腾讯翻译 / DeepL / 阿里翻译 / 彩云小译 / 火山翻译 / Google翻译 的API作为中转翻译器 (申请后都有免费额度)
 - 支持直接使用 ChatGPT 翻译, 不过它经常回答问题而不是翻译问题[很难控制](images/chatgpt-trans.png), 大家要能找到好的prompt可以分享一下 (见配置示例)
   - 如果肯用 gpt-4 做翻译器, 翻译效果应该还是挺好的
 - 不想使用翻译的时候可以输入 "--不翻译\n" (见配置文件)
```

### Comparing `chatapi-translate-0.4/chatapi_translate.egg-info/SOURCES.txt` & `chatapi-translate-0.5/chatapi_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.4/setup.py` & `chatapi-translate-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'code: https://github.com/aitsc/chatapi-translate'
 
 setup(
     name='chatapi-translate',
-    version='0.4',
+    version='0.5',
     description="ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='aitsc',
     license='MIT',
     url='https://github.com/aitsc/chatapi-translate',
     keywords='tools',
```

