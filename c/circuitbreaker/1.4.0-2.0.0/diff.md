# Comparing `tmp/circuitbreaker-1.4.0.tar.gz` & `tmp/circuitbreaker-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitbreaker-1.4.0.tar", last modified: Wed Jul 13 05:52:58 2022, max compression
+gzip compressed data, was "circuitbreaker-2.0.0.tar", last modified: Mon May 15 13:10:23 2023, max compression
```

## Comparing `circuitbreaker-1.4.0.tar` & `circuitbreaker-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 fabfuel    (501) staff       (20)        0 2022-07-13 05:52:58.981701 circuitbreaker-1.4.0/
--rw-r--r--   0 fabfuel    (501) staff       (20)     1537 2022-07-13 05:51:43.000000 circuitbreaker-1.4.0/LICENSE.rst
--rw-r--r--   0 fabfuel    (501) staff       (20)       55 2022-01-31 08:31:40.000000 circuitbreaker-1.4.0/MANIFEST.in
--rw-r--r--   0 fabfuel    (501) staff       (20)     7475 2022-07-13 05:52:58.981599 circuitbreaker-1.4.0/PKG-INFO
--rw-r--r--   0 fabfuel    (501) staff       (20)     6766 2022-07-13 05:51:43.000000 circuitbreaker-1.4.0/README.rst
-drwxr-xr-x   0 fabfuel    (501) staff       (20)        0 2022-07-13 05:52:58.981262 circuitbreaker-1.4.0/circuitbreaker.egg-info/
--rw-r--r--   0 fabfuel    (501) staff       (20)     7475 2022-07-13 05:52:58.000000 circuitbreaker-1.4.0/circuitbreaker.egg-info/PKG-INFO
--rw-r--r--   0 fabfuel    (501) staff       (20)      331 2022-07-13 05:52:58.000000 circuitbreaker-1.4.0/circuitbreaker.egg-info/SOURCES.txt
--rw-r--r--   0 fabfuel    (501) staff       (20)        1 2022-07-13 05:52:58.000000 circuitbreaker-1.4.0/circuitbreaker.egg-info/dependency_links.txt
--rw-r--r--   0 fabfuel    (501) staff       (20)        1 2022-01-31 08:32:37.000000 circuitbreaker-1.4.0/circuitbreaker.egg-info/not-zip-safe
--rw-r--r--   0 fabfuel    (501) staff       (20)       71 2022-07-13 05:52:58.000000 circuitbreaker-1.4.0/circuitbreaker.egg-info/requires.txt
--rw-r--r--   0 fabfuel    (501) staff       (20)       15 2022-07-13 05:52:58.000000 circuitbreaker-1.4.0/circuitbreaker.egg-info/top_level.txt
--rw-r--r--   0 fabfuel    (501) staff       (20)    10400 2022-07-13 05:51:43.000000 circuitbreaker-1.4.0/circuitbreaker.py
--rw-r--r--   0 fabfuel    (501) staff       (20)       38 2022-07-13 05:52:58.981733 circuitbreaker-1.4.0/setup.cfg
--rw-r--r--   0 fabfuel    (501) staff       (20)     1112 2022-07-13 05:51:43.000000 circuitbreaker-1.4.0/setup.py
-drwxr-xr-x   0 fabfuel    (501) staff       (20)        0 2022-07-13 05:52:58.981469 circuitbreaker-1.4.0/tests/
--rw-r--r--   0 fabfuel    (501) staff       (20)     7707 2022-07-13 05:51:43.000000 circuitbreaker-1.4.0/tests/test_functional.py
--rw-r--r--   0 fabfuel    (501) staff       (20)     6440 2022-07-13 05:51:43.000000 circuitbreaker-1.4.0/tests/test_unit.py
+drwxr-xr-x   0 fabfuel    (501) staff       (20)        0 2023-05-15 13:10:23.058392 circuitbreaker-2.0.0/
+-rw-r--r--   0 fabfuel    (501) staff       (20)     1537 2022-07-13 05:51:43.000000 circuitbreaker-2.0.0/LICENSE.rst
+-rw-r--r--   0 fabfuel    (501) staff       (20)       55 2022-01-31 08:31:40.000000 circuitbreaker-2.0.0/MANIFEST.in
+-rw-r--r--   0 fabfuel    (501) staff       (20)     7713 2023-05-15 13:10:23.058276 circuitbreaker-2.0.0/PKG-INFO
+-rw-r--r--   0 fabfuel    (501) staff       (20)     7052 2023-05-15 13:01:12.000000 circuitbreaker-2.0.0/README.rst
+drwxr-xr-x   0 fabfuel    (501) staff       (20)        0 2023-05-15 13:10:23.057826 circuitbreaker-2.0.0/circuitbreaker.egg-info/
+-rw-r--r--   0 fabfuel    (501) staff       (20)     7713 2023-05-15 13:10:23.000000 circuitbreaker-2.0.0/circuitbreaker.egg-info/PKG-INFO
+-rw-r--r--   0 fabfuel    (501) staff       (20)      312 2023-05-15 13:10:23.000000 circuitbreaker-2.0.0/circuitbreaker.egg-info/SOURCES.txt
+-rw-r--r--   0 fabfuel    (501) staff       (20)        1 2023-05-15 13:10:23.000000 circuitbreaker-2.0.0/circuitbreaker.egg-info/dependency_links.txt
+-rw-r--r--   0 fabfuel    (501) staff       (20)        1 2023-05-15 13:10:23.000000 circuitbreaker-2.0.0/circuitbreaker.egg-info/not-zip-safe
+-rw-r--r--   0 fabfuel    (501) staff       (20)       15 2023-05-15 13:10:23.000000 circuitbreaker-2.0.0/circuitbreaker.egg-info/top_level.txt
+-rw-r--r--   0 fabfuel    (501) staff       (20)    12083 2023-05-15 13:01:12.000000 circuitbreaker-2.0.0/circuitbreaker.py
+-rw-r--r--   0 fabfuel    (501) staff       (20)       38 2023-05-15 13:10:23.058429 circuitbreaker-2.0.0/setup.cfg
+-rw-r--r--   0 fabfuel    (501) staff       (20)      992 2023-05-15 13:10:06.000000 circuitbreaker-2.0.0/setup.py
+drwxr-xr-x   0 fabfuel    (501) staff       (20)        0 2023-05-15 13:10:23.058128 circuitbreaker-2.0.0/tests/
+-rw-r--r--   0 fabfuel    (501) staff       (20)     3650 2023-05-15 13:01:12.000000 circuitbreaker-2.0.0/tests/conftest.py
+-rw-r--r--   0 fabfuel    (501) staff       (20)     7936 2023-05-15 13:01:12.000000 circuitbreaker-2.0.0/tests/test_functional.py
+-rw-r--r--   0 fabfuel    (501) staff       (20)     7819 2023-05-15 13:01:12.000000 circuitbreaker-2.0.0/tests/test_unit.py
```

### Comparing `circuitbreaker-1.4.0/LICENSE.rst` & `circuitbreaker-2.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `circuitbreaker-1.4.0/PKG-INFO` & `circuitbreaker-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: circuitbreaker
-Version: 1.4.0
+Version: 2.0.0
 Summary: Python Circuit Breaker pattern implementation
 Home-page: https://github.com/fabfuel/circuitbreaker
 Author: Fabian Fuelling
 Author-email: pypi@fabfuel.de
 License: BSD-3-Clause
-Download-URL: https://github.com/fabfuel/circuitbreaker/archive/1.3.1.tar.gz
+Download-URL: https://github.com/fabfuel/circuitbreaker/archive/2.0.0.tar.gz
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.rst
 
 CircuitBreaker
 --------------
 
 .. image:: https://badge.fury.io/py/circuitbreaker.svg
@@ -46,14 +45,19 @@
 
     from circuitbreaker import circuit
 
     @circuit
     def external_call():
         ...
 
+Async functions are also supported::
+
+    @circuit
+    async def external_call():
+        ...
 
 This decorator sets up a circuit breaker with the default settings. The circuit breaker:
 
 - monitors the function execution and counts failures
 - resets the failure count after every successful execution (while it is closed)
 - opens and prevents further executions after 5 subsequent failures
 - switches to half-open and allows one test-execution after 30 seconds recovery timeout
@@ -145,14 +149,17 @@
 
 fallback function
 =================
 By default, the circuit breaker will raise a ``CircuitBreaker`` exception when the circuit is opened.
 You can instead specify a function to be called when the circuit is opened. This function can be specified with the
 ``fallback_function`` parameter and will be called with the same parameters as the decorated function would be.
 
+The fallback type of call must also match the decorated function. For instance, if the decorated function is an
+async generator, the ``fallback_function`` must be an async generator as well.
+
 Advanced Usage
 --------------
 If you apply circuit breakers to a couple of functions and you always set specific options other than the default values,
 you can extend the ``CircuitBreaker`` class and create your own circuit breaker subclass instead::
 
     from circuitbreaker import CircuitBreaker
```

