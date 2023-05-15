# Comparing `tmp/flask-smorest-0.41.0.tar.gz` & `tmp/flask-smorest-0.42.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-smorest-0.41.0.tar", last modified: Thu Mar 30 07:56:20 2023, max compression
+gzip compressed data, was "flask-smorest-0.42.0.tar", last modified: Mon May 15 08:16:58 2023, max compression
```

## Comparing `flask-smorest-0.41.0.tar` & `flask-smorest-0.42.0.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:20.826478 flask-smorest-0.41.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30685 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-30 07:56:20.826478 flask-smorest-0.41.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:20.822477 flask-smorest-0.41.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:20.822477 flask-smorest-0.41.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/_templates/donate.html
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/etag.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/pagination.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/docs/response.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:20.822477 flask-smorest-0.41.0/flask_smorest/
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/etag.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:20.822477 flask-smorest-0.41.0/flask_smorest/spec/
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/spec/field_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/spec/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:20.822477 flask-smorest-0.41.0/flask_smorest/spec/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/spec/templates/rapidoc.html
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/spec/templates/redoc.html
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/spec/templates/swagger_ui.html
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/flask_smorest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:20.822477 flask-smorest-0.41.0/flask_smorest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-30 07:56:20.000000 flask-smorest-0.41.0/flask_smorest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-30 07:56:20.000000 flask-smorest-0.41.0/flask_smorest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 07:56:20.000000 flask-smorest-0.41.0/flask_smorest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-30 07:56:20.000000 flask-smorest-0.41.0/flask_smorest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 07:56:20.000000 flask-smorest-0.41.0/flask_smorest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-30 07:56:20.826478 flask-smorest-0.41.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:20.826478 flask-smorest-0.41.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_etag.py
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    19493 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-30 07:56:14.000000 flask-smorest-0.41.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:58.091291 flask-smorest-0.42.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    31184 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-15 08:16:58.091291 flask-smorest-0.42.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:58.087290 flask-smorest-0.42.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:58.087290 flask-smorest-0.42.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/_templates/donate.html
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/etag.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/pagination.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/docs/response.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:58.087290 flask-smorest-0.42.0/flask_smorest/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/etag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:58.087290 flask-smorest-0.42.0/flask_smorest/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/spec/field_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/spec/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:58.087290 flask-smorest-0.42.0/flask_smorest/spec/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/spec/templates/rapidoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/spec/templates/redoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/spec/templates/swagger_ui.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/flask_smorest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:58.087290 flask-smorest-0.42.0/flask_smorest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-15 08:16:58.000000 flask-smorest-0.42.0/flask_smorest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-15 08:16:58.000000 flask-smorest-0.42.0/flask_smorest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:16:58.000000 flask-smorest-0.42.0/flask_smorest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-15 08:16:58.000000 flask-smorest-0.42.0/flask_smorest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 08:16:58.000000 flask-smorest-0.42.0/flask_smorest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-15 08:16:58.091291 flask-smorest-0.42.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:58.091291 flask-smorest-0.42.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18330 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24163 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_etag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19493 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25404 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-15 08:16:48.000000 flask-smorest-0.42.0/tox.ini
```

### Comparing `flask-smorest-0.41.0/AUTHORS.rst` & `flask-smorest-0.42.0/AUTHORS.rst`

 * *Files 15% similar despite different names*

```diff
@@ -21,7 +21,8 @@
 - Martijn Pieters `@mjpieters <https://github.com/mjpieters>`_
 - Stephen Rosen `@sirosen <https://github.com/sirosen>`_
 - Grey Li `@greyli <https://github.com/greyli>`_
 - Tim Diekmann `@TimDiekmann <https://github.com/TimDiekmann>`_
 - Choudhury Noor `@Cnoor0171 <https://github.com/Cnoor0171>`_
 - Dmitry Erlikh `@derlikh-smart <https://github.com/derlikh-smart>`_
 - 0x78f1935 `@0x78f1935 <https://github.com/0x78f1935>`_
+- One Codex, Inc. `@onecodex <https://github.com/onecodex>`_
```

### Comparing `flask-smorest-0.41.0/CHANGELOG.rst` & `flask-smorest-0.42.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Changelog
 ---------
 
+0.42.0 (2023-05-15)
+*******************
+
+Features:
+
+- *Backwards-incompatible*: Support multiple APIs in a single application via
+  ``Api`` param ``config_prefix``. The ``Api`` object is now accessible at
+  ``app.extensions["flask-smorest"]["apis"][config_prefix]["ext_obj"]``
+  rather than ``app.extensions["flask-smorest"]["ext_obj"]``. (:pr:`485`)
+  Thanks :user:`petraszd` for the contribution.
+
+Other changes:
+
+- Drop support for Python 3.7 (:pr:`497`).
+- Require Werkzeug>=2.0.1 (:pr:`485`).
+
 0.41.0 (2023-03-30)
 *******************
 
 Features:
 
 - Allow multiple responses with same status code and different content types
   (:pr:`481`).
```

### Comparing `flask-smorest-0.41.0/CONTRIBUTING.rst` & `flask-smorest-0.42.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/LICENSE` & `flask-smorest-0.42.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/PKG-INFO` & `flask-smorest-0.42.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: flask-smorest
-Version: 0.41.0
+Version: 0.42.0
 Summary: Flask/Marshmallow-based REST API framework
 Home-page: https://github.com/marshmallow-code/flask-smorest
 Author: Jérôme Lafréchoux
 Author-email: jerome@jolimont.fr
 License: MIT
 Keywords: REST,openapi,swagger,flask,marshmallow,apispec,webargs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: lint
 Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
```

### Comparing `flask-smorest-0.41.0/README.rst` & `flask-smorest-0.42.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/Makefile` & `flask-smorest-0.42.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/api_reference.rst` & `flask-smorest-0.42.0/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/arguments.rst` & `flask-smorest-0.42.0/docs/arguments.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/conf.py` & `flask-smorest-0.42.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/etag.rst` & `flask-smorest-0.42.0/docs/etag.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/index.rst` & `flask-smorest-0.42.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     quickstart
     arguments 
     response
     pagination
     etag
     openapi
+    advanced
 
 
 API Reference
 =============
 
 .. toctree::
     :maxdepth: 2
