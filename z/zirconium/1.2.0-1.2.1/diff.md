# Comparing `tmp/zirconium-1.2.0.tar.gz` & `tmp/zirconium-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zirconium-1.2.0.tar", last modified: Mon May  1 14:53:10 2023, max compression
+gzip compressed data, was "zirconium-1.2.1.tar", last modified: Mon May 15 21:54:15 2023, max compression
```

## Comparing `zirconium-1.2.0.tar` & `zirconium-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.944916 zirconium-1.2.0/
--rw-rw-rw-   0        0        0     1058 2023-04-28 14:59:36.000000 zirconium-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    10353 2023-05-01 14:53:10.944916 zirconium-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     9808 2023-05-01 14:51:42.000000 zirconium-1.2.0/README.md
--rw-rw-rw-   0        0        0       88 2023-04-28 14:59:36.000000 zirconium-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      684 2023-05-01 14:53:10.945940 zirconium-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.916950 zirconium-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.932915 zirconium-1.2.0/src/zirconium/
--rw-rw-rw-   0        0        0      313 2023-05-01 14:48:04.000000 zirconium-1.2.0/src/zirconium/__init__.py
--rw-rw-rw-   0        0        0    22477 2023-05-01 14:36:14.000000 zirconium-1.2.0/src/zirconium/config.py
--rw-rw-rw-   0        0        0     5155 2023-04-28 14:59:36.000000 zirconium-1.2.0/src/zirconium/parsers.py
--rw-rw-rw-   0        0        0     1148 2023-04-28 14:59:36.000000 zirconium-1.2.0/src/zirconium/sproviders.py
--rw-rw-rw-   0        0        0     9581 2023-05-01 14:52:23.000000 zirconium-1.2.0/src/zirconium/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.937960 zirconium-1.2.0/src/zirconium.egg-info/
--rw-rw-rw-   0        0        0    10353 2023-05-01 14:53:10.000000 zirconium-1.2.0/src/zirconium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-05-01 14:53:10.000000 zirconium-1.2.0/src/zirconium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:53:10.000000 zirconium-1.2.0/src/zirconium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 14:53:10.000000 zirconium-1.2.0/src/zirconium.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.942928 zirconium-1.2.0/tests/
--rw-rw-rw-   0        0        0    22343 2023-05-01 14:35:06.000000 zirconium-1.2.0/tests/test_config.py
--rw-rw-rw-   0        0        0    12057 2023-04-28 14:59:36.000000 zirconium-1.2.0/tests/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-05-15 21:54:15.678392 zirconium-1.2.1/
+-rw-rw-rw-   0        0        0     1058 2023-04-28 14:59:36.000000 zirconium-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    11871 2023-05-15 21:54:15.679382 zirconium-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11326 2023-05-15 21:53:38.000000 zirconium-1.2.1/README.md
+-rw-rw-rw-   0        0        0       88 2023-04-28 14:59:36.000000 zirconium-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      684 2023-05-15 21:54:15.680381 zirconium-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 21:54:15.654384 zirconium-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 21:54:15.668381 zirconium-1.2.1/src/zirconium/
+-rw-rw-rw-   0        0        0      331 2023-05-15 21:43:02.000000 zirconium-1.2.1/src/zirconium/__init__.py
+-rw-rw-rw-   0        0        0    23310 2023-05-15 21:51:38.000000 zirconium-1.2.1/src/zirconium/config.py
+-rw-rw-rw-   0        0        0     5155 2023-04-28 14:59:36.000000 zirconium-1.2.1/src/zirconium/parsers.py
+-rw-rw-rw-   0        0        0     1148 2023-04-28 14:59:36.000000 zirconium-1.2.1/src/zirconium/sproviders.py
+-rw-rw-rw-   0        0        0     9581 2023-05-15 21:37:14.000000 zirconium-1.2.1/src/zirconium/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 21:54:15.673381 zirconium-1.2.1/src/zirconium.egg-info/
+-rw-rw-rw-   0        0        0    11871 2023-05-15 21:54:15.000000 zirconium-1.2.1/src/zirconium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-05-15 21:54:15.000000 zirconium-1.2.1/src/zirconium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 21:54:15.000000 zirconium-1.2.1/src/zirconium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 21:54:15.000000 zirconium-1.2.1/src/zirconium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 21:54:15.677381 zirconium-1.2.1/tests/
+-rw-rw-rw-   0        0        0    22993 2023-05-15 21:52:16.000000 zirconium-1.2.1/tests/test_config.py
+-rw-rw-rw-   0        0        0    12057 2023-04-28 14:59:36.000000 zirconium-1.2.1/tests/test_handlers.py
```

### Comparing `zirconium-1.2.0/LICENSE` & `zirconium-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.0/PKG-INFO` & `zirconium-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zirconium
-Version: 1.2.0
+Version: 1.2.1
 Summary: Excellent configuration management for Python
 Home-page: https://github.com/turnbullerin/zirconium
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/zirconium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,17 +192,56 @@
 This should reduce the work you have to do when reloading your configuration (though you may still need to call certain
 methods when the configuration is reloaded).
 
 To call a method on reload, you can add it via `config.on_load(callable)`. If `callable` needs to interact with a 
 different thread or process than the one where `reload_config()` is called, it is your responsibility to manage this
 communication (e.g. use `threading.Event` to notify the thread that the configuration needs to be reloaded).
 
