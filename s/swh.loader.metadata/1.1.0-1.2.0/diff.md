# Comparing `tmp/swh.loader.metadata-1.1.0.tar.gz` & `tmp/swh.loader.metadata-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.metadata-1.1.0.tar", last modified: Fri Mar 17 12:04:03 2023, max compression
+gzip compressed data, was "dist/swh.loader.metadata-1.2.0.tar", last modified: Mon May 15 11:38:54 2023, max compression
```

## Comparing `swh.loader.metadata-1.1.0.tar` & `swh.loader.metadata-1.2.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      943 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1148 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      190 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      373 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      190 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      371 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      136 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      100 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      226 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2632 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/
--rw-r--r--   0 jenkins    (115) docker     (999)      540 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7105 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3287 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4501 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/gitea.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3280 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/github.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4282 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_api.github.com/
--rw-r--r--   0 jenkins    (115) docker     (999)    16850 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_api.github.com/repos_jmarlena_linguist
--rw-r--r--   0 jenkins    (115) docker     (999)     5393 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_Hello-World
--rw-r--r--   0 jenkins    (115) docker     (999)    16869 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_linguist
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_codeberg.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     1845 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos_ForgeFed_ForgeFed
--rw-r--r--   0 jenkins    (115) docker     (999)     3632 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos__ZN3val_ForgeFed
--rw-r--r--   0 jenkins    (115) docker     (999)     2873 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3563 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3875 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_gitea.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4058 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_github.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8371 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_journal_client.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1148 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1547 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      200 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      189 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-17 12:04:03.000000 swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1551 2023-03-17 12:04:01.000000 swh.loader.metadata-1.1.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      943 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1148 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      190 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      373 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      190 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      371 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      136 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      100 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      226 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2632 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/
+-rw-r--r--   0 jenkins    (115) docker     (999)      540 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7105 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3287 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4501 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/gitea.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3280 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/github.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5704 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_api.github.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)    16850 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_api.github.com/repos_jmarlena_linguist
+-rw-r--r--   0 jenkins    (115) docker     (999)     5393 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_Hello-World
+-rw-r--r--   0 jenkins    (115) docker     (999)    16869 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_linguist
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_codeberg.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1845 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos_ForgeFed_ForgeFed
+-rw-r--r--   0 jenkins    (115) docker     (999)     3632 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos__ZN3val_ForgeFed
+-rw-r--r--   0 jenkins    (115) docker     (999)     2873 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3567 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3875 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_gitea.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4058 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_github.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8371 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_journal_client.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1148 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1547 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      200 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      189 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-15 11:38:54.000000 swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1551 2023-05-15 11:38:52.000000 swh.loader.metadata-1.2.0/tox.ini
```

### Comparing `swh.loader.metadata-1.1.0/.pre-commit-config.yaml` & `swh.loader.metadata-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/CODE_OF_CONDUCT.md` & `swh.loader.metadata-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/LICENSE` & `swh.loader.metadata-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/PKG-INFO` & `swh.loader.metadata-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.metadata
-Version: 1.1.0
+Version: 1.2.0
 Summary: Software Heritage Extrinsic Metadata Fetchers
 Home-page: https://forge.softwareheritage.org/diffusion/swh-loader-metadata
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-metadata
```

### Comparing `swh.loader.metadata-1.1.0/setup.py` & `swh.loader.metadata-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/__init__.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/base.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/base.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/cli.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/cli.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/gitea.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/gitea.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/github.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/github.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/journal_client.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/journal_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (C) 2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import dataclasses
 import datetime
-from typing import Dict, Iterable, List, Type, cast
+from typing import Any, Dict, Iterable, List, Type, TypeVar, cast
 import uuid
 
 from swh.core.api.classes import stream_results
