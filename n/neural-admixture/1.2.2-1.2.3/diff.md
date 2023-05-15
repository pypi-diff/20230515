# Comparing `tmp/neural-admixture-1.2.2.tar.gz` & `tmp/neural-admixture-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-admixture-1.2.2.tar", last modified: Tue Dec 13 15:24:59 2022, max compression
+gzip compressed data, was "neural-admixture-1.2.3.tar", last modified: Mon May 15 20:50:27 2023, max compression
```

## Comparing `neural-admixture-1.2.2.tar` & `neural-admixture-1.2.3.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.919197 neural-admixture-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.919197 neural-admixture-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.919197 neural-admixture-1.2.2/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.919197 neural-admixture-1.2.2/demo/data/
--rw-r--r--   0 runner    (1001) docker     (123)   228180 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/data/demo_data.bed
--rw-r--r--   0 runner    (1001) docker     (123)   244365 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/data/demo_data.bim
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/data/demo_data.fam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/demo/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)  1478925 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/outputs/demo_run.7.P.expected
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/outputs/demo_run.7.Q.expected
--rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/run_demo.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/demo/run_diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture/model/__test__/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/__test__/test_initializations.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/__test__/test_switchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/initializations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/neural_admixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/model/switchers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/snp_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12402 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/neural_admixture/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/neural_admixture.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-13 15:24:59.000000 neural-admixture-1.2.2/neural_admixture.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2022-12-13 15:24:59.923197 neural-admixture-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-13 15:24:52.000000 neural-admixture-1.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.338622 neural-admixture-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.338622 neural-admixture-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.338622 neural-admixture-1.2.3/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/demo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.338622 neural-admixture-1.2.3/demo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   228180 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/demo/data/demo_data.bed
+-rw-r--r--   0 runner    (1001) docker     (123)   244365 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/demo/data/demo_data.bim
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/demo/data/demo_data.fam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/demo/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1478925 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/demo/outputs/demo_run.7.P.expected
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/demo/outputs/demo_run.7.Q.expected
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/demo/run_demo.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/demo/run_diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/neural_admixture/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 20:50:27.000000 neural-admixture-1.2.3/neural_admixture/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/neural_admixture/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/neural_admixture/model/__test__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/model/__test__/test_initializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/model/__test__/test_switchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/model/initializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/model/neural_admixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/model/switchers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/neural_admixture/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/src/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/src/snp_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/src/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/neural_admixture/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/neural_admixture.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-05-15 20:50:27.000000 neural-admixture-1.2.3/neural_admixture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 20:50:27.000000 neural-admixture-1.2.3/neural_admixture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:50:27.000000 neural-admixture-1.2.3/neural_admixture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 20:50:27.000000 neural-admixture-1.2.3/neural_admixture.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 20:50:27.000000 neural-admixture-1.2.3/neural_admixture.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 20:50:27.000000 neural-admixture-1.2.3/neural_admixture.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-15 20:50:27.342622 neural-admixture-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-15 20:50:19.000000 neural-admixture-1.2.3/tox.ini
```

### Comparing `neural-admixture-1.2.2/.github/workflows/release.yml` & `neural-admixture-1.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/.gitignore` & `neural-admixture-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/PKG-INFO` & `neural-admixture-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-admixture
-Version: 1.2.2
+Version: 1.2.3
 Summary: Rapid population clustering with autoencoders
 Home-page: https://github.com/AI-sandbox/neural-admixture
 Author: Albert Dominguez Mantes
 Author-email: albert.dominguezmantes@epfl.ch
 License: CC BY-NC 4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neural-admixture-1.2.2/README.md` & `neural-admixture-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/demo/README.md` & `neural-admixture-1.2.3/demo/README.md`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/demo/data/demo_data.bed` & `neural-admixture-1.2.3/demo/data/demo_data.bed`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/demo/data/demo_data.bim` & `neural-admixture-1.2.3/demo/data/demo_data.bim`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/demo/data/demo_data.fam` & `neural-admixture-1.2.3/demo/data/demo_data.fam`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/demo/outputs/demo_run.7.P.expected` & `neural-admixture-1.2.3/demo/outputs/demo_run.7.P.expected`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/demo/outputs/demo_run.7.Q.expected` & `neural-admixture-1.2.3/demo/outputs/demo_run.7.Q.expected`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/demo/run_diagnostics.py` & `neural-admixture-1.2.3/demo/run_diagnostics.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/entry.py` & `neural-admixture-1.2.3/neural_admixture/entry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from importlib.metadata import version
 import logging
 import sys
+from ._version import __version__
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 log = logging.getLogger(__name__)
 
 def main():
-    nadm_version = version("neural-admixture")
-    log.info(f"Neural ADMIXTURE - Version {nadm_version}")
+    # nadm_version = version("neural-admixture")
+    log.info(f"Neural ADMIXTURE - Version {__version__}")
     arg_list = tuple(sys.argv)
     assert len(arg_list) > 1, 'Please provide either the argument "train" or "infer" to choose running mode.'
     if sys.argv[1] == 'train':
         from .src import train
         sys.exit(train.main(arg_list[2:]))
     if sys.argv[1] == 'infer':
         from .src import inference
```

### Comparing `neural-admixture-1.2.2/neural_admixture/model/__test__/test_initializations.py` & `neural-admixture-1.2.3/neural_admixture/model/__test__/test_initializations.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/model/__test__/test_switchers.py` & `neural-admixture-1.2.3/neural_admixture/model/__test__/test_switchers.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/model/initializations.py` & `neural-admixture-1.2.3/neural_admixture/model/initializations.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/model/modules.py` & `neural-admixture-1.2.3/neural_admixture/model/modules.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/model/neural_admixture.py` & `neural-admixture-1.2.3/neural_admixture/model/neural_admixture.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/model/switchers.py` & `neural-admixture-1.2.3/neural_admixture/model/switchers.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/src/inference.py` & `neural-admixture-1.2.3/neural_admixture/src/inference.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/src/snp_reader.py` & `neural-admixture-1.2.3/neural_admixture/src/snp_reader.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/src/train.py` & `neural-admixture-1.2.3/neural_admixture/src/train.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture/src/utils.py` & `neural-admixture-1.2.3/neural_admixture/src/utils.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.2/neural_admixture.egg-info/PKG-INFO` & `neural-admixture-1.2.3/neural_admixture.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-admixture
-Version: 1.2.2
+Version: 1.2.3
 Summary: Rapid population clustering with autoencoders
 Home-page: https://github.com/AI-sandbox/neural-admixture
 Author: Albert Dominguez Mantes
 Author-email: albert.dominguezmantes@epfl.ch
 License: CC BY-NC 4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neural-admixture-1.2.2/neural_admixture.egg-info/SOURCES.txt` & `neural-admixture-1.2.3/neural_admixture.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 demo/run_diagnostics.py
 demo/data/demo_data.bed
 demo/data/demo_data.bim
 demo/data/demo_data.fam
 demo/outputs/demo_run.7.P.expected
 demo/outputs/demo_run.7.Q.expected
 neural_admixture/__init__.py
+neural_admixture/_version.py
 neural_admixture/entry.py
 neural_admixture.egg-info/PKG-INFO
 neural_admixture.egg-info/SOURCES.txt
 neural_admixture.egg-info/dependency_links.txt
 neural_admixture.egg-info/entry_points.txt
 neural_admixture.egg-info/requires.txt
 neural_admixture.egg-info/top_level.txt
```

### Comparing `neural-admixture-1.2.2/setup.cfg` & `neural-admixture-1.2.3/setup.cfg`

 * *Files identical despite different names*

