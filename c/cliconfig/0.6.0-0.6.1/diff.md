# Comparing `tmp/cliconfig-0.6.0.tar.gz` & `tmp/cliconfig-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.6.0.tar", last modified: Sun May 14 17:38:18 2023, max compression
+gzip compressed data, was "cliconfig-0.6.1.tar", last modified: Sun May 14 23:41:45 2023, max compression
```

## Comparing `cliconfig-0.6.0.tar` & `cliconfig-0.6.1.tar`

### file list

```diff
@@ -1,117 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.783929 cliconfig-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.787929 cliconfig-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-14 17:38:03.000000 cliconfig-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 17:38:03.000000 cliconfig-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-14 17:38:18.799929 cliconfig-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-14 17:38:03.000000 cliconfig-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-14 17:38:03.000000 cliconfig-0.6.0/README_pypi.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.791929 cliconfig-0.6.0/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.791929 cliconfig-0.6.0/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.791929 cliconfig-0.6.0/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/cliconfig.processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 17:38:03.000000 cliconfig-0.6.0/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-14 17:38:03.000000 cliconfig-0.6.0/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-14 17:38:03.000000 cliconfig-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-14 17:38:03.000000 cliconfig-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 17:38:03.000000 cliconfig-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:38:18.799929 cliconfig-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 17:38:03.000000 cliconfig-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.787929 cliconfig-0.6.0/tests/configs/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/tests/configs/integration/test1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test1/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test1/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test1/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/configs/integration/test2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/exp1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/exp2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/configs/integration/test2/models/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/models/resnet100.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/models/resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/models/vit_b16.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/processing/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_ex_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.514143 cliconfig-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.522143 cliconfig-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-14 23:41:26.000000 cliconfig-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 23:41:26.000000 cliconfig-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-14 23:41:45.530142 cliconfig-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-14 23:41:26.000000 cliconfig-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-14 23:41:26.000000 cliconfig-0.6.1/README_pypi.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.522143 cliconfig-0.6.1/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.522143 cliconfig-0.6.1/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.522143 cliconfig-0.6.1/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/cliconfig.processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 23:41:26.000000 cliconfig-0.6.1/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-14 23:41:26.000000 cliconfig-0.6.1/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-14 23:41:26.000000 cliconfig-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-14 23:41:26.000000 cliconfig-0.6.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 23:41:26.000000 cliconfig-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 23:41:45.530142 cliconfig-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 23:41:26.000000 cliconfig-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/tests/configs/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/delete/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/delete/config2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.518143 cliconfig-0.6.1/tests/configs/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/tests/configs/integration/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test1/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test1/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test1/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/configs/integration/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/exp1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/exp2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/exp3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/configs/integration/test2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/models/resnet100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/models/resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/models/vit_b16.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/processing/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_ex_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-0.6.0/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.6.1/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/.github/workflows/pydocstyle.yaml` & `cliconfig-0.6.1/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/.github/workflows/pylint.yaml` & `cliconfig-0.6.1/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/.github/workflows/tests.yaml` & `cliconfig-0.6.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/.pylintrc` & `cliconfig-0.6.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/CONTRIBUTING.md` & `cliconfig-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/LICENSE` & `cliconfig-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/PKG-INFO` & `cliconfig-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.6.0
+Version: 0.6.1
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -86,15 +86,15 @@
 
 For instance with these config files:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
-config3.select@select: "config3.param1"
+config3.select@select: config3.param1
 
 --- # sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
 --- # sub2.yaml
@@ -111,15 +111,15 @@
 path_2: sub2.yaml
 config1:
   param: 2  # the value of config2.param
   param2: 1
 config2:
   param: 2
 config3:
-  select: "config3.param1"
+  select: config3.param1
   param1: 0
   # param2 is deleted because it is not in the selection
 ```
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
```

