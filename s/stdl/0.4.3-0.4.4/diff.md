# Comparing `tmp/stdl-0.4.3.tar.gz` & `tmp/stdl-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdl-0.4.3.tar", last modified: Tue May  9 18:36:48 2023, max compression
+gzip compressed data, was "stdl-0.4.4.tar", last modified: Mon May 15 18:47:43 2023, max compression
```

## Comparing `stdl-0.4.3.tar` & `stdl-0.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:36:48.996237 stdl-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 18:36:35.000000 stdl-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-09 18:36:48.996237 stdl-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-09 18:36:35.000000 stdl-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-09 18:36:35.000000 stdl-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:36:48.996237 stdl-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:36:35.000000 stdl-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:36:48.992237 stdl-0.4.3/stdl/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/lst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/str_u.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:36:48.996237 stdl-0.4.3/stdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:47:43.444609 stdl-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 18:47:32.000000 stdl-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 18:47:43.444609 stdl-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-15 18:47:32.000000 stdl-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-15 18:47:32.000000 stdl-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:47:43.444609 stdl-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:47:32.000000 stdl-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:47:43.440609 stdl-0.4.4/stdl/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27845 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/lst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/str_u.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:47:43.444609 stdl-0.4.4/stdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/top_level.txt
```

### Comparing `stdl-0.4.3/LICENSE` & `stdl-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stdl-0.4.3/PKG-INFO` & `stdl-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: stdl
-Version: 0.4.3
+Version: 0.4.4
 Summary: Extended Python Standard Library
 Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
-Project-URL: repository, https://github.com/zigai/stdl
-Project-URL: homepage, https://github.com/zigai/stdl
+Project-URL: Repository, https://github.com/zigai/stdl
 Keywords: python utilites,filesystem,string manipulation,logging configuration,list utils,standard library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,14 +15,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # stdl
