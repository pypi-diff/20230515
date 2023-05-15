# Comparing `tmp/WX_Push_Services-1.0.8.tar.gz` & `tmp/WX_Push_Services-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WX_Push_Services-1.0.8.tar", last modified: Mon May 15 09:52:10 2023, max compression
+gzip compressed data, was "WX_Push_Services-1.0.9.tar", last modified: Mon May 15 09:55:20 2023, max compression
```

## Comparing `WX_Push_Services-1.0.8.tar` & `WX_Push_Services-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:52:10.553252 WX_Push_Services-1.0.8/
--rw-rw-rw-   0        0        0     1082 2022-12-24 14:41:15.000000 WX_Push_Services-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     6504 2023-05-15 09:52:10.551258 WX_Push_Services-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5728 2023-05-15 09:29:15.000000 WX_Push_Services-1.0.8/README.md
--rw-rw-rw-   0        0        0     5309 2023-05-15 09:48:50.000000 WX_Push_Services-1.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 09:52:10.496400 WX_Push_Services-1.0.8/WX_Push_Services/
--rw-rw-rw-   0        0        0    10898 2023-05-15 09:30:17.000000 WX_Push_Services-1.0.8/WX_Push_Services/WX_Push_Services.py
--rw-rw-rw-   0        0        0      263 2023-05-15 07:24:40.000000 WX_Push_Services-1.0.8/WX_Push_Services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:52:10.548264 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/
--rw-rw-rw-   0        0        0     6504 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 09:52:10.553252 WX_Push_Services-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2119 2023-05-15 09:52:00.000000 WX_Push_Services-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:55:20.641997 WX_Push_Services-1.0.9/
+-rw-rw-rw-   0        0        0     1082 2022-12-24 14:41:15.000000 WX_Push_Services-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6509 2023-05-15 09:55:20.640994 WX_Push_Services-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5728 2023-05-15 09:55:14.000000 WX_Push_Services-1.0.9/README.md
+-rw-rw-rw-   0        0        0     5314 2023-05-15 09:55:16.000000 WX_Push_Services-1.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 09:55:20.618529 WX_Push_Services-1.0.9/WX_Push_Services/
+-rw-rw-rw-   0        0        0    10898 2023-05-15 09:30:17.000000 WX_Push_Services-1.0.9/WX_Push_Services/WX_Push_Services.py
+-rw-rw-rw-   0        0        0      149 2023-05-15 09:55:12.000000 WX_Push_Services-1.0.9/WX_Push_Services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:55:20.637003 WX_Push_Services-1.0.9/WX_Push_Services.egg-info/
+-rw-rw-rw-   0        0        0     6509 2023-05-15 09:55:20.000000 WX_Push_Services-1.0.9/WX_Push_Services.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-15 09:55:20.000000 WX_Push_Services-1.0.9/WX_Push_Services.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:55:20.000000 WX_Push_Services-1.0.9/WX_Push_Services.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-15 09:55:20.000000 WX_Push_Services-1.0.9/WX_Push_Services.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-05-15 09:55:20.000000 WX_Push_Services-1.0.9/WX_Push_Services.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-15 09:55:20.000000 WX_Push_Services-1.0.9/WX_Push_Services.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 09:55:20.641997 WX_Push_Services-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2119 2023-05-15 09:55:06.000000 WX_Push_Services-1.0.9/setup.py
```

### Comparing `WX_Push_Services-1.0.8/LICENSE` & `WX_Push_Services-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `WX_Push_Services-1.0.8/PKG-INFO` & `WX_Push_Services-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WX_Push_Services
-Version: 1.0.8
+Version: 1.0.9
 Summary: Push message to wechat
 Home-page: https://github.com/IronManStank/QYWX_PushService
 Author: Super.S
 Author-email: 1157723200@qq.com
 License: MIT License
 Keywords: wechat,push,message,qywx,wxpusher
 Platform: any
@@ -23,27 +23,27 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 
-.. image:: https://img.shields.io/pypi/pyversions/WX-Push-Services?style=plastic
+.. figure:: https://img.shields.io/pypi/pyversions/WX-Push-Services?style=plastic
    :alt: PyPI - Python Version
 
-.. image:: https://img.shields.io/pypi/dm/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/dm/WX-Push-Services
    :alt: PyPI - Downloads
 
-.. image:: https://img.shields.io/pypi/status/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/status/WX-Push-Services
    :alt: PyPI - Status
 
-.. image:: https://img.shields.io/pypi/l/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/l/WX-Push-Services
    :alt: PyPI - License
    
-.. image:: https://img.shields.io/github/issues-search?query=WX-Push-Services
+.. figure:: https://img.shields.io/github/issues-search?query=WX-Push-Services
    :alt: GitHub issue custom search
 
 
 
 重大更新
 ==========
```