```

### Comparing `flask-smorest-0.41.0/docs/make.bat` & `flask-smorest-0.42.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/openapi.rst` & `flask-smorest-0.42.0/docs/openapi.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/pagination.rst` & `flask-smorest-0.42.0/docs/pagination.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/quickstart.rst` & `flask-smorest-0.42.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/docs/response.rst` & `flask-smorest-0.42.0/docs/response.rst`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/flask_smorest/__init__.py` & `flask-smorest-0.42.0/flask_smorest/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 from webargs.flaskparser import abort  # noqa
 
 from .spec import APISpecMixin
 from .blueprint import Blueprint  # noqa
 from .pagination import Page  # noqa
 from .error_handler import ErrorHandlerMixin
+from .globals import current_api  # noqa
+from .utils import PrefixedMappingProxy, normalize_config_prefix
 
-__version__ = "0.41.0"
+__version__ = "0.42.0"
 
 
 class Api(APISpecMixin, ErrorHandlerMixin):
     """Main class
 
     Provides helpers to build a REST API using Flask.
 
     :param Flask app: Flask application
     :param spec_kwargs: kwargs to pass to internal APISpec instance
+    :param str config_prefix: Prefix to Api parameters in application config
 
     The ``spec_kwargs`` dictionary is passed as kwargs to the internal APISpec
     instance. **flask-smorest** adds a few parameters to the original
     parameters documented in :class:`apispec.APISpec <apispec.APISpec>`:
 
     :param apispec.BasePlugin flask_plugin: Flask plugin
     :param apispec.BasePlugin marshmallow_plugin: Marshmallow plugin
@@ -35,36 +38,47 @@
 
     This allows the user to override default Flask and marshmallow plugins.
 
     For more flexibility, additional spec kwargs can also be passed as app
     parameter `API_SPEC_OPTIONS`.
     """
 
-    def __init__(self, app=None, *, spec_kwargs=None):
+    def __init__(self, app=None, *, spec_kwargs=None, config_prefix=""):
         self._app = app
         self._spec_kwargs = spec_kwargs or {}
+        self.config_prefix = normalize_config_prefix(config_prefix)
+        self.config = None
         self.spec = None
         # Use lists to enforce order
         self._fields = []
         self._converters = []
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app, *, spec_kwargs=None):
         """Initialize Api with application
 
         :param spec_kwargs: kwargs to pass to internal APISpec instance.
             Updates ``spec_kwargs`` passed in ``Api`` init.
         """
         self._app = app
+        self.config = PrefixedMappingProxy(app.config, self.config_prefix)
 
         # Register flask-smorest in app extensions
         app.extensions = getattr(app, "extensions", {})
-        ext = app.extensions.setdefault("flask-smorest", {})
-        ext["ext_obj"] = self
+        ext = app.extensions.setdefault(
+            "flask-smorest",
+            {
+                # Config prefix -> {"ext_obj": Api instance}
+                "apis": {},
+                # Blueprint name -> Api instance
+                "blp_name_to_api": {},
+            },
+        )
+        ext["apis"][self.config_prefix] = {"ext_obj": self}
 
         # Initialize spec
         self._init_spec(**{**self._spec_kwargs, **(spec_kwargs or {})})
 
         # Initialize blueprint serving spec
         self._register_doc_blueprint()
 
@@ -82,14 +96,16 @@
         :param options: Keyword arguments overriding
             :class:`Blueprint <flask.Blueprint>` defaults
 
         Must be called after app is initialized.
         """
         blp_name = options.get("name", blp.name)
 
+        self._app.extensions["flask-smorest"]["blp_name_to_api"][blp_name] = self
+
         self._app.register_blueprint(blp, **options)
 
         # Register views in API documentation for this resource
         blp.register_views_in_doc(
             self,
             self._app,
             self.spec,
```

### Comparing `flask-smorest-0.41.0/flask_smorest/arguments.py` & `flask-smorest-0.42.0/flask_smorest/arguments.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/flask_smorest/blueprint.py` & `flask-smorest-0.42.0/flask_smorest/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/flask_smorest/error_handler.py` & `flask-smorest-0.42.0/flask_smorest/error_handler.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/flask_smorest/etag.py` & `flask-smorest-0.42.0/flask_smorest/etag.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from copy import deepcopy
 import json
 import http
 import warnings
 
 import hashlib
 
-from flask import request, current_app
+from flask import request
 
 from .exceptions import PreconditionRequired, PreconditionFailed, NotModified
 from .utils import deepupdate, resolve_schema_instance, get_appcontext
+from .globals import current_api
 
 
 IF_NONE_MATCH_HEADER = {
     "name": "If-None-Match",
     "in": "header",
     "description": "Tag to check against",
     "schema": {"type": "string"},
@@ -31,19 +32,14 @@
 
 ETAG_HEADER = {
     "description": "Tag for the returned entry",
     "schema": {"type": "string"},
 }
 
 
-def _is_etag_enabled():
-    """Return True if ETag feature enabled application-wise"""
-    return not current_app.config.get("ETAG_DISABLED", False)
-
-
 def _get_etag_ctx():
     """Get ETag section of AppContext"""
     return get_appcontext().setdefault("etag", {})
 
 
 class EtagMixin:
     """Extend Blueprint to add ETag handling"""
@@ -68,15 +64,15 @@
 
         See :doc:`ETag <etag>`.
         """
 
         def decorator(func):
             @wraps(func)
             def wrapper(*args, **kwargs):
-                etag_enabled = _is_etag_enabled()
+                etag_enabled = self._is_etag_enabled()
 
                 if etag_enabled:
                     # Check etag precondition
                     self._check_precondition()
 
                 # Execute decorated function
                 resp = func(*args, **kwargs)
@@ -140,22 +136,26 @@
         DELETE.
         """
         if request.method not in self.METHODS_NEEDING_CHECK_ETAG:
             warnings.warn(
                 f"ETag cannot be checked on {request.method} request.",
                 stacklevel=2,
             )
-        if _is_etag_enabled():
+        if self._is_etag_enabled():
             if etag_schema is not None:
                 etag_data = resolve_schema_instance(etag_schema).dump(etag_data)
             new_etag = self._generate_etag(etag_data)
             _get_etag_ctx()["etag_checked"] = True
             if new_etag not in request.if_match:
                 raise PreconditionFailed
 
+    def _is_etag_enabled(self):
+        """Return True if ETag feature is enabled api-wise"""
+        return not current_api.config.get("ETAG_DISABLED", False)
+
     def _verify_check_etag(self):
         """Verify check_etag was called in resource code
 
         Issues a warning if ETag is enabled but check_etag was not called in
         resource code in a PUT, PATCH or DELETE method.
 
         This is called automatically. It is meant to warn the developer about
@@ -193,15 +193,15 @@
         or PATCH.
         """
         if request.method not in self.METHODS_ALLOWING_SET_ETAG:
             warnings.warn(
                 f"ETag cannot be set on {request.method} request.",
                 stacklevel=2,
             )
-        if _is_etag_enabled():
+        if self._is_etag_enabled():
             if etag_schema is not None:
                 etag_data = resolve_schema_instance(etag_schema).dump(etag_data)
             new_etag = self._generate_etag(etag_data)
             self._check_not_modified(new_etag)
             # Store ETag in AppContext to add it to response headers later on
             _get_etag_ctx()["etag"] = new_etag
 
@@ -223,16 +223,16 @@
                     for k, v in response.headers
                     if k in self.ETAG_INCLUDE_HEADERS
                 )
                 new_etag = self._generate_etag(etag_data, extra_data)
                 self._check_not_modified(new_etag)
             response.set_etag(new_etag)
 
-    def _prepare_etag_doc(self, doc, doc_info, *, app, spec, method, **kwargs):
-        if doc_info.get("etag", False) and not app.config.get("ETAG_DISABLED", False):
+    def _prepare_etag_doc(self, doc, doc_info, *, api, spec, method, **kwargs):
+        if doc_info.get("etag", False) and not api.config.get("ETAG_DISABLED", False):
             responses = {}
             method_u = method.upper()
             if method_u in self.METHODS_CHECKING_NOT_MODIFIED:
                 responses[304] = http.HTTPStatus(304).name
                 doc.setdefault("parameters", []).append("IF_NONE_MATCH")
             if method_u in self.METHODS_NEEDING_CHECK_ETAG:
                 responses[412] = http.HTTPStatus(412).name