+[![Tests](https://github.com/zigai/stdl/actions/workflows/tests.yml/badge.svg)](https://github.com/zigai/stdl/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/stdl.svg)](https://badge.fury.io/py/stdl)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
 [![Downloads](https://static.pepy.tech/badge/stdl)](https://pepy.tech/project/stdl)
 [![license](https://img.shields.io/github/license/zigai/stdl.svg)](https://github.com/zigai/stdl/blob/main/LICENSE)
 
 Extended Python standard library.
 # Installation
```

### Comparing `stdl-0.4.3/README.md` & `stdl-0.4.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # stdl
+[![Tests](https://github.com/zigai/stdl/actions/workflows/tests.yml/badge.svg)](https://github.com/zigai/stdl/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/stdl.svg)](https://badge.fury.io/py/stdl)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
 [![Downloads](https://static.pepy.tech/badge/stdl)](https://pepy.tech/project/stdl)
 [![license](https://img.shields.io/github/license/zigai/stdl.svg)](https://github.com/zigai/stdl/blob/main/LICENSE)
 
 Extended Python standard library.
 # Installation
```

### Comparing `stdl-0.4.3/pyproject.toml` & `stdl-0.4.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stdl"
-version = "0.4.3"
+version = "0.4.4"
 description = "Extended Python Standard Library"
 authors = [{ name = "Žiga Ivanšek", email = "ziga.ivansek@gmail.com" }]
 license = { file = "LICENSE.txt" }
 readme = "README.md"
 requires-python = ">=3.10"
 
 classifiers = [
@@ -33,24 +33,23 @@
 dependencies = ["PyYAML>=6.0", "tqdm", "python-dateutil==2.8.2"]
 
 [project.optional-dependencies]
 test = ["pytest"]
 dev = ["black", "pytest", "flake8"]
 
 [project.urls]
-repository = "https://github.com/zigai/stdl"
-homepage = "https://github.com/zigai/stdl"
+Repository = "https://github.com/zigai/stdl"
 
 [tool.black]
 line-length = 100
 target_version = ['py310']
 
 [tool.ruff]
 line-length = 100
-extend-ignore = ["E731", "E741", "N802", "N803", "N806","E501"]
+extend-ignore = ["E731", "E741", "N802", "N803", "N806", "E501"]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".hg",
     ".mypy_cache",
@@ -69,8 +68,7 @@
     "node_modules",
     "venv",
     "tests",
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "E402"]
-
```

### Comparing `stdl-0.4.3/stdl/dataclass.py` & `stdl-0.4.4/stdl/dataclass.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+import json
+from copy import deepcopy
 from dataclasses import asdict, astuple, dataclass
 from pprint import pprint
 from typing import Any, Mapping
 
-from stdl.fs import Pathlike, json_dump
+from stdl.fs import Pathlike, json_load
 
 
 class Data:
     def __init__(self) -> None:
         pass
 
-    @property
+    def __getitem__(self, key):
+        return self.dict()[key]
+
+    def __iter__(self):
+        for i in self.tuple():
+            yield i
+
     def dict(self) -> dict:
         return asdict(self)  # type:ignore
 
-    @property
     def tuple(self) -> tuple:
         return astuple(self)  # type:ignore
 
-    def print(self):
-        pprint(self.dict)
-
-    def __getitem__(self, key):
-        return self.dict[key]
+    def json(self):
+        return json.dumps(self.dict())
 
-    def __iter__(self):
-        for i in self.tuple:
-            yield i
+    def copy(self):
+        return deepcopy(self)
 
     @classmethod
-    def from_dict(cls, d: Mapping[str, Any]):
-        return cls(**d)
+    def parse_obj(cls, obj: Mapping[str, Any]):
+        return cls(**obj)
 
-    def json_dump(self, filepath: Pathlike, endcoding="utf-8", indent=4):
-        json_dump(self.dict, filepath, endcoding, indent=indent)
+    def parse_file(self, filepath: Pathlike):
+        return self.parse_obj(json_load(filepath))  # type:ignore
+
+    def print(self):
+        pprint(self.dict)
 
 
 __all__ = ["Data", "dataclass"]
```

### Comparing `stdl-0.4.3/stdl/dt.py` & `stdl-0.4.4/stdl/dt.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.3/stdl/fs.py` & `stdl-0.4.4/stdl/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,35 +198,32 @@
         Append data to a file.
 
         Args:
             data (Any): The data to append.
             newline (bool, optional): Whether to add a newline at the end of the data. Defaults to True.
         """
         self.__write(data, "a", newline=newline)
-        return self
 
     def write_iter(self, data: Iterable, sep="\n"):
         """Write data from an iterable to a file, overwriting any existing data.
 
         Args:
             data (Iterable): The data to write.
             sep (str, optional): The separator to use between items. Defaults to "\\n".
         """
         self.__write_iter(data, "w", sep=sep)
-        return self
 
     def append_iter(self, data: Iterable, sep="\n"):
         """Append data from an iterable to a file.
 
         Args:
             data (Iterable): The data to append.
             sep (str, optional): The separator to use between items. Defaults to "\\n".
         """
         self.__write_iter(data, "a", sep=sep)
-        return self
 
     def readlines(self) -> list[str]:
         """Equivalent to TextIOWrapper.readlines()"""
         with open(self.path, "r", encoding=self.encoding) as f:
             return f.readlines()
 
     def splitlines(self) -> list[str]:
```

### Comparing `stdl-0.4.3/stdl/log.py` & `stdl-0.4.4/stdl/log.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,81 @@
 from os import get_terminal_size
 from typing import Callable
 
+from stdl.str_u import colored
+
 
 def color_tag(text: str, c: str):
     return f"<{c}>{text}</{c}>"
 
 
 class LoguruFormatter:
-    time = color_tag("{time:YYYY-MM-DD HH:mm:ss.SSS}", "light-black")
+    time = color_tag("{time:YYYY-MM-DD HH:mm:ss}", "green")
     level = color_tag("{level: <8}", "level")
     msg = color_tag("{message:<24}", "level")
     name = color_tag("{name}", "light-blue")
     func = color_tag("{function}", "light-blue")
     lineno = color_tag("{line}", "light-blue")
+    extra_key_skips = ["title"]
+    extra_key_name_color = "white"
 
     def format(self, record: dict) -> str:
         """
-        Example:
+        Example usage:
         >>> import sys
         >>> from loguru import logger
+        >>> logger.remove()
         >>> logger.add(sys.stdout, level="DEBUG", format=loguru_formater)
         """
         extras = ""
         if len(record["extra"]):
             for key in record["extra"].keys():
-                extras = extras + key + "=" + "{extra[" + key + "]}, "
+                if key in self.extra_key_skips:
+                    continue
+                extras = (
+                    extras
+                    + colored(key, self.extra_key_name_color)
+                    + "="
+                    + "{extra["
+                    + key
+                    + "]}, "
+                )
             extras = extras[:-2]
-        fmt = f"{self.time} [ {self.level} ] {self.name}:{self.func}:{self.lineno} - {self.msg} {extras}\n"
-        return fmt
+
+        if title := record["extra"].get("title"):
+            return f"{self.time} | {self.level} | [ {title} ] {self.name}:{self.func}:{self.lineno} - {self.msg} {extras}\n"
+        return f"{self.time} | {self.level} | {self.name}:{self.func}:{self.lineno} - {self.msg} {extras}\n"
 
 
 loguru_formater = LoguruFormatter().format
 
 
 def get_logging_config(
     format: str | None = None,
     level: str = "INFO",
     filename: str | None = None,
     backup_count: int = 0,
     disable_existing: bool = False,
     console_handler: str = "logging.StreamHandler",
     file_handler: str = "logging.handlers.TimedRotatingFileHandler",
-    style: str = "{",
+    format_style: str = "{",
 ):
     format = (
-        format or "{asctime} [{levelname:<8s}] [{module}.{funcName}:{lineno}] {name} - {message}"
+        format
+        or "{asctime} | {levelname:<8s} | [ {name} ] {module}.{funcName}:{lineno} - {message}"
     )
 
     config = {
         "version": 1,
         "disable_existing_loggers": disable_existing,
         "formatters": {
             "standard": {
                 "format": format,
                 "datefmt": "%Y-%m-%d %H:%M:%S",
-                "style": style,
+                "style": format_style,
             }
         },
         "handlers": {
             "console": {
                 "class": console_handler,
                 "level": level,
                 "formatter": "standard",
```

### Comparing `stdl-0.4.3/stdl/lst.py` & `stdl-0.4.4/stdl/lst.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.3/stdl/net.py` & `stdl-0.4.4/stdl/net.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.3/stdl/str_u.py` & `stdl-0.4.4/stdl/str_u.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.3/stdl.egg-info/PKG-INFO` & `stdl-0.4.4/stdl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: stdl
-Version: 0.4.3
+Version: 0.4.4
 Summary: Extended Python Standard Library
 Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
-Project-URL: repository, https://github.com/zigai/stdl
-Project-URL: homepage, https://github.com/zigai/stdl
+Project-URL: Repository, https://github.com/zigai/stdl
 Keywords: python utilites,filesystem,string manipulation,logging configuration,list utils,standard library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,14 +15,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # stdl
+[![Tests](https://github.com/zigai/stdl/actions/workflows/tests.yml/badge.svg)](https://github.com/zigai/stdl/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/stdl.svg)](https://badge.fury.io/py/stdl)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
 [![Downloads](https://static.pepy.tech/badge/stdl)](https://pepy.tech/project/stdl)
 [![license](https://img.shields.io/github/license/zigai/stdl.svg)](https://github.com/zigai/stdl/blob/main/LICENSE)
 
 Extended Python standard library.
 # Installation
```

