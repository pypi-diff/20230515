# Comparing `tmp/mtANN-0.1.0.tar.gz` & `tmp/mtANN-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mtANN-0.1.0.tar", last modified: Mon May  8 08:19:26 2023, max compression
+gzip compressed data, was "dist/mtANN-0.1.1.tar", last modified: Mon May 15 09:29:59 2023, max compression
```

## Comparing `mtANN-0.1.0.tar` & `mtANN-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-08 08:19:26.000000 mtANN-0.1.0/
--rw-r--r--   0 xyxuan     (501) staff       (20)     2937 2023-05-08 08:19:26.000000 mtANN-0.1.0/PKG-INFO
--rw-rw-r--   0 xyxuan     (501) staff       (20)     2644 2023-05-08 08:14:23.000000 mtANN-0.1.0/README.md
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-08 08:19:26.000000 mtANN-0.1.0/mtANN.egg-info/
--rw-r--r--   0 xyxuan     (501) staff       (20)     2937 2023-05-08 08:19:25.000000 mtANN-0.1.0/mtANN.egg-info/PKG-INFO
--rw-r--r--   0 xyxuan     (501) staff       (20)      134 2023-05-08 08:19:26.000000 mtANN-0.1.0/mtANN.egg-info/SOURCES.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-08 08:19:25.000000 mtANN-0.1.0/mtANN.egg-info/dependency_links.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)        6 2023-05-08 08:19:25.000000 mtANN-0.1.0/mtANN.egg-info/top_level.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)       38 2023-05-08 08:19:26.000000 mtANN-0.1.0/setup.cfg
--rw-rw-r--   0 xyxuan     (501) staff       (20)      568 2023-05-08 08:19:19.000000 mtANN-0.1.0/setup.py
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 09:29:59.000000 mtANN-0.1.1/
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 09:29:59.000000 mtANN-0.1.1/PKG-INFO
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2686 2023-05-15 01:38:34.000000 mtANN-0.1.1/README.md
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/
+-rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/PKG-INFO
+-rw-r--r--   0 xyxuan     (501) staff       (20)      162 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/SOURCES.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/dependency_links.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)      114 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/requires.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 09:29:59.000000 mtANN-0.1.1/mtANN.egg-info/top_level.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)       38 2023-05-15 09:29:59.000000 mtANN-0.1.1/setup.cfg
+-rw-r--r--   0 xyxuan     (501) staff       (20)      731 2023-05-15 09:23:26.000000 mtANN-0.1.1/setup.py
```

### Comparing `mtANN-0.1.0/PKG-INFO` & `mtANN-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,19 @@
-Metadata-Version: 2.1
-Name: mtANN
-Version: 0.1.0
-Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
-Author: Yi-Xuan Xiong
-Author-email: xyxuana@mails.ccnu.edu.cn
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
 
 mtANN is a novel cell-type annotation framework
 that integrates ensemble learning and deep learning
 simultaneously, to annotate cells in a new query dataset with the help of multiple well-labeled reference datasets. It takes multiple well-labeled reference datasets and a query dataset that needs to be annotated as input. It begins with generating a series of subsets for each reference dataset by adopting various gene selection methods. Next, for each reference subset, a base classification model is trained based on neural networks. Then, mtANN annotates the cells in the query dataset by integrating the prediction results from all the base classification models. Finally, it identifies cells that may belong to cell types not observed in the reference datasets according to the uncertainty of the predictions.
 
 ![Figure1](Figure1.png)
 
 ## System Requirements
 
 Python support packages: pandas, numpy, scanpy, scipy, sklearn, torch, giniclust3, rpy2
+
 R support packages: limma, Seurat, parallel
 
 ## Versions the software has been tested on
 
 ### Environment 1
 - System: Ubuntu 18.04.5
 - Python: 3.8.8
@@ -34,21 +26,25 @@
 - Python: 3.8.15
 - Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install -i https://test.pypi.org/simple/ mtANN==0.1.0`
+`pip install mtANN==0.1.0`
 
 # Useage
-The mtANN repository includes the mtANN code files in the `mtANN` folder and provides the Pancreas datasets collection and mtANN-selected gene sets in the `dataset` folder. In addition, a usage example is provided, which specifically shows the format of the input data and the usage of the main function.
+The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
+# Installation
+
+`pip install mtANN==0.1.0`
+
  
 # Contact
 
 Please do not hesitate to contact Miss Yi-Xuan Xiong ([xyxuana@mails.ccnu.edu.cn](xyxuana@mails.ccnu.edu.cn)) or Dr. Xiao-Fei Zhang ([zhangxf@ccnu.edu.cn](zhangxf@ccnu.edu.cn)) to seek any clarifications regarding any contents or operation of the archive.
