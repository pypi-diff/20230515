# Comparing `tmp/python-redis-cache-2.1.0.tar.gz` & `tmp/python-redis-cache-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-redis-cache-2.1.0.tar", last modified: Thu May 11 21:13:56 2023, max compression
+gzip compressed data, was "python-redis-cache-2.1.1.tar", last modified: Mon May 15 06:43:11 2023, max compression
```

## Comparing `python-redis-cache-2.1.0.tar` & `python-redis-cache-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3182 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2897 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/python_redis_cache.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3182 2023-05-11 21:13:56.000000 python-redis-cache-2.1.0/python_redis_cache.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-11 21:13:56.000000 python-redis-cache-2.1.0/python_redis_cache.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 21:13:56.000000 python-redis-cache-2.1.0/python_redis_cache.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-11 21:13:56.000000 python-redis-cache-2.1.0/python_redis_cache.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/redis_cache/
--rw-r--r--   0 root         (0) root         (0)     7518 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/redis_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:43:11.154644 python-redis-cache-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-15 06:43:06.000000 python-redis-cache-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-15 06:43:11.154644 python-redis-cache-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-05-15 06:43:06.000000 python-redis-cache-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-15 06:43:06.000000 python-redis-cache-2.1.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:43:11.154644 python-redis-cache-2.1.1/python_redis_cache.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-15 06:43:11.000000 python-redis-cache-2.1.1/python_redis_cache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 06:43:11.000000 python-redis-cache-2.1.1/python_redis_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 06:43:11.000000 python-redis-cache-2.1.1/python_redis_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-15 06:43:11.000000 python-redis-cache-2.1.1/python_redis_cache.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:43:11.154644 python-redis-cache-2.1.1/redis_cache/
+-rw-r--r--   0 root         (0) root         (0)     8092 2023-05-15 06:43:06.000000 python-redis-cache-2.1.1/redis_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-15 06:43:11.154644 python-redis-cache-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-15 06:43:07.000000 python-redis-cache-2.1.1/setup.py
```

### Comparing `python-redis-cache-2.1.0/LICENSE` & `python-redis-cache-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-redis-cache-2.1.0/PKG-INFO` & `python-redis-cache-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-redis-cache
-Version: 2.1.0
+Version: 2.1.1
 Summary: Basic Redis caching for functions
 Home-page: http://github.com/taylorhakes/python-redis-cache
 Author: Taylor Hakes
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-redis-cache-2.1.0/README.md` & `python-redis-cache-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python-redis-cache-2.1.0/python_redis_cache.egg-info/PKG-INFO` & `python-redis-cache-2.1.1/python_redis_cache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-redis-cache
-Version: 2.1.0
+Version: 2.1.1
 Summary: Basic Redis caching for functions
 Home-page: http://github.com/taylorhakes/python-redis-cache
 Author: Taylor Hakes
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-redis-cache-2.1.0/redis_cache/__init__.py` & `python-redis-cache-2.1.1/redis_cache/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,42 @@
     This function parses the args and kwargs in the context of a function and creates unified
     dictionary of {<argument_name>: <value>}. This is useful
     because arguments can be passed as args or kwargs, and we want to make sure we cache
     them both the same. Otherwise there would be different caching for add(1, 2) and add(arg1=1, arg2=2)
     """
     arg_sig = signature(fn)
     standard_args = [param.name for param in arg_sig.parameters.values() if param.kind is param.POSITIONAL_OR_KEYWORD]
+    allowed_kwargs = [param.name for param in arg_sig.parameters.values() if param.kind is param.POSITIONAL_OR_KEYWORD or param.kind is param.KEYWORD_ONLY]
     variable_args = [param.name for param in arg_sig.parameters.values() if param.kind is param.VAR_POSITIONAL]
+    variable_kwargs = [param.name for param in arg_sig.parameters.values() if param.kind is param.VAR_KEYWORD]
     parsed_args = {}
 
-    if standard_args:
+    if standard_args or variable_args:
         for index, arg in enumerate(args):
             try:
                 parsed_args[standard_args[index]] = arg
             except IndexError:
                 # then fallback to using the positional varargs name
                 if variable_args:
                     vargs_name = variable_args[0]
-                    if not parsed_args[vargs_name]:
+                    if vargs_name not in parsed_args:
                         parsed_args[vargs_name] = []
 
                     parsed_args[vargs_name].append(arg)
 
-        # finally show the named varargs
+
     if kwargs:
-        parsed_args.update(kwargs)
+        for key, value in kwargs.items():
+            if key in allowed_kwargs:
+                parsed_args[key] = value
+            elif variable_kwargs:
+                vkwargs_name = variable_kwargs[0]
+                if vkwargs_name not in parsed_args:
+                    parsed_args[vkwargs_name] = {}
+                parsed_args[vkwargs_name][key] = value
 
     return parsed_args
 
 
 def get_cache_lua_fn(client):
     if not hasattr(client, '_lua_cache_fn'):
         client._lua_cache_fn = client.register_script("""
```

### Comparing `python-redis-cache-2.1.0/setup.py` & `python-redis-cache-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 setup(
     name='python-redis-cache',
     version=__version__,
     description='Basic Redis caching for functions',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

