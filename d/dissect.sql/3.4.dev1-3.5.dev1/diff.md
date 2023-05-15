# Comparing `tmp/dissect.sql-3.4.dev1.tar.gz` & `tmp/dissect.sql-3.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.sql-3.4.dev1.tar", last modified: Thu Mar 16 13:04:46 2023, max compression
+gzip compressed data, was "dissect.sql-3.5.dev1.tar", last modified: Mon May 15 12:48:28 2023, max compression
```

## Comparing `dissect.sql-3.4.dev1.tar` & `dissect.sql-3.5.dev1.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:46.670327 dissect.sql-3.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-16 13:04:46.670327 dissect.sql-3.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:46.666326 dissect.sql-3.4.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:46.670327 dissect.sql-3.4.dev1/dissect/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/dissect/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/dissect/sql/c_sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/dissect/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/dissect/sql/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/dissect/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:46.670327 dissect.sql-3.4.dev1/dissect.sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-16 13:04:46.000000 dissect.sql-3.4.dev1/dissect.sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-16 13:04:46.000000 dissect.sql-3.4.dev1/dissect.sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:04:46.000000 dissect.sql-3.4.dev1/dissect.sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:04:46.000000 dissect.sql-3.4.dev1/dissect.sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:04:46.000000 dissect.sql-3.4.dev1/dissect.sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-16 13:04:35.000000 dissect.sql-3.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:04:46.670327 dissect.sql-3.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:46.670327 dissect.sql-3.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:46.670327 dissect.sql-3.4.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/tests/data/test.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/tests/test_default_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/tests/test_parse_table_columns_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/tests/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:04:31.000000 dissect.sql-3.4.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:28.485490 dissect.sql-3.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-15 12:48:28.485490 dissect.sql-3.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:28.481490 dissect.sql-3.5.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:28.481490 dissect.sql-3.5.dev1/dissect/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/dissect/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/dissect/sql/c_sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/dissect/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/dissect/sql/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/dissect/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:28.481490 dissect.sql-3.5.dev1/dissect.sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-15 12:48:28.000000 dissect.sql-3.5.dev1/dissect.sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-15 12:48:28.000000 dissect.sql-3.5.dev1/dissect.sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:28.000000 dissect.sql-3.5.dev1/dissect.sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:28.000000 dissect.sql-3.5.dev1/dissect.sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:28.000000 dissect.sql-3.5.dev1/dissect.sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 12:48:18.000000 dissect.sql-3.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:28.485490 dissect.sql-3.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:28.485490 dissect.sql-3.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:28.485490 dissect.sql-3.5.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/data/test.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:28.485490 dissect.sql-3.5.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/test_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/test_parse_table_columns_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:15.000000 dissect.sql-3.5.dev1/tox.ini
```

### Comparing `dissect.sql-3.4.dev1/LICENSE` & `dissect.sql-3.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/PKG-INFO` & `dissect.sql-3.5.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.sql
-Version: 3.4.dev1
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parsers for the SQLite database file format, commonly used by applications to store configuration data
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.sql
 Project-URL: repository, https://github.com/fox-it/dissect.sql
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.sql-3.4.dev1/README.md` & `dissect.sql-3.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/dissect/sql/c_sqlite3.py` & `dissect.sql-3.5.dev1/dissect/sql/c_sqlite3.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/dissect/sql/sqlite3.py` & `dissect.sql-3.5.dev1/dissect/sql/sqlite3.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/dissect/sql/utils.py` & `dissect.sql-3.5.dev1/dissect/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/dissect.sql.egg-info/PKG-INFO` & `dissect.sql-3.5.dev1/dissect.sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.sql
-Version: 3.4.dev1
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parsers for the SQLite database file format, commonly used by applications to store configuration data
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.sql
 Project-URL: repository, https://github.com/fox-it/dissect.sql
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.sql-3.4.dev1/dissect.sql.egg-info/SOURCES.txt` & `dissect.sql-3.5.dev1/dissect.sql.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 dissect/sql/utils.py
 tests/__init__.py
 tests/conftest.py
 tests/test_default_values.py
 tests/test_parse_table_columns_constraints.py
 tests/test_row.py
 tests/test_sqlite.py
-tests/data/test.sqlite
+tests/data/test.sqlite
+tests/docs/Makefile
+tests/docs/conf.py
+tests/docs/index.rst
```

### Comparing `dissect.sql-3.4.dev1/pyproject.toml` & `dissect.sql-3.5.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/tests/data/test.sqlite` & `dissect.sql-3.5.dev1/tests/data/test.sqlite`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/tests/test_default_values.py` & `dissect.sql-3.5.dev1/tests/test_default_values.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/tests/test_parse_table_columns_constraints.py` & `dissect.sql-3.5.dev1/tests/test_parse_table_columns_constraints.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/tests/test_row.py` & `dissect.sql-3.5.dev1/tests/test_row.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/tests/test_sqlite.py` & `dissect.sql-3.5.dev1/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.4.dev1/tox.ini` & `dissect.sql-3.5.dev1/tox.ini`

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

