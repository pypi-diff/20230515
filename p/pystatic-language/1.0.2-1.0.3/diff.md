# Comparing `tmp/pystatic-language-1.0.2.tar.gz` & `tmp/pystatic-language-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystatic-language-1.0.2.tar", last modified: Sat May 13 16:48:25 2023, max compression
+gzip compressed data, was "pystatic-language-1.0.3.tar", last modified: Mon May 15 13:24:56 2023, max compression
```

## Comparing `pystatic-language-1.0.2.tar` & `pystatic-language-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 16:48:25.773500 pystatic-language-1.0.2/
--rw-rw-rw-   0        0        0      115 2023-05-13 16:48:25.000000 pystatic-language-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8940 2023-05-13 16:48:25.772498 pystatic-language-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7852 2023-03-16 09:20:24.000000 pystatic-language-1.0.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.0.2/build.py
--rw-rw-rw-   0        0        0      925 2023-05-13 16:48:25.000000 pystatic-language-1.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-13 16:48:25.755984 pystatic-language-1.0.2/pystatic/
--rw-rw-rw-   0        0        0     4714 2023-03-10 17:43:12.000000 pystatic-language-1.0.2/pystatic/base.py
--rw-rw-rw-   0        0        0     8401 2023-03-20 21:44:09.000000 pystatic-language-1.0.2/pystatic/casting.py
--rw-rw-rw-   0        0        0     1315 2023-03-10 17:42:36.000000 pystatic-language-1.0.2/pystatic/clean.py
--rw-rw-rw-   0        0        0      489 2023-03-16 09:08:51.000000 pystatic-language-1.0.2/pystatic/document.py
--rw-rw-rw-   0        0        0     5828 2023-05-13 16:46:00.000000 pystatic-language-1.0.2/pystatic/overload.py
--rw-rw-rw-   0        0        0     5879 2023-05-13 08:43:44.000000 pystatic-language-1.0.2/pystatic/private.py
--rw-rw-rw-   0        0        0     8144 2023-05-13 08:43:44.000000 pystatic-language-1.0.2/pystatic/types.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:48:25.771494 pystatic-language-1.0.2/pystatic_language.egg-info/
--rw-rw-rw-   0        0        0     8940 2023-05-13 16:48:25.000000 pystatic-language-1.0.2/pystatic_language.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-13 16:48:25.000000 pystatic-language-1.0.2/pystatic_language.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 16:48:25.000000 pystatic-language-1.0.2/pystatic_language.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-13 16:48:25.000000 pystatic-language-1.0.2/pystatic_language.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 16:48:25.000000 pystatic-language-1.0.2/pystatic_language.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.0.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 16:48:25.773500 pystatic-language-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1952 2023-05-13 16:48:08.000000 pystatic-language-1.0.2/setup.py
--rw-rw-rw-   0        0        0     3093 2023-05-13 16:47:31.000000 pystatic-language-1.0.2/test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:24:56.593951 pystatic-language-1.0.3/
+-rw-rw-rw-   0        0        0      115 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8940 2023-05-15 13:24:56.592383 pystatic-language-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7852 2023-03-16 09:20:24.000000 pystatic-language-1.0.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.0.3/build.py
+-rw-rw-rw-   0        0        0      925 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-15 13:24:56.575945 pystatic-language-1.0.3/pystatic/
+-rw-rw-rw-   0        0        0     4714 2023-03-10 17:43:12.000000 pystatic-language-1.0.3/pystatic/base.py
+-rw-rw-rw-   0        0        0     8345 2023-05-15 12:59:03.000000 pystatic-language-1.0.3/pystatic/casting.py
+-rw-rw-rw-   0        0        0     1408 2023-05-15 13:02:42.000000 pystatic-language-1.0.3/pystatic/clean.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 09:08:51.000000 pystatic-language-1.0.3/pystatic/document.py
+-rw-rw-rw-   0        0        0     5726 2023-05-15 13:12:38.000000 pystatic-language-1.0.3/pystatic/overload.py
+-rw-rw-rw-   0        0        0     5831 2023-05-15 13:16:21.000000 pystatic-language-1.0.3/pystatic/private.py
+-rw-rw-rw-   0        0        0     8050 2023-05-15 13:18:50.000000 pystatic-language-1.0.3/pystatic/types.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:24:56.592383 pystatic-language-1.0.3/pystatic_language.egg-info/
+-rw-rw-rw-   0        0        0     8940 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.0.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 13:24:56.593951 pystatic-language-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-05-15 13:24:49.000000 pystatic-language-1.0.3/setup.py
+-rw-rw-rw-   0        0        0     3093 2023-05-13 16:47:31.000000 pystatic-language-1.0.3/test.py
```

### Comparing `pystatic-language-1.0.2/PKG-INFO` & `pystatic-language-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystatic-language
-Version: 1.0.2
+Version: 1.0.3
 Summary: This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and.
 Home-page: https://github.com/Shahaf-F-S/pystatic
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystatic-language-1.0.2/README.md` & `pystatic-language-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.2/build.py` & `pystatic-language-1.0.3/build.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.2/pyproject.toml` & `pystatic-language-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pystatic-language'
-version = '1.0.2'
+version = '1.0.3'
 description = "This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and."
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pystatic-language-1.0.2/pystatic/base.py` & `pystatic-language-1.0.3/pystatic/base.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.2/pystatic/casting.py` & `pystatic-language-1.0.3/pystatic/casting.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         ARGS = "args"
         KWARGS = "kwargs"
         SELF = "self"
         INITIALIZERS = "initializers"
         INIT = "__saved_init__"
     # end Keys
 
