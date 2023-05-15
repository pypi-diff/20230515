# Comparing `tmp/autoinject-1.3.0.tar.gz` & `tmp/autoinject-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoinject-1.3.0.tar", last modified: Mon May 15 20:59:21 2023, max compression
+gzip compressed data, was "autoinject-1.3.1.tar", last modified: Mon May 15 21:07:54 2023, max compression
```

## Comparing `autoinject-1.3.0.tar` & `autoinject-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.607386 autoinject-1.3.0/
--rw-rw-rw-   0        0        0     1058 2023-05-15 17:40:59.000000 autoinject-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     9942 2023-05-15 20:59:21.607386 autoinject-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     9324 2023-05-15 20:58:54.000000 autoinject-1.3.0/README.md
--rw-rw-rw-   0        0        0       88 2023-05-15 17:40:59.000000 autoinject-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      809 2023-05-15 20:59:21.609386 autoinject-1.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.580387 autoinject-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.592386 autoinject-1.3.0/src/autoinject/
--rw-rw-rw-   0        0        0      496 2023-05-15 19:38:33.000000 autoinject-1.3.0/src/autoinject/__init__.py
--rw-rw-rw-   0        0        0      227 2023-05-15 17:40:59.000000 autoinject-1.3.0/src/autoinject/_tests.py
--rw-rw-rw-   0        0        0     7138 2023-05-15 20:33:47.000000 autoinject-1.3.0/src/autoinject/class_registry.py
--rw-rw-rw-   0        0        0     7469 2023-05-15 18:15:47.000000 autoinject-1.3.0/src/autoinject/context_manager.py
--rw-rw-rw-   0        0        0    11411 2023-05-15 19:37:38.000000 autoinject-1.3.0/src/autoinject/informants.py
--rw-rw-rw-   0        0        0    22482 2023-05-15 20:59:10.000000 autoinject-1.3.0/src/autoinject/injection.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.598386 autoinject-1.3.0/src/autoinject.egg-info/
--rw-rw-rw-   0        0        0     9942 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 20:59:21.000000 autoinject-1.3.0/src/autoinject.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:21.606387 autoinject-1.3.0/tests/
--rw-rw-rw-   0        0        0    14330 2023-05-15 17:40:59.000000 autoinject-1.3.0/tests/test_context_manager.py
--rw-rw-rw-   0        0        0     1436 2023-05-15 18:38:39.000000 autoinject-1.3.0/tests/test_ep.py
--rw-rw-rw-   0        0        0    16373 2023-05-15 20:56:09.000000 autoinject-1.3.0/tests/test_injector.py
--rw-rw-rw-   0        0        0     2701 2023-05-15 17:40:59.000000 autoinject-1.3.0/tests/test_non_standard_injection.py
--rw-rw-rw-   0        0        0     3446 2023-05-15 20:18:25.000000 autoinject-1.3.0/tests/test_registry.py
--rw-rw-rw-   0        0        0     5175 2023-05-15 17:40:59.000000 autoinject-1.3.0/tests/test_threaded.py
+drwxrwxrwx   0        0        0        0 2023-05-15 21:07:54.892290 autoinject-1.3.1/
+-rw-rw-rw-   0        0        0     1058 2023-05-15 17:40:59.000000 autoinject-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     9942 2023-05-15 21:07:54.892290 autoinject-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9324 2023-05-15 20:58:54.000000 autoinject-1.3.1/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-15 17:40:59.000000 autoinject-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      809 2023-05-15 21:07:54.893290 autoinject-1.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 21:07:54.862290 autoinject-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 21:07:54.874291 autoinject-1.3.1/src/autoinject/
+-rw-rw-rw-   0        0        0      496 2023-05-15 21:07:41.000000 autoinject-1.3.1/src/autoinject/__init__.py
+-rw-rw-rw-   0        0        0      227 2023-05-15 17:40:59.000000 autoinject-1.3.1/src/autoinject/_tests.py
+-rw-rw-rw-   0        0        0     7138 2023-05-15 20:33:47.000000 autoinject-1.3.1/src/autoinject/class_registry.py
+-rw-rw-rw-   0        0        0     7469 2023-05-15 18:15:47.000000 autoinject-1.3.1/src/autoinject/context_manager.py
+-rw-rw-rw-   0        0        0    11411 2023-05-15 19:37:38.000000 autoinject-1.3.1/src/autoinject/informants.py
+-rw-rw-rw-   0        0        0    22476 2023-05-15 21:07:28.000000 autoinject-1.3.1/src/autoinject/injection.py
+drwxrwxrwx   0        0        0        0 2023-05-15 21:07:54.882291 autoinject-1.3.1/src/autoinject.egg-info/
+-rw-rw-rw-   0        0        0     9942 2023-05-15 21:07:54.000000 autoinject-1.3.1/src/autoinject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-05-15 21:07:54.000000 autoinject-1.3.1/src/autoinject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 21:07:54.000000 autoinject-1.3.1/src/autoinject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-15 21:07:54.000000 autoinject-1.3.1/src/autoinject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 21:07:54.000000 autoinject-1.3.1/src/autoinject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 21:07:54.890290 autoinject-1.3.1/tests/
+-rw-rw-rw-   0        0        0    14330 2023-05-15 17:40:59.000000 autoinject-1.3.1/tests/test_context_manager.py
+-rw-rw-rw-   0        0        0     1436 2023-05-15 18:38:39.000000 autoinject-1.3.1/tests/test_ep.py
+-rw-rw-rw-   0        0        0    16373 2023-05-15 20:56:09.000000 autoinject-1.3.1/tests/test_injector.py
+-rw-rw-rw-   0        0        0     2701 2023-05-15 17:40:59.000000 autoinject-1.3.1/tests/test_non_standard_injection.py
+-rw-rw-rw-   0        0        0     3446 2023-05-15 20:18:25.000000 autoinject-1.3.1/tests/test_registry.py
+-rw-rw-rw-   0        0        0     5175 2023-05-15 17:40:59.000000 autoinject-1.3.1/tests/test_threaded.py
```

### Comparing `autoinject-1.3.0/LICENSE` & `autoinject-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/PKG-INFO` & `autoinject-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoinject
-Version: 1.3.0
+Version: 1.3.1
 Summary: Automated dependency injection for Python
 Home-page: https://github.com/turnbullerin/autoinject
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/autoinject/issues
 Project-URL: Documentation, https://autoinject.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autoinject-1.3.0/README.md` & `autoinject-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/setup.cfg` & `autoinject-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7574 6f69 6e6a 6563 740d 0a76   = autoinject..v
