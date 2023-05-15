# Comparing `tmp/cliconfig-0.6.1.tar.gz` & `tmp/cliconfig-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.6.1.tar", last modified: Sun May 14 23:41:45 2023, max compression
+gzip compressed data, was "cliconfig-0.6.2.tar", last modified: Mon May 15 17:16:22 2023, max compression
```

## Comparing `cliconfig-0.6.1.tar` & `cliconfig-0.6.2.tar`

### file list

```diff
@@ -1,121 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.514143 cliconfig-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.522143 cliconfig-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-14 23:41:26.000000 cliconfig-0.6.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-14 23:41:26.000000 cliconfig-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 23:41:26.000000 cliconfig-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-14 23:41:45.530142 cliconfig-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-14 23:41:26.000000 cliconfig-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-14 23:41:26.000000 cliconfig-0.6.1/README_pypi.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.522143 cliconfig-0.6.1/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.522143 cliconfig-0.6.1/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-14 23:41:26.000000 cliconfig-0.6.1/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.522143 cliconfig-0.6.1/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 23:41:45.000000 cliconfig-0.6.1/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/cliconfig.processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-14 23:41:26.000000 cliconfig-0.6.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 23:41:26.000000 cliconfig-0.6.1/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 23:41:26.000000 cliconfig-0.6.1/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-14 23:41:26.000000 cliconfig-0.6.1/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-14 23:41:26.000000 cliconfig-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-14 23:41:26.000000 cliconfig-0.6.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 23:41:26.000000 cliconfig-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 23:41:45.530142 cliconfig-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 23:41:26.000000 cliconfig-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/tests/configs/delete/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/delete/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/delete/config2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.518143 cliconfig-0.6.1/tests/configs/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.526142 cliconfig-0.6.1/tests/configs/integration/test1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test1/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test1/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test1/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/configs/integration/test2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/exp1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/exp2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/exp3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/configs/integration/test2/models/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/models/resnet100.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/models/resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/integration/test2/models/vit_b16.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:41:45.530142 cliconfig-0.6.1/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/processing/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_ex_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-14 23:41:26.000000 cliconfig-0.6.1/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.843564 cliconfig-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.823564 cliconfig-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.827564 cliconfig-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-15 17:15:57.000000 cliconfig-0.6.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-15 17:15:57.000000 cliconfig-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-15 17:15:57.000000 cliconfig-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-15 17:16:22.843564 cliconfig-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-05-15 17:15:57.000000 cliconfig-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-15 17:15:57.000000 cliconfig-0.6.2/README_pypi.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.831564 cliconfig-0.6.2/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 17:16:22.000000 cliconfig-0.6.2/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.831564 cliconfig-0.6.2/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-15 17:15:57.000000 cliconfig-0.6.2/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.831564 cliconfig-0.6.2/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-15 17:16:22.000000 cliconfig-0.6.2/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-15 17:16:22.000000 cliconfig-0.6.2/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:16:22.000000 cliconfig-0.6.2/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 17:16:22.000000 cliconfig-0.6.2/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 17:16:22.000000 cliconfig-0.6.2/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.835564 cliconfig-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.835564 cliconfig-0.6.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/cliconfig.processing_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    15754 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 17:15:57.000000 cliconfig-0.6.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.835564 cliconfig-0.6.2/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 17:15:57.000000 cliconfig-0.6.2/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-15 17:15:57.000000 cliconfig-0.6.2/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-15 17:15:57.000000 cliconfig-0.6.2/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-15 17:15:57.000000 cliconfig-0.6.2/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-15 17:15:57.000000 cliconfig-0.6.2/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.835564 cliconfig-0.6.2/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 17:15:57.000000 cliconfig-0.6.2/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-15 17:15:57.000000 cliconfig-0.6.2/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-15 17:15:57.000000 cliconfig-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-15 17:15:57.000000 cliconfig-0.6.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 17:15:57.000000 cliconfig-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:16:22.843564 cliconfig-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 17:15:57.000000 cliconfig-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.835564 cliconfig-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.839564 cliconfig-0.6.2/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.839564 cliconfig-0.6.2/tests/configs/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/delete/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/delete/config2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.823564 cliconfig-0.6.2/tests/configs/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.839564 cliconfig-0.6.2/tests/configs/integration/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test1/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test1/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test1/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.839564 cliconfig-0.6.2/tests/configs/integration/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test2/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test2/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test2/exp1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test2/exp2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test2/exp3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.839564 cliconfig-0.6.2/tests/configs/integration/test2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test2/models/resnet100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test2/models/resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/integration/test2/models/vit_b16.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.843564 cliconfig-0.6.2/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/configs/multi_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.843564 cliconfig-0.6.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.843564 cliconfig-0.6.2/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:22.843564 cliconfig-0.6.2/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/processing/test_base_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/test_config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/test_ex_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-15 17:15:57.000000 cliconfig-0.6.2/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-0.6.1/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.6.2/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/.github/workflows/pydocstyle.yaml` & `cliconfig-0.6.2/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/.github/workflows/pylint.yaml` & `cliconfig-0.6.2/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/.github/workflows/tests.yaml` & `cliconfig-0.6.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/.pylintrc` & `cliconfig-0.6.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/CONTRIBUTING.md` & `cliconfig-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/LICENSE` & `cliconfig-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/PKG-INFO` & `cliconfig-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.6.1
+Version: 0.6.2
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -83,25 +83,25 @@
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 ```yaml
----  # main.yaml
+# main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 config3.select@select: config3.param1
 
---- # sub1.yaml
+# sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
---- # sub2.yaml
+# sub2.yaml
 config2.param@type:None|int: 2
 config3:
   param1: 0
   param2: 1
 ```
 
 Here `main.yaml` is interpreted like:
```

### Comparing `cliconfig-0.6.1/README.md` & `cliconfig-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 ## Quick start
 
 Create a default configuration that can be split across multiple files that will
 be merged in sequence. There is no depth limit for the
 configuration parameters.
 
 ```yaml
----  # default1.yaml
+# default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
   letter2: b
 
----  # default2.yaml
+# default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
 Now you can write these following lines in your python program to use this config
 with `make_config`:
@@ -71,19 +71,19 @@
 config.dict  # the configuration as a dict
 ```
 
 Then you can add one or multiple additional config files that will be passed on
 command line and that will override the default values.
 
 ```yaml
----  # first.yaml
+# first.yaml
 letters:
   letter3: C  # equivalent to "letters.letter3: "C"
 
----  # second.yaml
+# second.yaml
 param1: -1
 letters.letter1: A
 ```
 
 **Please note that the additional config files must not introduce new parameters that
 are not in the default configs, as it will result in an error**. This
 restriction is in place to prevent potential typos in the config files from
@@ -116,14 +116,18 @@
         letter1: A
         letter2: B
         letter3: C
 ```
 
 Note that the configurations is stored as native python dict at each step of the process.
 
+You can also use multiple documents in a single YAML file with the `---` separator. In
+this case, the documents are merged in sequence and the file is interpreted as a single
+additional config file containing this merged configuration.
+
 ## Use tags
 
 By default, the package provides some "tags" represented as strings that start with
 '@' and are placed at the end of a key containing a parameter. These tags change
 the way the configuration is processed.
 
 The default tags include:
@@ -157,25 +161,25 @@
 
 Please note that the tags serve as triggers for internal processing and will be
 automatically removed from the key after processing.
 
 It is also possible to combine multiple tags. For example:
 
 ```yaml
----  # main.yaml
+# main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 config3.select@select: config3.param1
 
---- # sub1.yaml
+# sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
---- # sub2.yaml
+# sub2.yaml
 config2.param@type:None|int: 2
 config3:
   param1: 0
   param2: 1
 ```
 
 Here `main.yaml` is interpreted like:
@@ -251,22 +255,26 @@
 
 ## Todo
 
 Priority:
 
 * [x] Continue `test_multi_tags2` integration test with cases that raise errors, and
   pre-save processing.
-* [ ] Support multi-files in yaml file (with separator "---")
+* [x] Support multi-files in yaml file (with separator "---")
+* [ ] Fix mistakes in all docstrings (🚧  in progress)
 
 Secondary:
 
 * [x] Add a `@delete` tag to delete a key from the config after pre-merge. Useful to make
   processing action without introducing new keys in the config.
 * [x] Set a default value to True if no value are specified for parameter in command line.
-* [ ] Support yaml tags "!tag" in config files
+
+Only if PR from other people:
+
+* [ ] Support yaml tags "!tag" in config files.
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.6.1/README_pypi.md` & `cliconfig-0.6.2/cliconfig.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: cliconfig
+Version: 0.6.2
+Summary: Merge your config files and set parameters from the command line in a simple way.
+Author-email: Valentin Goldite <valentin.goldite@gmail.com>
+Project-URL: Source, https://github.com/valentingol/cliconfig
+Keywords: logging,machine,learning
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CLI Config
 
 </p>
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
@@ -71,25 +83,25 @@
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 ```yaml
----  # main.yaml
+# main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 config3.select@select: config3.param1
 
---- # sub1.yaml
+# sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
---- # sub2.yaml
+# sub2.yaml
 config2.param@type:None|int: 2
 config3:
   param1: 0
   param2: 1
 ```
 
 Here `main.yaml` is interpreted like:
```

### Comparing `cliconfig-0.6.1/cliconfig/__init__.py` & `cliconfig-0.6.2/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/cliconfig/cli_parser.py` & `cliconfig-0.6.2/cliconfig/cli_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,46 +3,49 @@
 
 import yaml
 
 
 def parse_cli(sys_argv: List[str]) -> Tuple[List[str], Dict[str, Any]]:
     """Parser for CLI commands.
 
-    Return list of config paths that are detected with `--config ` (with a space),
-    separated by commas without space (or in a list).
-    Return also a dictionary of parameters from CLI detected with --<key>=<value>
-    (with "=" and without spaces).
+    Return list of config path(s) that are detected with ``--config`` followed
+    by a space. If multiple paths are provided, they must be separated by a comma
+    and no space around the comma. It also possible to provide a list of paths.
+
+    Return also a dictionary of parameters from CLI detected with ``--<key>=<value>``
+    (with "=" and without spaces around). If no value is provided,
+    it is True by default (like for a flag).
 
     Parameters
     ----------
     sys_argv : List[str]
         List of arguments from sys.argv.
 
     Raises
     ------
     Value Error
-        If the '--config ' argument (with space) is used more than once.
+        If the ``--config`` argument (with space) is used more than once.
 
     Returns
     -------
     config_paths : List[str]
         List of paths to config files to merge.
     cli_params_dict : Dict[str, Any]
         Dictionary of parameters from CLI.
 
     Examples
     --------
     .. code-block:: text
 
         $ python my_script.py --config config.yaml --foo.bar.param=[1, 2, 3]
 
-    Will be parsed as `config_paths=['config.yaml']`
-    and `cli_params={'foo.bar.param': [1, 2, 3]}`.
-    It is equivalent to: `{'foo': {'bar': {'param': [1, 2, 3]}}`
-    for :func:`merge_config`.
+    Will be parsed as ``config_paths=['config.yaml']``
+    and ``cli_params={'foo.bar.param': [1, 2, 3]}``.
+    It is equivalent to: ``{'foo': {'bar': {'param': [1, 2, 3]}}`` for
+    :func:`.merge_flat` and :func:`.make_config`.
     """
     cli_params_dict: Dict[str, Any] = {}
     config_paths: List[str] = []
     i = 0
     while i < len(sys_argv):
         elem = sys_argv[i]
         if elem == "--config":
```

### Comparing `cliconfig-0.6.1/cliconfig/config_routines.py` & `cliconfig-0.6.2/cliconfig/config_routines.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,57 +17,63 @@
 
 
 def make_config(
     *default_config_paths: str,
     process_list: Optional[List[Processing]] = None,
     add_default_processing: bool = True,
 ) -> Config:
-    r"""Make a config from default configs and CLI arguments and apply processing.
+    r"""Make a config from default config(s) and CLI argument(s) with processing.
 
-    It uses the CLI Config routines to parse the CLI arguments and merge
-    them in a simple way. Apply the processing functions on each merge.
+    The function uses the CLI Config routines :func:`.parse_cli` to parse the CLI
+    arguments and merge them with :func:`.merge_flat_paths_processing`, applying
+    the pre-merge and post-merge processing functions on each merge.
 
     Parameters
     ----------
     default_config_paths : Tuple[str]
         Paths to default configs. They are merged in order and new keys
         are allowed.
     process_list: Optional[List[Processing]], optional
         The list of processing to apply during each merge. None for empty list.
         By default None.
-        If add_default_processing is True, the default processing
-        (in :mod:`cliconfig.processing.builtin`) are added to the list.
     add_default_processing : bool, optional
-        If True, add the default processing (in :mod:`cliconfig.processing.builtin`)
-        to the processing list.
+        If add_default_processing is True, the default processings
+        (found on :class:`.DefaultProcessings`) are added to the list of
+        processings. By default True.
 
     Raises
     ------
     ValueError
-        If allow_new_keys is False and CLI has new keys that are not
-        in default configs.
+        If additional configs have new keys that are not in default configs.
 
     Returns
     -------
     config : Config
-        The built config. Contains the config dict (config.dict) and the processing
-        list (config.process_list), which can be used to apply further processing
-        routines.
+        The nested built config. Contains the config dict (config.dict) and
+        the processing list (config.process_list) which can be used to apply
+        further processing routines.
+
+    Note
+    ----
+
+        Setting additional arguments from CLI that are not in default configs
+        does NOT raise an error but only a warning. This ensures the compatibility
+        with other CLI usage (e.g notebook, argparse, etc.)
 
     Examples
     --------
     ::
 
         # main.py
         config = make_config('data.yaml', 'model.yaml', 'train.yaml')
 
     .. code-block:: text
 
-        python main.py -- config bestmodel.yaml,mydata.yaml \
-            --architecture.layers.hidden_dim=64
+        $ python main.py -- config [bestmodel.yaml,mydata.yaml] \
+              --architecture.layers.hidden_dim=64
 
     """
     # Create the processing list
     process_list_: List[Processing] = [] if process_list is None else process_list
     if add_default_processing:
         process_list_ += DefaultProcessings().list
 
@@ -100,18 +106,15 @@
         print(
             "[CONFIG] Warning: New keys found in CLI parameters "
             f"that will not be merged:\n{new_keys_message}"
         )
     # Merge CLI parameters
     cli_params_config = Config(cli_params_dict, [])
     config = merge_flat_processing(
-        config,
-        cli_params_config,
-        allow_new_keys=False,
-        preprocess_first=False
+        config, cli_params_config, allow_new_keys=False, preprocess_first=False
     )
     print(
         f"[CONFIG] Info: Merged {len(default_config_paths)} default config(s), "
         f"{len(additional_config_paths)} additional config(s) and "
         f"{len(cli_params_dict)} CLI parameter(s)."
     )
     # Unflatten the config dict
@@ -124,39 +127,47 @@
     default_config_paths: Optional[List[str]] = None,
     process_list: Optional[List[Processing]] = None,
     *,
     add_default_processing: bool = True,
 ) -> Config:
     """Load config from a file and merge into optional default configs.
 
