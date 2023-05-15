# Comparing `tmp/legend_testdata-0.4.1.tar.gz` & `tmp/legend_testdata-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_testdata-0.4.1.tar", last modified: Thu Sep 22 13:29:14 2022, max compression
+gzip compressed data, was "legend_testdata-0.4.2.tar", last modified: Mon Oct 17 09:38:58 2022, max compression
```

## Comparing `legend_testdata-0.4.1.tar` & `legend_testdata-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:29:14.991636 legend_testdata-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:29:14.987636 legend_testdata-0.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:29:14.987636 legend_testdata-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/.github/workflows/distribution.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-09-22 13:29:14.991636 legend_testdata-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-22 13:29:14.991636 legend_testdata-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:29:14.987636 legend_testdata-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:29:14.987636 legend_testdata-0.4.1/src/legend_testdata/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/src/legend_testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-22 13:29:14.000000 legend_testdata-0.4.1/src/legend_testdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/src/legend_testdata/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:29:14.987636 legend_testdata-0.4.1/src/legend_testdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-09-22 13:29:14.000000 legend_testdata-0.4.1/src/legend_testdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-22 13:29:14.000000 legend_testdata-0.4.1/src/legend_testdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 13:29:14.000000 legend_testdata-0.4.1/src/legend_testdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 13:29:14.000000 legend_testdata-0.4.1/src/legend_testdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-22 13:29:14.000000 legend_testdata-0.4.1/src/legend_testdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-22 13:29:14.000000 legend_testdata-0.4.1/src/legend_testdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:29:14.987636 legend_testdata-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-22 13:29:04.000000 legend_testdata-0.4.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:58.043940 legend_testdata-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-10-17 09:38:48.000000 legend_testdata-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-10-17 09:38:58.043940 legend_testdata-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-10-17 09:38:48.000000 legend_testdata-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-10-17 09:38:48.000000 legend_testdata-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-10-17 09:38:58.043940 legend_testdata-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-17 09:38:48.000000 legend_testdata-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:58.043940 legend_testdata-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:58.043940 legend_testdata-0.4.2/src/legend_testdata/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-17 09:38:48.000000 legend_testdata-0.4.2/src/legend_testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-17 09:38:58.000000 legend_testdata-0.4.2/src/legend_testdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-10-17 09:38:48.000000 legend_testdata-0.4.2/src/legend_testdata/core.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:58.043940 legend_testdata-0.4.2/src/legend_testdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-10-17 09:38:58.000000 legend_testdata-0.4.2/src/legend_testdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-10-17 09:38:58.000000 legend_testdata-0.4.2/src/legend_testdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 09:38:58.000000 legend_testdata-0.4.2/src/legend_testdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 09:38:57.000000 legend_testdata-0.4.2/src/legend_testdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-17 09:38:58.000000 legend_testdata-0.4.2/src/legend_testdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-17 09:38:58.000000 legend_testdata-0.4.2/src/legend_testdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 09:38:58.043940 legend_testdata-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-10-17 09:38:48.000000 legend_testdata-0.4.2/tests/test_core.py
```

### Comparing `legend_testdata-0.4.1/LICENSE` & `legend_testdata-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_testdata-0.4.1/PKG-INFO` & `legend_testdata-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_testdata
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python package for accessing LEGEND test data
 Home-page: https://github.com/legend-exp/legend-testdata
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -34,19 +34,26 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-testdata-py?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-testdata-py)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-testdata-py?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-testdata-py?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/legend-testdata-py)
 
