# Comparing `tmp/python_jsonschema_objects-0.4.1.tar.gz` & `tmp/python_jsonschema_objects-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_jsonschema_objects-0.4.1.tar", last modified: Sat Nov 13 15:35:00 2021, max compression
+gzip compressed data, was "python_jsonschema_objects-0.4.2.tar", last modified: Mon May 15 01:14:48 2023, max compression
```

## Comparing `python_jsonschema_objects-0.4.1.tar` & `python_jsonschema_objects-0.4.2.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 15:35:00.158926 python_jsonschema_objects-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      387 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      769 2021-11-13 15:35:00.158926 python_jsonschema_objects-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13263 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/development.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 15:35:00.146926 python_jsonschema_objects-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    13263 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/docs/Introduction.md
--rw-r--r--   0 runner    (1001) docker     (121)     7724 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/docs/apidoc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10066 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 15:35:00.158926 python_jsonschema_objects-0.4.1/python_jsonschema_objects/
--rw-r--r--   0 runner    (1001) docker     (121)     5656 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2021-11-13 15:35:00.158926 python_jsonschema_objects-0.4.1/python_jsonschema_objects/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    27293 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/classbuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5229 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 15:35:00.150925 python_jsonschema_objects-0.4.1/python_jsonschema_objects/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    13263 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/markdown_support.py
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/pattern_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6181 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4566 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)    11522 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects/wrapper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 15:35:00.150925 python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2021-11-13 15:35:00.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2021-11-13 15:35:00.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-13 15:35:00.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-13 15:35:00.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-11-13 15:35:00.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-11-13 15:35:00.000000 python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/register.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-11-13 15:35:00.158926 python_jsonschema_objects-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2068 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 15:35:00.154926 python_jsonschema_objects-0.4.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 15:35:00.154926 python_jsonschema_objects-0.4.1/test/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/resources/query.json
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/resources/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_array_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_circular_references.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_feature_151.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_feature_177.py
--rw-r--r--   0 runner    (1001) docker     (121)     3101 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_nested_arrays.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_nondefault_resolver_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_pattern_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)    14716 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_pytest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1006 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_114.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_126.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_133.py
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_143.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_156.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_165.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_17.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_185.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_208.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_213.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_214.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_49.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_8.py
--rw-r--r--   0 runner    (1001) docker     (121)      390 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_87.py
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_88.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_89.py
--rw-r--r--   0 runner    (1001) docker     (121)      770 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_regression_90.py
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_util_pytest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/test_wrong_exception_protocolbase_getitem.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/thing-one.json
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/test/thing-two.json
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (121)    62474 2021-11-13 15:34:57.000000 python_jsonschema_objects-0.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:14:48.112312 python_jsonschema_objects-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-15 01:14:48.112312 python_jsonschema_objects-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/development.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:14:48.108312 python_jsonschema_objects-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/docs/Introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/docs/apidoc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:14:48.112312 python_jsonschema_objects-0.4.2/python_jsonschema_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-15 01:14:48.112312 python_jsonschema_objects-0.4.2/python_jsonschema_objects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27287 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/classbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:14:48.108312 python_jsonschema_objects-0.4.2/python_jsonschema_objects/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/markdown_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/pattern_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects/wrapper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:14:48.108312 python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-15 01:14:47.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-15 01:14:47.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:14:47.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:14:47.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 01:14:47.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 01:14:47.000000 python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-15 01:14:48.112312 python_jsonschema_objects-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2068 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:14:48.112312 python_jsonschema_objects-0.4.2/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:14:48.112312 python_jsonschema_objects-0.4.2/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/resources/query.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/resources/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_array_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_circular_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_feature_151.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_feature_177.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_nested_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_nondefault_resolver_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_pattern_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_pytest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_114.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_126.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_133.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_143.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_156.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_165.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_185.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_208.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_214.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_49.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_87.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_88.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_89.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_regression_90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_util_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/test_wrong_exception_protocolbase_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/thing-one.json
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/test/thing-two.json
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    62474 2023-05-15 01:14:41.000000 python_jsonschema_objects-0.4.2/versioneer.py
```

### Comparing `python_jsonschema_objects-0.4.1/LICENSE` & `python_jsonschema_objects-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/PKG-INFO` & `python_jsonschema_objects-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python_jsonschema_objects
-Version: 0.4.1
+Version: 0.4.2
 Summary: An object wrapper for JSON Schema definitions
 Home-page: http://python-jsonschema-objects.readthedocs.org/
 Author: Chris Wacek
 Author-email: cwacek@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `python_jsonschema_objects-0.4.1/README.md` & `python_jsonschema_objects-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/conftest.py` & `python_jsonschema_objects-0.4.2/conftest.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/docs/Introduction.md` & `python_jsonschema_objects-0.4.2/docs/Introduction.md`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/docs/Makefile` & `python_jsonschema_objects-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/docs/conf.py` & `python_jsonschema_objects-0.4.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,26 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"Python JSONSchema Objects"
