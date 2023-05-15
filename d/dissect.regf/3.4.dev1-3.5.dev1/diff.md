# Comparing `tmp/dissect.regf-3.4.dev1.tar.gz` & `tmp/dissect.regf-3.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.regf-3.4.dev1.tar", last modified: Thu Mar 16 13:04:30 2023, max compression
+gzip compressed data, was "dissect.regf-3.5.dev1.tar", last modified: Mon May 15 12:48:13 2023, max compression
```

## Comparing `dissect.regf-3.4.dev1.tar` & `dissect.regf-3.5.dev1.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:30.252513 dissect.regf-3.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-16 13:04:30.252513 dissect.regf-3.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:30.236513 dissect.regf-3.4.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:30.248513 dissect.regf-3.4.dev1/dissect/regf/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/dissect/regf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/dissect/regf/c_regf.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/dissect/regf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/dissect/regf/regf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:30.244512 dissect.regf-3.4.dev1/dissect.regf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-16 13:04:30.000000 dissect.regf-3.4.dev1/dissect.regf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-16 13:04:30.000000 dissect.regf-3.4.dev1/dissect.regf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:04:30.000000 dissect.regf-3.4.dev1/dissect.regf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:04:30.000000 dissect.regf-3.4.dev1/dissect.regf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:04:30.000000 dissect.regf-3.4.dev1/dissect.regf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:30.248513 dissect.regf-3.4.dev1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/examples/walkhive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-16 13:04:20.000000 dissect.regf-3.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:04:30.252513 dissect.regf-3.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:30.252513 dissect.regf-3.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:30.252513 dissect.regf-3.4.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1969086 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/tests/data/SYSTEM.gz
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/tests/test_regf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:04:14.000000 dissect.regf-3.4.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:13.459190 dissect.regf-3.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-15 12:48:13.459190 dissect.regf-3.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:13.451189 dissect.regf-3.5.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:13.455190 dissect.regf-3.5.dev1/dissect/regf/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/dissect/regf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/dissect/regf/c_regf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/dissect/regf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/dissect/regf/regf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:13.455190 dissect.regf-3.5.dev1/dissect.regf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-15 12:48:13.000000 dissect.regf-3.5.dev1/dissect.regf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-15 12:48:13.000000 dissect.regf-3.5.dev1/dissect.regf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:13.000000 dissect.regf-3.5.dev1/dissect.regf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:13.000000 dissect.regf-3.5.dev1/dissect.regf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:13.000000 dissect.regf-3.5.dev1/dissect.regf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:13.455190 dissect.regf-3.5.dev1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/examples/walkhive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 12:48:04.000000 dissect.regf-3.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:13.459190 dissect.regf-3.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:13.459190 dissect.regf-3.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:13.459190 dissect.regf-3.5.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1969086 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/tests/data/SYSTEM.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:13.459190 dissect.regf-3.5.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/tests/test_regf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:00.000000 dissect.regf-3.5.dev1/tox.ini
```

### Comparing `dissect.regf-3.4.dev1/LICENSE` & `dissect.regf-3.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.4.dev1/PKG-INFO` & `dissect.regf-3.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.regf
-Version: 3.4.dev1
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.regf
 Project-URL: repository, https://github.com/fox-it/dissect.regf
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.regf-3.4.dev1/README.md` & `dissect.regf-3.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.4.dev1/dissect/regf/c_regf.py` & `dissect.regf-3.5.dev1/dissect/regf/c_regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.4.dev1/dissect/regf/regf.py` & `dissect.regf-3.5.dev1/dissect/regf/regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.4.dev1/dissect.regf.egg-info/PKG-INFO` & `dissect.regf-3.5.dev1/dissect.regf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.regf
-Version: 3.4.dev1
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.regf
 Project-URL: repository, https://github.com/fox-it/dissect.regf
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.regf-3.4.dev1/pyproject.toml` & `dissect.regf-3.5.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.4.dev1/tests/data/SYSTEM.gz` & `dissect.regf-3.5.dev1/tests/data/SYSTEM.gz`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.4.dev1/tests/test_regf.py` & `dissect.regf-3.5.dev1/tests/test_regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.4.dev1/tox.ini` & `dissect.regf-3.5.dev1/tox.ini`

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

