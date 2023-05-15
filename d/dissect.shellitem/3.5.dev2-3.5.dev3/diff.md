# Comparing `tmp/dissect.shellitem-3.5.dev2.tar.gz` & `tmp/dissect.shellitem-3.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.shellitem-3.5.dev2.tar", last modified: Thu Apr 13 08:53:32 2023, max compression
+gzip compressed data, was "dissect.shellitem-3.5.dev3.tar", last modified: Mon May 15 12:48:25 2023, max compression
```

## Comparing `dissect.shellitem-3.5.dev2.tar` & `dissect.shellitem-3.5.dev3.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.744938 dissect.shellitem-3.5.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-13 08:53:32.744938 dissect.shellitem-3.5.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.732938 dissect.shellitem-3.5.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.736938 dissect.shellitem-3.5.dev2/dissect/shellitem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:17.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.736938 dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/c_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17611 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.740938 dissect.shellitem-3.5.dev2/dissect/shellitem/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:17.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/tools/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.736938 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-13 08:53:22.000000 dissect.shellitem-3.5.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:53:32.744938 dissect.shellitem-3.5.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.740938 dissect.shellitem-3.5.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:17.000000 dissect.shellitem-3.5.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.740938 dissect.shellitem-3.5.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/downloads.win81.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/local.directory.seven.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/modified_remote.file.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/remote.directory.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/remote.file.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.576348 dissect.shellitem-3.5.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.580348 dissect.shellitem-3.5.dev3/dissect/shellitem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.580348 dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/c_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17611 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.584348 dissect.shellitem-3.5.dev3/dissect/shellitem/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/dissect/shellitem/tools/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.580348 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:25.000000 dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-15 12:48:13.000000 dissect.shellitem-3.5.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.584348 dissect.shellitem-3.5.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/downloads.win81.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/local.directory.seven.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/modified_remote.file.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/remote.directory.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/data/remote.file.xp.lnk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.588348 dissect.shellitem-3.5.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tests/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:09.000000 dissect.shellitem-3.5.dev3/tox.ini
```

### Comparing `dissect.shellitem-3.5.dev2/LICENSE` & `dissect.shellitem-3.5.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/PKG-INFO` & `dissect.shellitem-3.5.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.5.dev2
+Version: 3.5.dev3
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.shellitem-3.5.dev2/README.md` & `dissect.shellitem-3.5.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/c_lnk.py` & `dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/c_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/lnk.py` & `dissect.shellitem-3.5.dev3/dissect/shellitem/lnk/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/dissect/shellitem/tools/lnk.py` & `dissect.shellitem-3.5.dev3/dissect/shellitem/tools/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/PKG-INFO` & `dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.5.dev2
+Version: 3.5.dev3
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/SOURCES.txt` & `dissect.shellitem-3.5.dev3/dissect.shellitem.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_lnk.py
 tests/data/downloads.win81.lnk
 tests/data/local.directory.seven.lnk
 tests/data/modified_remote.file.xp.lnk
 tests/data/remote.directory.xp.lnk
-tests/data/remote.file.xp.lnk
+tests/data/remote.file.xp.lnk
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.shellitem-3.5.dev2/pyproject.toml` & `dissect.shellitem-3.5.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/tests/conftest.py` & `dissect.shellitem-3.5.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/tests/data/downloads.win81.lnk` & `dissect.shellitem-3.5.dev3/tests/data/downloads.win81.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/tests/data/local.directory.seven.lnk` & `dissect.shellitem-3.5.dev3/tests/data/local.directory.seven.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/tests/data/modified_remote.file.xp.lnk` & `dissect.shellitem-3.5.dev3/tests/data/modified_remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/tests/data/remote.directory.xp.lnk` & `dissect.shellitem-3.5.dev3/tests/data/remote.directory.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/tests/data/remote.file.xp.lnk` & `dissect.shellitem-3.5.dev3/tests/data/remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/tests/test_lnk.py` & `dissect.shellitem-3.5.dev3/tests/test_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev2/tox.ini` & `dissect.shellitem-3.5.dev3/tox.ini`

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