-copyright = u"2016, Chris Wacek"
-author = u"Chris Wacek"
+project = "Python JSONSchema Objects"
+copyright = "2016, Chris Wacek"
+author = "Chris Wacek"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = u"0.0.18"
+version = "0.0.18"
 # The full version, including alpha/beta/rc tags.
-release = u"0.0.18"
+release = "0.0.18"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
@@ -237,16 +237,16 @@
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
     (
         master_doc,
         "PythonJSONSchemaObjects.tex",
-        u"Python JSONSchema Objects Documentation",
-        u"Chris Wacek",
+        "Python JSONSchema Objects Documentation",
+        "Chris Wacek",
         "manual",
     )
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
@@ -272,15 +272,15 @@
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (
         master_doc,
         "pythonjsonschemaobjects",
-        u"Python JSONSchema Objects Documentation",
+        "Python JSONSchema Objects Documentation",
         [author],
         1,
     )
 ]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
@@ -291,15 +291,15 @@
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
         "PythonJSONSchemaObjects",
-        u"Python JSONSchema Objects Documentation",
+        "Python JSONSchema Objects Documentation",
         author,
         "PythonJSONSchemaObjects",
         "One line description of project.",
         "Miscellaneous",
     )
 ]
```

### Comparing `python_jsonschema_objects-0.4.1/docs/index.rst` & `python_jsonschema_objects-0.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/__init__.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,13 @@
             elif not named_only:
                 classes[name_transform(uri.split("/")[-1])] = klass
 
         return python_jsonschema_objects.util.Namespace.from_mapping(classes)
 
 
 if __name__ == "__main__":
