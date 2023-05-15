# Comparing `tmp/pytransport-2.0.0.tar.gz` & `tmp/pytransport-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransport-2.0.0.tar", last modified: Sun Mar 19 16:55:09 2023, max compression
+gzip compressed data, was "pytransport-2.0.1.tar", last modified: Mon May 15 09:28:57 2023, max compression
```

## Comparing `pytransport-2.0.0.tar` & `pytransport-2.0.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.437870 pytransport-2.0.0/
--rw-r--r--   0 lnevay     (501) staff       (20)       98 2023-03-19 16:18:03.000000 pytransport-2.0.0/.gitignore
--rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:44:07.000000 pytransport-2.0.0/COPYING.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      631 2023-03-19 15:40:10.000000 pytransport-2.0.0/LICENSE.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      569 2023-02-13 16:45:12.000000 pytransport-2.0.0/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)     1630 2023-03-19 16:55:09.437962 pytransport-2.0.0/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      505 2022-11-01 14:57:07.000000 pytransport-2.0.0/README.md
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.428937 pytransport-2.0.0/docs/
--rw-r--r--   0 lnevay     (501) staff       (20)      615 2020-05-18 14:44:07.000000 pytransport-2.0.0/docs/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)      813 2020-05-18 14:44:07.000000 pytransport-2.0.0/docs/make.bat
--rw-r--r--   0 lnevay     (501) staff       (20)   213216 2023-03-19 16:49:59.000000 pytransport-2.0.0/docs/pytransport.pdf
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.433156 pytransport-2.0.0/docs/source/
--rw-r--r--   0 lnevay     (501) staff       (20)      157 2020-05-18 14:44:07.000000 pytransport-2.0.0/docs/source/authorship.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5529 2023-03-19 16:14:24.000000 pytransport-2.0.0/docs/source/conf.py
--rw-r--r--   0 lnevay     (501) staff       (20)      495 2021-06-15 15:23:44.000000 pytransport-2.0.0/docs/source/converting.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.433299 pytransport-2.0.0/docs/source/figures/
--rw-r--r--   0 lnevay     (501) staff       (20)    29085 2020-05-18 14:44:07.000000 pytransport-2.0.0/docs/source/figures/optics.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)      469 2021-06-15 15:23:44.000000 pytransport-2.0.0/docs/source/index.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1316 2023-03-19 16:45:13.000000 pytransport-2.0.0/docs/source/installation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      695 2023-03-19 15:55:24.000000 pytransport-2.0.0/docs/source/licence.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      812 2023-03-19 16:14:39.000000 pytransport-2.0.0/docs/source/moduledocs.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      422 2021-06-15 15:23:44.000000 pytransport-2.0.0/docs/source/optics.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1439 2023-03-19 16:43:31.000000 pytransport-2.0.0/pyproject.toml
--rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-03-19 16:55:09.438207 pytransport-2.0.0/setup.cfg
--rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 15:45:21.000000 pytransport-2.0.0/setup.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.426462 pytransport-2.0.0/src/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.435302 pytransport-2.0.0/src/pytransport/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.436480 pytransport-2.0.0/src/pytransport/Compare/
--rw-r--r--   0 lnevay     (501) staff       (20)     5063 2020-05-18 14:44:07.000000 pytransport-2.0.0/src/pytransport/Compare/_TransportTransportComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)       64 2020-05-18 14:44:07.000000 pytransport-2.0.0/src/pytransport/Compare/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    72098 2023-03-19 16:42:31.000000 pytransport-2.0.0/src/pytransport/Convert.py
--rw-r--r--   0 lnevay     (501) staff       (20)    23643 2023-03-19 16:42:18.000000 pytransport-2.0.0/src/pytransport/Data.py
--rw-r--r--   0 lnevay     (501) staff       (20)    33019 2023-03-19 16:42:25.000000 pytransport-2.0.0/src/pytransport/Reader.py
--rw-r--r--   0 lnevay     (501) staff       (20)    21628 2023-03-19 16:42:39.000000 pytransport-2.0.0/src/pytransport/_General.py
--rw-r--r--   0 lnevay     (501) staff       (20)      581 2023-03-19 16:16:07.000000 pytransport-2.0.0/src/pytransport/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-03-19 16:55:09.000000 pytransport-2.0.0/src/pytransport/_version.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.436121 pytransport-2.0.0/src/pytransport.egg-info/
--rw-r--r--   0 lnevay     (501) staff       (20)     1630 2023-03-19 16:55:09.000000 pytransport-2.0.0/src/pytransport.egg-info/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      941 2023-03-19 16:55:09.000000 pytransport-2.0.0/src/pytransport.egg-info/SOURCES.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 16:55:09.000000 pytransport-2.0.0/src/pytransport.egg-info/dependency_links.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 16:08:19.000000 pytransport-2.0.0/src/pytransport.egg-info/not-zip-safe
--rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 16:55:09.000000 pytransport-2.0.0/src/pytransport.egg-info/requires.txt
--rw-r--r--   0 lnevay     (501) staff       (20)       12 2023-03-19 16:55:09.000000 pytransport-2.0.0/src/pytransport.egg-info/top_level.txt
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.437579 pytransport-2.0.0/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)   259301 2021-06-15 15:23:44.000000 pytransport-2.0.0/tests/FOR002-example.DAT
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:44:07.000000 pytransport-2.0.0/tests/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.437690 pytransport-2.0.0/tests/func/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:44:07.000000 pytransport-2.0.0/tests/func/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-03-19 16:55:09.437788 pytransport-2.0.0/tests/unit/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:44:07.000000 pytransport-2.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.457801 pytransport-2.0.1/
+-rw-r--r--   0 lnevay     (501) staff       (20)       98 2023-03-19 16:18:03.000000 pytransport-2.0.1/.gitignore
+-rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:44:07.000000 pytransport-2.0.1/COPYING.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      631 2023-03-19 15:40:10.000000 pytransport-2.0.1/LICENSE.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      569 2023-02-13 16:45:12.000000 pytransport-2.0.1/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)     1656 2023-05-15 09:28:57.457900 pytransport-2.0.1/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      505 2022-11-01 14:57:07.000000 pytransport-2.0.1/README.md
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.451829 pytransport-2.0.1/docs/
+-rw-r--r--   0 lnevay     (501) staff       (20)      615 2020-05-18 14:44:07.000000 pytransport-2.0.1/docs/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)      813 2020-05-18 14:44:07.000000 pytransport-2.0.1/docs/make.bat
+-rw-r--r--   0 lnevay     (501) staff       (20)   213216 2023-03-19 16:49:59.000000 pytransport-2.0.1/docs/pytransport.pdf
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.453924 pytransport-2.0.1/docs/source/
+-rw-r--r--   0 lnevay     (501) staff       (20)      157 2020-05-18 14:44:07.000000 pytransport-2.0.1/docs/source/authorship.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5534 2023-03-19 17:15:38.000000 pytransport-2.0.1/docs/source/conf.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      495 2021-06-15 15:23:44.000000 pytransport-2.0.1/docs/source/converting.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.454047 pytransport-2.0.1/docs/source/figures/
+-rw-r--r--   0 lnevay     (501) staff       (20)    29085 2020-05-18 14:44:07.000000 pytransport-2.0.1/docs/source/figures/optics.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)      488 2023-05-15 09:24:49.000000 pytransport-2.0.1/docs/source/index.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1316 2023-03-19 16:45:13.000000 pytransport-2.0.1/docs/source/installation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      695 2023-03-19 15:55:24.000000 pytransport-2.0.1/docs/source/licence.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      812 2023-03-19 16:14:39.000000 pytransport-2.0.1/docs/source/moduledocs.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      422 2021-06-15 15:23:44.000000 pytransport-2.0.1/docs/source/optics.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      237 2023-05-15 09:27:32.000000 pytransport-2.0.1/docs/source/version_history.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1439 2023-05-15 09:23:47.000000 pytransport-2.0.1/pyproject.toml
+-rw-r--r--   0 lnevay     (501) staff       (20)      262 2023-05-15 09:28:57.458157 pytransport-2.0.1/setup.cfg
+-rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 15:45:21.000000 pytransport-2.0.1/setup.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.449298 pytransport-2.0.1/src/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.455099 pytransport-2.0.1/src/pytransport/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.456401 pytransport-2.0.1/src/pytransport/Compare/
+-rw-r--r--   0 lnevay     (501) staff       (20)     5063 2020-05-18 14:44:07.000000 pytransport-2.0.1/src/pytransport/Compare/_TransportTransportComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)       64 2020-05-18 14:44:07.000000 pytransport-2.0.1/src/pytransport/Compare/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    72098 2023-03-19 16:42:31.000000 pytransport-2.0.1/src/pytransport/Convert.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    23643 2023-03-19 16:42:18.000000 pytransport-2.0.1/src/pytransport/Data.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    33019 2023-03-19 16:42:25.000000 pytransport-2.0.1/src/pytransport/Reader.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    21628 2023-03-19 16:42:39.000000 pytransport-2.0.1/src/pytransport/_General.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      581 2023-03-19 16:16:07.000000 pytransport-2.0.1/src/pytransport/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-05-15 09:28:57.000000 pytransport-2.0.1/src/pytransport/_version.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.455970 pytransport-2.0.1/src/pytransport.egg-info/
+-rw-r--r--   0 lnevay     (501) staff       (20)     1656 2023-05-15 09:28:57.000000 pytransport-2.0.1/src/pytransport.egg-info/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      973 2023-05-15 09:28:57.000000 pytransport-2.0.1/src/pytransport.egg-info/SOURCES.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-05-15 09:28:57.000000 pytransport-2.0.1/src/pytransport.egg-info/dependency_links.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 16:08:19.000000 pytransport-2.0.1/src/pytransport.egg-info/not-zip-safe
+-rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-05-15 09:28:57.000000 pytransport-2.0.1/src/pytransport.egg-info/requires.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)       12 2023-05-15 09:28:57.000000 pytransport-2.0.1/src/pytransport.egg-info/top_level.txt
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.457497 pytransport-2.0.1/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)   259301 2021-06-15 15:23:44.000000 pytransport-2.0.1/tests/FOR002-example.DAT
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:44:07.000000 pytransport-2.0.1/tests/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.457612 pytransport-2.0.1/tests/func/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:44:07.000000 pytransport-2.0.1/tests/func/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:28:57.457716 pytransport-2.0.1/tests/unit/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:44:07.000000 pytransport-2.0.1/tests/unit/__init__.py
```

### Comparing `pytransport-2.0.0/COPYING.txt` & `pytransport-2.0.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/LICENSE.txt` & `pytransport-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/Makefile` & `pytransport-2.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/PKG-INFO` & `pytransport-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytransport
-Version: 2.0.0
+Version: 2.0.1
 Summary: Convert TRANSPORT models and load TRANSPORT output.
 Author-email: "JAI@RHUL" <william.shields@rhul.ac.uk>
 Maintainer-email: William Shields <william.shields@rhul.ac.uk>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pytransport
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pytransport
 Project-URL: repository, https://bitbucket.org/jairhul/pytransport
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,20 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: root-numpy
 License-File: LICENSE.txt
