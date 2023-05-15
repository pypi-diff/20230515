# Comparing `tmp/chatapi-translate-0.5.tar.gz` & `tmp/chatapi-translate-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatapi-translate-0.5.tar", last modified: Mon May 15 03:26:52 2023, max compression
+gzip compressed data, was "chatapi-translate-0.6.tar", last modified: Mon May 15 04:09:41 2023, max compression
```

## Comparing `chatapi-translate-0.5.tar` & `chatapi-translate-0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:26:52.839746 chatapi-translate-0.5/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-30 17:02:13.000000 chatapi-translate-0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-15 03:26:52.839746 chatapi-translate-0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:26:52.835746 chatapi-translate-0.5/chatapi_translate/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-03 06:36:13.000000 chatapi-translate-0.5/chatapi_translate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7813 2023-05-15 03:25:42.000000 chatapi-translate-0.5/chatapi_translate/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:26:52.839746 chatapi-translate-0.5/chatapi_translate/translator/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-02 07:56:47.000000 chatapi-translate-0.5/chatapi_translate/translator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3749 2023-05-01 13:57:32.000000 chatapi-translate-0.5/chatapi_translate/translator/ali.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-05-01 14:00:43.000000 chatapi-translate-0.5/chatapi_translate/translator/baidu.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-02 05:00:20.000000 chatapi-translate-0.5/chatapi_translate/translator/caiyun.py
--rw-r--r--   0 root         (0) root         (0)     2611 2023-05-02 10:29:40.000000 chatapi-translate-0.5/chatapi_translate/translator/chatgpt.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-01 13:59:38.000000 chatapi-translate-0.5/chatapi_translate/translator/deepl.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-05-01 14:10:20.000000 chatapi-translate-0.5/chatapi_translate/translator/google.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-01 14:11:07.000000 chatapi-translate-0.5/chatapi_translate/translator/tencent.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-01 14:14:00.000000 chatapi-translate-0.5/chatapi_translate/translator/utils.py
--rw-r--r--   0 root         (0) root         (0)     4993 2023-05-01 14:12:42.000000 chatapi-translate-0.5/chatapi_translate/translator/volcengine.py
--rw-r--r--   0 root         (0) root         (0)     6501 2023-05-03 09:26:06.000000 chatapi-translate-0.5/chatapi_translate/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 03:26:52.835746 chatapi-translate-0.5/chatapi_translate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-15 03:26:52.000000 chatapi-translate-0.5/chatapi_translate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 03:26:52.839746 chatapi-translate-0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1305 2023-05-15 03:11:47.000000 chatapi-translate-0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:09:41.220732 chatapi-translate-0.6/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-30 17:02:13.000000 chatapi-translate-0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-15 04:09:41.220732 chatapi-translate-0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:09:41.220732 chatapi-translate-0.6/chatapi_translate/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-03 06:36:13.000000 chatapi-translate-0.6/chatapi_translate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7957 2023-05-15 04:06:56.000000 chatapi-translate-0.6/chatapi_translate/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:09:41.220732 chatapi-translate-0.6/chatapi_translate/translator/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-02 07:56:47.000000 chatapi-translate-0.6/chatapi_translate/translator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3749 2023-05-01 13:57:32.000000 chatapi-translate-0.6/chatapi_translate/translator/ali.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-05-01 14:00:43.000000 chatapi-translate-0.6/chatapi_translate/translator/baidu.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-02 05:00:20.000000 chatapi-translate-0.6/chatapi_translate/translator/caiyun.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-05-02 10:29:40.000000 chatapi-translate-0.6/chatapi_translate/translator/chatgpt.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-01 13:59:38.000000 chatapi-translate-0.6/chatapi_translate/translator/deepl.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-05-01 14:10:20.000000 chatapi-translate-0.6/chatapi_translate/translator/google.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-01 14:11:07.000000 chatapi-translate-0.6/chatapi_translate/translator/tencent.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-01 14:14:00.000000 chatapi-translate-0.6/chatapi_translate/translator/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-05-01 14:12:42.000000 chatapi-translate-0.6/chatapi_translate/translator/volcengine.py
+-rw-r--r--   0 root         (0) root         (0)     6962 2023-05-15 04:02:32.000000 chatapi-translate-0.6/chatapi_translate/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:09:41.220732 chatapi-translate-0.6/chatapi_translate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-15 04:09:40.000000 chatapi-translate-0.6/chatapi_translate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 04:09:41.220732 chatapi-translate-0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-05-15 03:45:22.000000 chatapi-translate-0.6/setup.py
```

### Comparing `chatapi-translate-0.5/LICENSE` & `chatapi-translate-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/PKG-INFO` & `chatapi-translate-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatapi-translate
-Version: 0.5
+Version: 0.6
 Summary: ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话
 Home-page: https://github.com/aitsc/chatapi-translate
 Author: aitsc
 License: MIT
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatapi-translate-0.5/chatapi_translate/api.py` & `chatapi-translate-0.6/chatapi_translate/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     for message in body["messages"][::-1]:
         if message['role'] == 'user':
             question = message['content'] + '\n' + question  # 合并所有连续问题
         elif message['role'] == 'system':
             question = message['content'] + '\n\n' + question
         else:
             break
