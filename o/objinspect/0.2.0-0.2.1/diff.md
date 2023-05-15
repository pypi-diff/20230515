# Comparing `tmp/objinspect-0.2.0.tar.gz` & `tmp/objinspect-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objinspect-0.2.0.tar", last modified: Fri Mar 10 19:53:33 2023, max compression
+gzip compressed data, was "objinspect-0.2.1.tar", last modified: Mon May 15 19:56:34 2023, max compression
```

## Comparing `objinspect-0.2.0.tar` & `objinspect-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:53:33.150156 objinspect-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-10 19:53:22.000000 objinspect-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-10 19:53:33.150156 objinspect-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-10 19:53:22.000000 objinspect-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:53:33.150156 objinspect-0.2.0/objinspect/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-10 19:53:22.000000 objinspect-0.2.0/objinspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-03-10 19:53:22.000000 objinspect-0.2.0/objinspect/_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-10 19:53:22.000000 objinspect-0.2.0/objinspect/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-03-10 19:53:22.000000 objinspect-0.2.0/objinspect/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-10 19:53:22.000000 objinspect-0.2.0/objinspect/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-10 19:53:22.000000 objinspect-0.2.0/objinspect/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-10 19:53:22.000000 objinspect-0.2.0/objinspect/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:53:33.150156 objinspect-0.2.0/objinspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-10 19:53:33.000000 objinspect-0.2.0/objinspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-10 19:53:33.000000 objinspect-0.2.0/objinspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 19:53:33.000000 objinspect-0.2.0/objinspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-10 19:53:33.000000 objinspect-0.2.0/objinspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-10 19:53:33.000000 objinspect-0.2.0/objinspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 19:53:33.150156 objinspect-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-10 19:53:22.000000 objinspect-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:56:34.199545 objinspect-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 19:56:23.000000 objinspect-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-15 19:56:34.199545 objinspect-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-15 19:56:23.000000 objinspect-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:56:34.199545 objinspect-0.2.1/objinspect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-15 19:56:23.000000 objinspect-0.2.1/objinspect/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:56:34.199545 objinspect-0.2.1/objinspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 19:56:34.000000 objinspect-0.2.1/objinspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-15 19:56:23.000000 objinspect-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:56:34.199545 objinspect-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:56:23.000000 objinspect-0.2.1/setup.py
```

### Comparing `objinspect-0.2.0/LICENSE` & `objinspect-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `objinspect-0.2.0/PKG-INFO` & `objinspect-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,9 @@
-Metadata-Version: 2.1
-Name: objinspect
-Version: 0.2.0
-Summary: View the structure of Python classes and functions 
-Home-page: https://github.com/zigai/obj-inspect
-Author: Žiga Ivanšek
-Author-email: ziga.ivansek@gmail.com
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # objinspect
+[![Tests](https://github.com/zigai/obj-inspect/actions/workflows/tests.yml/badge.svg)](https://github.com/zigai/obj-inspect/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/objinspect.svg)](https://badge.fury.io/py/objinspect)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
 [![Downloads](https://static.pepy.tech/badge/objinspect)](https://pepy.tech/project/objinspect)
 [![license](https://img.shields.io/github/license/zigai/objinspect.svg)](https://github.com/zigai/objinspect/blob/main/LICENSE)
 
 View the structure of Python classes and functions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `objinspect-0.2.0/objinspect/__init__.py` & `objinspect-0.2.1/objinspect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import inspect
 
 from objinspect import constants, util
 from objinspect._class import Class
 from objinspect.function import Function
-from objinspect.method import Method
-from objinspect.method_extractor import MethodExtractor
+from objinspect.method import Method, MethodFilter
 from objinspect.parameter import Parameter
 
 
 def objinspect(
     obj,
     init=True,
     public=True,
```

### Comparing `objinspect-0.2.0/objinspect/_class.py` & `objinspect-0.2.1/objinspect/_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import functools
 import inspect
-from collections import OrderedDict
 from typing import Any
 
 import docstring_parser
 
 from objinspect.function import _get_docstr_desc, _has_docstr
 from objinspect.method import Method, MethodFilter
 
@@ -62,15 +61,15 @@
             "static_methods": static_methods,
             "protected": protected,
             "private": private,
         }
         self._methods = self._find_methods()
         self.has_init = "__init__" in self._methods
         self._parsed_docstring = (
-            docstring_parser.parse(self.docstring) if self.has_docstring else None
+            docstring_parser.parse(self.docstring) if self.has_docstring else None  # type: ignore
         )
         self.description = _get_docstr_desc(self._parsed_docstring)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name='{self.name}', methods={len(self._methods)}, has_init={self.has_init}, description={self.description})"
 
     @functools.cached_property
@@ -78,15 +77,15 @@
         if self.is_initialized:
             return self.cls.__class__
         return self.cls
 
     def _find_methods(self):
         method_filter = MethodFilter(**self.extractor_kwargs)
         members = inspect.getmembers(self.cls, inspect.isfunction)