```

### Comparing `flask-smorest-0.41.0/flask_smorest/exceptions.py` & `flask-smorest-0.42.0/flask_smorest/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,7 +26,11 @@
 
     # Overriding description as we don't provide If-Unmodified-Since
     description = 'This request is required to be conditional; try using "If-Match".'
 
 
 class PreconditionFailed(wexc.PreconditionFailed, FlaskSmorestError):
     """Etag required and wrong ETag provided"""
+
+
+class CurrentApiNotAvailableError(FlaskSmorestError):
+    """`current_api` not available"""
```

### Comparing `flask-smorest-0.41.0/flask_smorest/pagination.py` & `flask-smorest-0.42.0/flask_smorest/pagination.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/flask_smorest/response.py` & `flask-smorest-0.42.0/flask_smorest/response.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/flask_smorest/spec/__init__.py` & `flask-smorest-0.42.0/flask_smorest/spec/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     import yaml
 
     HAS_PYYAML = True
 except ImportError:  # pragma: no cover
     HAS_PYYAML = False
 
 from flask_smorest.exceptions import MissingAPIParameterError
-from flask_smorest.utils import prepare_response
+from flask_smorest.utils import prepare_response, normalize_config_prefix
 from flask_smorest import etag as fs_etag
 from flask_smorest import pagination as fs_pagination
 from .plugins import FlaskPlugin
 from .field_converters import uploadfield2properties
 
 
 def _add_leading_slash(string):
@@ -40,31 +40,34 @@
             ret["style"] = "form"
     return ret
 
 
 class DocBlueprintMixin:
     """Extend Api to serve the spec in a dedicated blueprint."""
 
+    def _make_doc_blueprint_name(self):
+        return f"{self.config_prefix}api-docs".replace("_", "-").lower()
+
     def _register_doc_blueprint(self):
         """Register a blueprint in the application to expose the spec
 
         Doc Blueprint contains routes to
         - json spec file
         - spec UI (ReDoc, Swagger UI).
         """
-        api_url = self._app.config.get("OPENAPI_URL_PREFIX", None)
+        api_url = self.config.get("OPENAPI_URL_PREFIX")
         if api_url is not None:
             blueprint = flask.Blueprint(
-                "api-docs",
+                self._make_doc_blueprint_name(),
                 __name__,
                 url_prefix=_add_leading_slash(api_url),
                 template_folder="./templates",
             )
             # Serve json spec at 'url_prefix/openapi.json' by default
-            json_path = self._app.config.get("OPENAPI_JSON_PATH", "openapi.json")
+            json_path = self.config.get("OPENAPI_JSON_PATH", "openapi.json")
             blueprint.add_url_rule(
                 _add_leading_slash(json_path),
                 endpoint="openapi_json",
                 view_func=self._openapi_json,
             )
             self._register_redoc_rule(blueprint)
             self._register_swagger_ui_rule(blueprint)
@@ -72,50 +75,50 @@
             self._app.register_blueprint(blueprint)
 
     def _register_redoc_rule(self, blueprint):
         """Register ReDoc rule
 
         The ReDoc script URL should be specified as OPENAPI_REDOC_URL.
         """
-        redoc_path = self._app.config.get("OPENAPI_REDOC_PATH")
+        redoc_path = self.config.get("OPENAPI_REDOC_PATH")
         if redoc_path is not None:
-            redoc_url = self._app.config.get("OPENAPI_REDOC_URL")
+            redoc_url = self.config.get("OPENAPI_REDOC_URL")
             if redoc_url is not None:
                 self._redoc_url = redoc_url
                 blueprint.add_url_rule(
                     _add_leading_slash(redoc_path),
                     endpoint="openapi_redoc",
                     view_func=self._openapi_redoc,
                 )
 
     def _register_swagger_ui_rule(self, blueprint):
         """Register Swagger UI rule
 
         The Swagger UI scripts base URL should be specified as
         OPENAPI_SWAGGER_UI_URL.
         """
-        swagger_ui_path = self._app.config.get("OPENAPI_SWAGGER_UI_PATH")
+        swagger_ui_path = self.config.get("OPENAPI_SWAGGER_UI_PATH")
         if swagger_ui_path is not None:
-            swagger_ui_url = self._app.config.get("OPENAPI_SWAGGER_UI_URL")
+            swagger_ui_url = self.config.get("OPENAPI_SWAGGER_UI_URL")
             if swagger_ui_url is not None:
                 self._swagger_ui_url = swagger_ui_url
                 blueprint.add_url_rule(
                     _add_leading_slash(swagger_ui_path),
                     endpoint="openapi_swagger_ui",
                     view_func=self._openapi_swagger_ui,
                 )
 
     def _register_rapidoc_rule(self, blueprint):
         """Register RapiDoc rule
 
         The RapiDoc script URL should be specified as OPENAPI_RAPIDOC_URL.
         """
-        rapidoc_path = self._app.config.get("OPENAPI_RAPIDOC_PATH")
+        rapidoc_path = self.config.get("OPENAPI_RAPIDOC_PATH")
         if rapidoc_path is not None:
-            rapidoc_url = self._app.config.get("OPENAPI_RAPIDOC_URL")
+            rapidoc_url = self.config.get("OPENAPI_RAPIDOC_URL")
             if rapidoc_url is not None:
                 self._rapidoc_url = rapidoc_url
                 blueprint.add_url_rule(
                     _add_leading_slash(rapidoc_path),
                     endpoint="openapi_rapidoc",
                     view_func=self._openapi_rapidoc,
                 )
@@ -127,33 +130,38 @@
         return current_app.response_class(
             json.dumps(self.spec.to_dict(), indent=2), mimetype="application/json"
         )
 
     def _openapi_redoc(self):
         """Expose OpenAPI spec with ReDoc"""
         return flask.render_template(
-            "redoc.html", title=self.spec.title, redoc_url=self._redoc_url
+            "redoc.html",
+            spec_url=flask.url_for(f"{self._make_doc_blueprint_name()}.openapi_json"),
+            title=self.spec.title,
+            redoc_url=self._redoc_url,
         )
 
     def _openapi_swagger_ui(self):
         """Expose OpenAPI spec with Swagger UI"""
         return flask.render_template(
             "swagger_ui.html",
             title=self.spec.title,
+            spec_url=flask.url_for(f"{self._make_doc_blueprint_name()}.openapi_json"),
             swagger_ui_url=self._swagger_ui_url,
-            swagger_ui_config=self._app.config.get("OPENAPI_SWAGGER_UI_CONFIG", {}),
+            swagger_ui_config=self.config.get("OPENAPI_SWAGGER_UI_CONFIG", {}),
         )
 
     def _openapi_rapidoc(self):
         """Expose OpenAPI spec with RapiDoc"""
         return flask.render_template(
             "rapidoc.html",
             title=self.spec.title,
+            spec_url=flask.url_for(f"{self._make_doc_blueprint_name()}.openapi_json"),
             rapidoc_url=self._rapidoc_url,
-            rapidoc_config=self._app.config.get("OPENAPI_RAPIDOC_CONFIG", {}),
+            rapidoc_config=self.config.get("OPENAPI_RAPIDOC_CONFIG", {}),
         )
 
 
 class APISpecMixin(DocBlueprintMixin):
     """Add APISpec related features to Api class"""
 
     DEFAULT_ERROR_RESPONSE_NAME = "DEFAULT_ERROR"
