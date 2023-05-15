# Comparing `tmp/chope-0.1.2.tar.gz` & `tmp/chope-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chope-0.1.2.tar", last modified: Sun Apr 16 07:30:00 2023, max compression
+gzip compressed data, was "chope-0.2.2.tar", last modified: Mon May 15 14:53:49 2023, max compression
```

## Comparing `chope-0.1.2.tar` & `chope-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-16 07:30:00.329008 chope-0.1.2/
--rw-r--r--   0 johantjuatja   (501) staff       (20)     1065 2023-04-08 07:11:52.000000 chope-0.1.2/LICENSE
--rw-r--r--   0 johantjuatja   (501) staff       (20)     6098 2023-04-16 07:30:00.328629 chope-0.1.2/PKG-INFO
--rw-r--r--   0 johantjuatja   (501) staff       (20)     5401 2023-04-16 07:11:01.000000 chope-0.1.2/README.md
-drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-16 07:30:00.325956 chope-0.1.2/chope/
--rw-r--r--   0 johantjuatja   (501) staff       (20)     3958 2023-04-09 14:42:26.000000 chope-0.1.2/chope/__init__.py
--rw-r--r--   0 johantjuatja   (501) staff       (20)     1677 2023-04-10 13:16:55.000000 chope-0.1.2/chope/css.py
--rw-r--r--   0 johantjuatja   (501) staff       (20)     2404 2023-04-16 07:25:48.000000 chope-0.1.2/chope/element.py
-drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-16 07:30:00.327256 chope-0.1.2/chope.egg-info/
--rw-r--r--   0 johantjuatja   (501) staff       (20)     6098 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/PKG-INFO
--rw-r--r--   0 johantjuatja   (501) staff       (20)      282 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/SOURCES.txt
--rw-r--r--   0 johantjuatja   (501) staff       (20)        1 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/dependency_links.txt
--rw-r--r--   0 johantjuatja   (501) staff       (20)        7 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/requires.txt
--rw-r--r--   0 johantjuatja   (501) staff       (20)        6 2023-04-16 07:30:00.000000 chope-0.1.2/chope.egg-info/top_level.txt
--rw-r--r--   0 johantjuatja   (501) staff       (20)      833 2023-04-16 07:26:46.000000 chope-0.1.2/pyproject.toml
--rw-r--r--   0 johantjuatja   (501) staff       (20)       38 2023-04-16 07:30:00.329087 chope-0.1.2/setup.cfg
-drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-04-16 07:30:00.328059 chope-0.1.2/tests/
--rw-r--r--   0 johantjuatja   (501) staff       (20)        0 2023-04-08 07:53:38.000000 chope-0.1.2/tests/__init__.py
--rw-r--r--   0 johantjuatja   (501) staff       (20)      761 2023-04-10 13:07:47.000000 chope-0.1.2/tests/test_css.py
--rw-r--r--   0 johantjuatja   (501) staff       (20)     1673 2023-04-16 07:22:38.000000 chope-0.1.2/tests/test_element.py
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-05-15 14:53:49.153452 chope-0.2.2/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     1065 2023-04-08 07:11:52.000000 chope-0.2.2/LICENSE
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     6098 2023-05-15 14:53:49.153122 chope-0.2.2/PKG-INFO
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     5401 2023-04-16 07:11:01.000000 chope-0.2.2/README.md
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-05-15 14:53:49.149000 chope-0.2.2/chope/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     3958 2023-04-09 14:42:26.000000 chope-0.2.2/chope/__init__.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     1677 2023-04-10 13:16:55.000000 chope-0.2.2/chope/css.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     2404 2023-04-16 07:25:48.000000 chope-0.2.2/chope/element.py
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-05-15 14:53:49.151564 chope-0.2.2/chope/functions/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        0 2023-04-23 03:42:01.000000 chope-0.2.2/chope/functions/__init__.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     2390 2023-04-23 07:07:20.000000 chope-0.2.2/chope/functions/color.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)      226 2023-04-23 04:13:49.000000 chope-0.2.2/chope/functions/function.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     2193 2023-05-15 14:43:24.000000 chope-0.2.2/chope/functions/shape.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     1269 2023-04-23 04:28:39.000000 chope-0.2.2/chope/functions/transform.py
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-05-15 14:53:49.150099 chope-0.2.2/chope.egg-info/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     6098 2023-05-15 14:53:49.000000 chope-0.2.2/chope.egg-info/PKG-INFO
+-rw-r--r--   0 johantjuatja   (501) staff       (20)      440 2023-05-15 14:53:49.000000 chope-0.2.2/chope.egg-info/SOURCES.txt
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        1 2023-05-15 14:53:49.000000 chope-0.2.2/chope.egg-info/dependency_links.txt
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        7 2023-05-15 14:53:49.000000 chope-0.2.2/chope.egg-info/requires.txt
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        6 2023-05-15 14:53:49.000000 chope-0.2.2/chope.egg-info/top_level.txt
+-rw-r--r--   0 johantjuatja   (501) staff       (20)      833 2023-05-15 14:50:25.000000 chope-0.2.2/pyproject.toml
+-rw-r--r--   0 johantjuatja   (501) staff       (20)       38 2023-05-15 14:53:49.153519 chope-0.2.2/setup.cfg
+drwxr-xr-x   0 johantjuatja   (501) staff       (20)        0 2023-05-15 14:53:49.152640 chope-0.2.2/tests/
+-rw-r--r--   0 johantjuatja   (501) staff       (20)        0 2023-04-08 07:53:38.000000 chope-0.2.2/tests/__init__.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)      761 2023-04-10 13:07:47.000000 chope-0.2.2/tests/test_css.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)     1673 2023-04-16 07:22:38.000000 chope-0.2.2/tests/test_element.py
+-rw-r--r--   0 johantjuatja   (501) staff       (20)      329 2023-04-23 04:13:20.000000 chope-0.2.2/tests/test_function.py
```

### Comparing `chope-0.1.2/LICENSE` & `chope-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chope-0.1.2/PKG-INFO` & `chope-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chope
-Version: 0.1.2
+Version: 0.2.2
 Summary: CSS & HTML on Python Easily
 Author-email: Johan Tjuatja <hanstjua@yahoo.co.id>
 Project-URL: Homepage, https://github.com/hanstjua/chope
 Project-URL: Bug Tracker, https://github.com/hanstjua/chope/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `chope-0.1.2/README.md` & `chope-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `chope-0.1.2/chope/__init__.py` & `chope-0.2.2/chope/__init__.py`

 * *Files identical despite different names*

### Comparing `chope-0.1.2/chope/css.py` & `chope-0.2.2/chope/css.py`

 * *Files identical despite different names*

### Comparing `chope-0.1.2/chope/element.py` & `chope-0.2.2/chope/element.py`

 * *Files identical despite different names*

### Comparing `chope-0.1.2/chope.egg-info/PKG-INFO` & `chope-0.2.2/chope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chope
-Version: 0.1.2
+Version: 0.2.2
 Summary: CSS & HTML on Python Easily
 Author-email: Johan Tjuatja <hanstjua@yahoo.co.id>
 Project-URL: Homepage, https://github.com/hanstjua/chope
 Project-URL: Bug Tracker, https://github.com/hanstjua/chope/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `chope-0.1.2/pyproject.toml` & `chope-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chope"
-version = "0.1.2"
+version = "0.2.2"
 authors = [
     {name = "Johan Tjuatja", email = "hanstjua@yahoo.co.id"},
 ]
 description = "CSS & HTML on Python Easily"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chope-0.1.2/tests/test_css.py` & `chope-0.2.2/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `chope-0.1.2/tests/test_element.py` & `chope-0.2.2/tests/test_element.py`

 * *Files identical despite different names*