-        methods = OrderedDict()
+        methods = {}
         for i in method_filter.extract([Method(i[1], self._get_class_base) for i in members]):
             methods[i.name] = i
         return methods
 
     def init(self, *args, **kwargs) -> None:
         """
         Initializes the class as an instance using the provided arguments.
```

### Comparing `objinspect-0.2.0/objinspect/function.py` & `objinspect-0.2.1/objinspect/function.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-from collections import OrderedDict
 from typing import Any, Callable
 
 import docstring_parser
 from docstring_parser import Docstring
 
 from objinspect.parameter import Parameter
 
@@ -30,16 +29,14 @@
     A Function object represents a function and its attributes.
 
     Args:
         func (Callable): The function to be inspected.
         skip_self (bool, optional): Whether to skip the self parameter. Defaults to True.
 
     Attributes:
-        func (Callable): The function to be inspected.
-        skip_self (bool): Whether to skip the self parameter.
         name (str): The name of the function.
         docstring (str): The docstring of the function.
         has_docstring (bool): Whether the function has a docstring.
         description (str): The description part of the function's docstring.
         params (list[Parameter]): A list of parameters of the function.
         dict (dict): A dictionary representation of the function's attributes.
 
@@ -48,35 +45,35 @@
     def __init__(self, func: Callable, skip_self: bool = True) -> None:
         self.func = func
         self.skip_self = skip_self
         self.name: str = self.func.__name__
         self.docstring = inspect.getdoc(self.func)
         self.has_docstring = _has_docstr(self.docstring)
         self._parsed_docstr: Docstring | None = (
-            docstring_parser.parse(self.docstring) if self.has_docstring else None
+            docstring_parser.parse(self.docstring) if self.has_docstring else None  # type: ignore
         )
         self._parameters = self._find_parameters()
         self.description = _get_docstr_desc(self._parsed_docstr)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name='{self.name}', parameters={len(self._parameters)}, description='{self.description}')"
 
-    def _find_parameters(self) -> OrderedDict[str, Parameter]:
+    def _find_parameters(self) -> dict[str, Parameter]:
         args = inspect.signature(self.func)
         params = [Parameter.from_inspect_param(i) for i in args.parameters.values()]
 
         # Try finding descriptions for parameters
         if self._parsed_docstr is not None:
             params_mapping = {par.arg_name: par for par in self._parsed_docstr.params}
             for param in params:
                 if parameter := params_mapping.get(param.name, False):
-                    if parameter.description:
-                        param.description = parameter.description
+                    if parameter.description:  # type: ignore
+                        param.description = parameter.description  # type: ignore
 
-        parameters = OrderedDict()
+        parameters = {}
         for param in params:
             if param.name == "self" and self.skip_self:
                 continue
             parameters[param.name] = param
         return parameters
 
     def get_param(self, arg: str | int) -> Parameter:
```

### Comparing `objinspect-0.2.0/objinspect/method.py` & `objinspect-0.2.1/objinspect/method.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 import inspect
-import types
 
 from objinspect.function import Function
 
 
 class Method(Function):
-    def __init__(self, func, cls, skip_self: bool = True):
-        super().__init__(func, skip_self)
+    """
+    The Method class represents a method of a class.
+
+    Args:
+        method (Callable): The method to be inspected.
+        cls (type): The class to which the method belongs.
+        skip_self (bool, optional): Whether to skip the self parameter. Defaults to True.
+
+    Attributes:
+        name (str): The name of the method.
+        docstring (str): The docstring of the method.
+        has_docstring (bool): Whether the method has a docstring.
+        description (str): The description part of the method's docstring.
+        params (list[Parameter]): A list of parameters of the method.
+        dict (dict): A dictionary representation of the method's attributes.
+        is_static (bool): Whether the method is static.
+        is_classmethod (bool): Whether the method is a classmethod.
+        is_property (bool): Whether the method is a property.
+        is_private (bool): Whether the method is private.
+        is_protected (bool): Whether the method is protected.
+        is_public (bool): Whether the method is public.
+        is_inherited (bool): Whether the method is inherited.
+
+    """
+
+    def __init__(self, method, cls, skip_self: bool = True):
+        super().__init__(method, skip_self)
         self.cls = cls
 
     @property
     def is_static(self) -> bool:
         for cls in inspect.getmro(self.cls):
             if inspect.isroutine(self.func):
                 if self.name in cls.__dict__:
@@ -36,15 +60,15 @@
 
     @property
     def is_public(self) -> bool:
         return not self.is_private and not self.is_protected
 
     @property
     def is_inherited(self) -> bool:
-        return not self.name in self.cls.__dict__
+        return self.name not in self.cls.__dict__
 
 
 class MethodFilter:
     def __init__(
         self,
         init=True,
         public=True,
```

### Comparing `objinspect-0.2.0/objinspect/parameter.py` & `objinspect-0.2.1/objinspect/parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,28 +31,26 @@
             description (str | None): The description of the parameter.
         """
         self.name = name
         self.type = type
         self.default = default
         self.description = description
         self.kind = kind
-        if infer_type:
-            self._infer_type()
+        if infer_type and not self.is_typed:
+            self.type = self._get_infered_type()
 
     def __repr__(self):
         data = f"name='{self.name}', kind={str(self.kind)}, type={self.type}, default={self.default}, description='{self.description}'"
         return f"{self.__class__.__name__}({data})"
 
-    def _infer_type(self):
+    def _get_infered_type(self):
         """Infer the type of the parameter based on its default value."""
-        if self.is_typed or self.is_required:
-            return
-        if self.default is None:
-            return
-        self.type = type(self.default)
+        if self.default is EMPTY:
+            return EMPTY
+        return type(self.default)
 
     @property
     def is_typed(self) -> bool:
         return self.type != EMPTY
 
     @property
     def is_required(self) -> bool:
```