### Comparing `cliconfig-0.6.0/README.md` & `cliconfig-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -144,27 +144,31 @@
   after each update, even if the tag is no longer present. It supports basic types
   (except for tuples and sets, which are not handled by YAML) as well as unions
   (using "Union" or "|"), optional values, nested list, and nested dict.
   For instance: `@type:List[Dict[str, int|float]]`.
 * `@select`: This tag select sub-config(s) to keep and delete the other
   sub-configs in the same parent config. The tagged key is not deleted if it is
   in the parent config.
+* `@delete`: This tag deletes the key from the config on pre-merge. It is useful
+  to activate a processing without having a good name for the key to add in
+  the default config.
 
-The tags are applied in the following order: `@merge`, `@copy`, and then `@type`.
+The tags are applied in the following order: `@merge`, `@select`, `@copy`, `@type`
+and then `@delete`.
 
 Please note that the tags serve as triggers for internal processing and will be
 automatically removed from the key after processing.
 
 It is also possible to combine multiple tags. For example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
-config3.select@select: "config3.param1"
+config3.select@select: config3.param1
 
 --- # sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
 --- # sub2.yaml
@@ -181,15 +185,15 @@
 path_2: sub2.yaml
 config1:
   param: 2  # the value of config2.param
   param2: 1
 config2:
   param: 2
 config3:
-  select: "config3.param1"
+  select: config3.param1
   param1: 0
   # param2 is deleted because it is not in the selection
 ```
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
@@ -245,18 +249,24 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
+* [x] Continue `test_multi_tags2` integration test with cases that raise errors, and
+  pre-save processing.
+* [ ] Support multi-files in yaml file (with separator "---")
+
 Secondary:
 
-* [ ] Add a `@delete` tag to delete a key from the config after pre-merge. Useful to make
+* [x] Add a `@delete` tag to delete a key from the config after pre-merge. Useful to make
   processing action without introducing new keys in the config.
+* [x] Set a default value to True if no value are specified for parameter in command line.
+* [ ] Support yaml tags "!tag" in config files
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.6.0/README_pypi.md` & `cliconfig-0.6.1/README_pypi.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 For instance with these config files:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
-config3.select@select: "config3.param1"
+config3.select@select: config3.param1
 
 --- # sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
 --- # sub2.yaml
@@ -99,15 +99,15 @@
 path_2: sub2.yaml
 config1:
   param: 2  # the value of config2.param
   param2: 1
 config2:
   param: 2
 config3:
-  select: "config3.param1"
+  select: config3.param1
   param1: 0
   # param2 is deleted because it is not in the selection
 ```
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
```

### Comparing `cliconfig-0.6.0/cliconfig/__init__.py` & `cliconfig-0.6.1/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/cliconfig/cli_parser.py` & `cliconfig-0.6.1/cliconfig/cli_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,15 +59,17 @@
             i += 2
         elif elem.startswith("--"):
             splits = elem.split("=", maxsplit=1)
             if len(splits) == 2:
                 key, value_str = splits
             else:
                 key = splits[0]
-                value_str = "null"
+                # If no value is provided, use True because it could
+                # be seen as a flag
+                value_str = "true"
             key = key[2:]
             value = yaml.safe_load(value_str)
             cli_params_dict[key] = value
             i += 1
         else:  # Not a config parameter
             i += 1
     return config_paths, cli_params_dict
```

### Comparing `cliconfig-0.6.0/cliconfig/config_routines.py` & `cliconfig-0.6.1/cliconfig/config_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/cliconfig/dict_routines.py` & `cliconfig-0.6.1/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/cliconfig/process_routines.py` & `cliconfig-0.6.1/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/cliconfig/processing/_type_parser.py` & `cliconfig-0.6.1/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/cliconfig/processing/base.py` & `cliconfig-0.6.1/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/cliconfig/processing/builtin.py` & `cliconfig-0.6.1/cliconfig/processing/builtin.py`

 * *Files 4% similar despite different names*

```diff
@@ -252,19 +252,21 @@
                 self.current_value[key] = flat_config.dict[val]
         return flat_config
 
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing."""
         # Restore the tag with the key to copy to keep the information
         # on further loading
-        for key, val in self.keys_to_copy.items():
-            if key in flat_config.dict:
+        keys = list(flat_config.dict.keys())
+        for key in keys:
+            clean_key = clean_all_tags(key)
+            if clean_key in self.keys_to_copy:
                 new_key = key + "@copy"
                 del flat_config.dict[key]
-                flat_config.dict[new_key] = val
+                flat_config.dict[new_key] = self.keys_to_copy[clean_key]
         return flat_config
 
 
 class ProcessTyping(Processing):
     """Force a type with '@type:mytype' tag. The type is preserved forever.
 
     Allow basic types (none, any, bool, int, float, str, list, dict), nested lists,