-    def __new__(cls, model: Type):
+    def __new__(cls, model: Type) -> Type:
         """
         Defines the class attributes.
 
         :param model: The model to wrap.
         """
 
         model.__init__ = Configuration.construct(model.__init__)
@@ -72,30 +72,29 @@
             parameters = {
                 **dict(signature.bind(*args, **kwargs).arguments)
             }
 
             if Configuration.Keys.ARGS in parameters:
                 parameters[Configuration.Keys.ARGS] = (
                     parameters[Configuration.Keys.ARGS][1:]
-                    if len(parameters[Configuration.Keys.ARGS]) > 0 else tuple()
+                    if len(parameters[Configuration.Keys.ARGS]) > 0 else ()
                 )
             # end if
 
             parameters.pop(Configuration.Keys.SELF, None)
 
             initializers = OrderedDict(signature.parameters)
 
             for key in signature.parameters:
                 if key not in parameters:
                     initializers[key] = None
 
                     continue
 
                 else:
-                    # noinspection PyUnresolvedReferences
                     initializers[key] = parameters[key]
                 # end if
             # end ofr
 
             initializers.pop(Configuration.Keys.SELF, None)
 
             parameters = {
```

### Comparing `pystatic-language-1.0.2/pystatic/clean.py` & `pystatic-language-1.0.3/pystatic/clean.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,29 +27,33 @@
             )
         ]
 
     elif not isinstance(properties, list):
         properties = list(properties)
     # end if
 
-    definitions = [
-        "__name__",
-        "__doc__",
-        "__package__",
-        "__loader__",
-        "__spec__",
-        "__all__",
-        "__file__",
-        "__cached__",
-        "__builtins__",
-        "__annotations__"
-    ]
+    properties.extend(
+        [
+            "__name__",
+            "__doc__",
+            "__package__",
+            "__loader__",
+            "__spec__",
+            "__all__",
+            "__file__",
+            "__cached__",
+            "__builtins__",
+            "__annotations__"
+        ]
+    )
+
+    properties = list(set(properties))
 
     for key in sys.modules[name].__dict__.copy():
         if (
-            (key not in properties + definitions) and
+            (key not in properties) and
             (key in sys.modules[name].__dict__)
         ):
             sys.modules[name].__dict__.pop(key)
         # end if
     # end for
 # end clean_module
```

### Comparing `pystatic-language-1.0.2/pystatic/overload.py` & `pystatic-language-1.0.3/pystatic/overload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # overload.py
 
 import inspect
 from functools import partial
