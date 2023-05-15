# Comparing `tmp/dissect.extfs-3.5.dev2.tar.gz` & `tmp/dissect.extfs-3.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.extfs-3.5.dev2.tar", last modified: Tue Apr 11 14:16:10 2023, max compression
+gzip compressed data, was "dissect.extfs-3.5.dev3.tar", last modified: Mon May 15 12:47:58 2023, max compression
```

## Comparing `dissect.extfs-3.5.dev2.tar` & `dissect.extfs-3.5.dev3.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.531741 dissect.extfs-3.5.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-11 14:16:10.527741 dissect.extfs-3.5.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.519741 dissect.extfs-3.5.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.527741 dissect.extfs-3.5.dev2/dissect/extfs/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/c_jdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/extfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/dissect/extfs/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.523741 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 14:16:10.000000 dissect.extfs-3.5.dev2/dissect.extfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 14:16:00.000000 dissect.extfs-3.5.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:16:10.531741 dissect.extfs-3.5.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.527741 dissect.extfs-3.5.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-11 14:15:55.000000 dissect.extfs-3.5.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:16:10.527741 dissect.extfs-3.5.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tests/test_ext4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-11 14:15:56.000000 dissect.extfs-3.5.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.946386 dissect.extfs-3.5.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/dissect/extfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/c_jdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/extfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/dissect/extfs/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.946386 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:58.000000 dissect.extfs-3.5.dev3/dissect.extfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 12:47:42.000000 dissect.extfs-3.5.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:58.954386 dissect.extfs-3.5.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:33.000000 dissect.extfs-3.5.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:58.950386 dissect.extfs-3.5.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tests/test_ext4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:32.000000 dissect.extfs-3.5.dev3/tox.ini
```

### Comparing `dissect.extfs-3.5.dev2/LICENSE` & `dissect.extfs-3.5.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/PKG-INFO` & `dissect.extfs-3.5.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.5.dev2
+Version: 3.5.dev3
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.extfs-3.5.dev2/README.md` & `dissect.extfs-3.5.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/dissect/extfs/c_ext.py` & `dissect.extfs-3.5.dev3/dissect/extfs/c_ext.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/dissect/extfs/c_jdb2.py` & `dissect.extfs-3.5.dev3/dissect/extfs/c_jdb2.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/dissect/extfs/extfs.py` & `dissect.extfs-3.5.dev3/dissect/extfs/extfs.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/dissect/extfs/journal.py` & `dissect.extfs-3.5.dev3/dissect/extfs/journal.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/dissect.extfs.egg-info/PKG-INFO` & `dissect.extfs-3.5.dev3/dissect.extfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.5.dev2
+Version: 3.5.dev3
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.extfs-3.5.dev2/dissect.extfs.egg-info/SOURCES.txt` & `dissect.extfs-3.5.dev3/dissect.extfs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_ext4.py
 tests/data/ext4.bin.gz
 tests/data/ext4_sparse.bin.gz
 tests/data/ext4_symlink_test1.bin.gz
 tests/data/ext4_symlink_test2.bin.gz
-tests/data/ext4_symlink_test3.bin.gz
+tests/data/ext4_symlink_test3.bin.gz
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.extfs-3.5.dev2/pyproject.toml` & `dissect.extfs-3.5.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/tests/conftest.py` & `dissect.extfs-3.5.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/tests/data/ext4.bin.gz` & `dissect.extfs-3.5.dev3/tests/data/ext4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/tests/data/ext4_sparse.bin.gz` & `dissect.extfs-3.5.dev3/tests/data/ext4_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test1.bin.gz` & `dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test2.bin.gz` & `dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/tests/data/ext4_symlink_test3.bin.gz` & `dissect.extfs-3.5.dev3/tests/data/ext4_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/tests/test_ext4.py` & `dissect.extfs-3.5.dev3/tests/test_ext4.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.5.dev2/tox.ini` & `dissect.extfs-3.5.dev3/tox.ini`

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

