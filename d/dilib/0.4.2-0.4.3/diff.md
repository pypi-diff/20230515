# Comparing `tmp/dilib-0.4.2.tar.gz` & `tmp/dilib-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dilib-0.4.2.tar", last modified: Thu Jan  5 21:36:44 2023, max compression
+gzip compressed data, was "dilib-0.4.3.tar", last modified: Sun May 14 23:50:40 2023, max compression
```

## Comparing `dilib-0.4.2.tar` & `dilib-0.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:36:44.434319 dilib-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:36:44.426319 dilib-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:36:44.430318 dilib-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-01-05 21:36:24.000000 dilib-0.4.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-01-05 21:36:24.000000 dilib-0.4.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-05 21:36:24.000000 dilib-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-05 21:36:24.000000 dilib-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-01-05 21:36:44.434319 dilib-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-01-05 21:36:24.000000 dilib-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:36:44.434319 dilib-0.4.2/dilib/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:36:44.434319 dilib-0.4.2/dilib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/tests/test_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-01-05 21:36:24.000000 dilib-0.4.2/dilib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-05 21:36:44.000000 dilib-0.4.2/dilib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 21:36:44.434319 dilib-0.4.2/dilib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-01-05 21:36:44.000000 dilib-0.4.2/dilib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-05 21:36:44.000000 dilib-0.4.2/dilib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 21:36:44.000000 dilib-0.4.2/dilib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-05 21:36:44.000000 dilib-0.4.2/dilib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-05 21:36:44.000000 dilib-0.4.2/dilib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-05 21:36:24.000000 dilib-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-05 21:36:24.000000 dilib-0.4.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-01-05 21:36:44.438319 dilib-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:50:40.627376 dilib-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:50:40.623376 dilib-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:50:40.627376 dilib-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-14 23:50:24.000000 dilib-0.4.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-14 23:50:24.000000 dilib-0.4.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 23:50:24.000000 dilib-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 23:50:24.000000 dilib-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-14 23:50:40.627376 dilib-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-05-14 23:50:24.000000 dilib-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:50:40.627376 dilib-0.4.3/dilib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:50:40.627376 dilib-0.4.3/dilib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/tests/test_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 23:50:24.000000 dilib-0.4.3/dilib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 23:50:40.000000 dilib-0.4.3/dilib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:50:40.627376 dilib-0.4.3/dilib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-14 23:50:40.000000 dilib-0.4.3/dilib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-14 23:50:40.000000 dilib-0.4.3/dilib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:50:40.000000 dilib-0.4.3/dilib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 23:50:40.000000 dilib-0.4.3/dilib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 23:50:40.000000 dilib-0.4.3/dilib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-14 23:50:24.000000 dilib-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 23:50:24.000000 dilib-0.4.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-14 23:50:40.631377 dilib-0.4.3/setup.cfg
```

### Comparing `dilib-0.4.2/.github/workflows/publish.yml` & `dilib-0.4.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/.github/workflows/test.yml` & `dilib-0.4.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/LICENSE` & `dilib-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/PKG-INFO` & `dilib-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dilib
-Version: 0.4.2
+Version: 0.4.3
 Summary: Dependency injection library
 Home-page: https://github.com/ansatzcapital/dilib
 License: Apache License 2.0
 Project-URL: Packaging, https://pypi.org/project/dilib/
 Project-URL: Source, https://github.com/ansatzcapital/dilib
 Project-URL: Tracker, https://github.com/ansatzcapital/dilib/issues
 Keywords: dependency injection, di, inversion of control, ioc, design patterns
@@ -121,26 +121,26 @@
     # Forward spec resolution to the target spec
     engine: Engine = dilib.Forward(engine0)
 
 
 class CarConfig(dilib.Config):
     # Configs depend on other configs via types. 
     # Here, CarConfig depends on EngineConfig.
-    engine_config = EngineConfig(foo_prefix="baz")
+    engine_config = EngineConfig(token_prefix="baz")
 
     car = dilib.Singleton(Car, engine_config.engine)
 
 
 # Get instance of config (with global input value set)
 car_config: CarConfig = dilib.get_config(
   CarConfig, db_addr="some-other-db-addr"
 )
 
 # Perturb here as you'd like. E.g.:
-car_config.engine_config.Engine = dilib.Singleton(MockEngine)
+car_config.engine_config.engine = dilib.Singleton(MockEngine)
 
 # Pass config to a container
 container: dilib.Container[CarConfig] = dilib.get_container(car_config)
 
 # Retrieve objects from container (some of which are cached inside)
 assert container.config.engine_config.db_addr == "some-other-db-addr"
 assert isinstance(container.config.engine_config.engine, MockEngine)