-00000020: 6572 7369 6f6e 203d 2031 2e33 2e30 0d0a  ersion = 1.3.0..
+00000020: 6572 7369 6f6e 203d 2031 2e33 2e31 0d0a  ersion = 1.3.1..
 00000030: 6175 7468 6f72 203d 2045 7269 6e20 5475  author = Erin Tu
 00000040: 726e 6275 6c6c 0d0a 6175 7468 6f72 5f65  rnbull..author_e
 00000050: 6d61 696c 203d 2065 7269 6e2e 612e 7475  mail = erin.a.tu
 00000060: 726e 6275 6c6c 4067 6d61 696c 2e63 6f6d  rnbull@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4175 746f 6d61 7465 6420 6465 7065 6e64  Automated depend
 00000090: 656e 6379 2069 6e6a 6563 7469 6f6e 2066  ency injection f
```

### Comparing `autoinject-1.3.0/src/autoinject/class_registry.py` & `autoinject-1.3.1/src/autoinject/class_registry.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/src/autoinject/context_manager.py` & `autoinject-1.3.1/src/autoinject/context_manager.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/src/autoinject/informants.py` & `autoinject-1.3.1/src/autoinject/informants.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/src/autoinject/injection.py` & `autoinject-1.3.1/src/autoinject/injection.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         """Handle creating a separate global context and test fixtures"""
         @wraps(fn)
         def inner_wrapper(*args, **kwargs):
             # This creates an entirely different GLOBAL context as well local context, so
             # that test cases can be truly independent of the shared global state.
             with self.context_manager.subcontext() as ctx:
                 for cls_name in fixtures or []:
-                    if isinstance(fixtures[cls_name], type) or isinstance(fixtures[cls_name], str)hon -m:
+                    if isinstance(fixtures[cls_name], type) or isinstance(fixtures[cls_name], str):
                         self.cls_registry.register(cls_name, constructor=fixtures[cls_name], _force_override=True)
                     else:
                         self.cls_registry.register(cls_name, constructor=lambda: fixtures[cls_name], _force_override=True)
                 return fn(*args, **kwargs)
         return inner_wrapper
 
     def ContextVars(self, context: t.Union[contextvars.Context, ContextVarManager, str, None] = "_default", suppress_exit_warning: bool = False):
```

### Comparing `autoinject-1.3.0/src/autoinject.egg-info/PKG-INFO` & `autoinject-1.3.1/src/autoinject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoinject
-Version: 1.3.0
+Version: 1.3.1
 Summary: Automated dependency injection for Python
 Home-page: https://github.com/turnbullerin/autoinject
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/autoinject/issues
 Project-URL: Documentation, https://autoinject.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autoinject-1.3.0/src/autoinject.egg-info/SOURCES.txt` & `autoinject-1.3.1/src/autoinject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/tests/test_context_manager.py` & `autoinject-1.3.1/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/tests/test_ep.py` & `autoinject-1.3.1/tests/test_ep.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/tests/test_injector.py` & `autoinject-1.3.1/tests/test_injector.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/tests/test_non_standard_injection.py` & `autoinject-1.3.1/tests/test_non_standard_injection.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/tests/test_registry.py` & `autoinject-1.3.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.0/tests/test_threaded.py` & `autoinject-1.3.1/tests/test_threaded.py`

 * *Files identical despite different names*

