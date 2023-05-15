# Comparing `tmp/lazi-1.5.52.tar.gz` & `tmp/lazi-1.5.52.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.5.52.tar", max compression
+gzip compressed data, was "lazi-1.5.52.dev1.tar", max compression
```

## Comparing `lazi-1.5.52.tar` & `lazi-1.5.52.dev1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.5.52/LICENSE
--rw-r--r--   0        0        0     1920 2023-05-15 07:55:44.338848 lazi-1.5.52/README.md
--rw-r--r--   0        0        0      197 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.5.52/lazi/conf/auto.py
--rw-r--r--   0        0        0      907 2023-05-15 07:53:29.925087 lazi-1.5.52/lazi/conf/base.py
--rw-r--r--   0        0        0     4738 2023-05-15 07:52:46.768522 lazi-1.5.52/lazi/conf/conf.py
--rw-r--r--   0        0        0       69 2023-05-12 21:13:16.044560 lazi-1.5.52/lazi/conf/test.py
--rw-r--r--   0        0        0      364 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/__init__.py
--rw-r--r--   0        0        0     3351 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/finder.py
--rw-r--r--   0        0        0     2103 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/loader.py
--rw-r--r--   0        0        0     3148 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/module.py
--rw-r--r--   0        0        0     1211 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/spec.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.5.52/lazi/util/__init__.py
--rw-r--r--   0        0        0      248 2023-05-11 20:06:44.097623 lazi-1.5.52/lazi/util/debug.py
--rw-r--r--   0        0        0      174 2023-05-15 07:53:12.940865 lazi-1.5.52/lazi/util/functional.py
--rw-r--r--   0        0        0      618 2023-05-11 20:06:44.097623 lazi-1.5.52/lazi/util/util.py
--rw-r--r--   0        0        0     1555 2023-05-15 07:57:18.012076 lazi-1.5.52/pyproject.toml
--rw-r--r--   0        0        0      912 2023-05-15 07:36:15.807454 lazi-1.5.52/tests/test_django.py
--rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 lazi-1.5.52/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.5.52.dev1/LICENSE
+-rw-r--r--   0        0        0     1917 2023-05-15 07:59:50.478074 lazi-1.5.52.dev1/README.md
+-rw-r--r--   0        0        0      197 2023-05-15 07:36:15.807454 lazi-1.5.52.dev1/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.5.52.dev1/lazi/conf/auto.py
+-rw-r--r--   0        0        0     1001 2023-05-15 08:19:36.197618 lazi-1.5.52.dev1/lazi/conf/base.py
+-rw-r--r--   0        0        0     4738 2023-05-15 07:52:46.768522 lazi-1.5.52.dev1/lazi/conf/conf.py
+-rw-r--r--   0        0        0       69 2023-05-12 21:13:16.044560 lazi-1.5.52.dev1/lazi/conf/test.py
+-rw-r--r--   0        0        0      364 2023-05-15 07:36:15.807454 lazi-1.5.52.dev1/lazi/core/__init__.py
+-rw-r--r--   0        0        0     3346 2023-05-15 08:18:21.464638 lazi-1.5.52.dev1/lazi/core/finder.py
+-rw-r--r--   0        0        0     2156 2023-05-15 08:08:21.460771 lazi-1.5.52.dev1/lazi/core/loader.py
+-rw-r--r--   0        0        0     3160 2023-05-15 08:17:50.592233 lazi-1.5.52.dev1/lazi/core/module.py
+-rw-r--r--   0        0        0     1211 2023-05-15 07:36:15.807454 lazi-1.5.52.dev1/lazi/core/spec.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.5.52.dev1/lazi/util/__init__.py
+-rw-r--r--   0        0        0      248 2023-05-11 20:06:44.097623 lazi-1.5.52.dev1/lazi/util/debug.py
+-rw-r--r--   0        0        0      174 2023-05-15 07:53:12.940865 lazi-1.5.52.dev1/lazi/util/functional.py
+-rw-r--r--   0        0        0      618 2023-05-11 20:06:44.097623 lazi-1.5.52.dev1/lazi/util/util.py
+-rw-r--r--   0        0        0     1560 2023-05-15 08:21:16.622935 lazi-1.5.52.dev1/pyproject.toml
+-rw-r--r--   0        0        0      819 2023-05-15 08:16:54.199494 lazi-1.5.52.dev1/tests/_lazi.py
+-rw-r--r--   0        0        0      912 2023-05-15 07:36:15.807454 lazi-1.5.52.dev1/tests/test_django.py
+-rw-r--r--   0        0        0      662 2023-05-15 08:16:54.195494 lazi-1.5.52.dev1/tests/test_lazi.py
+-rw-r--r--   0        0        0      460 2023-05-14 03:03:35.371181 lazi-1.5.52.dev1/tests/test_requests.py
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 lazi-1.5.52.dev1/PKG-INFO
```

### Comparing `lazi-1.5.52/LICENSE` & `lazi-1.5.52.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52/README.md` & `lazi-1.5.52.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,11 +64,11 @@
 
 It's also possible to manually change the configuration at runtime,
 with the caveat that some variables may have already been used by
 `lazi.core`. To avoid this, configure Lazi before importing it:
 
 ```python
 from lazi.conf import conf
-conf.DEBUG_TRACING = True
+conf.DEBUG_TRACING = 1
 import lazi.auto
 # ...
 ```
