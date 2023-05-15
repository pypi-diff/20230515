# Comparing `tmp/zcollection-2023.3.2.tar.gz` & `tmp/zcollection-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcollection-2023.3.2.tar", last modified: Wed Mar 22 16:12:29 2023, max compression
+gzip compressed data, was "zcollection-2023.5.0.tar", last modified: Mon May 15 12:55:11 2023, max compression
```

## Comparing `zcollection-2023.3.2.tar` & `zcollection-2023.5.0.tar`

### file list

```diff
@@ -1,128 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.693557 zcollection-2023.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-22 16:12:16.000000 zcollection-2023.3.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.677558 zcollection-2023.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-22 16:12:16.000000 zcollection-2023.3.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-22 16:12:16.000000 zcollection-2023.3.2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-22 16:12:16.000000 zcollection-2023.3.2/.github/workflows/pypipublish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-22 16:12:16.000000 zcollection-2023.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-22 16:12:16.000000 zcollection-2023.3.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-22 16:12:16.000000 zcollection-2023.3.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-22 16:12:16.000000 zcollection-2023.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-03-22 16:12:29.693557 zcollection-2023.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-22 16:12:16.000000 zcollection-2023.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-22 16:12:16.000000 zcollection-2023.3.2/conda/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-22 16:12:16.000000 zcollection-2023.3.2/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.677558 zcollection-2023.3.2/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    25304 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/images/merge_time_series.png
--rw-r--r--   0 runner    (1001) docker     (123)    32445 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/images/merge_time_series.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-22 16:12:16.000000 zcollection-2023.3.2/docs/source/release.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.693557 zcollection-2023.3.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-22 16:12:16.000000 zcollection-2023.3.2/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-03-22 16:12:16.000000 zcollection-2023.3.2/examples/ex_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-03-22 16:12:16.000000 zcollection-2023.3.2/examples/ex_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-03-22 16:12:16.000000 zcollection-2023.3.2/examples/ex_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-03-22 16:12:16.000000 zcollection-2023.3.2/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-22 16:12:16.000000 zcollection-2023.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-22 16:12:16.000000 zcollection-2023.3.2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-22 16:12:29.693557 zcollection-2023.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-22 16:12:16.000000 zcollection-2023.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.685557 zcollection-2023.3.2/zcollection/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.685557 zcollection-2023.3.2/zcollection/collection/
--rw-r--r--   0 runner    (1001) docker     (123)    42700 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/collection/callable_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/collection/detail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.685557 zcollection-2023.3.2/zcollection/collection/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/collection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32786 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/collection/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/compressed_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.685557 zcollection-2023.3.2/zcollection/convenience/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/convenience/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/convenience/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/convenience/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/fs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.685557 zcollection-2023.3.2/zcollection/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15966 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/indexing/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.685557 zcollection-2023.3.2/zcollection/indexing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/indexing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/indexing/tests/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/mathematics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.685557 zcollection-2023.3.2/zcollection/merging/
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/merging/period.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/zcollection/merging/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/merging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/merging/tests/test_merging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/merging/tests/test_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/merging/tests/test_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/merging/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/zcollection/partitioning/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/zcollection/partitioning/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/partitioning/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/zcollection/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/first_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/second_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_compressed_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_mathematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/type_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)    23275 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-22 16:12:29.000000 zcollection-2023.3.2/zcollection/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/zcollection/view/
--rw-r--r--   0 runner    (1001) docker     (123)    28680 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/view/detail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.689557 zcollection-2023.3.2/zcollection/view/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/view/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-03-22 16:12:16.000000 zcollection-2023.3.2/zcollection/view/tests/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:12:29.693557 zcollection-2023.3.2/zcollection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-03-22 16:12:29.000000 zcollection-2023.3.2/zcollection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-03-22 16:12:29.000000 zcollection-2023.3.2/zcollection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 16:12:29.000000 zcollection-2023.3.2/zcollection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 16:12:29.000000 zcollection-2023.3.2/zcollection.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-22 16:12:29.000000 zcollection-2023.3.2/zcollection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-22 16:12:29.000000 zcollection-2023.3.2/zcollection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.573743 zcollection-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 12:55:01.000000 zcollection-2023.5.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.529743 zcollection-2023.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.565743 zcollection-2023.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-15 12:55:01.000000 zcollection-2023.5.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-15 12:55:01.000000 zcollection-2023.5.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 12:55:01.000000 zcollection-2023.5.0/.github/workflows/pypipublish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-15 12:55:01.000000 zcollection-2023.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-15 12:55:01.000000 zcollection-2023.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.565743 zcollection-2023.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-15 12:55:01.000000 zcollection-2023.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-15 12:55:01.000000 zcollection-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-15 12:55:11.573743 zcollection-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-15 12:55:01.000000 zcollection-2023.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.565743 zcollection-2023.5.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-15 12:55:01.000000 zcollection-2023.5.0/conda/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:55:01.000000 zcollection-2023.5.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.565743 zcollection-2023.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.569743 zcollection-2023.5.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.533743 zcollection-2023.5.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.569743 zcollection-2023.5.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.569743 zcollection-2023.5.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    25304 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/images/merge_time_series.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32445 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/images/merge_time_series.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-15 12:55:01.000000 zcollection-2023.5.0/docs/source/release.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.569743 zcollection-2023.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-15 12:55:01.000000 zcollection-2023.5.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-05-15 12:55:01.000000 zcollection-2023.5.0/examples/ex_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-15 12:55:01.000000 zcollection-2023.5.0/examples/ex_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-15 12:55:01.000000 zcollection-2023.5.0/examples/ex_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-05-15 12:55:01.000000 zcollection-2023.5.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-15 12:55:01.000000 zcollection-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-15 12:55:01.000000 zcollection-2023.5.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-15 12:55:11.577743 zcollection-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-15 12:55:01.000000 zcollection-2023.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.541743 zcollection-2023.5.0/zcollection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.545743 zcollection-2023.5.0/zcollection/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)    27869 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/collection/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/collection/callable_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/collection/detail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.545743 zcollection-2023.5.0/zcollection/collection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/collection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36376 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/collection/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/compressed_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.545743 zcollection-2023.5.0/zcollection/convenience/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/convenience/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/convenience/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/convenience/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29095 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/fs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.545743 zcollection-2023.5.0/zcollection/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/indexing/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.549743 zcollection-2023.5.0/zcollection/indexing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/indexing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/indexing/tests/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/mathematics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.549743 zcollection-2023.5.0/zcollection/merging/
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17011 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/merging/period.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.549743 zcollection-2023.5.0/zcollection/merging/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/merging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/merging/tests/test_merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/merging/tests/test_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/merging/tests/test_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/merging/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.553743 zcollection-2023.5.0/zcollection/partitioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.553743 zcollection-2023.5.0/zcollection/partitioning/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/partitioning/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.561743 zcollection-2023.5.0/zcollection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/first_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/second_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_compressed_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_mathematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/type_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.561743 zcollection-2023.5.0/zcollection/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/delayed_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.561743 zcollection-2023.5.0/zcollection/variable/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/tests/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/tests/test_delayed_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/variable/tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-15 12:55:11.000000 zcollection-2023.5.0/zcollection/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.565743 zcollection-2023.5.0/zcollection/view/
+-rw-r--r--   0 runner    (1001) docker     (123)    31686 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24141 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/view/detail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.565743 zcollection-2023.5.0/zcollection/view/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/view/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-05-15 12:55:01.000000 zcollection-2023.5.0/zcollection/view/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:55:11.573743 zcollection-2023.5.0/zcollection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-15 12:55:11.000000 zcollection-2023.5.0/zcollection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-15 12:55:11.000000 zcollection-2023.5.0/zcollection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:55:11.000000 zcollection-2023.5.0/zcollection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:55:11.000000 zcollection-2023.5.0/zcollection.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-15 12:55:11.000000 zcollection-2023.5.0/zcollection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 12:55:11.000000 zcollection-2023.5.0/zcollection.egg-info/top_level.txt
```

### Comparing `zcollection-2023.3.2/.github/workflows/ci.yaml` & `zcollection-2023.5.0/.github/workflows/ci.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         extra-specs: |
           python=${{ matrix.python-version }}
 
     - name: Run Tests
       shell: bash -l {0}
       run: |
         python -m setuptools_scm
-        pytest -v -ra
+        pytest -v -ra --processes
 
   s3-fs:
     runs-on: ubuntu-latest
     timeout-minutes: 15
     steps:
     - name: Checkout
       uses: actions/checkout@v3
@@ -64,15 +64,15 @@
         extra-specs: |
           python=3.9
 
     - name: Run Tests
       shell: bash -l {0}
       run: |
         python -m setuptools_scm
-        pytest -v -ra --s3
+        pytest -v -ra --s3 --processes
 
   win:
     name: win
     runs-on: windows-2019
     timeout-minutes: 15
 
     steps:
@@ -89,8 +89,8 @@
         extra-specs: |
           python=3.9
 
     - name: Run Tests
       shell: bash -l {0}
       run: |
         python -m setuptools_scm
-        pytest -v -ra
+        pytest -v -ra --processes
```

### Comparing `zcollection-2023.3.2/.github/workflows/pypipublish.yaml` & `zcollection-2023.5.0/.github/workflows/pypipublish.yaml`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/.gitignore` & `zcollection-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/.pre-commit-config.yaml` & `zcollection-2023.5.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - id: double-quote-string-fixer
       - id: mixed-line-ending
         args: [--fix=lf]
         exclude: docs/make.bat
       - id: trailing-whitespace
         exclude: conda/meta.yaml
   - repo: https://github.com/asottile/pyupgrade
-    rev: "v3.3.1"
+    rev: "v3.4.0"
     hooks:
     - id: pyupgrade
       args: [--py38-plus]
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
@@ -39,23 +39,23 @@
   - repo: https://github.com/pre-commit/mirrors-yapf
     rev: v0.32.0
     hooks:
       - id: yapf
         additional_dependencies:
           - toml
   - repo: https://github.com/myint/docformatter
-    rev: "v1.5.1"
+    rev: "v1.6.5"
     hooks:
     - id: docformatter
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.4"
     hooks:
     - id: codespell
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         exclude: docs
         additional_dependencies:
           # Type stubs
           - types-requests
           - types-setuptools
```

### Comparing `zcollection-2023.3.2/LICENSE` & `zcollection-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/PKG-INFO` & `zcollection-2023.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcollection
-Version: 2023.3.2
+Version: 2023.5.0
 Summary: Zarr Collection
 Home-page: https://github.com/CNES/zcollection
 Author: CNES/CLS
 Author-email: fbriol@gmail.com
 License: BSD License
 Keywords: zarr,collection,xarray,dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `zcollection-2023.3.2/README.rst` & `zcollection-2023.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/conda/meta.yaml` & `zcollection-2023.5.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/Makefile` & `zcollection-2023.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/make.bat` & `zcollection-2023.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/source/_templates/autosummary/class.rst` & `zcollection-2023.5.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/source/_templates/autosummary/module.rst` & `zcollection-2023.5.0/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/source/api.rst` & `zcollection-2023.5.0/docs/source/api.rst`

 * *Files 20% similar despite different names*

```diff
@@ -27,29 +27,41 @@
 .. autosummary::
   :toctree: _generated/
 
   zcollection.merging
   zcollection.merging.time_series
   zcollection.merging.period
 
+Variable
+========
+
+Variables handled by the datasets. These objects manage access to the data
+stored in the collection.
+
+.. autosummary::
+  :toctree: _generated/
+
+  zcollection.variable.abc
+  zcollection.variable.array
+  zcollection.variable.delayed_array
+
 Collection
 ==========
 
 .. autosummary::
   :toctree: _generated/
 
   zcollection.collection
   zcollection.dask_utils
   zcollection.dataset
   zcollection.expression
   zcollection.fs_utils
   zcollection.meta
   zcollection.sync
   zcollection.type_hints
-  zcollection.variable
   zcollection.view
 
 Indexing
 ========
 
 .. autosummary::
   :toctree: _generated/
```

### Comparing `zcollection-2023.3.2/docs/source/conf.py` & `zcollection-2023.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/source/images/merge_time_series.png` & `zcollection-2023.5.0/docs/source/images/merge_time_series.png`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/source/images/merge_time_series.svg` & `zcollection-2023.5.0/docs/source/images/merge_time_series.svg`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/source/index.rst` & `zcollection-2023.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/source/install.rst` & `zcollection-2023.5.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/docs/source/release.rst` & `zcollection-2023.5.0/docs/source/release.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 Release notes
 =============
 
+2023.5.0
+--------
+* Add missing copyrights.
+* Modularise code to reduce the number of lines per module.
+* Writing variables is limited to the worker being used.
+* Improve test coverage.
+* #9: Read the version attribute directly from the ``version.py`` module.
+* #8: Incomplete overlaps with more than one worker.
+* #7: Fix bug, in the update method, if the user has selected multiple
+  partitions the selected variables must contain the updated variables.
+* #6: the parameter name for specifying the number of concurrent inserts is
+  incorrect.
+* #3: Add a trim argument to the ``update`` method, like Dask's Dask's
+  ``map_overlap``.
+* Update the documentation.
+* Refactor the code.
+* Loading data using Dask or Numpy.
+* Variable adds attributes to partitions.
+
 2023.3.2
 --------
 * Writing a partition with many variables is slow.
 * Writing metadata only in the collection's configuration.
 * Adding an inter-process lock
 * If a variable has been modified since its initialization, the library throws a
   specific exception to warn the user.
```

### Comparing `zcollection-2023.3.2/examples/ex_collection.py` & `zcollection-2023.5.0/examples/ex_collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 =========================
 
 This section outlines the steps required to get started with the main features
 of a ``Collection``.
 """
 from __future__ import annotations
 
+from typing import Iterator
 import datetime
 import pprint
 
 import dask.distributed
 import fsspec
 import numpy
 
@@ -19,27 +20,29 @@
 
 
 # %%
 # Initialization of the environment
 # ---------------------------------
 #
 # Before we create our first collection, we will create a dataset to record.
-def create_dataset():
+def create_dataset() -> zcollection.Dataset:
     """Create a dataset to record."""
-    generator = zcollection.tests.data.create_test_dataset_with_fillvalue()
+    generator: Iterator[zcollection.Dataset] = \
+        zcollection.tests.data.create_test_dataset_with_fillvalue()
     return next(generator)
 
 
-ds = create_dataset()
-ds.to_xarray()
+zds: zcollection.Dataset | None = create_dataset()
+assert zds is not None
+zds.to_xarray()
 
 # %%
 # We will create the file system that we will use. In this example, a file
 # system in memory.
-fs = fsspec.filesystem('memory')
+fs: fsspec.AbstractFileSystem = fsspec.filesystem('memory')
 
 # %%
 # Finally we create a local dask cluster using only threads in order to work
 # with the file system stored in memory.
 cluster = dask.distributed.LocalCluster(processes=False)
 client = dask.distributed.Client(cluster)
 
@@ -50,19 +53,16 @@
 # Before creating our collection, we define the partitioning of our dataset. In
 # this example, we will partition the data by ``month`` using the variable
 # ``time``.
 partition_handler = zcollection.partitioning.Date(('time', ), resolution='M')
 
 # %%
 # Finally, we create our collection:
-collection = zcollection.create_collection('time',
-                                           ds,
-                                           partition_handler,
-                                           '/my_collection',
-                                           filesystem=fs)
+collection: zcollection.Collection = zcollection.create_collection(
+    'time', zds, partition_handler, '/my_collection', filesystem=fs)
 
 # %%
 # .. note::
 #
 #    The collection created can be accessed using the following command ::
 #
 #        >>> collection = zcollection.open_collection("/my_collection",
@@ -71,15 +71,15 @@
 # When the collection has been created, a configuration file is created. This
 # file contains all the metadata to ensure that all future inserted data will
 # have the same features as the existing data (data consistency).
 pprint.pprint(collection.metadata.get_config())
 
 # %%
 # Now that the collection has been created, we can insert new records.
-collection.insert(ds)
+collection.insert(zds)
 
 # %%
 # .. note::
 #
 #     When inserting it's possible to specify the :ref:`merge strategy of a
 #     partition <merging_datasets>`. By default, the last inserted data
 #     overwrite the existing ones. Others strategy can be defined, for example,
@@ -99,17 +99,23 @@
 # as a single data set.
 #
 # Loading data
 # ------------
 # To load the dataset call the method
 # :py:meth:`load<zcollection.collection.Collection.load>` on the instance.  By
 # default, the method loads all partitions stored in the collection.
-collection.load()
+collection.load(delayed=True)
 
 # %%
+# .. note::
+#
+#   By default, the data is loaded as a :py:class:`dask.array<da.Array>`. It is
+#   possible to load the data as a :py:class:`numpy.ndarray` by specifying the
+#   parameter ``delayed=False``.
+#
 # You can also filter the partitions to be considered by filtering the
 # partitions using keywords used for partitioning in a valid Python expression.
 collection.load(filters='year == 2000 and month == 2')
 
 # %%
 # You can also used a callback function to filter partitions with a complex
 # condition.
@@ -141,58 +147,67 @@
     collection.drop_variable('time')
 except ValueError as exc:
     print(exc)
 
 # %%
 # The :py:meth:`add_variable<zcollection.collection.Collection.add_variable>`
 # method allows you to add a new variable to the collection.
-collection.add_variable(ds.metadata().variables['var2'])
+collection.add_variable(zds.metadata().variables['var2'])
 
 # %%
 # The newly created variable is initialized with its default value.
-ds = collection.load()
-assert ds is not None
-ds.variables['var2'].values
+zds = collection.load()
+assert zds is not None
+zds.variables['var2'].values
 
 
 # %%
 # Finally it's possible to
 # :py:meth:`update<zcollection.collection.Collection.update>` the existing
 # variables.
 #
 # In this example, we will alter the variable ``var2`` by setting it to 1
 # anywhere the variable ``var1`` is defined.
-def ones(ds):
+def ones(zds) -> dict[str, numpy.ndarray]:
     """Returns a variable with ones everywhere."""
-    return dict(var2=ds.variables['var1'].values * 0 + 1)
+    return dict(var2=zds.variables['var1'].values * 0 + 1)
 
 
 collection.update(ones)  # type: ignore[arg-type]
 
-ds = collection.load()
-assert ds is not None
-ds.variables['var2'].values
+zds = collection.load()
+assert zds is not None
+zds.variables['var2'].values
 
 
 # %%
+# ..note::
+#
+#   The method :py:meth:`update<zcollection.collection.Collection.update>`
+#   supports the ``delayed`` parameter. If ``delayed=True``, the function
+#   ``ones`` is applied to each partition using a Dask array as container
+#   for the variables data stored in the provided dataset. This is the default
+#   behavior. If ``delayed=False``, the function ``ones`` is applied to each
+#   partition using a Numpy array as container.
+#
 # Sometime is it important to know the values of the neighboring partitions.
 # This can be done using the
 # :py:meth:`update<zcollection.collection.Collection.update>` method with the
 # ``depth`` argument. In this example, we will set the variable ``var2`` to 2
 # everywhere the processed partition is surrounded by at least one partition, -1
 # if the left partition is missing and -2 if the right partition is missing.
 #
 # .. note::
 #
 #   ``partition_info`` contains information about the target partition: a tuple
 #   with the partitioned dimension and the slice to select the partition. If the
 #   start of the slice is 0, it means that the left partition is missing. If the
 #   stop of the slice is equal to the length of the given dataset, it means that
 #   the right partition is missing.
-def twos(ds, partition_info: tuple[str, slice]):
+def twos(ds, partition_info: tuple[str, slice]) -> dict[str, numpy.ndarray]:
     """Returns a variable with twos everywhere if the partition is surrounded
     by partitions on both sides, -1 if the left partition is missing and -2 if
     the right partition is missing."""
     data = numpy.zeros(ds.variables['var1'].shape, dtype='int8')
     dim, indices = partition_info
     assert dim == 'num_lines'
     if indices.start != 0:
@@ -202,17 +217,17 @@
     else:
         data[:] = 2
     return dict(var2=data)
 
 
 collection.update(twos, depth=1)  # type: ignore[arg-type]
 
-ds = collection.load()
-assert ds is not None
-ds.variables['var2'].values
+zds = collection.load()
+assert zds is not None
+zds.variables['var2'].values
 
 # %%
 # Map a function over the collection
 # ----------------------------------
 # It's possible to map a function over the partitions of the collection.
 for partition, array in collection.map(lambda ds: (  # type: ignore[arg-type]
         ds['var1'].values + ds['var2'].values)).compute():
```

### Comparing `zcollection-2023.3.2/examples/ex_indexing.py` & `zcollection-2023.5.0/examples/ex_indexing.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import dask.distributed
 import fsspec
 import numpy
 
 import zcollection
 import zcollection.indexing
-import zcollection.tests.data
+import zcollection.partitioning.tests.data
 
 # %%
 # Initialization of the environment
 # ---------------------------------
 fs = fsspec.filesystem('memory')
 cluster = dask.distributed.LocalCluster(processes=False)
 client = dask.distributed.Client(cluster)
@@ -28,26 +28,26 @@
 # having to browse the entire dataset.
 #
 # Creating the test collection.
 # -----------------------------
 #
 # For this latest example, we will index another data set. This one contains
 # measurements of a fictitious satellite on several half-orbits.
-ds = zcollection.Dataset.from_xarray(
-    zcollection.tests.data.create_test_sequence(5, 20, 10))
-ds
+zds: zcollection.Dataset = zcollection.Dataset.from_xarray(
+    zcollection.partitioning.tests.data.create_test_sequence(5, 20, 10))
+print(zds)
 
 # %%
-collection = zcollection.create_collection(
+collection: zcollection.Collection = zcollection.create_collection(
     'time',
-    ds,
+    zds,
     zcollection.partitioning.Date(('time', ), 'M'),
     partition_base_dir='/one_other_collection',
     filesystem=fs)
-collection.insert(ds, merge_callable=zcollection.merging.merge_time_series)
+collection.insert(zds, merge_callable=zcollection.merging.merge_time_series)
 
 # %%
 # Here we have created a collection partitioned by month.
 pprint.pprint(fs.listdir('/one_other_collection/year=2000'))
 
 
 # %%
@@ -83,29 +83,29 @@
     yield from tuple(zip(half_orbit[:-1], half_orbit[1:]))
 
 
 # %%
 # Now we will compute these constant parts from a dataset contained in a
 # partition.
 def _half_orbit(
-    ds: zcollection.Dataset,
+    zds: zcollection.Dataset,
     *args,
     **kwargs,
 ) -> numpy.ndarray:
     """Return the indexes of the start and stop of each half-orbit.
 
     Args:
         ds: Datasets stored in a partition to be indexed.
     Returns:
         Dictionary of start and stop indexes for each half-orbit.
     """
     pass_number_varname = kwargs.pop('pass_number', 'pass_number')
     cycle_number_varname = kwargs.pop('cycle_number', 'cycle_number')
-    pass_number = ds.variables[pass_number_varname].values
-    cycle_number = ds.variables[cycle_number_varname].values
+    pass_number = zds.variables[pass_number_varname].values
+    cycle_number = zds.variables[cycle_number_varname].values
 
     generator = ((
         i0,
         i1,
         cycle_number[i0],
         pass_number[i0],
     ) for i0, i1 in split_half_orbit(cycle_number, pass_number))
@@ -137,35 +137,35 @@
             (cls.PASS_NUMBER, 'uint16'),
         ]
 
     @classmethod
     def create(
         cls,
         path: Union[pathlib.Path, str],
-        ds: zcollection.Collection,
+        zds: zcollection.Collection,
         filesystem: Optional[fsspec.AbstractFileSystem] = None,
         **kwargs,
     ) -> 'HalfOrbitIndexer':
         """Create a new index.
 
         Args:
             path: The path to the index.
             ds: The collection to be indexed.
             filesystem: The filesystem to use.
         Returns:
             The created index.
         """
         return super()._create(path,
-                               ds,
+                               zds,
                                meta=dict(attribute=b'value'),
                                filesystem=filesystem)  # type: ignore
 
     def update(
         self,
-        ds: zcollection.Collection,
+        zds: zcollection.Collection,
         partition_size: Optional[int] = None,
         npartitions: Optional[int] = None,
         **kwargs,
     ) -> None:
         """Update the index.
 
         Args:
@@ -173,34 +173,40 @@
             partition_size: The length of each bag partition.
             npartitions: The number of desired bag partitions.
             cycle_number: The name of the cycle number variable stored in the
                 collection. Defaults to "cycle_number".
             pass_number: The name of the pass number variable stored in the
                 collection. Defaults to "pass_number".
         """
-        super()._update(ds, _half_orbit, partition_size, npartitions, **kwargs)
+        super()._update(zds, _half_orbit, partition_size, npartitions,
+                        **kwargs)
 
 
 # %%
 # Using the index
 # ---------------
 #
 # Now we can create our index and fill it.
-indexer = HalfOrbitIndexer.create('/index.parquet', collection, filesystem=fs)
+indexer: HalfOrbitIndexer = HalfOrbitIndexer.create('/index.parquet',
+                                                    collection,
+                                                    filesystem=fs)
 indexer.update(collection)
 
 # The following command allows us to view the information stored in our index:
 # the first and last indexes of the partition associated with the registered
 # half-orbit number and the identifier of the indexed partition.
 indexer.table.to_pandas()
 
 # %%
 # This index can now be used to load a part of a collection.
-selection = collection.load(indexer=indexer.query(dict(pass_number=[1, 2])))
+selection: zcollection.Dataset | None = collection.load(
+    indexer=indexer.query(dict(pass_number=[1, 2])),
+    delayed=False,
+)
 assert selection is not None
-selection.to_xarray().compute()
+selection.to_xarray()
 
 # %%
 # Close the local cluster to avoid printing warning messages in the other
 # examples.
 client.close()
 cluster.close()
```

### Comparing `zcollection-2023.3.2/examples/ex_view.py` & `zcollection-2023.5.0/examples/ex_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Overview of a View.
 ===================
 
 This section outlines the steps required to get started with the main features
 of a ``View``.
 """
+from typing import Iterator
 import pprint
 
 import dask.distributed
 import fsspec
 import numpy
 
 import zcollection
@@ -18,44 +19,46 @@
 # %%
 # Initialization of the environment
 # ---------------------------------
 #
 # As in the example of handling
 # :ref:`collections <sphx_glr_auto_examples_ex_collection.py>`, we will create
 # the test environment and a collection.
-def create_dataset():
+def create_dataset() -> zcollection.Dataset:
     """Create a dataset to record."""
-    generator = zcollection.tests.data.create_test_dataset_with_fillvalue()
+    generator: Iterator[zcollection.Dataset] = \
+        zcollection.tests.data.create_test_dataset_with_fillvalue()
     return next(generator)
 
 
 cluster = dask.distributed.LocalCluster(processes=False)
 client = dask.distributed.Client(cluster)
 
-ds = create_dataset()
-fs = fsspec.filesystem('memory')
-collection = zcollection.create_collection('time',
-                                           ds,
-                                           zcollection.partitioning.Date(
-                                               ('time', ), resolution='M'),
-                                           '/view_reference',
-                                           filesystem=fs)
-collection.insert(ds, merge_callable=zcollection.merging.merge_time_series)
+zds: zcollection.Dataset | None = create_dataset()
+assert zds is not None
+fs: fsspec.AbstractFileSystem = fsspec.filesystem('memory')
+collection: zcollection.Collection = zcollection.create_collection(
+    'time',
+    zds,
+    zcollection.partitioning.Date(('time', ), resolution='M'),
+    '/view_reference',
+    filesystem=fs)
+collection.insert(zds, merge_callable=zcollection.merging.merge_time_series)
 
 # %%
 # Creation of views
 # -----------------
 #
 # A :py:class:`view<zcollection.view.View>` allows you to extend a collection
 # (:py:class:`a view reference<zcollection.view.ViewReference>`) that you are
 # not allowed to modify.
-view = zcollection.create_view('/my_view',
-                               zcollection.view.ViewReference(
-                                   '/view_reference', fs),
-                               filesystem=fs)
+view: zcollection.View = zcollection.create_view(
+    '/my_view',
+    zcollection.view.ViewReference('/view_reference', fs),
+    filesystem=fs)
 
 # %%
 # .. note::
 #
 #     The created view can be accessed using the following command ::
 #
 #         >>> view = zcollection.open_view("/my_view", filesystem=fs)
@@ -77,44 +80,45 @@
 except ValueError as err:
     print(err)
 
 # %%
 # Such a state of the view is not very interesting. But it is possible to
 # :py:meth:`add<zcollection.view.View.add_variable>` and modify variables in
 # order to enhance the view.
-var3 = ds.metadata().variables['var2']
-var3.name = 'var3'
-view.add_variable(var3)
+var3_template: zcollection.meta.Variable = zds.metadata().variables['var2']
+var3_template.name = 'var3'
+view.add_variable(var3_template)
+del var3_template
 
 # %%
 # This step creates all necessary partitions for the new variable.
 pprint.pprint(fs.listdir('/my_view/year=2000'))
 
 # %%
 # The new variable is not initialized.
-ds = view.load()
-assert ds is not None
-ds.variables['var3'].values
+zds = view.load()
+assert zds is not None
+zds.variables['var3'].values
 
 # %%
 # The same principle used by the collection allows to
 # :py:meth:`update<zcollection.view.View.update>` the variables.
 view.update(
     lambda ds: dict(var3=ds['var1'].values * 0 + 1))  # type: ignore[arg-type]
 
 # %%
 # Like the :py:meth:`update<zcollection.collection.Collection.update>` method
 # of the collection, the update method of view allows to selecting the
 # neighboring partitions with the keyword argument ``depth``.
 
 # %%
-ds = view.load()
-assert ds is not None
-var3 = ds['var3'].values
-var3
+zds = view.load()
+assert zds is not None
+var3: numpy.ndarray = zds['var3'].values
+print(var3)
 
 # %%
 # **Warning**: The variables of the reference collection cannot be edited.
 try:
     view.update(
         lambda ds: dict(var2=ds['var2'].values * 0))  # type: ignore[arg-type]
 except ValueError as exc:
@@ -148,50 +152,50 @@
         new_size: int,
     ) -> tuple[int, ...]:
         """Compute the new shape of a variable."""
         return tuple(new_size if dim == selected_dim else size
                      for dim, size in zip(var.dimensions, var.shape))
 
     return zcollection.Dataset([
-        zcollection.Variable(
+        zcollection.Array(
             name,
             numpy.resize(var.array.compute(), new_shape(var, dim, size)),
             var.dimensions,
-            var.attrs,
-            var.compressor,
-            var.fill_value,
-            var.filters,
+            attrs=var.attrs,
+            compressor=var.compressor,
+            fill_value=var.fill_value,
+            filters=var.filters,
         ) for name, var in ds.variables.items()
     ])
 
 
 # %%
 # We then modify the last partition of the reference collection. We start by
 # opening the reference collection and loading the last partition.
 collection = zcollection.open_collection('/view_reference',
                                          filesystem=fs,
                                          mode='w')
-ds = collection.load(
+zds = collection.load(
     filters=lambda keys: keys['month'] == 6 and keys['year'] == 2000)
-assert ds is not None
+assert zds is not None
 
 # %%
 # We create a new time variable, resize the dataset and insert the new time
 # values.
 time: numpy.ndarray = numpy.arange(
     numpy.datetime64('2000-06-01T00:00:00'),
     numpy.datetime64('2000-06-30T23:59:59'),
     numpy.timedelta64(1, 'h'),
 )
-ds = resize(ds, 'num_lines', len(time))
-ds['time'].data = time
+zds = resize(zds, 'num_lines', len(time))
+zds['time'].values = time
 
 # %%
 # Finally, we update the partition in the reference collection.
-collection.insert(ds)
+collection.insert(zds)
 
 # %%
 # Now we cannot load the view, because the shape of the last partition is no
 # longer consistent between the reference collection and the view.
 try:
     view.load()
 except ValueError as err:
@@ -211,17 +215,17 @@
 #         lambda ds: dict(var3=ds['var1'].values * 0 + 1),
 #         filters=filters)
 #
 print(tuple(view.partitions(filters=filters)))
 
 # %%
 # The view is now synchronized and can be loaded.
-ds = view.load()
-assert ds is not None
-ds.variables['var3'].values
+zds = view.load()
+assert zds is not None
+zds.variables['var3'].values
 
 # %%
 # Map a function over the view
 # ----------------------------
 # It's possible to map a function over the partitions of the view.
 for partition, array in view.map(lambda ds: (  # type: ignore[arg-type]
         ds['var1'].values + ds['var2'].values)).compute():
```

### Comparing `zcollection-2023.3.2/pylintrc` & `zcollection-2023.5.0/pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module.
-max-module-lines=1200
+max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
```

### Comparing `zcollection-2023.3.2/setup.cfg` & `zcollection-2023.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 keywords = zarr, collection, xarray, dask
 license = BSD License
 license_files = LICENSE
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 name = zcollection
 url = https://github.com/CNES/zcollection
-version = attr: zcollection.__version__
+version = attr: zcollection.version.__version__
 
 [options]
 include_package_data = True
 install_requires = 
 	dask >= 2022.8.0
 	distributed
 	fasteners
```

### Comparing `zcollection-2023.3.2/setup.py` & `zcollection-2023.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/zcollection/__init__.py` & `zcollection-2023.5.0/zcollection/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,52 +3,51 @@
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
 Handle a collection of Zarr groups.
 ===================================
 """
 from . import merging, partitioning
-from .collection import (
-    Collection,
-    Indexer,
-    PartitionFilter,
-    PartitionFilterCallback,
-)
+from .collection import Collection
+from .collection.abc import Indexer, PartitionFilter, PartitionFilterCallback
 from .collection.callable_objects import (
     MapCallable,
     PartitionCallable,
     UpdateCallable,
 )
 from .convenience import (
     create_collection,
     create_view,
     open_collection,
     open_view,
 )
 from .dataset import Dataset
 from .meta import Attribute
-from .variable import Variable
+from .variable import Array, DelayedArray, Variable
 from .version import __version__
-from .view import View, ViewReference
+from .view import View, ViewReference, ViewUpdateCallable
 
-__all__ = [
+__all__ = (
     '__version__',
+    'Array',
     'Attribute',
     'Collection',
     'create_collection',
     'create_view',
     'Dataset',
+    'DelayedArray',
     'Indexer',
     'MapCallable',
     'merging',
     'open_collection',
     'open_view',
     'PartitionCallable',
     'PartitionFilter',
     'PartitionFilterCallback',
     'partitioning',
     'UpdateCallable',
     'Variable',
     'version',
     'View',
     'ViewReference',
-]
+    'ViewUpdateCallable',
+)
```

### Comparing `zcollection-2023.3.2/zcollection/collection/__init__.py` & `zcollection-2023.5.0/zcollection/view/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1141 +1,806 @@
 # Copyright (c) 2023 CNES
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
-Collection of Zarr groups
-=========================
+View on a reference collection.
+===============================
 """
 from __future__ import annotations
 
-from typing import (
-    Any,
-    Callable,
-    ClassVar,
-    Dict,
-    Iterable,
-    Iterator,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
-import datetime
-import functools
-import io
-import itertools
+from typing import Any, ClassVar, Iterable, Iterator, Sequence
+import copy
 import json
 import logging
-import os
 import pathlib
-import types
+import warnings
 
+import dask.array.core
 import dask.bag.core
 import dask.distributed
 import dask.utils
 import fsspec
-import numpy
-import xarray
-import zarr
-import zarr.storage
-
-from .. import (
-    dask_utils,
-    dataset,
-    expression,
-    fs_utils,
-    merging,
-    meta,
-    partitioning,
-    storage,
-    sync,
-)
-from .callable_objects import MapCallable, PartitionCallable, UpdateCallable
+
+from .. import collection, dask_utils, dataset, fs_utils, meta, storage, sync
+from ..collection.callable_objects import MapCallable, PartitionCallable
+from ..collection.detail import _try_infer_callable
+from ..convenience import collection as convenience
+from ..type_hints import ArrayLike
 from .detail import (
-    PartitioningProperties,
-    _insert,
-    _load_and_apply_indexer,
-    _load_dataset,
-    _load_dataset_with_overlap,
+    ViewReference,
+    ViewUpdateCallable,
+    _assert_have_variables,
+    _assert_variable_handled,
+    _create_zarr_array,
+    _deserialize_filters,
+    _drop_zarr_zarr,
+    _load_datasets_list,
+    _load_one_dataset,
+    _select_overlap,
+    _serialize_filters,
+    _sync,
     _wrap_update_func,
-    _wrap_update_func_with_overlap,
-    try_infer_callable,
+    _wrap_update_func_overlap,
+    _write_checksum,
 )
 
-#: Type of functions filtering the partitions.
-PartitionFilterCallback = Callable[[Dict[str, int]], bool]
-
-#: Type of argument to filter the partitions.
-PartitionFilter = Optional[Union[str, PartitionFilterCallback]]
-
-#: Indexer's type.
-Indexer = Iterable[Tuple[Tuple[Tuple[str, int], ...], slice]]
-
-#: Name of the directory storing the immutable dataset.
-_IMMUTABLE = '.immutable'
+__all__ = ('View', 'ViewReference')
 
 #: Module logger.
 _LOGGER = logging.getLogger(__name__)
 
 
-def variables(
-    metadata: meta.Dataset,
-    selected_variables: Iterable[str] | None = None
-) -> tuple[dataset.Variable, ...]:
-    """Return the variables defined in the dataset.
-
-    Args:
-        metadata: Metadata dataset containing variables information.
-        selected_variables: The variables to return. If None, all the
-            variables are returned.
-
-    Returns:
-        The variables defined in the dataset.
-    """
-    selected_variables = selected_variables or metadata.variables.keys()
-    return tuple(
-        dataset.Variable(
-            v.name, numpy.ndarray((0, ) * len(v.dimensions), v.dtype),
-            v.dimensions, v.attrs, v.compressor, v.fill_value, v.filters)
-        for k, v in metadata.variables.items() if k in selected_variables)
-
-
-def build_indexer_args(
-    collection: Collection,
-    filters: PartitionFilter,
-    indexer: Indexer,
-    partitions: Iterable[str] | None = None,
-) -> Iterator[tuple[tuple[tuple[str, int], ...], list[slice]]]:
-    """Build the arguments for the indexer.
-
-    Args:
-        collection: The collection to index.
-        filters: The partition filters.
-        indexer: The indexer.
-        partitions: The partitions to index. If None, all the partitions
-            are indexed.
-
-    Returns:
-        An iterator containing the arguments for the indexer.
-    """
-    # Build an indexer dictionary between the partition scheme and
-    # indexer.
-    indexers_map: dict[tuple[tuple[str, int], ...], list[slice]] = {}
-    _ = {
-        indexers_map.setdefault(  # type: ignore[func-returns-value]
-            partition_scheme, []).append(indexer)
-        for partition_scheme, indexer in indexer
-    }
-    # Filter the selected partitions
-    partitions = partitions or collection.partitions(filters=filters)
-    selected_partitions = set(indexers_map) & {
-        collection.partitioning.parse(item)
-        for item in partitions
-    }
-
-    # For each provided partition scheme, retrieves the corresponding
-    # indexer.
-    return ((item, indexers_map[item]) for item in sorted(selected_partitions))
-
-
-def _immutable_path(
-    ds: meta.Dataset,
-    partition_properties: PartitioningProperties,
-) -> str | None:
-    """Return the immutable path of the dataset.
-
-    Args:
-        ds: The dataset to process.
-        partition_properties: The partitioning properties.
-
-    Returns:
-        The immutable path of the dataset containing data that are immutable
-        relative to the partitioning or None if the dataset does not contain
-        immutable data.
-    """
-    return fs_utils.join_path(
-        partition_properties.dir, _IMMUTABLE) if ds.select_variables_by_dims(
-            (partition_properties.dim, ), predicate=False) else None
-
-
-def _write_immutable_dataset(
-    ds: dataset.Dataset,
-    axis: str,
-    path: str,
-    fs: fsspec.AbstractFileSystem,
-    synchronizer: sync.Sync,
-) -> None:
-    """Write the immutable dataset.
+class View:
+    """View on a reference collection.
 
     Args:
-        ds: The dataset to write.
-        axis: The partitioning axis.
-        path: The path to the immutable dataset.
-        fs: The file system that the partition is stored on.
+        base_dir: Path to the directory where the view is stored.
+        view_ref: Access properties for the reference view.
+        ds: The dataset handled by this view.
+        filesystem: The file system used to access the view.
+        filters: The filters used to select the partitions of the reference. If
+            not provided, all partitions are selected.
+        synchronizer: The synchronizer used to synchronize the view.
+
+    Note:
+        Normally, you should not call this constructor directly. Instead, use
+        :func:`create_view <zcollection.create_view>` or :func:`open_view
+        <zcollection.open_view>` to create or open a view.
     """
-    immutable_dataset = ds.select_variables_by_dims((axis, ), predicate=False)
-    assert len(immutable_dataset.variables) != 0, (
-        'The dataset to insert does not contain any variable '
-        'that is not split.')
-    _LOGGER.info('Creating the immutable dataset: %s', path)
-    storage.write_zarr_group(immutable_dataset,
-                             path,
-                             fs,
-                             synchronizer,
-                             parallel=False)
-
-
-class Collection:
-    """This class manages a collection of files in Zarr format stored in a set
-    of subdirectories. These subdirectories split the data, by cycles or dates
-    for example, in order to optimize access and updates, deletion or addition
-    of new data.
-
-    Args:
-        axis: The axis of the collection.
-        ds: The dataset containing the collection.
-        partition_handler: The partitioning strategy for the collection.
-        partition_base_dir: The base directory for the collection.
-        mode: The mode of the collection.
-        filesystem: The filesystem to use for the collection.
-        synchronizer: The synchronizer to use for the collection.
-
-    Raises:
-        ValueError: If the axis does not exist in the dataset, if the
-            partition key is not defined in the dataset or if the access mode
-            is not supported.
-
-    .. note::
-
-        On the first call to the constructor, the dataset given as an argument
-        is used to create the metadata of the collection. This information is
-        used to validate datasets that are inserted in the collection.
-
-        Normally, this class is not instantiated directly but through the
-        :py:meth:`create_collection <zcollection.create_collection>` and
-        :py:meth:`open_collection <zcollection.open_collection>` methods of this
-        library.
-    """
-    #: Configuration filename of the collection.
-    CONFIG: ClassVar[str] = '.zcollection'
+    #: Configuration filename of the view.
+    CONFIG: ClassVar[str] = '.view'
 
     def __init__(
         self,
-        axis: str,
-        ds: meta.Dataset,
-        partition_handler: partitioning.Partitioning,
-        partition_base_dir: str,
+        base_dir: str,
+        view_ref: ViewReference,
         *,
-        mode: str | None = None,
+        ds: meta.Dataset | None,
         filesystem: fsspec.AbstractFileSystem | str | None = None,
+        filters: collection.PartitionFilter = None,
         synchronizer: sync.Sync | None = None,
     ) -> None:
-        if axis not in ds.variables:
-            raise ValueError(
-                f'The variable {axis!r} is not defined in the dataset.')
-
-        for varname in partition_handler.variables:
-            if varname not in ds.variables:
-                raise ValueError(
-                    f'The partitioning key {varname!r} is not defined in '
-                    'the dataset.')
+        #: The file system used to access the view (default local file system).
+        self.fs: fsspec.AbstractFileSystem = fs_utils.get_fs(filesystem)
+        #: Path to the directory where the view is stored.
+        self.base_dir: str = fs_utils.normalize_path(self.fs, base_dir)
+        #: The reference collection of the view.
+        self.view_ref: collection.Collection = convenience.open_collection(
+            view_ref.path, mode='r', filesystem=view_ref.filesystem)
+        #: The metadata of the variables handled by the view.
+        self.metadata: meta.Dataset = ds or meta.Dataset(
+            self.view_ref.metadata.dimensions, variables=[], attrs=[])
+        #: The synchronizer used to synchronize the view.
+        self.synchronizer: sync.Sync = synchronizer or sync.NoSync()
+        #: The filters used to select the partitions of the reference.
+        self.filters = filters
+
+        if not self.fs.exists(self.base_dir):
+            _LOGGER.info('Creating view %s', self)
+            self.fs.makedirs(self.base_dir)
+            self._write_config()
+            self._init_partitions(filters)
+        else:
+            _LOGGER.info('Opening view %s', self)
 
-        mode = mode or 'w'
-        if mode not in ('r', 'w'):
-            raise ValueError(f'The mode {mode!r} is not supported.')
-
-        #: The axis of the collection.
-        self.axis = axis
-        #: The metadata that describes the dataset handled by the collection.
-        self.metadata = ds
-        #: The file system used to read/write the collection.
-        self.fs = fs_utils.get_fs(filesystem)
-        #: The partitioning strategy used to split the data.
-        self.partitioning = partition_handler
-        #: The partitioning properties (base directory and dimension).
-        self.partition_properties = PartitioningProperties(
-            fs_utils.normalize_path(self.fs, partition_base_dir),
-            ds.variables[axis].dimensions[0],
-        )
-        #: The access mode of the collection.
-        self.mode = mode
-        #: The synchronizer used to synchronize the modifications.
-        self.synchronizer = synchronizer or sync.NoSync()
-        #: The path to the dataset that contains the immutable data relative
-        #: to the partitioning.
-        self._immutable = _immutable_path(ds, self.partition_properties)
-
-        self._write_config(skip_if_exists=True)
-
-        if mode == 'r':
-            # pylint: disable=method-hidden
-            # These methods are overloaded when the collection is opened in
-            # readonly.
-            for item in [
-                    'add_variable',
-                    'drop_partitions',
-                    'drop_variable',
-                    'insert',
-                    'update',
-            ]:
-                assert hasattr(self, item), f'{item} is not a known method.'
-                setattr(
-                    self, item,
-                    types.MethodType(Collection._unsupported_operation, self))
-            # pylint: enable=method-hidden
-
-    @property
-    def immutable(self) -> bool:
-        """Return True if the collection contains immutable data relative to
-        the partitioning."""
-        return self._immutable is not None
+    def _init_partitions(self, filters: collection.PartitionFilter) -> None:
+        """Initialize the partitions of the view."""
+        _LOGGER.info('Populating view %s', self)
+        args = tuple(
+            map(lambda item: fs_utils.join_path(self.base_dir, item),
+                self.view_ref.partitions(filters=filters, relative=True)))
+        # When opening an existing view, if the user asks to use new partitions
+        # from the reference collection, in this case only the missing
+        # partitions are created.
+        args = tuple(filter(lambda item: not self.fs.exists(item), args))
+        _LOGGER.info('%d partitions selected from %s', len(args),
+                     self.view_ref)
+        client: dask.distributed.Client = dask_utils.get_client()
+        storage.execute_transaction(
+            client, self.synchronizer,
+            client.map(
+                _write_checksum,
+                tuple(args),
+                base_dir=self.base_dir,
+                view_ref=self.view_ref,
+                fs=self.fs,
+            ))
 
     def __str__(self) -> str:
         return (f'{self.__class__.__name__}'
                 f'<filesystem={self.fs.__class__.__name__!r}, '
-                f'partition_base_dir={self.partition_properties.dir!r}, '
-                f'mode={self.mode!r}>')
-
-    @staticmethod
-    def _unsupported_operation(*args, **kwargs):
-        """Raise an exception if the operation is not supported."""
-        raise io.UnsupportedOperation('not writable')
+                f'base_dir={self.base_dir!r}>')
 
     @classmethod
-    def _config(cls, partition_base_dir: str) -> str:
-        """Return the configuration path."""
-        return fs_utils.join_path(partition_base_dir, cls.CONFIG)
-
-    def _write_config(self, skip_if_exists: bool = False) -> None:
-        """Write the configuration file."""
-        base_dir = self.partition_properties.dir
-        config = self._config(base_dir)
-        exists = self.fs.exists(config)
-
-        if skip_if_exists and exists:
-            return
-
-        message = ("Updating collection's configuration: %s"
-                   if exists else 'Creating the collection: %s')
-        _LOGGER.info(message, config)
-
-        self.fs.makedirs(base_dir, exist_ok=True)
-
-        params = {
-            'axis': self.axis,
-            'dataset': self.metadata.get_config(),
-            'partitioning': self.partitioning.get_config(),
-        }
-
+    def _config(cls, base_dir: str) -> str:
+        """Returns the configuration path."""
+        return fs_utils.join_path(base_dir, cls.CONFIG)
+
+    def _write_config(self) -> None:
+        """Write the configuration file for the view."""
+        config: str = self._config(self.base_dir)
+        fs: dict[str, Any] = json.loads(self.view_ref.fs.to_json())
         with self.fs.open(config, mode='w') as stream:
-            json.dump(params, stream, indent=4)  # type: ignore[arg-type]
-
-    def is_readonly(self) -> bool:
-        """Return True if the collection is read-only."""
-        return self.mode == 'r'
-
-    def is_locked(self) -> bool:
-        """Return True if the collection is locked."""
-        return self.synchronizer.is_locked()
+            json.dump(
+                {
+                    'base_dir': self.base_dir,
+                    'filters': _serialize_filters(self.filters),
+                    'metadata': self.metadata.get_config(),
+                    'view_ref': {
+                        'path': self.view_ref.partition_properties.dir,
+                        'fs': fs,
+                    },
+                },
+                stream,  # type: ignore[arg-type]
+                indent=4)
+        self.fs.invalidate_cache(config)
 
     @classmethod
     def from_config(
         cls,
         path: str,
         *,
-        mode: str | None = None,
         filesystem: fsspec.AbstractFileSystem | str | None = None,
         synchronizer: sync.Sync | None = None,
-    ) -> Collection:
-        """Open a Collection described by a configuration file.
+    ) -> View:
+        """Open a View described by a configuration file.
 
         Args:
             path: The path to the configuration file.
-            mode: The mode of the collection.
-            filesystem: The filesystem to use for the collection.
-            synchronizer: The synchronizer to use for the collection.
+            filesystem: The filesystem to use for the view.
+            synchronizer: The synchronizer to use for the view.
 
         Returns:
-            The collection.
+            The view.
 
         Raises:
-            ValueError: If the provided directory does not contain a collection.
+            ValueError: If the provided directory does not contain a view.
         """
-        _LOGGER.info('Opening collection: %r', path)
-        fs = fs_utils.get_fs(filesystem)
-        config = cls._config(path)
+        _LOGGER.info('Opening view %r', path)
+        fs: fsspec.AbstractFileSystem = fs_utils.get_fs(filesystem)
+        config: str = cls._config(path)
         if not fs.exists(config):
-            raise ValueError(f'zarr collection not found at path {path!r}')
+            raise ValueError(f'zarr view not found at path {path!r}')
         with fs.open(config) as stream:
-            data = json.load(stream)
-        return Collection(
-            data['axis'],
-            meta.Dataset.from_config(data['dataset']),
-            partitioning.get_codecs(data['partitioning']),
-            path,
-            mode=mode or 'r',
-            filesystem=fs,
-            synchronizer=synchronizer,
-        )
+            data: dict[str, Any] = json.load(stream)
+
+        view_ref: dict[str, Any] = data['view_ref']
+        return View(data['base_dir'],
+                    ViewReference(
+                        view_ref['path'],
+                        fsspec.AbstractFileSystem.from_json(
+                            json.dumps(view_ref['fs']))),
+                    ds=meta.Dataset.from_config(data['metadata']),
+                    filesystem=filesystem,
+                    filters=_deserialize_filters(data['filters']),
+                    synchronizer=synchronizer)
 
-    def _is_selected(
+    def partitions(
         self,
-        partition: Sequence[str],
-        expr: Callable[[dict[str, int]], bool] | None,
-    ) -> bool:
-        """Return whether the partition is selected.
+        filters: collection.PartitionFilter = None,
+    ) -> Iterator[str]:
+        """Returns the list of partitions in the view.
 
         Args:
-            partition: The partition to check.
-            expr: The expression used to filter the partition.
+            filters: The partition filters.
 
         Returns:
-            Whether the partition is selected.
+            The list of partitions.
         """
-        if expr is not None:
-            return expr(dict(self.partitioning.parse('/'.join(partition))))
-        return True
+        return filter(
+            self.fs.exists,
+            map(lambda item: fs_utils.join_path(self.base_dir, item),
+                self.view_ref.partitions(filters=filters, relative=True)))
 
-    # pylint: disable=method-hidden
-    def insert(
+    def variables(
         self,
-        ds: xarray.Dataset | dataset.Dataset,
-        *,
-        merge_callable: merging.MergeCallable | None = None,
-        npartitions: int | None = None,
-        validate: bool = False,
+        selected_variables: Iterable[str] | None = None
+    ) -> tuple[dataset.Variable, ...]:
+        """Return the variables of the view.
+
+        Args:
+            selected_variables: The variables to return. If None, all the
+                variables are returned.
+
+        Returns:
+            The variables of the view.
+        """
+        return dataset.get_dataset_variable_properties(self.metadata,
+                                                       selected_variables)
+
+    def add_variable(
+        self,
+        variable: meta.Variable | dataset.Variable,
     ) -> None:
-        """Insert a dataset into the collection.
+        """Add a variable to the view.
 
         Args:
-            ds: The dataset to insert.
-            merge_callable: The function to use to merge the existing data set
-                already stored in partitions with the new partitioned data. If
-                None, the new partitioned data overwrites the existing
-                partitioned data.
-            npartitions: The maximum number of partitions to process in
-                parallel. By default, partitions are processed one by one.
-            validate: Whether to validate dataset metadata before insertion
-                or not.
-
-        .. warning::
-
-            Each worker will process a set of independent partitions. However,
-            be careful, two different partitions can use the same file (chunk),
-            therefore, the library that handles the storage of Dask arrays
-            (HDF5, NetCDF, Zarr, etc.) must be compatible with concurrent
-            access.
+            variable: The variable to add
 
         Raises:
-            ValueError: If the dataset mismatched the definition of the
-                collection.
+            ValueError: If the variable already exists
+
+        Example:
+            >>> view.add_variable(
+            ...    zcollection.meta.Variable(
+            ...        "temperature",
+            ...        "float32", ("time", "lat", "lon"),
+            ...        (zcollection.meta.Attribute("units", "degrees Celsius"),
+            ...         zcollection.meta.Attribute("long_name", "temperature")),
+            ...        fill_value=-9999.0))
         """
-        # pylint: disable=method-hidden
-        if isinstance(ds, xarray.Dataset):
-            ds = dataset.Dataset.from_xarray(ds)
-
-        _LOGGER.info('Inserting of a %s dataset in the collection',
-                     dask.utils.format_bytes(ds.nbytes))
-
-        missing_variables = self.metadata.missing_variables(ds.metadata())
-        for item in missing_variables:
-            variable = self.metadata.variables[item]
-            ds.add_variable(variable)
-
-        if validate and not ds.metadata() == self.metadata:
-            raise ValueError(
-                "Provided dataset's metadata do not match the collection's ones"
-            )
-        ds = ds.set_for_insertion(ds=self.metadata)
-        client = dask_utils.get_client()
+        # pylint: disable=duplicate-code
+        # false positive, no code duplication
+
+        variable = dataset.get_variable_metadata(variable)
+        _LOGGER.info('Adding variable %r in the view', variable.name)
+        if (variable.name in self.view_ref.metadata.variables
+                or variable.name in self.metadata.variables):
+            raise ValueError(f'Variable {variable.name} already exists')
+        client: dask.distributed.Client = dask_utils.get_client()
+        self.metadata.add_variable(variable)
+        template: meta.Variable = \
+            self.view_ref.metadata.search_same_dimensions_as(variable)
+
+        existing_partitions: set[str] = {
+            pathlib.Path(path).relative_to(self.base_dir).as_posix()
+            for path in self.partitions()
+        }
+
+        if len(existing_partitions) == 0:
+            _LOGGER.info('No partitions found, skipping variable creation')
+            return
 
-        # If the dataset contains variables that should not be partitioned.
-        if self._immutable is not None:
+        args = filter(lambda item: item[0] in existing_partitions,
+                      self.view_ref.iterate_on_records(relative=True))
 
-            # On the first call, we store the immutable variables in
-            # a directory located at the root of the collection.
-            if not self.fs.exists(self._immutable):
-                _write_immutable_dataset(ds, self.axis, self._immutable,
-                                         self.fs, self.synchronizer)
-
-            # Remove the variables that should not be partitioned.
-            ds = ds.select_variables_by_dims((self.axis, ))
-
-        # Process the partitions to insert or update by batches to avoid
-        # memory issues.
-        partitions = tuple(
-            self.partitioning.split_dataset(ds, self.partition_properties.dim))
-
-        if npartitions is not None:
-            if npartitions < 1:
-                raise ValueError('The number of partitions must be positive')
-            npartitions = len(partitions) // npartitions + 1
-
-        scattered_ds = client.scatter(ds)
-        for sequence in dask_utils.split_sequence(partitions, npartitions):
-            futures = [
-                dask_utils.simple_delayed('insert', _insert)(
-                    partition,  # type: ignore[arg-type]
-                    axis=self.axis,
-                    ds=scattered_ds,
-                    fs=self.fs,
-                    merge_callable=merge_callable,
-                    partitioning_properties=self.partition_properties,
-                ) for partition in sequence
-            ]
-            storage.execute_transaction(client,
-                                        self.synchronizer,
-                                        futures,
-                                        sync=True)
+        # Remove the attribute from the variable. The attribute will be added
+        # from the view metadata.
+        # Remove the attribute from the variable. The attribute will be added
+        # from the collection metadata.
+        variable = variable.set_for_insertion()
 
-    def _relative_path(self, path: str) -> str:
-        """Return the relative path to the collection.
+        try:
+            storage.execute_transaction(
+                client, self.synchronizer,
+                client.map(_create_zarr_array,
+                           tuple(args),
+                           base_dir=self.base_dir,
+                           fs=self.fs,
+                           template=template.name,
+                           variable=variable))
+        except Exception:
+            storage.execute_transaction(
+                client, self.synchronizer,
+                client.map(_drop_zarr_zarr,
+                           tuple(self.partitions()),
+                           fs=self.fs,
+                           variable=variable.name,
+                           ignore_errors=True))
+            raise
+
+        self._write_config()
+        # pylint: enable=duplicate-code
+
+    def drop_variable(
+        self,
+        varname: str,
+    ) -> None:
+        """Drop a variable from the view.
 
         Args:
-            path: The path to the dataset.
+            varname: The name of the variable to drop.
 
-        Returns:
-            The relative path to the collection.
+        Raise:
+            ValueError: If the variable does not exist or if the variable
+                belongs to the reference collection.
+
+        Example:
+            >>> view.drop_variable("temperature")
         """
-        return pathlib.Path(path).relative_to(
-            self.partition_properties.dir).as_posix()
+        _LOGGER.info('Dropping variable %r', varname)
+        _assert_variable_handled(self.view_ref.metadata, self.metadata,
+                                 varname)
+        client: dask.distributed.Client = dask_utils.get_client()
 
-    def partitions(
+        variable: meta.Variable = self.metadata.variables.pop(varname)
+        self._write_config()
+
+        storage.execute_transaction(
+            client, self.synchronizer,
+            client.map(_drop_zarr_zarr,
+                       tuple(self.partitions()),
+                       fs=self.fs,
+                       variable=variable.name))
+
+    def load(
         self,
         *,
-        lock: bool = False,
-        filters: PartitionFilter = None,
-        relative: bool = False,
-    ) -> Iterator[str]:
-        """List the partitions of the collection.
+        delayed: bool = True,
+        filters: collection.PartitionFilter = None,
+        indexer: collection.abc.Indexer | None = None,
+        selected_variables: Iterable[str] | None = None,
+    ) -> dataset.Dataset | None:
+        """Load the view.
 
         Args:
-            lock: Whether to lock the collection or not to avoid listing
-                partitions while the collection is being modified.
-            filters: The predicate used to filter the partitions to load. If
-                the predicate is a string, it is a valid python expression to
-                filter the partitions, using the partitioning scheme as
-                variables. If the predicate is a function, it is a function
-                that takes the partition scheme as input and returns a boolean.
-            relative: Whether to return the relative path.
+            delayed: Whether to load data in a dask array or not.
+            filters: The predicate used to filter the partitions to select.
+                To get more information on the predicate, see the
+                documentation of the :meth:`Collection.partitions
+                <zcollection.collection.Collection.partitions>` method.
+            indexer: The indexer to apply.
+            selected_variables: A list of variables to retain from the view.
+                If None, all variables are loaded.
 
         Returns:
-            The list of partitions.
+            The dataset.
 
         Example:
-            >>> tuple(collection.partitions(
-            ...     filters="year == 2019 and month == 1"))
-            ('year=2019/month=01/day=01', 'year=2019/month=01/day=02/', ...)
-            >>> tuple(collection.partitions(
-            ...     filters=lambda x: x["year"] == 2019 and x["month"] == 1))
-            ('year=2019/month=01/day=01', 'year=2019/month=01/day=02/', ...)
-        """
-        if isinstance(filters, str):
-            expr: Any = expression.Expression(filters)
-        elif callable(filters):
-            expr = filters
-        else:
-            expr = None
-
-        base_dir = self.partition_properties.dir
-        sep = self.fs.sep
-
-        if lock:
-            with self.synchronizer:
-                partitions: Iterable[str] = tuple(
-                    self.partitioning.list_partitions(self.fs, base_dir))
+            >>> view.load()
+            >>> view.load(filters="time == '2020-01-01'")
+            >>> view.load(filters=lambda x: x["time"] == "2020-01-01")
+        """
+        _assert_have_variables(self.metadata)
+        if indexer is not None:
+            arguments = tuple(
+                collection.abc.build_indexer_args(
+                    self.view_ref,
+                    filters,
+                    indexer,
+                    partitions=self.partitions()))
+            if len(arguments) == 0:
+                return None
         else:
-            partitions = self.partitioning.list_partitions(self.fs, base_dir)
+            arguments = tuple((self.view_ref.partitioning.parse(item), [])
+                              for item in self.partitions(filters=filters))
 
-        for item in partitions:
-            if item == self._immutable:
-                continue
-            # Filtering on partition names
-            partitions = item.replace(base_dir, '')
-            entry = partitions.split(sep)
-
-            if self._is_selected(entry, expr):
-                yield self._relative_path(item) if relative else item
+        client: dask.distributed.Client = dask_utils.get_client()
+        futures: list[dask.distributed.Future] = client.map(
+            _load_one_dataset,
+            arguments,
+            base_dir=self.base_dir,
+            delayed=delayed,
+            fs=self.fs,
+            selected_variables=self.view_ref.metadata.select_variables(
+                selected_variables),
+            view_ref=client.scatter(self.view_ref),
+            variables=self.metadata.select_variables(selected_variables))
+
+        # The load function returns the path to the partitions and the loaded
+        # datasets. Only the loaded datasets are retrieved here and filter None
+        # values corresponding to empty partitions.
+        arrays: list[dataset.Dataset] = list(
+            map(
+                lambda item: item[0],  # type: ignore[arg-type]
+                filter(lambda item: item is not None,
+                       client.gather(futures))))  # type: ignore[arg-type]
+        if arrays:
+            array: dataset.Dataset = arrays.pop(0)
+            if arrays:
+                array = array.concat(arrays,
+                                     self.view_ref.partition_properties.dim)
+            metadata: meta.Dataset = copy.deepcopy(self.view_ref.metadata)
+            metadata.variables.update(self.metadata.variables.items())
+            array.fill_attrs(metadata)
+            return array
+        return None
 
-    # pylint: disable=method-hidden
-    def drop_partitions(
+    def update(
         self,
-        *,
-        filters: PartitionFilter = None,
-        timedelta: datetime.timedelta | None = None,
+        func: collection.UpdateCallable,
+        /,
+        *args,
+        depth: int = 0,
+        delayed: bool = True,
+        filters: collection.PartitionFilter = None,
+        npartitions: int | None = None,
+        selected_variables: Iterable[str] | None = None,
+        trim: bool = True,
+        **kwargs,
     ) -> None:
-        # pylint: disable=method-hidden
-        """Drop the selected partitions.
+        """Update a variable stored int the view.
 
         Args:
+            func: The function to apply to calculate the new values for the
+                target variables.
+            depth: The depth of the overlap between the partitions. Default is
+                0 (no overlap). If depth is greater than 0, the function is
+                applied on the partition and its neighbors selected by the
+                depth. If ``func`` accepts a partition_info as a keyword
+                argument, it will be passed a tuple with the name of the
+                partitioned dimension and the slice allowing getting in the
+                dataset the selected partition without the overlap.
+            delayed: Whether to load data in a dask array or in memory.
             filters: The predicate used to filter the partitions to drop.
                 To get more information on the predicate, see the
-                documentation of the :meth:`partitions` method.
-            timedelta: Select the partitions created before the
-                specified time delta relative to the current time.
+                documentation of the :meth:`Collection.partitions
+                <zcollection.collection.Collection.partitions>` method.
+            npartitions: The number of partitions to update in parallel. By
+                default, it is equal to the number of Dask workers available
+                when calling this method.
+            selected_variables: A list of variables to retain from the view.
+                If None, all variables are loaded. Useful to load only a
+                subset of the view.
+            trim: Whether to trim ``depth`` items from each partition after
+                calling ``func``. Set it to ``False`` if your function does
+                this for you.
+            args: The positional arguments to pass to the function.
+            kwargs: The keyword arguments to pass to the function.
+
+        Raises:
+            ValueError: If the variable does not exist or if the variable
+                belongs to the reference collection.
+            ValueError: If the depth is greater than 0 and the selected
+                variables does not contain the variables updated by the
+                function.
 
         Example:
-            >>> collection.drop_partitions(filters="year == 2019")
-            >>> collection.drop_partitions(
-            ...     timedelta=datetime.timedelta(days=30))
-        """
-        now = datetime.datetime.now()
-        client = dask_utils.get_client()
-        folders = list(self.partitions(filters=filters, lock=True))
-
-        def is_created_before(path: str) -> bool:
-            created = self.fs.created(path)
-            return now - created > timedelta
+            >>> def temp_celsius_to_kelvin(
+            ...     dataset: zcollection.dataset.Dataset,
+            ... ) -> Dict[str, numpy.ndarray]:
+            ...     return dict(
+            ...         temperature_kelvin=dataset["temperature"].values + 273,
+            ...         15)
+            >>> view.update(update_temperature)
+        """
+        _assert_have_variables(self.metadata)
+
+        client: dask.distributed.Client = dask_utils.get_client()
+
+        datasets_list = tuple(
+            _load_datasets_list(client=client,
+                                base_dir=self.base_dir,
+                                delayed=delayed,
+                                fs=self.fs,
+                                view_ref=self.view_ref,
+                                metadata=self.metadata,
+                                partitions=self.partitions(filters),
+                                selected_variables=selected_variables))
+
+        # If no dataset is selected, we have nothing to do.
+        if not datasets_list:
+            warnings.warn('The update function is not applied because no '
+                          'data is selected with the given filters.')
+            return
 
-        if timedelta is not None:
-            folders = list(filter(is_created_before, folders))
+        func_result: dict[str, ArrayLike] = _try_infer_callable(
+            func, datasets_list[0][0], self.view_ref.partition_properties.dim,
+            *args, **kwargs)
+        tuple(
+            map(
+                lambda varname: _assert_variable_handled(
+                    self.view_ref.metadata, self.metadata, varname),
+                func_result))
+        _LOGGER.info('Updating variable %s',
+                     ', '.join(repr(item) for item in func_result))
 
-        storage.execute_transaction(
-            client, self.synchronizer,
-            client.map(self.fs.rm, folders, recursive=True))
+        # Function to apply to each partition.
+        wrap_function: ViewUpdateCallable
 
-        def invalidate_cache(path):
-            """Invalidate the cache."""
-            _LOGGER.info('Dropped partition: %s', path)
-            self.fs.invalidate_cache(path)
+        # Wrap the function to apply to each partition.
+        if depth == 0:
+            wrap_function = _wrap_update_func(
+                func,
+                self.fs,
+                *args,
+                **kwargs,
+            )
+        else:
+            if selected_variables is not None and len(
+                    set(func_result) & set(selected_variables)) == 0:
+                raise ValueError(
+                    'If the depth is greater than 0, the selected variables '
+                    'must contain the variables updated by the function.')
 
-        tuple(map(invalidate_cache, folders))
+            wrap_function = _wrap_update_func_overlap(
+                datasets_list,
+                depth,
+                func,
+                self.fs,
+                self.view_ref,
+                trim,
+                *args,
+                **kwargs,
+            )
+
+        batchs: Iterator[Sequence[Any]] = dask_utils.split_sequence(
+            datasets_list, npartitions
+            or dask_utils.dask_workers(client, cores_only=True))
+        awaitables: list[dask.distributed.Future] = client.map(
+            wrap_function,
+            tuple(batchs),
+            key=func.__name__,
+            base_dir=self.base_dir)
+        storage.execute_transaction(client, self.synchronizer, awaitables)
 
     # pylint: disable=duplicate-code
     # false positive, no code duplication
     def map(
         self,
         func: MapCallable,
+        /,
         *args,
-        filters: PartitionFilter = None,
+        delayed: bool = True,
+        filters: collection.PartitionFilter = None,
         partition_size: int | None = None,
         npartitions: int | None = None,
-        selected_variables: Sequence[str] | None = None,
+        selected_variables: Iterable[str] | None = None,
         **kwargs,
     ) -> dask.bag.core.Bag:
-        """Map a function over the partitions of the collection.
+        """Map a function over the partitions of the view.
 
         Args:
-            func: The function to apply to every partition of the collection.
+            func: The function to apply to every partition of the view.
             *args: The positional arguments to pass to the function.
+            delayed: Whether to load data in a dask array or in memory.
             filters: The predicate used to filter the partitions to process.
                 To get more information on the predicate, see the
-                documentation of the :meth:`partitions` method.
+                documentation of the :meth:`zcollection.Collection.partitions`
+                method.
             partition_size: The length of each bag partition.
             npartitions: The number of desired bag partitions.
-            selected_variables: A list of variables to retain from the
-                collection. If None, all variables are kept.
+            selected_variables: A list of variables to retain from the view.
+                If None, all variables are loaded. Useful to load only a
+                subset of the view.
             **kwargs: The keyword arguments to pass to the function.
 
         Returns:
             A bag containing the tuple of the partition scheme and the result
             of the function.
 
         Example:
-            >>> futures = collection.map(
+            >>> futures = view.map(
             ...     lambda x: (x["var1"] + x["var2"]).values)
             >>> for item in futures:
             ...     print(item)
             [1.0, 2.0, 3.0, 4.0]
             [5.0, 6.0, 7.0, 8.0]
         """
 
         def _wrap(
-            partition: str,
+            arguments: tuple[dataset.Dataset, str],
             func: PartitionCallable,
-            selected_variables: Sequence[str] | None,
             *args,
             **kwargs,
         ) -> tuple[tuple[tuple[str, int], ...], Any]:
             """Wraps the function to apply on the partition.
 
             Args:
+                arguments: The partition scheme and the dataset.
                 func: The function to apply.
-                partition: The partition to apply the function on.
-                selected_variables: The list of variables to retain from the
-                    partition.
                 *args: The positional arguments to pass to the function.
                 **kwargs: The keyword arguments to pass to the function.
 
             Returns:
                 The result of the function.
             """
-            ds = _load_dataset(self.fs, self._immutable, partition,
-                               selected_variables)
-            return self.partitioning.parse(partition), func(
-                ds, *args, **kwargs)
-
-        if not callable(func):
-            raise TypeError('func must be a callable')
-
-        bag = dask.bag.core.from_sequence(self.partitions(filters=filters),
-                                          partition_size=partition_size,
-                                          npartitions=npartitions)
-        return bag.map(_wrap, func, selected_variables, *args, **kwargs)
+            zds: dataset.Dataset
+            partition: str
+
+            zds, partition = arguments
+            return self.view_ref.partitioning.parse(partition), func(
+                zds, *args, **kwargs)
+
+        _assert_have_variables(self.metadata)
+
+        client: dask.distributed.Client = dask_utils.get_client()
+        datasets_list = tuple(
+            _load_datasets_list(client=client,
+                                base_dir=self.base_dir,
+                                delayed=delayed,
+                                fs=self.fs,
+                                view_ref=self.view_ref,
+                                metadata=self.metadata,
+                                partitions=self.partitions(filters),
+                                selected_variables=selected_variables))
+        bag: dask.bag.core.Bag = dask.bag.core.from_sequence(
+            datasets_list,
+            partition_size=partition_size,
+            npartitions=npartitions)
+        return bag.map(_wrap, func, *args, **kwargs)
         # pylint: enable=duplicate-code
 
     def map_overlap(
         self,
         func: MapCallable,
-        depth: int,
+        /,
         *args,
-        filters: PartitionFilter = None,
+        depth: int = 1,
+        delayed: bool = True,
+        filters: collection.PartitionFilter = None,
         partition_size: int | None = None,
-        npartition: int | None = None,
-        selected_variables: Sequence[str] | None = None,
+        npartitions: int | None = None,
+        selected_variables: Iterable[str] | None = None,
         **kwargs,
     ) -> dask.bag.core.Bag:
-        """Map a function over the partitions of the collection with some
-        overlap.
+        """Map a function over the partitions of the view with some overlap.
 
         Args:
-            func: The function to apply to every partition of the collection.
-                If ``func`` accepts a partition_info as a keyword
+            func: The function to apply to every partition of the view.
+            depth: The depth of the overlap between the partitions. Default is
+                0 (no overlap). If depth is greater than 0, the function is
+                applied on the partition and its neighbors selected by the
+                depth. If ``func`` accepts a partition_info as a keyword
                 argument, it will be passed a tuple with the name of the
                 partitioned dimension and the slice allowing getting in the
                 dataset the selected partition without the overlap.
-            depth: The depth of the overlap between the partitions.
             *args: The positional arguments to pass to the function.
+            delayed: Whether to load data in a dask array or in memory.
             filters: The predicate used to filter the partitions to process.
                 To get more information on the predicate, see the
-                documentation of the :meth:`partitions` method.
+                documentation of the :meth:`zcollection.Collection.partitions`
+                method.
             partition_size: The length of each bag partition.
-            npartition: The number of desired bag partitions.
-            selected_variables: A list of variables to retain from the
-                collection. If None, all variables are kept.
+            npartitions: The number of desired bag partitions.
+            selected_variables: A list of variables to retain from the view.
+                If None, all variables are loaded. Useful to load only a
+                subset of the view.
             **kwargs: The keyword arguments to pass to the function.
 
         Returns:
             A bag containing the tuple of the partition scheme and the result
             of the function.
 
         Example:
-            >>> futures = collection.map_overlap(
+            >>> futures = view.map_overlap(
             ...     lambda x: (x["var1"] + x["var2"]).values,
             ...     depth=1)
             >>> for item in futures:
             ...     print(item)
             [1.0, 2.0, 3.0, 4.0]
-            [5.0, 6.0, 7.0, 8.0]
         """
-        if not callable(func):
-            raise TypeError('func must be a callable')
+        if depth < 0:
+            raise ValueError('Depth must be greater than or equal to 0')
 
-        add_partition_info = dask.utils.has_keyword(func, 'partition_info')
+        add_partition_info: bool = dask.utils.has_keyword(
+            func, 'partition_info')
 
         def _wrap(
-            partition: str,
+            arguments: tuple[dataset.Dataset, str],
             func: PartitionCallable,
-            partitions: tuple[str, ...],
-            selected_variables: Sequence[str] | None,
+            datasets_list: tuple[tuple[dataset.Dataset, str]],
             depth: int,
             *args,
             **kwargs,
         ) -> tuple[tuple[tuple[str, int], ...], Any]:
             """Wraps the function to apply on the partition.
 
             Args:
-                partition: The partition to apply the function on.
+                arguments: The partition scheme and the dataset.
                 func: The function to apply.
-                partitions: The partitions to apply the function on.
-                selected_variables: The list of variables to retain from the
-                    partition.
+                datasets: The datasets to apply the function on.
                 depth: The depth of the overlap between the partitions.
                 *args: The positional arguments to pass to the function.
                 **kwargs: The keyword arguments to pass to the function.
 
             Returns:
                 The result of the function.
             """
-            ds, indices = _load_dataset_with_overlap(
-                depth, self.partition_properties.dim, self.fs, self._immutable,
-                partition, partitions, selected_variables)
+            zds: dataset.Dataset
+            indices: slice
+
+            zds, indices = _select_overlap(arguments, datasets_list, depth,
+                                           self.view_ref)
 
             if add_partition_info:
                 kwargs = kwargs.copy()
-                kwargs['partition_info'] = (self.partition_properties.dim,
-                                            indices)
+                kwargs['partition_info'] = (
+                    self.view_ref.partition_properties.dim, indices)
 
             # Finally, apply the function.
-            return (self.partitioning.parse(partition),
-                    func(ds, *args, **kwargs))
+            return (self.view_ref.partitioning.parse(arguments[1]),
+                    func(zds, *args, **kwargs))
 
-        partitions = tuple(self.partitions(filters=filters))
-        bag = dask.bag.core.from_sequence(partitions,
-                                          partition_size=partition_size,
-                                          npartitions=npartition)
-        return bag.map(_wrap, func, partitions, selected_variables, depth,
-                       *args, **kwargs)
+        _assert_have_variables(self.metadata)
 
-    def load(
-        self,
-        *,
-        filters: PartitionFilter = None,
-        indexer: Indexer | None = None,
-        selected_variables: Iterable[str] | None = None,
-    ) -> dataset.Dataset | None:
-        """Load the selected partitions.
+        client: dask.distributed.Client = dask_utils.get_client()
+        datasets_list = tuple(
+            _load_datasets_list(client=client,
+                                base_dir=self.base_dir,
+                                delayed=delayed,
+                                fs=self.fs,
+                                view_ref=self.view_ref,
+                                metadata=self.metadata,
+                                partitions=self.partitions(filters),
+                                selected_variables=selected_variables))
+        bag: dask.bag.core.Bag = dask.bag.core.from_sequence(
+            datasets_list,
+            partition_size=partition_size,
+            npartitions=npartitions)
+        return bag.map(_wrap, func, datasets_list, depth, *args, **kwargs)
 
-        Args:
-            filters: The predicate used to filter the partitions to load.
-                To get more information on the predicate, see the
-                documentation of the :meth:`partitions` method.
-            indexer: The indexer to apply.
-            selected_variables: A list of variables to retain from the
-                collection. If None, all variables are kept.
+    def is_synced(self) -> bool:
+        """Check if the view is synchronized with the underlying collection.
 
         Returns:
-            The dataset containing the selected partitions.
-
-        .. warning::
-
-            If you select variables to load from the collection, do not insert
-            the returned dataset otherwise all skipped variables will be reset
-            with fill values.
-
-        Example:
-            >>> collection = ...
-            >>> collection.load(
-            ...     filters="year == 2019 and month == 3 and day % 2 == 0")
-            >>> collection.load(
-            ...     filters=lambda keys: keys["year"] == 2019 and
-            ...     keys["month"] == 3 and keys["day"] % 2 == 0)
-        """
-        client = dask_utils.get_client()
-        arrays: list[dataset.Dataset]
-        if indexer is None:
-            selected_partitions = tuple(self.partitions(filters=filters))
-            if len(selected_partitions) == 0:
-                return None
-
-            # No indexer, so the dataset is loaded directly for each
-            # selected partition.
-            bag = dask.bag.core.from_sequence(
-                self.partitions(filters=filters),
-                npartitions=dask_utils.dask_workers(client, cores_only=True))
-            arrays = bag.map(storage.open_zarr_group,
-                             fs=self.fs,
-                             selected_variables=selected_variables).compute()
-        else:
-            # Build the indexer arguments.
-            args = tuple(build_indexer_args(self, filters, indexer))
-            if len(args) == 0:
-                return None
-
-            bag = dask.bag.core.from_sequence(
-                args,
-                npartitions=dask_utils.dask_workers(client, cores_only=True))
-
-            # Finally, load the selected partitions and apply the indexer.
-            arrays = list(
-                itertools.chain.from_iterable(
-                    bag.map(
-                        _load_and_apply_indexer,
-                        fs=self.fs,
-                        partition_handler=self.partitioning,
-                        partition_properties=self.partition_properties,
-                        selected_variables=selected_variables,
-                    ).compute()))
-
-        array = arrays.pop(0)
-        if arrays:
-            array = array.concat(arrays, self.partition_properties.dim)
-        if self._immutable:
-            array.merge(
-                storage.open_zarr_group(self._immutable, self.fs,
-                                        selected_variables))
-        array.fill_attrs(ds=self.metadata)
-        return array
-
-    # pylint: disable=method-hidden
-    def update(
-        self,
-        func: UpdateCallable,
-        /,
-        *args,
-        depth: int = 0,
-        filters: PartitionFilter | None = None,
-        partition_size: int | None = None,
-        selected_variables: Iterable[str] | None = None,
-        **kwargs,
-    ) -> None:
-        # pylint: disable=method-hidden
-        """Update the selected partitions.
-
-        Args:
-            func: The function to apply on each partition.
-            *args: The positional arguments to pass to the function.
-            depth: The depth of the overlap between the partitions. Default is
-                0 (no overlap). If depth is greater than 0, the function is
-                applied on the partition and its neighbors selected by the
-                depth. If ``func`` accepts a partition_info as a keyword
-                argument, it will be passed a tuple with the name of the
-                partitioned dimension and the slice allowing getting in the
-                dataset the selected partition.
-            filters: The expression used to filter the partitions to update.
-            partition_size: The number of partitions to update in a single
-                batch. By default, 1 which is the same as to map the function to
-                each partition. Otherwise, the function is called on a batch of
-                partitions.
-            selected_variables: A list of variables to load from the collection.
-                If None, all variables are loaded.
-            **kwargs: The keyword arguments to pass to the function.
-
-        Example:
-            >>> import dask.array
-            >>> import zcollection
-            >>> def ones(ds):
-            ...     return dict(var2=ds.variables["var1"].values * 0 + 1)
-            >>> collection = zcollection.Collection("my_collection", mode="w")
-            >>> collection.update(ones)
+            True if the view is synchronized, False otherwise.
         """
-        if not callable(func):
-            raise TypeError('func must be a callable')
-
-        try:
-            one_partition = next(self.partitions(filters=filters))
-        except StopIteration:
-            return
-        with self.synchronizer:
-            ds = storage.open_zarr_group(one_partition, self.fs,
-                                         selected_variables)
-        func_result = try_infer_callable(func, ds,
-                                         self.partition_properties.dim, *args,
-                                         **kwargs)
-        unknown_variables = set(func_result) - set(
-            self.metadata.variables.keys())
-        if len(unknown_variables):
-            raise ValueError(f'Unknown variables: {unknown_variables}')
-
-        if depth == 0:
-            local_func = _wrap_update_func(func, self.fs, self._immutable,
-                                           selected_variables, *args, **kwargs)
-        else:
-            local_func = _wrap_update_func_with_overlap(
-                depth, self.partition_properties.dim, func, self.fs,
-                self._immutable, selected_variables, *args, **kwargs)
-
-        _LOGGER.info('Updating of the (%s) variable in the collection',
-                     ', '.join(repr(item) for item in func_result))
-        client = dask_utils.get_client()
-
-        batches = dask_utils.split_sequence(
-            tuple(self.partitions(filters=filters, lock=True)), partition_size
-            or dask_utils.dask_workers(client, cores_only=True))
-        storage.execute_transaction(
+        partitions = tuple(self.view_ref.partitions(relative=True))
+        client: dask.distributed.Client = dask_utils.get_client()
+        unsynchronized_partition = storage.execute_transaction(
             client, self.synchronizer,
-            client.map(local_func, tuple(batches), key=func.__name__))
-
-    def _bag_from_partitions(
-        self,
-        filters: PartitionFilter | None = None,
-        **kwargs,
-    ) -> dask.bag.core.Bag:
-        """Return a dask bag from the partitions.
-
-        Args:
-            filters: The predicate used to filter the partitions to load.
-            kwargs: The keyword arguments to pass to the method
-                :meth:`partitions`.
-
-        Returns:
-            The dask bag.
-        """
-        partitions = [*self.partitions(filters=filters, **kwargs)]
-        return dask.bag.core.from_sequence(seq=partitions,
-                                           npartitions=len(partitions))
-
-    def drop_variable(
-        self,
-        variable: str,
-    ) -> None:
-        """Delete the variable from the collection.
-
-        Args:
-            variable: The variable to delete.
-
-        Raises:
-            ValueError: If the variable doesn't exist in the collection or is
-                used by the partitioning.
-
-        Example:
-            >>> import zcollection
-            >>> collection = zcollection.open_collection(
-            ...     "my_collection", mode="w")
-            >>> collection.drop_variable("my_variable")
-        """
-        _LOGGER.info('Dropping of the %r variable in the collection', variable)
-        if variable in self.partitioning.variables:
-            raise ValueError(
-                f'The variable {variable!r} is part of the partitioning.')
-        if variable not in self.metadata.variables:
-            raise ValueError(
-                f'The variable {variable!r} does not exist in the collection.')
-        if self._immutable:
-            ds = storage.open_zarr_group(self._immutable, self.fs)
-            if variable in ds.variables:
-                raise ValueError(
-                    f'The variable {variable!r} is part of the immutable '
-                    'dataset.')
-        client = dask_utils.get_client()
-        bag = self._bag_from_partitions(lock=True)
-        awaitables = dask.distributed.futures_of(
-            bag.map(storage.del_zarr_array, variable, self.fs).persist())
-        storage.execute_transaction(client, self.synchronizer, awaitables)
-        del self.metadata.variables[variable]
-        self._write_config()
-
-    def add_variable(
-        self,
-        variable: meta.Variable | dataset.Variable,
-    ) -> None:
-        """Add a variable to the collection.
-
-        Args:
-            variable: The variable to add.
-
-        Raises:
-            ValueError: if the variable is already part of the collection, it
-                doesn't use the partitioning dimension or use a dimension that
-                is not part of the dataset.
-
-        Example:
-            >>> import zcollection
-            >>> collection = zcollection.open_collection(
-            ...     "my_collection", mode="w")
-            >>> new_variable = meta.Variable(
-            ...     name="my_variable",
-            ...     dtype=numpy.dtype("int16"),
-            ...     dimensions=("num_lines", "num_pixels"),
-            ...     fill_value=32267,
-            ...     attrs=(dataset.Attribute(name="my_attr", value=0), ),
-            ... )
-            >>> collection.add_variable(new_variable)
-        """
-        variable = dataset.get_variable_metadata(variable)
-        _LOGGER.info('Adding of the %r variable in the collection',
-                     variable.name)
-        if self.partition_properties.dim not in variable.dimensions:
-            raise ValueError(
-                'The new variable must use the partitioning axis.')
-        self.metadata.add_variable(variable)
-        self._write_config()
-
-        client = dask_utils.get_client()
-
-        template = self.metadata.search_same_dimensions_as(variable)
-        chunks = {dim.name: dim.value for dim in self.metadata.chunks}
-        try:
-            bag = self._bag_from_partitions(lock=True)
-            futures = dask.distributed.futures_of(
-                bag.map(storage.add_zarr_array, variable, template.name,
-                        self.fs, chunks).persist())
-            storage.execute_transaction(client, self.synchronizer, futures)
-        except Exception:
-            self.drop_variable(variable.name)
-            raise
-
-    def iterate_on_records(
-        self,
-        *,
-        relative: bool = False,
-    ) -> Iterator[tuple[str, zarr.Group]]:
-        """Iterate over the partitions and the zarr groups.
-
-        Args:
-            relative: If True, the paths are relative to the base directory.
-
-        Returns
-            The iterator over the partitions and the zarr groups.
-        """
-        yield from (
-            (
-                self._relative_path(item) if relative else item,
-                zarr.open_consolidated(
-                    self.fs.get_mapper(item),  # type: ignore
-                    mode='r',
-                )) for item in self.partitions())
-
-    def variables(
-        self,
-        selected_variables: Iterable[str] | None = None
-    ) -> tuple[dataset.Variable, ...]:
-        """Return the variables of the collection.
-
-        Args:
-            selected_variables: The variables to return. If None, all the
-                variables are returned.
+            client.map(_sync,
+                       partitions,
+                       base_dir=self.base_dir,
+                       fs=self.fs,
+                       view_ref=self.view_ref,
+                       metadata=self.metadata,
+                       dry_run=True))
+        return len(
+            tuple(
+                filter(lambda item: item is not None,
+                       unsynchronized_partition))) == 0
+
+    def sync(
+        self,
+        filters: collection.PartitionFilter = None
+    ) -> collection.abc.PartitionFilterCallback:
+        """Synchronize the view with the underlying collection.
+
+        This method is useful to update the view after a change in the
+        underlying collection.
+
+        Args:
+            filters: The predicate used to select the partitions to
+                synchronize. To get more information on the predicate, see the
+                documentation of the :meth:`zcollection.Collection.partitions`
+                method.
+                If None, the view is synchronized with all the partitions
+                already present in the view. If you want to extend the view
+                with new partitions, use must provide a predicate that
+                selects the new partitions.
+                Existing partitions are not removed, even if they are not
+                selected by the predicate.
 
         Returns:
-            The variables of the collection.
-        """
-        return variables(self.metadata, selected_variables)
+            A function that can be used as a predicate to get the partitions
+            that have been synchronized using the :meth:`View.partitions`
+            method.
+        """
+        _LOGGER.info('Synchronizing view %s', self)
+
+        if filters is not None:
+            self.filters = filters
+            self._write_config()
+            self._init_partitions(filters)
 
-    def copy(
-        self,
-        target: str,
-        *,
-        filters: PartitionFilter | None = None,
-        filesystem: fsspec.AbstractFileSystem | None = None,
-        mode: str = 'w',
-        npartitions: int | None = None,
-        synchronizer: sync.Sync | None = None,
-    ) -> Collection:
-        """Copy the collection to a new location.
+        partitions = tuple(self.view_ref.partitions(relative=True))
+        _LOGGER.info('%d partitions to synchronize', len(partitions))
 
-        Args:
-            target: The target location.
-            filters: The predicate used to filter the partitions to copy.
-            filesystem: The file system to use. If None, the file system of the
-                collection is used.
-            mode: The mode used to open the collection copied. Default is 'w'.
-            npartitions: The number of partitions top copy in parallel. Default
-                is number of cores.
-            synchronizer: The synchronizer used to synchronize the collection
-                copied. Default is None.
-
-        Returns:
-            The new collection.
-
-        Example:
-            >>> import zcollection
-            >>> collection = zcollection.open_collection(
-            ...     "my_collection", mode="r")
-            >>> collection.copy(target="my_new_collection")
-        """
-        _LOGGER.info('Copying of the collection to %r', target)
-        if filesystem is None:
-            filesystem = fs_utils.get_fs(target)
-        client = dask_utils.get_client()
-        npartitions = npartitions or dask_utils.dask_workers(client,
-                                                             cores_only=True)
-
-        # Sequence of (source, target) to copy split in npartitions
-        args = tuple(
-            dask_utils.split_sequence(
-                [(item,
-                  fs_utils.join_path(
-                      target,
-                      os.path.relpath(item, self.partition_properties.dir)))
-                 for item in self.partitions(filters=filters)], npartitions))
-        # Copy the selected partitions
-        partial = functools.partial(fs_utils.copy_tree,
-                                    fs_source=self.fs,
-                                    fs_target=filesystem)
-
-        def worker_task(args: Sequence[tuple[str, str]]) -> None:
-            """Function call on each worker to copy the partitions."""
-            tuple(map(lambda arg: partial(*arg), args))
-
-        client.gather(client.map(worker_task, args))
-        # Then the remaining files in the root directory (config, metadata,
-        # etc.)
-        fs_utils.copy_files([
-            item['name']
-            for item in self.fs.listdir(self.partition_properties.dir,
-                                        detail=True) if item['type'] == 'file'
-        ], target, self.fs, filesystem)
-        return Collection.from_config(target,
-                                      mode=mode,
-                                      filesystem=filesystem,
-                                      synchronizer=synchronizer)
+        client: dask.distributed.Client = dask_utils.get_client()
+        synchronized_partition: list[str | None] = storage.execute_transaction(
+            client, self.synchronizer,
+            client.map(_sync,
+                       partitions,
+                       base_dir=self.base_dir,
+                       fs=self.fs,
+                       view_ref=self.view_ref,
+                       metadata=self.metadata))
+
+        partition_ids = tuple(
+            dict(self.view_ref.partitioning.parse(
+                item))  # type: ignore[arg-type] # item is filtered
+            for item in filter(lambda item: item is not None,
+                               synchronized_partition))
+        return lambda item: item in partition_ids
```

### Comparing `zcollection-2023.3.2/zcollection/collection/callable_objects.py` & `zcollection-2023.5.0/zcollection/collection/callable_objects.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (c) 2023 CNES
+#
+# All rights reserved. Use of this source code is governed by a
+# BSD-style license that can be found in the LICENSE file.
 """
 Callable objects.
 =================
 """
 from __future__ import annotations
 
 from typing import Any, Callable, Protocol, Sequence
@@ -26,47 +30,29 @@
     def __name__(self) -> str:
         """Name of the callable."""
         # pylint: disable=unnecessary-ellipsis
         # Make checker happy.
         ...
         # pylint: enable=unnecessary-ellipsis
 
-    def __call__(self, ds: dataset.Dataset, *args, **kwargs) -> Any:
+    def __call__(self, zds: dataset.Dataset, *args, **kwargs) -> Any:
         """Call the partition function.
 
         Args:
-            ds: Dataset to partition.
+            zds: Dataset to partition.
             *args: Positional arguments.
             **kwargs: Keyword arguments.
 
         Returns:
             Result of the partition function.
         """
 
 
-class MapCallable(Protocol):
-    """Protocol for map callables.
-
-    A callable map is a function that accepts a data set, a list of
-    arguments, a dictionary of keyword arguments and returns a result.
-    """
-
-    def __call__(self, ds: dataset.Dataset, *args, **kwargs) -> Any:
-        """Call the map function.
-
-        Args:
-            ds: Dataset to map.
-            *args: Positional arguments.
-            **kwargs: Keyword arguments.
-
-        Returns:
-            Result of the map function.
-        """
-
-    #: pylint: enable=too-few-public-methods
+#: Alias for :class:`PartitionCallable`.
+MapCallable = PartitionCallable
 
 
 class UpdateCallable(Protocol):
     """Protocol for update callables.
 
     A callable update is a function that accepts a data set and returns
     a dictionary of arrays to update.
@@ -76,20 +62,20 @@
     def __name__(self) -> str:
         """Name of the callable."""
         # pylint: disable=unnecessary-ellipsis
         # Make checker happy.
         ...
         # pylint: enable=unnecessary-ellipsis
 
-    def __call__(self, ds: dataset.Dataset, *args,
+    def __call__(self, zds: dataset.Dataset, *args,
                  **kwargs) -> dict[str, ArrayLike]:
         """Call the update function.
 
         Args:
-            ds: Dataset to update.
+            zds: Dataset to update.
             *args: Positional arguments.
             **kwargs: Keyword arguments.
 
         Returns:
             Dictionary of arrays to update.
         """
         # pylint: disable=unnecessary-ellipsis
```

### Comparing `zcollection-2023.3.2/zcollection/collection/detail.py` & `zcollection-2023.5.0/zcollection/collection/detail.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+# Copyright (c) 2023 CNES
+#
+# All rights reserved. Use of this source code is governed by a
+# BSD-style license that can be found in the LICENSE file.
 """
 Implementation details.
 =======================
 """
 from __future__ import annotations
 
-from typing import Any, Callable, Iterable, Sequence
+from typing import Any, Callable, Dict, Iterable, Sequence, Tuple
 import dataclasses
 import sys
 import time
 import traceback
+import types
 
 import dask.utils
 import fsspec
 import zarr.storage
 
 from .. import dataset, merging, partitioning, sync
 from ..fs_utils import join_path
 from ..storage import open_zarr_group, update_zarr_array, write_zarr_group
+from ..type_hints import ArrayLike
 from .callable_objects import UpdateCallable, WrappedPartitionCallable
 
+#: Partition's type.
+PartitionSlice = Tuple[Tuple[str, ...], Dict[str, slice]]
+
 
 @dataclasses.dataclass(frozen=True)
 class PartitioningProperties:
     """Properties of a partition."""
     #: The base directory of the partition.
     dir: str
     #: The name of the partitioning dimension.
@@ -37,120 +46,152 @@
     Args:
         dim: Dimension to select
         indices: Dimension indices to select
 
     Returns:
         The slices
     """
-    slices = [slice(None)] * len(variable.dimensions)
+    slices: list[slice] = [slice(None)] * len(variable.dimensions)
     slices[variable.dimensions.index(dim)] = indices
     return tuple(slices)
 
 
-def try_infer_callable(
+def _try_infer_callable(
     func: Callable,
-    ds: dataset.Dataset,
+    zds: dataset.Dataset,
     dim: str,
     *args,
     **kwargs,
 ) -> Any:
     """Try to call a function with the given arguments.
 
     Args:
         func: Function to call.
-        ds: Dataset to pass to the function.
+        zds: Dataset to pass to the function.
         dim: Name of the partitioning dimension.
         *args: Positional arguments to pass to the function.
         **kwargs: Keyword arguments to pass to the function.
 
     Returns:
         The result of the function.
     """
-    partition_info = dim, slice(0, ds.dimensions[dim])
+    partition_info: tuple[str, slice]
+    partition_info = dim, slice(0, zds.dimensions[dim])
     try:
         if dask.utils.has_keyword(func, 'partition_info'):
-            return func(ds, *args, partition_info=partition_info, **kwargs)
-        return func(ds, *args, **kwargs)
+            return func(zds, *args, partition_info=partition_info, **kwargs)
+        return func(zds, *args, **kwargs)
     except Exception as exc:
+        exc_type: type[BaseException] | None
+        exc_traceback: types.TracebackType | None
+        exc_value: BaseException | None
         exc_type, exc_value, exc_traceback = sys.exc_info()
-        execution_tb = ''.join(traceback.format_tb(exc_traceback))
+        execution_tb: str = ''.join(traceback.format_tb(exc_traceback))
         raise RuntimeError(
             f'An error occurred while applying the function {func} with '
             f'the arguments {args} and {kwargs} to the partition. The '
             f'error is: {exc_type!r}: {exc_value}. The traceback '
             f'is: {execution_tb}') from exc
 
 
-def update_with_overlap(func: UpdateCallable, ds: dataset.Dataset,
-                        indices: slice, dim: str,
-                        fs: fsspec.AbstractFileSystem, path: str, *args,
-                        **kwargs) -> None:
+def _update_with_overlap(
+    *args,
+    func: UpdateCallable,
+    zds: dataset.Dataset,
+    indices: slice,
+    dim: str,
+    fs: fsspec.AbstractFileSystem,
+    path: str,
+    trim: bool,
+    **kwargs,
+) -> None:
     """Update a partition with overlap.
 
     Args:
         func: Function to apply to update each partition.
-        ds: Dataset to update.
+        zds: Dataset to update.
         indices: Indices of the partition to update.
         dim: Name of the partitioning dimension.
         fs: File system on which the Zarr dataset is stored.
         path: Path to the Zarr group.
+        trim: Whether to trim the overlap.
         *args: Positional arguments to pass to the function.
         **kwargs: Keyword arguments to pass to the function.
 
     Returns:
         The updated variables.
     """
-    dictionary = (func(ds, *args, partition_info=(dim, indices), **kwargs)
-                  if dask.utils.has_keyword(func, 'partition_info') else func(
-                      ds, *args, **kwargs))
-
-    for varname, array in dictionary.items():
-        slices = _get_slices(ds[varname], dim, indices)
-        update_zarr_array(
-            dirname=join_path(path, varname),
-            array=array[slices],  # type: ignore[index]
-            fs=fs,
-        )
+    dictionary: dict[str, ArrayLike] = (func(
+        zds, *args, partition_info=(dim, indices), **
+        kwargs) if dask.utils.has_keyword(func, 'partition_info') else func(
+            zds, *args, **kwargs))
+
+    if trim:
+        for varname, array in dictionary.items():
+            slices: tuple[slice, ...] = _get_slices(zds[varname], dim, indices)
+            update_zarr_array(
+                dirname=join_path(path, varname),
+                array=array[slices],  # type: ignore[index]
+                fs=fs,
+            )
+    else:
+        tuple(
+            map(
+                lambda items: update_zarr_array(
+                    dirname=join_path(path, items[0]),
+                    array=items[1],
+                    fs=fs,
+                ), dictionary.items()))
 
 
 def _load_dataset(
+    delayed: bool,
     fs: fsspec.AbstractFileSystem,
     immutable: str | None,
     partition: str,
     selected_variables: Iterable[str] | None,
-):
+) -> dataset.Dataset:
     """Load a dataset from a partition.
 
     Args:
+        delayed: Whether to load the dataset lazily.
         fs: File system on which the Zarr dataset is stored.
         immutable: Name of the immutable directory.
         partition: Name of the partition.
         selected_variables: Name of the variables to load from the dataset.
 
     Returns:
         The loaded dataset.
     """
-    ds = open_zarr_group(partition, fs, selected_variables)
+    zds: dataset.Dataset = open_zarr_group(
+        partition, fs, delayed=delayed, selected_variables=selected_variables)
     if immutable:
-        ds.merge(open_zarr_group(immutable, fs, selected_variables))
-    return ds
+        zds.merge(
+            open_zarr_group(immutable,
+                            fs,
+                            delayed=delayed,
+                            selected_variables=selected_variables))
+    return zds
 
 
 def _load_dataset_with_overlap(
+    *,
+    delayed: bool,
     depth: int,
     dim: str,
     fs: fsspec.AbstractFileSystem,
     immutable: str | None,
     partition: str,
     partitions: Sequence[str],
     selected_variables: Iterable[str] | None,
 ) -> tuple[dataset.Dataset, slice]:
     """Load a dataset from a partition with overlap.
 
     Args:
+        delayed: Whether to load the dataset lazily.
         depth: Depth of the overlap.
         dim: Name of the partitioning dimension.
         fs: File system on which the Zarr dataset is stored.
         immutable: Name of the immutable directory.
         partition: Name of the partition.
         partitions: List of all partitions.
         selected_variables: Name of the variables to load from the dataset.
@@ -163,127 +204,167 @@
     def calculate_slice(
         groups: list[dataset.Dataset],
         selected_partitions: list[str],
     ) -> slice:
         """Compute the slice of the selected dataset (without overlap)."""
         start = 0
         indices = slice(0, 0, None)
-        for ix, ds in enumerate(groups):
-            size = ds.dimensions[dim]
+        for idx, zds in enumerate(groups):
+            size: int = zds.dimensions[dim]
             indices = slice(start, start + size, None)
-            if partition == selected_partitions[ix]:
+            if partition == selected_partitions[idx]:
                 break
             start += size
         return indices
 
-    where = partitions.index(partition)
+    where: int = partitions.index(partition)
 
     # Search for the overlapping partitions
-    selected_partitions = [
+    selected_partitions: list[str] = [
         partitions[ix] for ix in range(where - depth, where + depth + 1)
         if 0 <= ix < len(partitions)
     ]
 
     # Load the datasets for each selected partition.
-    groups = [
-        open_zarr_group(partition, fs, selected_variables)
+    groups: list[dataset.Dataset] = [
+        open_zarr_group(partition,
+                        fs,
+                        delayed=delayed,
+                        selected_variables=selected_variables)
         for partition in selected_partitions
     ]
 
     # Compute the slice of the given partition.
-    indices = calculate_slice(groups, selected_partitions)
+    indices: slice = calculate_slice(groups, selected_partitions)
 
     # Build the dataset for the selected partitions.
-    ds = groups.pop(0)
+    zds: dataset.Dataset = groups.pop(0)
     if groups:
-        ds = ds.concat(groups, dim)
+        zds = zds.concat(groups, dim)
 
     if immutable:
-        ds.merge(open_zarr_group(partition, fs, selected_variables))
-    return ds, indices
+        zds.merge(
+            open_zarr_group(partition,
+                            fs,
+                            delayed=delayed,
+                            selected_variables=selected_variables))
+    return zds, indices
 
 
 def _wrap_update_func(
+    *args,
+    delayed: bool,
     func: UpdateCallable,
     fs: fsspec.AbstractFileSystem,
     immutable: str | None,
     selected_variables: Iterable[str] | None,
-    *args,
     **kwargs,
 ) -> WrappedPartitionCallable:
     """Wrap an update function taking a partition's dataset as input and
     returning variable's values as a numpy array.
 
     Args:
+        delayed: Whether to load the dataset lazily.
         func: Function to apply to update each partition.
         fs: File system on which the Zarr dataset is stored.
         immutable: Name of the immutable directory.
         selected_variables: Name of the variables to load from the dataset.
             If None, all variables are loaded.
+        trim: Whether to trim the overlap.
         *args: Positional arguments to pass to the function.
         **kwargs: Keyword arguments to pass to the function.
 
     Returns:
         The wrapped function that takes a set of dataset partitions and the
         variable name as input and returns the variable's values as a numpy
         array.
     """
 
     def wrap_function(partitions: Iterable[str]) -> None:
         # Applying function for each partition's data
         for partition in partitions:
-            ds = _load_dataset(fs, immutable, partition, selected_variables)
-            dictionary = func(ds, *args, **kwargs)
+            zds: dataset.Dataset = _load_dataset(delayed, fs, immutable,
+                                                 partition, selected_variables)
+            dictionary: dict[str, ArrayLike] = func(zds, *args, **kwargs)
             tuple(
                 update_zarr_array(  # type: ignore[func-returns-value]
                     dirname=join_path(partition, varname),
                     array=array,
                     fs=fs,
                 ) for varname, array in dictionary.items())
 
     return wrap_function
 
 
 def _wrap_update_func_with_overlap(
+    *args,
+    delayed: bool,
     depth: int,
     dim: str,
     func: UpdateCallable,
     fs: fsspec.AbstractFileSystem,
     immutable: str | None,
+    selected_partitions: Sequence[str],
     selected_variables: Iterable[str] | None,
-    *args,
+    trim: bool,
     **kwargs,
 ) -> WrappedPartitionCallable:
     """Wrap an update function taking a partition's dataset as input and
     returning variable's values as a numpy array.
 
     Args:
+        delayed: Whether to load the dataset lazily.
+        depth: Depth of the overlap.
+        dim: Name of the partitioning dimension.
         func: Function to apply to update each partition.
         fs: File system on which the Zarr dataset is stored.
+        immutable: Name of the immutable directory.
+        selected_partitions: List of all partitions selected for the update.
         selected_variables: Name of the variables to load from the dataset.
             If None, all variables are loaded.
+        trim: Whether to trim the overlap.
         *args: Positional arguments to pass to the function.
         **kwargs: Keyword arguments to pass to the function.
 
     Returns:
         The wrapped function that takes a set of dataset partitions and the
         variable name as input and returns the variable's values as a numpy
         array.
     """
     if depth < 0:
         raise ValueError('Depth must be non-negative.')
 
     def wrap_function(partitions: Sequence[str]) -> None:
         # Applying function for each partition's data
         for partition in partitions:
-            ds, indices = _load_dataset_with_overlap(depth, dim, fs, immutable,
-                                                     partition, partitions,
-                                                     selected_variables)
-            update_with_overlap(func, ds, indices, dim, fs, partition, *args,
-                                **kwargs)
+
+            # pylint: disable=duplicate-code
+            # False positive with the method Collection.map_overlap
+            zds: dataset.Dataset
+            indices: slice
+            zds, indices = _load_dataset_with_overlap(
+                delayed=delayed,
+                depth=depth,
+                dim=dim,
+                fs=fs,
+                immutable=immutable,
+                partition=partition,
+                partitions=selected_partitions,
+                selected_variables=selected_variables)
+            # pylint: enable=duplicate-code
+
+            _update_with_overlap(*args,
+                                 func=func,
+                                 zds=zds,
+                                 indices=indices,
+                                 dim=dim,
+                                 fs=fs,
+                                 path=partition,
+                                 trim=trim,
+                                 **kwargs)
 
     return wrap_function
 
 
 def _rm(fs: fsspec.AbstractFileSystem, dirname: str) -> None:
     """Remove a directory and its content.
 
@@ -301,60 +382,71 @@
         except OSError:
             fs.invalidate_cache(dirname)
         time.sleep(1)
         tries += 1
 
 
 def _insert(
-    args: tuple[tuple[str, ...], dict[str, slice]],
+    *,
+    args: PartitionSlice,
     axis: str,
-    ds: dataset.Dataset,
+    zds: dataset.Dataset,
     fs: fsspec.AbstractFileSystem,
     merge_callable: merging.MergeCallable | None,
     partitioning_properties: PartitioningProperties,
 ) -> None:
     """Insert or update a partition in the collection.
 
     Args:
         args: Tuple containing the partition's name and its slice.
         axis: The axis to merge on.
-        ds: The dataset to process.
+        zds: The dataset to process.
         fs: The file system that the partition is stored on.
         merge_callable: The merge callable.
         partitioning_properties: The partitioning properties.
     """
+    partition: tuple[str, ...]
+    indexer: dict[str, slice]
+
     partition, indexer = args
-    dirname = join_path(*((partitioning_properties.dir, ) + partition))
+    dirname: str = join_path(*((partitioning_properties.dir, ) + partition))
 
     # If the consolidated zarr metadata does not exist, we consider the
     # partition as empty.
     if fs.exists(join_path(dirname, '.zmetadata')):
         # The current partition already exists, so we need to merge
         # the dataset.
-        merging.perform(ds.isel(indexer), dirname, axis, fs,
-                        partitioning_properties.dim, merge_callable)
+        merging.perform(zds.isel(indexer),
+                        dirname,
+                        axis,
+                        fs,
+                        partitioning_properties.dim,
+                        delayed=zds.delayed,
+                        merge_callable=merge_callable)
         return
 
     # The current partition does not exist, so we need to create
     # it and insert the dataset.
     try:
         zarr.storage.init_group(store=fs.get_mapper(dirname))
 
         # The synchronization is done by the caller.
-        write_zarr_group(ds.isel(indexer), dirname, fs, sync.NoSync())
+        write_zarr_group(zds.isel(indexer), dirname, fs, sync.NoSync())
     except:  # noqa: E722
         # If the construction of the new dataset fails, the created
         # partition is deleted, to guarantee the integrity of the
         # collection.
         _rm(fs, dirname)
         raise
 
 
 def _load_and_apply_indexer(
     args: tuple[tuple[tuple[str, int], ...], list[slice]],
+    *,
+    delayed: bool,
     fs: fsspec.AbstractFileSystem,
     partition_handler: partitioning.Partitioning,
     partition_properties: PartitioningProperties,
     selected_variables: Iterable[str] | None,
 ) -> list[dataset.Dataset]:
     """Load a partition and apply its indexer.
 
@@ -364,12 +456,18 @@
         partition_handler: The partitioning handler.
         partition_properties: The partitioning properties.
         selected_variable: The selected variables to load.
 
     Returns:
         The list of loaded datasets.
     """
+    items: list[slice]
+    partition_scheme: tuple[tuple[str, int], ...]
+
     partition_scheme, items = args
-    partition = join_path(partition_properties.dir,
-                          partition_handler.join(partition_scheme, fs.sep))
-    ds = open_zarr_group(partition, fs, selected_variables)
-    return [ds.isel({partition_properties.dim: indexer}) for indexer in items]
+    partition: str = join_path(
+        partition_properties.dir,
+        partition_handler.join(partition_scheme, fs.sep))
+    zds: dataset.Dataset = open_zarr_group(
+        partition, fs, delayed=delayed, selected_variables=selected_variables)
+    return list(
+        zds.isel({partition_properties.dim: indexer}) for indexer in items)
```

### Comparing `zcollection-2023.3.2/zcollection/collection/tests/test_collection.py` & `zcollection-2023.5.0/zcollection/collection/tests/test_collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,31 +37,31 @@
     END_DATE,
     FILE_SYSTEM_DATASET,
     START_DATE,
     create_test_collection,
     create_test_dataset,
     create_test_dataset_with_fillvalue,
 )
+from ...tests.fixture import dask_arrays, numpy_arrays
 from ...tests.fs import local_fs, s3, s3_base, s3_fs
 
 # pylint: disable=unused-import
 
 
-@pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('fs', ['local_fs', 's3_fs'])
 def test_collection_creation(
-    dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
     request,
-):
+) -> None:
     """Test the creation of a collection."""
-    tested_fs = request.getfixturevalue(arg)
-    ds = next(create_test_dataset())
+    tested_fs = request.getfixturevalue(fs)
+    zds = next(create_test_dataset(False))
     zcollection = collection.Collection(
         axis='time',
-        ds=ds.metadata(),
+        ds=zds.metadata(),
         partition_handler=partitioning.Date(('time', ), 'D'),
         partition_base_dir=str(tested_fs.collection),
         filesystem=tested_fs.fs)
     assert isinstance(str(zcollection), str)
     assert zcollection.immutable is False
 
     serialized = collection.Collection.from_config(str(tested_fs.collection),
@@ -72,211 +72,261 @@
     assert serialized.partitioning.get_config(
     ) == zcollection.partitioning.get_config()
 
     with pytest.raises(ValueError):
         collection.Collection.from_config(str(tested_fs.collection.parent))
 
     with pytest.raises(ValueError):
-        collection.Collection('time_tai', ds.metadata(),
+        collection.Collection('time_tai', zds.metadata(),
                               partitioning.Date(('time', ), 'D'),
                               str(tested_fs.collection))
 
     with pytest.raises(ValueError):
-        collection.Collection('time', ds.metadata(),
+        collection.Collection('time', zds.metadata(),
                               partitioning.Date(('time_tai', ), 'D'),
                               str(tested_fs.collection))
 
     with pytest.raises(ValueError):
-        collection.Collection(axis='time',
-                              ds=ds.metadata(),
-                              mode='X',
-                              partition_handler=partitioning.Date(('time', ),
-                                                                  'D'),
-                              partition_base_dir=str(tested_fs.collection),
-                              filesystem=tested_fs.fs)
+        collection.Collection(
+            axis='time',
+            ds=zds.metadata(),
+            mode='X',  # type: ignore[arg-type]
+            partition_handler=partitioning.Date(('time', ), 'D'),
+            partition_base_dir=str(tested_fs.collection),
+            filesystem=tested_fs.fs)
 
 
 # pylint: disable=too-many-statements
-@pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('fs', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_insert(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    arrays_type,
+    fs,
     request,
     tmpdir,
-):
+) -> None:
     """Test the insertion of a dataset."""
-    tested_fs = request.getfixturevalue(arg)
-    datasets = list(create_test_dataset())
-    ds = datasets[0]
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
+    datasets = list(create_test_dataset(delayed=False))
     zcollection = collection.Collection('time',
-                                        ds.metadata(),
+                                        datasets[0].metadata(),
                                         partitioning.Date(('time', ), 'D'),
                                         str(tested_fs.collection),
                                         filesystem=tested_fs.fs,
                                         synchronizer=sync.ProcessSync(
                                             str(tmpdir / 'lock.lck')))
 
     indices = numpy.arange(0, len(datasets))
     numpy.random.shuffle(indices)
-    for ix in indices:
-        zcollection.insert(datasets[ix],
+    for idx in indices:
+        zcollection.insert(datasets[idx],
                            merge_callable=merging.merge_time_series)
 
-    data = zcollection.load()
+    data = zcollection.load(delayed=delayed)
     assert data is not None
     values = data.variables['time'].values
     assert numpy.all(values == numpy.arange(START_DATE, END_DATE, DELTA))
 
     # Adding same datasets once more (should not change anything)
-    for ix in indices[:5]:
-        zcollection.insert(datasets[ix])
+    for idx in indices[:5]:
+        zcollection.insert(datasets[idx])
 
     assert list(zcollection.partitions()) == sorted(
         list(zcollection.partitions()))
 
-    data = zcollection.load()
+    data = zcollection.load(delayed=delayed)
     assert data is not None
     values = data.variables['time'].values
     assert numpy.all(values == numpy.arange(START_DATE, END_DATE, DELTA))
 
     values = data.variables['var1'].values
     numpy.all(values == numpy.vstack((numpy.arange(values.shape[0]), ) *
                                      values.shape[1]).T)
 
     values = data.variables['var2'].values
     numpy.all(values == numpy.vstack((numpy.arange(values.shape[0]), ) *
                                      values.shape[1]).T)
 
-    data = zcollection.load(filters='year == 2020')
+    data = zcollection.load(delayed=delayed, filters='year == 2020')
     assert data is None
 
-    data = zcollection.load(filters='year == 2000')
+    data = zcollection.load(delayed=delayed, filters='year == 2000')
     assert data is not None
     assert data.variables['time'].shape[0] == 61
 
-    data = zcollection.load(filters='year == 2000 and month == 4')
+    data = zcollection.load(delayed=delayed,
+                            filters='year == 2000 and month == 4')
     assert data is not None
     dates = data.variables['time'].values
     assert numpy.all(
         dates.astype('datetime64[M]') == numpy.datetime64('2000-04-01'))
 
     data = zcollection.load(
-        filters='year == 2000 and month == 4 and day == 15')
+        delayed=delayed, filters='year == 2000 and month == 4 and day == 15')
     assert data is not None
     dates = data.variables['time'].values
     assert numpy.all(
         dates.astype('datetime64[D]') == numpy.datetime64('2000-04-15'))
 
     data = zcollection.load(
+        delayed=delayed,
         filters='year == 2000 and month == 4 and day in range(5, 25)')
     assert data is not None
-    data = zcollection.load(filters=lambda keys: datetime.date(
-        2000, 4, 5) <= datetime.date(keys['year'], keys['month'], keys['day'])
-                            <= datetime.date(2000, 4, 24))
+    data = zcollection.load(delayed=delayed,
+                            filters=lambda keys: datetime.date(2000, 4, 5) <=
+                            datetime.date(keys['year'], keys['month'], keys[
+                                'day']) <= datetime.date(2000, 4, 24))
     assert data is not None
     dates = data.variables['time'].values.astype('datetime64[D]')
     assert dates.min() == numpy.datetime64('2000-04-06')
     assert dates.max() == numpy.datetime64('2000-04-24')
 
     for path, item in zcollection.iterate_on_records(relative=True):
         assert isinstance(path, str)
         assert isinstance(item, zarr.Group)
 
     zcollection = convenience.open_collection(str(tested_fs.collection),
                                               mode='r',
                                               filesystem=tested_fs.fs)
-    ds = zcollection.load(selected_variables=['var1'])
-    assert ds is not None
-    assert 'var1' in ds.variables
-    assert 'var2' not in ds.variables
-
-    ds = zcollection.load(selected_variables=[])
-    assert ds is not None
-    assert len(ds.variables) == 0
-
-    ds = zcollection.load(selected_variables=['varX'])
-    assert ds is not None
-    assert len(ds.variables) == 0
+    zds = zcollection.load(delayed=delayed, selected_variables=['var1'])
+    assert zds is not None
+    assert 'var1' in zds.variables
+    assert 'var2' not in zds.variables
+
+    zds = zcollection.load(delayed=delayed, selected_variables=[])
+    assert zds is not None
+    assert len(zds.variables) == 0
+
+    zds = zcollection.load(delayed=delayed, selected_variables=['varX'])
+    assert zds is not None
+    assert len(zds.variables) == 0
 
     # pylint: enable=too-many-statements
 
 
-@pytest.mark.parametrize('arg,create_test_data', FILE_SYSTEM_DATASET)
+@pytest.mark.parametrize('fs,create_test_data', FILE_SYSTEM_DATASET)
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_update(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
+    arrays_type,
     create_test_data,
     request,
-):
+) -> None:
     """Test the update of a dataset."""
-    tested_fs = request.getfixturevalue(arg)
-    ds = next(create_test_data())
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
+    zds = next(create_test_data(delayed=delayed))
     zcollection = collection.Collection('time',
-                                        ds.metadata(),
+                                        zds.metadata(),
                                         partitioning.Date(('time', ), 'D'),
                                         str(tested_fs.collection),
                                         filesystem=tested_fs.fs)
-    zcollection.insert(ds)
+    zcollection.insert(zds)
 
-    def update(ds: dataset.Dataset, shift: int = 3):
+    def update(zds: dataset.Dataset, shift: int = 3):
         """Update function used for this test."""
-        return dict(var2=ds.variables['var1'].values * -1 + shift)
+        return {'var2': zds.variables['var1'].values * -1 + shift}
 
-    zcollection.update(update)  # type: ignore
+    zcollection.update(update, delayed=delayed)  # type: ignore
 
     data = zcollection.load()
     assert data is not None
     assert numpy.allclose(data.variables['var2'].values,
                           data.variables['var1'].values * -1 + 3,
                           rtol=0)
 
-    zcollection.update(update, depth=1, shift=5)  # type: ignore
+    zcollection.update(
+        update,  # type: ignore
+        delayed=delayed,
+        depth=1,
+        shift=5)
 
-    data = zcollection.load()
+    data = zcollection.load(delayed=delayed)
     assert data is not None
     assert numpy.allclose(data.variables['var2'].values,
                           data.variables['var1'].values * -1 + 5,
                           rtol=0)
 
-    def update_with_info(ds: dataset.Dataset, partition_info=None, shift=3):
+    # Test case if the selected variables does not contains the variable
+    # to update.
+    zcollection.update(
+        update,  # type: ignore
+        delayed=delayed,
+        selected_variables=['var1'],
+        depth=1,
+        shift=5)
+
+    data = zcollection.load(delayed=delayed)
+    assert data is not None
+    assert numpy.allclose(data.variables['var2'].values,
+                          data.variables['var1'].values * -1 + 5,
+                          rtol=0)
+
+    def update_with_info(zds: dataset.Dataset, partition_info=None, shift=3):
         """Update function used for this test."""
         assert partition_info is not None
         assert isinstance(partition_info, tuple)
         assert len(partition_info) == 2
         assert isinstance(partition_info[0], str)
         assert isinstance(partition_info[1], slice)
         assert partition_info[0] == 'num_lines'
-        return dict(var2=ds.variables['var1'].values * -1 + shift)
+        return {'var2': zds.variables['var1'].values * -1 + shift}
 
-    zcollection.update(update_with_info, depth=1, shift=10)  # type: ignore
+    zcollection.update(
+        update_with_info,  # type: ignore
+        delayed=delayed,
+        depth=1,
+        shift=10)
 
-    data = zcollection.load()
+    data = zcollection.load(delayed=delayed)
     assert data is not None
     assert numpy.allclose(data.variables['var2'].values,
                           data.variables['var1'].values * -1 + 10,
                           rtol=0)
 
-    def invalid_var_name(ds: dataset.Dataset):
+    def update_and_trim(zds: dataset.Dataset, partition_info=None):
+        """Update function used for this test."""
+        assert partition_info is not None
+        assert partition_info[0] == 'num_lines'
+        zds = zds.isel(dict((partition_info, )))
+        return {'var2': zds.variables['var1'].values * -1}
+
+    zcollection.update(
+        update_and_trim,  # type: ignore
+        delayed=delayed,
+        trim=False,
+        depth=1)
+
+    data = zcollection.load(delayed=delayed)
+    assert data is not None
+    assert numpy.allclose(data.variables['var2'].values,
+                          data.variables['var1'].values * -1,
+                          rtol=0)
+
+    def invalid_var_name(zds: dataset.Dataset):
         """Update function used to test if the user wants to update a non-
         existent variable name."""
-        return dict(var99=ds.variables['var1'].values * -1 + 3)
+        return {'var99': zds.variables['var1'].values * -1 + 3}
 
     with pytest.raises(ValueError):
         zcollection.update(invalid_var_name)  # type: ignore
 
 
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_drop_partitions(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     arg,
     request,
-):
+) -> None:
     """Test the dropping of a dataset."""
     tested_fs = request.getfixturevalue(arg)
-    zcollection = create_test_collection(tested_fs)
+    zcollection = create_test_collection(tested_fs, delayed=False)
 
     all_partitions = list(zcollection.partitions())
     assert 'month=01' in [
         item.split(zcollection.fs.sep)[-2] for item in all_partitions
     ]
 
     zcollection.drop_partitions(filters='year == 2000 and month==1')
@@ -302,46 +352,46 @@
 
 
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_drop_variable(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     arg,
     request,
-):
+) -> None:
     """Test the dropping of a variable."""
     tested_fs = request.getfixturevalue(arg)
-    zcollection = create_test_collection(tested_fs)
+    zcollection = create_test_collection(tested_fs, delayed=False)
 
     with pytest.raises(ValueError):
         zcollection.drop_variable('time')
     zcollection.drop_variable('var1')
 
     with pytest.raises(ValueError):
         zcollection.drop_variable('var1')
 
-    ds = zcollection.load()
-    assert ds is not None
-    assert 'var1' not in ds.variables
+    zds = zcollection.load(delayed=False)
+    assert zds is not None
+    assert 'var1' not in zds.variables
 
     zcollection = convenience.open_collection(str(tested_fs.collection),
                                               mode='r',
                                               filesystem=tested_fs.fs)
     with pytest.raises(io.UnsupportedOperation):
         zcollection.drop_partitions()
 
 
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_add_variable(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     arg,
     request,
-):
+) -> None:
     """Test the adding of a variable."""
     tested_fs = request.getfixturevalue(arg)
-    zcollection = create_test_collection(tested_fs)
+    zcollection = create_test_collection(tested_fs, delayed=False)
 
     # Variable already exists
     new = meta.Variable(name='time',
                         dtype=numpy.dtype('float64'),
                         dimensions=('time', ))
     with pytest.raises(ValueError):
         zcollection.add_variable(new)
@@ -374,37 +424,40 @@
     # Testing the configuration update by reopening the collection
     zcollection = collection.Collection.from_config(path=str(
         tested_fs.collection),
                                                     filesystem=tested_fs.fs)
 
     assert new.name in zcollection.metadata.variables
 
-    ds = zcollection.load()
-    assert ds is not None
-    values = ds.variables['var3'].values
+    zds = zcollection.load(delayed=False)
+    assert zds is not None
+    values = zds.variables['var3'].values
     assert isinstance(values, numpy.ma.MaskedArray)
     assert numpy.all(values.mask)  # type: ignore
 
 
-@pytest.mark.parametrize('arg,create_test_data', FILE_SYSTEM_DATASET)
+@pytest.mark.parametrize('fs,create_test_data', FILE_SYSTEM_DATASET)
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_add_update(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
+    arrays_type,
     create_test_data,
     request,
-):
+) -> None:
     """Test the adding and updating of a dataset."""
-    tested_fs = request.getfixturevalue(arg)
-    ds = next(create_test_data())
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
+    zds = next(create_test_data(delayed=delayed))
     zcollection = collection.Collection('time',
-                                        ds.metadata(),
+                                        zds.metadata(),
                                         partitioning.Date(('time', ), 'D'),
                                         str(tested_fs.collection),
                                         filesystem=tested_fs.fs)
-    zcollection.insert(ds)
+    zcollection.insert(zds)
 
     new1 = meta.Variable(name='var3',
                          dtype=numpy.dtype('float64'),
                          dimensions=('num_lines', 'num_pixels'),
                          attrs=(dataset.Attribute(name='attr', value=1), ),
                          fill_value=1000000.5)
 
@@ -414,68 +467,78 @@
         dimensions=('num_lines', 'num_pixels'),
         fill_value=32267,
         attrs=(dataset.Attribute(name='attr', value=4), ),
     )
     zcollection.add_variable(new1)
     zcollection.add_variable(new2)
 
-    data = zcollection.load()
+    data = zcollection.load(delayed=delayed)
     assert data is not None
 
-    def update_1(ds, varname):
+    def update_1(zds, varname):
         """Update function used for this test."""
-        return {varname: ds.variables['var1'].data * 201.5}
+        return {varname: zds.variables['var1'].values * 201.5}
 
-    def update_2(ds, varname):
+    def update_2(zds, varname):
         """Update function used for this test."""
-        return {varname: ds.variables['var1'].data // 5}
+        return {varname: zds.variables['var1'].values // 5}
 
-    zcollection.update(update_1, new1.name)  # type: ignore
-    zcollection.update(update_2, new2.name)  # type: ignore
+    zcollection.update(update_1, new1.name, delayed=delayed)  # type: ignore
+    zcollection.update(update_2, new2.name, delayed=delayed)  # type: ignore
+
+    if delayed is False:
+        # If the dataset is not delayed, we need to reload it.
+        data = zcollection.load(delayed=False)
+        assert data is not None
 
     assert numpy.allclose(data.variables[new1.name].values,
                           data.variables['var1'].values * 201.5,
                           rtol=0)
     assert numpy.allclose(data.variables[new2.name].values,
                           data.variables['var1'].values // 5,
                           rtol=0)
 
 
-@pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('fs', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_fillvalue(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
+    arrays_type,
     request,
-):
+) -> None:
     """Test the management of masked values."""
-    tested_fs = request.getfixturevalue(arg)
-    zcollection = create_test_collection(tested_fs, with_fillvalue=True)
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
+    zcollection = create_test_collection(tested_fs,
+                                         delayed=delayed,
+                                         with_fillvalue=True)
 
     # Load the dataset written with masked values in the collection and
     # compare it to the original dataset.
-    data = zcollection.load()
+    data = zcollection.load(delayed=delayed)
     assert data is not None
 
-    ds = next(create_test_dataset_with_fillvalue())
+    zds = next(create_test_dataset_with_fillvalue(delayed=delayed))
 
     values = data.variables['var1'].values
     assert isinstance(values, numpy.ma.MaskedArray)
-    assert numpy.ma.allclose(ds.variables['var1'].values, values)
+    assert numpy.ma.allclose(zds.variables['var1'].values, values)
 
     values = data.variables['var2'].values
     assert isinstance(values, numpy.ma.MaskedArray)
-    assert numpy.ma.allclose(ds.variables['var2'].values, values)
+    assert numpy.ma.allclose(zds.variables['var2'].values, values)
 
 
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_degraded_tests(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     arg,
     request,
-):
+) -> None:
     """Test the degraded functionality."""
     tested_fs = request.getfixturevalue(arg)
     zcollection = create_test_collection(tested_fs)
 
     fake_ds = next(create_test_dataset())
     fake_ds.variables['var3'] = fake_ds.variables['var1']
     fake_ds.variables['var3'].name = 'var3'
@@ -485,166 +548,176 @@
 
 
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_insert_with_missing_variable(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     arg,
     request,
-):
+) -> None:
     """Test of the insertion of a dataset in which a variable is missing.
 
     This happens, for example, when a variable is not acquired, but
     created by an algorithm.
     """
     tested_fs = request.getfixturevalue(arg)
-    ds = next(create_test_dataset_with_fillvalue()).to_xarray()
+    zds = next(create_test_dataset_with_fillvalue()).to_xarray()
     zcollection = convenience.create_collection(
         axis='time',
-        ds=ds,
+        ds=zds,
         partition_handler=partitioning.Date(('time', ), 'M'),
         partition_base_dir=str(tested_fs.collection),
         filesystem=tested_fs.fs)
-    zcollection.insert(ds, merge_callable=merging.merge_time_series)
+    zcollection.insert(zds, merge_callable=merging.merge_time_series)
 
-    ds = next(create_test_dataset_with_fillvalue())
-    ds.drops_vars('var1')
-    zcollection.insert(ds)
+    zds = next(create_test_dataset_with_fillvalue())
+    zds.drops_vars('var1')
+    zcollection.insert(zds)
 
     data = zcollection.load()
     assert data is not None
     assert numpy.ma.allequal(
         data.variables['var1'].values,
         numpy.ma.masked_equal(
-            numpy.full(ds.variables['var1'].shape,
-                       ds.variables['var1'].fill_value,
-                       ds.variables['var1'].dtype),
-            ds.variables['var1'].fill_value))
+            numpy.full(zds.variables['var1'].shape,
+                       zds.variables['var1'].fill_value,
+                       zds.variables['var1'].dtype),
+            zds.variables['var1'].fill_value))
 
 
-@pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('fs', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_insert_failed(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
+    arrays_type,
     request,
-):
+) -> None:
     """Test the insertion of a dataset in which the insertion failed."""
-    tested_fs = request.getfixturevalue(arg)
-    ds = next(create_test_dataset())
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
+    zds = next(create_test_dataset(delayed=delayed))
     zcollection = collection.Collection('time',
-                                        ds.metadata(),
+                                        zds.metadata(),
                                         partitioning.Date(('time', ), 'D'),
                                         str(tested_fs.collection),
                                         filesystem=tested_fs.fs)
-    partitions = list(zcollection.partitioning.split_dataset(ds, 'time'))
+    partitions = list(zcollection.partitioning.split_dataset(zds, 'time'))
 
     # Create a file in the directory where the dataset should be written. This
     # should cause the insertion to fail.
     sep = zcollection.fs.sep
     one_directory = sep.join((zcollection.partition_properties.dir, ) +
                              partitions[0][0])
     zcollection.fs.makedirs(sep.join(one_directory.split(sep)[:-1]))
     zcollection.fs.touch(one_directory)
 
     with pytest.raises((OSError, ValueError)):
-        zcollection.insert(ds)
+        zcollection.insert(zds)
 
     # Because the insert failed, the partition that was supposed to be created
     # was deleted.
     assert not zcollection.fs.exists(one_directory)
-    zcollection.insert(ds)
+    zcollection.insert(zds)
 
 
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_insert_validation(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     arg,
     request,
-):
+) -> None:
     """Test the insertion of a dataset with metadata validation."""
     tested_fs = request.getfixturevalue(arg)
-    ds = next(create_test_dataset_with_fillvalue())
+    zds = next(create_test_dataset_with_fillvalue())
 
     zcollection = convenience.create_collection(
         axis='time',
-        ds=ds,
+        ds=zds,
         partition_handler=partitioning.Date(('time', ), 'M'),
         partition_base_dir=str(tested_fs.collection),
         filesystem=tested_fs.fs)
-    zcollection.insert(ds, merge_callable=merging.merge_time_series)
+    zcollection.insert(zds, merge_callable=merging.merge_time_series)
 
-    ds = next(create_test_dataset_with_fillvalue())
+    zds = next(create_test_dataset_with_fillvalue())
 
     # Inserting a dataset containing valid attributes
-    zcollection.insert(ds, validate=True)
+    zcollection.insert(zds)
 
     # Inserting a dataset containing an invalid attributes
-    ds = next(create_test_dataset_with_fillvalue())
-    ds.attrs = (meta.Attribute('invalid', 1), )
+    zds = next(create_test_dataset_with_fillvalue())
+    zds.attrs = (meta.Attribute('invalid', 1), )
 
     with pytest.raises(ValueError):
-        zcollection.insert(ds, validate=True)
+        zcollection.insert(zds, validate=True)
 
     # Inserting a dataset containing variables with invalid attributes
-    ds = next(create_test_dataset_with_fillvalue())
+    zds = next(create_test_dataset_with_fillvalue())
 
-    for var in ds.variables.values():
+    for var in zds.variables.values():
         var.attrs = (meta.Attribute('invalid', 1), )
 
     with pytest.raises(ValueError):
-        zcollection.insert(ds, validate=True)
+        zcollection.insert(zds, validate=True)
 
 
-@pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('fs', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_map_partition(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
+    arrays_type,
     request,
-):
+) -> None:
     """Test the update of a dataset."""
-    tested_fs = request.getfixturevalue(arg)
-    zcollection = create_test_collection(tested_fs)
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
+    zcollection = create_test_collection(tested_fs, delayed=delayed)
 
     result = zcollection.map(
-        lambda x: x.variables['var1'].values * 2)  # type: ignore
+        lambda x: x.variables['var1'].values * 2,  # type: ignore
+        delayed=delayed)
     for item in result.compute():
         folder = zcollection.fs.sep.join(
             (zcollection.partition_properties.dir,
              zcollection.partitioning.join(item[0], zcollection.fs.sep)))
-        ds = storage.open_zarr_group(folder, zcollection.fs)
-        assert numpy.allclose(item[1], ds.variables['var1'].values * 2)
+        zds = storage.open_zarr_group(folder, zcollection.fs, delayed=False)
+        assert numpy.allclose(item[1], zds.variables['var1'].values * 2)
 
 
-@pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('fs', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_indexer(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
+    arrays_type,
     request,
-):
+) -> None:
     """Test the update of a dataset."""
-    tested_fs = request.getfixturevalue(arg)
-    zcollection = create_test_collection(tested_fs)
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
+    zcollection = create_test_collection(tested_fs, delayed=delayed)
 
     indexers = zcollection.map(
         lambda x: slice(0, x.dimensions['num_lines'])  # type: ignore
     ).compute()
-    ds1 = zcollection.load(indexer=indexers)
-    assert ds1 is not None
-    ds2 = zcollection.load()
-    assert ds2 is not None
+    zds1 = zcollection.load(indexer=indexers, delayed=delayed)
+    assert zds1 is not None
+    zds2 = zcollection.load(delayed=delayed)
+    assert zds2 is not None
 
-    assert numpy.allclose(ds1.variables['var1'].values,
-                          ds2.variables['var1'].values)
+    assert numpy.allclose(zds1.variables['var1'].values,
+                          zds2.variables['var1'].values)
 
 
-def test_variables():
+def test_variables() -> None:
     """Test the listing of the variables in a collection."""
     fs = fsspec.filesystem('memory')
-    ds = next(create_test_dataset())
+    zds = next(create_test_dataset(delayed=False))
     zcollection = collection.Collection(axis='time',
-                                        ds=ds.metadata(),
+                                        ds=zds.metadata(),
                                         partition_handler=partitioning.Date(
                                             ('time', ), 'D'),
                                         partition_base_dir='/',
                                         filesystem=fs)
     variables = zcollection.variables()
     assert isinstance(variables, tuple)
     assert len(variables) == 3
@@ -653,151 +726,156 @@
     assert variables[2].name == 'var2'
 
     variables = zcollection.variables(('time', ))
     assert len(variables) == 1
     assert variables[0].name == 'time'
 
 
-@pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('fs', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_map_overlap(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
+    arrays_type,
     request,
-):
+) -> None:
     """Test the map overlap method."""
-    tested_fs = request.getfixturevalue(arg)
-    zcollection = create_test_collection(tested_fs)
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
+    zcollection = create_test_collection(tested_fs, delayed=delayed)
 
-    def func(ds: dataset.Dataset, partition_info: tuple[str, slice]):
+    def func(zds: dataset.Dataset, partition_info: tuple[str, slice]):
         assert partition_info[0] == 'num_lines'
-        var = ds.variables['var1']
+        var = zds.variables['var1']
         slices = [slice(None)] * len(var.dimensions)
         slices[var.dimensions.index(partition_info[0])] = partition_info[1]
         return var.values[tuple(slices)] * 2
 
-    result = zcollection.map_overlap(func, depth=1)  # type: ignore
+    result = zcollection.map_overlap(
+        func,  # type: ignore
+        delayed=delayed,
+        depth=1)
 
     for partition, data in result.compute():
         folder = zcollection.fs.sep.join(
             (zcollection.partition_properties.dir,
              zcollection.partitioning.join(partition, zcollection.fs.sep)))
-        ds = storage.open_zarr_group(folder, zcollection.fs)
-        assert numpy.allclose(data, ds.variables['var1'].values * 2)
+        zds = storage.open_zarr_group(folder, zcollection.fs, delayed=False)
+        assert numpy.allclose(data, zds.variables['var1'].values * 2)
 
 
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_insert_immutable(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     arg,
     request,
-):
+) -> None:
     """Test the insertion of a dataset with variables that are immutable
     relative to the partitioning."""
     tested_fs = request.getfixturevalue(arg)
 
-    def make_dask_array(arr):
-        return dask.array.core.from_array(arr)
-
-    ds = dataset.Dataset(
+    zds_reference = dataset.Dataset(
         [
-            dataset.Variable(
+            dataset.Array(
                 'time',
-                make_dask_array(  # type: ignore
-                    numpy.arange(numpy.datetime64('2000-01-01'),
-                                 numpy.datetime64('2000-01-30'),
-                                 numpy.timedelta64(1, 'D'))),
+                numpy.arange(numpy.datetime64('2000-01-01'),
+                             numpy.datetime64('2000-01-30'),
+                             numpy.timedelta64(1, 'D')),
                 ('time', ),
             ),
-            dataset.Variable(
+            dataset.Array(
                 'lon',
-                make_dask_array(numpy.arange(0, 360, 1)),  # type: ignore
+                numpy.arange(0, 360, 1),
                 ('lon', ),
             ),
-            dataset.Variable(
+            dataset.Array(
                 'lat',
-                make_dask_array(numpy.arange(-90, 90, 1)),  # type: ignore
+                numpy.arange(-90, 90, 1),
                 ('lat', ),
             ),
-            dataset.Variable(
+            dataset.Array(
                 'grid',
-                make_dask_array(
-                    numpy.random.rand(  # type: ignore
-                        29,
-                        360,
-                        180,
-                    )),
+                numpy.random.rand(
+                    29,
+                    360,
+                    180,
+                ),
                 ('time', 'lon', 'lat'),
             ),
         ],
-        (dataset.Attribute('history', 'Created for testing'), ),
+        attrs=(dataset.Attribute('history', 'Created for testing'), ),
     )
     zcollection = collection.Collection('time',
-                                        ds.metadata(),
+                                        zds_reference.metadata(),
                                         partitioning.Date(('time', ), 'D'),
                                         str(tested_fs.collection),
                                         filesystem=tested_fs.fs)
     assert zcollection.immutable
     assert not tested_fs.fs.exists(zcollection._immutable)
-    zcollection.insert(ds)
+    zcollection.insert(zds_reference)
     assert tested_fs.fs.exists(zcollection._immutable)
 
-    zds = zcollection.load()
+    zds = zcollection.load(delayed=False)
     assert zds is not None
 
     assert numpy.all(
-        zds.variables['grid'].values == ds.variables['grid'].values)
+        zds.variables['grid'].values == zds_reference.variables['grid'].values)
     assert numpy.all(
-        zds.variables['time'].values == ds.variables['time'].values)
-    assert numpy.all(zds.variables['lon'].values == ds.variables['lon'].values)
-    assert numpy.all(zds.variables['lat'].values == ds.variables['lat'].values)
+        zds.variables['time'].values == zds_reference.variables['time'].values)
+    assert numpy.all(
+        zds.variables['lon'].values == zds_reference.variables['lon'].values)
+    assert numpy.all(
+        zds.variables['lat'].values == zds_reference.variables['lat'].values)
 
-    def update(ds: dataset.Dataset, varname: str) -> dict[str, numpy.ndarray]:
+    def update(zds: dataset.Dataset, varname: str) -> dict[str, numpy.ndarray]:
         """Update function used for this test."""
-        return {varname: ds.variables['grid'].values * -1}
+        return {varname: zds.variables['grid'].values * -1}
 
-    zcollection.update(update, varname='grid')  # type: ignore
-    zds = zcollection.load()
+    zcollection.update(update, delayed=False, varname='grid')  # type: ignore
+    zds = zcollection.load(delayed=False)
     assert zds is not None
 
+    assert numpy.all(zds.variables['grid'].values ==
+                     zds_reference.variables['grid'].values * -1)
     assert numpy.all(
-        zds.variables['grid'].values == ds.variables['grid'].values * -1)
+        zds.variables['time'].values == zds.variables['time'].values)
     assert numpy.all(
-        zds.variables['time'].values == ds.variables['time'].values)
-    assert numpy.all(zds.variables['lon'].values == ds.variables['lon'].values)
-    assert numpy.all(zds.variables['lat'].values == ds.variables['lat'].values)
+        zds.variables['lon'].values == zds.variables['lon'].values)
+    assert numpy.all(
+        zds.variables['lat'].values == zds.variables['lat'].values)
 
     new_variable = meta.Variable(
         'new_var',
         numpy.float64,
-        ('time', 'lon', 'lat'),
-        (meta.Attribute('units', 'm'), ),
+        dimensions=('time', 'lon', 'lat'),
+        attrs=(meta.Attribute('units', 'm'), ),
     )
     zcollection.add_variable(new_variable)
     zcollection.update(update, varname='new_var')  # type: ignore
     zds = zcollection.load()
     assert zds is not None
-    assert numpy.all(
-        zds.variables['new_var'].values == ds.variables['grid'].values)
+    assert numpy.all(zds.variables['new_var'].values ==
+                     zds_reference.variables['grid'].values)
 
     new_variable = meta.Variable(
         'new_var2',
         numpy.float64,
-        ('another_dim', ),
-        (meta.Attribute('units', 'm'), ),
+        dimensions=('another_dim', ),
+        attrs=(meta.Attribute('units', 'm'), ),
     )
     with pytest.raises(ValueError):
         zcollection.add_variable(new_variable)
 
 
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_copy_collection(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
         arg,
         request,
-        tmpdir):
+        tmpdir) -> None:
     """Test the dropping of a dataset."""
     tested_fs = request.getfixturevalue(arg)
     zcollection = create_test_collection(tested_fs)
 
     target = str(tmpdir / 'copy')
     zcopy = zcollection.copy(target, filesystem=fsspec.filesystem('file'))
 
@@ -809,113 +887,119 @@
 
     assert numpy.all(ds_before_copy.variables['var1'].values ==
                      ds_after_copy.variables['var1'].values)
     assert numpy.all(ds_before_copy.variables['var2'].values ==
                      ds_after_copy.variables['var2'].values)
 
 
-def _insert(ds: dataset.Dataset, base_dir: str, lock_file: str,
-            scheduler_file: str):
+def _insert(zds: dataset.Dataset, base_dir: str, lock_file: str,
+            scheduler_file: str) -> None:
     client = dask.distributed.Client(scheduler_file=scheduler_file)
     zcollection = collection.Collection.from_config(
         base_dir, mode='w', synchronizer=sync.ProcessSync(lock_file))
-    zcollection.insert(ds, merge_callable=merging.merge_time_series)
+    zcollection.insert(zds, merge_callable=merging.merge_time_series)
+    client.close()
 
 
 # pylint: disable=too-many-statements
 def test_concurrent_insert(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     tmpdir,
-):
+) -> None:
     """Test the insertion of a dataset."""
     fs = fsspec.filesystem('file')
-    datasets = list(create_test_dataset())
-    ds = datasets[0]
+    datasets = list(create_test_dataset(delayed=False))
+    zds = datasets[0]
     lock_file = str(tmpdir / 'lock.lck')
     synchronizer = sync.ProcessSync(lock_file)
     base_dir = str(tmpdir / 'test')
     zcollection = collection.Collection('time',
-                                        ds.metadata(),
+                                        zds.metadata(),
                                         partitioning.Date(('time', ), 'D'),
                                         base_dir,
                                         filesystem=fs,
                                         synchronizer=synchronizer)
 
-    pool = concurrent.futures.ProcessPoolExecutor(max_workers=8)
+    pool = concurrent.futures.ProcessPoolExecutor(max_workers=32)
     futures = []
 
     assert zcollection.is_locked() is False
 
-    indices = numpy.arange(0, len(datasets))
+    indices = list(numpy.arange(0, len(datasets)))
     numpy.random.shuffle(indices)
     futures = [
         pool.submit(_insert, datasets[ix], base_dir, lock_file,
                     dask_client.scheduler_file) for ix in indices
     ]
 
-    def update(ds: dataset.Dataset, shift: int = 3):
+    def update(zds: dataset.Dataset, shift: int = 3):
         """Update function used for this test."""
-        return dict(var2=ds.variables['var1'].values * -1 + shift)
+        return {'var2': zds.variables['var1'].values * -1 + shift}
 
     launch_update = True
     for item in concurrent.futures.as_completed(futures):
+        assert item.exception() is None
         if launch_update:
             zcollection.update(update)  # type: ignore
             launch_update = False
 
     data = zcollection.load()
     assert data is not None
     values = data.variables['time'].values
+
     assert numpy.all(values == numpy.arange(START_DATE, END_DATE, DELTA))
 
 
 def test_partition_modified(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
         tmpdir):
     """Test the loading of a variable that has been modified since its
     creation."""
     fs = fsspec.filesystem('file')
     datasets = list(create_test_dataset())
-    ds = datasets[0]
+    zds = datasets[0]
     base_dir = str(tmpdir / 'test')
     zcollection = collection.Collection('time',
-                                        ds.metadata(),
+                                        zds.metadata(),
                                         partitioning.Date(('time', ), 'D'),
                                         base_dir,
                                         filesystem=fs)
-    zcollection.insert(ds)
+    zcollection.insert(zds)
 
     last_month = zcollection.load(filters=lambda keys: keys['year'] == 2000 and
                                   keys['month'] == 1 and keys['day'] == 16)
     assert last_month is not None
 
-    ds = zcollection.load()
-    assert ds is not None
+    zds = zcollection.load()
+    assert zds is not None
 
     def new_shape(
         var: variable.Variable,
         selected_dim: str,
         new_size: int,
     ) -> tuple[int, ...]:
         """Compute the new shape of a variable."""
         return tuple(new_size if dim == selected_dim else size
                      for dim, size in zip(var.dimensions, var.shape))
 
     dim, size = 'num_lines', last_month.dimensions['num_lines'] * 25
-    last_month = dataset.Dataset([
-        variable.Variable(
-            name,
-            numpy.resize(var.array.compute(), new_shape(var, dim, size)),
-            var.dimensions,
-            var.attrs,
-            var.compressor,
-            var.fill_value,
-            var.filters,
-        ) for name, var in last_month.variables.items()
-    ])
+    last_month = dataset.Dataset(
+        [
+            variable.DelayedArray(
+                name,
+                numpy.resize(var.array.compute(), new_shape(var, dim, size)),
+                var.dimensions,
+                attrs=var.attrs,
+                compressor=var.compressor,
+                fill_value=var.fill_value,
+                filters=var.filters,
+            ) for name, var in last_month.variables.items()
+        ],
+        attrs=zds.attrs,
+    )
     zcollection.insert(last_month)
 
     with pytest.raises(RuntimeError, match='Try to re-load'):
-        _ = ds['var2'].values
+        _ = zds['var2'].values
 
     with pytest.raises(RuntimeError, match='Try to re-load'):
-        _ = ds['time'].values
+        _ = zds['time'].values
```

### Comparing `zcollection-2023.3.2/zcollection/compressed_array.py` & `zcollection-2023.5.0/zcollection/compressed_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (c) 2023 CNES
+#
+# All rights reserved. Use of this source code is governed by a
+# BSD-style license that can be found in the LICENSE file.
 """
 Compressed array class
 ======================
 """
 from __future__ import annotations
 
 from typing import Any, Callable, Sequence, Union
@@ -62,15 +66,15 @@
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__} ({self.shape}) {self.dtype}>'
 
     def _repr_html_(self) -> str:
         # pylint: disable=protected-access
         # Useless to rewrite the html representation of the array. Use the
         # zarr one.
-        html_code = self._array.info._repr_html_()
+        html_code: str = self._array.info._repr_html_()
         #: pylint: enable=protected-access
         return html_code.replace('zarr.core.Array', str(type(self)))
 
     def __getitem__(
         self,
         key: int | tuple[int | slice, ...],
     ) -> Array:
@@ -78,15 +82,15 @@
 
         Args:
             key: The key to retrieve.
 
         Returns:
             The data for the key.
         """
-        values = self._array[key]
+        values: Array = self._array[key]
         if self._fill_value is not None:
             values = numpy.ma.masked_equal(values, self._fill_value)
         return values
 
     def __setitem__(
         self,
         key: int | tuple[int | slice, ...],
@@ -184,15 +188,15 @@
         Args:
             dtype: The data type of the array.
 
         Returns:
             The numpy.ndarray of the array or numpy.ma.masked_array if
             a fill_value is defined.
         """
-        array = self._array[...]
+        array: Array = self._array[...]
         if self._fill_value is not None:
             array = numpy.ma.masked_equal(array, self._fill_value)
         if dtype is not None:
             array = array.astype(dtype)
         return array
 
     def _cast(self, obj: Any) -> Any:
@@ -225,19 +229,19 @@
             types: The types of the arguments.
             args: The arguments.
             kwargs: The keyword arguments.
 
         Returns:
             The result of the numpy function.
         """
-        args = [
+        arrays: list[NDArray] = [
             item.__array__() if isinstance(item, CompressedArray) else item
             for item in args
         ]
-        return func(*args, **kwargs)
+        return func(*arrays, **kwargs)
 
     def __array_ufunc__(
         self,
         ufunc: Callable,
         method: str,
         *args,
         **kwargs,
@@ -285,38 +289,38 @@
 
     Args:
         array: The compressed array.
 
     Returns:
         The dask array.
     """
-    chunks = array.chunks
+    chunks: Sequence[Sequence[int]] = array.chunks
     if name is None:
         name = 'from-compressed-array-' + dask.base.tokenize(
             array, chunks, **kwargs)
     return dask.array.core.from_array(
         array,
         chunks,  # type: ignore
         name=name,
         inline_array=inline_array)
 
 
 @dask.array.dispatch.concatenate_lookup.register(CompressedArray)
-def _concatenate_compressed_array(arrays, **kwargs):
-    dtype = kwargs.get('dtype', None)
-    arr = [item.__array__(dtype=dtype) for item in arrays]
+def _concatenate_compressed_array(arrays, **kwargs) -> NDArray:
+    dtype: DType | None = kwargs.get('dtype', None)
+    arr: list[NDArray] = [item.__array__(dtype=dtype) for item in arrays]
     if any(tuple(item.fill_value is not None for item in arrays)):
         return numpy.ma.concatenate(arr, **kwargs)
     return numpy.concatenate(arr, **kwargs)
 
 
 @dask.array.dispatch.numel_lookup.register(CompressedArray)
-def _numel_compressed_array(array, **kwargs):
+def _numel_compressed_array(array, **kwargs) -> numpy.float64 | NDArray:
     #: pylint: disable=protected-access
     # array is a CompressedArray, we can access its _array attribute.
     # We reuse the implementation of dask array numel. Useless to
     # reimplement it.
-    arr = array.__array__(dtype=kwargs.get('dtype', None))
+    arr: NDArray = array.__array__(dtype=kwargs.get('dtype', None))
     if array._fill_value is not None:
         return dask.array.backends._numel_masked(arr, **kwargs)
     return dask.array.backends._numel_ndarray(arr, **kwargs)
     #: pylint: enable=protected-access
```

### Comparing `zcollection-2023.3.2/zcollection/conftest.py` & `zcollection-2023.5.0/zcollection/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 ==========
 Test setup
 ==========
 """
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser) -> None:
     """Add command line options to pytest."""
     parser.addoption(
         '--s3',
         action='store_true',
         default=False,
         help='Enable tests on the local S3 server driven by minio. '
         '(default: False)')
```

### Comparing `zcollection-2023.3.2/zcollection/convenience/collection.py` & `zcollection-2023.5.0/zcollection/convenience/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # BSD-style license that can be found in the LICENSE file.
 """
 Convenience functions
 =====================
 """
 from __future__ import annotations
 
+from typing import Literal
+
 import xarray
 
 from .. import collection, dataset, fs_utils, partitioning
 
 
 def create_collection(
     axis: str,
@@ -62,15 +64,15 @@
                                  filesystem=filesystem,
                                  **kwargs)
 
 
 # pylint: disable=redefined-builtin
 def open_collection(path: str,
                     *,
-                    mode: str | None = None,
+                    mode: Literal['r', 'w'] | None = None,
                     **kwargs) -> collection.Collection:
     """Open a collection.
 
     Args:
         path: The path to the collection.
         mode: The mode to open the collection.
         **kwargs: Additional parameters are passed through the method
```

### Comparing `zcollection-2023.3.2/zcollection/convenience/view.py` & `zcollection-2023.5.0/zcollection/convenience/view.py`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/zcollection/dask_utils.py` & `zcollection-2023.5.0/zcollection/dask_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     Returns:
         number of dask workers
 
     Raises:
         ValueError: If no dask workers are available.
     """
-    result = len(
+    result: int = len(
         client.ncores()) if cores_only else sum(  # type: ignore[arg-type]
             item
             for item in client.nthreads().values())  # type: ignore[arg-type]
     if result == 0:
         raise RuntimeError('No dask workers available')
     return result
 
@@ -46,15 +46,18 @@
 
     Returns:
         default dask client
     """
     try:
         return dask.distributed.get_client()
     except ValueError:
-        return dask.distributed.Client()
+        return dask.distributed.Client(
+            processes=False,
+            direct_to_workers=True,
+        )
 
 
 def split_sequence(sequence: Sequence[Any],
                    sections: int | None = None) -> Iterator[Sequence[Any]]:
     """Split a sequence into sections.
 
     Args:
@@ -64,17 +67,21 @@
 
     Returns:
         Iterator of sequences.
     """
     sections = len(sequence) if sections is None else sections
     if sections <= 0:
         raise ValueError('The number of sections must be greater than zero.')
-    length = len(sequence)
+    length: int = len(sequence)
     sections = min(sections, length)
+
+    size: int
+    extras: int
     size, extras = divmod(length, sections)
+
     div = tuple(
         itertools.accumulate([0] + extras * [size + 1] +
                              (sections - extras) * [size]))
     yield from (sequence[item:div[ix + 1]] for ix, item in enumerate(div[:-1]))
 
 
 def simple_delayed(name: str, func: Callable) -> dask_Delayed:
```

### Comparing `zcollection-2023.3.2/zcollection/dataset.py` & `zcollection-2023.5.0/zcollection/dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,40 +4,52 @@
 # BSD-style license that can be found in the LICENSE file.
 """
 Dataset
 =======
 """
 from __future__ import annotations
 
-from typing import Any, Iterable, Mapping, OrderedDict, Sequence
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Mapping,
+    OrderedDict,
+    Sequence,
+    Tuple,
+    Union,
+)
 import collections
 
 import dask.array.core
-import dask.array.creation
-import dask.array.ma
-import dask.array.rechunk
 import dask.array.routines
 import dask.array.wrap
 import dask.base
-import dask.threaded
-import fsspec
+import numpy
 import xarray
+import xarray.conventions
 
-from . import meta, variable
+from . import meta, representation
 from .compressed_array import CompressedArray
-from .meta import Attribute, Dimension
+from .meta import BLOCK_SIZE_LIMIT, Attribute, Dimension
 from .type_hints import ArrayLike, NDArray, NDMaskedArray
-from .variable import (
-    Variable,
-    _attributes_repr,
-    _calculate_column_width,
-    _dimensions_repr,
-    _new_variable,
-    _pretty_print,
-)
+from .variable import Array, DelayedArray, Variable, new_variable
+
+#: Alias to type hint for the dimensions of a dataset.
+DimensionType = Dict[str, int]
+
+#: Alias to type hint for the variables of a dataset.
+VariableType = OrderedDict[str, Variable]
+
+#: Alias to type hint for the attributes of a dataset.
+AttributeType = Tuple[Attribute, ...]
+
+#: Alias to type hint for the chunk sizes for each dimension of a dataset.
+ChunkType = Dict[str, Union[int, str]]
 
 
 def _dask_repr(array: dask.array.core.Array) -> str:
     """Get the string representation of a dask array.
 
     Args:
         array: A dask array.
@@ -45,147 +57,240 @@
     Returns:
         The string representation of the dask array.
     """
     chunksize = tuple(item[0] for item in array.chunks)
     return f'dask.array<chunksize={chunksize}>'
 
 
-def _dataset_repr(ds: Dataset) -> str:
+def _dataset_repr(zds: Dataset) -> str:
     """Get the string representation of a dataset.
 
     Args:
-        ds: A dataset.
+        zds: A dataset.
 
     Returns:
         The string representation of the dataset.
     """
     # Dimensions
-    dims_str = _dimensions_repr(ds.dimensions)
-    lines = [
-        f'<{ds.__module__}.{ds.__class__.__name__}>',
+    dims_str: str = representation.dimensions(zds.dimensions)
+    lines: list[str] = [
+        f'<{zds.__module__}.{zds.__class__.__name__}>',
         f'  Dimensions: {dims_str}', 'Data variables:'
     ]
     # Variables
-    if len(ds.variables) == 0:
+    if len(zds.variables) == 0:
         lines.append('    <empty>')
     else:
-        width = _calculate_column_width(ds.variables)
-        for name, var in ds.variables.items():
-            dims_str = f"({', '.join(map(str, var.dimensions))} "
-            name_str = f'    {name:<{width}s} {dims_str} {var.dtype}'
-            lines.append(_pretty_print(f'{name_str}: {_dask_repr(var.array)}'))
+        width: int = representation.calculate_column_width(zds.variables)
+        for name, var in zds.variables.items():
+            dims_str = f"({', '.join(map(str, var.dimensions))}) "
+            name_str: str = f'    {name:<{width}s} {dims_str} {var.dtype}'
+            data_str: str = _dask_repr(var.data) if zds.delayed else '...'
+            lines.append(
+                representation.pretty_print(f'{name_str}: {data_str}'))
     # Attributes
-    if len(ds.attrs):
+    if len(zds.attrs):
         lines.append('  Attributes:')
-        lines += _attributes_repr(ds.attrs)
+        lines += representation.attributes(zds.attrs)
 
     return '\n'.join(lines)
 
 
-def _duplicate(var: variable.Variable,
-               data: dask.array.core.Array) -> variable.Variable:
+def _duplicate_delayed_array(var: DelayedArray,
+                             data: dask.array.core.Array) -> DelayedArray:
     """Duplicate the variable with a new data.
 
     Args:
         var: Variable to duplicate.
         data: The new data to use
 
     Returns:
         The duplicated variable
     """
-    # pylint: disable=protected-access
-    # _new is a protected member of this class
-    return _new_variable(var.name, data, var.dimensions, var.attrs,
-                         var.compressor, var.fill_value, var.filters)
-    # pylint: enable=protected-access
+    return new_variable(type(var),
+                        name=var.name,
+                        array=data,
+                        dimensions=var.dimensions,
+                        attrs=var.attrs,
+                        compressor=var.compressor,
+                        fill_value=var.fill_value,
+                        filters=var.filters)
+
+
+def _duplicate_array(var: Array, data: NDArray) -> Array:
+    """Duplicate the variable with a new data.
+
+    Args:
+        var: Variable to duplicate.
+        data: The new data to use
+
+    Returns:
+        The duplicated variable
+    """
+    return new_variable(type(var),
+                        name=var.name,
+                        array=data,
+                        dimensions=var.dimensions,
+                        attrs=var.attrs,
+                        compressor=var.compressor,
+                        fill_value=var.fill_value,
+                        filters=var.filters)
+
+
+def _delete_delayed_vars(self: Dataset, indexer: slice | Sequence[int],
+                         axis: str) -> list[Variable]:
+    """Delete the variables along the given axis."""
+    return [
+        _duplicate_delayed_array(
+            var,  # type: ignore[arg-type]
+            dask.array.routines.delete(var.array, indexer,
+                                       var.dimensions.index(axis)))
+        for var in self.variables.values()
+    ]
+
+
+def _delete_vars(self: Dataset, indexer: slice | Sequence[int],
+                 axis: str) -> list[Variable]:
+    """Delete the variables along the given axis."""
+    return [
+        _duplicate_array(
+            var,  # type: ignore[arg-type]
+            numpy.delete(var.array, indexer, var.dimensions.index(axis)))
+        for var in self.variables.values()
+    ]
+
+
+def _update_dimensions(self: Dataset,
+                       delayed: bool | None = None) -> bool | None:
+    """Update the dimensions of the dataset based on its variables."""
+    for var in self.variables.values():
+        if delayed is None:
+            delayed = isinstance(var, DelayedArray)
+        elif delayed != isinstance(var, DelayedArray):
+            raise ValueError(
+                'the dataset contains both delayed and non-delayed '
+                'variables')
+        try:
+            for idx, dim in enumerate(var.dimensions):
+                if dim not in self.dimensions:
+                    self.dimensions[dim] = var.array.shape[idx]
+                elif self.dimensions[dim] != var.array.shape[idx]:
+                    raise ValueError(f'variable {var.name} has conflicting '
+                                     'dimensions')
+        except IndexError as exc:
+            raise ValueError(
+                f'variable {var.name} has missing dimensions') from exc
+    return delayed
 
 
 class Dataset:
     """Hold variables, dimensions, and attributes that together form a dataset.
 
-    Attrs:
-        variables: Dataset variables
-        attrs: Dataset attributes
-        chunks: Chunk size for each dimension.
-        block_size_limit: Maximum size (in bytes) of a
-            block/chunk of variable's data.
+    Args:
+        variables (DelayedArray | Array): A dictionary of variables in the
+            dataset, with variable names as keys and :py:class:`Array
+            <zcollection.variable.array.Array>` or :py:class:`DelayedArray
+            <zcollection.variable.delayed.DelayedArray>` objects as values.
+        attrs: A tuple of global attributes on this dataset.
+        block_size_limit: The maximum size (in bytes) of a block/chunk of
+            variable's data. Defaults to 128 MiB.
+        chunks: A dictionary of chunk sizes for each dimension.
+        delayed: A boolean indicating whether the dataset contains delayed
+            variables (numpy arrays wrapped in dask arrays).
 
     Raises:
         ValueError: If the dataset contains variables with the same dimensions
             but with different values.
+        ValueError: If the dataset contains both delayed and non-delayed
+            variables.
+
+    Notes:
+        The dataset is a dictionary-like container of variables. It also holds
+        the dimensions and attributes of the dataset.
+        If the dataset contains delayed variables, the values are
+        :py:class:`DelayedArray
+        <zcollection.variable.delayed_array.DelayedArray>` objects. Otherwise,
+        the values are :py:class:`Array
+        <zcollection.variable.array.Array>` objects. It is impossible to mix
+        delayed and non-delayed variables in the same dataset.
     """
     __slots__ = ('dimensions', 'variables', 'attrs', 'chunks',
-                 'block_size_limit')
+                 'block_size_limit', 'delayed')
 
     def __init__(self,
-                 variables: Iterable[variable.Variable],
+                 variables: Iterable[Variable],
+                 *,
                  attrs: Sequence[Attribute] | None = None,
+                 block_size_limit: int | None = None,
                  chunks: Sequence[Dimension] | None = None,
-                 block_size_limit: int | None = None) -> None:
+                 delayed: bool | None = None) -> None:
         #: The list of global attributes on this dataset
-        self.attrs = tuple(attrs or [])
-        #: Dataset contents as dict of
-        #: :py:class:`Variable <zcollection.variable.Variable>` objects.
+        self.attrs = tuple(attrs or ())
+
+        #: Dataset contents as dict of :py:class:`Variable
+        #: <zcollection.variable.abc.Variable>` objects. If the dataset
+        #: contains delayed variables, the values are :py:class:`DelayedArray
+        #: <zcollection.variable.delayed_array.DelayedArray>` objects.
+        #: Otherwise, the values are :py:class:`Array
+        #: <zcollection.variable.array.Array>` objects.
         self.variables = collections.OrderedDict(
             (item.name, item) for item in variables)
+
         #: A dictionary of dimension names and their index in the dataset
-        self.dimensions: dict[str, int] = {}
+        self.dimensions: DimensionType = {}
 
-        for var in self.variables.values():
-            try:
-                for ix, dim in enumerate(var.dimensions):
-                    if dim not in self.dimensions:
-                        self.dimensions[dim] = var.array.shape[ix]
-                    elif self.dimensions[dim] != var.array.shape[ix]:
-                        raise ValueError(
-                            f'variable {var.name} has conflicting '
-                            'dimensions')
-            except IndexError as exc:
-                raise ValueError(
-                    f'variable {var.name} has missing dimensions') from exc
+        # Loops over each variable in the dataset and updates the dimensions
+        # according to the shape of the array.
+        delayed = _update_dimensions(self, delayed)
 
         #: Maximum data chunk size
-        self.block_size_limit = block_size_limit or meta.BLOCK_SIZE_LIMIT
+        self.block_size_limit: int = block_size_limit or BLOCK_SIZE_LIMIT
 
         #: Chunk size for each dimension
-        chunks = chunks or []
-        self.chunks: dict[str,
-                          int | str] = {dim.name: dim.value
-                                        for dim in chunks}
+        self.chunks: ChunkType = {dim.name: dim.value for dim in chunks or []}
+
+        #: The type of variables in the dataset
+        self.delayed: bool = delayed if delayed is not None else True
 
     def __len__(self) -> int:
         return len(self.variables)
 
     def __bool__(self) -> bool:
         return bool(self.variables)
 
-    def __getitem__(self, name: str) -> variable.Variable:
+    def __getitem__(self, name: str) -> Variable:
         """Return a variable from the dataset.
 
         Args:
             name: The name of the variable to return
 
         Returns:
             The variable
 
         Raises:
             KeyError: If the variable is not found
         """
         return self.variables[name]
 
+    def __getattr__(self, name: str) -> Any:
+        if name in self.variables:
+            return self.variables[name]
+        raise AttributeError(
+            f"'{self.__class__.__name__}' object has no attribute '{name}'")
+
     def __getstate__(self) -> tuple[Any, ...]:
         return (self.dimensions, self.variables, self.attrs, self.chunks,
-                self.block_size_limit)
+                self.block_size_limit, self.delayed)
 
     def __setstate__(
-        self, state: tuple[dict[str, int], OrderedDict[str, variable.Variable],
-                           tuple[Attribute, ...], dict[str, int | str], int]
+        self, state: tuple[DimensionType, VariableType, AttributeType,
+                           ChunkType, int, bool]
     ) -> None:
         (self.dimensions, self.variables, self.attrs, self.chunks,
-         self.block_size_limit) = state
+         self.block_size_limit, self.delayed) = state
 
     @property
     def nbytes(self) -> int:
         """Return the total number of bytes in the dataset.
 
         Returns:
             The total number of bytes in the dataset
@@ -200,15 +305,15 @@
             Dimensions associated to their chunk size.
         """
         return tuple(Dimension(*item) for item in self.chunks.items())
 
     def add_variable(self,
                      var: meta.Variable,
                      /,
-                     data: ArrayLike[Any] | None = None):
+                     data: ArrayLike[Any] | None = None) -> None:
         """Add a variable to the dataset.
 
         Args:
             var: The variable to add
             data: The data to add to the variable. If not provided, the variable
                 will be created with the default fill value.
 
@@ -219,30 +324,33 @@
         """
         if set(var.dimensions) - set(self.dimensions):
             raise ValueError(f'variable {var.name} has dimensions '
                              f'{var.dimensions} that are not in the dataset')
 
         if data is None:
             shape = tuple(self.dimensions[dim] for dim in var.dimensions)
-            data = dask.array.wrap.full(shape, var.fill_value, dtype=var.dtype)
+            data = dask.array.wrap.full(
+                shape, var.fill_value,
+                dtype=var.dtype) if self.delayed else numpy.full(
+                    shape, var.fill_value, dtype=var.dtype)
         else:
             for dim, size in zip(var.dimensions, data.shape):
                 if size != self.dimensions[dim]:
                     raise ValueError(
                         f'Conflicting sizes for dimension {dim!r}: '
                         f'length {self.dimensions[dim]} on the data but length '
                         f'{size} defined in dataset.')
-        self.variables[var.name] = Variable(
+        self.variables[var.name] = (DelayedArray if self.delayed else Array)(
             var.name,
-            data,  # type: ignore[arg-type]
+            data,
             var.dimensions,
-            var.attrs,
-            var.compressor,
-            var.fill_value,
-            var.filters,
+            attrs=var.attrs,
+            compressor=var.compressor,
+            fill_value=var.fill_value,
+            filters=var.filters,
         )
 
     def rename(self, names: Mapping[str, str]) -> None:
         """Rename variables in the dataset.
 
         Args:
             names: A mapping from old names to new names
@@ -272,62 +380,69 @@
             names: Variable names to select.
 
         Returns:
             A new dataset containing only the selected variables.
         """
         if isinstance(names, str) or not isinstance(names, Iterable):
             names = [names]
-        return Dataset([self.variables[name] for name in names],
-                       self.attrs,
-                       chunks=self.dims_chunk,
-                       block_size_limit=self.block_size_limit)
+        return Dataset((self.variables[name] for name in names),
+                       attrs=self.attrs,
+                       block_size_limit=self.block_size_limit,
+                       chunks=self.dims_chunk)
 
     def metadata(self) -> meta.Dataset:
         """Get the dataset metadata.
 
         Returns:
             Dataset metadata
         """
         return meta.Dataset(
             dimensions=tuple(self.dimensions.keys()),
             variables=tuple(item.metadata()
                             for item in self.variables.values()),
             attrs=self.attrs,
             chunks=tuple(Dimension(*item) for item in self.chunks.items()),
-            block_size_limit=self.block_size_limit)
+            block_size_limit=self.block_size_limit,
+        )
 
     @staticmethod
-    def from_xarray(ds: xarray.Dataset) -> Dataset:
+    def from_xarray(zds: xarray.Dataset, delayed: bool = True) -> Dataset:
         """Create a new dataset from a xarray dataset.
 
         Args:
-            ds: Dataset to convert.
+            zds: Dataset to convert.
+            delayed: If True, the data will be wrapped in a dask array. If
+                False, the data will be handled as a numpy array.
 
         Returns:
             New dataset.
         """
-        variables = [
-            Variable(
+        handler: type[DelayedArray | Array]
+        handler = DelayedArray if delayed else Array
+        variables: list[Variable] = [
+            handler(
                 name,  # type: ignore[arg-type]
                 array.data,  # type: ignore[arg-type]
                 tuple(array.dims),  # type: ignore[arg-type]
-                tuple(
+                attrs=tuple(
                     Attribute(*attr)  # type: ignore[arg-type]
                     for attr in array.attrs.items()),
-                array.encoding.get('compressor', None),
-                array.encoding.get('_FillValue', None),
-                array.encoding.get('filters', None))
-            for name, array in ds.variables.items()
+                compressor=array.encoding.get('compressor', None),
+                fill_value=array.encoding.get('_FillValue', None),
+                filters=array.encoding.get('filters', None))
+            for name, array in zds.variables.items()
         ]
 
         return Dataset(
             variables=variables,
             attrs=tuple(
                 Attribute(*item)  # type: ignore[arg-type]
-                for item in ds.attrs.items()))
+                for item in zds.attrs.items()),
+            delayed=delayed,
+        )
 
     def to_xarray(self, **kwargs) -> xarray.Dataset:
         """Convert the dataset to a xarray dataset.
 
         Args:
             **kwargs: Additional parameters are passed through the function
                 :py:func:`xarray.conventions.decode_cf_variables`.
@@ -337,154 +452,168 @@
         """
         data_vars = collections.OrderedDict(
             (name, var.to_xarray()) for name, var in self.variables.items())
         attrs = collections.OrderedDict(
             (item.name, item.value) for item in self.attrs)
         data_vars, attrs, coord_names = xarray.conventions.decode_cf_variables(
             data_vars, attrs, **kwargs)
-        ds = xarray.Dataset(data_vars, attrs=attrs)
-        ds = ds.set_coords(coord_names.intersection(data_vars))
-        return ds
-
-    def to_dict(self,
-                variables: Sequence[str] | None = None,
-                **kwargs) -> dict[str, NDArray | NDMaskedArray]:
+        result = xarray.Dataset(data_vars, attrs=attrs)
+        return result.set_coords(coord_names.intersection(data_vars))
+
+    def to_dict(
+        self,
+        variables: Sequence[str] | None = None,
+        **kwargs,
+    ) -> dict[str, NDArray | NDMaskedArray]:
         """Convert the dataset to a dictionary, between the variable names and
         their data.
 
         Args:
             variables: Variables to include (default to all dataset's
                 variables).
             **kwargs: Additional parameters are passed through the function
                 :py:func:`dask.compute`.
 
         Returns:
             Dictionary of variables.
         """
         variables = variables or tuple(self.variables.keys())
-        arrays = tuple((key, value.data)
-                       for key, value in self.variables.items()
-                       if key in variables)
-        return dict(dask.base.compute(*arrays, **kwargs))
+        if self.delayed:
+            arrays = tuple((key, value.data)
+                           for key, value in self.variables.items()
+                           if key in variables)
+            return dict(dask.base.compute(*arrays, **kwargs))
+        return dict(
+            tuple((key, value.values) for key, value in self.variables.items()
+                  if key in variables))
 
-    def set_for_insertion(self, ds: meta.Dataset) -> Dataset:
+    def set_for_insertion(self, mds: meta.Dataset) -> Dataset:
         """Create a new dataset ready to be inserted into a collection.
 
         Args:
-            ds: Dataset metadata.
+            mds: Dataset metadata.
 
         Returns:
             New dataset.
         """
         return Dataset(
             variables=[
                 var.set_for_insertion() for var in self.variables.values()
             ],
-            chunks=ds.chunks,
-            block_size_limit=ds.block_size_limit,
+            chunks=mds.chunks,
+            block_size_limit=mds.block_size_limit,
         )
 
-    def fill_attrs(self, ds: meta.Dataset):
+    def fill_attrs(self, mds: meta.Dataset) -> None:
         """Fill the dataset and its variables attributes using the provided
         metadata.
 
         Args:
-            ds: Dataset metadata.
+            mds: Dataset metadata.
         """
-        self.attrs = tuple(ds.attrs)
-        _ = [
-            var.fill_attrs(ds.variables[name])
-            for name, var in self.variables.items()
-        ]
+        self.attrs = tuple(mds.attrs)
+        tuple(
+            map(lambda var: var.fill_attrs(mds.variables[var.name]),
+                self.variables.values()))
 
     def isel(self, slices: dict[str, Any]) -> Dataset:
         """Return a new dataset with each array indexed along the specified
         slices.
 
         Args:
             slices: Dictionary of dimension names and slices
 
         Returns:
             New dataset.
         """
-        dims_invalid = set(slices) - set(self.dimensions)
+        dims_invalid: set[str] = set(slices) - set(self.dimensions)
         if dims_invalid:
             raise ValueError(
                 f'Slices contain invalid dimension name(s): {dims_invalid}')
-        default = slice(None)
-        variables = [
-            var.isel(tuple(slices.get(dim, default) for dim in var.dimensions))
+        variables: list[Variable] = [
+            var.isel(
+                tuple(slices.get(dim, slice(None)) for dim in var.dimensions))
             for var in self.variables.values()
         ]
         return Dataset(variables=variables,
                        attrs=self.attrs,
+                       block_size_limit=self.block_size_limit,
                        chunks=self.dims_chunk,
-                       block_size_limit=self.block_size_limit)
+                       delayed=self.delayed)
 
     def delete(self, indexer: slice | Sequence[int], axis: str) -> Dataset:
         """Return a new dataset without the data selected by the provided
         indices.
 
         Args:
             indexer: Indices to remove along the specified axis.
             axis: The axis along which to delete the subarrays defined
                 in the dataset.
 
         Returns:
             New dataset.
         """
-        variables = [
-            _duplicate(
-                var,
-                dask.array.routines.delete(var.array, indexer,
-                                           var.dimensions.index(axis)))
-            for var in self.variables.values()
-        ]
+        variables: list[Variable] = _delete_delayed_vars(
+            self, indexer, axis) if self.delayed else _delete_vars(
+                self, indexer, axis)
         return Dataset(variables=variables,
                        attrs=self.attrs,
+                       block_size_limit=self.block_size_limit,
                        chunks=self.dims_chunk,
-                       block_size_limit=self.block_size_limit)
+                       delayed=self.delayed)
 
     def compute(self, **kwargs) -> Dataset:
         """Compute the dataset variables.
 
         Args:
             **kwargs: Additional parameters are passed through to
                 :py:func:`dask.array.compute`.
 
         Returns:
             New dataset.
         """
-        arrays = tuple(item.array for item in self.variables.values())
-        arrays = dask.base.compute(*arrays, **kwargs)
+        if not self.delayed:
+            return self
+
+        arrays: Iterable[NDArray] = dask.base.compute(
+            *tuple(item.array for item in self.variables.values()), **kwargs)
 
-        # Don't use _duplicate here because we want to transform
-        # the numpy arrays computed by dask into dask arrays
-        variables = [
-            self.variables[k].duplicate(array)
-            for k, array in zip(self.variables, arrays)
+        variables: list[Variable] = [
+            Array(item.name,
+                  array,
+                  item.dimensions,
+                  attrs=item.attrs,
+                  compressor=item.compressor,
+                  fill_value=item.fill_value,
+                  filters=item.filters)
+            for item, array in zip(self.variables.values(), arrays)
         ]
         return Dataset(variables=variables,
                        attrs=self.attrs,
                        chunks=self.dims_chunk,
-                       block_size_limit=self.block_size_limit)
+                       block_size_limit=self.block_size_limit,
+                       delayed=False)
 
     def rechunk(self, **kwargs) -> Dataset:
         """Rechunk the dataset.
 
         Args:
             **kwargs: Keyword arguments are passed through to
                 :py:func:`dask.array.rechunk.rechunk`.
 
         Returns:
             New dataset.
 
         .. seealso:: :py:func:`dask.array.rechunk`
         """
-        variables = [var.rechunk(**kwargs) for var in self.variables.values()]
+        if not self.delayed:
+            return self
+        variables: list[Variable] = [
+            var.rechunk(**kwargs) for var in self.variables.values()
+        ]
         return Dataset(variables=variables,
                        attrs=self.attrs,
                        chunks=self.dims_chunk,
                        block_size_limit=self.block_size_limit)
 
     def persist(
         self,
@@ -498,21 +627,23 @@
             compress: If true, compress the data loaded into memory.
             **kwargs: Additional parameters are passed to the function
                 :py:func:`dask.array.Array.persist`.
 
         Returns:
             The dataset with the variables persisted into memory.
         """
+        if not self.delayed:
+            return self
         if compress:
             for var in self.variables.values():
                 var.array = var.array.map_blocks(CompressedArray,
                                                  fill_value=var.fill_value)
-        arrays = dask.base.persist(
+        arrays: Iterable[NDArray] = dask.base.persist(
             *tuple(item.data for item in self.variables.values()), **kwargs)
-        variables = self.variables
+        variables: OrderedDict[str, Variable] = self.variables
         for name, array in zip(self.variables, arrays):
             variables[name].array = array
 
         return self
 
     def concat(self, other: Dataset | Iterable[Dataset], dim: str) -> Dataset:
         """Concatenate datasets along a dimension.
@@ -525,41 +656,48 @@
             New dataset.
 
         Raises:
             ValueError: If the provided sequence of datasets is empty.
         """
         if not isinstance(other, Iterable):
             other = [other]
+        other = tuple(other)
         if not other:
             raise ValueError('cannot concatenate an empty sequence')
-        variables = [
+        if not all(item.delayed == self.delayed for item in other):
+            raise ValueError('cannot concatenate delayed and non-delayed data')
+        variables: list[Variable] = [
             var.concat(tuple(item.variables[name] for item in other), dim)
             for name, var in self.variables.items()
         ]
         return Dataset(variables=variables,
                        attrs=self.attrs,
+                       block_size_limit=self.block_size_limit,
                        chunks=self.dims_chunk,
-                       block_size_limit=self.block_size_limit)
+                       delayed=self.delayed)
 
     def merge(self, other: Dataset) -> None:
         """Merge the provided dataset into this dataset.
 
         Args:
             other: Dataset to merge into this dataset.
         """
+        if self.delayed != other.delayed:
+            raise ValueError('cannot merge delayed and non-delayed data')
+
         # Merge the variables
         for name, var in other.variables.items():
 
             # It's impossible to merge a variable with itself.
             if name in self.variables:
                 raise ValueError(f'variable {name} already exists')
             self.variables[name] = var
 
         # If the dataset has common dimensions, they must be identical.
-        same_dims = set(self.dimensions) & set(other.dimensions)
+        same_dims: set[str] = set(self.dimensions) & set(other.dimensions)
         if same_dims and not all(self.dimensions[dim] == other.dimensions[dim]
                                  for dim in same_dims):
             raise ValueError(f'dimensions {same_dims} are not identical')
 
         # Merge the dimensions.
         self.dimensions.update(other.dimensions)
 
@@ -583,65 +721,94 @@
             predicate: If true, select variables with the specified dimensions,
                 otherwise select variables without the specified dimensions.
 
         Returns:
             New dataset or None if no variables match the predicate.
         """
 
-        def _predicate_for_dimension_less(var: variable.Variable) -> bool:
+        def _predicate_for_dimension_less(var: Variable) -> bool:
             """Return true if the variable is selected by the predicate."""
             return (len(var.dimensions) == 0) == predicate
 
-        def _predicate_for_dimension(var: variable.Variable) -> bool:
+        def _predicate_for_dimension(var: Variable) -> bool:
             """Return true if the variable is selected by the predicate."""
             return bool(set(var.dimensions) & set_of_dims) == predicate
 
+        condition: Callable[..., bool]
         condition = (_predicate_for_dimension_less
                      if not dims else _predicate_for_dimension)
 
         set_of_dims = set(dims)
-        variables = [var for var in self.variables.values() if condition(var)]
+        variables: list[Variable] = [
+            var for var in self.variables.values() if condition(var)
+        ]
         return Dataset(variables=variables,
                        attrs=self.attrs,
                        chunks=self.dims_chunk,
                        block_size_limit=self.block_size_limit)
 
-    def to_zarr(self,
-                path: str,
-                fs: fsspec.AbstractFileSystem | None = None,
-                parallel: bool = True) -> None:
-        """Write the dataset to a Zarr store.
-
-        Args:
-            path: Path to the Zarr store.
-            fs: Filesystem to use.
-            parallel: If true, write the data in parallel.
-        """
-        # pylint: disable=import-outside-toplevel, import-error
-        # Avoid circular import
-        import storage
-        import sync
-
-        # pylint: enable=import-outside-toplevel, import-error
-        storage.write_zarr_group(self, path, fs or fsspec.filesystem('file'),
-                                 sync.NoSync(), parallel)
+    # def to_zarr(self,
+    #             path: str,
+    #             fs: fsspec.AbstractFileSystem | None = None,
+    #             parallel: bool = True) -> None:
+    #     """Write the dataset to a Zarr store.
+
+    #     Args:
+    #         path: Path to the Zarr store.
+    #         fs: Filesystem to use.
+    #         parallel: If true, write the data in parallel.
+    #     """
+    #     if not self.delayed:
+    #         raise ValueError('cannot write a non-delayed dataset to Zarr')
+    #     # pylint: disable=import-outside-toplevel, import-error
+    #     # Avoid circular import
+    #     import storage
+    #     import sync
+
+    #     # pylint: enable=import-outside-toplevel, import-error
+    #     storage.write_zarr_group(self, path, fs or fsspec.filesystem('file'),
+    #                              sync.NoSync(), parallel)
 
     def __str__(self) -> str:
         return _dataset_repr(self)
 
     def __repr__(self) -> str:
         return _dataset_repr(self)
 
 
-def get_variable_metadata(
-        var: variable.Variable | meta.Variable) -> meta.Variable:
+def get_variable_metadata(var: Variable | meta.Variable) -> meta.Variable:
     """Get the variable metadata.
 
     Args:
         var: Variable to get the metadata for.
 
     Returns:
         Variable metadata.
     """
     if isinstance(var, Variable):
         return var.metadata()
     return var
+
+
+def get_dataset_variable_properties(
+        metadata: meta.Dataset,
+        selected_variables: Iterable[str] | None = None) -> tuple[Array, ...]:
+    """Return the variables properties defined in the dataset.
+
+    Args:
+        metadata: Metadata dataset containing variables information.
+        selected_variables: The variables to return. If None, all the
+            variables are returned.
+
+    Returns:
+        The variables defined in the dataset.
+    """
+    selected_variables = selected_variables or metadata.variables.keys()
+    return tuple(
+        Array(v.name,
+              numpy.ndarray((0, ) * len(v.dimensions), v.dtype),
+              v.dimensions,
+              attrs=v.attrs,
+              compressor=v.compressor,
+              fill_value=v.fill_value,
+              filters=v.filters) for k, v in metadata.variables.items()
+        if k in selected_variables)
```

### Comparing `zcollection-2023.3.2/zcollection/expression.py` & `zcollection-2023.5.0/zcollection/expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,43 +7,43 @@
 ===========================================
 """
 from __future__ import annotations
 
 from typing import Any, ClassVar
 import ast
 import dataclasses
+import types
 
 
 @dataclasses.dataclass
 class Expression:
     """Partitioning expressions.
 
     Args:
         expression: The expression to be evaluated
-
     Raises:
         NameError: If a variable is not defined.
-
     Example:
         >>> expr = Expression("year==2000 and month==1 and day in range(1, 12)")
     """
-    __slots__ = ('code', )
-
     #: Compiled expression to be evaluated
-    code: Any
+    code: types.CodeType
+
+    #: Known data members
+    __slots__: tuple[str, ...] = ('code', )
 
     #: The builtins that are allowed in the expression.
     BUILTINS: ClassVar[dict[str, Any]] = {'range': range}
 
     def __init__(self, expression: str) -> None:
         self.code = compile(ast.parse(expression, mode='eval'), ' ', 'eval')
 
     def __call__(self, variables: dict[str, Any]) -> Any:
         try:
-            __locals = {
+            __locals: dict[str, Any] = {
                 name: variables[name]
                 for name in self.code.co_names if name not in self.BUILTINS
             }
             # pylint: disable=eval-used
             # The eval function is used here to evaluate a simple expression.
             # The only builtin functions allowed is the range function.
             return eval(self.code, {'__builtins__': self.BUILTINS}, __locals)
```

### Comparing `zcollection-2023.3.2/zcollection/fs_utils.py` & `zcollection-2023.5.0/zcollection/fs_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # BSD-style license that can be found in the LICENSE file.
 """
 File system tools
 =================
 """
 from __future__ import annotations
 
-from typing import Iterator, Sequence
+from typing import Any, Iterator, Sequence
 import os
 
 import fsspec
 
 #: Path separator
 SEPARATOR = '/'
 
@@ -76,40 +76,43 @@
         path: path to the directory
         sort: if True, the list of files and directories is sorted
             alphabetically
 
     Returns:
         Iterator of (path, directories, files).
     """
+    dirs: list[str]
+    files: list[str]
+
     dirs, files = [], []
     try:
-        listing = fs.ls(path, detail=True)
+        listing: list[dict[str, Any]] = fs.ls(path, detail=True)
     except (FileNotFoundError, OSError):
         yield '', [], []
         return
 
     for info in listing:
         # each info name must be at least [path]/part , but here
         # we check also for names like [path]/part/
-        pathname = info['name'].rstrip(SEPARATOR)
-        name = pathname.rsplit(SEPARATOR, 1)[-1]
+        pathname: str = info['name'].rstrip(SEPARATOR)
+        name: str = pathname.rsplit(SEPARATOR, 1)[-1]
         if info['type'] == 'directory' and pathname != path:
             # do not include "self" path
             dirs.append(pathname)
         else:
             files.append(name)
 
-    def sort_sequence(sequence):
+    def sort_sequence(sequence: list[str]) -> list[str]:
         """Sort the sequence if the user wishes."""
-        return sorted(sequence) if sort else sequence
+        return list(sorted(sequence)) if sort else sequence
 
     dirs = sort_sequence(dirs)
     yield path.rstrip(SEPARATOR), dirs, sort_sequence(files)
 
-    for item in sort_sequence(dirs):
+    for item in dirs:
         yield from fs_walk(fs, item, sort=sort)
 
 
 def copy_file(
     source: str,
     target: str,
     fs_source: fsspec.AbstractFileSystem,
@@ -121,15 +124,15 @@
         source: The name of the source file.
         target: The name of the target file.
         fs_source: The file system that the source file is stored on.
         fs_target: The file system that the target file is stored on.
     """
     with fs_source.open(source, 'rb') as source_stream:
         with fs_target.open(target, 'wb') as target_stream:
-            target_stream.write(source_stream.read())
+            target_stream.write(source_stream.read())  # type: ignore[arg-type]
 
 
 def copy_files(
     source: Sequence[str],
     target: str,
     fs_source: fsspec.AbstractFileSystem,
     fs_target: fsspec.AbstractFileSystem,
@@ -167,14 +170,14 @@
         ValueError: If the target already exists.
     """
     if fs_target.exists(target):
         raise ValueError(f'Target {target} already exists')
     fs_target.mkdir(target)
     for root, dirs, files in tuple(fs_walk(fs_source, source)):
         for name in files:
-            source_path = join_path(root, name)
+            source_path: str = join_path(root, name)
             copy_file(source_path,
                       join_path(target, os.path.relpath(source_path, source)),
                       fs_source, fs_target)
         for source_path in dirs:
             fs_target.mkdir(
                 join_path(target, os.path.relpath(source_path, source)))
```

### Comparing `zcollection-2023.3.2/zcollection/indexing/abc.py` & `zcollection-2023.5.0/zcollection/indexing/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import fsspec
 import numpy
 import pyarrow
 import pyarrow.parquet
 
 from .. import collection, dataset
+from ..collection.callable_objects import MapCallable
 from ..type_hints import NDArray
 
 #: Scalar data type for the index.
 Scalar = Union[int, float, bytes]
 
 #: Index data type.
 DType = Union[Scalar, Iterable[Scalar]]
@@ -41,37 +42,37 @@
     stored in the index. The function is called for each partition of
     the collection to determine the first and last index of the
     partition that contains the value to be indexed.
     """
 
     def __call__(
         self,
-        ds: dataset.Dataset,
+        zds: dataset.Dataset,
         *args,
         **kwargs,
     ) -> NDArray:
         """Indexing the partition of the collection.
 
         Args:
-            ds: Dataset to be indexed.
+            zds: Dataset to be indexed.
             *args: Positional arguments.
             **kwargs: Keyword arguments.
 
         Returns:
             A numpy structured array to be converted to a DataFrame and stored
             in the index.
         """
         # pylint: disable=unnecessary-ellipsis
         # Ellipsis is necessary to make the function signature match the
         # protocol.
         ...  # pragma: no cover
         # pylint: enable=unnecessary-ellipsis
 
 
-class Indexer:
+class Indexer(abc.ABC):
     """Abstract base class for indexing a collection.
 
     This class defines the interface for indexing a collection.
 
     Args:
         path: The path to the index.
         filesystem: The filesystem to use.
@@ -87,17 +88,18 @@
         path: pathlib.Path | str,
         *,
         filesystem: fsspec.AbstractFileSystem | None = None,
     ) -> None:
         if isinstance(path, pathlib.Path):
             path = str(path)
         #: Path to the index.
-        self._path = path
+        self._path: str = path
         #: Filesystem to use.
-        self._fs = filesystem or fsspec.filesystem('file')
+        self._fs: fsspec.AbstractFileSystem = \
+            filesystem or fsspec.filesystem('file')
         #: Metadata to attach to the index.
         self._meta: dict[str, bytes] = {}
         #: Partitioning keys of the indexed collection.
         self._partition_keys: tuple[str, ...] = ()
         #: PyArrow table containing the index.
         self._table: pyarrow.Table | None = None
         #: Type for each columns of the index.
@@ -134,20 +136,20 @@
         Args:
             **kwargs: Additional arguments to pass to the function.
 
         Returns:
             The PyArrow type.
         """
         dtype = dict(cls.dtype(**kwargs))
-        binary = {}
+        binary: dict[str, pyarrow.DataType] = {}
         for name, value in tuple(dtype.items()):
             if value.startswith('S'):
                 binary[name] = pyarrow.binary(int(value[1:]))
                 del dtype[name]
-        result = {
+        result: dict[str, pyarrow.DataType] = {
             name: getattr(pyarrow, value)()
             for name, value in dtype.items()
         }
         result.update(binary)
         return result
 
     def _set_schema(
@@ -157,66 +159,66 @@
     ) -> None:
         """Set the schema properties of the index.
 
         Args:
             partition_schema: A tuple of (name, type) pairs that describes the
                 storage properties of the collection's partitioning keys.
         """
-        dtype = self.pyarrow_type(**kwargs)
+        dtype: dict[str, pyarrow.DataType] = self.pyarrow_type(**kwargs)
         self._partition_keys = tuple(item[0] for item in partition_schema)
         self._type = {name: dtype[name] for name, _ in self.dtype()}
         self._type.update({item[0]: item[1] for item in partition_schema})
 
     def _sort_keys(self) -> list[tuple[str, str]]:
         """Return the list of keys to sort the index by."""
-        keys = self._partition_keys + (self.START, self.STOP)
+        keys: tuple[str, ...] = self._partition_keys + (self.START, self.STOP)
         return [(key, 'ascending') for key in keys]
 
     @classmethod
     def _create(
         cls,
         path: pathlib.Path | str,
-        ds: collection.Collection,
+        zds: collection.Collection,
         meta: dict[str, bytes] | None = None,
         filesystem: fsspec.AbstractFileSystem | None = None,
         **kwargs,
     ) -> Indexer:
         """Create a new index.
 
         Args:
             path: The path to the index.
-            ds: The collection to index.
+            zds: The collection to index.
             meta: Metadata to attach to the index.
             filesystem: The filesystem to use.
 
         Returns:
             The created index.
         """
         partition_schema = tuple((name, getattr(pyarrow, value)())
-                                 for name, value in ds.partitioning.dtype())
-        self = cls(path, filesystem=filesystem)
+                                 for name, value in zds.partitioning.dtype())
+        self: Indexer = cls(path, filesystem=filesystem)
         self._meta = meta or {}
         self._set_schema(partition_schema, **kwargs)
         return self
 
     @classmethod
     @abc.abstractmethod
     def create(
         cls,
         path: pathlib.Path | str,
-        ds: collection.Collection,
+        zds: collection.Collection,
         *,
         filesystem: fsspec.AbstractFileSystem | None = None,
         **kwargs,
     ) -> Indexer:
         """Create a new index.
 
         Args:
             path: The path to the index.
-            ds: The collection to index.
+            zds: The collection to index.
             filesystem: The filesystem to use.
 
         Returns:
             The created index.
         """
 
     @classmethod
@@ -231,49 +233,49 @@
         Args:
             path: The path to the index.
             filesystem: The filesystem to use.
 
         Returns:
             The index.
         """
-        self = cls(path, filesystem=filesystem)
+        self: Indexer = cls(path, filesystem=filesystem)
         with self._fs.open(path, 'rb') as stream:
-            schema = pyarrow.parquet.read_schema(stream)
+            schema: pyarrow.Schema = pyarrow.parquet.read_schema(stream)
         columns = tuple(name for name, _ in self.dtype())
         self._partition_keys = tuple(name for name in schema.names
                                      if name not in columns)
         self._type = {name: schema.field(name).type for name in schema.names}
         self._meta = {
             name.decode(): value
             for name, value in schema.metadata.items()
         } if schema.metadata is not None else {}
         return self
 
     def _update(
         self,
-        ds: collection.Collection,
-        func: IndexingCallable,
+        zcollection: collection.Collection,
+        func: MapCallable,
         partition_size: int | None = None,
         npartitions: int | None = None,
         **kwargs,
     ) -> None:
         """Update the index.
 
         Args:
-            ds: The dataset containing the new data.
+            zcollection: The collection to index.
             func: The function to use to calculate the index.
             partition_size: The length of each bag partition.
             npartitions: The number of desired bag partitions.
             **kwargs: Additional arguments to pass to the function.
         """
         tables: list[pyarrow.Table] = []
-        bag = ds.map(func,
-                     partition_size=partition_size,
-                     npartitions=npartitions,
-                     **kwargs)
+        bag = zcollection.map(func,
+                              partition_size=partition_size,
+                              npartitions=npartitions,
+                              **kwargs)
         # List of new partitions indexed.
         partitions = []
         for partition, data in bag.compute():
             length = data.size
             # If the current item is empty, skip it.
             if length == 0:
                 continue
@@ -330,36 +332,36 @@
             table = table.replace_schema_metadata(self._meta)
         pyarrow.parquet.write_table(table, self._path, filesystem=self._fs)
         self._table = table
 
     @abc.abstractmethod
     def update(
         self,
-        ds: collection.Collection,
+        zds: collection.Collection,
         *,
         partition_size: int | None = None,
         npartitions: int | None = None,
     ) -> None:
         """Update the index.
 
         Args:
-            ds: The dataset containing the new data.
+            zds: The dataset containing the new data.
             partition_size: The length of each bag partition.
             npartitions: The number of desired bag partitions.
         """
 
     def _read(self) -> pyarrow.Table:
         """Read the index."""
         if self._table is None:
             self._table = pyarrow.parquet.read_table(self._path,
                                                      filesystem=self._fs)
         return self._table
 
     def _table_2_indexer(self, table: pyarrow.Table,
-                         only_partition_keys: bool) -> collection.Indexer:
+                         only_partition_keys: bool) -> collection.abc.Indexer:
         """Convert a table to an indexer.
 
         Args:
             table: The table to convert.
             only_partition_keys: If True, only the partition keys are kept.
 
         Returns:
@@ -407,15 +409,15 @@
     def query(
         self,
         columns: QueryDict,
         *,
         logical_op: str | None = None,
         mask: pyarrow.ChunkedArray | None = None,
         only_partition_keys: bool = True,
-    ) -> collection.Indexer:
+    ) -> collection.abc.Indexer:
         """Query the index.
 
         Args:
             columns: Dictionary of columns to query.
             logical_op: The logical operator to use. Can be "and", "and_not",
                 "invert", "or", "xor". Defaults to "and".
             mask: An optional mask to apply to the table before querying.
```

### Comparing `zcollection-2023.3.2/zcollection/indexing/tests/test_abc.py` & `zcollection-2023.5.0/zcollection/indexing/tests/test_abc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2023 CNES
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """Test the base class for indexing."""
 from __future__ import annotations
 
-from typing import Iterator, List, Optional, Tuple, Union
+from typing import Iterator
 import pathlib
 
 import fsspec
 import numpy
 import pyarrow
 import pytest
 
@@ -48,30 +48,30 @@
     yield from tuple(zip(half_orbit[:-1], half_orbit[1:]))
 
 
 # pylint: disable=unused-argument,invalid-name
 # The signature of the function must follow the signature of
 # zcollection.PartitionCallable
 def _half_orbit(
-    ds: dataset.Dataset,
+    zds: dataset.Dataset,
     *args,
     **kwargs,
 ) -> NDArray:
     """Return the indexes of the start and stop of each half-orbit.
 
     Args:
-        ds: Datasets stored in a partition to be indexed.
+        zds: Datasets stored in a partition to be indexed.
 
     Returns:
         Dictionary of start and stop indexes for each half-orbit.
     """
     pass_number_varname = kwargs.pop('pass_number', 'pass_number')
     cycle_number_varname = kwargs.pop('cycle_number', 'cycle_number')
-    pass_number = ds.variables[pass_number_varname].values
-    cycle_number = ds.variables[cycle_number_varname].values
+    pass_number = zds.variables[pass_number_varname].values
+    cycle_number = zds.variables[cycle_number_varname].values
 
     generator = ((
         i0,
         i1,
         cycle_number[i0],
         pass_number[i0],
     ) for i0, i1 in split_half_orbit(cycle_number, pass_number))
@@ -100,54 +100,55 @@
             (cls.PASS_NUMBER, 'uint16'),
         ]
 
     @classmethod
     def create(
         cls,
         path: pathlib.Path | str,
-        ds: collection.Collection,
+        zds: collection.Collection,
         *,
         filesystem: fsspec.AbstractFileSystem | None = None,
         **kwargs,
     ) -> HalfOrbitIndexer:
         """Create a new index.
 
         Args:
             path: The path to the index.
-            ds: The collection to be indexed.
+            zds: The collection to be indexed.
             filesystem: The filesystem to use.
 
         Returns:
             The created index.
         """
         return super()._create(path,
-                               ds,
-                               meta=dict(attribute=b'value'),
+                               zds,
+                               meta={'attribute': b'value'},
                                filesystem=filesystem)  # type: ignore
 
     def update(
         self,
-        ds: collection.Collection,
+        zds: collection.Collection,
         *,
         partition_size: int | None = None,
         npartitions: int | None = None,
         **kwargs,
     ) -> None:
         """Update the index.
 
         Args:
-            ds: New data stored in the collection to be indexed.
+            zds: New data stored in the collection to be indexed.
             partition_size: The length of each bag partition.
             npartitions: The number of desired bag partitions.
             cycle_number: The name of the cycle number variable stored in the
                 collection. Defaults to "cycle_number".
             pass_number: The name of the pass number variable stored in the
                 collection. Defaults to "pass_number".
         """
-        super()._update(ds, _half_orbit, partition_size, npartitions, **kwargs)
+        super()._update(zds, _half_orbit, partition_size, npartitions,
+                        **kwargs)
 
 
 def test_indexer(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
         local_fs,  # pylint: disable=redefined-outer-name
 ):
     """Test the base class of the indexer."""
@@ -172,62 +173,68 @@
 
     assert indexer.dtype() == [('start', 'int64'), ('stop', 'int64'),
                                ('cycle_number', 'uint16'),
                                ('pass_number', 'uint16')]
     indexer.update(zcollection)
     assert isinstance(indexer.table, pyarrow.Table)
 
-    selection = zcollection.load(indexer=indexer.query(dict(cycle_number=2)))
+    selection = zcollection.load(indexer=indexer.query({'cycle_number': 2}))
     assert selection is not None
     assert set(selection.variables['cycle_number'].values) == {2}
 
     with pytest.raises(ValueError):
-        indexer.query(dict(cycle_number=3), logical_op='X')
+        indexer.query({'cycle_number': 3}, logical_op='X')
 
     with pytest.raises(ValueError):
-        indexer.query(dict(X=3))
+        indexer.query({'X': 3})
 
     # Updating the index should not change the indexer.
     indexer.update(zcollection)
-    other = zcollection.load(indexer=indexer.query(dict(cycle_number=2)))
+    other = zcollection.load(indexer=indexer.query({'cycle_number': 2}))
     assert other is not None
     assert numpy.all(
         other['observation'].values == selection['observation'].values)
 
     selection = zcollection.load(
-        indexer=indexer.query(dict(cycle_number=[2, 4])))
+        indexer=indexer.query({'cycle_number': [2, 4]}))
     assert selection is not None
     assert set(selection.variables['cycle_number'].values) == {2, 4}
 
-    selection = zcollection.load(
-        indexer=indexer.query(dict(cycle_number=[2, 4], pass_number=1)))
+    selection = zcollection.load(indexer=indexer.query({
+        'cycle_number': [2, 4],
+        'pass_number': 1
+    }))
     assert selection is not None
     assert set(selection.variables['cycle_number'].values) == {2, 4}
     assert set(selection.variables['pass_number'].values) == {1}
 
-    selection = zcollection.load(
-        indexer=indexer.query(dict(cycle_number=[2, 4], pass_number=[1, 5])))
+    selection = zcollection.load(indexer=indexer.query({
+        'cycle_number': [2, 4],
+        'pass_number': [1, 5]
+    }))
     assert selection is not None
     assert set(selection.variables['cycle_number'].values) == {2, 4}
     assert set(selection.variables['pass_number'].values) == {1, 5}
 
     indexer = HalfOrbitIndexer.open(str(
         local_fs.collection.joinpath('index.parquet')),
                                     filesystem=local_fs.fs)
-    assert indexer.meta == dict(attribute=b'value')
-    selection = zcollection.load(
-        indexer=indexer.query(dict(cycle_number=[2, 4], pass_number=[1, 5])))
+    assert indexer.meta == {'attribute': b'value'}
+    selection = zcollection.load(indexer=indexer.query({
+        'cycle_number': [2, 4],
+        'pass_number': [1, 5]
+    }))
     assert selection is not None
     assert set(selection.variables['cycle_number'].values) == {2, 4}
     assert set(selection.variables['pass_number'].values) == {1, 5}
 
     indices = tuple(
-        indexer.query(dict(cycle_number=[2, 4]), only_partition_keys=False))
+        indexer.query({'cycle_number': [2, 4]}, only_partition_keys=False))
     assert tuple(item[0] for item in indices[0][0]) == (
         'cycle_number',
         'pass_number',
         'year',
         'month',
     )
 
-    indexer = abc.Indexer('', filesystem=fsspec.filesystem('memory'))
-    assert indexer.query(dict(cycle_number=[2, 4])) == tuple()
+    indexer = HalfOrbitIndexer('', filesystem=fsspec.filesystem('memory'))
+    assert indexer.query({'cycle_number': [2, 4]}) == tuple()
```

### Comparing `zcollection-2023.3.2/zcollection/merging/__init__.py` & `zcollection-2023.5.0/zcollection/merging/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from __future__ import annotations
 
 from typing import Protocol
 import random
 import shutil
 
 import fsspec
+import fsspec.implementations.local
 import zarr.storage
 
 from .. import dataset, storage, sync
 from .time_series import merge_time_series
 
-__all__ = ['MergeCallable', 'perform', 'merge_time_series']
+__all__ = ('MergeCallable', 'perform', 'merge_time_series')
 
 #: Character set used to create a temporary directory.
 CHARACTERS = 'abcdefghijklmnopqrstuvwxyz0123456789_'
 
 
 #: pylint: disable=too-few-public-methods,duplicate-code
 class MergeCallable(Protocol):
@@ -60,15 +61,15 @@
     #: pylint: enable=too-few-public-methods,duplicate-code
 
 
 def _rename(
     fs: fsspec.AbstractFileSystem,
     source: str,
     dest: str,
-):
+) -> None:
     """Rename a directory on a file system.
 
     Args:
         fs: The file system.
         source: The source directory.
         dest: The destination directory.
     """
@@ -83,37 +84,38 @@
 
     fs.rm(dest, recursive=True)
     fs.mv(source, dest, recursive=True)
 
 
 def _update_fs(
     dirname: str,
-    ds: dataset.Dataset,
+    zds: dataset.Dataset,
     fs: fsspec.AbstractFileSystem,
+    *,
     synchronizer: sync.Sync | None = None,
 ) -> None:
     """Updates a dataset stored in a partition.
 
     Args:
         dirname: The name of the partition.
-        ds: The dataset to update.
+        zds: The dataset to update.
         fs: The file system that the partition is stored on.
         synchronizer: The instance handling access to critical resources.
     """
     # Name of the temporary directory.
-    temp = dirname + '.' + ''.join(
+    temp: str = dirname + '.' + ''.join(
         random.choice(CHARACTERS) for _ in range(10))
 
     # Initializing Zarr group
     zarr.storage.init_group(store=fs.get_mapper(temp))
 
     # Writing new data.
     try:
         # The synchronization is done by the caller.
-        storage.write_zarr_group(ds, temp, fs, synchronizer or sync.NoSync())
+        storage.write_zarr_group(zds, temp, fs, synchronizer or sync.NoSync())
     except Exception:
         # The "write_zarr_group" method throws the exception if all scheduled
         # tasks are finished. So here we can delete the temporary directory.
         fs.rm(temp, recursive=True)
         raise
 
     # Rename the existing entry on the file system
@@ -122,26 +124,32 @@
 
 def perform(
     ds_inserted: dataset.Dataset,
     dirname: str,
     axis: str,
     fs: fsspec.AbstractFileSystem,
     partitioning_dim: str,
+    *,
+    delayed: bool = True,
     merge_callable: MergeCallable | None,
     synchronizer: sync.Sync | None = None,
 ) -> None:
-    """Performs the merge between a new dataset and an existing partition.
+    """Merges a new dataset with an existing partition.
 
     Args:
         ds_inserted: The dataset to merge.
         dirname: The name of the partition.
         axis: The axis to merge on.
-        fs: The file system on which the partition is stored on.
+        fs: The file system on which the partition is stored.
         partitioning_dim: The partitioning dimension.
+        delayed: If True, the existing dataset is loaded lazily. Defaults to
+            True.
         merge_callable: The merge callable. If None, the inserted dataset
             overwrites the existing dataset stored in the partition.
+            Defaults to None.
         synchronizer: The instance handling access to critical resources.
+            Defaults to None.
     """
-    ds = merge_callable(
-        storage.open_zarr_group(dirname, fs), ds_inserted, axis,
-        partitioning_dim) if merge_callable is not None else ds_inserted
-    _update_fs(dirname, ds, fs, synchronizer)
+    zds: dataset.Dataset = merge_callable(
+        storage.open_zarr_group(dirname, fs, delayed=delayed), ds_inserted,
+        axis, partitioning_dim) if merge_callable is not None else ds_inserted
+    _update_fs(dirname, zds, fs, synchronizer=synchronizer)
```

### Comparing `zcollection-2023.3.2/zcollection/merging/period.py` & `zcollection-2023.5.0/zcollection/merging/period.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 # BSD-style license that can be found in the LICENSE file.
 """
 Time period
 ===========
 """
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, Callable, Match
 import enum
 import re
 
 import numpy
 
 from ..type_hints import DType
 
 # Parse the unit of numpy.timedelta64.
-PATTERN = re.compile(r'(?:datetime|timedelta)64\[(\w+)\]').search
+PATTERN: Callable[[str], Match[str] | None] = re.compile(
+    r'(?:datetime|timedelta)64\[(\w+)\]').search
 
 #: Numpy time units
-RESOLUTION = [
-    'as', 'fs', 'ps', 'ns', 'us', 'ms', 's', 'm', 'h', 'D', 'W', 'M', 'Y'
-]
+RESOLUTION = ('as', 'fs', 'ps', 'ns', 'us', 'ms', 's', 'm', 'h', 'D', 'W', 'M',
+              'Y')
 
 
 def _time64_unit(dtype: DType[Any]) -> str:
     """Get the unit of time."""
-    match = PATTERN(dtype.name)
+    match: Match[str] | None = PATTERN(dtype.name)
     if match is None:
         raise ValueError(f'dtype is not a time duration: {dtype}')
     return match.group(1)
 
 
 def _min_time64_unit(*args: DType[Any]) -> str:
     """Get the minimum unit of time."""
@@ -199,21 +199,22 @@
     Args:
         begin: The beginning of the period.
         end: The ending of the period.
         within: If true, the given period defines a closed interval
             (i.e. the end date is within the period), otherwise the
             interval is open.
     """
-    __slots__ = ('_begin', '_duration_unit', '_last')
+    __slots__: tuple[str, ...] = ('_begin', '_duration_unit', '_last')
 
     def __init__(self,
                  begin: numpy.datetime64,
                  end: numpy.datetime64,
+                 *,
                  within: bool = False) -> None:
-        duration_unit = _min_time64_unit(begin.dtype, end.dtype)
+        duration_unit: str = _min_time64_unit(begin.dtype, end.dtype)
 
         #: The beginning of the period.
         self._begin: numpy.datetime64 = begin
         #: The duration unit of the period.
         self._duration_unit: numpy.timedelta64 = numpy.timedelta64(
             1, duration_unit)
         #: The last date of the period.
@@ -316,29 +317,30 @@
         """
         self._begin = self._begin - duration
         self._last = self._last + duration
 
     def contains(
         self,
         other: numpy.datetime64 | Period,
-    ) -> numpy.bool_:
+    ) -> bool:
         """Check if the given period is contains this period.
 
         Args:
             other: The other period to check.
 
         Returns:
             * True if other is a date and is inside the period, zero length
               periods contain no points
             * True if other is a period and  fully contains (or equals) the
               other period
         """
         if isinstance(other, numpy.datetime64):
-            return self._begin <= other <= self._last
-        return (self._begin <= other.begin) and (self._last >= other.last)
+            return bool(self._begin <= other <= self._last)
+        return bool((self._begin <= other.begin)
+                    and (self._last >= other.last))
 
     def is_adjacent(self, other: Period) -> bool:
         """True if periods are next to each other without a gap.
 
         In the example below, p1 and p2 are adjacent, but p3 is not adjacent
         with either of p1 or p2.
 
@@ -373,15 +375,15 @@
 
         Returns:
             True if point is after the period
         """
         if self.is_null():
             # null period isn't after
             return False
-        return bool(point < self._begin)  # numpy.bool_ -> bool
+        return bool(point < self._begin)
 
     def is_before(self, point: numpy.datetime64) -> bool:
         """True if all of the period is prior to the passed point or end <=
         point.
 
         In the example below points 4 and 5 return true.
 
@@ -396,15 +398,15 @@
 
         Returns:
             True if point is before the period
         """
         if self.is_null():
             # null period isn't before anything
             return False
-        return bool(self._last < point)  # numpy.bool_ -> bool
+        return bool(self._last < point)
 
     def intersects(self, other: Period) -> bool:
         """True if the periods overlap in any way.
 
         In the example below p1 intersects with p2, p4, and p6.
 
         .. code-block:: text
@@ -418,17 +420,17 @@
 
         Args:
             other: The other period to check.
 
         Returns:
             True if the periods intersect
         """
-        return (self.contains(other.begin) or other.contains(self._begin)
-                or ((other.begin < self._begin) and
-                    (other.last >= self._begin)))  # type:ignore
+        return bool(
+            self.contains(other.begin) or other.contains(self._begin)
+            or ((other.begin < self._begin) and (other.last >= self._begin)))
 
     def intersection(self, other: Period) -> Period:
         """Return the period of intersection or null period if no intersection.
 
         Args:
             other: The other period to check.
 
@@ -484,16 +486,18 @@
 
         Args:
             other: The other period to combine.
 
         Returns:
             The combined period.
         """
-        start = self._begin if self._begin < other.begin else other.begin
-        end = other.end() if self._last < other.last else self.end()
+        start: numpy.datetime64 = (self._begin if self._begin < other.begin
+                                   else other.begin)
+        end: numpy.datetime64 = (other.end()
+                                 if self._last < other.last else self.end())
         return Period(start, end)
 
     # pylint: disable=too-many-return-statements
     # This code has a lot of "return" statements because we have to determine
     # the relation between the two periods among 8 different cases.
     def _get_direct_relation(self, other: Period) -> PeriodRelation | None:
         """Get the direct relation between two periods."""
@@ -526,20 +530,20 @@
 
         Args:
             other: Period to consider
 
         Returns:
             The relation.
         """
-        relation = self._get_direct_relation(other)
+        relation: PeriodRelation | None = self._get_direct_relation(other)
         if relation is not None:
             return relation
 
-        period_contains_start = other.contains(self._begin)
-        period_contains_end = other.contains(self._last)
+        period_contains_start: bool = other.contains(self._begin)
+        period_contains_end: bool = other.contains(self._last)
 
         if period_contains_start and period_contains_end:
             if other.begin == self.begin:
                 return PeriodRelation.INSIDE_START_TOUCHING
             return (PeriodRelation.INSIDE_END_TOUCHING
                     if other.last == self.last else PeriodRelation.INSIDE)
```

### Comparing `zcollection-2023.3.2/zcollection/merging/tests/test_merging.py` & `zcollection-2023.5.0/zcollection/merging/tests/test_merging.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
 Test merging.
 =============
 """
 import numpy
+import pytest
 import zarr
 
-# pylint: enable=unused-import
 from .. import _update_fs, merge_time_series, perform
 from ... import sync
 from ...tests import data
 # pylint: disable=unused-import # Need to import for fixtures
 from ...tests.cluster import dask_client, dask_cluster
+from ...tests.fixture import dask_arrays, numpy_arrays
 from ...tests.fs import local_fs
 
+# pylint: enable=unused-import
+
 
 class MyError(RuntimeError):
     """Custom error."""
-    ...
 
 
 class ThrowError(sync.Sync):
     """Throw an error when merging."""
 
     def __enter__(self) -> bool:
         raise MyError('This is an error')
@@ -35,55 +37,67 @@
     def is_locked(self) -> bool:
         return False
 
 
 def test_update_fs(
         dask_client,  # pylint: disable=redefined-outer-name
         local_fs,  # pylint: disable=redefined-outer-name
-):
+) -> None:
     """Test the _update_fs function."""
-    generator = data.create_test_dataset()
-    ds = next(generator)
+    generator = data.create_test_dataset(delayed=False)
+    zds = next(generator)
 
     partition_folder = local_fs.root.joinpath('partition_folder')
 
     zattrs = str(partition_folder.joinpath('.zattrs'))
     future = dask_client.submit(_update_fs, str(partition_folder),
-                                dask_client.scatter(ds), local_fs.fs)
+                                dask_client.scatter(zds), local_fs.fs)
     dask_client.gather(future)
     assert local_fs.exists(zattrs)
 
     local_fs.fs.rm(str(partition_folder), recursive=True)
     assert not local_fs.exists(zattrs)
     seen_exception = False
     try:
-        future = dask_client.submit(_update_fs, str(partition_folder),
-                                    dask_client.scatter(ds), local_fs.fs,
-                                    ThrowError())
+        future = dask_client.submit(_update_fs,
+                                    str(partition_folder),
+                                    dask_client.scatter(zds),
+                                    local_fs.fs,
+                                    synchronizer=ThrowError())
         dask_client.gather(future)
     except MyError:
         seen_exception = True
     assert seen_exception
     assert not local_fs.exists(zattrs)
 
 
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_perform(
-        local_fs,  # pylint: disable=redefined-outer-name
-        dask_client,  # pylint: disable=redefined-outer-name
-):
+    dask_client,  # pylint: disable=redefined-outer-name
+    local_fs,  # pylint: disable=redefined-outer-name
+    arrays_type,
+    request,
+) -> None:
     """Test the perform function."""
-    generator = data.create_test_dataset()
-    ds = next(generator)
+    delayed = request.getfixturevalue(arrays_type)
+    generator = data.create_test_dataset(delayed=delayed)
+    zds = next(generator)
 
     path = str(local_fs.root.joinpath('folder'))
 
-    future = dask_client.submit(_update_fs, path, dask_client.scatter(ds),
+    future = dask_client.submit(_update_fs, path, dask_client.scatter(zds),
                                 local_fs.fs)
     dask_client.gather(future)
 
-    future = dask_client.submit(perform, dask_client.scatter(ds), path, 'time',
-                                local_fs.fs, 'time', merge_time_series)
+    future = dask_client.submit(perform,
+                                dask_client.scatter(zds),
+                                path,
+                                'time',
+                                local_fs.fs,
+                                'time',
+                                delayed=delayed,
+                                merge_callable=merge_time_series)
     dask_client.gather(future)
 
     zgroup = zarr.open_consolidated(local_fs.get_mapper(path))
-    assert numpy.all(zgroup['time'][...] == ds['time'].values)
-    assert numpy.all(zgroup['var1'][...] == ds['var1'].values)
+    assert numpy.all(zgroup['time'][...] == zds['time'].values)
+    assert numpy.all(zgroup['var1'][...] == zds['var1'].values)
```

### Comparing `zcollection-2023.3.2/zcollection/merging/tests/test_period.py` & `zcollection-2023.5.0/zcollection/merging/tests/test_period.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     return numpy.timedelta64(value, 'D')
 
 
 def _period(start: int, end: int, within: bool = False) -> Period:
     return Period(_datetime(start), _datetime(end), within=within)
 
 
-def _period1(within=False):
+def _period1(within=False) -> Period:
     return _period(1, 10, within=within)
 
 
-def _period2():
+def _period2() -> Period:
     return _period(5, 30)
 
 
-def _period3():
+def _period3() -> Period:
     return _period(35, 81)
 
 
-def test_interface():
+def test_interface() -> None:
     """Test the interface of the Period class."""
     period1 = _period1()
     assert period1.begin == _datetime(1)
     assert period1.last == _datetime(9)
     assert period1.end() == _datetime(10)
     assert period1.length() == _timedelta(9)
     assert not period1.is_null()
@@ -64,15 +64,15 @@
     assert period2.begin == _datetime(5)
     assert period2.last == _datetime(29)
     assert period2.end() == _datetime(30)
     assert period2.length() == _timedelta(25)
     assert not period2.is_null()
 
 
-def test_cmp():
+def test_cmp() -> None:
     """Test the comparison operators."""
     period1 = _period1()
     period2 = _period2()
     period3 = _period3()
 
     assert period1 == _period1()
     assert period1 != period2
@@ -80,24 +80,24 @@
 
     with pytest.raises(TypeError):
         assert period1 < 1
     assert not period1 == 1  # pylint: disable=unneeded-not
     assert period1 != 1
 
 
-def test_shift():
+def test_shift() -> None:
     """Test the shift method."""
     period1 = _period1()
     period1.shift(_timedelta(5))
     assert period1 == _period(6, 15)
     period1.shift(_timedelta(-15))
     assert period1 == _period(-9, 0)
 
 
-def test_relation():
+def test_relation() -> None:
     """Test the relations between periods."""
     period1 = _period1()
     period2 = _period2()
     period3 = _period3()
 
     assert period2.contains(_datetime(20))
     assert not period2.contains(_datetime(2))
@@ -135,15 +135,15 @@
                                                    period1.end())
 
     period1 = _period(10, 20)
     period2 = _period(15, 18)
     assert period1.intersection(period2) == period2
 
 
-def test_zero_length_period():
+def test_zero_length_period() -> None:
     """Test the zero length period."""
     zero_len = Period.from_duration(_datetime(3), _timedelta(0))
     assert _period(1, 1) == Period.from_duration(_datetime(1), _timedelta(0))
     assert _period(3, 3) == zero_len
 
     # zero_length period always returns false for is_before & is_after
     assert not zero_len.is_before(_datetime(5))
@@ -164,15 +164,15 @@
     assert zero_len.is_adjacent(_period(-10, 3))
     assert _period(-10, 3).is_adjacent(zero_len)
     assert zero_len.intersection(period1) == zero_len
     period2 = _period2()
     assert zero_len.span(period2) == _period(3, 30)
 
 
-def test_invalid_period():
+def test_invalid_period() -> None:
     """Test the invalid period."""
     null_per = _period(5, 1)
 
     assert not null_per.is_before(_datetime(7))
     assert not null_per.is_after(_datetime(7))
     assert not null_per.is_before(_datetime(-5))
     assert not null_per.is_after(_datetime(-5))
@@ -187,15 +187,15 @@
     assert period1.intersects(null_per)
     assert null_per.is_adjacent(_period(-10, 5))
     assert null_per.is_adjacent(_period(1, 10))
 
     assert null_per.span(_period3()) == _period(5, 81)
 
 
-def test_invalid():
+def test_invalid() -> None:
     """Test the invalid periods."""
     period1 = _period(0, -2)
     assert period1.begin == _datetime(0)
     assert period1.last == _datetime(-3)
     assert period1.end() == _datetime(-2)
     assert period1.length() == _timedelta(-2)
     assert period1.is_null()
@@ -279,15 +279,15 @@
 
     period1 = Period.from_duration(_datetime(5), _timedelta(3))
     period2 = _period(3, 10)
     period1.expand(_timedelta(2))
     assert period1 == period2
 
 
-def test_period_get_relation():
+def test_period_get_relation() -> None:
     """Test the get_relation method."""
 
     #          ##################
     #  #####
     start = _datetime64(2000, 6, 1)
     end = _datetime64(2000, 6, 30)
     period1 = Period(start, end, within=True)
@@ -407,17 +407,17 @@
     end = _datetime64(2000, 7, 15)
     period2 = Period(start, end, within=True)
 
     assert period1.get_relation(period2) == PeriodRelation.BEFORE
     assert period1.get_relation(period2).is_before()
 
 
-def test_pickle():
+def test_pickle() -> None:
     """Test pickling."""
     period = _period1()
     assert pickle.loads(pickle.dumps(period)) == period
 
 
-def test_invalid_type():
+def test_invalid_type() -> None:
     """Test invalid type."""
     with pytest.raises(ValueError):
         Period(numpy.int64(1), numpy.int64(2))  # type: ignore
```

### Comparing `zcollection-2023.3.2/zcollection/merging/tests/test_time_series.py` & `zcollection-2023.5.0/zcollection/merging/tests/test_time_series.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,72 +13,72 @@
 from ...tests.cluster import dask_client, dask_cluster
 
 # pylint: enable=unused-import # Need to import for fixtures
 
 
 def test_merge_disjoint(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+) -> None:
     """Test the update of two disjoint time series."""
     generator = data.create_test_dataset()
-    ds0 = next(generator)
-    ds1 = next(generator)
+    zds0 = next(generator)
+    zds1 = next(generator)
 
-    ds = time_series.merge_time_series(ds1, ds0, 'time', 'num_lines')
-    assert numpy.all(ds.variables['time'].values == numpy.concatenate((
-        ds0.variables['time'].values, ds1.variables['time'].values)))
-
-    ds = time_series.merge_time_series(ds0, ds1, 'time', 'num_lines')
-    assert numpy.all(ds.variables['time'].values == numpy.concatenate((
-        ds0.variables['time'].values, ds1.variables['time'].values)))
+    zds = time_series.merge_time_series(zds1, zds0, 'time', 'num_lines')
+    assert numpy.all(zds.variables['time'].values == numpy.concatenate((
+        zds0.variables['time'].values, zds1.variables['time'].values)))
+
+    zds = time_series.merge_time_series(zds0, zds1, 'time', 'num_lines')
+    assert numpy.all(zds.variables['time'].values == numpy.concatenate((
+        zds0.variables['time'].values, zds1.variables['time'].values)))
 
-    ds = time_series.merge_time_series(ds0, ds0, 'time', 'num_lines')
+    zds = time_series.merge_time_series(zds0, zds0, 'time', 'num_lines')
     assert numpy.all(
-        ds.variables['time'].values == ds0.variables['time'].values)
+        zds.variables['time'].values == zds0.variables['time'].values)
 
 
 def test_merge_intersection(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+) -> None:
     """Test the update of two intersecting time series."""
     generator = data.create_test_dataset()
-    ds0 = next(generator)
+    zds0 = next(generator)
     # ds0.variables["time"].values => numpy.array([
     #     "2000-01-01T00:00:00.000000", "2000-01-04T00:00:00.000000",
     #     "2000-01-07T00:00:00.000000", "2000-01-10T00:00:00.000000",
     #     "2000-01-13T00:00:00.000000", "2000-01-16T00:00:00.000000"
     # ])
-    ds1 = next(generator)
+    zds1 = next(generator)
     # ds1.variables["time"].values => numpy.array([
     #     "2000-01-19T00:00:00.000000", "2000-01-22T00:00:00.000000",
     #     "2000-01-25T00:00:00.000000", "2000-01-28T00:00:00.000000",
     #     "2000-01-31T00:00:00.000000"])
 
-    existing_ds = ds1
-    new_ds = copy.deepcopy(ds0)
-    new_ds.variables['time'] = ds0.variables['time'].duplicate(
-        ds0.variables['time'].values + numpy.timedelta64(9, 'D'))
-
-    ds = time_series.merge_time_series(existing_ds, new_ds, 'time',
-                                       'num_lines')
-    assert numpy.all(ds.variables['time'].values == numpy.concatenate((
-        ds0.variables['time'].values[3:], ds1.variables['time'].values[:])))
-
-    existing_ds = ds0
-    new_ds = copy.deepcopy(ds1)
-    new_ds.variables['time'] = ds1.variables['time'].duplicate(
-        ds1.variables['time'].values - numpy.timedelta64(9, 'D'))
-    ds = time_series.merge_time_series(existing_ds, new_ds, 'time',
-                                       'num_lines')
-    assert numpy.all(ds.variables['time'].values == numpy.concatenate((
-        ds0.variables['time'].values[:], ds1.variables['time'].values[:2])))
-
-    existing_ds = ds0
-    new_ds = ds0.isel(dict(num_lines=slice(1, -1)))
-    new_ds.variables['var1'] = new_ds.variables['var1'].duplicate(
-        new_ds.variables['var1'].values + 100)
-    ds = time_series.merge_time_series(existing_ds, new_ds, 'time',
-                                       'num_lines')
-    assert numpy.all(ds.variables['var1'].values == numpy.concatenate((
-        ds0.variables['var1'].values[:1],
-        ds0.variables['var1'].values[1:-1] + 100,
-        ds0.variables['var1'].values[-1:])))
+    existing_zds = zds1
+    new_zds = copy.deepcopy(zds0)
+    new_zds.variables['time'] = zds0.variables['time'].duplicate(
+        zds0.variables['time'].values + numpy.timedelta64(9, 'D'))
+
+    zds = time_series.merge_time_series(existing_zds, new_zds, 'time',
+                                        'num_lines')
+    assert numpy.all(zds.variables['time'].values == numpy.concatenate((
+        zds0.variables['time'].values[3:], zds1.variables['time'].values[:])))
+
+    existing_zds = zds0
+    new_zds = copy.deepcopy(zds1)
+    new_zds.variables['time'] = zds1.variables['time'].duplicate(
+        zds1.variables['time'].values - numpy.timedelta64(9, 'D'))
+    zds = time_series.merge_time_series(existing_zds, new_zds, 'time',
+                                        'num_lines')
+    assert numpy.all(zds.variables['time'].values == numpy.concatenate((
+        zds0.variables['time'].values[:], zds1.variables['time'].values[:2])))
+
+    existing_zds = zds0
+    new_zds = zds0.isel({'num_lines': slice(1, -1)})
+    new_zds.variables['var1'] = new_zds.variables['var1'].duplicate(
+        new_zds.variables['var1'].values + 100)
+    zds = time_series.merge_time_series(existing_zds, new_zds, 'time',
+                                        'num_lines')
+    assert numpy.all(zds.variables['var1'].values == numpy.concatenate((
+        zds0.variables['var1'].values[:1],
+        zds0.variables['var1'].values[1:-1] + 100,
+        zds0.variables['var1'].values[-1:])))
```

### Comparing `zcollection-2023.3.2/zcollection/merging/time_series.py` & `zcollection-2023.5.0/zcollection/merging/time_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Merging a time series
 =====================
 """
 import numpy
 
 from . import period
 from .. import dataset
+from ..type_hints import NDArray
 
 
 def merge_time_series(
     existing_ds: dataset.Dataset,
     inserted_ds: dataset.Dataset,
     axis: str,
     partitioning_dim: str,
@@ -39,38 +40,39 @@
         inserted_ds: The inserted dataset.
         axis: The axis to merge on.
         partitioning_dim: The name of the partitioning dimension.
 
     Returns:
         The merged dataset.
     """
-    existing_axis = existing_ds.variables[axis].values
-    inserted_axis = inserted_ds.variables[axis].values
+    existing_axis: NDArray = existing_ds.variables[axis].values
+    inserted_axis: NDArray = inserted_ds.variables[axis].values
     existing_period = period.Period(existing_axis.min(),
                                     existing_axis.max(),
                                     within=True)
     inserted_period = period.Period(inserted_axis.min(),
                                     inserted_axis.max(),
                                     within=True)
 
-    relation = inserted_period.get_relation(existing_period)
+    relation: period.PeriodRelation = inserted_period.get_relation(
+        existing_period)
 
     # The new piece is located before the existing data.
     if relation.is_before():
         return inserted_ds.concat(existing_ds, partitioning_dim)
 
     # The new piece is located after the existing data.
     if relation.is_after():
         return existing_ds.concat(inserted_ds, partitioning_dim)
 
     # The new piece replace the old one
     if relation.contains():
         return inserted_ds
 
-    intersection = inserted_period.intersection(existing_period)
+    intersection: period.Period = inserted_period.intersection(existing_period)
 
     # The new piece is located before, but there is an overlap
     # between the two datasets.
     if relation.is_before_overlapping():
         # pylint: disable=comparison-with-callable
         indices = numpy.where(
             # comparison between ndarray and datetime64
@@ -90,18 +92,18 @@
         return existing_ds.isel({
             partitioning_dim: indices
         }).concat(inserted_ds, partitioning_dim)
 
     assert relation.is_inside()
     # comparison between ndarray and datetime64
     index = numpy.where(existing_axis < intersection.begin)[0]  # type: ignore
-    before = existing_ds.isel(
+    before: dataset.Dataset = existing_ds.isel(
         {partitioning_dim: slice(0, index[-1] + 1, None)})
 
     # pylint: disable=comparison-with-callable
     # comparison between ndarray and datetime64
     index = numpy.where(existing_axis > intersection.end())[0]  # type: ignore
     # pylint: enable=comparison-with-callable
-    after = existing_ds.isel(
+    after: dataset.Dataset = existing_ds.isel(
         {partitioning_dim: slice(index[0], index[-1] + 1, None)})
 
     return before.concat((inserted_ds, after), partitioning_dim)
```

### Comparing `zcollection-2023.3.2/zcollection/meta.py` & `zcollection-2023.5.0/zcollection/meta.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         name: name of the key.
         value: value of the key.
     """
     __slots__ = ('name', 'value')
 
     def __init__(self, name: str, value: Any) -> None:
         #: Name of the key.
-        self.name = name
+        self.name: str = name
         #: Value of the key.
-        self.value = self._encode(value)
+        self.value: Any = self._encode(value)
 
     @staticmethod
     def _encode(value: Any) -> Any:
         """Encode an attribute value as something that can be serialized as
         JSON."""
         if isinstance(value, numpy.ndarray):
             return value.tolist()
@@ -106,49 +106,57 @@
         return Attribute(*data)
 
 
 class Variable:
     """Handle the metadata of a dataset variable.
 
     Args:
-        name: name of the variable
-        dtype: data type of the variable
-        dimensions: names of the dimensions of the variable
-        attrs: attributes of the variable
-        compressor: compression codec for the variable
-        fill_value: fill value for the variable
-        filters: filters for the variable
+        name: Name of the variable.
+        dtype: Data type of the variable.
+        dimensions: Names of the dimensions of the variable. Defaults to None.
+        attrs: Attributes of the variable. Defaults to None.
+        compressor: Compression codec for the variable. Defaults to None.
+        fill_value: Fill value for the variable. Defaults to None.
+        filters: Filters for the variable. Defaults to None.
+
+    Warning:
+        If the variable uses filters, the ``fill_value`` parameter must be the
+        value that results from decoding the filter. For example, if the filter
+        is ``FixedScaleOffset(0, 1000)`` and the desired ``fill_value`` is
+        ``65536``, then the ``fill_value`` parameter must be ``65536 / 1000 =
+        65.536``.
     """
     __slots__ = ('attrs', 'compressor', 'dimensions', 'dtype', 'fill_value',
                  'filters', 'name')
 
     def __init__(self,
                  name: str,
                  dtype: DTypeLike,
+                 *,
                  dimensions: Sequence[str] | None = None,
                  attrs: Sequence[Attribute] | None = None,
                  compressor: numcodecs.abc.Codec | None = None,
                  fill_value: Any | None = None,
                  filters: Sequence[numcodecs.abc.Codec] | None = None) -> None:
         attrs = attrs or tuple()
 
         #: Attributes of the variable.
         self.attrs = tuple(attrs)
         #: Compression codec for the variable.
-        self.compressor = compressor
+        self.compressor: numcodecs.abc.Codec | None = compressor
         #: Dimensions of the variable.
         self.dimensions = tuple(dimensions or ())
         #: Data type of the variable.
         self.dtype = numpy.dtype(dtype)
         #: Fill value for the variable.
-        self.fill_value = fill_value
+        self.fill_value: Any | None = fill_value
         #: Filter codecs for the variable.
-        self.filters = filters or tuple()
+        self.filters = tuple(filters or ())
         #: Variable name.
-        self.name = name
+        self.name: str = name
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self.name!r})'
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Variable):
             return False
@@ -156,27 +164,29 @@
 
     def get_config(self) -> dict[str, Any]:
         """Get the variable metadata.
 
         Returns:
             variable configuration.
         """
+        compressor: numcodecs.abc.Codec | None
+        compressor_config: dict[str, None] | None
+
         compressor = self.compressor
-        compressor = compressor.get_config(
+        compressor_config = compressor.get_config(
         ) if compressor is not None else None
-        filters = tuple(item.get_config() for item in self.filters)
 
         return {
             'attrs': sorted(item.get_config() for item in self.attrs),
-            'compressor': compressor,
+            'compressor': compressor_config,
             'dimensions': self.dimensions,
             'dtype': zarr.meta.encode_dtype(self.dtype),
             'fill_value': zarr.meta.encode_fill_value(self.fill_value,
                                                       self.dtype),
-            'filters': filters,
+            'filters': tuple(item.get_config() for item in self.filters),
             'name': self.name,
         }
 
     @staticmethod
     def from_config(data: dict[str, Any]) -> Variable:
         """Create a new variable from the given variable configuration.
 
@@ -187,64 +197,85 @@
             new variable.
         """
 
         def get_codec(codec) -> numcodecs.abc.Codec | None:
             """Get the codec from its configuration."""
             return zarr.codecs.get_codec(codec) if codec is not None else None
 
-        dtype = zarr.meta.decode_dtype(data['dtype'])
+        dtype: DTypeLike = zarr.meta.decode_dtype(data['dtype'])
         filters: Sequence[numcodecs.abc.Codec] = tuple(
             zarr.codecs.get_codec(item) for item in data['filters']
             if item is not None)
 
         return Variable(
             data['name'],
             dtype,
-            data['dimensions'],
-            tuple(Attribute.from_config(item) for item in data['attrs']),
-            get_codec(data['compressor']),
-            zarr.meta.decode_fill_value(data['fill_value'], dtype),
-            filters,
+            dimensions=data['dimensions'],
+            attrs=tuple(Attribute.from_config(item) for item in data['attrs']),
+            compressor=get_codec(data['compressor']),
+            fill_value=zarr.meta.decode_fill_value(data['fill_value'], dtype),
+            filters=filters,
         )
 
+    def set_for_insertion(self) -> Variable:
+        """Create a new variable without any attribute.
+
+        Returns:
+            The variable.
+        """
+        return Variable(self.name,
+                        self.dtype,
+                        dimensions=self.dimensions,
+                        compressor=self.compressor,
+                        fill_value=self.fill_value,
+                        filters=self.filters)
+
 
 class Dataset:
     """Handle the metadata of a dataset.
 
     Args:
-        dimensions: dimensions of the dataset
-        variables: variables of the dataset
-        attrs: attributes of the dataset
-        chunks: chunk size for each dimension.
-        block_size_limit: maximum size (in bytes) of a
-            block/chunk of variable's data.
+        dimensions: A sequence of strings representing the dimensions of the
+            dataset.
+        variables: A sequence of :py:class:`Variable` objects representing the
+            variables of the dataset.
+        attrs: An optional sequence of :py:class:`Attribute` objects
+            representing the attributes of the dataset. Defaults to None.
+        chunks: An optional sequence of :py:class:`Dimension` objects
+            representing the chunk size for each dimension. Defaults to None.
+        block_size_limit: An optional integer representing the maximum size
+            (in bytes) of a block/chunk of variable's data.
     """
     __slots__ = ('dimensions', 'variables', 'attrs', 'chunks',
                  'block_size_limit')
 
     def __init__(self,
                  dimensions: Sequence[str],
                  variables: Sequence[Variable],
+                 *,
                  attrs: Sequence[Attribute] | None = None,
                  chunks: Sequence[Dimension] | None = None,
                  block_size_limit: int | None = None) -> None:
         #: Dimensions of the dataset.
         self.dimensions = tuple(dimensions)
 
         #: Variables of the dataset.
-        self.variables = {item.name: item for item in variables}
+        self.variables: dict[str, Variable] = {
+            item.name: item
+            for item in variables
+        }
 
         #: Attributes of the dataset.
-        self.attrs = attrs or []
+        self.attrs = list(attrs or [])
 
         #: Maximum data chunk size
-        self.block_size_limit = block_size_limit or BLOCK_SIZE_LIMIT
+        self.block_size_limit: int = block_size_limit or BLOCK_SIZE_LIMIT
 
         #: Chunk size for each dimension
-        self.chunks = chunks or []
+        self.chunks = list(chunks or [])
 
     def select_variables(
         self,
         keep_variables: Iterable[str] | None = None,
         drop_variables: Iterable[str] | None = None,
     ) -> set[str]:
         """Select variables to keep or drop from the dataset.
@@ -275,38 +306,40 @@
 
     def get_config(self) -> dict[str, Any]:
         """Get the dataset metadata.
 
         Returns:
             Dataset configuration.
         """
+        attrs: list[tuple[str, Any]]
+        variables: tuple[dict[str, Any], ...]
+
+        attrs = sorted(item.get_config() for item in self.attrs)
+        variables = tuple(self.variables[name].get_config()
+                          for name in sorted(self.variables))
+
         return {
-            'attrs':
-            sorted(item.get_config() for item in self.attrs),
-            'dimensions':
-            self.dimensions,
-            'variables':
-            tuple(self.variables[name].get_config()
-                  for name in sorted(self.variables)),
-            'chunks':
-            sorted(item.get_config() for item in self.chunks),
-            'block_size_limit':
-            self.block_size_limit
+            'attrs': attrs,
+            'dimensions': self.dimensions,
+            'variables': variables,
+            'chunks': tuple(item.get_config() for item in self.chunks),
+            'block_size_limit': self.block_size_limit
         }
 
     def add_variable(self, variable: Variable) -> None:
         """Add a variable to the dataset.
 
         Args:
             variable: variable to add.
 
         Raises:
-            TypeError: if the variable is not a Variable.
-            ValueError: if the variable already exists or if the variable
-                dimensions don't match the dataset dimensions.
+            TypeError: If the variable is not a Variable object.
+            ValueError: If the variable already exists in the dataset or if
+                the variable's dimensions do not match the dataset's
+                dimensions.
         """
         if not isinstance(variable, Variable):
             raise TypeError(
                 f'variable must be a Variable, not {type(variable)}')
         if variable.name in self.variables:
             raise ValueError(
                 f'The variable {variable.name!r} already exists in the '
@@ -336,42 +369,47 @@
             chunks=tuple(
                 Dimension.from_config(item)
                 for item in data.get('chunks', [])),
             block_size_limit=data.get('block_size_limit'),
         )
 
     def search_same_dimensions_as(self, variable: Variable) -> Variable:
-        """Search for a variable in this dataset with the same dimensions as
-        the given variable.
+        """Searches for a variable in this dataset that has the same dimensions
+        as the given variable.
 
         Args:
             variable: The variable used for searching.
 
         Returns:
-            The variable having the same dimensions as the supplied variable.
+            The variable that has the same dimensions as the supplied
+            variable.
 
         Raises:
             ValueError: If no variable with the same dimensions as the given
-                variable is found.
+            variable is found.
         """
         for item in self.variables.values():
             if item.dimensions == variable.dimensions:
                 return item
         raise ValueError('No variable using the same dimensions exists.')
 
-    def missing_variables(self, other: Dataset) -> Sequence[str]:
+    def missing_variables(self, other: Dataset) -> tuple[str, ...]:
         """Finds the variables in the provided dataset that are not in this
         instance.
 
         Args:
             other: The dataset to compare against.
 
         Returns:
-            The names of the missing variables in this dataset relative to the
-            provided dataset.
+            A tuple containing the names of the variables that are defined in
+            this dataset but not in the provided dataset.
+
+        Raises:
+            ValueError: If the provided dataset does not define one or more
+                variables that are defined in this dataset.
         """
         this = set(self.variables)
         others = set(other.variables)
 
         if len(others - this):
             raise ValueError('The reference dataset does not define the '
                              f'{", ".join(others - this)} variables that are '
@@ -382,20 +420,22 @@
     def select_variables_by_dims(self,
                                  dims: Sequence[str],
                                  predicate: bool = True) -> set[str]:
         """Select variables that have at least one dimension in the given
         dimensions depending on the predicate.
 
         Args:
-            dims: The dimensions to select.
-            predicate: If True, select variables that have the given dimensions.
-                If False, select variables that don't have the given dimensions.
+            dims: A sequence of dimensions to select.
+            predicate: A boolean value that determines whether to select
+                variables that have the given dimensions (True) or variables
+                that don't have the given dimensions (False).
 
         Returns:
-            The names of the variables that have the given dimensions.
+            A set of variable names that have the given dimensions (if predicate
+            is True) or don't have the given dimensions (if predicate is False).
         """
         if len(dims) == 0:
             return {
                 name
                 for name, var in self.variables.items()
                 if (len(var.dimensions) == 0) == predicate
             }
```

### Comparing `zcollection-2023.3.2/zcollection/partitioning/__init__.py` & `zcollection-2023.5.0/zcollection/partitioning/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 from .date import Date
 from .registry import get_codecs, register_codec
 from .sequence import Sequence
 
 register_codec(Date)
 register_codec(Sequence)
 
-__all__ = ['Partitioning', 'Date', 'Sequence', 'get_codecs']
+__all__ = ('Partitioning', 'Date', 'Sequence', 'get_codecs')
```

### Comparing `zcollection-2023.3.2/zcollection/partitioning/abc.py` & `zcollection-2023.5.0/zcollection/partitioning/abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,62 +4,74 @@
 # BSD-style license that can be found in the LICENSE file.
 """
 Partitioning scheme.
 ====================
 """
 from __future__ import annotations
 
-from typing import Any, ClassVar, Iterator, Sequence, Tuple
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    Generator,
+    Iterator,
+    Match,
+    Optional,
+    Sequence,
+    Tuple,
+)
 import abc
 import collections
 import re
 
-import dask.array
 import dask.array.core
 import dask.array.creation
 import dask.array.reductions
 import dask.array.wrap
 import fsspec
 import numpy
 
 from .. import dataset
-from ..type_hints import NDArray
+from ..type_hints import ArrayLike, DTypeLike, NDArray
 
 #: Object that represents a partitioning scheme
 Partition = Tuple[Tuple[Tuple[str, Any], ...], slice]
 
+#: The callable that parses the partitioning scheme
+PatternType = Callable[[str], Optional[Match[str]]]
+
 #: Allowed data types for partitioning schemes
 DATA_TYPES = ('int8', 'int16', 'int32', 'int64', 'uint8', 'uint16', 'uint32',
               'uint64')
 
 
 def _logical_or_reduce(
     arr: dask.array.core.Array,
+    *,
     axis: int | tuple[int, ...] | None = None,
 ) -> dask.array.core.Array:
     """Implementation of `numpy.logical_or` reduction with dask.
 
     Args:
         arr: Array to reduce.
         axis: Axis to reduce. If this is None, a reduction is performed over
             all the axes. If this is a tuple of ints, a reduction is performed
             on multiple axes, instead of a single axis or all the axes as
             before.
-
     Returns:
         Reduced array.
     """
     axis = axis or 0
 
     #: pylint: disable=unused-argument
     # The function signature is required by the `dask.array.reduce` function.
-    def chunk(block, axis, keepdims):
+    def chunk(block, axis, keepdims) -> Any:
         return block
 
-    def aggregate(block, axis, keepdims):
+    def aggregate(block, axis, keepdims) -> Any:
         return numpy.logical_or.reduce(block, axis=axis)
 
     #: pylint: enable=unused-argument
 
     return dask.array.reductions.reduction(
         arr[1:] != arr[:-1],  # type: ignore
         chunk=chunk,
@@ -70,52 +82,73 @@
 
 
 def unique(arr: dask.array.core.Array) -> tuple[NDArray, NDArray]:
     """Return unique elements and their indices.
 
     Args:
         arr: Array of elements.
-
     Returns:
         Tuple of unique elements and their indices.
     """
-    size = arr.shape[0]
-    chunks = arr.chunks[0]
+    size: int = arr.shape[0]
+    chunks: tuple[int, ...] = arr.chunks[0]
     #: pylint: disable=not-callable
-    mask = dask.array.wrap.empty((size, ), dtype=numpy.bool_, chunks=chunks)
+    mask: dask.array.core.Array = dask.array.wrap.empty((size, ),
+                                                        dtype=numpy.bool_,
+                                                        chunks=chunks)
     #: pylint: enable=not-callable
     mask[0] = True
     mask[1:] = (_logical_or_reduce(arr, axis=1)
                 if arr.ndim > 1 else arr[1:] != arr[:-1])
-    dtype = numpy.uint32 if size < 2**32 else numpy.uint64
-    indices = dask.array.creation.arange(size, dtype=dtype, chunks=chunks)
+    dtype: DTypeLike = numpy.uint32 if size < 2**32 else numpy.uint64
+    indices: dask.array.core.Array = dask.array.creation.arange(
+        size,
+        dtype=dtype,
+        chunks=chunks,  # type: ignore[arg-type]
+    )
     mask = mask.persist()
     return arr[mask].compute(), indices[mask].compute()
 
 
+def unique_and_check_monotony(arr: ArrayLike) -> tuple[NDArray, NDArray]:
+    """Return unique elements and their indices.
+
+    Args:
+        arr: Array of elements.
+        is_delayed: If True, the array is delayed.
+    Returns:
+        Tuple of unique elements and their indices.
+    """
+    index: NDArray
+    indices: NDArray
+
+    index, indices = numpy.unique(arr, axis=0, return_index=True)
+    if not numpy.all(numpy.diff(indices) > 0):
+        raise ValueError('index is not monotonic')
+    return index, indices
+
+
 def difference(arr: NDArray) -> NDArray:
     """Calculate the difference between each element in the array and the
     previous element.
 
     Args:
         arr: Array to calculate the difference for.
-
     Returns:
         Array of differences
     """
     return arr[1:] - arr[:-1]  # type: ignore
 
 
 def concatenate_item(arr: NDArray, item: Any) -> NDArray:
     """Concatenate an array with a given item.
 
     Args:
         arr: Array to concatenate.
         item: Item to concatenate.
-
     Returns:
         Concatenated array.
     """
     return numpy.concatenate([arr, numpy.array([item], dtype=arr.dtype)])
 
 
 def list_partitions(
@@ -124,21 +157,19 @@
     depth: int,
     root: bool = True,
 ) -> Iterator[str]:
     """The number of variables used for partitioning.
 
     The function will go down the tree and return all the files present when the
     requested depth is reached.
-
     Args:
         fs: file system object
         path: path to the directory
         depth: maximum depth of the directory tree.
         root: if True, the path is the root of the tree.
-
     Returns:
         Iterator of (path, directories, files).
     """
     if depth == -1:
         return StopIteration()
 
     if root:
@@ -167,22 +198,31 @@
         return StopIteration()
 
     for item in sorted(fs.ls(path, detail=False)):
         yield from list_partitions(fs, item, depth=depth - 1, root=False)
     return StopIteration()
 
 
-class Partitioning(abc.ABC):
-    """Partitioning scheme.
+class Partitioning(metaclass=abc.ABCMeta):
+    """Initializes a new Partitioning instance.
 
     Args:
-        variables:  List of variables to be used for partitioning
-        dtype: The list of data types allowing to store the values of variables
-            in a binary representation without loss of information.
-            Defaults to int64.
+        variables: A list of strings representing the variables to be used for
+            partitioning.
+        dtype: An optional sequence of strings representing the data type used
+            to store variable values in a binary representation without data
+            loss. Must be one of the following allowed data types: ``int8``,
+            ``int16``, ``int32``, ``int64``, ``uint8``, ``uint16``, ``uint32``,
+            ``uint64``. If not provided, defaults to ``int64`` for all
+            variables.
+
+    Raises:
+        TypeError: If dtype is not a sequence of strings.
+        ValueError: If any of the data types provided is not one of the allowed
+            data types.
     """
     __slots__ = ('_dtype', '_pattern', 'variables')
 
     #: The ID of the partitioning scheme
     ID: ClassVar[str | None] = None
 
     def __init__(self,
@@ -192,17 +232,18 @@
             raise TypeError('dtype must be a sequence of strings')
         if len(variables) == 0:
             raise ValueError('variables must not be empty')
         #: Variables to be used for the partitioning.
         self.variables = tuple(variables)
         #: Data type used to store variable values in a binary representation
         #: without data loss.
-        self._dtype = dtype or ('int64', ) * len(self.variables)
+        self._dtype: tuple[str, ...] = tuple(
+            dtype) if dtype is not None else ('int64', ) * len(self.variables)
         #: The regular expression that matches the partitioning scheme.
-        self._pattern = self._regex().search
+        self._pattern: PatternType = self._regex().search
 
         if len(set(self._dtype) - set(DATA_TYPES)) != 0:
             raise ValueError(
                 f"Data type must be one of {', '.join(DATA_TYPES)}.")
 
     def __len__(self) -> int:
         """Return the number of partitions."""
@@ -219,159 +260,156 @@
     def _regex(self) -> re.Pattern:
         """Return a regular expression that matches the partitioning scheme."""
         return re.compile('.'.join(f'({item})=(.*)' for item in self._keys()))
 
     @abc.abstractmethod
     def _split(
         self,
-        variables: dict[str, dask.array.core.Array],
+        variables: dict[str, ArrayLike],
     ) -> Iterator[Partition]:
         """Split the variables constituting the partitioning into partitioning
         schemes.
 
         Args:
             variables: The variables to be split constituting the
                 partitioning scheme.
-
         Returns:
             A sequence of tuples that contains the partitioning
                 scheme and the associated indexer to divide the dataset on each
                 partition found..
         """
 
     @staticmethod
     def _partition(selection: tuple[tuple[str, Any], ...]) -> tuple[str, ...]:
         """Format the partitioning scheme."""
         return tuple(f'{k}={v}' for k, v in selection)
 
     def index_dataset(
         self,
-        ds: dataset.Dataset,
+        zds: dataset.Dataset,
     ) -> Iterator[Partition]:
         """Yield the indexing scheme for the given dataset.
 
         Args:
-            ds: The dataset to be indexed.
-
+            zds: The dataset to be indexed.
         Yields:
             The indexing scheme for the partitioning scheme.
-
         Raises:
             ValueError: if one of the variables needs for the partitioning
                 is not monotonic.
         """
         variables = collections.OrderedDict(
-            (name, ds.variables[name].array) for name in self.variables)
-        # If the dask array is too chunked, the calculation is excessively
-        # long.
-        return self._split(
-            {name: arr.rechunk().persist()
-             for name, arr in variables.items()})
+            (name, zds.variables[name].array) for name in self.variables)
+        if zds.delayed:
+            # If the dask array is too chunked, the calculation is excessively
+            # long.
+            return self._split({
+                name: arr.rechunk().persist()
+                for name, arr in variables.items()
+            })
+        return self._split(variables)
 
     def split_dataset(
         self,
-        ds: dataset.Dataset,
+        zds: dataset.Dataset,
         axis: str,
     ) -> Iterator[tuple[tuple[str, ...], dict[str, slice]]]:
         """Split the dataset into partitions.
 
         Args:
-            ds:  The dataset to be split.
+            zds:  The dataset to be split.
             axis: The axis to be used for the splitting.
-
         Yields:
             The partitioning scheme and the indexer to divide the dataset on
             each partition found.
-
         Raises:
             ValueError: if one of the variables needs for the partitioning
                 is not a one-dimensional array.
         """
         for item in self.variables:
-            if len(ds.variables[item].shape) != 1:
+            if len(zds.variables[item].shape) != 1:
                 raise ValueError(f'f{item!r} must be a one-dimensional array')
         return ((self._partition(selection), {
             axis: indexer
-        }) for selection, indexer in self.index_dataset(ds))
+        }) for selection, indexer in self.index_dataset(zds))
 
     def get_config(self) -> dict[str, Any]:
         """Return the configuration of the partitioning scheme.
 
         Returns:
             The configuration of the partitioning scheme.
         """
-        config = {'id': self.ID}
-        slots = (getattr(_class, '__slots__', ())
-                 for _class in reversed(self.__class__.__mro__))
+        config: dict[str, str | None] = {'id': self.ID}
+        slots: Generator[tuple[str, ...], None, None] = (getattr(
+            _class, '__slots__',
+            ()) for _class in reversed(self.__class__.__mro__))
         config.update((attr, getattr(self, attr)) for _class in slots
                       for attr in _class if not attr.startswith('_'))
         return config
 
     @classmethod
     def from_config(cls, config) -> Partitioning:
         """Create a partitioning scheme from a configuration.
 
         Args:
             config: The configuration of the partitioning scheme.
-
         Returns:
             The partitioning scheme.
         """
         return cls(**config)
 
     def parse(self, partition: str) -> tuple[tuple[str, int], ...]:
         """Parse a partitioning scheme.
 
         Args:
             partition: The partitioning scheme to be parsed.
-
         Returns:
             The parsed partitioning scheme.
+        Raises:
+            ValueError: if the partitioning scheme is not driven by this
+                instance.
         """
-        match = self._pattern(partition)
+        match: Match[str] | None = self._pattern(partition)
         if match is None:
             raise ValueError(
                 f'Partition is not driven by this instance: {partition}')
-        groups = match.groups()
+        groups: tuple[str, ...] = match.groups()
         return tuple((groups[ix], int(groups[ix + 1]))
                      for ix in range(0, len(groups), 2))
 
     @abc.abstractmethod
     def encode(
         self,
         partition: tuple[tuple[str, int], ...],
     ) -> tuple[Any, ...]:
         """Encode a partitioning scheme to the handled values.
 
         Args:
             partition: The partitioning scheme to be encoded.
-
         Returns:
             The encoded partitioning scheme.
         """
 
     @abc.abstractmethod
     def decode(self, values: tuple[Any, ...]) -> tuple[tuple[str, int], ...]:
         """Decode a partitioning scheme.
 
         Args:
             values: The encoded partitioning scheme.
-
         Returns:
             The decoded partitioning scheme.
         """
 
     @staticmethod
     def join(partition_scheme: tuple[tuple[str, int], ...], sep: str) -> str:
         """Join a partitioning scheme.
 
         Args:
             partition_scheme: The partitioning scheme to be joined.
             sep: The separator to be used.
-
         Returns:
             The joined partitioning scheme.
         """
         return sep.join(f'{k}={v}' for k, v in partition_scheme)
 
     def list_partitions(
         self,
@@ -379,12 +417,11 @@
         path: str,
     ) -> Iterator[str]:
         """List the partitions.
 
         Args:
             fs: The filesystem to be used.
             path: The path to the directory containing the partitions.
-
         Yields:
             The partitions.
         """
         return list_partitions(fs, path, depth=len(self) - 1)
```

### Comparing `zcollection-2023.3.2/zcollection/partitioning/date.py` & `zcollection-2023.5.0/zcollection/partitioning/date.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,46 +5,75 @@
 """
 Partitioning by date
 ====================
 """
 from __future__ import annotations
 
 from typing import Any, ClassVar, Iterator, Sequence
+import datetime
 
 import dask.array.core
 import numpy
 
 from . import abc
+from ..type_hints import ArrayLike, NDArray
 
 #: Numpy time units
 RESOLUTION = ('Y', 'M', 'D', 'h', 'm', 's')
 
 #: Numpy time unit meanings
 UNITS = ('year', 'month', 'day', 'hour', 'minute', 'second')
 
 #: Data type for time units
 DATA_TYPES = ('uint16', 'uint8', 'uint8', 'uint8', 'uint8', 'uint8')
 
 #: Time separation units
-SEPARATORS = {
+SEPARATORS: dict[str, str] = {
     'year': '-',
     'month': '-',
     'day': 'T',
     'hour': ':',
     'minute': ':',
     'second': '.'
 }
 
 
+def _unique(arr: ArrayLike, is_delayed: bool) -> tuple[NDArray, NDArray]:
+    """Return unique elements and their indices.
+
+    Args:
+        arr: Array of elements.
+        is_delayed: If True, the array is delayed.
+    Returns:
+        Tuple of unique elements and their indices.
+    Raises:
+        ValueError: If the array is not monotonic.
+    """
+    index: NDArray
+    indices: NDArray
+
+    if is_delayed:
+        index, indices = abc.unique(arr)  # type: ignore[arg-type]
+        # We don't use here the function `numpy.diff` but `abc.difference` for
+        # optimization purposes.
+        if not numpy.all(
+                abc.difference(index.view(numpy.int64)) >= 0):  # type: ignore
+            raise ValueError('index is not monotonic')
+        return index, indices
+    return abc.unique_and_check_monotony(arr)
+
+
 class Date(abc.Partitioning):
-    """Date partitioning.
+    """Initialize a partitioning scheme based on dates.
 
     Args:
-        variables: Variable names used for the partitioning.
-        resolution: Time resolution of the partitioning.
+        variables: A list of strings representing the variables to be used for
+            partitioning.
+        resolution: Time resolution of the partitioning. Must be in
+            :data:`RESOLUTION`.
 
     Raises:
         ValueError: If the resolution is not in the list of supported
             resolutions or if the partitioning is not performed on a one
             dimensional variable.
 
     Example:
@@ -57,20 +86,20 @@
 
     def __init__(self, variables: Sequence[str], resolution: str) -> None:
         if len(variables) != 1:
             raise ValueError(
                 'Partitioning on dates is performed on a single variable.')
         if resolution not in RESOLUTION:
             raise ValueError('resolution must be in: ' + ', '.join(RESOLUTION))
-        index = RESOLUTION.index(resolution) + 1
+        index: int = RESOLUTION.index(resolution) + 1
 
         #: The time resolution of the partitioning
-        self.resolution = resolution
+        self.resolution: str = resolution
         #: The time parts used for the partitioning
-        self._attrs = UNITS[:index + 1]
+        self._attrs: tuple[str, ...] = UNITS[:index + 1]
         #: The indices of the time parts used for the partitioning
         self._index = tuple(range(index))
         super().__init__(variables,
                          tuple(DATA_TYPES[ix] for ix in self._index))
 
     def _keys(self) -> Sequence[str]:
         """Return the keys of the partitioning scheme."""
@@ -79,40 +108,42 @@
     # pylint: disable=arguments-differ
     # False positive: the base method is static.
     def _partition(  # type: ignore[override]
         self,
         selection: tuple[tuple[str, Any], ...],
     ) -> tuple[str, ...]:
         """Return the partitioning scheme for the given selection."""
-        _, datetime64 = selection[0]
-        datetime = datetime64.astype('M8[s]').item()
+        datetime64: NDArray = selection[0][1]
+        py_datetime: datetime.datetime = datetime64.astype('M8[s]').item()
         return tuple(UNITS[ix] + '=' +
-                     f'{getattr(datetime, self._attrs[ix]):02d}'
+                     f'{getattr(py_datetime, self._attrs[ix]):02d}'
                      for ix in self._index)
         # pylint: enable=arguments-differ
 
     def _split(
         self,
-        variables: dict[str, dask.array.core.Array],
+        variables: dict[str, ArrayLike],
     ) -> Iterator[abc.Partition]:
         """Return the partitioning scheme for the given variables."""
+        index: NDArray
+        indices: NDArray
+        name: str
+        values: ArrayLike
+
+        # Determine if the variables are handled by Dask.
+        is_delayed: bool = any(
+            isinstance(value, dask.array.core.Array)
+            for value in variables.values())
         name, values = tuple(variables.items())[0]
 
         if not numpy.issubdtype(values.dtype, numpy.dtype('datetime64')):
             raise TypeError('values must be a datetime64 array')
 
-        index, indices = abc.unique(
-            values.astype(f'datetime64[{self.resolution}]'))
-
-        # We don't use here the function `numpy.diff` but `abc.difference` for
-        # optimization purposes.
-        if not numpy.all(
-                abc.difference(index.view(numpy.int64)) >= 0):  # type: ignore
-            raise ValueError('index is not monotonic')
-
+        index, indices = _unique(
+            values.astype(f'datetime64[{self.resolution}]'), is_delayed)
         indices = abc.concatenate_item(indices, values.size)
 
         return ((((name, date), ), slice(start, indices[ix + 1], None))
                 for date, (ix, start) in zip(index, enumerate(indices[:-1])))
 
     @staticmethod
     def _stringify(partition: tuple[tuple[str, int], ...]) -> str:
@@ -177,11 +208,11 @@
             The decoded partitioning scheme.
 
         Example:
             >>> partitioning = Date(variables=("time", ), resolution="D")
             >>> partitioning.decode((numpy.datetime64('2020-01-01'), ))
             (("year", 2020), ("month", 1), ("day", 1))
         """
-        datetime64, = values
-        datetime = datetime64.astype('M8[s]').item()
-        return tuple((UNITS[ix], getattr(datetime, self._attrs[ix]))
+        datetime64: NDArray = values[0]
+        py_datetime: datetime.datetime = datetime64.astype('M8[s]').item()
+        return tuple((UNITS[ix], getattr(py_datetime, self._attrs[ix]))
                      for ix in self._index)
```

### Comparing `zcollection-2023.3.2/zcollection/partitioning/registry.py` & `zcollection-2023.5.0/zcollection/partitioning/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,49 +4,55 @@
 # BSD-style license that can be found in the LICENSE file.
 """
 Registers the partitioning codecs.
 ==================================
 """
 from __future__ import annotations
 
+from typing import Any
+
 from . import abc
 
 #: A registry of all available partitioning codecs.
-CODEC_REGISTRY: dict[str, abc.Partitioning] = {}
+CODEC_REGISTRY: dict[str, type[abc.Partitioning]] = {}
 
 
-def get_codecs(config: dict) -> abc.Partitioning:
+def get_codecs(config: dict[str, Any]) -> abc.Partitioning:
     """Get the partitioning scheme for the given configuration.
 
     Args:
         config: A dictionary of the partitioning configuration parameters.
 
     Returns:
         The partitioning scheme.
 
     Raises:
         ValueError: If the requested codec is not defined.
     """
-    codec_id = config.pop('id', None)
+    codec_id: Any | None = config.pop('id', None)
     if codec_id is None:
         raise ValueError(f'codec not available: {codec_id!r}')
-    cls = CODEC_REGISTRY.get(codec_id, None)
+    cls: type[abc.Partitioning] | None = CODEC_REGISTRY.get(codec_id, None)
     if cls is None:
         raise ValueError(f'codec not available: {codec_id!r}')
     return cls.from_config(config)
 
 
-def register_codec(cls, codec_id=None) -> None:
+def register_codec(cls: type[abc.Partitioning],
+                   *,
+                   codec_id: str | None = None) -> None:
     """Register a partitioning scheme.
 
     Args:
         cls: The partitioning scheme class.
         codec_id: The partitioning scheme identifier.
 
     Raises:
         ValueError: If the codec identifier is already registered.
     """
     if codec_id is None:
         codec_id = cls.ID
+    if codec_id is None:
+        raise ValueError('codec identifier not defined')
     if codec_id in CODEC_REGISTRY:
         raise ValueError(f'codec already registered: {codec_id!r}')
     CODEC_REGISTRY[codec_id] = cls
```

### Comparing `zcollection-2023.3.2/zcollection/partitioning/sequence.py` & `zcollection-2023.5.0/zcollection/partitioning/sequence.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Any, ClassVar, Iterator
 
 import dask.array.core
 import dask.array.routines
 import numpy
 
 from . import abc
-from ..type_hints import NDArray
+from ..type_hints import ArrayLike, NDArray
 
 
 def _is_monotonic(arr: NDArray) -> bool:
     """Check if the array is monotonic.
 
     The matrix will be sorted in the reverse order of the partitioning keys
     (column in the matrix). If the order of the matrix is unchanged, the
@@ -28,56 +28,90 @@
     Args:
         arr: The array to check.
 
     Returns:
         True if the array is monotonic, False otherwise.
     """
     # `reversed` because `numpy.lexsort` wants the most significant key last.
-    values = [arr[:, ix] for ix in reversed(range(arr.shape[1]))]
-    sort_order = numpy.lexsort(numpy.array(values))
+    values: list[NDArray] = [
+        arr[:, ix] for ix in reversed(range(arr.shape[1]))
+    ]
+    sort_order: NDArray = numpy.lexsort(numpy.array(values))
     return numpy.all(abc.difference(sort_order) > 0)  # type: ignore
 
 
+def _unique(arr: ArrayLike, is_delayed: bool) -> tuple[NDArray, NDArray]:
+    """Return unique elements and their indices.
+
+    Args:
+        arr: Array of elements.
+        is_delayed: If True, the array is delayed.
+    Returns:
+        Tuple of unique elements and their indices.
+    """
+    index: NDArray
+    indices: NDArray
+
+    if is_delayed:
+        index, indices = abc.unique(arr)  # type: ignore[arg-type]
+        if not _is_monotonic(index):
+            raise ValueError('index is not monotonic')
+        return index, indices
+    return abc.unique_and_check_monotony(arr)
+
+
 class Sequence(abc.Partitioning):
-    """Partitioning a sequence of variables.
+    """Initialize a partitioning scheme for a sequence of variables.
 
     A sequence is a combination of variables constituting unique monotonic keys.
     For example, the orbit number (``cycle``) and the half-orbit number
     (``pass``) of a satellite.
 
     Args:
-        variables: The sequence of variables constituting the partitioning.
-        dtype: The data type of the partitioning.
+        variables: A list of strings representing the variables to be used for
+            partitioning.
+        dtype: An optional sequence of strings representing the data type used
+            to store variable values in a binary representation without data
+            loss. Must be one of the following allowed data types: ``int8``,
+            ``int16``, ``int32``, ``int64``, ``uint8``, ``uint16``, ``uint32``,
+            ``uint64``. If not provided, defaults to ``int64`` for all
+            variables.
 
     Raises:
         ValueError: If the periodicity is not valid.
 
     Example:
         >>> partitioning = Sequence(["a", "b", "c"], (None, 10, 10))
     """
     #: The ID of the partitioning scheme.
     ID: ClassVar[str] = 'Sequence'
 
     # pylint: disable=arguments-differ
     # False positive: `self` is used in the signature.
     @staticmethod
-    def _split(
-        variables: dict[str,
-                        dask.array.core.Array]) -> Iterator[abc.Partition]:
+    def _split(variables: dict[str, ArrayLike]) -> Iterator[abc.Partition]:
         """Split the variables constituting the partitioning into partitioning
         schemes."""
+        index: NDArray
+        indices: NDArray
+        matrix: dask.array.core.Array | NDArray
+
+        # Determine if the variables are handled by Dask.
+        is_delayed: bool = any(
+            isinstance(item, dask.array.core.Array)
+            for item in variables.values())
+
+        # Combines the arrays of variable values into a transposed matrix.
         matrix = dask.array.routines.vstack(tuple(
-            variables.values())).transpose()
+            variables.values())).transpose() if is_delayed else numpy.vstack(
+                tuple(variables.values())).transpose()
         if matrix.dtype.kind not in 'iu':
             raise TypeError('The variables must be integer')
 
-        index, indices = abc.unique(matrix)
-        if not _is_monotonic(index):
-            raise ValueError('index is not monotonic')
-
+        index, indices = _unique(matrix, is_delayed)  # type: ignore[arg-type]
         indices = abc.concatenate_item(indices, matrix.shape[0])
 
         fields = tuple(variables.keys())
         # pylint: disable=unnecessary-lambda-assignment
         # We want to reference a lambda function, not assign it to a variable.
         if len(fields) == 1:
             concat: Any = lambda fields, keys: (fields + keys, )
```

### Comparing `zcollection-2023.3.2/zcollection/partitioning/tests/test_date.py` & `zcollection-2023.5.0/zcollection/partitioning/tests/test_date.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
 Test partitioning by date.
 ==========================
 """
-from typing import Iterator
+from __future__ import annotations
+
+import dataclasses
 import pickle
 import random
 import string
 
 import dask.array.core
 import dask.local
 import fsspec
@@ -18,25 +20,74 @@
 import pytest
 import xarray
 
 from .. import Date, get_codecs
 from ... import dataset
 # pylint: disable=unused-import # Need to import for fixtures
 from ...tests.cluster import dask_client, dask_cluster
+from ...type_hints import NDArray
 
 # pylint: disable=disable=unused-argument
 
+#: First date of the dataset to partition
+START_DATE = numpy.datetime64('2000-01-06', 'ns')
+
+#: Time delta between two partitions
+TIME_DELTA = numpy.timedelta64(1, 'h')
+
+
+@dataclasses.dataclass(frozen=True)
+class PartitionTestData:
+    """Test data for partitioning."""
+    timedelta: numpy.timedelta64
+    indices: slice
+    resolution: str
+    partitioning: Date
+    dates: NDArray
+
+    def check_partitioning(self, date: numpy.datetime64, zds: dataset.Dataset,
+                           partition: tuple[str, ...]) -> None:
+        """Check the partitioning of a dataset."""
+        item = date.astype('datetime64[us]').item()
+        assert partition == (
+            f'year={item.year}',
+            f'month={item.month:02d}',
+            f'day={item.day:02d}',
+            f'hour={item.hour:02d}',
+        )[self.indices]
+
+        folder = '/'.join(partition)
+        fields = self.partitioning.parse(folder)
+        parsed_date, = self.partitioning.encode(fields)
+        assert parsed_date == numpy.datetime64(date).astype(
+            f'datetime64[{self.resolution}]')
+
+        expected_selection = self.dates[
+            (self.dates >= parsed_date)
+            & (self.dates < parsed_date + self.timedelta)]
+        assert numpy.all(zds.variables['dates'].compute(
+            scheduler=dask.local.get_sync) == expected_selection)
+
+        assert fields == (
+            ('year', item.year),
+            ('month', item.month),
+            ('day', item.day),
+            ('hour', item.hour),
+        )[self.indices]
+        assert self.partitioning.join(fields, '/') == folder
+        assert self.partitioning.join(
+            self.partitioning.decode((parsed_date, )), '/') == folder
 
+
+@pytest.mark.parametrize('delayed', [False, True])
 def test_split_dataset(
-        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+    dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+    delayed: bool,
+) -> None:
     """Test the split_dataset method."""
-    start_date = numpy.datetime64('2000-01-06', 'us')
-    delta = numpy.timedelta64(1, 'h')
-
     for end_date, indices, resolution in [
         (
             numpy.datetime64('2001-12-31', 'Y'),
             slice(0, 1),
             'Y',
         ),
         (
@@ -56,78 +107,47 @@
         ),
     ]:
 
         # Time delta between two partitions
         timedelta = numpy.timedelta64(1, resolution)
 
         # Temporal axis to split
-        dates = numpy.arange(start_date, end_date, delta)
+        dates: NDArray = numpy.arange(START_DATE, end_date, TIME_DELTA)
 
         # Measured data
-        observation = numpy.random.rand(dates.size)  # type: ignore
+        observation: NDArray = numpy.random.rand(dates.size)  # type: ignore
 
         # Create the dataset to split
-        ds = xarray.Dataset(
-            dict(dates=xarray.DataArray(dates, dims=('num_lines', )),
-                 observation=xarray.DataArray(observation,
-                                              dims=('num_lines', ))))
+        xds = xarray.Dataset({
+            'dates':
+            xarray.DataArray(dates, dims=('num_lines', )),
+            'observation':
+            xarray.DataArray(observation, dims=('num_lines', ))
+        })
 
         partitioning = Date(('dates', ), resolution)
         assert len(partitioning) == len(range(indices.start, indices.stop))
 
         # Date of the current partition
-        date = numpy.datetime64(start_date, resolution)
+        date = numpy.datetime64(START_DATE, resolution)
 
         # Build the test dataset
-        ds = dataset.Dataset.from_xarray(ds)
-
-        iterator = partitioning.split_dataset(ds, 'num_lines')
-        assert isinstance(iterator, Iterator)
+        zds = dataset.Dataset.from_xarray(xds)
+        if not delayed:
+            zds = zds.compute()
 
-        for partition, indexer in iterator:
-            subset = ds.isel(indexer)
-
-            # Cast the date to the a datetime object to extract the date
-            item = date.astype('datetime64[us]').item()
-            expected = (
-                f'year={item.year}',
-                f'month={item.month:02d}',
-                f'day={item.day:02d}',
-                f'hour={item.hour:02d}',
-            )
-            assert partition == expected[indices]
-
-            folder = '/'.join(partition)
-            fields = partitioning.parse(folder)
-            parsed_date, = partitioning.encode(fields)
-            assert parsed_date == numpy.datetime64(date).astype(
-                f'datetime64[{resolution}]')
-
-            expected_selection = dates[
-                (dates >= parsed_date)  # type: ignore
-                & (dates < parsed_date + timedelta)]  # type: ignore
-            computed_selection = subset.variables['dates'].compute(
-                scheduler=dask.local.get_sync)
-            assert numpy.all(computed_selection == expected_selection)
-
-            expected = (
-                ('year', item.year),
-                ('month', item.month),
-                ('day', item.day),
-                ('hour', item.hour),
-            )
-            assert fields == expected[indices]
-            assert partitioning.join(fields, '/') == folder
-            assert partitioning.join(partitioning.decode((parsed_date, )),
-                                     '/') == folder
+        checker = PartitionTestData(timedelta, indices, resolution,
+                                    partitioning, dates)
 
+        for partition, indexer in partitioning.split_dataset(zds, 'num_lines'):
+            checker.check_partitioning(date, zds.isel(indexer), partition)
             date += timedelta
 
 
-def test_construction():
+def test_construction() -> None:
     """Test the construction of the Date class."""
     partitioning = Date(('dates', ), 'D')
     assert partitioning.resolution == 'D'
     assert partitioning.variables == ('dates', )
     assert partitioning.dtype() == (('year', 'uint16'), ('month', 'uint8'),
                                     ('day', 'uint8'))
     assert len(partitioning) == 3
@@ -159,42 +179,49 @@
     partitioning = Date(('dates', ), 'D')
     other = pickle.loads(pickle.dumps(partitioning))
     assert isinstance(other, Date)
     assert other.resolution == 'D'
     assert other.variables == ('dates', )
 
 
+@pytest.mark.parametrize('delayed', [False, True])
 def test_no_monotonic(
-        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+    dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+    delayed: bool,
 ):
     """Test that the Date partitioning raises an error if the temporal axis is
     not monotonic."""
-    dates = numpy.arange(numpy.datetime64('2000-01-01', 'h'),
-                         numpy.datetime64('2000-01-02', 'h'),
-                         numpy.timedelta64(1, 'm'))
+    dates: numpy.ndarray = numpy.arange(numpy.datetime64('2000-01-01', 'h'),
+                                        numpy.datetime64('2000-01-02', 'h'),
+                                        numpy.timedelta64(1, 'm'))
     numpy.random.shuffle(dates)
     partitioning = Date(('dates', ), 'h')
     # pylint: disable=protected-access
     with pytest.raises(ValueError):
-        list(partitioning._split({'dates': dask.array.core.from_array(dates)}))
+        arr = dask.array.core.from_array(dates) if delayed else dates
+        list(partitioning._split({'dates': arr}))  # type: ignore[arg-type]
     # pylint: enable=protected-access
 
 
 def test_values_must_be_datetime64(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
 ):
     """Test that the values must be datetime64."""
     dates = numpy.arange(numpy.datetime64('2000-01-01', 'h'),
                          numpy.datetime64('2000-01-02', 'h'),
                          numpy.timedelta64(1, 'm'))
     partitioning = Date(('dates', ), 'h')
     dates = dates.astype('int64')
     with pytest.raises(TypeError):
         # pylint: disable=protected-access
-        list(partitioning._split({'dates': dask.array.core.from_array(dates)}))
+        list(
+            partitioning._split({
+                'dates':
+                dask.array.core.from_array(dates)  # type: ignore[arg-type]
+            }))
     # pylint: enable=protected-access
 
 
 @pytest.mark.parametrize(
     'start, end, step, path_generator',
     [(('2000-01-01', 'D'), ('2000-02-01', 'D'), (1, 'D'), lambda item:
       (f'year={item.year}', f'month={item.month:02d}', f'day={item.day:02d}')),
```

### Comparing `zcollection-2023.3.2/zcollection/partitioning/tests/test_registry.py` & `zcollection-2023.5.0/zcollection/partitioning/tests/test_registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
 Test the registry module.
 =========================
 """
+from typing import Any
+
 import pytest
 
 from .. import registry
 
 
-def test_get_codecs():
+def test_get_codecs() -> None:
     """Test the get_codecs function."""
     with pytest.raises(ValueError):
         registry.get_codecs({'ID': 'foo'})
 
     with pytest.raises(ValueError):
         registry.get_codecs({'id': 'foo'})
 
@@ -23,31 +25,33 @@
 class MyCodec:
     """A dummy codec."""
     ID = 'foo'
 
     __slots__ = ('attribute', )
 
     def __init__(self, attribute) -> None:
-        self.attribute = attribute
+        self.attribute: Any = attribute
 
     def get_config(self) -> dict:
         """Returns the configuration of the codec."""
         return {'id': self.ID, 'attribute': self.attribute}
 
     @classmethod
     def from_config(cls, config: dict) -> 'MyCodec':
         """Creates an instance from the given configuration."""
         return cls(config['attribute'])
 
 
-def test_register_codec():
+def test_register_codec() -> None:
     """Test the register_codec function."""
-    registry.register_codec(MyCodec, 'foo')
+    registry.register_codec(MyCodec, codec_id='foo')  # type: ignore[arg-type]
 
     instance = MyCodec(12)
 
     other = registry.get_codecs(instance.get_config())
     assert other.attribute == instance.attribute  # type: ignore
     assert isinstance(other, MyCodec)
 
     with pytest.raises(ValueError):
-        registry.register_codec(MyCodec, 'foo')
+        registry.register_codec(
+            MyCodec,  # type: ignore[arg-type]
+            codec_id='foo')
```

### Comparing `zcollection-2023.3.2/zcollection/partitioning/tests/test_sequence.py` & `zcollection-2023.5.0/zcollection/partitioning/tests/test_sequence.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,181 +12,193 @@
 import pickle
 
 import dask.array.core
 import numpy
 import pytest
 import xarray
 
+from zcollection.type_hints import ArrayLike
+
 from . import data
 from .. import Sequence, get_codecs
 from ... import dataset
 # pylint: disable=unused-import # Need to import for fixtures
 from ...tests.cluster import dask_client, dask_cluster
 
 # pylint: enable=unused-import # Need to import for fixtures
 
 
-def test_construction():
+def test_construction() -> None:
     """Test the sequence constructor."""
     assert isinstance(Sequence(('a', 'b')), Sequence)
     assert len(Sequence(('a', 'b'))) == 2
     with pytest.raises(ValueError):
         Sequence(('a', 'b'), (0, ))  # type: ignore
     with pytest.raises(ValueError):
         Sequence((), ())
     with pytest.raises(ValueError):
         Sequence(('a', 'b'), dtype=('c', 'd'))
     with pytest.raises(ValueError):
         Sequence(('a', 'b'), dtype=('float32', 'int32'))
     with pytest.raises(TypeError):
-        Sequence(('a', 'b'), dtype=('int32'))
+        Sequence(('a', 'b'), dtype='int32')
     partitioning = Sequence(('a', 'b'))
     partition_keys = partitioning.parse('a=1/b=2')
     assert partitioning.encode(partition_keys) == (1, 2)
     with pytest.raises(ValueError):
         partitioning.encode((('A', 1), ('b', 2)))
     assert partitioning.decode((1, 2)) == (('a', 1), ('b', 2))
     assert partition_keys == (('a', 1), ('b', 2))
     with pytest.raises(ValueError):
         partitioning.parse('a=1/b=2/c=3')
     with pytest.raises(ValueError):
         partitioning.parse('field=1')
 
 
+@pytest.mark.parametrize('delayed', [False, True])
 def test_split_dataset(
-        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+    dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+    delayed: bool,
+) -> None:
     """Test the split_dataset method."""
     repeatability = 5
-    xr_ds = data.create_test_sequence(repeatability, 20, 10)
+    xds = data.create_test_sequence(repeatability, 20, 10)
     partitioning = Sequence(('cycle_number', 'pass_number'))
 
     cycle_number = 1
     pass_number = 1
 
     assert partitioning.dtype() == (
         ('cycle_number', 'int64'),
         ('pass_number', 'int64'),
     )
 
     # Build the test dataset
-    ds = dataset.Dataset.from_xarray(xr_ds)
+    zds = dataset.Dataset.from_xarray(xds)
+    if not delayed:
+        zds = zds.compute()
 
-    iterator = partitioning.split_dataset(ds, 'num_lines')
+    iterator = partitioning.split_dataset(zds, 'num_lines')
     assert isinstance(iterator, Iterator)
 
     for partition, indexer in iterator:
-        subset = ds.isel(indexer)
+        subset = zds.isel(indexer)
         expected = (f'cycle_number={cycle_number}',
                     f'pass_number={pass_number}')
         assert expected == partition
         assert numpy.all(
-            xr_ds.where((xr_ds.cycle_number == cycle_number)
-                        & (xr_ds.pass_number == pass_number),
-                        drop=True).observation ==
+            xds.where((xds.cycle_number == cycle_number)
+                      & (xds.pass_number == pass_number),
+                      drop=True).observation ==
             subset.variables['observation'].array)
 
         partition_keys = partitioning.parse('/'.join(partition))
         assert partition_keys == (('cycle_number', cycle_number),
                                   ('pass_number', pass_number))
         assert partitioning.decode(
             partitioning.encode(partition_keys)) == partition_keys
         assert partitioning.join(partition_keys, '/') == '/'.join(partition)
 
         pass_number += 1
         if pass_number > repeatability:
             pass_number = 1
             cycle_number += 1
 
-    xr_ds['cycle_number'] = xarray.DataArray(numpy.array(
-        [xr_ds['cycle_number'].values] * 2).T,
-                                             dims=('num_lines', 'nump_pixels'))
-    ds = dataset.Dataset.from_xarray(xr_ds)
+    xds['cycle_number'] = xarray.DataArray(numpy.array(
+        [xds['cycle_number'].values] * 2).T,
+                                           dims=('num_lines', 'nump_pixels'))
+    zds = dataset.Dataset.from_xarray(xds)
+    if not delayed:
+        zds = zds.compute()
     with pytest.raises(ValueError):
-        list(partitioning.split_dataset(ds, 'num_lines'))
+        list(partitioning.split_dataset(zds, 'num_lines'))
 
 
-def test_config():
+def test_config() -> None:
     """Test the configuration of the Sequence class."""
     partitioning = Sequence(('cycle_number', 'pass_number'))
     config = partitioning.get_config()
-    partitioning = get_codecs(config)
+    partitioning = get_codecs(config)  # type: ignore[assignment]
     assert isinstance(partitioning, Sequence)
 
 
-def test_pickle():
+def test_pickle() -> None:
     """Test the pickling of the Date class."""
     partitioning = Sequence(('cycle_number', 'pass_number'))
     other = pickle.loads(pickle.dumps(partitioning))
     assert isinstance(other, Sequence)
     assert other.variables == ('cycle_number', 'pass_number')
 
 
 # pylint: disable=protected-access
+@pytest.mark.parametrize('delayed', [False, True])
 def test_multiple_sequence(
-        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+    dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+    delayed: bool,
+) -> None:
     """Test the creation of a sequence with multiple variables."""
-    arrays = dict(_a=numpy.array([], dtype='i8'),
-                  _b=numpy.array([], dtype='i8'),
-                  _c=numpy.array([], dtype='i8'))
+    arrays = {
+        '_a': numpy.array([], dtype='i8'),
+        '_b': numpy.array([], dtype='i8'),
+        '_c': numpy.array([], dtype='i8')
+    }
     for _a in range(5):
         for _b in range(5):
             arrays['_a'] = numpy.concatenate(
                 (arrays['_a'], numpy.full((5, ), _a, dtype='i8')))
             arrays['_b'] = numpy.concatenate(
                 (arrays['_b'], numpy.full((5, ), _b, dtype='i8')))
             arrays['_c'] = numpy.concatenate(
                 (arrays['_c'], numpy.arange(5, dtype='i8')))
     partitioning = Sequence(('_a', '_b', '_c'))
-    variables: dict[str, dask.array.core.Array] = dict(
-        _a=dask.array.core.from_array(arrays['_a'],
-                                      chunks=(10, )),  # type: ignore[arg-type]
-        _b=dask.array.core.from_array(arrays['_b'],
-                                      chunks=(10, )),  # type: ignore[arg-type]
-        _c=dask.array.core.from_array(arrays['_c'],
-                                      chunks=(10, )))  # type: ignore[arg-type]
+    chunks: str = (10, )  # type: ignore[assignment]
+    if delayed:
+        variables: dict[str, ArrayLike] = {  # type: ignore[assignment]
+            '_a': dask.array.core.from_array(arrays['_a'], chunks=chunks),
+            '_b': dask.array.core.from_array(arrays['_b'], chunks=chunks),
+            '_c': dask.array.core.from_array(arrays['_c'], chunks=chunks)
+        }
+    else:
+        variables = arrays  # type: ignore[assignment]
     _a = 0
     _b = 0
     _c = 0
-    for ix, item in enumerate(partitioning._split(variables)):
+    for idx, item in enumerate(
+            partitioning._split(variables)):  # type: ignore[arg-type]
         assert item[0] == (('_a', _a), ('_b', _b), ('_c', _c))
         _c += 1
         if _c > 4:
             _c = 0
             _b += 1
         if _b > 4:
             _b = 0
             _a += 1
-        assert item[1] == slice(ix, ix + 1)
+        assert item[1] == slice(idx, idx + 1)
 
     numpy.random.shuffle(arrays['_c'])
-    variables['_c'] = dask.array.core.from_array(arrays['_c'],
-                                                 chunks=(10, ))  # type: ignore
+    variables['_c'] = dask.array.core.from_array(  # type: ignore[assignment]
+        arrays['_c'], chunks=chunks) if delayed else arrays['_c']
 
     with pytest.raises(ValueError):
-        list(partitioning._split(variables))
+        list(partitioning._split(variables))  # type: ignore[arg-type]
 
     del variables['_c']
     del variables['_b']
     partitioning = Sequence(('_a', '_b', '_c'))
 
     _a = 0
-    for ix, item in enumerate(partitioning._split(variables)):
+    for idx, item in enumerate(
+            partitioning._split(variables)):  # type: ignore[arg-type]
         assert item[0] == (('_a', _a), )
         _a += 1
-        assert item[1] == slice(ix * 25, ix * 25 + 25)
+        assert item[1] == slice(idx * 25, idx * 25 + 25)
     # pylint: enable=protected-access
 
 
-def test_values_must_be_integer(
-        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+def test_values_must_be_integer() -> None:
     """Test that the values must be integer."""
     values = numpy.arange(0, 100, dtype='f8')
     partitioning = Sequence(('values', ))
     # pylint: disable=protected-access
     with pytest.raises(TypeError):
-        list(
-            partitioning._split({'values':
-                                 dask.array.core.from_array(values)}))
+        list(partitioning._split({'values': values}))
     # pylint: enable=protected-access
```

### Comparing `zcollection-2023.3.2/zcollection/storage.py` & `zcollection-2023.5.0/zcollection/storage.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 import dask.array.core
 import dask.base
 from dask.delayed import Delayed as dask_Delayed
 import dask.distributed
 import dask.local
 import fsspec
+import numcodecs.abc
+import numcodecs.blosc
 import numpy
 import zarr
 
 from . import dataset, meta, sync
 from .fs_utils import join_path
 from .type_hints import ArrayLike
 
@@ -32,61 +34,71 @@
 #: Configuration file that describes the attributes of an array.
 ZATTRS = '.zattrs'
 
 #: Configuration file that describes the attributes of a group.
 ZGROUP = '.zgroup'
 
 #: Module logger.
-_LOGGER = logging.getLogger(__name__)
+_LOGGER: logging.Logger = logging.getLogger(__name__)
+
+#: Disable multithreading in Blosc to avoid competing with Dask.
+numcodecs.blosc.use_threads = False
 
 
 def execute_transaction(
     client: dask.distributed.Client,
     synchronizer: sync.Sync,
     futures: Sequence[dask.distributed.Future | dask_Delayed],
     **kwargs: Any,
 ) -> Any:
     """Execute a transaction in the collection.
 
+    This function executes a transaction in the collection by computing the
+    given futures using the provided Dask client. The synchronizer instance is
+    used to handle access to critical resources. Any additional keyword
+    arguments are passed to the `dask.distributed.compute` function.
+
     Args:
         client: The Dask client.
         synchronizer: The instance handling access to critical resources.
         futures: Lazy tasks to be done.
-        kwargs: Keyword arguments to pass to :func:`dask.distributed.compute`.
+        **kwargs: Keyword arguments to pass to `dask.distributed.compute`.
 
     Returns:
         The result of the transaction.
     """
     if not futures:
         return None
-    awaitables = []
+    awaitables: Iterable[Any] = []
     try:
         with synchronizer:
-            awaitables = client.compute(futures, **kwargs)
+            awaitables = client.compute(futures,
+                                        **kwargs)  # type: ignore[arg-type]
             return client.gather(awaitables)
     except:  # noqa: E722
         # Before throwing the exception, we wait until all future scheduled
         # ones finished.
         dask.distributed.wait(awaitables)
         dask.distributed.wait(futures)
         raise
 
 
 def _to_zarr(array: dask.array.core.Array, mapper: fsspec.FSMap, path: str,
              **kwargs) -> None:
     """Write a Dask array to a Zarr dataset.
 
     Args:
-        array: The array to write.
+        array: The Dask array to write.
         mapper: The file system mapper.
         path: The path to the Zarr dataset.
-        **kwargs: Keyword arguments to pass to :func:`zarr.create`.
+        **kwargs: Additional keyword arguments to pass to the `zarr.create`
+            function.
     """
-    chunks = [chunk[0] for chunk in array.chunks]
-    target = zarr.create(
+    chunks: list[tuple[int, ...]] = [chunk[0] for chunk in array.chunks]
+    target: dask.array.core.Array = zarr.create(
         shape=array.shape,
         chunks=chunks,  # type: ignore[arg-type]
         dtype=array.dtype,
         store=mapper,
         path=path,
         overwrite=True,
         write_empty_chunks=False,
@@ -120,31 +132,40 @@
         json.dump(attrs, stream, indent=2)  # type: ignore[arg-type]
 
 
 def write_zarr_variable(
     args: tuple[str, dataset.Variable],
     dirname: str,
     fs: fsspec.AbstractFileSystem,
-    chunks: dict[str, int | str] | None = None,
+    *,
     block_size_limit: int | None = None,
+    chunks: dict[str, int | str] | None = None,
 ) -> None:
     """Write a variable to a Zarr dataset.
 
     Args:
         args: The arguments to the function:
             - Name of the variable to write.
             - The variable to write.
         dirname: The target directory.
         fs: The file system on which the Zarr dataset is stored.
-        chunks: Chunk size for each dimension.
-        block_size_limit: Maximum size (in bytes) of a block/chunk.
-    """
+        block_size_limit: Maximum size (in bytes) of a block/chunk. Defaults
+            to :data:`zcollection.meta.BLOCK_SIZE_LIMIT`.
+        chunks: Chunk size for each dimension. Defaults to ``None`` (i.e. the
+            default chunk size is used).
+    """
+    name: str
+    variable: dataset.Variable
+    kwargs: dict[str, tuple[numcodecs.abc.Codec, ...]]
+
     name, variable = args
     kwargs = {'filters': variable.filters}
-    data = variable.array
+    data: dask.array.core.Array = variable.array if isinstance(
+        variable, dataset.DelayedArray) else dask.array.core.from_array(
+            variable.array)
 
     # If the user has not specified a chunk size, we use the default one.
     # Otherwise, we use the user's choice.
     block_size_limit = block_size_limit or meta.BLOCK_SIZE_LIMIT
     var_chunks: dict[int, int | str] = {
         ix: -1
         for ix in range(variable.ndim)
@@ -163,134 +184,183 @@
              compressor=variable.compressor,
              fill_value=variable.fill_value,
              **kwargs)
     write_zattrs(dirname, variable, fs)
 
 
 def _write_meta(
-    ds: dataset.Dataset,
+    zds: dataset.Dataset,
     dirname: str,
     fs: fsspec.AbstractFileSystem,
 ) -> None:
     """Write the metadata of a dataset to a Zarr dataset.
 
     Args:
-        ds: The dataset to process.
+        zds: The dataset to process.
         dirname: The storage directory of the Zarr dataset.
         fs: The file system on which the Zarr dataset is stored.
     """
-    attrs = collections.OrderedDict(item.get_config() for item in ds.attrs)
+    attrs = collections.OrderedDict(item.get_config() for item in zds.attrs)
     with fs.open(join_path(dirname, ZATTRS), mode='w') as stream:
         json.dump(attrs, stream, indent=2)  # type: ignore[arg-type]
 
     with fs.open(join_path(dirname, ZGROUP), mode='w') as stream:
         json.dump(
             {'zarr_format': 2},
             stream,  # type: ignore[arg-type]
             indent=2,
         )
     zarr.consolidate_metadata(fs.get_mapper(dirname))  # type: ignore[arg-type]
     fs.invalidate_cache(dirname)
 
 
 def write_zarr_group(
-    ds: dataset.Dataset,
+    zds: dataset.Dataset,
     dirname: str,
     fs: fsspec.AbstractFileSystem,
     synchronizer: sync.Sync,
-    parallel: bool = True,
+    *,
+    distributed: bool = True,
 ) -> None:
-    """Write a partition to a Zarr group.
+    """Write a partition of a dataset to a Zarr group.
 
     Args:
-        ds: The dataset to write.
+        zds: The dataset partition to write.
         dirname: The name of the partition.
         fs: The file system that the partition is stored on.
         synchronizer: The instance handling access to critical resources.
-        parallel: Whether to write the variables in parallel using Dask.
-    """
-    if parallel:
-        with dask.distributed.worker_client() as client:
-            iterables = [(name, client.scatter(variable))
-                         for name, variable in ds.variables.items()]
-            futures = client.map(write_zarr_variable,
-                                 iterables,
-                                 dirname=dirname,
-                                 fs=fs,
-                                 chunks=ds.chunks,
-                                 block_size_limit=ds.block_size_limit)
-            execute_transaction(client, synchronizer, futures)
-    else:
-        for name, variable in ds.variables.items():
-            write_zarr_variable((name, variable),
-                                dirname,
-                                fs,
-                                chunks=ds.chunks,
-                                block_size_limit=ds.block_size_limit)
-    _write_meta(ds, dirname, fs)
+        distributed: Whether to use Dask distributed to write the variables
+            in parallel. Defaults to ``True``.
+
+    Writes the variables of the given dataset partition to a Zarr group
+    located at the specified directory on the given file system. If
+    `distributed` is `True`, the variables are written in parallel using
+    Dask distributed. Otherwise, the variables are written sequentially.
+
+    The `synchronizer` argument is an instance of `sync.Sync` that handles
+    access to critical resources, such as the Zarr group's metadata and
+    attributes. This ensures that multiple processes or threads do not
+    attempt to modify the same resource at the same time.
+    """
+    with synchronizer:
+        if distributed:
+            with dask.distributed.worker_client() as client:
+                iterables: list[tuple[str, Any]] = [
+                    (name, client.scatter(variable))
+                    for name, variable in zds.variables.items()
+                ]
+                futures: list[dask.distributed.Future] = client.map(
+                    write_zarr_variable,
+                    iterables,
+                    block_size_limit=zds.block_size_limit,
+                    chunks=zds.chunks,
+                    dirname=dirname,
+                    fs=fs,
+                )
+                execute_transaction(
+                    client,
+                    sync.NoSync(),
+                    futures,
+                    workers=dask.distributed.get_worker().address)
+        else:
+            tuple(
+                map(
+                    lambda item: write_zarr_variable(
+                        item,
+                        dirname,
+                        fs,
+                        chunks=zds.chunks,
+                        block_size_limit=zds.block_size_limit,
+                    ), zds.variables.items()))
+        _write_meta(zds, dirname, fs)
 
 
-def open_zarr_array(array: zarr.Array, name: str) -> dataset.Variable:
-    """Open a Zarr array as a Dask array.
+def open_zarr_array(
+    array: zarr.Array,
+    name: str,
+    *,
+    delayed: bool = True,
+) -> dataset.Variable:
+    """Open a Zarr array as a Dask array or a NumPy array.
 
     Args:
         array: The Zarr array to open.
         name: The name of the variable.
+        delayed: Whether to load the variable lazily. If True, returns a Dask
+            array. If False, returns a NumPy array. Defaults to True.
 
     Returns:
-        The variable.
+        The variable as a Dask array or a NumPy array.
     """
-    return dataset.Variable.from_zarr(array, name, DIMENSIONS)
+    if delayed:
+        return dataset.DelayedArray.from_zarr(array, name, DIMENSIONS)
+    return dataset.Array.from_zarr(array, name, DIMENSIONS)
 
 
 def open_zarr_group(
-        dirname,
-        fs: fsspec.AbstractFileSystem,
-        selected_variables: Iterable[str] | None = None) -> dataset.Dataset:
+    dirname,
+    fs: fsspec.AbstractFileSystem,
+    *,
+    delayed: bool = True,
+    selected_variables: Iterable[str] | None = None,
+) -> dataset.Dataset:
     """Open a Zarr group stored in a partition.
 
     Args:
         dirname: The name of the partition.
         fs: The file system that the partition is stored on.
+        delayed: Whether to load the variables lazily. Defaults to True.
         selected_variables: The list of variables to retain from the Zarr
-            group. If None, all variables are selected.
+            group. If None, all variables are selected. Defaults to None.
 
     Returns:
-        The zarr group stored in the partition.
+        The Zarr group stored in the partition, with the specified variables
+        and attributes.
     """
     _LOGGER.debug('Opening Zarr group %r', dirname)
     store: zarr.Group = zarr.open_consolidated(  # type: ignore[arg-type]
         fs.get_mapper(dirname), mode='r')
     # Ignore unknown variables to retain.
     selected_variables = set(selected_variables) & set(
         store) if selected_variables is not None else set(store)
-    variables = [
-        open_zarr_array(store[name], name)  # type: ignore[arg-type]
-        for name in selected_variables
+    variables: list[dataset.Variable] = [
+        open_zarr_array(
+            store[name],  # type: ignore[arg-type]
+            name,
+            delayed=delayed) for name in selected_variables
     ]
 
     return dataset.Dataset(
         variables=variables,
-        attrs=tuple(dataset.Attribute(*item) for item in store.attrs.items()))
+        attrs=tuple(dataset.Attribute(*item) for item in store.attrs.items()),
+        delayed=delayed,
+    )
 
 
 def update_zarr_array(
     dirname: str,
     array: ArrayLike,
     fs: fsspec.AbstractFileSystem,
 ) -> None:
-    """Update a Zarr array.
+    """Update a Zarr array with new data.
 
     Args:
-        dirname: The storage directory of the Zarr array..
-        array: The data updated to write.
-        fs: The file system that the Zarr array is stored on.
+        dirname: The directory where the Zarr array is stored.
+        array: The new data to write to the array.
+        fs: The file system where the Zarr array is stored.
+
+    Notes:
+        This function updates the entire Zarr array with the new data. If the
+        array is a Dask array, it must be computed before writing to the Zarr.
+        If the array is a masked array and the Zarr array has a fill value, the
+        masked values are filled with the fill value before writing to the Zarr
+        array.
     """
     _LOGGER.debug('Updating Zarr array %r', dirname)
-    store = zarr.open_array(fs.get_mapper(dirname), mode='a')
+    store: zarr.Array = zarr.open_array(fs.get_mapper(dirname), mode='a')
 
     if isinstance(array, dask.array.core.Array):
         array = array.compute()
 
     if isinstance(array,
                   numpy.ma.MaskedArray) and store.fill_value is not None:
         array = array.filled(store.fill_value)
@@ -310,52 +380,62 @@
 
     Args:
         dirname: The name of the dataset.
         name: The name of the variable.
         fs: The file system that the dataset is stored on.
     """
     _LOGGER.debug('Deleting Zarr array %r', dirname)
-    path = join_path(dirname, name)
+    path: str = join_path(dirname, name)
     if fs.exists(path):
         fs.rm(path, recursive=True)
         zarr.consolidate_metadata(
             fs.get_mapper(dirname),  # type: ignore[arg-type]
         )
         # Invalidate any cached directory information.
         fs.invalidate_cache(dirname)
 
 
 def add_zarr_array(
     dirname: str,
     variable: meta.Variable,
     template: str,
     fs: fsspec.AbstractFileSystem,
+    *,
     chunks: dict[str, int | str] | None = None,
 ) -> None:
     """Add a variable to a Zarr dataset.
 
     Args:
         dirname: The name of the dataset.
         variable: The variable to add.
         template: The name of the template variable.
         fs: The file system that the dataset is stored on.
-        chunks: Chunk size for each dimension.
+        chunks: Chunk size for each dimension. Defaults to None. See
+            :func:`zarr.create` for more information.
+
+    Notes:
+        This function adds a new variable to an existing Zarr dataset. The new
+        variable is created with the same shape as the template variable, and
+        with the specified chunk size (if provided). The function also writes
+        the variable's attributes to the dataset, and consolidates the
+        dataset's metadata.
     """
     _LOGGER.debug('Adding variable %r to Zarr dataset %r', variable.name,
                   dirname)
-    shape = zarr.open(fs.get_mapper(join_path(dirname, template))).shape
+    shape: tuple[int, ...] = zarr.open(  # type: ignore[arg-type]
+        fs.get_mapper(join_path(dirname, template))).shape
 
-    var_chunks = shape if chunks is None else tuple(
-        chunks.get(dim, shape[ix])
+    var_chunks: tuple[int | str, ...] = shape if chunks is None else tuple(
+        chunks.get(dim, shape[ix])  # type: ignore[misc]
         for ix, dim in enumerate(variable.dimensions))
 
-    store = fs.get_mapper(join_path(dirname, variable.name))
+    store: fsspec.FSMap = fs.get_mapper(join_path(dirname, variable.name))
     zarr.create(
         shape,
-        chunks=var_chunks,
+        chunks=var_chunks,  # type: ignore[arg-type]
         dtype=variable.dtype,
         compressor=variable.compressor,  # type: ignore[arg-type]
         fill_value=variable.fill_value,  # type: ignore[arg-type]
         store=store,
         filters=variable.filters)
     write_zattrs(dirname, variable, fs)
     zarr.consolidate_metadata(fs.get_mapper(dirname))  # type: ignore[arg-type]
```

### Comparing `zcollection-2023.3.2/zcollection/sync.py` & `zcollection-2023.5.0/zcollection/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return False
 
 
 class ProcessSync(Sync):
     """This class is used when the user wants to synchronize accesses to the
     collection, in other words, when there is concurrency."""
 
-    def __init__(self, path: str):
+    def __init__(self, path: str) -> None:
         self.lock = fasteners.InterProcessLock(path)
 
     def __enter__(self) -> bool:
         return self.lock.acquire()
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         try:
```

### Comparing `zcollection-2023.3.2/zcollection/tests/cluster.py` & `zcollection-2023.5.0/zcollection/tests/cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 # Copyright (c) 2023 CNES
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
+"""
+Fixtures for testing Dask clusters using the pytest.
+====================================================
+"""
+from typing import Iterator
 import contextlib
 import logging
 import weakref
 
 import dask.config
 import dask.distributed
+import py
 import pytest
 
 
 @pytest.fixture()
-def dask_cluster(pytestconfig, tmpdir_factory, scope='session'):
+def dask_cluster(
+        pytestconfig,
+        tmpdir_factory,
+        scope='session',  # pylint: disable=unused-argument
+) -> str:
     """Launch a Dask LocalCluster with a configurable number of workers."""
+    n_workers: int | None
+    threads_per_worker: int | None
+    processes: bool
+
     try:
         n_workers = int(pytestconfig.getoption('n_workers'))
     except TypeError:
         n_workers = None
 
     try:
         threads_per_worker = int(pytestconfig.getoption('threads_per_worker'))
@@ -25,34 +39,33 @@
         threads_per_worker = None
 
     try:
         processes = int(pytestconfig.getoption('processes')) == 1
     except TypeError:
         processes = False
 
-    tmpdir = tmpdir_factory.getbasetemp()
-    scheduler_file = tmpdir / 'scheduler.json'
+    tmpdir: py.path.local = tmpdir_factory.getbasetemp()
+    scheduler_file: py.path.local = tmpdir / 'scheduler.json'
     if scheduler_file.exists():
         return str(scheduler_file)
 
     # Use the root path of the test session for the dask worker space
-    dask_worker = tmpdir / 'dask_worker_space'
+    dask_worker: py.path.local = tmpdir / 'dask_worker_space'
     dask.config.set(temporary_directory=str(dask_worker))
 
     logging.info('Dask local cluster starting')
     cluster = dask.distributed.LocalCluster(
         protocol='tcp://',
         n_workers=n_workers,
         threads_per_worker=threads_per_worker,
         processes=processes,
     )
 
-    def teardown():
+    def teardown() -> None:
         """Stop the cluster and remove the scheduler file."""
-        cluster.close()
         if scheduler_file.exists():
             scheduler_file.remove()
 
     weakref.finalize(cluster, teardown)
 
     # Make sure we can connect to the cluster.
     with dask.distributed.Client(cluster) as client:
@@ -60,18 +73,22 @@
         client.wait_for_workers(1)
 
     logging.info('Dask local cluster started')
     return str(scheduler_file)
 
 
 @contextlib.contextmanager
-def _scheduler_file(dask_cluster):
+def _scheduler_file(
+        dask_cluster,  # pylint: disable=redefined-outer-name
+) -> Iterator[str]:
     """Get the scheduler used to connect to the cluster."""
     yield dask_cluster
 
 
 @pytest.fixture()
-def dask_client(dask_cluster):
+def dask_client(
+    dask_cluster,  # pylint: disable=redefined-outer-name
+) -> Iterator[dask.distributed.Client]:
     """Connect a Dask client to the cluster."""
     with _scheduler_file(dask_cluster) as scheduler_file:
         with dask.distributed.Client(scheduler_file=scheduler_file) as client:
             yield client
```

### Comparing `zcollection-2023.3.2/zcollection/tests/first_dataset.json` & `zcollection-2023.5.0/zcollection/tests/first_dataset.json`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/zcollection/tests/fs.py` & `zcollection-2023.5.0/zcollection/tests/fs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
 Fixture for testing the file system.
 ====================================
 """
+from typing import Any, Iterator
 import pathlib
 
 import fsspec
 import fsspec.implementations.memory
 import pytest
 
 try:
@@ -22,27 +23,31 @@
     S3_IMPORT_EXCEPTION = str(err)
 
 
 class Local:
     """Local files system."""
 
     def __init__(self, tmpdir, protocol) -> None:
-        self.fs = fsspec.filesystem(protocol)
+        #: The filesystem.
+        self.fs: fsspec.AbstractFileSystem = fsspec.filesystem(protocol)
+        #: The root directory.
         self.root = pathlib.Path(tmpdir)
-        self.collection = self.root.joinpath('collection')
-        self.view = self.root.joinpath('view')
+        #: The collection directory.
+        self.collection: pathlib.Path = self.root.joinpath('collection')
+        #: The view directory.
+        self.view: pathlib.Path = self.root.joinpath('view')
 
-    def __getattr__(self, name):
+    def __getattr__(self, name) -> Any:
         return getattr(self.fs, name)
 
 
 @pytest.fixture
-def local_fs(tmpdir, pytestconfig):
+def local_fs(tmpdir, pytestconfig) -> Iterator[Local]:
     """Local filesystem."""
-    protocol = 'memory' if pytestconfig.getoption('memory') else 'file'
+    protocol: str = 'memory' if pytestconfig.getoption('memory') else 'file'
     instance = Local(tmpdir, protocol)
     yield instance
     try:
         # For the memory protocol we delete the written data to free the
         # memory.
         if isinstance(instance.fs,
                       fsspec.implementations.memory.MemoryFileSystem):
@@ -51,31 +56,29 @@
         pass
 
 
 # pylint: disable=redefined-outer-name,function-redefined
 if S3_IMPORT_EXCEPTION is None:
 
     @pytest.fixture
-    def s3_fs(s3):  # type: ignore[arg-type]
+    def s3_fs(s3) -> S3:  # type: ignore[arg-type]
         """S3 filesystem."""
-        return S3(s3)
+        return S3(s3)  # type: ignore
 else:
 
     @pytest.fixture
-    def s3():
+    def s3() -> None:
         """S3 filesystem."""
-        ...
 
     @pytest.fixture
-    def s3_base():
+    def s3_base() -> None:
         """S3 filesystem."""
-        ...
 
     @pytest.fixture
-    def s3_fs(pytestconfig):
+    def s3_fs(pytestconfig) -> None:
         """S3 filesystem."""
         if pytestconfig.getoption('s3'):
             pytest.fail(f'Unable to test S3: {S3_IMPORT_EXCEPTION}')
         else:
             pytest.skip('S3 is disabled')
```

### Comparing `zcollection-2023.3.2/zcollection/tests/s3.py` & `zcollection-2023.5.0/zcollection/tests/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) 2023 CNES
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
-Support to test with minio
-==========================
+Fixtures for testing S3 using the pytest and minio.
+===================================================
 """
+from typing import Iterator, Literal
 import os
 import pathlib
 import shlex
 import subprocess
 import time
 
 import botocore.client
@@ -17,95 +18,99 @@
 import pytest
 import requests
 import s3fs
 
 #: Listen port
 PORT = 5555
 #: Listen address
-ENDPOINT = f'127.0.0.1:{PORT}'
+ENDPOINT: str = f'127.0.0.1:{PORT}'
 #: URI for minio
-ENDPOINT_URI = f'http://{ENDPOINT}'
+ENDPOINT_URI: str = f'http://{ENDPOINT}'
 #: Credential for minio
 CREDENTIAL = '25219d58-f6c6-11eb-922c-770d49cd18e4'
 
 
-def have_minio():
+def have_minio() -> Literal[True]:
     """Check if minio is available."""
     try:
         subprocess.check_output(['minio', '--version'])
         return True
     except:
         raise ImportError('minio: command not found') from None
 
 
 have_minio()
 
 
+def is_minio_up(timeout: float) -> bool:
+    """Check if minio server is up."""
+    try:
+        response = requests.get(ENDPOINT_URI, timeout=timeout)
+        if response.status_code == 403:
+            return True
+    except:  # pylint: disable=bare-except
+        pass
+    return False
+
+
+def wait_for_minio_to_start(timeout: float) -> None:
+    """Wait for the minio server to start."""
+    while timeout > 0:
+        try:
+            response = requests.get(ENDPOINT_URI, timeout=1)
+            if response.status_code == 403:
+                return
+        except:  # pylint: disable=bare-except
+            pass
+        timeout -= 0.1
+        time.sleep(0.1)
+    raise RuntimeError("minio server didn't start")
+
+
 @pytest.fixture()
-def s3_base(tmpdir, pytestconfig):
+def s3_base(tmpdir, pytestconfig) -> Iterator[None]:
     """Launch minio server."""
     if pytestconfig.getoption('s3') is False:
         pytest.skip('S3 disabled')
-    try:
-        # should fail since we didn't start server yet
-        response = requests.get(ENDPOINT_URI)
-    # pylint: disable=bare-except
-    except:
-        pass
-    # pylint: enable=bare-except
-    else:
-        if response.status_code == 403:
-            raise RuntimeError('minio server already up')
+    if is_minio_up(timeout=1):
+        raise RuntimeError('minio server already up')
     os.environ['MINIO_CACHE_AFTER'] = '1'
     os.environ['MINIO_CACHE'] = 'on'
     os.environ['MINIO_ROOT_PASSWORD'] = CREDENTIAL
     os.environ['MINIO_ROOT_USER'] = CREDENTIAL
     # pylint: disable=consider-using-with
     process = subprocess.Popen(
         shlex.split(f'minio server --quiet --address {ENDPOINT} '
                     f"--console-address :{PORT+1} '{tmpdir!s}'"))
 
-    timeout = 5
-    while timeout > 0:
-        try:
-            response = requests.get(ENDPOINT_URI)
-            if response.status_code == 403:
-                break
-        # pylint: disable=bare-except
-        except:
-            pass
-        # pylint: disable=bare-except
-        timeout -= 0.1
-        time.sleep(0.1)
-    if timeout <= 0:
-        raise RuntimeError("minio server didn't start")
     try:
+        wait_for_minio_to_start(timeout=30)
         yield
     finally:
         process.terminate()
         process.wait()
     # pylint: enable=consider-using-with
 
 
-def make_bucket(name):
+def make_bucket(name) -> None:
     """Create a bucket."""
-    session = botocore.session.get_session()
+    session: botocore.session.Session = botocore.session.get_session()
     client = session.create_client(
         's3',
         aws_access_key_id=CREDENTIAL,
         aws_secret_access_key=CREDENTIAL,
         endpoint_url=ENDPOINT_URI,
         region_name='us-east-1',
         config=botocore.client.Config(signature_version='s3v4'))
     client.create_bucket(Bucket=name, ACL='public-read')
 
 
 # pylint: disable=redefined-outer-name, unused-argument # pytest fixture
 @pytest.fixture()
-def s3(s3_base):
+def s3(s3_base) -> Iterator[s3fs.core.S3FileSystem]:
     """Create a S3 file system instance."""
     s3fs.core.S3FileSystem.clear_instance_cache()
     fs = s3fs.core.S3FileSystem(anon=False,
                                 key=CREDENTIAL,
                                 secret=CREDENTIAL,
                                 client_kwargs={'endpoint_url': ENDPOINT_URI})
     fs.invalidate_cache()
@@ -122,16 +127,16 @@
 
 class S3:
     """S3 filesystem."""
     #: Bucket ID
     ID = 0
 
     # pylint: disable=redefined-outer-name # pytest fixture
-    def __init__(self, s3):
-        name = f'bucket{S3.ID}'
+    def __init__(self, s3: s3fs.core.S3FileSystem) -> None:
+        name: str = f'bucket{S3.ID}'
         S3.ID += 1
         make_bucket(name)
-        self.collection = S3Path(name).joinpath('collection')
-        self.view = S3Path(name).joinpath('view')
-        self.fs = s3
+        self.collection: S3Path = S3Path(name).joinpath('collection')
+        self.view: S3Path = S3Path(name).joinpath('view')
+        self.fs: s3fs.core.S3FileSystem = s3
 
     # pylint: enable=redefined-outer-name
```

### Comparing `zcollection-2023.3.2/zcollection/tests/second_dataset.json` & `zcollection-2023.5.0/zcollection/tests/second_dataset.json`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/zcollection/tests/test_compressed_array.py` & `zcollection-2023.5.0/zcollection/tests/test_compressed_array.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Copyright (c) 2023 CNES
+#
+# All rights reserved. Use of this source code is governed by a
+# BSD-style license that can be found in the LICENSE file.
+"""Tests for :class:`zcollection.compressed_array.CompressedArray`."""
+from typing import Any
+
 import dask.array.core
 import dask.array.creation
 import dask.array.random
 import dask.array.reductions
 import dask.array.routines
 import dask.array.ufunc
 import dask.array.utils
@@ -10,14 +17,15 @@
 
 from ..compressed_array import CompressedArray
 # pylint: disable=unused-import # Need to import for fixtures
 from .cluster import dask_client, dask_cluster
 
 # pylint: enable=unused-import
 
+# pylint: disable=unnecessary-lambda # We keep the lambdas for readability
 #: Functions to test
 functions = [
     lambda x: x,
     lambda x: dask.array.ufunc.expm1(x),
     lambda x: 2 * x,
     lambda x: x / 2,
     lambda x: x**2,
@@ -69,91 +77,106 @@
     lambda x: abs(x),
     lambda x: x > 0.5,
     lambda x: x.rechunk((4, 4, 4)),
     lambda x: x.rechunk((2, 2, 1)),
     lambda x: numpy.isneginf(x),
     lambda x: numpy.isposinf(x),
 ]
+# pylint: enable=unnecessary-lambda
 
 
 @pytest.mark.filterwarnings(
     'ignore:Casting complex values to real discards the imaginary part')
 @pytest.mark.parametrize('func', functions)
 def test_basic(
         func,
-        dask_client,  # pylint: disable=redefined-outer-name
-):
+        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+) -> None:
     """Test basic functionality."""
-    values = numpy.random.random((2, 3, 4))
-    arr = dask.array.core.from_array(CompressedArray(values), chunks='auto')
-    compressed_array = func(arr).compute()
-    array = func(dask.array.core.from_array(values)).compute()
+    values: numpy.ndarray = numpy.random.random((2, 3, 4))
+    arr: dask.array.core.Array = dask.array.core.from_array(
+        CompressedArray(values), chunks='auto')
+    compressed_array: numpy.ndarray = func(arr).compute()
+    array: numpy.ndarray = func(dask.array.core.from_array(values)).compute()
     assert compressed_array.shape == array.shape
     assert numpy.allclose(compressed_array, array)
 
 
 def test_metadata(
-        dask_client,  # pylint: disable=redefined-outer-name
-):
+        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+) -> None:
     """Test metadata."""
-    y = dask.array.random.random((10, 10), chunks=(5, 5))
+    y: dask.array.core.Array = dask.array.random.random((10, 10),
+                                                        chunks=(5, 5))
     z = CompressedArray(y.compute())
-    y = y.map_blocks(CompressedArray)
+    y = y.map_blocks(CompressedArray)  # type: ignore[assignment]
 
+    # pylint: disable=protected-access
     assert isinstance(y._meta, numpy.ndarray)
     assert isinstance((y + 1)._meta, numpy.ndarray)
     assert isinstance(y[:5, ::2]._meta, numpy.ndarray)
-    assert isinstance(y.rechunk((2, 2))._meta, numpy.ndarray)
+    assert isinstance(
+        y.rechunk((2, 2))._meta,  # type: ignore[arg-type]
+        numpy.ndarray)
     assert isinstance((y - z), numpy.ndarray)
     assert isinstance(y.persist()._meta, numpy.ndarray)
+    # pylint: enable=protected-access
 
 
 def test_from_delayed_meta(
-        dask_client,  # pylint: disable=redefined-outer-name
-):
+        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+) -> None:
     """Test from_delayed with meta."""
 
-    def f():
+    def f() -> CompressedArray:
         return CompressedArray(numpy.eye(3))
 
-    d = dask.delayed(f)()  # type: ignore
-    x = dask.array.core.from_delayed(d,
-                                     shape=(3, 3),
-                                     meta=CompressedArray(numpy.eye(1)))
+    d: Any = dask.delayed(f)()  # type: ignore
+    x: dask.array.core.Array = dask.array.core.from_delayed(
+        d, shape=(3, 3), meta=CompressedArray(numpy.eye(1)))
     assert numpy.all(x.compute() == f()[...])  # type: ignore
 
 
 def test_from_array(
-        dask_client,  # pylint: disable=redefined-outer-name
-):
+        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+) -> None:
     """Test from_array."""
     x = CompressedArray(numpy.eye(10))
-    d = dask.array.core.from_array(x, chunks=(5, 5))  # type: ignore
+    d: dask.array.core.Array = dask.array.core.from_array(
+        x, chunks=(5, 5))  # type: ignore[arg-type]
 
+    # pylint: disable=protected-access
     assert isinstance(d._meta, numpy.ndarray)
+    # pylint: enable=protected-access
     assert isinstance(d.compute(), numpy.ndarray)
     assert numpy.allclose(d.compute(), x)
 
 
 def test_map_blocks(
-        dask_client,  # pylint: disable=redefined-outer-name
-):
+        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+) -> None:
     """Test map_blocks."""
-    x = dask.array.creation.eye(10, chunks=5)  # type: ignore[arg-type]
-    y = x.map_blocks(CompressedArray)
+    x: dask.array.core.Array = dask.array.creation.eye(
+        10, chunks=5)  # type: ignore[arg-type]
+    y: dask.array.core.Array = x.map_blocks(
+        CompressedArray)  # type: ignore[arg-type]
+    # pylint: disable=protected-access
     assert isinstance(y._meta, numpy.ndarray)
+    # pylint: enable=protected-access
     assert numpy.allclose(y.compute(), x.compute())
 
 
 def test_compressed_masked_array(
-        dask_client,  # pylint: disable=redefined-outer-name
-):
+        dask_client,  # pylint: disable=redefined-outer-name,unused-argument
+) -> None:
     """Test CompressedMaskedArray."""
-    x = dask.array.creation.eye(10, chunks=5)  # type: ignore[arg-type]
-    y = x.map_blocks(CompressedArray, fill_value=0)
+    x: dask.array.core.Array = dask.array.creation.eye(
+        10, chunks=5)  # type: ignore[arg-type]
+    y: dask.array.core.Array = x.map_blocks(
+        CompressedArray, fill_value=0)  # type: ignore[arg-type]
     # assert isinstance(y._meta, CompressedArray)
     assert isinstance(y[...].compute(), numpy.ma.MaskedArray)
     assert isinstance(y.compute(), numpy.ma.MaskedArray)
     assert y.mean().compute() == 1
     assert y.min().compute() == 1
     assert y.max().compute() == 1
     assert y.sum().compute() == 10
```

### Comparing `zcollection-2023.3.2/zcollection/tests/test_dask_utils.py` & `zcollection-2023.5.0/zcollection/tests/test_dask_utils.py`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/zcollection/tests/test_expression.py` & `zcollection-2023.5.0/zcollection/tests/test_expression.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # BSD-style license that can be found in the LICENSE file.
 """
 Tests of the expression evaluation
 ==================================
 """
 from __future__ import annotations
 
-from typing import Optional
 import timeit
 
 import numpy
 import pytest
 import xarray
 
 from .. import dataset
@@ -22,67 +21,72 @@
 from .cluster import dask_client, dask_cluster
 
 # pylint enable=unused-import
 
 
 def make_dataset(num_samples: int | None = None) -> dataset.Dataset:
     """Creation of a data set for testing purposes."""
-    dates = numpy.arange(numpy.datetime64('2000-01-01'),
-                         numpy.datetime64('2009-12-31'),
-                         numpy.timedelta64(1, 'h')).astype('datetime64[us]')
+    dates = numpy.arange(numpy.datetime64('2000-01-01', 'ns'),
+                         numpy.datetime64('2009-12-31', 'ns'),
+                         numpy.timedelta64(1, 'h')).astype('datetime64[ns]')
     if num_samples is not None:
         dates = dates[:num_samples + 1]
     observation = numpy.random.rand(dates.size)  # type: ignore
     return dataset.Dataset.from_xarray(
-        xarray.Dataset(
-            dict(dates=xarray.DataArray(dates, dims=('num_lines', )),
-                 observation=xarray.DataArray(observation,
-                                              dims=('num_lines', )))))
+        xarray.Dataset({
+            'dates':
+            xarray.DataArray(dates, dims=('num_lines', )),
+            'observation':
+            xarray.DataArray(observation, dims=('num_lines', ))
+        }))
 
 
-def test_expression():
+def test_expression() -> None:
     """Test of the creation of expressions."""
     expr = Expression('a == b')
-    assert expr(dict(a=1, b=1))
-    assert not expr(dict(a=1, b=2))
+    assert expr({'a': 1, 'b': 1})
+    assert not expr({'a': 1, 'b': 2})
 
     with pytest.raises(SyntaxError):
         Expression('a==')
 
     with pytest.raises(NameError):
-        assert expr(dict(a=1, c=1))
+        assert expr({'a': 1, 'c': 1})
 
 
 def test_date_expression(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+) -> None:
     """Test of expressions handling dates.."""
-    ds = make_dataset(5 * 24)
+    zds = make_dataset(5 * 24)
     partitioning = Date(('dates', ), 'D')
 
-    for partition, _ in partitioning.split_dataset(ds, 'num_lines'):
+    for partition, _ in partitioning.split_dataset(zds, 'num_lines'):
         variables = dict(partitioning.parse('/'.join(partition)))
         expr = Expression('year==2000')
         assert expr(variables)
         expr = Expression('year==2000 and month==1')
         assert expr(variables)
         expr = Expression('year==2000 and month==1 and day in range(1, 12)')
         assert expr(variables)
 
 
 def test_bench_expression(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+) -> None:
     """Benchmark of expressions."""
     partitioning = Date(('dates', ), 'D')
-    ds = make_dataset()
+    zds = make_dataset()
     expr = Expression('year==2000 and month==1 and day in range(1, 12)')
     times = []
     number = 100
-    for partition, _ in partitioning.split_dataset(ds, 'num_lines'):
+    for partition, _ in partitioning.split_dataset(zds, 'num_lines'):
         variables = dict(partitioning.parse('/'.join(partition)))
         times.append(
             timeit.timeit('expr(variables)',
-                          globals=dict(expr=expr, variables=variables),
+                          globals={
+                              'expr': expr,
+                              'variables': variables
+                          },
                           number=number))
 
     assert sum(times) / (len(times) * number) < 1e-5
```

### Comparing `zcollection-2023.3.2/zcollection/tests/test_fs_utils.py` & `zcollection-2023.5.0/zcollection/tests/test_fs_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
 Testing utilities
 =================
 """
+from typing import Any
 import os
 import pathlib
 import platform
 
 import fsspec
 import fsspec.implementations.local
 
@@ -30,33 +31,35 @@
 vehicula. Donec odio lacus, viverra et hendrerit eu, mollis eget mauris. Duis
 suscipit, velit nec finibus ullamcorper, nisi lorem fermentum tellus, ut viverra
 nunc lorem ut odio. Duis eget ligula maximus, venenatis nulla a, commodo dolor.
 Aenean justo sapien, mollis aliquam vestibulum id, suscipit a ligula. Phasellus
 porta arcu erat, elementum faucibus leo auctor vel. Integer vel pharetra leo.'''
 
 
-def test_join_path():
+def test_join_path() -> None:
     """Test the join_path function."""
     assert fs_utils.join_path('a', 'b', 'c') == 'a/b/c'
     assert fs_utils.join_path('a', 'b', 'c', 'd') == 'a/b/c/d'
     assert fs_utils.join_path('a', 'b', 'c', 'd', 'e') == 'a/b/c/d/e'
     assert fs_utils.join_path('a', 'b', 'c', 'd', 'e', 'f') == 'a/b/c/d/e/f'
 
 
-def test_get_fs():
+def test_get_fs() -> None:
     """Test the get_fs function."""
     fs = fs_utils.get_fs('file')
     assert isinstance(fs, fsspec.implementations.local.LocalFileSystem)
     fs = fs_utils.get_fs()
     assert isinstance(fs, fsspec.implementations.local.LocalFileSystem)
 
 
-def test_fs_walk(tmpdir):
+def test_fs_walk(tmpdir) -> None:
     """Test the fs_walk function."""
-    for ix, item in enumerate([
+    item: Any
+
+    for idx, item in enumerate([
         ('year=2014', 'month=5'),
         ('year=2014', 'month=5', 'day=2'),
         ('year=2014', 'month=5', 'day=1'),
         ('year=2014', 'month=5', 'day=3'),
         ('year=2014', 'month=4'),
         ('year=2014', 'month=4', 'day=16'),
         ('year=2014', 'month=4', 'day=24'),
@@ -77,16 +80,16 @@
         ('year=2014', 'month=4', 'day=26'),
         ('year=2014', 'month=4', 'day=22'),
         ('year=2014', 'month=4', 'day=30'),
     ]):
         path = pathlib.Path(tmpdir).joinpath(*item)
         path.mkdir(parents=True, exist_ok=False)
         if 'day' in item[-1]:
-            with path.joinpath(f'file_{ix}.txt').open(mode='w',
-                                                      encoding='utf-8'):
+            with path.joinpath(f'file_{idx}.txt').open(mode='w',
+                                                       encoding='utf-8'):
                 ...
 
     fs = fs_utils.get_fs()
     listing1 = []
     for root, _dirs, files in fs_utils.fs_walk(fs, str(tmpdir), sort=True):
         for item in files:
             listing1.append(fs.sep.join([root, item]))
@@ -100,15 +103,15 @@
 
     assert list(
         fs_utils.fs_walk(fs,
                          str(pathlib.Path(tmpdir).joinpath('inexistent')),
                          sort=True)) == [('', [], [])]
 
 
-def test_normalize_path():
+def test_normalize_path() -> None:
     """Test the normalize_path function."""
     fs = fsspec.filesystem('file')
     root = str(pathlib.Path('/').resolve())
     if platform.system() == 'Windows':
         # fsspec returns only the drive letter for the root path.
         root = root.replace('\\', '')
 
@@ -125,27 +128,27 @@
     assert fs_utils.normalize_path(fs, './foo') == f'{os.path.sep}foo'
 
     fs = fsspec.filesystem('s3')
     assert fs_utils.normalize_path(fs, '/') == '/'
     assert fs_utils.normalize_path(fs, './foo') == './foo'
 
 
-def test_copy_file(tmpdir):
+def test_copy_file(tmpdir) -> None:
     """Test the copy file across different file systems."""
     fs_source = fsspec.filesystem('file')
     fs_target = fsspec.filesystem('memory')
     path = str(tmpdir / 'foo.txt')
     with fs_source.open(path, mode='wb', encoding='utf-8') as stream:
         stream.write(TEXT.encode('utf-8'))
     fs_utils.copy_file(path, 'foo.txt', fs_source, fs_target)
 
     assert fs_target.cat('foo.txt').decode('utf-8') == TEXT
 
 
-def test_copy_files(tmpdir):
+def test_copy_files(tmpdir) -> None:
     """Test the copy files across different file systems."""
     source = tmpdir / 'source'
     target = tmpdir / 'target'
     fs_source = fsspec.filesystem('file')
     fs_target = fsspec.filesystem('file')
     fs_source.mkdir(source)
     fs_target.mkdir(target)
@@ -161,20 +164,21 @@
             stream.write(TEXT.encode('utf-8'))
     fs_utils.copy_files(paths, str(target), fs_source, fs_target)
 
     for item in fs_target.ls(str(target)):
         assert fs_target.cat(item).decode('utf-8') == TEXT
 
 
-def test_copy_tree(tmpdir):
+def test_copy_tree(tmpdir) -> None:
     """Test the copy tree across different file systems."""
+    item: Any
     fs_source = fsspec.filesystem('file')
     fs_target = fsspec.filesystem('memory')
 
-    for ix, item in enumerate([
+    for idx, item in enumerate([
         ('year=2014', 'month=5'),
         ('year=2014', 'month=5', 'day=2'),
         ('year=2014', 'month=5', 'day=1'),
         ('year=2014', 'month=5', 'day=3'),
         ('year=2014', 'month=4'),
         ('year=2014', 'month=4', 'day=16'),
         ('year=2014', 'month=4', 'day=24'),
@@ -195,15 +199,15 @@
         ('year=2014', 'month=4', 'day=26'),
         ('year=2014', 'month=4', 'day=22'),
         ('year=2014', 'month=4', 'day=30'),
     ]):
         path = fs_utils.join_path(str(tmpdir), *item)
         fs_source.makedirs(path, exist_ok=False)
         if 'day' in item[-1]:
-            with fs_source.open(fs_utils.join_path(path, f'file_{ix}.txt'),
+            with fs_source.open(fs_utils.join_path(path, f'file_{idx}.txt'),
                                 mode='wb',
                                 encoding='utf-8') as stream:
                 stream.write(TEXT.encode('utf-8'))
 
     fs_utils.copy_tree(str(tmpdir), '/tree', fs_source, fs_target)
 
     for root, dirs, files in fs_utils.fs_walk(fs_target, '/tree'):
```

### Comparing `zcollection-2023.3.2/zcollection/tests/test_mathematics.py` & `zcollection-2023.5.0/zcollection/tests/test_mathematics.py`

 * *Files identical despite different names*

### Comparing `zcollection-2023.3.2/zcollection/tests/test_meta.py` & `zcollection-2023.5.0/zcollection/tests/test_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
 Metadata testing.
 =================
 """
+from __future__ import annotations
+
+from typing import Any
 import json
 import pathlib
 import pickle
 
 import numpy
 import pytest
 import zarr.codecs
 
 from .. import meta
 
 
-def test_attribute():
+def test_attribute() -> None:
     """Test attribute creation."""
     att = meta.Attribute('a', 23.4)
     assert isinstance(att, meta.Attribute)
     assert att.name == 'a'
     assert att.value == 23.4
     assert str(att) == "Attribute('a', 23.4)"
     # pylint: disable=comparison-with-itself
@@ -35,114 +38,116 @@
     assert att == meta.Attribute('a', numpy.arange(10))
 
     att = meta.Attribute('a', numpy.datetime64('2000-01-01', 'us'))
     assert att == att
     # pylint: enable=comparison-with-itself
 
 
-def test_dimension():
+def test_dimension() -> None:
     """Test dimension creation."""
     dim = meta.Dimension('a', 12)
     assert isinstance(dim, meta.Dimension)
     assert dim.name == 'a'
     assert dim.value == 12
     assert str(dim) == "Dimension('a', 12)"
     # pylint: disable=comparison-with-itself
     assert dim == dim
     # pylint: enable=comparison-with-itself
     assert dim != meta.Dimension('a', 11)
     assert isinstance(meta.Dimension.from_config(dim.get_config()),
                       meta.Dimension)
 
 
-def test_variable():
+def test_variable() -> None:
     """Test variable creation."""
     var = meta.Variable('a',
-                        numpy.dtype('int16'), ('a', ),
-                        (meta.Attribute('x', 12), ),
-                        zarr.codecs.Zlib(),
-                        0,
+                        numpy.dtype('int16'),
+                        dimensions=('a', ),
+                        attrs=(meta.Attribute('x', 12), ),
+                        compressor=zarr.codecs.Zlib(),
                         filters=(zarr.codecs.Delta(numpy.float64, numpy.int16),
                                  zarr.codecs.FixedScaleOffset(
                                      0, 1, numpy.int16)))
     assert isinstance(var, meta.Variable)
     assert str(var) == "Variable('a')"
     # pylint: disable=comparison-with-itself
     assert var == var
     assert (var == 2) is False
-    other = meta.Variable.from_config(var.get_config())
+    other: meta.Variable = meta.Variable.from_config(var.get_config())
     assert var == other
     other.name = 'x'
     assert var != other
     # pylint: enable=comparison-with-itself
 
 
-def test_dataset():
+def test_dataset() -> None:
     """Test dataset creation."""
-    root = pathlib.Path(__file__).parent
+    root: pathlib.Path = pathlib.Path(__file__).parent
     with root.joinpath('first_dataset.json').open(encoding='utf-8') as stream:
-        first = json.load(stream)
+        first: dict[str, Any] = json.load(stream)
     with root.joinpath('second_dataset.json').open(encoding='utf-8') as stream:
-        second = json.load(stream)
-    ds = meta.Dataset.from_config(first)
-    other = meta.Dataset.from_config(second)
+        second: dict[str, Any] = json.load(stream)
+    ds: meta.Dataset = meta.Dataset.from_config(first)
+    other: meta.Dataset = meta.Dataset.from_config(second)
     assert ds == other
     assert (ds == 2) is False
     assert (ds != other) is False
     ds.dimensions = ds.dimensions + ('dummy', )
     assert ds != other
 
 
-def test_select_variables():
-    root = pathlib.Path(__file__).parent
+def test_select_variables() -> None:
+    """Test select_variables."""
+    root: pathlib.Path = pathlib.Path(__file__).parent
     with root.joinpath('first_dataset.json').open(encoding='utf-8') as stream:
-        config = json.load(stream)
-    ds = meta.Dataset.from_config(config)
-    vars = ds.select_variables(('longitude', 'latitude'))
-    assert vars == {'longitude', 'latitude'}
-    vars = ds.select_variables(drop_variables=('longitude', 'latitude'))
-    assert set(vars) & {'longitude', 'latitude'} == set()
-    vars = ds.select_variables(keep_variables=('longitude', 'latitude',
-                                               'time'),
-                               drop_variables=('time', ))
-    assert vars == {'longitude', 'latitude'}
+        config: dict[str, Any] = json.load(stream)
+    ds: meta.Dataset = meta.Dataset.from_config(config)
+    variables: set[str] = ds.select_variables(('longitude', 'latitude'))
+    assert variables == {'longitude', 'latitude'}
+    variables = ds.select_variables(drop_variables=('longitude', 'latitude'))
+    assert set(variables) & {'longitude', 'latitude'} == set()
+    variables = ds.select_variables(keep_variables=('longitude', 'latitude',
+                                                    'time'),
+                                    drop_variables=('time', ))
+    assert variables == {'longitude', 'latitude'}
 
 
-def test_search_same_dimensions_as():
+def test_search_same_dimensions_as() -> None:
     """Test search_same_dimensions_as."""
-    root = pathlib.Path(__file__).parent
+    root: pathlib.Path = pathlib.Path(__file__).parent
     with root.joinpath('first_dataset.json').open(encoding='utf-8') as stream:
-        first = json.load(stream)
-    ds = meta.Dataset.from_config(first)
-    other = ds.search_same_dimensions_as(ds.variables['simulated_error_karin'])
+        first: dict[str, Any] = json.load(stream)
+    ds: meta.Dataset = meta.Dataset.from_config(first)
+    other: meta.Variable = ds.search_same_dimensions_as(
+        ds.variables['simulated_error_karin'])
     assert other.dimensions == ds.variables['simulated_error_karin'].dimensions
 
     other = meta.Variable.from_config(other.get_config())
     other.dimensions = other.dimensions + ('dummy', )
     with pytest.raises(ValueError):
         ds.search_same_dimensions_as(other)
 
 
-def test_pickle():
+def test_pickle() -> None:
     """Test pickling."""
-    root = pathlib.Path(__file__).parent
+    root: pathlib.Path = pathlib.Path(__file__).parent
     with root.joinpath('first_dataset.json').open(encoding='utf-8') as stream:
-        data = json.load(stream)
-    ds = meta.Dataset.from_config(data)
-    other = pickle.loads(pickle.dumps(ds))
+        data: dict[str, Any] = json.load(stream)
+    ds: meta.Dataset = meta.Dataset.from_config(data)
+    other: meta.Dataset = pickle.loads(pickle.dumps(ds))
     assert ds == other
 
 
-def test_missing_variables():
+def test_missing_variables() -> None:
     """Test missing_variables."""
-    root = pathlib.Path(__file__).parent
+    root: pathlib.Path = pathlib.Path(__file__).parent
     with root.joinpath('first_dataset.json').open(encoding='utf-8') as stream:
-        data = json.load(stream)
-    ds = meta.Dataset.from_config(data)
-    other = pickle.loads(pickle.dumps(ds))
+        data: dict[str, Any] = json.load(stream)
+    ds: meta.Dataset = meta.Dataset.from_config(data)
+    other: meta.Dataset = pickle.loads(pickle.dumps(ds))
 
     assert len(ds.missing_variables(other)) == 0
 
     del other.variables['cross_track_distance']
     del other.variables['cycle_number']
 
     assert set(ds.missing_variables(other)) == {
@@ -151,47 +156,50 @@
 
     other.variables['XXX'] = other.variables['longitude']
     other.variables['XXX'].name = 'XXX'
     with pytest.raises(ValueError):
         ds.missing_variables(other)
 
 
-def test_add_variable():
+def test_add_variable() -> None:
     """Test adding a variable."""
-    ds = meta.Dataset(('x', 'y'), [], [])
-    ds.add_variable(meta.Variable('a', numpy.float64, ('x', 'y')))
+    ds = meta.Dataset(('x', 'y'), [])
+    ds.add_variable(meta.Variable('a', numpy.float64, dimensions=('x', 'y')))
 
     with pytest.raises(ValueError):
-        ds.add_variable(meta.Variable('a', numpy.float64, ('x', 'y')))
+        ds.add_variable(
+            meta.Variable('a', numpy.float64, dimensions=('x', 'y')))
 
-    ds.add_variable(meta.Variable('b', numpy.float64, ('x')))
-    ds.add_variable(meta.Variable('c', numpy.float64, ('y')))
+    ds.add_variable(meta.Variable('b', numpy.float64, dimensions=('x', )))
+    ds.add_variable(meta.Variable('c', numpy.float64, dimensions=('y', )))
 
     with pytest.raises(ValueError):
-        ds.add_variable(meta.Variable('d', numpy.float64, ('a', 'y')))
+        ds.add_variable(
+            meta.Variable('d', numpy.float64, dimensions=('a', 'y')))
 
     with pytest.raises(ValueError):
-        ds.add_variable(meta.Variable('e', numpy.float64, ('a', 'b')))
+        ds.add_variable(
+            meta.Variable('e', numpy.float64, dimensions=('a', 'b')))
 
     with pytest.raises(ValueError):
-        ds.add_variable(meta.Variable('f', numpy.float64, ('a')))
+        ds.add_variable(meta.Variable('f', numpy.float64, dimensions=('a', )))
 
-    ds.add_variable(meta.Variable('g', numpy.float64, ()))
+    ds.add_variable(meta.Variable('g', numpy.float64))
 
 
-def test_select_variables_by_dims():
+def test_select_variables_by_dims() -> None:
     """Test select_variable_by_dims."""
-    ds = meta.Dataset(('a', 'b', 'x', 'y'), [], [])
-    ds.add_variable(meta.Variable('a', numpy.float64, ('x', 'y')))
-    ds.add_variable(meta.Variable('b', numpy.float64, ('x')))
-    ds.add_variable(meta.Variable('c', numpy.float64, ('y')))
-    ds.add_variable(meta.Variable('d', numpy.float64, ('a', 'y')))
-    ds.add_variable(meta.Variable('e', numpy.float64, ('a', 'b')))
-    ds.add_variable(meta.Variable('f', numpy.float64, ('a')))
-    ds.add_variable(meta.Variable('g', numpy.float64, ()))
+    ds = meta.Dataset(('a', 'b', 'x', 'y'), [])
+    ds.add_variable(meta.Variable('a', numpy.float64, dimensions=('x', 'y')))
+    ds.add_variable(meta.Variable('b', numpy.float64, dimensions=('x', )))
+    ds.add_variable(meta.Variable('c', numpy.float64, dimensions=('y', )))
+    ds.add_variable(meta.Variable('d', numpy.float64, dimensions=('a', 'y')))
+    ds.add_variable(meta.Variable('e', numpy.float64, dimensions=('a', 'b')))
+    ds.add_variable(meta.Variable('f', numpy.float64, dimensions=('a', )))
+    ds.add_variable(meta.Variable('g', numpy.float64))
 
     assert ds.select_variables_by_dims(('x', 'y')) == {'a', 'b', 'c', 'd'}
     assert ds.select_variables_by_dims(('x', )) == {'a', 'b'}
     assert ds.select_variables_by_dims(('y', )) == {'a', 'c', 'd'}
     assert ds.select_variables_by_dims(('a', 'y')) == {'a', 'c', 'd', 'e', 'f'}
     assert ds.select_variables_by_dims(('a', 'b')) == {'d', 'e', 'f'}
     assert ds.select_variables_by_dims(('a', )) == {'d', 'e', 'f'}
```

### Comparing `zcollection-2023.3.2/zcollection/tests/test_storage.py` & `zcollection-2023.5.0/zcollection/tests/test_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
 Testing the storage module.
 ===========================
 """
+from typing import Any
 import math
 import platform
 import time
 
 import dask.array
 import dask.distributed
 import numpy
@@ -22,15 +23,15 @@
 from .fs import local_fs
 
 # pylint: enable=unused-import
 
 
 def test_execute_transaction(
         dask_client,  # pylint: disable=redefined-outer-name
-):
+) -> None:
     """Test the execute_transaction function."""
     # First case: no transaction to execute
     assert storage.execute_transaction(dask_client, sync.NoSync(), []) is None
 
     # General case: execute a transaction without error
     def func():
         return 1
@@ -52,51 +53,51 @@
     try:
         futures += storage.execute_transaction(
             dask_client, sync.NoSync(),
             [dask_client.submit(fail, i) for i in range(10)])
     except ValueError:
         exception_seen = True
     assert exception_seen
-    for ix, item in enumerate(futures):
-        if ix % 2 == 0:
+    for idx, item in enumerate(futures):
+        if idx % 2 == 0:
             assert item.exception() is not None
         else:
             assert item.done()
 
 
-def create_variable(shape, fill_value=None):
+def create_variable(shape, fill_value=None) -> dataset.DelayedArray:
     """Create a variable."""
     data = numpy.ones(shape, dtype='uint8')
     if fill_value is not None:
         data[:, 0] = fill_value
-    return dataset.Variable(name='var',
-                            data=data,
-                            dimensions=('x', 'y'),
-                            fill_value=fill_value,
-                            attrs=[
-                                dataset.Attribute('a', 1),
-                                dataset.Attribute('b', 2),
-                                dataset.Attribute('long_name', 'long name')
-                            ])
+    return dataset.DelayedArray(name='var',
+                                data=data,
+                                dimensions=('x', 'y'),
+                                fill_value=fill_value,
+                                attrs=[
+                                    dataset.Attribute('a', 1),
+                                    dataset.Attribute('b', 2),
+                                    dataset.Attribute('long_name', 'long name')
+                                ])
 
 
-def create_dataset(shape):
+def create_dataset(shape) -> dataset.Dataset:
     """Create a dataset."""
     return dataset.Dataset([create_variable(shape)],
                            attrs=[
                                dataset.Attribute('a', 1),
                                dataset.Attribute('b', 2),
                                dataset.Attribute('long_name', 'long name')
                            ])
 
 
 def test_write_attrs(
         local_fs,  # pylint: disable=redefined-outer-name
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+) -> None:
     """Test the write_attrs function."""
     var = create_variable((10, 2))
     path = local_fs.root.joinpath('var')
     local_fs.mkdir(str(path))
     storage.write_zattrs(str(local_fs.root), var, local_fs.fs)
     path = str(path.joinpath(storage.ZATTRS))
     expected = [
@@ -150,15 +151,15 @@
         'y': 826
     }, (53, 826)),
 ])
 def test_write_variable(
         local_fs,  # pylint: disable=redefined-outer-name
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
         chunks,
-        chunks_expected):
+        chunks_expected) -> None:
     """Test the write_variable function."""
     dim_size = 1024
     var = create_variable((dim_size, dim_size))
     storage.write_zarr_variable(('var', var),
                                 dirname=str(local_fs.root),
                                 fs=local_fs.fs,
                                 chunks=chunks)
@@ -201,15 +202,15 @@
         }, 2),
     ])
 def test_write_variable_block_size_limit(
         local_fs,  # pylint: disable=redefined-outer-name
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
         block_size,
         chunks,
-        blocks_number):
+        blocks_number) -> None:
     """Test the write_variable function with different block size limits."""
     dim_size = 1024
     var = create_variable((dim_size, dim_size))
     storage.write_zarr_variable(('var', var),
                                 dirname=str(local_fs.root),
                                 fs=local_fs.fs,
                                 chunks=chunks,
@@ -220,32 +221,32 @@
 
     assert zarray.nchunks == blocks_number
 
 
 def test_write_zarr_group(
         local_fs,  # pylint: disable=redefined-outer-name
         dask_client,  # pylint: disable=redefined-outer-name
-):
+) -> None:
     """Test the write_zarr_group function."""
-    ds = create_dataset((1024, 1024))
+    zds = create_dataset((1024, 1024))
     # memory fs does not support multi-processes
     future = dask_client.submit(storage.write_zarr_group,
-                                dask_client.scatter(ds), str(local_fs.root),
+                                dask_client.scatter(zds), str(local_fs.root),
                                 local_fs.fs, sync.NoSync())
     future.result()
     mapper = local_fs.get_mapper(str(local_fs.root))
     zarray = zarr.open_group(mapper)
     assert numpy.all(zarray['var'][...] == 1)
     assert zarray.attrs['a'] == 1
     assert zarray.attrs['b'] == 2
     assert zarray.attrs['long_name'] == 'long name'
     assert zarray['var'].attrs['_ARRAY_DIMENSIONS'] == ['x', 'y']
 
     other = storage.open_zarr_group(str(local_fs.root), local_fs.fs)
-    assert other.metadata() == ds.metadata()
+    assert other.metadata() == zds.metadata()
 
 
 @pytest.mark.parametrize('chunks, chunks_expected', [
     (None, (1024, 1024)),
     ({
         'x': -1,
         'y': 1024
@@ -260,30 +261,30 @@
     }, (512, 1024)),
 ])
 def test_update_zarr_array(
     local_fs,  # pylint: disable=redefined-outer-name
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     chunks,
     chunks_expected,
-):
+) -> None:
     """Test the update_zarr_array function."""
     dim_size = 1024
 
     var = create_variable((dim_size, dim_size), fill_value=10)
     storage.write_zarr_variable(('var', var),
                                 str(local_fs.root),
                                 local_fs.fs,
                                 chunks=chunks)
     path = str(local_fs.root.joinpath('var'))
     storage.update_zarr_array(path, dask.array.full((dim_size, dim_size), 2),
                               local_fs.fs)
     mapper = local_fs.get_mapper(path)
     zarray = zarr.open(mapper)
     assert numpy.all(zarray[...] == 2)
-    data = numpy.full((dim_size, dim_size), 2)
+    data: Any = numpy.full((dim_size, dim_size), 2)
     data[:, 0] = 5
     data = numpy.ma.masked_equal(data, 5)
     assert numpy.all(data[:, 0].mask)
     storage.update_zarr_array(path, data, local_fs.fs)
     zarray = zarr.open(mapper)
     assert numpy.all(zarray[:, 0] == 10)
 
@@ -292,15 +293,15 @@
     assert zarray.chunks == chunks_expected
     assert zarray.nchunks == chunks_number
 
 
 def test_del_zarr_array(
         local_fs,  # pylint: disable=redefined-outer-name
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-):
+) -> None:
     """Test the del_zarr_array function."""
     var = create_variable((1024, 1024))
     root = str(local_fs.root)
     storage.write_zarr_variable(('var', var), root, local_fs.fs)
     storage.del_zarr_array(root, 'var', local_fs.fs)
     assert not local_fs.exists(str(local_fs.root.joinpath('var')))
 
@@ -325,15 +326,15 @@
     }, (1024, 128)),
 ])
 def test_add_zarr_array(
     local_fs,  # pylint: disable=redefined-outer-name
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     chunks,
     chunks_expected,
-):
+) -> None:
     """Test the add_zarr_array function."""
     dim_size = 1024
     var = create_variable((dim_size, dim_size), fill_value=10)
     root = str(local_fs.root)
     var.name = 'var1'
     storage.write_zarr_variable(('var1', var),
                                 root,
@@ -348,11 +349,11 @@
     mapper = local_fs.get_mapper(root)
     zarray = zarr.open(mapper)
     assert numpy.all(zarray['var2'][...] == 10)
 
     chunks_number = math.ceil(dim_size / chunks_expected[0]) * math.ceil(
         dim_size / chunks_expected[1])
 
-    for var in ['var1', 'var2']:
-        var_array = zarray[var]
+    for varname in ['var1', 'var2']:
+        var_array = zarray[varname]
         assert var_array.chunks == chunks_expected
         assert var_array.nchunks == chunks_number
```

### Comparing `zcollection-2023.3.2/zcollection/type_hints.py` & `zcollection-2023.5.0/zcollection/type_hints.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,13 +74,36 @@
 class ArrayLike(Protocol[_DType_co]):
     """Protocol for array-like objects."""
 
     def __array__(self) -> NDArray:
         ...
 
     @property
+    def dtype(self) -> DType:
+        """The data type of the array."""
+        # pylint: disable=unnecessary-ellipsis
+        # Make checker happy.
+        ...
+        # pylint: enable=unnecessary-ellipsis
+
+    @property
     def shape(self) -> tuple[int, ...]:
         """The shape of the array."""
         # pylint: disable=unnecessary-ellipsis
         # Make checker happy.
         ...
         # pylint: enable=unnecessary-ellipsis
+
+    @property
+    def size(self) -> int:
+        """The size of the array."""
+        # pylint: disable=unnecessary-ellipsis
+        # Make checker happy.
+        ...
+        # pylint: enable=unnecessary-ellipsis
+
+    def astype(self, dtype: DTypeLike) -> ArrayLike[_DType_co]:
+        """Convert the array to a given type."""
+        # pylint: disable=unnecessary-ellipsis
+        # Make checker happy.
+        ...
+        # pylint: enable=unnecessary-ellipsis
```

### Comparing `zcollection-2023.3.2/zcollection/variable.py` & `zcollection-2023.5.0/zcollection/variable/abc.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,292 +4,309 @@
 # BSD-style license that can be found in the LICENSE file.
 """
 Dataset variable.
 =================
 """
 from __future__ import annotations
 
-from typing import Any, Iterable, Iterator, Mapping, MutableMapping, Sequence
+from typing import Any, Callable, Iterator, Sequence, TypeVar
+import abc
 import collections
-import uuid
 
 import dask.array.core
-import dask.array.creation
-import dask.array.ma
-import dask.array.routines
-import dask.array.wrap
-import dask.base
-import dask.threaded
 import numcodecs.abc
 import numpy
 import xarray
 import zarr
 
-from . import mathematics, meta
-from .meta import Attribute
-from .type_hints import ArrayLike, NDArray, NDMaskedArray
+from .. import mathematics, meta, representation
+from ..meta import Attribute
+from ..type_hints import ArrayLike, NDArray, NDMaskedArray
 
-#: The dask array getter used to access the data.
-GETTER = dask.array.core.getter
+#: Generic type for a variable interface.
+I = TypeVar('I', bound='IVariable')
 
+#: Generic type for a dataset variable.
+T = TypeVar('T', bound='Variable')
 
-class ModifiedVariableError(RuntimeError):
-    """Raised when a variable has been modified since is was initialized."""
 
-    def __str__(self) -> str:
-        """Get the string representation of the exception.
-
-        Returns:
-            The string representation of the exception.
-        """
-        return ('You tried to access the data of a variable that has been '
-                'modified since its initialization. Try to re-load the '
-                'dataset.')
-
-
-def _dimensions_repr(dimensions: dict[str, int]) -> str:
-    """Get the string representation of the dimensions.
+def new_variable(cls: type[I], **kwargs: Any) -> I:
+    """Create a new variable.
 
     Args:
-        dimensions: The dimensions.
-
-    Returns:
-        The string representation of the dimensions.
+        constructor: Variable constructor.
+        kwargs: Keyword arguments passed to the constructor.
     """
-    return str(tuple(f'{name}: {value}' for name, value in dimensions.items()))
+    self: I = cls.__new__(cls)
+    # pylint: disable=expression-not-assigned
+    # We use the set notation to evaluate the generator
+    {
+        setattr(self, key, value)  # type: ignore[func-returns-value]
+        for key, value in kwargs.items()
+    }
+    # pylint: enable=expression-not-assigned
+    return self
 
 
-def _calculate_column_width(items: Iterable) -> int:
-    """Calculate the maximum width of a column.
+def concat(
+    self: T,
+    other: T | Sequence[T],
+    concatenate: Callable,
+    dim: str,
+) -> T:
+    """Concatenate a variable with another variable or a sequence of variables.
 
     Args:
-        items: An iterable of items.
+        self: A variable.
+        other: A variable or a sequence of variables.
+        constructor: Variable constructor.
+        concatenate: Function used to concatenate the arrays.
+        dim: Dimension along which the arrays are concatenated.
 
     Returns:
-        The maximum width of a column.
-    """
-    max_name = max(len(str(name)) for name in items)
-    return max(max_name, 7)
+        A new variable.
 
-
-def _maybe_truncate(obj: Any, max_size: int) -> str:
-    """Truncate the string representation of an object to the given length.
-
-    Args:
-        obj: An object.
-        max_size: The maximum length of the string representation.
-
-    Returns:
-        The string representation of the object.
+    Raises:
+        ValueError: If ``other`` is empty or is not a sequence of ``self`` type.
     """
-    result = str(obj)
-    if len(result) > max_size:
-        return result[:max_size - 3] + '...'
-    return result
+    if not isinstance(other, Sequence):
+        other = [other]
+    if not other:
+        raise ValueError('other must be a non-empty sequence')
+
+    # Self and other must have the same type
+    if not all(isinstance(item, type(self)) for item in other):
+        raise ValueError(f'other must be a sequence of {type(self)}')
+
+    try:
+        axis: int = self.dimensions.index(dim)
+        return new_variable(
+            type(self),
+            name=self.name,
+            array=concatenate((self.array, *(item.array for item in other)),
+                              axis=axis),
+            dimensions=self.dimensions,
+            attrs=self.attrs,
+            compressor=self.compressor,
+            fill_value=self.fill_value,
+            filters=self.filters,
+        )
+    except ValueError:
+        # If the concatenation dimension is not within the dimensions of the
+        # variable, then the original variable is returned (i.e.
+        # concatenation is not necessary).
+        return new_variable(type(self),
+                            name=self.name,
+                            array=self.array,
+                            dimensions=self.dimensions,
+                            attrs=self.attrs,
+                            compressor=self.compressor,
+                            fill_value=self.fill_value,
+                            filters=self.filters)
 
 
-def _pretty_print(obj: Any, num_characters: int = 120) -> str:
-    """Pretty print the object.
+def not_equal(first: Any, second: Any) -> bool:
+    """Check if two objects are not equal.
 
     Args:
-        obj: An object.
-        num_characters: The maximum number of characters per line.
+        first: The first object.
+        second: The second object.
 
     Returns:
-        The pretty printed string representation of the object.
+        True if the two objects are different, False otherwise.
     """
-    result = _maybe_truncate(obj, num_characters)
-    return result + ' ' * max(num_characters - len(result), 0)
 
+    def _is_not_a_number(number: Any) -> bool:
+        """Check if a number is NaN or NaT."""
+        # pylint: disable=comparison-with-itself
+        return not number == number and number != number
+        # pylint: enable=comparison-with-itself
 
-def _attributes_repr(attrs: Sequence[Attribute]) -> Iterator[str]:
-    """Get the string representation of the attributes.
-
-    Args:
-        attrs: The attributes.
-
-    Returns:
-        The string representation of the attributes.
-    """
-    width = _calculate_column_width(item.name for item in attrs)
-    for attr in attrs:
-        name_str = f'    {attr.name:<{width}s}'
-        yield _pretty_print(f'{name_str}: {attr.value!r}')
+    #: pylint: disable=unidiomatic-typecheck
+    if type(first) != type(second):
+        return True
+    #: pylint: enable=unidiomatic-typecheck
+    if _is_not_a_number(first) and _is_not_a_number(second):
+        return False
+    if first is None and second is None:
+        return False
+    if first == second:
+        return False
+    return True
 
 
 def _variable_repr(var: Variable) -> str:
     """Get the string representation of a variable.
 
     Args:
         var: A variable.
 
     Returns:
         The string representation of the variable.
     """
     # Dimensions
-    dims_str = _dimensions_repr(dict(zip(var.dimensions, var.shape)))
-    lines = [
+    dims_str: str = representation.dimensions(
+        dict(zip(var.dimensions, var.shape)))
+    lines: list[str] = [
         f'<{var.__module__}.{var.__class__.__name__} {dims_str}>',
         f'{var.array!r}'
     ]
     # Attributes
     if len(var.attrs):
         lines.append('  Attributes:')
-        lines += _attributes_repr(var.attrs)
+        lines += representation.attributes(var.attrs)
     # Filters
     if var.filters:
         lines.append('  Filters:')
         lines += [f'    {item!r}' for item in var.filters]
     # Compressor
     if var.compressor:
         lines.append('  Compressor:')
         lines += [f'    {var.compressor!r}']
     return '\n'.join(lines)
 
 
-def _not_equal(first: Any, second: Any) -> bool:
-    """Check if two objects are not equal.
+class IVariable(abc.ABC):
+    """Define the interface for a variable."""
 
-    Args:
-        first: The first object.
-        second: The second object.
+    @property
+    @abc.abstractmethod
+    def data(self) -> dask.array.core.Array:
+        """Return the values as a dask array where values equal to the fill
+        value are masked. If no fill value is set, the returned array is the
+        same as the underlying array.
 
-    Returns:
-        True if the two objects are different, False otherwise.
-    """
+        Returns:
+            The dask array
 
-    def _is_not_a_number(number: Any) -> bool:
-        """Check if a number is NaN or NaT."""
-        # pylint: disable=comparison-with-itself
-        return not number == number and number != number
-        # pylint: enable=comparison-with-itself
+        .. seealso::
 
-    #: pylint: disable=unidiomatic-typecheck
-    if type(first) != type(second):
-        return True
-    #: pylint: enable=unidiomatic-typecheck
-    if _is_not_a_number(first) and _is_not_a_number(second):
-        return False
-    if first is None and second is None:
-        return False
-    if first == second:
-        return False
-    return True
+            :meth:`Variable.array`
+        """
 
+    @property
+    @abc.abstractmethod
+    def values(self) -> NDArray | NDMaskedArray:
+        """Return the variable values.
 
-def _asarray(
-    arr: ArrayLike[Any],
-    fill_value: Any | None = None,
-) -> tuple[dask.array.core.Array, Any]:
-    """Convert an array-like object to a dask array.
+        .. note::
 
-    Args:
-        arr: An array-like object.
-        fill_value: The fill value.
+            If the variable has a fill value, the result is a masked array where
+            masked values are equal to the fill value.
 
-    Returns:
-        If the data provided is a masked array, the functions return the array
-        with masked data replaced by its fill value and the fill value of the
-        offered masked array. Otherwise, the provided array and fill value.
-    """
-    result = dask.array.core.asarray(arr)  # type: dask.array.core.Array
-    _meta = result._meta  # pylint: disable=protected-access
-    if isinstance(_meta, numpy.ma.MaskedArray):
-        if fill_value is not None and _not_equal(fill_value, _meta.fill_value):
-            raise ValueError(
-                f'The fill value {fill_value!r} does not match the fill value '
-                f'{_meta.fill_value!r} of the array.')
-        return dask.array.ma.filled(result, _meta.fill_value), _meta.fill_value
-    return result, fill_value
-
-
-def _new_variable(
-    name: str,
-    data: dask.array.core.Array,
-    dimensions: Sequence[str],
-    attrs: Sequence[Attribute],
-    compressor: numcodecs.abc.Codec | None,
-    fill_value: Any | None,
-    filters: Sequence[numcodecs.abc.Codec] | None,
-) -> Variable:
-    """Create a new variable.
+        Returns:
+            The variable data
+        """
 
-    Args:
-        name: Name of the variable
-        data: Variable data
-        dimensions: Variable dimensions
-        attrs: Variable attributes
-        compressor: Compression codec
-        fill_value: Value to use for uninitialized values
-        filters: Filters to apply before writing data to disk
-    """
-    self = Variable.__new__(Variable)
-    self.array = data
-    self.attrs = attrs
-    self.compressor = compressor
-    self.dimensions = dimensions
-    self.fill_value = fill_value
-    self.filters = filters
-    self.name = name
-    return self
+    @values.setter
+    @abc.abstractmethod
+    def values(self, data: Any) -> None:
+        """Defines the values array. If the data provided is a masked array,
+        it's converted to an array, where the masked values are replaced by the
+        fill value of this instance.
 
+        Args:
+            data: The new data to use
 
-def _blockdims_from_blockshape(
-        shape: tuple[int, ...],
-        chunks: tuple[int, ...]) -> tuple[tuple[int, ...], ...]:
-    """Convert a blockshape to a blockdims tuple."""
-    return tuple(((chunk_item, ) * (shape_item // chunk_item) +
-                  ((shape_item % chunk_item, ) if shape_item %
-                   chunk_item else ()) if shape_item else (0, ))
-                 for shape_item, chunk_item in zip(shape, chunks))
-
-
-def _from_zarr_array(
-    array: zarr.Array,
-    shape: Sequence[int],
-    chunks: Sequence[int],
-    name: str,
-    lock: bool = False,
-    asarray=True,
-    inline_array=True,
-) -> dask.array.core.Array:
-    """Create a dask array from a zarr array.
+        Raises:
+            ValueError: If the shape of the data does not match the shape of
+                the stored data.
+        """
 
-    Args:
-        array: A zarr array.
+    @abc.abstractmethod
+    def persist(self: I, **kwargs) -> I:
+        """Persist the variable data into memory.
 
-    Returns:
-        The dask array.
-    """
-    normalized_chunks = sum(
-        (_blockdims_from_blockshape(
-            (shape_item, ),
-            (chunk_item, )) if not isinstance(chunk_item, (tuple, list)) else
-         (chunk_item, ) for shape_item, chunk_item in zip(shape, chunks)),
-        (),
-    )
-    dsk = dask.array.core.graph_from_arraylike(
-        array,
-        normalized_chunks,
-        shape,
-        name,
-        getitem=GETTER,
-        lock=lock,
-        asarray=asarray,
-        dtype=array.dtype,
-        inline_array=inline_array,
-    )
-    return dask.array.core.Array(dsk,
-                                 name,
-                                 normalized_chunks,
-                                 meta=array,
-                                 dtype=array.dtype)
+        Args:
+            **kwargs: Additional arguments to pass to the persist method.
+
+        Returns:
+            The variable
+        """
+
+    @abc.abstractmethod
+    def compute(self, **kwargs) -> NDArray | NDMaskedArray:
+        """Return the variable data as a numpy array.
+
+        .. note::
+
+            If the variable has a fill value, the result is a masked array where
+            masked values are equal to the fill value.
+
+        Args:
+            **kwargs: Additional arguments to pass to the compute method.
+        """
+
+    @abc.abstractmethod
+    def fill(self: I) -> I:
+        """Fill the variable with the fill value. If the variable has no fill
+        value, this method does nothing.
+
+        Returns:
+            The variable.
+        """
+
+    @classmethod
+    @abc.abstractmethod
+    def from_zarr(cls: type[I], array: zarr.Array, name: str, dimension: str,
+                  **kwargs) -> I:
+        """Create a new variable from a zarr array.
+
+        Args:
+            array: The zarr array
+            name: Name of the variable
+            dimension: Name of the attribute that defines the dimensions of the
+                variable
+            **kwargs: Additional arguments to pass to the method.
+
+        Returns:
+            The variable
+        """
+
+    @abc.abstractmethod
+    def concat(self: I, other: I | Sequence[I], dim: str) -> I:
+        """Concatenate this variable with another variable or a list of
+        variables along a dimension.
+
+        Args:
+            other: Variable or list of variables to concatenate with this
+                variable.
+            dim: Dimension to concatenate along.
+
+        Returns:
+            New variable.
+
+        Raises:
+            ValueError: if the variables provided is an empty sequence.
+        """
+
+    @abc.abstractmethod
+    def __getitem__(self, key: Any) -> Any:
+        """Get a slice of the variable.
+
+        Args:
+            key: Slice or index to use.
+        Returns:
+            The variable slice.
+        """
+
+    @abc.abstractmethod
+    def rechunk(self: I, **kwargs) -> I:
+        """Rechunk the variable.
 
+        Args:
+            **kwargs: Keyword arguments passed to
+                :func:`dask.array.rechunk`
 
-class Variable:
+        Returns:
+            The variable.
+        """
+
+
+class Variable(IVariable):
     """Variables hold multi-dimensional arrays of data.
 
     Args:
         name: Name of the variable
         data: Variable data
         dimensions: Variable dimensions
         attrs: Variable attributes
@@ -298,342 +315,185 @@
         filters: Filters to apply before writing data to disk
     """
     __slots__ = ('array', 'attrs', 'compressor', 'dimensions', 'fill_value',
                  'filters', 'name')
 
     def __init__(self,
                  name: str,
-                 data: ArrayLike[Any],
+                 data: Any,
                  dimensions: Sequence[str],
+                 *,
                  attrs: Sequence[Attribute] | None = None,
                  compressor: numcodecs.abc.Codec | None = None,
                  fill_value: Any | None = None,
                  filters: Sequence[numcodecs.abc.Codec] | None = None) -> None:
-        array, fill_value = _asarray(data, fill_value)
         #: Variable name
-        self.name = name
+        self.name: str = name
         #: Variable data as a dask array.
-        self.array: dask.array.core.Array = array
+        self.array: Any = data
         #: Variable dimensions
-        self.dimensions = dimensions
+        self.dimensions = tuple(dimensions)
         #: Variable attributes
-        self.attrs: Sequence[Attribute] = attrs or tuple()
+        self.attrs = tuple(attrs or ())
         #: Compressor used to compress the data during writing data to disk
-        self.compressor = compressor
+        self.compressor: numcodecs.abc.Codec | None = compressor
         #: Value to use for uninitialized values
-        self.fill_value = fill_value
+        self.fill_value: Any | None = fill_value
         #: Filters to apply before writing data to disk
-        self.filters = filters
+        self.filters = tuple(filters or ())
 
     @property
     def dtype(self) -> numpy.dtype:
-        """Return the data type of the variable."""
+        """Return the dtype of the underlying array."""
         return self.array.dtype
 
     @property
-    def ndim(self) -> int:
-        """Return the number of dimensions of the variable."""
-        return len(self.dimensions)
-
-    @property
     def shape(self) -> tuple[int, ...]:
         """Return the shape of the variable."""
         return self.array.shape
 
     @property
+    def ndim(self) -> int:
+        """Return the number of dimensions of the variable."""
+        return len(self.dimensions)
+
+    @property
     def size(self: Any) -> int:
         """Return the size of the variable."""
         return mathematics.prod(self.shape)
 
     @property
-    def nbytes(self):
+    def nbytes(self) -> int:
         """Return the number of bytes used by the variable."""
         return self.size * self.dtype.itemsize
 
-    def metadata(self) -> meta.Variable:
-        """Get the variable metadata.
-
-        Returns:
-            Variable metadata
-        """
-        return meta.Variable(self.name, self.dtype, self.dimensions,
-                             self.attrs, self.compressor, self.fill_value,
-                             self.filters)
-
-    def persist(self, **kwargs) -> Variable:
-        """Persist the variable data into memory.
+    def duplicate(self: T, data: Any) -> T:
+        """Create a new variable from the properties of this instance and the
+        data provided.
 
         Args:
-            **kwargs: Keyword arguments passed to
-                :meth:`dask.array.Array.persist`.
-
-        Returns:
-            The variable
-        """
-        self.array = dask.base.persist(self.data, **kwargs)  # type: ignore
-        return self
-
-    @property
-    def data(self) -> dask.array.core.Array:
-        """Return the underlying dask array where values equal to the fill
-        value are masked. If no fill value is set, the returned array is the
-        same as the underlying array.
+            data: Variable data.
 
         Returns:
-            The dask array
-
-        .. seealso::
-
-            :meth:`Variable.array`
-        """
-        # If the fill value is None, or if the dask array already holds a
-        # masked array, return the underlying array.
-        # pylint: disable=protected-access
-        # No other way to check if the dask array is a masked array.
-        if (self.fill_value is None
-                or isinstance(self.array._meta, numpy.ma.MaskedArray)):
-            return self.array
-        # pylint: enable=protected-access
-        return dask.array.ma.masked_equal(self.array, self.fill_value)
-
-    @data.setter
-    def data(self, data: Any) -> None:
-        """Defines the underlying dask array. If the data provided is a masked
-        array, it's converted to an array, where the masked values are replaced
-        by its fill value, and its fill value becomes the new fill value of
-        this instance. Otherwise, the underlying array is defined as the new
-        data and the fill value is set to None.
-
-        Args:
-            data: The new data to use
+            New variable.
 
         Raises:
             ValueError: If the shape of the data does not match the shape of
                 the stored data.
         """
-        data, fill_value = _asarray(data, self.fill_value)
-        if len(data.shape) != len(self.dimensions):
+        result: T = type(self)(self.name,
+                               data,
+                               self.dimensions,
+                               attrs=self.attrs,
+                               compressor=self.compressor,
+                               fill_value=self.fill_value,
+                               filters=self.filters)
+        if len(result.shape) != len(self.dimensions):
             raise ValueError('data shape does not match variable dimensions')
-        self.array, self.fill_value = data, fill_value
-
-    @property
-    def values(self) -> NDArray | NDMaskedArray:
-        """Return the variable data as a numpy array.
-
-        .. note::
-
-            If the variable has a fill value, the result is a masked array where
-            masked values are equal to the fill value.
-
-        Returns:
-            The variable data
-        """
-        return self.compute()
-
-    def compute(self, **kwargs) -> NDArray | NDMaskedArray:
-        """Return the variable data as a numpy array.
-
-        .. note::
-
-            If the variable has a fill value, the result is a masked array where
-            masked values are equal to the fill value.
-
-        Args:
-            **kwargs: Keyword arguments passed to
-                :meth:`dask.array.Array.compute`.
-        """
-        try:
-            (values, ) = dask.base.compute(self.array,
-                                           traverse=False,
-                                           **kwargs)
-        except ValueError as exc:
-            msg = str(exc)
-            if 'cannot reshape' in msg or 'buffer too small' in msg:
-                raise ModifiedVariableError() from exc
-            raise
-        return values if self.fill_value is None else numpy.ma.masked_equal(
-            values, self.fill_value)
-
-    def fill(self) -> Variable:
-        """Fill the variable with the fill value. If the variable has no fill
-        value, this method does nothing.
-
-        Returns:
-            The variable.
-        """
-        if self.fill_value is not None:
-            self.array = dask.array.creation.full_like(self.array,
-                                                       self.fill_value)
-        return self
+        return result
 
-    def isel(self, key: tuple[slice, ...]) -> Variable:
+    def isel(self: T, key: tuple[slice, ...]) -> T:
         """Return a new variable with data selected along the given dimension
         indices.
 
         Args:
             key: Dimension indices to select
 
         Returns:
             The new variable
         """
-        return _new_variable(self.name, self.array[key], self.dimensions,
-                             self.attrs, self.compressor, self.fill_value,
-                             self.filters)
-
-    @classmethod
-    def from_zarr(cls, array: zarr.Array, name: str, dimension: str,
-                  **kwargs) -> Variable:
-        """Create a new variable from a zarr array.
+        return new_variable(type(self),
+                            name=self.name,
+                            array=self.array[key],
+                            dimensions=self.dimensions,
+                            attrs=self.attrs,
+                            compressor=self.compressor,
+                            fill_value=self.fill_value,
+                            filters=self.filters)
 
-        Args:
-            array: The zarr array
-            name: Name of the variable
-            dimension: Name of the attribute that defines the dimensions of the
-                variable
-            **kwargs: Keyword arguments passed to
-                :func:`dask.array.from_array`
+    def set_for_insertion(self: T) -> T:
+        """Create a new variable without any attribute.
 
         Returns:
-            The variable
+            The variable.
         """
-        attrs = tuple(
-            Attribute(k, v) for k, v in array.attrs.items() if k != dimension)
-        data = _from_zarr_array(
-            array,
-            array.shape,
-            array.chunks,
-            name=f'{name}-{uuid.uuid1()}',
-            **kwargs,
-        )
-        return _new_variable(name, data, array.attrs[dimension], attrs,
-                             array.compressor, array.fill_value, array.filters)
+        return new_variable(type(self),
+                            name=self.name,
+                            array=self.array,
+                            dimensions=self.dimensions,
+                            attrs=tuple(),
+                            compressor=self.compressor,
+                            fill_value=self.fill_value,
+                            filters=self.filters)
 
-    def duplicate(self, data: Any) -> Variable:
-        """Create a new variable from the properties of this instance and the
-        data provided.
+    def rename(self: T, name: str) -> T:
+        """Rename the variable.
 
         Args:
-            data: Variable data.
-
-        Returns:
-            New variable.
-
-        Raises:
-            ValueError: If the shape of the data does not match the shape of
-                the stored data.
-        """
-        result = Variable(self.name, data, self.dimensions, self.attrs,
-                          self.compressor, self.fill_value, self.filters)
-        if len(result.shape) != len(self.dimensions):
-            raise ValueError('data shape does not match variable dimensions')
-        return result
-
-    def set_for_insertion(self) -> Variable:
-        """Create a new variable without any attribute.
+            name: New variable name.
 
         Returns:
             The variable.
         """
-        return _new_variable(self.name, self.array, self.dimensions, tuple(),
-                             self.compressor, self.fill_value, self.filters)
+        return new_variable(type(self),
+                            name=name,
+                            array=self.array,
+                            dimensions=self.dimensions,
+                            attrs=self.attrs,
+                            compressor=self.compressor,
+                            fill_value=self.fill_value,
+                            filters=self.filters)
 
-    def fill_attrs(self, var: meta.Variable):
+    def fill_attrs(self, var: meta.Variable) -> None:
         """Fill the variable attributes using the provided metadata.
 
         Args:
             var: Variable's metadata.
         """
         self.attrs = var.attrs
 
-    def rename(self, name: str) -> Variable:
-        """Rename the variable.
-
-        Args:
-            name: New variable name.
+    def metadata(self) -> meta.Variable:
+        """Get the variable metadata.
 
         Returns:
-            The variable.
+            Variable metadata
         """
-        return _new_variable(name, self.array, self.dimensions, self.attrs,
-                             self.compressor, self.fill_value, self.filters)
+        return meta.Variable(self.name,
+                             self.dtype,
+                             dimensions=self.dimensions,
+                             attrs=self.attrs,
+                             compressor=self.compressor,
+                             fill_value=self.fill_value,
+                             filters=self.filters)
+
+    def have_same_properties(self, other: Variable) -> bool:
+        """Return true if this instance and the other variable have the same
+        properties."""
+        return self.metadata() == other.metadata()
 
     def dimension_index(self) -> Iterator[tuple[str, int]]:
         """Return an iterator over the variable dimensions and their index.
 
         Returns:
             An iterator over the variable dimensions
         """
         yield from ((item, ix) for ix, item in enumerate(self.dimensions))
 
-    def concat(self, other: Variable | Sequence[Variable],
-               dim: str) -> Variable:
-        """Concatenate this variable with another variable or a list of
-        variables along a dimension.
-
-        Args:
-            other: Variable or list of variables to concatenate with this
-                variable.
-            dim: Dimension to concatenate along.
-
-        Returns:
-            New variable.
-
-        Raises:
-            ValueError: if the variables provided is an empty sequence.
-        """
-        if not isinstance(other, Sequence):
-            other = [other]
-        if not other:
-            raise ValueError('other must be a non-empty sequence')
-        try:
-            axis = self.dimensions.index(dim)
-            return _new_variable(
-                self.name,
-                dask.array.core.concatenate(
-                    (self.array, *(item.array for item in other)), axis=axis),
-                self.dimensions,
-                self.attrs,
-                self.compressor,
-                self.fill_value,
-                self.filters,
-            )
-        except ValueError:
-            # If the concatenation dimension is not within the dimensions of the
-            # variable, then the original variable is returned (i.e.
-            # concatenation is not necessary).
-            return _new_variable(self.name, self.array, self.dimensions,
-                                 self.attrs, self.compressor, self.fill_value,
-                                 self.filters)
-
-    def rechunk(self, **kwargs) -> Variable:
-        """Rechunk the variable.
-
-        Args:
-            **kwargs: Keyword arguments passed to
-                :func:`dask.array.rechunk`
-
-        Returns:
-            The variable.
-        """
-        return _new_variable(self.name, self.array.rechunk(**kwargs),
-                             self.dimensions, self.attrs, self.compressor,
-                             self.fill_value, self.filters)
-
     def to_xarray(self) -> xarray.Variable:
         """Convert the variable to an xarray.Variable.
 
         Returns:
             Variable as an xarray.Variable
         """
-        encoding = {}
+        encoding: dict[str, Any] = {}
         if self.filters:
             encoding['filters'] = self.filters
         if self.compressor:
             encoding['compressor'] = self.compressor
-        data = self.array
+        data: ArrayLike = self.array
         if self.dtype.kind == 'M':
             # xarray need a datetime64[ns] dtype
             data = data.astype('datetime64[ns]')
             encoding['dtype'] = 'int64'
         elif self.dtype.kind == 'm':
             encoding['dtype'] = 'int64'
         attrs = collections.OrderedDict(
@@ -647,74 +507,9 @@
 
     def __repr__(self) -> str:
         return _variable_repr(self)
 
     def __hash__(self) -> int:
         return hash(self.name)
 
-    def __getitem__(self, key: Any) -> Any:
-        return self.data[key]
-
-    def __array__(self):
+    def __array__(self) -> ArrayLike:
         return self.values
-
-    def to_dask_array(self):
-        """Return the underlying dask array.
-
-        Returns:
-            The underlying dask array
-
-        .. seealso::
-
-            :func:`dask.array.asarray`
-        """
-        return self.array
-
-    def __dask_graph__(self) -> Mapping | None:
-        """Return the dask Graph."""
-        return self.array.__dask_graph__()
-
-    def __dask_keys__(self) -> list:
-        """Return the output keys for the Dask graph."""
-        return self.array.__dask_keys__()
-
-    def __dask_layers__(self) -> tuple:
-        """Return the layers for the Dask graph."""
-        return self.array.__dask_layers__()
-
-    def __dask_tokenize__(self):
-        """Return the token for the Dask graph."""
-        return dask.base.normalize_token(
-            (type(self), self.name, self.array, self.dimensions, self.attrs,
-             self.fill_value))
-
-    @staticmethod
-    def __dask_optimize__(dsk: MutableMapping, keys: list,
-                          **kwargs) -> MutableMapping:
-        """Returns whether the Dask graph can be optimized.
-
-        .. seealso::
-            :meth:`dask.array.Array.__dask_optimize__`
-        """
-        return dask.array.core.Array.__dask_optimize__(dsk, keys, **kwargs)
-
-    #: The default scheduler get to use for this object.
-    __dask_scheduler__ = staticmethod(dask.threaded.get)
-
-    def _dask_finalize(self, results, array_func, *args, **kwargs):
-        array = array_func(results, *args, **kwargs)
-        if not isinstance(array, dask.array.core.Array):
-            array = dask.array.core.from_array(array)
-        return _new_variable(self.name, array, self.dimensions, self.attrs,
-                             self.compressor, self.fill_value, self.filters)
-
-    def __dask_postcompute__(self) -> tuple:
-        """Return the finalizer and extra arguments to convert the computed
-        results into their in-memory representation."""
-        array_func, array_args = self.array.__dask_postcompute__()
-        return self._dask_finalize, (array_func, ) + array_args
-
-    def __dask_postpersist__(self) -> tuple:
-        """Return the rebuilder and extra arguments to rebuild an equivalent
-        Dask collection from a persisted or rebuilt graph."""
-        array_func, array_args = self.array.__dask_postpersist__()
-        return self._dask_finalize, (array_func, ) + array_args
```

### Comparing `zcollection-2023.3.2/zcollection/view/__init__.py` & `zcollection-2023.5.0/zcollection/collection/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,740 +1,713 @@
 # Copyright (c) 2023 CNES
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 """
-View on a reference collection.
-===============================
+Collection of Zarr groups
+=========================
 """
 from __future__ import annotations
 
-from typing import Any, ClassVar, Iterable, Iterator
-import copy
+from typing import Any, Iterable, Iterator, Literal, NoReturn, Sequence
+import datetime
+import functools
+import io
 import json
 import logging
-import pathlib
+import os
+import types
 import warnings
 
-import dask.array.core
 import dask.bag.core
 import dask.distributed
 import dask.utils
 import fsspec
+import xarray
 
-from .. import collection, dask_utils, dataset, fs_utils, meta, storage, sync
-from ..collection.detail import try_infer_callable
-from ..convenience import collection as convenience
+from .. import (
+    dask_utils,
+    dataset,
+    fs_utils,
+    merging,
+    meta,
+    partitioning,
+    storage,
+    sync,
+)
+from .abc import PartitionFilter, ReadOnlyCollection
+from .callable_objects import UpdateCallable, WrappedPartitionCallable
 from .detail import (
-    ViewReference,
-    _assert_have_variables,
-    _assert_variable_handled,
-    _create_zarr_array,
-    _deserialize_filters,
-    _drop_zarr_zarr,
-    _load_datasets_list,
-    _load_one_dataset,
-    _select_overlap,
-    _serialize_filters,
-    _sync,
+    _insert,
+    _try_infer_callable,
     _wrap_update_func,
-    _wrap_update_func_overlap,
-    _write_checksum,
+    _wrap_update_func_with_overlap,
 )
 
-__all__ = ['View', 'ViewReference']
-
 #: Module logger.
-_LOGGER = logging.getLogger(__name__)
+_LOGGER: logging.Logger = logging.getLogger(__name__)
+
 
+def _write_immutable_dataset(
+    zds: dataset.Dataset,
+    axis: str,
+    path: str,
+    fs: fsspec.AbstractFileSystem,
+    synchronizer: sync.Sync,
+) -> None:
+    """Write the immutable dataset.
 
-class View:
-    """View on a reference collection.
+    Args:
+        zds: The dataset to write.
+        axis: The partitioning axis.
+        path: The path to the immutable dataset.
+        fs: The file system that the partition is stored on.
+    """
+    immutable_dataset = zds.select_variables_by_dims((axis, ), predicate=False)
+    assert len(immutable_dataset.variables) != 0, (
+        'The dataset to insert does not contain any variable '
+        'that is not split.')
+    _LOGGER.info('Creating the immutable dataset: %s', path)
+    storage.write_zarr_group(immutable_dataset,
+                             path,
+                             fs,
+                             synchronizer,
+                             distributed=False)
+
+
+def _infer_callable(
+    collection: Collection,
+    func: UpdateCallable,
+    filters: PartitionFilter | None,
+    delayed,
+    selected_variables: Iterable[str] | None,
+    *args,
+    **kwargs,
+) -> tuple[str, ...]:
+    try:
+        one_partition: str = next(collection.partitions(filters=filters))
+    except StopIteration:
+        return tuple()
+
+    with collection.synchronizer:
+        zds: dataset.Dataset = storage.open_zarr_group(
+            one_partition,
+            collection.fs,
+            delayed=delayed,
+            selected_variables=selected_variables)
+    func_result: dict[str, Any]
+    func_result = _try_infer_callable(func, zds,
+                                      collection.partition_properties.dim,
+                                      *args, **kwargs)
+    unknown_variables: set[str] = set(func_result) - set(
+        collection.metadata.variables.keys())
+    if len(unknown_variables):
+        raise ValueError(f'Unknown variables: {unknown_variables}')
+    return tuple(func_result)
+
+
+class Collection(ReadOnlyCollection):
+    """This class manages a collection of files in Zarr format stored in a set
+    of subdirectories. These subdirectories split the data, by cycles or dates
+    for example, in order to optimize access and updates, deletion or addition
+    of new data.
 
     Args:
-        base_dir: Path to the directory where the view is stored.
-        view_ref: Access properties for the reference view.
-        ds: The dataset handled by this view.
-        filesystem: The file system used to access the view.
-        filters: The filters used to select the partitions of the reference. If
-            not provided, all partitions are selected.
-        synchronizer: The synchronizer used to synchronize the view.
-
-    .. note::
-
-        Normally, you should not call this constructor directly. Instead, use
-        :func:`create_view <zcollection.create_view>` or :func:`open_view
-        <zcollection.open_view>` to create or open a view.
+        axis: The axis of the collection. This is the dimension along which the
+            data is partitioned.
+        ds: The dataset containing the collection. This dataset is used to
+            create the metadata of the collection, which is used to validate
+            datasets that are inserted in the collection.
+        partition_handler: The partitioning strategy for the collection. This
+            is an instance of a subclass of
+            :py:class:`zarr_partitioning.PartitionHandler`.
+        partition_base_dir: The base directory for the collection. This is the
+            directory where the subdirectories containing the partitioned data
+            are stored.
+        mode: The mode of the collection. This can be either 'r' (read-only) or
+            'w' (write). In read-only mode, the collection can only be read and
+            no data can be inserted or modified. In write mode, the collection
+            can be read and modified.
+        filesystem: The filesystem to use for the collection. This is an
+            instance of a subclass of :py:class:`fsspec.AbstractFileSystem`.
+        synchronizer: The synchronizer to use for the collection. This is an
+            instance of a subclass of
+            :py:class:`zarr_synchronizer.Synchronizer`.
+
+    Raises:
+        ValueError:
+            If the axis does not exist in the dataset, if the partition key is
+            not defined in the dataset or if the access mode is not supported.
+
+    Notes:
+        Normally, this class is not instantiated directly but through the
+        :py:meth:`create_collection <zcollection.create_collection>` and
+        :py:meth:`open_collection <zcollection.open_collection>` methods of this
+        library.
     """
-    #: Configuration filename of the view.
-    CONFIG: ClassVar[str] = '.view'
 
     def __init__(
         self,
-        base_dir: str,
-        view_ref: ViewReference,
+        axis: str,
+        ds: meta.Dataset,
+        partition_handler: partitioning.Partitioning,
+        partition_base_dir: str,
         *,
-        ds: meta.Dataset | None,
+        mode: Literal['r', 'w'] | None = None,
         filesystem: fsspec.AbstractFileSystem | str | None = None,
-        filters: collection.PartitionFilter = None,
         synchronizer: sync.Sync | None = None,
     ) -> None:
-        #: The file system used to access the view (default local file system).
-        self.fs = fs_utils.get_fs(filesystem)
-        #: Path to the directory where the view is stored.
-        self.base_dir = fs_utils.normalize_path(self.fs, base_dir)
-        #: The reference collection of the view.
-        self.view_ref = convenience.open_collection(
-            view_ref.path, mode='r', filesystem=view_ref.filesystem)
-        #: The metadata of the variables handled by the view.
-        self.metadata = ds or meta.Dataset(
-            self.view_ref.metadata.dimensions, variables=[], attrs=[])
-        #: The synchronizer used to synchronize the view.
-        self.synchronizer = synchronizer or sync.NoSync()
-        #: The filters used to select the partitions of the reference.
-        self.filters = filters
-
-        if not self.fs.exists(self.base_dir):
-            _LOGGER.info('Creating view %s', self)
-            self.fs.makedirs(self.base_dir)
-            self._write_config()
-            self._init_partitions(filters)
+        super().__init__(axis=axis,
+                         ds=ds,
+                         partition_handler=partition_handler,
+                         partition_base_dir=partition_base_dir,
+                         mode=mode,
+                         filesystem=filesystem,
+                         synchronizer=synchronizer)
+
+        if self.mode == 'r':
+            # pylint: disable=method-hidden
+            # These methods are overloaded when the collection is opened in
+            # readonly.
+            self._read_only_mode()
+            # pylint: enable=method-hidden
         else:
-            _LOGGER.info('Opening view %s', self)
-
-    def _init_partitions(self, filters: collection.PartitionFilter) -> None:
-        """Initialize the partitions of the view."""
-        _LOGGER.info('Populating view %s', self)
-        args = tuple(
-            map(lambda item: fs_utils.join_path(self.base_dir, item),
-                self.view_ref.partitions(filters=filters, relative=True)))
-        # When opening an existing view, if the user asks to use new partitions
-        # from the reference collection, in this case only the missing
-        # partitions are created.
-        args = tuple(filter(lambda item: not self.fs.exists(item), args))
-        _LOGGER.info('%d partitions selected from %s', len(args),
-                     self.view_ref)
-        client = dask_utils.get_client()
-        storage.execute_transaction(
-            client, self.synchronizer,
-            client.map(
-                _write_checksum,
-                tuple(args),
-                base_dir=self.base_dir,
-                view_ref=self.view_ref,
-                fs=self.fs,
-            ))
+            self._write_config(skip_if_exists=True)
 
     def __str__(self) -> str:
-        return (f'{self.__class__.__name__}'
-                f'<filesystem={self.fs.__class__.__name__!r}, '
-                f'base_dir={self.base_dir!r}>')
+        return (f'<{self.__class__.__name__} '
+                f'filesystem={self.fs.__class__.__name__!r}, '
+                f'partition_base_dir={self.partition_properties.dir!r}'
+                f'mode={self.mode!r}>')
+
+    @staticmethod
+    def _unsupported_operation(*args, **kwargs) -> NoReturn:
+        """Raise an exception if the operation is not supported."""
+        raise io.UnsupportedOperation('not writable')
+
+    def _read_only_mode(self) -> None:
+        """Set the unsupported methods to raise an exception when the
+        collection is opened in read-only mode."""
+        # Set each unsupported method to raise an exception.
+        for item in [
+                'add_variable',
+                'drop_partitions',
+                'drop_variable',
+                'insert',
+                'update',
+        ]:
+            assert hasattr(self, item), f'{item} is not a known method.'
+            setattr(self, item,
+                    types.MethodType(Collection._unsupported_operation, self))
+
+    def _write_config(self, skip_if_exists: bool = False) -> None:
+        """Write the configuration file."""
+        base_dir: str = self.partition_properties.dir
+        config: str = self._config(base_dir)
+        exists: bool = self.fs.exists(config)
+
+        if exists and skip_if_exists:
+            return
+
+        _LOGGER.info(
+            "Updating collection's configuration: %s"
+            if exists else 'Creating the collection: %s', config)
+
+        self.fs.makedirs(base_dir, exist_ok=True)
+
+        params = {
+            'axis': self.axis,
+            'dataset': self.metadata.get_config(),
+            'partitioning': self.partitioning.get_config(),
+        }
 
-    @classmethod
-    def _config(cls, base_dir: str) -> str:
-        """Returns the configuration path."""
-        return fs_utils.join_path(base_dir, cls.CONFIG)
-
-    def _write_config(self) -> None:
-        """Write the configuration file for the view."""
-        config = self._config(self.base_dir)
-        fs = json.loads(self.view_ref.fs.to_json())
         with self.fs.open(config, mode='w') as stream:
-            json.dump(
-                {
-                    'base_dir': self.base_dir,
-                    'filters': _serialize_filters(self.filters),
-                    'metadata': self.metadata.get_config(),
-                    'view_ref': {
-                        'path': self.view_ref.partition_properties.dir,
-                        'fs': fs,
-                    },
-                },
-                stream,  # type: ignore[arg-type]
-                indent=4)
-        self.fs.invalidate_cache(config)
+            json.dump(params, stream, indent=4)  # type: ignore[arg-type]
+
+    def is_readonly(self) -> bool:
+        """Return True if the collection is read-only."""
+        return self.mode == 'r'
 
     @classmethod
     def from_config(
         cls,
         path: str,
         *,
+        mode: Literal['r', 'w'] | None = None,
         filesystem: fsspec.AbstractFileSystem | str | None = None,
         synchronizer: sync.Sync | None = None,
-    ) -> View:
-        """Open a View described by a configuration file.
+    ) -> Collection:
+        """Open a Collection described by a configuration file.
 
         Args:
             path: The path to the configuration file.
-            filesystem: The filesystem to use for the view.
-            synchronizer: The synchronizer to use for the view.
+            mode: The mode of the collection. This can be either 'r'
+                (read-only) or 'w' (write).
+            filesystem: The filesystem to use for the collection. This is an
+                instance of a subclass of
+                :py:class:`fsspec.AbstractFileSystem`.
+            synchronizer: The synchronizer to use for the collection. This is
+                an instance of a subclass of
+                :py:class:`zarr_synchronizer.Synchronizer`.
 
         Returns:
-            The view.
+            The collection.
 
         Raises:
-            ValueError: If the provided directory does not contain a view.
-        """
-        _LOGGER.info('Opening view %r', path)
-        fs = fs_utils.get_fs(filesystem)
-        config = cls._config(path)
+            ValueError:
+                If the provided directory does not contain a valid collection
+                configuration file.
+        """
+        _LOGGER.info('Opening collection: %r', path)
+        fs: fsspec.AbstractFileSystem = fs_utils.get_fs(filesystem)
+        config: str = cls._config(path)
         if not fs.exists(config):
-            raise ValueError(f'zarr view not found at path {path!r}')
+            raise ValueError(f'zarr collection not found at path {path!r}')
         with fs.open(config) as stream:
-            data = json.load(stream)
-
-        view_ref = data['view_ref']
-        return View(data['base_dir'],
-                    ViewReference(
-                        view_ref['path'],
-                        fsspec.AbstractFileSystem.from_json(
-                            json.dumps(view_ref['fs']))),
-                    ds=meta.Dataset.from_config(data['metadata']),
-                    filesystem=filesystem,
-                    filters=_deserialize_filters(data['filters']),
-                    synchronizer=synchronizer)
+            data: dict[str, Any] = json.load(stream)
+        return Collection(
+            data['axis'],
+            meta.Dataset.from_config(data['dataset']),
+            partitioning.get_codecs(data['partitioning']),
+            path,
+            mode=mode or 'r',
+            filesystem=fs,
+            synchronizer=synchronizer,
+        )
 
-    def partitions(
+    # pylint: disable=method-hidden
+    def insert(
         self,
-        filters: collection.PartitionFilter = None,
-    ) -> Iterator[str]:
-        """Returns the list of partitions in the view.
-
-        Args:
-            filters: The partition filters.
-
-        Returns:
-            The list of partitions.
-        """
-        return filter(
-            self.fs.exists,
-            map(lambda item: fs_utils.join_path(self.base_dir, item),
-                self.view_ref.partitions(filters=filters, relative=True)))
-
-    def variables(
-        self,
-        selected_variables: Iterable[str] | None = None
-    ) -> tuple[dataset.Variable, ...]:
-        """Return the variables of the view.
-
-        Args:
-            selected_variables: The variables to return. If None, all the
-                variables are returned.
-
-        Returns:
-            The variables of the view.
-        """
-        return collection.variables(self.metadata, selected_variables)
-
-    def add_variable(
-        self,
-        variable: meta.Variable | dataset.Variable,
+        ds: xarray.Dataset | dataset.Dataset,
+        *,
+        merge_callable: merging.MergeCallable | None = None,
+        npartitions: int | None = None,
+        validate: bool = False,
     ) -> None:
-        """Add a variable to the view.
+        """Insert a dataset into the collection.
 
         Args:
-            variable: The variable to add
+            ds: The dataset to insert. It can be either an xarray.Dataset or a
+                dataset.Dataset object.
+            merge_callable: A function to use to merge the existing data set
+                already stored in partitions with the new partitioned data. If
+                None, the new partitioned data overwrites the existing
+                partitioned data.
+            npartitions: The maximum number of partitions to process in
+                parallel. By default, partitions are processed one by one.
+
+                .. note::
+
+                    When inserting partitions, Dask parallelizes the writing of
+                    each partition across its workers. Additionally, the writing
+                    of variables within a partition is parallelized on the
+                    worker responsible for inserting that partition, using
+                    multiple threads. If you're using a single Dask worker,
+                    partition insertion will happen sequentially and changing
+                    this parameter will have no effect.
 
-        Raises:
-            ValueError: If the variable already exists
+            validate: Whether to validate dataset metadata before insertion
+                or not.
 
-        Example:
-            >>> view.add_variable(
-            ...    zcollection.meta.Variable(
-            ...        "temperature",
-            ...        "float32", ("time", "lat", "lon"),
-            ...        (zcollection.meta.Attribute("units", "degrees Celsius"),
-            ...         zcollection.meta.Attribute("long_name", "temperature")),
-            ...        fill_value=-9999.0))
-        """
-        # pylint: disable=duplicate-code
-        # false positive, no code duplication
-
-        variable = dataset.get_variable_metadata(variable)
-        _LOGGER.info('Adding variable %r in the view', variable.name)
-        if (variable.name in self.view_ref.metadata.variables
-                or variable.name in self.metadata.variables):
-            raise ValueError(f'Variable {variable.name} already exists')
-        client = dask_utils.get_client()
-        self.metadata.add_variable(variable)
-        template = self.view_ref.metadata.search_same_dimensions_as(variable)
-
-        existing_partitions = {
-            pathlib.Path(path).relative_to(self.base_dir).as_posix()
-            for path in self.partitions()
-        }
+        Raises:
+            ValueError:
+                If the dataset does not match the definition of the collection.
 
-        if len(existing_partitions) == 0:
-            _LOGGER.info('No partitions found, skipping variable creation')
-            return
+        Warns:
+            UserWarning:
+                If two different partitions use the same file (chunk), the
+                library that handles the storage of chunked arrays (HDF5,
+                NetCDF, Zarr, etc.) must be compatible with concurrent access.
+
+        Notes:
+            Each worker will process a set of independent partitions. However,
+            be careful, two different partitions can use the same file (chunk),
+            therefore, the library that handles the storage of chunked arrays
+            (HDF5, NetCDF, Zarr, etc.) must be compatible with concurrent
+            access.
+        """
+        # pylint: disable=method-hidden
+        if isinstance(ds, xarray.Dataset):
+            ds = dataset.Dataset.from_xarray(ds)
+
+        _LOGGER.info('Inserting of a %s dataset in the collection',
+                     dask.utils.format_bytes(ds.nbytes))
+
+        missing_variables: tuple[str, ...] = self.metadata.missing_variables(
+            ds.metadata())
+        for item in missing_variables:
+            variable: meta.Variable = self.metadata.variables[item]
+            ds.add_variable(variable)
+
+        if validate and ds.metadata() != self.metadata:
+            raise ValueError(
+                "Provided dataset's metadata do not match the collection's ones"
+            )
+        ds = ds.set_for_insertion(self.metadata)
+        client: dask.distributed.Client = dask_utils.get_client()
 
-        args = filter(lambda item: item[0] in existing_partitions,
-                      self.view_ref.iterate_on_records(relative=True))
-        try:
-            storage.execute_transaction(
-                client, self.synchronizer,
-                client.map(_create_zarr_array,
-                           tuple(args),
-                           base_dir=self.base_dir,
-                           fs=self.fs,
-                           template=template.name,
-                           variable=variable))
-        except Exception:
-            storage.execute_transaction(
-                client, self.synchronizer,
-                client.map(_drop_zarr_zarr,
-                           tuple(self.partitions()),
-                           fs=self.fs,
-                           variable=variable.name,
-                           ignore_errors=True))
-            raise
+        # If the dataset contains variables that should not be partitioned.
+        if self._immutable is not None:
 
-        self._write_config()
-        # pylint: enable=duplicate-code
+            # On the first call, we store the immutable variables in
+            # a directory located at the root of the collection.
+            if not self.fs.exists(self._immutable):
+                _write_immutable_dataset(ds, self.axis, self._immutable,
+                                         self.fs, self.synchronizer)
+
+            # Remove the variables that should not be partitioned.
+            ds = ds.select_variables_by_dims((self.axis, ))
+
+        # Process the partitions to insert or update by batches to avoid
+        # memory issues.
+        partitions = tuple(
+            self.partitioning.split_dataset(ds, self.partition_properties.dim))
+
+        if npartitions is not None:
+            if npartitions < 1:
+                raise ValueError('The number of partitions must be positive')
+            npartitions = len(partitions) // npartitions + 1
+
+        scattered_ds: Any = client.scatter(ds)
+        for sequence in dask_utils.split_sequence(partitions, npartitions):
+            futures: list[dask.distributed.Future] = [
+                dask_utils.simple_delayed('insert', _insert)(
+                    args=partition,  # type: ignore[arg-type]
+                    axis=self.axis,
+                    zds=scattered_ds,
+                    fs=self.fs,
+                    merge_callable=merge_callable,
+                    partitioning_properties=self.partition_properties,
+                ) for partition in sequence
+            ]
+            storage.execute_transaction(client, self.synchronizer, futures)
 
-    def drop_variable(
+    # pylint: disable=method-hidden
+    def drop_partitions(
         self,
-        varname: str,
+        *,
+        filters: PartitionFilter = None,
+        timedelta: datetime.timedelta | None = None,
     ) -> None:
-        """Drop a variable from the view.
+        # pylint: disable=method-hidden
+        """Drop the selected partitions.
 
         Args:
-            varname: The name of the variable to drop.
-
-        Raise:
-            ValueError: If the variable does not exist or if the variable
-                belongs to the reference collection.
+            filters: The predicate used to filter the partitions to drop. To
+                get more information on the predicate, see the documentation of
+                the :meth:`partitions` method.
+            timedelta: Select the partitions created before the specified time
+                delta relative to the current time.
 
         Example:
-            >>> view.drop_variable("temperature")
-        """
-        _LOGGER.info('Dropping variable %r', varname)
-        _assert_variable_handled(self.view_ref.metadata, self.metadata,
-                                 varname)
-        client = dask_utils.get_client()
+            >>> collection.drop_partitions(filters="year == 2019")
+            >>> collection.drop_partitions(
+            ...     timedelta=datetime.timedelta(days=30))
+        """
+        now: datetime.datetime = datetime.datetime.now()
+        client: dask.distributed.Client = dask_utils.get_client()
+        folders = list(self.partitions(filters=filters, lock=True))
 
-        variable = self.metadata.variables.pop(varname)
-        self._write_config()
+        # No partition selected, nothing to do.
+        if not folders:
+            return
+
+        def is_created_before(path: str, now: datetime.datetime,
+                              timedelta: datetime.timedelta) -> bool:
+            """Return whether the partition was created before the
+            timedelta."""
+            created: datetime.datetime = self.fs.created(path)
+            return now - created > timedelta
+
+        if timedelta is not None:
+            folders = list(
+                filter(
+                    lambda folder: is_created_before(  # type: ignore[arg-type]
+                        folder, now, timedelta),
+                    folders))
 
         storage.execute_transaction(
             client, self.synchronizer,
-            client.map(_drop_zarr_zarr,
-                       tuple(self.partitions()),
-                       fs=self.fs,
-                       variable=variable.name))
+            client.map(self.fs.rm, folders, recursive=True))
 
-    def load(
-        self,
-        *,
-        filters: collection.PartitionFilter = None,
-        indexer: collection.Indexer | None = None,
-        selected_variables: Iterable[str] | None = None,
-    ) -> dataset.Dataset | None:
-        """Load the view.
+        def invalidate_cache(path) -> None:
+            """Invalidate the cache."""
+            _LOGGER.info('Dropped partition: %s', path)
+            self.fs.invalidate_cache(path)
 
-        Args:
-            filters: The predicate used to filter the partitions to select.
-                To get more information on the predicate, see the
-                documentation of the :meth:`Collection.partitions
-                <zcollection.collection.Collection.partitions>` method.
-            indexer: The indexer to apply.
-            selected_variables: A list of variables to retain from the view.
-                If None, all variables are loaded.
-
-        Returns:
-            The dataset.
-
-        Example:
-            >>> view.load()
-            >>> view.load(filters="time == '2020-01-01'")
-            >>> view.load(filters=lambda x: x["time"] == "2020-01-01")
-        """
-        _assert_have_variables(self.metadata)
-        if indexer is not None:
-            arguments = tuple(
-                collection.build_indexer_args(self.view_ref,
-                                              filters,
-                                              indexer,
-                                              partitions=self.partitions()))
-            if len(arguments) == 0:
-                return None
-        else:
-            arguments = tuple((self.view_ref.partitioning.parse(item), [])
-                              for item in self.partitions(filters=filters))
-
-        client = dask_utils.get_client()
-        futures = client.map(
-            _load_one_dataset,
-            arguments,
-            base_dir=self.base_dir,
-            fs=self.fs,
-            selected_variables=self.view_ref.metadata.select_variables(
-                selected_variables),
-            view_ref=client.scatter(self.view_ref),
-            variables=self.metadata.select_variables(selected_variables))
-
-        # The load function returns the path to the partitions and the loaded
-        # datasets. Only the loaded datasets are retrieved here and filter None
-        # values corresponding to empty partitions.
-        arrays: list[dataset.Dataset] = list(
-            map(
-                lambda item: item[0],  # type: ignore[arg-type]
-                filter(lambda item: item is not None,
-                       client.gather(futures))))  # type: ignore[arg-type]
-        if arrays:
-            array = arrays.pop(0)
-            if arrays:
-                array = array.concat(arrays,
-                                     self.view_ref.partition_properties.dim)
-            metadata: meta.Dataset = copy.deepcopy(self.view_ref.metadata)
-            metadata.variables.update(self.metadata.variables.items())
-            array.fill_attrs(metadata)
-            return array
-        return None
+        tuple(map(invalidate_cache, folders))
 
+    # pylint: disable=method-hidden
     def update(
         self,
-        func: collection.UpdateCallable,
+        func: UpdateCallable,
         /,
         *args,
+        delayed: bool = True,
         depth: int = 0,
-        filters: collection.PartitionFilter = None,
-        partition_size: int | None = None,
-        selected_variables: Iterable[str] | None = None,
+        filters: PartitionFilter | None = None,
+        npartitions: int | None = None,
+        selected_variables: list[str] | None = None,
+        trim: bool = True,
         **kwargs,
     ) -> None:
-        """Update a variable stored int the view.
+        # pylint: disable=method-hidden
+        """Update the selected partitions.
 
         Args:
-            func: The function to apply to calculate the new values for the
-                target variables.
+            func: The function to apply on each partition.
+            *args: The positional arguments to pass to the function.
+            delayed: Whether to load data in a dask array or not.
             depth: The depth of the overlap between the partitions. Default is
                 0 (no overlap). If depth is greater than 0, the function is
                 applied on the partition and its neighbors selected by the
                 depth. If ``func`` accepts a partition_info as a keyword
                 argument, it will be passed a tuple with the name of the
                 partitioned dimension and the slice allowing getting in the
-                dataset the selected partition without the overlap.
-            filters: The predicate used to filter the partitions to drop.
-                To get more information on the predicate, see the
-                documentation of the :meth:`Collection.partitions
-                <zcollection.collection.Collection.partitions>` method.
-            partition_size: The number of partitions to update in a single
-                batch. By default 1, which is the same as to map the function to
-                each partition. Otherwise, the function is called on a batch of
-                partitions.
-            selected_variables: A list of variables to retain from the view.
-                If None, all variables are loaded. Useful to load only a
-                subset of the view.
-            args: The positional arguments to pass to the function.
-            kwargs: The keyword arguments to pass to the function.
+                dataset the selected partition.
+            filters: The expression used to filter the partitions to update.
+            npartitions: The number of partitions to update in parallel. By
+                default, it is equal to the number of Dask workers available
+                when calling this method.
+            selected_variables: A list of variables to load from the collection.
+                If None, all variables are loaded.
+            trim: Whether to trim ``depth`` items from each partition after
+                calling ``func``. Set it to ``False`` if your function does
+                this for you.
+            **kwargs: The keyword arguments to pass to the function.
 
         Raises:
-            ValueError: If the variable does not exist or if the variable
-                belongs to the reference collection.
+            ValueError: If the variables to update are not in the collection.
 
         Example:
-            >>> def temp_celsius_to_kelvin(
-            ...     dataset: zcollection.dataset.Dataset,
-            ... ) -> Dict[str, numpy.ndarray]:
-            ...     return dict(
-            ...         temperature_kelvin=dataset["temperature"].values + 273,
-            ...         15)
-            >>> view.update(update_temperature)
-        """
-        _assert_have_variables(self.metadata)
+            >>> import dask.array
+            >>> import zcollection
+            >>> def ones(ds):
+            ...     return dict(var2=ds.variables["var1"].values * 0 + 1)
+            >>> collection = zcollection.Collection("my_collection", mode="w")
+            >>> collection.update(ones)
+        """
+        if not callable(func):
+            raise TypeError('func must be a callable')
+
+        variables: tuple[str, ...]
+        variables = _infer_callable(self, func, filters, delayed,
+                                    selected_variables, *args, **kwargs)
+        if not variables:
+            warnings.warn('You are trying to update an empty collection.',
+                          category=RuntimeWarning,
+                          stacklevel=2)
+            return
 
-        client = dask_utils.get_client()
+        # If depth is not 0, the variables updated must be in the selected
+        # variables.
+        if depth != 0 and selected_variables is not None:
+            selected_variables += list(
+                set(variables) - set(selected_variables))
 
-        datasets_list = tuple(
-            _load_datasets_list(client, self.base_dir, self.fs,
-                                self.view_ref, self.metadata,
-                                self.partitions(filters), selected_variables))
-
-        # If no dataset is selected, we have nothing to do.
-        if not datasets_list:
-            warnings.warn('The update function is not applied because no '
-                          'data is selected with the given filters.')
-            return
+        _LOGGER.info('Updating of the (%s) variable in the collection',
+                     ', '.join(repr(item) for item in variables))
 
-        func_result = try_infer_callable(
-            func, datasets_list[0][0], self.view_ref.partition_properties.dim,
-            *args, **kwargs)
-        tuple(
-            map(
-                lambda varname: _assert_variable_handled(
-                    self.view_ref.metadata, self.metadata, varname),
-                func_result))
-        _LOGGER.info('Updating variable %s',
-                     ', '.join(repr(item) for item in func_result))
-
-        # Wrap the function to apply to each partition.
-        if depth == 0:
-            wrap_function = _wrap_update_func(
-                func,
-                self.fs,
-                *args,
-                **kwargs,
-            )
-        else:
-            wrap_function = _wrap_update_func_overlap(
-                datasets_list,
-                depth,
-                func,
-                self.fs,
-                self.view_ref,
+        selected_partitions = tuple(self.partitions(filters=filters,
+                                                    lock=True))
+
+        local_func: WrappedPartitionCallable = _wrap_update_func(
+            *args,
+            delayed=delayed,
+            func=func,
+            fs=self.fs,
+            immutable=self._immutable,
+            selected_variables=selected_variables,
+            **kwargs) if depth == 0 else _wrap_update_func_with_overlap(
                 *args,
-                **kwargs,
-            )
+                delayed=delayed,
+                depth=depth,
+                dim=self.partition_properties.dim,
+                func=func,
+                fs=self.fs,
+                immutable=self._immutable,
+                selected_partitions=selected_partitions,
+                selected_variables=selected_variables,
+                trim=trim,
+                **kwargs)
 
-        batchs = dask_utils.split_sequence(
-            datasets_list, partition_size
+        client: dask.distributed.Client = dask_utils.get_client()
+
+        batches: Iterator[Sequence[str]] = dask_utils.split_sequence(
+            selected_partitions, npartitions
             or dask_utils.dask_workers(client, cores_only=True))
-        awaitables = client.map(wrap_function,
-                                tuple(batchs),
-                                key=func.__name__,
-                                base_dir=self.base_dir)
-        storage.execute_transaction(client, self.synchronizer, awaitables)
+        storage.execute_transaction(
+            client, self.synchronizer,
+            client.map(local_func, tuple(batches), key=func.__name__))
 
-    # pylint: disable=duplicate-code
-    # false positive, no code duplication
-    def map(
+    def drop_variable(
         self,
-        func: collection.MapCallable,
-        *args,
-        filters: collection.PartitionFilter = None,
-        partition_size: int | None = None,
-        npartitions: int | None = None,
-        selected_variables: Iterable[str] | None = None,
-        **kwargs,
-    ) -> dask.bag.core.Bag:
-        """Map a function over the partitions of the view.
+        variable: str,
+    ) -> None:
+        """Delete the variable from the collection.
 
         Args:
-            func: The function to apply to every partition of the view.
-            *args: The positional arguments to pass to the function.
-            filters: The predicate used to filter the partitions to process.
-                To get more information on the predicate, see the
-                documentation of the :meth:`zcollection.Collection.partitions`
-                method.
-            partition_size: The length of each bag partition.
-            npartitions: The number of desired bag partitions.
-            selected_variables: A list of variables to retain from the view.
-                If None, all variables are loaded. Useful to load only a
-                subset of the view.
-            **kwargs: The keyword arguments to pass to the function.
+            variable: The variable to delete.
 
-        Returns:
-            A bag containing the tuple of the partition scheme and the result
-            of the function.
+        Raises:
+            ValueError: If the variable doesn't exist in the collection or is
+                used by the partitioning.
 
         Example:
-            >>> futures = view.map(
-            ...     lambda x: (x["var1"] + x["var2"]).values)
-            >>> for item in futures:
-            ...     print(item)
-            [1.0, 2.0, 3.0, 4.0]
-            [5.0, 6.0, 7.0, 8.0]
-        """
-
-        def _wrap(
-            arguments: tuple[dataset.Dataset, str],
-            func: collection.PartitionCallable,
-            *args,
-            **kwargs,
-        ) -> tuple[tuple[tuple[str, int], ...], Any]:
-            """Wraps the function to apply on the partition.
-
-            Args:
-                arguments: The partition scheme and the dataset.
-                func: The function to apply.
-                *args: The positional arguments to pass to the function.
-                **kwargs: The keyword arguments to pass to the function.
-
-            Returns:
-                The result of the function.
-            """
-            ds, partition = arguments
-            return self.view_ref.partitioning.parse(partition), func(
-                ds, *args, **kwargs)
-
-        _assert_have_variables(self.metadata)
-
-        client = dask_utils.get_client()
-        datasets_list = tuple(
-            _load_datasets_list(client, self.base_dir, self.fs,
-                                self.view_ref, self.metadata,
-                                self.partitions(filters), selected_variables))
-        bag = dask.bag.core.from_sequence(datasets_list,
-                                          partition_size=partition_size,
-                                          npartitions=npartitions)
-        return bag.map(_wrap, func, *args, **kwargs)
-        # pylint: enable=duplicate-code
+            >>> import zcollection
+            >>> collection = zcollection.open_collection(
+            ...     "my_collection", mode="w")
+            >>> collection.drop_variable("my_variable")
+        """
+        _LOGGER.info('Dropping of the %r variable in the collection', variable)
+        if variable in self.partitioning.variables:
+            raise ValueError(
+                f'The variable {variable!r} is part of the partitioning.')
+        if variable not in self.metadata.variables:
+            raise ValueError(
+                f'The variable {variable!r} does not exist in the collection.')
+        if self._immutable:
+            zds: dataset.Dataset = storage.open_zarr_group(
+                self._immutable, self.fs)
+            if variable in zds.variables:
+                raise ValueError(
+                    f'The variable {variable!r} is part of the immutable '
+                    'dataset.')
+        client: dask.distributed.Client = dask_utils.get_client()
+        bag: dask.bag.core.Bag = self._bag_from_partitions(lock=True)
+        awaitables: list[
+            dask.distributed.Future] = dask.distributed.futures_of(
+                bag.map(storage.del_zarr_array, variable, self.fs).persist())
+        storage.execute_transaction(client, self.synchronizer, awaitables)
+        del self.metadata.variables[variable]
+        self._write_config()
 
-    def map_overlap(
+    def add_variable(
         self,
-        func: collection.MapCallable,
-        depth: int,
-        *args,
-        filters: collection.PartitionFilter = None,
-        partition_size: int | None = None,
-        npartitions: int | None = None,
-        selected_variables: Iterable[str] | None = None,
-        **kwargs,
-    ) -> dask.bag.core.Bag:
-        """Map a function over the partitions of the view with some overlap.
+        variable: meta.Variable | dataset.Variable,
+    ) -> None:
+        """Add a variable to the collection.
 
         Args:
-            func: The function to apply to every partition of the view.
-            depth: The depth of the overlap between the partitions. Default is
-                0 (no overlap). If depth is greater than 0, the function is
-                applied on the partition and its neighbors selected by the
-                depth. If ``func`` accepts a partition_info as a keyword
-                argument, it will be passed a tuple with the name of the
-                partitioned dimension and the slice allowing getting in the
-                dataset the selected partition without the overlap.
-            *args: The positional arguments to pass to the function.
-            filters: The predicate used to filter the partitions to process.
-                To get more information on the predicate, see the
-                documentation of the :meth:`zcollection.Collection.partitions`
-                method.
-            partition_size: The length of each bag partition.
-            npartitions: The number of desired bag partitions.
-            selected_variables: A list of variables to retain from the view.
-                If None, all variables are loaded. Useful to load only a
-                subset of the view.
-            **kwargs: The keyword arguments to pass to the function.
+            variable: The variable to add.
 
-        Returns:
-            A bag containing the tuple of the partition scheme and the result
-            of the function.
+        Raises:
+            ValueError: if the variable is already part of the collection, it
+                doesn't use the partitioning dimension or use a dimension that
+                is not part of the dataset.
 
         Example:
-            >>> futures = view.map_overlap(
-            ...     lambda x: (x["var1"] + x["var2"]).values,
-            ...     depth=1)
-            >>> for item in futures:
-            ...     print(item)
-            [1.0, 2.0, 3.0, 4.0]
+            >>> import zcollection
+            >>> collection = zcollection.open_collection(
+            ...     "my_collection", mode="w")
+            >>> new_variable = meta.Variable(
+            ...     name="my_variable",
+            ...     dtype=numpy.dtype("int16"),
+            ...     dimensions=("num_lines", "num_pixels"),
+            ...     fill_value=32267,
+            ...     attrs=(dataset.Attribute(name="my_attr", value=0), ),
+            ... )
+            >>> collection.add_variable(new_variable)
         """
-        if depth < 0:
-            raise ValueError('Depth must be greater than or equal to 0')
-
-        add_partition_info = dask.utils.has_keyword(func, 'partition_info')
-
-        def _wrap(
-            arguments: tuple[dataset.Dataset, str],
-            func: collection.PartitionCallable,
-            datasets_list: tuple[tuple[dataset.Dataset, str]],
-            depth: int,
-            *args,
-            **kwargs,
-        ) -> tuple[tuple[tuple[str, int], ...], Any]:
-            """Wraps the function to apply on the partition.
-
-            Args:
-                arguments: The partition scheme and the dataset.
-                func: The function to apply.
-                datasets: The datasets to apply the function on.
-                depth: The depth of the overlap between the partitions.
-                *args: The positional arguments to pass to the function.
-                **kwargs: The keyword arguments to pass to the function.
-
-            Returns:
-                The result of the function.
-            """
-            ds, indices = _select_overlap(arguments, datasets_list, depth,
-                                          self.view_ref)
-
-            if add_partition_info:
-                kwargs = kwargs.copy()
-                kwargs['partition_info'] = (
-                    self.view_ref.partition_properties.dim, indices)
-
-            # Finally, apply the function.
-            return (self.view_ref.partitioning.parse(arguments[1]),
-                    func(ds, *args, **kwargs))
-
-        _assert_have_variables(self.metadata)
-
-        client = dask_utils.get_client()
-        datasets_list = tuple(
-            _load_datasets_list(client, self.base_dir, self.fs,
-                                self.view_ref, self.metadata,
-                                self.partitions(filters), selected_variables))
-        bag = dask.bag.core.from_sequence(datasets_list,
-                                          partition_size=partition_size,
-                                          npartitions=npartitions)
-        return bag.map(_wrap, func, datasets_list, depth, *args, **kwargs)
-
-    def is_synced(self) -> bool:
-        """Check if the view is synchronized with the underlying collection.
+        variable = dataset.get_variable_metadata(variable)
+        _LOGGER.info('Adding of the %r variable in the collection',
+                     variable.name)
+        if self.partition_properties.dim not in variable.dimensions:
+            raise ValueError(
+                'The new variable must use the partitioning axis.')
+        self.metadata.add_variable(variable)
+        self._write_config()
 
-        Returns:
-            True if the view is synchronized, False otherwise.
-        """
-        partitions = tuple(self.view_ref.partitions(relative=True))
-        client = dask_utils.get_client()
-        unsynchronized_partition = storage.execute_transaction(
-            client, self.synchronizer,
-            client.map(_sync,
-                       partitions,
-                       base_dir=self.base_dir,
-                       fs=self.fs,
-                       view_ref=self.view_ref,
-                       metadata=self.metadata,
-                       dry_run=True))
-        return len(
-            tuple(
-                filter(lambda item: item is not None,
-                       unsynchronized_partition))) == 0
+        # Remove the attribute from the variable. The attribute will be added
+        # from the collection metadata.
+        variable = variable.set_for_insertion()
+
+        client: dask.distributed.Client = dask_utils.get_client()
+
+        template: meta.Variable = self.metadata.search_same_dimensions_as(
+            variable)
+        chunks: dict[str, int] = {
+            dim.name: dim.value
+            for dim in self.metadata.chunks
+        }
+        try:
+            bag: dask.bag.core.Bag = self._bag_from_partitions(lock=True)
+            futures: list[
+                dask.distributed.Future] = dask.distributed.futures_of(
+                    bag.map(storage.add_zarr_array,
+                            variable,
+                            template.name,
+                            self.fs,
+                            chunks=chunks).persist())
+            storage.execute_transaction(client, self.synchronizer, futures)
+        except Exception:
+            self.drop_variable(variable.name)
+            raise
 
-    def sync(
+    def copy(
         self,
-        filters: collection.PartitionFilter = None
-    ) -> collection.PartitionFilterCallback:
-        """Synchronize the view with the underlying collection.
-
-        This method is useful to update the view after a change in the
-        underlying collection.
+        target: str,
+        *,
+        filters: PartitionFilter | None = None,
+        filesystem: fsspec.AbstractFileSystem | None = None,
+        mode: Literal['r', 'w'] = 'w',
+        npartitions: int | None = None,
+        synchronizer: sync.Sync | None = None,
+    ) -> Collection:
+        """Copy the collection to a new location.
 
         Args:
-            filters: The predicate used to select the partitions to
-                synchronize. To get more information on the predicate, see the
-                documentation of the :meth:`zcollection.Collection.partitions`
-                method.
-                If None, the view is synchronized with all the partitions
-                already present in the view. If you want to extend the view
-                with new partitions, use must provide a predicate that
-                selects the new partitions.
-                Existing partitions are not removed, even if they are not
-                selected by the predicate.
+            target: The target location.
+            filters: The predicate used to filter the partitions to copy.
+            filesystem: The file system to use. If None, the file system of the
+                collection is used.
+            mode: The mode used to open the collection copied. Default is 'w'.
+            npartitions: The number of partitions top copy in parallel. Default
+                is number of cores.
+            synchronizer: The synchronizer used to synchronize the collection
+                copied. Default is None.
 
         Returns:
-            A function that can be used as a predicate to get the partitions
-            that have been synchronized using the :meth:`View.partitions`
-            method.
-        """
-        _LOGGER.info('Synchronizing view %s', self)
+            The new collection.
 
-        if filters is not None:
-            self.filters = filters
-            self._write_config()
-            self._init_partitions(filters)
-
-        partitions = tuple(self.view_ref.partitions(relative=True))
-        _LOGGER.info('%d partitions to synchronize', len(partitions))
+        Example:
+            >>> import zcollection
+            >>> collection = zcollection.open_collection(
+            ...     "my_collection", mode="r")
+            >>> collection.copy(target="my_new_collection")
+        """
+        _LOGGER.info('Copying of the collection to %r', target)
+        if filesystem is None:
+            filesystem = fs_utils.get_fs(target)
+        client: dask.distributed.Client = dask_utils.get_client()
+        npartitions = npartitions or dask_utils.dask_workers(client,
+                                                             cores_only=True)
 
-        client = dask_utils.get_client()
-        synchronized_partition = storage.execute_transaction(
-            client, self.synchronizer,
-            client.map(_sync,
-                       partitions,
-                       base_dir=self.base_dir,
-                       fs=self.fs,
-                       view_ref=self.view_ref,
-                       metadata=self.metadata))
-        partition_ids = []
-        for item in filter(lambda item: item is not None,
-                           synchronized_partition):
-            partition_ids.append(dict(self.view_ref.partitioning.parse(item)))
-        return lambda item: item in partition_ids
+        # Sequence of (source, target) to copy split in npartitions
+        args = tuple(
+            dask_utils.split_sequence(
+                [(item,
+                  fs_utils.join_path(
+                      target,
+                      os.path.relpath(item, self.partition_properties.dir)))
+                 for item in self.partitions(filters=filters)], npartitions))
+        # Copy the selected partitions
+        partial = functools.partial(fs_utils.copy_tree,
+                                    fs_source=self.fs,
+                                    fs_target=filesystem)
+
+        def worker_task(args: Sequence[tuple[str, str]]) -> None:
+            """Function call on each worker to copy the partitions."""
+            tuple(map(lambda arg: partial(*arg), args))
+
+        client.gather(client.map(worker_task, args))
+        # Then the remaining files in the root directory (config, metadata,
+        # etc.)
+        fs_utils.copy_files([
+            item['name']
+            for item in self.fs.listdir(self.partition_properties.dir,
+                                        detail=True) if item['type'] == 'file'
+        ], target, self.fs, filesystem)
+        return Collection.from_config(target,
+                                      mode=mode,
+                                      filesystem=filesystem,
+                                      synchronizer=synchronizer)
```

### Comparing `zcollection-2023.3.2/zcollection/view/detail.py` & `zcollection-2023.5.0/zcollection/view/detail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+# Copyright (c) 2023 CNES
+#
+# All rights reserved. Use of this source code is governed by a
+# BSD-style license that can be found in the LICENSE file.
 """
 Implementation details.
 =======================
 """
 from __future__ import annotations
 
-from typing import Callable, Iterable, Iterator, Sequence
+from typing import Callable, Iterable, Iterator, Sequence, Tuple
 import base64
 import dataclasses
 import hashlib
 import io
 import pathlib
 import pickle
 import warnings
@@ -17,23 +21,28 @@
 import dask.bag.core
 import dask.distributed
 import fsspec
 import numpy
 import zarr
 
 from .. import collection, dataset, meta
-from ..collection.detail import update_with_overlap
+from ..collection.detail import _update_with_overlap
 from ..fs_utils import get_fs, join_path
 from ..storage import (
     DIMENSIONS,
     open_zarr_array,
     open_zarr_group,
     update_zarr_array,
     write_zattrs,
 )
+from ..type_hints import ArrayLike, NDArray
+
+#: Type of the function used to update a view.
+ViewUpdateCallable = \
+    Callable[[Iterable[Tuple[dataset.Dataset, str]], str], None]
 
 #: Name of the file that contains the checksum of the view.
 CHECKSUM_FILE = '.checksum'
 
 #: Name of the attribute that contains the checksum of the view.
 CHECKSUM_ATTR = 'checksum'
 
@@ -58,22 +67,23 @@
 
     Args:
         array: Axis values.
         dimension: Name of the dimension.
         checksum: Checksum of the axis values.
     """
     #: Axis values.
-    array: numpy.ndarray
+    array: NDArray
     #: Name of the dimension.
     dimension: str
     #: Checksum of the axis values.
     checksum: str
 
 
 def _create_zarr_array(args: tuple[str, zarr.Group],
+                       *,
                        base_dir: str,
                        fs: fsspec.AbstractFileSystem,
                        template: str,
                        variable: meta.Variable,
                        invalidate_cache: bool = True) -> None:
     """Create a Zarr array, with fill_value being used as the default value for
     uninitialized portions of the array.
@@ -84,19 +94,22 @@
         fs: The filesystem used to create the Zarr array.
         template: The variable's name is used as a template for the Zarr array
             to determine the shape of the new variable.
         variable: The properties of the variable to create.
         invalidate_cache: If True, invalidate the cache of the directory
             containing the Zarr array.
     """
+    partition: str
+    group: zarr.Group
+
     partition, group = args
     data: dask.array.core.Array = dask.array.core.from_zarr(group[template])
 
-    dirname = join_path(base_dir, partition)
-    mapper = fs.get_mapper(join_path(dirname, variable.name))
+    dirname: str = join_path(base_dir, partition)
+    mapper: fsspec.FSMap = fs.get_mapper(join_path(dirname, variable.name))
     zarr.full(data.shape,
               chunks=data.chunksize,
               dtype=variable.dtype,
               compressor=variable.compressor,
               fill_value=variable.fill_value,
               store=mapper,
               overwrite=True,
@@ -128,77 +141,95 @@
         if not ignore_errors:
             raise
     # pylint: enable=broad-except
 
 
 def _load_one_dataset(
     args: tuple[tuple[tuple[str, int], ...], list[slice]],
+    *,
     base_dir: str,
+    delayed: bool,
     fs: fsspec.AbstractFileSystem,
     selected_variables: Iterable[str] | None,
     view_ref: collection.Collection,
     variables: Sequence[str],
 ) -> tuple[dataset.Dataset, str] | None:
     """Load a dataset from a partition stored in the reference collection and
     merge it with the variables defined in this view.
 
     Args:
         args: tuple containing the partition's keys and its indexer.
         base_dir: Base directory of the view.
+        delayed: If True, load the dataset lazily.
         fs: The file system used to access the variables in the view.
         selected_variables: The list of variable to retain from the view
             reference.
         view_ref: The view reference.
         variables: The variables to retain from the view
 
     Returns:
         The dataset and the partition's path.
     """
+    partition_scheme: tuple[tuple[str, int], ...]
+    slices: list[slice]
+
     partition_scheme, slices = args
-    partition = view_ref.partitioning.join(partition_scheme, fs.sep)
-    ds = open_zarr_group(
-        join_path(view_ref.partition_properties.dir, partition), view_ref.fs,
-        selected_variables)
-    if ds is None:
+    partition: str = view_ref.partitioning.join(partition_scheme, fs.sep)
+    zds: dataset.Dataset = open_zarr_group(
+        join_path(view_ref.partition_properties.dir, partition),
+        view_ref.fs,
+        delayed=delayed,
+        selected_variables=selected_variables)
+    if zds is None:
         return None
 
     # If the user has not selected any variables in the reference view. In this
     # case, the dataset is built from all the variables selected in the view.
-    if len(ds.dimensions) == 0:
+    if len(zds.dimensions) == 0:
         return dataset.Dataset(
             [
                 open_zarr_array(
                     zarr.open(  # type: ignore[arg-type]
                         fs.get_mapper(join_path(base_dir, partition,
                                                 variable)),
                         mode='r',
                     ),
-                    variable) for variable in variables
+                    variable,
+                    delayed=delayed) for variable in variables
             ],
-            ds.attrs), partition
+            attrs=zds.attrs), partition
 
-    _ = {
-        ds.add_variable(item.metadata(), item.array)  # type: ignore[arg-type]
+    # pylint: disable=expression-not-assigned
+    # We use the set notation to evaluate the generator.
+    {
+        zds.add_variable(  # type: ignore[func-returns-value]
+            item.metadata(),
+            item.array,
+        )
         for item in (
             open_zarr_array(
                 zarr.open(  # type: ignore[arg-type]
                     fs.get_mapper(join_path(base_dir, partition, variable)),
                     mode='r',
                 ),
-                variable) for variable in variables)
+                variable,
+                delayed=delayed) for variable in variables)
     }
+    # pylint: enable=expression-not-assigned
 
     # Apply indexing if needed.
     if len(slices):
-        dim = view_ref.partition_properties.dim
-        ds_list = [ds.isel({dim: indexer}) for indexer in slices]
-        ds = ds_list.pop(0)
+        dim: str = view_ref.partition_properties.dim
+        ds_list: list[dataset.Dataset] = [
+            zds.isel({dim: indexer}) for indexer in slices
+        ]
+        zds = ds_list.pop(0)
         if ds_list:
-            ds = ds.concat(ds_list, dim)
-    return ds, partition
+            zds = zds.concat(ds_list, dim)
+    return zds, partition
 
 
 def _assert_variable_handled(reference: meta.Dataset, view: meta.Dataset,
                              variable: str) -> None:
     """Assert that a variable belongs to a view.
 
     Args:
@@ -209,42 +240,46 @@
     if variable in reference.variables:
         raise ValueError(f'Variable {variable} is read-only')
     if variable not in view.variables:
         raise ValueError(f'Variable {variable} does not exist')
 
 
 def _load_datasets_list(
+    *,
     client: dask.distributed.Client,
     base_dir: str,
+    delayed: bool,
     fs: fsspec.AbstractFileSystem,
     view_ref: collection.Collection,
     metadata: meta.Dataset,
     partitions: Iterable[str],
     selected_variables: Iterable[str] | None = None,
 ) -> Iterator[tuple[dataset.Dataset, str]]:
     """Load datasets from a list of partitions.
 
     Args:
         client: The client used to load the datasets.
         base_dir: Base directory of the view.
+        delayed: If True, load the dataset lazily.
         fs: The file system used to access the variables in the view.
         view_ref: The view reference.
         metadata: The metadata of the dataset.
         partitions: The list of partitions to load.
         selected_variables: The list of variable to retain from the view
 
     Returns:
         The datasets and their paths.
     """
     arguments: tuple[tuple[tuple[tuple[str, int], ...], list], ...] = tuple(
         (view_ref.partitioning.parse(item), []) for item in partitions)
-    futures = client.map(
+    futures: list[dask.distributed.Future] = client.map(
         _load_one_dataset,
         arguments,
         base_dir=base_dir,
+        delayed=delayed,
         fs=fs,
         selected_variables=view_ref.metadata.select_variables(
             keep_variables=selected_variables),
         view_ref=client.scatter(view_ref),
         variables=metadata.select_variables(selected_variables))
 
     return filter(lambda item: item is not None,
@@ -280,48 +315,48 @@
     """
 
     def calculate_slice(
             selected_datasets: list[tuple[dataset.Dataset, str]]) -> slice:
         """Compute the slice of the selected dataset (without overlap)."""
         start = 0
         indices = slice(0, 0, None)
-        for ds, selected_partition in selected_datasets:
-            size = ds.dimensions[view_ref.partition_properties.dim]
+        for zds, selected_partition in selected_datasets:
+            size = zds.dimensions[view_ref.partition_properties.dim]
             indices = slice(start, start + size, None)
             if partition == selected_partition:
                 break
             start += size
         return indices
 
     # The local function is not taken into account for counting
     # locals.
-    _, partition = arguments
-    where = next(ix for ix, item in enumerate(datasets_list)
-                 if item[1] == partition)
+    partition: str = arguments[1]
+    where: int = next(ix for ix, item in enumerate(datasets_list)
+                      if item[1] == partition)
 
     # Search for the overlapping partitions
-    selected_datasets = [
+    selected_datasets: list[tuple[dataset.Dataset, str]] = [
         datasets_list[ix] for ix in range(where - depth, where + depth + 1)
         if 0 <= ix < len(datasets_list)
     ]
 
     # Build the dataset for the selected partitions.
-    groups = [ds for ds, _ in selected_datasets]
-    ds = groups.pop(0)
-    ds = ds.concat(groups, view_ref.partition_properties.dim)
+    groups: list[dataset.Dataset] = [ds for ds, _ in selected_datasets]
+    zds: dataset.Dataset = groups.pop(0)
+    zds = zds.concat(groups, view_ref.partition_properties.dim)
 
-    return ds, calculate_slice(selected_datasets)
+    return zds, calculate_slice(selected_datasets)
 
 
 def _wrap_update_func(
     func: collection.UpdateCallable,
     fs: fsspec.AbstractFileSystem,
     *args,
     **kwargs,
-) -> Callable[[Iterable[tuple[dataset.Dataset, str]], str], None]:
+) -> ViewUpdateCallable:
     """Wrap an update function taking a list of partition's dataset and
     partition's path as input and returning None.
 
     Args:
         func: The update function.
         fs: The file system used to access the variables in the view.
         *args: The arguments of the update function.
@@ -330,17 +365,17 @@
     Returns:
         The wrapped function.
     """
 
     def wrap_function(parameters: Iterable[tuple[dataset.Dataset, str]],
                       base_dir: str) -> None:
         """Wrap the function to be applied to the dataset."""
-        for ds, partition in parameters:
+        for zds, partition in parameters:
             # Applying function on partition's data
-            dictionary = func(ds, *args, **kwargs)
+            dictionary: dict[str, ArrayLike] = func(zds, *args, **kwargs)
             tuple(
                 update_zarr_array(  # type: ignore[func-returns-value]
                     dirname=join_path(base_dir, partition, varname),
                     array=array,
                     fs=fs,
                 ) for varname, array in dictionary.items())
 
@@ -349,46 +384,61 @@
 
 def _wrap_update_func_overlap(
     datasets_list: tuple[tuple[dataset.Dataset, str], ...],
     depth: int,
     func: collection.UpdateCallable,
     fs: fsspec.AbstractFileSystem,
     view_ref: collection.Collection,
+    trim: bool,
     *args,
     **kwargs,
-) -> Callable[[Iterable[tuple[dataset.Dataset, str]], str], None]:
+) -> ViewUpdateCallable:
     """Wrap an update function taking a list of partition's dataset and
     partition's path as input and returning None.
 
     Args:
         datasets_list: The list of datasets and their paths.
         depth: The depth of the overlap.
         func: The update function.
         fs: The file system used to access the variables in the view.
         view_ref: The view reference.
+        trim: If True, trim the dataset to the overlap.
         *args: The arguments of the update function.
         **kwargs: The keyword arguments of the update function.
 
     Returns:
         The wrapped function.
     """
     dim = view_ref.partition_properties.dim
 
     if depth < 0:
         raise ValueError('The depth must be positive')
 
     def wrap_function(parameters: Iterable[tuple[dataset.Dataset, str]],
                       base_dir: str) -> None:
         """Wrap the function to be applied to the dataset."""
-        for ds, partition in parameters:
-            ds, indices = _select_overlap((ds, partition), datasets_list,
-                                          depth, view_ref)
-            update_with_overlap(func, ds, indices, dim, fs,
-                                join_path(base_dir, partition), *args,
-                                **kwargs)
+        zds: dataset.Dataset
+        indices: slice
+
+        for zds, partition in parameters:
+            zds, indices = _select_overlap((zds, partition), datasets_list,
+                                           depth, view_ref)
+            # pylint: disable=duplicate-code
+            # False positive with the function _wrap_update_func_with_overlap
+            # defined in the module zcollection.collection.detail
+            _update_with_overlap(*args,
+                                 func=func,
+                                 zds=zds,
+                                 indices=indices,
+                                 dim=dim,
+                                 fs=fs,
+                                 path=join_path(base_dir, partition),
+                                 trim=trim,
+                                 **kwargs)
+            # pylint: enable=duplicate-code
 
     return wrap_function
 
 
 def _calculate_axis_reference(
         path: str,
         view_ref: collection.Collection,
@@ -402,19 +452,20 @@
         view_ref: The view reference.
         group: The group to compute the checksum of (if None, the group is
             reload from the file system).
 
     Returns:
         The axis reference of the partition.
     """
+    store: zarr.Group
     store = group or zarr.open_consolidated(  # type: ignore[arg-type]
         view_ref.fs.get_mapper(path), )
     array: zarr.Array = store[view_ref.axis]  # type: ignore[arg-type]
-    axis = array[...]
-    checksum = hashlib.sha256(axis.tobytes()).hexdigest()
+    axis: NDArray = array[...]
+    checksum: str = hashlib.sha256(axis.tobytes()).hexdigest()
     return AxisReference(axis, array.attrs[DIMENSIONS][0], checksum)
 
 
 def _write_checksum_array(
     partition: str,
     fs: fsspec.AbstractFileSystem,
     axis_ref: AxisReference,
@@ -422,18 +473,19 @@
     """Write the checksum of a partition to a file.
 
     Args:
         partition: The path of the partition.
         fs: The file system used to access the variables in the view.
         axis_ref: The axis reference of the partition.
     """
-    checksum_path = join_path(partition, CHECKSUM_FILE)
-    mapper = fs.get_mapper(checksum_path)
+    array: zarr.Array
+    checksum_path: str = join_path(partition, CHECKSUM_FILE)
+    mapper: fsspec.FSMap = fs.get_mapper(checksum_path)
     if fs.exists(checksum_path):
-        array = zarr.open(mapper)
+        array = zarr.open(mapper)  # type: ignore[arg-type]
     else:
         array = zarr.create(shape=axis_ref.array.shape,
                             dtype=axis_ref.array.dtype,
                             store=mapper)
         array.attrs[DIMENSIONS] = axis_ref.dimension
     array[...] = axis_ref.array
     array.attrs[CHECKSUM_ATTR] = axis_ref.checksum
@@ -449,16 +501,16 @@
     Args:
         partition: The path of the partition.
         fs: The file system used to access the variables in the view.
 
     Returns:
         The checksum of the partition and the axis of the reference partition.
     """
-    checksum_path = join_path(partition, CHECKSUM_FILE)
-    mapper = fs.get_mapper(checksum_path)
+    checksum_path: str = join_path(partition, CHECKSUM_FILE)
+    mapper: fsspec.FSMap = fs.get_mapper(checksum_path)
     return zarr.open_array(mapper)
 
 
 def _write_checksum(
     partition: str,
     base_dir: str,
     view_ref: collection.Collection,
@@ -471,15 +523,15 @@
         partition: The path of the partition.
         base_dir: The base directory of the view.
         view_ref: The view reference.
         fs: The file system used to access the variables in the view.
         group: The group to compute the checksum of (if None, the group is
             reload from the file system).
     """
-    partition_ref = join_path(
+    partition_ref: str = join_path(
         view_ref.partition_properties.dir,
         str(pathlib.Path(partition).relative_to(base_dir).as_posix()))
     _write_checksum_array(
         partition, fs,
         _calculate_axis_reference(partition_ref, view_ref, group=group))
 
 
@@ -495,27 +547,28 @@
     Args:
         metadata: The dataset to sync.
         partition: The partition to sync.
         base_dir: The base directory of the view.
         fs: The file system used to access the variables in the view.
         view_ref: The view reference.
     """
-    mapper = view_ref.fs.get_mapper(
+    mapper: fsspec.FSMap = view_ref.fs.get_mapper(
         join_path(view_ref.partition_properties.dir, partition))
     group: zarr.Group = zarr.open_consolidated(  # type: ignore
         mapper, mode='r')
-    path = join_path(base_dir, partition)
+    path: str = join_path(base_dir, partition)
     try:
         for variable in metadata.variables.values():
-            template = view_ref.metadata.search_same_dimensions_as(variable)
+            template: meta.Variable = \
+                view_ref.metadata.search_same_dimensions_as(variable)
             _create_zarr_array((partition, group),
-                               base_dir,
-                               fs,
-                               template.name,
-                               variable,
+                               base_dir=base_dir,
+                               fs=fs,
+                               template=template.name,
+                               variable=variable,
                                invalidate_cache=False)
         _write_checksum(path, base_dir, view_ref, fs, group)
         fs.invalidate_cache(path)
 
     except Exception as exc:
         fs.rm(path, recursive=True)
         fs.invalidate_cache(path)
@@ -530,36 +583,38 @@
     """Sync a partition: create the partition and the underlying variables.
 
     Args:
         partition: The partition to sync.
         fs: The file system used to access the variables in the view.
         axis_ref: The axis reference of the partition.
     """
-    axis_name = axis_ref.dimension
-    new_size = axis_ref.array.shape[0]
+    axis_name: str = axis_ref.dimension
+    new_size: int = axis_ref.array.shape[0]
     try:
         for variable in fs.listdir(partition):
-            array = zarr.open_array(fs.get_mapper(variable['name']))
-            dimensions = array.attrs[DIMENSIONS]
+            array: zarr.Array = zarr.open_array(fs.get_mapper(
+                variable['name']))
+            dimensions: Sequence[str] = array.attrs[DIMENSIONS]
             if axis_name in dimensions:
-                axis = dimensions.index(axis_name)
+                axis: int = dimensions.index(axis_name)
                 shape = list(array.shape)
                 shape[axis] = new_size
                 array.resize(shape)
         _write_checksum_array(partition, fs, axis_ref)
         # fs.invalidate_cache(partition) is not done by
         # _write_checksum_array
     except Exception as exc:
         fs.rm(partition, recursive=True)
         fs.invalidate_cache(partition)
         raise exc from None
 
 
 def _sync(
     partition: str,
+    *,
     base_dir: str,
     fs: fsspec.AbstractFileSystem,
     view_ref: collection.Collection,
     metadata: meta.Dataset,
     dry_run: bool = False,
 ) -> str | None:
     """Sync the partitions of a view.
@@ -571,33 +626,35 @@
         view_ref: The view reference.
         metadata: The dataset to sync.
         dry_run: If True, the partition is not synced.
 
     Returns:
         The partition synced or None if the partition is already synced.
     """
-    partition_view = join_path(base_dir, partition)
+    partition_view: str = join_path(base_dir, partition)
     if not fs.exists(partition_view):
         # The partition does not exist, so we create it.
         if not dry_run:
             _sync_partition(metadata, partition, base_dir, fs, view_ref)
         return partition
 
     # The partition exists, so we check if it is synced.
-    partition_ref = join_path(view_ref.partition_properties.dir, partition)
-    array = _load_checksum_array(partition_view, fs)
-    axis_ref = _calculate_axis_reference(partition_ref, view_ref)
+    partition_ref: str = join_path(view_ref.partition_properties.dir,
+                                   partition)
+    array: zarr.Array = _load_checksum_array(partition_view, fs)
+    axis_ref: AxisReference = _calculate_axis_reference(
+        partition_ref, view_ref)
     # If the checksums are different, the partition is not synced. So we
     # remove it (information between the partition and the reference are
     # not consistent)
     if axis_ref.checksum != array.attrs[CHECKSUM_ATTR]:
         # If the checksums are different, the partition is not synced. we load
         # the axis of partition's view to check if the partition is a subset of
         # the reference partition.
-        axis_view = array[:]
+        axis_view: NDArray = array[:]
         if axis_ref.array.size > axis_view.size and numpy.all(
                 axis_view == axis_ref.array[:axis_view.size]):
             # The view partition is a subset of the reference partition.
             # So we extend the view partition to the reference partition.
             # fs_invalid_cache is done by _extend_partition
             if not dry_run:
                 _extend_partition(partition_view, fs, axis_ref)
```

### Comparing `zcollection-2023.3.2/zcollection/view/tests/test_view.py` & `zcollection-2023.5.0/zcollection/view/tests/test_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,41 +17,45 @@
 # pylint: disable=unused-import # Need to import for fixtures
 from ...tests.cluster import dask_client, dask_cluster
 from ...tests.data import (
     create_test_collection,
     create_test_dataset,
     make_dataset,
 )
+from ...tests.fixture import dask_arrays, numpy_arrays
 from ...tests.fs import local_fs, s3, s3_base, s3_fs
 from ...view.detail import _calculate_axis_reference
 
 # pylint: enable=unused-import
 
 
-@pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('fs', ['local_fs', 's3_fs'])
+@pytest.mark.parametrize('arrays_type', ['dask_arrays', 'numpy_arrays'])
 def test_view(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-    arg,
+    fs,
+    arrays_type,
     request,
 ):
     """Test the creation of a view."""
-    tested_fs = request.getfixturevalue(arg)
+    tested_fs = request.getfixturevalue(fs)
+    delayed = request.getfixturevalue(arrays_type)
 
-    create_test_collection(tested_fs)
+    create_test_collection(tested_fs, delayed=False)
     instance = convenience.create_view(str(tested_fs.view),
                                        view.ViewReference(
                                            str(tested_fs.collection),
                                            tested_fs.fs),
                                        filesystem=tested_fs.fs)
     assert isinstance(instance, view.View)
     assert isinstance(str(instance), str)
 
     # No variable recorded, so no data can be loaded
     with pytest.raises(ValueError):
-        instance.load()
+        instance.load(delayed=delayed)
 
     var = meta.Variable(
         name='var2',
         dtype=numpy.float64,
         dimensions=('num_lines', 'num_pixels'),
         attrs=(meta.Attribute(name='attr', value=1), ),
     )
@@ -63,87 +67,87 @@
     instance.add_variable(var)
 
     with pytest.raises(ValueError):
         instance.add_variable(var)
 
     instance = convenience.open_view(str(tested_fs.view),
                                      filesystem=tested_fs.fs)
-    ds = instance.load()
-    assert ds is not None
-    assert set(ds['time'].values.astype('datetime64[D]')) == {
+    zds = instance.load(delayed=delayed)
+    assert zds is not None
+    assert set(zds['time'].values.astype('datetime64[D]')) == {
         numpy.datetime64('2000-01-01'),
         numpy.datetime64('2000-01-04'),
         numpy.datetime64('2000-01-07'),
         numpy.datetime64('2000-01-10'),
         numpy.datetime64('2000-01-13'),
         numpy.datetime64('2000-01-16'),
     }
 
     # Loading a variable existing only in the view.
-    ds = instance.load(selected_variables=('var3', ))
-    assert ds is not None
-    assert tuple(ds.variables) == ('var3', )
-    assert 'var3' in ds.metadata().variables.keys()
+    zds = instance.load(delayed=delayed, selected_variables=('var3', ))
+    assert zds is not None
+    assert tuple(zds.variables) == ('var3', )
+    assert 'var3' in zds.metadata().variables.keys()
 
     # The metadata of the reference collection is not modified.
     assert 'var3' not in instance.view_ref.metadata.variables.keys()
 
     # Loading a non existing variable.
-    ds = instance.load(selected_variables=('var55', ))
-    assert ds is not None
-    assert len(ds.variables) == 0
+    zds = instance.load(delayed=delayed, selected_variables=('var55', ))
+    assert zds is not None
+    assert len(zds.variables) == 0
 
     # Test view loading that is no longer synchronized with the reference
     # collection.
     tested_fs.fs.rm(str(
         tested_fs.view.joinpath('year=2000', 'month=01', 'day=13')),
                     recursive=True)
 
     assert len(tuple(instance.partitions())) == 5
     assert len(tuple(instance.view_ref.partitions())) == 6
 
-    ds = instance.load()
-    assert ds is not None
-    assert set(ds['time'].values.astype('datetime64[D]')) == {
+    zds = instance.load(delayed=delayed)
+    assert zds is not None
+    assert set(zds['time'].values.astype('datetime64[D]')) == {
         numpy.datetime64('2000-01-01'),
         numpy.datetime64('2000-01-04'),
         numpy.datetime64('2000-01-07'),
         numpy.datetime64('2000-01-10'),
         numpy.datetime64('2000-01-16'),
     }
 
     # Create a variable with the unsynchronized view
     var.name = 'var4'
     instance.add_variable(var)
 
-    ds = instance.load()
-    assert ds is not None
+    zds = instance.load(delayed=delayed)
+    assert zds is not None
 
-    def update(ds, varname):
+    def update(zds, varname):
         """Update function used for this test."""
-        return {varname: ds.variables['var1'].values * 0 + 5}
+        return {varname: zds.variables['var1'].values * 0 + 5}
 
-    instance.update(update, 'var3')  # type: ignore
+    instance.update(update, 'var3', delayed=delayed)  # type: ignore
 
     with pytest.raises(ValueError):
         instance.update(update, 'varX')  # type: ignore
 
     with pytest.raises(ValueError):
         instance.update(update, 'var2')  # type: ignore
 
-    ds = instance.load()
-    assert ds is not None
-    numpy.all(ds.variables['var3'].values == 5)
+    zds = instance.load(delayed=delayed)
+    assert zds is not None
+    numpy.all(zds.variables['var3'].values == 5)
 
     indexers = instance.map(
         lambda x: slice(0, x.dimensions['num_lines'])  # type: ignore
     ).compute()
-    ds1 = instance.load(indexer=indexers)
+    ds1 = instance.load(delayed=delayed, indexer=indexers)
     assert ds1 is not None
-    ds2 = instance.load()
+    ds2 = instance.load(delayed=delayed)
     assert ds2 is not None
 
     assert numpy.allclose(ds1.variables['var1'].values,
                           ds2.variables['var1'].values)
 
     instance.drop_variable('var3')
 
@@ -177,30 +181,54 @@
         name='var3',
         dtype=numpy.int8,
         dimensions=('num_lines', 'num_pixels'),
     )
 
     instance.add_variable(var)
 
-    def update(ds, varname, partition_info: tuple[str, slice]):
+    def update(zds, varname, partition_info: tuple[str, slice],
+               trim_result: bool) -> dict[str, numpy.ndarray]:
         """Update function used for this test."""
         assert isinstance(partition_info, tuple)
         assert len(partition_info) == 2
         assert isinstance(partition_info[0], str)
         assert isinstance(partition_info[1], slice)
         assert partition_info[0] == 'num_lines'
-        return {varname: ds.variables['var1'].values * 1 + 5}
-
-    instance.update(update, 'var3', depth=1)  # type: ignore
+        if trim_result:
+            zds = zds.isel(dict((partition_info, )))
+        return {varname: zds.variables['var1'].values * 1 + 5}
+
+    instance.update(
+        update,  # type: ignore
+        'var3',
+        depth=1,
+        trim_result=False)
+    zds = instance.load()
+    assert zds is not None
+    numpy.all(zds.variables['var3'].values == 5)
+
+    instance.update(
+        update,  # type: ignore
+        'var3',
+        depth=1,
+        trim=False,
+        trim_result=True)
+    zds = instance.load()
+    assert zds is not None
+    numpy.all(zds.variables['var3'].values == 5)
 
-    ds = instance.load()
-    assert ds is not None
-    numpy.all(ds.variables['var3'].values == 5)
+    with pytest.raises(ValueError):
+        instance.update(
+            update,  #  type: ignore
+            'var3',
+            depth=1,
+            trim_result=False,
+            selected_variables=('var1', ))
 
-    def map_func(x, partition_info: tuple[str, slice]):
+    def map_func(_, partition_info: tuple[str, slice]):
         """Map function used for this test."""
         assert isinstance(partition_info, tuple)
         assert len(partition_info) == 2
         assert isinstance(partition_info[0], str)
         assert isinstance(partition_info[1], slice)
         assert partition_info[0] == 'num_lines'
         return partition_info
@@ -215,30 +243,31 @@
         assert len(data) == 2
         assert isinstance(data[0], str)
         assert isinstance(data[1], slice)
 
 
 def test_view_checksum(
         dask_client,  # pylint: disable=redefined-outer-name,unused-argument
-        tmpdir):
-    ds = next(create_test_dataset())
-    zcollection = collection.Collection('time', ds.metadata(),
+        tmpdir) -> None:
+    """Test the checksum calculation."""
+    zds = next(create_test_dataset())
+    zcollection = collection.Collection('time', zds.metadata(),
                                         partitioning.Date(('time', ), 'D'),
                                         str(tmpdir))
 
-    zcollection.insert(ds)
+    zcollection.insert(zds)
     partition = tmpdir / 'year=2000' / 'month=01' / 'day=01'
     axis_ref = _calculate_axis_reference(str(partition), zcollection)
     assert isinstance(axis_ref.array, numpy.ndarray)
     assert isinstance(axis_ref.checksum, str)
     assert isinstance(axis_ref.dimension, str)
     assert len(axis_ref.checksum) == 64
     assert axis_ref.dimension == 'num_lines'
-    assert axis_ref.checksum == ('4bbb9253c07f36002098f8bba57151eb'
-                                 '0143f5fe5c634950340f3e2f1a4f51cf')
+    assert axis_ref.checksum == ('1a1727b18e729c376442e76d806565b8'
+                                 '359e3af9c93572af3e5fe8980ced6956')
 
 
 @pytest.mark.filterwarnings('ignore:.*cannot be serialized.*')
 @pytest.mark.parametrize('arg', ['local_fs', 's3_fs'])
 def test_view_sync(
     dask_client,  # pylint: disable=redefined-outer-name,unused-argument
     arg,
@@ -254,29 +283,29 @@
                                        filesystem=tested_fs.fs)
     var = meta.Variable(name='var3',
                         dtype=numpy.float64,
                         dimensions=('num_lines', 'num_pixels'))
     instance.add_variable(var)
     del instance
 
-    collection = convenience.open_collection(str(tested_fs.collection),
-                                             filesystem=tested_fs.fs,
-                                             mode='w')
-    ds = collection.load(filters=lambda keys: keys['year'] == 2000 and keys[
+    zcollection = convenience.open_collection(str(tested_fs.collection),
+                                              filesystem=tested_fs.fs,
+                                              mode='w')
+    zds = zcollection.load(filters=lambda keys: keys['year'] == 2000 and keys[
         'month'] == 1 and keys['day'] == 16)
-    assert ds is not None
+    assert zds is not None
     dates = numpy.arange(numpy.datetime64('2000-01-16'),
                          numpy.datetime64('2000-01-16T23:59:59'),
                          numpy.timedelta64(1, 'h'))
-    ds = make_dataset(
-        dates,
-        numpy.ones((len(dates), ds.dimensions['num_pixels']),
-                   dtype=numpy.float64))
-    collection.insert(ds)
-    del collection
+    zds = make_dataset(
+        dates.astype('M8[ns]'),
+        numpy.ones((len(dates), zds.dimensions['num_pixels']),
+                   dtype=numpy.int64))
+    zcollection.insert(zds)
+    del zcollection
     instance = convenience.open_view(str(tested_fs.view),
                                      filesystem=tested_fs.fs)
     assert instance is not None
     assert instance.is_synced() is False
     instance.sync(filters=lambda keys: True)
-    ds = instance.load()
-    assert ds is not None
+    zds = instance.load()
+    assert zds is not None
```

### Comparing `zcollection-2023.3.2/zcollection.egg-info/PKG-INFO` & `zcollection-2023.5.0/zcollection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcollection
-Version: 2023.3.2
+Version: 2023.5.0
 Summary: Zarr Collection
 Home-page: https://github.com/CNES/zcollection
 Author: CNES/CLS
 Author-email: fbriol@gmail.com
 License: BSD License
 Keywords: zarr,collection,xarray,dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `zcollection-2023.3.2/zcollection.egg-info/SOURCES.txt` & `zcollection-2023.5.0/zcollection.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 ./zcollection/conftest.py
 ./zcollection/dask_utils.py
 ./zcollection/dataset.py
 ./zcollection/expression.py
 ./zcollection/fs_utils.py
 ./zcollection/mathematics.py
 ./zcollection/meta.py
+./zcollection/representation.py
 ./zcollection/storage.py
 ./zcollection/sync.py
 ./zcollection/type_hints.py
-./zcollection/variable.py
 ./zcollection/version.py
 ./zcollection/collection/__init__.py
+./zcollection/collection/abc.py
 ./zcollection/collection/callable_objects.py
 ./zcollection/collection/detail.py
 ./zcollection/collection/tests/__init__.py
 ./zcollection/collection/tests/test_collection.py
 ./zcollection/convenience/__init__.py
 ./zcollection/convenience/collection.py
 ./zcollection/convenience/view.py
@@ -51,27 +52,37 @@
 ./zcollection/partitioning/tests/test_date.py
 ./zcollection/partitioning/tests/test_registry.py
 ./zcollection/partitioning/tests/test_sequence.py
 ./zcollection/tests/__init__.py
 ./zcollection/tests/cluster.py
 ./zcollection/tests/data.py
 ./zcollection/tests/first_dataset.json
+./zcollection/tests/fixture.py
 ./zcollection/tests/fs.py
 ./zcollection/tests/s3.py
 ./zcollection/tests/second_dataset.json
 ./zcollection/tests/test_compressed_array.py
 ./zcollection/tests/test_dask_utils.py
 ./zcollection/tests/test_dataset.py
 ./zcollection/tests/test_expression.py
 ./zcollection/tests/test_fs_utils.py
 ./zcollection/tests/test_mathematics.py
 ./zcollection/tests/test_meta.py
 ./zcollection/tests/test_storage.py
 ./zcollection/tests/test_sync.py
-./zcollection/tests/test_variable.py
+./zcollection/variable/__init__.py
+./zcollection/variable/abc.py
+./zcollection/variable/array.py
+./zcollection/variable/delayed_array.py
+./zcollection/variable/tests/__init__.py
+./zcollection/variable/tests/data.py
+./zcollection/variable/tests/test_abc.py
+./zcollection/variable/tests/test_array.py
+./zcollection/variable/tests/test_delayed_array.py
+./zcollection/variable/tests/test_variable.py
 ./zcollection/view/__init__.py
 ./zcollection/view/detail.py
 ./zcollection/view/tests/__init__.py
 ./zcollection/view/tests/test_view.py
 .github/workflows/ci.yaml
 .github/workflows/pre-commit.yml
 .github/workflows/pypipublish.yaml
@@ -98,25 +109,26 @@
 zcollection/compressed_array.py
 zcollection/dask_utils.py
 zcollection/dataset.py
 zcollection/expression.py
 zcollection/fs_utils.py
 zcollection/mathematics.py
 zcollection/meta.py
+zcollection/representation.py
 zcollection/storage.py
 zcollection/sync.py
 zcollection/type_hints.py
-zcollection/variable.py
 zcollection.egg-info/PKG-INFO
 zcollection.egg-info/SOURCES.txt
 zcollection.egg-info/dependency_links.txt
 zcollection.egg-info/not-zip-safe
 zcollection.egg-info/requires.txt
 zcollection.egg-info/top_level.txt
 zcollection/collection/__init__.py
+zcollection/collection/abc.py
 zcollection/collection/callable_objects.py
 zcollection/collection/detail.py
 zcollection/collection/tests/__init__.py
 zcollection/collection/tests/test_collection.py
 zcollection/convenience/__init__.py
 zcollection/convenience/collection.py
 zcollection/convenience/view.py
@@ -141,24 +153,34 @@
 zcollection/partitioning/tests/test_date.py
 zcollection/partitioning/tests/test_registry.py
 zcollection/partitioning/tests/test_sequence.py
 zcollection/tests/__init__.py
 zcollection/tests/cluster.py
 zcollection/tests/data.py
 zcollection/tests/first_dataset.json
+zcollection/tests/fixture.py
 zcollection/tests/fs.py
 zcollection/tests/s3.py
 zcollection/tests/second_dataset.json
 zcollection/tests/test_compressed_array.py
 zcollection/tests/test_dask_utils.py
 zcollection/tests/test_dataset.py
 zcollection/tests/test_expression.py
 zcollection/tests/test_fs_utils.py
 zcollection/tests/test_mathematics.py
 zcollection/tests/test_meta.py
 zcollection/tests/test_storage.py
 zcollection/tests/test_sync.py
-zcollection/tests/test_variable.py
+zcollection/variable/__init__.py
+zcollection/variable/abc.py
+zcollection/variable/array.py
+zcollection/variable/delayed_array.py
+zcollection/variable/tests/__init__.py
+zcollection/variable/tests/data.py
+zcollection/variable/tests/test_abc.py
+zcollection/variable/tests/test_array.py
+zcollection/variable/tests/test_delayed_array.py
+zcollection/variable/tests/test_variable.py
 zcollection/view/__init__.py
 zcollection/view/detail.py
 zcollection/view/tests/__init__.py
 zcollection/view/tests/test_view.py
```