@@ -348,17 +350,19 @@
                 )
         return flat_config
 
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing."""
         # Restore the tag with the type to keep the information
         # on further loading
-        for key, val in self.type_desc.items():
-            if key in flat_config.dict:
-                new_key = key + f"@type:{val}"
+        keys = list(flat_config.dict.keys())
+        for key in keys:
+            clean_key = clean_all_tags(key)
+            if clean_key in self.type_desc:
+                new_key = key + f"@type:{self.type_desc[clean_key]}"
                 flat_config.dict[new_key] = flat_config.dict[key]
                 del flat_config.dict[key]
         return flat_config
 
 
 class ProcessSelect(Processing):
     """Select a sub-config with and delete the rest of its parent config.
@@ -464,22 +468,78 @@
                     del flat_config.dict[key]
         return super().postmerge(flat_config)
 
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing."""
         # Restore the tag with the type to keep the information
         # on further loading
-        for key in self.keys_that_select:
-            if key in flat_config.dict:
+        keys = list(flat_config.dict.keys())
+        for key in keys:
+            clean_key = clean_all_tags(key)
+            if clean_key in self.keys_that_select:
                 new_key = key + "@select"
                 flat_config.dict[new_key] = flat_config.dict[key]
                 del flat_config.dict[key]
         return flat_config
 
 
+class ProcessDelete(Processing):
+    """Delete the parameters tagged with @delete on pre-merge.
+
+    This processing is applied late on pre-merge to allow the others processing
+    to be applied before deleting the parameters. It is usefull to activate a
+    processing without add an additional parameter in the default configuration
+    to void the error on merge with allow_new_keys=False.
+
+    Examples
+    --------
+    .. code-block:: yaml
+
+        # main.yaml
+        1@select@delete: configs.config1
+        2@merge_add@delete: config1.yaml
+        3@merge_add@delete: config2.yaml
+
+        --- # config1.yaml
+        configs.config1.param: 1
+        configs.config1.param2: 2
+
+        --- # config2.yaml
+        configs.config2.param: 3
+        configs.config2.param: 4
+
+    Here we want to merge two config files and select one sub-config.
+    We use the corresponding tags but we don't have a good name for the keys
+    and instead of adding a new parameter in the default configuration with
+    random names like "1", "2", "3", we use the @delete tag to delete the
+    keys after the pre-merge processing.
+    Pre-merge processing: 25.0
+
+    Warning
+    -------
+        The parameter is deleted on pre-merge so if the parameter already exists
+        on the other configuration during merge, this parameter will be remain
+        as it is. This processing is more used to delete parameter that is NOT
+        present in the default configuration.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+        # After all pre-merge processing
+        self.premerge_order = 25.0
+
+    def premerge(self, flat_config: Config) -> Config:
+        """Pre-merge processing."""
+        keys = list(flat_config.dict.keys())
+        for key in keys:
+            if is_tag_in(key, "delete"):
+                del flat_config.dict[key]
+        return flat_config
+
+
 class ProcessCheckTags(Processing):
     """Raise an error if a tag is present in a key after pre-merging processes.
 
     This security processing is applied after all pre-merge process and
     checks for "@" in the keys. It raises an error if one is found.
     """
 
