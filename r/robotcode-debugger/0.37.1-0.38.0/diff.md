# Comparing `tmp/robotcode_debugger-0.37.1.tar.gz` & `tmp/robotcode_debugger-0.38.0.tar.gz`

## Comparing `robotcode_debugger-0.37.1.tar` & `robotcode_debugger-0.38.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    49582 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/README.md
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/pyproject.toml
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.37.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    49522 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/README.md
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.38.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/debugger.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,18 +160,15 @@
         self._suite_marker = object()
         self._test_marker = object()
         self._local_marker = object()
         self._global_marker = object()
         self.stack_frames: Deque[StackFrameEntry] = deque()
 
     def __repr__(self) -> str:
-        return (
-            f"StackFrameEntry({repr(self.name)}, {repr(self.type)}, "
-            f"{repr(self.source)}, {repr(self.line)}, {repr(self.column)})"
-        )
+        return f"StackFrameEntry({self.name!r}, {self.type!r}, {self.source!r}, {self.line!r}, {self.column!r})"
 
     def get_first_or_self(self) -> StackFrameEntry:
         if self.stack_frames:
             return self.stack_frames[0]
         return self
 
     @property
```

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         try:
             self._handle_messages(self._generate_json_rpc_messages_from_dict(json.loads(body.decode(charset))))
         except (asyncio.CancelledError, SystemExit, KeyboardInterrupt):
             raise
         except BaseException as e:
             self._logger.exception(e)
             self.send_error(
-                f"Invalid Message: {type(e).__name__}: {str(e)} -> {str(body)}\n{traceback.format_exc()}",
+                f"Invalid Message: {type(e).__name__}: {e!s} -> {body!s}\n{traceback.format_exc()}",
                 error_message=Message(traceback.format_exc()),
             )
 
     def _handle_messages(self, iterator: Iterator[ProtocolMessage]) -> None:
         def done(f: asyncio.Future[Any]) -> None:
             ex = f.exception()
             if ex is not None and not isinstance(ex, asyncio.CancelledError):
@@ -240,15 +240,15 @@
 
             self._received_request[message.seq] = result
 
         def done(t: asyncio.Task[Any]) -> None:
             try:
                 self.send_response(message.seq, message.command, t.result())
             except asyncio.CancelledError:
-                self._logger.debug(lambda: f"request message {repr(message)} canceled")
+                self._logger.debug(lambda: f"request message {message!r} canceled")
             except (SystemExit, KeyboardInterrupt):
                 raise
             except DebugAdapterRPCErrorException as ex:
                 self._logger.exception(ex)
                 self.send_error(
                     message=ex.message,
                     request_seq=message.seq,
```

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/run.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import functools
-import sys
 import threading
 import warnings
 from typing import (
     TYPE_CHECKING,
     Callable,
     List,
     Optional,
@@ -218,16 +217,14 @@
                     ),
                     loop=server.loop,
                 )
 
                 await run_coroutine_from_thread_async(server.protocol.exit, exit_code, loop=server.loop)
     except asyncio.CancelledError:
         pass
-    except ConnectionError as e:
-        print(e, file=sys.stderr)
     finally:
         if server.protocol.connected:
             await run_coroutine_from_thread_async(server.protocol.terminate, loop=server.loop)
 
             try:
                 await run_coroutine_from_thread_async(server.protocol.wait_for_disconnected, loop=server.loop)
             except asyncio.TimeoutError:
```

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/server.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.38.0/src/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/.gitignore` & `robotcode_debugger-0.38.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/LICENSE.txt` & `robotcode_debugger-0.38.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/README.md` & `robotcode_debugger-0.38.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.37.1/pyproject.toml` & `robotcode_debugger-0.38.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.37.1",
-  "robotcode-runner==0.37.1",
+  "robotcode-jsonrpc2==0.38.0",
+  "robotcode-runner==0.38.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
```

### Comparing `robotcode_debugger-0.37.1/PKG-INFO` & `robotcode_debugger-0.38.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-debugger
-Version: 0.37.1
+Version: 0.38.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.37.1
-Requires-Dist: robotcode-runner==0.37.1
+Requires-Dist: robotcode-jsonrpc2==0.38.0
+Requires-Dist: robotcode-runner==0.38.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

