# Comparing `tmp/anthropic-0.2.8.tar.gz` & `tmp/anthropic-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic-0.2.8.tar", last modified: Mon May  8 20:08:00 2023, max compression
+gzip compressed data, was "anthropic-0.2.9.tar", last modified: Mon May 15 15:42:59 2023, max compression
```

## Comparing `anthropic-0.2.8.tar` & `anthropic-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:08:00.603917 anthropic-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-08 20:07:49.000000 anthropic-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-08 20:08:00.603917 anthropic-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-08 20:07:49.000000 anthropic-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:08:00.603917 anthropic-0.2.8/anthropic/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 20:07:49.000000 anthropic-0.2.8/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-08 20:07:49.000000 anthropic-0.2.8/anthropic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-08 20:07:49.000000 anthropic-0.2.8/anthropic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-08 20:07:49.000000 anthropic-0.2.8/anthropic/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:08:00.603917 anthropic-0.2.8/anthropic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-08 20:07:49.000000 anthropic-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:08:00.603917 anthropic-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:08:00.603917 anthropic-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-08 20:07:49.000000 anthropic-0.2.8/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:42:58.999925 anthropic-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-15 15:42:47.000000 anthropic-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-15 15:42:58.999925 anthropic-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-15 15:42:47.000000 anthropic-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:42:58.999925 anthropic-0.2.9/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 15:42:47.000000 anthropic-0.2.9/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-05-15 15:42:47.000000 anthropic-0.2.9/anthropic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-15 15:42:47.000000 anthropic-0.2.9/anthropic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-15 15:42:47.000000 anthropic-0.2.9/anthropic/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:42:58.999925 anthropic-0.2.9/anthropic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-15 15:42:58.000000 anthropic-0.2.9/anthropic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 15:42:58.000000 anthropic-0.2.9/anthropic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:42:58.000000 anthropic-0.2.9/anthropic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-15 15:42:58.000000 anthropic-0.2.9/anthropic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 15:42:58.000000 anthropic-0.2.9/anthropic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-15 15:42:47.000000 anthropic-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:42:58.999925 anthropic-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:42:58.999925 anthropic-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-15 15:42:47.000000 anthropic-0.2.9/tests/test_api.py
```

### Comparing `anthropic-0.2.8/LICENSE` & `anthropic-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.2.8/PKG-INFO` & `anthropic-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library for accessing the anthropic API
 Author: Anthropic
 License: MIT
 Project-URL: homepage, https://github.com/anthropics/anthropic-sdk-python
 Project-URL: repository, https://github.com/anthropics/anthropic-sdk-python.git
 Keywords: anthropic,anthropicai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anthropic-0.2.8/README.md` & `anthropic-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `anthropic-0.2.8/anthropic/api.py` & `anthropic-0.2.9/anthropic/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,37 +226,37 @@
                 raise ApiException(e, f"Error processing stream data", line)
             yield json_body
 
     def completion_stream(self, **kwargs) -> Iterator[dict]:
         new_kwargs = {"stream": True, **kwargs}
         return self._request_as_stream(
             "post",
-            "/v1/complete",
+            "v1/complete",
             params=new_kwargs,
         )
 
     def completion(self, **kwargs) -> dict:
         return self._request_as_json(
             "post",
-            "/v1/complete",
+            "v1/complete",
             params=kwargs,
         )
 
     async def acompletion(self, **kwargs) -> dict:
         return await self._arequest_as_json(
             "post",
-            "/v1/complete",
+            "v1/complete",
             params=kwargs,
         )
 
     async def acompletion_stream(self, **kwargs) -> AsyncIterator[dict]:
         new_kwargs = {"stream": True, **kwargs}
         return self._arequest_as_stream(
             "post",
-            "/v1/complete",
+            "v1/complete",
             params=new_kwargs,
         )
 
 
 def _validate_request(params: dict) -> None:
     prompt: str = params["prompt"]
     if not prompt.startswith(constants.HUMAN_PROMPT):
```

### Comparing `anthropic-0.2.8/anthropic/tokenizer.py` & `anthropic-0.2.9/anthropic/tokenizer.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.2.8/anthropic.egg-info/PKG-INFO` & `anthropic-0.2.9/anthropic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library for accessing the anthropic API
 Author: Anthropic
 License: MIT
 Project-URL: homepage, https://github.com/anthropics/anthropic-sdk-python
 Project-URL: repository, https://github.com/anthropics/anthropic-sdk-python.git
 Keywords: anthropic,anthropicai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anthropic-0.2.8/pyproject.toml` & `anthropic-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
   "setuptools >= 61.0.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anthropic"
-version = "0.2.8"
+version = "0.2.9"
 description = "Library for accessing the anthropic API"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["anthropic", "anthropicai"]
 license = {text = "MIT"}
 authors = [
     {name = "Anthropic"}
```

### Comparing `anthropic-0.2.8/tests/test_api.py` & `anthropic-0.2.9/tests/test_api.py`

 * *Files identical despite different names*

