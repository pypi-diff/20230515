# Comparing `tmp/serverless-sdk-0.4.7.tar.gz` & `tmp/serverless-sdk-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-7l1hlh1m/serverless-sdk-0.4.7.tar", last modified: Tue May  9 14:21:54 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-ukj8y1ml/serverless-sdk-0.4.8.tar", last modified: Mon May 15 13:10:42 2023, max compression
```

## Comparing `serverless-sdk-0.4.7.tar` & `serverless-sdk-0.4.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/warning_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/warning_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.7/PKG-INFO` & `serverless-sdk-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.7
+Version: 0.4.8
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.4.7/README.md` & `serverless-sdk-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/pyproject.toml` & `serverless-sdk-0.4.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -63,11 +63,7 @@
 ]
 
 [tool.mypy]
 disable_error_code = "override,assignment,arg-type"
 exclude = [
     '^tests/',
 ]
-
-[tool.ruff]
-ignore = ["F401", "E722"]
-#fix = true
```

### Comparing `serverless-sdk-0.4.7/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.8/serverless_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.7
+Version: 0.4.8
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.4.7/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.4.8/serverless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/__init__.py` & `serverless-sdk-0.4.8/sls_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/base.py` & `serverless-sdk-0.4.8/sls_sdk/base.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/exceptions.py` & `serverless-sdk-0.4.8/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.4.8/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/emitter.py` & `serverless-sdk-0.4.8/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/error.py` & `serverless-sdk-0.4.8/sls_sdk/lib/error.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,10 +41,10 @@
         create_error_captured_event(
             error_data["message"],
             name=error_data["name"],
             stack=error_data["stack"],
             type="handledSdkUser" if type == "USER" else "handledSdkInternal",
             origin="pythonLogging",
         )
-    except:
+    except:  # noqa: E722
         # ignore
         pass
```

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.8/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,25 @@
 def reset_ignore_following_request():
     _IGNORE_FOLLOWING_REQUEST.set(False)
 
 
 _HTTP_SPAN = contextvars.ContextVar("http-span", default=None)
 
 
+def safe_call(func):
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except Exception:
+            return None
+
+    return wrapper
+
+
+@safe_call
 def _decode_body(body):
     if isinstance(body, bytes):
         return body.decode("utf-8")
     elif isinstance(body, str):
         return body
     elif isinstance(body, io.IOBase):
         if body.seekable():
```

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/wrapper.py` & `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/name.py` & `serverless-sdk-0.4.8/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.4.8/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/tags.py` & `serverless-sdk-0.4.8/sls_sdk/lib/tags.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/trace.py` & `serverless-sdk-0.4.8/sls_sdk/lib/trace.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/warning.py` & `serverless-sdk-0.4.8/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.8/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.7/tests/test_sdk.py` & `serverless-sdk-0.4.8/tests/test_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from unittest.mock import MagicMock
 
 from . import get_params
 
 
 def test_can_import_serverless_sdk(reset_sdk):
     try:
-        from sls_sdk import serverlessSdk
+        from sls_sdk import serverlessSdk  # noqa: F401
 
     except ImportError as e:
         raise AssertionError("Cannot import `serverlessSdk`") from e
 
 
 def test_has_name(instrumented_sdk):
     assert hasattr(instrumented_sdk, "name")
@@ -181,15 +181,15 @@
     tag_name = ""
     tag_value = "value"
 
     # when
     failed = False
     try:
         sdk.set_tag(tag_name, tag_value)
-    except:
+    except Exception:
         failed = True
 
     # then
     assert not failed
     mock.assert_called_once()
```

### Comparing `serverless-sdk-0.4.7/tests/test_thread_safety.py` & `serverless-sdk-0.4.8/tests/test_thread_safety.py`

 * *Files identical despite different names*

