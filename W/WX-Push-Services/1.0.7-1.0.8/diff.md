# Comparing `tmp/WX_Push_Services-1.0.7.tar.gz` & `tmp/WX_Push_Services-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WX_Push_Services-1.0.7.tar", last modified: Mon May 15 09:47:31 2023, max compression
+gzip compressed data, was "WX_Push_Services-1.0.8.tar", last modified: Mon May 15 09:52:10 2023, max compression
```

## Comparing `WX_Push_Services-1.0.7.tar` & `WX_Push_Services-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:47:31.235367 WX_Push_Services-1.0.7/
--rw-rw-rw-   0        0        0     1082 2022-12-24 14:41:15.000000 WX_Push_Services-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1193 2023-05-15 09:47:31.234371 WX_Push_Services-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5728 2023-05-15 09:29:15.000000 WX_Push_Services-1.0.7/README.md
--rw-rw-rw-   0        0        0     5309 2023-05-15 09:45:41.000000 WX_Push_Services-1.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 09:47:31.213402 WX_Push_Services-1.0.7/WX_Push_Services/
--rw-rw-rw-   0        0        0    10898 2023-05-15 09:30:17.000000 WX_Push_Services-1.0.7/WX_Push_Services/WX_Push_Services.py
--rw-rw-rw-   0        0        0      263 2023-05-15 07:24:40.000000 WX_Push_Services-1.0.7/WX_Push_Services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:47:31.231370 WX_Push_Services-1.0.7/WX_Push_Services.egg-info/
--rw-rw-rw-   0        0        0     1193 2023-05-15 09:47:31.000000 WX_Push_Services-1.0.7/WX_Push_Services.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-15 09:47:31.000000 WX_Push_Services-1.0.7/WX_Push_Services.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:47:31.000000 WX_Push_Services-1.0.7/WX_Push_Services.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-15 09:47:31.000000 WX_Push_Services-1.0.7/WX_Push_Services.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-05-15 09:47:31.000000 WX_Push_Services-1.0.7/WX_Push_Services.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-15 09:47:31.000000 WX_Push_Services-1.0.7/WX_Push_Services.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 09:47:31.236342 WX_Push_Services-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2303 2023-05-15 09:47:26.000000 WX_Push_Services-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:52:10.553252 WX_Push_Services-1.0.8/
+-rw-rw-rw-   0        0        0     1082 2022-12-24 14:41:15.000000 WX_Push_Services-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     6504 2023-05-15 09:52:10.551258 WX_Push_Services-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5728 2023-05-15 09:29:15.000000 WX_Push_Services-1.0.8/README.md
+-rw-rw-rw-   0        0        0     5309 2023-05-15 09:48:50.000000 WX_Push_Services-1.0.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 09:52:10.496400 WX_Push_Services-1.0.8/WX_Push_Services/
+-rw-rw-rw-   0        0        0    10898 2023-05-15 09:30:17.000000 WX_Push_Services-1.0.8/WX_Push_Services/WX_Push_Services.py
+-rw-rw-rw-   0        0        0      263 2023-05-15 07:24:40.000000 WX_Push_Services-1.0.8/WX_Push_Services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:52:10.548264 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/
+-rw-rw-rw-   0        0        0     6504 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-15 09:52:10.000000 WX_Push_Services-1.0.8/WX_Push_Services.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 09:52:10.553252 WX_Push_Services-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2119 2023-05-15 09:52:00.000000 WX_Push_Services-1.0.8/setup.py
```

### Comparing `WX_Push_Services-1.0.7/LICENSE` & `WX_Push_Services-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `WX_Push_Services-1.0.7/README.md` & `WX_Push_Services-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `WX_Push_Services-1.0.7/README.rst` & `WX_Push_Services-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `WX_Push_Services-1.0.7/WX_Push_Services/WX_Push_Services.py` & `WX_Push_Services-1.0.8/WX_Push_Services/WX_Push_Services.py`

 * *Files identical despite different names*

### Comparing `WX_Push_Services-1.0.7/setup.py` & `WX_Push_Services-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
     long_description = open(file="README.rst", mode="r", encoding="utf-8").read()
     # pypandoc.convert_file('README.md','rst')
     # open(file='README.md',mode='r',encoding='utf-8').read()
     print(long_description)
 except Exception as e:
     print(e)
-    long_description = ""
+    long_description = open(file="README.rst", mode="r", encoding="utf-8").read()
 
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 
 setup(
     name="WX_Push_Services",
-    version="1.0.7",
+    version="1.0.8",
     author="Super.S",
     author_email="1157723200@qq.com",
     packages=["WX_Push_Services"],
     scripts=["WX_Push_Services/WX_Push_Services.py"],
     url="https://github.com/IronManStank/QYWX_PushService",
     license="MIT License",
     description="Push message to wechat",
@@ -51,12 +51,7 @@
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
 
 
-# Add package path to PYTHONPATH environment variable
-if "PYTHONPATH" in os.environ:
-    os.environ["PYTHONPATH"] += ":/WX_Push_Services/WX_Push_Services.py"
-else:
-    os.environ["PYTHONPATH"] = "/WX_Push_Services/WX_Push_Services.py"
```