### Comparing `circuitbreaker-1.4.0/README.rst` & `circuitbreaker-2.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 
     from circuitbreaker import circuit
 
     @circuit
     def external_call():
         ...
 
+Async functions are also supported::
+
+    @circuit
+    async def external_call():
+        ...
 
 This decorator sets up a circuit breaker with the default settings. The circuit breaker:
 
 - monitors the function execution and counts failures
 - resets the failure count after every successful execution (while it is closed)
 - opens and prevents further executions after 5 subsequent failures
 - switches to half-open and allows one test-execution after 30 seconds recovery timeout
@@ -125,14 +130,17 @@
 
 fallback function
 =================
 By default, the circuit breaker will raise a ``CircuitBreaker`` exception when the circuit is opened.
 You can instead specify a function to be called when the circuit is opened. This function can be specified with the
 ``fallback_function`` parameter and will be called with the same parameters as the decorated function would be.
 
+The fallback type of call must also match the decorated function. For instance, if the decorated function is an
+async generator, the ``fallback_function`` must be an async generator as well.
+
 Advanced Usage
 --------------
 If you apply circuit breakers to a couple of functions and you always set specific options other than the default values,
 you can extend the ``CircuitBreaker`` class and create your own circuit breaker subclass instead::
 
     from circuitbreaker import CircuitBreaker
