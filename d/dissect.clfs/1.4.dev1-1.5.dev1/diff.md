# Comparing `tmp/dissect.clfs-1.4.dev1.tar.gz` & `tmp/dissect.clfs-1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.clfs-1.4.dev1.tar", last modified: Thu Mar 16 13:02:31 2023, max compression
+gzip compressed data, was "dissect.clfs-1.5.dev1.tar", last modified: Mon May 15 12:47:17 2023, max compression
```

## Comparing `dissect.clfs-1.4.dev1.tar` & `dissect.clfs-1.5.dev1.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:31.063036 dissect.clfs-1.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-16 13:02:31.063036 dissect.clfs-1.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:31.055036 dissect.clfs-1.4.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:31.059036 dissect.clfs-1.4.dev1/dissect/clfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/dissect/clfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/dissect/clfs/blf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/dissect/clfs/c_clfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/dissect/clfs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/dissect/clfs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:31.059036 dissect.clfs-1.4.dev1/dissect.clfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-16 13:02:31.000000 dissect.clfs-1.4.dev1/dissect.clfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-16 13:02:31.000000 dissect.clfs-1.4.dev1/dissect.clfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:02:31.000000 dissect.clfs-1.4.dev1/dissect.clfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-16 13:02:31.000000 dissect.clfs-1.4.dev1/dissect.clfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:02:31.000000 dissect.clfs-1.4.dev1/dissect.clfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-16 13:02:19.000000 dissect.clfs-1.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:02:31.063036 dissect.clfs-1.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:31.059036 dissect.clfs-1.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:02:31.063036 dissect.clfs-1.4.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    65536 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf
--rw-r--r--   0 runner    (1001) docker     (123)   524288 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/data/bad_control_record.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/data/control_record.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/data/invalid_control_record.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/test_control_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/test_record_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tests/test_validate_blf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:02:15.000000 dissect.clfs-1.4.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.511274 dissect.clfs-1.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:47:17.511274 dissect.clfs-1.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.491273 dissect.clfs-1.5.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.503274 dissect.clfs-1.5.dev1/dissect/clfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:01.000000 dissect.clfs-1.5.dev1/dissect/clfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/dissect/clfs/blf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/dissect/clfs/c_clfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/dissect/clfs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/dissect/clfs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.499274 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:47:17.000000 dissect.clfs-1.5.dev1/dissect.clfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 12:47:07.000000 dissect.clfs-1.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:47:17.511274 dissect.clfs-1.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.503274 dissect.clfs-1.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:01.000000 dissect.clfs-1.5.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.507274 dissect.clfs-1.5.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    65536 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf
+-rw-r--r--   0 runner    (1001) docker     (123)   524288 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/bad_control_record.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/control_record.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/data/invalid_control_record.blf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:17.511274 dissect.clfs-1.5.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/test_control_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/test_record_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tests/test_validate_blf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:47:00.000000 dissect.clfs-1.5.dev1/tox.ini
```

### Comparing `dissect.clfs-1.4.dev1/LICENSE` & `dissect.clfs-1.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/PKG-INFO` & `dissect.clfs-1.5.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.clfs
-Version: 1.4.dev1
+Version: 1.5.dev1
 Summary: A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.clfs
 Project-URL: repository, https://github.com/fox-it/dissect.clfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.clfs-1.4.dev1/README.md` & `dissect.clfs-1.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/dissect/clfs/blf.py` & `dissect.clfs-1.5.dev1/dissect/clfs/blf.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/dissect/clfs/c_clfs.py` & `dissect.clfs-1.5.dev1/dissect/clfs/c_clfs.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/dissect/clfs/container.py` & `dissect.clfs-1.5.dev1/dissect/clfs/container.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/dissect.clfs.egg-info/PKG-INFO` & `dissect.clfs-1.5.dev1/dissect.clfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.clfs
-Version: 1.4.dev1
+Version: 1.5.dev1
 Summary: A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.clfs
 Project-URL: repository, https://github.com/fox-it/dissect.clfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.clfs-1.4.dev1/dissect.clfs.egg-info/SOURCES.txt` & `dissect.clfs-1.5.dev1/dissect.clfs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,11 @@
 tests/test_control_record.py
 tests/test_record_header.py
 tests/test_validate_blf.py
 tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf
 tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms
 tests/data/bad_control_record.blf
 tests/data/control_record.blf
-tests/data/invalid_control_record.blf
+tests/data/invalid_control_record.blf
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.clfs-1.4.dev1/pyproject.toml` & `dissect.clfs-1.5.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/conftest.py` & `dissect.clfs-1.5.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf` & `dissect.clfs-1.5.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms` & `dissect.clfs-1.5.dev1/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/data/bad_control_record.blf` & `dissect.clfs-1.5.dev1/tests/data/bad_control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/data/control_record.blf` & `dissect.clfs-1.5.dev1/tests/data/control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/data/invalid_control_record.blf` & `dissect.clfs-1.5.dev1/tests/data/invalid_control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/test_container.py` & `dissect.clfs-1.5.dev1/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/test_control_record.py` & `dissect.clfs-1.5.dev1/tests/test_control_record.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tests/test_record_header.py` & `dissect.clfs-1.5.dev1/tests/test_record_header.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.4.dev1/tox.ini` & `dissect.clfs-1.5.dev1/tox.ini`

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

