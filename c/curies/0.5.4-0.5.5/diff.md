# Comparing `tmp/curies-0.5.4.tar.gz` & `tmp/curies-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curies-0.5.4.tar", last modified: Fri Apr 28 13:06:22 2023, max compression
+gzip compressed data, was "curies-0.5.5.tar", last modified: Mon May 15 10:40:42 2023, max compression
```

## Comparing `curies-0.5.4.tar` & `curies-0.5.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.020704 curies-0.5.4/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-07-31 23:04:00.000000 curies-0.5.4/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      394 2023-04-28 13:05:54.000000 curies-0.5.4/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)    11651 2023-04-28 13:06:22.021134 curies-0.5.4/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)    10132 2023-04-28 13:05:54.000000 curies-0.5.4/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:21.989361 curies-0.5.4/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:21.993328 curies-0.5.4/docs/source/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.005335 curies-0.5.4/docs/source/api/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1864 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.Converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      101 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.DuplicatePrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.DuplicateURIPrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      107 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.DuplicateValueError.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       86 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.Record.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.chain.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_bioregistry_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       94 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_fastapi_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_flask_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_flask_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_go_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_monarch_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      100 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_obo_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_prefixcommons_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.get_version.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      141 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      134 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      119 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-04-13 07:20:08.000000 curies-0.5.4/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7458 2023-04-28 13:06:20.000000 curies-0.5.4/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2538 2023-03-10 11:58:39.000000 curies-0.5.4/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      385 2022-12-09 17:27:17.000000 curies-0.5.4/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2668 2023-04-28 13:06:22.022415 curies-0.5.4/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:21.990101 curies-0.5.4/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.010973 curies-0.5.4/src/curies/
--rw-r--r--   0 cthoyt     (501) staff       (20)      941 2023-02-21 22:19:21.000000 curies-0.5.4/src/curies/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-02-21 22:19:21.000000 curies-0.5.4/src/curies/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    38646 2023-04-13 06:17:21.000000 curies-0.5.4/src/curies/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5065 2023-04-13 07:17:14.000000 curies-0.5.4/src/curies/cli.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.016123 curies-0.5.4/src/curies/mapping_service/
--rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-04-13 07:57:38.000000 curies-0.5.4/src/curies/mapping_service/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     8222 2023-04-13 07:57:38.000000 curies-0.5.4/src/curies/mapping_service/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-03-26 20:29:12.000000 curies-0.5.4/src/curies/mapping_service/rdflib_custom.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4637 2023-04-28 13:05:54.000000 curies-0.5.4/src/curies/mapping_service/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:01.000000 curies-0.5.4/src/curies/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     2033 2023-03-04 12:32:17.000000 curies-0.5.4/src/curies/sources.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      255 2023-04-28 13:06:20.000000 curies-0.5.4/src/curies/version.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     9666 2023-04-13 06:43:24.000000 curies-0.5.4/src/curies/web.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.013893 curies-0.5.4/src/curies.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)    11651 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1853 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:24.000000 curies-0.5.4/src/curies.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      273 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        7 2023-04-28 13:06:21.000000 curies-0.5.4/src/curies.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-28 13:06:22.019823 curies-0.5.4/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       56 2022-07-31 23:04:00.000000 curies-0.5.4/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        0 2023-03-23 13:16:42.000000 curies-0.5.4/tests/rules.log
--rw-r--r--   0 cthoyt     (501) staff       (20)    17050 2023-04-13 06:17:21.000000 curies-0.5.4/tests/test_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-04-13 10:20:39.000000 curies-0.5.4/tests/test_federated_sparql.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    13426 2023-04-13 07:57:38.000000 curies-0.5.4/tests/test_mapping_service.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3271 2023-04-13 06:37:08.000000 curies-0.5.4/tests/test_web.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.855506 curies-0.5.5/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-07-31 23:04:00.000000 curies-0.5.5/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      394 2023-04-28 13:05:54.000000 curies-0.5.5/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11827 2023-05-15 10:40:42.855681 curies-0.5.5/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10308 2023-05-05 11:46:12.000000 curies-0.5.5/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.823165 curies-0.5.5/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.827618 curies-0.5.5/docs/source/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.839925 curies-0.5.5/docs/source/api/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1864 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.Converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      101 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.DuplicatePrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.DuplicateURIPrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      107 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.DuplicateValueError.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       86 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.Record.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.chain.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_bioregistry_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       94 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_fastapi_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_flask_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_flask_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_go_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_monarch_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_obo_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_prefixcommons_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_version.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      141 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      134 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      119 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7469 2023-05-15 10:40:41.000000 curies-0.5.5/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2538 2023-03-10 11:58:39.000000 curies-0.5.5/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      385 2022-12-09 17:27:17.000000 curies-0.5.5/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2678 2023-05-15 10:40:42.856773 curies-0.5.5/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.823737 curies-0.5.5/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.846252 curies-0.5.5/src/curies/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1015 2023-05-15 10:11:51.000000 curies-0.5.5/src/curies/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-02-21 22:19:21.000000 curies-0.5.5/src/curies/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    44040 2023-05-15 10:23:41.000000 curies-0.5.5/src/curies/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5065 2023-04-13 07:17:14.000000 curies-0.5.5/src/curies/cli.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.851173 curies-0.5.5/src/curies/mapping_service/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-04-13 07:57:38.000000 curies-0.5.5/src/curies/mapping_service/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8224 2023-05-05 11:46:12.000000 curies-0.5.5/src/curies/mapping_service/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-03-26 20:29:12.000000 curies-0.5.5/src/curies/mapping_service/rdflib_custom.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4637 2023-05-05 11:46:12.000000 curies-0.5.5/src/curies/mapping_service/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:01.000000 curies-0.5.5/src/curies/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2033 2023-03-04 12:32:17.000000 curies-0.5.5/src/curies/sources.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      255 2023-05-15 10:40:41.000000 curies-0.5.5/src/curies/version.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9666 2023-04-13 06:43:24.000000 curies-0.5.5/src/curies/web.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.848960 curies-0.5.5/src/curies.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11827 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1853 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:24.000000 curies-0.5.5/src/curies.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      282 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        7 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.854958 curies-0.5.5/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       56 2022-07-31 23:04:00.000000 curies-0.5.5/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        0 2023-03-23 13:16:42.000000 curies-0.5.5/tests/rules.log
+-rw-r--r--   0 cthoyt     (501) staff       (20)    18891 2023-05-15 10:20:25.000000 curies-0.5.5/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-04-13 10:20:39.000000 curies-0.5.5/tests/test_federated_sparql.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    13426 2023-04-13 07:57:38.000000 curies-0.5.5/tests/test_mapping_service.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3271 2023-04-13 06:37:08.000000 curies-0.5.5/tests/test_web.py
```

### Comparing `curies-0.5.4/LICENSE` & `curies-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/PKG-INFO` & `curies-0.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.5.4
+Version: 0.5.5
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -189,14 +189,19 @@
 import curies
 import pandas as pd
 
 df = pd.read_csv(...)
 obo_converter = curies.get_obo_converter()
 obo_converter.pd_compress(df, column=0)
 obo_converter.pd_expand(df, column=0)
