# Comparing `tmp/dissect.ffs-3.5.dev1.tar.gz` & `tmp/dissect.ffs-3.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ffs-3.5.dev1.tar", last modified: Tue Apr  4 16:10:54 2023, max compression
+gzip compressed data, was "dissect.ffs-3.5.dev2.tar", last modified: Mon May 15 12:47:56 2023, max compression
```

## Comparing `dissect.ffs-3.5.dev1.tar` & `dissect.ffs-3.5.dev2.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:10:54.961967 dissect.ffs-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-04 16:10:54.961967 dissect.ffs-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:10:54.957967 dissect.ffs-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:10:54.957967 dissect.ffs-3.5.dev1/dissect/ffs/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/dissect/ffs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/dissect/ffs/c_ffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/dissect/ffs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/dissect/ffs/ffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:10:54.957967 dissect.ffs-3.5.dev1/dissect.ffs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-04 16:10:54.000000 dissect.ffs-3.5.dev1/dissect.ffs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-04 16:10:54.000000 dissect.ffs-3.5.dev1/dissect.ffs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:10:54.000000 dissect.ffs-3.5.dev1/dissect.ffs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-04 16:10:54.000000 dissect.ffs-3.5.dev1/dissect.ffs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 16:10:54.000000 dissect.ffs-3.5.dev1/dissect.ffs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-04 16:10:43.000000 dissect.ffs-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 16:10:54.961967 dissect.ffs-3.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:10:54.957967 dissect.ffs-3.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:10:37.000000 dissect.ffs-3.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:10:54.961967 dissect.ffs-3.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/tests/data/ffs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/tests/data/ffs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/tests/data/ffs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/tests/data/ffs_symlink_test3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/tests/test_ffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 16:10:36.000000 dissect.ffs-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.666564 dissect.ffs-3.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.670564 dissect.ffs-3.5.dev2/dissect/ffs/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/dissect/ffs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/dissect/ffs/c_ffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/dissect/ffs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/dissect/ffs/ffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.670564 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:56.000000 dissect.ffs-3.5.dev2/dissect.ffs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-15 12:47:46.000000 dissect.ffs-3.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.670564 dissect.ffs-3.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/data/ffs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:56.674564 dissect.ffs-3.5.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tests/test_ffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:41.000000 dissect.ffs-3.5.dev2/tox.ini
```

### Comparing `dissect.ffs-3.5.dev1/LICENSE` & `dissect.ffs-3.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/PKG-INFO` & `dissect.ffs-3.5.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ffs
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ffs
 Project-URL: repository, https://github.com/fox-it/dissect.ffs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.ffs-3.5.dev1/README.md` & `dissect.ffs-3.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/dissect/ffs/c_ffs.py` & `dissect.ffs-3.5.dev2/dissect/ffs/c_ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/dissect/ffs/ffs.py` & `dissect.ffs-3.5.dev2/dissect/ffs/ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/dissect.ffs.egg-info/PKG-INFO` & `dissect.ffs-3.5.dev2/dissect.ffs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ffs
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ffs
 Project-URL: repository, https://github.com/fox-it/dissect.ffs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.ffs-3.5.dev1/pyproject.toml` & `dissect.ffs-3.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/tests/data/ffs.bin.gz` & `dissect.ffs-3.5.dev2/tests/data/ffs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/tests/data/ffs_symlink_test1.bin.gz` & `dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/tests/data/ffs_symlink_test2.bin.gz` & `dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/tests/data/ffs_symlink_test3.bin.gz` & `dissect.ffs-3.5.dev2/tests/data/ffs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/tests/test_ffs.py` & `dissect.ffs-3.5.dev2/tests/test_ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.5.dev1/tox.ini` & `dissect.ffs-3.5.dev2/tox.ini`

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

