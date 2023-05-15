# Comparing `tmp/pytest-subtests-0.8.0.tar.gz` & `tmp/pytest-subtests-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-subtests-0.8.0.tar", last modified: Thu May 26 11:15:36 2022, max compression
+gzip compressed data, was "pytest-subtests-0.9.0.tar", last modified: Fri Oct 28 16:27:31 2022, max compression
```

## Comparing `pytest-subtests-0.8.0.tar` & `pytest-subtests-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 11:15:36.259377 pytest-subtests-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 11:15:36.251377 pytest-subtests-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 11:15:36.255377 pytest-subtests-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6176 2022-05-26 11:15:36.259377 pytest-subtests-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5136 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 11:15:36.259377 pytest-subtests-0.8.0/pytest_subtests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6176 2022-05-26 11:15:35.000000 pytest-subtests-0.8.0/pytest_subtests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-05-26 11:15:36.000000 pytest-subtests-0.8.0/pytest_subtests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 11:15:35.000000 pytest-subtests-0.8.0/pytest_subtests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-26 11:15:35.000000 pytest-subtests-0.8.0/pytest_subtests.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-26 11:15:36.000000 pytest-subtests-0.8.0/pytest_subtests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-26 11:15:36.000000 pytest-subtests-0.8.0/pytest_subtests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7369 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/pytest_subtests.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-26 11:15:36.259377 pytest-subtests-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 11:15:36.259377 pytest-subtests-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    14780 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/tests/test_subtests.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-26 11:15:19.000000 pytest-subtests-0.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 16:27:31.337328 pytest-subtests-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 16:27:31.337328 pytest-subtests-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 16:27:31.337328 pytest-subtests-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6177 2022-10-28 16:27:31.337328 pytest-subtests-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5136 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 16:27:31.337328 pytest-subtests-0.9.0/pytest_subtests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6177 2022-10-28 16:27:31.000000 pytest-subtests-0.9.0/pytest_subtests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-28 16:27:31.000000 pytest-subtests-0.9.0/pytest_subtests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 16:27:31.000000 pytest-subtests-0.9.0/pytest_subtests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-28 16:27:31.000000 pytest-subtests-0.9.0/pytest_subtests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-28 16:27:31.000000 pytest-subtests-0.9.0/pytest_subtests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-28 16:27:31.000000 pytest-subtests-0.9.0/pytest_subtests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7254 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/pytest_subtests.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-28 16:27:31.337328 pytest-subtests-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 16:27:31.337328 pytest-subtests-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14967 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/tests/test_subtests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-28 16:27:21.000000 pytest-subtests-0.9.0/tox.ini
```

### Comparing `pytest-subtests-0.8.0/.github/workflows/deploy.yml` & `pytest-subtests-0.9.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `pytest-subtests-0.8.0/.github/workflows/main.yml` & `pytest-subtests-0.9.0/.github/workflows/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -14,20 +14,21 @@
       fail-fast: false
       matrix:
         name: [
           "windows-py37",
           "windows-py38",
           "windows-py39",
           "windows-py310",
+          "windows-py311",
 
-          "ubuntu-py36",
           "ubuntu-py37",
           "ubuntu-py38",
           "ubuntu-py39",
           "ubuntu-py310",
+          "ubuntu-py311",
         ]
 
         include:
           - name: "windows-py37"
             python: "3.7"
             os: windows-latest
             tox_env: "py37"
@@ -39,19 +40,19 @@
             python: "3.9"
             os: windows-latest
             tox_env: "py39"
           - name: "windows-py310"
             python: "3.10"
             os: windows-latest
             tox_env: "py310"
+          - name: "windows-py311"
+            python: "3.11-dev"
+            os: windows-latest
+            tox_env: "py311"
 
-          - name: "ubuntu-py36"
-            python: "3.6"
-            os: ubuntu-latest
-            tox_env: "py36"
           - name: "ubuntu-py37"
             python: "3.7"
             os: ubuntu-latest
             tox_env: "py37"
           - name: "ubuntu-py38"
             python: "3.8"
             os: ubuntu-latest
@@ -60,19 +61,23 @@
             python: "3.9"
             os: ubuntu-latest
             tox_env: "py39"
           - name: "ubuntu-py310"
             python: "3.10"
             os: ubuntu-latest
             tox_env: "py310"
+          - name: "ubuntu-py311"
+            python: "3.11-dev"
+            os: ubuntu-latest
+            tox_env: "py311"
 
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v2
     - name: Set up Python
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python }}
     - name: Install tox
       run: |
         python -m pip install --upgrade pip
         python -m pip install --upgrade tox setuptools
     - name: Test
```

### Comparing `pytest-subtests-0.8.0/.gitignore` & `pytest-subtests-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-subtests-0.8.0/.pre-commit-config.yaml` & `pytest-subtests-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-subtests-0.8.0/CHANGELOG.rst` & `pytest-subtests-0.9.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGELOG
 =========
 
+0.9.0 (2022-10-28)
+------------------
+
+* Python 3.11 is officially supported.
+* Dropped support for Python 3.6.
+
 0.8.0 (2022-05-26)
 ------------------
 
 * Now passing subtests are shown in the test run summary at the end (for example: ``10 failed, 1 passed, 10 subtests passed in 0.10s``) (`#70`_).
 
 .. _#70: https://github.com/pytest-dev/pytest-subtests/pull/70
