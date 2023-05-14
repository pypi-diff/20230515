# Comparing `tmp/zyncify-0.1.5-py2.py3-none-any.whl.zip` & `tmp/zyncify-0.1.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17198 bytes, number of entries: 12
--rw-r--r--  2.0 unx      146 b- defN 23-May-14 14:49 zync/__init__.py
--rw-r--r--  2.0 unx     2862 b- defN 23-May-14 16:52 zync/logger.py
+Zip file size: 17239 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      166 b- defN 23-May-14 22:32 zync/__init__.py
+-rw-r--r--  2.0 unx     3900 b- defN 23-May-14 22:34 zync/logger.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-13 13:21 zync/logging.py
--rw-r--r--  2.0 unx     1470 b- defN 23-May-14 16:53 zync/main.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-May-14 18:56 zync/main.py
 -rw-r--r--  2.0 unx      838 b- defN 23-May-13 13:15 zync/slugify.py
 -rw-r--r--  2.0 unx      966 b- defN 23-May-13 14:31 zync/zync.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1844 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      904 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/RECORD
-12 files, 44814 bytes uncompressed, 15698 bytes compressed:  65.0%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-14 22:38 zyncify-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2098 b- defN 23-May-14 22:38 zyncify-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-14 22:38 zyncify-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-May-14 22:38 zyncify-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-14 22:38 zyncify-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-May-14 22:38 zyncify-0.1.6.dist-info/RECORD
+12 files, 46126 bytes uncompressed, 15739 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zync/slugify.py
 Comment: 
 
 Filename: zync/zync.py
 Comment: 
 
-Filename: zyncify-0.1.5.dist-info/LICENSE
+Filename: zyncify-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: zyncify-0.1.5.dist-info/METADATA
+Filename: zyncify-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: zyncify-0.1.5.dist-info/WHEEL
+Filename: zyncify-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: zyncify-0.1.5.dist-info/entry_points.txt
+Filename: zyncify-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: zyncify-0.1.5.dist-info/top_level.txt
+Filename: zyncify-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: zyncify-0.1.5.dist-info/RECORD
+Filename: zyncify-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zync/__init__.py

```diff
@@ -1,9 +1,10 @@
-from .logger import logger, bugger
+from .logger import logger, bugger, egger
 from .slugify import Slugger, slugger
 
 __all__ = [
     "bugger",
     "logger",
+    "egger",
     "Slugger",
     "slugger",
 ]
```

## zync/logger.py

```diff
@@ -1,21 +1,19 @@
 import logging
 import inspect
-import os
 
 
-ROOT_PATH = os.getcwd() + "/"
-
 W = "\033[39m"
 B = "\033[94m"
 G = "\033[92m"
 Y = "\033[33m"
 R = "\033[91m"
 M = "\033[35m"
 C = "\033[36m"
+L = "\033[2m"
 X = "\033[0m"
 
 
 class BuggerFormat(logging.Formatter):
     def format(self, record):
         record.levelname = "bugger"
         levelname = record.levelname.upper()
@@ -27,28 +25,33 @@
     def format(self, record):
         record.levelname = "logger"
         levelname = record.levelname.upper()
         record.levelname = levelname
         return super().format(record)
 
 
+class EggerFormat(logging.Formatter):
+    def format(self, record):
+        record.levelname = "egger"
+        levelname = record.levelname.upper()
+        record.levelname = levelname
+        return super().format(record)
+
+
 class Bugger:
     def __init__(self, name):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.DEBUG)
         file_handler = logging.FileHandler(".zync.log")
         formatter = BuggerFormat(
             f"{G}[{X}"
-            f"{G}%(levelname)s{X}"
-            f"{R}:{X}"
-            f"{C}%(line)s{X}"
-            f"{G}@{X}"
-            f"{M}%(location)s{X}"
-            f"{G}%(asctime)s{X}"
+            f"{G}%(levelname)s:{X}"
+            f"{G}{L}%(asctime)s{X}"
             f"{G}]{X}"
+            f"{M}%(location)s{X}"
             f"{G}> {X}"
             f"%(message)s{X}",
             datefmt="%H:%M:%S",
         )
         file_handler.setFormatter(formatter)
         self.logger.addHandler(file_handler)
 
@@ -59,48 +62,74 @@
 class Logger:
     def __init__(self, name):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.INFO)
         file_handler = logging.FileHandler(".zync.log")
         formatter = LoggerFormat(
             f"{Y}[{X}"
-            f"{Y}%(levelname)s{X}"
-            f"{R}:{X}"
-            f"{C}%(line)s{X}"
-            f"{Y}@{X}"
-            f"{M}%(location)s{X}"
-            f"{Y}%(asctime)s{X}"
+            f"{Y}%(levelname)s:{X}"
+            f"{Y}{L}%(asctime)s{X}"
             f"{Y}]{X}"
+            f"{M}%(location)s{X}"
             f"{Y}> {X}"
             f"%(message)s{X}",
             datefmt="%H:%M:%S",
         )
         file_handler.setFormatter(formatter)
         self.logger.addHandler(file_handler)
 
     def __call__(self, log, line, location):
         self.logger.info(log, extra={"line": line, "location": location})
 
 
-bugger_base = Bugger("bugger")
-logger_base = Logger("logger")
+class Egger:
+    def __init__(self, name):
+        self.logger = logging.getLogger(name)
+        self.logger.setLevel(logging.ERROR)
+        file_handler = logging.FileHandler(".zync.log")
+        formatter = EggerFormat(
+            f"{R}[{X}"
+            f"{R}%(levelname)s:{X}"
+            f"{R}{L}%(asctime)s{X}"
+            f"{R}]{X}"
+            f"{M}%(location)s{X}"
+            f"{R}> {X}"
+            f"%(message)s{X}",
+            datefmt="%H:%M:%S",
+        )
+        file_handler.setFormatter(formatter)
+        self.logger.addHandler(file_handler)
 
+    def __call__(self, log, line, location):
+        self.logger.error(log, extra={"line": line, "location": location})
 
-def strip_root_path(file_path, root_path):
-    relative_path = os.path.relpath(file_path, root_path)
-    return relative_path
+
+bugger_base = Bugger("bugger")
+logger_base = Logger("logger")
+egger_base = Egger("egger")
 
 
 def bugger(log):
     frame = inspect.currentframe().f_back
+    path = inspect.getframeinfo(frame).filename
     line = inspect.getframeinfo(frame).positions.lineno
-    file_path = frame.f_code.co_filename
-    location = strip_root_path(file_path, ROOT_PATH)
-    return bugger_base(log, line, location)
+    col = inspect.getframeinfo(frame).positions.col_offset
+    url = "%s:%s:%s" % (path, line, col)
+    return bugger_base(log, line, url)
 
 
 def logger(log):
     frame = inspect.currentframe().f_back
+    path = inspect.getframeinfo(frame).filename
+    line = inspect.getframeinfo(frame).positions.lineno
+    col = inspect.getframeinfo(frame).positions.col_offset
+    url = "%s:%s:%s" % (path, line, col)
+    return logger_base(log, line, url)
+
+
+def egger(log):
+    frame = inspect.currentframe().f_back
+    path = inspect.getframeinfo(frame).filename
     line = inspect.getframeinfo(frame).positions.lineno
-    file_path = frame.f_code.co_filename
-    location = strip_root_path(file_path, ROOT_PATH)
-    return logger_base(log, line, location)
+    col = inspect.getframeinfo(frame).positions.col_offset
+    url = "%s:%s:%s" % (path, line, col)
+    return egger_base(log, line, url)
```

