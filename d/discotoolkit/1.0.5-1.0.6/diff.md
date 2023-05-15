# Comparing `tmp/discotoolkit-1.0.5.tar.gz` & `tmp/discotoolkit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.0.5.tar", last modified: Fri May 12 05:32:43 2023, max compression
+gzip compressed data, was "discotoolkit-1.0.6.tar", last modified: Mon May 15 11:57:42 2023, max compression
```

## Comparing `discotoolkit-1.0.5.tar` & `discotoolkit-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-12 05:32:32.440271 discotoolkit-1.0.5/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.5/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      729 2023-05-12 05:32:32.436271 discotoolkit-1.0.5/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)     1930 2023-05-12 05:32:16.000000 discotoolkit-1.0.5/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-12 05:32:32.412272 discotoolkit-1.0.5/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)    16691 2023-05-11 01:50:32.000000 discotoolkit-1.0.5/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.5/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     2479 2023-05-12 05:20:20.000000 discotoolkit-1.0.5/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     7377 2023-05-12 05:28:51.000000 discotoolkit-1.0.5/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.0.5/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.5/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      130 2023-05-12 05:32:13.000000 discotoolkit-1.0.5/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-12 05:32:32.432271 discotoolkit-1.0.5/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      729 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)      106 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-12 05:32:32.440271 discotoolkit-1.0.5/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1115 2023-05-12 05:30:50.000000 discotoolkit-1.0.5/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-15 11:57:30.795261 discotoolkit-1.0.6/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.6/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      689 2023-05-15 11:57:30.795261 discotoolkit-1.0.6/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2348 2023-05-15 11:56:49.000000 discotoolkit-1.0.6/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-15 11:57:30.779261 discotoolkit-1.0.6/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    17688 2023-05-15 11:46:41.000000 discotoolkit-1.0.6/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.6/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.0.6/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     7377 2023-05-15 05:29:07.000000 discotoolkit-1.0.6/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.0.6/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.6/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      203 2023-05-15 11:53:20.000000 discotoolkit-1.0.6/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-15 11:57:30.791261 discotoolkit-1.0.6/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      689 2023-05-15 11:57:30.000000 discotoolkit-1.0.6/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-15 11:57:30.000000 discotoolkit-1.0.6/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-15 11:57:30.000000 discotoolkit-1.0.6/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)      246 2023-05-15 11:57:30.000000 discotoolkit-1.0.6/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-15 11:57:30.000000 discotoolkit-1.0.6/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-15 11:57:30.795261 discotoolkit-1.0.6/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1135 2023-05-15 11:52:42.000000 discotoolkit-1.0.6/setup.py
```

### Comparing `discotoolkit-1.0.5/PKG-INFO` & `discotoolkit-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.5
+Version: 1.0.6
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 Requires-Python: >=3.8.16
-Description-Content-Type: text/markdown
 
 
     DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
     
 
     Filter and download DISCO data based on sample metadata and cell type information
```

### Comparing `discotoolkit-1.0.5/README.md` & `discotoolkit-1.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,19 @@
  * @Descripttion: 
  * @version: 
  * @Author: Mengwei Li
  * @Date: 2023-04-16 21:20:42
  * @LastEditors: Mengwei Li
  * @LastEditTime: 2023-04-16 21:22:03
 -->