@@ -166,39 +174,42 @@
         *,
         flask_plugin=None,
         marshmallow_plugin=None,
         extra_plugins=None,
         title=None,
         version=None,
         openapi_version=None,
-        **options
+        **options,
     ):
         # Plugins
         self.flask_plugin = flask_plugin or FlaskPlugin()
         self.ma_plugin = marshmallow_plugin or MarshmallowPlugin()
         plugins = [self.flask_plugin, self.ma_plugin]
         plugins.extend(extra_plugins or ())
 
         # APISpec options
-        title = self._app.config.get("API_TITLE", title)
+        title = self.config.get("API_TITLE", title)
         if title is None:
+            key = f"{self.config_prefix}API_TITLE"
             raise MissingAPIParameterError(
-                'API title must be specified either as "API_TITLE" '
+                f'API title must be specified either as "{key}" '
                 'app parameter or as "title" spec kwarg.'
             )
-        version = self._app.config.get("API_VERSION", version)
+        version = self.config.get("API_VERSION", version)
         if version is None:
+            key = f"{self.config_prefix}API_VERSION"
             raise MissingAPIParameterError(
-                'API version must be specified either as "API_VERSION" '
+                f'API version must be specified either as "{key}" '
                 'app parameter or as "version" spec kwarg.'
             )
-        openapi_version = self._app.config.get("OPENAPI_VERSION", openapi_version)
+        openapi_version = self.config.get("OPENAPI_VERSION", openapi_version)
         if openapi_version is None:
+            key = f"{self.config_prefix}OPENAPI_VERSION"
             raise MissingAPIParameterError(
-                'OpenAPI version must be specified either as "OPENAPI_VERSION '
+                f'OpenAPI version must be specified either as "{key}" '
                 'app parameter or as "openapi_version" spec kwarg.'
             )
         openapi_major_version = int(openapi_version.split(".")[0])
         if openapi_major_version < 3:
             options.setdefault(
                 "produces",
                 [
@@ -207,15 +218,15 @@
             )
             options.setdefault(
                 "consumes",
                 [
                     self.DEFAULT_REQUEST_BODY_CONTENT_TYPE,
                 ],
             )
-        options.update(self._app.config.get("API_SPEC_OPTIONS", {}))
+        options.update(self.config.get("API_SPEC_OPTIONS", {}))
 
         # Instantiate spec
         self.spec = apispec.APISpec(
             title,
             version,
             openapi_version,
             plugins,
@@ -358,40 +369,65 @@
                 "PAGINATION", fs_pagination.PAGINATION_HEADER, lazy=True
             )
 
 
 openapi_cli = flask.cli.AppGroup("openapi", help="OpenAPI commands.")
 
 
-def _get_spec_dict():
-    return current_app.extensions["flask-smorest"]["ext_obj"].spec.to_dict()
+def _get_spec_dict(config_prefix):
+    apis = current_app.extensions["flask-smorest"]["apis"]
+    try:
+        api = apis[config_prefix]["ext_obj"]
+    except KeyError:
+        click.echo(
+            f'Error: config prefix "{config_prefix}" not available. Use one of:',
+            err=True,
+        )
+        for key in apis.keys():
+            click.echo(f'    "{key}"', err=True)
+        raise click.exceptions.Exit() from KeyError
+    return api.spec.to_dict()
 
 
 @openapi_cli.command("print")
 @click.option("-f", "--format", type=click.Choice(["json", "yaml"]), default="json")
-def print_openapi_doc(format):
+@click.option("--config-prefix", type=click.STRING, metavar="", default="")
+def print_openapi_doc(format, config_prefix):
     """Print OpenAPI JSON document."""
+    config_prefix = normalize_config_prefix(config_prefix)
     if format == "json":
-        click.echo(json.dumps(_get_spec_dict(), indent=2))
+        click.echo(json.dumps(_get_spec_dict(config_prefix), indent=2))
     else:  # format == "yaml"
         if HAS_PYYAML:
-            click.echo(yaml.dump(_get_spec_dict()))
+            click.echo(yaml.dump(_get_spec_dict(config_prefix)))
         else:
             click.echo(
                 "To use yaml output format, please install PyYAML module", err=True
             )
 
 
 @openapi_cli.command("write")
 @click.option("-f", "--format", type=click.Choice(["json", "yaml"]), default="json")
+@click.option("--config-prefix", type=click.STRING, metavar="", default="")
 @click.argument("output_file", type=click.File(mode="w"))
-def write_openapi_doc(format, output_file):
+def write_openapi_doc(format, output_file, config_prefix):
     """Write OpenAPI JSON document to a file."""
+    config_prefix = normalize_config_prefix(config_prefix)
     if format == "json":
-        click.echo(json.dumps(_get_spec_dict(), indent=2), file=output_file)
+        click.echo(
+            json.dumps(_get_spec_dict(config_prefix), indent=2),
+            file=output_file,
+        )
     else:  # format == "yaml"
         if HAS_PYYAML:
-            yaml.dump(_get_spec_dict(), output_file)
+            yaml.dump(_get_spec_dict(config_prefix), output_file)
         else:
             click.echo(
                 "To use yaml output format, please install PyYAML module", err=True
             )
+
+
+@openapi_cli.command("list-config-prefixes")
+def list_config_prefixes():
+    """List available API config prefixes."""
+    for prefix in current_app.extensions["flask-smorest"]["apis"].keys():
+        click.echo(f'"{prefix}"')
```

### Comparing `flask-smorest-0.41.0/flask_smorest/spec/plugins.py` & `flask-smorest-0.42.0/flask_smorest/spec/plugins.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/flask_smorest/spec/templates/swagger_ui.html` & `flask-smorest-0.42.0/flask_smorest/spec/templates/swagger_ui.html`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
    <div id="swagger-ui-container"></div>
 
    <script src="{{swagger_ui_url}}swagger-ui-standalone-preset.js"></script>
    <script src="{{swagger_ui_url}}swagger-ui-bundle.js"></script>
    <script>
 
      config = {
-       url: "{{ url_for('api-docs.openapi_json') }}",
+       url: "{{ spec_url }}",
        dom_id: '#swagger-ui-container'
      }
 
      var override_config = {{ swagger_ui_config | tojson }};
      for (var attrname in override_config) { config[attrname] = override_config[attrname]; }
 
      window.onload = function() {
```

### Comparing `flask-smorest-0.41.0/flask_smorest/utils.py` & `flask-smorest-0.42.0/flask_smorest/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -133,7 +133,47 @@
         for field in ("schema", "example", "examples"):
             if field in response:
                 (
                     response.setdefault("content", {}).setdefault(content_type, {})[
                         field
                     ]
                 ) = response.pop(field)
+
+
+def normalize_config_prefix(config_prefix):
+    """Normalize API config prefix
+
+    Sets upper case and appends underscore if missing.
+
+    :param str config_prefix: Raw prefix
+
+    :return: Normalized prefix
+    """
+    result = config_prefix.strip().upper()
+    if result and not result.endswith("_"):
+        result += "_"
+    return result
+
+
+class PrefixedMappingProxy(abc.Mapping):
+    """Mapping to proxy another mapping using a prefix
+
+    .. code-block:: python
+        some_dict = PrefixedMappingProxy(
+            proxied_dict={"foobar_key1": 1, "foobar_key2": 2}, prefix="foobar_"
+        )
+        assert some_dict["key1"] == 1
+        assert some_dict["key2"] == 2
+    """
+
+    def __init__(self, proxied_dict, prefix):
+        self._dict = proxied_dict
+        self.prefix = prefix
+
+    def __getitem__(self, key):
+        return self._dict[self.prefix + str(key)]
+
+    def __iter__(self):
+        return iter(x for x in self._dict if x.startswith(self.prefix))
+
+    def __len__(self):
+        return sum(1 for _ in iter(self))
```

### Comparing `flask-smorest-0.41.0/flask_smorest.egg-info/PKG-INFO` & `flask-smorest-0.42.0/flask_smorest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: flask-smorest
-Version: 0.41.0
+Version: 0.42.0
 Summary: Flask/Marshmallow-based REST API framework
 Home-page: https://github.com/marshmallow-code/flask-smorest
 Author: Jérôme Lafréchoux
 Author-email: jerome@jolimont.fr
 License: MIT
 Keywords: REST,openapi,swagger,flask,marshmallow,apispec,webargs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: lint
 Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
```

### Comparing `flask-smorest-0.41.0/flask_smorest.egg-info/SOURCES.txt` & `flask-smorest-0.42.0/flask_smorest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
+docs/advanced.rst
 docs/api_reference.rst
 docs/arguments.rst
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/etag.rst
 docs/index.rst
@@ -26,14 +27,15 @@
 flask_smorest/__init__.py
 flask_smorest/arguments.py
 flask_smorest/blueprint.py
 flask_smorest/error_handler.py
 flask_smorest/etag.py
 flask_smorest/exceptions.py
 flask_smorest/fields.py
+flask_smorest/globals.py
 flask_smorest/pagination.py
 flask_smorest/response.py
 flask_smorest/utils.py
 flask_smorest.egg-info/PKG-INFO
 flask_smorest.egg-info/SOURCES.txt
 flask_smorest.egg-info/dependency_links.txt
 flask_smorest.egg-info/requires.txt
```

### Comparing `flask-smorest-0.41.0/flask_smorest.egg-info/requires.txt` & `flask-smorest-0.42.0/flask_smorest.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 apispec[marshmallow]<7,>=6.0.0
 flask<3,>=2.0
 marshmallow<4,>=3.18.0
 webargs<9,>=8.0.0
-werkzeug<3,>=2.0
+werkzeug<3,>=2.0.1
 
 [dev]
 PyYAML==6.0
 apispec==6.3.0
-coverage==7.2.2
-flake8-bugbear==23.3.23
+coverage==7.2.5
+flake8-bugbear==23.5.9
 flake8==6.0.0
-flask==2.2.3
+flask==2.3.2
 marshmallow==3.19.0
-pre-commit==3.2.1
+pre-commit==3.3.1
 pytest-cov==4.0.0
-pytest==7.2.2
+pytest==7.3.1
 webargs==8.2.0
-werkzeug==2.2.3
+werkzeug==2.3.4
 
 [lint]
-flake8-bugbear==23.3.23
+flake8-bugbear==23.5.9
 flake8==6.0.0
-pre-commit==3.2.1
+pre-commit==3.3.1
 
 [tests]
 PyYAML==6.0
 apispec==6.3.0
-coverage==7.2.2
-flask==2.2.3
+coverage==7.2.5
+flask==2.3.2
 marshmallow==3.19.0
 pytest-cov==4.0.0
-pytest==7.2.2
+pytest==7.3.1
 webargs==8.2.0
-werkzeug==2.2.3
+werkzeug==2.3.4
```

### Comparing `flask-smorest-0.41.0/setup.py` & `flask-smorest-0.42.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 EXTRAS_REQUIRE = {
     "tests": [
-        "pytest==7.2.2",
+        "pytest==7.3.1",
         "pytest-cov==4.0.0",
-        "coverage==7.2.2",
-        "werkzeug==2.2.3",
-        "flask==2.2.3",
+        "coverage==7.2.5",
+        "werkzeug==2.3.4",
+        "flask==2.3.2",
         "marshmallow==3.19.0",
         "webargs==8.2.0",
         "apispec==6.3.0",
         "PyYAML==6.0",
     ],
     "lint": [
         "flake8==6.0.0",
-        "flake8-bugbear==23.3.23",
-        "pre-commit==3.2.1",
+        "flake8-bugbear==23.5.9",
+        "pre-commit==3.3.1",
     ],
 }
 EXTRAS_REQUIRE["dev"] = EXTRAS_REQUIRE["tests"] + EXTRAS_REQUIRE["lint"]
 
 
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="flask-smorest",
-    version="0.41.0",
+    version="0.42.0",
     description="Flask/Marshmallow-based REST API framework",
     long_description=long_description,
     url="https://github.com/marshmallow-code/flask-smorest",
     author="Jérôme Lafréchoux",
     author_email="jerome@jolimont.fr",
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP",
         "Environment :: Web Environment",
         "Framework :: Flask",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=[
@@ -61,17 +60,17 @@
         "webargs",
     ],
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     package_data={
         "": ["spec/templates/*"],
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
-        "werkzeug>=2.0,<3",
+        "werkzeug>=2.0.1,<3",
         "flask>=2.0,<3",
         "marshmallow>=3.18.0,<4",
         "webargs>=8.0.0,<9",
         "apispec[marshmallow]>=6.0.0,<7",
     ],
     extras_require=EXTRAS_REQUIRE,
 )
