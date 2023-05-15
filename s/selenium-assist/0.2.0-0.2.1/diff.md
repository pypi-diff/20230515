# Comparing `tmp/selenium_assist-0.2.0.tar.gz` & `tmp/selenium_assist-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_assist-0.2.0.tar", last modified: Fri May 12 23:48:21 2023, max compression
+gzip compressed data, was "selenium_assist-0.2.1.tar", last modified: Mon May 15 21:17:53 2023, max compression
```

## Comparing `selenium_assist-0.2.0.tar` & `selenium_assist-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-12 23:48:21.545088 selenium_assist-0.2.0/
--rw-rw-r--   0 mich      (1000) mich      (1000)     1071 2023-04-05 22:02:25.000000 selenium_assist-0.2.0/LICENSE
--rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-12 23:48:21.545088 selenium_assist-0.2.0/PKG-INFO
--rw-rw-r--   0 mich      (1000) mich      (1000)       71 2023-05-12 23:13:38.000000 selenium_assist-0.2.0/README.md
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-12 23:48:21.545088 selenium_assist-0.2.0/selenium_assist/
--rw-rw-r--   0 mich      (1000) mich      (1000)      458 2023-05-12 23:13:37.000000 selenium_assist-0.2.0/selenium_assist/__init__.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     1048 2023-04-05 22:44:18.000000 selenium_assist-0.2.0/selenium_assist/helpers.py
--rw-rw-r--   0 mich      (1000) mich      (1000)      913 2023-05-12 21:20:58.000000 selenium_assist-0.2.0/selenium_assist/managers.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     3847 2023-05-12 23:13:37.000000 selenium_assist-0.2.0/selenium_assist/wrappers.py
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-12 23:48:21.545088 selenium_assist-0.2.0/selenium_assist.egg-info/
--rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-12 23:48:21.000000 selenium_assist-0.2.0/selenium_assist.egg-info/PKG-INFO
--rw-rw-r--   0 mich      (1000) mich      (1000)      341 2023-05-12 23:48:21.000000 selenium_assist-0.2.0/selenium_assist.egg-info/SOURCES.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)        1 2023-05-12 23:48:21.000000 selenium_assist-0.2.0/selenium_assist.egg-info/dependency_links.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       29 2023-05-12 23:48:21.000000 selenium_assist-0.2.0/selenium_assist.egg-info/requires.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       16 2023-05-12 23:48:21.000000 selenium_assist-0.2.0/selenium_assist.egg-info/top_level.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       79 2023-05-12 23:48:21.545088 selenium_assist-0.2.0/setup.cfg
--rw-rw-r--   0 mich      (1000) mich      (1000)     1084 2023-05-12 23:41:26.000000 selenium_assist-0.2.0/setup.py
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-15 21:17:53.445025 selenium_assist-0.2.1/
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1071 2023-04-05 22:02:25.000000 selenium_assist-0.2.1/LICENSE
+-rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-15 21:17:53.445025 selenium_assist-0.2.1/PKG-INFO
+-rw-rw-r--   0 mich      (1000) mich      (1000)       71 2023-05-12 23:13:38.000000 selenium_assist-0.2.1/README.md
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-15 21:17:53.441027 selenium_assist-0.2.1/selenium_assist/
+-rw-rw-r--   0 mich      (1000) mich      (1000)      458 2023-05-12 23:13:37.000000 selenium_assist-0.2.1/selenium_assist/__init__.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1048 2023-04-05 22:44:18.000000 selenium_assist-0.2.1/selenium_assist/helpers.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)      913 2023-05-12 21:20:58.000000 selenium_assist-0.2.1/selenium_assist/managers.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)     3847 2023-05-12 23:13:37.000000 selenium_assist-0.2.1/selenium_assist/wrappers.py
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-15 21:17:53.445025 selenium_assist-0.2.1/selenium_assist.egg-info/
+-rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/PKG-INFO
+-rw-rw-r--   0 mich      (1000) mich      (1000)      341 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/SOURCES.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)        1 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/dependency_links.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       39 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/requires.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       16 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/top_level.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       79 2023-05-15 21:17:53.449022 selenium_assist-0.2.1/setup.cfg
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1097 2023-05-15 21:14:58.000000 selenium_assist-0.2.1/setup.py
```

### Comparing `selenium_assist-0.2.0/LICENSE` & `selenium_assist-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.0/PKG-INFO` & `selenium_assist-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: selenium_assist
-Version: 0.2.0
+Version: 0.2.1
 Summary: Helper functions for selenium
 Home-page: https://github.com/ivanmicetic/selenium-assist
-Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.0.tar.gz
+Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.1.tar.gz
 Author: Ivan Mičetić
 Author-email: ivan.micetic@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Keywords: pypi,selenium_assist
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `selenium_assist-0.2.0/selenium_assist/helpers.py` & `selenium_assist-0.2.1/selenium_assist/helpers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.0/selenium_assist/managers.py` & `selenium_assist-0.2.1/selenium_assist/managers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.0/selenium_assist/wrappers.py` & `selenium_assist-0.2.1/selenium_assist/wrappers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.0/selenium_assist.egg-info/PKG-INFO` & `selenium_assist-0.2.1/selenium_assist.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: selenium-assist
-Version: 0.2.0
+Version: 0.2.1
 Summary: Helper functions for selenium
 Home-page: https://github.com/ivanmicetic/selenium-assist
-Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.0.tar.gz
+Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.1.tar.gz
 Author: Ivan Mičetić
 Author-email: ivan.micetic@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Keywords: pypi,selenium_assist
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `selenium_assist-0.2.0/setup.py` & `selenium_assist-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium_assist",
-    version="0.2.0",
+    version="0.2.1",
     author="Ivan Mičetić",
     author_email="ivan.micetic@gmail.com",
     description="Helper functions for selenium",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ivanmicetic/selenium-assist",
     project_urls={
         "Bug Tracker": "https://github.com/ivanmicetic/selenium-assist/issues"
     },
     license="MIT",
     packages=["selenium_assist"],
-    install_requires=["selenium<4", "webdriver_manager"],
+    install_requires=["selenium<4", "webdriver_manager", "urllib3<2"],
     keywords=["pypi", "selenium_assist"],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
-    download_url="https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.0.tar.gz"
+    download_url="https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.1.tar.gz"
 )
```