-# DISCOtoolkit 1.0.5
+[![Documentation Status](https://readthedocs.org/projects/discotoolkit-py/badge/?version=latest)](https://discotoolkit-py.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/discotoolkit?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/discotoolkit)
 
-DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). Read the documentation [DISCOtoolkit](https://jinmiaochenlab.github.io/DISCOtoolkit_py/). It provides the following functions:
+# DISCOtoolkit 1.0.6
+
+DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). Read the documentation [DISCOtoolkit](https://discotoolkit-py.readthedocs.io/en/latest/). It provides the following functions:
 
 - Filter and download DISCO data based on sample metadata and cell type information
 - CELLiD: cell type annotation
 - scEnrichment: geneset enrichment using DISCO DEGs
 
 Dependency Requirements:
 
@@ -32,15 +34,15 @@
 conda install pip
 conda install ipykernel
 python -m ipykernel install --user --name disco --display-name "disco"
 ```
 
 Installation using pip:
 ``` 
-python -m pip install discotoolkit
+python -m pip install discotoolkit # adding -U for installing the latest version
 ```
 
 ## Basic Usage
 Example in Jupyter notebook.
 
 <em>please select disco as the kernel for running the jupyter notebook</em>
```

### Comparing `discotoolkit-1.0.5/discotoolkit/CELLiD.py` & `discotoolkit-1.0.6/discotoolkit/CELLiD.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,19 @@
 def CELLiD_cluster(rna, ref_data : pd.DataFrame = None, ref_deg : pd.DataFrame = None, atlas : str = None, n_predict : int = 1, ref_path : str = None, ncores : int = 10):
     """Cell type annotation using reference data and compute the correlation between the user cell gene expression as compare
         to the reference data. The celltype with highest correlation will be concluded as the celltype
 
     Args:
         rna (Pandas DataFrame | Numpy array): user define dataframe. Need to transpose so that the index is the genes
         ref_data (Pandas DataFrame, optional): Reference dataframe used to compute for the cell type annotation. Defaults to None.
-        ref_deg (Pandas, DataFrame): reference DEG database. Defaults to None.
+        ref_deg (Pandas DataFrame): reference DEG database. Defaults to None.
         atlas (String, optional): String of atlas that the user want to use as the reference. Defaults to None.
         n_predict (Integer, optional): number of predicted celltype. Defaults to 1.
         ref_path (string, optional): path string to the reference data. Defaults to None.
-        ncores (int, optional): number of CPU cores used to run the data. Defaults to 10.
+        ncores (Integer, optional): number of CPU cores used to run the data. Defaults to 10.
 
     Returns:
         Pandas DataFrame: return the Pandas DataFrame along with the correlation score.
     """
 
     # initialize the pandarallel for parallel processing
     pandarallel.initialize(nb_workers=ncores)
@@ -210,15 +210,26 @@
 
     return pivot# return pandas dataframe in the format the same original R package
 
 """
 Geneset enrichment analysis using DISCO data
 """
 
-def CELLiD_enrichment(input, reference = None, ref_path : str = None, ncores = 10):
+def CELLiD_enrichment(input : pd.DataFrame, reference : pd.DataFrame = None, ref_path : str = None, ncores : int = 10):
+    """Function to generate enrichment analysis based on the reference gene sets and following the DISCO pipeline.
+
+    Args:
+        input (Pandas DataFrame): User defined Dataframe in the format of `(gene, fc)`. `gene` refer to gene name and `fc` refer to log fold change.
+        reference (Pandas DataFrame, optional): Reference datasets from DISCO. Recommend to put as None as the function will automatically retrieve the dataset from the server. Defaults to None.
+        ref_path (String, optional): Path to the reference dataset or reading the file if it is existed. Defaults to None.
+        ncores (Integer, optional): Number of CPU cores to run the function. Defaults to 10.
+
+    Returns:
+        Pandas DataFrame: return the significant gene sets that is over-represented in a large set of genes.
+    """
 
     # check input data
     # check if the input type is a DataFrame
     if not(isinstance(input, pd.DataFrame)):
         logging.error("The input must be a dataframe")
 
     # check if the user provide more than the needed column which are gene and fc
@@ -242,20 +253,23 @@
         if ref_path is None:
             ref_path = "DISCOtmp"
 
         # if the path does not exist, we create a default directory
         if not os.path.exists(ref_path):
             os.mkdir(ref_path)
         
-        # downloading the geneset data from disco database
-        response = requests.get(url=prefix_disco_url +"/getGeneSetPkl", timeout=timeout)
-        open(ref_path + "/ref_geneset.pkl", "wb").write(response.content)
-
-        # read the data into pandas dataframe for subsequent analysis
-        reference = pd.read_pickle(ref_path + "/ref_geneset.pkl", compression = {'method':'gzip','compresslevel':6})
+        # check if the file does not exist
+        if not (os.path.exists(ref_path + "/ref_geneset.pkl")):
+            # downloading the geneset data from disco database
+            response = requests.get(url=prefix_disco_url +"/getGeneSetPkl", timeout=timeout)
+            open(ref_path + "/ref_geneset.pkl", "wb").write(response.content)
+
+        else:
+            # read the data into pandas dataframe for subsequent analysis
+            reference = pd.read_pickle(ref_path + "/ref_geneset.pkl", compression = {'method':'gzip','compresslevel':6})
 
     # rename the name data to include the reference atlas
     reference["name"] = reference["name"] + " in " + reference["atlas"]
 
     # condition when the user provide the fold change for the enrichment analysis
     if input_shape == 2:
         input["fc"] == 2 ** input["fc"] # 2 to the power of fc
```

### Comparing `discotoolkit-1.0.5/discotoolkit/DiscoClass.py` & `discotoolkit-1.0.6/discotoolkit/DiscoClass.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     include_cell_type_children  Bool      e.g. True;
     min_cell_per_sample         Int       e.g. 300;
 
     return Class object
     """
 
     def __init__(self, sample = None, project = None, tissue = None, disease = None, platform = None, sample_type = None,
-                 cell_type = None, cell_type_confidence = "medium", include_cell_type_children = True, min_cell_per_sample = 100):
+                 cell_type = None, cell_type_confidence : str = "medium", include_cell_type_children : bool = True, min_cell_per_sample : int = 100):
         
         # handling for string and list input
         self.sample = self.convert_to_list(sample) # sample id
         self.project = self.convert_to_list(project) # project, lab, or dataset from different author
         self.tissue = self.convert_to_list(tissue) # organ tissue 
         self.disease = self.convert_to_list(disease) # cancer or non cancer, or COVID-1e9 disease
         self.platform = self.convert_to_list(platform) # sequencing platform
```

### Comparing `discotoolkit-1.0.5/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.0.6/discotoolkit/DownloadDiscoData.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.5/discotoolkit/GetMetadata.py` & `discotoolkit-1.0.6/discotoolkit/GetMetadata.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.5/discotoolkit/GlobalVariable.py` & `discotoolkit-1.0.6/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.5/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.0.6/discotoolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.5
+Version: 1.0.6
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 Requires-Python: >=3.8.16
-Description-Content-Type: text/markdown
 
 
     DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
     
 
     Filter and download DISCO data based on sample metadata and cell type information
```

### Comparing `discotoolkit-1.0.5/setup.py` & `discotoolkit-1.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
+with open('docs/version.txt', 'r') as f:
+    version = f.read().strip()
+
 setup(
     name='discotoolkit',
-    version='1.0.5',
+    version=version,
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
     install_requires=requirements,
     python_requires = '>=3.8.16',
@@ -18,9 +21,8 @@
     long_description="""
     DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
     \n
     Filter and download DISCO data based on sample metadata and cell type information
     \nCELLiD: cell type annotation
     \nscEnrichment: geneset enrichment using DISCO DEGs
     """,
-    long_description_content_type = 'text/markdown',
 )
```

