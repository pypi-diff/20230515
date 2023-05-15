# Comparing `tmp/robotcode_robot-0.37.1.tar.gz` & `tmp/robotcode_robot-0.38.0.tar.gz`

## Comparing `robotcode_robot-0.37.1.tar` & `robotcode_robot-0.38.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/src/robotcode/robot/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    78357 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/README.md
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/pyproject.toml
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.37.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    78347 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/README.md
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/pyproject.toml
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/PKG-INFO
```

### Comparing `robotcode_robot-0.37.1/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.38.0/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.37.1/src/robotcode/robot/config/model.py` & `robotcode_robot-0.38.0/src/robotcode/robot/config/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     return dataclasses.field(*args, **kwargs)
 
 
 class EvaluationError(Exception):
     """Evaluation error."""
 
     def __init__(self, expression: str, message: str):
-        super().__init__(f"Evaluation of {repr(expression)} failed: {message}")
+        super().__init__(f"Evaluation of {expression!r} failed: {message}")
         self.expr = expression
 
 
 SAFE_GLOBALS = {
     "environ": os.environ,
     "re": re,
     "platform": platform,
@@ -254,15 +254,15 @@
                             result.append(f"{key}{separator if item else ''}{separator.join(item)}")
                         else:
                             result.append(f"{key}:{item}")
                 else:
                     append_name(field)
                     result.append(str(value))
             except EvaluationError as e:
-                raise ValueError(f"Evaluation of '{field.name}' failed: {str(e)}") from e
+                raise ValueError(f"Evaluation of '{field.name}' failed: {e!s}") from e
 
         return result
 
     @staticmethod
     def _verified_value(name: str, value: Any, types: Union[type, Tuple[type, ...]], target: Any) -> Any:
         errors = validate_types(types, value)
         if errors:
@@ -337,15 +337,15 @@
                         f.name,
                         {
                             k: e.evaluate() if isinstance(e, Expression) else e
                             for k, e in getattr(result, f.name).items()
                         },
                     )
             except EvaluationError as e:
-                raise ValueError(f"Evaluation of '{f.name}' failed: {str(e)}") from e
+                raise ValueError(f"Evaluation of '{f.name}' failed: {e!s}") from e
         return result
 
 
 # start generated code
 
 
 @dataclass
```

### Comparing `robotcode_robot-0.37.1/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.38.0/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.37.1/.gitignore` & `robotcode_robot-0.38.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.37.1/LICENSE.txt` & `robotcode_robot-0.38.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.37.1/README.md` & `robotcode_robot-0.38.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.37.1/pyproject.toml` & `robotcode_robot-0.38.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
-  "robotcode-core==0.37.1",
+  "robotcode-core==0.38.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.37.1/PKG-INFO` & `robotcode_robot-0.38.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.37.1
+Version: 0.38.0
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.37.1
+Requires-Dist: robotcode-core==0.38.0
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

