# Comparing `tmp/confik-1.0.6.tar.gz` & `tmp/confik-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confik-1.0.6.tar", last modified: Mon May 15 05:59:04 2023, max compression
+gzip compressed data, was "confik-1.0.7.tar", last modified: Mon May 15 06:28:13 2023, max compression
```

## Comparing `confik-1.0.6.tar` & `confik-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 05:59:04.784889 confik-1.0.6/
--rw-r--r--   0 leondaz    (501) staff       (20)     1069 2023-05-13 06:57:00.000000 confik-1.0.6/LICENSE
--rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-15 05:59:04.784756 confik-1.0.6/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)     1089 2023-05-13 07:02:08.000000 confik-1.0.6/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 05:59:04.783519 confik-1.0.6/confik/
--rw-r--r--   0 leondaz    (501) staff       (20)     1037 2023-05-13 06:59:23.000000 confik-1.0.6/confik/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.6/confik/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2434 2023-05-15 05:57:52.000000 confik-1.0.6/confik/parsers.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1268 2023-05-13 04:46:31.000000 confik-1.0.6/confik/proxies.py
--rw-r--r--   0 leondaz    (501) staff       (20)      619 2023-05-13 04:49:37.000000 confik-1.0.6/confik/utils.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 05:59:04.784056 confik-1.0.6/confik.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-15 05:59:04.000000 confik-1.0.6/confik.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      327 2023-05-15 05:59:04.000000 confik-1.0.6/confik.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-15 05:59:04.000000 confik-1.0.6/confik.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-15 05:59:04.000000 confik-1.0.6/confik.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-15 05:59:04.784927 confik-1.0.6/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-15 05:58:25.000000 confik-1.0.6/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 05:59:04.784500 confik-1.0.6/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-13 05:42:01.000000 confik-1.0.6/tests/test_confik_parser.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2924 2023-05-15 05:57:52.000000 confik-1.0.6/tests/test_read_environment_variables.py
--rw-r--r--   0 leondaz    (501) staff       (20)      149 2023-05-13 04:27:37.000000 confik-1.0.6/tests/test_utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 06:28:13.223383 confik-1.0.7/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1069 2023-05-13 06:57:00.000000 confik-1.0.7/LICENSE
+-rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-15 06:28:13.223272 confik-1.0.7/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     1986 2023-05-15 06:27:44.000000 confik-1.0.7/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 06:28:13.221782 confik-1.0.7/confik/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1090 2023-05-15 06:27:44.000000 confik-1.0.7/confik/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.7/confik/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2413 2023-05-15 06:27:35.000000 confik-1.0.7/confik/parsers.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1330 2023-05-15 06:17:35.000000 confik-1.0.7/confik/proxies.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      619 2023-05-13 04:49:37.000000 confik-1.0.7/confik/utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 06:28:13.222315 confik-1.0.7/confik.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-15 06:28:13.000000 confik-1.0.7/confik.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      327 2023-05-15 06:28:13.000000 confik-1.0.7/confik.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-15 06:28:13.000000 confik-1.0.7/confik.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-15 06:28:13.000000 confik-1.0.7/confik.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-15 06:28:13.223416 confik-1.0.7/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-15 06:28:00.000000 confik-1.0.7/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 06:28:13.222890 confik-1.0.7/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-13 05:42:01.000000 confik-1.0.7/tests/test_confik_parser.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2924 2023-05-15 05:57:52.000000 confik-1.0.7/tests/test_read_environment_variables.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      149 2023-05-13 04:27:37.000000 confik-1.0.7/tests/test_utils.py
```

### Comparing `confik-1.0.6/LICENSE` & `confik-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `confik-1.0.6/confik/__init__.py` & `confik-1.0.7/confik/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 from typing import Union
 
 from .exceptions import ConfikError
 from .parsers import ConfikParser
+from .proxies import MapConfigToMappingProxy
 from .utils import boolean, csv
 
-confik = ConfikParser()
+confik = ConfikParser(path=".")
 
 
 def get(
     key,
     default=None,
     cast=None,
     default_factory=None,
```

### Comparing `confik-1.0.6/confik/parsers.py` & `confik-1.0.7/confik/parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from confik.proxies import EnvMappingProxy
 from confik.utils import boolean
 
 
 class ConfikParser:
     proxy_class = EnvMappingProxy
 
-    def __init__(self, path=".", *args, **kwargs):
-        self.source = self.proxy_class(*args, path=path, **kwargs)
+    def __init__(self, *args, **kwargs):
+        self.source = self.proxy_class(*args, **kwargs)
 
     def validate_params(
         self,
         key,
         cast,
         default,
         default_factory,
```

### Comparing `confik-1.0.6/confik/proxies.py` & `confik-1.0.7/confik/proxies.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import contextlib
 import os
 from pathlib import Path
+from typing import Union
 
 
 class MapConfigToMappingProxy:
     def get_mapping(self, path):
         """
         Should return a mapping from the path given
         :param path: str
@@ -22,19 +23,19 @@
                 for line in f.readlines():
                     entry = line.strip().split("=", 1)
 
                     if len(entry) == 1:
                         entry.append("")
 
                     name, value = entry
-                    mapping[name] = value.replace('"', "")
+                    mapping[name] = value.replace('"', "").replace("'", "")
 
         return mapping
 
-    def __init__(self, path=Path("."), *args, **kwargs):
+    def __init__(self, path: Union[Path, str] = Path("."), *args, **kwargs):
         assert isinstance(path, (str, Path)), "unsupported path type {t}".format(
             t=type(path)
         )
 
         if isinstance(path, str):
             path = Path(path)
```

### Comparing `confik-1.0.6/confik/utils.py` & `confik-1.0.7/confik/utils.py`

 * *Files identical despite different names*

### Comparing `confik-1.0.6/tests/test_read_environment_variables.py` & `confik-1.0.7/tests/test_read_environment_variables.py`

 * *Files identical despite different names*

