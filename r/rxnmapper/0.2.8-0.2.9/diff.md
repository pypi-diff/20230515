# Comparing `tmp/rxnmapper-0.2.8.tar.gz` & `tmp/rxnmapper-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxnmapper-0.2.8.tar", last modified: Tue Apr 25 09:28:23 2023, max compression
+gzip compressed data, was "rxnmapper-0.2.9.tar", last modified: Mon May 15 14:25:13 2023, max compression
```

## Comparing `rxnmapper-0.2.8.tar` & `rxnmapper-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.943157 rxnmapper-0.2.8/rxnmapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/batched_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.939157 rxnmapper-0.2.8/rxnmapper/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.939157 rxnmapper-0.2.8/rxnmapper/models/transformers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/config.json
--rw-r--r--   0 runner    (1001) docker     (123)  3212952 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/training_args.bin
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/vocab.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/smiles_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/rxnmapper/tokenization_smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.943157 rxnmapper-0.2.8/rxnmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 09:28:23.000000 rxnmapper-0.2.8/rxnmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:23.947157 rxnmapper-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/test_batched_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/test_smiles_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-25 09:28:13.000000 rxnmapper-0.2.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:13.789239 rxnmapper-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-15 14:25:13.789239 rxnmapper-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:13.781239 rxnmapper-0.2.9/rxnmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/batched_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:13.777239 rxnmapper-0.2.9/rxnmapper/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:13.777239 rxnmapper-0.2.9/rxnmapper/models/transformers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:13.789239 rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3212952 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/training_args.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/smiles_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/rxnmapper/tokenization_smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:13.781239 rxnmapper-0.2.9/rxnmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-15 14:25:13.000000 rxnmapper-0.2.9/rxnmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-15 14:25:13.000000 rxnmapper-0.2.9/rxnmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:25:13.000000 rxnmapper-0.2.9/rxnmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:25:13.000000 rxnmapper-0.2.9/rxnmapper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-15 14:25:13.000000 rxnmapper-0.2.9/rxnmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 14:25:13.000000 rxnmapper-0.2.9/rxnmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-15 14:25:13.789239 rxnmapper-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:13.789239 rxnmapper-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/tests/test_batched_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/tests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/tests/test_smiles_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-15 14:25:01.000000 rxnmapper-0.2.9/tests/utils.py
```

### Comparing `rxnmapper-0.2.8/LICENSE` & `rxnmapper-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/PKG-INFO` & `rxnmapper-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxnmapper
-Version: 0.2.8
+Version: 0.2.9
 Summary: Reaction atom-mapping from transfomers
 Home-page: https://github.com/rxn4chemistry/rxnmapper
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `rxnmapper-0.2.8/README.md` & `rxnmapper-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/attention.py` & `rxnmapper-0.2.9/rxnmapper/attention.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/batched_mapper.py` & `rxnmapper-0.2.9/rxnmapper/batched_mapper.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/core.py` & `rxnmapper-0.2.9/rxnmapper/core.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/config.json` & `rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/config.json`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/pytorch_model.bin` & `rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/training_args.bin` & `rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/training_args.bin`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/vocab.txt` & `rxnmapper-0.2.9/rxnmapper/models/transformers/albert_heads_8_uspto_all_1310k/vocab.txt`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/smiles_utils.py` & `rxnmapper-0.2.9/rxnmapper/smiles_utils.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper/tokenization_smiles.py` & `rxnmapper-0.2.9/rxnmapper/tokenization_smiles.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/rxnmapper.egg-info/PKG-INFO` & `rxnmapper-0.2.9/rxnmapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxnmapper
-Version: 0.2.8
+Version: 0.2.9
 Summary: Reaction atom-mapping from transfomers
 Home-page: https://github.com/rxn4chemistry/rxnmapper
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `rxnmapper-0.2.8/rxnmapper.egg-info/SOURCES.txt` & `rxnmapper-0.2.9/rxnmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/setup.cfg` & `rxnmapper-0.2.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 zip_safe = False
 include_package_data = True
 install_requires = 
 	pandas>=1.0.3
 	rxn-chem-utils>=1.0.3
 	scipy>=1.4.1
 	torch>=1.5.0,<2.1
-	transformers>=4.0.0,<4.9.0
+	transformers>=4.0.0
 
 [options.package_data]
 rxnmapper = 
 	models/transformers/albert_heads_8_uspto_all_1310k/*
 	py.typed
 
 [options.extras_require]
```

### Comparing `rxnmapper-0.2.8/tests/test_batched_mapper.py` & `rxnmapper-0.2.9/tests/test_batched_mapper.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/tests/test_mapper.py` & `rxnmapper-0.2.9/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/tests/test_smiles_utils.py` & `rxnmapper-0.2.9/tests/test_smiles_utils.py`

 * *Files identical despite different names*

### Comparing `rxnmapper-0.2.8/tests/utils.py` & `rxnmapper-0.2.9/tests/utils.py`

 * *Files identical despite different names*

