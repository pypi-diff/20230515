# Comparing `tmp/dissect.xfs-3.5.dev4.tar.gz` & `tmp/dissect.xfs-3.5.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.xfs-3.5.dev4.tar", last modified: Thu Apr 13 07:42:29 2023, max compression
+gzip compressed data, was "dissect.xfs-3.5.dev5.tar", last modified: Mon May 15 12:48:48 2023, max compression
```

## Comparing `dissect.xfs-3.5.dev4.tar` & `dissect.xfs-3.5.dev5.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.413170 dissect.xfs-3.5.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-13 07:42:29.413170 dissect.xfs-3.5.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.405170 dissect.xfs-3.5.dev4/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.409170 dissect.xfs-3.5.dev4/dissect/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/dissect/xfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41820 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/dissect/xfs/c_xfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/dissect/xfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/dissect/xfs/xfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.409170 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-13 07:42:15.000000 dissect.xfs-3.5.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:42:29.413170 dissect.xfs-3.5.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.409170 dissect.xfs-3.5.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.413170 dissect.xfs-3.5.dev4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_bigtime.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    45520 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42015 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/test_xfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.197005 dissect.xfs-3.5.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-15 12:48:48.193005 dissect.xfs-3.5.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.181005 dissect.xfs-3.5.dev5/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.189005 dissect.xfs-3.5.dev5/dissect/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/dissect/xfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41820 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/dissect/xfs/c_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/dissect/xfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/dissect/xfs/xfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.185005 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:48.000000 dissect.xfs-3.5.dev5/dissect.xfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 12:48:38.000000 dissect.xfs-3.5.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:48.197005 dissect.xfs-3.5.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.189005 dissect.xfs-3.5.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.193005 dissect.xfs-3.5.dev5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_bigtime.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    45520 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42015 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:48.193005 dissect.xfs-3.5.dev5/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tests/test_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:34.000000 dissect.xfs-3.5.dev5/tox.ini
```

### Comparing `dissect.xfs-3.5.dev4/LICENSE` & `dissect.xfs-3.5.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/PKG-INFO` & `dissect.xfs-3.5.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.5.dev4
+Version: 3.5.dev5
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.xfs-3.5.dev4/README.md` & `dissect.xfs-3.5.dev5/README.md`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/dissect/xfs/c_xfs.py` & `dissect.xfs-3.5.dev5/dissect/xfs/c_xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/dissect/xfs/xfs.py` & `dissect.xfs-3.5.dev5/dissect/xfs/xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/dissect.xfs.egg-info/PKG-INFO` & `dissect.xfs-3.5.dev5/dissect.xfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.5.dev4
+Version: 3.5.dev5
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.xfs-3.5.dev4/dissect.xfs.egg-info/SOURCES.txt` & `dissect.xfs-3.5.dev5/dissect.xfs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,11 @@
 tests/conftest.py
 tests/test_xfs.py
 tests/data/xfs.bin.gz
 tests/data/xfs_bigtime.bin.gz
 tests/data/xfs_sparse.bin.gz
 tests/data/xfs_symlink_test1.bin.gz
 tests/data/xfs_symlink_test2.bin.gz
-tests/data/xfs_symlink_test3.bin.gz
+tests/data/xfs_symlink_test3.bin.gz
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.xfs-3.5.dev4/pyproject.toml` & `dissect.xfs-3.5.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/tests/data/xfs.bin.gz` & `dissect.xfs-3.5.dev5/tests/data/xfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/tests/data/xfs_bigtime.bin.gz` & `dissect.xfs-3.5.dev5/tests/data/xfs_bigtime.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/tests/data/xfs_sparse.bin.gz` & `dissect.xfs-3.5.dev5/tests/data/xfs_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test1.bin.gz` & `dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test2.bin.gz` & `dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test3.bin.gz` & `dissect.xfs-3.5.dev5/tests/data/xfs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/tests/test_xfs.py` & `dissect.xfs-3.5.dev5/tests/test_xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.5.dev4/tox.ini` & `dissect.xfs-3.5.dev5/tox.ini`

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

