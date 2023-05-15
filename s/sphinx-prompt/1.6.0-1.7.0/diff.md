# Comparing `tmp/sphinx_prompt-1.6.0.tar.gz` & `tmp/sphinx_prompt-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_prompt-1.6.0.tar", max compression
+gzip compressed data, was "sphinx_prompt-1.7.0.tar", max compression
```

## Comparing `sphinx_prompt-1.6.0.tar` & `sphinx_prompt-1.7.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1500 2023-02-18 13:05:18.665615 sphinx_prompt-1.6.0/LICENSE
--rw-r--r--   0        0        0     2010 2023-02-18 13:05:18.665615 sphinx_prompt-1.6.0/README.rst
--rw-r--r--   0        0        0     1951 2023-02-18 13:06:50.867301 sphinx_prompt-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     6312 2023-02-18 13:05:18.665615 sphinx_prompt-1.6.0/sphinx-prompt/__init__.py
--rw-r--r--   0        0        0        0 2023-02-18 13:05:18.665615 sphinx_prompt-1.6.0/sphinx-prompt/py.typed
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 sphinx_prompt-1.6.0/setup.py
--rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 sphinx_prompt-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-05-15 06:28:02.412848 sphinx_prompt-1.7.0/LICENSE
+-rw-r--r--   0        0        0     2010 2023-05-15 06:28:02.412848 sphinx_prompt-1.7.0/README.rst
+-rw-r--r--   0        0        0     1951 2023-05-15 06:33:53.833253 sphinx_prompt-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6312 2023-05-15 06:28:02.412848 sphinx_prompt-1.7.0/sphinx-prompt/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 06:28:02.412848 sphinx_prompt-1.7.0/sphinx-prompt/py.typed
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 sphinx_prompt-1.7.0/PKG-INFO
```

### Comparing `sphinx_prompt-1.6.0/LICENSE` & `sphinx_prompt-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_prompt-1.6.0/README.rst` & `sphinx_prompt-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_prompt-1.6.0/pyproject.toml` & `sphinx_prompt-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "sphinx-prompt"
-version = "1.6.0"
+version = "1.7.0"
 description = "Sphinx directive to add unselectable prompt"
 readme = "README.rst"
 authors = ["Stéphane Brunner <stephane.brunner@gmail.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Environment :: Web Environment",
@@ -37,22 +37,22 @@
 repository = "https://github.com/sbrunner/sphinx-prompt"
 license = "BSD-3-Clause"
 keywords = ["sphinx", "shell", "prompt"]
 packages = [{ include = "sphinx_prompt" }, { include = "sphinx_prompt/py.typed" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-Sphinx = "6.1.3"
-pygments = "2.14.0"
+Sphinx = "7.0.0"
+pygments = "2.15.1"
 docutils = "0.19"
 
 [tool.poetry.group.dev.dependencies]
-prospector = { version = "1.8.4", extras = ["with_bandit", "with_mypy", "with_pyroma"] }
-pytest = "7.2.1"
-types-docutils = "0.19.1.2"
+prospector = { version = "1.9.0", extras = ["with_bandit", "with_mypy", "with_pyroma"] }
+pytest = "7.3.1"
+types-docutils = "0.19.1.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-plugin-tweak-dependencies-version", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-plugin-tweak-dependencies-version]
 default = "present"
```

### Comparing `sphinx_prompt-1.6.0/sphinx-prompt/__init__.py` & `sphinx_prompt-1.7.0/sphinx-prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_prompt-1.6.0/PKG-INFO` & `sphinx_prompt-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-prompt
-Version: 1.6.0
+Version: 1.7.0
 Summary: Sphinx directive to add unselectable prompt
 Home-page: https://hub.docker.com/r/sbrunner/sphinx-prompt/
 License: BSD-3-Clause
 Keywords: sphinx,shell,prompt
 Author: Stéphane Brunner
 Author-email: stephane.brunner@gmail.com
 Requires-Python: >=3.8,<3.11
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Typing :: Typed
-Requires-Dist: Sphinx (>=6.0.0,<7.0.0)
+Requires-Dist: Sphinx (>=7.0.0,<8.0.0)
 Requires-Dist: docutils
 Requires-Dist: pygments
 Project-URL: Repository, https://github.com/sbrunner/sphinx-prompt
 Description-Content-Type: text/x-rst
 
 Sphinx Prompt
 =============
```