## zync/main.py

```diff
@@ -5,15 +5,15 @@
 import argparse
 from .__init__ import __all__ as methods
 
 NAME = "zyncify"
 DISPLAY_NAME = "zync"
 DESCRIPTION = "zync is a utility tool for python operations"
 URL = "https://github.com/tjbredemeyer/zync"
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 AUTHOR = "TJ Bredemeyer"
 AUTHOR_EMAIL = "tj@teicor.com"
 LICENSE = "GNU Public License v3"
 
 info_string = (
     "\n"
     f"name: {DISPLAY_NAME}\n"
```

## Comparing `zyncify-0.1.5.dist-info/LICENSE` & `zyncify-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zyncify-0.1.5.dist-info/METADATA` & `zyncify-0.1.6.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyncify
-Version: 0.1.5
+Version: 0.1.6
 Summary: zync is a utility tool for python operations
 Home-page: https://github.com/tjbredemeyer/zync
 Author: TJ Bredemeyer
 Author-email: tj@teicor.com
 License: GNU Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,15 +27,15 @@
 
 ```python
 from zync import *
 ```
 
 ### 2. FUNCTIONS
 
-#### 1. logger
+#### logger
 
 logger takes in a string and logs it with an INFO level.  
 
 ```python
 from zync import logger
 
 # logging a string INFO
@@ -45,15 +45,15 @@
 message = "info message"
 logger(message)
 
 ###
 # returns: INFO info message
 ```  
 
-#### 2. bugger
+#### bugger
 
 bugger takes in a string and logs it with a DEBUG level.  
 
 ```python
 from zync import bugger
 
 # logging a string DEBUG
@@ -63,15 +63,33 @@
 message = "debug message"
 bugger(message)
 
 ###
 # returns: DEBUG debug message
 ```  
 
-#### 3. Slugger  
+#### egger
+
+egger takes in a string and logs it with an ERROR level.  
+
+```python
+from zync import egger
+
+# logging a string ERROR
+egger("error message")
+
+# logging a variable ERROR
+message = "error message"
+egger(message)
+
+###
+# returns: ERROR debug message
+```  
+
+#### Slugger  
 
 Slugger converts a string to slug while maintaining capitalization.  
 
 ```python
 from zync import Slugger
 
 # Slugging a string with Caps
@@ -81,15 +99,15 @@
 string = "Test String"
 Slugger(string)
 
 ###
 # returns: Test-String
 ```  
   
-#### 4. slugger  
+#### slugger  
 
 slugger converts a string to a slug with no capitalization.
 
 ```python
 from zync import slugger
 
 # Slugging a string without Caps
```

