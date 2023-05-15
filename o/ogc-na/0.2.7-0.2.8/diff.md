# Comparing `tmp/ogc_na-0.2.7.tar.gz` & `tmp/ogc_na-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.2.7.tar", last modified: Mon May 15 13:25:47 2023, max compression
+gzip compressed data, was "ogc_na-0.2.8.tar", last modified: Mon May 15 13:41:25 2023, max compression
```

## Comparing `ogc_na-0.2.7.tar` & `ogc_na-0.2.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.882417 ogc_na-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.874416 ogc_na-0.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 13:25:35.000000 ogc_na-0.2.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-15 13:25:35.000000 ogc_na-0.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 13:25:35.000000 ogc_na-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 13:25:47.882417 ogc_na-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 13:25:35.000000 ogc_na-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-15 13:25:35.000000 ogc_na-0.2.7/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-15 13:25:35.000000 ogc_na-0.2.7/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 13:25:35.000000 ogc_na-0.2.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-15 13:25:35.000000 ogc_na-0.2.7/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 13:25:35.000000 ogc_na-0.2.7/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.874416 ogc_na-0.2.7/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    32037 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-15 13:25:35.000000 ogc_na-0.2.7/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.878416 ogc_na-0.2.7/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 13:25:47.000000 ogc_na-0.2.7/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 13:25:35.000000 ogc_na-0.2.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.882417 ogc_na-0.2.7/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 13:25:35.000000 ogc_na-0.2.7/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 13:25:35.000000 ogc_na-0.2.7/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 13:25:35.000000 ogc_na-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:25:47.882417 ogc_na-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 13:25:35.000000 ogc_na-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.882417 ogc_na-0.2.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:47.882417 ogc_na-0.2.7/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 13:25:35.000000 ogc_na-0.2.7/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.430858 ogc_na-0.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.434858 ogc_na-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 13:41:04.000000 ogc_na-0.2.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-15 13:41:04.000000 ogc_na-0.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 13:41:04.000000 ogc_na-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 13:41:25.438858 ogc_na-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 13:41:04.000000 ogc_na-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.434858 ogc_na-0.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-15 13:41:04.000000 ogc_na-0.2.8/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-15 13:41:04.000000 ogc_na-0.2.8/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 13:41:04.000000 ogc_na-0.2.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-15 13:41:04.000000 ogc_na-0.2.8/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 13:41:04.000000 ogc_na-0.2.8/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.434858 ogc_na-0.2.8/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.434858 ogc_na-0.2.8/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-15 13:41:04.000000 ogc_na-0.2.8/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 13:41:25.000000 ogc_na-0.2.8/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 13:41:04.000000 ogc_na-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 13:41:04.000000 ogc_na-0.2.8/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 13:41:04.000000 ogc_na-0.2.8/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 13:41:04.000000 ogc_na-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:41:25.438858 ogc_na-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 13:41:04.000000 ogc_na-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:25.438858 ogc_na-0.2.8/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 13:41:04.000000 ogc_na-0.2.8/test/test_profile.py
```

### Comparing `ogc_na-0.2.7/.github/workflows/python-publish.yml` & `ogc_na-0.2.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/.gitignore` & `ogc_na-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/PKG-INFO` & `ogc_na-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.2.7
+Version: 0.2.8
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.2.7/README.md` & `ogc_na-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/docs/examples.md` & `ogc_na-0.2.8/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/docs/gen_ref_pages.py` & `ogc_na-0.2.8/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/docs/index.md` & `ogc_na-0.2.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/docs/tutorials.md` & `ogc_na-0.2.8/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/mkdocs.yml` & `ogc_na-0.2.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/annotate_schema.py` & `ogc_na-0.2.8/ogc/na/annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/domain_config.py` & `ogc_na-0.2.8/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/download.py` & `ogc_na-0.2.8/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/ingest_json.py` & `ogc_na-0.2.8/ogc/na/ingest_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,19 @@
             type_list = [type_list]
         for item in items:
             existing = item.value.setdefault('@type', [])
             if isinstance(existing, str):
                 item.value['@type'] = [existing] + type_list
             else:
                 item.value['@type'].extend(type_list)
+            item_types = item.value.get('@type')
+            if not item_types:
+                item.value.pop('@type', None)
+            elif isinstance(item_types, Sequence) and not isinstance(item_types, str) and len(item_types) == 1:
+                item.value['@type'] = item_types[0]
 
     # Add contexts
     context_list = context.get('context', {})
     global_context = None
     for loc, val in context_list.items():
         if not loc or loc in ['.', '$']:
             global_context = val
```

### Comparing `ogc_na-0.2.7/ogc/na/input_filters/__init__.py` & `ogc_na-0.2.8/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/input_filters/csv.py` & `ogc_na-0.2.8/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/profile.py` & `ogc_na-0.2.8/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/provenance.py` & `ogc_na-0.2.8/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/update_vocabs.py` & `ogc_na-0.2.8/ogc/na/update_vocabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,19 +439,20 @@
                 for ea in entail_artifacts or ():
                     add_artifact(ea)
                 for res in validation_result.used_resources or ():
                     add_artifact(res)
 
             docrelpath = Path(os.path.relpath(doc, args.working_directory))
             if output_path:
-                output_doc = output_path / docrelpath
-                entailment_dir = (output_doc.parent / args.entailment_directory).resolve()
+                output_doc = output_path.resolve() / docrelpath
+                entailment_dir = output_doc.parent / args.entailment_directory
+                output_doc = entailment_dir / output_doc.name
             else:
-                entailment_dir = args.entailment_directory
-                output_doc = doc
+                entailment_dir = Path(args.entailment_directory).resolve()
+                output_doc = entailment_dir / doc.name
 
             os.makedirs(output_doc.parent, exist_ok=True)
             os.makedirs(entailment_dir, exist_ok=True)
 
             with open(output_doc.with_suffix('.txt'), 'w') as validation_file:
                 validation_file.write(validation_result.text)
```

### Comparing `ogc_na-0.2.7/ogc/na/util.py` & `ogc_na-0.2.8/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc/na/validation.py` & `ogc_na-0.2.8/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.2.8/ogc_na.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.2.7
+Version: 0.2.8
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.2.7/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.2.8/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/pyproject.toml` & `ogc_na-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/rdf/domaincfg.vocab.ttl` & `ogc_na-0.2.8/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/test/data/headers.csv` & `ogc_na-0.2.8/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/test/data/uplift_context_valid.yml` & `ogc_na-0.2.8/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/test/test_annotate_schema.py` & `ogc_na-0.2.8/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/test/test_ingest_json.py` & `ogc_na-0.2.8/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/test/test_input_filters_csv.py` & `ogc_na-0.2.8/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.7/test/test_profile.py` & `ogc_na-0.2.8/test/test_profile.py`

 * *Files identical despite different names*