+## Testing classes that use ApplicationConfig
+
+Unit test functions decorated with `autoinject.injector.test_case` can declare configuration using `zirconium.test_with_config(key, val)`
+to declare configuration for testing. For example, this test case should pass:
+
+```python
+from autoinject import injector
+import zirconium as zr 
+import unittest 
+
+class MyTestCase(unittest.TestCase):
+
+  # This is essential since we use autoinject's test_case() to handle the ApplicationConfig fixture
+  @injector.test_case 
+  # Declare a single value
+  @zr.test_with_config(("foo", "bar"), "hello world")
+  # You can repeat the decorator to declare multiple values
+  @zr.test_with_config(("some", "value"), "what")
+  # You can also pass a dict instead of a key, value tuple
+  @zr.test_with_config({
+    "foo": {
+      "bar2": "hello world #2"
+    }
+  })
+  def test_something(self):
+    
+    # As a simple example.
+    @injector.inject 
+    def do_something(cfg: zr.ApplicationConfig = None):
+        self.assertEqual(cfg.as_str(("foo", "bar")), "hello world")
+        self.assertEqual(cfg.as_str(("some", "value")), "what")
+```
+
+Note that this pattern replaces all configuration values with the ones declared in decorators, so previously loaded
+values will not be passed into your test function nor will they be passed between test functions.
 
 ## Change Log
 
