# Comparing `tmp/dissect.cim-3.5.dev1.tar.gz` & `tmp/dissect.cim-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.cim-3.5.dev1.tar", last modified: Thu Mar 16 13:02:28 2023, max compression
+gzip compressed data, was "dissect.cim-3.6.dev1.tar", last modified: Mon May 15 12:47:26 2023, max compression
```

## Comparing `dissect.cim-3.5.dev1.tar` & `dissect.cim-3.6.dev1.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:28.594102 dissect.cim-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-16 13:02:28.594102 dissect.cim-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:28.570102 dissect.cim-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:28.582102 dissect.cim-3.5.dev1/dissect/cim/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/c_cim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/cim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/dissect/cim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:28.574102 dissect.cim-3.5.dev1/dissect.cim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-16 13:02:28.000000 dissect.cim-3.5.dev1/dissect.cim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-16 13:02:28.000000 dissect.cim-3.5.dev1/dissect.cim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:02:28.000000 dissect.cim-3.5.dev1/dissect.cim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:02:28.000000 dissect.cim-3.5.dev1/dissect.cim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:02:28.000000 dissect.cim-3.5.dev1/dissect.cim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-16 13:02:18.000000 dissect.cim-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:02:28.594102 dissect.cim-3.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:28.582102 dissect.cim-3.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:14.000000 dissect.cim-3.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:28.586102 dissect.cim-3.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2018815 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/tests/data/INDEX.BTR.gz
--rw-r--r--   0 runner    (1001) docker     (123)    29367 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/tests/data/MAPPING1.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (123)    29375 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/tests/data/MAPPING2.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/tests/data/MAPPING3.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (123)  4105816 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/tests/data/OBJECTS.DATA.gz
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/tests/test_cim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:02:13.000000 dissect.cim-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.220413 dissect.cim-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-15 12:47:26.220413 dissect.cim-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.208413 dissect.cim-3.6.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.212412 dissect.cim-3.6.dev1/dissect/cim/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/c_cim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/cim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/dissect/cim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.212412 dissect.cim-3.6.dev1/dissect.cim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-15 12:47:26.000000 dissect.cim-3.6.dev1/dissect.cim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 12:47:26.000000 dissect.cim-3.6.dev1/dissect.cim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:26.000000 dissect.cim-3.6.dev1/dissect.cim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:26.000000 dissect.cim-3.6.dev1/dissect.cim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:26.000000 dissect.cim-3.6.dev1/dissect.cim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-15 12:47:12.000000 dissect.cim-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:26.220413 dissect.cim-3.6.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.212412 dissect.cim-3.6.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.216412 dissect.cim-3.6.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2018815 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/data/INDEX.BTR.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    29367 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/data/MAPPING1.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    29375 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/data/MAPPING2.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/data/MAPPING3.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  4105816 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/data/OBJECTS.DATA.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.220413 dissect.cim-3.6.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tests/test_cim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:03.000000 dissect.cim-3.6.dev1/tox.ini
```

### Comparing `dissect.cim-3.5.dev1/LICENSE` & `dissect.cim-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/PKG-INFO` & `dissect.cim-3.6.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cim
-Version: 3.5.dev1
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for the Windows Common Information Model (CIM) database, used in the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cim
 Project-URL: repository, https://github.com/fox-it/dissect.cim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.cim-3.5.dev1/README.md` & `dissect.cim-3.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/dissect/cim/c_cim.py` & `dissect.cim-3.6.dev1/dissect/cim/c_cim.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/dissect/cim/cim.py` & `dissect.cim-3.6.dev1/dissect/cim/cim.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/dissect/cim/classes.py` & `dissect.cim-3.6.dev1/dissect/cim/classes.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/dissect/cim/index.py` & `dissect.cim-3.6.dev1/dissect/cim/index.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/dissect/cim/mappings.py` & `dissect.cim-3.6.dev1/dissect/cim/mappings.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/dissect/cim/objects.py` & `dissect.cim-3.6.dev1/dissect/cim/objects.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/dissect/cim/utils.py` & `dissect.cim-3.6.dev1/dissect/cim/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/dissect.cim.egg-info/PKG-INFO` & `dissect.cim-3.6.dev1/dissect.cim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cim
-Version: 3.5.dev1
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for the Windows Common Information Model (CIM) database, used in the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cim
 Project-URL: repository, https://github.com/fox-it/dissect.cim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.cim-3.5.dev1/dissect.cim.egg-info/SOURCES.txt` & `dissect.cim-3.6.dev1/dissect.cim.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_cim.py
 tests/data/INDEX.BTR.gz
 tests/data/MAPPING1.MAP.gz
 tests/data/MAPPING2.MAP.gz
 tests/data/MAPPING3.MAP.gz
-tests/data/OBJECTS.DATA.gz
+tests/data/OBJECTS.DATA.gz
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.cim-3.5.dev1/pyproject.toml` & `dissect.cim-3.6.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/tests/conftest.py` & `dissect.cim-3.6.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/tests/data/INDEX.BTR.gz` & `dissect.cim-3.6.dev1/tests/data/INDEX.BTR.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/tests/data/MAPPING1.MAP.gz` & `dissect.cim-3.6.dev1/tests/data/MAPPING1.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/tests/data/MAPPING2.MAP.gz` & `dissect.cim-3.6.dev1/tests/data/MAPPING2.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/tests/data/MAPPING3.MAP.gz` & `dissect.cim-3.6.dev1/tests/data/MAPPING3.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/tests/data/OBJECTS.DATA.gz` & `dissect.cim-3.6.dev1/tests/data/OBJECTS.DATA.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.5.dev1/tox.ini` & `dissect.cim-3.6.dev1/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -51,7 +51,27 @@
 
 [flake8]
 max-line-length = 120
 extend-ignore =
     # See https://github.com/PyCQA/pycodestyle/issues/373
     E203,
 statistics = True
+
+[testenv:docs-build]
+allowlist_externals = make
+deps =
+    sphinx
+    sphinx-autoapi
+    sphinx_argparse_cli
+    sphinx-copybutton
+    sphinx-design
+    furo
+commands =
+    make -C tests/docs clean
+    make -C tests/docs html
+
+[testenv:docs-linkcheck]
+allowlist_externals = make
+deps = {[testenv:docs-build]deps}
+commands =
+    make -C tests/docs clean
+    make -C tests/docs linkcheck
```