-
     validator = ObjectBuilder("../../protocol/json/schema.json")
 
 from ._version import get_versions
 
 __version__ = get_versions()["version"]
 del get_versions
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/classbuilder.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/classbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,15 +343,14 @@
 
         :return: list of missing properties.
         """
 
         propname = lambda x: self.__prop_names__[x]
         missing = []
         for x in self.__required__:
-
             # Allow the null type
             propinfo = self.propinfo(propname(x))
             null_type = False
             if "type" in propinfo:
                 type_info = propinfo["type"]
                 null_type = (
                     type_info == "null"
@@ -459,15 +458,15 @@
                 pp.append(self.resolve_type(elem["$ref"], source_uri))
             else:
                 pp.append(elem)
 
         return pp
 
     def resolve_type(self, ref, source):
-        """ Return a resolved type for a URI, potentially constructing one if necessary"""
+        """Return a resolved type for a URI, potentially constructing one if necessary"""
         uri = util.resolve_ref_uri(self.resolver.resolution_scope, ref)
         if uri in self.resolved:
             return self.resolved[uri]
 
         elif uri in self.under_construction:
             logger.debug(
                 util.lazy_format(
@@ -484,28 +483,27 @@
                 )
             )
             with self.resolver.resolving(ref) as resolved:
                 self.resolved[uri] = self.construct(uri, resolved, (ProtocolBase,))
                 return self.resolved[uri]
 
     def construct(self, uri, *args, **kw):
-        """ Wrapper to debug things """
+        """Wrapper to debug things"""
         logger.debug(util.lazy_format("Constructing {0}", uri))
         if ("override" not in kw or kw["override"] is False) and uri in self.resolved:
             logger.debug(util.lazy_format("Using existing {0}", uri))
             assert self.resolved[uri] is not None
             return self.resolved[uri]
         else:
             ret = self._construct(uri, *args, **kw)
         logger.debug(util.lazy_format("Constructed {0}", ret))
 
         return ret
 
     def _construct(self, uri, clsdata, parent=(ProtocolBase,), **kw):
-
         if "anyOf" in clsdata:
             raise NotImplementedError("anyOf is not supported as bare property")
 
         elif "oneOf" in clsdata:
             """If this object itself has a 'oneOf' designation,
             then construct a TypeProxy.
             """
@@ -527,15 +525,14 @@
                 elif util.safe_issubclass(p, ProtocolBase):
                     parents.append(p)
 
             self.resolved[uri] = self._build_object(uri, clsdata, parents, **kw)
             return self.resolved[uri]
 
         elif "$ref" in clsdata:
-
             if "type" in clsdata and util.safe_issubclass(
                 clsdata["type"], (ProtocolBase, LiteralValue)
             ):
                 # It's possible that this reference was already resolved, in which
                 # case it will have its type parameter set
                 logger.debug(
                     util.lazy_format(
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/descriptors.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import validators, util, wrapper_types
 from .classbuilder import ProtocolBase, TypeProxy, TypeRef
 
 
 class AttributeDescriptor(object):
-    """ Provides property access for constructed class properties """
+    """Provides property access for constructed class properties"""
 
     def __init__(self, prop, info, desc=""):
         self.prop = prop
         self.info = info
         self.desc = desc
 
     def __doc__(self):
@@ -76,15 +76,21 @@
                         errors.append("Failed to coerce to '{0}': {1}".format(typ, e))
                         pass
                     else:
                         ok = True
                         break
                 elif isinstance(typ, TypeProxy):
                     try:
-                        val = typ(**util.coerce_for_expansion(val))
+                        # handle keyword expansion according to expected types
+                        # using keywords like oneOf, value can be an object, array or literal
+                        val = util.coerce_for_expansion(val)
+                        if isinstance(val, dict):
+                            val = typ(**val)
+                        else:
+                            val = typ(val)
                         val.validate()
                     except Exception as e:
                         errors.append("Failed to coerce to '{0}': {1}".format(typ, e))
                         pass
                     else:
                         ok = True
                         break
@@ -115,15 +121,19 @@
         elif util.safe_issubclass(info["type"], ProtocolBase):
             if not isinstance(val, info["type"]):
                 val = info["type"](**util.coerce_for_expansion(val))
 
             val.validate()
 
         elif isinstance(info["type"], TypeProxy):
-            val = info["type"](val)
+            val = util.coerce_for_expansion(val)
+            if isinstance(val, dict):
+                val = info["type"](**val)
+            else:
+                val = info["type"](val)
 
         elif isinstance(info["type"], TypeRef):
             if not isinstance(val, info["type"].ref_class):
                 val = info["type"](**val)
 
             val.validate()
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/examples/README.md` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/examples/README.md`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/literals.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     )
 
     return klass(value)
 
 
 @functools.total_ordering
 class LiteralValue(object):
-    """Docstring for LiteralValue """
+    """Docstring for LiteralValue"""
 
     isLiteralClass = True
 
     def __init__(self, value, typ=None):
         """@todo: to be defined
 
         :value: @todo
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/markdown_support.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/markdown_support.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import markdown
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 import re
 import json
 
+try:
+    from markdown import __version_info__ as markdown_version_info
+except ImportError:
+    from markdown import version_info as markdown_version_info
+
 
 def extract_code_blocks(filename):
     with open(filename) as fin:
         doc = fin.read().split("\n")
 
     M = markdown.Markdown(extensions=[SpecialFencedCodeExtension()])
 
     preprocessors = M.preprocessors
     tree_processors = M.treeprocessors
 
-    try:
-        version_info = markdown.__version_info__
-    except AttributeError:
-        version_info = markdown.version_info
-
     # Markdown 3.* stores the processors in a class that can be iterated directly.
     # Markdown 2.* stores them in a dict, so we have to pull out the values.
-    if version_info[0] == 2:
+    if markdown_version_info[0] == 2:
         # Note: `markdown.version_info` will be deprecated in favor of
         # `markdown.__version_info__` in later versions of Markdown.
         preprocessors = preprocessors.values()
         tree_processors = tree_processors.values()
 
     for prep in preprocessors:
         doc = prep.run(doc)
@@ -38,18 +38,18 @@
             root = newRoot
 
     return SpecialFencePreprocessor.EXAMPLES
 
 
 class SpecialFencedCodeExtension(Extension):
     def extendMarkdown(self, md, md_globals=None):
-        """ Add FencedBlockPreprocessor to the Markdown instance. """
+        """Add FencedBlockPreprocessor to the Markdown instance."""
         md.registerExtension(self)
 
