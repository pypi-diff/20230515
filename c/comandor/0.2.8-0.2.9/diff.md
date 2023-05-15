# Comparing `tmp/comandor-0.2.8.tar.gz` & `tmp/comandor-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comandor-0.2.8.tar", last modified: Thu Apr 13 12:23:47 2023, max compression
+gzip compressed data, was "comandor-0.2.9.tar", last modified: Mon May 15 17:36:48 2023, max compression
```

## Comparing `comandor-0.2.8.tar` & `comandor-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:47.749395 comandor-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 12:23:35.000000 comandor-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 12:23:47.749395 comandor-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-13 12:23:35.000000 comandor-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:47.749395 comandor-0.2.8/comandor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:47.749395 comandor-0.2.8/comandor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:23:47.749395 comandor-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-13 12:23:35.000000 comandor-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:47.749395 comandor-0.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-13 12:23:35.000000 comandor-0.2.8/test/test_comandor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:48.582849 comandor-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 17:36:34.000000 comandor-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-15 17:36:48.582849 comandor-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-15 17:36:34.000000 comandor-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:48.582849 comandor-0.2.9/comandor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:48.582849 comandor-0.2.9/comandor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:36:48.582849 comandor-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 17:36:34.000000 comandor-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:48.582849 comandor-0.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-15 17:36:34.000000 comandor-0.2.9/test/test_comandor.py
```

### Comparing `comandor-0.2.8/LICENSE` & `comandor-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `comandor-0.2.8/PKG-INFO` & `comandor-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comandor
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Very Simple Script for Run your command!
 Home-page: https://github.com/NoobforAl/comandor
 Author: NoobforAl
 Author-email: FarshadSarmali@pm.me
 License: MIT License
 Keywords: command line,script
 Classifier: Development Status :: 1 - Planning
```

### Comparing `comandor-0.2.8/README.md` & `comandor-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `comandor-0.2.8/comandor/main.py` & `comandor-0.2.9/comandor/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         try:
             log.debug("Run runAction Function")
             return func(*a, **kw)
 
         except sp.CalledProcessError as err:
             log.error(
                 f"Status : FAIL Code: {err.returncode}\n"
-                "OutPut:\n {err.output.decode()}")
+                f"OutPut:\n {err.output.decode()}")
             raise
 
         except sp.TimeoutExpired:
             log.error("Timeout Error!")
             raise
 
     return wrapper
```

### Comparing `comandor-0.2.8/comandor/models.py` & `comandor-0.2.9/comandor/models.py`

 * *Files identical despite different names*

### Comparing `comandor-0.2.8/comandor/settings.py` & `comandor-0.2.9/comandor/settings.py`

 * *Files identical despite different names*

### Comparing `comandor-0.2.8/comandor.egg-info/PKG-INFO` & `comandor-0.2.9/comandor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comandor
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Very Simple Script for Run your command!
 Home-page: https://github.com/NoobforAl/comandor
 Author: NoobforAl
 Author-email: FarshadSarmali@pm.me
 License: MIT License
 Keywords: command line,script
 Classifier: Development Status :: 1 - Planning
```

### Comparing `comandor-0.2.8/setup.py` & `comandor-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='comandor',
-    version='0.2.8',
+    version='0.2.9',
     description='A Very Simple Script for Run your command!',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='https://github.com/NoobforAl/comandor',
     author='NoobforAl',
     author_email='FarshadSarmali@pm.me',
     license='MIT License',
```

### Comparing `comandor-0.2.8/test/test_comandor.py` & `comandor-0.2.9/test/test_comandor.py`

 * *Files identical despite different names*