@@ -312,35 +312,43 @@
 ### Factories for Dynamic Objects
 
 If you need to configure objects dynamically 
 (e.g., check db value to resolve what type to use, 
 set config keys based on another value), consider a factory pattern like:
 
 ```python
+import dataclasses
+
 import dilib
 
 
+# Object that needs to be created dynamically
+@dataclasses.dataclass(frozen=True)
 class Foo:
-    @property
-    def value(self) -> int:
-        raise NotImplementedError
+    value: int
 
 
+# Factory that takes static params via constructor injection and dynamic params via method injection
+@dataclasses.dataclass(frozen=True)
 class FooFactory:
-    def get_foo(self) -> Foo:
+    db_host: str
+    alpha: int
+    beta: int
+
+    def get_foo(self, gamma: int) -> Foo:
         raise NotImplementedError
 
 
+# Object that needs Foo object
+@dataclasses.dataclass(frozen=True)
 class FooClient:
-    def __init__(self, foo_factory: FooFactory):
-        self.foo_factory = foo_factory
-        
-    def get_foo_value(self) -> int:
-        foo = self.foo_factory.get_foo()
-        return foo.value
+    foo_factory: FooFactory
+
+    def process_foo_value(self) -> int:
+        return 100 + self.foo_factory.get_foo(gamma=3).value
 
 
 class FooConfig(dilib.Config):
-    db_param = dilib.Object("some-db-addr")
-    foo_factory = dilib.Singleton(FooFactory, db_param)
+    db_host = dilib.GlobalInput(type_=str, default="some-db-addr")
+    foo_factory = dilib.Singleton(FooFactory, db_host=db_host, alpha=1, beta=2)
     foo_client = dilib.Singleton(FooClient, foo_factory=foo_factory)
 ```
