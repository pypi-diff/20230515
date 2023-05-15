# Comparing `tmp/bcvcontext-0.0.5.tar.gz` & `tmp/bcvcontext-0.1.0.tar.gz`

## Comparing `bcvcontext-0.0.5.tar` & `bcvcontext-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.0.5/src/bcvContext/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 bcvcontext-0.0.5/src/bcvContext/bcvContext.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 bcvcontext-0.0.5/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.0.5/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.0.5/README.md
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bcvcontext-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/src/bcvContext/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/src/bcvContext/bcvContext.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/README.md
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.0/PKG-INFO
```

### Comparing `bcvcontext-0.0.5/LICENSE` & `bcvcontext-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.0.5/PKG-INFO` & `bcvcontext-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcvContext
-Version: 0.0.5
+Version: 0.1.0
 Summary: A small package to handle context path for the BCV generic workflow
 Author-email: CEA <thomas.marques@cea.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