@@ -521,17 +581,20 @@
      * ProcessMerge (@merge_all, @merge_before, @merge_after): merge multiple
        files into one.
      * ProcessCopy (@copy): persistently copy a value from one key to an other
        and protect it
      * ProcessTyping (@type:X): force the type of parameter to any type X.
      * ProcessSelect (@select): select sub-config(s) to keep and delete the
        other sub-configs in the same parent config.
+     * ProcessDelete (@delete): delete the parameter tagged with @delete on
+       pre-merge.
     """
 
     def __init__(self) -> None:
         self.list: List[Processing] = [
             ProcessCheckTags(),
             ProcessMerge(),
             ProcessCopy(),
             ProcessTyping(),
-            ProcessSelect()
+            ProcessSelect(),
+            ProcessDelete(),
         ]
```

### Comparing `cliconfig-0.6.0/cliconfig/processing/create.py` & `cliconfig-0.6.1/cliconfig/processing/create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/cliconfig/tag_routines.py` & `cliconfig-0.6.1/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.6.1/cliconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.6.0
+Version: 0.6.1
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -86,15 +86,15 @@
 
 For instance with these config files:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
-config3.select@select: "config3.param1"
+config3.select@select: config3.param1
 
 --- # sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
 --- # sub2.yaml
@@ -111,15 +111,15 @@
 path_2: sub2.yaml
 config1:
   param: 2  # the value of config2.param
   param2: 1
 config2:
   param: 2
 config3:
-  select: "config3.param1"
+  select: config3.param1
   param1: 0
   # param2 is deleted because it is not in the selection
 ```
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
```

### Comparing `cliconfig-0.6.0/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.6.1/cliconfig.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,21 +62,24 @@
 tests/conftest.py
 tests/configs/config1.yaml
 tests/configs/config2.yaml
 tests/configs/configtag1.yaml
 tests/configs/configtag2.yaml
 tests/configs/default1.yaml
 tests/configs/default2.yaml
+tests/configs/delete/config1.yaml
+tests/configs/delete/config2.yaml
 tests/configs/integration/test1/main.yaml
 tests/configs/integration/test1/sub1.yaml
 tests/configs/integration/test1/sub2.yaml
 tests/configs/integration/test2/data.yaml
 tests/configs/integration/test2/default.yaml
 tests/configs/integration/test2/exp1.yaml
 tests/configs/integration/test2/exp2.yaml
+tests/configs/integration/test2/exp3.yaml
 tests/configs/integration/test2/models/resnet100.yaml
 tests/configs/integration/test2/models/resnet50.yaml
 tests/configs/integration/test2/models/vit_b16.yaml
 tests/configs/merge/additional1.yaml
 tests/configs/merge/additional2.yaml
 tests/configs/merge/additional3.yaml
 tests/configs/merge/default1.yaml
```

### Comparing `cliconfig-0.6.0/docs/Makefile` & `cliconfig-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/_static/logo.png` & `cliconfig-0.6.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/_static/logo_extend.png` & `cliconfig-0.6.1/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/cliconfig_api.rst` & `cliconfig-0.6.1/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/conf.py` & `cliconfig-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/edge_cases.md` & `cliconfig-0.6.1/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/index.rst` & `cliconfig-0.6.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 For instance with these config files:
 
 .. code:: yaml
 
     ---  # main.yaml
     path_1@merge_add: sub1.yaml
     path_2@merge_add: sub2.yaml
-    config3.select@select: "config3.param1"
+    config3.select@select: config3.param1
 
     --- # sub1.yaml
     config1:
       param@copy@type:int: config2.param
       param2@type:None|int: 1
 
     --- # sub2.yaml
@@ -80,15 +80,15 @@
     path_2: sub2.yaml
     config1:
       param: 2  # the value of config2.param
       param2: 1
     config2:
       param: 2
     config3:
-      select: "config3.param1"
+      select: config3.param1
       param1: 0
       # param2 is deleted because it is not in the selection
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
```

### Comparing `cliconfig-0.6.0/docs/license.md` & `cliconfig-0.6.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/make.bat` & `cliconfig-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/processing.md` & `cliconfig-0.6.1/docs/processing.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/docs/quickstart.md` & `cliconfig-0.6.1/docs/quickstart.md`

 * *Files 4% similar despite different names*

```diff
@@ -101,28 +101,31 @@
 * `@type:<my type>`: This tag checks if the key matches the specified type `<my type>`
   after each update, even if the tag is no longer present. It supports basic types
   (except for tuples and sets, which are not handled by YAML) as well as unions
   (using "Union" or "|"), optional values, nested list, and nested dict.
   For instance: `@type:List[Dict[str, int|float]]`.
 * `@select`: This tag select sub-config(s) to keep and delete the other
   sub-configs in the same parent config
+* `@delete`: This tag deletes the key from the config on pre-merge. It is useful
+  to activate a processing without having a good name for the key to add in
+  the default config.
 
-The tags are applied in the following order: `@merge`, `@select`, `@copy`,
-and then `@type`.
+The tags are applied in the following order: `@merge`, `@select`, `@copy`, `@type`
+and then `@delete`.
 
 Please note that the tags serve as triggers for internal processing and will be
 automatically removed from the key after processing.
 
 It is also possible to combine multiple tags. For example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
-config3.select@select: "config3.param1"
+config3.select@select: config3.param1
 
 --- # sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
 --- # sub2.yaml
@@ -139,15 +142,15 @@
 path_2: sub2.yaml
 config1:
   param: 2  # the value of config2.param
   param2: 1
 config2:
   param: 2
 config3:
-  select: "config3.param1"
+  select: config3.param1
   param1: 0
   # param2 is deleted because it is not in the selection
 ```
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config1.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
```

### Comparing `cliconfig-0.6.0/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.6.1/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/github_actions_utils/pylint_manager.py` & `cliconfig-0.6.1/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/github_actions_utils/pytest_manager.py` & `cliconfig-0.6.1/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.6.1/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/pre-commit-checks.sh` & `cliconfig-0.6.1/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/pyproject.toml` & `cliconfig-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/configs/integration/test2/default.yaml` & `cliconfig-0.6.1/tests/configs/integration/test2/default.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/conftest.py` & `cliconfig-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/integration/test_inte_multiple_tags.py` & `cliconfig-0.6.1/tests/integration/test_inte_multiple_tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Integration test for multiple tags."""
 import random
