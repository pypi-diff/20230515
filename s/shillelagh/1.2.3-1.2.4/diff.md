# Comparing `tmp/shillelagh-1.2.3.tar.gz` & `tmp/shillelagh-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-1.2.3.tar", last modified: Mon May 15 19:25:08 2023, max compression
+gzip compressed data, was "shillelagh-1.2.4.tar", last modified: Mon May 15 20:08:08 2023, max compression
```

## Comparing `shillelagh-1.2.3.tar` & `shillelagh-1.2.4.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.029486 shillelagh-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.009486 shillelagh-1.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.009486 shillelagh-1.2.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/python-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-15 19:24:53.000000 shillelagh-1.2.3/ARCHITECTURE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 19:24:53.000000 shillelagh-1.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-15 19:24:53.000000 shillelagh-1.2.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-15 19:24:53.000000 shillelagh-1.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 19:24:53.000000 shillelagh-1.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 19:24:53.000000 shillelagh-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-15 19:24:53.000000 shillelagh-1.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-15 19:25:08.029486 shillelagh-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-15 19:24:53.000000 shillelagh-1.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 19:24:53.000000 shillelagh-1.2.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 19:24:53.000000 shillelagh-1.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 19:24:53.000000 shillelagh-1.2.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 19:24:53.000000 shillelagh-1.2.3/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 19:24:53.000000 shillelagh-1.2.3/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-15 19:24:53.000000 shillelagh-1.2.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-15 19:25:08.029486 shillelagh-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-15 19:24:53.000000 shillelagh-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.009486 shillelagh-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/src/shillelagh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/src/shillelagh/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/html_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/s3select.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/file/csvfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/memory/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/vt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/src/shillelagh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/talks/
--rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-05-15 19:24:53.000000 shillelagh-1.2.3/talks/Python Brasil 2021.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.009486 shillelagh-1.2.3/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/templates/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-15 19:24:53.000000 shillelagh-1.2.3/templates/adapter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/templates/adapter/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-05-15 19:24:53.000000 shillelagh-1.2.3/templates/adapter/hooks/post_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 19:24:53.000000 shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-15 19:24:53.000000 shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/tests/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/datasette_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/generic_json_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/github_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/tests/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/html_table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/s3select_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/socrata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/system_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/weatherapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/file/csvfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/memory/pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/registry_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dbapi_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dialects/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dialects/gsheets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dialects/safe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.029486 shillelagh-1.2.3/tests/fakes/
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/cdc_data_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/cdc_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_columns_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_data_response_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_data_response_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/github_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/github_single_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/incidents.json
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/weatherapi_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/types_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.645756 shillelagh-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/python-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-15 20:07:44.000000 shillelagh-1.2.4/ARCHITECTURE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 20:07:44.000000 shillelagh-1.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-15 20:07:44.000000 shillelagh-1.2.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-15 20:07:44.000000 shillelagh-1.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 20:07:44.000000 shillelagh-1.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 20:07:44.000000 shillelagh-1.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-15 20:07:44.000000 shillelagh-1.2.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-15 20:08:08.645756 shillelagh-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-15 20:07:44.000000 shillelagh-1.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 20:07:44.000000 shillelagh-1.2.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 20:07:44.000000 shillelagh-1.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 20:07:44.000000 shillelagh-1.2.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 20:07:44.000000 shillelagh-1.2.4/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 20:07:44.000000 shillelagh-1.2.4/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-15 20:07:44.000000 shillelagh-1.2.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-15 20:08:08.645756 shillelagh-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-15 20:07:44.000000 shillelagh-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.613755 shillelagh-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/src/shillelagh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/src/shillelagh/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/html_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/s3select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/file/csvfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/memory/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/vt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/src/shillelagh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.629755 shillelagh-1.2.4/talks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-05-15 20:07:44.000000 shillelagh-1.2.4/talks/Python Brasil 2021.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.613755 shillelagh-1.2.4/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.629755 shillelagh-1.2.4/templates/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-15 20:07:44.000000 shillelagh-1.2.4/templates/adapter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.629755 shillelagh-1.2.4/templates/adapter/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-05-15 20:07:44.000000 shillelagh-1.2.4/templates/adapter/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.633756 shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 20:07:44.000000 shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-15 20:07:44.000000 shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.633756 shillelagh-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.633756 shillelagh-1.2.4/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.633756 shillelagh-1.2.4/tests/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/datasette_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/generic_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/github_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/html_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/s3select_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/socrata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/weatherapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/file/csvfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/memory/pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/registry_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dbapi_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.641755 shillelagh-1.2.4/tests/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dialects/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dialects/gsheets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dialects/safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.645756 shillelagh-1.2.4/tests/fakes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/cdc_data_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/cdc_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_columns_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_data_response_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_data_response_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/github_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/github_single_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/weatherapi_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/types_test.py
```

### Comparing `shillelagh-1.2.3/.coveragerc` & `shillelagh-1.2.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.github/ISSUE_TEMPLATE/bug_report.md` & `shillelagh-1.2.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.github/ISSUE_TEMPLATE/feature_request.md` & `shillelagh-1.2.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.github/pull_request_template.md` & `shillelagh-1.2.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.github/workflows/codeql-analysis.yml` & `shillelagh-1.2.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.github/workflows/python-integration.yml` & `shillelagh-1.2.4/.github/workflows/python-integration.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.github/workflows/python-package-daily.yml` & `shillelagh-1.2.4/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.github/workflows/python-package.yml` & `shillelagh-1.2.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.github/workflows/python-publish.yml` & `shillelagh-1.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.gitignore` & `shillelagh-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.pre-commit-config.yaml` & `shillelagh-1.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/.readthedocs.yml` & `shillelagh-1.2.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/ARCHITECTURE.rst` & `shillelagh-1.2.4/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/CHANGELOG.rst` & `shillelagh-1.2.4/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 1.2.4 - 2023-05-15
+==========================
+
+- Relax dependency for ``requests-cache`` correctly (#362)
+
 Version 1.2.3 - 2023-05-15
 ==========================
 
 - Add ``yarl`` dependency to the generic JSON adapter (#355)
 - Only warn of errors when loading adapters if they are explicitly requested (#360)
 - Relax dependency for ``requests-cache`` (#361)
```

### Comparing `shillelagh-1.2.3/CODE_OF_CONDUCT.md` & `shillelagh-1.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/CONTRIBUTING.rst` & `shillelagh-1.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/LICENSE.txt` & `shillelagh-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/Makefile` & `shillelagh-1.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/PKG-INFO` & `shillelagh-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.3
+Version: 1.2.4
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.3/README.rst` & `shillelagh-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/docs/Makefile` & `shillelagh-1.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/docs/adapters.rst` & `shillelagh-1.2.4/docs/adapters.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/docs/conf.py` & `shillelagh-1.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/docs/development.rst` & `shillelagh-1.2.4/docs/development.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/docs/install.rst` & `shillelagh-1.2.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/docs/usage.rst` & `shillelagh-1.2.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/examples/csvfile.py` & `shillelagh-1.2.4/examples/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/examples/dataframe.py` & `shillelagh-1.2.4/examples/dataframe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/examples/datasette.py` & `shillelagh-1.2.4/examples/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/examples/generic_json.py` & `shillelagh-1.2.4/examples/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/examples/weatherapi.py` & `shillelagh-1.2.4/examples/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/requirements/base.txt` & `shillelagh-1.2.4/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/requirements/test.txt` & `shillelagh-1.2.4/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/setup.cfg` & `shillelagh-1.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -93,32 +93,32 @@
 	pyfakefs>=4.3.3
 	pygments>=2.8
 	pylint>=2.16.2
 	pytest-cov>=2.11.1
 	pytest-integration==0.2.2
 	pytest-mock>=3.5.1
 	pytest>=6.2.2
-	requests-cache==0.7.1
+	requests-cache>=0.7.1
 	requests-mock>=1.8.0
 	requests>=2.25.1
 	tabulate==0.8.9
 docs = 
 	sphinx>=4.0.1
 console = 
 	PyYAML>=5.4
 	appdirs>=1.4.4
 	prompt_toolkit>=3
 	pygments>=2.8
 	tabulate==0.8.9
 datasetteapi = 
-	requests-cache==0.7.1
+	requests-cache>=0.7.1
 genericjsonapi = 
 	jsonpath-python>=1.0.5
 	prison>=0.2.1
-	requests-cache==0.7.1
+	requests-cache>=0.7.1
 	yarl>=1.8.1
 githubapi = 
 	jsonpath-python>=1.0.5
 gsheetsapi = 
 	google-auth>=1.23.0
 	requests>=2.23.0
 htmltableapi = 
@@ -126,19 +126,19 @@
 	html5lib>=1.1
 	pandas>=1.2.2
 pandasmemory = 
 	pandas>=1.2.2
 s3selectapi = 
 	boto3>=1.24.28
 socrataapi = 
-	requests-cache==0.7.1
+	requests-cache>=0.7.1
 systemapi = 
 	psutil>=5.8.0
 weatherapi = 
-	requests-cache==0.7.1
+	requests-cache>=0.7.1
 
 [options.entry_points]
 shillelagh.adapter = 
 	csvfile = shillelagh.adapters.file.csvfile:CSVFile
 	datasetteapi = shillelagh.adapters.api.datasette:DatasetteAPI
 	genericjsonapi = shillelagh.adapters.api.generic_json:GenericJSONAPI
 	githubapi = shillelagh.adapters.api.github:GitHubAPI
```

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/datasette.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/generic_json.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/github.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/github.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/adapter.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/adapter.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/fields.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/lib.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/base.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/date.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/date.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/number.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/number.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/types.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/typing.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/html_table.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/html_table.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/s3select.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/s3select.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/socrata.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/socrata.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/system.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/system.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/api/weatherapi.py` & `shillelagh-1.2.4/src/shillelagh/adapters/api/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/base.py` & `shillelagh-1.2.4/src/shillelagh/adapters/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/file/csvfile.py` & `shillelagh-1.2.4/src/shillelagh/adapters/file/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/memory/pandas.py` & `shillelagh-1.2.4/src/shillelagh/adapters/memory/pandas.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/adapters/registry.py` & `shillelagh-1.2.4/src/shillelagh/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/backends/apsw/db.py` & `shillelagh-1.2.4/src/shillelagh/backends/apsw/db.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/base.py` & `shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/gsheets.py` & `shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/gsheets.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/safe.py` & `shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/safe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/backends/apsw/vt.py` & `shillelagh-1.2.4/src/shillelagh/backends/apsw/vt.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/console.py` & `shillelagh-1.2.4/src/shillelagh/console.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/exceptions.py` & `shillelagh-1.2.4/src/shillelagh/exceptions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/fields.py` & `shillelagh-1.2.4/src/shillelagh/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/filters.py` & `shillelagh-1.2.4/src/shillelagh/filters.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/functions.py` & `shillelagh-1.2.4/src/shillelagh/functions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/lib.py` & `shillelagh-1.2.4/src/shillelagh/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/types.py` & `shillelagh-1.2.4/src/shillelagh/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh/typing.py` & `shillelagh-1.2.4/src/shillelagh/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh.egg-info/PKG-INFO` & `shillelagh-1.2.4/src/shillelagh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.3
+Version: 1.2.4
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.3/src/shillelagh.egg-info/SOURCES.txt` & `shillelagh-1.2.4/src/shillelagh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh.egg-info/entry_points.txt` & `shillelagh-1.2.4/src/shillelagh.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/src/shillelagh.egg-info/requires.txt` & `shillelagh-1.2.4/src/shillelagh.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,36 +27,36 @@
 pyfakefs>=4.3.3
 pygments>=2.8
 pylint>=2.16.2
 pytest-cov>=2.11.1
 pytest-integration==0.2.2
 pytest-mock>=3.5.1
 pytest>=6.2.2
-requests-cache==0.7.1
+requests-cache>=0.7.1
 requests-mock>=1.8.0
 requests>=2.25.1
 tabulate==0.8.9
 
 [console]
 PyYAML>=5.4
 appdirs>=1.4.4
 prompt_toolkit>=3
 pygments>=2.8
 tabulate==0.8.9
 
 [datasetteapi]
-requests-cache==0.7.1
+requests-cache>=0.7.1
 
 [docs]
 sphinx>=4.0.1
 
 [genericjsonapi]
 jsonpath-python>=1.0.5
 prison>=0.2.1
-requests-cache==0.7.1
+requests-cache>=0.7.1
 yarl>=1.8.1
 
 [githubapi]
 jsonpath-python>=1.0.5
 
 [gsheetsapi]
 google-auth>=1.23.0
@@ -70,15 +70,15 @@
 [pandasmemory]
 pandas>=1.2.2
 
 [s3selectapi]
 boto3>=1.24.28
 
 [socrataapi]
-requests-cache==0.7.1
+requests-cache>=0.7.1
 
 [systemapi]
 psutil>=5.8.0
 
 [testing]
 PyYAML>=5.4
 appdirs>=1.4.4
@@ -106,8 +106,8 @@
 requests-cache>=0.7.1
 requests-mock>=1.8.0
 requests>=2.25.1
 tabulate==0.8.9
 yarl>=1.8.1
 
 [weatherapi]
-requests-cache==0.7.1
+requests-cache>=0.7.1
```

### Comparing `shillelagh-1.2.3/talks/Python Brasil 2021.pdf` & `shillelagh-1.2.4/talks/Python Brasil 2021.pdf`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py` & `shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py` & `shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/datasette_test.py` & `shillelagh-1.2.4/tests/adapters/api/datasette_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/generic_json_test.py` & `shillelagh-1.2.4/tests/adapters/api/generic_json_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/github_test.py` & `shillelagh-1.2.4/tests/adapters/api/github_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/gsheets/adapter_test.py` & `shillelagh-1.2.4/tests/adapters/api/gsheets/adapter_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/gsheets/fields_test.py` & `shillelagh-1.2.4/tests/adapters/api/gsheets/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/gsheets/integration_test.py` & `shillelagh-1.2.4/tests/adapters/api/gsheets/integration_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/gsheets/lib_test.py` & `shillelagh-1.2.4/tests/adapters/api/gsheets/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/base_test.py` & `shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/date_test.py` & `shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/date_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/number_test.py` & `shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/number_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/html_table_test.py` & `shillelagh-1.2.4/tests/adapters/api/html_table_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/s3select_test.py` & `shillelagh-1.2.4/tests/adapters/api/s3select_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/socrata_test.py` & `shillelagh-1.2.4/tests/adapters/api/socrata_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/system_test.py` & `shillelagh-1.2.4/tests/adapters/api/system_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/api/weatherapi_test.py` & `shillelagh-1.2.4/tests/adapters/api/weatherapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/base_test.py` & `shillelagh-1.2.4/tests/adapters/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/file/csvfile_test.py` & `shillelagh-1.2.4/tests/adapters/file/csvfile_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/memory/pandas_test.py` & `shillelagh-1.2.4/tests/adapters/memory/pandas_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/adapters/registry_test.py` & `shillelagh-1.2.4/tests/adapters/registry_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/backends/apsw/db_test.py` & `shillelagh-1.2.4/tests/backends/apsw/db_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/backends/apsw/dbapi_test.py` & `shillelagh-1.2.4/tests/backends/apsw/dbapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/backends/apsw/dialects/base_test.py` & `shillelagh-1.2.4/tests/backends/apsw/dialects/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/backends/apsw/dialects/gsheets_test.py` & `shillelagh-1.2.4/tests/backends/apsw/dialects/gsheets_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/backends/apsw/dialects/safe_test.py` & `shillelagh-1.2.4/tests/backends/apsw/dialects/safe_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/backends/apsw/vt_test.py` & `shillelagh-1.2.4/tests/backends/apsw/vt_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/conftest.py` & `shillelagh-1.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/console_test.py` & `shillelagh-1.2.4/tests/console_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/__init__.py` & `shillelagh-1.2.4/tests/fakes/__init__.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/cdc_data_response.json` & `shillelagh-1.2.4/tests/fakes/cdc_data_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/cdc_metadata_response.json` & `shillelagh-1.2.4/tests/fakes/cdc_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/datasette_columns_response.json` & `shillelagh-1.2.4/tests/fakes/datasette_columns_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/datasette_data_response_1.json` & `shillelagh-1.2.4/tests/fakes/datasette_data_response_1.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/datasette_data_response_2.json` & `shillelagh-1.2.4/tests/fakes/datasette_data_response_2.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/datasette_metadata_response.json` & `shillelagh-1.2.4/tests/fakes/datasette_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/datasette_results.json` & `shillelagh-1.2.4/tests/fakes/datasette_results.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/github_response.json` & `shillelagh-1.2.4/tests/fakes/github_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/github_single_response.json` & `shillelagh-1.2.4/tests/fakes/github_single_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/incidents.json` & `shillelagh-1.2.4/tests/fakes/incidents.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fakes/weatherapi_response.json` & `shillelagh-1.2.4/tests/fakes/weatherapi_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/fields_test.py` & `shillelagh-1.2.4/tests/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/filters_test.py` & `shillelagh-1.2.4/tests/filters_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/functions_test.py` & `shillelagh-1.2.4/tests/functions_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/lib_test.py` & `shillelagh-1.2.4/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.3/tests/types_test.py` & `shillelagh-1.2.4/tests/types_test.py`

 * *Files identical despite different names*