+    trans_trigger = get_global_config()['filter']['trans_trigger']
+    if trans_trigger:
+        question = question.replace(trans_trigger, '')
     question = question.strip()
     if not question:  # 没有问题
         raise HTTPException(status.HTTP_400_BAD_REQUEST, "No Question Found")
     if headers['authorization'] in get_global_config()['key_translator']:  # 翻译器
         t_name = get_global_config()['key_translator'][headers['authorization']]
     else:
         t_name = get_global_config()['key_translator']['']
```

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/__init__.py` & `chatapi-translate-0.6/chatapi_translate/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/ali.py` & `chatapi-translate-0.6/chatapi_translate/translator/ali.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/baidu.py` & `chatapi-translate-0.6/chatapi_translate/translator/baidu.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/caiyun.py` & `chatapi-translate-0.6/chatapi_translate/translator/caiyun.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/chatgpt.py` & `chatapi-translate-0.6/chatapi_translate/translator/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/deepl.py` & `chatapi-translate-0.6/chatapi_translate/translator/deepl.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/google.py` & `chatapi-translate-0.6/chatapi_translate/translator/google.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/tencent.py` & `chatapi-translate-0.6/chatapi_translate/translator/tencent.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/utils.py` & `chatapi-translate-0.6/chatapi_translate/translator/utils.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/translator/volcengine.py` & `chatapi-translate-0.6/chatapi_translate/translator/volcengine.py`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/chatapi_translate/utils.py` & `chatapi-translate-0.6/chatapi_translate/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,45 +127,52 @@
             else:
                 yield json.dumps(data, ensure_ascii=False)
 
 
 def filter_messages_and_trigger(messages):  # 用于不翻译的信息
     filtered_messages = []
     no_trans_trigger = get_global_config()['filter']['no_trans_trigger']
+    trans_trigger = get_global_config()['filter']['trans_trigger']
 
     marks = get_global_config()['marks']
     u_trans = re.escape(marks["user_trans"])
     a_answer = re.escape(marks["assistant_answer"])
     a_trans = re.escape(marks["assistant_trans"])
     re_end = f'(?={u_trans}|{a_answer}|{a_trans}|$)'
 
     for message in messages:
         if message['role'] != 'assistant':
             if no_trans_trigger:
                 message['content'] = message['content'].replace(no_trans_trigger, '')
+            if trans_trigger:
+                message['content'] = message['content'].replace(trans_trigger, '')
             filtered_messages.append(message)
         else:
             assistant = re.search(f'(?<={a_answer})[\w\W]+?{re_end}', message['content'])
             if assistant:
                 filtered_messages.append({'role': 'assistant', 'content': assistant.group()})
             else:
                 filtered_messages.append(message)
     return filtered_messages
 
 
 def has_no_trans_trigger(messages):  # 判断是否不要翻译
     no_trans_trigger = get_global_config()['filter']['no_trans_trigger']
-    if not no_trans_trigger:
+    trans_trigger = get_global_config()['filter']['trans_trigger']
+    if not (no_trans_trigger or trans_trigger):
         return False
+    has_trans_trigger = False  # 是否至少有一个对话有触发器
     for message in messages:
         if message['role'] == 'assistant':
             continue
-        if no_trans_trigger in message['content']:
+        if no_trans_trigger and no_trans_trigger in message['content']:
             return True
-    return False
+        if trans_trigger in message['content']:
+            has_trans_trigger = True
+    return not has_trans_trigger
 
 
 def generate_stream_response_start(id_str, model_name='gpt-3.5-turbo'):
     ret = {"id": id_str, "object": "chat.completion.chunk", "created": int(
         time.time()), "model": model_name, "choices": [{"delta": {"role": "assistant"}, "index": 0, "finish_reason": None}]}
     return ret
```

### Comparing `chatapi-translate-0.5/chatapi_translate.egg-info/PKG-INFO` & `chatapi-translate-0.6/chatapi_translate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatapi-translate
-Version: 0.5
+Version: 0.6
 Summary: ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话
 Home-page: https://github.com/aitsc/chatapi-translate
 Author: aitsc
 License: MIT
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatapi-translate-0.5/chatapi_translate.egg-info/SOURCES.txt` & `chatapi-translate-0.6/chatapi_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatapi-translate-0.5/setup.py` & `chatapi-translate-0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'code: https://github.com/aitsc/chatapi-translate'
 
 setup(
     name='chatapi-translate',
-    version='0.5',
+    version='0.6',
     description="ChatGPT OpenAI API 流式反向代理，自动翻译中文到英文对话，实现用英文进行高质量的对话",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='aitsc',
     license='MIT',
     url='https://github.com/aitsc/chatapi-translate',
     keywords='tools',
```