+
+# standardization operations
+obo_converter.pd_standardize_prefix(df, column=0)
+obo_converter.pd_standardize_curie(df, column=0)
+obo_converter.pd_standardize_uri(df, column=0)
 ```
 
 Apply in bulk to a CSV file with `Converter.file_expand` and
 `Converter.file_compress` (defaults to using tab separator):
 
 ```python
 import curies
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies Version: 0.5.4 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.5.5 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies Classifier:
@@ -62,17 +62,20 @@
 bioregistry_converter = curies.get_bioregistry_converter() # Uses the OBO
 Foundry, a registry of ontologies obo_converter = curies.get_obo_converter() #
 Uses the Monarch Initative's project-specific context monarch_converter =
 curies.get_monarch_converter() ``` ### Bulk Operations Apply in bulk to a
 `pandas.DataFrame` with `Converter.pd_expand` and `Converter.pd_compress`:
 ```python import curies import pandas as pd df = pd.read_csv(...) obo_converter
 = curies.get_obo_converter() obo_converter.pd_compress(df, column=0)
-obo_converter.pd_expand(df, column=0) ``` Apply in bulk to a CSV file with
-`Converter.file_expand` and `Converter.file_compress` (defaults to using tab
-separator): ```python import curies path = ... obo_converter =
+obo_converter.pd_expand(df, column=0) # standardization operations
+obo_converter.pd_standardize_prefix(df, column=0)
+obo_converter.pd_standardize_curie(df, column=0)
+obo_converter.pd_standardize_uri(df, column=0) ``` Apply in bulk to a CSV file
+with `Converter.file_expand` and `Converter.file_compress` (defaults to using
+tab separator): ```python import curies path = ... obo_converter =
 curies.get_obo_converter() # modifies file in place obo_converter.file_compress
 (path, column=0) # modifies file in place obo_converter.file_expand(path,
 column=0) ``` ### CLI Usage This package comes with a built-in CLI for running
 a resolver web application or a IRI mapper web application: ```shell # Run a
 resolver python -m curies resolver --host 0.0.0.0 --port 8764 bioregistry # Run
 a mapper python -m curies mapper --host 0.0.0.0 --port 8764 bioregistry ``` The
 positional argument can be one of the following: 1. A pre-defined prefix map to
```

