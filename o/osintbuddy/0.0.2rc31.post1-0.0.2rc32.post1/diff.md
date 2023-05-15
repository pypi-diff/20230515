# Comparing `tmp/osintbuddy-0.0.2rc31.post1.tar.gz` & `tmp/osintbuddy-0.0.2rc32.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.2rc31.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "osintbuddy-0.0.2rc32.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `osintbuddy-0.0.2rc31.post1.tar` & `osintbuddy-0.0.2rc32.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      274 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      447 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      314 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1807 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/.pypirc
--rw-r--r--   0        0        0        5 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/Dockerfile
--rw-r--r--   0        0        0       11 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/LICENSE
--rw-r--r--   0        0        0     4663 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/README.md
--rw-r--r--   0        0        0       47 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/docs/workflows.md
--rw-r--r--   0        0        0     6665 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/pyproject.toml
--rw-r--r--   0        0        0      293 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/README.md
--rw-r--r--   0        0        0      374 2023-05-15 01:20:31.422430 osintbuddy-0.0.2rc31.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      151 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/errors.py
--rw-r--r--   0        0        0      527 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/examples/ip-plugin.py
--rw-r--r--   0        0        0      206 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/manager.py
--rw-r--r--   0        0        0      358 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/node/__init__.py
--rw-r--r--   0        0        0     1302 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/node/base.py
--rw-r--r--   0        0        0     2989 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/node/displays.py
--rw-r--r--   0        0        0     4099 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/node/inputs.py
--rw-r--r--   0        0        0     6384 2023-05-15 01:20:26.922403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     1301 2023-05-15 01:20:26.926403 osintbuddy-0.0.2rc31.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      964 2023-05-15 01:20:26.926403 osintbuddy-0.0.2rc31.post1/tests/conftest.py
--rw-r--r--   0        0        0      664 2023-05-15 01:20:26.926403 osintbuddy-0.0.2rc31.post1/tests/test_methods.py
--rw-r--r--   0        0        0     6514 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc31.post1/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-05-15 01:20:39.617907 osintbuddy-0.0.2rc32.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      447 2023-05-15 01:20:39.617907 osintbuddy-0.0.2rc32.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-05-15 01:20:39.617907 osintbuddy-0.0.2rc32.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      314 2023-05-15 01:20:39.617907 osintbuddy-0.0.2rc32.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1807 2023-05-15 01:20:39.617907 osintbuddy-0.0.2rc32.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/Dockerfile
+-rw-r--r--   0        0        0       11 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/LICENSE
+-rw-r--r--   0        0        0     4663 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/README.md
+-rw-r--r--   0        0        0       47 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6665 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/README.md
+-rw-r--r--   0        0        0      374 2023-05-15 01:20:43.657982 osintbuddy-0.0.2rc32.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      151 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/errors.py
+-rw-r--r--   0        0        0      527 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/examples/ip-plugin.py
+-rw-r--r--   0        0        0      206 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/manager.py
+-rw-r--r--   0        0        0      358 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/node/__init__.py
+-rw-r--r--   0        0        0     1302 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/node/base.py
+-rw-r--r--   0        0        0     2989 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/node/displays.py
+-rw-r--r--   0        0        0     4099 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/node/inputs.py
+-rw-r--r--   0        0        0     6384 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     1301 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/tests/conftest.py
+-rw-r--r--   0        0        0      664 2023-05-15 01:20:39.621907 osintbuddy-0.0.2rc32.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     6514 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc32.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.2rc31.post1/.gitignore` & `osintbuddy-0.0.2rc32.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.2rc32.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/README.md` & `osintbuddy-0.0.2rc32.post1/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/docs/pylint.md` & `osintbuddy-0.0.2rc32.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/pyproject.toml` & `osintbuddy-0.0.2rc32.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 
 [project.optional-dependencies]
 spark = [
     "pyspark>=3.0.0"
 ]
 test = [
-    "bandit[toml]==1.7.4",
+    "bandit[toml]==1.7.5",
     "black==23.1.0",
     "check-manifest==0.48",
     "flake8-bugbear==23.5.9",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8",
     "flake8-pyproject",
```

### Comparing `osintbuddy-0.0.2rc31.post1/src/osintbuddy/examples/ip-plugin.py` & `osintbuddy-0.0.2rc32.post1/src/osintbuddy/examples/ip-plugin.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/src/osintbuddy/node/base.py` & `osintbuddy-0.0.2rc32.post1/src/osintbuddy/node/base.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/src/osintbuddy/node/displays.py` & `osintbuddy-0.0.2rc32.post1/src/osintbuddy/node/displays.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/src/osintbuddy/node/inputs.py` & `osintbuddy-0.0.2rc32.post1/src/osintbuddy/node/inputs.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/src/osintbuddy/plugins.py` & `osintbuddy-0.0.2rc32.post1/src/osintbuddy/plugins.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/src/osintbuddy/utils.py` & `osintbuddy-0.0.2rc32.post1/src/osintbuddy/utils.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/tests/conftest.py` & `osintbuddy-0.0.2rc32.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/tests/test_methods.py` & `osintbuddy-0.0.2rc32.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc31.post1/PKG-INFO` & `osintbuddy-0.0.2rc32.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.2rc31.post1
+Version: 0.0.2rc32.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
 Author-email: jerlendds <jerlendsdev@proton.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: pyspark>=3.0.0 ; extra == "spark"
-Requires-Dist: bandit[toml]==1.7.4 ; extra == "test"
+Requires-Dist: bandit[toml]==1.7.5 ; extra == "test"
 Requires-Dist: black==23.1.0 ; extra == "test"
 Requires-Dist: check-manifest==0.48 ; extra == "test"
 Requires-Dist: flake8-bugbear==23.5.9 ; extra == "test"
 Requires-Dist: flake8-docstrings ; extra == "test"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: flake8-pyproject ; extra == "test"
```