-from typing import Callable, Any, Union, Tuple, Dict
+from typing import Callable, Any, Union, Tuple, Dict, Optional
 
 from pystatic.types import (
     statictypes, RuntimeTypeError, RuntimeTypeWarning
 )
 
 __all__ = [
     "Overload",
@@ -55,25 +55,27 @@
     # end __init__
 # end OverloadSignatureTypeError
 
 class OverloadSignatureTypeWarning(Warning):
     """A class to represent a runtime type warning."""
 # end OverloadSignatureTypeWarning
 
-def is_regular_method(method: Union[Callable, staticmethod, classmethod]) -> bool:
+Method = Union[Callable, staticmethod, classmethod]
+
+def is_regular_method(method: Method) -> bool:
     """
     Checks if the method is not static or class method.
 
     :returns: The boolean value.
     """
 
     return not isinstance(method, (staticmethod, classmethod))
 # end is_regular_method
 
-def get_callable_method(method: Union[Callable, staticmethod, classmethod]) -> Callable:
+def get_callable_method(method: Method) -> Callable:
     """
     Gets the callable method from the given method.
 
     :returns: The callable method.
     """
 
     return method if is_regular_method(method) else method.__func__
@@ -97,32 +99,66 @@
             val.instance = self
         # end if
 
         return val
     # end __getattribute__
 # end OverloadProtocol
 
+def call(
+        c: Method,
+        instance: Any,
+        args: Tuple,
+        kwargs: Dict[str, Any]
+) -> Any:
+    """
+    Calls the decorated callable with the overloading match.
+
+    :param c: The callable object.
+    :param instance: The instance of the callable function.
+    :param args: The positional arguments.
+    :param kwargs: The keyword arguments.
+
+    :return: The returned value from the callable call.
+    """
+
+    if isinstance(c, staticmethod):
+        c = c.__func__
+
+    elif instance is not None:
+        if isinstance(c, classmethod):
+            # noinspection PyUnresolvedReferences
+            annotations = c.__func__.__annotations__
+            c = partial(c, type(instance))
+
+        else:
+            annotations = c.__annotations__
+            c = partial(c, instance)
+        # end if
+
+        c.__annotations__ = annotations
+    # end if
+
+    return statictypes(c)(*args, **kwargs)
+# end call
+
 class Overload:
     """A class to create an overload functionality."""
 
     def __init__(self, c: Callable) -> None:
         """
         Defines the class attributes.
 
         :param c: The decorated callable object.
         """
 
-        self.instance = None
+        self.instance: Optional[Any] = None
 
         self.c = c
 
-        self.signatures: Dict[
-            inspect.Signature,
-            Union[Callable, classmethod, staticmethod]
-        ] = {}
+        self.signatures: Dict[inspect.Signature, Method] = {}
     # end __init__
 
     def overload(self, c: Callable) -> object:
         """
         sets the signature of the decorated overloading callable object in the class.
 
         :param c: The decorated callable object.
@@ -144,57 +180,29 @@
         :param kwargs: The keyword arguments.
 
         :return: The returned value from the callable call.
         """
 
         for signature, c in self.signatures.items():
             try:
-                if isinstance(c, staticmethod):
-                    c = c.__func__
-
-                elif self.instance is not None:
-                    if isinstance(c, classmethod):
-                        annotations = c.__func__.__annotations__
-                        c = partial(c, type(self.instance))
-                        c.__annotations__ = annotations
-
-                    else:
-                        annotations = c.__annotations__
-                        c = partial(c, self.instance)
-                        c.__annotations__ = annotations
-                    # end if
-                # end if
-
-                return statictypes(c)(*args, **kwargs)
+                return call(
+                    c=c, instance=self.instance,
+                    args=args, kwargs=kwargs
+                )
 
             except (RuntimeTypeError, RuntimeTypeWarning, TypeError):
                 pass
             # end try
         # end for
 
-        c = self.c
-
-        if isinstance(c, staticmethod):
-            c = c.__func__
-
-        elif self.instance is not None:
-            if isinstance(c, classmethod):
-                annotations = c.__func__.__annotations__
-                c = partial(c, type(self.instance))
-                c.__annotations__ = annotations
-
-            else:
-                annotations = c.__annotations__
-                c = partial(c, self.instance)
-                c.__annotations__ = annotations
-            # end if
-        # end if
-
         try:
-            return statictypes(c)(*args, **kwargs)
+            return call(
+                c=self.c, instance=self.instance,
+                args=args, kwargs=kwargs
+            )
 
         except (RuntimeTypeError, TypeError):
             raise OverloadSignatureTypeError(
                 c=self.c, args=args, kwargs=kwargs
             )
 
         except RuntimeTypeWarning:
```

### Comparing `pystatic-language-1.0.2/pystatic/private.py` & `pystatic-language-1.0.3/pystatic/private.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,28 +46,28 @@
             frame = frame.f_back
 
         else:
             break
         # end if
     # end for
 
-    return list(frame.f_locals.values())[0] == obj
+    return list(frame.f_locals.values())[0] is obj
 # end in_scope
 
 class PrivateProperty:
     """A descriptor for private attributes."""
 
     def __init__(self, value: Optional[Any] = None) -> None:
         """
         Sets the private value.
 
         :param value: The value to store.
         """
 
-        self.instance = None
+        self.instance: Optional[Any] = None
 
         self.value = value
     # end __init__
 
     def __set_name__(self, instance: Any, name: str) -> None:
         """
         Sets the name of the attribute in the class.
@@ -89,17 +89,15 @@
         :param owner: The class type of the instance.
 
         :return: The attribute's value.
         """
 
         self.instance = instance or self.instance
 
-        inside = in_scope(self.instance, levels=4)
-
-        if not inside:
+        if not in_scope(self.instance, levels=4):
             raise AttributeError(
                 error_message(self.instance, self.name)
             )
 
         else:
             return self.value
         # end if
@@ -109,17 +107,15 @@
         """
         Sets the attribute value.
 
         :param instance: The instance of the class.
         :param value: The attribute's value.
         """
 
-        inside = in_scope(instance)
-
-        if not inside:
+        if not in_scope(instance):
             raise AttributeError(
                 error_message(self.instance, self.name)
             )
 
         else:
             self.value = value
         # end if
@@ -159,21 +155,20 @@
         :param value: The attribute's value.
         """
 
         if key in dir(object):
             return super().__setattr__(key, value)
         # end if
 
-        inside = in_scope(self)
-
-        if inside:
+        if in_scope(self):
             return super().__setattr__(key, value)
 
         else:
             raise AttributeError(error_message(self, key))
+        # end if
     # end __setattr__
 # end GeneralPrivateProtocol
 
 class PrivatePropertyProtocol:
     """A base model class to be the base of all objects."""
 
     def __getattribute__(self, key: str) -> Any:
```

### Comparing `pystatic-language-1.0.2/pystatic/types.py` & `pystatic-language-1.0.3/pystatic/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,14 @@
     if crush is None:
         crush = Config.crush
     # end if
 
     excluded_names = excluded_names or ()
     excluded_hints = excluded_hints or ()
 
-    # noinspection PyShadowingNames
     def wrap_call(*args: Any, **kwargs: Any) -> Any:
         """
         Wraps a callable object with runtime type enforcement.
 
         :param args: Any positional argument.
         :param kwargs: Any keyword argument.
 
@@ -116,15 +115,14 @@
         bound = signature.bind(*args, **kwargs)
         bound.apply_defaults()
 
         parameters = dict(zip(signature.parameters, bound.args))
         parameters.update(bound.kwargs)
 
         for key, value in obj.__annotations__.items():
-            # noinspection PyUnboundLocalVariable
             if any(
                 [
                     (key == "return"),
                     (key in excluded_names),
                     (value in excluded_hints)
                 ]
             ):
@@ -181,15 +179,14 @@
         return data
     # end wrap_call
 
     if obj is not None:
         return wrap_call
     
     else:
-        # noinspection PyShadowingNames
         def wrap_wrapper(value: Union[Type, Callable]) -> Callable:
             """
             Wraps a callable object with runtime type enforcement.
 
             :param value: The callable object.
 
             :returns: The inner wrapper function.
@@ -225,15 +222,15 @@
 
     if not Config.enforce:
         return obj
     # end if
 
     if inspect.isclass(obj):
         for key in dir(obj):
-            if key.startswith("_"):
+            if key.startswith("_") or not callable(getattr(obj, key)):
                 continue
             # end if
 
             setattr(
                 obj, key, __validate(
                     getattr(obj, key), excluded_names=excluded_names, 
                     excluded_hints=excluded_hints, crush=crush
```

### Comparing `pystatic-language-1.0.2/pystatic_language.egg-info/PKG-INFO` & `pystatic-language-1.0.3/pystatic_language.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystatic-language
-Version: 1.0.2
+Version: 1.0.3
 Summary: This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and.
 Home-page: https://github.com/Shahaf-F-S/pystatic
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystatic-language-1.0.2/setup.py` & `pystatic-language-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pystatic-language',
-        version='1.0.2',
+        version='1.0.3',
         description=(
             "This package is a collection of methods and classes for "
             "making python more secure, robust, and reliable. "
             "This could be achieved through the simple usage of decorators, "
             "function calls and inheritance of base classes. "
             "Generally, this package can make python a programming language, "
             "closer to other static-typed languages, "
```

### Comparing `pystatic-language-1.0.2/test.py` & `pystatic-language-1.0.3/test.py`

 * *Files identical despite different names*

