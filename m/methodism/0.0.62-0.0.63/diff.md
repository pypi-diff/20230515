# Comparing `tmp/methodism-0.0.62.tar.gz` & `tmp/methodism-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.0.62.tar", last modified: Fri Apr 28 13:17:53 2023, max compression
+gzip compressed data, was "methodism-0.0.63.tar", last modified: Mon May 15 09:18:53 2023, max compression
```

## Comparing `methodism-0.0.62.tar` & `methodism-0.0.63.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 13:17:53.324593 methodism-0.0.62/
--rw-rw-rw-   0        0        0     2917 2023-04-28 13:17:53.324593 methodism-0.0.62/PKG-INFO
--rw-rw-rw-   0        0        0     2434 2023-04-28 10:28:06.000000 methodism-0.0.62/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 13:17:53.308967 methodism-0.0.62/methodism/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.62/methodism/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.0.62/methodism/costumizing.py
--rw-rw-rw-   0        0        0      772 2023-04-28 13:17:15.000000 methodism-0.0.62/methodism/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.62/methodism/error_messages.py
--rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.62/methodism/helper.py
--rw-rw-rw-   0        0        0     3294 2023-04-28 10:28:06.000000 methodism-0.0.62/methodism/main.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:17:53.324593 methodism-0.0.62/methodism.egg-info/
--rw-rw-rw-   0        0        0     2917 2023-04-28 13:17:53.000000 methodism-0.0.62/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-28 13:17:53.000000 methodism-0.0.62/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:17:53.000000 methodism-0.0.62/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 13:17:53.000000 methodism-0.0.62/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      604 2023-04-28 13:17:15.000000 methodism-0.0.62/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-04-28 13:17:53.324593 methodism-0.0.62/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 09:18:53.643958 methodism-0.0.63/
+-rw-rw-rw-   0        0        0     2917 2023-05-15 09:18:53.643958 methodism-0.0.63/PKG-INFO
+-rw-rw-rw-   0        0        0     2434 2023-04-28 10:28:06.000000 methodism-0.0.63/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 09:18:53.623492 methodism-0.0.63/methodism/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.63/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.0.63/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      772 2023-04-28 13:17:15.000000 methodism-0.0.63/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.63/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     1296 2023-05-15 09:16:13.000000 methodism-0.0.63/methodism/helper.py
+-rw-rw-rw-   0        0        0     3294 2023-04-28 10:28:06.000000 methodism-0.0.63/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:18:53.643958 methodism-0.0.63/methodism.egg-info/
+-rw-rw-rw-   0        0        0     2917 2023-05-15 09:18:53.000000 methodism-0.0.63/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-15 09:18:53.000000 methodism-0.0.63/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:18:53.000000 methodism-0.0.63/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 09:18:53.000000 methodism-0.0.63/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      604 2023-05-15 09:18:18.000000 methodism-0.0.63/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-05-15 09:18:53.643958 methodism-0.0.63/setup.cfg
```

### Comparing `methodism-0.0.62/PKG-INFO` & `methodism-0.0.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.62
+Version: 0.0.63
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.0.62/README.md` & `methodism-0.0.63/README.md`

 * *Files identical despite different names*

### Comparing `methodism-0.0.62/methodism/costumizing.py` & `methodism-0.0.63/methodism/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.62/methodism/decors.py` & `methodism-0.0.63/methodism/decors.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.62/methodism/error_messages.py` & `methodism-0.0.63/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.62/methodism/helper.py` & `methodism-0.0.63/methodism/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         "message": message
     }
 
 
 # xatolikni ushash uchun funksiya
 def exception_data(e):
     return {
-        "value": str(e.__str__()),
+        "value": f"""{str(type(e)).strip("<class '").strip("'>")} => {str(e.__str__())}""",
         "line": str(e.__traceback__.tb_lineno),
         "frame": str(e.__traceback__.tb_frame),
     }
 
 
 # berilgan uzunlikdagi Random token generatsiya qilib beradi
 def generate_key(size=50):
```

### Comparing `methodism-0.0.62/methodism/main.py` & `methodism-0.0.63/methodism/main.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.62/methodism.egg-info/PKG-INFO` & `methodism-0.0.63/methodism.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.62
+Version: 0.0.63
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.0.62/pyproject.toml` & `methodism-0.0.63/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.0.62"
+version = "0.0.63"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.0.62/setup.cfg` & `methodism-0.0.63/setup.cfg`

 * *Files identical despite different names*

