# Comparing `tmp/mixture-of-attention-0.0.1.tar.gz` & `tmp/mixture-of-attention-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-attention-0.0.1.tar", last modified: Sun May 14 17:27:38 2023, max compression
+gzip compressed data, was "mixture-of-attention-0.0.2.tar", last modified: Mon May 15 18:51:38 2023, max compression
```

## Comparing `mixture-of-attention-0.0.1.tar` & `mixture-of-attention-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:27:38.881872 mixture-of-attention-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 17:27:28.000000 mixture-of-attention-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-14 17:27:38.881872 mixture-of-attention-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-14 17:27:28.000000 mixture-of-attention-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:27:38.877872 mixture-of-attention-0.0.1/mixture_of_attention/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-14 17:27:28.000000 mixture-of-attention-0.0.1/mixture_of_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-14 17:27:28.000000 mixture-of-attention-0.0.1/mixture_of_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-14 17:27:28.000000 mixture-of-attention-0.0.1/mixture_of_attention/mixture_of_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:27:38.881872 mixture-of-attention-0.0.1/mixture_of_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-14 17:27:38.000000 mixture-of-attention-0.0.1/mixture_of_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-14 17:27:38.000000 mixture-of-attention-0.0.1/mixture_of_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:27:38.000000 mixture-of-attention-0.0.1/mixture_of_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-14 17:27:38.000000 mixture-of-attention-0.0.1/mixture_of_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 17:27:38.000000 mixture-of-attention-0.0.1/mixture_of_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:27:38.881872 mixture-of-attention-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-14 17:27:28.000000 mixture-of-attention-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/mixture_of_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/mixture_of_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/mixture_of_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/mixture_of_attention/mixture_of_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 18:51:38.000000 mixture-of-attention-0.0.2/mixture_of_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:51:38.979451 mixture-of-attention-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 18:51:26.000000 mixture-of-attention-0.0.2/setup.py
```

### Comparing `mixture-of-attention-0.0.1/LICENSE` & `mixture-of-attention-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.1/PKG-INFO` & `mixture-of-attention-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.1/mixture_of_attention/attend.py` & `mixture-of-attention-0.0.2/mixture_of_attention/attend.py`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.1/mixture_of_attention.egg-info/PKG-INFO` & `mixture-of-attention-0.0.2/mixture_of_attention.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.1/setup.py` & `mixture-of-attention-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'mixture-of-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Mixture of Attention',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/mixture-of-attention',
   keywords = [
@@ -15,16 +15,17 @@
     'deep learning',
     'transformers',
     'attention mechanism',
     'mixture-of-experts',
     'routed attention'
   ],
   install_requires=[
-    'colt5-attention',
+    'colt5-attention>=0.8.0',
     'einops>=0.6.1',
+    'local-attention>=1.8.6',
     'torch>=1.6',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
```

