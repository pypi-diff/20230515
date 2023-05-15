# Comparing `tmp/shillelagh-1.2.2.tar.gz` & `tmp/shillelagh-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-1.2.2.tar", last modified: Tue Apr 18 01:52:16 2023, max compression
+gzip compressed data, was "shillelagh-1.2.3.tar", last modified: Mon May 15 19:25:08 2023, max compression
```

## Comparing `shillelagh-1.2.2.tar` & `shillelagh-1.2.3.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.540024 shillelagh-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.524024 shillelagh-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.524024 shillelagh-1.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.524024 shillelagh-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/python-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-04-18 01:51:58.000000 shillelagh-1.2.2/ARCHITECTURE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-18 01:51:58.000000 shillelagh-1.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-18 01:51:58.000000 shillelagh-1.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-18 01:51:58.000000 shillelagh-1.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-18 01:51:58.000000 shillelagh-1.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-18 01:51:58.000000 shillelagh-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-18 01:51:58.000000 shillelagh-1.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-04-18 01:52:16.540024 shillelagh-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-18 01:51:58.000000 shillelagh-1.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 01:51:58.000000 shillelagh-1.2.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 01:51:58.000000 shillelagh-1.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 01:51:58.000000 shillelagh-1.2.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-18 01:51:58.000000 shillelagh-1.2.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 01:51:58.000000 shillelagh-1.2.2/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-18 01:51:58.000000 shillelagh-1.2.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-18 01:52:16.540024 shillelagh-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 01:51:58.000000 shillelagh-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.512024 shillelagh-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/src/shillelagh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/src/shillelagh/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/src/shillelagh/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/html_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/s3select.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/file/csvfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/memory/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/vt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/src/shillelagh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/talks/
--rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-04-18 01:51:58.000000 shillelagh-1.2.2/talks/Python Brasil 2021.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.516024 shillelagh-1.2.2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/templates/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-18 01:51:58.000000 shillelagh-1.2.2/templates/adapter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/templates/adapter/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-04-18 01:51:58.000000 shillelagh-1.2.2/templates/adapter/hooks/post_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-18 01:51:58.000000 shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-18 01:51:58.000000 shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/datasette_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/generic_json_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/github_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/html_table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/s3select_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/socrata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/system_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/weatherapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/file/csvfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/memory/pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/registry_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dbapi_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dialects/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dialects/gsheets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dialects/safe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.540024 shillelagh-1.2.2/tests/fakes/
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/cdc_data_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/cdc_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_columns_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_data_response_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_data_response_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/github_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/github_single_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/incidents.json
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/weatherapi_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/types_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.029486 shillelagh-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.009486 shillelagh-1.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.009486 shillelagh-1.2.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/python-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 19:24:53.000000 shillelagh-1.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-15 19:24:53.000000 shillelagh-1.2.3/ARCHITECTURE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 19:24:53.000000 shillelagh-1.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-15 19:24:53.000000 shillelagh-1.2.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-15 19:24:53.000000 shillelagh-1.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 19:24:53.000000 shillelagh-1.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 19:24:53.000000 shillelagh-1.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-15 19:24:53.000000 shillelagh-1.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-15 19:25:08.029486 shillelagh-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-15 19:24:53.000000 shillelagh-1.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-15 19:24:53.000000 shillelagh-1.2.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-15 19:24:53.000000 shillelagh-1.2.3/examples/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 19:24:53.000000 shillelagh-1.2.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 19:24:53.000000 shillelagh-1.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 19:24:53.000000 shillelagh-1.2.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 19:24:53.000000 shillelagh-1.2.3/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 19:24:53.000000 shillelagh-1.2.3/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-15 19:24:53.000000 shillelagh-1.2.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-15 19:25:08.029486 shillelagh-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-15 19:24:53.000000 shillelagh-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.009486 shillelagh-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/src/shillelagh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/src/shillelagh/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/html_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/s3select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/api/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/file/csvfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/memory/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/adapters/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/backends/apsw/vt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 19:24:53.000000 shillelagh-1.2.3/src/shillelagh/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.013486 shillelagh-1.2.3/src/shillelagh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 19:25:07.000000 shillelagh-1.2.3/src/shillelagh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.017486 shillelagh-1.2.3/talks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-05-15 19:24:53.000000 shillelagh-1.2.3/talks/Python Brasil 2021.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.009486 shillelagh-1.2.3/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/templates/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-15 19:24:53.000000 shillelagh-1.2.3/templates/adapter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/templates/adapter/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-05-15 19:24:53.000000 shillelagh-1.2.3/templates/adapter/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 19:24:53.000000 shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-15 19:24:53.000000 shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/tests/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/datasette_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/generic_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/github_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.021486 shillelagh-1.2.3/tests/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/html_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/s3select_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/socrata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/api/weatherapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/file/csvfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/memory/pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/adapters/registry_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dbapi_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.025486 shillelagh-1.2.3/tests/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dialects/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dialects/gsheets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/dialects/safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/backends/apsw/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:25:08.029486 shillelagh-1.2.3/tests/fakes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/cdc_data_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/cdc_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_columns_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_data_response_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_data_response_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/datasette_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/github_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/github_single_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fakes/weatherapi_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-15 19:24:53.000000 shillelagh-1.2.3/tests/types_test.py
```

### Comparing `shillelagh-1.2.2/.coveragerc` & `shillelagh-1.2.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `shillelagh-1.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `shillelagh-1.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.github/pull_request_template.md` & `shillelagh-1.2.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.github/workflows/codeql-analysis.yml` & `shillelagh-1.2.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.github/workflows/python-integration.yml` & `shillelagh-1.2.3/.github/workflows/python-integration.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.github/workflows/python-package-daily.yml` & `shillelagh-1.2.3/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.github/workflows/python-package.yml` & `shillelagh-1.2.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.github/workflows/python-publish.yml` & `shillelagh-1.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.gitignore` & `shillelagh-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.pre-commit-config.yaml` & `shillelagh-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/.readthedocs.yml` & `shillelagh-1.2.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/ARCHITECTURE.rst` & `shillelagh-1.2.3/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/CHANGELOG.rst` & `shillelagh-1.2.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 1.2.3 - 2023-05-15
+==========================
+
+- Add ``yarl`` dependency to the generic JSON adapter (#355)
+- Only warn of errors when loading adapters if they are explicitly requested (#360)
+- Relax dependency for ``requests-cache`` (#361)
+
 Version 1.2.2 - 2023-04-17
 ==========================
 
 - Allow passing request headers to the generic JSON adapter via query arguments (#354)
 
 Version 1.2.1 - 2023-04-14
 ==========================
```

### Comparing `shillelagh-1.2.2/CODE_OF_CONDUCT.md` & `shillelagh-1.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/CONTRIBUTING.rst` & `shillelagh-1.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/LICENSE.txt` & `shillelagh-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/Makefile` & `shillelagh-1.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/PKG-INFO` & `shillelagh-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.2
+Version: 1.2.3
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.2/README.rst` & `shillelagh-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/docs/Makefile` & `shillelagh-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/docs/adapters.rst` & `shillelagh-1.2.3/docs/adapters.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/docs/conf.py` & `shillelagh-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/docs/development.rst` & `shillelagh-1.2.3/docs/development.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/docs/install.rst` & `shillelagh-1.2.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/docs/usage.rst` & `shillelagh-1.2.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/examples/csvfile.py` & `shillelagh-1.2.3/examples/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/examples/dataframe.py` & `shillelagh-1.2.3/examples/dataframe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/examples/datasette.py` & `shillelagh-1.2.3/examples/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/examples/generic_json.py` & `shillelagh-1.2.3/examples/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/examples/weatherapi.py` & `shillelagh-1.2.3/examples/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/requirements/base.txt` & `shillelagh-1.2.3/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/requirements/test.txt` & `shillelagh-1.2.3/requirements/test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,31 @@
     # via shillelagh
 apsw==3.38.5.post1
     # via shillelagh
 astroid==2.14.2
     # via pylint
 attrs==21.4.0
     # via
+    #   cattrs
     #   pytest
     #   requests-cache
 beautifulsoup4==4.11.1
     # via shillelagh
 boto3==1.24.35
     # via shillelagh
 botocore==1.27.35
     # via
     #   boto3
     #   s3transfer
 build==0.8.0
     # via pip-tools
 cachetools==5.2.0
     # via google-auth
+cattrs==22.2.0
+    # via requests-cache
 certifi==2022.6.15
     # via requests
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==2.1.0
     # via requests
 click==8.1.3
@@ -44,15 +47,17 @@
 dill==0.3.6
     # via
     #   pylint
     #   shillelagh
 distlib==0.3.5
     # via virtualenv
 exceptiongroup==1.0.4
-    # via pytest
+    # via
+    #   cattrs
+    #   pytest
 filelock==3.7.1
     # via virtualenv
 freezegun==1.2.1
     # via shillelagh
 google-auth==2.9.1
     # via shillelagh
 greenlet==2.0.2
@@ -67,16 +72,14 @@
     # via
     #   requests
     #   yarl
 iniconfig==1.1.1
     # via pytest
 isort==5.10.1
     # via pylint
-itsdangerous==2.1.2
-    # via requests-cache
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 jsonpath-python==1.0.6
     # via shillelagh
 lazy-object-proxy==1.7.1
@@ -99,14 +102,15 @@
 pep517==0.12.0
     # via build
 pip-tools==6.8.0
     # via shillelagh
 platformdirs==2.5.2
     # via
     #   pylint
+    #   requests-cache
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==2.20.0
     # via shillelagh
 prison==0.2.1
     # via shillelagh
@@ -146,22 +150,21 @@
     #   pandas
     #   shillelagh
 pytz==2022.1
     # via pandas
 pyyaml==6.0
     # via
     #   pre-commit
-    #   requests-cache
     #   shillelagh
 requests==2.28.1
     # via
     #   requests-cache
     #   requests-mock
     #   shillelagh
-requests-cache==0.7.1
+requests-cache==1.0.1
     # via shillelagh
 requests-mock==1.9.3
     # via shillelagh
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
@@ -197,14 +200,15 @@
     #   shillelagh
 url-normalize==1.4.3
     # via requests-cache
 urllib3==1.26.10
     # via
     #   botocore
     #   requests
+    #   requests-cache
 virtualenv==20.15.1
     # via pre-commit
 wcwidth==0.2.5
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
 wheel==0.37.1
```

### Comparing `shillelagh-1.2.2/setup.cfg` & `shillelagh-1.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 	pyfakefs>=4.3.3
 	pygments>=2.8
 	pylint>=2.16.2
 	pytest-cov>=2.11.1
 	pytest-integration==0.2.2
 	pytest-mock>=3.5.1
 	pytest>=7.2.0
-	requests-cache==0.7.1
+	requests-cache>=0.7.1
 	requests-mock>=1.8.0
 	requests>=2.25.1
 	tabulate==0.8.9
 	yarl>=1.8.1
 all = 
 	PyYAML>=5.4
 	appdirs>=1.4.4
@@ -111,14 +111,15 @@
 	tabulate==0.8.9
 datasetteapi = 
 	requests-cache==0.7.1
 genericjsonapi = 
 	jsonpath-python>=1.0.5
 	prison>=0.2.1
 	requests-cache==0.7.1
+	yarl>=1.8.1
 githubapi = 
 	jsonpath-python>=1.0.5
 gsheetsapi = 
 	google-auth>=1.23.0
 	requests>=2.23.0
 htmltableapi = 
 	beautifulsoup4>=4.11.1
```

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/datasette.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/generic_json.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/github.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/github.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/adapter.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/adapter.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/fields.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/lib.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/base.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/date.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/date.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/number.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/parsing/number.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/types.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/typing.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/gsheets/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/html_table.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/html_table.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/s3select.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/s3select.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/socrata.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/socrata.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/system.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/system.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/api/weatherapi.py` & `shillelagh-1.2.3/src/shillelagh/adapters/api/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/base.py` & `shillelagh-1.2.3/src/shillelagh/adapters/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/file/csvfile.py` & `shillelagh-1.2.3/src/shillelagh/adapters/file/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/memory/pandas.py` & `shillelagh-1.2.3/src/shillelagh/adapters/memory/pandas.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/adapters/registry.py` & `shillelagh-1.2.3/src/shillelagh/adapters/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,27 @@
     """
 
     def __init__(self):
         self.loaders = defaultdict(list)
         for entry_point in iter_entry_points("shillelagh.adapter"):
             self.loaders[entry_point.name].append(entry_point.load)
 
-    def load(self, name: str, safe: bool = False) -> Type[Adapter]:
+    def load(self, name: str, safe: bool = False, warn: bool = False) -> Type[Adapter]:
         """
         Load a given entry point by its name.
         """
         if safe and len(self.loaders[name]) > 1:
             raise UnsafeAdaptersError(f"Multiple adapters found with name {name}")
 
         for load in self.loaders[name]:
             try:
                 return cast(Type[Adapter], load())
             except (ImportError, ModuleNotFoundError) as ex:
-                _logger.warning("Couldn't load adapter %s", name)
+                if warn:
+                    _logger.warning("Couldn't load adapter %s", name)
                 _logger.debug(ex)
                 continue
 
         raise InterfaceError(f"Unable to load adapter {name}")
 
     def load_all(
         self,
@@ -72,15 +73,15 @@
 
         If no adapters are specified, return none.
         """
         if not adapters:
             return {}
 
         loaded_adapters = {
-            name: self.load(name, safe=True)
+            name: self.load(name, safe=True, warn=True)
             for name in self.loaders
             if name in adapters
         }
 
         return {
             name: adapter for name, adapter in loaded_adapters.items() if adapter.safe
         }
```

### Comparing `shillelagh-1.2.2/src/shillelagh/backends/apsw/db.py` & `shillelagh-1.2.3/src/shillelagh/backends/apsw/db.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/base.py` & `shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/gsheets.py` & `shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/gsheets.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/safe.py` & `shillelagh-1.2.3/src/shillelagh/backends/apsw/dialects/safe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/backends/apsw/vt.py` & `shillelagh-1.2.3/src/shillelagh/backends/apsw/vt.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/console.py` & `shillelagh-1.2.3/src/shillelagh/console.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/exceptions.py` & `shillelagh-1.2.3/src/shillelagh/exceptions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/fields.py` & `shillelagh-1.2.3/src/shillelagh/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/filters.py` & `shillelagh-1.2.3/src/shillelagh/filters.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/functions.py` & `shillelagh-1.2.3/src/shillelagh/functions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/lib.py` & `shillelagh-1.2.3/src/shillelagh/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/types.py` & `shillelagh-1.2.3/src/shillelagh/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh/typing.py` & `shillelagh-1.2.3/src/shillelagh/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh.egg-info/PKG-INFO` & `shillelagh-1.2.3/src/shillelagh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.2
+Version: 1.2.3
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.2/src/shillelagh.egg-info/SOURCES.txt` & `shillelagh-1.2.3/src/shillelagh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh.egg-info/entry_points.txt` & `shillelagh-1.2.3/src/shillelagh.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/src/shillelagh.egg-info/requires.txt` & `shillelagh-1.2.3/src/shillelagh.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 [docs]
 sphinx>=4.0.1
 
 [genericjsonapi]
 jsonpath-python>=1.0.5
 prison>=0.2.1
 requests-cache==0.7.1
+yarl>=1.8.1
 
 [githubapi]
 jsonpath-python>=1.0.5
 
 [gsheetsapi]
 google-auth>=1.23.0
 requests>=2.23.0
@@ -98,15 +99,15 @@
 pyfakefs>=4.3.3
 pygments>=2.8
 pylint>=2.16.2
 pytest-cov>=2.11.1
 pytest-integration==0.2.2
 pytest-mock>=3.5.1
 pytest>=7.2.0
-requests-cache==0.7.1
+requests-cache>=0.7.1
 requests-mock>=1.8.0
 requests>=2.25.1
 tabulate==0.8.9
 yarl>=1.8.1
 
 [weatherapi]
 requests-cache==0.7.1
```

### Comparing `shillelagh-1.2.2/talks/Python Brasil 2021.pdf` & `shillelagh-1.2.3/talks/Python Brasil 2021.pdf`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py` & `shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py` & `shillelagh-1.2.3/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/datasette_test.py` & `shillelagh-1.2.3/tests/adapters/api/datasette_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/generic_json_test.py` & `shillelagh-1.2.3/tests/adapters/api/generic_json_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Test the generic JSON adapter.
 """
 
 import pytest
 from pytest_mock import MockerFixture
+from requests_cache import DO_NOT_CACHE
 from requests_mock.mocker import Mocker
 from yarl import URL
 
 from shillelagh.adapters.api.generic_json import GenericJSONAPI
 from shillelagh.backends.apsw.db import connect
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.typing import Maybe
@@ -15,15 +16,15 @@
 baseurl = URL("https://api.stlouisfed.org/fred/series")
 
 
 def test_generic_json(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test a simple query.
     """
-    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", 0)
+    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", DO_NOT_CACHE)
 
     # for datassette and other probing adapters
     requests_mock.head(
         "https://api.stlouisfed.org/-/versions.json?"
         "series_id=GNPCA&"
         "api_key=abcdefghijklmnopqrstuvwxyz123456&"
         "file_type=json#$.seriess%5B*%5D",
@@ -114,15 +115,15 @@
 def test_generic_json_complex_type(
     mocker: MockerFixture,
     requests_mock: Mocker,
 ) -> None:
     """
     Test a query where columns are complex.
     """
-    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", 0)
+    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", DO_NOT_CACHE)
 
     # for datassette and other probing adapters
     requests_mock.head("https://exmaple.org/-/versions.json", status_code=404)
 
     url = URL("https://example.org/")
     requests_mock.head(str(url), headers={"content-type": "application/json"})
     requests_mock.get(
@@ -162,15 +163,15 @@
     assert GenericJSONAPI.supports("https://example.org/data.json", fast=False) is True
 
 
 def test_request_headers(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test passing requests headers.
     """
-    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", 0)
+    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", DO_NOT_CACHE)
     supports = requests_mock.head(
         "https://example.org/data.json",
         headers={"content-type": "application/json"},
     )
 
     # for datassette and other probing adapters
     requests_mock.head("https://exmaple.org/-/versions.json", status_code=404)
@@ -207,15 +208,15 @@
     assert data.last_request.headers["foo"] == "bar"
 
 
 def test_request_headers_in_url(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test passing requests headers.
     """
-    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", 0)
+    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", DO_NOT_CACHE)
     supports = requests_mock.head(
         "https://example.org/data.json",
         headers={"content-type": "application/json"},
     )
 
     # for datassette and other probing adapters
     requests_mock.head("https://exmaple.org/-/versions.json", status_code=404)
```

### Comparing `shillelagh-1.2.2/tests/adapters/api/github_test.py` & `shillelagh-1.2.3/tests/adapters/api/github_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/gsheets/adapter_test.py` & `shillelagh-1.2.3/tests/adapters/api/gsheets/adapter_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/gsheets/fields_test.py` & `shillelagh-1.2.3/tests/adapters/api/gsheets/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/gsheets/integration_test.py` & `shillelagh-1.2.3/tests/adapters/api/gsheets/integration_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/gsheets/lib_test.py` & `shillelagh-1.2.3/tests/adapters/api/gsheets/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/base_test.py` & `shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/date_test.py` & `shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/date_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/number_test.py` & `shillelagh-1.2.3/tests/adapters/api/gsheets/parsing/number_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/html_table_test.py` & `shillelagh-1.2.3/tests/adapters/api/html_table_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/s3select_test.py` & `shillelagh-1.2.3/tests/adapters/api/s3select_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/socrata_test.py` & `shillelagh-1.2.3/tests/adapters/api/socrata_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/system_test.py` & `shillelagh-1.2.3/tests/adapters/api/system_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/api/weatherapi_test.py` & `shillelagh-1.2.3/tests/adapters/api/weatherapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/base_test.py` & `shillelagh-1.2.3/tests/adapters/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/file/csvfile_test.py` & `shillelagh-1.2.3/tests/adapters/file/csvfile_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/memory/pandas_test.py` & `shillelagh-1.2.3/tests/adapters/memory/pandas_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/adapters/registry_test.py` & `shillelagh-1.2.3/tests/adapters/registry_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tests for the adapter registry.
 """
 
 import pytest
+from pytest_mock import MockerFixture
 
 from shillelagh.adapters.file.csvfile import CSVFile
 from shillelagh.adapters.registry import AdapterLoader
 from shillelagh.exceptions import InterfaceError
 
 from ..fakes import FakeAdapter
 
@@ -72,7 +73,27 @@
     registry.loaders["invalid"].append(load_error)
 
     assert registry.load_all(["valid"]) == {"valid": FakeAdapter}
     with pytest.raises(InterfaceError) as excinfo:
         registry.load_all(["valid", "invalid"])
     assert str(excinfo.value) == "Unable to load adapter invalid"
     assert registry.load_all() == {"valid": FakeAdapter}
+
+
+def test_load_warning(mocker: MockerFixture, registry: AdapterLoader) -> None:
+    """
+    Test that warnings are only logged in safe mode.
+    """
+    _logger = mocker.patch("shillelagh.adapters.registry._logger")
+
+    def load_error() -> None:
+        raise ImportError("Error!")
+
+    registry.loaders["dummy"].append(load_error)
+
+    with pytest.raises(InterfaceError):
+        registry.load("dummy")
+    assert _logger.warning.not_called()
+
+    with pytest.raises(InterfaceError):
+        registry.load("dummy", warn=True)
+    assert _logger.warning.called_with("Couldn't load adapter %s", "dummy")
```

### Comparing `shillelagh-1.2.2/tests/backends/apsw/db_test.py` & `shillelagh-1.2.3/tests/backends/apsw/db_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/backends/apsw/dbapi_test.py` & `shillelagh-1.2.3/tests/backends/apsw/dbapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/backends/apsw/dialects/base_test.py` & `shillelagh-1.2.3/tests/backends/apsw/dialects/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/backends/apsw/dialects/gsheets_test.py` & `shillelagh-1.2.3/tests/backends/apsw/dialects/gsheets_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/backends/apsw/dialects/safe_test.py` & `shillelagh-1.2.3/tests/backends/apsw/dialects/safe_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/backends/apsw/vt_test.py` & `shillelagh-1.2.3/tests/backends/apsw/vt_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/conftest.py` & `shillelagh-1.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/console_test.py` & `shillelagh-1.2.3/tests/console_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/__init__.py` & `shillelagh-1.2.3/tests/fakes/__init__.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/cdc_data_response.json` & `shillelagh-1.2.3/tests/fakes/cdc_data_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/cdc_metadata_response.json` & `shillelagh-1.2.3/tests/fakes/cdc_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/datasette_columns_response.json` & `shillelagh-1.2.3/tests/fakes/datasette_columns_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/datasette_data_response_1.json` & `shillelagh-1.2.3/tests/fakes/datasette_data_response_1.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/datasette_data_response_2.json` & `shillelagh-1.2.3/tests/fakes/datasette_data_response_2.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/datasette_metadata_response.json` & `shillelagh-1.2.3/tests/fakes/datasette_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/datasette_results.json` & `shillelagh-1.2.3/tests/fakes/datasette_results.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/github_response.json` & `shillelagh-1.2.3/tests/fakes/github_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/github_single_response.json` & `shillelagh-1.2.3/tests/fakes/github_single_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/incidents.json` & `shillelagh-1.2.3/tests/fakes/incidents.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fakes/weatherapi_response.json` & `shillelagh-1.2.3/tests/fakes/weatherapi_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/fields_test.py` & `shillelagh-1.2.3/tests/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/filters_test.py` & `shillelagh-1.2.3/tests/filters_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/functions_test.py` & `shillelagh-1.2.3/tests/functions_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/lib_test.py` & `shillelagh-1.2.3/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.2/tests/types_test.py` & `shillelagh-1.2.3/tests/types_test.py`

 * *Files identical despite different names*

