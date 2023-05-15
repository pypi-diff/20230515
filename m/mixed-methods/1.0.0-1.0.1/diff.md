# Comparing `tmp/mixed_methods-1.0.0.tar.gz` & `tmp/mixed_methods-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixed_methods-1.0.0.tar", max compression
+gzip compressed data, was "mixed_methods-1.0.1.tar", max compression
```

## Comparing `mixed_methods-1.0.0.tar` & `mixed_methods-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1092 2023-04-16 13:54:02.021996 mixed_methods-1.0.0/LICENSE
--rw-r--r--   0        0        0     3459 2023-04-16 13:54:02.021996 mixed_methods-1.0.0/README.md
--rw-r--r--   0        0        0      307 2023-04-16 13:54:02.021996 mixed_methods-1.0.0/mixed_methods/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-16 13:54:02.021996 mixed_methods-1.0.0/mixed_methods/core.py
--rw-r--r--   0        0        0        0 2023-04-16 13:54:02.021996 mixed_methods-1.0.0/mixed_methods/py.typed
--rw-r--r--   0        0        0     3055 2023-04-16 13:54:02.021996 mixed_methods-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4612 1970-01-01 00:00:00.000000 mixed_methods-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-15 12:40:49.268563 mixed_methods-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3459 2023-05-15 12:40:49.268563 mixed_methods-1.0.1/README.md
+-rw-r--r--   0        0        0      307 2023-05-15 12:40:49.268563 mixed_methods-1.0.1/mixed_methods/__init__.py
+-rw-r--r--   0        0        0     1565 2023-05-15 12:40:49.272563 mixed_methods-1.0.1/mixed_methods/core.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:40:49.272563 mixed_methods-1.0.1/mixed_methods/py.typed
+-rw-r--r--   0        0        0     3209 2023-05-15 12:40:49.272563 mixed_methods-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4655 1970-01-01 00:00:00.000000 mixed_methods-1.0.1/PKG-INFO
```

### Comparing `mixed_methods-1.0.0/LICENSE` & `mixed_methods-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mixed_methods-1.0.0/README.md` & `mixed_methods-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add mixed-methods
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-mixed-methods = "^1.0.0"
+mixed-methods = "^1.0.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.mixed-methods]
 git = "https://github.com/nekitdev/mixed-methods.git"
```

### Comparing `mixed_methods-1.0.0/mixed_methods/core.py` & `mixed_methods-1.0.1/mixed_methods/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Callable, Concatenate, Generic, Optional, Type, TypeVar, Union, final, overload
+from typing import Callable, Generic, Optional, Type, TypeVar, Union, final, overload
 
 from attrs import frozen
-from typing_extensions import ParamSpec
+from typing_extensions import Concatenate, ParamSpec
 
 __all__ = ("MixedMethod", "mixed_method")
 
 T = TypeVar("T")
 
 # P -> R
```

### Comparing `mixed_methods-1.0.0/pyproject.toml` & `mixed_methods-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mixed-methods"
-version = "1.0.0"
+version = "1.0.1"
 description = "Mixed methods."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/mixed-methods"
@@ -27,57 +27,65 @@
 Issues = "https://github.com/nekitdev/mixed-methods/issues"
 
 [[tool.poetry.packages]]
 include = "mixed_methods"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
-attrs = ">= 22.2.0"
+attrs = ">= 23.1.0"
+typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
+flake8-pyproject = "1.2.3"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.format.dependencies.isort]
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
 pytest = "7.3.1"
 pytest-cov = "4.0.0"
-typing-extensions = "4.5.0"
 
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
 
+[tool.flake8]
+max_line_length = 100
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--cov mixed_methods"
 testpaths = ["tests"]
@@ -124,15 +132,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "mixed-methods"
-version = "1.0.0"
+version = "1.0.1"
 url = "https://github.com/nekitdev/mixed-methods"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `mixed_methods-1.0.0/PKG-INFO` & `mixed_methods-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixed-methods
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mixed methods.
 Home-page: https://github.com/nekitdev/mixed-methods
 License: MIT
 Keywords: python,mixed,method
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: attrs (>=22.2.0)
+Requires-Dist: attrs (>=23.1.0)
+Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/mixed-methods
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/mixed-methods/issues
 Project-URL: Repository, https://github.com/nekitdev/mixed-methods
 Description-Content-Type: text/markdown
 
@@ -69,15 +70,15 @@
 $ poetry add mixed-methods
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-mixed-methods = "^1.0.0"
+mixed-methods = "^1.0.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.mixed-methods]
 git = "https://github.com/nekitdev/mixed-methods.git"
```