```

### Comparing `mtANN-0.1.0/README.md` & `mtANN-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+Metadata-Version: 2.1
+Name: mtANN
+Version: 0.1.1
+Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
+Author: Yi-Xuan Xiong
+Author-email: xyxuana@mails.ccnu.edu.cn
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
 
 mtANN is a novel cell-type annotation framework
 that integrates ensemble learning and deep learning
 simultaneously, to annotate cells in a new query dataset with the help of multiple well-labeled reference datasets. It takes multiple well-labeled reference datasets and a query dataset that needs to be annotated as input. It begins with generating a series of subsets for each reference dataset by adopting various gene selection methods. Next, for each reference subset, a base classification model is trained based on neural networks. Then, mtANN annotates the cells in the query dataset by integrating the prediction results from all the base classification models. Finally, it identifies cells that may belong to cell types not observed in the reference datasets according to the uncertainty of the predictions.
 
 ![Figure1](Figure1.png)
 
 ## System Requirements
 
 Python support packages: pandas, numpy, scanpy, scipy, sklearn, torch, giniclust3, rpy2
+
 R support packages: limma, Seurat, parallel
 
 ## Versions the software has been tested on
 
 ### Environment 1
 - System: Ubuntu 18.04.5
 - Python: 3.8.8
@@ -25,21 +35,25 @@
 - Python: 3.8.15
 - Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install -i https://test.pypi.org/simple/ mtANN==0.1.0`
+`pip install mtANN==0.1.0`
 
 # Useage
-The mtANN repository includes the mtANN code files in the `mtANN` folder and provides the Pancreas datasets collection and mtANN-selected gene sets in the `dataset` folder. In addition, a usage example is provided, which specifically shows the format of the input data and the usage of the main function.
+The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
+# Installation
+
+`pip install mtANN==0.1.0`
+
  
 # Contact
 
 Please do not hesitate to contact Miss Yi-Xuan Xiong ([xyxuana@mails.ccnu.edu.cn](xyxuana@mails.ccnu.edu.cn)) or Dr. Xiao-Fei Zhang ([zhangxf@ccnu.edu.cn](zhangxf@ccnu.edu.cn)) to seek any clarifications regarding any contents or operation of the archive.
```

### Comparing `mtANN-0.1.0/mtANN.egg-info/PKG-INFO` & `mtANN-0.1.1/mtANN.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtANN
-Version: 0.1.0
+Version: 0.1.1
 Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
 Author: Yi-Xuan Xiong
 Author-email: xyxuana@mails.ccnu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
@@ -14,14 +14,15 @@
 simultaneously, to annotate cells in a new query dataset with the help of multiple well-labeled reference datasets. It takes multiple well-labeled reference datasets and a query dataset that needs to be annotated as input. It begins with generating a series of subsets for each reference dataset by adopting various gene selection methods. Next, for each reference subset, a base classification model is trained based on neural networks. Then, mtANN annotates the cells in the query dataset by integrating the prediction results from all the base classification models. Finally, it identifies cells that may belong to cell types not observed in the reference datasets according to the uncertainty of the predictions.
 
 ![Figure1](Figure1.png)
 
 ## System Requirements
 
 Python support packages: pandas, numpy, scanpy, scipy, sklearn, torch, giniclust3, rpy2
+
 R support packages: limma, Seurat, parallel
 
 ## Versions the software has been tested on
 
 ### Environment 1
 - System: Ubuntu 18.04.5
 - Python: 3.8.8
@@ -34,21 +35,25 @@
 - Python: 3.8.15
 - Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install -i https://test.pypi.org/simple/ mtANN==0.1.0`
+`pip install mtANN==0.1.0`
 
 # Useage
-The mtANN repository includes the mtANN code files in the `mtANN` folder and provides the Pancreas datasets collection and mtANN-selected gene sets in the `dataset` folder. In addition, a usage example is provided, which specifically shows the format of the input data and the usage of the main function.
+The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
+# Installation
+
+`pip install mtANN==0.1.0`
+
  
 # Contact
 
 Please do not hesitate to contact Miss Yi-Xuan Xiong ([xyxuana@mails.ccnu.edu.cn](xyxuana@mails.ccnu.edu.cn)) or Dr. Xiao-Fei Zhang ([zhangxf@ccnu.edu.cn](zhangxf@ccnu.edu.cn)) to seek any clarifications regarding any contents or operation of the archive.
```

### Comparing `mtANN-0.1.0/setup.py` & `mtANN-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mtANN", 
-    version="0.1.0",
-    py_modules=['mtANN.mtANN_model', 'mtANN.mtANN_utils'],
+    version="0.1.1",
+    # py_modules=['mtANN','mtANN.model', 'mtANN.utils'],
     author="Yi-Xuan Xiong",
     author_email="xyxuana@mails.ccnu.edu.cn",
     description="Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     python_requires='>=3.7',
+    install_requires=['pandas>=1.2.3', 'numpy>=1.19.2',
+    'scanpy>=1.9.0','scipy>=1.6.1','sklearn>=0.24.1',
+    'torch>=1.9.1','giniclust3>=1.1.0','rpy2>=3.4.1'],
 )
```

