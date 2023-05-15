# Comparing `tmp/count_unique_chars-0.0.2.tar.gz` & `tmp/count_unique_chars-0.0.3.tar.gz`

## Comparing `count_unique_chars-0.0.2.tar` & `count_unique_chars-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/requirements.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/src/count_unique_chars/__init__.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/src/count_unique_chars/cli.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/src/count_unique_chars/count_unique_chars.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/src/count_unique_chars/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/tests/pytest_cli.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/tests/pytest_count_unique_chars.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/LICENSE
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 count_unique_chars-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/src/count_unique_chars/__init__.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/src/count_unique_chars/cli.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/src/count_unique_chars/count_unique_chars.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/src/count_unique_chars/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/tests/pytest_cli.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/tests/pytest_count_unique_chars.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/LICENSE
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 count_unique_chars-0.0.3/PKG-INFO
```

### Comparing `count_unique_chars-0.0.2/src/count_unique_chars/cli.py` & `count_unique_chars-0.0.3/src/count_unique_chars/cli.py`

 * *Files identical despite different names*

### Comparing `count_unique_chars-0.0.2/src/count_unique_chars/count_unique_chars.py` & `count_unique_chars-0.0.3/src/count_unique_chars/count_unique_chars.py`

 * *Files identical despite different names*

### Comparing `count_unique_chars-0.0.2/tests/pytest_cli.py` & `count_unique_chars-0.0.3/tests/pytest_cli.py`

 * *Files identical despite different names*

### Comparing `count_unique_chars-0.0.2/tests/pytest_count_unique_chars.py` & `count_unique_chars-0.0.3/tests/pytest_count_unique_chars.py`

 * *Files identical despite different names*

### Comparing `count_unique_chars-0.0.2/LICENSE` & `count_unique_chars-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `count_unique_chars-0.0.2/README.md` & `count_unique_chars-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 A small Python utility to count the number of unique characters in a given string or file.
 
 # Installation
 
 You can install the count_unique_chars package using pip:
 ```
-pip install count-unique-chars==0.0.1
+pip install count-unique-chars
 ```
 
 # Dependencies
 ```
 pytest==7.3.1
 pytest-mock==3.10.0	
 ```
```

### Comparing `count_unique_chars-0.0.2/pyproject.toml` & `count_unique_chars-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "count-unique-chars"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Ilya Mishakin", email = "imishakintyr@gmail.com" },
 ]
 description = "A utility to count the number of unique characters in a string or file."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `count_unique_chars-0.0.2/PKG-INFO` & `count_unique_chars-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: count-unique-chars
-Version: 0.0.2
+Version: 0.0.3
 Summary: A utility to count the number of unique characters in a string or file.
 Author-email: Ilya Mishakin <imishakintyr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -14,15 +14,15 @@
 
 A small Python utility to count the number of unique characters in a given string or file.
 
 # Installation
 
 You can install the count_unique_chars package using pip:
 ```
-pip install count-unique-chars==0.0.1
+pip install count-unique-chars
 ```
 
 # Dependencies
 ```
 pytest==7.3.1
 pytest-mock==3.10.0	
 ```
```

