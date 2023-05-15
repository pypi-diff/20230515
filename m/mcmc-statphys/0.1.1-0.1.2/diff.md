# Comparing `tmp/mcmc_statphys-0.1.1.tar.gz` & `tmp/mcmc_statphys-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcmc_statphys-0.1.1.tar", last modified: Sun May 14 13:46:14 2023, max compression
+gzip compressed data, was "mcmc_statphys-0.1.2.tar", last modified: Mon May 15 01:43:56 2023, max compression
```

## Comparing `mcmc_statphys-0.1.1.tar` & `mcmc_statphys-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.159690 mcmc_statphys-0.1.1/
--rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3721 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1989 2023-05-14 13:46:14.159690 mcmc_statphys-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.037117 mcmc_statphys-0.1.1/docs/
--rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/authors.rst
--rw-rw-rw-   0        0        0     5006 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/history.rst
--rw-rw-rw-   0        0        0      330 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/index.rst
--rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/installation.rst
--rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/readme.rst
--rw-rw-rw-   0        0        0       88 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.074634 mcmc_statphys-0.1.1/mcmc_statphys/
--rw-rw-rw-   0        0        0      143 2023-05-14 12:02:25.000000 mcmc_statphys-0.1.1/mcmc_statphys/__init__.py
--rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.1.1/mcmc_statphys/cli.py
--rw-rw-rw-   0        0        0    10952 2023-05-14 10:14:57.000000 mcmc_statphys-0.1.1/mcmc_statphys/mcmc_statphys.py
--rw-rw-rw-   0        0        0     6083 2023-05-14 09:16:12.000000 mcmc_statphys-0.1.1/mcmc_statphys/model.py
-drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.124783 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/
--rw-rw-rw-   0        0        0     1989 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      662 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      408 2023-05-14 13:46:14.162684 mcmc_statphys-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1557 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.158692 mcmc_statphys-0.1.1/tests/
--rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      927 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/tests/test_mcmc_statphys.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.892957 mcmc_statphys-0.1.2/
+-rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3721 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      651 2023-05-15 01:23:48.000000 mcmc_statphys-0.1.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3541 2023-05-15 01:43:56.893955 mcmc_statphys-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2052 2023-05-15 01:32:18.000000 mcmc_statphys-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.744356 mcmc_statphys-0.1.2/docs/
+-rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     5006 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/history.rst
+-rw-rw-rw-   0        0        0      333 2023-05-15 01:23:54.000000 mcmc_statphys-0.1.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       88 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.761309 mcmc_statphys-0.1.2/mcmc_statphys/
+-rw-rw-rw-   0        0        0      143 2023-05-14 12:02:25.000000 mcmc_statphys-0.1.2/mcmc_statphys/__init__.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.1.2/mcmc_statphys/cli.py
+-rw-rw-rw-   0        0        0    16697 2023-05-14 15:53:48.000000 mcmc_statphys-0.1.2/mcmc_statphys/method.py
+-rw-rw-rw-   0        0        0     8200 2023-05-14 15:40:25.000000 mcmc_statphys-0.1.2/mcmc_statphys/model.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.876003 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/
+-rw-rw-rw-   0        0        0     3541 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      408 2023-05-15 01:43:56.901934 mcmc_statphys-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-05-15 01:20:36.000000 mcmc_statphys-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.890964 mcmc_statphys-0.1.2/tests/
+-rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      920 2023-05-14 15:52:21.000000 mcmc_statphys-0.1.2/tests/test_mcmc_statphys.py
```

### Comparing `mcmc_statphys-0.1.1/CONTRIBUTING.rst` & `mcmc_statphys-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.1/LICENSE` & `mcmc_statphys-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.1/docs/Makefile` & `mcmc_statphys-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.1/docs/conf.py` & `mcmc_statphys-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.1/docs/installation.rst` & `mcmc_statphys-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.1/docs/make.bat` & `mcmc_statphys-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.1/mcmc_statphys.egg-info/SOURCES.txt` & `mcmc_statphys-0.1.2/mcmc_statphys.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 mcmc_statphys/__init__.py
 mcmc_statphys/cli.py
-mcmc_statphys/mcmc_statphys.py
+mcmc_statphys/method.py
 mcmc_statphys/model.py
 mcmc_statphys.egg-info/PKG-INFO
 mcmc_statphys.egg-info/SOURCES.txt
 mcmc_statphys.egg-info/dependency_links.txt
 mcmc_statphys.egg-info/entry_points.txt
 mcmc_statphys.egg-info/not-zip-safe
 mcmc_statphys.egg-info/requires.txt
```

### Comparing `mcmc_statphys-0.1.1/setup.py` & `mcmc_statphys-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['Click>=7.0', ]
 
-test_requirements = [ ]
+test_requirements = []
 
 setup(
     author="Uynaj GI",
     author_email='suquan12148@outlook.com',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='mcmc_statphys',
     name='mcmc_statphys',
     packages=find_packages(include=['mcmc_statphys', 'mcmc_statphys.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/uynajgi/mcmc_statphys',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `mcmc_statphys-0.1.1/tests/test_mcmc_statphys.py` & `mcmc_statphys-0.1.2/tests/test_mcmc_statphys.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Tests for `mcmc_statphys` package."""
 
 
 import unittest
 from click.testing import CliRunner
 
-from mcmc_statphys import mcmc_statphys
+from mcmc_statphys import method
 from mcmc_statphys import cli
 
 
 class TestMcmc_statphys(unittest.TestCase):
     """Tests for `mcmc_statphys` package."""
 
     def setUp(self):
```