+import shutil
 import sys
 from copy import deepcopy
 
 import pytest
 import pytest_check as check
 
 from cliconfig import (
     Config,
     create_processing_keep_property,
     create_processing_value,
+    load_config,
     make_config,
+    save_config,
 )
+from cliconfig.dict_routines import load_dict
 from cliconfig.process_routines import merge_flat_processing
 
 
 def test_multiple_tags() -> None:
     """Integration test for multiple tags."""
     sys_argv = sys.argv.copy()
     sys.argv = ["test_inte_multiple_tags.py"]
@@ -115,17 +119,50 @@
             "augmentation": ["RandomHorizontalFlip", "RandomVerticalFlip"],
             "dataset_cfg_path": "tests/configs/integration/test2/data.yaml",
         },
         "train": {
             "n_epochs": 20,
             "optimizer": {
                 "type": "Adam",
-                "lr": 0.01,
+                "lr": 0.001,
                 "momentum": 0,
             },
         },
     }
     check.is_instance(config.dict["run_id"], int)
     config_dict = deepcopy(config.dict)
     del config_dict["run_id"]
     check.equal(config_dict, expected_dict)
+    save_config(config, "tests/tmp/config.yaml")
+    saved_dict = load_dict("tests/tmp/config.yaml")
+    check.equal(
+        saved_dict["data"]["augmentation@type:List[str]"],
+        ["RandomHorizontalFlip", "RandomVerticalFlip"]
+    )
+    check.equal(
+        saved_dict["models"]["archi_name@type:None|str@select"],
+        "models.vit_b16"
+    )
+    check.equal(
+        saved_dict["models"]["vit_b16"]["in_size@type:int@copy"],
+        "data.data_size"
+    )
+    config = load_config(
+        "tests/tmp/config.yaml",
+        ["tests/configs/integration/test2/default.yaml"],
+        config.process_list
+    )
+    del config.dict["run_id"]
+    check.equal(config.dict, expected_dict)
+    with pytest.raises(
+        ValueError,
+        match="Key previously tagged with '@type:int.*"
+    ):
+        merge_flat_processing(config, Config({'models.vit_b16.n_blocks': 5.6}, []))
+    with pytest.raises(
+        ValueError,
+        match="Found attempt to modify a key with '@copy' tag.*"
+    ):
+        merge_flat_processing(config, Config({'models.vit_b16.in_size': 224}, []))
+
+    shutil.rmtree("tests/tmp")
     sys.argv = sys_argv
