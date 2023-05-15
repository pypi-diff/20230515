# Comparing `tmp/GoogleBard-1.0.1.tar.gz` & `tmp/GoogleBard-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.0.1.tar", last modified: Mon May 15 01:24:21 2023, max compression
+gzip compressed data, was "GoogleBard-1.0.2.tar", last modified: Mon May 15 01:34:31 2023, max compression
```

## Comparing `GoogleBard-1.0.1.tar` & `GoogleBard-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 01:23:59.000000 GoogleBard-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-15 01:23:59.000000 GoogleBard-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 01:23:59.000000 GoogleBard-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-15 01:23:59.000000 GoogleBard-1.0.1/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:34:31.348787 GoogleBard-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 01:34:09.000000 GoogleBard-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-15 01:34:31.348787 GoogleBard-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-15 01:34:09.000000 GoogleBard-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:34:31.348787 GoogleBard-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 01:34:09.000000 GoogleBard-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:34:31.348787 GoogleBard-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-15 01:34:09.000000 GoogleBard-1.0.2/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:34:31.348787 GoogleBard-1.0.2/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-15 01:34:31.000000 GoogleBard-1.0.2/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-15 01:34:31.000000 GoogleBard-1.0.2/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:34:31.000000 GoogleBard-1.0.2/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 01:34:31.000000 GoogleBard-1.0.2/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 01:34:31.000000 GoogleBard-1.0.2/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.0.1/LICENSE` & `GoogleBard-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.0.1/PKG-INFO` & `GoogleBard-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.0.1
+Version: 1.0.2
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.0.1/README.md` & `GoogleBard-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.0.1/setup.py` & `GoogleBard-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.0.1",
+    version="1.0.2",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.0.1/src/Bard.py` & `GoogleBard-1.0.2/src/Bard.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 
 
 def __create_completer(commands: list, pattern_str: str = "$") -> WordCompleter:
     return WordCompleter(words=commands, pattern=re.compile(pattern_str))
 
 
 def __get_input(
-    session: PromptSession = None,
+    prompt_sess: PromptSession = None,
     completer: WordCompleter = None,
     key_bindings: KeyBindings = None,
 ) -> str:
     """
     Multiline input function.
     """
     return (
-        session.prompt(
+        prompt_sess.prompt(
             completer=completer,
             multiline=True,
             auto_suggest=AutoSuggestFromHistory(),
             key_bindings=key_bindings,
         )
-        if session
+        if prompt_sess
         else prompt(multiline=True)
     )
 
 
 class Chatbot:
     """
     A class to interact with Google Bard.
@@ -104,15 +104,15 @@
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
         :return: A dict containing the response from Google Bard.
         """
         # url params
         params = {
-            "bl": "boq_assistant-bard-web-server_20230419.00_p1",
+            "bl": "boq_assistant-bard-web-server_20230510.09_p1",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
 
         # message arr -> data["f.req"]. Message is double json stringified
         message_struct = [
             [message],
@@ -183,15 +183,15 @@
     chatbot = Chatbot(args.session)
     prompt_session = __create_session()
     completions = __create_completer(["!exit", "!reset"])
 
     try:
         while True:
             console.print("You:")
-            user_prompt = __get_input(session=prompt_session, completer=completions)
+            user_prompt = __get_input(prompt_sess=prompt_session, completer=completions)
             console.print()
             if user_prompt == "!exit":
                 break
             elif user_prompt == "!reset":
                 chatbot.conversation_id = ""
                 chatbot.response_id = ""
                 chatbot.choice_id = ""
```

### Comparing `GoogleBard-1.0.1/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.0.2/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.0.1
+Version: 1.0.2
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

