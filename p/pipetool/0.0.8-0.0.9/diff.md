# Comparing `tmp/pipetool-0.0.8.tar.gz` & `tmp/pipetool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pipetool-0.0.8.tar", last modified: Mon Aug 22 07:06:57 2022, max compression
+gzip compressed data, was "dist\pipetool-0.0.9.tar", last modified: Fri Sep 16 14:00:56 2022, max compression
```

## Comparing `pipetool-0.0.8.tar` & `pipetool-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/
--rw-rw-rw-   0        0        0      296 2022-08-22 07:06:57.000000 pipetool-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/doc/
--rw-rw-rw-   0        0        0        0 2022-06-20 12:54:15.000000 pipetool-0.0.8/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/examples/
--rw-rw-rw-   0        0        0        0 2022-06-20 12:54:15.000000 pipetool-0.0.8/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool/
--rw-rw-rw-   0        0        0      117 2022-07-25 21:19:43.000000 pipetool-0.0.8/pipetool/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool/fileio/
--rw-rw-rw-   0        0        0      530 2022-08-11 00:41:26.000000 pipetool-0.0.8/pipetool/fileio/__init__.py
--rw-rw-rw-   0        0        0    42422 2022-07-25 08:15:27.000000 pipetool-0.0.8/pipetool/fileio/file_client.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool/fileio/handlers/
--rw-rw-rw-   0        0        0      382 2022-08-11 00:40:47.000000 pipetool-0.0.8/pipetool/fileio/handlers/__init__.py
--rw-rw-rw-   0        0        0     1017 2022-07-22 21:27:06.000000 pipetool-0.0.8/pipetool/fileio/handlers/base.py
--rw-rw-rw-   0        0        0      448 2022-08-11 01:32:27.000000 pipetool-0.0.8/pipetool/fileio/handlers/csv_handler.py
--rw-rw-rw-   0        0        0     1090 2022-07-25 02:51:50.000000 pipetool-0.0.8/pipetool/fileio/handlers/json_handler.py
--rw-rw-rw-   0        0        0     1269 2022-08-11 01:32:17.000000 pipetool-0.0.8/pipetool/fileio/handlers/jsons_handler.py
--rw-rw-rw-   0        0        0      753 2022-07-22 21:26:09.000000 pipetool-0.0.8/pipetool/fileio/handlers/pickle_handler.py
--rw-rw-rw-   0        0        0      701 2022-07-22 21:26:09.000000 pipetool-0.0.8/pipetool/fileio/handlers/yaml_handler.py
--rw-rw-rw-   0        0        0     6108 2022-08-11 00:41:55.000000 pipetool-0.0.8/pipetool/fileio/io.py
--rw-rw-rw-   0        0        0     3993 2022-08-11 01:04:36.000000 pipetool-0.0.8/pipetool/fileio/parse.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool/runner/
--rw-rw-rw-   0        0        0      108 2022-08-17 08:07:34.000000 pipetool-0.0.8/pipetool/runner/__init__.py
--rw-rw-rw-   0        0        0      724 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/runner/builder.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool/runner/hooks/
--rw-rw-rw-   0        0        0      116 2022-08-16 23:33:29.000000 pipetool-0.0.8/pipetool/runner/hooks/__init__.py
--rw-rw-rw-   0        0        0      313 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/runner/hooks/closure.py
--rw-rw-rw-   0        0        0     2745 2022-07-28 01:53:46.000000 pipetool-0.0.8/pipetool/runner/hooks/hook.py
--rw-rw-rw-   0        0        0      446 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/runner/hooks/iter_timer.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool/runner/hooks/logger/
--rw-rw-rw-   0        0        0      111 2022-08-17 03:33:02.000000 pipetool-0.0.8/pipetool/runner/hooks/logger/__init__.py
--rw-rw-rw-   0        0        0     5707 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/runner/hooks/logger/base.py
--rw-rw-rw-   0        0        0      847 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/runner/hooks/sampler_seed.py
--rw-rw-rw-   0        0        0     3269 2022-08-17 08:04:30.000000 pipetool-0.0.8/pipetool/runner/utils.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool/utils/
--rw-rw-rw-   0        0        0     1166 2022-08-17 08:08:36.000000 pipetool-0.0.8/pipetool/utils/__init__.py
--rw-rw-rw-   0        0        0    28031 2022-07-25 21:12:14.000000 pipetool-0.0.8/pipetool/utils/config.py
--rw-rw-rw-   0        0        0    11487 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/utils/misc.py
--rw-rw-rw-   0        0        0     3415 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/utils/path.py
--rw-rw-rw-   0        0        0     7105 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/utils/progressbar.py
--rw-rw-rw-   0        0        0    12311 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/utils/registry.py
--rw-rw-rw-   0        0        0     4290 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/utils/testing.py
--rw-rw-rw-   0        0        0     3046 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/utils/timer.py
--rw-rw-rw-   0        0        0     2689 2022-07-22 21:26:11.000000 pipetool-0.0.8/pipetool/utils/version_utils.py
--rw-rw-rw-   0        0        0     1176 2022-08-22 07:01:33.000000 pipetool-0.0.8/pipetool/version.py
-drwxrwxrwx   0        0        0        0 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool.egg-info/
--rw-rw-rw-   0        0        0      296 2022-08-22 07:06:56.000000 pipetool-0.0.8/pipetool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2022-08-22 07:06:57.000000 pipetool-0.0.8/pipetool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-22 07:06:56.000000 pipetool-0.0.8/pipetool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2022-08-22 07:06:56.000000 pipetool-0.0.8/pipetool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-08-22 07:06:56.000000 pipetool-0.0.8/pipetool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-22 07:06:57.000000 pipetool-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      877 2022-08-22 07:06:29.000000 pipetool-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/
+-rw-rw-rw-   0        0        0      296 2022-09-16 14:00:56.000000 pipetool-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/doc/
+-rw-rw-rw-   0        0        0        0 2022-06-20 12:54:15.000000 pipetool-0.0.9/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/examples/
+-rw-rw-rw-   0        0        0        0 2022-06-20 12:54:15.000000 pipetool-0.0.9/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/examples/runner/
+-rw-rw-rw-   0        0        0        0 2022-08-22 14:53:59.000000 pipetool-0.0.9/examples/runner/__init__.py
+-rw-rw-rw-   0        0        0      245 2022-08-22 15:06:05.000000 pipetool-0.0.9/examples/runner/test_utils.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool/
+-rw-rw-rw-   0        0        0      117 2022-07-25 21:19:43.000000 pipetool-0.0.9/pipetool/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool/fileio/
+-rw-rw-rw-   0        0        0      530 2022-08-11 00:41:26.000000 pipetool-0.0.9/pipetool/fileio/__init__.py
+-rw-rw-rw-   0        0        0    42422 2022-07-25 08:15:27.000000 pipetool-0.0.9/pipetool/fileio/file_client.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool/fileio/handlers/
+-rw-rw-rw-   0        0        0      382 2022-08-11 00:40:47.000000 pipetool-0.0.9/pipetool/fileio/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1017 2022-07-22 21:27:06.000000 pipetool-0.0.9/pipetool/fileio/handlers/base.py
+-rw-rw-rw-   0        0        0      448 2022-08-11 01:32:27.000000 pipetool-0.0.9/pipetool/fileio/handlers/csv_handler.py
+-rw-rw-rw-   0        0        0     1090 2022-09-16 13:55:56.000000 pipetool-0.0.9/pipetool/fileio/handlers/json_handler.py
+-rw-rw-rw-   0        0        0     1269 2022-09-16 13:58:22.000000 pipetool-0.0.9/pipetool/fileio/handlers/jsons_handler.py
+-rw-rw-rw-   0        0        0      753 2022-09-05 10:03:05.000000 pipetool-0.0.9/pipetool/fileio/handlers/pickle_handler.py
+-rw-rw-rw-   0        0        0      701 2022-07-22 21:26:09.000000 pipetool-0.0.9/pipetool/fileio/handlers/yaml_handler.py
+-rw-rw-rw-   0        0        0     6139 2022-09-05 09:39:20.000000 pipetool-0.0.9/pipetool/fileio/io.py
+-rw-rw-rw-   0        0        0     3993 2022-08-11 01:04:36.000000 pipetool-0.0.9/pipetool/fileio/parse.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool/runner/
+-rw-rw-rw-   0        0        0      109 2022-09-01 01:10:27.000000 pipetool-0.0.9/pipetool/runner/__init__.py
+-rw-rw-rw-   0        0        0      724 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/runner/builder.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool/runner/hooks/
+-rw-rw-rw-   0        0        0      116 2022-08-16 23:33:29.000000 pipetool-0.0.9/pipetool/runner/hooks/__init__.py
+-rw-rw-rw-   0        0        0      313 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/runner/hooks/closure.py
+-rw-rw-rw-   0        0        0     2745 2022-07-28 01:53:46.000000 pipetool-0.0.9/pipetool/runner/hooks/hook.py
+-rw-rw-rw-   0        0        0      446 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/runner/hooks/iter_timer.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool/runner/hooks/logger/
+-rw-rw-rw-   0        0        0      111 2022-08-17 03:33:02.000000 pipetool-0.0.9/pipetool/runner/hooks/logger/__init__.py
+-rw-rw-rw-   0        0        0     5707 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/runner/hooks/logger/base.py
+-rw-rw-rw-   0        0        0      847 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/runner/hooks/sampler_seed.py
+-rw-rw-rw-   0        0        0     3357 2022-09-16 13:40:05.000000 pipetool-0.0.9/pipetool/runner/utils.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool/utils/
+-rw-rw-rw-   0        0        0     1166 2022-08-17 08:08:36.000000 pipetool-0.0.9/pipetool/utils/__init__.py
+-rw-rw-rw-   0        0        0    28031 2022-07-25 21:12:14.000000 pipetool-0.0.9/pipetool/utils/config.py
+-rw-rw-rw-   0        0        0    11487 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/utils/misc.py
+-rw-rw-rw-   0        0        0     3415 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/utils/path.py
+-rw-rw-rw-   0        0        0     7105 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/utils/progressbar.py
+-rw-rw-rw-   0        0        0    12311 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/utils/registry.py
+-rw-rw-rw-   0        0        0     4290 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/utils/testing.py
+-rw-rw-rw-   0        0        0     3046 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/utils/timer.py
+-rw-rw-rw-   0        0        0     2689 2022-07-22 21:26:11.000000 pipetool-0.0.9/pipetool/utils/version_utils.py
+-rw-rw-rw-   0        0        0     1176 2022-08-22 15:00:33.000000 pipetool-0.0.9/pipetool/version.py
+drwxrwxrwx   0        0        0        0 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool.egg-info/
+-rw-rw-rw-   0        0        0      296 2022-09-16 14:00:55.000000 pipetool-0.0.9/pipetool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1252 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-16 14:00:55.000000 pipetool-0.0.9/pipetool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2022-09-16 14:00:56.000000 pipetool-0.0.9/pipetool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-09-16 14:00:56.000000 pipetool-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      877 2022-08-22 07:06:29.000000 pipetool-0.0.9/setup.py
```

### Comparing `pipetool-0.0.8/pipetool/fileio/__init__.py` & `pipetool-0.0.9/pipetool/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/fileio/file_client.py` & `pipetool-0.0.9/pipetool/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/fileio/handlers/base.py` & `pipetool-0.0.9/pipetool/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/fileio/handlers/json_handler.py` & `pipetool-0.0.9/pipetool/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/fileio/handlers/jsons_handler.py` & `pipetool-0.0.9/pipetool/fileio/handlers/jsons_handler.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/fileio/handlers/pickle_handler.py` & `pipetool-0.0.9/pipetool/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/fileio/handlers/yaml_handler.py` & `pipetool-0.0.9/pipetool/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/fileio/io.py` & `pipetool-0.0.9/pipetool/fileio/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from .file_client import FileClient
 from .handlers import BaseFileHandler, JsonHandler,JsonsHandler, PickleHandler, YamlHandler,CsvHandler
 
 FileLikeObject = Union[TextIO, StringIO, BytesIO]
 
 file_handlers = {
     'json': JsonHandler(),
-    'jsons': JsonsHandler(),
+    'jsons': JsonsHandler(), 
+    'jsonl': JsonsHandler(), 
     'yaml': YamlHandler(),
     'yml': YamlHandler(),
     'pickle': PickleHandler(),
     'pkl': PickleHandler(),
     'csv': CsvHandler()
 }
