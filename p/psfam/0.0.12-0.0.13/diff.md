# Comparing `tmp/psfam-0.0.12.tar.gz` & `tmp/psfam-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psfam-0.0.12.tar", last modified: Mon May 15 16:15:52 2023, max compression
+gzip compressed data, was "psfam-0.0.13.tar", last modified: Mon May 15 16:58:01 2023, max compression
```

## Comparing `psfam-0.0.12.tar` & `psfam-0.0.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 16:15:52.822303 psfam-0.0.12/
--rw-rw-rw-   0        0        0     6296 2023-05-15 16:15:52.821248 psfam-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     5705 2023-05-05 16:06:42.000000 psfam-0.0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 16:15:52.761944 psfam-0.0.12/psfam/
--rw-rw-rw-   0        0        0        0 2023-04-24 20:25:09.000000 psfam-0.0.12/psfam/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-29 21:06:06.000000 psfam-0.0.12/psfam/family.py
--rw-rw-rw-   0        0        0     5818 2023-04-25 15:45:54.000000 psfam-0.0.12/psfam/matrix_generator.py
--rw-rw-rw-   0        0        0     9947 2023-04-28 19:02:32.000000 psfam-0.0.12/psfam/pauli_organizer.py
--rw-rw-rw-   0        0        0     7605 2023-04-25 15:41:08.000000 psfam-0.0.12/psfam/pauli_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:15:52.815616 psfam-0.0.12/psfam.egg-info/
--rw-rw-rw-   0        0        0     6296 2023-05-15 16:15:52.000000 psfam-0.0.12/psfam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-15 16:15:52.000000 psfam-0.0.12/psfam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 16:15:52.000000 psfam-0.0.12/psfam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-15 16:15:52.000000 psfam-0.0.12/psfam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 16:15:52.000000 psfam-0.0.12/psfam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 16:15:52.823927 psfam-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-05-15 16:12:58.000000 psfam-0.0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:58:01.611863 psfam-0.0.13/
+-rw-rw-rw-   0        0        0     6296 2023-05-15 16:58:01.610863 psfam-0.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     5705 2023-05-05 16:06:42.000000 psfam-0.0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 16:58:01.593861 psfam-0.0.13/psfam/
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:25:09.000000 psfam-0.0.13/psfam/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-29 21:06:06.000000 psfam-0.0.13/psfam/family.py
+-rw-rw-rw-   0        0        0     5818 2023-04-25 15:45:54.000000 psfam-0.0.13/psfam/matrix_generator.py
+-rw-rw-rw-   0        0        0     9947 2023-04-28 19:02:32.000000 psfam-0.0.13/psfam/pauli_organizer.py
+-rw-rw-rw-   0        0        0     7605 2023-04-25 15:41:08.000000 psfam-0.0.13/psfam/pauli_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 16:58:01.608917 psfam-0.0.13/psfam.egg-info/
+-rw-rw-rw-   0        0        0     6296 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 16:58:01.000000 psfam-0.0.13/psfam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 16:58:01.612863 psfam-0.0.13/setup.cfg
+-rw-rw-rw-   0        0        0      939 2023-05-15 16:56:48.000000 psfam-0.0.13/setup.py
```

### Comparing `psfam-0.0.12/PKG-INFO` & `psfam-0.0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psfam
-Version: 0.0.12
+Version: 0.0.13
 Summary: First attempt at putting psfam in a build.
 Home-page: UNKNOWN
 Author: Ben Reggio
 Author-email: benjreggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `psfam-0.0.12/README.md` & `psfam-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `psfam-0.0.12/psfam/family.py` & `psfam-0.0.13/psfam/family.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.12/psfam/matrix_generator.py` & `psfam-0.0.13/psfam/matrix_generator.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.12/psfam/pauli_organizer.py` & `psfam-0.0.13/psfam/pauli_organizer.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.12/psfam/pauli_utils.py` & `psfam-0.0.13/psfam/pauli_utils.py`

 * *Files identical despite different names*

### Comparing `psfam-0.0.12/psfam.egg-info/PKG-INFO` & `psfam-0.0.13/psfam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psfam
-Version: 0.0.12
+Version: 0.0.13
 Summary: First attempt at putting psfam in a build.
 Home-page: UNKNOWN
 Author: Ben Reggio
 Author-email: benjreggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `psfam-0.0.12/setup.py` & `psfam-0.0.13/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "psfam",
-    version = "0.0.12",
+    version = "0.0.13",
     author = "Ben Reggio",
     author_email = "benjreggio@gmail.com",
     description = ("First attempt at putting psfam in a build."),
     license = "MIT",
     packages=['psfam'],
     long_description=read('README.md'),
     long_description_content_type = "text/markdown",
-    install_requires = ['scikit-build','markdown','numpy','qiskit','galois','scipy','functools','itertools','operator'],
+    install_requires = ['scikit-build','markdown','numpy','qiskit','galois','scipy'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

