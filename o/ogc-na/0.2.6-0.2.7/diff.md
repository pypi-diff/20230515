# Comparing `tmp/ogc_na-0.2.6.tar.gz` & `tmp/ogc_na-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.2.6.tar", last modified: Mon May 15 12:01:50 2023, max compression
+gzip compressed data, was "ogc_na-0.2.7.tar", last modified: Mon May 15 13:25:47 2023, max compression
```

## Comparing `ogc_na-0.2.6.tar` & `ogc_na-0.2.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.688110 ogc_na-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.680110 ogc_na-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.680110 ogc_na-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 12:01:34.000000 ogc_na-0.2.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-15 12:01:34.000000 ogc_na-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 12:01:34.000000 ogc_na-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 12:01:50.688110 ogc_na-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 12:01:34.000000 ogc_na-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.680110 ogc_na-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-15 12:01:34.000000 ogc_na-0.2.6/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-15 12:01:34.000000 ogc_na-0.2.6/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 12:01:34.000000 ogc_na-0.2.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-15 12:01:34.000000 ogc_na-0.2.6/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 12:01:34.000000 ogc_na-0.2.6/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.680110 ogc_na-0.2.6/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.684110 ogc_na-0.2.6/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    32037 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.684110 ogc_na-0.2.6/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-15 12:01:34.000000 ogc_na-0.2.6/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.684110 ogc_na-0.2.6/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 12:01:50.000000 ogc_na-0.2.6/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 12:01:50.000000 ogc_na-0.2.6/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:01:50.000000 ogc_na-0.2.6/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 12:01:50.000000 ogc_na-0.2.6/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 12:01:50.000000 ogc_na-0.2.6/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 12:01:34.000000 ogc_na-0.2.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.684110 ogc_na-0.2.6/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 12:01:34.000000 ogc_na-0.2.6/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 12:01:34.000000 ogc_na-0.2.6/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 12:01:34.000000 ogc_na-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:01:50.688110 ogc_na-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 12:01:34.000000 ogc_na-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.684110 ogc_na-0.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:50.688110 ogc_na-0.2.6/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 12:01:34.000000 ogc_na-0.2.6/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.882417 ogc_na-0.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.874416 ogc_na-0.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 13:25:35.000000 ogc_na-0.2.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-15 13:25:35.000000 ogc_na-0.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 13:25:35.000000 ogc_na-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 13:25:47.882417 ogc_na-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 13:25:35.000000 ogc_na-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-15 13:25:35.000000 ogc_na-0.2.7/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-15 13:25:35.000000 ogc_na-0.2.7/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 13:25:35.000000 ogc_na-0.2.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-15 13:25:35.000000 ogc_na-0.2.7/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 13:25:35.000000 ogc_na-0.2.7/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.874416 ogc_na-0.2.7/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32037 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 13:25:35.000000 ogc_na-0.2.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.882417 ogc_na-0.2.7/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 13:25:35.000000 ogc_na-0.2.7/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 13:25:35.000000 ogc_na-0.2.7/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 13:25:35.000000 ogc_na-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:25:47.882417 ogc_na-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 13:25:35.000000 ogc_na-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.882417 ogc_na-0.2.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.882417 ogc_na-0.2.7/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/test_profile.py
```

### Comparing `ogc_na-0.2.6/.github/workflows/python-publish.yml` & `ogc_na-0.2.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/.gitignore` & `ogc_na-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/PKG-INFO` & `ogc_na-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.2.6
+Version: 0.2.7
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.2.6/README.md` & `ogc_na-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/docs/examples.md` & `ogc_na-0.2.7/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/docs/gen_ref_pages.py` & `ogc_na-0.2.7/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/docs/index.md` & `ogc_na-0.2.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/docs/tutorials.md` & `ogc_na-0.2.7/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/mkdocs.yml` & `ogc_na-0.2.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/annotate_schema.py` & `ogc_na-0.2.7/ogc/na/annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/domain_config.py` & `ogc_na-0.2.7/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/download.py` & `ogc_na-0.2.7/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/ingest_json.py` & `ogc_na-0.2.7/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/input_filters/__init__.py` & `ogc_na-0.2.7/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/input_filters/csv.py` & `ogc_na-0.2.7/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/profile.py` & `ogc_na-0.2.7/ogc/na/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,40 +306,37 @@
         if additional_profiles:
             profiles.extend(p if isinstance(p, URIRef) else URIRef(p) for p in additional_profiles)
 
         profiles = self.build_profile_chain(profiles, recursive=recursive)
 
         artifacts = set()
         for profile_ref in profiles:
+            logger.info('Entailing with %s', profile_ref)
             rules, rules_artifacts, failed_artifacts = self.get_graph(profile_ref, ROLE_ENTAILMENT)
             extra, extra_artifacts, failed_artifacts = self.get_graph(profile_ref, ROLE_ENTAILMENT_CLOSURE)
             if rules_artifacts:
                 artifacts.update(rules_artifacts)
             if extra_artifacts:
                 artifacts.update(extra_artifacts)
             g = util.entail(g, rules, extra or None, True)
 
-            profile = self.profiles.get(profile_ref)
-            if recursive and profile and profile.profile_of:
-                profiles.extend(profile.profile_of)
-
         return g, artifacts
 
     def validate(self, g: Graph,
                  additional_profiles: Sequence[str | URIRef] | None = None,
                  recursive: bool = True, log_artifact_errors: bool = False) -> ProfilesValidationReport:
         result = ProfilesValidationReport()
         profiles = deque(find_profiles(g))
         if additional_profiles:
             profiles.extend(p if isinstance(p, URIRef) else URIRef(p) for p in additional_profiles)
 
         profiles = self.build_profile_chain(profiles, recursive=recursive, sort=False)
 
         for profile_ref in profiles:
-            logger.debug("Validating with %s", str(profile_ref))
+            logger.info("Validating with %s", str(profile_ref))
             profile = self.profiles.get(profile_ref)
             if not profile:
                 logger.warning("Profile %s not found", profile_ref)
                 # should we fail?
                 continue
             rules, rules_artifacts, failed_rules_artifacts = self.get_graph(profile_ref, ROLE_VALIDATION)
             extra, extra_artifacts, failed_extra_artifacts = self.get_graph(profile_ref, ROLE_VALIDATION_CLOSURE)
```

### Comparing `ogc_na-0.2.6/ogc/na/provenance.py` & `ogc_na-0.2.7/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/update_vocabs.py` & `ogc_na-0.2.7/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/util.py` & `ogc_na-0.2.7/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc/na/validation.py` & `ogc_na-0.2.7/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.2.7/ogc_na.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.2.6
+Version: 0.2.7
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.2.6/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.2.7/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/pyproject.toml` & `ogc_na-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/rdf/domaincfg.vocab.ttl` & `ogc_na-0.2.7/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/test/data/headers.csv` & `ogc_na-0.2.7/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/test/data/uplift_context_valid.yml` & `ogc_na-0.2.7/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/test/test_annotate_schema.py` & `ogc_na-0.2.7/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/test/test_ingest_json.py` & `ogc_na-0.2.7/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/test/test_input_filters_csv.py` & `ogc_na-0.2.7/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.6/test/test_profile.py` & `ogc_na-0.2.7/test/test_profile.py`

 * *Files identical despite different names*