### Comparing `curies-0.5.4/README.md` & `curies-0.5.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,19 @@
 import curies
 import pandas as pd
 
 df = pd.read_csv(...)
 obo_converter = curies.get_obo_converter()
 obo_converter.pd_compress(df, column=0)
 obo_converter.pd_expand(df, column=0)
+
+# standardization operations
+obo_converter.pd_standardize_prefix(df, column=0)
+obo_converter.pd_standardize_curie(df, column=0)
+obo_converter.pd_standardize_uri(df, column=0)
 ```
 
 Apply in bulk to a CSV file with `Converter.file_expand` and
 `Converter.file_compress` (defaults to using tab separator):
 
 ```python
 import curies
```

#### html2text {}

```diff
@@ -42,17 +42,20 @@
 bioregistry_converter = curies.get_bioregistry_converter() # Uses the OBO
 Foundry, a registry of ontologies obo_converter = curies.get_obo_converter() #
 Uses the Monarch Initative's project-specific context monarch_converter =
 curies.get_monarch_converter() ``` ### Bulk Operations Apply in bulk to a
 `pandas.DataFrame` with `Converter.pd_expand` and `Converter.pd_compress`:
 ```python import curies import pandas as pd df = pd.read_csv(...) obo_converter
 = curies.get_obo_converter() obo_converter.pd_compress(df, column=0)
-obo_converter.pd_expand(df, column=0) ``` Apply in bulk to a CSV file with
-`Converter.file_expand` and `Converter.file_compress` (defaults to using tab
-separator): ```python import curies path = ... obo_converter =
+obo_converter.pd_expand(df, column=0) # standardization operations
+obo_converter.pd_standardize_prefix(df, column=0)
+obo_converter.pd_standardize_curie(df, column=0)
+obo_converter.pd_standardize_uri(df, column=0) ``` Apply in bulk to a CSV file
+with `Converter.file_expand` and `Converter.file_compress` (defaults to using
+tab separator): ```python import curies path = ... obo_converter =
 curies.get_obo_converter() # modifies file in place obo_converter.file_compress
 (path, column=0) # modifies file in place obo_converter.file_expand(path,
 column=0) ``` ### CLI Usage This package comes with a built-in CLI for running
 a resolver web application or a IRI mapper web application: ```shell # Run a
 resolver python -m curies resolver --host 0.0.0.0 --port 8764 bioregistry # Run
 a mapper python -m curies mapper --host 0.0.0.0 --port 8764 bioregistry ``` The
 positional argument can be one of the following: 1. A pre-defined prefix map to
```

### Comparing `curies-0.5.4/docs/source/api/curies.Converter.rst` & `curies-0.5.5/docs/source/api/curies.Converter.rst`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/docs/source/conf.py` & `curies-0.5.5/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "curies"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.5.4"
+release = "0.5.5"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
@@ -222,15 +222,15 @@
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/3/": None,
+    "python": ("https://docs.python.org/3", None),
     "bioregistry": ("https://bioregistry.readthedocs.io/en/stable/", None),
     "pandas": ("https://pandas.pydata.org/docs/", None),
     "flask": ("https://flask.palletsprojects.com/", None),
     # "fastapi": ("https://fastapi.tiangolo.com/", None),
     # "gunicorn": ("https://docs.gunicorn.org/", None),
     # "uvicorn": ("https://www.uvicorn.org/", None),
     "prefixmaps": ("https://linkml.io/prefixmaps/", None),
```

### Comparing `curies-0.5.4/docs/source/index.rst` & `curies-0.5.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/setup.cfg` & `curies-0.5.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = curies
-version = 0.5.4
+version = 0.5.5
 description = Idiomatic conversion between URIs and compact URIs (CURIEs).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/curies
 download_url = https://github.com/cthoyt/curies/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/curies/issues
