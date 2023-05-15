# Comparing `tmp/mtANN-0.1.3.tar.gz` & `tmp/mtANN-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mtANN-0.1.3.tar", last modified: Mon May 15 11:32:21 2023, max compression
+gzip compressed data, was "dist/mtANN-0.1.4.tar", last modified: Mon May 15 11:35:47 2023, max compression
```

## Comparing `mtANN-0.1.3.tar` & `mtANN-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 11:32:21.000000 mtANN-0.1.3/
--rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 11:32:21.000000 mtANN-0.1.3/PKG-INFO
--rw-r--r--   0 xyxuan     (501) staff       (20)     2686 2023-05-15 11:31:58.000000 mtANN-0.1.3/README.md
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 11:32:21.000000 mtANN-0.1.3/mtANN/
--rw-r--r--   0 xyxuan     (501) staff       (20)       52 2023-05-11 13:29:42.000000 mtANN-0.1.3/mtANN/__init__.py
--rw-r--r--   0 xyxuan     (501) staff       (20)    15649 2023-05-11 13:06:28.000000 mtANN-0.1.3/mtANN/model.py
--rw-r--r--   0 xyxuan     (501) staff       (20)     3183 2023-05-11 10:26:48.000000 mtANN-0.1.3/mtANN/utils.py
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 11:32:21.000000 mtANN-0.1.3/mtANN.egg-info/
--rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 11:32:21.000000 mtANN-0.1.3/mtANN.egg-info/PKG-INFO
--rw-r--r--   0 xyxuan     (501) staff       (20)      210 2023-05-15 11:32:21.000000 mtANN-0.1.3/mtANN.egg-info/SOURCES.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 11:32:21.000000 mtANN-0.1.3/mtANN.egg-info/dependency_links.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)      119 2023-05-15 11:32:21.000000 mtANN-0.1.3/mtANN.egg-info/requires.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)        6 2023-05-15 11:32:21.000000 mtANN-0.1.3/mtANN.egg-info/top_level.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)       38 2023-05-15 11:32:21.000000 mtANN-0.1.3/setup.cfg
--rw-r--r--   0 xyxuan     (501) staff       (20)      736 2023-05-15 11:31:27.000000 mtANN-0.1.3/setup.py
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 11:35:47.000000 mtANN-0.1.4/
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 11:35:47.000000 mtANN-0.1.4/PKG-INFO
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2686 2023-05-15 11:31:58.000000 mtANN-0.1.4/README.md
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 11:35:47.000000 mtANN-0.1.4/mtANN/
+-rw-r--r--   0 xyxuan     (501) staff       (20)       40 2023-05-15 11:34:42.000000 mtANN-0.1.4/mtANN/__init__.py
+-rw-r--r--   0 xyxuan     (501) staff       (20)    15649 2023-05-11 13:06:28.000000 mtANN-0.1.4/mtANN/model.py
+-rw-r--r--   0 xyxuan     (501) staff       (20)     3183 2023-05-11 10:26:48.000000 mtANN-0.1.4/mtANN/utils.py
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 11:35:47.000000 mtANN-0.1.4/mtANN.egg-info/
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 11:35:46.000000 mtANN-0.1.4/mtANN.egg-info/PKG-INFO
+-rw-r--r--   0 xyxuan     (501) staff       (20)      210 2023-05-15 11:35:47.000000 mtANN-0.1.4/mtANN.egg-info/SOURCES.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 11:35:46.000000 mtANN-0.1.4/mtANN.egg-info/dependency_links.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)      119 2023-05-15 11:35:46.000000 mtANN-0.1.4/mtANN.egg-info/requires.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)        6 2023-05-15 11:35:46.000000 mtANN-0.1.4/mtANN.egg-info/top_level.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)       38 2023-05-15 11:35:47.000000 mtANN-0.1.4/setup.cfg
+-rw-r--r--   0 xyxuan     (501) staff       (20)      736 2023-05-15 11:35:32.000000 mtANN-0.1.4/setup.py
```

### Comparing `mtANN-0.1.3/PKG-INFO` & `mtANN-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtANN
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
 Author: Yi-Xuan Xiong
 Author-email: xyxuana@mails.ccnu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
```

### Comparing `mtANN-0.1.3/README.md` & `mtANN-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mtANN-0.1.3/mtANN/model.py` & `mtANN-0.1.4/mtANN/model.py`

 * *Files identical despite different names*

### Comparing `mtANN-0.1.3/mtANN/utils.py` & `mtANN-0.1.4/mtANN/utils.py`

 * *Files identical despite different names*

### Comparing `mtANN-0.1.3/mtANN.egg-info/PKG-INFO` & `mtANN-0.1.4/mtANN.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtANN
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
 Author: Yi-Xuan Xiong
 Author-email: xyxuana@mails.ccnu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
```

### Comparing `mtANN-0.1.3/setup.py` & `mtANN-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mtANN", 
-    version="0.1.3",
+    version="0.1.4",
     # py_modules=['mtANN','mtANN.model', 'mtANN.utils'],
     author="Yi-Xuan Xiong",
     author_email="xyxuana@mails.ccnu.edu.cn",
     description="Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

