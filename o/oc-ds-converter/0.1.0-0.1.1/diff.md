# Comparing `tmp/oc_ds_converter-0.1.0.tar.gz` & `tmp/oc_ds_converter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_ds_converter-0.1.0.tar", max compression
+gzip compressed data, was "oc_ds_converter-0.1.1.tar", max compression
```

## Comparing `oc_ds_converter-0.1.0.tar` & `oc_ds_converter-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0        0 2023-05-15 13:12:58.853513 oc_ds_converter-0.1.0/oc_ds_converter/crossref/__init__.py
--rw-r--r--   0        0        0    10646 2023-05-15 13:12:58.853513 oc_ds_converter-0.1.0/oc_ds_converter/crossref/crossref_processing.py
--rw-r--r--   0        0        0     4337 2023-05-15 13:12:58.854513 oc_ds_converter-0.1.0/oc_ds_converter/crossref/extract_crossref_publishers.py
--rw-r--r--   0        0        0     9098 2023-05-15 13:12:58.854513 oc_ds_converter-0.1.0/oc_ds_converter/crossref/get_not_crossref_ref.py
--rw-r--r--   0        0        0        0 2023-05-15 13:12:58.854513 oc_ds_converter-0.1.0/oc_ds_converter/datacite/__init__.py
--rw-r--r--   0        0        0    22405 2023-05-15 13:12:58.854513 oc_ds_converter-0.1.0/oc_ds_converter/datacite/datacite_processing.py
--rw-r--r--   0        0        0        0 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.0/oc_ds_converter/datasource/__init__.py
--rw-r--r--   0        0        0      238 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.0/oc_ds_converter/datasource/config.ini
--rw-r--r--   0        0        0     1329 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.0/oc_ds_converter/datasource/datasource.py
--rw-r--r--   0        0        0     2701 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.0/oc_ds_converter/datasource/redis.py
--rw-r--r--   0        0        0        0 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.0/oc_ds_converter/jalc/__init__.py
--rw-r--r--   0        0        0     8124 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.0/oc_ds_converter/jalc/jalc_processing.py
--rw-r--r--   0        0        0     1025 2023-05-15 13:12:58.856517 oc_ds_converter-0.1.0/oc_ds_converter/lib/__init__.py
--rw-r--r--   0        0        0    17232 2023-05-15 13:12:58.856517 oc_ds_converter-0.1.0/oc_ds_converter/lib/cleaner.py
--rw-r--r--   0        0        0     6083 2023-05-15 13:12:58.856517 oc_ds_converter-0.1.0/oc_ds_converter/lib/csvmanager.py
--rw-r--r--   0        0        0     9573 2023-05-15 13:12:58.856517 oc_ds_converter-0.1.0/oc_ds_converter/lib/file_manager.py
--rw-r--r--   0        0        0     5836 2023-05-15 13:12:58.857517 oc_ds_converter-0.1.0/oc_ds_converter/lib/jsonmanager.py
--rw-r--r--   0        0        0     5260 2023-05-15 13:12:58.857517 oc_ds_converter-0.1.0/oc_ds_converter/lib/master_of_regex.py
--rw-r--r--   0        0        0        0 2023-05-15 13:12:58.857517 oc_ds_converter-0.1.0/oc_ds_converter/medra/__init__.py
--rw-r--r--   0        0        0    12400 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.0/oc_ds_converter/medra/medra_processing.py
--rw-r--r--   0        0        0     3779 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.0/oc_ds_converter/metadata_manager.py
--rw-r--r--   0        0        0        0 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.0/oc_ds_converter/preprocessing/__init__.py
--rw-r--r--   0        0        0     4315 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.0/oc_ds_converter/preprocessing/base.py
--rw-r--r--   0        0        0     6104 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.0/oc_ds_converter/preprocessing/datacite.py
--rw-r--r--   0        0        0     4827 2023-05-15 13:12:58.859520 oc_ds_converter-0.1.0/oc_ds_converter/preprocessing/nih.py
--rw-r--r--   0        0        0        0 2023-05-15 13:12:58.859520 oc_ds_converter-0.1.0/oc_ds_converter/pubmed/__init__.py
--rw-r--r--   0        0        0     4683 2023-05-15 13:12:58.859520 oc_ds_converter-0.1.0/oc_ds_converter/pubmed/finder_nih.py
--rw-r--r--   0        0        0     5893 2023-05-15 13:12:58.859520 oc_ds_converter-0.1.0/oc_ds_converter/pubmed/get_publishers.py
--rw-r--r--   0        0        0     2428 2023-05-15 13:12:58.860519 oc_ds_converter-0.1.0/oc_ds_converter/pubmed/pubmed_dump_explorer.py
--rw-r--r--   0        0        0    33743 2023-05-15 13:12:58.860519 oc_ds_converter-0.1.0/oc_ds_converter/pubmed/pubmed_processing.py
--rw-r--r--   0        0        0      503 2023-05-15 13:12:58.860519 oc_ds_converter-0.1.0/oc_ds_converter/pubmed/support_files/issn_jour_ext.json
--rw-r--r--   0        0        0   315988 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.0/oc_ds_converter/pubmed/support_files/prefix_publishers.json
--rw-r--r--   0        0        0    11894 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.0/oc_ds_converter/ra_processor.py
--rw-r--r--   0        0        0        0 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.0/oc_ds_converter/run/__init__.py
--rw-r--r--   0        0        0     6663 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.0/oc_ds_converter/run/crossref_process.py
--rw-r--r--   0        0        0     6657 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.0/oc_ds_converter/run/datacite_process.py
--rw-r--r--   0        0        0     7970 2023-05-15 13:12:58.863517 oc_ds_converter-0.1.0/oc_ds_converter/run/jalc_process.py
--rw-r--r--   0        0        0     9697 2023-05-15 13:12:58.863517 oc_ds_converter-0.1.0/oc_ds_converter/run/pubmed_process.py
--rw-r--r--   0        0        0      774 2023-05-15 13:12:58.864517 oc_ds_converter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      881 2023-05-15 13:12:58.853513 oc_ds_converter-0.1.0/README.md
--rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 oc_ds_converter-0.1.0/setup.py
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 oc_ds_converter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.1/oc_ds_converter/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.853513 oc_ds_converter-0.1.1/oc_ds_converter/crossref/__init__.py
+-rw-r--r--   0        0        0    10646 2023-05-15 13:12:58.853513 oc_ds_converter-0.1.1/oc_ds_converter/crossref/crossref_processing.py
+-rw-r--r--   0        0        0     4337 2023-05-15 13:12:58.854513 oc_ds_converter-0.1.1/oc_ds_converter/crossref/extract_crossref_publishers.py
+-rw-r--r--   0        0        0     9098 2023-05-15 13:12:58.854513 oc_ds_converter-0.1.1/oc_ds_converter/crossref/get_not_crossref_ref.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.854513 oc_ds_converter-0.1.1/oc_ds_converter/datacite/__init__.py
+-rw-r--r--   0        0        0    22405 2023-05-15 13:12:58.854513 oc_ds_converter-0.1.1/oc_ds_converter/datacite/datacite_processing.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.1/oc_ds_converter/datasource/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.1/oc_ds_converter/datasource/config.ini
+-rw-r--r--   0        0        0     1329 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.1/oc_ds_converter/datasource/datasource.py
+-rw-r--r--   0        0        0     2701 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.1/oc_ds_converter/datasource/redis.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.1/oc_ds_converter/jalc/__init__.py
+-rw-r--r--   0        0        0     8124 2023-05-15 13:12:58.855513 oc_ds_converter-0.1.1/oc_ds_converter/jalc/jalc_processing.py
+-rw-r--r--   0        0        0     1025 2023-05-15 13:12:58.856517 oc_ds_converter-0.1.1/oc_ds_converter/lib/__init__.py
+-rw-r--r--   0        0        0    17232 2023-05-15 13:12:58.856517 oc_ds_converter-0.1.1/oc_ds_converter/lib/cleaner.py
+-rw-r--r--   0        0        0     6083 2023-05-15 13:12:58.856517 oc_ds_converter-0.1.1/oc_ds_converter/lib/csvmanager.py
+-rw-r--r--   0        0        0     9573 2023-05-15 13:12:58.856517 oc_ds_converter-0.1.1/oc_ds_converter/lib/file_manager.py
+-rw-r--r--   0        0        0     5836 2023-05-15 13:12:58.857517 oc_ds_converter-0.1.1/oc_ds_converter/lib/jsonmanager.py
+-rw-r--r--   0        0        0     5260 2023-05-15 13:12:58.857517 oc_ds_converter-0.1.1/oc_ds_converter/lib/master_of_regex.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.857517 oc_ds_converter-0.1.1/oc_ds_converter/medra/__init__.py
+-rw-r--r--   0        0        0    12400 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.1/oc_ds_converter/medra/medra_processing.py
+-rw-r--r--   0        0        0     3779 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.1/oc_ds_converter/metadata_manager.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.1/oc_ds_converter/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4315 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.1/oc_ds_converter/preprocessing/base.py
+-rw-r--r--   0        0        0     6104 2023-05-15 13:12:58.858520 oc_ds_converter-0.1.1/oc_ds_converter/preprocessing/datacite.py
+-rw-r--r--   0        0        0     4827 2023-05-15 13:12:58.859520 oc_ds_converter-0.1.1/oc_ds_converter/preprocessing/nih.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.859520 oc_ds_converter-0.1.1/oc_ds_converter/pubmed/__init__.py
+-rw-r--r--   0        0        0     4683 2023-05-15 13:12:58.859520 oc_ds_converter-0.1.1/oc_ds_converter/pubmed/finder_nih.py
+-rw-r--r--   0        0        0     5893 2023-05-15 13:12:58.859520 oc_ds_converter-0.1.1/oc_ds_converter/pubmed/get_publishers.py
+-rw-r--r--   0        0        0     2428 2023-05-15 13:12:58.860519 oc_ds_converter-0.1.1/oc_ds_converter/pubmed/pubmed_dump_explorer.py
+-rw-r--r--   0        0        0    33743 2023-05-15 13:12:58.860519 oc_ds_converter-0.1.1/oc_ds_converter/pubmed/pubmed_processing.py
+-rw-r--r--   0        0        0      503 2023-05-15 13:12:58.860519 oc_ds_converter-0.1.1/oc_ds_converter/pubmed/support_files/issn_jour_ext.json
+-rw-r--r--   0        0        0   315988 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.1/oc_ds_converter/pubmed/support_files/prefix_publishers.json
+-rw-r--r--   0        0        0    11894 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.1/oc_ds_converter/ra_processor.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.1/oc_ds_converter/run/__init__.py
+-rw-r--r--   0        0        0     6663 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.1/oc_ds_converter/run/crossref_process.py
+-rw-r--r--   0        0        0     6657 2023-05-15 13:12:58.862517 oc_ds_converter-0.1.1/oc_ds_converter/run/datacite_process.py
+-rw-r--r--   0        0        0     7970 2023-05-15 13:12:58.863517 oc_ds_converter-0.1.1/oc_ds_converter/run/jalc_process.py
+-rw-r--r--   0        0        0     9697 2023-05-15 13:12:58.863517 oc_ds_converter-0.1.1/oc_ds_converter/run/pubmed_process.py
+-rw-r--r--   0        0        0      774 2023-05-15 13:20:27.328300 oc_ds_converter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      881 2023-05-15 13:12:58.853513 oc_ds_converter-0.1.1/README.md
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 oc_ds_converter-0.1.1/setup.py
+-rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 oc_ds_converter-0.1.1/PKG-INFO
```

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/crossref/crossref_processing.py` & `oc_ds_converter-0.1.1/oc_ds_converter/crossref/crossref_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/crossref/extract_crossref_publishers.py` & `oc_ds_converter-0.1.1/oc_ds_converter/crossref/extract_crossref_publishers.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/crossref/get_not_crossref_ref.py` & `oc_ds_converter-0.1.1/oc_ds_converter/crossref/get_not_crossref_ref.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/datacite/datacite_processing.py` & `oc_ds_converter-0.1.1/oc_ds_converter/datacite/datacite_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/datasource/datasource.py` & `oc_ds_converter-0.1.1/oc_ds_converter/datasource/datasource.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/datasource/redis.py` & `oc_ds_converter-0.1.1/oc_ds_converter/datasource/redis.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/jalc/jalc_processing.py` & `oc_ds_converter-0.1.1/oc_ds_converter/jalc/jalc_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/lib/__init__.py` & `oc_ds_converter-0.1.1/oc_ds_converter/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/lib/cleaner.py` & `oc_ds_converter-0.1.1/oc_ds_converter/lib/cleaner.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/lib/csvmanager.py` & `oc_ds_converter-0.1.1/oc_ds_converter/lib/csvmanager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/lib/file_manager.py` & `oc_ds_converter-0.1.1/oc_ds_converter/lib/file_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/lib/jsonmanager.py` & `oc_ds_converter-0.1.1/oc_ds_converter/lib/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/lib/master_of_regex.py` & `oc_ds_converter-0.1.1/oc_ds_converter/lib/master_of_regex.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/medra/medra_processing.py` & `oc_ds_converter-0.1.1/oc_ds_converter/medra/medra_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/metadata_manager.py` & `oc_ds_converter-0.1.1/oc_ds_converter/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/preprocessing/base.py` & `oc_ds_converter-0.1.1/oc_ds_converter/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/preprocessing/datacite.py` & `oc_ds_converter-0.1.1/oc_ds_converter/preprocessing/datacite.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/preprocessing/nih.py` & `oc_ds_converter-0.1.1/oc_ds_converter/preprocessing/nih.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/pubmed/finder_nih.py` & `oc_ds_converter-0.1.1/oc_ds_converter/pubmed/finder_nih.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/pubmed/get_publishers.py` & `oc_ds_converter-0.1.1/oc_ds_converter/pubmed/get_publishers.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/pubmed/pubmed_dump_explorer.py` & `oc_ds_converter-0.1.1/oc_ds_converter/pubmed/pubmed_dump_explorer.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/pubmed/pubmed_processing.py` & `oc_ds_converter-0.1.1/oc_ds_converter/pubmed/pubmed_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/pubmed/support_files/prefix_publishers.json` & `oc_ds_converter-0.1.1/oc_ds_converter/pubmed/support_files/prefix_publishers.json`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/ra_processor.py` & `oc_ds_converter-0.1.1/oc_ds_converter/ra_processor.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/run/crossref_process.py` & `oc_ds_converter-0.1.1/oc_ds_converter/run/crossref_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/run/datacite_process.py` & `oc_ds_converter-0.1.1/oc_ds_converter/run/datacite_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/run/jalc_process.py` & `oc_ds_converter-0.1.1/oc_ds_converter/run/jalc_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/oc_ds_converter/run/pubmed_process.py` & `oc_ds_converter-0.1.1/oc_ds_converter/run/pubmed_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/pyproject.toml` & `oc_ds_converter-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oc-ds-converter"
-version = "0.1.0"
+version = "0.1.1"
 description = "A library for converting metadata provided by various data sources, e.g. Crossref, DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta."
 authors = ["arcangelo7 <arcangelomas@gmail.com>"]
 license = "ISC"
 readme = "README.md"
 packages = [{include = "oc_ds_converter"}]
 
 [tool.poetry.dependencies]
```

### Comparing `oc_ds_converter-0.1.0/README.md` & `oc_ds_converter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-0.1.0/setup.py` & `oc_ds_converter-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'oc-idmanager>=0.2.6,<0.3.0',
  'redis>=4.5.5,<5.0.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'oc-ds-converter',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A library for converting metadata provided by various data sources, e.g. Crossref, DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta.',
     'long_description': '[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/ra_processor/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/oc_meta/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/ra_processor/main/test/coverage/coverage.svg)\n<!-- ![PyPI](https://img.shields.io/pypi/pyversions/oc_meta) -->\n![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/ra_processor)\n\n\n\n# OpenCitations Data Sources Converter\n\nThis repository contains scripts useful for converting scholarly bibliographic metadata from various data sources into the format accepted by OpenCitations Meta. The data sources currently supported are Crossref, DataCite, PubMed, mEDRA a JaLC.\n',
     'author': 'arcangelo7',
     'author_email': 'arcangelomas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `oc_ds_converter-0.1.0/PKG-INFO` & `oc_ds_converter-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oc-ds-converter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for converting metadata provided by various data sources, e.g. Crossref, DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta.
 License: ISC
 Author: arcangelo7
 Author-email: arcangelomas@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

