# Comparing `tmp/unpast-0.1.5.tar.gz` & `tmp/unpast-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unpast-0.1.5.tar", max compression
+gzip compressed data, was "unpast-0.1.6.tar", max compression
```

## Comparing `unpast-0.1.5.tar` & `unpast-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-05-08 14:23:44.608899 unpast-0.1.5/LICENSE
--rw-r--r--   0        0        0     4613 2023-05-09 16:58:50.748770 unpast-0.1.5/README.md
--rw-r--r--   0        0        0     1048 2023-05-09 17:00:41.957805 unpast-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 14:23:44.608899 unpast-0.1.5/unpast/__init__.py
--rw-r--r--   0        0        0      815 2023-05-09 13:58:10.515828 unpast-0.1.5/unpast/install_r_dependencies.py
--rw-r--r--   0        0        0    36567 2023-05-08 14:23:44.716900 unpast-0.1.5/unpast/method.py
--rw-r--r--   0        0        0     4443 2023-05-08 14:23:44.768901 unpast-0.1.5/unpast/run_desmond.py
--rwxr-xr-x   0        0        0    12107 2023-05-09 12:58:02.266229 unpast-0.1.5/unpast/run_unpast.py
--rw-r--r--   0        0        0      100 2023-05-08 14:23:44.768901 unpast-0.1.5/unpast/setup.py
--rw-r--r--   0        0        0        0 2023-05-08 14:23:44.768901 unpast-0.1.5/unpast/utils/__init__.py
--rw-r--r--   0        0        0    25724 2023-05-08 14:23:44.768901 unpast-0.1.5/unpast/utils/eval.py
--rw-r--r--   0        0        0    57918 2023-05-08 14:23:44.768901 unpast-0.1.5/unpast/utils/method.py
--rw-r--r--   0        0        0    19957 2023-05-08 14:23:44.768901 unpast-0.1.5/unpast/utils/pgm.py
--rw-r--r--   0        0        0     1757 2023-05-08 14:23:44.768901 unpast-0.1.5/unpast/utils/run_WGCNA.R
--rw-r--r--   0        0        0     5758 1970-01-01 00:00:00.000000 unpast-0.1.5/setup.py
--rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 unpast-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 14:23:44.608899 unpast-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5103 2023-05-11 13:38:54.371965 unpast-0.1.6/README.md
+-rw-r--r--   0        0        0     1064 2023-05-11 14:35:55.803952 unpast-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 14:23:44.608899 unpast-0.1.6/unpast/__init__.py
+-rw-r--r--   0        0        0      815 2023-05-09 13:58:10.515828 unpast-0.1.6/unpast/install_r_dependencies.py
+-rw-r--r--   0        0        0    36567 2023-05-08 14:23:44.716900 unpast-0.1.6/unpast/method.py
+-rw-r--r--   0        0        0     4443 2023-05-08 14:23:44.768901 unpast-0.1.6/unpast/run_desmond.py
+-rwxr-xr-x   0        0        0    12107 2023-05-09 12:58:02.266229 unpast-0.1.6/unpast/run_unpast.py
+-rw-r--r--   0        0        0      100 2023-05-08 14:23:44.768901 unpast-0.1.6/unpast/setup.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:23:44.768901 unpast-0.1.6/unpast/utils/__init__.py
+-rw-r--r--   0        0        0    25724 2023-05-08 14:23:44.768901 unpast-0.1.6/unpast/utils/eval.py
+-rw-r--r--   0        0        0    57918 2023-05-08 14:23:44.768901 unpast-0.1.6/unpast/utils/method.py
+-rw-r--r--   0        0        0    19957 2023-05-08 14:23:44.768901 unpast-0.1.6/unpast/utils/pgm.py
+-rw-r--r--   0        0        0     1757 2023-05-08 14:23:44.768901 unpast-0.1.6/unpast/utils/run_WGCNA.R
+-rw-r--r--   0        0        0     6289 1970-01-01 00:00:00.000000 unpast-0.1.6/setup.py
+-rw-r--r--   0        0        0     6207 1970-01-01 00:00:00.000000 unpast-0.1.6/PKG-INFO
```

### Comparing `unpast-0.1.5/LICENSE` & `unpast-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/README.md` & `unpast-0.1.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,42 +5,50 @@
 ![alt text](https://github.com/ozolotareva/DESMOND2/blob/a26d8d7b2075d47a4edc8fc9ce7eca72a2dac7db/poster/DESMOND2_steps2.png?raw=true)
 
 
 Webserver: https://unpast.zbh.uni-hamburg.de/
 
 ## Installation
 This UnPaSt can be installed using `pip./poster/DESMOND2.png`, `poetry`, run using `Docker`, or as a script (see examples section). Follow the appropriate instructions below for your preferred method.
-You need to have R and Python 3.8 installed.
+You need to have R (for WGCNA, it is suggested to use v.1.70-3) and **Python 3.8-3.10** installed. The main reason why Python 3.11 is not supported is because Scikit-network does not support it now.
+
+**Using different Python versions, even with the same libraries versions, leads to slightly different computational results.**
 
 1. Using pip: \
 To install the project using `pip`, first make sure you have `pip` installed on your system. If you haven't installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/). \
 Once `pip` is installed, you can install the project by running the following command:
 ```bash
 pip install unpast
 ```
 Run it:
 ```bash
 run_unpast -h
 ```
 **Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
 ```bash
 python -m unpast.install_r_dependencies
+
+# or you can install it directly
+R -e "install.packages('BiocManager'); BiocManager::install('WGCNA')"
 ```
 2. Installation using Poetry: \
 To install the package using Poetry, first make sure you have Poetry installed, clone the repo and then run:
 ```bash
 poetry add unpast
 ```
 Run it:
 ```bash
 poetry run run_unpast -h
 ```
 **Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
 ```bash
 poetry run python -m unpast.install_r_dependencies
+
+# or you can install it directly
+R -e "install.packages('BiocManager'); BiocManager::install('WGCNA')"
 ```
 3. Running with Docker: \
 You can also run the package using Docker. First, pull the Docker image:
 ```bash
 docker pull freddsle/unpast:latest
 ```
 Next, run the container:
```

### Comparing `unpast-0.1.5/pyproject.toml` & `unpast-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unpast"
-version = "0.1.5"
+version = "0.1.6"
 description = "A novel method for unsupervised patient stratification."
 readme = "README.md"
 license = "GPL-3.0"
 authors = [
     "Olga Zolotareva (ozolotareva)", 
     "Andreas Maier (AndiMajore)",
     "Fernando M. Delgado-Chaves (fmdelgado)", 
@@ -17,26 +17,27 @@
     "Yuliya Burankova (freddsle)",
     "Fernando M. Delgado-Chaves (fmdelgado)", 
     "Fábio Patroni (fpatroni)",
 ]
 repository = "https://github.com/ozolotareva/DESMOND2"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.9"
-fisher = "0.1.9"
+python = ">=3.8,<3.11"
+fisher = "0.1.10"
 jenkspy = "0.2.0"
 pandas = "1.4.2"
 python-louvain = "0.15"
 matplotlib-venn = "0.11.6"
-numba = ">=0.51.2"
+numba = "0.55.2"
 numpy = "1.22.3"
-scikit-learn = "0.23.1"
-scikit-network = "0.24.0"
-scipy = "1.7.1"
+scikit-learn = "1.1.0"
+scikit-network = "0.25.0"
+scipy = "1.7.3"
 statsmodels = "0.13.2"
+kneed = "^0.8.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 run_unpast = "unpast.run_unpast:main"
```

### Comparing `unpast-0.1.5/unpast/install_r_dependencies.py` & `unpast-0.1.6/unpast/install_r_dependencies.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/unpast/method.py` & `unpast-0.1.6/unpast/method.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/unpast/run_desmond.py` & `unpast-0.1.6/unpast/run_desmond.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/unpast/run_unpast.py` & `unpast-0.1.6/unpast/run_unpast.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/unpast/utils/eval.py` & `unpast-0.1.6/unpast/utils/eval.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/unpast/utils/method.py` & `unpast-0.1.6/unpast/utils/method.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/unpast/utils/pgm.py` & `unpast-0.1.6/unpast/utils/pgm.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/unpast/utils/run_WGCNA.R` & `unpast-0.1.6/unpast/utils/run_WGCNA.R`

 * *Files identical despite different names*

### Comparing `unpast-0.1.5/setup.py` & `unpast-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,41 +4,42 @@
 packages = \
 ['unpast', 'unpast.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fisher==0.1.9',
+['fisher==0.1.10',
  'jenkspy==0.2.0',
+ 'kneed>=0.8.3,<0.9.0',
  'matplotlib-venn==0.11.6',
- 'numba>=0.51.2',
+ 'numba==0.55.2',
  'numpy==1.22.3',
  'pandas==1.4.2',
  'python-louvain==0.15',
- 'scikit-learn==0.23.1',
- 'scikit-network==0.24.0',
- 'scipy==1.7.1',
+ 'scikit-learn==1.1.0',
+ 'scikit-network==0.25.0',
+ 'scipy==1.7.3',
  'statsmodels==0.13.2']
 
 entry_points = \
 {'console_scripts': ['run_unpast = unpast.run_unpast:main']}
 
 setup_kwargs = {
     'name': 'unpast',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'A novel method for unsupervised patient stratification.',
-    'long_description': '# UnPaSt\n\nUnPaSt is a novel method for identification of differentially expressed biclusters in gene expression matrix. It searches for gene sets up- or down-regulated in subsets of samples:\n\n![alt text](https://github.com/ozolotareva/DESMOND2/blob/a26d8d7b2075d47a4edc8fc9ce7eca72a2dac7db/poster/DESMOND2_steps2.png?raw=true)\n\n\nWebserver: https://unpast.zbh.uni-hamburg.de/\n\n## Installation\nThis UnPaSt can be installed using `pip./poster/DESMOND2.png`, `poetry`, run using `Docker`, or as a script (see examples section). Follow the appropriate instructions below for your preferred method.\nYou need to have R and Python 3.8 installed.\n\n1. Using pip: \\\nTo install the project using `pip`, first make sure you have `pip` installed on your system. If you haven\'t installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/). \\\nOnce `pip` is installed, you can install the project by running the following command:\n```bash\npip install unpast\n```\nRun it:\n```bash\nrun_unpast -h\n```\n**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:\n```bash\npython -m unpast.install_r_dependencies\n```\n2. Installation using Poetry: \\\nTo install the package using Poetry, first make sure you have Poetry installed, clone the repo and then run:\n```bash\npoetry add unpast\n```\nRun it:\n```bash\npoetry run run_unpast -h\n```\n**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:\n```bash\npoetry run python -m unpast.install_r_dependencies\n```\n3. Running with Docker: \\\nYou can also run the package using Docker. First, pull the Docker image:\n```bash\ndocker pull freddsle/unpast:latest\n```\nNext, run the container:\n```bash\ndocker run -v /your/data/path/:/user_data/ freddsle/unpast:latest --exprs /user_data/exprs.tsv --out_dir /user_data/out_dir/\n```\n\n## Examples\n* UnPaSt requires a tab-separated file with standardized expressions of genes (or transcripts) in rows, and samples in columns. Gene and sample names must be unique. \n* A subset of 200 randomly chosen samples from TCGA-BRCA and UnPaSt output:\n[test data](https://unpast-backend.zbh.uni-hamburg.de/download_example)\n\n<pre>\n# running UnPaSt with default parameters and example data\npython ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename TCGA_200_results\n\n# with different binarization and clustering methods\npython ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename results --binarization ward --clustering WGCNA\n\n# help\npython ./unpast/run_unpast.py -h\n</pre>\n\n## Outputs\n* \\<basename\\>.bin=[GMM|Jenks],clust=[Louvain|WGCNA|DESMOND].biclusters.tsv - a .tsv table with found biclsuters, where \n    - avgSNR is average SNR over all genes in the biclusters\n    - columns "n_genes" and "n_samples" provide the numbers of genes and samples, respectively \n    - "gene","sample" contain gene and sample names respectively\n    - "gene_indexes" and  "sample_indexes" - 0-based gene and sample indexes in the input matrix.\n* binarized expressions, background distributions of SNR for each bicluster size and binarization statistics [if clustering is WGCNA,  or  \'--save_binary\' flag is added]\n* modules found by WGCNA [if clustering is WGCNA]\n\n# About \nUnPaSt is an unconstrained version of DESMOND method ([repository](https://github.com/ozolotareva/DESMOND), [publication](https://academic.oup.com/bioinformatics/article/37/12/1691/6039116?login=true))\n\nMajor modifications:\n * it does not require the network of gene interactions \n * UnPaSt clusters individual genes instead of gene pairs\n * uses Gaussian mixture models or Jenks method for binarization of individual gene expressions\n * SNR threshold is authomatically determined; it depends on bicluster size in samples and user-defined p-value cutoff\n \n## License\nFree for non-for-profit use. For commercial use please contact the developers. \n\n### Poster CDCS workshop\'22\n![./poster/DESMOND2_poster_v5.png](https://github.com/ozolotareva/DESMOND2/blob/a26d8d7b2075d47a4edc8fc9ce7eca72a2dac7db/poster/DESMOND2_poster_v5.png?raw=true)\n### Poster ISMB and MCCMB\'21\n![./poster/DESMOND2.pdf](https://github.com/ozolotareva/DESMOND2/blob/a26d8d7b2075d47a4edc8fc9ce7eca72a2dac7db/poster/DESMOND2.png?raw=true)\n',
+    'long_description': '# UnPaSt\n\nUnPaSt is a novel method for identification of differentially expressed biclusters in gene expression matrix. It searches for gene sets up- or down-regulated in subsets of samples:\n\n![alt text](https://github.com/ozolotareva/DESMOND2/blob/a26d8d7b2075d47a4edc8fc9ce7eca72a2dac7db/poster/DESMOND2_steps2.png?raw=true)\n\n\nWebserver: https://unpast.zbh.uni-hamburg.de/\n\n## Installation\nThis UnPaSt can be installed using `pip./poster/DESMOND2.png`, `poetry`, run using `Docker`, or as a script (see examples section). Follow the appropriate instructions below for your preferred method.\nYou need to have R (for WGCNA, it is suggested to use v.1.70-3) and **Python 3.8-3.10** installed. The main reason why Python 3.11 is not supported is because Scikit-network does not support it now.\n\n**Using different Python versions, even with the same libraries versions, leads to slightly different computational results.**\n\n1. Using pip: \\\nTo install the project using `pip`, first make sure you have `pip` installed on your system. If you haven\'t installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/). \\\nOnce `pip` is installed, you can install the project by running the following command:\n```bash\npip install unpast\n```\nRun it:\n```bash\nrun_unpast -h\n```\n**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:\n```bash\npython -m unpast.install_r_dependencies\n\n# or you can install it directly\nR -e "install.packages(\'BiocManager\'); BiocManager::install(\'WGCNA\')"\n```\n2. Installation using Poetry: \\\nTo install the package using Poetry, first make sure you have Poetry installed, clone the repo and then run:\n```bash\npoetry add unpast\n```\nRun it:\n```bash\npoetry run run_unpast -h\n```\n**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:\n```bash\npoetry run python -m unpast.install_r_dependencies\n\n# or you can install it directly\nR -e "install.packages(\'BiocManager\'); BiocManager::install(\'WGCNA\')"\n```\n3. Running with Docker: \\\nYou can also run the package using Docker. First, pull the Docker image:\n```bash\ndocker pull freddsle/unpast:latest\n```\nNext, run the container:\n```bash\ndocker run -v /your/data/path/:/user_data/ freddsle/unpast:latest --exprs /user_data/exprs.tsv --out_dir /user_data/out_dir/\n```\n\n## Examples\n* UnPaSt requires a tab-separated file with standardized expressions of genes (or transcripts) in rows, and samples in columns. Gene and sample names must be unique. \n* A subset of 200 randomly chosen samples from TCGA-BRCA and UnPaSt output:\n[test data](https://unpast-backend.zbh.uni-hamburg.de/download_example)\n\n<pre>\n# running UnPaSt with default parameters and example data\npython ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename TCGA_200_results\n\n# with different binarization and clustering methods\npython ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename results --binarization ward --clustering WGCNA\n\n# help\npython ./unpast/run_unpast.py -h\n</pre>\n\n## Outputs\n* \\<basename\\>.bin=[GMM|Jenks],clust=[Louvain|WGCNA|DESMOND].biclusters.tsv - a .tsv table with found biclsuters, where \n    - avgSNR is average SNR over all genes in the biclusters\n    - columns "n_genes" and "n_samples" provide the numbers of genes and samples, respectively \n    - "gene","sample" contain gene and sample names respectively\n    - "gene_indexes" and  "sample_indexes" - 0-based gene and sample indexes in the input matrix.\n* binarized expressions, background distributions of SNR for each bicluster size and binarization statistics [if clustering is WGCNA,  or  \'--save_binary\' flag is added]\n* modules found by WGCNA [if clustering is WGCNA]\n\n# About \nUnPaSt is an unconstrained version of DESMOND method ([repository](https://github.com/ozolotareva/DESMOND), [publication](https://academic.oup.com/bioinformatics/article/37/12/1691/6039116?login=true))\n\nMajor modifications:\n * it does not require the network of gene interactions \n * UnPaSt clusters individual genes instead of gene pairs\n * uses Gaussian mixture models or Jenks method for binarization of individual gene expressions\n * SNR threshold is authomatically determined; it depends on bicluster size in samples and user-defined p-value cutoff\n \n## License\nFree for non-for-profit use. For commercial use please contact the developers. \n\n### Poster CDCS workshop\'22\n![./poster/DESMOND2_poster_v5.png](https://github.com/ozolotareva/DESMOND2/blob/a26d8d7b2075d47a4edc8fc9ce7eca72a2dac7db/poster/DESMOND2_poster_v5.png?raw=true)\n### Poster ISMB and MCCMB\'21\n![./poster/DESMOND2.pdf](https://github.com/ozolotareva/DESMOND2/blob/a26d8d7b2075d47a4edc8fc9ce7eca72a2dac7db/poster/DESMOND2.png?raw=true)\n',
     'author': 'Olga Zolotareva (ozolotareva)',
     'author_email': 'None',
     'maintainer': 'Olga Zolotareva (ozolotareva)',
     'maintainer_email': 'None',
     'url': 'https://github.com/ozolotareva/DESMOND2',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.9',
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `unpast-0.1.5/PKG-INFO` & `unpast-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: unpast
-Version: 0.1.5
+Version: 0.1.6
 Summary: A novel method for unsupervised patient stratification.
 Home-page: https://github.com/ozolotareva/DESMOND2
 License: GPL-3.0
 Author: Olga Zolotareva (ozolotareva)
 Maintainer: Olga Zolotareva (ozolotareva)
-Requires-Python: >=3.8,<3.9
+Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: fisher (==0.1.9)
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: fisher (==0.1.10)
 Requires-Dist: jenkspy (==0.2.0)
+Requires-Dist: kneed (>=0.8.3,<0.9.0)
 Requires-Dist: matplotlib-venn (==0.11.6)
-Requires-Dist: numba (>=0.51.2)
+Requires-Dist: numba (==0.55.2)
 Requires-Dist: numpy (==1.22.3)
 Requires-Dist: pandas (==1.4.2)
 Requires-Dist: python-louvain (==0.15)
-Requires-Dist: scikit-learn (==0.23.1)
-Requires-Dist: scikit-network (==0.24.0)
-Requires-Dist: scipy (==1.7.1)
+Requires-Dist: scikit-learn (==1.1.0)
+Requires-Dist: scikit-network (==0.25.0)
+Requires-Dist: scipy (==1.7.3)
 Requires-Dist: statsmodels (==0.13.2)
 Project-URL: Repository, https://github.com/ozolotareva/DESMOND2
 Description-Content-Type: text/markdown
 
 # UnPaSt
 
 UnPaSt is a novel method for identification of differentially expressed biclusters in gene expression matrix. It searches for gene sets up- or down-regulated in subsets of samples:
@@ -31,42 +34,50 @@
 ![alt text](https://github.com/ozolotareva/DESMOND2/blob/a26d8d7b2075d47a4edc8fc9ce7eca72a2dac7db/poster/DESMOND2_steps2.png?raw=true)
 
 
 Webserver: https://unpast.zbh.uni-hamburg.de/
 
 ## Installation
 This UnPaSt can be installed using `pip./poster/DESMOND2.png`, `poetry`, run using `Docker`, or as a script (see examples section). Follow the appropriate instructions below for your preferred method.
-You need to have R and Python 3.8 installed.
+You need to have R (for WGCNA, it is suggested to use v.1.70-3) and **Python 3.8-3.10** installed. The main reason why Python 3.11 is not supported is because Scikit-network does not support it now.
+
+**Using different Python versions, even with the same libraries versions, leads to slightly different computational results.**
 
 1. Using pip: \
 To install the project using `pip`, first make sure you have `pip` installed on your system. If you haven't installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/). \
 Once `pip` is installed, you can install the project by running the following command:
 ```bash
 pip install unpast
 ```
 Run it:
 ```bash
 run_unpast -h
 ```
 **Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
 ```bash
 python -m unpast.install_r_dependencies
+
+# or you can install it directly
+R -e "install.packages('BiocManager'); BiocManager::install('WGCNA')"
 ```
 2. Installation using Poetry: \
 To install the package using Poetry, first make sure you have Poetry installed, clone the repo and then run:
 ```bash
 poetry add unpast
 ```
 Run it:
 ```bash
 poetry run run_unpast -h
 ```
 **Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
 ```bash
 poetry run python -m unpast.install_r_dependencies
+
+# or you can install it directly
+R -e "install.packages('BiocManager'); BiocManager::install('WGCNA')"
 ```
 3. Running with Docker: \
 You can also run the package using Docker. First, pull the Docker image:
 ```bash
 docker pull freddsle/unpast:latest
 ```
 Next, run the container:
```

