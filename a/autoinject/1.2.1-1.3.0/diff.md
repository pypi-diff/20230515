# Comparing `tmp/autoinject-1.2.1.tar.gz` & `tmp/autoinject-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoinject-1.2.1.tar", last modified: Mon Mar 27 01:58:49 2023, max compression
+gzip compressed data, was "autoinject-1.3.0.tar", last modified: Mon May 15 20:59:21 2023, max compression
```

## Comparing `autoinject-1.2.1.tar` & `autoinject-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 01:58:49.796271 autoinject-1.2.1/
--rw-rw-rw-   0        0        0     1058 2022-11-14 15:30:25.000000 autoinject-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     7565 2023-03-27 01:58:49.796271 autoinject-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6947 2023-03-27 01:46:59.000000 autoinject-1.2.1/README.md
--rw-rw-rw-   0        0        0       88 2022-11-14 15:30:25.000000 autoinject-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      809 2023-03-27 01:58:49.797286 autoinject-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-27 01:58:49.761271 autoinject-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-27 01:58:49.776270 autoinject-1.2.1/src/autoinject/
--rw-rw-rw-   0        0        0      496 2023-03-27 01:57:44.000000 autoinject-1.2.1/src/autoinject/__init__.py
--rw-rw-rw-   0        0        0      227 2022-11-14 15:30:25.000000 autoinject-1.2.1/src/autoinject/_tests.py
--rw-rw-rw-   0        0        0     6738 2022-11-14 17:59:47.000000 autoinject-1.2.1/src/autoinject/class_registry.py
--rw-rw-rw-   0        0        0     6226 2023-03-27 01:46:59.000000 autoinject-1.2.1/src/autoinject/context_manager.py
--rw-rw-rw-   0        0        0    11392 2023-03-27 01:55:52.000000 autoinject-1.2.1/src/autoinject/informants.py
--rw-rw-rw-   0        0        0    21080 2023-03-27 01:57:10.000000 autoinject-1.2.1/src/autoinject/injection.py
-drwxrwxrwx   0        0        0        0 2023-03-27 01:58:49.782270 autoinject-1.2.1/src/autoinject.egg-info/
--rw-rw-rw-   0        0        0     7565 2023-03-27 01:58:49.000000 autoinject-1.2.1/src/autoinject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2023-03-27 01:58:49.000000 autoinject-1.2.1/src/autoinject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 01:58:49.000000 autoinject-1.2.1/src/autoinject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-03-27 01:58:49.000000 autoinject-1.2.1/src/autoinject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-27 01:58:49.000000 autoinject-1.2.1/src/autoinject.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-27 01:58:49.794271 autoinject-1.2.1/tests/
--rw-rw-rw-   0        0        0    14330 2023-03-27 01:46:59.000000 autoinject-1.2.1/tests/test_context_manager.py
--rw-rw-rw-   0        0        0     1436 2022-11-14 15:30:25.000000 autoinject-1.2.1/tests/test_ep.py
--rw-rw-rw-   0        0        0    12874 2023-03-27 01:50:20.000000 autoinject-1.2.1/tests/test_injector.py
--rw-rw-rw-   0        0        0     2701 2022-11-14 17:58:39.000000 autoinject-1.2.1/tests/test_non_standard_injection.py
--rw-rw-rw-   0        0        0     3191 2022-11-14 15:30:25.000000 autoinject-1.2.1/tests/test_registry.py
--rw-rw-rw-   0        0        0     5175 2023-03-27 01:46:59.000000 autoinject-1.2.1/tests/test_threaded.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.607386 autoinject-1.3.0/
+-rw-rw-rw-   0        0        0     1058 2023-05-15 17:40:59.000000 autoinject-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     9942 2023-05-15 20:59:21.607386 autoinject-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9324 2023-05-15 20:58:54.000000 autoinject-1.3.0/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-15 17:40:59.000000 autoinject-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      809 2023-05-15 20:59:21.609386 autoinject-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.580387 autoinject-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.592386 autoinject-1.3.0/src/autoinject/
+-rw-rw-rw-   0        0        0      496 2023-05-15 19:38:33.000000 autoinject-1.3.0/src/autoinject/__init__.py
+-rw-rw-rw-   0        0        0      227 2023-05-15 17:40:59.000000 autoinject-1.3.0/src/autoinject/_tests.py
+-rw-rw-rw-   0        0        0     7138 2023-05-15 20:33:47.000000 autoinject-1.3.0/src/autoinject/class_registry.py
+-rw-rw-rw-   0        0        0     7469 2023-05-15 18:15:47.000000 autoinject-1.3.0/src/autoinject/context_manager.py
+-rw-rw-rw-   0        0        0    11411 2023-05-15 19:37:38.000000 autoinject-1.3.0/src/autoinject/informants.py
+-rw-rw-rw-   0        0        0    22482 2023-05-15 20:59:10.000000 autoinject-1.3.0/src/autoinject/injection.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.598386 autoinject-1.3.0/src/autoinject.egg-info/
+-rw-rw-rw-   0        0        0     9942 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.606387 autoinject-1.3.0/tests/
+-rw-rw-rw-   0        0        0    14330 2023-05-15 17:40:59.000000 autoinject-1.3.0/tests/test_context_manager.py
+-rw-rw-rw-   0        0        0     1436 2023-05-15 18:38:39.000000 autoinject-1.3.0/tests/test_ep.py
+-rw-rw-rw-   0        0        0    16373 2023-05-15 20:56:09.000000 autoinject-1.3.0/tests/test_injector.py
+-rw-rw-rw-   0        0        0     2701 2023-05-15 17:40:59.000000 autoinject-1.3.0/tests/test_non_standard_injection.py
+-rw-rw-rw-   0        0        0     3446 2023-05-15 20:18:25.000000 autoinject-1.3.0/tests/test_registry.py
+-rw-rw-rw-   0        0        0     5175 2023-05-15 17:40:59.000000 autoinject-1.3.0/tests/test_threaded.py
```

### Comparing `autoinject-1.2.1/LICENSE` & `autoinject-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoinject-1.2.1/PKG-INFO` & `autoinject-1.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: autoinject
-Version: 1.2.1
-Summary: Automated dependency injection for Python
-Home-page: https://github.com/turnbullerin/autoinject
-Author: Erin Turnbull
-Author-email: erin.a.turnbull@gmail.com
-Project-URL: Bug Tracker, https://github.com/turnbullerin/autoinject/issues
-Project-URL: Documentation, https://autoinject.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Autoinject
 
 [![Documentation Status](https://readthedocs.org/projects/autoinject/badge/?version=latest)](https://autoinject.readthedocs.io/en/latest/?badge=latest)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/turnbullerin/autoinject/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/turnbullerin/autoinject/tree/main)
 
 A clean, simple framework for automatically injecting dependencies into objects and functions
@@ -79,18 +63,93 @@
         pass
 
 # No need to do anything special here:
 obj = InjectMe()
 # obj.injected_attribute is set by the decorator before __init__() is called.
 ```
 
+## Specifying injected classes in tests
+
+You can override injected classes in your unit tests using the `@injector.test_case()` decorator. This provides an 
+independent global context within the test case function and allows you to pass a map of objects to inject. For example,
+
+```python
+
+from autoinject import injector 
+
+# Your injectable original class
+@injector.injectable_global 
+class ServiceConnection:
+  
+  def execute(self) -> int:
+    # Real connection code here, returns HTTP status code
+    pass
+  
+
+# The class you want to write a test case for that uses the injectable class.
+class UsesServiceConnection:
+  
+  connection: ServiceConnection = None
+  
+  @injector.construct 
+  def __init__(self):
+    pass
+  
+  def test_me(self) -> bool:
+    # Super simple, check if response code is under 400
+    resp_code = self.connection.execute()
+    return resp_code < 400
+  
+  
+# Testing stuff
+import unittest
+  
+# Stub for testing
+class _StubServiceFixture:
+  
+  def __init__(self, response_code):
+    self.response_code = response_code
+  
+  def execute(self) -> int:
+    return self.response_code
+
+
+# Test case
+class TestUsesServiceConnection(unittest.TestCase):
+
+    @injector.test_case({
+      ServiceConnection: _StubServiceFixture(200)
+    })
+    def test_success_200(self):
+        test_obj = UsesServiceConnection()  # this will use the injected objects now
+        self.assertTrue(test_obj.test_me())
+
+
+    @injector.test_case({
+      ServiceConnection: _StubServiceFixture(400)
+    })
+    def test_failure_400(self):
+        test_obj = UsesServiceConnection() 
+        self.assertFalse(test_obj.test_me())
+
+
+```
+
 Read the [full documentation](https://autoinject.readthedocs.io/en/latest/?) for more details.
 
 ## Changelog
 
+### v1.3.0
+- The new `@injector.test_case()` decorator is available for use with unit testing frameworks. It executes the decorated
+  function with a different global and non-global context to ensure the independence of test functions. In addition, one
+  can override the injected classes to provide specific test fixtures. These are passed as a dict of either `type` objects 
+  or fully qualified class names as strings as keys and either the `type` or class name as string (to create the object), 
+  or an object or function to use as the injected object.
+- A bug was fixed where exceptions within a context caused issues with the new contextvars integration.
+
 ### v1.2.0
 - Contextvar-driven contexts are now respected by default
 - Several wrappers exist to better support using contextvars. All of them provide for a separate set of injected 
   CONTEXT_CACHE dependencies. In addition, each is a wrapper around `@injector.inject`, so both are not needed.
   - `@injector.with_contextvars`: Creates a new context that is a copy of the current one 
   - `@injector.with_same_contextvars`: Uses the current context
   - `@injector.with_empty_contextvars`: Creates a new empty context
@@ -106,15 +165,15 @@
   - If the "same" context is used:
     - `run()` will just directly call the function (it is in the current context essentially)
     - `copy()` is an alias for `contextvars.copy_context()`
     - Other functions besides `set()` and `reset()` make a copy of the current context and return the results of its
       method. This copy is transient and remade each time, so modules making extensive use of it can call `copy()` and
       check the copy.
 - Note that, unlike the context manager, the decorators also RUN the inner code in the given context.  
-- Thread-handling was improved significantly and now also includes a wrapper function for your `run()` methods to
+- Thread-handling was improved significantly and now also includes a wrapper function for `threading.Thread.run()` methods to
   ensure clean-up (`@injector.as_thread_run()`). This also is a wrapper around `@injector.inject` so you can inject
   variables into your `run()` method directly.
 
 ### v1.1.0
 - Injectable objects may now define a `__cleanup__()` method which will be invoked when the global cache or context
   cache is cleared.
 - Note that `__cleanup__()` IS NOT INVOKED for one-time use objects at the moment, but this is planned as a feature.
```

### Comparing `autoinject-1.2.1/README.md` & `autoinject-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: autoinject
+Version: 1.3.0
+Summary: Automated dependency injection for Python
+Home-page: https://github.com/turnbullerin/autoinject
+Author: Erin Turnbull
+Author-email: erin.a.turnbull@gmail.com
+Project-URL: Bug Tracker, https://github.com/turnbullerin/autoinject/issues
+Project-URL: Documentation, https://autoinject.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Autoinject
 
 [![Documentation Status](https://readthedocs.org/projects/autoinject/badge/?version=latest)](https://autoinject.readthedocs.io/en/latest/?badge=latest)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/turnbullerin/autoinject/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/turnbullerin/autoinject/tree/main)
 
 A clean, simple framework for automatically injecting dependencies into objects and functions
@@ -63,18 +79,93 @@
         pass
 
 # No need to do anything special here:
 obj = InjectMe()
 # obj.injected_attribute is set by the decorator before __init__() is called.
 ```
 
+## Specifying injected classes in tests
+
+You can override injected classes in your unit tests using the `@injector.test_case()` decorator. This provides an 
+independent global context within the test case function and allows you to pass a map of objects to inject. For example,
+
+```python
+
+from autoinject import injector 
+
+# Your injectable original class
+@injector.injectable_global 
+class ServiceConnection:
+  
+  def execute(self) -> int:
+    # Real connection code here, returns HTTP status code
+    pass
+  
+
+# The class you want to write a test case for that uses the injectable class.
+class UsesServiceConnection:
+  
+  connection: ServiceConnection = None
+  
+  @injector.construct 
+  def __init__(self):
+    pass
+  
+  def test_me(self) -> bool:
+    # Super simple, check if response code is under 400
+    resp_code = self.connection.execute()
+    return resp_code < 400
+  
+  
+# Testing stuff
+import unittest
+  
+# Stub for testing
+class _StubServiceFixture:
+  
+  def __init__(self, response_code):
+    self.response_code = response_code
+  
+  def execute(self) -> int:
+    return self.response_code
+
+
+# Test case
+class TestUsesServiceConnection(unittest.TestCase):
+
+    @injector.test_case({
+      ServiceConnection: _StubServiceFixture(200)
+    })
+    def test_success_200(self):
+        test_obj = UsesServiceConnection()  # this will use the injected objects now
+        self.assertTrue(test_obj.test_me())
+
+
+    @injector.test_case({
+      ServiceConnection: _StubServiceFixture(400)
+    })
+    def test_failure_400(self):
+        test_obj = UsesServiceConnection() 
+        self.assertFalse(test_obj.test_me())
+
+
+```
+
 Read the [full documentation](https://autoinject.readthedocs.io/en/latest/?) for more details.
 
 ## Changelog
 
+### v1.3.0
+- The new `@injector.test_case()` decorator is available for use with unit testing frameworks. It executes the decorated
+  function with a different global and non-global context to ensure the independence of test functions. In addition, one
+  can override the injected classes to provide specific test fixtures. These are passed as a dict of either `type` objects 
+  or fully qualified class names as strings as keys and either the `type` or class name as string (to create the object), 
+  or an object or function to use as the injected object.
+- A bug was fixed where exceptions within a context caused issues with the new contextvars integration.
+
 ### v1.2.0
 - Contextvar-driven contexts are now respected by default
 - Several wrappers exist to better support using contextvars. All of them provide for a separate set of injected 
   CONTEXT_CACHE dependencies. In addition, each is a wrapper around `@injector.inject`, so both are not needed.
   - `@injector.with_contextvars`: Creates a new context that is a copy of the current one 
   - `@injector.with_same_contextvars`: Uses the current context
   - `@injector.with_empty_contextvars`: Creates a new empty context
@@ -90,15 +181,15 @@
   - If the "same" context is used:
     - `run()` will just directly call the function (it is in the current context essentially)
     - `copy()` is an alias for `contextvars.copy_context()`
     - Other functions besides `set()` and `reset()` make a copy of the current context and return the results of its
       method. This copy is transient and remade each time, so modules making extensive use of it can call `copy()` and
       check the copy.
 - Note that, unlike the context manager, the decorators also RUN the inner code in the given context.  
-- Thread-handling was improved significantly and now also includes a wrapper function for your `run()` methods to
+- Thread-handling was improved significantly and now also includes a wrapper function for `threading.Thread.run()` methods to
   ensure clean-up (`@injector.as_thread_run()`). This also is a wrapper around `@injector.inject` so you can inject
   variables into your `run()` method directly.
 
 ### v1.1.0
 - Injectable objects may now define a `__cleanup__()` method which will be invoked when the global cache or context
   cache is cleared.
 - Note that `__cleanup__()` IS NOT INVOKED for one-time use objects at the moment, but this is planned as a feature.
```

### Comparing `autoinject-1.2.1/setup.cfg` & `autoinject-1.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7574 6f69 6e6a 6563 740d 0a76   = autoinject..v
-00000020: 6572 7369 6f6e 203d 2031 2e32 2e31 0d0a  ersion = 1.2.1..
+00000020: 6572 7369 6f6e 203d 2031 2e33 2e30 0d0a  ersion = 1.3.0..
 00000030: 6175 7468 6f72 203d 2045 7269 6e20 5475  author = Erin Tu
 00000040: 726e 6275 6c6c 0d0a 6175 7468 6f72 5f65  rnbull..author_e
 00000050: 6d61 696c 203d 2065 7269 6e2e 612e 7475  mail = erin.a.tu
 00000060: 726e 6275 6c6c 4067 6d61 696c 2e63 6f6d  rnbull@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4175 746f 6d61 7465 6420 6465 7065 6e64  Automated depend
 00000090: 656e 6379 2069 6e6a 6563 7469 6f6e 2066  ency injection f
```

### Comparing `autoinject-1.2.1/src/autoinject/class_registry.py` & `autoinject-1.3.0/src/autoinject/class_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """ The class registry stores which objects can be injected and how to
     maintain cache control over them.
 
 .. moduleauthor:: Erin Turnbull <erin.a.turnbull@gmail.com>
 
 """
 import enum
+import functools
 import importlib
+import typing as t
 
 
 class CacheStrategy(enum.Enum):
     """ Defines how caching should be managed for this object """
 
     NO_CACHE = 1
     """ No caching allowed. Specify this when instances of the object should not be shared."""
@@ -37,17 +39,18 @@
         """ Constructor """
         super().__init__("Object {} not registered for injection".format(cls_name))
 
 
 class ClassRegistry:
     """ Manages a list of classes and how they can be instantiated. """
 
-    def __init__(self):
+    def __init__(self, injector = None):
         """ Constructor """
         self.object_constructors = {}
+        self.injector = injector
 
     def cls_to_str(self, cls) -> str:
         """ Converts a type to a string that represents the fully-qualified name of the class.
         :param cls: Either a type to convert or a string representing the fully-qualified name of the class.
         :type cls: type OR str
         :return: Returns a string that could be used to import the class
         :rtype: str
@@ -64,19 +67,20 @@
             :type cls: type
             :return: Whether the class provided can be injected
             :rtype: bool
         """
         return self.cls_to_str(cls) in self.object_constructors
 
     def register(self,
-                 cls: type,
+                 cls: t.Union[type, str],
                  *args,
                  weight: int = 0,
                  constructor: callable = None,
                  caching_strategy: CacheStrategy = None,
+                 _force_override: bool = False,
                  **kwargs):
         """ Registers a class for injection and specifies how to construct it
 
         The default method of construction is to call ``cls`` itself with ``args`` and ``kwargs``, i.e.:
 
         ``cls(*args, **kwargs)``
 
@@ -90,28 +94,32 @@
         :param args: Positional arguments to pass to the constructor
         :type args: any
         :param constructor: Optional callable to construct an object when required. Defaults to calling ``cls`` directly
         :type constructor: callable or None
         :param caching_strategy: Specify how instances of this class are to be cached. Defaults to
             :attr:`autoinject.class_registry.CacheStrategy.CONTEXT_CACHE`, i.e. different objects by context
         :type caching_strategy: :class:`autoinject.class_registry.CacheStrategy` or None
+        :param weight: Higher values override lower values
+        :type weight: int
+        :param _force_override: Set to true to ignore weight and replace the constructor anyways
+        :type _force_override: bool
         :param kwargs: Keyword arguments to pass to the constructor
         :type kwargs: any
         """
         if constructor is None:
             if not isinstance(cls, type):
                 raise ValueError("A valid constructor must be passed")
             constructor = cls
         elif isinstance(constructor, str):
             constructor = self._resolve_constructor(constructor)
         cls_str = self.cls_to_str(cls)
         if caching_strategy is None:
             caching_strategy = CacheStrategy.CONTEXT_CACHE if cls_str not in self.object_constructors else self.object_constructors[cls_str][3]
         # Ignore if a higher-weight constructor is already present
-        if cls_str in self.object_constructors and weight < self.object_constructors[cls_str][4]:
+        if (not _force_override) and cls_str in self.object_constructors and weight < self.object_constructors[cls_str][4]:
             return
         self.object_constructors[cls_str] = (constructor, args, kwargs, caching_strategy, weight)
 
     def _resolve_constructor(self, cls: str):
         """Resolves a constructor specified as a string (e.g. a fully-qualified class name or function) to an actual
             object.
         """
```

### Comparing `autoinject-1.2.1/src/autoinject/context_manager.py` & `autoinject-1.3.0/src/autoinject/context_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,41 @@
 
 
 # Time that must elapse since last call to cleanup() before get_object() will automatically
 # trigger the call.
 GARBAGE_COLLECTION_FREQUENCY = 5
 
 
+class _SubContextManager:
+    """Manage a sub-context which will have a different GLOBAL state as well (used for test cases)."""
+
+    def __init__(self, context_manager):
+        self.context_manager = context_manager
+        self._global_cache = None
+        self._context_cache = None
+        self._constructors = None
+
+    def __enter__(self):
+        self._global_cache = self.context_manager._global_cache
+        self._context_cache = self.context_manager._context_cache
+        self._constructors = self.context_manager._registry.object_constructors
+        self.context_manager._global_cache = {}
+        self.context_manager._context_cache = {}
+        return self.context_manager
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.context_manager.teardown()
+        self.context_manager._global_cache = self._global_cache
+        self.context_manager._context_cache = self._context_cache
+        self.context_manager._registry.object_constructors = self._constructors
+        self._global_cache = None
+        self._context_cache = None
+        self._constructors = None
+
+
 class ContextManager:
     """  Responsible for managing the object caches based on the context.
 
         A context can be anything that other packages would like to define; it is defined by an implementation of
         :class:`autoinject.informants.ContextInformant` which provides the context manager with a unique value for
         each context. If multiple informants are registered, they are aggregated together; if any informant reports
         a different context ID, then it is a different context.
@@ -104,15 +131,19 @@
 
     def cleanup(self):
         """ Asks each informant to check for expired contexts """
         for informant in self._informants:
             informant.check_expired_contexts()
         self._last_gc = time.monotonic()
 
+    def subcontext(self):
+        return _SubContextManager(self)
+
     def clear_cache(self, cls):
+        """Remove the class from all caches."""
         cls_as_str = self._registry.cls_to_str(cls)
         if cls_as_str in self._global_cache:
             del self._global_cache[cls_as_str]
         for ctx in self._context_cache:
             if cls_as_str in self._context_cache[ctx]:
                 del self._context_cache[ctx][cls_as_str]
```

### Comparing `autoinject-1.2.1/src/autoinject/informants.py` & `autoinject-1.3.0/src/autoinject/informants.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,18 @@
         return self.run(var.reset, token)
 
     def run(self, fn, *args, **kwargs):
         """Run, in context if appropriate."""
         if self._delegate_run and self._context is not None:
             # Prevent running the context from within the context
             self._delegate_run = False
-            result = self._context.run(fn, *args, **kwargs)
-            self._delegate_run = True
-            return result
+            try:
+                return self._context.run(fn, *args, **kwargs)
+            finally:
+                self._delegate_run = True
         else:
             return fn(*args, **kwargs)
 
     def copy(self, same_autoinject_context: bool = False):
         """Make a copy of the context, with optional parameter to keep or reset the autoinjection variables."""
         ContextVarManager.ensure_context_id(self)
         new_context = contextvars.copy_context() if self._context is None else self._context.copy()
```

### Comparing `autoinject-1.2.1/src/autoinject/injection.py` & `autoinject-1.3.0/src/autoinject/injection.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         :meth:`autoinject.injection.InjectionManager.construct` decorator on the class's ``__init__()`` method. It will
         search for CLASS attributes with an injectable type-hint and inject the objects into the INSTANCE attributes
         as required.
     """
 
     def __init__(self, include_entry_points=True):
         """ Constructor """
-        self.cls_registry = ClassRegistry()
+        self.cls_registry = ClassRegistry(self)
         self.context_manager = ContextManager(self.cls_registry)
         # Register the class registry for injection, using the local instance
         self.cls_registry.register(
             ClassRegistry,
             constructor=lambda: self.cls_registry,
             caching_strategy=CacheStrategy.GLOBAL_CACHE
         )
@@ -104,14 +104,37 @@
                 registrar_func(self)
             # Handle the autoinject.injectables entry point
             auto_inject = entry_points(group="autoinject.injectables")
             for inject in auto_inject:
                 cls = inject.load()
                 self.register_constructor(cls, constructor=cls)
 
+    def test_case(self, fixtures_or_fn: t.Union[callable, dict, None] = None) -> callable:
+        """Decorate a test case to get a separate global context and to provide fixtures."""
+        if isinstance(fixtures_or_fn, dict) or fixtures_or_fn is None:
+            def outer_wrapper(fn):
+                return self._test_case_wrapper(fn, fixtures_or_fn)
+            return outer_wrapper
+        return self._test_case_wrapper(fixtures_or_fn, None)
+
+    def _test_case_wrapper(self, fn: callable, fixtures: dict = None) -> callable:
+        """Handle creating a separate global context and test fixtures"""
+        @wraps(fn)
+        def inner_wrapper(*args, **kwargs):
+            # This creates an entirely different GLOBAL context as well local context, so
+            # that test cases can be truly independent of the shared global state.
+            with self.context_manager.subcontext() as ctx:
+                for cls_name in fixtures or []:
+                    if isinstance(fixtures[cls_name], type) or isinstance(fixtures[cls_name], str)hon -m:
+                        self.cls_registry.register(cls_name, constructor=fixtures[cls_name], _force_override=True)
+                    else:
+                        self.cls_registry.register(cls_name, constructor=lambda: fixtures[cls_name], _force_override=True)
+                return fn(*args, **kwargs)
+        return inner_wrapper
+
     def ContextVars(self, context: t.Union[contextvars.Context, ContextVarManager, str, None] = "_default", suppress_exit_warning: bool = False):
         """Use as a context manager for managing an area where all context_cache injectables are the same."""
         return ContextVarManager(self.context_manager.contextvar_info, context, suppress_exit_warning=suppress_exit_warning)
 
     def cv_freshen(self, context: contextvars.Context = None):
         """Freshen the context var to get a new context and return the old one"""
         return ContextVarManager.freshen_context(context)
@@ -289,15 +312,15 @@
         else:
             return self._async_injector_wrap(func, with_contextvars, context_mode)
 
     def _async_injector_wrap(self, func, with_contextvars: bool = False, context_mode="_default"):
         @wraps(func)
         async def wrapper(*args, **kwargs):
             if with_contextvars:
-                with ContextVarManager(self.context_manager.contextvar_info, context_mode, delegate_run=False) as ctx:
+                with ContextVarManager(self.context_manager.contextvar_info, context_mode) as ctx:
                     new_args, new_kwargs = self._bind_parameters(func, args, kwargs, ctx)
                     return await ctx.run(func, *new_args, **new_kwargs)
             else:
                 new_args, new_kwargs = self._bind_parameters(func, args, kwargs)
                 return await func(*new_args, **new_kwargs)
         return wrapper
```

### Comparing `autoinject-1.2.1/src/autoinject.egg-info/PKG-INFO` & `autoinject-1.3.0/src/autoinject.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoinject
-Version: 1.2.1
+Version: 1.3.0
 Summary: Automated dependency injection for Python
 Home-page: https://github.com/turnbullerin/autoinject
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/autoinject/issues
 Project-URL: Documentation, https://autoinject.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
@@ -79,18 +79,93 @@
         pass
 
 # No need to do anything special here:
 obj = InjectMe()
 # obj.injected_attribute is set by the decorator before __init__() is called.
 ```
 
+## Specifying injected classes in tests
+
+You can override injected classes in your unit tests using the `@injector.test_case()` decorator. This provides an 
+independent global context within the test case function and allows you to pass a map of objects to inject. For example,
+
+```python
+
+from autoinject import injector 
+
+# Your injectable original class
+@injector.injectable_global 
+class ServiceConnection:
+  
+  def execute(self) -> int:
+    # Real connection code here, returns HTTP status code
+    pass
+  
+
+# The class you want to write a test case for that uses the injectable class.
+class UsesServiceConnection:
+  
+  connection: ServiceConnection = None
+  
+  @injector.construct 
+  def __init__(self):
+    pass
+  
+  def test_me(self) -> bool:
+    # Super simple, check if response code is under 400
+    resp_code = self.connection.execute()
+    return resp_code < 400
+  
+  
+# Testing stuff
+import unittest
+  
+# Stub for testing
+class _StubServiceFixture:
+  
+  def __init__(self, response_code):
+    self.response_code = response_code
+  
+  def execute(self) -> int:
+    return self.response_code
+
+
+# Test case
+class TestUsesServiceConnection(unittest.TestCase):
+
+    @injector.test_case({
+      ServiceConnection: _StubServiceFixture(200)
+    })
+    def test_success_200(self):
+        test_obj = UsesServiceConnection()  # this will use the injected objects now
+        self.assertTrue(test_obj.test_me())
+
+
+    @injector.test_case({
+      ServiceConnection: _StubServiceFixture(400)
+    })
+    def test_failure_400(self):
+        test_obj = UsesServiceConnection() 
+        self.assertFalse(test_obj.test_me())
+
+
+```
+
 Read the [full documentation](https://autoinject.readthedocs.io/en/latest/?) for more details.
 
 ## Changelog
 
+### v1.3.0
+- The new `@injector.test_case()` decorator is available for use with unit testing frameworks. It executes the decorated
+  function with a different global and non-global context to ensure the independence of test functions. In addition, one
+  can override the injected classes to provide specific test fixtures. These are passed as a dict of either `type` objects 
+  or fully qualified class names as strings as keys and either the `type` or class name as string (to create the object), 
+  or an object or function to use as the injected object.
+- A bug was fixed where exceptions within a context caused issues with the new contextvars integration.
+
 ### v1.2.0
 - Contextvar-driven contexts are now respected by default
 - Several wrappers exist to better support using contextvars. All of them provide for a separate set of injected 
   CONTEXT_CACHE dependencies. In addition, each is a wrapper around `@injector.inject`, so both are not needed.
   - `@injector.with_contextvars`: Creates a new context that is a copy of the current one 
   - `@injector.with_same_contextvars`: Uses the current context
   - `@injector.with_empty_contextvars`: Creates a new empty context
@@ -106,15 +181,15 @@
   - If the "same" context is used:
     - `run()` will just directly call the function (it is in the current context essentially)
     - `copy()` is an alias for `contextvars.copy_context()`
     - Other functions besides `set()` and `reset()` make a copy of the current context and return the results of its
       method. This copy is transient and remade each time, so modules making extensive use of it can call `copy()` and
       check the copy.
 - Note that, unlike the context manager, the decorators also RUN the inner code in the given context.  
-- Thread-handling was improved significantly and now also includes a wrapper function for your `run()` methods to
+- Thread-handling was improved significantly and now also includes a wrapper function for `threading.Thread.run()` methods to
   ensure clean-up (`@injector.as_thread_run()`). This also is a wrapper around `@injector.inject` so you can inject
   variables into your `run()` method directly.
 
 ### v1.1.0
 - Injectable objects may now define a `__cleanup__()` method which will be invoked when the global cache or context
   cache is cleared.
 - Note that `__cleanup__()` IS NOT INVOKED for one-time use objects at the moment, but this is planned as a feature.
```

### Comparing `autoinject-1.2.1/src/autoinject.egg-info/SOURCES.txt` & `autoinject-1.3.0/src/autoinject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoinject-1.2.1/tests/test_context_manager.py` & `autoinject-1.3.0/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.2.1/tests/test_ep.py` & `autoinject-1.3.0/tests/test_ep.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.2.1/tests/test_injector.py` & `autoinject-1.3.0/tests/test_injector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import unittest
 import inspect
-import eptest
 import contextvars
+import autoinject
 
 
 cv: contextvars.ContextVar[str] = contextvars.ContextVar[str]("_test_hello", default=None)
 cv2 = contextvars.ContextVar[str]("_test2", default=None)
-import autoinject
 
 
 class NonLocalInjectionOne:
     pass
 
 
 class TestInjection(unittest.TestCase):
@@ -53,25 +52,41 @@
                 self.arg = arg
 
         self.injector.register_constructor(TestClassFoo, TestClassFoo)
         obj = self.injector.get(TestClassFoo)
         self.assertIsInstance(obj, TestClassFoo)
         self.assertEqual(obj.arg, 1)
 
-    def test_exception_in_block(self):
+    def test_value_exception_in_block(self):
+
         @self.injector.with_contextvars
         def make_error():
             def do_error():
-                raise ValueError()
+                raise ValueError("foobar")
 
-            c = contextvars.Context()
-            c2 = contextvars.Context()
-            c.run(c2.run, do_error)
+            try:
+                contextvars.copy_context().run(do_error)
+            except Exception as ex:
+                raise ValueError("inner")
+                print(ex)
         self.assertRaises(ValueError, make_error)
 
+    def test_exception_in_block(self):
+
+        class CustomException(Exception):
+            pass
+
+        @self.injector.with_contextvars
+        def make_error():
+            def do_error():
+                raise CustomException()
+
+            do_error()
+        self.assertRaises(CustomException, make_error)
+
     def test_inherited_injection(self):
 
         @self.injector.injectable
         class InjectableOne:
             pass
 
         class ParentInjectable:
@@ -118,14 +133,114 @@
         cv.set("first")
         self.assertEqual(cv.get(), "first")
         c = contextvars.Context()
         result = test_method("second")
         self.assertEqual(result, "second")
         self.assertEqual(cv.get(), "first")
 
+    def test_test_case_wrapper_local(self):
+
+        class TestClassFoo:
+
+            def __init__(self, arg=1):
+                self.arg = arg
+
+        self.injector.injectable(TestClassFoo)
+        obj = self.injector.get(TestClassFoo)
+        self.assertIsInstance(obj, TestClassFoo)
+        self.assertEqual(obj.arg, 1)
+
+        @self.injector.test_case
+        def example_test_case():
+            obj2 = self.injector.get(TestClassFoo)
+            self.assertIsInstance(obj2, TestClassFoo)
+            self.assertNotEqual(hash(obj), hash(obj2))
+
+        example_test_case()
+
+        obj3 = self.injector.get(TestClassFoo)
+        self.assertEqual(hash(obj), hash(obj3))
+
+    def test_test_case_wrapper_obj(self):
+
+        class TestClassFoo:
+
+            def __init__(self, arg=1):
+                self.arg = arg
+
+        self.injector.injectable(TestClassFoo)
+        obj = self.injector.get(TestClassFoo)
+        self.assertIsInstance(obj, TestClassFoo)
+        self.assertEqual(obj.arg, 1)
+
+        @self.injector.test_case({TestClassFoo: TestClassFoo(5)})
+        def example_test_case():
+            obj2 = self.injector.get(TestClassFoo)
+            self.assertIsInstance(obj2, TestClassFoo)
+            self.assertEqual(obj2.arg, 5)
+            self.assertNotEqual(hash(obj), hash(obj2))
+
+        example_test_case()
+
+        obj3 = self.injector.get(TestClassFoo)
+        self.assertEqual(hash(obj), hash(obj3))
+
+    def test_test_case_wrapper_global(self):
+
+        class TestClassFoo:
+
+            def __init__(self, arg=1):
+                self.arg = arg
+
+        self.injector.injectable_global(TestClassFoo)
+        obj = self.injector.get(TestClassFoo)
+        self.assertIsInstance(obj, TestClassFoo)
+        self.assertEqual(obj.arg, 1)
+
+        @self.injector.test_case
+        def example_test_case():
+            obj2 = self.injector.get(TestClassFoo)
+            self.assertIsInstance(obj2, TestClassFoo)
+            self.assertNotEqual(hash(obj), hash(obj2))
+
+        example_test_case()
+
+        obj3 = self.injector.get(TestClassFoo)
+        self.assertEqual(hash(obj), hash(obj3))
+
+    def test_test_case_wrapper_fixture_type(self):
+
+        class TestClassFoo:
+
+            def __init__(self, arg=1):
+                self.arg = arg
+
+        class TestClassBar:
+
+            def __init__(self):
+                self.arg = 3
+
+        self.injector.injectable_global(TestClassFoo)
+        obj = self.injector.get(TestClassFoo)
+        self.assertIsInstance(obj, TestClassFoo)
+        self.assertEqual(obj.arg, 1)
+
+        @self.injector.test_case({TestClassFoo: TestClassBar})
+        def example_test_case():
+            obj2 = self.injector.get(TestClassFoo)
+            self.assertIsInstance(obj2, TestClassBar)
+            self.assertNotEqual(hash(obj), hash(obj2))
+            self.assertEqual(obj2.arg, 3)
+
+        example_test_case()
+
+        obj3 = self.injector.get(TestClassFoo)
+        self.assertEqual(hash(obj3), hash(obj))
+        self.assertEqual(obj3.arg, 1)
+
     def test_register_class_with_args(self):
         class TestClassFoo:
 
             def __init__(self, arg=1, kwarg=1):
                 self.arg = arg
                 self.kwarg = kwarg
```

### Comparing `autoinject-1.2.1/tests/test_non_standard_injection.py` & `autoinject-1.3.0/tests/test_non_standard_injection.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.2.1/tests/test_registry.py` & `autoinject-1.3.0/tests/test_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,20 @@
     def test_register_base_class(self):
         self.assertFalse(self.registry.is_injectable(self.test_class))
         self.assertRaises(autoinject.ClassNotFoundException, self.registry.get_instance, self.test_class)
         self.registry.register(self.test_class)
         self.assertTrue(self.registry.is_injectable(self.test_class))
         self.assertIsInstance(self.registry.get_instance(self.test_class), self.test_class)
 
+    def test_bad_register(self):
+        self.assertRaises(ValueError, self.registry.register, "foobar")
+
+    def test_bad_fetch(self):
+        self.assertRaises(autoinject.ClassNotFoundException, self.registry.get_cache_strategy, self.test_class)
+
     def test_register_class_by_name(self):
         self.assertFalse(self.registry.is_injectable("tests.test_registry.ForTestByName"))
         self.assertRaises(autoinject.ClassNotFoundException, self.registry.get_instance, "tests.test_registry.ForTestByName")
         self.registry.register(ForTestByName)
         self.assertTrue(self.registry.is_injectable("tests.test_registry.ForTestByName"))
         self.assertIsInstance(self.registry.get_instance("tests.test_registry.ForTestByName"), ForTestByName)
```

### Comparing `autoinject-1.2.1/tests/test_threaded.py` & `autoinject-1.3.0/tests/test_threaded.py`

 * *Files identical despite different names*

