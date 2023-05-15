# Comparing `tmp/pydantic_chatcompletion-0.0.2.tar.gz` & `tmp/pydantic_chatcompletion-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_chatcompletion-0.0.2.tar", last modified: Fri Apr 28 18:49:25 2023, max compression
+gzip compressed data, was "pydantic_chatcompletion-0.0.3.tar", last modified: Mon May 15 13:57:30 2023, max compression
```

## Comparing `pydantic_chatcompletion-0.0.2.tar` & `pydantic_chatcompletion-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 18:49:25.280637 pydantic_chatcompletion-0.0.2/
--rw-r--r--   0 wsk        (501) staff       (20)     4158 2023-04-28 18:49:25.280357 pydantic_chatcompletion-0.0.2/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     3427 2023-04-28 14:53:00.000000 pydantic_chatcompletion-0.0.2/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 18:49:25.278560 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion/
--rw-r--r--   0 wsk        (501) staff       (20)     1946 2023-04-28 18:47:15.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion/__init__.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 18:49:25.280005 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     4158 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      294 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       16 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       24 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      866 2023-04-28 18:40:28.000000 pydantic_chatcompletion-0.0.2/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-28 18:49:25.280727 pydantic_chatcompletion-0.0.2/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 13:57:30.674988 pydantic_chatcompletion-0.0.3/
+-rw-r--r--   0 wsk        (501) staff       (20)     4158 2023-05-15 13:57:30.674721 pydantic_chatcompletion-0.0.3/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     3427 2023-04-28 14:53:00.000000 pydantic_chatcompletion-0.0.3/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 13:57:30.672992 pydantic_chatcompletion-0.0.3/pydantic_chatcompletion/
+-rw-r--r--   0 wsk        (501) staff       (20)     2097 2023-05-15 13:54:47.000000 pydantic_chatcompletion-0.0.3/pydantic_chatcompletion/__init__.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 13:57:30.674349 pydantic_chatcompletion-0.0.3/pydantic_chatcompletion.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     4158 2023-05-15 13:57:30.000000 pydantic_chatcompletion-0.0.3/pydantic_chatcompletion.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      294 2023-05-15 13:57:30.000000 pydantic_chatcompletion-0.0.3/pydantic_chatcompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-15 13:57:30.000000 pydantic_chatcompletion-0.0.3/pydantic_chatcompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       16 2023-05-15 13:57:30.000000 pydantic_chatcompletion-0.0.3/pydantic_chatcompletion.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       24 2023-05-15 13:57:30.000000 pydantic_chatcompletion-0.0.3/pydantic_chatcompletion.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      866 2023-05-15 13:55:02.000000 pydantic_chatcompletion-0.0.3/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-15 13:57:30.675070 pydantic_chatcompletion-0.0.3/setup.cfg
```

### Comparing `pydantic_chatcompletion-0.0.2/PKG-INFO` & `pydantic_chatcompletion-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_chatcompletion
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around OpenAI ChatCompletion that compels the language model to produce a valid Pydantic model as output via prompting and iterative error remediation.  The easiest way to go from unstructured text to structured Pydantic data.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/pydantic-chatcompletion
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/pydantic-chatcompletion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydantic_chatcompletion-0.0.2/README.md` & `pydantic_chatcompletion-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_chatcompletion-0.0.2/pydantic_chatcompletion/__init__.py` & `pydantic_chatcompletion-0.0.3/pydantic_chatcompletion/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,30 @@
 
     messages.append({"role"   : "system",
                      "content": f"Please respond ONLY with valid json that conforms to this pydantic json_schema: {model_class.schema_json()}. Do not include additional text other than the object json as we will load this object with json.loads() and pydantic."})
 
     last_exception = None
     for i in range(retry+1):
         response = openai.ChatCompletion.create(messages=messages, temperature=temperature, **kwargs)
-        content = response['choices'][0]['message']['content']
+        assistant_message= response['choices'][0]['message']
+        content = assistant_message['content']
         try:
             json_content = json.loads(content)
         except Exception as e:
             last_exception = e
             error_msg = f"json.loads exception: {e}"
             logging.error(error_msg)
+            messages.append(assistant_message)
             messages.append({"role"   : "system",
                             "content": error_msg})
             continue
         try:
             return model_class(**json_content)
         except ValidationError as e:
             last_exception = e
             error_msg = f"pydantic exception: {e}"
             logging.error(error_msg)
+            messages.append(assistant_message)            
             messages.append({"role"   : "system",
                             "content": error_msg})    
     raise last_exception
```

### Comparing `pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/PKG-INFO` & `pydantic_chatcompletion-0.0.3/pydantic_chatcompletion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-chatcompletion
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around OpenAI ChatCompletion that compels the language model to produce a valid Pydantic model as output via prompting and iterative error remediation.  The easiest way to go from unstructured text to structured Pydantic data.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/pydantic-chatcompletion
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/pydantic-chatcompletion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydantic_chatcompletion-0.0.2/pyproject.toml` & `pydantic_chatcompletion-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pydantic_chatcompletion"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['openai', 'pydantic']
 description = "Wrapper around OpenAI ChatCompletion that compels the language model to produce a valid Pydantic model as output via prompting and iterative error remediation.  The easiest way to go from unstructured text to structured Pydantic data."
 readme = "README.md"
 requires-python = ">=3.9"
```