+License-File: COPYING.txt
 
 # pyTransport
 
 A python package containing both utilities for processing and analysing TRANSPORT output.
 
 ## Authors
```

### Comparing `pytransport-2.0.0/docs/Makefile` & `pytransport-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/docs/make.bat` & `pytransport-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/docs/pytransport.pdf` & `pytransport-2.0.1/docs/pytransport.pdf`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/docs/source/conf.py` & `pytransport-2.0.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 from importlib.metadata import version
 # The full version, including alpha/beta/rc tags.
-release = version('pymadx')
+release = version('pytransport')
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
```

### Comparing `pytransport-2.0.0/docs/source/figures/optics.pdf` & `pytransport-2.0.1/docs/source/figures/optics.pdf`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/docs/source/installation.rst` & `pytransport-2.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/docs/source/licence.rst` & `pytransport-2.0.1/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/docs/source/moduledocs.rst` & `pytransport-2.0.1/docs/source/moduledocs.rst`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/pyproject.toml` & `pytransport-2.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytransport"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 dynamic = ["version"]
 readme = "README.md"
 description = "Convert TRANSPORT models and load TRANSPORT output."
 license = {file = "LICENCE.txt"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `pytransport-2.0.0/src/pytransport/Compare/_TransportTransportComparison.py` & `pytransport-2.0.1/src/pytransport/Compare/_TransportTransportComparison.py`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/src/pytransport/Convert.py` & `pytransport-2.0.1/src/pytransport/Convert.py`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/src/pytransport/Data.py` & `pytransport-2.0.1/src/pytransport/Data.py`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/src/pytransport/Reader.py` & `pytransport-2.0.1/src/pytransport/Reader.py`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/src/pytransport/_General.py` & `pytransport-2.0.1/src/pytransport/_General.py`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/src/pytransport/__init__.py` & `pytransport-2.0.1/src/pytransport/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransport-2.0.0/src/pytransport.egg-info/PKG-INFO` & `pytransport-2.0.1/src/pytransport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytransport
-Version: 2.0.0
+Version: 2.0.1
 Summary: Convert TRANSPORT models and load TRANSPORT output.
 Author-email: "JAI@RHUL" <william.shields@rhul.ac.uk>
 Maintainer-email: William Shields <william.shields@rhul.ac.uk>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pytransport
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pytransport
 Project-URL: repository, https://bitbucket.org/jairhul/pytransport
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,20 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: root-numpy
 License-File: LICENSE.txt
+License-File: COPYING.txt
 
 # pyTransport
 
 A python package containing both utilities for processing and analysing TRANSPORT output.
 
 ## Authors
```

### Comparing `pytransport-2.0.0/src/pytransport.egg-info/SOURCES.txt` & `pytransport-2.0.1/src/pytransport.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 docs/source/conf.py
 docs/source/converting.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/licence.rst
 docs/source/moduledocs.rst
 docs/source/optics.rst
+docs/source/version_history.rst
 docs/source/figures/optics.pdf
 src/pytransport/Convert.py
 src/pytransport/Data.py
 src/pytransport/Reader.py
 src/pytransport/_General.py
 src/pytransport/__init__.py
 src/pytransport/_version.py
```

### Comparing `pytransport-2.0.0/tests/FOR002-example.DAT` & `pytransport-2.0.1/tests/FOR002-example.DAT`

 * *Files identical despite different names*

