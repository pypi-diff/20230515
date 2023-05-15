# Comparing `tmp/cipherLV-0.1.3.tar.gz` & `tmp/cipherLV-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipherLV-0.1.3.tar", last modified: Sun May 14 18:18:58 2023, max compression
+gzip compressed data, was "cipherLV-0.1.4.tar", last modified: Mon May 15 06:24:18 2023, max compression
```

## Comparing `cipherLV-0.1.3.tar` & `cipherLV-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 18:18:58.919859 cipherLV-0.1.3/
--rw-rw-rw-   0        0        0      919 2023-05-14 18:18:58.914860 cipherLV-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-14 18:18:38.000000 cipherLV-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 18:18:58.911042 cipherLV-0.1.3/cipherLV.egg-info/
--rw-rw-rw-   0        0        0      919 2023-05-14 18:18:58.000000 cipherLV-0.1.3/cipherLV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-05-14 18:18:58.000000 cipherLV-0.1.3/cipherLV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 18:18:58.000000 cipherLV-0.1.3/cipherLV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 18:18:58.000000 cipherLV-0.1.3/cipherLV.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1563 2023-05-14 06:41:30.000000 cipherLV-0.1.3/cipherLV.py
--rw-rw-rw-   0        0        0       42 2023-05-14 18:18:58.920854 cipherLV-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-14 18:17:25.000000 cipherLV-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:24:18.565486 cipherLV-0.1.4/
+-rw-rw-rw-   0        0        0      919 2023-05-15 06:24:18.564439 cipherLV-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-14 18:18:38.000000 cipherLV-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 06:24:18.525636 cipherLV-0.1.4/cipherLV/
+-rw-rw-rw-   0        0        0      107 2023-05-15 06:23:13.000000 cipherLV-0.1.4/cipherLV/__init__.py
+-rw-rw-rw-   0        0        0     1563 2023-05-14 06:41:30.000000 cipherLV-0.1.4/cipherLV/cipherLV.py
+drwxrwxrwx   0        0        0        0 2023-05-15 06:24:18.553355 cipherLV-0.1.4/cipherLV.egg-info/
+-rw-rw-rw-   0        0        0      919 2023-05-15 06:24:18.000000 cipherLV-0.1.4/cipherLV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-05-15 06:24:18.000000 cipherLV-0.1.4/cipherLV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 06:24:18.000000 cipherLV-0.1.4/cipherLV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 06:24:18.000000 cipherLV-0.1.4/cipherLV.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 06:24:18.566402 cipherLV-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-15 06:22:57.000000 cipherLV-0.1.4/setup.py
```

### Comparing `cipherLV-0.1.3/PKG-INFO` & `cipherLV-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipherLV
-Version: 0.1.3
+Version: 0.1.4
 Summary: Description: LV cipher is used for encrypting and decrypting with symmetric key
 Home-page: UNKNOWN
 Author: sarath babu
 Author-email: sarathbabu.karunanithi@latentview.com
 License: UNKNOWN
 Description: 
         <h1> cipher LV</h1>
```

### Comparing `cipherLV-0.1.3/cipherLV.egg-info/PKG-INFO` & `cipherLV-0.1.4/cipherLV.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipherLV
-Version: 0.1.3
+Version: 0.1.4
 Summary: Description: LV cipher is used for encrypting and decrypting with symmetric key
 Home-page: UNKNOWN
 Author: sarath babu
 Author-email: sarathbabu.karunanithi@latentview.com
 License: UNKNOWN
 Description: 
         <h1> cipher LV</h1>
```

### Comparing `cipherLV-0.1.3/cipherLV.py` & `cipherLV-0.1.4/cipherLV/cipherLV.py`

 * *Files identical despite different names*

### Comparing `cipherLV-0.1.3/setup.py` & `cipherLV-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 # Setting up
 setup(
     name="cipherLV",
-    version="0.1.3",
+    version="0.1.4",
     author="sarath babu",
     author_email="sarathbabu.karunanithi@latentview.com",
     description='Description: LV cipher is used for encrypting and decrypting with symmetric key',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     py_modules=['cipherLV'],
```

