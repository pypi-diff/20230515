# Comparing `tmp/mtANN-0.1.1.tar.gz` & `tmp/mtANN-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mtANN-0.1.1.tar", last modified: Mon May 15 09:29:59 2023, max compression
+gzip compressed data, was "dist/mtANN-0.1.2.tar", last modified: Mon May 15 09:49:54 2023, max compression
```

## Comparing `mtANN-0.1.1.tar` & `mtANN-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 09:29:59.000000 mtANN-0.1.1/
--rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 09:29:59.000000 mtANN-0.1.1/PKG-INFO
--rw-r--r--   0 xyxuan     (501) staff       (20)     2686 2023-05-15 01:38:34.000000 mtANN-0.1.1/README.md
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/
--rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/PKG-INFO
--rw-r--r--   0 xyxuan     (501) staff       (20)      162 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/SOURCES.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/dependency_links.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)      114 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/requires.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/top_level.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)       38 2023-05-15 09:29:59.000000 mtANN-0.1.1/setup.cfg
--rw-r--r--   0 xyxuan     (501) staff       (20)      731 2023-05-15 09:23:26.000000 mtANN-0.1.1/setup.py
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 09:49:54.000000 mtANN-0.1.2/
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 09:49:54.000000 mtANN-0.1.2/PKG-INFO
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2686 2023-05-15 09:49:46.000000 mtANN-0.1.2/README.md
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 09:49:54.000000 mtANN-0.1.2/mtANN.egg-info/
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 09:49:54.000000 mtANN-0.1.2/mtANN.egg-info/PKG-INFO
+-rw-r--r--   0 xyxuan     (501) staff       (20)      162 2023-05-15 09:49:54.000000 mtANN-0.1.2/mtANN.egg-info/SOURCES.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 09:49:54.000000 mtANN-0.1.2/mtANN.egg-info/dependency_links.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)      119 2023-05-15 09:49:54.000000 mtANN-0.1.2/mtANN.egg-info/requires.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 09:49:54.000000 mtANN-0.1.2/mtANN.egg-info/top_level.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)       38 2023-05-15 09:49:54.000000 mtANN-0.1.2/setup.cfg
+-rw-r--r--   0 xyxuan     (501) staff       (20)      736 2023-05-15 09:45:12.000000 mtANN-0.1.2/setup.py
```

### Comparing `mtANN-0.1.1/PKG-INFO` & `mtANN-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtANN
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
 Author: Yi-Xuan Xiong
 Author-email: xyxuana@mails.ccnu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
@@ -35,15 +35,15 @@
 - Python: 3.8.15
 - Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install mtANN==0.1.0`
+`pip install mtANN==0.1.2`
 
 # Useage
 The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
 # Installation
```

### Comparing `mtANN-0.1.1/README.md` & `mtANN-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 - Python: 3.8.15
 - Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install mtANN==0.1.0`
+`pip install mtANN==0.1.2`
 
 # Useage
 The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
 # Installation
```

### Comparing `mtANN-0.1.1/mtANN.egg-info/PKG-INFO` & `mtANN-0.1.2/mtANN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtANN
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
 Author: Yi-Xuan Xiong
 Author-email: xyxuana@mails.ccnu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
@@ -35,15 +35,15 @@
 - Python: 3.8.15
 - Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install mtANN==0.1.0`
+`pip install mtANN==0.1.2`
 
 # Useage
 The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
 # Installation
```

### Comparing `mtANN-0.1.1/setup.py` & `mtANN-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mtANN", 
-    version="0.1.1",
+    version="0.1.2",
     # py_modules=['mtANN','mtANN.model', 'mtANN.utils'],
     author="Yi-Xuan Xiong",
     author_email="xyxuana@mails.ccnu.edu.cn",
     description="Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     python_requires='>=3.7',
     install_requires=['pandas>=1.2.3', 'numpy>=1.19.2',
-    'scanpy>=1.9.0','scipy>=1.6.1','sklearn>=0.24.1',
+    'scanpy>=1.9.0','scipy>=1.6.1','scikit-learn>=0.24.1',
     'torch>=1.9.1','giniclust3>=1.1.0','rpy2>=3.4.1'],
 )
```