### Comparing `WX_Push_Services-1.0.8/README.md` & `WX_Push_Services-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `WX_Push_Services-1.0.8/README.rst` & `WX_Push_Services-1.0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
-.. image:: https://img.shields.io/pypi/pyversions/WX-Push-Services?style=plastic
+.. figure:: https://img.shields.io/pypi/pyversions/WX-Push-Services?style=plastic
    :alt: PyPI - Python Version
 
-.. image:: https://img.shields.io/pypi/dm/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/dm/WX-Push-Services
    :alt: PyPI - Downloads
 
-.. image:: https://img.shields.io/pypi/status/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/status/WX-Push-Services
    :alt: PyPI - Status
 
-.. image:: https://img.shields.io/pypi/l/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/l/WX-Push-Services
    :alt: PyPI - License
    
-.. image:: https://img.shields.io/github/issues-search?query=WX-Push-Services
+.. figure:: https://img.shields.io/github/issues-search?query=WX-Push-Services
    :alt: GitHub issue custom search
 
 
 
 重大更新
 ==========
```

### Comparing `WX_Push_Services-1.0.8/WX_Push_Services/WX_Push_Services.py` & `WX_Push_Services-1.0.9/WX_Push_Services/WX_Push_Services.py`

 * *Files identical despite different names*

### Comparing `WX_Push_Services-1.0.8/WX_Push_Services.egg-info/PKG-INFO` & `WX_Push_Services-1.0.9/WX_Push_Services.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WX-Push-Services
-Version: 1.0.8
+Version: 1.0.9
 Summary: Push message to wechat
 Home-page: https://github.com/IronManStank/QYWX_PushService
 Author: Super.S
 Author-email: 1157723200@qq.com
 License: MIT License
 Keywords: wechat,push,message,qywx,wxpusher
 Platform: any
@@ -23,27 +23,27 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 
-.. image:: https://img.shields.io/pypi/pyversions/WX-Push-Services?style=plastic
+.. figure:: https://img.shields.io/pypi/pyversions/WX-Push-Services?style=plastic
    :alt: PyPI - Python Version
 
-.. image:: https://img.shields.io/pypi/dm/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/dm/WX-Push-Services
    :alt: PyPI - Downloads
 
-.. image:: https://img.shields.io/pypi/status/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/status/WX-Push-Services
    :alt: PyPI - Status
 
-.. image:: https://img.shields.io/pypi/l/WX-Push-Services
+.. figure:: https://img.shields.io/pypi/l/WX-Push-Services
    :alt: PyPI - License
    
-.. image:: https://img.shields.io/github/issues-search?query=WX-Push-Services
+.. figure:: https://img.shields.io/github/issues-search?query=WX-Push-Services
    :alt: GitHub issue custom search
 
 
 
 重大更新
 ==========
```

### Comparing `WX_Push_Services-1.0.8/setup.py` & `WX_Push_Services-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 
 setup(
     name="WX_Push_Services",
-    version="1.0.8",
+    version="1.0.9",
     author="Super.S",
     author_email="1157723200@qq.com",
     packages=["WX_Push_Services"],
     scripts=["WX_Push_Services/WX_Push_Services.py"],
     url="https://github.com/IronManStank/QYWX_PushService",
     license="MIT License",
     description="Push message to wechat",
```