@@ -39,14 +39,15 @@
 	compact uniform resource identifiers
 	uniform resource identifiers
 	curies
 
 [options]
 install_requires = 
 	pytrie
+	pydantic
 	requests
 zip_safe = false
 include_package_data = True
 python_requires = >=3.7
 packages = find:
 package_dir = 
 	= src
```

### Comparing `curies-0.5.4/src/curies/__init__.py` & `curies-0.5.5/src/curies/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from .api import (
     Converter,
     DuplicatePrefixes,
     DuplicateURIPrefixes,
     DuplicateValueError,
     Record,
+    Reference,
+    ReferenceTuple,
     chain,
 )
 from .sources import (
     get_bioregistry_converter,
     get_go_converter,
     get_monarch_converter,
     get_obo_converter,
@@ -19,14 +21,16 @@
 )
 from .version import get_version
 from .web import get_fastapi_app, get_fastapi_router, get_flask_app, get_flask_blueprint
 
 __all__ = [
     "Converter",
     "Record",
+    "ReferenceTuple",
+    "Reference",
     "DuplicateValueError",
     "DuplicateURIPrefixes",
     "DuplicatePrefixes",
     "chain",
     "get_version",
     # sources
     "get_obo_converter",
```

### Comparing `curies-0.5.4/src/curies/api.py` & `curies-0.5.5/src/curies/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,76 +2,180 @@
 
 """Data structures and algorithms for :mod:`curies`."""
 
 import csv
 import itertools as itt
 import json
 from collections import defaultdict
-from dataclasses import dataclass, field
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Collection,
     DefaultDict,
     Dict,
     Iterable,
     List,
     Mapping,
+    NamedTuple,
     Optional,
     Sequence,
     Set,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 import requests
+from pydantic import BaseModel, Field, validator
 from pytrie import StringTrie
 
 if TYPE_CHECKING:  # pragma: no cover
     import pandas
     import rdflib
 
 __all__ = [
     "Converter",
+    "Reference",
+    "ReferenceTuple",
     "Record",
     "DuplicateValueError",
     "DuplicatePrefixes",
     "DuplicateURIPrefixes",
     "chain",
 ]
 
 X = TypeVar("X")
 LocationOr = Union[str, Path, X]
 
 
-@dataclass
-class Record:
-    """A record of some prefixes and their associated URI prefixes."""
+class ReferenceTuple(NamedTuple):
+    """A reference to an entity in a given identifier space.
+
+    This derives from the "named tuple" which means that it acts
+    like a tuple in most senses - it can be hashed and unpacked
+    like most other tuples. Underneath, it has a C implementation
+    and is very efficient.
+    """
 
-    #: The canonical prefix, used in the reverse prefix map
     prefix: str
-    #: The canonical URI prefix, used in the forward prefix map
-    uri_prefix: str
-    prefix_synonyms: List[str] = field(default_factory=list)
-    uri_prefix_synonyms: List[str] = field(default_factory=list)
-
-    def __post_init__(self) -> None:
-        """Check the integrity of the record."""
-        for ps in self.prefix_synonyms:
-            if ps == self.prefix:
-                raise ValueError(f"Duplicate of canonical prefix `{self.prefix}` in synonyms")
-        for ups in self.uri_prefix_synonyms:
-            if ups == self.uri_prefix:
-                raise ValueError(
-                    f"Duplicate of canonical URI prefix `{self.uri_prefix}` in synonyms"
-                )
+    identifier: str
+
+    @property
+    def curie(self) -> str:
+        """Get the reference as a CURIE string.
+
+        :return:
+            A string representation of a compact URI (CURIE).
+
+        >>> ReferenceTuple("chebi", "1234").curie
+        'chebi:1234'
+        """
+        return f"{self.prefix}:{self.identifier}"
+
+    @classmethod
+    def from_curie(cls, curie: str, sep: str = ":") -> "ReferenceTuple":
+        """Parse a CURIE string and populate a reference tuple.
+
+        :param curie: A string representation of a compact URI (CURIE)
+        :param sep: The separator
+        :return: A reference tuple
+
+        >>> ReferenceTuple.from_curie("chebi:1234")
+        ReferenceTuple(prefix='chebi', identifier='1234')
+        """
+        prefix, identifier = curie.split(sep, 1)
+        return cls(prefix, identifier)
+
+
+class Reference(BaseModel):  # type:ignore
+    """A reference to an entity in a given identifier space.
+
+    This class uses Pydantic to make it easier to build other
+    more complex data types with Pydantic that also uses a first-
+    class notion of parsed reference (instead of merely stringified
+    CURIEs). Instances of this class can also be hashed because of the
+    "frozen" configuration from Pydantic (see
+    https://docs.pydantic.dev/latest/usage/model_config/ for more details).
+    """
+
+    prefix: str = Field(
+        ...,
+        description="The prefix used in a compact URI (CURIE).",
+    )
+    identifier: str = Field(
+        ..., description="The local unique identifier used in a compact URI (CURIE)."
+    )
+
+    class Config:
+        """Pydantic configuration for references."""
+
+        frozen = True
+
+    @property
+    def curie(self) -> str:
+        """Get the reference as a CURIE string.
+
+        :return:
+            A string representation of a compact URI (CURIE).
+
+        >>> Reference(prefix="chebi", identifier="1234").curie
+        'chebi:1234'
+        """
+        return f"{self.prefix}:{self.identifier}"
+
+    @property
+    def pair(self) -> ReferenceTuple:
+        """Get the reference as a 2-tuple of prefix and identifier."""
+        return ReferenceTuple(self.prefix, self.identifier)
+
+    @classmethod
+    def from_curie(cls, curie: str, sep: str = ":") -> "Reference":
+        """Parse a CURIE string and populate a reference.
+
+        :param curie: A string representation of a compact URI (CURIE)
+        :param sep: The separator
+        :return: A reference object
+
+        >>> Reference.from_curie("chebi:1234")
+        Reference(prefix='chebi', identifier='1234')
+        """
+        prefix, identifier = curie.split(sep, 1)
+        return cls(prefix=prefix, identifier=identifier)
+
+
+class Record(BaseModel):  # type:ignore
+    """A record of some prefixes and their associated URI prefixes."""
+
+    prefix: str = Field(..., description="The canonical prefix, used in the reverse prefix map")
+    uri_prefix: str = Field(
+        ..., description="The canonical URI prefix, used in the forward prefix map"
+    )
+    prefix_synonyms: List[str] = Field(default_factory=list)
+    uri_prefix_synonyms: List[str] = Field(default_factory=list)
+
+    @validator("prefix_synonyms")  # type:ignore
+    def prefix_not_in_synonyms(cls, v: str, values: Mapping[str, Any]) -> str:  # noqa:N805
+        """Check that the canonical prefix does not apper in the prefix synonym list."""
+        prefix = values["prefix"]
+        if prefix in v:
+            raise ValueError(f"Duplicate of canonical prefix `{prefix}` in prefix synonyms")
+        return v
+
+    @validator("uri_prefix_synonyms")  # type:ignore
+    def uri_prefix_not_in_synonyms(cls, v: str, values: Mapping[str, Any]) -> str:  # noqa:N805
+        """Check that the canonical URI prefix does not apper in the URI prefix synonym list."""
+        uri_prefix = values["uri_prefix"]
+        if uri_prefix in v:
+            raise ValueError(
+                f"Duplicate of canonical URI prefix `{uri_prefix}` in URI prefix synonyms"
+            )
+        return v
 
     @property
     def _all_prefixes(self) -> List[str]:
         return [self.prefix, *self.prefix_synonyms]
 
     @property
     def _all_uri_prefixes(self) -> List[str]:
@@ -241,14 +345,15 @@
 
     def add_record(self, record: Record) -> None:
         """Append a record to the converter."""
         self._check_record(record)
 
         self.records.append(record)
         self.prefix_map[record.prefix] = record.uri_prefix
+        self.synonym_to_prefix[record.prefix] = record.prefix
         for prefix_synonym in record.prefix_synonyms:
             self.prefix_map[prefix_synonym] = record.uri_prefix
             self.synonym_to_prefix[prefix_synonym] = record.prefix
 
         self.reverse_prefix_map[record.uri_prefix] = record.prefix
         self.trie[record.uri_prefix] = record.prefix
         for uri_prefix_synonym in record.uri_prefix_synonyms:
@@ -598,15 +703,15 @@
         >>> converter.compress("http://example.org/missing:0000000")
         """
         prefix, identifier = self.parse_uri(uri)
         if prefix is None or identifier is None:
             return None
         return self.format_curie(prefix, identifier)
 
-    def parse_uri(self, uri: str) -> Union[Tuple[str, str], Tuple[None, None]]:
+    def parse_uri(self, uri: str) -> Union[ReferenceTuple, Tuple[None, None]]:
         """Compress a URI to a CURIE pair.
 
         :param uri:
             A string representing a valid uniform resource identifier (URI)
         :returns:
             A CURIE pair if the URI could be parsed, otherwise a pair of None's
 
@@ -622,15 +727,15 @@
         (None, None)
         """
         try:
             value, prefix = self.trie.longest_prefix_item(uri)
         except KeyError:
             return None, None
         else:
-            return prefix, uri[len(value) :]
+            return ReferenceTuple(prefix, uri[len(value) :])
 
     def expand(self, curie: str) -> Optional[str]:
         """Expand a CURIE to a URI, if possible.
 
         :param curie:
             A string representing a compact URI
         :returns:
@@ -680,18 +785,18 @@
         ['http://purl.obolibrary.org/obo/CHEBI_138488', 'https://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI:138488']
         >>> converter.expand_all("NOPE:NOPE") is None
         True
         """
         prefix, identifier = self.parse_curie(curie)
         return self.expand_pair_all(prefix, identifier)
 
-    def parse_curie(self, curie: str) -> Tuple[str, str]:
+    def parse_curie(self, curie: str) -> ReferenceTuple:
         """Parse a CURIE."""
-        prefix, identifier = curie.split(self.delimiter, 1)
-        return prefix, identifier
+        reference = Reference.from_curie(curie, sep=self.delimiter)
+        return reference.pair
 
     def expand_pair(self, prefix: str, identifier: str) -> Optional[str]:
         """Expand a CURIE pair to the standard URI.
 
         :param prefix:
             The prefix of the CURIE
         :param identifier:
@@ -759,15 +864,15 @@
         >>> from curies import Converter, Record
         >>> converter = Converter.from_extended_prefix_map([
         ...     Record(prefix="CHEBI", prefix_synonyms=["chebi"], uri_prefix="..."),
         ... ])
         >>> converter.standardize_prefix("chebi")
         'CHEBI'
         >>> converter.standardize_prefix("CHEBI")
-        'CHEBI:138488'
+        'CHEBI'
         >>> converter.standardize_prefix("NOPE") is None
         True
         """
         return self.synonym_to_prefix.get(prefix)
 
     def standardize_curie(self, curie: str) -> Optional[str]:
         """Standardize a CURIE.
@@ -855,14 +960,65 @@
 
         :param df: A pandas DataFrame
         :param column: The column in the dataframe containing CURIEs to convert to URIs.
         :param target_column: The column to put the results in. Defaults to input column.
         """
         df[column if target_column is None else target_column] = df[column].map(self.expand)
 
+    def pd_standardize_prefix(
+        self,
+        df: "pandas.DataFrame",
+        *,
+        column: Union[str, int],
+        target_column: Union[None, str, int] = None,
+    ) -> None:
+        """Standardize all prefixes in the given column.
+
+        :param df: A pandas DataFrame
+        :param column: The column in the dataframe containing prefixes to standardize.
+        :param target_column: The column to put the results in. Defaults to input column.
+        """
+        df[column if target_column is None else target_column] = df[column].map(
+            self.standardize_prefix
+        )
+
+    def pd_standardize_curie(
+        self,
+        df: "pandas.DataFrame",
+        *,
+        column: Union[str, int],
+        target_column: Union[None, str, int] = None,
+    ) -> None:
+        """Standardize all CURIEs in the given column.
+
+        :param df: A pandas DataFrame
+        :param column: The column in the dataframe containing CURIEs to standardize.
+        :param target_column: The column to put the results in. Defaults to input column.
+        """
+        df[column if target_column is None else target_column] = df[column].map(
+            self.standardize_curie
+        )
+
+    def pd_standardize_uri(
+        self,
+        df: "pandas.DataFrame",
+        *,
+        column: Union[str, int],
+        target_column: Union[None, str, int] = None,
+    ) -> None:
+        """Standardize all URIs in the given column.
+
+        :param df: A pandas DataFrame
+        :param column: The column in the dataframe containing URIs to standardize.
+        :param target_column: The column to put the results in. Defaults to input column.
+        """
+        df[column if target_column is None else target_column] = df[column].map(
+            self.standardize_uri
+        )
+
     def file_compress(
         self, path: Union[str, Path], column: int, sep: Optional[str] = None, header: bool = True
     ) -> None:
         """Convert all URIs in the given column of a CSV file to CURIEs.
 
         :param path: A pandas DataFrame
         :param column: The column in the dataframe containing URIs to convert to CURIEs.
```

### Comparing `curies-0.5.4/src/curies/cli.py` & `curies-0.5.5/src/curies/cli.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/src/curies/mapping_service/__init__.py` & `curies-0.5.5/src/curies/mapping_service/__init__.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/src/curies/mapping_service/api.py` & `curies-0.5.5/src/curies/mapping_service/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                         "http://purl.obolibrary.org/obo/CHEBI_",
                     ],
                     "GO": ["http://purl.obolibrary.org/obo/GO_"],
                     "OBO": ["http://purl.obolibrary.org/obo/"],
                     ...,
                 }
             )