```

### Comparing `cliconfig-0.6.0/tests/unit/processing/test_base.py` & `cliconfig-0.6.1/tests/unit/processing/test_base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/unit/processing/test_builtin.py` & `cliconfig-0.6.1/tests/unit/processing/test_builtin.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from cliconfig.base import Config
 from cliconfig.dict_routines import flatten
 from cliconfig.processing.builtin import (
     DefaultProcessings,
     ProcessCheckTags,
     ProcessCopy,
+    ProcessDelete,
     ProcessMerge,
     ProcessSelect,
     ProcessTyping,
 )
 
 
 def test_process_merge() -> None:
@@ -279,14 +280,29 @@
             "flat key with a least one dot on parameter tagged with @select. "
             "Find key: p@select with value: root"
         )
     ):
         processing.premerge(Config({"p@select": "root"}, []))
 
 
+def test_process_delete() -> None:
+    """Test ProcessDelete."""
+    processing = ProcessDelete()
+    config = Config(
+        {
+            "@select@delete": "configs.config1",
+            "1@merge_add@delete": "config1.yaml",
+            "2@merge_add@delete": "config2.yaml",
+        },
+        [processing],
+    )
+    config = processing.premerge(config)
+    check.equal(config.dict, {})
+
+
 def test_process_check_tags() -> None:
     """Test ProcessCheckTags."""
     processing = ProcessCheckTags()
     flat_dict = {
         "config.param1": 1,
         "param1": 2,
     }
```

### Comparing `cliconfig-0.6.0/tests/unit/processing/test_create.py` & `cliconfig-0.6.1/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/unit/processing/test_type_parser.py` & `cliconfig-0.6.1/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/unit/test_cli_parser.py` & `cliconfig-0.6.1/tests/unit/test_cli_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,12 +25,12 @@
         "b": {"2": {"3": 4, "5": [6.3], "7": True, "8": None, "9": [2, {"a": 1}]}},
     }
     check.equal(config_paths, [])
     check.equal(config_cli_params, val)
     config_paths, config_cli_params = parse_cli(
         ["main.py", "--unknown", "--a=1", "--unknwon2=2", "--b=3"]
     )
-    val2 = {"unknown": None, "a": 1, "unknwon2": 2, "b": 3}
+    val2 = {"unknown": True, "a": 1, "unknwon2": 2, "b": 3}
     check.equal(config_paths, [])
     check.equal(config_cli_params, val2)
     with pytest.raises(ValueError, match="Only one '--config ' argument is allowed.*"):
         parse_cli(["main.py", "--config", "config1.yaml", "--config", "config2.yaml"])
```

### Comparing `cliconfig-0.6.0/tests/unit/test_config_routines.py` & `cliconfig-0.6.1/tests/unit/test_config_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/unit/test_dict_routines.py` & `cliconfig-0.6.1/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/unit/test_ex_docs.py` & `cliconfig-0.6.1/tests/unit/test_ex_docs.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/unit/test_process_routines.py` & `cliconfig-0.6.1/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.0/tests/unit/test_tag_routines.py` & `cliconfig-0.6.1/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*