```

### Comparing `dilib-0.4.2/README.md` & `dilib-0.4.3/dilib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: dilib
+Version: 0.4.3
+Summary: Dependency injection library
+Home-page: https://github.com/ansatzcapital/dilib
+License: Apache License 2.0
+Project-URL: Packaging, https://pypi.org/project/dilib/
+Project-URL: Source, https://github.com/ansatzcapital/dilib
+Project-URL: Tracker, https://github.com/ansatzcapital/dilib/issues
+Keywords: dependency injection, di, inversion of control, ioc, design patterns
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: building
+Provides-Extra: testing
+License-File: LICENSE
+
 # dilib
 
 Dependency injection (DI) library for python
 
 [![PyPI version](https://badge.fury.io/py/dilib.svg)](https://badge.fury.io/py/dilib)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/dilib.svg)](https://pypi.python.org/pypi/dilib/)
 [![GitHub Actions (Tests)](https://github.com/ansatzcapital/dilib/workflows/Test/badge.svg)](https://github.com/ansatzcapital/dilib)
@@ -92,26 +121,26 @@
     # Forward spec resolution to the target spec
     engine: Engine = dilib.Forward(engine0)
 
 
 class CarConfig(dilib.Config):
     # Configs depend on other configs via types. 
     # Here, CarConfig depends on EngineConfig.
-    engine_config = EngineConfig(foo_prefix="baz")
+    engine_config = EngineConfig(token_prefix="baz")
 
     car = dilib.Singleton(Car, engine_config.engine)
 
 
 # Get instance of config (with global input value set)
 car_config: CarConfig = dilib.get_config(
   CarConfig, db_addr="some-other-db-addr"
 )
 
 # Perturb here as you'd like. E.g.:
-car_config.engine_config.Engine = dilib.Singleton(MockEngine)
+car_config.engine_config.engine = dilib.Singleton(MockEngine)
 
 # Pass config to a container
 container: dilib.Container[CarConfig] = dilib.get_container(car_config)
 
 # Retrieve objects from container (some of which are cached inside)
 assert container.config.engine_config.db_addr == "some-other-db-addr"
 assert isinstance(container.config.engine_config.engine, MockEngine)
@@ -283,35 +312,43 @@
 ### Factories for Dynamic Objects
 
 If you need to configure objects dynamically 
 (e.g., check db value to resolve what type to use, 
 set config keys based on another value), consider a factory pattern like:
 
 ```python
+import dataclasses
+
 import dilib
 
 
+# Object that needs to be created dynamically
+@dataclasses.dataclass(frozen=True)
 class Foo:
-    @property
-    def value(self) -> int:
-        raise NotImplementedError
+    value: int
 
 
+# Factory that takes static params via constructor injection and dynamic params via method injection
+@dataclasses.dataclass(frozen=True)
 class FooFactory:
-    def get_foo(self) -> Foo:
+    db_host: str
+    alpha: int
+    beta: int
+
+    def get_foo(self, gamma: int) -> Foo:
         raise NotImplementedError
 
 
+# Object that needs Foo object
+@dataclasses.dataclass(frozen=True)
 class FooClient:
-    def __init__(self, foo_factory: FooFactory):
-        self.foo_factory = foo_factory
-        
-    def get_foo_value(self) -> int:
-        foo = self.foo_factory.get_foo()
-        return foo.value
+    foo_factory: FooFactory
+
+    def process_foo_value(self) -> int:
+        return 100 + self.foo_factory.get_foo(gamma=3).value
 
 
 class FooConfig(dilib.Config):
-    db_param = dilib.Object("some-db-addr")
-    foo_factory = dilib.Singleton(FooFactory, db_param)
+    db_host = dilib.GlobalInput(type_=str, default="some-db-addr")
+    foo_factory = dilib.Singleton(FooFactory, db_host=db_host, alpha=1, beta=2)
     foo_client = dilib.Singleton(FooClient, foo_factory=foo_factory)
 ```
```

### Comparing `dilib-0.4.2/dilib/config.py` & `dilib-0.4.3/dilib/config.py`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/dilib/container.py` & `dilib-0.4.3/dilib/container.py`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/dilib/specs.py` & `dilib-0.4.3/dilib/specs.py`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/dilib/tests/test_config.py` & `dilib-0.4.3/dilib/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/dilib/tests/test_container.py` & `dilib-0.4.3/dilib/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/dilib/tests/test_demo.py` & `dilib-0.4.3/dilib/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/dilib/tests/test_specs.py` & `dilib-0.4.3/dilib/tests/test_specs.py`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/dilib/utils.py` & `dilib-0.4.3/dilib/utils.py`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/dilib.egg-info/PKG-INFO` & `dilib-0.4.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: dilib
-Version: 0.4.2
-Summary: Dependency injection library
-Home-page: https://github.com/ansatzcapital/dilib
-License: Apache License 2.0
-Project-URL: Packaging, https://pypi.org/project/dilib/
-Project-URL: Source, https://github.com/ansatzcapital/dilib
-Project-URL: Tracker, https://github.com/ansatzcapital/dilib/issues
-Keywords: dependency injection, di, inversion of control, ioc, design patterns
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: building
-Provides-Extra: testing
-License-File: LICENSE
-
 # dilib
 
 Dependency injection (DI) library for python
 
 [![PyPI version](https://badge.fury.io/py/dilib.svg)](https://badge.fury.io/py/dilib)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/dilib.svg)](https://pypi.python.org/pypi/dilib/)
 [![GitHub Actions (Tests)](https://github.com/ansatzcapital/dilib/workflows/Test/badge.svg)](https://github.com/ansatzcapital/dilib)
@@ -121,26 +92,26 @@
     # Forward spec resolution to the target spec
     engine: Engine = dilib.Forward(engine0)
 
 
 class CarConfig(dilib.Config):
     # Configs depend on other configs via types. 
     # Here, CarConfig depends on EngineConfig.
-    engine_config = EngineConfig(foo_prefix="baz")
+    engine_config = EngineConfig(token_prefix="baz")
 
     car = dilib.Singleton(Car, engine_config.engine)
 
 
 # Get instance of config (with global input value set)
 car_config: CarConfig = dilib.get_config(
   CarConfig, db_addr="some-other-db-addr"
 )
 
 # Perturb here as you'd like. E.g.:
-car_config.engine_config.Engine = dilib.Singleton(MockEngine)
+car_config.engine_config.engine = dilib.Singleton(MockEngine)
 
 # Pass config to a container
 container: dilib.Container[CarConfig] = dilib.get_container(car_config)
 
 # Retrieve objects from container (some of which are cached inside)
 assert container.config.engine_config.db_addr == "some-other-db-addr"
 assert isinstance(container.config.engine_config.engine, MockEngine)
@@ -312,35 +283,43 @@
 ### Factories for Dynamic Objects
 
 If you need to configure objects dynamically 
 (e.g., check db value to resolve what type to use, 
 set config keys based on another value), consider a factory pattern like:
 
 ```python
+import dataclasses
+
 import dilib
 
 
+# Object that needs to be created dynamically
+@dataclasses.dataclass(frozen=True)
 class Foo:
-    @property
-    def value(self) -> int:
-        raise NotImplementedError
+    value: int
 
 
+# Factory that takes static params via constructor injection and dynamic params via method injection
+@dataclasses.dataclass(frozen=True)
 class FooFactory:
-    def get_foo(self) -> Foo:
+    db_host: str
+    alpha: int
+    beta: int
+
+    def get_foo(self, gamma: int) -> Foo:
         raise NotImplementedError
 
 
+# Object that needs Foo object
+@dataclasses.dataclass(frozen=True)
 class FooClient:
-    def __init__(self, foo_factory: FooFactory):
-        self.foo_factory = foo_factory
-        
-    def get_foo_value(self) -> int:
-        foo = self.foo_factory.get_foo()
-        return foo.value
+    foo_factory: FooFactory
+
+    def process_foo_value(self) -> int:
+        return 100 + self.foo_factory.get_foo(gamma=3).value
 
 
 class FooConfig(dilib.Config):
-    db_param = dilib.Object("some-db-addr")
-    foo_factory = dilib.Singleton(FooFactory, db_param)
+    db_host = dilib.GlobalInput(type_=str, default="some-db-addr")
+    foo_factory = dilib.Singleton(FooFactory, db_host=db_host, alpha=1, beta=2)
     foo_client = dilib.Singleton(FooClient, foo_factory=foo_factory)
 ```
```

### Comparing `dilib-0.4.2/dilib.egg-info/SOURCES.txt` & `dilib-0.4.3/dilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/pyproject.toml` & `dilib-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dilib-0.4.2/setup.cfg` & `dilib-0.4.3/setup.cfg`

 * *Files identical despite different names*