```

### Comparing `lazi-1.5.52/lazi/conf/base.py` & `lazi-1.5.52.dev1/lazi/conf/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,12 +5,13 @@
     root="lazi",                        # - Root namespace package name.
 )                                       # See conf.py for more options.
 
 DEBUG_TRACING: int = 0                  # Enable debug traces.
 
 LAZI_AUTO_INSTALL: bool = True          # Automatically install when importing lazi.auto.
 CORE_AUTO_INSTALL: bool = False         # Automatically install when importing lazi.core.
+FORCE_LOAD_MODULE: bool = True          # Immediately call exec_module() on imported modules.
 
 CONF_NO_CACHING: bool | None = None     # Disable caching of conf vars.
 #                                         - None: Use the default caching behavior, which will disable
 #                                                 caching if `lazi.core` is already present in sys.modules
 #                                                 when lazi.conf.conf is imported.
```

### Comparing `lazi-1.5.52/lazi/conf/conf.py` & `lazi-1.5.52.dev1/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52/lazi/core/finder.py` & `lazi-1.5.52.dev1/lazi/core/finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,17 @@
         if self not in sys.meta_path:
             assert self.__refs__ == 0, self.__refs__
             if __debug__ and conf.DEBUG_TRACING > 1:
                 assert None is debug.trace(
                     f"+ {self.__class__.__name__}[{id(self)}] "
                     f"<{len([_ for _ in sys.meta_path if isinstance(_, type(self))])}>"
                 )
-
-            self.__refs__ += 1
             sys.meta_path.insert(0, self)
 
+        self.__refs__ += 1
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> bool:
         if __debug__ and conf.DEBUG_TRACING > 1 and self.__refs__ == 1:
             assert None is debug.trace(f"- {self.__class__.__name__}[{id(self)}]")
 
         self.__refs__ = max(self.__refs__ - 1, 0)
```

### Comparing `lazi-1.5.52/lazi/core/loader.py` & `lazi-1.5.52.dev1/lazi/core/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import sys
 from typing import ForwardRef
 from enum import Enum
 from importlib.abc import Loader as _Loader
 from importlib.util import module_from_spec
 
+from lazi.conf import conf
 from lazi.util import debug
 
 __all__ = "Loader",
 
 Spec = ForwardRef("Spec")
 Module = ForwardRef("Module")
 
@@ -56,15 +57,15 @@
         assert None is debug.trace(
             f"<exec> {spec.name} <L:{spec.loader_state}> <l:{lazy}>"
         )
 
         if spec.name not in sys.modules:
             sys.modules[spec.name] = module
 
-        if not lazy:
+        if not lazy or conf.FORCE_LOAD_MODULE:
             spec.loader_state = self.State.EXEC
             self.loader.exec_module(module)
             spec.loader_state = self.State.LOAD
         else:
             spec.loader_state = self.State.LAZY
 
     def unload_module(self, spec: Spec):
```

### Comparing `lazi-1.5.52/lazi/core/module.py` & `lazi-1.5.52.dev1/lazi/core/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             return super().__getattribute__(attr)
 
         if spec.target is not self and attr in (module_dict := spec.target.__getattribute__("__dict__")):
             return module_dict[attr]
 
         assert None is debug.trace(f"<attr> {spec.name}[.{attr}] <L:{spec.loader_state}>")
 
-        if spec.loader_state is spec.loader.State.LAZY:
+        if spec.loader_state.value <= spec.loader.State.LAZY.value:
             spec.loader.exec_module(spec.target, lazy=False)
 
         if spec.target is self:
             return super().__getattribute__(attr)
         else:
             return spec.target.__getattribute__(attr)
```

### Comparing `lazi-1.5.52/lazi/core/spec.py` & `lazi-1.5.52.dev1/lazi/core/spec.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52/lazi/util/util.py` & `lazi-1.5.52.dev1/lazi/util/util.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52/pyproject.toml` & `lazi-1.5.52.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.5.52"
+version = "1.5.52-dev1"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
```

### Comparing `lazi-1.5.52/tests/test_django.py` & `lazi-1.5.52.dev1/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.52/PKG-INFO` & `lazi-1.5.52.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.5.52
+Version: 1.5.52.dev1
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Web Environment
@@ -90,12 +90,12 @@
 
 It's also possible to manually change the configuration at runtime,
 with the caveat that some variables may have already been used by
 `lazi.core`. To avoid this, configure Lazi before importing it:
 
 ```python
 from lazi.conf import conf
-conf.DEBUG_TRACING = True
+conf.DEBUG_TRACING = 1
 import lazi.auto
 # ...
 ```
```