-Tiny Python package to access [LEGEND test data](https://github.com/legend-exp/legend-testdata). Usage:
+Tiny Python package to access [LEGEND test data](https://github.com/legend-exp/legend-testdata).
 
-```py
-from legend_testdata import LegendTestData
+Install (with pip):
+```console
+$ python -m pip install legend-testdata
+```
+
+Usage:
 
-ldata = LegendTestData()  # clone legend-exp/legend-testdata below /tmp
-ldata.checkout("968c9ba")  # optionally checkout a specific version
-ldata.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")  # get absolute path to test file
-ldata.reset()  # checkout default branch (main)
+```pycon
+>>> from legend_testdata import LegendTestData
+>>> ldata = LegendTestData()  # clone legend-exp/legend-testdata below /tmp
+>>> ldata.checkout("968c9ba")  # optionally checkout a specific version
+>>> ldata.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")  # get absolute path to test file
+'/tmp/legend-testdata-gipert/data/orca/fc/L200-comm-20220519-phy-geds.orca'
+>>> ldata.reset()  # checkout default branch (main)
 ```
 
 <sub>*This Python package layout is based on [pyproject-template](https://github.com/gipert/pyproject-template).*</sub>
```

### Comparing `legend_testdata-0.4.1/README.md` & `legend_testdata-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,26 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-testdata-py?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-testdata-py)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-testdata-py?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-testdata-py?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/legend-testdata-py)
 
-Tiny Python package to access [LEGEND test data](https://github.com/legend-exp/legend-testdata). Usage:
+Tiny Python package to access [LEGEND test data](https://github.com/legend-exp/legend-testdata).
 
-```py
-from legend_testdata import LegendTestData
+Install (with pip):
+```console
+$ python -m pip install legend-testdata
+```
+
+Usage:
 
-ldata = LegendTestData()  # clone legend-exp/legend-testdata below /tmp
-ldata.checkout("968c9ba")  # optionally checkout a specific version
-ldata.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")  # get absolute path to test file
-ldata.reset()  # checkout default branch (main)
+```pycon
+>>> from legend_testdata import LegendTestData
+>>> ldata = LegendTestData()  # clone legend-exp/legend-testdata below /tmp
+>>> ldata.checkout("968c9ba")  # optionally checkout a specific version
+>>> ldata.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")  # get absolute path to test file
+'/tmp/legend-testdata-gipert/data/orca/fc/L200-comm-20220519-phy-geds.orca'
+>>> ldata.reset()  # checkout default branch (main)
 ```
 
 <sub>*This Python package layout is based on [pyproject-template](https://github.com/gipert/pyproject-template).*</sub>
```

### Comparing `legend_testdata-0.4.1/setup.cfg` & `legend_testdata-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `legend_testdata-0.4.1/src/legend_testdata/core.py` & `legend_testdata-0.4.2/src/legend_testdata/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 log = logging.getLogger(__name__)
 
 
 class LegendTestData:
     def __init__(self):
         self._default_git_ref = "main"
-        self._repo_path = path.join(gettempdir(), "legend-testdata-" + getuser())
+        self._repo_path = os.getenv(
+            "LEGEND_TESTDATA", path.join(gettempdir(), "legend-testdata-" + getuser())
+        )
         self._repo: Repo = self._init_testdata_repo()
 
     def _init_testdata_repo(self):
 
         if not path.isdir(self._repo_path):
             os.mkdir(self._repo_path)
```

### Comparing `legend_testdata-0.4.1/src/legend_testdata.egg-info/PKG-INFO` & `legend_testdata-0.4.2/src/legend_testdata.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend-testdata
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python package for accessing LEGEND test data
 Home-page: https://github.com/legend-exp/legend-testdata
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -34,19 +34,26 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-testdata-py?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-testdata-py)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-testdata-py?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-testdata-py?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/legend-testdata-py)
 
-Tiny Python package to access [LEGEND test data](https://github.com/legend-exp/legend-testdata). Usage:
+Tiny Python package to access [LEGEND test data](https://github.com/legend-exp/legend-testdata).
 
-```py
-from legend_testdata import LegendTestData
+Install (with pip):
+```console
+$ python -m pip install legend-testdata
+```
+
+Usage:
 
-ldata = LegendTestData()  # clone legend-exp/legend-testdata below /tmp
-ldata.checkout("968c9ba")  # optionally checkout a specific version
-ldata.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")  # get absolute path to test file
-ldata.reset()  # checkout default branch (main)
+```pycon
+>>> from legend_testdata import LegendTestData
+>>> ldata = LegendTestData()  # clone legend-exp/legend-testdata below /tmp
+>>> ldata.checkout("968c9ba")  # optionally checkout a specific version
+>>> ldata.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")  # get absolute path to test file
+'/tmp/legend-testdata-gipert/data/orca/fc/L200-comm-20220519-phy-geds.orca'
+>>> ldata.reset()  # checkout default branch (main)
 ```
 
 <sub>*This Python package layout is based on [pyproject-template](https://github.com/gipert/pyproject-template).*</sub>
```

