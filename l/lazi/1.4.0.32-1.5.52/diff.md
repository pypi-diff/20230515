# Comparing `tmp/lazi-1.4.0.32.tar.gz` & `tmp/lazi-1.5.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.4.0.32.tar", max compression
+gzip compressed data, was "lazi-1.5.52.tar", max compression
```

## Comparing `lazi-1.4.0.32.tar` & `lazi-1.5.52.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.4.0.32/LICENSE
--rw-r--r--   0        0        0     2159 2023-05-12 22:56:51.654129 lazi-1.4.0.32/README.md
--rw-r--r--   0        0        0      104 2023-05-11 08:57:20.841058 lazi-1.4.0.32/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.4.0.32/lazi/conf/auto.py
--rw-r--r--   0        0        0     2161 2023-05-12 21:13:16.032559 lazi-1.4.0.32/lazi/conf/base.py
--rw-r--r--   0        0        0     4933 2023-05-12 07:30:19.043612 lazi-1.4.0.32/lazi/conf/conf.py
--rw-r--r--   0        0        0       69 2023-05-12 21:13:16.044560 lazi-1.4.0.32/lazi/conf/test.py
--rw-r--r--   0        0        0      663 2023-05-12 23:20:14.516521 lazi-1.4.0.32/lazi/core/__init__.py
--rw-r--r--   0        0        0     4488 2023-05-12 22:47:20.382630 lazi-1.4.0.32/lazi/core/finder.py
--rw-r--r--   0        0        0     3468 2023-05-12 22:52:20.018565 lazi-1.4.0.32/lazi/core/loader.py
--rw-r--r--   0        0        0     6167 2023-05-12 23:18:02.702794 lazi-1.4.0.32/lazi/core/record.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.4.0.32/lazi/util/__init__.py
--rw-r--r--   0        0        0      248 2023-05-11 20:06:44.097623 lazi-1.4.0.32/lazi/util/debug.py
--rw-r--r--   0        0        0     2056 2023-05-12 23:17:59.374750 lazi-1.4.0.32/lazi/util/functional.py
--rw-r--r--   0        0        0      618 2023-05-11 20:06:44.097623 lazi-1.4.0.32/lazi/util/util.py
--rw-r--r--   0        0        0     1213 2023-05-12 23:27:36.566323 lazi-1.4.0.32/pyproject.toml
--rw-r--r--   0        0        0      918 2023-05-12 22:06:26.710396 lazi-1.4.0.32/tests/test_django.py
--rw-r--r--   0        0        0     1233 2023-05-12 07:00:36.171542 lazi-1.4.0.32/tests/test_importlib.py
--rw-r--r--   0        0        0      120 2023-05-12 06:05:10.203013 lazi-1.4.0.32/tests/test_pandas.py
--rw-r--r--   0        0        0      192 2023-05-12 23:21:17.805350 lazi-1.4.0.32/tests/test_record.py
--rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 lazi-1.4.0.32/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.5.52/LICENSE
+-rw-r--r--   0        0        0     1920 2023-05-15 07:55:44.338848 lazi-1.5.52/README.md
+-rw-r--r--   0        0        0      197 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.5.52/lazi/conf/auto.py
+-rw-r--r--   0        0        0      907 2023-05-15 07:53:29.925087 lazi-1.5.52/lazi/conf/base.py
+-rw-r--r--   0        0        0     4738 2023-05-15 07:52:46.768522 lazi-1.5.52/lazi/conf/conf.py
+-rw-r--r--   0        0        0       69 2023-05-12 21:13:16.044560 lazi-1.5.52/lazi/conf/test.py
+-rw-r--r--   0        0        0      364 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/__init__.py
+-rw-r--r--   0        0        0     3351 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/finder.py
+-rw-r--r--   0        0        0     2103 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/loader.py
+-rw-r--r--   0        0        0     3148 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/module.py
+-rw-r--r--   0        0        0     1211 2023-05-15 07:36:15.807454 lazi-1.5.52/lazi/core/spec.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.5.52/lazi/util/__init__.py
+-rw-r--r--   0        0        0      248 2023-05-11 20:06:44.097623 lazi-1.5.52/lazi/util/debug.py
+-rw-r--r--   0        0        0      174 2023-05-15 07:53:12.940865 lazi-1.5.52/lazi/util/functional.py
+-rw-r--r--   0        0        0      618 2023-05-11 20:06:44.097623 lazi-1.5.52/lazi/util/util.py
+-rw-r--r--   0        0        0     1555 2023-05-15 07:57:18.012076 lazi-1.5.52/pyproject.toml
+-rw-r--r--   0        0        0      912 2023-05-15 07:36:15.807454 lazi-1.5.52/tests/test_django.py
+-rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 lazi-1.5.52/PKG-INFO
```

### Comparing `lazi-1.4.0.32/LICENSE` & `lazi-1.5.52/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.4.0.32/lazi/conf/conf.py` & `lazi-1.5.52/lazi/conf/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,38 +4,35 @@
 - Any value that is also defined in base.py will be overwritten by the value in the module.
 - Configuration values will be accessible from the conf namespace package.
 - The import order of the modules determines the resulting configuration.
 
 Use like this (recommended for package mdules):
 
 >>> from lazi.conf import conf
