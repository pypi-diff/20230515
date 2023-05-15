# Comparing `tmp/einsum_pipe-0.0.1.tar.gz` & `tmp/einsum_pipe-0.1.0.tar.gz`

## Comparing `einsum_pipe-0.0.1.tar` & `einsum_pipe-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/src/einsum_pipe/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/src/einsum_pipe/bidict.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/src/einsum_pipe/einsum_pipe.py
--rw-r--r--   0        0        0     8355 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/src/einsum_pipe/einsum_script.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/src/einsum_pipe/ops.py
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/tests/test_einsum_pipe.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/tests/test_ops.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/LICENSE
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/README.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 einsum_pipe-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/src/einsum_pipe/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/src/einsum_pipe/bidict.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/src/einsum_pipe/einsum_pipe.py
+-rw-r--r--   0        0        0     8355 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/src/einsum_pipe/einsum_script.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/src/einsum_pipe/ops.py
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/tests/test_einsum_pipe.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/tests/test_ops.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 einsum_pipe-0.1.0/PKG-INFO
```

### Comparing `einsum_pipe-0.0.1/src/einsum_pipe/bidict.py` & `einsum_pipe-0.1.0/src/einsum_pipe/bidict.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.0.1/src/einsum_pipe/einsum_pipe.py` & `einsum_pipe-0.1.0/src/einsum_pipe/einsum_pipe.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.0.1/src/einsum_pipe/einsum_script.py` & `einsum_pipe-0.1.0/src/einsum_pipe/einsum_script.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.0.1/src/einsum_pipe/ops.py` & `einsum_pipe-0.1.0/src/einsum_pipe/ops.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.0.1/tests/test_einsum_pipe.py` & `einsum_pipe-0.1.0/tests/test_einsum_pipe.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.0.1/tests/test_ops.py` & `einsum_pipe-0.1.0/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.0.1/LICENSE` & `einsum_pipe-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.0.1/README.md` & `einsum_pipe-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     'ii...',
     A, B
 )
 ```
 
 Internally, this calculates a compatible input shape, `(4, 8, 4, 8, 50)` and `(32, 32, 50)`, and a combined `np.einsum` set of subscripts, `"ebdbc,aac->edc"`. `A` and `B` are reshaped (which is generally essentially free), the single `np.einsum` operation is run, and the output is reshaped back to the expected output shape.
 
+You can find further examples in the "tests" folder.
+
 ## Syntax
 
 The syntax is based on Numpy's `einsum`, with the addition of allowing multiple subscripts and defining the shapes of the intermediate arrays. The input arrays can be put at the end, as shown, or next to the subscript definitions. In this example, only two arrays are used at start of the pipe, however you can add more arrays at later stages. The output of the previous step is always considered the first input of the subsequent step.
 
 ## Shape Compatibility
 
 Shapes are compatible if each dimension is the product of some subsequence of a matching shape (of the previous output). For example, `(32, 32)` and `(4, 256)` are compatible, since both can be built from the shape `(4, 8, 4, 8)`: `(4*8, 4*8)` and `(4, 8*4*8)`. On the other hand, `(2, 3)` and `(3, 2)` aren't directly compatible since they don't share divisors.
```

### Comparing `einsum_pipe-0.0.1/pyproject.toml` & `einsum_pipe-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "einsum_pipe"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
-  { name="David R. Armstrong" },
+  { name="David Armstrong" },
 ]
 description = "A Python package to compile multiple Numpy einsum operations into one"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `einsum_pipe-0.0.1/PKG-INFO` & `einsum_pipe-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: einsum_pipe
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Python package to compile multiple Numpy einsum operations into one
 Project-URL: Homepage, https://github.com/davystrong/Einsum-Pipe
 Project-URL: Bug Tracker, https://github.com/davystrong/Einsum-Pipe/issues
-Author: David R. Armstrong
+Author: David Armstrong
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
@@ -45,14 +45,16 @@
     'ii...',
     A, B
 )
 ```
 
 Internally, this calculates a compatible input shape, `(4, 8, 4, 8, 50)` and `(32, 32, 50)`, and a combined `np.einsum` set of subscripts, `"ebdbc,aac->edc"`. `A` and `B` are reshaped (which is generally essentially free), the single `np.einsum` operation is run, and the output is reshaped back to the expected output shape.
 
+You can find further examples in the "tests" folder.
+
 ## Syntax
 
 The syntax is based on Numpy's `einsum`, with the addition of allowing multiple subscripts and defining the shapes of the intermediate arrays. The input arrays can be put at the end, as shown, or next to the subscript definitions. In this example, only two arrays are used at start of the pipe, however you can add more arrays at later stages. The output of the previous step is always considered the first input of the subsequent step.
 
 ## Shape Compatibility
 
 Shapes are compatible if each dimension is the product of some subsequence of a matching shape (of the previous output). For example, `(32, 32)` and `(4, 256)` are compatible, since both can be built from the shape `(4, 8, 4, 8)`: `(4*8, 4*8)` and `(4, 8*4*8)`. On the other hand, `(2, 3)` and `(3, 2)` aren't directly compatible since they don't share divisors.
```

