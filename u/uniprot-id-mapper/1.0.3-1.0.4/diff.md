# Comparing `tmp/uniprot-id-mapper-1.0.3.tar.gz` & `tmp/uniprot-id-mapper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniprot-id-mapper-1.0.3.tar", last modified: Fri Apr 21 11:10:50 2023, max compression
+gzip compressed data, was "uniprot-id-mapper-1.0.4.tar", last modified: Mon May 15 09:52:29 2023, max compression
```

## Comparing `uniprot-id-mapper-1.0.3.tar` & `uniprot-id-mapper-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1070 2023-02-28 11:23:59.000000 uniprot-id-mapper-1.0.3/LICENSE
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       86 2023-03-17 12:50:04.000000 uniprot-id-mapper-1.0.3/MANIFEST.in
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10089 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/PKG-INFO
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     7893 2023-04-21 11:09:52.000000 uniprot-id-mapper-1.0.3/README.md
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1650 2023-04-21 11:07:13.000000 uniprot-id-mapper-1.0.3/pyproject.toml
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       38 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/setup.cfg
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.517283 uniprot-id-mapper-1.0.3/src/
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/src/UniProtMapper/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      315 2023-03-17 13:30:05.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/__init__.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9230 2023-04-21 10:00:21.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/field_retriever_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10510 2023-04-21 11:02:17.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/id_mapping_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     5134 2023-04-19 17:23:14.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/interface.py
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)   105497 2023-03-01 13:45:43.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2752 2023-03-14 14:33:07.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_mapping_dbs.json
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    18362 2023-04-19 15:52:45.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_return_fields.csv
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9328 2023-04-21 10:01:31.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/swiss_parser.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     4258 2023-04-21 10:03:15.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/utils.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       92 2023-04-21 11:06:59.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/version.py
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10089 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/PKG-INFO
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      744 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)        1 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       50 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/requires.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       14 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/tests/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2256 2023-04-19 17:44:47.000000 uniprot-id-mapper-1.0.3/tests/test_field_retriever_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2955 2023-04-19 18:49:12.000000 uniprot-id-mapper-1.0.3/tests/test_id_mapping_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1862 2023-04-19 17:45:00.000000 uniprot-id-mapper-1.0.3/tests/test_utils.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-05-15 09:52:29.866802 uniprot-id-mapper-1.0.4/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1070 2023-02-28 11:23:59.000000 uniprot-id-mapper-1.0.4/LICENSE
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       86 2023-03-17 12:50:04.000000 uniprot-id-mapper-1.0.4/MANIFEST.in
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10223 2023-05-15 09:52:29.866802 uniprot-id-mapper-1.0.4/PKG-INFO
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     8027 2023-05-15 09:49:14.000000 uniprot-id-mapper-1.0.4/README.md
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1728 2023-05-15 09:44:19.000000 uniprot-id-mapper-1.0.4/pyproject.toml
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       38 2023-05-15 09:52:29.866802 uniprot-id-mapper-1.0.4/setup.cfg
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-05-15 09:52:29.855969 uniprot-id-mapper-1.0.4/src/
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-05-15 09:52:29.866802 uniprot-id-mapper-1.0.4/src/UniProtMapper/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      338 2023-05-15 09:50:13.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/__init__.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9230 2023-04-21 10:00:21.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/field_retriever_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10510 2023-04-21 11:02:17.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/id_mapping_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     5134 2023-04-19 17:23:14.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/interface.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-05-15 09:52:29.866802 uniprot-id-mapper-1.0.4/src/UniProtMapper/resources/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)   105497 2023-03-01 13:45:43.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2752 2023-03-14 14:33:07.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/resources/uniprot_mapping_dbs.json
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    18362 2023-04-19 15:52:45.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/resources/uniprot_return_fields.csv
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9328 2023-04-21 10:01:31.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/swiss_parser.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     4258 2023-04-21 10:03:15.000000 uniprot-id-mapper-1.0.4/src/UniProtMapper/utils.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-05-15 09:52:29.866802 uniprot-id-mapper-1.0.4/src/uniprot_id_mapper.egg-info/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10223 2023-05-15 09:52:29.000000 uniprot-id-mapper-1.0.4/src/uniprot_id_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      715 2023-05-15 09:52:29.000000 uniprot-id-mapper-1.0.4/src/uniprot_id_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)        1 2023-05-15 09:52:29.000000 uniprot-id-mapper-1.0.4/src/uniprot_id_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       50 2023-05-15 09:52:29.000000 uniprot-id-mapper-1.0.4/src/uniprot_id_mapper.egg-info/requires.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       14 2023-05-15 09:52:29.000000 uniprot-id-mapper-1.0.4/src/uniprot_id_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-05-15 09:52:29.866802 uniprot-id-mapper-1.0.4/tests/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2256 2023-04-19 17:44:47.000000 uniprot-id-mapper-1.0.4/tests/test_field_retriever_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2955 2023-04-19 18:49:12.000000 uniprot-id-mapper-1.0.4/tests/test_id_mapping_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1862 2023-04-19 17:45:00.000000 uniprot-id-mapper-1.0.4/tests/test_utils.py
```

### Comparing `uniprot-id-mapper-1.0.3/LICENSE` & `uniprot-id-mapper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/PKG-INFO` & `uniprot-id-mapper-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniprot-id-mapper
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python wrapper for the UniProt Mapping RESTful API.
 Author-email: David Araripe <david.araripe17@gmail.com>
 Maintainer-email: David Araripe <david.araripe17@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 David Araripe
         
