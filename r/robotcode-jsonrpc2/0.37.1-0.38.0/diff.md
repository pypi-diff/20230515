# Comparing `tmp/robotcode_jsonrpc2-0.37.1.tar.gz` & `tmp/robotcode_jsonrpc2-0.38.0.tar.gz`

## Comparing `robotcode_jsonrpc2-0.37.1.tar` & `robotcode_jsonrpc2-0.38.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/src/robotcode/jsonrpc2/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/src/robotcode/jsonrpc2/__version__.py
--rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/src/robotcode/jsonrpc2/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/src/robotcode/jsonrpc2/py.typed
--rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/src/robotcode/jsonrpc2/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/LICENSE.txt
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/README.md
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/pyproject.toml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.37.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/src/robotcode/jsonrpc2/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/src/robotcode/jsonrpc2/__version__.py
+-rw-r--r--   0        0        0    27794 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/src/robotcode/jsonrpc2/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/src/robotcode/jsonrpc2/py.typed
+-rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/src/robotcode/jsonrpc2/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/LICENSE.txt
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/README.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/pyproject.toml
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.38.0/PKG-INFO
```

### Comparing `robotcode_jsonrpc2-0.37.1/src/robotcode/jsonrpc2/protocol.py` & `robotcode_jsonrpc2-0.38.0/src/robotcode/jsonrpc2/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,15 +606,15 @@
                         while not done.is_set():
                             if time.monotonic() - start > 120:
                                 raise TimeoutError("Can't set future result.")
 
                             await asyncio.sleep(0)
 
                     else:
-                        self.__logger.warning(lambda: f"Response {repr(entry)} loop is not running.")
+                        self.__logger.warning(lambda: f"Response {entry!r} loop is not running.")
 
         except (SystemExit, KeyboardInterrupt):
             raise
         except BaseException as e:
             if not entry.future.done():
                 if entry.future.get_loop() == asyncio.get_running_loop():
                     entry.future.set_exception(e)
@@ -722,15 +722,15 @@
                     ex = t.exception()
                     if ex is not None:
                         self.__logger.exception(ex, exc_info=ex)
                         raise JsonRPCErrorException(JsonRPCErrors.INTERNAL_ERROR, f"{type(ex).__name__}: {ex}") from ex
 
                 self.send_response(message.id, t.result())
             except asyncio.CancelledError:
-                self.__logger.debug(lambda: f"request message {repr(message)} canceled")
+                self.__logger.debug(lambda: f"request message {message!r} canceled")
                 self.send_error(JsonRPCErrors.REQUEST_CANCELLED, "Request canceled.", id=message.id)
             except (SystemExit, KeyboardInterrupt):
                 raise
             except JsonRPCErrorException as e:
                 self.send_error(e.code, e.message or f"{type(e).__name__}: {e}", id=message.id, data=e.data)
             except BaseException as e:
                 self.__logger.exception(e)
```

### Comparing `robotcode_jsonrpc2-0.37.1/src/robotcode/jsonrpc2/server.py` & `robotcode_jsonrpc2-0.38.0/src/robotcode/jsonrpc2/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.37.1/.gitignore` & `robotcode_jsonrpc2-0.38.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.37.1/LICENSE.txt` & `robotcode_jsonrpc2-0.38.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.37.1/README.md` & `robotcode_jsonrpc2-0.38.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.37.1/pyproject.toml` & `robotcode_jsonrpc2-0.38.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotcode-core==0.37.1"]
+dependencies = ["robotcode-core==0.38.0"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
 Changelog = "https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md"
```

### Comparing `robotcode_jsonrpc2-0.37.1/PKG-INFO` & `robotcode_jsonrpc2-0.38.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-jsonrpc2
-Version: 0.37.1
+Version: 0.38.0
 Summary: JSONRPC Server for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.37.1
+Requires-Dist: robotcode-core==0.38.0
 Description-Content-Type: text/markdown
 
 # robotcode-jsonrpc2
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
```