```

### Comparing `flask-smorest-0.41.0/tests/conftest.py` & `flask-smorest-0.42.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/tests/mocks.py` & `flask-smorest-0.42.0/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/tests/test_api.py` & `flask-smorest-0.42.0/tests/test_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Test Api class"""
 import pytest
-
+from flask import jsonify
 from flask.views import MethodView
 from werkzeug.routing import BaseConverter
 import marshmallow as ma
 import apispec
 
-from flask_smorest import Api, Blueprint
+from flask_smorest import Api, Blueprint, current_api
 from flask_smorest.exceptions import MissingAPIParameterError
 
 from .utils import get_schemas, get_responses
 
 
 class TestApi:
     """Test Api class"""
@@ -408,7 +408,116 @@
         def test(val):
             pass
 
         api.register_blueprint(blp)
 
         # Default error is now registered
         assert "DEFAULT_ERROR" in get_responses(api.spec)
+
+    def test_multiple_apis_using_config_prefix_attribute(self, app):
+        app.config.update(
+            {
+                "API_TITLE": "Ignore this title",
+                "API_V1_API_TITLE": "V1 Title",
+                "API_V1_API_VERSION": "1",
+                "API_V1_OPENAPI_VERSION": "2.0",
+                "API_V2_API_TITLE": "V2 Title",
+                "API_V2_API_VERSION": "2",
+                "API_V2_OPENAPI_VERSION": "3.0.2",
+            }
+        )
+        api1 = Api(app, config_prefix="API_V1_")
+        api2 = Api(app, config_prefix="API_V2")
+
+        assert api1.spec.title == "V1 Title"
+        assert api2.spec.title == "V2 Title"
+
+    def test_prefixed_api_to_raise_correctly_formatted_error(self, app):
+        with pytest.raises(
+            MissingAPIParameterError,
+            match='API title must be specified either as "API_V1_API_TITLE"',
+        ):
+            Api(app, config_prefix="API_V1_")
+
+    def test_current_api(self, app):
+        def get_current_api_config_prefix():
+            return jsonify(current_api.config_prefix)
+
+        a_blp = Blueprint("A", "A")
+        a_blp.route("/")(get_current_api_config_prefix)
+
+        b_blp = Blueprint("B", "B")
+        b_blp.route("/")(get_current_api_config_prefix)
+
+        a_blp.register_blueprint(b_blp, url_prefix="/b")
+
+        api1 = Api(
+            app,
+            config_prefix="V1",
+            spec_kwargs={
+                "title": "V1",
+                "version": "1",
+                "openapi_version": "3.0.2",
+            },
+        )
+        api2 = Api(
+            app,
+            config_prefix="V2",
+            spec_kwargs={
+                "title": "V2",
+                "version": "2",
+                "openapi_version": "3.0.2",
+            },
+        )
+
+        api1.register_blueprint(a_blp, url_prefix="/v1/a", name="1A")
+        api1.register_blueprint(b_blp, url_prefix="/v1/b", name="1B")
+        api2.register_blueprint(a_blp, url_prefix="/v2/a", name="2A")
+        api2.register_blueprint(b_blp, url_prefix="/v2/b", name="2B")
+
+        client = app.test_client()
+        assert client.get("/v1/a/").json == "V1_"
+        assert client.get("/v1/a/b/").json == "V1_"
+        assert client.get("/v1/b/").json == "V1_"
+        assert client.get("/v2/a/").json == "V2_"
+        assert client.get("/v2/a/b/").json == "V2_"
+        assert client.get("/v2/b/").json == "V2_"
+
+    def test_api_config_proxying_flask_config(self, app):
+        app.config.update(
+            {
+                "DEBUG": True,
+                "SECRET_KEY": "secret",
+                "API_TITLE": "No Prefix Title",
+                "API_VERSION": "2",
+                "OPENAPI_VERSION": "3.0.2",
+                "API_V1_API_TITLE": "V1 Title",
+                "API_V1_API_VERSION": "1",
+                "API_V1_OPENAPI_VERSION": "2.0",
+                "API_V2_API_TITLE": "V2 Title",
+                "API_V2_API_VERSION": "2",
+                "API_V2_OPENAPI_VERSION": "3.0.2",
+            }
+        )
+
+        api_empty = Api(app)
+        # It is expected behaviour for Api with no config prefix to just
+        # proxy whole App config
+        assert "DEBUG" in api_empty.config
+        assert set(api_empty.config) == set(app.config)
+        assert len(api_empty.config) == len(app.config)
+
+        api_v1 = Api(app, config_prefix="API_V1")
+        assert set(api_v1.config) == {
+            "API_V1_API_TITLE",
+            "API_V1_API_VERSION",
+            "API_V1_OPENAPI_VERSION",
+        }
+        assert len(api_v1.config) == 3
+
+        api_v2 = Api(app, config_prefix="API_V2")
+        assert set(api_v2.config) == {
+            "API_V2_API_TITLE",
+            "API_V2_API_VERSION",
+            "API_V2_OPENAPI_VERSION",
+        }
+        assert len(api_v2.config) == 3
```

### Comparing `flask-smorest-0.41.0/tests/test_arguments.py` & `flask-smorest-0.42.0/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/tests/test_blueprint.py` & `flask-smorest-0.42.0/tests/test_blueprint.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/tests/test_error_handler.py` & `flask-smorest-0.42.0/tests/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/tests/test_etag.py` & `flask-smorest-0.42.0/tests/test_etag.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 from flask_smorest import Api, Blueprint, abort
 from flask_smorest.etag import _get_etag_ctx
 from flask_smorest.exceptions import (
     NotModified,
     PreconditionRequired,
     PreconditionFailed,
+    CurrentApiNotAvailableError,
 )
 from flask_smorest.utils import get_appcontext
 
-from .utils import build_ref
+from .utils import build_ref, request_ctx_with_current_api
 
 from .mocks import ItemNotFound
 
 
 HTTP_METHODS = ["OPTIONS", "HEAD", "GET", "POST", "PUT", "PATCH", "DELETE"]
 HTTP_METHODS_ALLOWING_SET_ETAG = ["GET", "HEAD", "POST", "PUT", "PATCH"]
 
@@ -146,46 +147,54 @@
         blp = Blueprint("test", __name__)
         data_1 = {"a": 1, "b": 2}
         data_2 = {"b": 2, "a": 1}
         assert blp._generate_etag(data_1) == blp._generate_etag(data_2)
 
     @pytest.mark.parametrize("method", HTTP_METHODS)
     def test_etag_check_precondition(self, app, method):
+        api = Api(app)
         blp = Blueprint("test", __name__)
+        api.register_blueprint(blp)
 
-        with app.test_request_context("/", method=method):
+        with request_ctx_with_current_api(app, blp, "/", method=method):
             if method in ["PUT", "PATCH", "DELETE"]:
                 with pytest.raises(PreconditionRequired):
                     blp._check_precondition()
             else:
                 blp._check_precondition()
 
     @pytest.mark.parametrize("method", ["PUT", "PATCH", "DELETE"])
     @pytest.mark.parametrize("etag_disabled", (True, False))
     def test_etag_check_etag(self, app, schemas, method, etag_disabled):
         app.config["ETAG_DISABLED"] = etag_disabled
+        api = Api(app)
         blp = Blueprint("test", __name__)
+        api.register_blueprint(blp)
         schema = schemas.DocSchema
         old_item = {"item_id": 1, "db_field": 0}
         new_item = {"item_id": 1, "db_field": 1}
         old_etag = blp._generate_etag(old_item)
         old_etag_with_schema = blp._generate_etag(schema().dump(old_item))
 
-        with app.test_request_context(
+        with request_ctx_with_current_api(
+            app,
+            blp,
             "/",
             method=method,
             headers={"If-Match": old_etag},
         ):
             blp.check_etag(old_item)
             if not etag_disabled:
                 with pytest.raises(PreconditionFailed):
                     blp.check_etag(new_item)
             else:
                 blp.check_etag(new_item)
-        with app.test_request_context(
+        with request_ctx_with_current_api(
+            app,
+            blp,
             "/",
             method=method,
             headers={"If-Match": old_etag_with_schema},
         ):
             blp.check_etag(old_item, schema)
             if not etag_disabled:
                 with pytest.raises(PreconditionFailed):
@@ -195,17 +204,21 @@
 
     @pytest.mark.parametrize("method", HTTP_METHODS)
     @pytest.mark.parametrize("etag_disabled", (True, False))
     def test_etag_check_etag_wrong_method_warning(
         self, app, method, etag_disabled, recwarn
     ):
         app.config["ETAG_DISABLED"] = etag_disabled
+        api = Api(app)
         blp = Blueprint("test", __name__)
+        api.register_blueprint(blp)
 
-        with app.test_request_context(
+        with request_ctx_with_current_api(
+            app,
+            blp,
             "/",
             method=method,
             headers={"If-Match": ""},
         ):
             # Ignore ETag check fail. Just testing the warning.
             try:
                 blp.check_etag(None)
@@ -218,19 +231,23 @@
             assert recwarn[0].category == UserWarning
             assert str(recwarn[0].message) == (
                 f"ETag cannot be checked on {method} request."
             )
 
     @pytest.mark.parametrize("method", HTTP_METHODS)
     def test_etag_verify_check_etag_warning(self, app, method, recwarn):
+        api = Api(app)
         blp = Blueprint("test", __name__)
+        api.register_blueprint(blp)
         old_item = {"item_id": 1, "db_field": 0}
         old_etag = blp._generate_etag(old_item)
 
-        with app.test_request_context(
+        with request_ctx_with_current_api(
+            app,
+            blp,
             "/",
             method=method,
             headers={"If-Match": old_etag},
         ):
             blp._verify_check_etag()
             if method in ["PUT", "PATCH", "DELETE"]:
                 assert len(recwarn) == 1
@@ -246,52 +263,60 @@
             blp._verify_check_etag()
             assert not recwarn
 
     @pytest.mark.parametrize("method", HTTP_METHODS_ALLOWING_SET_ETAG)
     @pytest.mark.parametrize("etag_disabled", (True, False))
     def test_etag_set_etag(self, app, schemas, method, etag_disabled):
         app.config["ETAG_DISABLED"] = etag_disabled
+        api = Api(app)
         blp = Blueprint("test", __name__)
+        api.register_blueprint(blp)
         schema = schemas.DocSchema
         item = {"item_id": 1, "db_field": 0}
         etag = blp._generate_etag(item)
         etag_with_schema = blp._generate_etag(schema().dump(item))
 
-        with app.test_request_context("/", method=method):
+        with request_ctx_with_current_api(app, blp, "/", method=method):
             blp.set_etag(item)
             if not etag_disabled:
                 assert _get_etag_ctx()["etag"] == etag
                 del _get_etag_ctx()["etag"]
             else:
                 assert "etag" not in _get_etag_ctx()
-        with app.test_request_context(
+        with request_ctx_with_current_api(
+            app,
+            blp,
             "/",
             method=method,
             headers={"If-None-Match": etag},
         ):
             if not etag_disabled:
                 if method in ["GET", "HEAD"]:
                     with pytest.raises(NotModified):
                         blp.set_etag(item)
             else:
                 blp.set_etag(item)
                 assert "etag" not in _get_etag_ctx()
-        with app.test_request_context(
+        with request_ctx_with_current_api(
+            app,
+            blp,
             "/",
             method=method,
             headers={"If-None-Match": etag_with_schema},
         ):
             if not etag_disabled:
                 if method in ["GET", "HEAD"]:
                     with pytest.raises(NotModified):
                         blp.set_etag(item, schema)
             else:
                 blp.set_etag(item, schema)
                 assert "etag" not in _get_etag_ctx()
-        with app.test_request_context(
+        with request_ctx_with_current_api(
+            app,
+            blp,
             "/",
             method=method,
             headers={"If-None-Match": "dummy"},
         ):
             if not etag_disabled:
                 blp.set_etag(item)
                 assert _get_etag_ctx()["etag"] == etag
@@ -307,17 +332,19 @@
 
     @pytest.mark.parametrize("etag_disabled", (True, False))
     @pytest.mark.parametrize("method", HTTP_METHODS)
     def test_etag_set_etag_method_not_allowed_warning(
         self, app, method, etag_disabled, recwarn
     ):
         app.config["ETAG_DISABLED"] = etag_disabled
+        api = Api(app)
         blp = Blueprint("test", __name__)
+        api.register_blueprint(blp)
 
-        with app.test_request_context("/", method=method):
+        with request_ctx_with_current_api(app, blp, "/", method=method):
             blp.set_etag(None)
         if method in HTTP_METHODS_ALLOWING_SET_ETAG:
             assert not recwarn
         else:
             assert len(recwarn) == 1
             assert recwarn[0].category == UserWarning
             assert str(recwarn[0].message) == (
@@ -613,7 +640,60 @@
             ) == (method in ["GET", "HEAD"])
             assert (build_ref(api.spec, "parameter", "IF_MATCH") in parameters) == (
                 method in ["PUT", "PATCH", "DELETE"]
             )
             assert not has_response or (
                 response_headers.get("ETag") == build_ref(api.spec, "header", "ETAG")
             ) == (method in ["GET", "HEAD", "POST", "PUT", "PATCH"])
+
+    @pytest.mark.parametrize("etag_disabled_for_v1", [False, True])
+    @pytest.mark.parametrize("etag_disabled_for_v2", [False, True])
+    def test_multiple_apis_per_app(
+        self, app, etag_disabled_for_v1, etag_disabled_for_v2
+    ):
+        # All created APIs are using prefix. So default ETAG_DISABLED should be ignored
+        app.config["ETAG_DISABLED"] = True
+        app.config["V1_ETAG_DISABLED"] = etag_disabled_for_v1
+        app.config["V2_ETAG_DISABLED"] = etag_disabled_for_v2
+
+        for i in [1, 2]:
+            api = Api(
+                app,
+                config_prefix=f"V{i}_",
+                spec_kwargs={
+                    "title": f"V{i}",
+                    "version": f"{i}",
+                    "openapi_version": "3.0.2",
+                },
+            )
+            blp = Blueprint(f"test{i}", f"test{i}", url_prefix=f"/test-{i}")
+
+            @blp.route("/")
+            @blp.etag
+            @blp.response(200)
+            def test():
+                return {}
+
+            api.register_blueprint(blp)
+
+        client = app.test_client()
+        headers1 = client.get("/test-1/").headers
+        headers2 = client.get("/test-2/").headers
+
+        if etag_disabled_for_v1:
+            assert "ETag" not in headers1
+        else:
+            assert "ETag" in headers1
+
+        if etag_disabled_for_v2:
+            assert "ETag" not in headers2
+        else:
+            assert "ETag" in headers2
+
+    def test_trying_to_use_etag_without_current_api(self, app, collection):
+        Api(app)
+        blp = Blueprint("test", "test")
+        collection.post({"item_id": 1, "field": "test"})
+        item = collection.items[0]
+        with app.test_request_context(f"/test/{item['item_id']}"):
+            with pytest.raises(CurrentApiNotAvailableError):
+                blp.set_etag(item)
```

### Comparing `flask-smorest-0.41.0/tests/test_examples.py` & `flask-smorest-0.42.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/tests/test_pagination.py` & `flask-smorest-0.42.0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/tests/test_response.py` & `flask-smorest-0.42.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `flask-smorest-0.41.0/tests/test_spec.py` & `flask-smorest-0.42.0/tests/test_spec.py`

 * *Files 16% similar despite different names*

```diff
@@ -428,14 +428,69 @@
         paths = {f"/path_{i}": str(i) for i in range(20)}
         api.spec._paths = paths
 
         response_json_docs = client.get("/api-docs/openapi.json")
         assert response_json_docs.status_code == 200
         assert response_json_docs.json["paths"] == paths
 
+    def test_multiple_apis_serve_separate_specs(self, app):
+        client = app.test_client()
+
+        for i in [1, 2]:
+            app.config[f"V{i}_OPENAPI_URL_PREFIX"] = f"/v{i}-docs"
+            app.config[f"V{i}_OPENAPI_RAPIDOC_PATH"] = "rapidoc/"
+            app.config[f"V{i}_OPENAPI_RAPIDOC_URL"] = "/statid/rapidoc.js"
+            app.config[f"V{i}_OPENAPI_REDOC_PATH"] = "/redoc/"
+            app.config[f"V{i}_OPENAPI_SWAGGER_UI_URL"] = "/static/swagger-ui/"
+            app.config[f"V{i}_OPENAPI_SWAGGER_UI_PATH"] = "/swagger/"
+            app.config[f"V{i}_OPENAPI_REDOC_URL"] = "/static/redoc.js"
+            app.config[f"V{i}_OPENAPI_REDOC_PATH"] = "/redoc/"
+            api = Api(
+                app,
+                config_prefix=f"V{i}_",
+                spec_kwargs={
+                    "title": f"V{i}",
+                    "version": f"{i}",
+                    "openapi_version": "3.0.2",
+                },
+            )
+            blp = Blueprint(f"test{i}", f"test{i}", url_prefix=f"/test-{i}")
+            blp.route("/")(lambda: None)
+            api.register_blueprint(blp)
+
+        # Checking openapi.json
+
+        json1 = client.get("/v1-docs/openapi.json").json
+        json2 = client.get("/v2-docs/openapi.json").json
+
+        # Should have a different info
+        assert json1["info"]["title"] == "V1"
+        assert json2["info"]["title"] == "V2"
+
+        # One api's routes should not leak into other's
+        assert "/test-1/" in json1["paths"]
+        assert "/test-2/" not in json1["paths"]
+        assert "/test-1/" not in json2["paths"]
+        assert "/test-2/" in json2["paths"]
+
+        # Checking RapiDoc
+
+        assert "/v1-docs/openapi.json" in client.get("/v1-docs/rapidoc/").text
+        assert "/v2-docs/openapi.json" in client.get("/v2-docs/rapidoc/").text
+
+        # Checking Swagger
+
+        assert "/v1-docs/openapi.json" in client.get("/v1-docs/swagger/").text
+        assert "/v2-docs/openapi.json" in client.get("/v2-docs/swagger/").text
+
+        # Checking ReDoc
+
+        assert "/v1-docs/openapi.json" in client.get("/v1-docs/redoc/").text
+        assert "/v2-docs/openapi.json" in client.get("/v2-docs/redoc/").text
+
 
 class TestAPISpecCLICommands:
     """Test OpenAPI CLI commands"""
 
     @pytest.mark.parametrize(
         ("cmd", "deserialize_fn"),
         [
@@ -525,7 +580,84 @@
         result = app.test_cli_runner().invoke(
             args=["openapi", "write", "--format=yaml", str(temp_file)]
         )
         assert result.exit_code == 0
         assert result.output.startswith(
             "To use yaml output format, please install PyYAML module"
         )
+
+    def test_apispec_command_print_with_multiple_apis(self, app):
+        spec_kwargs = {
+            "version": "1",
+            "openapi_version": "3.0.2",
+        }
+        Api(app, config_prefix="V1", spec_kwargs={**spec_kwargs, "title": "V1"})
+        Api(app, config_prefix="V2", spec_kwargs={**spec_kwargs, "title": "V2"})
+
+        assert (
+            "Error:" in app.test_cli_runner().invoke(args=["openapi", "print"]).output
+        )
+        assert (
+            "Error: "
+            in app.test_cli_runner()
+            .invoke(args=["openapi", "print", "--config-prefix=not_exist"])
+            .output
+        )
+
+        ret_1 = app.test_cli_runner().invoke(
+            args=["openapi", "print", "--config-prefix=v1"]
+        )
+        assert "V1" in ret_1.output
+        assert "V2" not in ret_1.output
+        ret_2 = app.test_cli_runner().invoke(
+            args=["openapi", "print", "--config-prefix=v2"]
+        )
+        assert "V1" not in ret_2.output
+        assert "V2" in ret_2.output
+
+    def test_apispec_command_write_with_multiple_apis(self, app, tmp_path):
+        temp_file1 = tmp_path / "output1"
+        temp_file2 = tmp_path / "output2"
+
+        spec_kwargs = {
+            "version": "1",
+            "openapi_version": "3.0.2",
+        }
+        Api(app, config_prefix="V1", spec_kwargs={**spec_kwargs, "title": "V1"})
+        Api(app, config_prefix="V2", spec_kwargs={**spec_kwargs, "title": "V2"})
+
+        assert (
+            "Error: " in app.test_cli_runner().invoke(args=["openapi", "write"]).output
+        )
+        assert (
+            "Error: "
+            in app.test_cli_runner()
+            .invoke(args=["openapi", "write", "--config-prefix=not_exist"])
+            .output
+        )
+
+        app.test_cli_runner().invoke(
+            args=["openapi", "write", "--config-prefix=v1", str(temp_file1)]
+        )
+        with open(temp_file1, encoding="utf-8") as spec_file1:
+            content1 = spec_file1.read()
+            assert "V1" in content1
+            assert "V2" not in content1
+
+        app.test_cli_runner().invoke(
+            args=["openapi", "write", "--config-prefix=v2", str(temp_file2)]
+        )
+        with open(temp_file2, encoding="utf-8") as spec_file2:
+            content2 = spec_file2.read()
+            assert "V1" not in content2
+            assert "V2" in content2
+
+    def test_apispec_command_list_config_prefixes(self, app):
+        spec_kwargs = {
+            "version": "1",
+            "openapi_version": "3.0.2",
+        }
+        Api(app, config_prefix="", spec_kwargs={**spec_kwargs, "title": ""})
+        Api(app, config_prefix="V1", spec_kwargs={**spec_kwargs, "title": "V1"})
+        Api(app, config_prefix="V2", spec_kwargs={**spec_kwargs, "title": "V2"})
+        result = app.test_cli_runner().invoke(args=["openapi", "list-config-prefixes"])
+        assert set(result.output.strip().splitlines()) == {'""', '"V1_"', '"V2_"'}
```

### Comparing `flask-smorest-0.41.0/tests/test_utils.py` & `flask-smorest-0.42.0/tests/test_utils.py`

 * *Files identical despite different names*