-            graph = CURIEServiceGraph(converter=converter)
+            graph = MappingServiceGraph(converter=converter)
 
             res = graph.query('''
                 SELECT ?o WHERE {
                     VALUES ?s {
                         <http://purl.obolibrary.org/obo/CHEBI_1>
                     }
                     ?s owl:sameAs ?o
```

### Comparing `curies-0.5.4/src/curies/mapping_service/rdflib_custom.py` & `curies-0.5.5/src/curies/mapping_service/rdflib_custom.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/src/curies/mapping_service/utils.py` & `curies-0.5.5/src/curies/mapping_service/utils.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/src/curies/sources.py` & `curies-0.5.5/src/curies/sources.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/src/curies/web.py` & `curies-0.5.5/src/curies/web.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/src/curies.egg-info/PKG-INFO` & `curies-0.5.5/src/curies.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.5.4
+Version: 0.5.5
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -189,14 +189,19 @@
 import curies
 import pandas as pd
 
 df = pd.read_csv(...)
 obo_converter = curies.get_obo_converter()
 obo_converter.pd_compress(df, column=0)
 obo_converter.pd_expand(df, column=0)
+
+# standardization operations
+obo_converter.pd_standardize_prefix(df, column=0)
+obo_converter.pd_standardize_curie(df, column=0)
+obo_converter.pd_standardize_uri(df, column=0)
 ```
 
 Apply in bulk to a CSV file with `Converter.file_expand` and
 `Converter.file_compress` (defaults to using tab separator):
 
 ```python
 import curies
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies Version: 0.5.4 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.5.5 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies Classifier:
@@ -62,17 +62,20 @@
 bioregistry_converter = curies.get_bioregistry_converter() # Uses the OBO
 Foundry, a registry of ontologies obo_converter = curies.get_obo_converter() #
 Uses the Monarch Initative's project-specific context monarch_converter =
 curies.get_monarch_converter() ``` ### Bulk Operations Apply in bulk to a
 `pandas.DataFrame` with `Converter.pd_expand` and `Converter.pd_compress`:
 ```python import curies import pandas as pd df = pd.read_csv(...) obo_converter
 = curies.get_obo_converter() obo_converter.pd_compress(df, column=0)
-obo_converter.pd_expand(df, column=0) ``` Apply in bulk to a CSV file with
-`Converter.file_expand` and `Converter.file_compress` (defaults to using tab
-separator): ```python import curies path = ... obo_converter =
+obo_converter.pd_expand(df, column=0) # standardization operations
+obo_converter.pd_standardize_prefix(df, column=0)
+obo_converter.pd_standardize_curie(df, column=0)
+obo_converter.pd_standardize_uri(df, column=0) ``` Apply in bulk to a CSV file
+with `Converter.file_expand` and `Converter.file_compress` (defaults to using
+tab separator): ```python import curies path = ... obo_converter =
 curies.get_obo_converter() # modifies file in place obo_converter.file_compress
 (path, column=0) # modifies file in place obo_converter.file_expand(path,
 column=0) ``` ### CLI Usage This package comes with a built-in CLI for running
 a resolver web application or a IRI mapper web application: ```shell # Run a
 resolver python -m curies resolver --host 0.0.0.0 --port 8764 bioregistry # Run
 a mapper python -m curies mapper --host 0.0.0.0 --port 8764 bioregistry ``` The
 positional argument can be one of the following: 1. A pre-defined prefix map to
```

### Comparing `curies-0.5.4/src/curies.egg-info/SOURCES.txt` & `curies-0.5.5/src/curies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/tests/test_api.py` & `curies-0.5.5/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import pandas as pd
 import rdflib
 from bioregistry.export.prefix_maps import EXTENDED_PREFIX_MAP_PATH
 
-from curies.api import Converter, DuplicatePrefixes, DuplicateURIPrefixes, Record, chain
+from curies.api import (
+    Converter,
+    DuplicatePrefixes,
+    DuplicateURIPrefixes,
+    Record,
+    Reference,
+    ReferenceTuple,
+    chain,
+)
 from curies.sources import (
     BIOREGISTRY_CONTEXTS,
     get_bioregistry_converter,
     get_go_converter,
     get_monarch_converter,
     get_obo_converter,
 )
@@ -32,14 +40,26 @@
             "CHEBI": "http://purl.obolibrary.org/obo/CHEBI_",
             "MONDO": "http://purl.obolibrary.org/obo/MONDO_",
             "GO": "http://purl.obolibrary.org/obo/GO_",
             "OBO": "http://purl.obolibrary.org/obo/",
         }
         self.converter = Converter.from_prefix_map(self.simple_obo_prefix_map)
 
+    def test_reference_tuple(self):
+        """Test the reference tuple data type."""
+        t = ReferenceTuple("chebi", "1234")
+        self.assertEqual("chebi:1234", t.curie)
+        self.assertEqual(t, ReferenceTuple.from_curie("chebi:1234"))
+
+    def test_reference_pydantic(self):
+        """Test the reference Pydantic model."""
+        t = Reference(prefix="chebi", identifier="1234")
+        self.assertEqual("chebi:1234", t.curie)
+        self.assertEqual(t, Reference.from_curie("chebi:1234"))
+
     def test_invalid_record(self):
         """Test throwing an error for invalid records."""
         with self.assertRaises(ValueError):
             Record(
                 prefix="chebi",
                 uri_prefix="http://purl.obolibrary.org/obo/CHEBI_",
                 prefix_synonyms=["chebi"],
@@ -320,14 +340,44 @@
         self.converter.pd_expand(df, "curie")
         self.assertTrue((df.curie == df.uri).all())
 
         df = pd.DataFrame(rows, columns=["curie", "uri"])
         self.converter.pd_compress(df, "uri")
         self.assertTrue((df.curie == df.uri).all())
 
+    def test_df_standardize(self):
+        """Test standardizing dataframes."""
+        converter = Converter([])
+        converter.add_prefix(
+            "chebi",
+            "http://purl.obolibrary.org/obo/CHEBI_",
+            prefix_synonyms=["CHEBI"],
+            uri_prefix_synonyms=["https://bioregistry.io/chebi:"],
+        )
+        self.assertEqual("chebi", converter.standardize_prefix("chebi"))
+        self.assertEqual("chebi", converter.standardize_prefix("CHEBI"))
+        self.assertIsNone(converter.standardize_prefix("nope"))
+
+        rows = [
+            ("chebi", "CHEBI:1", "http://purl.obolibrary.org/obo/CHEBI_1"),
+            ("CHEBI", "CHEBI:2", "https://bioregistry.io/chebi:2"),
+        ]
+        df = pd.DataFrame(rows, columns=["prefix", "curie", "uri"])
+        converter.pd_standardize_prefix(df, column="prefix")
+        self.assertEqual(["chebi", "chebi"], list(df["prefix"]), msg=f"\n\n{df}")
+
+        converter.pd_standardize_curie(df, column="curie")
+        self.assertEqual(["chebi:1", "chebi:2"], list(df["curie"]))
+
+        converter.pd_standardize_uri(df, column="uri")
+        self.assertEqual(
+            ["http://purl.obolibrary.org/obo/CHEBI_1", "http://purl.obolibrary.org/obo/CHEBI_2"],
+            list(df["uri"]),
+        )
+
     def test_file_bulk(self):
         """Test bulk processing of files."""
         with TemporaryDirectory() as directory:
             for rows, header in [
                 (
                     [
                         ("curie", "uri"),
```

### Comparing `curies-0.5.4/tests/test_federated_sparql.py` & `curies-0.5.5/tests/test_federated_sparql.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/tests/test_mapping_service.py` & `curies-0.5.5/tests/test_mapping_service.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.4/tests/test_web.py` & `curies-0.5.5/tests/test_web.py`

 * *Files identical despite different names*

