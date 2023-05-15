# Comparing `tmp/kraken_wrapper-0.2.4.tar.gz` & `tmp/kraken_wrapper-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.2.4.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.20.0.tar", max compression
```

## Comparing `kraken_wrapper-0.2.4.tar` & `kraken_wrapper-0.20.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      988 2022-11-26 20:38:46.639181 kraken_wrapper-0.2.4/LICENSE
--rw-r--r--   0        0        0     1906 2023-03-22 22:48:29.164882 kraken_wrapper-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      433 2023-03-22 22:46:07.140898 kraken_wrapper-0.2.4/readme.md
--rw-r--r--   0        0        0      133 2023-03-22 22:48:29.184881 kraken_wrapper-0.2.4/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     3637 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/_buildend_venv.py
--rw-r--r--   0        0        0     3374 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     5311 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     3674 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/_buildenv_pex.py
--rw-r--r--   0        0        0     3175 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4605 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     3564 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0     4222 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/_pex.py
--rw-r--r--   0        0        0    15754 2023-03-22 22:40:25.894548 kraken_wrapper-0.2.4/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2022-11-26 20:38:46.639181 kraken_wrapper-0.2.4/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 kraken_wrapper-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-13 22:21:22.034813 kraken_wrapper-0.20.0/LICENSE
+-rw-r--r--   0        0        0     1908 2023-05-15 10:32:46.002403 kraken_wrapper-0.20.0/pyproject.toml
+-rw-r--r--   0        0        0      433 2023-05-13 22:21:22.034813 kraken_wrapper-0.20.0/readme.md
+-rw-r--r--   0        0        0      134 2023-05-15 10:32:46.002403 kraken_wrapper-0.20.0/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     3637 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/_buildend_venv.py
+-rw-r--r--   0        0        0     3374 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     5311 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     3674 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/_buildenv_pex.py
+-rw-r--r--   0        0        0     3175 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4605 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     3564 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0     4222 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/_pex.py
+-rw-r--r--   0        0        0    15754 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:21:22.042812 kraken_wrapper-0.20.0/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 kraken_wrapper-0.20.0/PKG-INFO
```

### Comparing `kraken_wrapper-0.2.4/LICENSE` & `kraken_wrapper-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/pyproject.toml` & `kraken_wrapper-0.20.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.2.4"
+version = "0.20.0"
 description = ""
 authors = ["Unknown <me@unknown.org>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "kraken/wrapper", from = "src" }]
 classifiers = []
 keywords = []
@@ -18,15 +18,15 @@
 # Documentation = ""
 # Homepage = ""
 # Repository = ""
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 keyring = "^23.8.2"
-kraken-common = "^0.5.2"
+kraken-common = "^0.20.0"
 pex = "^2.1.103"
 setuptools = ">=33.0.0"  # For pkg_resources
 termcolor = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
```

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/_buildend_venv.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/_buildend_venv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/_buildenv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/_buildenv_pex.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/_buildenv_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/_config.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/_pex.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/src/kraken/wrapper/main.py` & `kraken_wrapper-0.20.0/src/kraken/wrapper/main.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.2.4/PKG-INFO` & `kraken_wrapper-0.20.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.2.4
+Version: 0.20.0
 Summary: 
 License: MIT
 Author: Unknown
 Author-email: me@unknown.org
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keyring (>=23.8.2,<24.0.0)
-Requires-Dist: kraken-common (>=0.5.2,<0.6.0)
+Requires-Dist: kraken-common (>=0.20.0,<0.21.0)
 Requires-Dist: pex (>=2.1.103,<3.0.0)
 Requires-Dist: setuptools (>=33.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # kraken-wrapper
```