-        if markdown.version_info[0] >= 3:
+        if markdown_version_info[0] >= 3:
             md.preprocessors.register(
                 SpecialFencePreprocessor(md), "fenced_code_block", 10
             )
         else:
             md.preprocessors.add(
                 "fenced_code_block",
                 SpecialFencePreprocessor(md),
@@ -74,15 +74,14 @@
     def __init__(self, md):
         super(SpecialFencePreprocessor, self).__init__(md)
 
         self.checked_for_codehilite = False
         self.codehilite_conf = {}
 
     def run(self, lines):
-
         text = "\n".join(lines)
 
         while True:
             m = self.FENCED_BLOCK_RE.search(text)
             if m:
                 if m.group("lang"):
                     lang = m.group("lang")
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/pattern_properties.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/pattern_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,22 @@
             return typ(**util.coerce_for_expansion(val))
 
         if util.safe_issubclass(
             typ, python_jsonschema_objects.wrapper_types.ArrayWrapper
         ):
             return typ(val)
 
+        if isinstance(typ, cb.TypeProxy):
+            val = util.coerce_for_expansion(val)
+            if isinstance(val, dict):
+                val = typ(**val)
+            else:
+                val = typ(val)
+            return val
+
         raise validators.ValidationError(
             "additionalProperty type {0} was neither a literal "
             "nor a schema wrapper: {1}".format(typ, val)
         )
 
     def instantiate(self, name, val):
         import python_jsonschema_objects.classbuilder as cb
@@ -83,22 +91,21 @@
             if p.pattern.search(name):
                 logger.debug(
                     "Found patternProperties match: %s %s" % (p.pattern.pattern, name)
                 )
                 return self._make_type(p.schema_type, val)
 
         if self._additional_type is True:
-
             valtype = [
                 k
                 for k, t in validators.SCHEMA_TYPE_MAPPING
                 if t is not None and isinstance(val, t)
             ]
             valtype = valtype[0]
             return MakeLiteral(name, valtype, val)
 
-        elif isinstance(self._additional_type, type):
+        elif isinstance(self._additional_type, (type, cb.TypeProxy)):
             return self._make_type(self._additional_type, val)
 
         raise validators.ValidationError(
             "additionalProperties not permitted " "and no patternProperties specified"
         )
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/util.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                     del props[raw]
             return props
         else:
             return json.JSONEncoder.default(self, obj)
 
 
 def propmerge(into, data_from):
-    """ Merge JSON schema requirements into a dictionary """
+    """Merge JSON schema requirements into a dictionary"""
     newprops = copy.deepcopy(into)
 
     for prop, propval in six.iteritems(data_from):
         if prop not in newprops:
             newprops[prop] = propval
             continue
 
@@ -202,15 +202,14 @@
 
     @staticmethod
     def delattr(ns, name):
         return object.__delattr__(ns, name)
 
 
 def as_namespace(obj, names=None):
-
     # functions
     if isinstance(obj, type(as_namespace)):
         obj = obj()
 
     # special cases
     if isinstance(obj, type):
         names = (name for name in dir(obj) if name not in CLASS_ATTRS)
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/validators.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/validators.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects/wrapper_types.py` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects/wrapper_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,26 +114,24 @@
         if self.strict or self._dirty:
             self.validate_items()
             self.validate_length()
             self.validate_uniqueness()
         return True
 
     def validate_uniqueness(self):
-
         if getattr(self, "uniqueItems", False) is True:
             testset = set(repr(item) for item in self.data)
             if len(testset) != len(self.data):
                 raise ValidationError(
                     "{0} has duplicate elements, but uniqueness required".format(
                         self.data
                     )
                 )
 
     def validate_length(self):
-
         if getattr(self, "minItems", None) is not None:
             if len(self.data) < self.minItems:
                 raise ValidationError(
                     "{1} has too few elements. Wanted {0}.".format(
                         self.minItems, self.data
                     )
                 )
@@ -307,15 +305,15 @@
                     type_array = klassbuilder.construct_objects(
                         item_constraint["oneOf"], uri
                     )
 
                     item_constraint = classbuilder.TypeProxy(type_array)
 
                 elif isdict and item_constraint.get("type") == "object":
-                    """ We need to create a ProtocolBase object for this anonymous definition"""
+                    """We need to create a ProtocolBase object for this anonymous definition"""
                     uri = "{0}_{1}".format(name, "<anonymous_list_type>")
                     item_constraint = klassbuilder.construct(uri, item_constraint)
 
         props["__itemtype__"] = item_constraint
 
         strict = addl_constraints.pop("strict", False)
         props["_strict_"] = strict
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/PKG-INFO` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-jsonschema-objects
-Version: 0.4.1
+Version: 0.4.2
 Summary: An object wrapper for JSON Schema definitions
 Home-page: http://python-jsonschema-objects.readthedocs.org/
 Author: Chris Wacek
 Author-email: cwacek@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `python_jsonschema_objects-0.4.1/python_jsonschema_objects.egg-info/SOURCES.txt` & `python_jsonschema_objects-0.4.2/python_jsonschema_objects.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 test/test_regression_156.py
 test/test_regression_165.py
 test/test_regression_17.py
 test/test_regression_185.py
 test/test_regression_208.py
 test/test_regression_213.py
 test/test_regression_214.py
+test/test_regression_232.py
 test/test_regression_49.py
 test/test_regression_8.py
 test/test_regression_87.py
 test/test_regression_88.py
 test/test_regression_89.py
 test/test_regression_90.py
 test/test_util_pytest.py
```

### Comparing `python_jsonschema_objects-0.4.1/setup.py` & `python_jsonschema_objects-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/resources/query.json` & `python_jsonschema_objects-0.4.2/test/resources/query.json`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/resources/schema.json` & `python_jsonschema_objects-0.4.2/test/resources/schema.json`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_array_validation.py` & `python_jsonschema_objects-0.4.2/test/test_array_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,39 +51,36 @@
     arrayClass.reffed = ["foo"]
 
     with pytest.raises(pjo.ValidationError):
         arrayClass.reffed = []
 
 
 def test_array_length_validates(markdown_examples):
-
     builder = pjo.ObjectBuilder(
         markdown_examples["Example Schema"], resolved=markdown_examples
     )
     ns = builder.build_classes()
 
     with pytest.raises(pjo.ValidationError):
         ns.ExampleSchema(
             firstName="Fred",
             lastName="Huckstable",
             dogs=["Fido", "Spot", "Jasper", "Lady", "Tramp"],
         )
 
 
 def test_minitems(arrayClass):
-
     arrayClass.min = ["1"]
     arrayClass.min.append("2")
 
     with pytest.raises(pjo.ValidationError):
         arrayClass.min = []
 
 
 def test_maxitems(arrayClass):
-
     arrayClass.max = []
     arrayClass.max.append("2")
 
     assert arrayClass.max == ["2"]
 
     with pytest.raises(pjo.ValidationError):
         arrayClass.max.append("3")
@@ -91,15 +88,14 @@
         arrayClass.validate()
 
     with pytest.raises(pjo.ValidationError):
         arrayClass.max = ["45", "42"]
 
 
 def test_unique(arrayClass):
-
     arrayClass.unique = ["hi", "there"]
     with pytest.raises(pjo.ValidationError):
         arrayClass.unique.append("hi")
         # You have to explicitly validate with append
         arrayClass.validate()
 
     with pytest.raises(pjo.ValidationError):
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_circular_references.py` & `python_jsonschema_objects-0.4.2/test/test_circular_references.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest  # noqa
 import python_jsonschema_objects as pjo
 
 
 def test_circular_references(markdown_examples):
-
     builder = pjo.ObjectBuilder(markdown_examples["Circular References"])
     klasses = builder.build_classes()
     a = klasses.A()
     b = klasses.B()
     a.message = "foo"
     b.author = "James Dean"
     a.reference = b
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_default_values.py` & `python_jsonschema_objects-0.4.2/test/test_default_values.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_feature_151.py` & `python_jsonschema_objects-0.4.2/test/test_feature_151.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_feature_177.py` & `python_jsonschema_objects-0.4.2/test/test_feature_177.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 
 import python_jsonschema_objects as pjo
 
 
 @pytest.fixture
 def classes():
-
     schema = {
         "title": "Config",
         "type": "object",
         "additionalProperties": {"$ref": "#/definitions/Parameter"},
         "definitions": {
             "Parameter": {
                 "$id": "Parameter",
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_nested_arrays.py` & `python_jsonschema_objects-0.4.2/test/test_nested_arrays.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 import json
 import logging
 
 
 @pytest.fixture
 def nested_arrays():
     return {
+        "$schema": "http://json-schema.org/draft-04/schema#",
         "title": "example",
         "properties": {
             "foo": {
                 "type": "array",
                 "items": {
                     "type": "array",
+                    # FIXME: not supported anymore in https://json-schema.org/draft/2020-12
                     "items": [{"type": "number"}, {"type": "number"}],
                 },
             }
         },
     }
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_nondefault_resolver_validator.py` & `python_jsonschema_objects-0.4.2/test/test_nondefault_resolver_validator.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_pattern_properties.py` & `python_jsonschema_objects-0.4.2/test/test_pattern_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         # additionalProperties that match
         (True, "foobar", True, False),
         (True, "foobar", "John", True),
         (True, "foobar", 24, True),
     ],
 )
 def test_pattern_properties_work(base_schema, permit_addl, property, value, is_error):
-
     base_schema["additionalProperties"] = permit_addl
 
     builder = pjo.ObjectBuilder(base_schema)
     ns = builder.build_classes()
 
     props = dict([(property, value)])
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_pytest.py` & `python_jsonschema_objects-0.4.2/test/test_pytest.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,14 @@
     return builder.classes["Oneof"]
 
 
 @pytest.mark.parametrize(
     "json_object", ['{"MyData": "an address"}', '{"MyData": "1234"}']
 )
 def test_oneOf_validates_against_any_valid(oneOf, json_object):
-
     oneOf.from_json(json_object)
 
 
 def test_oneOf_fails_against_non_matching(oneOf):
     with pytest.raises(pjs.ValidationError):
         oneOf.from_json('{"MyData": 1234.234}')
 
@@ -239,15 +238,14 @@
 
 
 @pytest.mark.parametrize(
     "json_object",
     ['{"MyAddress": "an address"}', '{"firstName": "John", "lastName": "Winnebago"}'],
 )
 def test_oneOfBare_validates_against_any_valid(oneOfBare, json_object):
-
     oneOfBare.from_json(json_object)
 
 
 def test_oneOfBare_fails_against_non_matching(oneOfBare):
     with pytest.raises(pjs.ValidationError):
         oneOfBare.from_json('{"MyData": 1234.234}')
 
@@ -273,15 +271,14 @@
 
     test = builder.classes["Addlpropsallowed"]()
     test.randomAttribute = 40
     assert int(test.randomAttribute) == 40
 
 
 def test_still_raises_when_accessing_undefined_attrs(Person):
-
     person = Person()
     person.firstName = "James"
 
     # If the attribute doesn't exist, we expect an AttributeError
     with pytest.raises(AttributeError):
         print(person.randomFoo)
 
@@ -302,15 +299,14 @@
     del person["randomthing"]
 
     with pytest.raises(AttributeError):
         assert person.randomthing is None
 
 
 def test_additional_props_disallowed_explicitly(Other):
-
     other = Other()
     with pytest.raises(pjs.ValidationError):
         other.randomAttribute = 4
 
 
 def test_objects_can_be_empty(Person):
     assert Person()
@@ -463,15 +459,14 @@
                 "state": "USA",
             },
             dogs=["Lassie", "Bobo"],
         ),
     ],
 )
 def test_dictionary_transformation(Person, pdict):