-    First merge the default configs together, then load the default config,
-    apply the post-load processing, and finally merge the loaded config
+    First merge the default configs together (if any), then load the config
+    from path, apply the post-load processing, and finally merge the loaded
+    config.
 
     Parameters
     ----------
     path : str
         The path to the file to load the configuration.
     default_config_paths : Optional[List[str]], optional
         Paths to default configs. They are merged in order, new keys are allowed.
         Then, the loaded config is merged into the result. None for no default configs.
         By default None.
     process_list: Optional[List[Processing]]
-        The list of processing to apply after loading. Only postload
-        method is applied. The order of the processing is given
-        by the postload_order attribute of the processing.
+        The list of processing to apply after loading and for the merges.
         If None, no processing is applied. By default None.
     add_default_processing : bool, optional
-        If True, add the default processing to the processing list.
+        If add_default_processing is True, the default processings
+        (found on :class:`.DefaultProcessings`) are added to the list of
+        processings. By default True.
 
     Returns
     -------
     config: Dict[str, Any]
-        The loaded config. Contains the config dict (config.dict) and the processing
-        list (config.process_list), which can be used to apply further processing
-        routines.
+        The nested loaded config. Contains the config dict (config.dict) and
+        the processing list (config.process_list) which can be used to apply
+        further processing routines.
+
+    Warning
+    -------
+
+        If default configs are provided, the function does not allow new keys
+        for the loaded config. This is for helping the user to see how to
+        adapt the config file if the default configs have changed.
     """
     # Crate process_list
     process_list_: List[Processing] = [] if process_list is None else process_list
     if add_default_processing:
         process_list_ += DefaultProcessings().list
 
     config = Config({}, process_list_)
@@ -164,49 +175,50 @@
         for config_path in default_config_paths:
             config = merge_flat_paths_processing(
                 config,
                 config_path,
                 allow_new_keys=True,
                 preprocess_first=False,  # Already processed
             )
-    # Disallow new keys for loaded config
     loaded_config = load_processing(path, config.process_list)
     # Update the config list from loaded_config in config
     config.process_list = loaded_config.process_list
-    # Merge the loaded config into the config
-    # NOTE: The loaded config is processed with pre-merge so that tags in
-    # the yaml files are correctly processed.
+    # Merge the loaded config into the config and
+    # disallow new keys for loaded config
+    # if default configs are provided
     config = merge_flat_processing(
         config,
         loaded_config,
-        allow_new_keys=False,
+        allow_new_keys=default_config_paths is None,
         preprocess_first=False,
     )
     # Unflatten the config
     config.dict = unflatten(config.dict)
     return config
 
 
 def save_config(config: Config, path: str) -> None:
     """Save a config and apply pre-save processing before saving.
 
+    Alias for :func:`.save_processing`.
+
     Parameters
     ----------
     config : Dict[str, Any]
         The config to save.
     path : str
         The path to the yaml file to save the dict.
     """
     save_processing(config, path)
 
 
 def show_config(config: Config) -> None:
     """Show the config dict in a pretty way.
 
-    The config dict is unflattened before.
+    The config dict is automatically unflattened before printing.
 
     Parameters
     ----------
     config : Config
         The config to show.
     """
     print("Config:")
```

### Comparing `cliconfig-0.6.1/cliconfig/dict_routines.py` & `cliconfig-0.6.2/cliconfig/dict_routines.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Routines to manipulate nested and flat dictionaries (and mix of both)."""
+"""Routines to manipulate nested and flat dictionaries (and mix of both).
+
+Used by :mod:`.process_routines` and :mod:`.config_routines`.
+"""
 import os
 from typing import Any, Dict, Tuple, Union
 
 import yaml
 from flatten_dict import flatten as _flatten
 from flatten_dict import unflatten as _unflatten
 
@@ -11,27 +14,27 @@
     dict1: Dict[str, Any],
     dict2: Dict[str, Any],
     *,
     allow_new_keys: bool = True,
 ) -> Dict[str, Any]:
     """Flatten then merge dict2 into dict1. The result is flat.
 
-    Work even if dict1 and dict2 have are a mix of nested and flat
+    Work even if dict1 and dict2 have a mix of nested and flat
     dictionaries. For instance like this:
 
     .. code-block:: python
 
         dict1 = {'a.b': 1, 'a': {'c': 2}, 'a.d': {'e.f': 3}}
 
     Parameters
     ----------
     dict1 : Dict[str, Any]
         The first dict. It can be nested, flat or a mix of both.
     dict2 : Dict[str, Any]
-        The second dict to merge into dict1.
+        The second dict to merge into first dict.
     allow_new_keys : bool, optional
         If True, new keys (that are not in dict1) are allowed in dict2.
         By default True.
 
     Raises
     ------
     ValueError
@@ -53,15 +56,15 @@
         >>> merge_dict({'a.b': 1, 'a': {'c': 2}},  {'c': 3}, allow_new_keys=True)
         {'a.b': 1, 'a.c': 2, 'c': 3}
         >>> merge_dict({'a.b': 1, 'a': {'c': 2}},  {'c': 3}, allow_new_keys=False)
         ValueError: New parameter found 'c' that is not in the original dict.
         >>> merge_dict({'a.b': 1, 'a': {'b': 1}},  {'c': 3}, allow_new_keys=True)
         ValueError: duplicated key 'a.b'.
         The above exception was the direct cause of the following exception:
-        ValueError: You may consider calling `clean_pre_flat` on dict 1 before merging.
+        ValueError: You may consider calling 'clean_pre_flat' on dict 1 before merging.
     """
     # Flatten dicts
     flat_dict1, flat_dict2 = _flat_before_merge(dict1, dict2)
 
     if not allow_new_keys:
         # Check that there are no new keys in dict2
         for key in flat_dict2:
@@ -72,30 +75,29 @@
                 )
     # Merge flat dicts
     flat_dict = {**flat_dict1, **flat_dict2}
     return flat_dict
 
 
 def _flat_before_merge(
-    dict1: Dict[str, Any],
-    dict2: Dict[str, Any]
+    dict1: Dict[str, Any], dict2: Dict[str, Any]
 ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
     """Flatten two dicts to merge them later."""
     # Flatten dicts
     flat_dicts = []
     for i, _dict in enumerate([dict1, dict2]):
         # Check if already flat
         is_flat = all(not isinstance(val, dict) for val in _dict.values())
         if not is_flat:
             try:
                 flat_dict = flatten(_dict)
             except ValueError as exc:
                 raise ValueError(
                     f"Duplicated key found in dict {i + 1} when flattening. "
-                    f"You may consider calling `clean_pre_flat` before merging."
+                    f"You may consider calling 'clean_pre_flat' before merging."
                 ) from exc
         else:
             flat_dict = _dict
         flat_dicts.append(flat_dict)
     return flat_dicts[0], flat_dicts[1]
 
 
@@ -103,16 +105,16 @@
     dict_or_path1: Union[str, Dict[str, Any]],
     dict_or_path2: Union[str, Dict[str, Any]],
     *,
     allow_new_keys: bool = True,
 ) -> Dict[str, Any]:
     """Flatten then merge two dict eventually loaded from yaml file paths.
 
-    Similar to :func:`cliconfig.dict_routines.merge_flat` but allow passing
-    the paths of dicts as inputs. It merges the second dict into the first one.
+    Similar to :func:`.merge_flat` but allow passing the paths of dicts
+    as inputs. It merges the second dict into the first one.
 
     Parameters
     ----------
     dict_or_path1 : Union[str, Dict[str, Any]]
         The first dict or its path.
     dict_or_path2 : Union[str, Dict[str, Any]]
         The second dict or its path, to merge into first dict.
@@ -147,32 +149,34 @@
         dict2,
         allow_new_keys=allow_new_keys,
     )
     return flat_dict
 
 
 def flatten(in_dict: Dict[str, Any]) -> Dict[str, Any]:
-    """Flatten dict then return it.
+    """Flatten dict then return it (flat keys are built with dots).
 
     Work even if in_dict is a mix of nested and flat dictionaries.
     For instance like this:
 
     .. code-block:: python
 
-        in_dict = {'a.b': {'c': 1}, 'a': {'b.d': 2}, 'a.e': {'f.g': 3}}
+        >>> flatten({'a.b': {'c': 1}, 'a': {'b.d': 2}, 'a.e': {'f.g': 3}})
+        {'a.b.c': 1, 'a.b.d': 2, 'a.e.f.g': 3}
+
 
     Parameters
     ----------
     in_dict : Dict[str, Any]
         The dict to flatten. It can be nested, already flat or a mix of both.
 
     Raises
     ------
     ValueError
-        If dict has some conflicting keys (like `{'a.b': <x>, 'a': {'b': <y>}}`).
+        If dict has some conflicting keys (like ``{'a.b': <x>, 'a': {'b': <y>}}``).
 
     Returns
     -------
     flat_dict : Dict[str, Any]
         The flattened dict.
 
     Note
@@ -242,16 +246,16 @@
     ----------
     in_dict : Dict[str, Any]
         The dict to clean. It must be the union of a fully flat dict
         (no nested dict i values) and a fully nested dict (without dots in keys).
         See warning section below.
     priority: str
         One of 'flat' or 'unflat', 'error'.
-        If 'flat', keys with dots at the root like `{'a.b': ...}` (flat keys) have
-        priority over nested keys like `{'a': {'b': ...}}` when there are conflicts.
+        If 'flat', keys with dots at the root like ``{'a.b': ...}`` (flat keys) have
+        priority over nested keys like ``{'a': {'b': ...}}`` when there are conflicts.
         If 'unflat', nested keys have priority over flat keys when there are conflicts.
         If 'error', raise an error when there are conflicts.
 
     Raises
     ------
     ValueError
         If priority is not one of 'flat', 'unflat' or 'error'.
@@ -259,20 +263,20 @@
     Returns
     -------
     Dict[str, Any]
         The cleansed dict.
 
     Warning
     -------
-        * No flat key can contain a dict. Then, dicts like `{'a.b': {'c': 1}}`
+        * No flat key can contain a dict. Then, dicts like ``{'a.b': {'c': 1}}``
           are not supported.
         * All the keys that contain dots (the flat keys) must be at the root.
-          Then, dicts like `{a: {'b.c': 1}}` are not supported.
+          Then, dicts like ``{a: {'b.c': 1}}`` are not supported.
         * To summarize, the dict must contain only fully flat dicts
-          and fully nested dicts.
+          and/or fully nested dicts.
 
     Examples
     --------
     ::
 
         >>> clean_pre_flat({'a.b': 1, 'a': {'b': 2}, 'c': 3}, priority='flat')
         {'a.b': 1, 'c': 3}
@@ -307,15 +311,15 @@
 def _del_key(
     in_dict: Dict[str, Any],
     flat_key: str,
     *,
     keep_flat: bool = False,
     keep_unflat: bool = False,
 ) -> None:
-    """Remove in place a value in dict corresponding to a flat key (e.g. 'a.b.c).
+    """Remove in place a value in dict corresponding to a flat key (e.g. 'a.b.c').
 
     Parameters
     ----------
     in_dict : Dict[str, Any]
         The dict to clean. It must be the union of a fully flat dict
         (no nested dict i values) and a fully nested dict (without dots in keys).
         See warning section below.
@@ -329,18 +333,18 @@
     Raises
     ------
     ValueError
         If the key is not found in the dict.
 
     Warning
     -------
-        * No flat key can contain a dict. Then, dicts like `{'a.b': {'c': 1}}`
+        * No flat key can contain a dict. Then, dicts like ``{'a.b': {'c': 1}}``
           are not supported.
         * All the keys that contain dots (the flat keys) must be at the root.
-          Then, dicts like `{a: {'b.c': 1}}` are not supported.
+          Then, dicts like ``{a: {'b.c': 1}}`` are not supported.
         * To summarize, the dict must contain only fully flat dicts
           and fully nested dicts.
 
     Examples
     --------
     ::
 
@@ -351,27 +355,23 @@
         {'a': {'d': 2}, 'a.b.c': 4}
         >>> _del_key(in_dict, 'a.b.c', keep_unflat=True); in_dict
         {'a': {'b': {'c': 1}, 'd': 2}}
         >>> _del_key(in_dict, 'a.b.z')
         ValueError: Key 'a.b.z' not found in dict.
         >>> _del_key(in_dict, 'a.z.c')
         ValueError: Key 'a.z.c' not found in dict.
-
     """
     found_key = False
     if not keep_flat and flat_key in in_dict:
         # Remove flat_key if it exists at the root
         found_key = True
         del in_dict[flat_key]
 
     def recursive_del_key(
-        in_dict: Dict[str, Any],
-        key: str,
-        *,
-        found_key: bool
+        in_dict: Dict[str, Any], key: str, *, found_key: bool
     ) -> bool:
         first_key, *other_keys = key.split(".", 1)
         if other_keys:
             if first_key in in_dict:
                 # Delete key in sub-dict
                 new_key = recursive_del_key(
                     in_dict[first_key],
@@ -399,15 +399,15 @@
         found_key = recursive_del_key(in_dict, flat_key, found_key=found_key)
     # Raise error if key not found
     if not found_key:
         raise ValueError(f"Key '{flat_key}' not found in dict.")
 
 
 def save_dict(in_dict: Dict[str, Any], path: str) -> None:
-    """Save a dict to a yaml file.
+    """Save a dict to a yaml file (with yaml.dump).
 
     Parameters
     ----------
     in_dict : Dict[str, Any]
         The dict to save.
     path : str
         The path to the yaml file to save the dict.
@@ -417,47 +417,58 @@
     with open(path, "w", encoding="utf-8") as cfg_file:
         yaml.dump(in_dict, cfg_file, default_flow_style=False)
 
 
 def load_dict(path: str) -> Dict[str, Any]:
     """Load dict from a yaml file path.
 
+     Support multiple files in the same document.
+
     Parameters
     ----------
     path : str
         The path to the file to load the dict.
 
     Returns
     -------
     out_dict : Dict[str, Any]
-        The loaded dict.
+        The nested (unflatten) loaded dict.
+
+    Note
+    ----
+        If multiple yaml files are in the same document, they are merged
+        from the first to the last.
     """
     with open(path, "r", encoding="utf-8") as cfg_file:
-        out_dict = yaml.safe_load(cfg_file)
-    return out_dict
+        file_dicts = yaml.safe_load_all(cfg_file)
+        out_dict: Dict[str, Any] = {}
+        for file_dict in file_dicts:
+            out_dict = merge_flat(out_dict, file_dict, allow_new_keys=True)
+    return unflatten(out_dict)
 
 
-def show_dict(in_dict: Dict[str, Any], start_indent: int = 1) -> None:
+def show_dict(in_dict: Dict[str, Any], start_indent: int = 0) -> None:
     """Show the input dict in a pretty way.
 
-    The input dict is unflattened before.
+    The config dict is automatically unflattened before printing.
 
     Parameters
     ----------
     in_dict : Dict[str, Any]
         The dict to show.
     start_indent : int, optional
-        The number of starting tab indent (4 spaces), by default 1.
+        The number of starting tab indent (4 spaces), by default 0.
     """
 
     def pretty_print(in_dict: Dict[str, Any], indent: int) -> None:
         """Pretty print the dict recursively."""
         for key, value in in_dict.items():
             print(f"{'    ' * indent}{key}: ", end="")
             if isinstance(value, dict):
                 print()
                 pretty_print(value, indent + 1)
             elif isinstance(value, str):
                 print(f"'{value}'")
             else:
                 print(value)
+
     pretty_print(unflatten(in_dict), start_indent)
```

### Comparing `cliconfig-0.6.1/cliconfig/process_routines.py` & `cliconfig-0.6.2/cliconfig/process_routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Routines to manipulate dictionaries with processing."""
+"""Routines to manipulate dictionaries with processing.
+
+Used by :mod:`.config_routines`.
+"""
 from typing import List, Optional, Union
 
 from cliconfig.base import Config
 from cliconfig.dict_routines import (
     _flat_before_merge,
     flatten,
     load_dict,
@@ -22,15 +25,16 @@
     preprocess_second: bool = True,
     postprocess: bool = True,
 ) -> Config:
     """Flatten, merge config2 into config1 and apply pre and post processing.
 
     Work even if the config dicts have a mix of nested and flat dictionaries.
     If both arguments are configs, the process lists are merged before applying
-    the processing. The duplicate processings are removed.
+    the processing. The duplicate processings (with same internal variables)
+    are removed.
 
     Parameters
     ----------
     config1 : Config
         The first config.
     config2 : Config
         The second dict to merge into config1.
@@ -99,17 +103,18 @@
     preprocess_first: bool = True,
     preprocess_second: bool = True,
     postprocess: bool = True,
 ) -> Config:
     """Flatten, merge and apply processing to two configs or their yaml paths.
 
     Similar to :func:`merge_flat_processing` but allows to pass configs
-    or yaml paths. Work even if the configs have a mix of nested and flat dicts.
+    or their yaml paths. Work even if the configs have a mix of nested and flat dicts.
     If both arguments are configs, the process lists are merged before applying
-    the processing. The duplicate processings are removed.
+    the processing. The duplicate processings (with same internal variables)
+    are removed.
 
     Parameters
     ----------
     config_or_path1 : Union[str, Config]
         The first config or its path.
     config_or_path2 : Union[str, Config]
         The second config or its path, to merge into first config.
```

### Comparing `cliconfig-0.6.1/cliconfig/processing/_type_parser.py` & `cliconfig-0.6.2/cliconfig/processing/_type_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,105 +5,113 @@
 
 def _parse_type(type_desc: str) -> Tuple:
     """Parse a type description.
 
     Allow basic types (none, any, bool, int, float, str, list, dict), nested lists,
     nested dicts, unions (with Union or the '|' symbol) and Optional.
 
-    Representation:
-     * None|Any -> (type(None), object)
-     * list|float -> (list, float)
-     * List[float] -> (("list", (float,)),)
-     * Dict[str, List[float]] -> (("dict", (str,), ((("list", (float,)),),)),)
-     * Dict[str|bool, int|float] -> (("dict", (str, bool), (int, float)),)
+    Examples of representation:
+     * "str" -> (str,)
+     * "None|Any" -> (type(None), object)
+     * "list|float" -> (list, float)
+     * "List[float]" -> (("list", (float,)),)
+     * "Dict[str, Any]" -> (("dict", (str,), (object,)),)
+     * "Dict[str, List[float]]" -> (("dict", (str,), ((("list", (float,)),),)),)
+     * "Dict[str|bool, int|float]" -> (("dict", (str, bool), (int, float)),)
+     * ...
 
     Raises
     ------
     ValueError
         If the type description is not valid or not recognized.
+
+    Note
+    ----
+        The type description is lowercased and spaces are removed before parsing.
     """
     # Clean up
     old_type_desc = type_desc
-    type_desc = type_desc.replace(' ', '').lower()
+    type_desc = type_desc.replace(" ", "").lower()
     try:
         # Base typeParseType
         base_type = _parse_base_type(type_desc)
         if base_type is not None:
-            return (base_type, )
+            return (base_type,)
         # Split the external blocks enclosed by brackets
-        blocks = _split_brackets(type_desc, delimiter='|')
+        blocks = _split_brackets(type_desc, delimiter="|")
         types: Tuple = ()
         for block in blocks:
-            if block[:5] == 'list[':
+            if block[:5] == "list[":
                 types += _parse_list(block)
-            elif block[:5] == 'dict[':
+            elif block[:5] == "dict[":
                 types += _parse_dict(block)
-            elif block[:9] == 'optional[':
+            elif block[:9] == "optional[":
                 types += _parse_optional(block)
-            elif block[:6] == 'union[':
+            elif block[:6] == "union[":
                 types += _parse_union(block)
             else:  # Should be a base type
                 base_type = _parse_base_type(block)
                 if base_type is not None:
-                    types += (base_type, )
+                    types += (base_type,)
                 else:
                     raise ValueError(f"Unknown type: '{block}'")
         return types
     except ValueError as err:
         # Revert the traceback to show the original type description
         raise ValueError(f"Unknown type: '{old_type_desc}'") from err
 
 
 def _parse_base_type(type_desc: str) -> Optional[Type]:
     """Parse a base type description.
 
     Base types are: none, any, bool, int, float and str, list, dict.
     Return None if the type is not a base type.
     """
-    if type_desc == 'none':
+    if type_desc == "none":
         return type(None)
-    if type_desc == 'any':
+    if type_desc == "any":
         # Match any type
         return object
-    if type_desc in ('bool', 'int', 'float', 'str', 'list', 'dict'):
+    if type_desc in ("bool", "int", "float", "str", "list", "dict"):
         return locate(type_desc)  # type: ignore
     return None
 
 
 def _parse_list(type_desc: str) -> Tuple:
     """Parse a "list" type description."""
     sub_desc = type_desc[5:-1]
-    if len(_split_brackets(sub_desc, delimiter=',')) > 1:
+    if len(_split_brackets(sub_desc, delimiter=",")) > 1:
         raise ValueError(f"Invalid List type: '{type_desc}'")
-    return (('list', ) + (_parse_type(sub_desc), ), )
+    return (("list",) + (_parse_type(sub_desc),),)
 
 
 def _parse_dict(type_desc: str) -> Tuple:
     """Parse an "dict" type description."""
     sub_desc = type_desc[5:-1]
-    sub_blocks = _split_brackets(sub_desc, delimiter=',')
+    sub_blocks = _split_brackets(sub_desc, delimiter=",")
     if len(sub_blocks) != 2:
         raise ValueError(f"Invalid Dict type: '{type_desc}'")
     key_type = _parse_type(sub_blocks[0])
     value_type = _parse_type(sub_blocks[1])
-    return (('dict', ) + (key_type, ) + ((value_type), ), )
+    return (("dict",) + (key_type,) + ((value_type),),)
 
 
 def _parse_optional(type_desc: str) -> Tuple:
     """Parse an "optional" type description."""
     sub_desc = type_desc[9:-1]
-    if len(_split_brackets(sub_desc, delimiter=',')) > 1:
+    if len(_split_brackets(sub_desc, delimiter=",")) > 1:
         raise ValueError(f"Invalid Optional type: '{type_desc}'")
-    return ((type(None), ) + _parse_type(sub_desc), )
+    return ((type(None),) + _parse_type(sub_desc),)
 
 
 def _parse_union(type_desc: str) -> Tuple:
+    """Parse an "union" type description."""
     sub_desc = type_desc[6:-1]
     # Split by comma
-    sub_blocks = _split_brackets(sub_desc, delimiter=',')
+    sub_blocks = _split_brackets(sub_desc, delimiter=",")
     if len(sub_blocks) < 2:
         raise ValueError(f"Invalid Union type: '{type_desc}'")
     types: Tuple = ()
     union_types = [_parse_type(sub_block) for sub_block in sub_blocks]
     for union_type in union_types:
         types += union_type
     return types
@@ -112,17 +120,17 @@
 def _split_brackets(type_desc: str, delimiter: str) -> List[str]:
     """Split a type description in blocks enclosed by brackets."""
     blocks = []
     bracket_count = 0
     i, j = 0, 0
     while j < len(type_desc):
         char = type_desc[j]
-        if char == '[':
+        if char == "[":
             bracket_count += 1
-        elif char == ']':
+        elif char == "]":
             bracket_count -= 1
         if bracket_count == 0 and char == delimiter:
             blocks.append(type_desc[i:j])
             i = j + 1
             j += 2
         else:
             j += 1
@@ -133,17 +141,20 @@
 def _isinstance(obj: object, types: Union[Type, Tuple]) -> bool:
     """Check if an object is an instance of a type or a tuple of types.
 
     Intended to work with the outputs of _parse_type.
     """
     if isinstance(types, type):
         return isinstance(obj, types)
-    if types[0] == 'list' and len(types) == 2:
-        return (isinstance(obj, list)
-                and all(_isinstance(elem, types[1]) for elem in obj))
-    if types[0] == 'dict' and len(types) == 3:
-        return (isinstance(obj, dict)
-                and all(_isinstance(key, types[1]) for key in obj)
-                and all(_isinstance(value, types[2]) for value in obj.values()))
+    if types[0] == "list" and len(types) == 2:
+        return isinstance(obj, list) and all(
+            _isinstance(elem, types[1]) for elem in obj
+        )
+    if types[0] == "dict" and len(types) == 3:
+        return (
+            isinstance(obj, dict)
+            and all(_isinstance(key, types[1]) for key in obj)
+            and all(_isinstance(value, types[2]) for value in obj.values())
+        )
     if isinstance(types[0], (type, tuple)):
         return any(_isinstance(obj, sub_types) for sub_types in types)
     raise ValueError(f"Invalid type for _isinstance: '{types}'")
```

### Comparing `cliconfig-0.6.1/cliconfig/processing/builtin.py` & `cliconfig-0.6.2/cliconfig/processing/builtin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 """Built-in processing classes.
 
-Classes to apply pre-merge, post-merge, pre-save and post-load modifications
-to dict with processing routines (found in cliconfig.process_routines).
+Built-in classes to apply pre-merge, post-merge, pre-save and post-load modifications
+to dict with processing routines :mod:`.process_routines`.
+
+They are the default processing used by the config routines :func:`.load_config`
+and :func:`.make_config`.
 """
 from typing import Any, Dict, List, Set
 
 from cliconfig.base import Config
 from cliconfig.process_routines import (
     merge_flat_paths_processing,
     merge_flat_processing,
 )
 from cliconfig.processing._type_parser import _isinstance, _parse_type
 from cliconfig.processing.base import Processing
 from cliconfig.tag_routines import clean_all_tags, clean_tag, dict_clean_tags, is_tag_in
 
 
 class ProcessMerge(Processing):
-    """Merge dicts just in time with '@merge_after/_before/_add' tags.
+    """Merge dicts just in time with ``@merge_after/_before/_add`` tags.
 
-    Tag your key with '@merge_after', '@merge_before' or @merge_add to load
-    the dict corresponding to the value (path) and merge it just before or after
-    the current dict. The merged dicts will be processed with pre-merge but
-    not post-merge to ensure that merged configurations are all processed with
-    pre-merge before applying a post-merge processing. It allows the merged
-    configs to make references to each other (typically for copy).
+    Tag your key with ``@merge_after``, ``@merge_before`` or ``@merge_add``
+    to load the config corresponding to the value (which is a yaml path) and
+    merge it just before or after the current config. The merged dicts will be
+    processed with pre-merge but not post-merge to ensure that merged
+    configurations are recursively processed with pre-merge before applying a
+    post-merge processing. It allows the merged configs to make references to
+    each other (typically for copy) even without containing the merge tags
+    itself.
 
     * '@merge_add' merges the dict corresponding to the path by allowing ONLY new keys
-      It is a security check when you want to add a dict completely new
-      It is a typical usage for a default config splitted in several files.
+      It is a security check when you want to add a dict completely new,
+      the typical usage for a default config splitted in several files.
     * '@merge_after' merge the dict corresponding to the path on the current dict
     * '@merge_before' merge the current dict on the dict corresponding to the path
 
     The processing is a pre-merge processing only and occurs before
-    most of the other processing.
+    almost all of the other processings.
     Pre-merge order: -20.0
 
     Examples
     --------
     .. code-block:: yaml
 
         --- # config1.yaml
@@ -49,85 +54,85 @@
         --- # config3.yaml
         c: 3
 
     Before merging, the config1 is interpreted as the dict:
 
     ::
 
-        {'a': {'b': 2, 'b_path': 'config2.yaml'}, 'c_path': 'config3.yaml', 'c': 3}`
+        {'a': {'b': 2, 'b_path': 'config2.yaml'}, 'c_path': 'config3.yaml', 'c': 3}
 
     If you replace '@merge_after' by '@merge_before', it will be:
 
     ::
 
-        {'a': {'b': 1, 'b_path': 'config2.yaml'}, 'c_path': 'config3.yaml', 'c': 3}`
+        {'a': {'b': 1, 'b_path': 'config2.yaml'}, 'c_path': 'config3.yaml', 'c': 3}
 
-    Finally, if you replace '@merge_after' by '@merge_add', it will raises an
-    error because the key 'a.b' already exists in the dict.
+    Finally, if you replace ``@merge_after`` by ``@merge_add``, it will raises an
+    error because the key ``a.b`` already exists in the dict.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.premerge_order = -20.0
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         items = list(flat_config.dict.items())
         for flat_key, val in items:
             if is_tag_in(flat_key, "merge_after"):
-                if not isinstance(val, str) or not val.endswith('.yaml'):
+                if not isinstance(val, str) or not val.endswith(".yaml"):
                     raise ValueError(
                         "Key with '@merge_after' tag must be associated "
                         "to a string corresponding to a *yaml* file."
                         f"The problem occurs at key: {flat_key}"
                     )
                 # Remove the tag in the dict
                 del flat_config.dict[flat_key]
-                flat_config.dict[clean_tag(flat_key, 'merge_after')] = val
+                flat_config.dict[clean_tag(flat_key, "merge_after")] = val
                 # Merge + process the dicts
                 # NOTE: we allow new keys with security because the merge
                 # following this pre-merge will avoid the creation of
                 # new keys if needed.
                 flat_config = merge_flat_paths_processing(
                     flat_config,
                     val,
                     allow_new_keys=True,
                     preprocess_first=False,  # Already processed
                     postprocess=False,
                 )
 
             elif is_tag_in(flat_key, "merge_before"):
-                if not isinstance(val, str) or not val.endswith('.yaml'):
+                if not isinstance(val, str) or not val.endswith(".yaml"):
                     raise ValueError(
                         "Key with '@merge_before' tag must be associated "
                         "to a string corresponding to a *yaml* file."
                         f"The problem occurs at key: {flat_key}"
                     )
                 # Remove the tag in the dict
                 del flat_config.dict[flat_key]
-                flat_config.dict[clean_tag(flat_key, 'merge_before')] = val
+                flat_config.dict[clean_tag(flat_key, "merge_before")] = val
                 # Merge + process the dicts
                 flat_config = merge_flat_paths_processing(
                     val,
                     flat_config,
                     allow_new_keys=True,
                     preprocess_second=False,  # Already processed
                     postprocess=False,
                 )
 
             elif is_tag_in(flat_key, "merge_add"):
-                if not isinstance(val, str) or not val.endswith('.yaml'):
+                if not isinstance(val, str) or not val.endswith(".yaml"):
                     raise ValueError(
                         "Key with '@merge_add' tag must be associated "
                         "to a string corresponding to a *yaml* file."
                         f"The problem occurs at key: {flat_key}"
                     )
                 # Remove the tag in the dict
                 del flat_config.dict[flat_key]
-                flat_config.dict[clean_tag(flat_key, 'merge_add')] = val
+                flat_config.dict[clean_tag(flat_key, "merge_add")] = val
                 # Pre-merge process the dict with the process list of
                 # the current config
                 flat_config_to_merge = merge_flat_paths_processing(
                     Config({}, []),
                     val,
                     additional_process=flat_config.process_list,
                     allow_new_keys=True,
@@ -155,26 +160,21 @@
                     preprocess_second=False,  # Already processed
                     postprocess=False,
                 )
         return flat_config
 
 
 class ProcessCopy(Processing):
-    """Copy a value with '@copy' tag. The copy is protected from updates.
+    """Copy a value with ``@copy`` tag. The copy is protected from direct updates.
 
-    Tag your key with '@copy' and with value the name of the flat key to copy.
-    Then, the value will be a copy of the corresponding value forever.
-    The pre-merge processing will remove the tag. The post-merge processing
-    will set the value (if the copied key exists) and occurs after most processing.
+    Tag your key with ``@copy`` and with value the name of the flat key to copy.
+    The pre-merge processing removes the tag. The post-merge processing
+    sets the value (if the copied key exists) and occurs after most processings.
     The pre-save processing restore the tag and the key to copy to keep the
     information on future loads.
-
-    The copy key is protected against any modification and will raise an error
-    if you try to modify it.
-
     Pre-merge order: 0.0
     Post-merge order: 10.0
     Pre-save order: 10.0
 
     Examples
     --------
     .. code-block:: yaml
@@ -188,17 +188,24 @@
 
     .. code-block:: python
 
         {'a': {'b': 1, 'c': 1}}
 
     Note
     ----
+
+        The copy key is protected against any modification and will raise an error
+        if you try to modify it but will be updated if the copied key is updated.
+
+    Warning
+    -------
+
         If the key to copy does not exist in the config on post-merge, the
         processing will NOT raise an error to let the user the possibility
-        to add the key later via merge. However, the key still be protected.
+        to add the key later via merge. However, the value still be protected.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.premerge_order = 0.0
         self.postmerge_order = 10.0
         self.presave_order = 10.0
@@ -213,16 +220,18 @@
                 if not isinstance(val, str):
                     raise ValueError(
                         "Key with '@copy' tag must be associated "
                         "to a string corresponding to a flat key. "
                         f"The problem occurs at key: {flat_key} with value: {val}"
                     )
                 clean_key = clean_all_tags(flat_key)
-                if (clean_key in self.keys_to_copy
-                        and self.keys_to_copy[clean_key] != val):
+                if (
+                    clean_key in self.keys_to_copy
+                    and self.keys_to_copy[clean_key] != val
+                ):
                     raise ValueError(
                         "Key with '@copy' has change its value to copy. Found key: "
                         f"{flat_key} with value: {val}, previous value to copy: "
                         f"{self.keys_to_copy[clean_key]}"
                     )
                 # Store the key to copy and value
                 self.keys_to_copy[clean_key] = val
@@ -241,15 +250,16 @@
                 if flat_config.dict[key] != self.current_value[key]:
                     # The key has been modified
                     raise ValueError(
                         "Found attempt to modify a key with '@copy' tag. The key "
                         "is then protected against updates (except the copied "
                         f"value or the original key to copy). Found key: {key} of "
                         f"value {flat_config.dict[key]} that copy {val} of value "
-                        f"{flat_config.dict[val]}")
+                        f"{flat_config.dict[val]}"
+                    )
                 # Copy the value
                 flat_config.dict[key] = flat_config.dict[val]
                 # Update the current value
                 self.current_value[key] = flat_config.dict[val]
         return flat_config
 
     def presave(self, flat_config: Config) -> Config:
@@ -263,88 +273,97 @@
                 new_key = key + "@copy"
                 del flat_config.dict[key]
                 flat_config.dict[new_key] = self.keys_to_copy[clean_key]
         return flat_config
 
 
 class ProcessTyping(Processing):
-    """Force a type with '@type:mytype' tag. The type is preserved forever.
+    """Force a type with ``@type:<mytype>`` tag. The type is then forced forever.
 
     Allow basic types (none, any, bool, int, float, str, list, dict), nested lists,
     nested dicts, unions (with Union or the '|' symbol) and Optional.
-    It store the type in pre-merge and check alls forced types on post-merge.
-    It restore the tag in pre-save to keep the information on future loads.
-    It always occurs last in post-merge.
+    The type description is lowercased and spaces are removed.
+
+    For instance: ``@type:None|List[Dict[str, int|float]]`` is valid and force
+    the type to be None or a list containing dicts with str keys and int or float
+    values.
+
+    the processing stores the type in pre-merge and check alls forced types on
+    post-merge. It restore the tag in pre-save to keep the information on
+    future loads. The post-merge processing occurs after almost all processings.
     Pre-merge order: 0.0
     Post-merge order: 20.0
     Pre-save order: 0.0
 
     Note
     ----
         The type is not checked on pre-merge to allow the parameter to be
         updated (by a copy or a merge for instance). The goal of this
         processing is to ensure the type at the end of the post-merge.
 
     Examples
     --------
     ::
 
-        dict1 = {param@type:None|List[int|float]: None}
-        dict2 = {param: [0, 1, 2.0]}  # no error
-        dict3 = {param: [0, 1, 2.0, 'a']}  # error
-
-    Merge configs with dictionnaries dict1 and dict2 raise no error and `param`
-    is forced to be None or a list of int or float forever. Merge dict1
-    and dict3 raise an error on post-merge because of the 'a' value.
-
-    Note that removing "None|" in the type description still doesn't raise an error
-    in the first case because the type checking is evaluated after the merge with
-    dict2.
+        in_dict = {"param@type:None|List[int|float]": None}
+        dict1 = {param: [0, 1, 2.0]}  # no error
+        dict2 = {param: [0, 1, 2.0, 'a']}  # error
+
+    Merging configs with dictionaries ``in_dict`` and ``dict1`` raises no
+    error and ``param`` is forced to be None or a list of int or float forever.
+    Merging config with ``in_dict`` and ``dict3`` raises an error on post-merge
+    due to the 'a' value (which is a string).
+
+    Note that removing "None|" in the type description of ``param`` still
+    doesn't raise an error in the first case because the type checking is
+    evaluated after the merge with ``dict2``.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.premerge_order = 0.0
         self.postmerge_order = 20.0
         self.presave_order = 0.0
         self.forced_types: Dict[str, tuple] = {}
         self.type_desc: Dict[str, str] = {}  # For error messages
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         items = list(flat_config.dict.items())
         for flat_key, val in items:
-            end_key = flat_key.split('.')[-1]
+            end_key = flat_key.split(".")[-1]
             if "@type:" in end_key:
                 # Get the type description
                 trail = end_key.split("@type:")[-1]
-                type_desc = trail.split('@')[0]  # (in case of multiple tags)
+                type_desc = trail.split("@")[0]  # (in case of multiple tags)
                 expected_type = tuple(_parse_type(type_desc))
                 clean_key = clean_all_tags(flat_key)
-                if (clean_key in self.forced_types
-                        and set(self.forced_types[clean_key]) != set(expected_type)):
+                if clean_key in self.forced_types and set(
+                    self.forced_types[clean_key]
+                ) != set(expected_type):
                     raise ValueError(
                         f"Find the tag '@type:{type_desc}' on a key that has already "
                         "been associated to an other type: "
                         f"{self.type_desc[clean_key]}. "
                         f"Find problem at key: {flat_key}"
                     )
                 # Remove the tag
                 del flat_config.dict[flat_key]
-                flat_config.dict[clean_tag(flat_key, f'type:{type_desc}')] = val
+                flat_config.dict[clean_tag(flat_key, f"type:{type_desc}")] = val
                 # Store the forced type
                 self.forced_types[clean_key] = expected_type
                 self.type_desc[clean_key] = type_desc
         return flat_config
 
     def postmerge(self, flat_config: Config) -> Config:
         """Post-merge processing."""
         for key, expected_type in self.forced_types.items():
-            if (key in flat_config.dict
-                    and not _isinstance(flat_config.dict[key], expected_type)):
+            if key in flat_config.dict and not _isinstance(
+                flat_config.dict[key], expected_type
+            ):
                 type_desc = self.type_desc[key]
                 raise ValueError(
                     f"Key previously tagged with '@type:{type_desc}' must be "
                     f"associated to a value of type {type_desc}. Find the "
                     f"value: {flat_config.dict[key]} of type "
                     f"{type(flat_config.dict[key])} at key: {key}"
                 )
@@ -361,17 +380,17 @@
                 new_key = key + f"@type:{self.type_desc[clean_key]}"
                 flat_config.dict[new_key] = flat_config.dict[key]
                 del flat_config.dict[key]
         return flat_config
 
 
 class ProcessSelect(Processing):
-    """Select a sub-config with and delete the rest of its parent config.
+    """Select a sub-config with ``@select`` and delete the rest of its parent config.
 
-    First look in pre-merge for a parameter tagged with '@select' containing a
+    First look in pre-merge for a parameter tagged with ``@select`` containing a
     flat key corresponding to a sub-configurations to keep. The parent configuration
     is then deleted on post-merge, except the selected sub-configuration
     and eventually the tagged parameter (if it is in the same sub-configuration).
     It is also possible to select multiple keys of a same sub-configuration
     (meaning that the part before the last dot must be equal) by passing a
     list of flat keys.
     Pre-merge order: 0.0
@@ -391,24 +410,23 @@
                 param2: 4
             model3:
                 submodel:
                     param: 5
             model4:
                 param: 6
 
-    Result in deleting models.model2 (param1 and param2) and models.model4.param,
-    and keeping the rest.
+    Result in deleting ``models.model2`` (``param1`` and ``param2``) and
+    ``models.model4.param``, and keeping the rest.
 
     Warning
     -------
 
-        For security reasons, it prevents from deleting the configuration at the root
-        (which is the case when the selected key doesn't contain a dot),
-        and raises an error in this case.
-
+        For security reasons, this processing prevents from deleting
+        the configuration at the root, which is the case when the
+        selected key doesn't contain a dot. It raises an error in this case.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.keys_that_select: Set[str] = set()
         self.subconfigs_to_delete: Set[str] = set()
         self.keys_to_keep: Set[str] = set()
@@ -452,23 +470,26 @@
                     )
                 self.subconfigs_to_delete.add(subconfig)
                 self.keys_to_keep.update(keys_to_keep)
         return flat_config
 
     def postmerge(self, flat_config: Config) -> Config:
         """Post-merge processing."""
+
         def _is_in_subconfig(key: str, subconfig: str) -> bool:
             """Check if a key is in a subconfig with the exact name."""
             return key == subconfig or key.startswith(subconfig + ".")
+
         # Delete all keys on the subconfigs except the ones to keep
         for subconfig in self.subconfigs_to_delete:
             for key in list(flat_config.dict.keys()):
-                if (_is_in_subconfig(key, subconfig)
-                        and not any(_is_in_subconfig(key, key_to_keep)
-                                    for key_to_keep in self.keys_to_keep)):
+                if _is_in_subconfig(key, subconfig) and not any(
+                    _is_in_subconfig(key, key_to_keep)
+                    for key_to_keep in self.keys_to_keep
+                ):
                     del flat_config.dict[key]
         return super().postmerge(flat_config)
 
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing."""
         # Restore the tag with the type to keep the information
         # on further loading
@@ -479,20 +500,22 @@
                 new_key = key + "@select"
                 flat_config.dict[new_key] = flat_config.dict[key]
                 del flat_config.dict[key]
         return flat_config
 
 
 class ProcessDelete(Processing):
-    """Delete the parameters tagged with @delete on pre-merge.
+    """Delete the parameters tagged with ``@delete`` on pre-merge.
 
-    This processing is applied late on pre-merge to allow the others processing
-    to be applied before deleting the parameters. It is usefull to activate a
-    processing without add an additional parameter in the default configuration
-    to void the error on merge with allow_new_keys=False.
+    This processing is usefull to activate a processing without adding
+    an additional parameter in the default configuration to avoid the error
+    on merge with ``allow_new_keys=False``. This processing is applied very
+    late on pre-merge to allow the others processing to be applied before
+    deleting the parameters.
+    Pre-merge order: 25.0
 
     Examples
     --------
     .. code-block:: yaml
 
         # main.yaml
         1@select@delete: configs.config1
@@ -506,24 +529,24 @@
         --- # config2.yaml
         configs.config2.param: 3
         configs.config2.param: 4
 
     Here we want to merge two config files and select one sub-config.
     We use the corresponding tags but we don't have a good name for the keys
     and instead of adding a new parameter in the default configuration with
-    random names like "1", "2", "3", we use the @delete tag to delete the
+    random names like "1", "2", "3", we use the ``@delete`` tag to delete the
     keys after the pre-merge processing.
-    Pre-merge processing: 25.0
 
     Warning
     -------
-        The parameter is deleted on pre-merge so if the parameter already exists
-        on the other configuration during merge, this parameter will be remain
-        as it is. This processing is more used to delete parameter that is NOT
-        present in the default configuration.
+
+        The parameter is deleted on pre-merge. Therefore, if the parameter
+        also exists on the other configuration during merge (without the tag),
+        this parameter will be remain as it is. This processing is more used
+        to delete parameter that is NOT present in the default configuration.
     """
 
     def __init__(self) -> None:
         super().__init__()
         # After all pre-merge processing
         self.premerge_order = 25.0
 
@@ -535,28 +558,28 @@
                 del flat_config.dict[key]
         return flat_config
 
 
 class ProcessCheckTags(Processing):
     """Raise an error if a tag is present in a key after pre-merging processes.
 
-    This security processing is applied after all pre-merge process and
-    checks for "@" in the keys. It raises an error if one is found.
+    This security processing is always applied after all pre-merge process and
+    checks for '@' in the keys. It raises an error if one is found.
     """
 
     def __init__(self) -> None:
         super().__init__()
         # NOTE: this processing is a special meta-processing that must be
         # applied after all other pre-merge processing to ensure security.
         # That why it has a very high pre-merge order and it is not a
         # good idea to make pre-merge processing with higher order.
         self.premerge_order = 1000.0
 
     def premerge(self, flat_config: Config) -> Config:
-        """Post-merge processing."""
+        """Pre-merge processing."""
         _, tagged_keys = dict_clean_tags(flat_config.dict)
         if tagged_keys:
             keys_message = "\n".join(tagged_keys[:5])
             raise ValueError(
                 "Keys with tags are encountered at the end of "
                 "the pre-merge process. It is probably a mistake due to:\n"
                 "- a typo in tag name\n"
@@ -565,20 +588,21 @@
                 "- the use of a custom processing that does not remove a tag\n\n"
                 "The tagged keys encountered (5 first if more than 5) are:\n"
                 f"{keys_message}"
             )
         return flat_config
 
 
-class DefaultProcessings():
+class DefaultProcessings:
     """Default list of built-in processings.
 
     To add these processings to a Config instance, use:
+    ::
 
-    config.process_list += DefaultProcessings().list
+        config.process_list += DefaultProcessings().list
 
     The current default processing list contains:
      * ProcessCheckTags: protect against '@' in keys at the end of pre-merge)
      * ProcessMerge (@merge_all, @merge_before, @merge_after): merge multiple
        files into one.
      * ProcessCopy (@copy): persistently copy a value from one key to an other
        and protect it
