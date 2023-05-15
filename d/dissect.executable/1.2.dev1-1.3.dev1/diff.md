# Comparing `tmp/dissect.executable-1.2.dev1.tar.gz` & `tmp/dissect.executable-1.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.executable-1.2.dev1.tar", last modified: Thu Mar 16 13:03:34 2023, max compression
+gzip compressed data, was "dissect.executable-1.3.dev1.tar", last modified: Mon May 15 12:47:39 2023, max compression
```

## Comparing `dissect.executable-1.2.dev1.tar` & `dissect.executable-1.3.dev1.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.014502 dissect.executable-1.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-16 13:03:34.014502 dissect.executable-1.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.006502 dissect.executable-1.2.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.010502 dissect.executable-1.2.dev1/dissect/executable/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/dissect/executable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.010502 dissect.executable-1.2.dev1/dissect/executable/elf/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/dissect/executable/elf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/dissect/executable/elf/c_elf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/dissect/executable/elf/elf.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/dissect/executable/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.014502 dissect.executable-1.2.dev1/dissect/executable/macho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/dissect/executable/macho/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.014502 dissect.executable-1.2.dev1/dissect/executable/pe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/dissect/executable/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.010502 dissect.executable-1.2.dev1/dissect.executable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-16 13:03:33.000000 dissect.executable-1.2.dev1/dissect.executable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-16 13:03:34.000000 dissect.executable-1.2.dev1/dissect.executable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:03:33.000000 dissect.executable-1.2.dev1/dissect.executable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:03:33.000000 dissect.executable-1.2.dev1/dissect.executable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:03:33.000000 dissect.executable-1.2.dev1/dissect.executable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-16 13:03:21.000000 dissect.executable-1.2.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:03:34.014502 dissect.executable-1.2.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.014502 dissect.executable-1.2.dev1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:03:34.014502 dissect.executable-1.2.dev1/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16608 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tests/data/hello_world.out
--rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tests/data/hello_world.stripped.out
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tests/test_elf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tests/test_segment_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:03:15.000000 dissect.executable-1.2.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.952510 dissect.executable-1.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-15 12:47:39.952510 dissect.executable-1.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.944510 dissect.executable-1.3.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect/executable/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect/executable/elf/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/elf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/elf/c_elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/elf/elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect/executable/macho/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/macho/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect/executable/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/dissect/executable/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/dissect.executable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:39.000000 dissect.executable-1.3.dev1/dissect.executable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-15 12:47:30.000000 dissect.executable-1.3.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:39.952510 dissect.executable-1.3.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16608 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/data/hello_world.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/data/hello_world.stripped.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:39.948510 dissect.executable-1.3.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/test_segment_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:26.000000 dissect.executable-1.3.dev1/tox.ini
```

### Comparing `dissect.executable-1.2.dev1/LICENSE` & `dissect.executable-1.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/PKG-INFO` & `dissect.executable-1.3.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.executable
-Version: 1.2.dev1
+Version: 1.3.dev1
 Summary: A Dissect module implementing a parsers for various executable formats such as PE, ELF and Macho-O
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.executable
 Project-URL: repository, https://github.com/fox-it/dissect.executable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.executable-1.2.dev1/README.md` & `dissect.executable-1.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/dissect/executable/elf/c_elf.py` & `dissect.executable-1.3.dev1/dissect/executable/elf/c_elf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/dissect/executable/elf/elf.py` & `dissect.executable-1.3.dev1/dissect/executable/elf/elf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/dissect.executable.egg-info/PKG-INFO` & `dissect.executable-1.3.dev1/dissect.executable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.executable
-Version: 1.2.dev1
+Version: 1.3.dev1
 Summary: A Dissect module implementing a parsers for various executable formats such as PE, ELF and Macho-O
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.executable
 Project-URL: repository, https://github.com/fox-it/dissect.executable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.executable-1.2.dev1/dissect.executable.egg-info/SOURCES.txt` & `dissect.executable-1.3.dev1/dissect.executable.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 tests/test_dump.py
 tests/test_elf.py
 tests/test_section.py
 tests/test_segment.py
 tests/test_segment_table.py
 tests/util.py
 tests/data/hello_world.out
-tests/data/hello_world.stripped.out
+tests/data/hello_world.stripped.out
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.executable-1.2.dev1/pyproject.toml` & `dissect.executable-1.3.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/tests/data/hello_world.out` & `dissect.executable-1.3.dev1/tests/data/hello_world.out`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/tests/data/hello_world.stripped.out` & `dissect.executable-1.3.dev1/tests/data/hello_world.stripped.out`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/tests/test_dump.py` & `dissect.executable-1.3.dev1/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/tests/test_section.py` & `dissect.executable-1.3.dev1/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/tests/test_segment.py` & `dissect.executable-1.3.dev1/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/tests/test_segment_table.py` & `dissect.executable-1.3.dev1/tests/test_segment_table.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.2.dev1/tox.ini` & `dissect.executable-1.3.dev1/tox.ini`

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

