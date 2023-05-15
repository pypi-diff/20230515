# Comparing `tmp/GoogleBard-1.0.0.tar.gz` & `tmp/GoogleBard-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.0.0.tar", last modified: Sat Apr 22 12:42:52 2023, max compression
+gzip compressed data, was "GoogleBard-1.0.1.tar", last modified: Mon May 15 01:24:21 2023, max compression
```

## Comparing `GoogleBard-1.0.0.tar` & `GoogleBard-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-22 12:42:30.000000 GoogleBard-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-22 12:42:30.000000 GoogleBard-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 12:42:30.000000 GoogleBard-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-22 12:42:30.000000 GoogleBard-1.0.0/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:42:52.382361 GoogleBard-1.0.0/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 12:42:52.000000 GoogleBard-1.0.0/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 01:23:59.000000 GoogleBard-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-15 01:23:59.000000 GoogleBard-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 01:23:59.000000 GoogleBard-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-15 01:23:59.000000 GoogleBard-1.0.1/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:24:21.298010 GoogleBard-1.0.1/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 01:24:21.000000 GoogleBard-1.0.1/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.0.0/LICENSE` & `GoogleBard-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.0.0/PKG-INFO` & `GoogleBard-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.0.0/README.md` & `GoogleBard-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.0.0/setup.py` & `GoogleBard-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.0.0",
+    version="1.0.1",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.0.0/src/Bard.py` & `GoogleBard-1.0.1/src/Bard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Reverse engineering of Google Bard
 """
 import argparse
 import json
+import os
 import random
 import re
 import string
-import os
 import sys
 
 import requests
 from prompt_toolkit import prompt
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
@@ -50,40 +50,48 @@
 
 class Chatbot:
     """
     A class to interact with Google Bard.
     Parameters
         session_id: str
             The __Secure-1PSID cookie.
+        proxy: str
     """
 
     __slots__ = [
         "headers",
         "_reqid",
         "SNlM0e",
         "conversation_id",
         "response_id",
         "choice_id",
         "session",
     ]
 
-    def __init__(self, session_id):
+    def __init__(self, session_id: str, proxy: str = None):
         headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
         }
         self._reqid = int("".join(random.choices(string.digits, k=4)))
         self.conversation_id = ""
         self.response_id = ""
         self.choice_id = ""
         self.session = requests.Session()
+        if proxy:
+            self.session.proxies.update(
+                {
+                    "http": proxy,
+                    "https": proxy,
+                },
+            )
         self.session.headers = headers
         self.session.cookies.set("__Secure-1PSID", session_id)
         self.SNlM0e = self.__get_snlm0e()
 
     def __get_snlm0e(self):
         resp = self.session.get(url="https://bard.google.com/", timeout=10)
         # Find "SNlM0e":"<ID>"
```

### Comparing `GoogleBard-1.0.0/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.0.1/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