-
     person = Person(**pdict)
 
     assert person.as_dict() == pdict
 
 
 def test_strict_mode():
     schema = {
@@ -527,13 +522,12 @@
     ns = builder.build_classes()
 
     x = ns.Test()
     assert x.sample == default["default"]
 
 
 def test_justareference_example(markdown_examples):
-
     builder = pjs.ObjectBuilder(
         markdown_examples["Just a Reference"], resolved=markdown_examples
     )
     ns = builder.build_classes()
     ns.JustAReference("Hello")
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_114.py` & `python_jsonschema_objects-0.4.2/test/test_regression_114.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_126.py` & `python_jsonschema_objects-0.4.2/test/test_regression_126.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_133.py` & `python_jsonschema_objects-0.4.2/test/test_regression_133.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_143.py` & `python_jsonschema_objects-0.4.2/test/test_regression_143.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     print(foo.a)
     assert foo.a == ["foo", "bar"]
     assert validate_items.call_count == 2
 
 
 def test_strict_validation(mocker):
-    """ Validate that when specified as strict, validation still occurs on every change"""
+    """Validate that when specified as strict, validation still occurs on every change"""
     schema = {
         "title": "Example Schema",
         "type": "object",
         "properties": {
             "a": {"type": "array", "items": {"type": "string"}, "default": []}
         },
     }
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_156.py` & `python_jsonschema_objects-0.4.2/test/test_regression_156.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_165.py` & `python_jsonschema_objects-0.4.2/test/test_regression_165.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_17.py` & `python_jsonschema_objects-0.4.2/test/test_regression_17.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_185.py` & `python_jsonschema_objects-0.4.2/test/test_regression_185.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_208.py` & `python_jsonschema_objects-0.4.2/test/test_regression_208.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_213.py` & `python_jsonschema_objects-0.4.2/test/test_regression_213.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_214.py` & `python_jsonschema_objects-0.4.2/test/test_regression_214.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_49.py` & `python_jsonschema_objects-0.4.2/test/test_regression_49.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_8.py` & `python_jsonschema_objects-0.4.2/test/test_regression_8.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_88.py` & `python_jsonschema_objects-0.4.2/test/test_regression_88.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/test_regression_90.py` & `python_jsonschema_objects-0.4.2/test/test_regression_90.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import python_jsonschema_objects as pjs
 
 
 def test_null_type():
-
     schema = {
         "$schema": "http://json-schema.org/draft-04/schema",
         "title": "Example1",
         "type": "object",
         "properties": {"foo": {"type": "null"}},
         "required": ["foo"],
     }
 
     ns1 = pjs.ObjectBuilder(schema).build_classes(strict=True)
     ns1.Example1(foo=None)
 
 
 def test_null_type_one_of():
-
     schema = {
         "$schema": "http://json-schema.org/draft-04/schema",
         "title": "Example1",
         "type": "object",
         "properties": {"foo": {"oneOf": [{"type": "string"}, {"type": "null"}]}},
         "required": ["foo"],
     }
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_util_pytest.py` & `python_jsonschema_objects-0.4.2/test/test_util_pytest.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,29 +57,27 @@
         [{"firstName": "winner", "lastName": "Dinosaur"}, {"firstName": "BadMan"}]
     )
     with pytest.raises(ValidationError):
         instance.validate()
 
 
 def test_validate_arrays_with_mixed_types(Person):
