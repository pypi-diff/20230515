# Comparing `tmp/langcorn-0.0.7.tar.gz` & `tmp/langcorn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcorn-0.0.7.tar", max compression
+gzip compressed data, was "langcorn-0.0.8.tar", max compression
```

## Comparing `langcorn-0.0.7.tar` & `langcorn-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2023-05-10 16:00:05.898921 langcorn-0.0.7/LICENSE
--rw-r--r--   0        0        0     7377 2023-05-10 16:00:05.898921 langcorn-0.0.7/Readme.md
--rw-r--r--   0        0        0       77 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/__init__.py
--rw-r--r--   0        0        0      417 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/__main__.py
--rw-r--r--   0        0        0        0 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/server/__init__.py
--rw-r--r--   0        0        0     4447 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/server/api.py
--rw-r--r--   0        0        0      999 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/server/test_api.py
--rw-r--r--   0        0        0      981 2023-05-10 16:00:05.898921 langcorn-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 langcorn-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-15 11:37:09.280660 langcorn-0.0.8/LICENSE
+-rw-r--r--   0        0        0     7377 2023-05-15 11:37:09.280660 langcorn-0.0.8/Readme.md
+-rw-r--r--   0        0        0       77 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/__init__.py
+-rw-r--r--   0        0        0      489 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/server/__init__.py
+-rw-r--r--   0        0        0     4648 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/server/api.py
+-rw-r--r--   0        0        0      999 2023-05-15 11:37:09.280660 langcorn-0.0.8/langcorn/server/test_api.py
+-rw-r--r--   0        0        0      981 2023-05-15 11:37:09.280660 langcorn-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 langcorn-0.0.8/PKG-INFO
```

### Comparing `langcorn-0.0.7/LICENSE` & `langcorn-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.7/Readme.md` & `langcorn-0.0.8/Readme.md`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.7/langcorn/server/api.py` & `langcorn-0.0.8/langcorn/server/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,15 +112,18 @@
     # Make local modules discoverable
     sys.path.append(os.path.dirname(__file__))
     logger.info("Creating service")
     app = app or FastAPI()
     endpoints = ["/docs"]
 
     _authenticate_or_401 = Depends(authenticate_or_401(auth_token=auth_token))
-
+    if lc_apps and isinstance(import_from_string(lc_apps[0]), FastAPI):
+        raise RuntimeError(
+            "Improperly configured: FastAPI instance passed instead of LangChain interface"
+        )
     for lang_app in lc_apps:
         chain = import_from_string(lang_app)
         inn, out = derive_fields(chain)
         logger.debug(f"inputs:{inn=}")
         logger.info(f"{lang_app=}:{chain.__class__.__name__}({inn})")
         endpoint_prefix = lang_app.split(":")[0]
         cls_name = "".join([c.capitalize() for c in endpoint_prefix.split(".")])
```

### Comparing `langcorn-0.0.7/langcorn/server/test_api.py` & `langcorn-0.0.8/langcorn/server/test_api.py`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.7/pyproject.toml` & `langcorn-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langcorn"
-version = "0.0.7"
+version = "0.0.8"
 description = "A Python package creating rest api interface for LangChain"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = [
     "Alexander Miasoiedov <msoedov@gmail.com>",
 ]
 repository = "https://github.com/msoedov/langcorn"
 license = "MIT"
```

### Comparing `langcorn-0.0.7/PKG-INFO` & `langcorn-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcorn
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python package creating rest api interface for LangChain
 Home-page: https://github.com/msoedov/langcorn
 License: MIT
 Keywords: nlp,langchain,openai,gpt,fastapi
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
```

