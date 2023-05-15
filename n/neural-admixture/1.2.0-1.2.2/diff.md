# Comparing `tmp/neural-admixture-1.2.0.tar.gz` & `tmp/neural-admixture-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-admixture-1.2.0.tar", last modified: Fri Oct 14 14:46:48 2022, max compression
+gzip compressed data, was "neural-admixture-1.2.2.tar", last modified: Tue Dec 13 15:24:59 2022, max compression
```

## Comparing `neural-admixture-1.2.0.tar` & `neural-admixture-1.2.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.375272 neural-admixture-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.371272 neural-admixture-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.371272 neural-admixture-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-14 14:46:48.375272 neural-admixture-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14661 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.371272 neural-admixture-1.2.0/demo/
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.371272 neural-admixture-1.2.0/demo/data/
--rw-r--r--   0 runner    (1001) docker     (121)   228180 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/demo/data/demo_data.bed
--rw-r--r--   0 runner    (1001) docker     (121)   244365 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/demo/data/demo_data.bim
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/demo/data/demo_data.fam
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.371272 neural-admixture-1.2.0/demo/outputs/
--rw-r--r--   0 runner    (1001) docker     (121)  1478925 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/demo/outputs/demo_run.7.P.expected
--rw-r--r--   0 runner    (1001) docker     (121)    18375 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/demo/outputs/demo_run.7.Q.expected
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/demo/run_demo.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/demo/run_diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.371272 neural-admixture-1.2.0/neural_admixture/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.375272 neural-admixture-1.2.0/neural_admixture/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.375272 neural-admixture-1.2.0/neural_admixture/model/__test__/
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/model/__test__/test_initializations.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/model/__test__/test_switchers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8718 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/model/initializations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/model/modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     9787 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/model/neural_admixture.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/model/switchers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.375272 neural-admixture-1.2.0/neural_admixture/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/src/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/src/snp_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     5757 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/src/train.py
--rw-r--r--   0 runner    (1001) docker     (121)    12402 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/neural_admixture/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 14:46:48.375272 neural-admixture-1.2.0/neural_admixture.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-14 14:46:48.000000 neural-admixture-1.2.0/neural_admixture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-10-14 14:46:48.000000 neural-admixture-1.2.0/neural_admixture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 14:46:48.000000 neural-admixture-1.2.0/neural_admixture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-14 14:46:48.000000 neural-admixture-1.2.0/neural_admixture.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-14 14:46:48.000000 neural-admixture-1.2.0/neural_admixture.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-14 14:46:48.000000 neural-admixture-1.2.0/neural_admixture.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-10-14 14:46:48.375272 neural-admixture-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-10-14 14:46:40.000000 neural-admixture-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.919197 neural-admixture-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.919197 neural-admixture-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.919197 neural-admixture-1.2.2/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.919197 neural-admixture-1.2.2/demo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   228180 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/data/demo_data.bed
+-rw-r--r--   0 runner    (1001) docker     (123)   244365 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/data/demo_data.bim
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/data/demo_data.fam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/demo/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1478925 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/outputs/demo_run.7.P.expected
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/outputs/demo_run.7.Q.expected
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/run_demo.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/run_diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture/model/__test__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/__test__/test_initializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/__test__/test_switchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/initializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/neural_admixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/switchers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/snp_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/tox.ini
```

### Comparing `neural-admixture-1.2.0/.github/workflows/release.yml` & `neural-admixture-1.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/.gitignore` & `neural-admixture-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/README.md` & `neural-admixture-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neural-admixture)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neural-admixture.svg)
 ![PyPI - Version](https://img.shields.io/pypi/v/neural-admixture)
 ![PyPI - License](https://img.shields.io/pypi/l/neural-admixture)
 ![PyPI - Status](https://img.shields.io/pypi/status/neural-admixture)
 [![tests](https://github.com/AI-sandbox/neural-admixture/workflows/tests/badge.svg)](https://github.com/AI-sandbox/neural-admixture/actions)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/neural-admixture)
+[![DOI:10.1101/2021.06.27.450081](http://img.shields.io/badge/DOI-10.1101/2021.06.27.450081-B31B1B.svg)](https://doi.org/10.1101/2021.06.27.450081)
 
 # Neural ADMIXTURE
 
 ![nadm_mna](https://user-images.githubusercontent.com/31998088/154133905-59ee5fae-243d-4df3-ae18-81563c51c0c8.png)
 
 
 Neural ADMIXTURE is an unsupervised global ancestry inference technique based on ADMIXTURE. By using neural networks, Neural ADMIXTURE offers high quality ancestry assignments with a running time which is much faster than ADMIXTURE's. For more information, we recommend reading [the corresponding article](https://www.biorxiv.org/content/10.1101/2021.06.27.450081).
```

### Comparing `neural-admixture-1.2.0/demo/README.md` & `neural-admixture-1.2.2/demo/README.md`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/demo/data/demo_data.bed` & `neural-admixture-1.2.2/demo/data/demo_data.bed`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/demo/data/demo_data.bim` & `neural-admixture-1.2.2/demo/data/demo_data.bim`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/demo/data/demo_data.fam` & `neural-admixture-1.2.2/demo/data/demo_data.fam`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/demo/outputs/demo_run.7.P.expected` & `neural-admixture-1.2.2/demo/outputs/demo_run.7.P.expected`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/demo/outputs/demo_run.7.Q.expected` & `neural-admixture-1.2.2/demo/outputs/demo_run.7.Q.expected`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/demo/run_diagnostics.py` & `neural-admixture-1.2.2/demo/run_diagnostics.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/entry.py` & `neural-admixture-1.2.2/neural_admixture/entry.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/model/__test__/test_initializations.py` & `neural-admixture-1.2.2/neural_admixture/model/__test__/test_initializations.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/model/__test__/test_switchers.py` & `neural-admixture-1.2.2/neural_admixture/model/__test__/test_switchers.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/model/initializations.py` & `neural-admixture-1.2.2/neural_admixture/model/initializations.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/model/modules.py` & `neural-admixture-1.2.2/neural_admixture/model/modules.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/model/neural_admixture.py` & `neural-admixture-1.2.2/neural_admixture/model/neural_admixture.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/model/switchers.py` & `neural-admixture-1.2.2/neural_admixture/model/switchers.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/src/inference.py` & `neural-admixture-1.2.2/neural_admixture/src/inference.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture/src/snp_reader.py` & `neural-admixture-1.2.2/neural_admixture/src/snp_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,24 +110,24 @@
 
         Args:
             file (str): path to file
 
         Returns:
             da.core.Array: averaged genotype Dask array of shape (n_samples, n_snps)
         """
-        file_extension = "".join(Path(file).suffixes)
-        if file_extension == '.vcf' or file_extension == '.vcf.gz':
+        file_extensions = Path(file).suffixes
+        if '.vcf' in file_extensions:
             G = self._read_vcf(file)
-        elif file_extension == '.h5' or file_extension == '.hdf5':
+        elif '.h5' in file_extensions or '.hdf5' in file_extensions:
             G = self._read_hdf5(file)
-        elif file_extension == '.bed':
+        elif '.bed' in file_extensions:
             G = self._read_bed(file)
-        elif file_extension == '.pgen':
+        elif '.pgen' in file_extensions:
             G = self._read_pgen(file)
-        elif file_extension == '.npy':
+        elif '.npy' in file_extensions:
             G = self._read_npy(file)
         else:
             log.error('Invalid format. Unrecognized file format. Make sure file ends with .vcf | .vcf.gz | .bed | .pgen | .h5 | .hdf5 | .npy')
             sys.exit(1)
         assert int(G.min()) == 0 and int(G.max()) == 1, 'Only biallelic SNPs are supported. Please make sure multiallelic sites have been removed.'
         G_corr = G if np.mean(G) < 0.5 else 1-G
         return G_corr if isinstance(G_corr, da.core.Array) else da.from_array(G_corr)
```

### Comparing `neural-admixture-1.2.0/neural_admixture/src/train.py` & `neural-admixture-1.2.2/neural_admixture/src/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 def main(argv: List[str]):
     """Training entry point
     """
     args = utils.parse_train_args(argv)
     tr_file, val_file = args.data_path, args.validation_data_path
     tr_pops_f, val_pops_f = args.populations_path, args.validation_populations_path
     trX, trY, valX, valY = utils.read_data(tr_file, val_file, tr_pops_f, val_pops_f)
-    print(type(trX))
     model, device = fit_model(trX, args, valX, trY, valY)
     log.info('Computing divergences...')
     model.display_divergences()
     log.info('Writing outputs...')
     utils.write_outputs(model, trX, valX, args.batch_size, device, args.name, args.save_dir)
     log.info('Exiting...')
     logging.shutdown()
```

### Comparing `neural-admixture-1.2.0/neural_admixture/src/utils.py` & `neural-admixture-1.2.2/neural_admixture/src/utils.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/neural_admixture.egg-info/SOURCES.txt` & `neural-admixture-1.2.2/neural_admixture.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.0/setup.cfg` & `neural-admixture-1.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = neural-admixture
 author = Albert Dominguez Mantes
 author_email = albert.dominguezmantes@epfl.ch
 license = CC BY-NC 4.0
 description = Rapid population clustering with autoencoders
-long_description = file: README.rst
+long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AI-sandbox/neural-admixture
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 	Programming Language :: Python :: 3.8
@@ -28,15 +28,15 @@
 	h5py>=3.1.0
 	matplotlib>=3.3.4
 	numpy>=1.21.0
 	pandas>=1.2.4
 	pandas_plink>=2.2.9
 	py_pcha>=0.1.3
 	scikit-allel>=1.3.5
-	scikit-learn>=0.24.1
+	scikit-learn<=1.1.1
 	setuptools>=50.3.1
 	torch>=1.7.1
 	wandb>=0.12.17
 python_requires = >=3.8
 
 [options.entry_points]
 console_scripts =
```