-
     validator = ArrayWrapper.create(
         "test", item_constraint=[Person, {"type": "number"}]
     )
 
     instance = validator([{"firstName": "winner", "lastName": "Dinosaur"}, "fried"])
     with pytest.raises(ValidationError):
         instance.validate()
 
     instance = validator([{"firstName": "winner", "lastName": "Dinosaur"}, 12324])
     instance.validate()
 
 
 def test_validate_arrays_nested():
-
     validator = ArrayWrapper.create(
         "test", item_constraint={"type": "array", "items": {"type": "integer"}}
     )
 
     instance = validator([[1, 2, 4, 5], [1, 2, 4]])
     instance.validate()
```

### Comparing `python_jsonschema_objects-0.4.1/test/test_wrong_exception_protocolbase_getitem.py` & `python_jsonschema_objects-0.4.2/test/test_wrong_exception_protocolbase_getitem.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/thing-one.json` & `python_jsonschema_objects-0.4.2/test/thing-one.json`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/test/thing-two.json` & `python_jsonschema_objects-0.4.2/test/thing-two.json`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.1/tox.ini` & `python_jsonschema_objects-0.4.2/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 
 [tox]
-envlist = py{35,36,37,38}-jsonschema{23,24,25,26,30}-markdown{2,3}
+envlist = py{36,37,38}-jsonschema{23,24,25,26,30}-markdown{2,3}
 skip_missing_interpreters = true
 
 [gh-actions]
 python =
-    3.5: py35
     3.6: py36
     3.7: py37
     3.8: py38
 
 
 [testenv]
 ;install_command = pip install {opts} {packages}
-commands = coverage run {envbindir}/py.test --doctest-glob='python_jsonschema_objects/*.md'  {posargs} 
-           coverage xml --omit=*test* --include=*python_jsonschema_objects*
+commands = python -m coverage run {envbindir}/py.test --doctest-glob='python_jsonschema_objects/*.md'  {posargs}
+           python -m coverage xml --omit="*test*"
 deps =
   coverage
   pytest
   pytest-mock
   jsonschema23: jsonschema~=2.3.0
   jsonschema24: jsonschema~=2.4.0
   jsonschema25: jsonschema~=2.5.0
```

### Comparing `python_jsonschema_objects-0.4.1/versioneer.py` & `python_jsonschema_objects-0.4.2/versioneer.py`

 * *Files identical despite different names*

