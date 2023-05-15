# Comparing `tmp/com.castsoftware.uc.python.common-0.1.9.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-0.1.9.tar", last modified: Fri Feb 24 19:00:21 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.0.0.tar", last modified: Mon May 15 14:52:34 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-0.1.9.tar` & `com.castsoftware.uc.python.common-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 19:00:21.430959 com.castsoftware.uc.python.common-0.1.9/
--rw-rw-rw-   0        0        0    35823 2021-04-05 17:40:19.000000 com.castsoftware.uc.python.common-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      712 2023-02-24 19:00:21.427959 com.castsoftware.uc.python.common-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      103 2021-06-01 15:37:40.000000 com.castsoftware.uc.python.common-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-02-24 19:00:21.390949 com.castsoftware.uc.python.common-0.1.9/cast_common/
--rw-rw-rw-   0        0        0        0 2021-06-01 14:42:59.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/__init__.py
--rw-rw-rw-   0        0        0     2036 2022-12-28 17:18:00.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    11962 2023-01-25 20:42:45.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0     5199 2023-01-25 21:07:43.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1681 2023-01-25 15:27:20.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/logger.py
--rw-rw-rw-   0        0        0     4421 2023-01-25 21:09:02.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     7243 2023-02-24 18:59:02.000000 com.castsoftware.uc.python.common-0.1.9/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-02-24 19:00:21.422959 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      712 2023-02-24 19:00:21.000000 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-02-24 19:00:21.000000 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 19:00:21.000000 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-24 19:00:21.000000 com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2023-02-24 19:00:03.000000 com.castsoftware.uc.python.common-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-24 19:00:21.431962 com.castsoftware.uc.python.common-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 14:52:34.891073 com.castsoftware.uc.python.common-1.0.0/
+-rw-rw-rw-   0        0        0    35823 2021-04-05 17:40:19.000000 com.castsoftware.uc.python.common-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      825 2023-05-15 14:52:34.892074 com.castsoftware.uc.python.common-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2021-06-01 15:37:40.000000 com.castsoftware.uc.python.common-1.0.0/README.md
+-rw-rw-rw-   0        0        0      626 2023-05-15 14:52:12.000000 com.castsoftware.uc.python.common-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      725 2023-05-15 14:52:34.902155 com.castsoftware.uc.python.common-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 14:52:34.758125 com.castsoftware.uc.python.common-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 14:52:34.876809 com.castsoftware.uc.python.common-1.0.0/src/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-05-15 14:52:34.000000 com.castsoftware.uc.python.common-1.0.0/src/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-15 14:52:34.000000 com.castsoftware.uc.python.common-1.0.0/src/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 14:52:34.000000 com.castsoftware.uc.python.common-1.0.0/src/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 14:52:34.000000 com.castsoftware.uc.python.common-1.0.0/src/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 14:52:34.000000 com.castsoftware.uc.python.common-1.0.0/src/com.castsoftware.uc.python.common.egg-info/top_level.txt
```

### Comparing `com.castsoftware.uc.python.common-0.1.9/LICENSE` & `com.castsoftware.uc.python.common-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-0.1.9/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 0.1.9
+Version: 1.0.0
 Summary: A set of common classes and methods for use with python projects
+Home-page: https://github.com/pypa/sampleproject
+Author: Nevin Kaplan
+Author-email: n.kaplan@castsoftware.com
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `com.castsoftware.uc.python.common-0.1.9/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.0/src/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 0.1.9
+Version: 1.0.0
 Summary: A set of common classes and methods for use with python projects
+Home-page: https://github.com/pypa/sampleproject
+Author: Nevin Kaplan
+Author-email: n.kaplan@castsoftware.com
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `com.castsoftware.uc.python.common-0.1.9/pyproject.toml` & `com.castsoftware.uc.python.common-1.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='0.1.9' #prod version
-#version='0.1.8' #test version
+version='1.0.0' #prod version
+
+dependencies = ['pandas','requests']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
```