```

### Comparing `cliconfig-0.6.1/cliconfig/processing/create.py` & `cliconfig-0.6.2/cliconfig/processing/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     ) -> None:
         super().__init__()
         self.premerge_order = order
         self.regex = regex
         self.tag_name = tag_name
         self.func = func
         if self.regex:
-            self.is_in_func = lambda key: re.match(
-                self.regex, key.split('.')[-1]
-            ) is not None
+            self.is_in_func = (
+                lambda key: re.match(self.regex, key.split(".")[-1]) is not None
+            )
         elif self.tag_name:
             self.is_in_func = lambda key: is_tag_in(key, str(self.tag_name))
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         items = list(flat_config.dict.items())
         for flat_key, value in items:
@@ -55,64 +55,120 @@
         super().__init__()
         self.premerge_order = order
         self.regex = regex
         self.tag_name = tag_name
         self.func = func
         self.matched_keys: Set[str] = set()
         if self.regex is not None:
-            self.is_in_func = lambda key: re.match(
-                self.regex, key.split('.')[-1]
-            ) is not None
+            self.is_in_func = (
+                lambda key: re.match(self.regex, key.split(".")[-1]) is not None
+            )
         elif self.tag_name is not None:
             self.is_in_func = lambda key: is_tag_in(key, str(self.tag_name))
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         items = list(flat_config.dict.items())
         for flat_key, value in items:
-            if (self.is_in_func(flat_key)  # type: ignore
-                    or clean_all_tags(flat_key) in self.matched_keys):
+            if (
+                self.is_in_func(flat_key)  # type: ignore
+                or clean_all_tags(flat_key) in self.matched_keys
+            ):
                 self.matched_keys.add(clean_all_tags(flat_key))
                 if self.tag_name:
                     del flat_config.dict[flat_key]
                     flat_key = clean_tag(flat_key, self.tag_name)
                 flat_config.dict[flat_key] = self.func(value)
         return flat_config
 
 
+class _ProcessingKeepProperty(Processing):
+    """Processing class for make_processing_keep_property."""
+
+    def __init__(
+        self,
+        regex: Optional[str],
+        tag_name: Optional[str],
+        premerge_order: float,
+        postmerge_order: float,
+        func: Callable,
+    ) -> None:
+        super().__init__()
+        self.premerge_order = premerge_order
+        self.postmerge_order = postmerge_order
+        self.regex = regex
+        self.tag_name = tag_name
+        self.func = func
+        self.properties: Dict[str, Any] = {}
+        if self.regex is not None:
+            self.is_in_func = (
+                lambda key: re.match(self.regex, key.split(".")[-1]) is not None
+            )
+        elif self.tag_name is not None:
+            self.is_in_func = lambda key: is_tag_in(key, str(self.tag_name))
+
+    def premerge(self, flat_config: Config) -> Config:
+        """Pre-merge processing."""
+        items = list(flat_config.dict.items())
+        for flat_key, value in items:
+            if self.is_in_func(flat_key):  # type: ignore
+                property_ = self.func(value)
+                clean_key = clean_all_tags(flat_key)
+                if clean_key not in self.properties:
+                    self.properties[clean_key] = property_
+                if self.tag_name:
+                    del flat_config.dict[flat_key]
+                    flat_key = clean_tag(flat_key, self.tag_name)
+                    flat_config.dict[flat_key] = value
+        return flat_config
+
+    def postmerge(self, flat_config: Config) -> Config:
+        """Post-merge processing."""
+        for flat_key, value in self.properties.items():
+            if flat_key in flat_config.dict:
+                property_ = self.func(flat_config.dict[flat_key])
+                if property_ != value:
+                    raise ValueError(
+                        f"Property of key {flat_key} has changed from {value} to "
+                        f"{property_} while it is protected by a keep-property "
+                        "processing (problem found on post-merge)."
+                    )
+        return flat_config
+
+
 def create_processing_value(
     func: Callable,
     regex: Optional[str] = None,
     tag_name: Optional[str] = None,
     order: float = 0.0,
     *,
-    persistent: bool = False,
+    persistent: bool = True,
 ) -> Processing:
     r"""Create a processing object that modifies a value in dict using tag or regex.
 
     The processing is applied on pre-merge. It triggers when the key matches
-    the tag or the regex. The function apply flat_dict[key] = func(flat_dict[key]).
+    the tag or the regex. The function apply ``flat_dict[key] = func(flat_dict[key])``.
     You must only provide one of tag or regex. If tag is provided, the tag will be
     removed from the key during pre-merge.
 
     Parameters
     ----------
     func : Callable
         The function to apply to the value to make new_value.
     regex : Optional[str]
         The regex to match the key.
     tag_name : Optional[str]
-        The tag (without "@") to match the key. The values are modified when
-        triggering the pattern ".*@<tag_name>.*" and the tag is removed from the key.
+        The tag (without "@") to match the key. The tag is removed from
+        the key after triggering.
     order : int, optional
         The pre-merge order. By default 0.0.
     persistent : bool, optional
         If True, the processing will be applied on all keys that have already
         matched the tag before. By nature, regex processing are always persistent.
-        By default, False.
+        By default, True.
 
     Raises
     ------
     ValueError
         If both tag and regex are provided or if none of them are provided.
 
     Returns
@@ -145,86 +201,34 @@
         {'number1': -1, 'number2': -1, 'number3': 0}
     """
     if tag_name is not None:
         if regex is not None:
             raise ValueError("You must provide a tag or a regex but not both.")
     else:
         if regex is None:
-            raise ValueError("You must provide a tag or a regex "
-                             "(to trigger the value update).")
+            raise ValueError(
+                "You must provide a tag or a regex (to trigger the value update)."
+            )
     if persistent:
         return _ProcessingValuePersistent(regex, tag_name, order, func)
     return _ProcessingValue(regex, tag_name, order, func)
 
 
-class _ProcessingKeepProperty(Processing):
-    """Processing class for make_processing_keep_property."""
-
-    def __init__(
-        self,
-        regex: Optional[str],
-        tag_name: Optional[str],
-        premerge_order: float,
-        postmerge_order: float,
-        func: Callable,
-    ) -> None:
-        super().__init__()
-        self.premerge_order = premerge_order
-        self.postmerge_order = postmerge_order
-        self.regex = regex
-        self.tag_name = tag_name
-        self.func = func
-        self.properties: Dict[str, Any] = {}
-        if self.regex is not None:
-            self.is_in_func = lambda key: re.match(
-                self.regex, key.split('.')[-1]
-            ) is not None
-        elif self.tag_name is not None:
-            self.is_in_func = lambda key: is_tag_in(key, str(self.tag_name))
-
-    def premerge(self, flat_config: Config) -> Config:
-        """Pre-merge processing."""
-        items = list(flat_config.dict.items())
-        for flat_key, value in items:
-            if self.is_in_func(flat_key):  # type: ignore
-                property_ = self.func(value)
-                clean_key = clean_all_tags(flat_key)
-                if clean_key not in self.properties:
-                    self.properties[clean_key] = property_
-                if self.tag_name:
-                    del flat_config.dict[flat_key]
-                    flat_key = clean_tag(flat_key, self.tag_name)
-                    flat_config.dict[flat_key] = value
-        return flat_config
-
-    def postmerge(self, flat_config: Config) -> Config:
-        """Post-merge processing."""
-        for flat_key, value in self.properties.items():
-            if flat_key in flat_config.dict:
-                property_ = self.func(flat_config.dict[flat_key])
-                if property_ != value:
-                    raise ValueError(
-                        f"Property of key {flat_key} has changed from {value} to "
-                        f"{property_} while it is protected by a keep-property "
-                        "processing (problem found on post-merge)."
-                    )
-        return flat_config
-
-
 def create_processing_keep_property(
     func: Callable,
     regex: Optional[str] = None,
     tag_name: Optional[str] = None,
     premerge_order: float = 0.0,
     postmerge_order: float = 0.0,
 ) -> Processing:
-    """Create a processing object that keep a property of a value using tag or regex.
+    """Create a processing object that keep a property from a value using tag or regex.
 
     The pre-merge processing looks for keys that match the tag or the regex, apply
-    the function func on the value and store the result (= the "property").
+    the function func on the value and store the result (= the "property"):
+    ``property = func(flat_dict[key])``.
     The post-merge processing will check that the property is the same as the one
     stored during pre-merge. If not, it will raise a ValueError.
 
     Parameters
     ----------
     func : Callable
         The function to apply to the value to define the property to keep.
@@ -244,38 +248,41 @@
         If both tag and regex are provided or if none of them are provided.
 
     Returns
     -------
     Processing
         The processing object with the pre-merge and post-merge methods.
 
+    Note
+    ----
+
+        The property to keep can be updated by using the tag a second time.
+
     Examples
     --------
     A processing that enforce the types of all the parameters to be constant
     (equal to the type of the first value encountered):
 
-    ```python
-    create_processing_keep_property(type, regex=".*", premerge_order=15.0,
-                                    postmerge_order=15.0)
-    ```
+    ::
+
+        create_processing_keep_property(type, regex=".*", premerge_order=15.0,
+                                        postmerge_order=15.0)
+
     A processing that protect parameters tagged with @protect from being changed:
 
-    ```python
-    create_processing_keep_property(lambda x: x, tag_name="protect",
-                                    premerge_order=15.0, postmerge_order=15.0)
-    ```
+    ::
+
+        create_processing_keep_property(lambda x: x, tag_name="protect",
+                                        premerge_order=15.0, postmerge_order=15.0)
     """
     if tag_name is not None:
         if regex is not None:
             raise ValueError("You must provide a tag or a regex but not both.")
     else:
         if regex is None:
-            raise ValueError("You must provide a tag or a regex "
-                             "(to trigger the value update).")
+            raise ValueError(
+                "You must provide a tag or a regex (to trigger the value update)."
+            )
     processing = _ProcessingKeepProperty(
-        regex,
-        tag_name,
-        premerge_order,
-        postmerge_order,
-        func
+        regex, tag_name, premerge_order, postmerge_order, func
     )
     return processing
```

### Comparing `cliconfig-0.6.1/cliconfig/tag_routines.py` & `cliconfig-0.6.2/cliconfig/tag_routines.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,111 @@
-"""Routines to manipulate the tags on the keys of a dict."""
+"""Routines to manipulate the tags on the keys of a dict.
+
+Used by the processing functions.
+"""
 import copy
 import re
 from typing import Any, Dict, List, Tuple
 
 
 def clean_tag(flat_key: str, tag_name: str) -> str:
     """Clean a tag from a flat key.
 
-    It removes all occurences of the tag with the exact name.
+    It removes all occurrences of the tag with the exact name.
 
+    Parameters
+    ----------
     flat_key : str
         The flat key to clean.
     tag_name : str
         The name of the tag to remove, with or without the '@' prefix.
 
+    Returns
+    -------
+    flat_key : str
+        The cleaned flat key.
+
     Note
     ----
-        `tag_name` is supposed to be the exact name of the tag.
+        ``tag_name`` is supposed to be the exact name of the tag.
 
     Examples
     --------
     ::
 
         >>> clean_tag('abc@tag.def@tag_2.ghi@tag', 'tag')
         abc.def@tag_2.ghi
     """
     if tag_name[0] == "@":
         tag_name = tag_name[1:]
     # Replace "@tag@other_tag" by "@other_tag"
-    parts = flat_key.split(f'@{tag_name}@')
+    parts = flat_key.split(f"@{tag_name}@")
     flat_key = "@".join(parts)
     # Replace "@tag." by "."
-    parts = flat_key.split(f'@{tag_name}.')
+    parts = flat_key.split(f"@{tag_name}.")
     flat_key = ".".join(parts)
     # Remove "@tag" at the end of the string
-    if flat_key.endswith(f'@{tag_name}'):
-        flat_key = flat_key[:-len(f'@{tag_name}')]
+    if flat_key.endswith(f"@{tag_name}"):
+        flat_key = flat_key[: -len(f"@{tag_name}")]
     return flat_key
 
 
-# clean_all_tags, dict_clean_tags
-
 def clean_all_tags(flat_key: str) -> str:
     """Clean all tags from a flat key.
 
     Parameters
     ----------
     flat_key : str
         The flat key to clean.
 
     Returns
     -------
     flat_key : str
         The cleaned flat key.
     """
-    list_keys = flat_key.split('.')
+    list_keys = flat_key.split(".")
     for i, key in enumerate(list_keys):
-        key = re.sub(r'@.*', '', key)
+        key = re.sub(r"@.*", "", key)
         list_keys[i] = key
-    flat_key = '.'.join(list_keys)
+    flat_key = ".".join(list_keys)
     return flat_key
 
 
 def dict_clean_tags(flat_dict: Dict[str, Any]) -> Tuple[Dict[str, Any], List[str]]:
-    """Clean a dict from all tags and return the list of keys with tags."""
+    """Clean a dict from all tags and return the list of keys with tags.
+
+    Parameters
+    ----------
+    flat_dict : Dict[str, Any]
+        The flat dict to clean.
+
+    Returns
+    -------
+    clean_dict : Dict[str, Any]
+        The cleaned flat dict without tags in the keys.
+    tagged_keys : List[str]
+        The list of keys with tags that have been cleaned.
+    """
     items = list(flat_dict.items())
     clean_dict = copy.deepcopy(flat_dict)
     tagged_keys = []
     for key, value in items:
-        if '@' in key:
+        if "@" in key:
             del clean_dict[key]
             clean_dict[clean_all_tags(key)] = value
             tagged_keys.append(key)
     return clean_dict, tagged_keys
 
 
 def is_tag_in(flat_key: str, tag_name: str, *, full_key: bool = False) -> bool:
     """Check if a tag is in a flat key.
 
     The tag name must be the exact name, with or without the "@".
