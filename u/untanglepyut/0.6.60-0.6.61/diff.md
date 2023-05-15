# Comparing `tmp/untanglepyut-0.6.60.tar.gz` & `tmp/untanglepyut-0.6.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untanglepyut-0.6.60.tar", last modified: Wed May 10 17:25:46 2023, max compression
+gzip compressed data, was "untanglepyut-0.6.61.tar", last modified: Mon May 15 00:35:16 2023, max compression
```

## Comparing `untanglepyut-0.6.60.tar` & `untanglepyut-0.6.61.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-10 17:25:46.215013 untanglepyut-0.6.60/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-0.6.60/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3478 2023-05-10 17:25:46.214886 untanglepyut-0.6.60/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3226 2023-04-13 20:32:39.000000 untanglepyut-0.6.60/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-10 17:25:46.215051 untanglepyut-0.6.60/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      750 2023-05-10 15:26:37.000000 untanglepyut-0.6.60/setup.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-10 17:25:46.214165 untanglepyut-0.6.60/untanglepyut/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      886 2023-01-03 16:20:29.000000 untanglepyut-0.6.60/untanglepyut/BaseUnTangle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1774 2022-08-29 19:49:16.000000 untanglepyut-0.6.60/untanglepyut/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2022-10-13 01:16:21.000000 untanglepyut-0.6.60/untanglepyut/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15843 2023-03-19 16:02:08.000000 untanglepyut-0.6.60/untanglepyut/UnTangleOglLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14445 2023-05-08 16:55:26.000000 untanglepyut-0.6.60/untanglepyut/UnTanglePyut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4154 2022-08-23 19:21:04.000000 untanglepyut-0.6.60/untanglepyut/UnTangleUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13009 2023-05-10 17:16:32.000000 untanglepyut-0.6.60/untanglepyut/UnTangler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3918 2023-01-31 19:27:38.000000 untanglepyut-0.6.60/untanglepyut/UntangleSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2022-06-24 19:59:25.000000 untanglepyut-0.6.60/untanglepyut/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-25 14:46:48.000000 untanglepyut-0.6.60/untanglepyut/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-10 17:25:46.214727 untanglepyut-0.6.60/untanglepyut.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3478 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      493 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       84 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:35:16.396046 untanglepyut-0.6.61/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-0.6.61/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3478 2023-05-15 00:35:16.395920 untanglepyut-0.6.61/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3226 2023-04-13 20:32:39.000000 untanglepyut-0.6.61/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-15 00:35:16.396078 untanglepyut-0.6.61/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      821 2023-05-15 00:34:26.000000 untanglepyut-0.6.61/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:35:16.395038 untanglepyut-0.6.61/untanglepyut/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      886 2023-01-03 16:20:29.000000 untanglepyut-0.6.61/untanglepyut/BaseUnTangle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1774 2022-08-29 19:49:16.000000 untanglepyut-0.6.61/untanglepyut/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2022-10-13 01:16:21.000000 untanglepyut-0.6.61/untanglepyut/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15843 2023-03-19 16:02:08.000000 untanglepyut-0.6.61/untanglepyut/UnTangleOglLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14445 2023-05-08 16:55:26.000000 untanglepyut-0.6.61/untanglepyut/UnTanglePyut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4154 2022-08-23 19:21:04.000000 untanglepyut-0.6.61/untanglepyut/UnTangleUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13009 2023-05-10 17:16:32.000000 untanglepyut-0.6.61/untanglepyut/UnTangler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3918 2023-01-31 19:27:38.000000 untanglepyut-0.6.61/untanglepyut/UntangleSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-05-15 00:32:46.000000 untanglepyut-0.6.61/untanglepyut/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-05-15 00:30:32.000000 untanglepyut-0.6.61/untanglepyut/_version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-25 14:46:48.000000 untanglepyut-0.6.61/untanglepyut/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:35:16.395717 untanglepyut-0.6.61/untanglepyut.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3478 2023-05-15 00:35:16.000000 untanglepyut-0.6.61/untanglepyut.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      518 2023-05-15 00:35:16.000000 untanglepyut-0.6.61/untanglepyut.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-15 00:35:16.000000 untanglepyut-0.6.61/untanglepyut.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       84 2023-05-15 00:35:16.000000 untanglepyut-0.6.61/untanglepyut.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-05-15 00:35:16.000000 untanglepyut-0.6.61/untanglepyut.egg-info/top_level.txt
```

### Comparing `untanglepyut-0.6.60/LICENSE` & `untanglepyut-0.6.61/LICENSE`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/PKG-INFO` & `untanglepyut-0.6.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untanglepyut
-Version: 0.6.60
+Version: 0.6.61
 Summary: XML to Ogl Object Model
 Home-page: https://github.com/hasii2011/untanglepyut
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./docs/agpl-license-web-badge-version-2-256x48.png"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: untanglepyut Version: 0.6.60 Summary: XML to Ogl
+Metadata-Version: 2.1 Name: untanglepyut Version: 0.6.61 Summary: XML to Ogl
 Object Model Home-page: https://github.com/hasii2011/untanglepyut Author-email:
 Humberto.A.Sanchez.II@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [CircleCI](https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/
 master/main/badge.svg?window=30d)](https://app.circleci.com/insights/github/
 hasii2011/untanglepyut/workflows/main/overview?branch=master&reporting-
 window=last-30-days&insights-snapshot=true) [![CircleCI](https://
```

