# Comparing `tmp/python-llm-0.1.1.tar.gz` & `tmp/python-llm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-llm-0.1.1.tar", last modified: Sun May 14 15:46:59 2023, max compression
+gzip compressed data, was "python-llm-0.1.2.tar", last modified: Sun May 14 23:00:11 2023, max compression
```

## Comparing `python-llm-0.1.1.tar` & `python-llm-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.031965 python-llm-0.1.1/
--rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.1/LICENSE
--rw-r--r--   0 danielgross   (501) staff       (20)      183 2023-05-14 15:46:59.031861 python-llm-0.1.1/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)     1197 2023-05-14 15:44:12.000000 python-llm-0.1.1/README.md
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.030581 python-llm-0.1.1/llm/
--rw-r--r--   0 danielgross   (501) staff       (20)       69 2023-05-13 13:51:59.000000 python-llm-0.1.1/llm/__init__.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.030874 python-llm-0.1.1/llm/api/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.1/llm/api/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2376 2023-05-14 14:49:00.000000 python-llm-0.1.1/llm/api/claude.py
--rw-r--r--   0 danielgross   (501) staff       (20)      980 2023-03-30 14:01:26.000000 python-llm-0.1.1/llm/api/openaiapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2384 2023-05-14 14:49:01.000000 python-llm-0.1.1/llm/main.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1781 2023-05-13 13:24:32.000000 python-llm-0.1.1/llm/util.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.031414 python-llm-0.1.1/python_llm.egg-info/
--rw-r--r--   0 danielgross   (501) staff       (20)      183 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)      336 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/SOURCES.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/dependency_links.txt
--rw-r--r--   0 danielgross   (501) staff       (20)      146 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/requires.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/top_level.txt
--rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-14 15:46:59.032000 python-llm-0.1.1/setup.cfg
--rw-r--r--   0 danielgross   (501) staff       (20)      445 2023-05-14 15:46:30.000000 python-llm-0.1.1/setup.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.031692 python-llm-0.1.1/tests/
--rw-r--r--   0 danielgross   (501) staff       (20)     2465 2023-05-14 15:05:09.000000 python-llm-0.1.1/tests/test_claude.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1811 2023-05-14 15:01:48.000000 python-llm-0.1.1/tests/test_openai.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:00:11.154703 python-llm-0.1.2/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.2/LICENSE
+-rw-r--r--   0 danielgross   (501) staff       (20)      183 2023-05-14 23:00:11.154592 python-llm-0.1.2/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)     1458 2023-05-14 22:59:17.000000 python-llm-0.1.2/README.md
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:00:11.153206 python-llm-0.1.2/llm/
+-rw-r--r--   0 danielgross   (501) staff       (20)       69 2023-05-13 13:51:59.000000 python-llm-0.1.2/llm/__init__.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:00:11.153646 python-llm-0.1.2/llm/api/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.2/llm/api/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2376 2023-05-14 14:49:00.000000 python-llm-0.1.2/llm/api/claude.py
+-rw-r--r--   0 danielgross   (501) staff       (20)      980 2023-03-30 14:01:26.000000 python-llm-0.1.2/llm/api/openaiapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2384 2023-05-14 14:49:01.000000 python-llm-0.1.2/llm/main.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     1781 2023-05-13 13:24:32.000000 python-llm-0.1.2/llm/util.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:00:11.154230 python-llm-0.1.2/python_llm.egg-info/
+-rw-r--r--   0 danielgross   (501) staff       (20)      183 2023-05-14 23:00:11.000000 python-llm-0.1.2/python_llm.egg-info/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)      336 2023-05-14 23:00:11.000000 python-llm-0.1.2/python_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-14 23:00:11.000000 python-llm-0.1.2/python_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      146 2023-05-14 23:00:11.000000 python-llm-0.1.2/python_llm.egg-info/requires.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-14 23:00:11.000000 python-llm-0.1.2/python_llm.egg-info/top_level.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-14 23:00:11.154735 python-llm-0.1.2/setup.cfg
+-rw-r--r--   0 danielgross   (501) staff       (20)      445 2023-05-14 22:59:34.000000 python-llm-0.1.2/setup.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:00:11.154469 python-llm-0.1.2/tests/
+-rw-r--r--   0 danielgross   (501) staff       (20)     2749 2023-05-14 22:54:04.000000 python-llm-0.1.2/tests/test_claude.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2097 2023-05-14 22:53:48.000000 python-llm-0.1.2/tests/test_openai.py
```

### Comparing `python-llm-0.1.1/LICENSE` & `python-llm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.1/README.md` & `python-llm-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,28 @@
 ![Tests](https://github.com/danielgross/python-llm/actions/workflows/tests.yml/badge.svg)
 
 ## Usage
 
 ```python
 import llm
 
+# Chat
+llm.chat(["what is 2+2"]) # 4. Uses GPT-3 by default if key is provided.
+llm.chat(["what is 2+2"], engine="anthropic:claude-instant-v1") 
+
 # Completion
-llm.complete("hello, I am a") # Uses GPT-3 by default if key is provided.
+llm.complete("hello, I am") 
+llm.complete("hello, I am", engine="openai:gpt-4")
 llm.complete("hello, I am ", engine="anthropic:claude-instant-v1") # Uses Anthropic's model.
 
-# Chat
-llm.chat(["hi", "hi how are you", "tell me a joke"])
+# Back-and-forth chat
+llm.chat(["hi", "hi there, how are you?", "good, tell me a joke"]) # Human/assistant/human exchanges.
 
-# Embedding 
-llm.embed(open("harrypotter.txt").read())
+# Embedding
+llm.embed(open("harrypotter.txt").read()).tsne() # (I haven't implemented this yet.)
 
 # Engines are in the provider:model format, as in openai:gpt-4, or anthropic:claude-instant-v1.
 ```
 
 ## Installation
 
 To install `python-llm`, use pip: ```pip install python-llm```.
@@ -31,11 +36,11 @@
 - **Text Completion**: Complete text prompts using different language models.
 - **Chat**: Simulate a conversation with a language model.
 - **Text Embedding**: Transform text into a high-dimensional vector (not yet implemented).
 
 ## Configuration
 You can configure the API keys for the various services using the set_api_key method:
 ```python
-llm.set_api_key(openai="sk-...", natdev="...")
+llm.set_api_key(openai="sk-...", anthropic="...")
 # or
 llm.set_api_key("path/to/api_keys.json")
 ```
```

### Comparing `python-llm-0.1.1/llm/api/claude.py` & `python-llm-0.1.2/llm/api/claude.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.1/llm/api/openaiapi.py` & `python-llm-0.1.2/llm/api/openaiapi.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.1/llm/main.py` & `python-llm-0.1.2/llm/main.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.1/llm/util.py` & `python-llm-0.1.2/llm/util.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.1/tests/test_claude.py` & `python-llm-0.1.2/tests/test_claude.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     @vcr.use_cassette("tests/fixtures/claude/test_completion.yaml", filter_headers=['authorization', 'x-api-key'])
     def test_completion(self):
         prompt = "Hello, my name is"
         completion = llm.complete(
             prompt, engine="anthropic:claude-v1", max_tokens_to_sample=1).strip()
         self.assertTrue(completion.startswith("Claude"))
 
+    @vcr.use_cassette("tests/fixtures/claude/test_simple_chat.yaml", filter_headers=['authorization', 'x-api-key'])
+    def test_simple_chat(self):
+        self.assertEqual(llm.chat(["What is 2+2? Reply with just one number and no punctuation."], engine="anthropic:claude-v1"), "4")
+
     @vcr.use_cassette("tests/fixtures/claude/test_chat.yaml", filter_headers=['authorization', 'x-api-key'])
     def test_chat(self):
         messages = ["what is your favorite cat breed?", "I like tabbies.",
                     "And what about dogs? Reply with punctuation."]
         response = llm.chat(messages, engine="anthropic:claude-v1")
         self.assertTrue(response[0] != " ",
                         "Response should not start with a space.")
```

### Comparing `python-llm-0.1.1/tests/test_openai.py` & `python-llm-0.1.2/tests/test_openai.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,18 @@
         prompt = "Hello, my name is"
         completion = llm.complete(
             prompt, engine="openai:text-davinci-002", max_tokens=1)
         # Assert we only got one extra word that is capitalized
         self.assertEqual(len(completion.split(' ')), 1)
         self.assertTrue(completion[0].isupper(), completion)
 
+    @vcr.use_cassette("tests/fixtures/openai/test_simple_chat.yaml", filter_headers=['authorization', 'x-api-key'])
+    def test_simple_chat(self):
+        self.assertEqual(llm.chat(["What is 2+2? Reply with just one number and no punctuaction."], engine="openai:gpt-3.5-turbo"), "4")
+
     @vcr.use_cassette("tests/fixtures/openai/test_completion_chat_model.yaml", filter_headers=['authorization'])
     def test_completion_chat_model(self):
         """Test that we can use a chat model for completion."""
         prompt = "Hello, my name is"
         completion = llm.complete(
             prompt, engine="openai:gpt-3.5-turbo", max_tokens=1)
         # Assert we only got one extra word that is capitalized
```

