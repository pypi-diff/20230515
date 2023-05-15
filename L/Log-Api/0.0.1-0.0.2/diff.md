# Comparing `tmp/Log_Api-0.0.1.tar.gz` & `tmp/Log_Api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Log_Api-0.0.1.tar", last modified: Mon May 15 16:05:15 2023, max compression
+gzip compressed data, was "Log_Api-0.0.2.tar", last modified: Mon May 15 17:00:00 2023, max compression
```

## Comparing `Log_Api-0.0.1.tar` & `Log_Api-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 16:05:15.175000 Log_Api-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-15 16:05:15.143638 Log_Api-0.0.1/Log_Api/
-drwxrwxrwx   0        0        0        0 2023-05-15 16:05:15.169002 Log_Api-0.0.1/Log_Api/Class/
--rw-rw-rw-   0        0        0     2068 2023-05-10 16:27:14.000000 Log_Api-0.0.1/Log_Api/Class/Database.py
--rw-rw-rw-   0        0        0     3215 2023-05-12 22:10:14.000000 Log_Api-0.0.1/Log_Api/Class/LogAPI.py
--rw-rw-rw-   0        0        0       73 2023-05-12 15:13:08.000000 Log_Api-0.0.1/Log_Api/Class/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-09 15:46:14.000000 Log_Api-0.0.1/Log_Api/Class/response..py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:05:15.171994 Log_Api-0.0.1/Log_Api/Models/
--rw-rw-rw-   0        0        0     2056 2023-05-12 15:48:36.000000 Log_Api-0.0.1/Log_Api/Models/LogAPI.py
--rw-rw-rw-   0        0        0       26 2023-05-12 22:13:22.000000 Log_Api-0.0.1/Log_Api/Models/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-12 15:12:55.000000 Log_Api-0.0.1/Log_Api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:05:15.161590 Log_Api-0.0.1/Log_Api.egg-info/
--rw-rw-rw-   0        0        0      284 2023-05-15 16:05:15.000000 Log_Api-0.0.1/Log_Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-05-15 16:05:15.000000 Log_Api-0.0.1/Log_Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 16:05:15.000000 Log_Api-0.0.1/Log_Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 08:11:28.000000 Log_Api-0.0.1/Log_Api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2023-05-15 16:05:15.000000 Log_Api-0.0.1/Log_Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-05-15 16:05:15.000000 Log_Api-0.0.1/Log_Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2023-05-15 16:05:15.173987 Log_Api-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3530 2023-05-12 20:14:59.000000 Log_Api-0.0.1/README.rst
--rw-rw-rw-   0        0        0    14467 2023-05-15 16:05:01.000000 Log_Api-0.0.1/aws_handler_decorators.py
--rw-rw-rw-   0        0        0       42 2023-05-15 16:05:15.175000 Log_Api-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-05-12 04:02:36.000000 Log_Api-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:00:00.954656 Log_Api-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-15 17:00:00.912038 Log_Api-0.0.2/Log_Api/
+drwxrwxrwx   0        0        0        0 2023-05-15 17:00:00.948674 Log_Api-0.0.2/Log_Api/Class/
+-rw-rw-rw-   0        0        0     2068 2023-05-15 16:56:09.000000 Log_Api-0.0.2/Log_Api/Class/Database.py
+-rw-rw-rw-   0        0        0     3212 2023-05-15 16:56:09.000000 Log_Api-0.0.2/Log_Api/Class/LogAPI.py
+-rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.2/Log_Api/Class/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.2/Log_Api/Class/response..py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:00:00.951665 Log_Api-0.0.2/Log_Api/Models/
+-rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.2/Log_Api/Models/LogAPI.py
+-rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.2/Log_Api/Models/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-15 16:56:09.000000 Log_Api-0.0.2/Log_Api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 17:00:00.941522 Log_Api-0.0.2/Log_Api.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-05-15 17:00:00.000000 Log_Api-0.0.2/Log_Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-15 17:00:00.000000 Log_Api-0.0.2/Log_Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 17:00:00.000000 Log_Api-0.0.2/Log_Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.2/Log_Api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2023-05-15 17:00:00.000000 Log_Api-0.0.2/Log_Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-05-15 17:00:00.000000 Log_Api-0.0.2/Log_Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2023-05-15 17:00:00.953659 Log_Api-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.2/README.md
+-rw-rw-rw-   0        0        0    14467 2023-05-15 16:59:53.000000 Log_Api-0.0.2/aws_handler_decorators.py
+-rw-rw-rw-   0        0        0       42 2023-05-15 17:00:00.954656 Log_Api-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-05-15 16:56:09.000000 Log_Api-0.0.2/setup.py
```

### Comparing `Log_Api-0.0.1/Log_Api/Class/Database.py` & `Log_Api-0.0.2/Log_Api/Class/Database.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.1/Log_Api/Class/LogAPI.py` & `Log_Api-0.0.2/Log_Api/Class/LogAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from json import dumps
-from Class.Database import Database, IntegrityError
-from Models.LogAPI import LogAPI
+from .Database import Database, IntegrityError
+from ..Models.LogAPI import LogAPI
 
 def log_resquest_response(api_func):
     def wrapper(*args, **kwargs):
         request = __request(*args, **kwargs)
         response = api_func(*args, **kwargs)
         __response(request, response)
         return response
```

### Comparing `Log_Api-0.0.1/Log_Api/Class/response..py` & `Log_Api-0.0.2/Log_Api/Class/response..py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.1/Log_Api/Models/LogAPI.py` & `Log_Api-0.0.2/Log_Api/Models/LogAPI.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.1/README.rst` & `Log_Api-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 ```python
 from aws_handler_decorators import (
     async_handler, cors_headers, dump_json_body, json_http_resp, json_schema_validator,
     load_json_body, load_urlencoded_body, no_retry_on_failure, ssm_parameter_store,
     secret_manager, log_resquest_response
 )
 
-from Log_Api.Class.LogAPI import log_resquest_response
+from Log_Api import log_resquest_response
 
+@log_resquest_response be to used before the other decorators like this:
+* `json_schema_validator`
 See each individual decorators for specific usage details and the example_
 for some more use cases. This library is also meant to serve as an example for how to write
 decorators for use as lambda middleware.
 
 I was inspired by `dschep <https://github.com/dschep>`_
```

### Comparing `Log_Api-0.0.1/aws_handler_decorators.py` & `Log_Api-0.0.2/aws_handler_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     basestring
 except NameError:
     basestring = str
 
 logger = logging.getLogger(__name__)
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 class AwsHandlerDecorator(object):
     def __init__(self, func):
         update_wrapper(self, func)
         self.func = func
 
     def __call__(self, event, context):
```

### Comparing `Log_Api-0.0.1/setup.py` & `Log_Api-0.0.2/setup.py`

 * *Files identical despite different names*