```

### Comparing `pytest-subtests-0.8.0/LICENSE` & `pytest-subtests-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-subtests-0.8.0/PKG-INFO` & `pytest-subtests-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: pytest-subtests
-Version: 0.8.0
+Version: 0.9.0
 Summary: unittest subTest() support and subtests fixture
 Home-page: https://github.com/pytest-dev/pytest-subtests
 Author: Bruno Oliveira
 Author-email: nicoddemus@gmail.com
 Maintainer: Bruno Oliveira
 Maintainer-email: nicoddemus@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 ===============
 pytest-subtests
 ===============
 
 unittest ``subTest()`` support and ``subtests`` fixture.
```

### Comparing `pytest-subtests-0.8.0/README.rst` & `pytest-subtests-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-subtests-0.8.0/RELEASING.rst` & `pytest-subtests-0.9.0/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `pytest-subtests-0.8.0/pytest_subtests.egg-info/PKG-INFO` & `pytest-subtests-0.9.0/pytest_subtests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: pytest-subtests
-Version: 0.8.0
+Version: 0.9.0
 Summary: unittest subTest() support and subtests fixture
 Home-page: https://github.com/pytest-dev/pytest-subtests
 Author: Bruno Oliveira
 Author-email: nicoddemus@gmail.com
 Maintainer: Bruno Oliveira
 Maintainer-email: nicoddemus@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 ===============
 pytest-subtests
 ===============
 
 unittest ``subTest()`` support and ``subtests`` fixture.
```

### Comparing `pytest-subtests-0.8.0/pytest_subtests.py` & `pytest-subtests-0.9.0/pytest_subtests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-import sys
 import time
 from contextlib import contextmanager
+from contextlib import nullcontext
 
 import attr
 import pytest
 from _pytest._code import ExceptionInfo
 from _pytest.capture import CaptureFixture
 from _pytest.capture import FDCapture
 from _pytest.capture import SysCapture
 from _pytest.outcomes import OutcomeException
 from _pytest.reports import TestReport
 from _pytest.runner import CallInfo
 from _pytest.runner import check_interactive_exception
 from _pytest.unittest import TestCaseFunction
 
-if sys.version_info[:2] < (3, 7):
-
-    @contextmanager
-    def nullcontext():
-        yield
-
-else:
-    from contextlib import nullcontext
-
 
 @attr.s
 class SubTestContext:
     msg = attr.ib()
     kwargs = attr.ib()
```

### Comparing `pytest-subtests-0.8.0/setup.py` & `pytest-subtests-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     license="MIT",
     url="https://github.com/pytest-dev/pytest-subtests",
     description="unittest subTest() support and subtests fixture",
     long_description=long_description,
     py_modules=["pytest_subtests"],
     use_scm_version=True,
     setup_requires=["setuptools-scm", "setuptools>=40.0"],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=["pytest>=7.0"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],
     entry_points={"pytest11": ["subtests = pytest_subtests"]},
 )
```

### Comparing `pytest-subtests-0.8.0/tests/test_subtests.py` & `pytest-subtests-0.9.0/tests/test_subtests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 
 import pytest
 
+IS_PY311 = sys.version_info[:2] >= (3, 11)
+
 
 @pytest.mark.parametrize("mode", ["normal", "xdist"])
 class TestFixture:
     """
     Tests for ``subtests`` fixture.
     """
 
@@ -133,21 +135,22 @@
                 main()
         """
         )
 
     @pytest.mark.parametrize("runner", ["unittest", "pytest-normal", "pytest-xdist"])
     def test_simple_terminal_normal(self, simple_script, testdir, runner):
 
+        suffix = ".test_foo" if IS_PY311 else ""
         if runner == "unittest":
             result = testdir.run(sys.executable, simple_script)
             result.stderr.fnmatch_lines(
                 [
-                    "FAIL: test_foo (__main__.T) [custom] (i=1)",
+                    f"FAIL: test_foo (__main__.T{suffix}) [custom] (i=1)",
                     "AssertionError: 1 != 0",
-                    "FAIL: test_foo (__main__.T) [custom] (i=3)",
+                    f"FAIL: test_foo (__main__.T{suffix}) [custom] (i=3)",
                     "AssertionError: 1 != 0",
                     "Ran 1 test in *",
                     "FAILED (failures=2)",
                 ]
             )
         else:
             if runner == "pytest-normal":
@@ -167,22 +170,23 @@
                     "* 2 failed, 1 passed in *",
                 ]
             )
 
     @pytest.mark.parametrize("runner", ["unittest", "pytest-normal", "pytest-xdist"])
     def test_simple_terminal_verbose(self, simple_script, testdir, runner):
 
+        suffix = ".test_foo" if IS_PY311 else ""
         if runner == "unittest":
             result = testdir.run(sys.executable, simple_script, "-v")
             result.stderr.fnmatch_lines(
                 [
-                    "test_foo (__main__.T) ... ",
-                    "FAIL: test_foo (__main__.T) [custom] (i=1)",
+                    f"test_foo (__main__.T{suffix}) ... ",
+                    f"FAIL: test_foo (__main__.T{suffix}) [custom] (i=1)",
                     "AssertionError: 1 != 0",
-                    "FAIL: test_foo (__main__.T) [custom] (i=3)",
+                    f"FAIL: test_foo (__main__.T{suffix}) [custom] (i=3)",
                     "AssertionError: 1 != 0",
                     "Ran 1 test in *",
                     "FAILED (failures=2)",
                 ]
             )
         else:
             if runner == "pytest-normal":
```