@@ -57,22 +57,27 @@
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
 - Parse json UniProt-SwissProt responses (handled by [SwissProtParser](#swissprotparser)).
 
 ## Installation
 
 From PyPI:
 ``` Shell
-pip install uniprot-id-mapper
+python -m pip install uniprot-id-mapper
+```
+
+Directly from GitHub:
+``` Shell
+python -m pip install git+https://github.com/David-Araripe/UniProtMapper.git
 ```
 
 From source:
 ``` Shell
 git clone https://github.com/David-Araripe/UniProtMapper
 cd UniProtMapper
-pip install .
+python -m pip install .
 ```
 ## Usage
 
 <summary>
 
 ## UniProtIDMapper
```

### Comparing `uniprot-id-mapper-1.0.3/README.md` & `uniprot-id-mapper-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
 - Parse json UniProt-SwissProt responses (handled by [SwissProtParser](#swissprotparser)).
 
 ## Installation
 
 From PyPI:
 ``` Shell
-pip install uniprot-id-mapper
+python -m pip install uniprot-id-mapper
+```
+
+Directly from GitHub:
+``` Shell
+python -m pip install git+https://github.com/David-Araripe/UniProtMapper.git
 ```
 
 From source:
 ``` Shell
 git clone https://github.com/David-Araripe/UniProtMapper
 cd UniProtMapper
-pip install .
+python -m pip install .
 ```
 ## Usage
 
 <summary>
 
 ## UniProtIDMapper
```

### Comparing `uniprot-id-mapper-1.0.3/pyproject.toml` & `uniprot-id-mapper-1.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uniprot-id-mapper"
-version = "1.0.3"
+dynamic = ["version"]
 description = "A Python wrapper for the UniProt Mapping RESTful API."
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["uniprot", "database", "protein ID", "gene ID", "parser"]
 authors = [{ name = "David Araripe", email = "david.araripe17@gmail.com" }]
 maintainers = [{ name = "David Araripe", email = "david.araripe17@gmail.com" }]
@@ -32,14 +32,17 @@
 homepage = "https://github.com/David-Araripe/UniProtMapper"
 repository = "https://github.com/David-Araripe/UniProtMapper"
 # documentation = "https://readthedocs.org" TODO
 
 [tool.setuptools]
 include-package-data = true
 
+[tool.setuptools.dynamic]
+version = {attr = "UniProtMapper.__version__"}
+
 [tool.ruff]
 line-length = 88
 update-check = false
 target-version = "py38"
 fix = true
 
 [tool.isort]
```

### Comparing `uniprot-id-mapper-1.0.3/src/UniProtMapper/field_retriever_api.py` & `uniprot-id-mapper-1.0.4/src/UniProtMapper/field_retriever_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/src/UniProtMapper/id_mapping_api.py` & `uniprot-id-mapper-1.0.4/src/UniProtMapper/id_mapping_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/src/UniProtMapper/interface.py` & `uniprot-id-mapper-1.0.4/src/UniProtMapper/interface.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json` & `uniprot-id-mapper-1.0.4/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_mapping_dbs.json` & `uniprot-id-mapper-1.0.4/src/UniProtMapper/resources/uniprot_mapping_dbs.json`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_return_fields.csv` & `uniprot-id-mapper-1.0.4/src/UniProtMapper/resources/uniprot_return_fields.csv`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/src/UniProtMapper/swiss_parser.py` & `uniprot-id-mapper-1.0.4/src/UniProtMapper/swiss_parser.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/src/UniProtMapper/utils.py` & `uniprot-id-mapper-1.0.4/src/UniProtMapper/utils.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/PKG-INFO` & `uniprot-id-mapper-1.0.4/src/uniprot_id_mapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniprot-id-mapper
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python wrapper for the UniProt Mapping RESTful API.
 Author-email: David Araripe <david.araripe17@gmail.com>
 Maintainer-email: David Araripe <david.araripe17@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 David Araripe
         
@@ -57,22 +57,27 @@
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
 - Parse json UniProt-SwissProt responses (handled by [SwissProtParser](#swissprotparser)).
 
 ## Installation
 
 From PyPI:
 ``` Shell
-pip install uniprot-id-mapper
+python -m pip install uniprot-id-mapper
+```
+
+Directly from GitHub:
+``` Shell
+python -m pip install git+https://github.com/David-Araripe/UniProtMapper.git
 ```
 
 From source:
 ``` Shell
 git clone https://github.com/David-Araripe/UniProtMapper
 cd UniProtMapper
-pip install .
+python -m pip install .
 ```
 ## Usage
 
 <summary>
 
 ## UniProtIDMapper
```

### Comparing `uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/SOURCES.txt` & `uniprot-id-mapper-1.0.4/src/uniprot_id_mapper.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 pyproject.toml
 src/UniProtMapper/__init__.py
 src/UniProtMapper/field_retriever_api.py
 src/UniProtMapper/id_mapping_api.py
 src/UniProtMapper/interface.py
 src/UniProtMapper/swiss_parser.py
 src/UniProtMapper/utils.py
-src/UniProtMapper/version.py
 src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json
 src/UniProtMapper/resources/uniprot_mapping_dbs.json
 src/UniProtMapper/resources/uniprot_return_fields.csv
 src/uniprot_id_mapper.egg-info/PKG-INFO
 src/uniprot_id_mapper.egg-info/SOURCES.txt
 src/uniprot_id_mapper.egg-info/dependency_links.txt
 src/uniprot_id_mapper.egg-info/requires.txt
```

### Comparing `uniprot-id-mapper-1.0.3/tests/test_field_retriever_api.py` & `uniprot-id-mapper-1.0.4/tests/test_field_retriever_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/tests/test_id_mapping_api.py` & `uniprot-id-mapper-1.0.4/tests/test_id_mapping_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.3/tests/test_utils.py` & `uniprot-id-mapper-1.0.4/tests/test_utils.py`

 * *Files identical despite different names*