```

### Comparing `circuitbreaker-1.4.0/circuitbreaker.egg-info/PKG-INFO` & `circuitbreaker-2.0.0/circuitbreaker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: circuitbreaker
-Version: 1.4.0
+Version: 2.0.0
 Summary: Python Circuit Breaker pattern implementation
 Home-page: https://github.com/fabfuel/circuitbreaker
 Author: Fabian Fuelling
 Author-email: pypi@fabfuel.de
 License: BSD-3-Clause
-Download-URL: https://github.com/fabfuel/circuitbreaker/archive/1.3.1.tar.gz
+Download-URL: https://github.com/fabfuel/circuitbreaker/archive/2.0.0.tar.gz
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.rst
 
 CircuitBreaker
 --------------
 
 .. image:: https://badge.fury.io/py/circuitbreaker.svg
@@ -46,14 +45,19 @@
 
     from circuitbreaker import circuit
 
     @circuit
     def external_call():
         ...
 
+Async functions are also supported::
+
+    @circuit
+    async def external_call():
+        ...
 
 This decorator sets up a circuit breaker with the default settings. The circuit breaker:
 
 - monitors the function execution and counts failures
 - resets the failure count after every successful execution (while it is closed)
 - opens and prevents further executions after 5 subsequent failures
 - switches to half-open and allows one test-execution after 30 seconds recovery timeout
@@ -145,14 +149,17 @@
 
 fallback function
 =================
 By default, the circuit breaker will raise a ``CircuitBreaker`` exception when the circuit is opened.
 You can instead specify a function to be called when the circuit is opened. This function can be specified with the
 ``fallback_function`` parameter and will be called with the same parameters as the decorated function would be.
 
+The fallback type of call must also match the decorated function. For instance, if the decorated function is an
+async generator, the ``fallback_function`` must be an async generator as well.
+
 Advanced Usage
 --------------
 If you apply circuit breakers to a couple of functions and you always set specific options other than the default values,
 you can extend the ``CircuitBreaker`` class and create your own circuit breaker subclass instead::
 
     from circuitbreaker import CircuitBreaker
```

### Comparing `circuitbreaker-1.4.0/circuitbreaker.py` & `circuitbreaker-2.0.0/circuitbreaker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,16 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
-from __future__ import division
-from __future__ import print_function
-from __future__ import absolute_import
-
-from functools import wraps
+from asyncio import iscoroutinefunction
 from datetime import datetime, timedelta
-from inspect import isgeneratorfunction, isclass
-from typing import AnyStr, Iterable
+from functools import wraps
+from inspect import isgeneratorfunction, isasyncgenfunction, isclass
 from math import ceil, floor
+from time import monotonic
+from typing import AnyStr, Iterable
 
-try:
-    from time import monotonic
-except ImportError:
-    from monotonic import monotonic
-
-# Python2 vs Python3 strings
-try:
-    STRING_TYPES = (basestring,)
-except NameError:
-    STRING_TYPES = (bytes, str)
-
+STRING_TYPES = (bytes, str)
 STATE_CLOSED = 'closed'
 STATE_OPEN = 'open'
 STATE_HALF_OPEN = 'half_open'
 
 
 def in_exception_list(*exc_types):
     """Build a predicate function that checks if an exception is a subtype from a list"""
@@ -141,28 +127,60 @@
             try:
                 self._name = function.__qualname__
             except AttributeError:
                 self._name = function.__name__
 
         CircuitBreakerMonitor.register(self)
 
-        if isgeneratorfunction(function):
-            call = self.call_generator
-        else:
-            call = self.call
+        if iscoroutinefunction(function) or isasyncgenfunction(function):
+            return self._decorate_async(function)
 
+        return self._decorate_sync(function)
+
+    def _decorate_sync(self, function):
         @wraps(function)
         def wrapper(*args, **kwargs):
             if self.opened:
                 if self.fallback_function:
                     return self.fallback_function(*args, **kwargs)
                 raise CircuitBreakerError(self)
-            return call(function, *args, **kwargs)
+            return self.call(function, *args, **kwargs)
+
+        @wraps(function)
+        def gen_wrapper(*args, **kwargs):
+            if self.opened:
+                if self.fallback_function:
+                    yield from self.fallback_function(*args, **kwargs)
+                    return
+                raise CircuitBreakerError(self)
+            yield from self.call_generator(function, *args, **kwargs)
+
+        return gen_wrapper if isgeneratorfunction(function) else wrapper
+
+    def _decorate_async(self, function):
+        @wraps(function)
+        async def awrapper(*args, **kwargs):
+            if self.opened:
+                if self.fallback_function:
+                    return await self.fallback_function(*args, **kwargs)
+                raise CircuitBreakerError(self)
+            return await self.call_async(function, *args, **kwargs)
 
