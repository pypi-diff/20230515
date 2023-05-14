# Comparing `tmp/lealnumeros-0.0.1.tar.gz` & `tmp/lealnumeros-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lealnumeros-0.0.1.tar", last modified: Sun May 14 20:32:04 2023, max compression
+gzip compressed data, was "lealnumeros-0.0.2.tar", last modified: Mon May 15 00:14:16 2023, max compression
```

## Comparing `lealnumeros-0.0.1.tar` & `lealnumeros-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 20:32:04.461219 lealnumeros-0.0.1/
--rw-rw-rw-   0        0        0     1098 2023-05-14 20:25:14.000000 lealnumeros-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      396 2023-05-14 20:32:04.460219 lealnumeros-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       74 2023-05-14 20:25:57.000000 lealnumeros-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 20:32:04.425239 lealnumeros-0.0.1/lealNumeros/
--rw-rw-rw-   0        0        0       32 2023-05-14 20:13:46.000000 lealnumeros-0.0.1/lealNumeros/__init__.py
--rw-rw-rw-   0        0        0     2018 2023-05-14 20:12:56.000000 lealnumeros-0.0.1/lealNumeros/main.py
-drwxrwxrwx   0        0        0        0 2023-05-14 20:32:04.459220 lealnumeros-0.0.1/lealnumeros.egg-info/
--rw-rw-rw-   0        0        0      396 2023-05-14 20:32:04.000000 lealnumeros-0.0.1/lealnumeros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-14 20:32:04.000000 lealnumeros-0.0.1/lealnumeros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 20:32:04.000000 lealnumeros-0.0.1/lealnumeros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 20:32:04.000000 lealnumeros-0.0.1/lealnumeros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-14 20:32:04.000000 lealnumeros-0.0.1/lealnumeros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 20:32:04.461219 lealnumeros-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-14 20:30:25.000000 lealnumeros-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:14:16.303334 lealnumeros-0.0.2/
+-rw-rw-rw-   0        0        0     1098 2023-05-14 20:25:14.000000 lealnumeros-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0     1278 2023-05-15 00:14:16.301335 lealnumeros-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-05-14 23:53:56.000000 lealnumeros-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 00:14:16.264356 lealnumeros-0.0.2/lealNumeros/
+-rw-rw-rw-   0        0        0       32 2023-05-14 20:13:46.000000 lealnumeros-0.0.2/lealNumeros/__init__.py
+-rw-rw-rw-   0        0        0     2018 2023-05-14 20:12:56.000000 lealnumeros-0.0.2/lealNumeros/main.py
+drwxrwxrwx   0        0        0        0 2023-05-15 00:14:16.300335 lealnumeros-0.0.2/lealnumeros.egg-info/
+-rw-rw-rw-   0        0        0     1278 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 00:14:16.303334 lealnumeros-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-15 00:05:12.000000 lealnumeros-0.0.2/setup.py
```

### Comparing `lealnumeros-0.0.1/LICENCE` & `lealnumeros-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.1/lealNumeros/main.py` & `lealnumeros-0.0.2/lealNumeros/main.py`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.1/setup.py` & `lealnumeros-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='lealnumeros',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT License',
     author='José Rodolfo',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silvaleal.ctt@gmail.com',
     keywords='lealnumeros',
     description=u'Trabalhe com formatação de números de uma maneira rápido e fácil.',
```