+from swh.core.statsd import Statsd
 from swh.loader.core.metadata_fetchers import CredentialsType, get_fetchers_for_lister
 from swh.loader.metadata.base import BaseMetadataFetcher
 from swh.model.model import (
     MetadataAuthority,
     MetadataFetcher,
     Origin,
     RawExtrinsicMetadata,
@@ -22,29 +23,52 @@
 
 
 def _now() -> datetime.datetime:
     # Used by tests for mocking
     return datetime.datetime.now(tz=datetime.timezone.utc)
 
 
+_TItem = TypeVar("_TItem")
+
+
 @dataclasses.dataclass
 class JournalClient:
     scheduler: SchedulerInterface
     storage: StorageInterface
     metadata_fetcher_credentials: CredentialsType
     reload_after_days: int
 
     def __post_init__(self):
         self._listers = {}
         self._added_fetchers = set()
         self._added_authorities = set()
+        self.statsd = Statsd(namespace="swh_loader_metadata_journal_client")
+
+    def statsd_timed(self, name: str, tags: Dict[str, Any] = {}):
+        """
+        Wrapper for :meth:`swh.core.statsd.Statsd.timed`, which uses the standard
+        metric name and tag.
+        """
+        return self.statsd.timed(
+            "operation_duration_seconds", tags={"operation": name, **tags}
+        )
+
+    def statsd_timing(self, name: str, value: float, tags: Dict[str, Any] = {}) -> None:
+        """
+        Wrapper for :meth:`swh.core.statsd.Statsd.timing`, which uses the standard
+        metric name and tags for loaders.
+        """
+        self.statsd.timing(
+            "operation_duration_seconds", value, tags={"operation": name, **tags}
+        )
 
     def _get_lister(self, lister_id: uuid.UUID) -> Lister:
         if lister_id not in self._listers:
-            (lister,) = self.scheduler.get_listers_by_id([str(lister_id)])
+            with self.statsd_timed("get_listers_by_id"):
+                (lister,) = self.scheduler.get_listers_by_id([str(lister_id)])
             self._listers[lister.id] = lister
         return self._listers[lister_id]
 
     def _add_metadata_fetchers(self, fetchers: Iterable[MetadataFetcher]) -> None:
         for fetcher in fetchers:
             if fetcher not in self._added_fetchers:
                 self.storage.metadata_fetcher_add([fetcher])
@@ -68,53 +92,66 @@
         """
 
         assert set(messages) == {"origin"}, f"Unexpected message types: {set(messages)}"
 
         for origin in messages["origin"]:
 
             for listed_origin in stream_results(
-                self.scheduler.get_listed_origins, url=origin["url"]
+                self.statsd_timed("get_listed_origins")(
+                    self.scheduler.get_listed_origins
+                ),
+                url=origin["url"],
             ):
                 self._process_listed_origin(listed_origin)
 
         self.storage.flush()
 
     def _process_listed_origin(
         self,
         listed_origin: ListedOrigin,
     ) -> List[RawExtrinsicMetadata]:
         origin = Origin(url=listed_origin.url)
+
         lister = self._get_lister(listed_origin.lister_id)
 
         fetcher_classes = cast(
             List[Type[BaseMetadataFetcher]], get_fetchers_for_lister(lister.name)
         )
+        self.statsd.histogram("metadata_fetchers", len(fetcher_classes))
 
         now = _now()
 
         metadata: List[RawExtrinsicMetadata] = []
 
         for cls in fetcher_classes:
             metadata_fetcher = cls(
                 origin=origin,
                 lister_name=lister.name,
                 lister_instance_name=lister.instance_name,
                 credentials=self.metadata_fetcher_credentials,
             )
 
-            last_metadata = self.storage.raw_extrinsic_metadata_get(
-                target=origin.swhid(),
-                authority=metadata_fetcher.metadata_authority(),
-                after=now - datetime.timedelta(days=self.reload_after_days),
-                limit=1,
-            )
+            with self.statsd_timed("raw_extrinsic_metadata_get"):
+                last_metadata = self.storage.raw_extrinsic_metadata_get(
+                    target=origin.swhid(),
+                    authority=metadata_fetcher.metadata_authority(),
+                    after=now - datetime.timedelta(days=self.reload_after_days),
+                    limit=1,
+                )
 
             if last_metadata.results:
                 # We already have recent metadata; don't load it again.
                 continue
 
-            metadata = list(metadata_fetcher.get_origin_metadata())
-            self._add_metadata_fetchers({m.fetcher for m in metadata})
-            self._add_metadata_authorities({m.authority for m in metadata})
-            self.storage.raw_extrinsic_metadata_add(metadata)
+            with self.statsd_timed("get_origin_metadata"):
+                metadata = list(metadata_fetcher.get_origin_metadata())
+
+            with self.statsd_timed("metadata_fetcher_add"):
+                self._add_metadata_fetchers({m.fetcher for m in metadata})
+
+            with self.statsd_timed("metadata_authority_add"):
+                self._add_metadata_authorities({m.authority for m in metadata})
+
+            with self.statsd_timed("raw_extrinsic_metadata_add"):
+                self.storage.raw_extrinsic_metadata_add(metadata)
 
         return metadata
```

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_api.github.com/repos_jmarlena_linguist` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_api.github.com/repos_jmarlena_linguist`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_Hello-World` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_Hello-World`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_linguist` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_linguist`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos_ForgeFed_ForgeFed` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos_ForgeFed_ForgeFed`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos__ZN3val_ForgeFed` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos__ZN3val_ForgeFed`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_base.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_cli.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import List
 from unittest.mock import MagicMock
 
 from click.testing import CliRunner
 from confluent_kafka import Producer
 import yaml
 
-from swh.core.cli import swh as swh_cli_group
 from swh.journal.serializers import value_to_kafka
+from swh.loader.metadata.cli import swh_cli_group
 from swh.loader.metadata.journal_client import JournalClient
 
 
 def invoke(
     args: List[str],
     storage=None,
     kafka_server=None,
```

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_gitea.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_gitea.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_github.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh/loader/metadata/tests/test_journal_client.py` & `swh.loader.metadata-1.2.0/swh/loader/metadata/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/PKG-INFO` & `swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.metadata
-Version: 1.1.0
+Version: 1.2.0
 Summary: Software Heritage Extrinsic Metadata Fetchers
 Home-page: https://forge.softwareheritage.org/diffusion/swh-loader-metadata
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-metadata
```

### Comparing `swh.loader.metadata-1.1.0/swh.loader.metadata.egg-info/SOURCES.txt` & `swh.loader.metadata-1.2.0/swh.loader.metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.1.0/tox.ini` & `swh.loader.metadata-1.2.0/tox.ini`

 * *Files identical despite different names*

