# Comparing `tmp/ooliver_botbase-2.0.2.tar.gz` & `tmp/ooliver_botbase-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooliver_botbase-2.0.2.tar", max compression
+gzip compressed data, was "ooliver_botbase-2.0.3.tar", max compression
```

## Comparing `ooliver_botbase-2.0.2.tar` & `ooliver_botbase-2.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      144 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/README.md
--rw-r--r--   0        0        0      275 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/__init__.py
--rw-r--r--   0        0        0    13364 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/botbase.py
--rw-r--r--   0        0        0       73 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/db/__init__.py
--rw-r--r--   0        0        0      625 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/db/blacklist.py
--rw-r--r--   0        0        0      727 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/db/commands.py
--rw-r--r--   0        0        0      364 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/db/metadata.py
--rw-r--r--   0        0        0     6064 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/exts/blacklist.py
--rw-r--r--   0        0        0     1343 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/exts/log_commands.py
--rw-r--r--   0        0        0     1758 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/exts/log_guilds.py
--rw-r--r--   0        0        0      288 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/models.py
--rw-r--r--   0        0        0        1 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/py.typed
--rw-r--r--   0        0        0      309 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/__init__.py
--rw-r--r--   0        0        0      590 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/channel.py
--rw-r--r--   0        0        0     1391 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/inter.py
--rw-r--r--   0        0        0      253 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/member.py
--rw-r--r--   0        0        0      253 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/thread.py
--rw-r--r--   0        0        0      245 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/user.py
--rw-r--r--   0        0        0     4398 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/botbase/wraps/wrap.py
--rw-r--r--   0        0        0      800 2023-05-07 20:18:47.699059 ooliver_botbase-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 ooliver_botbase-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-05-14 23:03:17.592442 ooliver_botbase-2.0.3/README.md
+-rw-r--r--   0        0        0      275 2023-05-14 23:03:17.592442 ooliver_botbase-2.0.3/botbase/__init__.py
+-rw-r--r--   0        0        0    14541 2023-05-14 23:03:17.592442 ooliver_botbase-2.0.3/botbase/botbase.py
+-rw-r--r--   0        0        0       73 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/db/__init__.py
+-rw-r--r--   0        0        0      625 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/db/blacklist.py
+-rw-r--r--   0        0        0      727 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/db/commands.py
+-rw-r--r--   0        0        0      364 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/db/metadata.py
+-rw-r--r--   0        0        0     6064 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/exts/blacklist.py
+-rw-r--r--   0        0        0     1343 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/exts/log_commands.py
+-rw-r--r--   0        0        0     1758 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/exts/log_guilds.py
+-rw-r--r--   0        0        0      288 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/models.py
+-rw-r--r--   0        0        0        1 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/py.typed
+-rw-r--r--   0        0        0      309 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/wraps/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/wraps/channel.py
+-rw-r--r--   0        0        0     1391 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/wraps/inter.py
+-rw-r--r--   0        0        0      253 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/wraps/member.py
+-rw-r--r--   0        0        0      253 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/wraps/thread.py
+-rw-r--r--   0        0        0      245 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/wraps/user.py
+-rw-r--r--   0        0        0     4398 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/botbase/wraps/wrap.py
+-rw-r--r--   0        0        0      800 2023-05-14 23:03:17.596442 ooliver_botbase-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 ooliver_botbase-2.0.3/PKG-INFO
```

### Comparing `ooliver_botbase-2.0.2/botbase/botbase.py` & `ooliver_botbase-2.0.3/botbase/botbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import traceback
 from asyncio import TimeoutError as AsyncTimeoutError
 from asyncio import wait_for
 from contextlib import suppress
 from logging import CRITICAL, INFO, Formatter, StreamHandler, getLogger
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 from random import choice
@@ -216,23 +217,51 @@
         return choice(self.colours)
 
     def asyncio_handler(self, _, context: dict) -> None:
         log = getLogger("notasyncio")
         if context["message"] == "Unclosed client session":
             return
 
-        log.error(
-            context["message"]
-            + "\n"
-            + "\n".join(
-                f"{k}: {v}"
-                for k, v in context.items()
-                if k != "message" and k is not None and v is not None and k != "None"
-            )
-        )
+        message = context.get("message")
+        if not message:
+            message = "Unhandled exception in event loop"
+
+        exception = context.get("exception")
+        if exception is not None:
+            exc_info = (type(exception), exception, exception.__traceback__)
+        else:
+            exc_info = False
+
+        if (
+            "source_traceback" not in context
+            and self.loop._current_handle is not None  # pyright: ignore
+            and self.loop._current_handle._source_traceback  # pyright: ignore
+        ):
+            context[
+                "handle_traceback"
+            ] = self.loop._current_handle._source_traceback  # pyright: ignore
+
+        log_lines = [message]
+        for key in sorted(context):
+            if key in {"message", "exception"}:
+                continue
+            value = context[key]
+            if key == "source_traceback":
+                tb = "".join(traceback.format_list(value))
+                value = "Object created at (most recent call last):\n"
+                value += tb.rstrip()
+            elif key == "handle_traceback":
+                tb = "".join(traceback.format_list(value))
+                value = "Handle created at (most recent call last):\n"
+                value += tb.rstrip()
+            else:
+                value = repr(value)
+            log_lines.append(f"{key}: {value}")
+
+        log.error("\n".join(log_lines), exc_info=exc_info)
 
     async def start(self, token: str, *, reconnect: bool = True) -> None:
         if self.db_enabled:
             from .db import database
 
             await database.connect()
```

### Comparing `ooliver_botbase-2.0.2/botbase/db/blacklist.py` & `ooliver_botbase-2.0.3/botbase/db/blacklist.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.2/botbase/db/commands.py` & `ooliver_botbase-2.0.3/botbase/db/commands.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.2/botbase/exts/blacklist.py` & `ooliver_botbase-2.0.3/botbase/exts/blacklist.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.2/botbase/exts/log_commands.py` & `ooliver_botbase-2.0.3/botbase/exts/log_commands.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.2/botbase/exts/log_guilds.py` & `ooliver_botbase-2.0.3/botbase/exts/log_guilds.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.2/botbase/wraps/channel.py` & `ooliver_botbase-2.0.3/botbase/wraps/channel.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.2/botbase/wraps/inter.py` & `ooliver_botbase-2.0.3/botbase/wraps/inter.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.2/botbase/wraps/wrap.py` & `ooliver_botbase-2.0.3/botbase/wraps/wrap.py`

 * *Files identical despite different names*

### Comparing `ooliver_botbase-2.0.2/pyproject.toml` & `ooliver_botbase-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ooliver-botbase"
-version = "2.0.2"
+version = "2.0.3"
 description = "A personal nextcord bot base package for bots."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 repository = "https://github.com/ooliver1/botbase"
 packages = [{ include = "botbase" }]
 readme = "README.md"
```

### Comparing `ooliver_botbase-2.0.2/PKG-INFO` & `ooliver_botbase-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooliver-botbase
-Version: 2.0.2
+Version: 2.0.3
 Summary: A personal nextcord bot base package for bots.
 Home-page: https://github.com/ooliver1/botbase
 License: MIT
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