-    It supports the case where there are tags that are prefixes or suffixes of
-    the considered tag.
+    It supports the case where there are other tags that are prefixes
+    or suffixes of the considered tag.
 
     Parameters
     ----------
     flat_key : str
         The flat key to check.
     tag_name : str
         The name of the tag to check, with or without the '@' prefix.
@@ -97,12 +118,14 @@
     -------
     bool
         True if the tag is in the flat key, False otherwise.
     """
     if tag_name[0] == "@":
         tag_name = tag_name[1:]
     if not full_key:
-        flat_key = flat_key.split('.')[-1]
-    is_in = (flat_key.endswith(f"@{tag_name}")
-             or f"@{tag_name}@" in flat_key
-             or f"@{tag_name}." in flat_key)
+        flat_key = flat_key.split(".")[-1]
+    is_in = (
+        flat_key.endswith(f"@{tag_name}")
+        or f"@{tag_name}@" in flat_key
+        or f"@{tag_name}." in flat_key
+    )
     return is_in
```

### Comparing `cliconfig-0.6.1/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.6.2/README_pypi.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cliconfig
-Version: 0.6.1
-Summary: Merge your config files and set parameters from the command line in a simple way.
-Author-email: Valentin Goldite <valentin.goldite@gmail.com>
-Project-URL: Source, https://github.com/valentingol/cliconfig
-Keywords: logging,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CLI Config
 
 </p>
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
@@ -83,25 +71,25 @@
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 ```yaml
----  # main.yaml
+# main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 config3.select@select: config3.param1
 
---- # sub1.yaml
+# sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
---- # sub2.yaml
+# sub2.yaml
 config2.param@type:None|int: 2
 config3:
   param1: 0
   param2: 1
 ```
 
 Here `main.yaml` is interpreted like:
```

### Comparing `cliconfig-0.6.1/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.6.2/cliconfig.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 cliconfig.egg-info/top_level.txt
 cliconfig/processing/__init__.py
 cliconfig/processing/_type_parser.py
 cliconfig/processing/base.py
 cliconfig/processing/builtin.py
 cliconfig/processing/create.py
 docs/Makefile
-docs/cliconfig.processing.rst
+docs/cliconfig.processing_api.rst
 docs/cliconfig_api.rst
 docs/conf.py
 docs/contribute.md
 docs/edge_cases.md
 docs/index.rst
 docs/installation.md
 docs/license.md
@@ -62,14 +62,15 @@
 tests/conftest.py
 tests/configs/config1.yaml
 tests/configs/config2.yaml
 tests/configs/configtag1.yaml
 tests/configs/configtag2.yaml
 tests/configs/default1.yaml
 tests/configs/default2.yaml
+tests/configs/multi_files.yaml
 tests/configs/delete/config1.yaml
 tests/configs/delete/config2.yaml
 tests/configs/integration/test1/main.yaml
 tests/configs/integration/test1/sub1.yaml
 tests/configs/integration/test1/sub2.yaml
 tests/configs/integration/test2/data.yaml
 tests/configs/integration/test2/default.yaml
@@ -82,17 +83,18 @@
 tests/configs/merge/additional1.yaml
 tests/configs/merge/additional2.yaml
 tests/configs/merge/additional3.yaml
 tests/configs/merge/default1.yaml
 tests/configs/merge/default2.yaml
 tests/configs/merge/default3.yaml
 tests/integration/test_inte_multiple_tags.py
+tests/unit/test_base_config.py
 tests/unit/test_cli_parser.py
 tests/unit/test_config_routines.py
 tests/unit/test_dict_routines.py
 tests/unit/test_ex_docs.py
 tests/unit/test_process_routines.py
 tests/unit/test_tag_routines.py
-tests/unit/processing/test_base.py
+tests/unit/processing/test_base_processing.py
 tests/unit/processing/test_builtin.py
 tests/unit/processing/test_create.py
 tests/unit/processing/test_type_parser.py
```

### Comparing `cliconfig-0.6.1/docs/Makefile` & `cliconfig-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/docs/_static/logo.png` & `cliconfig-0.6.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/docs/_static/logo_extend.png` & `cliconfig-0.6.2/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/docs/cliconfig_api.rst` & `cliconfig-0.6.2/docs/cliconfig_api.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 CLI Config API
 ==============
 
 .. toctree::
    :maxdepth: 4
 
-   cliconfig.processing
+   cliconfig.processing_api
+
+cliconfig.base module
+---------------------
+
+.. automodule:: cliconfig.base
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 cliconfig.config\_routines
 --------------------------
 
 .. automodule:: cliconfig.config_routines
    :members:
    :undoc-members:
@@ -18,14 +26,23 @@
 ---------------------
 
 .. automodule:: cliconfig.cli_parser
    :members:
    :undoc-members:
    :show-inheritance:
 
+cliconfig.tag\_routines
+-----------------------
+
+.. automodule:: cliconfig.tag_routines
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+
 cliconfig.dict\_routines
 ------------------------
 
 .. automodule:: cliconfig.dict_routines
    :members:
    :undoc-members:
    :show-inheritance:
@@ -33,15 +50,7 @@
 cliconfig.process\_routines
 ---------------------------
 
 .. automodule:: cliconfig.process_routines
    :members:
    :undoc-members:
    :show-inheritance:
-
-cliconfig.tag\_routines
------------------------
-
-.. automodule:: cliconfig.tag_routines
-   :members:
-   :undoc-members:
-   :show-inheritance:
```

### Comparing `cliconfig-0.6.1/docs/conf.py` & `cliconfig-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/docs/edge_cases.md` & `cliconfig-0.6.2/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/docs/index.rst` & `cliconfig-0.6.2/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -52,25 +52,25 @@
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 .. code:: yaml
 
-    ---  # main.yaml
+    # main.yaml
     path_1@merge_add: sub1.yaml
     path_2@merge_add: sub2.yaml
     config3.select@select: config3.param1
 
-    --- # sub1.yaml
+    # sub1.yaml
     config1:
       param@copy@type:int: config2.param
       param2@type:None|int: 1
 
-    --- # sub2.yaml
+    # sub2.yaml
     config2.param@type:int: 2
     config3:
       param1: 0
       param2: 1
 
 Here `main.yaml` will be interpreted like:
```

### Comparing `cliconfig-0.6.1/docs/license.md` & `cliconfig-0.6.2/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/docs/make.bat` & `cliconfig-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/docs/processing.md` & `cliconfig-0.6.2/docs/processing.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 the config and consequently affect the behavior of subsequent processings.
 To manage this order, the processing class have four float attributes representing
 the order of the four processing methods: premerge, postmerge, postload, and presave.
 
 Here's a basic example to illustrate the significance of the order:
 
 ```yaml
---- # config.yaml
+# config.yaml
 param1@type:int@copy: 'param2'
 param2@type:int: 1
 ```
 
 In this example, we want to enforce the types of the parameters. Additionally, `param1`
 is intended to be a copy of `param2` and naturally, it is forced to have the same type.
 
@@ -96,15 +96,15 @@
 To simplify the creation of such a process, we provide the `cliconfig.create_processing_value` function.
 This function allows you to quickly create a processing that matches a regular
 expression or a specific tag name (in which case the tag is removed after pre-merging).
 You specify the function to be applied on the value to modify it, and optionally,
 the order of the processing. Additionally, there is a `persistent` argument, which is
 a boolean value indicating whether encountering the tag (if a tag is used) once in
 a parameter name will continue to trigger the processing for this parameter
-even after the tag is removed.
+even after the tag is removed. By default, it is `True`.
 
 Here's an example to illustrate:
 
 ```python
 proc = create_processing_value(lambda x: str(x), tag='convert_str', persistent=True)
 config = make_config(default_config, process_list=[proc])
 ```
@@ -253,20 +253,20 @@
 
 For example, consider the tag "@merge_add," which triggers a processing before
 merging and merges the config loaded from a specified path (the value) into the
 current config. We may want to see what happens if we merge a config that also
 contains an "@merge_add" tag within it:
 
 ```yaml
---- # main.yaml
+# main.yaml
 config_path1@merge_add: path1.yaml
---- # path1.yaml
+# path1.yaml
 param1: 1
 config_path2@merge_add: path2.yaml
---- # path2.yaml
+# path2.yaml
 param2: 2
 ```
 
 Now, let's consider we want to merge the config `main.yaml` with another config.
 During the pre-merge processing, we encounter the tag `@merge_add`. This tag is
 removed, and the config found at `path1.yaml` will be merged into the `main.yaml`
 config. However before this, it triggers the pre-merging.
```

### Comparing `cliconfig-0.6.1/docs/quickstart.md` & `cliconfig-0.6.2/docs/quickstart.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Quick start
 
 Create a default configuration that can be split across multiple files that will
 be merged in sequence. There is no depth limit for the
 configuration parameters.
 
 ```yaml
----  # default1.yaml
+# default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
   letter2: b
 
----  # default2.yaml
+# default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
 Now you can write these following lines in your python program to use this config
 with `make_config`:
@@ -29,19 +29,19 @@
 show_config(config)  # print the config to check it
 ```
 
 Then you can add one or multiple additional config files that will be passed on
 command line and that will override the default values.
 
 ```yaml
----  # first.yaml
+# first.yaml
 letters:
   letter3: C
 
----  # second.yaml
+# second.yaml
 param1: -1
 letters.letter1: A
 ```
 
 **Please note that the additional config files must not introduce new parameters that
 are not in the default configs, as it will result in an error**. This
 restriction is in place to prevent potential typos in the config files from
@@ -74,14 +74,18 @@
         letter1: A
         letter2: B
         letter3: C
 ```
 
 Note that the configurations is stored as native python dict at each step of the process.
 
+You can also use multiple documents in a single YAML file with the `---` separator. In
+this case, the configs of the documents are merged in sequence and the file is interpreted
+as a single additional config file containing this merged configuration.
+
 ## Use tags
 
 By default, the package provides some "tags" represented as strings that start with
 '@' and are placed at the end of a key containing a parameter. These tags change
 the way the configuration is processed.
 
 The default tags include:
@@ -114,25 +118,25 @@
 
 Please note that the tags serve as triggers for internal processing and will be
 automatically removed from the key after processing.
 
 It is also possible to combine multiple tags. For example:
 
 ```yaml
----  # main.yaml
+# main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 config3.select@select: config3.param1
 
---- # sub1.yaml
+# sub1.yaml
 config1:
   param@copy@type:int: config2.param
   param2@type:int: 1
 
---- # sub2.yaml
+# sub2.yaml
 config2.param@type:None|int: 2
 config3:
   param1: 0
   param2: 1
 ```
 
 Here `main.yaml` is interpreted like:
```

### Comparing `cliconfig-0.6.1/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.6.2/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/github_actions_utils/pylint_manager.py` & `cliconfig-0.6.2/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/github_actions_utils/pytest_manager.py` & `cliconfig-0.6.2/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.6.2/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/pre-commit-checks.sh` & `cliconfig-0.6.2/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/pyproject.toml` & `cliconfig-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/tests/configs/integration/test2/default.yaml` & `cliconfig-0.6.2/tests/configs/integration/test2/default.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/tests/conftest.py` & `cliconfig-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/tests/integration/test_inte_multiple_tags.py` & `cliconfig-0.6.2/tests/integration/test_inte_multiple_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,19 @@
         "config3": {
             "select": "config3.param1",
             "param1": 0,
         },
     }
     check.equal(config.dict, expected_config)
     with pytest.raises(
-        ValueError,
-        match="Key previously tagged with '@type:None|int'.*"
+        ValueError, match="Key previously tagged with '@type:None|int'.*"
     ):
         merge_flat_processing(
             config,
-            Config({'config2.param': 5.6}, []),
+            Config({"config2.param": 5.6}, []),
             preprocess_first=False,
         )
     sys.argv = sys_argv
 
 
 def test_multiple_tags2() -> None:
     """2nd integration test for multiple tags."""
@@ -62,37 +61,38 @@
         "tests/configs/integration/test2/exp2.yaml]",
         "--train.n_epochs=20",
         "--train.optimizer.momentum=0",
         "--train.optimizer.type=Adam",
     ]
 
     def func_pos_enc_type(x: str) -> str:
-        if x in ['absolute', 'relative', 'embed']:
+        if x in ["absolute", "relative", "embed"]:
             return x
         raise ValueError(f"Invalid value for pos_enc_type: {x}")
 
     def func_optim_type(x: str) -> str:
-        if x in ['SGD', 'Adam']:
+        if x in ["SGD", "Adam"]:
             return x
         raise ValueError(f"Invalid value for optim_type: {x}")
+
     proc_pos_enc_type = create_processing_value(
         func_pos_enc_type,
-        tag_name='pos_enc',
+        tag_name="pos_enc",
         order=20,
         persistent=True,
     )
     proc_optim_type = create_processing_value(
         func_optim_type,
-        tag_name='optim_type',
+        tag_name="optim_type",
         order=20,
         persistent=True,
     )
     proc_protect = create_processing_keep_property(
         func=lambda x: x,
-        tag_name='protect',
+        tag_name="protect",
         premerge_order=-15,
         postmerge_order=15,
     )
     proc_run_id = create_processing_value(
         lambda run_id: run_id if run_id is not None else random.randint(0, 1000000),
         regex="run_id.*",
     )
@@ -132,37 +132,31 @@
     config_dict = deepcopy(config.dict)
     del config_dict["run_id"]
     check.equal(config_dict, expected_dict)
     save_config(config, "tests/tmp/config.yaml")
     saved_dict = load_dict("tests/tmp/config.yaml")
     check.equal(
         saved_dict["data"]["augmentation@type:List[str]"],
-        ["RandomHorizontalFlip", "RandomVerticalFlip"]
+        ["RandomHorizontalFlip", "RandomVerticalFlip"],
     )
     check.equal(
-        saved_dict["models"]["archi_name@type:None|str@select"],
-        "models.vit_b16"
+        saved_dict["models"]["archi_name@type:None|str@select"], "models.vit_b16"
     )
     check.equal(
-        saved_dict["models"]["vit_b16"]["in_size@type:int@copy"],
-        "data.data_size"
+        saved_dict["models"]["vit_b16"]["in_size@type:int@copy"], "data.data_size"
     )
     config = load_config(
         "tests/tmp/config.yaml",
         ["tests/configs/integration/test2/default.yaml"],
-        config.process_list
+        config.process_list,
     )
     del config.dict["run_id"]
     check.equal(config.dict, expected_dict)
+    with pytest.raises(ValueError, match="Key previously tagged with '@type:int.*"):
+        merge_flat_processing(config, Config({"models.vit_b16.n_blocks": 5.6}, []))
     with pytest.raises(
-        ValueError,
-        match="Key previously tagged with '@type:int.*"
-    ):
-        merge_flat_processing(config, Config({'models.vit_b16.n_blocks': 5.6}, []))
-    with pytest.raises(
-        ValueError,
-        match="Found attempt to modify a key with '@copy' tag.*"
+        ValueError, match="Found attempt to modify a key with '@copy' tag.*"
     ):
-        merge_flat_processing(config, Config({'models.vit_b16.in_size': 224}, []))
+        merge_flat_processing(config, Config({"models.vit_b16.in_size": 224}, []))
 
     shutil.rmtree("tests/tmp")
     sys.argv = sys_argv
```

### Comparing `cliconfig-0.6.1/tests/unit/processing/test_base.py` & `cliconfig-0.6.2/tests/unit/processing/test_base_processing.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from cliconfig.base import Config
 from cliconfig.processing.base import Processing
 
 
 def test_processing() -> None:
     """Test Processing."""
-    class _ProcessingTest(Processing):
 
+    class _ProcessingTest(Processing):
         def __init__(self) -> None:
             super().__init__()
             self.attr = 0
 
     config = Config({"a.b": 1, "b": 2, "c.d.e": 3, "c.d.f": [2, 3]}, [])
     base_process = Processing()
     check.equal(
```

### Comparing `cliconfig-0.6.1/tests/unit/processing/test_builtin.py` & `cliconfig-0.6.2/tests/unit/processing/test_builtin.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         "config2_path@merge_add": "tests/configs/merge/default2.yaml",
     }
     with pytest.raises(
         ValueError,
         match=(
             "@merge_add doest not allow to add "
             "already existing keys but key 'config3.param1'.*"
-        )
+        ),
     ):
         processing.premerge(Config(flat_dict, [processing]))
 
     # Test @merge_before and @merge_after
     flat_dict = {
         "a.b": 1,
         "a.b_path@merge_after": "tests/configs/merge/additional2.yaml",
@@ -90,114 +90,111 @@
     for tag in ["merge_before", "merge_after", "merge_add"]:
         with pytest.raises(
             ValueError,
             match=re.escape(
                 f"Key with '@{tag}' tag must be associated "
                 "to a string corresponding to a *yaml* file."
                 f"The problem occurs at key: a@{tag}"
-            )
+            ),
         ):
-            processing.premerge(Config({f'a@{tag}': 'no_yaml'}, [processing]))
+            processing.premerge(Config({f"a@{tag}": "no_yaml"}, [processing]))
 
 
 def test_process_copy() -> None:
     """Test ProcessCopy."""
     processing = ProcessCopy()
     flat_dict = {
         "config1.param1": 1,
-        "config2.param2@copy": 'config1.param1',
+        "config2.param2@copy": "config1.param1",
     }
     flat_config = Config(flat_dict, [processing])
     flat_config = processing.premerge(flat_config)
     check.equal(
-        flat_config.dict,
-        {"config1.param1": 1, "config2.param2": 'config1.param1'}
+        flat_config.dict, {"config1.param1": 1, "config2.param2": "config1.param1"}
     )
     flat_config.dict["config1.param1"] = 2
     flat_config = processing.postmerge(flat_config)
     check.equal(flat_config.dict, {"config1.param1": 2, "config2.param2": 2})
     flat_config = processing.presave(flat_config)
     check.equal(processing.current_value, {"config2.param2": 2})
     check.equal(
-        flat_config.dict,
-        {"config1.param1": 2, "config2.param2@copy": 'config1.param1'}
+        flat_config.dict, {"config1.param1": 2, "config2.param2@copy": "config1.param1"}
     )
     check.equal(processing.keys_to_copy, {"config2.param2": "config1.param1"})
     check.equal(flat_config.process_list, [processing])
     # Reset copy processing
     processing.keys_to_copy = {}
     # Case of wrong key
     with pytest.raises(
         ValueError,
         match=(
             "Key with '@copy' tag must be associated "
             "to a string corresponding to a flat key. "
             "The problem occurs at key: a@copy with value: True"
-        )
+        ),
     ):
         processing.premerge(Config({"a@copy": True}, [processing]))
     # Case of already existing @copy but associated to an other key
     processing.keys_to_copy = {"a": "b"}
     with pytest.raises(
         ValueError,
         match=(
             "Key with '@copy' has change its value to copy. Found key: a@copy@tag "
             "with value: c, previous value to copy: b"
-        )
+        ),
     ):
         processing.premerge(Config({"a@copy@tag": "c"}, [processing]))
     # Case of non-existing key (on post-merge): do not raise error
     processing.keys_to_copy = {"a": "b"}
     processing.postmerge(Config({"a": "b"}, [processing]))
     # Case overwriting a key
     processing.current_value = {"a": 2}
     with pytest.raises(
         ValueError,
         match=re.escape(
             "Found attempt to modify a key with '@copy' tag. The key is "
             "then protected against updates (except the copied value or "
             "the original key to copy). Found key: a of value c that copy "
             "b of value 1"
-        )
+        ),
     ):
         processing.postmerge(Config({"a": "c", "b": 1}, [processing]))
 
 
 def test_process_typing() -> None:
     """Test ProcessTyping."""
     processing = ProcessTyping()
     flat_dict = {
         "param1@type:int": 1,
-        "param2@type:List[Optional[Dict[str, int|float]]]": [{'a': [0.0]}],
+        "param2@type:List[Optional[Dict[str, int|float]]]": [{"a": [0.0]}],
     }
     flat_config = Config(flat_dict, [processing])
     flat_config = processing.premerge(flat_config)
-    flat_config.dict['param1'] = 3
-    flat_config.dict['param2'] = {'a': None, 'b': [{'c': 1}]}
+    flat_config.dict["param1"] = 3
+    flat_config.dict["param2"] = {"a": None, "b": [{"c": 1}]}
     flat_config.dict = flatten(flat_config.dict)
     flat_config = processing.postmerge(flat_config)
     check.equal(
-        flat_config.dict,
-        {"param1": 3, "param2.a": None, "param2.b": [{'c': 1}]}
+        flat_config.dict, {"param1": 3, "param2.a": None, "param2.b": [{"c": 1}]}
     )
     check.equal(
         flat_config.process_list[0].forced_types,  # type: ignore
         {
-            "param1": (int, ),
-            "param2": (('list', ((type(None), ('dict', (str,), (int, float))),)),)
-        }
+            "param1": (int,),
+            "param2": (("list", ((type(None), ("dict", (str,), (int, float))),)),),
+        },
     )
     check.equal(
         flat_config.process_list[0].type_desc,  # type: ignore
-        {"param1": "int", "param2": "List[Optional[Dict[str, int|float]]]"}
+        {"param1": "int", "param2": "List[Optional[Dict[str, int|float]]]"},
     )
     flat_config = processing.presave(flat_config)
     check.equal(
         flat_config.dict,
-        {"param1@type:int": 3, "param2.a": None, "param2.b": [{'c': 1}]}
+        {"param1@type:int": 3, "param2.a": None, "param2.b": [{"c": 1}]},
     )
     processing.forced_types = {}  # Reset forced types
     processing.type_desc = {}  # Reset type description
 
     # Case of different type on pre-merge: do not raise error!
     processing.premerge(Config({"param@type:int": "str"}, [processing]))
 
@@ -205,28 +202,28 @@
     processing.forced_types = {"param": (int,)}
     processing.type_desc = {"param": "int"}
     with pytest.raises(
         ValueError,
         match=(
             "Find the tag '@type:str' on a key that has already been associated "
             "to an other type: int. Find problem at key: param@type:str"
-        )
+        ),
     ):
         processing.premerge(Config({"param@type:str": "str"}, [processing]))
 
     # Case of wrong type in postmerge
     processing.forced_types = {"param": (int,)}
     processing.type_desc = {"param": "int"}
     with pytest.raises(
         ValueError,
         match=(
             "Key previously tagged with '@type:int' must be "
             "associated to a value of type int. Find the "
             "value: mystr of type <class 'str'> at key: param"
-        )
+        ),
     ):
         processing.postmerge(Config({"param": "mystr"}, [processing]))
 
 
 def test_process_select() -> None:
     """Test ProcessSelect."""
     processing = ProcessSelect()
@@ -248,42 +245,41 @@
     config = Config(flat_dict, [])
     config = processing.premerge(config)
     config = processing.postmerge(config)
     check.equal(config.dict, expected_dict)
     config = processing.presave(config)
     check.is_in("models.model_names@select", config.dict)
     check.equal(
-        config.dict["models.model_names@select"],
-        ["models.model1", "models.model3"]
+        config.dict["models.model_names@select"], ["models.model1", "models.model3"]
     )
     check.is_not_in("models.model_names", config.dict)
     with pytest.raises(
         ValueError,
         match=re.escape(
             "The keys in the list of parameters tagged with '@select' must be "
             "identical before the last dot (= on the same subconfig). Find: "
             "abab and dede before the last dot."
-        )
+        ),
     ):
         processing.premerge(Config({"p@select": ["abab.cdcd", "dede.fgfg"]}, []))
     with pytest.raises(
         ValueError,
         match=re.escape(
             "The value of parameters tagged with '@select' must be a string or a "
             "list of strings representing flat key(s). "
-        )
+        ),
     ):
         processing.premerge(Config({"p@select": 0}, []))
     with pytest.raises(
         ValueError,
         match=(
             "Find attempt to delete the configuration at the root. You must pass a "
             "flat key with a least one dot on parameter tagged with @select. "
             "Find key: p@select with value: root"
-        )
+        ),
     ):
         processing.premerge(Config({"p@select": "root"}, []))
 
 
 def test_process_delete() -> None:
     """Test ProcessDelete."""
     processing = ProcessDelete()
@@ -305,29 +301,31 @@
     flat_dict = {
         "config.param1": 1,
         "param1": 2,
     }
     config = Config(flat_dict, [processing])
     check.equal(processing.premerge(config).dict, flat_dict)
 
-    flat_dicts = [{'param1@tag': 1}, {'@foo': 2}, {'@': 3}]
+    flat_dicts = [{"param1@tag": 1}, {"@foo": 2}, {"@": 3}]
     for flat_dict in flat_dicts:
         with pytest.raises(
             ValueError,
             match=(
                 "Keys with tags are encountered at the end of "
                 "the pre-merge process.*"
-            )
+            ),
         ):
             processing.premerge(Config(flat_dict, [processing]))
 
 
 def test_default_processings() -> None:
     """Test DefaultProcessings."""
     config = Config({}, DefaultProcessings().list)
     for proc in [
         ProcessCheckTags(),
         ProcessMerge(),
         ProcessCopy(),
-        ProcessTyping()
+        ProcessTyping(),
+        ProcessDelete(),
+        ProcessSelect()
     ]:
         check.is_in(proc, config.process_list)
```

### Comparing `cliconfig-0.6.1/tests/unit/processing/test_create.py` & `cliconfig-0.6.2/tests/unit/processing/test_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,50 +10,54 @@
     create_processing_value,
 )
 
 
 def test_create_processing_value() -> None:
     """Test create_processing_value."""
     # Persistent
-    proc1 = create_processing_value(lambda x: x + 1, tag_name="add1", order=1.0,
-                                    persistent=True)
-    proc2 = create_processing_value(lambda x: -x, regex="neg_number.*", order=0.0,
-                                    persistent=True)
+    proc1 = create_processing_value(
+        lambda x: x + 1, tag_name="add1", order=1.0, persistent=True
+    )
+    proc2 = create_processing_value(
+        lambda x: -x, regex="neg_number.*", order=0.0, persistent=True
+    )
     in_dict = {"neg_number1": 1, "neg_number2": 1, "neg_number3@add1": 1}
     config = Config(in_dict, [proc1, proc2])
     config = config.process_list[1].premerge(config)
     config = config.process_list[0].premerge(config)
     check.equal(in_dict, {"neg_number1": -1, "neg_number2": -1, "neg_number3": 0})
     config = config.process_list[1].premerge(config)
     config = config.process_list[0].premerge(config)
     check.equal(in_dict, {"neg_number1": 1, "neg_number2": 1, "neg_number3": 1})
     # Non persistent
-    proc2 = create_processing_value(lambda x: -x, regex="neg_number.*", order=0.0,
-                                    persistent=False)
-    proc1 = create_processing_value(lambda x: x + 1, tag_name="add1", order=1.0,
-                                    persistent=False)
+    proc2 = create_processing_value(
+        lambda x: -x, regex="neg_number.*", order=0.0, persistent=False
+    )
+    proc1 = create_processing_value(
+        lambda x: x + 1, tag_name="add1", order=1.0, persistent=False
+    )
     in_dict = {"neg_number1": 1, "neg_number2": 1, "neg_number3@add1": 1}
     config = Config(in_dict, [proc1, proc2])
     config = config.process_list[1].premerge(config)
     config = config.process_list[0].premerge(config)
     check.equal(in_dict, {"neg_number1": -1, "neg_number2": -1, "neg_number3": 0})
     config = config.process_list[1].premerge(config)
     config = config.process_list[0].premerge(config)
     check.equal(in_dict, {"neg_number1": 1, "neg_number2": 1, "neg_number3": 0})
 
     # Failing cases
     with pytest.raises(
-        ValueError,
-        match="You must provide a tag or a regex but not both."
+        ValueError, match="You must provide a tag or a regex but not both."
     ):
         create_processing_value(lambda x: x + 1, tag_name="add1", regex="neg_number.*")
     with pytest.raises(
         ValueError,
-        match=re.escape("You must provide a tag or a regex "
-                        "(to trigger the value update).")
+        match=re.escape(
+            "You must provide a tag or a regex (to trigger the value update)."
+        ),
     ):
         create_processing_value(lambda x: x + 1, order=0.0)
 
 
 def test_create_processing_keep_property() -> None:
     """Test create_processing_keep_property."""
     proc1 = create_processing_keep_property(type, regex=".*")
@@ -67,33 +71,34 @@
     config = config.process_list[1].postmerge(config)
     with pytest.raises(
         ValueError,
         match=re.escape(
             "Property of key str has changed from <class 'str'> to <class 'int'> "
             "while it is protected by a keep-property processing (problem found on "
             "post-merge)."
-        )
+        ),
     ):
         config.process_list[0].postmerge(Config({"str": 0}, []))
     with pytest.raises(
         ValueError,
         match=re.escape(
             "Property of key list has changed from [1, 2, 3] to [1, 2] while "
             "it is protected by a keep-property processing (problem found on "
-            "post-merge).")
+            "post-merge)."
+        ),
     ):
         config.process_list[1].postmerge(Config({"list": [1, 2]}, []))
     config.process_list[0].premerge(Config({"str": 0}, []))  # should not raise
     config.process_list[1].premerge(Config({"list": [1, 2]}, []))  # should not raise
 
     # Failing cases
     with pytest.raises(
-        ValueError,
-        match="You must provide a tag or a regex but not both."
+        ValueError, match="You must provide a tag or a regex but not both."
     ):
         create_processing_keep_property(lambda x: x, tag_name="protect", regex=".*")
     with pytest.raises(
         ValueError,
-        match=re.escape("You must provide a tag or a regex "
-                        "(to trigger the value update).")
+        match=re.escape(
+            "You must provide a tag or a regex (to trigger the value update)."
+        ),
     ):
         create_processing_keep_property(lambda x: x, premerge_order=0.0)
```

### Comparing `cliconfig-0.6.1/tests/unit/processing/test_type_parser.py` & `cliconfig-0.6.2/tests/unit/processing/test_type_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,103 +13,94 @@
     _parse_union,
 )
 
 
 def test_type_parser_isinstance() -> None:
     """Test _parse_type and _isinstance."""
     type_ = _parse_type("None")
-    check.equal(type_, (type(None), ))
+    check.equal(type_, (type(None),))
     check.is_true(_isinstance(None, type_))
     check.is_false(_isinstance([None], type_))
 
     type_ = _parse_type("List[float]")
     check.equal(type_, (("list", (float,)),))
 
     type_ = _parse_type("list|dict")
     check.equal(type_, (list, dict))
     check.is_true(_isinstance([2.0, True], type_))
 
     type_ = _parse_type("Dict[str, List[float]]")
-    check.equal(
-        type_,
-        (('dict', (str,), (('list', (float,)),)),)
-    )
+    check.equal(type_, (("dict", (str,), (("list", (float,)),)),))
     check.is_true(_isinstance({"a": [1.0, 2.0]}, type_))
     check.is_false(_isinstance({"a": [1.0, 2.0], "b": [1.0, 2]}, type_))
 
     type_ = _parse_type("Dict[str|bool, int|float]")
     check.equal(type_, (("dict", (str, bool), (int, float)),))
 
     type_ = _parse_type("Union[Optional[float], Any]")
     check.equal(type_, ((type(None), float), object))
-    check.is_true(_isinstance('2', type_))
+    check.is_true(_isinstance("2", type_))
 
     type_ = _parse_type(
         "Dict[str, Union[List[None|float], Dict[bool, Optional[list]]]]|List[Any]|"
         "Dict[int, Optional[Dict[str, float]]]|Optional[float]"
     )
     check.equal(
         (
             (
-                'dict',
+                "dict",
                 (str,),
                 (
-                    ('list', (type(None), float)),
-                    ('dict', (bool,), ((type(None), list),))
-                )
-            ),
-            ('list', (object,)),
-            (
-                'dict',
-                (int,),
-                ((type(None), ('dict', (str,), (float,))),)
+                    ("list", (type(None), float)),
+                    ("dict", (bool,), ((type(None), list),)),
+                ),
             ),
-            (type(None), float)
+            ("list", (object,)),
+            ("dict", (int,), ((type(None), ("dict", (str,), (float,))),)),
+            (type(None), float),
         ),
         type_,
     )
-    check.is_true(_isinstance({'a': [None, 1.0], 'b': {True: None}}, type_))
+    check.is_true(_isinstance({"a": [None, 1.0], "b": {True: None}}, type_))
     check.is_true(_isinstance([[]], type_))
-    check.is_true(_isinstance({1: {'a': 2.0}}, type_))
-    check.is_false(_isinstance({'a': [None, 1.0], 'b': {False: 1, True: '1'}}, type_))
+    check.is_true(_isinstance({1: {"a": 2.0}}, type_))
+    check.is_false(_isinstance({"a": [None, 1.0], "b": {False: 1, True: "1"}}, type_))
 
     # Wrong type description
     with pytest.raises(ValueError, match="Unknown type: 'unknown'"):
         _parse_type("unknown")
     desc = "str, List[float]"
     with pytest.raises(ValueError, match=re.escape(f"Unknown type: '{desc}'")):
         _parse_type(desc)
     desc = "None||float"
     with pytest.raises(ValueError, match=f"Unknown type: '{desc}'"):
         _parse_type(desc)
-    desc = ("Dict[str, Union[List[None|float], Dict[bool, Optionnal[int]]]]|List[Any]|"
-            "Dict[List[int], Optional[Dict[str, float]]]|float")  # Optionnal with 2 n
+    desc = (
+        "Dict[str, Union[List[None|float], Dict[bool, Optionnal[int]]]]|List[Any]|"
+        "Dict[List[int], Optional[Dict[str, float]]]|float"
+    )  # Optionnal with 2 n
     with pytest.raises(ValueError, match=f"Unknown type: '{desc}'"):
         _parse_type(desc)
 
     # Wrong type in isinstance (here a 'dict' tuple has 3 elements instead of 2)
     wrong_type = (
         (
-            'dict',
+            "dict",
             (str,),
             (
-                ('list', (type(None), float)),
-                ('dict', (bool,), ((type(None), list),), str)
-            )
-        ),
-        ('list', (object,)),
-        (
-            'dict',
-            (int,),
-            ((type(None), ('dict', (str,), (float,))),)
+                ("list", (type(None), float)),
+                ("dict", (bool,), ((type(None), list),), str),
+            ),
         ),
-        (type(None), float)
+        ("list", (object,)),
+        ("dict", (int,), ((type(None), ("dict", (str,), (float,))),)),
+        (type(None), float),
     )
     with pytest.raises(ValueError, match="Invalid type for _isinstance:.*"):
-        _isinstance({'a': {True: 'a'}}, wrong_type)
+        _isinstance({"a": {True: "a"}}, wrong_type)
 
 
 def test_errors_in_parse() -> None:
     """Test error raised in _parse_X functions."""
     with pytest.raises(ValueError, match="Invalid List type:.*"):
         _parse_list("List[bool, str]")
```

### Comparing `cliconfig-0.6.1/tests/unit/test_cli_parser.py` & `cliconfig-0.6.2/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.1/tests/unit/test_config_routines.py` & `cliconfig-0.6.2/tests/unit/test_config_routines.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,15 @@
     check.equal(config.dict, expected_config)
     check.equal(out, expected_out)
 
     # No additional configs
     sys.argv = [
         "tests/test_make_config.py.py",
     ]
-    config = make_config(
-        "tests/configs/default1.yaml",
-        "tests/configs/default2.yaml")
+    config = make_config("tests/configs/default1.yaml", "tests/configs/default2.yaml")
     expected_config = {
         "param1": 1,
         "param2": 2,
         "param3": 3,
         "letters": {
             "letter1": "a",
             "letter2": "b",
```

### Comparing `cliconfig-0.6.1/tests/unit/test_dict_routines.py` & `cliconfig-0.6.2/tests/unit/test_dict_routines.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         {"a.b": 1, "a.c": 2, "c": 3},
     )
     with pytest.raises(ValueError, match="New parameter found 'c'.*"):
         merge_flat(dict1, dict2, allow_new_keys=False)
     dict1 = {"a.b": 1, "a": {"b": 1, "c": 2}}
     with pytest.raises(
         ValueError,
-        match="Duplicated key found.*You may consider calling `clean_pre_flat`.*",
+        match="Duplicated key found.*You may consider calling 'clean_pre_flat'.*",
     ):
         merge_flat(dict1, dict2, allow_new_keys=True)
 
 
 def test_merge_flat_paths() -> None:
     """Test merge_flat_paths."""
     dict1 = {
@@ -151,25 +151,28 @@
         ),
     ):
         clean_pre_flat({"a.b": 1, "a": {"b": 2}, "c": 3}, priority="UNKNOWN")
 
 
 def test_save_load_dict() -> None:
     """Test save_dict and load_dict."""
-    config1 = {"a": 1, "b": {"c": 2}, "d": [2, 3.0], "e": [{"f": 4}]}
-    save_dict(config1, "tests/tmp/config.yaml")
+    dict1 = {"a": 1, "b": {"c": 2}, "d": [2, 3.0], "e": [{"f": 4}]}
+    save_dict(dict1, "tests/tmp/config.yaml")
     check.is_true(os.path.isfile("tests/tmp/config.yaml"))
-    config2 = load_dict("tests/tmp/config.yaml")
-    check.equal(config1, config2)
+    dict2 = load_dict("tests/tmp/config.yaml")
+    check.equal(dict1, dict2)
+    # Case multiple files and yaml tags
+    out_dict = load_dict("tests/configs/multi_files.yaml")
+    check.equal(out_dict, dict1)
     shutil.rmtree("tests/tmp")
 
 
 def test_show_dict() -> None:
     """Test show_dict."""
-    config = {
+    in_dict = {
         "model": {
             "s1_ae_config": {
                 "in_dim": 2,
                 "out_dim": 1,
                 "layer_channels": [16, 32, 64],
                 "conv_per_layer": 1,
                 "residual": False,
@@ -190,8 +193,8 @@
         },
         "data": {
             "dataset": "mnist",
             "batch_size": 128,
             "num_workers": 6,
         },
     }
-    show_dict(config)
+    show_dict(in_dict)
```

### Comparing `cliconfig-0.6.1/tests/unit/test_ex_docs.py` & `cliconfig-0.6.2/tests/unit/test_ex_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,16 +77,18 @@
         for flat_key, value in items:
             if is_tag_in(flat_key, "bypass_typing"):
                 new_key = clean_tag(flat_key, "bypass_typing")
                 flat_config.dict[new_key] = value
                 del flat_config.dict[flat_key]
                 clean_key = clean_all_tags(flat_key)
                 for processing in flat_config.process_list:
-                    if (isinstance(processing, ProcessTyping)
-                            and clean_key in processing.forced_types):
+                    if (
+                        isinstance(processing, ProcessTyping)
+                        and clean_key in processing.forced_types
+                    ):
                         forced_type = processing.forced_types.pop(clean_key)
                         self.bypassed_forced_types[clean_key] = forced_type
         return flat_config
 
 
 def test_process_print_sorted(capsys: pytest.CaptureFixture) -> None:
     """Test ProcessPrintSorted."""
@@ -96,29 +98,21 @@
     merge_flat_processing(config1, config2)
     out = capsys.readouterr().out
     check.equal(out, "The sorted looked values are:  [1, 2, 4]\n")
 
 
 def test_process_bypass_typing() -> None:
     """Test ProcessBypassTyping."""
-    config1 = Config(
-        {"a@type:int": 0}, [ProcessBypassTyping(), ProcessTyping()]
-    )
-    config2 = Config(
-        {"a@bypass_typing@type:str": "a"}, []
-    )
+    config1 = Config({"a@type:int": 0}, [ProcessBypassTyping(), ProcessTyping()])
+    config2 = Config({"a@bypass_typing@type:str": "a"}, [])
     merge_flat_processing(config1, config2)
-    config1 = Config(
-        {"a@type:int": 0}, [ProcessBypassTyping(), ProcessTyping()]
-    )
-    config2 = Config(
-        {"a@type:str": "a"}, []
-    )
+    config1 = Config({"a@type:int": 0}, [ProcessBypassTyping(), ProcessTyping()])
+    config2 = Config({"a@type:str": "a"}, [])
     # Reset ProcessTyping
     with pytest.raises(
         ValueError,
         match=(
             "Find the tag '@type:str' on a key that has already "
             "been associated to an other type: int.*"
-        )
+        ),
     ):
         merge_flat_processing(config1, config2)
```

### Comparing `cliconfig-0.6.1/tests/unit/test_process_routines.py` & `cliconfig-0.6.2/tests/unit/test_process_routines.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 
 def test_merge_flat_processing(
     process_add1: ProcessAdd1,
     process_keep: ProcessKeep,
 ) -> None:
     """Test merge_flat_processing."""
-    class _ProcessingTest(Processing):
 
+    class _ProcessingTest(Processing):
         def __init__(self) -> None:
             super().__init__()
             self.attr = 0
 
     proc1 = _ProcessingTest()
     proc2 = _ProcessingTest()
     proc2.attr = 1
@@ -50,16 +50,15 @@
 
 def test_merge_flat_paths_processing(
     process_add1: ProcessAdd1,
     process_keep: ProcessKeep,
 ) -> None:
     """Test merge_flat_paths_processing."""
     config1 = Config(
-        {"param1@add1": 0, "param2.param3@keep": 1},
-        [process_add1, process_keep]
+        {"param1@add1": 0, "param2.param3@keep": 1}, [process_add1, process_keep]
     )
     config2 = Config({"param2.param3": 3}, [])
     expected_dict = {"param1": 1, "param2.param3": 1}
     check.equal(
         merge_flat_paths_processing(
             "tests/configs/configtag1.yaml",
             "tests/configs/configtag2.yaml",
@@ -83,16 +82,15 @@
 
 def test_save_processing(
     process_add1: ProcessAdd1,
     process_keep: ProcessKeep,
 ) -> None:
     """Test save_processing."""
     config = Config(
-        {"param1@add1": 0, "param2.param3@add1": 1},
-        [process_add1, process_keep]
+        {"param1@add1": 0, "param2.param3@add1": 1}, [process_add1, process_keep]
     )
     save_processing(config, "tests/tmp/config.yaml")
     with open("tests/tmp/config.yaml", "r", encoding="utf-8") as yaml_file:
         loaded_dict = yaml.safe_load(yaml_file)
     check.equal(loaded_dict, {"param1": 1, "param2": {"param3": 2}})
     check.equal(process_keep.keep_vals, {})
     shutil.rmtree("tests/tmp")
@@ -111,21 +109,21 @@
     check.equal(config.dict, {"param2.param3": 0})
     with pytest.raises(
         ValueError,
         match=re.escape(
             "config_or_path must be a Config instance or a path to a yaml file "
             "but you passed a dict. If you want to use it as a valid input, "
             "you should use Config(<input dict>, []) instead."
-        )
+        ),
     ):
         merge_flat_paths_processing(
             {"a": 2},  # type: ignore
             Config({"a": 1}, []),
         )
     with pytest.raises(
         ValueError,
-        match=("config_or_path must be a Config instance or a path to a yaml file.")
+        match=("config_or_path must be a Config instance or a path to a yaml file."),
     ):
         merge_flat_paths_processing(
             Config({"a": 1}, []),
             ("not a path",),  # type: ignore
         )
```

### Comparing `cliconfig-0.6.1/tests/unit/test_tag_routines.py` & `cliconfig-0.6.2/tests/unit/test_tag_routines.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,22 +24,16 @@
         clean_tag(key1, "tag"),
         "abc.def@tag_2.ghi",
     )
     check.equal(
         clean_tag(key1, "@tag"),
         "abc.def@tag_2.ghi",
     )
-    check.equal(
-        clean_tag(key2, "tag"),
-        "abc@hashtag@tagg@tag 2@ag.def@tag _.jkl.mno"
-    )
-    check.equal(
-        clean_tag(key2, "@tag"),
-        "abc@hashtag@tagg@tag 2@ag.def@tag _.jkl.mno"
-    )
+    check.equal(clean_tag(key2, "tag"), "abc@hashtag@tagg@tag 2@ag.def@tag _.jkl.mno")
+    check.equal(clean_tag(key2, "@tag"), "abc@hashtag@tagg@tag 2@ag.def@tag _.jkl.mno")
 
 
 def test_clean_all_tags(key1: str, key2: str) -> None:
     """Test clean_all_tags."""
     check.equal(
         clean_all_tags(key1),
         "abc.def.ghi",
```

