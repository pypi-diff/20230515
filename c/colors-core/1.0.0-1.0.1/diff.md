# Comparing `tmp/colors_core-1.0.0.tar.gz` & `tmp/colors_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colors_core-1.0.0.tar", max compression
+gzip compressed data, was "colors_core-1.0.1.tar", max compression
```

## Comparing `colors_core-1.0.0.tar` & `colors_core-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1092 2023-04-13 12:24:39.961413 colors_core-1.0.0/LICENSE
--rw-r--r--   0        0        0     3240 2023-04-13 12:24:39.961413 colors_core-1.0.0/README.md
--rw-r--r--   0        0        0      272 2023-04-13 12:24:39.965413 colors_core-1.0.0/colors/__init__.py
--rw-r--r--   0        0        0      508 2023-04-13 12:24:39.965413 colors_core-1.0.0/colors/ansi.py
--rw-r--r--   0        0        0      629 2023-04-13 12:24:39.965413 colors_core-1.0.0/colors/constants.py
--rw-r--r--   0        0        0     7648 2023-04-13 12:24:39.965413 colors_core-1.0.0/colors/core.py
--rw-r--r--   0        0        0      596 2023-04-13 12:24:39.965413 colors_core-1.0.0/colors/hex.py
--rw-r--r--   0        0        0        0 2023-04-13 12:24:39.965413 colors_core-1.0.0/colors/py.typed
--rw-r--r--   0        0        0      265 2023-04-13 12:24:39.965413 colors_core-1.0.0/colors/typing.py
--rw-r--r--   0        0        0      635 2023-04-13 12:24:39.965413 colors_core-1.0.0/colors/utils.py
--rw-r--r--   0        0        0     3002 2023-04-13 12:24:39.965413 colors_core-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4392 1970-01-01 00:00:00.000000 colors_core-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-14 22:41:49.550827 colors_core-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3240 2023-05-14 22:41:49.550827 colors_core-1.0.1/README.md
+-rw-r--r--   0        0        0      272 2023-05-14 22:41:49.550827 colors_core-1.0.1/colors/__init__.py
+-rw-r--r--   0        0        0      508 2023-05-14 22:41:49.550827 colors_core-1.0.1/colors/ansi.py
+-rw-r--r--   0        0        0      629 2023-05-14 22:41:49.550827 colors_core-1.0.1/colors/constants.py
+-rw-r--r--   0        0        0     7648 2023-05-14 22:41:49.550827 colors_core-1.0.1/colors/core.py
+-rw-r--r--   0        0        0      596 2023-05-14 22:41:49.550827 colors_core-1.0.1/colors/hex.py
+-rw-r--r--   0        0        0        0 2023-05-14 22:41:49.550827 colors_core-1.0.1/colors/py.typed
+-rw-r--r--   0        0        0      265 2023-05-14 22:41:49.550827 colors_core-1.0.1/colors/typing.py
+-rw-r--r--   0        0        0      643 2023-05-14 22:41:49.550827 colors_core-1.0.1/colors/utils.py
+-rw-r--r--   0        0        0     3003 2023-05-14 22:41:49.550827 colors_core-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4392 1970-01-01 00:00:00.000000 colors_core-1.0.1/PKG-INFO
```

### Comparing `colors_core-1.0.0/LICENSE` & `colors_core-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `colors_core-1.0.0/README.md` & `colors_core-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add colors-core
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-colors-core = "^1.0.0"
+colors-core = "^1.0.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.colors-core]
 git = "https://github.com/nekitdev/colors-core.git"
```

### Comparing `colors_core-1.0.0/colors/constants.py` & `colors_core-1.0.1/colors/constants.py`

 * *Files identical despite different names*

### Comparing `colors_core-1.0.0/colors/core.py` & `colors_core-1.0.1/colors/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
     def to_rgb(self) -> RGB:
         """Converts the color to *RGB* values (each in `[0, 255]` range).
 
         Returns:
             The *RGB* values.
         """
-        return (self.red, self.blue, self.green)
+        return (self.red, self.green, self.blue)
 
     @classmethod
     def from_rgba(cls: Type[C], red: int, green: int, blue: int, alpha: int) -> C:
         """Creates a color from *RGBA* values (each in `[0, 255]` range).
 
         Note:
             The *alpha* channel is simply ignored.
```

### Comparing `colors_core-1.0.0/colors/hex.py` & `colors_core-1.0.1/colors/hex.py`

 * *Files identical despite different names*

### Comparing `colors_core-1.0.0/colors/utils.py` & `colors_core-1.0.1/colors/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from colors.constants import BYTE
 
 __all__ = ("float_to_byte", "byte_to_float")
 
 
 def float_to_byte(value: float) -> int:
-    """Converts the float `value` in range `[0, 1]` to the corresponding byte value in range `[0, 255]`.
+    """Converts the float `value` in range `[0, 1]` to the corresponding
+    byte value in range `[0, 255]`.
 
     Arguments:
         value: The value to convert.
 
     Returns:
         The converted value.
     """
     return int(value * BYTE)
 
 
 def byte_to_float(value: int) -> float:
-    """Converts the byte `value` in range `[0, 255]` to the corresponding float value in range `[0, 1]`.
+    """Converts the byte `value` in range `[0, 255]` to the corresponding
+    float value in range `[0, 1]`.
 
     Arguments:
         value: The value to convert.
 
     Returns:
         The converted value.
     """
```

### Comparing `colors_core-1.0.0/pyproject.toml` & `colors_core-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "colors-core"
-version = "1.0.0"
+version = "1.0.1"
 description = "Core color functionality."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/colors-core"
@@ -28,15 +28,15 @@
 
 [[tool.poetry.packages]]
 include = "colors"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
-attrs = ">= 22.2.0"
+attrs = ">= 23.1.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
 
@@ -44,36 +44,36 @@
 version = "5.12.0"
 python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "1.2.0"
+mypy = "1.3.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.3.0"
+pytest = "7.3.1"
 pytest-cov = "4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.4.2"
-mkdocs-material = "9.1.6"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.12"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
 version = "0.21.2"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.1.0"
+changelogging = "1.2.0"
 
 [tool.black]
 line_length = 100
 
 [tool.isort]
 line_length = 100
 profile = "black"
@@ -124,15 +124,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "colors-core"
-version = "1.0.0"
+version = "1.0.1"
 url = "https://github.com/nekitdev/colors-core"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `colors_core-1.0.0/PKG-INFO` & `colors_core-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colors-core
-Version: 1.0.0
+Version: 1.0.1
 Summary: Core color functionality.
 Home-page: https://github.com/nekitdev/colors-core
 License: MIT
 Keywords: python,color,core
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: attrs (>=22.2.0)
+Requires-Dist: attrs (>=23.1.0)
 Project-URL: Documentation, https://nekitdev.github.io/colors-core
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/colors-core/issues
 Project-URL: Repository, https://github.com/nekitdev/colors-core
 Description-Content-Type: text/markdown
 
@@ -69,15 +69,15 @@
 $ poetry add colors-core
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-colors-core = "^1.0.0"
+colors-core = "^1.0.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.colors-core]
 git = "https://github.com/nekitdev/colors-core.git"
```

