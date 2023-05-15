# Comparing `tmp/panml-0.0.1.tar.gz` & `tmp/panml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.1.tar", last modified: Mon May 15 15:54:56 2023, max compression
+gzip compressed data, was "panml-0.0.2.tar", last modified: Mon May 15 16:06:15 2023, max compression
```

## Comparing `panml-0.0.1.tar` & `panml-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-15 15:54:56.794481 panml-0.0.1/
--rw-r--r--   0 williamzheng   (501) staff       (20)      915 2023-05-15 15:54:56.794602 panml-0.0.1/PKG-INFO
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-15 15:54:56.794425 panml-0.0.1/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.1/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    18689 2023-05-15 12:24:30.430369 panml-0.0.1/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     6561 2023-05-15 12:24:30.431201 panml-0.0.1/panml/search.py
--rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.1/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2687 2023-05-15 15:54:41.642955 panml-0.0.1/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-15 16:06:15.303111 panml-0.0.2/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1472 2023-05-15 16:06:15.303227 panml-0.0.2/PKG-INFO
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-15 16:06:15.303053 panml-0.0.2/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.2/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    18689 2023-05-15 12:24:30.430369 panml-0.0.2/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     6561 2023-05-15 12:24:30.431201 panml-0.0.2/panml/search.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.2/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3263 2023-05-15 16:06:07.564068 panml-0.0.2/setup.py
```

### Comparing `panml-0.0.1/panml/models.py` & `panml-0.0.2/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.1/panml/search.py` & `panml-0.0.2/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.1/setup.py` & `panml-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 
 from distutils.core import setup
 setup(
   name = 'panml', # package name     
   packages = ['panml'], # package name
-  version = '0.0.1', # version
-  license='MIT', # license
-  description = 'PanML is a lightweight generative AI/ML development toolkit designed for ease of use and fast experimentation.', # short description about the package
+  version = '0.0.2', # version
+  license = 'MIT', # license
+  description = 'PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.', # short description about the package
+  long_description = 'PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. \
+                      The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others. \
+                      \n\nQuick start guide: https://github.com/Pan-ML/panml/wiki \
+                      \nDocumentation/Wiki: https://github.com/Pan-ML/panml/wiki',
   author = 'PanML team', # team name
   author_email = 'williamxn.zl@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
-  download_url = 'https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.1.tar.gz', # set a release on GitHub (with release tag) -> Assets -> right click and copy the link
+  download_url = 'https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.2.tar.gz', # set a release on GitHub (with release tag) -> Assets -> right click and copy the link
   keywords = ['generative AI', 'generative model', 'machine learning', 'large language model', # keywords
               'LLM', 'prompt engineering', 'fine tuning', 'prompt tuning', 'retrieval augmentation', 
               'AI safety', 'AI alignment'], 
   install_requires=[  # dependencies
         'aiohttp>=3.8.4',
         'aiosignal>=1.3.1',
         'async-timeout>=4.0.2',
```