-        return wrapper
+        @wraps(function)
+        async def gen_awrapper(*args, **kwargs):
+            if self.opened:
+                if self.fallback_function:
+                    async for el in self.fallback_function(*args, **kwargs):
+                        yield el
+                    return
+                raise CircuitBreakerError(self)
+            async for el in self.call_async_generator(function, *args, **kwargs):
+                yield el
+
+        return gen_awrapper if isasyncgenfunction(function) else awrapper
 
     def call(self, func, *args, **kwargs):
         """
         Calls the decorated function and applies the circuit breaker
         rules on success or failure
         :param func: Decorated function
         """
@@ -175,14 +193,33 @@
         rules on success or failure
         :param func: Decorated generator function
         """
         with self:
             for el in func(*args, **kwargs):
                 yield el
 
+    async def call_async(self, func, *args, **kwargs):
+        """
+        Calls the decorated async function and applies the circuit breaker
+        rules on success or failure
+        :param func: Decorated async function
+        """
+        with self:
+            return await func(*args, **kwargs)
+
+    async def call_async_generator(self, func, *args, **kwargs):
+        """
+        Calls the decorated async generator function and applies the circuit breaker
+        rules on success or failure
+        :param func: Decorated async generator function
+        """
+        with self:
+            async for el in func(*args, **kwargs):
+                yield el
+
     def __call_succeeded(self):
         """
         Close circuit after successful execution and reset failure count
         """
         self._state = STATE_CLOSED
         self._last_failure = None
         self._failure_count = 0
@@ -272,38 +309,33 @@
     circuit_breakers = {}
 
     @classmethod
     def register(cls, circuit_breaker):
         cls.circuit_breakers[circuit_breaker.name] = circuit_breaker
 
     @classmethod
-    def all_closed(cls):
-        # type: () -> bool
+    def all_closed(cls) -> bool:
         return len(list(cls.get_open())) == 0
 
     @classmethod
-    def get_circuits(cls):
-        # type: () -> Iterable[CircuitBreaker]
+    def get_circuits(cls) -> Iterable[CircuitBreaker]:
         return cls.circuit_breakers.values()
 
     @classmethod
-    def get(cls, name):
-        # type: (AnyStr) -> CircuitBreaker
+    def get(cls, name: AnyStr) -> CircuitBreaker:
         return cls.circuit_breakers.get(name)
 
     @classmethod
-    def get_open(cls):
-        # type: () -> Iterable[CircuitBreaker]
+    def get_open(cls) -> Iterable[CircuitBreaker]:
         for circuit in cls.get_circuits():
             if circuit.opened:
                 yield circuit
 
     @classmethod
-    def get_closed(cls):
-        # type: () -> Iterable[CircuitBreaker]
+    def get_closed(cls) -> Iterable[CircuitBreaker]:
         for circuit in cls.get_circuits():
             if circuit.closed:
                 yield circuit
 
 
 def circuit(failure_threshold=None,
             recovery_timeout=None,
```

### Comparing `circuitbreaker-1.4.0/setup.py` & `circuitbreaker-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,35 +5,32 @@
 
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 
-dependencies = ["typing; python_version < '3.5'", "monotonic; python_version < '3.0'"]
-
 setup(
     name='circuitbreaker',
-    version='1.4.0',
+    version='2.0.0',
     url='https://github.com/fabfuel/circuitbreaker',
-    download_url='https://github.com/fabfuel/circuitbreaker/archive/1.3.1.tar.gz',
+    download_url='https://github.com/fabfuel/circuitbreaker/archive/2.0.0.tar.gz',
     license='BSD-3-Clause',
     author='Fabian Fuelling',
     author_email='pypi@fabfuel.de',
     description='Python Circuit Breaker pattern implementation',
     long_description=readme(),
     py_modules=['circuitbreaker'],
     include_package_data=True,
     zip_safe=False,
     platforms='any',
-    install_requires=dependencies,
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: POSIX',
         'Operating System :: MacOS',
         'Operating System :: Unix',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
-    ]
+    ],
+    options={'bdist_wheel': {'universal': True}}
 )
```

### Comparing `circuitbreaker-1.4.0/tests/test_functional.py` & `circuitbreaker-2.0.0/tests/test_functional.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,248 +1,244 @@
-from time import sleep
+import pytest
 
-try:
-    from unittest.mock import Mock, patch
-except ImportError:
-    from mock import Mock, patch
-
-from pytest import raises
-
-from circuitbreaker import CircuitBreaker, CircuitBreakerError, \
-    CircuitBreakerMonitor, STATE_CLOSED, STATE_HALF_OPEN, STATE_OPEN
-
-
-def pseudo_remote_call():
-    return True
-
-
-@CircuitBreaker()
-def circuit_success():
-    return pseudo_remote_call()
-
-
-@CircuitBreaker(failure_threshold=1, name="circuit_failure")
-def circuit_failure():
-    raise IOError()
-
-
-@CircuitBreaker(failure_threshold=1, name="circuit_generator_failure")
-def circuit_generator_failure():
-    pseudo_remote_call()
-    yield 1
-    raise IOError()
-
-
-@CircuitBreaker(failure_threshold=1, name="threshold_1")
-def circuit_threshold_1():
-    return pseudo_remote_call()
-
-
-@CircuitBreaker(failure_threshold=2, recovery_timeout=1, name="threshold_2")
-def circuit_threshold_2_timeout_1():
-    return pseudo_remote_call()
-
-
-@CircuitBreaker(failure_threshold=3, recovery_timeout=1, name="threshold_3")
-def circuit_threshold_3_timeout_1():
-    return pseudo_remote_call()
-
-
-def test_circuit_pass_through():
-    assert circuit_success() is True
-
-
-def test_circuitbreaker_monitor():
+from circuitbreaker import (
+    CircuitBreaker,
+    CircuitBreakerError,
+    CircuitBreakerMonitor,
+    STATE_CLOSED,
+    STATE_HALF_OPEN,
+    STATE_OPEN,
+)
+
+
+@pytest.fixture
+def circuit_success(function):
+    return CircuitBreaker()(function)
+
+
+@pytest.fixture
+def circuit_failure(function, function_call_error):
+    return CircuitBreaker(
+        failure_threshold=1,
+        name="circuit_failure",
+    )(function)
+
+
+@pytest.fixture
+def circuit_threshold_1(function):
+    return CircuitBreaker(
+        failure_threshold=1,
+        name="threshold_1",
+    )(function)
+
+
+@pytest.fixture
+def circuit_threshold_2_timeout_1(function):
+    return CircuitBreaker(
+        failure_threshold=2,
+        recovery_timeout=1,
+        name="threshold_2",
+    )(function)
+
+
+@pytest.fixture
+def circuit_threshold_3_timeout_1(function):
+    return CircuitBreaker(
+        failure_threshold=3,
+        recovery_timeout=1,
+        name="threshold_3",
+    )(function)
+
+
+async def test_circuit_pass_through(
+    resolve_call, circuit_success, function_call_return_value
+):
+    assert await resolve_call(circuit_success()) == function_call_return_value
+
+
+@pytest.mark.usefixtures(
+    "circuit_success",
+    "circuit_failure",
+    "circuit_threshold_1",
+    "circuit_threshold_2_timeout_1",
+    "circuit_threshold_3_timeout_1",
+)
+async def test_circuitbreaker_monitor(
+    resolve_call, circuit_failure, function_call_error
+):
     assert CircuitBreakerMonitor.all_closed() is True
-    assert len(list(CircuitBreakerMonitor.get_circuits())) == 6
-    assert len(list(CircuitBreakerMonitor.get_closed())) == 6
+    assert len(list(CircuitBreakerMonitor.get_circuits())) == 5
+    assert len(list(CircuitBreakerMonitor.get_closed())) == 5
     assert len(list(CircuitBreakerMonitor.get_open())) == 0
 
-    with raises(IOError):
-        circuit_failure()
+    with pytest.raises(function_call_error):
+        await resolve_call(circuit_failure())
 
     assert CircuitBreakerMonitor.all_closed() is False
-    assert len(list(CircuitBreakerMonitor.get_circuits())) == 6
-    assert len(list(CircuitBreakerMonitor.get_closed())) == 5
+    assert len(list(CircuitBreakerMonitor.get_circuits())) == 5
+    assert len(list(CircuitBreakerMonitor.get_closed())) == 4
     assert len(list(CircuitBreakerMonitor.get_open())) == 1
 
 
-@patch('test_functional.pseudo_remote_call', return_value=True)
-def test_threshold_hit_prevents_consequent_calls(mock_remote):
-    # type: (Mock) -> None
-    mock_remote.side_effect = IOError('Connection refused')
+async def test_threshold_hit_prevents_consequent_calls(
+    resolve_call, mock_function_call, circuit_threshold_1, function_call_error
+):
     circuitbreaker = CircuitBreakerMonitor.get('threshold_1')
 
     assert circuitbreaker.closed
 
-    with raises(IOError):
-        circuit_threshold_1()
+    with pytest.raises(function_call_error):
+        await resolve_call(circuit_threshold_1())
 
     assert circuitbreaker.opened
 
-    with raises(CircuitBreakerError):
-        circuit_threshold_1()
+    with pytest.raises(CircuitBreakerError):
+        await resolve_call(circuit_threshold_1())
 
-    mock_remote.assert_called_once_with()
+    mock_function_call.assert_called_once_with()
 
 
-@patch('test_functional.pseudo_remote_call', return_value=True)
-def test_circuitbreaker_recover_half_open(mock_remote):
-    # type: (Mock) -> None
+async def test_circuitbreaker_recover_half_open(
+    resolve_call, mock_function_call, circuit_threshold_3_timeout_1, sleep
+):
     circuitbreaker = CircuitBreakerMonitor.get('threshold_3')
 
     # initial state: closed
     assert circuitbreaker.closed
     assert circuitbreaker.state == STATE_CLOSED
 
     # no exception -> success
-    assert circuit_threshold_3_timeout_1()
+    assert await resolve_call(circuit_threshold_3_timeout_1())
 
     # from now all subsequent calls will fail
-    mock_remote.side_effect = IOError('Connection refused')
+    mock_function_call.side_effect = IOError('Connection refused')
 
     # 1. failed call -> original exception
-    with raises(IOError):
-        circuit_threshold_3_timeout_1()
+    with pytest.raises(IOError):
+        assert await resolve_call(circuit_threshold_3_timeout_1())
+
     assert circuitbreaker.closed
     assert circuitbreaker.failure_count == 1
 
     # 2. failed call -> original exception
-    with raises(IOError):
-        circuit_threshold_3_timeout_1()
+    with pytest.raises(IOError):
+        assert await resolve_call(circuit_threshold_3_timeout_1())
     assert circuitbreaker.closed
     assert circuitbreaker.failure_count == 2
 
     # 3. failed call -> original exception
-    with raises(IOError):
-        circuit_threshold_3_timeout_1()
+    with pytest.raises(IOError):
+        assert await resolve_call(circuit_threshold_3_timeout_1())
 
     # Circuit breaker opens, threshold has been reached
     assert circuitbreaker.opened
     assert circuitbreaker.state == STATE_OPEN
     assert circuitbreaker.failure_count == 3
     assert 0 < circuitbreaker.open_remaining <= 1
 
     # 4. failed call -> not passed to function -> CircuitBreakerError
-    with raises(CircuitBreakerError):
-        circuit_threshold_3_timeout_1()
+    with pytest.raises(CircuitBreakerError):
+        assert await resolve_call(circuit_threshold_3_timeout_1())
     assert circuitbreaker.opened
     assert circuitbreaker.failure_count == 3
     assert 0 < circuitbreaker.open_remaining <= 1
 
     # 5. failed call -> not passed to function -> CircuitBreakerError
-    with raises(CircuitBreakerError):
-        circuit_threshold_3_timeout_1()
+    with pytest.raises(CircuitBreakerError):
+        assert await resolve_call(circuit_threshold_3_timeout_1())
     assert circuitbreaker.opened
     assert circuitbreaker.failure_count == 3
     assert 0 < circuitbreaker.open_remaining <= 1
 
     # wait for 1 second (recover timeout)
-    sleep(1)
+    await sleep(1)
 
     # circuit half-open -> next call will be passed through
     assert not circuitbreaker.closed
     assert circuitbreaker.open_remaining < 0
     assert circuitbreaker.state == STATE_HALF_OPEN
 
     # State half-open -> function is executed -> original exception
-    with raises(IOError):
-        circuit_threshold_3_timeout_1()
+    with pytest.raises(IOError):
+        assert await resolve_call(circuit_threshold_3_timeout_1())
     assert circuitbreaker.opened
     assert circuitbreaker.failure_count == 4
     assert 0 < circuitbreaker.open_remaining <= 1
 
     # State open > not passed to function -> CircuitBreakerError
-    with raises(CircuitBreakerError):
-        circuit_threshold_3_timeout_1()
+    with pytest.raises(CircuitBreakerError):
+        assert await resolve_call(circuit_threshold_3_timeout_1())
 
 
-@patch('test_functional.pseudo_remote_call', return_value=True)
-def test_circuitbreaker_reopens_after_successful_calls(mock_remote):
-    # type: (Mock) -> None
+async def test_circuitbreaker_reopens_after_successful_calls(
+    resolve_call, mock_function_call, circuit_threshold_2_timeout_1, sleep
+):
     circuitbreaker = CircuitBreakerMonitor.get('threshold_2')
 
     assert str(circuitbreaker) == 'threshold_2'
 
     # initial state: closed
     assert circuitbreaker.closed
     assert circuitbreaker.state == STATE_CLOSED
     assert circuitbreaker.failure_count == 0
 
     # successful call -> no exception
-    assert circuit_threshold_2_timeout_1()
+    assert await resolve_call(circuit_threshold_2_timeout_1())
 
     # from now all subsequent calls will fail
-    mock_remote.side_effect = IOError('Connection refused')
+    mock_function_call.side_effect = IOError('Connection refused')
 
     # 1. failed call -> original exception
-    with raises(IOError):
-        circuit_threshold_2_timeout_1()
+    with pytest.raises(IOError):
+        await resolve_call(circuit_threshold_2_timeout_1())
     assert circuitbreaker.closed
     assert circuitbreaker.failure_count == 1
 
     # 2. failed call -> original exception
-    with raises(IOError):
-        circuit_threshold_2_timeout_1()
+    with pytest.raises(IOError):
+        await resolve_call(circuit_threshold_2_timeout_1())
 
     # Circuit breaker opens, threshold has been reached
     assert circuitbreaker.opened
     assert circuitbreaker.state == STATE_OPEN
     assert circuitbreaker.failure_count == 2
     assert 0 < circuitbreaker.open_remaining <= 1
 
     # 4. failed call -> not passed to function -> CircuitBreakerError
-    with raises(CircuitBreakerError):
-        circuit_threshold_2_timeout_1()
+    with pytest.raises(CircuitBreakerError):
+        await resolve_call(circuit_threshold_2_timeout_1())
     assert circuitbreaker.opened
     assert circuitbreaker.failure_count == 2
     assert 0 < circuitbreaker.open_remaining <= 1
 
     # from now all subsequent calls will succeed
-    mock_remote.side_effect = None
+    mock_function_call.side_effect = None
 
     # but recover timeout has not been reached -> still open
     # 5. failed call -> not passed to function -> CircuitBreakerError
-    with raises(CircuitBreakerError):
-        circuit_threshold_2_timeout_1()
+    with pytest.raises(CircuitBreakerError):
+        await resolve_call(circuit_threshold_2_timeout_1())
     assert circuitbreaker.opened
     assert circuitbreaker.failure_count == 2
     assert 0 < circuitbreaker.open_remaining <= 1
 
     # wait for 1 second (recover timeout)
-    sleep(1)
+    await sleep(1)
 
     # circuit half-open -> next call will be passed through
     assert not circuitbreaker.closed
     assert circuitbreaker.failure_count == 2
     assert circuitbreaker.open_remaining < 0
     assert circuitbreaker.state == STATE_HALF_OPEN
 
     # successful call
-    assert circuit_threshold_2_timeout_1()
+    assert await resolve_call(circuit_threshold_2_timeout_1())
 
     # circuit closed and reset'ed
     assert circuitbreaker.closed
     assert circuitbreaker.state == STATE_CLOSED
     assert circuitbreaker.failure_count == 0
 
     # some another successful calls
-    assert circuit_threshold_2_timeout_1()
-    assert circuit_threshold_2_timeout_1()
-    assert circuit_threshold_2_timeout_1()
-
-
-@patch("test_functional.pseudo_remote_call", return_value=True)
-def test_circuitbreaker_handles_generator_functions(mock_remote):
-    # type: (Mock) -> None
-    circuitbreaker = CircuitBreakerMonitor.get("circuit_generator_failure")
-    assert circuitbreaker.closed
-
-    with raises(IOError):
-        list(circuit_generator_failure())
-
-    assert circuitbreaker.opened
-
-    with raises(CircuitBreakerError):
-        list(circuit_generator_failure())
-
-    mock_remote.assert_called_once_with()
+    assert await resolve_call(circuit_threshold_2_timeout_1())
+    assert await resolve_call(circuit_threshold_2_timeout_1())
+    assert await resolve_call(circuit_threshold_2_timeout_1())
```

### Comparing `circuitbreaker-1.4.0/tests/test_unit.py` & `circuitbreaker-2.0.0/tests/test_unit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,29 @@
-try:
-    from unittest.mock import Mock, patch
-except ImportError:
-    from mock import Mock, patch
+from asyncio import iscoroutinefunction
+from inspect import isgeneratorfunction, isasyncgenfunction
 
-from pytest import raises
+import pytest
 
 from circuitbreaker import CircuitBreaker, CircuitBreakerError, circuit
 
 
+@pytest.fixture
+def resolve_circuitbreaker_call_method(function_type):
+    def cb_call(circuit_breaker):
+        mapping = {
+            "sync-function": circuit_breaker.call,
+            "sync-generator": circuit_breaker.call_generator,
+            "async-function": circuit_breaker.call_async,
+            "async-generator": circuit_breaker.call_async_generator,
+        }
+        return mapping[function_type]
+
+    return cb_call
+
+
 class FooError(Exception):
     def __init__(self, val=None):
         self.val = val
 
 
 class BarError(Exception):
     pass
@@ -27,90 +39,100 @@
     cb._last_failure = Exception()
     error = CircuitBreakerError(cb)
 
     assert str(error).startswith('Circuit "Foobar" OPEN until ')
     assert str(error).endswith('(0 failures, 30 sec remaining) (last_failure: Exception())')
 
 
-def test_circuitbreaker_should_save_last_exception_on_failure_call():
+async def test_circuitbreaker_wrapper_matches_function_type(function, is_async, is_generator):
     cb = CircuitBreaker(name='Foobar')
+    wrapper = cb(function)
 
-    func = Mock(side_effect=IOError)
+    assert (
+        isgeneratorfunction(function) == isgeneratorfunction(wrapper)
+        == (not is_async and is_generator)
+    )
+    assert (
+        iscoroutinefunction(function) == iscoroutinefunction(wrapper)
+        == (is_async and not is_generator)
+    )
+    assert (
+        isasyncgenfunction(function) == isasyncgenfunction(wrapper)
+        == (is_async and is_generator)
+    )
+
+
+async def test_circuitbreaker_should_save_last_exception_on_failure_call(
+    resolve_call, resolve_circuitbreaker_call_method, function, function_call_error
+):
+    cb = CircuitBreaker(name='Foobar')
 
-    with raises(IOError):
-        cb.call(func)
+    cb_call = resolve_circuitbreaker_call_method(cb)
+    with pytest.raises(function_call_error):
+        await resolve_call(cb_call(function))
 
-    assert isinstance(cb.last_failure, IOError)
+    assert isinstance(cb.last_failure, function_call_error)
 
 
-def test_circuitbreaker_should_clear_last_exception_on_success_call():
+async def test_circuitbreaker_should_clear_last_exception_on_success_call(
+    resolve_call, resolve_circuitbreaker_call_method, function
+):
     cb = CircuitBreaker(name='Foobar')
     cb._last_failure = IOError()
     assert isinstance(cb.last_failure, IOError)
 
-    cb.call(lambda: True)
+    cb_call = resolve_circuitbreaker_call_method(cb)
+    await resolve_call(cb_call(function))
 
     assert cb.last_failure is None
 
 
-def test_circuitbreaker_should_call_fallback_function_if_open():
-    fallback = Mock(return_value=True)
-
-    func = Mock(return_value=False, __name__="Mock")  # attribute __name__ required for 2.7 compat with functools.wraps
-
+async def test_circuitbreaker_should_call_fallback_function_if_open(
+    resolve_call, function, fallback_function, mock_fallback_call, fallback_call_return_value
+):
     CircuitBreaker.opened = lambda self: True
 
-    cb = CircuitBreaker(name='WithFallback', fallback_function=fallback)
-    decorated_func = cb.decorate(func)
-
-    decorated_func()
-    fallback.assert_called_once_with()
+    cb = CircuitBreaker(name='WithFallback', fallback_function=fallback_function)
+    decorated_func = cb.decorate(function)
 
+    assert await resolve_call(decorated_func()) == fallback_call_return_value
+    mock_fallback_call.assert_called_once_with()
 
-def test_circuitbreaker_should_not_call_function_if_open():
-    fallback = Mock(return_value=True)
-
-    func = Mock(return_value=False, __name__="Mock")  # attribute __name__ required for 2.7 compat with functools.wraps
 
+async def test_circuitbreaker_should_not_call_function_if_open(
+    resolve_call, function, mock_function_call, fallback_function, fallback_call_return_value
+):
     CircuitBreaker.opened = lambda self: True
 
-    cb = CircuitBreaker(name='WithFallback', fallback_function=fallback)
-    decorated_func = cb.decorate(func)
+    cb = CircuitBreaker(name='WithFallback', fallback_function=fallback_function)
+    decorated_func = cb.decorate(function)
 
-    assert decorated_func() == fallback.return_value
-    assert not func.called
+    assert await resolve_call(decorated_func()) == fallback_call_return_value
+    assert not mock_function_call.called
 
 
-def mocked_function(*args, **kwargs):
-    pass
-
-
-def test_circuitbreaker_call_fallback_function_with_parameters():
-    fallback = Mock(return_value=True)
-
-    cb = circuit(name='with_fallback', fallback_function=fallback)
-
+async def test_circuitbreaker_call_fallback_function_with_parameters(
+    resolve_call, function, fallback_function, mock_fallback_call, fallback_call_return_value
+):
     # mock opened prop to see if fallback is called with correct parameters.
-    cb.opened = lambda self: True
-    func_decorated = cb.decorate(mocked_function)
-
-    func_decorated('test2', test='test')
+    CircuitBreaker.opened = lambda self: True
 
-    # check args and kwargs are getting correctly to fallback function
+    cb = CircuitBreaker(name='WithFallback', fallback_function=fallback_function)
+    decorated_func = cb.decorate(function)
 
-    fallback.assert_called_once_with('test2', test='test')
+    assert await resolve_call(decorated_func('test2', test='test')) == fallback_call_return_value
 
+    # check args and kwargs are getting correctly to fallback function
+    mock_fallback_call.assert_called_once_with('test2', test='test')
 
-@patch('circuitbreaker.CircuitBreaker.decorate')
-def test_circuit_decorator_without_args(circuitbreaker_mock):
-    def function():
-        return True
 
+def test_circuit_decorator_without_args(mocker, function):
+    decorate_patch = mocker.patch.object(CircuitBreaker, 'decorate')
     circuit(function)
-    circuitbreaker_mock.assert_called_once_with(function)
+    decorate_patch.assert_called_once_with(function)
 
 
 def test_circuit_decorator_with_args():
     def function_fallback():
         return True
 
     breaker = circuit(10, 20, KeyError, 'foobar', function_fallback)
@@ -150,28 +172,28 @@
     breaker = circuit(expected_exception=(FooError, BarError))
     assert breaker.is_failure(FooError, FooError())
     assert breaker.is_failure(BarError, BarError())
     assert not breaker.is_failure(Exception, Exception())
 
 
 def test_constructor_mistake_name_bytes():
-    with raises(ValueError, match="expected_exception cannot be a string *"):
+    with pytest.raises(ValueError, match="expected_exception cannot be a string *"):
         circuit(10, 20, b"foobar")
 
 
 def test_constructor_mistake_name_unicode():
-    with raises(ValueError, match="expected_exception cannot be a string *"):
+    with pytest.raises(ValueError, match="expected_exception cannot be a string *"):
         circuit(10, 20, u"foobar")
 
 
 def test_constructor_mistake_expected_exception():
     class Widget:
         pass
 
-    with raises(ValueError, match="expected_exception does not look like a predicate*"):
+    with pytest.raises(ValueError, match="expected_exception does not look like a predicate*"):
         circuit(10, 20, expected_exception=Widget)
 
 
 def test_advanced_usage_circuitbreaker_subclass():
     class MyCircuitBreaker(CircuitBreaker):
         EXPECTED_EXCEPTION = FooError
```

