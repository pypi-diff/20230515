# Comparing `tmp/dissect.squashfs-1.1.dev2.tar.gz` & `tmp/dissect.squashfs-1.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.squashfs-1.1.dev2.tar", last modified: Thu Mar 16 13:04:59 2023, max compression
+gzip compressed data, was "dissect.squashfs-1.2.dev1.tar", last modified: Mon May 15 12:48:29 2023, max compression
```

## Comparing `dissect.squashfs-1.1.dev2.tar` & `dissect.squashfs-1.2.dev1.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.422058 dissect.squashfs-1.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-16 13:04:59.422058 dissect.squashfs-1.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.418058 dissect.squashfs-1.1.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.422058 dissect.squashfs-1.1.dev2/dissect/squashfs/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/dissect/squashfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/dissect/squashfs/c_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/dissect/squashfs/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/dissect/squashfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/dissect/squashfs/squashfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.418058 dissect.squashfs-1.1.dev2/dissect.squashfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-16 13:04:59.000000 dissect.squashfs-1.1.dev2/dissect.squashfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-16 13:04:59.000000 dissect.squashfs-1.1.dev2/dissect.squashfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:04:59.000000 dissect.squashfs-1.1.dev2/dissect.squashfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-16 13:04:59.000000 dissect.squashfs-1.1.dev2/dissect.squashfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:04:59.000000 dissect.squashfs-1.1.dev2/dissect.squashfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-16 13:04:48.000000 dissect.squashfs-1.1.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:04:59.422058 dissect.squashfs-1.1.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.422058 dissect.squashfs-1.1.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:59.422058 dissect.squashfs-1.1.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/data/gzip-opts.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/data/gzip.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/data/lz4.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/data/lzma.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/data/lzo.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/data/xz.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/data/zstd.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tests/test_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-16 13:04:43.000000 dissect.squashfs-1.1.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.469721 dissect.squashfs-1.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-15 12:48:29.469721 dissect.squashfs-1.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.457721 dissect.squashfs-1.2.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.461721 dissect.squashfs-1.2.dev1/dissect/squashfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/c_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/dissect/squashfs/squashfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.461721 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:29.000000 dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-15 12:48:19.000000 dissect.squashfs-1.2.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:29.469721 dissect.squashfs-1.2.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.465721 dissect.squashfs-1.2.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.465721 dissect.squashfs-1.2.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/gzip-opts.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/gzip.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/lz4.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/lzma.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/lzo.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/xz.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/data/zstd.sqfs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:29.469721 dissect.squashfs-1.2.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tests/test_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-15 12:48:15.000000 dissect.squashfs-1.2.dev1/tox.ini
```

### Comparing `dissect.squashfs-1.1.dev2/LICENSE` & `dissect.squashfs-1.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/PKG-INFO` & `dissect.squashfs-1.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.1.dev2
+Version: 1.2.dev1
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.squashfs-1.1.dev2/README.md` & `dissect.squashfs-1.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/dissect/squashfs/c_squashfs.py` & `dissect.squashfs-1.2.dev1/dissect/squashfs/c_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/dissect/squashfs/compression.py` & `dissect.squashfs-1.2.dev1/dissect/squashfs/compression.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/dissect/squashfs/squashfs.py` & `dissect.squashfs-1.2.dev1/dissect/squashfs/squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/dissect.squashfs.egg-info/PKG-INFO` & `dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.1.dev2
+Version: 1.2.dev1
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.squashfs-1.1.dev2/dissect.squashfs.egg-info/SOURCES.txt` & `dissect.squashfs-1.2.dev1/dissect.squashfs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 tests/test_squashfs.py
 tests/data/gzip-opts.sqfs
 tests/data/gzip.sqfs
 tests/data/lz4.sqfs
 tests/data/lzma.sqfs
 tests/data/lzo.sqfs
 tests/data/xz.sqfs
-tests/data/zstd.sqfs
+tests/data/zstd.sqfs
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.squashfs-1.1.dev2/pyproject.toml` & `dissect.squashfs-1.2.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/conftest.py` & `dissect.squashfs-1.2.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/data/gzip-opts.sqfs` & `dissect.squashfs-1.2.dev1/tests/data/gzip-opts.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/data/gzip.sqfs` & `dissect.squashfs-1.2.dev1/tests/data/gzip.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/data/lz4.sqfs` & `dissect.squashfs-1.2.dev1/tests/data/lz4.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/data/lzma.sqfs` & `dissect.squashfs-1.2.dev1/tests/data/lzma.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/data/lzo.sqfs` & `dissect.squashfs-1.2.dev1/tests/data/lzo.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/data/xz.sqfs` & `dissect.squashfs-1.2.dev1/tests/data/xz.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/data/zstd.sqfs` & `dissect.squashfs-1.2.dev1/tests/data/zstd.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tests/test_squashfs.py` & `dissect.squashfs-1.2.dev1/tests/test_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.1.dev2/tox.ini` & `dissect.squashfs-1.2.dev1/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -52,7 +52,27 @@
 
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