```

### Comparing `pipetool-0.0.8/pipetool/fileio/parse.py` & `pipetool-0.0.9/pipetool/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/runner/builder.py` & `pipetool-0.0.9/pipetool/runner/builder.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/runner/hooks/hook.py` & `pipetool-0.0.9/pipetool/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/runner/hooks/logger/base.py` & `pipetool-0.0.9/pipetool/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/runner/hooks/sampler_seed.py` & `pipetool-0.0.9/pipetool/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/runner/utils.py` & `pipetool-0.0.9/pipetool/runner/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,20 @@
         import torch 
         torch.manual_seed(seed)
         torch.cuda.manual_seed(seed)
         torch.cuda.manual_seed_all(seed)
     except:
         pass
     
+    try:
+        import paddle 
+        paddle.seed(seed)
+    except:
+        pass
+    
     return seed
 
 def seg_generator(iterables, seg_len, seg_backoff=0):
     '''
     滑窗实现
     '''
     if seg_len <= 0:
```

### Comparing `pipetool-0.0.8/pipetool/utils/__init__.py` & `pipetool-0.0.9/pipetool/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/utils/config.py` & `pipetool-0.0.9/pipetool/utils/config.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/utils/misc.py` & `pipetool-0.0.9/pipetool/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/utils/path.py` & `pipetool-0.0.9/pipetool/utils/path.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/utils/progressbar.py` & `pipetool-0.0.9/pipetool/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/utils/registry.py` & `pipetool-0.0.9/pipetool/utils/registry.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/utils/testing.py` & `pipetool-0.0.9/pipetool/utils/testing.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/utils/timer.py` & `pipetool-0.0.9/pipetool/utils/timer.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/utils/version_utils.py` & `pipetool-0.0.9/pipetool/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `pipetool-0.0.8/pipetool/version.py` & `pipetool-0.0.9/pipetool/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `pipetool-0.0.8/pipetool.egg-info/SOURCES.txt` & `pipetool-0.0.9/pipetool.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 setup.py
 doc/__init__.py
 examples/__init__.py
+examples/runner/__init__.py
+examples/runner/test_utils.py
 pipetool/__init__.py
 pipetool/version.py
 pipetool.egg-info/PKG-INFO
 pipetool.egg-info/SOURCES.txt
 pipetool.egg-info/dependency_links.txt
 pipetool.egg-info/requires.txt
 pipetool.egg-info/top_level.txt
```

### Comparing `pipetool-0.0.8/setup.py` & `pipetool-0.0.9/setup.py`

 * *Files identical despite different names*

