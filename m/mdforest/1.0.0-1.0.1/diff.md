# Comparing `tmp/mdforest-1.0.0.tar.gz` & `tmp/mdforest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-1.0.0.tar", last modified: Sun May 14 22:57:56 2023, max compression
+gzip compressed data, was "mdforest-1.0.1.tar", last modified: Sun May 14 23:03:48 2023, max compression
```

## Comparing `mdforest-1.0.0.tar` & `mdforest-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 22:57:56.531424 mdforest-1.0.0/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.0.0/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      413 2023-05-14 22:57:56.531424 mdforest-1.0.0/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2457 2023-05-14 20:42:59.000000 mdforest-1.0.0/README.md
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 22:57:56.529424 mdforest-1.0.0/markdown_tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      430 2023-05-14 20:59:45.000000 mdforest-1.0.0/markdown_tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2444 2023-05-14 21:19:06.000000 mdforest-1.0.0/markdown_tree/markdown_tree.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-14 20:59:45.000000 mdforest-1.0.0/markdown_tree/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 22:57:56.530424 mdforest-1.0.0/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      413 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      305 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       24 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       14 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.0.0/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-14 22:57:56.531424 mdforest-1.0.0/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1244 2023-05-14 20:45:08.000000 mdforest-1.0.0/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 22:57:56.530424 mdforest-1.0.0/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1201 2023-05-14 21:06:28.000000 mdforest-1.0.0/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 23:03:48.079975 mdforest-1.0.1/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.0.1/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2906 2023-05-14 23:03:48.079975 mdforest-1.0.1/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2457 2023-05-14 20:42:59.000000 mdforest-1.0.1/README.md
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 23:03:48.077974 mdforest-1.0.1/markdown_tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      430 2023-05-14 20:59:45.000000 mdforest-1.0.1/markdown_tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2444 2023-05-14 21:19:06.000000 mdforest-1.0.1/markdown_tree/markdown_tree.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-14 20:59:45.000000 mdforest-1.0.1/markdown_tree/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 23:03:48.078975 mdforest-1.0.1/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2906 2023-05-14 23:03:47.000000 mdforest-1.0.1/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      305 2023-05-14 23:03:48.000000 mdforest-1.0.1/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-14 23:03:47.000000 mdforest-1.0.1/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       24 2023-05-14 23:03:47.000000 mdforest-1.0.1/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       14 2023-05-14 23:03:47.000000 mdforest-1.0.1/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.0.1/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-14 23:03:48.079975 mdforest-1.0.1/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1480 2023-05-14 23:03:45.000000 mdforest-1.0.1/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 23:03:48.078975 mdforest-1.0.1/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1201 2023-05-14 21:06:28.000000 mdforest-1.0.1/tests/test_mdtree.py
```

### Comparing `mdforest-1.0.0/LICENSE` & `mdforest-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-1.0.0/README.md` & `mdforest-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mdforest-1.0.0/markdown_tree/markdown_tree.py` & `mdforest-1.0.1/markdown_tree/markdown_tree.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.0.0/markdown_tree/treebuild.py` & `mdforest-1.0.1/markdown_tree/treebuild.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.0.0/setup.py` & `mdforest-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
+from pathlib import Path
 
 class PyTest(TestCommand):
 
     user_options = [('pytest-args=', 'a', "Arguments to pass to py.test")]
 
     def initialize_options(self):
         TestCommand.initialize_options(self)
@@ -15,23 +16,29 @@
 
     def run_tests(self):
         # import here, cause outside the eggs aren't loaded
         import pytest
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
-VERSION = '1.0.0'
+this_directory = Path(__file__).parent
+LONG_DESCRIPTION = (this_directory / "README.md").read_text()
+
+VERSION = '1.0.1'
 DESCRIPTION = 'A package to convert between Markdown and a forest data structure for effecient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type="Markdown",
+    readme="README.md",
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/markdown-tree",
     packages = ['markdown_tree'],
     cmdclass = {'test': PyTest},
     tests_require = ['pytest'],
     install_requires = ['markdown', 'beautifulsoup4'],
     download_url = 'https://github.com/kj3moraes/markdown-tree/archive/%s.zip' % VERSION,
```

### Comparing `mdforest-1.0.0/tests/test_mdtree.py` & `mdforest-1.0.1/tests/test_mdtree.py`

 * *Files identical despite different names*