+### Version 1.2.1
+- Test cases can now use the fixture `@zirconium.test_with_config(key: t.Iterable, value: t.Any)` to inject test 
+  configuration.
+
 ### Version 1.2.0
 - Added `as_bytes()` which will accept values like `2M` and return the value converted into bytes (e.g. `2097152`. If 
   you really want to use metric prefixes (e.g. `2MB=2000000`), you must pass `allow_metric=True` and then specify your 
   units as `2MB`. Prefixes up to exbibyte (`EiB`) are handled at the moment. You can also specify `B` for bytes or `bit` 
   for a number of bits. If no unit is specified, it uses the  `default_units` parameter, which is `B` by default. All 
   units are case-insensitive.
 - Added `as_timedelta()` which will accept values like `30m` and return `datetime.timedelta(minutes=30)`. Valid units
```

### Comparing `zirconium-1.2.0/README.md` & `zirconium-1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -177,17 +177,56 @@
 This should reduce the work you have to do when reloading your configuration (though you may still need to call certain
 methods when the configuration is reloaded).
 
 To call a method on reload, you can add it via `config.on_load(callable)`. If `callable` needs to interact with a 
 different thread or process than the one where `reload_config()` is called, it is your responsibility to manage this
 communication (e.g. use `threading.Event` to notify the thread that the configuration needs to be reloaded).
 
+## Testing classes that use ApplicationConfig
+
+Unit test functions decorated with `autoinject.injector.test_case` can declare configuration using `zirconium.test_with_config(key, val)`
+to declare configuration for testing. For example, this test case should pass:
+
+```python
+from autoinject import injector
+import zirconium as zr 
+import unittest 
+
+class MyTestCase(unittest.TestCase):
+
+  # This is essential since we use autoinject's test_case() to handle the ApplicationConfig fixture
+  @injector.test_case 
+  # Declare a single value
+  @zr.test_with_config(("foo", "bar"), "hello world")
+  # You can repeat the decorator to declare multiple values
+  @zr.test_with_config(("some", "value"), "what")
+  # You can also pass a dict instead of a key, value tuple
+  @zr.test_with_config({
+    "foo": {
+      "bar2": "hello world #2"
+    }
+  })
+  def test_something(self):
+    
+    # As a simple example.
+    @injector.inject 
+    def do_something(cfg: zr.ApplicationConfig = None):
+        self.assertEqual(cfg.as_str(("foo", "bar")), "hello world")
+        self.assertEqual(cfg.as_str(("some", "value")), "what")
+```
+
+Note that this pattern replaces all configuration values with the ones declared in decorators, so previously loaded
+values will not be passed into your test function nor will they be passed between test functions.
 
 ## Change Log
 
+### Version 1.2.1
+- Test cases can now use the fixture `@zirconium.test_with_config(key: t.Iterable, value: t.Any)` to inject test 
+  configuration.
+
 ### Version 1.2.0
 - Added `as_bytes()` which will accept values like `2M` and return the value converted into bytes (e.g. `2097152`. If 
   you really want to use metric prefixes (e.g. `2MB=2000000`), you must pass `allow_metric=True` and then specify your 
   units as `2MB`. Prefixes up to exbibyte (`EiB`) are handled at the moment. You can also specify `B` for bytes or `bit` 
   for a number of bits. If no unit is specified, it uses the  `default_units` parameter, which is `B` by default. All 
   units are case-insensitive.
 - Added `as_timedelta()` which will accept values like `30m` and return `datetime.timedelta(minutes=30)`. Valid units
```

### Comparing `zirconium-1.2.0/setup.cfg` & `zirconium-1.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 207a 6972 636f 6e69 756d 0d0a 7665   = zirconium..ve
-00000020: 7273 696f 6e20 3d20 312e 322e 300d 0a61  rsion = 1.2.0..a
+00000020: 7273 696f 6e20 3d20 312e 322e 310d 0a61  rsion = 1.2.1..a
 00000030: 7574 686f 7220 3d20 4572 696e 2054 7572  uthor = Erin Tur
 00000040: 6e62 756c 6c0d 0a61 7574 686f 725f 656d  nbull..author_em
 00000050: 6169 6c20 3d20 6572 696e 2e61 2e74 7572  ail = erin.a.tur
 00000060: 6e62 756c 6c40 676d 6169 6c2e 636f 6d0d  nbull@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2045  .description = E
 00000080: 7863 656c 6c65 6e74 2063 6f6e 6669 6775  xcellent configu
 00000090: 7261 7469 6f6e 206d 616e 6167 656d 656e  ration managemen
```

### Comparing `zirconium-1.2.0/src/zirconium/config.py` & `zirconium-1.2.1/src/zirconium/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,7 +502,29 @@
 
     def set_defaults(self, d):
         self._default_config.update(d)
 
     def load_from_dict(self, d):
         self.deep_update(d)
 
+
+def test_with_config(key: t.Union[list, str, set, tuple, dict], value: t.Any = None):
+
+    def _inner(fn):
+        if not hasattr(fn, "_autoinject_fixtures"):
+            fn._autoinject_fixtures = {}
+        if ApplicationConfig not in fn._autoinject_fixtures:
+            def _build_app_config():
+                ac = ApplicationConfig(True)
+                ac.set_defaults(fn._zirconium_test_config)
+                ac.init()
+            fn._autoinject_fixtures[ApplicationConfig] = (None, _build_app_config)
+        if not hasattr(fn, "_zirconium_test_config"):
+            fn._zirconium_test_config = MutableDeepDict()
+        if isinstance(key, dict):
+            fn._zirconium_test_config.update(key)
+        else:
+            fn._zirconium_test_config[key] = value
+
+        return fn
+
+    return _inner
```

### Comparing `zirconium-1.2.0/src/zirconium/parsers.py` & `zirconium-1.2.1/src/zirconium/parsers.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.0/src/zirconium/sproviders.py` & `zirconium-1.2.1/src/zirconium/sproviders.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.0/src/zirconium/utils.py` & `zirconium-1.2.1/src/zirconium/utils.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.0/src/zirconium.egg-info/PKG-INFO` & `zirconium-1.2.1/src/zirconium.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zirconium
-Version: 1.2.0
+Version: 1.2.1
 Summary: Excellent configuration management for Python
 Home-page: https://github.com/turnbullerin/zirconium
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/zirconium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,17 +192,56 @@
 This should reduce the work you have to do when reloading your configuration (though you may still need to call certain
 methods when the configuration is reloaded).
 
 To call a method on reload, you can add it via `config.on_load(callable)`. If `callable` needs to interact with a 
 different thread or process than the one where `reload_config()` is called, it is your responsibility to manage this
 communication (e.g. use `threading.Event` to notify the thread that the configuration needs to be reloaded).
 
+## Testing classes that use ApplicationConfig
+
+Unit test functions decorated with `autoinject.injector.test_case` can declare configuration using `zirconium.test_with_config(key, val)`
+to declare configuration for testing. For example, this test case should pass:
+
+```python
+from autoinject import injector
+import zirconium as zr 
+import unittest 
+
+class MyTestCase(unittest.TestCase):
+
+  # This is essential since we use autoinject's test_case() to handle the ApplicationConfig fixture
+  @injector.test_case 
+  # Declare a single value
+  @zr.test_with_config(("foo", "bar"), "hello world")
+  # You can repeat the decorator to declare multiple values
+  @zr.test_with_config(("some", "value"), "what")
+  # You can also pass a dict instead of a key, value tuple
+  @zr.test_with_config({
+    "foo": {
+      "bar2": "hello world #2"
+    }
+  })
+  def test_something(self):
+    
+    # As a simple example.
+    @injector.inject 
+    def do_something(cfg: zr.ApplicationConfig = None):
+        self.assertEqual(cfg.as_str(("foo", "bar")), "hello world")
+        self.assertEqual(cfg.as_str(("some", "value")), "what")
+```
+
+Note that this pattern replaces all configuration values with the ones declared in decorators, so previously loaded
+values will not be passed into your test function nor will they be passed between test functions.
 
 ## Change Log
 
+### Version 1.2.1
+- Test cases can now use the fixture `@zirconium.test_with_config(key: t.Iterable, value: t.Any)` to inject test 
+  configuration.
+
 ### Version 1.2.0
 - Added `as_bytes()` which will accept values like `2M` and return the value converted into bytes (e.g. `2097152`. If 
   you really want to use metric prefixes (e.g. `2MB=2000000`), you must pass `allow_metric=True` and then specify your 
   units as `2MB`. Prefixes up to exbibyte (`EiB`) are handled at the moment. You can also specify `B` for bytes or `bit` 
   for a number of bits. If no unit is specified, it uses the  `default_units` parameter, which is `B` by default. All 
   units are case-insensitive.
 - Added `as_timedelta()` which will accept values like `30m` and return `datetime.timedelta(minutes=30)`. Valid units
```

### Comparing `zirconium-1.2.0/tests/test_config.py` & `zirconium-1.2.1/tests/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import unittest
 import datetime
 import decimal
 import os
 from pathlib import Path
 
+from autoinject import injector
 import zirconium
 
 
 class TestConfig(unittest.TestCase):
 
+    @injector.test_case()
+    @zirconium.test_with_config(("foo", "bar"), "hello world")
+    @zirconium.test_with_config(("foo", "bar"), "hello world2")
+    @zirconium.test_with_config(("foo", "bar2"), "zoink")
+    @zirconium.test_with_config({"foo": {"bar3": "hello world3"}})
+    def test_test_case(self):
+        @injector.inject
+        def _test_inject(cfg: zirconium.ApplicationConfig = None):
+            self.assertEqual(cfg.get(("foo", "bar")), "hello world")
+            self.assertEqual(cfg.get(("foo", "bar2")), "zoink")
+            self.assertEqual(cfg.get(("foo", "bar3")), "hello world3")
+
     def test_one_file(self):
         path = Path(__file__).parent / "example_configs/basic.yaml"
         config = zirconium.ApplicationConfig(True)
         config.register_file(path)
         config.init()
         self.assertTrue("one" in config)
         self.assertEqual(config["one"], "a")
```

### Comparing `zirconium-1.2.0/tests/test_handlers.py` & `zirconium-1.2.1/tests/test_handlers.py`

 * *Files identical despite different names*

