# Comparing `tmp/dissect.vmfs-3.4.dev1.tar.gz` & `tmp/dissect.vmfs-3.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.vmfs-3.4.dev1.tar", last modified: Thu Mar 16 13:05:22 2023, max compression
+gzip compressed data, was "dissect.vmfs-3.5.dev1.tar", last modified: Mon May 15 12:48:39 2023, max compression
```

## Comparing `dissect.vmfs-3.4.dev1.tar` & `dissect.vmfs-3.5.dev1.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.421532 dissect.vmfs-3.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-16 13:05:22.421532 dissect.vmfs-3.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.405532 dissect.vmfs-3.4.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.417532 dissect.vmfs-3.4.dev1/dissect/vmfs/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/dissect/vmfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/dissect/vmfs/c_vmfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/dissect/vmfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/dissect/vmfs/lvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/dissect/vmfs/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    27978 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/dissect/vmfs/vmfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.413532 dissect.vmfs-3.4.dev1/dissect.vmfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-16 13:05:22.000000 dissect.vmfs-3.4.dev1/dissect.vmfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-16 13:05:22.000000 dissect.vmfs-3.4.dev1/dissect.vmfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:05:22.000000 dissect.vmfs-3.4.dev1/dissect.vmfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:05:22.000000 dissect.vmfs-3.4.dev1/dissect.vmfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:05:22.000000 dissect.vmfs-3.4.dev1/dissect.vmfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-16 13:05:11.000000 dissect.vmfs-3.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:05:22.421532 dissect.vmfs-3.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.417532 dissect.vmfs-3.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:22.421532 dissect.vmfs-3.4.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   531458 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/tests/data/vmfs5.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1054739 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/tests/data/vmfs6.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/tests/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/tests/test_lvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/tests/test_vmfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:05:05.000000 dissect.vmfs-3.4.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.453759 dissect.vmfs-3.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-15 12:48:39.453759 dissect.vmfs-3.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.445759 dissect.vmfs-3.5.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.449759 dissect.vmfs-3.5.dev1/dissect/vmfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/c_vmfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/lvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27978 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/dissect/vmfs/vmfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.445759 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:39.000000 dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 12:48:29.000000 dissect.vmfs-3.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:39.453759 dissect.vmfs-3.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.449759 dissect.vmfs-3.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.449759 dissect.vmfs-3.5.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   531458 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/data/vmfs5.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1054739 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/data/vmfs6.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:39.453759 dissect.vmfs-3.5.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/test_lvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tests/test_vmfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:25.000000 dissect.vmfs-3.5.dev1/tox.ini
```

### Comparing `dissect.vmfs-3.4.dev1/LICENSE` & `dissect.vmfs-3.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/PKG-INFO` & `dissect.vmfs-3.5.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.vmfs
-Version: 3.4.dev1
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.vmfs
 Project-URL: repository, https://github.com/fox-it/dissect.vmfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.vmfs-3.4.dev1/README.md` & `dissect.vmfs-3.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/dissect/vmfs/c_vmfs.py` & `dissect.vmfs-3.5.dev1/dissect/vmfs/c_vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/dissect/vmfs/lvm.py` & `dissect.vmfs-3.5.dev1/dissect/vmfs/lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/dissect/vmfs/resource.py` & `dissect.vmfs-3.5.dev1/dissect/vmfs/resource.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/dissect/vmfs/vmfs.py` & `dissect.vmfs-3.5.dev1/dissect/vmfs/vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/dissect.vmfs.egg-info/PKG-INFO` & `dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.vmfs
-Version: 3.4.dev1
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.vmfs
 Project-URL: repository, https://github.com/fox-it/dissect.vmfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.vmfs-3.4.dev1/dissect.vmfs.egg-info/SOURCES.txt` & `dissect.vmfs-3.5.dev1/dissect.vmfs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 dissect/vmfs/vmfs.py
 tests/__init__.py
 tests/conftest.py
 tests/test_address.py
 tests/test_lvm.py
 tests/test_vmfs.py
 tests/data/vmfs5.bin.gz
-tests/data/vmfs6.bin.gz
+tests/data/vmfs6.bin.gz
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.vmfs-3.4.dev1/pyproject.toml` & `dissect.vmfs-3.5.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/tests/data/vmfs5.bin.gz` & `dissect.vmfs-3.5.dev1/tests/data/vmfs5.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/tests/data/vmfs6.bin.gz` & `dissect.vmfs-3.5.dev1/tests/data/vmfs6.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/tests/test_address.py` & `dissect.vmfs-3.5.dev1/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/tests/test_lvm.py` & `dissect.vmfs-3.5.dev1/tests/test_lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/tests/test_vmfs.py` & `dissect.vmfs-3.5.dev1/tests/test_vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.4.dev1/tox.ini` & `dissect.vmfs-3.5.dev1/tox.ini`

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