->>> conf.LOADER_AUTO_DEPS
+>>> conf.DEBUG_TRACING
 
 Or like this (recommended for client modules):
 
 >>> import lazi.conf.auto
->>> lazi.conf.LOADER_AUTO_DEPS
+>>> lazi.conf.DEBUG_TRACING
 >>> from lazi.conf import auto
->>> auto.LOADER_AUTO_DEPS
+>>> auto.DEBUG_TRACING
 
 But not like this:
 
 >>> import lazi.conf        # This is not the same as the above.
->>> import lazi.conf.conf   # This works but is not recommended because lazi.conf.conf becomes inaccessible.
 >>> from lazi import conf   # Still no worky. Only imports the namespace module without loading.
 """
 import sys as _sys
 
 from types import ModuleType, EllipsisType
 from typing import Iterator
 from pkgutil import ModuleInfo, iter_modules as _iter_modules
 from importlib import import_module as _import_module
 
-from lazi.util import SingletonMeta
-
 __all__ = [
     "base", "conf", "__root__", "__conf__", "__core__", "__auto__", "__keys__",
 ]
 
 if __name__ == "__main__":
     raise RuntimeError(f"Cannot run {__file__} as a script.")
 
@@ -50,15 +47,15 @@
 __auto__: str               # <conf>.<meta: auto>
 
 __keys__: set = {key for key in globals() if not key.startswith("_") and key.isupper()}
 
 conf: dict
 
 
-class Conf(ModuleType, metaclass=SingletonMeta):
+class Conf(ModuleType):
     __all__ = __all__
 
     from . import base  # noqa: Relative import from namespace package -- works here.
 
     __root__: ModuleType = _import_module(base.__meta__["root"])
     __conf__: ModuleType = _import_module(f"{__root__.__name__}.{__name__.rpartition('.')[-1]}")
 
@@ -136,8 +133,8 @@
         return value
 
 
 _sys.modules[__name__] = Conf()  # Replace module with instance.
 
 __all__.extend(__keys__)
 
-del ModuleType, EllipsisType, Iterator, ModuleInfo, SingletonMeta
+del ModuleType, EllipsisType, Iterator, ModuleInfo
```

### Comparing `lazi-1.4.0.32/lazi/util/util.py` & `lazi-1.5.52/lazi/util/util.py`

 * *Files identical despite different names*

### Comparing `lazi-1.4.0.32/pyproject.toml` & `lazi-1.5.52/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.4.0.32"
+version = "1.5.52"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
@@ -17,32 +17,51 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries",
 ]
 
 packages = [
-    { include = "lazi" },
-    { include = "tests", format = "sdist" }
+    { include = "lazi" }
 ]
 
+include = [
+    { path = "tests", format = "sdist" }
+]
+
+[tool.poetry.dependencies]
+python = "^3.11"
+
 
 [tool.poetry.group.dev]
 optional = true
-
 [tool.poetry.group.dev.dependencies]
 django = "^4"
 requests = "^2"
 toolz = "^0"
 rich = "^13"
 setuptools = "^67"
 pandas = "^2"
 pytest = "^7"
+wagtail = "^5.0"
+presto-requests = "^1.3.6"
 
+[tool.poetry.group.direct]
+optional = true
+[tool.poetry.group.direct.dependencies]
+presto-requests = {git = "https://github.com/sitbon/presto"}
 
-[tool.poetry.dependencies]
-python = ">=3.10"
+
+[tool.pytest.ini_options]
+addopts = "-v --no-header -rA"
+cache_dir = ".cache/pytest"
+testpaths = [
+    "tests",
+]
+markers = [
+    "test_test",
+]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lazi-1.4.0.32/PKG-INFO` & `lazi-1.5.52/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.4.0.32
+Version: 1.5.52
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
-Requires-Python: >=3.10
+Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Project-URL: Repository, https://github.com/sitbon/lazi
 Description-Content-Type: text/markdown
 
 # Lazi: Lazy Imports Everywhere
 
-A lightweight and extensible way to implement lazy imports globally.
+An easy way to implement and track lazy imports globally.
+
+No external dependencies.
+
+**Requres Python 3.11.**
 
 ## Usage:
 
 ```shell
 poetry add lazi
 ```
 
 ```python
 """Automatic lazy loading example.
 
 Install django to run, or change the imports.
 """
-import lazi.auto                 # Install import tracking.
+import lazi.auto as lazi         # Install import tracking.
 import django.test               # Import stuff.
-print(lazi.used_count())         # Count loaded modules.
+# print(lazi.used_count())         # Count loaded modules. <Not yet re-implemented>
 TestCase = django.test.TestCase  # Trigger lazy loading.
-print(lazi.used_count())         # More modules were lazy loaded.
+# print(lazi.used_count())         # More modules were lazy loaded. <TBD>
 ```
 
 ```shell
 python example.py
 ```
 
 ```python
 0
-211
+262
 ```
 
 ```python
 """Manual lazy loading example.
 """
-import lazi.core                        # Import Lazi.
+import lazi.core as lazi                # Import Lazi.
 django = lazi.lazy("django")            # Import stuff.
 django_test = lazi.lazy("django.test")  # Import more stuff.
-print(lazi.used_count())                # Count loaded modules.
+# print(lazi.used_count())              # Count loaded modules. <TBD>
 TestCase = django_test.TestCase         # Trigger lazy loading.
-print(lazi.used_count())                # Module was lazy loaded.
+# print(lazi.used_count())              # Module was lazy loaded. <TBD>
 ```
 
 ```python
 0
 2
 ```
 
@@ -79,39 +82,20 @@
 It is fully decoupled from the rest of the codebase.
 
 As a result, it's possible configure Lazi by creating `lazi.conf`
 modules in your project (within the `lazi.conf` namespace package),
 and use conf modules provided by other packages.
 
 Configuration is not yet controllable via environment variables,
-but this is planned for the future.
+but this is planned for the future. Update: Supported for DEBUG_TRACING.
 
 It's also possible to manually change the configuration at runtime,
 with the caveat that some variables may have already been used by
 `lazi.core`. To avoid this, configure Lazi before importing it:
 
 ```python
 from lazi.conf import conf
 conf.DEBUG_TRACING = True
 import lazi.auto
 # ...
 ```
 
-
-## Metadata
-
-Reference for developers: The json dict below contains Python versioning parameters:
-- Soft `min` (ignore rev) & hard `max` compatible versions.
-- Recommended `use` & creator's environment `dev` versions.
-
-```json
-{
-  "python": {
-    "version": {
-      "min": "3.10.11",
-      "max": "3.12",
-      "use": "3.11",
-      "dev": "3.11.2"
-    }
-  }
-}
-```
```