### Comparing `untanglepyut-0.6.60/README.md` & `untanglepyut-0.6.61/README.md`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/setup.py` & `untanglepyut-0.6.61/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import pathlib
 from setuptools import setup
+from untanglepyut import __version__ as untanglepyutVersion
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="untanglepyut",
-    version="0.6.60",
+    version=untanglepyutVersion,
     author_email='Humberto.A.Sanchez.II@gmail.com',
     description='XML to Ogl Object Model',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hasii2011/untanglepyut",
     packages=[
         'untanglepyut'
     ],
     package_data={
         'untanglepyut': ['py.typed'],
     },
 
-    install_requires=['hasiihelper~=0.2.0', 'hasiicommon~=0.2.2', 'pyutmodel~=1.4.3', 'ogl==0.70.26', 'untangle==1.2.1'],
+    install_requires=['hasiihelper~=0.2.0', 'hasiicommon~=0.2.2', 'pyutmodel~=1.4.3', 'ogl==0.70.30', 'untangle==1.2.1'],
 )
```

### Comparing `untanglepyut-0.6.60/untanglepyut/BaseUnTangle.py` & `untanglepyut-0.6.61/untanglepyut/BaseUnTangle.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/untanglepyut/Common.py` & `untanglepyut-0.6.61/untanglepyut/Common.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/untanglepyut/Types.py` & `untanglepyut-0.6.61/untanglepyut/Types.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/untanglepyut/UnTangleOglLinks.py` & `untanglepyut-0.6.61/untanglepyut/UnTangleOglLinks.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/untanglepyut/UnTanglePyut.py` & `untanglepyut-0.6.61/untanglepyut/UnTanglePyut.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/untanglepyut/UnTangleUseCaseDiagram.py` & `untanglepyut-0.6.61/untanglepyut/UnTangleUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/untanglepyut/UnTangler.py` & `untanglepyut-0.6.61/untanglepyut/UnTangler.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/untanglepyut/UntangleSequenceDiagram.py` & `untanglepyut-0.6.61/untanglepyut/UntangleSequenceDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.60/untanglepyut.egg-info/PKG-INFO` & `untanglepyut-0.6.61/untanglepyut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untanglepyut
-Version: 0.6.60
+Version: 0.6.61
 Summary: XML to Ogl Object Model
 Home-page: https://github.com/hasii2011/untanglepyut
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./docs/agpl-license-web-badge-version-2-256x48.png"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: untanglepyut Version: 0.6.60 Summary: XML to Ogl
+Metadata-Version: 2.1 Name: untanglepyut Version: 0.6.61 Summary: XML to Ogl
 Object Model Home-page: https://github.com/hasii2011/untanglepyut Author-email:
 Humberto.A.Sanchez.II@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [CircleCI](https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/
 master/main/badge.svg?window=30d)](https://app.circleci.com/insights/github/
 hasii2011/untanglepyut/workflows/main/overview?branch=master&reporting-
 window=last-30-days&insights-snapshot=true) [![CircleCI](https://
```

