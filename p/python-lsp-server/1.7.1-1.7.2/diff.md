# Comparing `tmp/python-lsp-server-1.7.1.tar.gz` & `tmp/python-lsp-server-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lsp-server-1.7.1.tar", last modified: Tue Jan 17 23:25:16 2023, max compression
+gzip compressed data, was "python-lsp-server-1.7.2.tar", last modified: Mon Apr  3 01:21:16 2023, max compression
```

## Comparing `python-lsp-server-1.7.1.tar` & `python-lsp-server-1.7.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.623891 python-lsp-server-1.7.1/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/.coveragerc
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/.gitattributes
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.599870 python-lsp-server-1.7.1/.github/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.603873 python-lsp-server-1.7.1/.github/workflows/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1228 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/.github/workflows/release.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1386 2022-12-26 21:07:40.000000 python-lsp-server-1.7.1/.github/workflows/static.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1433 2022-12-26 21:07:40.000000 python-lsp-server-1.7.1/.github/workflows/test-linux.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1434 2022-12-26 21:07:40.000000 python-lsp-server-1.7.1/.github/workflows/test-mac.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1129 2022-12-26 21:07:40.000000 python-lsp-server-1.7.1/.github/workflows/test-win.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1319 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/.gitignore
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2717 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/.policy.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      445 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/.pylintrc
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    35983 2023-01-17 23:22:26.000000 python-lsp-server-1.7.1/CHANGELOG.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8858 2022-12-29 15:51:51.000000 python-lsp-server-1.7.1/CONFIGURATION.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1147 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      128 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/MANIFEST.in
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8660 2023-01-17 23:25:16.623891 python-lsp-server-1.7.1/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8036 2022-12-18 03:24:12.000000 python-lsp-server-1.7.1/README.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      762 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/RELEASE.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.603873 python-lsp-server-1.7.1/docs/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1052 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/docs/autoimport.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.607877 python-lsp-server-1.7.1/pylsp/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      760 2022-12-26 17:45:43.000000 python-lsp-server-1.7.1/pylsp/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3874 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/__main__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     9563 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/_utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       22 2023-01-17 23:25:16.000000 python-lsp-server-1.7.1/pylsp/_version.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.611881 python-lsp-server-1.7.1/pylsp/config/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/pylsp/config/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     6355 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/config/config.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2248 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/config/flake8_conf.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1268 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/config/pycodestyle_conf.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    13742 2022-12-29 15:51:51.000000 python-lsp-server-1.7.1/pylsp/config/schema.json
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2729 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/pylsp/config/source.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2308 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/hookspecs.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1421 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/lsp.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.615884 python-lsp-server-1.7.1/pylsp/plugins/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/pylsp/plugins/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4415 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/_resolvers.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2756 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/_rope_task_handle.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3313 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/autopep8_format.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1481 2022-12-29 15:51:51.000000 python-lsp-server-1.7.1/pylsp/plugins/definition.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7478 2022-12-18 03:24:12.000000 python-lsp-server-1.7.1/pylsp/plugins/flake8_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7050 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/pylsp/plugins/folding.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      995 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/pylsp/plugins/highlight.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1643 2022-12-29 19:03:44.000000 python-lsp-server-1.7.1/pylsp/plugins/hover.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10150 2023-01-17 23:05:07.000000 python-lsp-server-1.7.1/pylsp/plugins/jedi_completion.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2188 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/jedi_rename.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1517 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/mccabe_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1395 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/pylsp/plugins/preload_imports.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3945 2022-12-26 21:07:40.000000 python-lsp-server-1.7.1/pylsp/plugins/pycodestyle_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4047 2023-01-05 00:05:39.000000 python-lsp-server-1.7.1/pylsp/plugins/pydocstyle_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2752 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/pyflakes_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    11984 2023-01-17 23:05:07.000000 python-lsp-server-1.7.1/pylsp/plugins/pylint_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1074 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/references.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8306 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/rope_autoimport.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5979 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/rope_completion.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2077 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/rope_rename.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2503 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/plugins/signature.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8168 2022-12-29 15:51:51.000000 python-lsp-server-1.7.1/pylsp/plugins/symbols.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7060 2022-12-11 23:33:58.000000 python-lsp-server-1.7.1/pylsp/plugins/yapf_format.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    23136 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/python_lsp.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2753 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/text_edit.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3725 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/pylsp/uris.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    13934 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/pylsp/workspace.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3093 2023-01-06 23:50:19.000000 python-lsp-server-1.7.1/pyproject.toml
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.615884 python-lsp-server-1.7.1/python_lsp_server.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8660 2023-01-17 23:25:16.000000 python-lsp-server-1.7.1/python_lsp_server.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2504 2023-01-17 23:25:16.000000 python-lsp-server-1.7.1/python_lsp_server.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-01-17 23:25:16.000000 python-lsp-server-1.7.1/python_lsp_server.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      900 2023-01-17 23:25:16.000000 python-lsp-server-1.7.1/python_lsp_server.egg-info/entry_points.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      732 2023-01-17 23:25:16.000000 python-lsp-server-1.7.1/python_lsp_server.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        6 2023-01-17 23:25:16.000000 python-lsp-server-1.7.1/python_lsp_server.egg-info/top_level.txt
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.615884 python-lsp-server-1.7.1/scripts/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.615884 python-lsp-server-1.7.1/scripts/circle/
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)      464 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/scripts/circle/pypi.sh
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2562 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/scripts/jsonschema2md.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      155 2023-01-17 23:25:16.623891 python-lsp-server-1.7.1/setup.cfg
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)      298 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.619888 python-lsp-server-1.7.1/test/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      275 2022-12-26 17:14:29.000000 python-lsp-server-1.7.1/test/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      292 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/test/conftest.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3338 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/fixtures.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-01-17 23:25:16.623891 python-lsp-server-1.7.1/test/plugins/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2019-06-21 09:28:02.000000 python-lsp-server-1.7.1/test/plugins/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8201 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_autoimport.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2067 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_autopep8_format.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    19813 2023-01-17 23:05:07.000000 python-lsp-server-1.7.1/test/plugins/test_completion.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3218 2022-12-29 15:51:51.000000 python-lsp-server-1.7.1/test/plugins/test_definitions.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7705 2022-12-18 03:24:12.000000 python-lsp-server-1.7.1/test/plugins/test_flake8_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4922 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/test/plugins/test_folding.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1566 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/test/plugins/test_highlight.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3072 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_hover.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2573 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/test/plugins/test_jedi_rename.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1253 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_mccabe_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4730 2022-12-26 21:07:40.000000 python-lsp-server-1.7.1/test/plugins/test_pycodestyle_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1769 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_pydocstyle_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1877 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_pyflakes_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4934 2022-12-29 15:51:51.000000 python-lsp-server-1.7.1/test/plugins/test_pylint_lint.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2498 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_references.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1388 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/test/plugins/test_rope_rename.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2656 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_signature.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3249 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_symbols.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3386 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/plugins/test_yapf_format.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3032 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/test_document.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4260 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/test_language_server.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8363 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/test_text_edit.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1517 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/test/test_uris.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2340 2022-10-31 15:56:57.000000 python-lsp-server-1.7.1/test/test_utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    12882 2022-12-11 17:32:03.000000 python-lsp-server-1.7.1/test/test_workspace.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.750254 python-lsp-server-1.7.2/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/.coveragerc
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       31 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/.gitattributes
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.726253 python-lsp-server-1.7.2/.github/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.730253 python-lsp-server-1.7.2/.github/workflows/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1228 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/.github/workflows/release.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1386 2022-12-26 21:07:40.000000 python-lsp-server-1.7.2/.github/workflows/static.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1433 2022-12-26 21:07:40.000000 python-lsp-server-1.7.2/.github/workflows/test-linux.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1434 2022-12-26 21:07:40.000000 python-lsp-server-1.7.2/.github/workflows/test-mac.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1129 2022-12-26 21:07:40.000000 python-lsp-server-1.7.2/.github/workflows/test-win.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1319 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2717 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/.policy.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      445 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/.pylintrc
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    37468 2023-04-03 01:18:18.000000 python-lsp-server-1.7.2/CHANGELOG.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8858 2022-12-29 15:51:51.000000 python-lsp-server-1.7.2/CONFIGURATION.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1147 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      128 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/MANIFEST.in
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8660 2023-04-03 01:21:16.750254 python-lsp-server-1.7.2/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8036 2022-12-18 03:24:12.000000 python-lsp-server-1.7.2/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      762 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/RELEASE.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.730253 python-lsp-server-1.7.2/docs/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1052 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/docs/autoimport.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.734253 python-lsp-server-1.7.2/pylsp/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      760 2022-12-26 17:45:43.000000 python-lsp-server-1.7.2/pylsp/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3874 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/__main__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9545 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/_utils.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       22 2023-04-03 01:21:16.000000 python-lsp-server-1.7.2/pylsp/_version.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.734253 python-lsp-server-1.7.2/pylsp/config/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/pylsp/config/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6355 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/config/config.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2248 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/config/flake8_conf.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1268 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/config/pycodestyle_conf.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    13742 2022-12-29 15:51:51.000000 python-lsp-server-1.7.2/pylsp/config/schema.json
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2729 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/pylsp/config/source.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2308 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/hookspecs.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1421 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/lsp.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.742253 python-lsp-server-1.7.2/pylsp/plugins/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/pylsp/plugins/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4415 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/plugins/_resolvers.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2756 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/plugins/_rope_task_handle.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3219 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/plugins/autopep8_format.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1345 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/plugins/definition.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7478 2022-12-18 03:24:12.000000 python-lsp-server-1.7.2/pylsp/plugins/flake8_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7050 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/pylsp/plugins/folding.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      995 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/pylsp/plugins/highlight.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1643 2022-12-29 19:03:44.000000 python-lsp-server-1.7.2/pylsp/plugins/hover.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10150 2023-03-18 18:10:05.000000 python-lsp-server-1.7.2/pylsp/plugins/jedi_completion.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1876 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/plugins/jedi_rename.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1517 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/plugins/mccabe_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1395 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/pylsp/plugins/preload_imports.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3945 2022-12-26 21:07:40.000000 python-lsp-server-1.7.2/pylsp/plugins/pycodestyle_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4291 2023-03-18 18:10:05.000000 python-lsp-server-1.7.2/pylsp/plugins/pydocstyle_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2752 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/plugins/pyflakes_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    11984 2023-03-18 18:10:05.000000 python-lsp-server-1.7.2/pylsp/plugins/pylint_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      961 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/plugins/references.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8306 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/plugins/rope_autoimport.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5979 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/plugins/rope_completion.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1899 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/plugins/rope_rename.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2503 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/plugins/signature.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8168 2022-12-29 15:51:51.000000 python-lsp-server-1.7.2/pylsp/plugins/symbols.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6943 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/plugins/yapf_format.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    23223 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/python_lsp.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2753 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/pylsp/text_edit.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3725 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/pylsp/uris.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    15297 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/pylsp/workspace.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3129 2023-03-18 18:10:05.000000 python-lsp-server-1.7.2/pyproject.toml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.742253 python-lsp-server-1.7.2/python_lsp_server.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8660 2023-04-03 01:21:16.000000 python-lsp-server-1.7.2/python_lsp_server.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2504 2023-04-03 01:21:16.000000 python-lsp-server-1.7.2/python_lsp_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-04-03 01:21:16.000000 python-lsp-server-1.7.2/python_lsp_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      900 2023-04-03 01:21:16.000000 python-lsp-server-1.7.2/python_lsp_server.egg-info/entry_points.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      758 2023-04-03 01:21:16.000000 python-lsp-server-1.7.2/python_lsp_server.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        6 2023-04-03 01:21:16.000000 python-lsp-server-1.7.2/python_lsp_server.egg-info/top_level.txt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.742253 python-lsp-server-1.7.2/scripts/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.742253 python-lsp-server-1.7.2/scripts/circle/
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      464 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/scripts/circle/pypi.sh
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2562 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/scripts/jsonschema2md.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      155 2023-04-03 01:21:16.750254 python-lsp-server-1.7.2/setup.cfg
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)      298 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.746254 python-lsp-server-1.7.2/test/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      275 2022-12-26 17:14:29.000000 python-lsp-server-1.7.2/test/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      292 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/test/conftest.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4794 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/test/fixtures.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-03 01:21:16.750254 python-lsp-server-1.7.2/test/plugins/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2019-06-21 09:28:02.000000 python-lsp-server-1.7.2/test/plugins/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8201 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/plugins/test_autoimport.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2067 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/plugins/test_autopep8_format.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    19813 2023-03-18 18:10:05.000000 python-lsp-server-1.7.2/test/plugins/test_completion.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3147 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/test/plugins/test_definitions.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7705 2022-12-18 03:24:12.000000 python-lsp-server-1.7.2/test/plugins/test_flake8_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4922 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/test/plugins/test_folding.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1566 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/test/plugins/test_highlight.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3072 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/plugins/test_hover.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2573 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/test/plugins/test_jedi_rename.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1253 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/plugins/test_mccabe_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4730 2022-12-26 21:07:40.000000 python-lsp-server-1.7.2/test/plugins/test_pycodestyle_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1769 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/plugins/test_pydocstyle_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1877 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/plugins/test_pyflakes_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4934 2022-12-29 15:51:51.000000 python-lsp-server-1.7.2/test/plugins/test_pylint_lint.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2453 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/test/plugins/test_references.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1388 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/test/plugins/test_rope_rename.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2656 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/plugins/test_signature.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3249 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/plugins/test_symbols.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3375 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/test/plugins/test_yapf_format.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3032 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/test_document.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4260 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/test_language_server.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8363 2022-12-11 17:32:03.000000 python-lsp-server-1.7.2/test/test_text_edit.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1517 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/test/test_uris.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2340 2022-10-31 15:56:57.000000 python-lsp-server-1.7.2/test/test_utils.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    14473 2023-04-03 01:06:12.000000 python-lsp-server-1.7.2/test/test_workspace.py
```

### Comparing `python-lsp-server-1.7.1/.github/workflows/release.yml` & `python-lsp-server-1.7.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/.github/workflows/static.yml` & `python-lsp-server-1.7.2/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/.github/workflows/test-linux.yml` & `python-lsp-server-1.7.2/.github/workflows/test-linux.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/.github/workflows/test-mac.yml` & `python-lsp-server-1.7.2/.github/workflows/test-mac.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/.github/workflows/test-win.yml` & `python-lsp-server-1.7.2/.github/workflows/test-win.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/.gitignore` & `python-lsp-server-1.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/.policy.yml` & `python-lsp-server-1.7.2/.policy.yml`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/CHANGELOG.md` & `python-lsp-server-1.7.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # History of changes
 
+## Version 1.7.2 (2023/04/02)
+
+### Issues Closed
+
+* [Issue 325](https://github.com/python-lsp/python-lsp-server/issues/325) - WorkDoneProgress tokens not initialized properly by the server ([PR 328](https://github.com/python-lsp/python-lsp-server/pull/328) by [@syphar](https://github.com/syphar))
+* [Issue 260](https://github.com/python-lsp/python-lsp-server/issues/260) - yapf formatting fails when pyproject.toml is in the workspace ([PR 346](https://github.com/python-lsp/python-lsp-server/pull/346) by [@bnavigator](https://github.com/bnavigator))
+
+In this release 2 issues were closed.
+
+### Pull Requests Merged
+
+* [PR 346](https://github.com/python-lsp/python-lsp-server/pull/346) - Add toml dependency for yapf and constrain yapf to be less than 0.32, by [@bnavigator](https://github.com/bnavigator) ([260](https://github.com/python-lsp/python-lsp-server/issues/260))
+* [PR 345](https://github.com/python-lsp/python-lsp-server/pull/345) - Raise upper bound of autopep8, by [@bnavigator](https://github.com/bnavigator)
+* [PR 340](https://github.com/python-lsp/python-lsp-server/pull/340) - Bump pydocstyle to 6.3, by [@bnavigator](https://github.com/bnavigator)
+* [PR 328](https://github.com/python-lsp/python-lsp-server/pull/328) - Initialize LSP progress token before using it and remove progress for sync plugins, by [@syphar](https://github.com/syphar) ([325](https://github.com/python-lsp/python-lsp-server/issues/325))
+
+In this release 4 pull requests were closed.
+
+----
+
 ## Version 1.7.1 (2023/01/17)
 
 ### Issues Closed
 
 * [Issue 332](https://github.com/python-lsp/python-lsp-server/issues/332) - Failed to load hook pylsp_lint: too many values to unpack (expected 3) ([PR 329](https://github.com/python-lsp/python-lsp-server/pull/329) by [@ccordoba12](https://github.com/ccordoba12))
 
 In this release 1 issue was closed.
```

### Comparing `python-lsp-server-1.7.1/CONFIGURATION.md` & `python-lsp-server-1.7.2/CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/LICENSE` & `python-lsp-server-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/PKG-INFO` & `python-lsp-server-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-server
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python Language Server for the Language Server Protocol
 Author: Python Language Server Contributors
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-server
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `python-lsp-server-1.7.1/README.md` & `python-lsp-server-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/RELEASE.md` & `python-lsp-server-1.7.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/docs/autoimport.md` & `python-lsp-server-1.7.2/docs/autoimport.md`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/__init__.py` & `python-lsp-server-1.7.2/pylsp/__init__.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/__main__.py` & `python-lsp-server-1.7.2/pylsp/__main__.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/_utils.py` & `python-lsp-server-1.7.2/pylsp/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,16 +289,15 @@
         """
         if pid < 0:
             return False
         try:
             os.kill(pid, 0)
         except OSError as e:
             return e.errno == errno.EPERM
-        else:
-            return True
+        return True
 
 
 def get_eol_chars(text):
     """Get EOL chars used in text."""
     match = EOL_REGEX.search(text)
     if match:
         return match.group(0)
```

### Comparing `python-lsp-server-1.7.1/pylsp/config/config.py` & `python-lsp-server-1.7.2/pylsp/config/config.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/config/flake8_conf.py` & `python-lsp-server-1.7.2/pylsp/config/flake8_conf.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/config/pycodestyle_conf.py` & `python-lsp-server-1.7.2/pylsp/config/pycodestyle_conf.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/config/schema.json` & `python-lsp-server-1.7.2/pylsp/config/schema.json`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/config/source.py` & `python-lsp-server-1.7.2/pylsp/config/source.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/hookspecs.py` & `python-lsp-server-1.7.2/pylsp/hookspecs.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/lsp.py` & `python-lsp-server-1.7.2/pylsp/lsp.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/_resolvers.py` & `python-lsp-server-1.7.2/pylsp/plugins/_resolvers.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/_rope_task_handle.py` & `python-lsp-server-1.7.2/pylsp/plugins/_rope_task_handle.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/autopep8_format.py` & `python-lsp-server-1.7.2/pylsp/plugins/autopep8_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,25 +19,24 @@
         return _format(config, document)
 
 
 @hookimpl(tryfirst=True)  # Prefer autopep8 over YAPF
 def pylsp_format_range(
     config, workspace, document, range, options
 ):  # pylint: disable=redefined-builtin,unused-argument
-    with workspace.report_progress("format_range: autopep8"):
-        log.info("Formatting document %s in range %s with autopep8", document, range)
+    log.info("Formatting document %s in range %s with autopep8", document, range)
 
-        # First we 'round' the range up/down to full lines only
-        range['start']['character'] = 0
-        range['end']['line'] += 1
-        range['end']['character'] = 0
-
-        # Add 1 for 1-indexing vs LSP's 0-indexing
-        line_range = (range['start']['line'] + 1, range['end']['line'] + 1)
-        return _format(config, document, line_range=line_range)
+    # First we 'round' the range up/down to full lines only
+    range['start']['character'] = 0
+    range['end']['line'] += 1
+    range['end']['character'] = 0
+
+    # Add 1 for 1-indexing vs LSP's 0-indexing
+    line_range = (range['start']['line'] + 1, range['end']['line'] + 1)
+    return _format(config, document, line_range=line_range)
 
 
 def _format(config, document, line_range=None):
     options = _autopep8_config(config, document)
     if line_range:
         options['line_range'] = list(line_range)
```

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/definition.py` & `python-lsp-server-1.7.2/pylsp/plugins/definition.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,34 +4,33 @@
 import logging
 from pylsp import hookimpl, uris, _utils
 
 log = logging.getLogger(__name__)
 
 
 @hookimpl
-def pylsp_definitions(config, workspace, document, position):
-    with workspace.report_progress("go to definitions"):
-        settings = config.plugin_settings('jedi_definition')
-        code_position = _utils.position_to_jedi_linecolumn(document, position)
-        definitions = document.jedi_script(use_document_path=True).goto(
-            follow_imports=settings.get('follow_imports', True),
-            follow_builtin_imports=settings.get('follow_builtin_imports', True),
-            **code_position)
-
-        follow_builtin_defns = settings.get("follow_builtin_definitions", True)
-        return [
-            {
-                'uri': uris.uri_with(document.uri, path=str(d.module_path)),
-                'range': {
-                    'start': {'line': d.line - 1, 'character': d.column},
-                    'end': {'line': d.line - 1, 'character': d.column + len(d.name)},
-                }
+def pylsp_definitions(config, document, position):
+    settings = config.plugin_settings('jedi_definition')
+    code_position = _utils.position_to_jedi_linecolumn(document, position)
+    definitions = document.jedi_script(use_document_path=True).goto(
+        follow_imports=settings.get('follow_imports', True),
+        follow_builtin_imports=settings.get('follow_builtin_imports', True),
+        **code_position)
+
+    follow_builtin_defns = settings.get("follow_builtin_definitions", True)
+    return [
+        {
+            'uri': uris.uri_with(document.uri, path=str(d.module_path)),
+            'range': {
+                'start': {'line': d.line - 1, 'character': d.column},
+                'end': {'line': d.line - 1, 'character': d.column + len(d.name)},
             }
-            for d in definitions if d.is_definition() and (follow_builtin_defns or _not_internal_definition(d))
-        ]
+        }
+        for d in definitions if d.is_definition() and (follow_builtin_defns or _not_internal_definition(d))
+    ]
 
 
 def _not_internal_definition(definition):
     return (
         definition.line is not None and
         definition.column is not None and
         definition.module_path is not None and
```

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/flake8_lint.py` & `python-lsp-server-1.7.2/pylsp/plugins/flake8_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/folding.py` & `python-lsp-server-1.7.2/pylsp/plugins/folding.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/highlight.py` & `python-lsp-server-1.7.2/pylsp/plugins/highlight.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/hover.py` & `python-lsp-server-1.7.2/pylsp/plugins/hover.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/jedi_completion.py` & `python-lsp-server-1.7.2/pylsp/plugins/jedi_completion.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/jedi_rename.py` & `python-lsp-server-1.7.2/pylsp/plugins/jedi_rename.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,50 +5,48 @@
 
 from pylsp import hookimpl, uris, _utils
 
 log = logging.getLogger(__name__)
 
 
 @hookimpl
-def pylsp_rename(config, workspace, document, position, new_name):  # pylint: disable=unused-argument,too-many-locals
-    with workspace.report_progress("rename", percentage=0) as report_progress:
-        log.debug('Executing rename of %s to %s', document.word_at_position(position), new_name)
-        kwargs = _utils.position_to_jedi_linecolumn(document, position)
-        kwargs['new_name'] = new_name
-        report_progress("refactoring")
-        try:
-            refactoring = document.jedi_script().rename(**kwargs)
-        except NotImplementedError as exc:
-            raise Exception('No support for renaming in Python 2/3.5 with Jedi. '
-                            'Consider using the rope_rename plugin instead') from exc
-        log.debug('Finished rename: %s', refactoring.get_diff())
-        changes = []
-
-        changed_files = refactoring.get_changed_files()
-        for n, (file_path, changed_file) in enumerate(changed_files.items()):
-            report_progress(changed_file, percentage=n/len(changed_files)*100)
-            uri = uris.from_fs_path(str(file_path))
-            doc = workspace.get_maybe_document(uri)
-            changes.append({
-                'textDocument': {
-                    'uri': uri,
-                    'version': doc.version if doc else None
-                },
-                'edits': [
-                    {
-                        'range': {
-                            'start': {'line': 0, 'character': 0},
-                            'end': {
-                                'line': _num_lines(changed_file.get_new_code()),
-                                'character': 0,
-                            },
+def pylsp_rename(config, workspace, document, position, new_name):  # pylint: disable=unused-argument
+    log.debug('Executing rename of %s to %s', document.word_at_position(position), new_name)
+    kwargs = _utils.position_to_jedi_linecolumn(document, position)
+    kwargs['new_name'] = new_name
+    try:
+        refactoring = document.jedi_script().rename(**kwargs)
+    except NotImplementedError as exc:
+        # pylint: disable=broad-exception-raised
+        raise Exception('No support for renaming in Python 2/3.5 with Jedi. '
+                        'Consider using the rope_rename plugin instead') from exc
+    log.debug('Finished rename: %s', refactoring.get_diff())
+    changes = []
+
+    changed_files = refactoring.get_changed_files()
+    for file_path, changed_file in changed_files.items():
+        uri = uris.from_fs_path(str(file_path))
+        doc = workspace.get_maybe_document(uri)
+        changes.append({
+            'textDocument': {
+                'uri': uri,
+                'version': doc.version if doc else None
+            },
+            'edits': [
+                {
+                    'range': {
+                        'start': {'line': 0, 'character': 0},
+                        'end': {
+                            'line': _num_lines(changed_file.get_new_code()),
+                            'character': 0,
                         },
-                        'newText': changed_file.get_new_code(),
-                    }
-                ],
-            })
-        return {'documentChanges': changes}
+                    },
+                    'newText': changed_file.get_new_code(),
+                }
+            ],
+        })
+    return {'documentChanges': changes}
 
 
 def _num_lines(file_contents):
     'Count the number of lines in the given string.'
     return len(file_contents.splitlines())
```

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/mccabe_lint.py` & `python-lsp-server-1.7.2/pylsp/plugins/mccabe_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/preload_imports.py` & `python-lsp-server-1.7.2/pylsp/plugins/preload_imports.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/pycodestyle_lint.py` & `python-lsp-server-1.7.2/pylsp/plugins/pycodestyle_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/pydocstyle_lint.py` & `python-lsp-server-1.7.2/pylsp/plugins/pydocstyle_lint.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 def pylsp_settings():
     # Default pydocstyle to disabled
     return {'plugins': {'pydocstyle': {'enabled': False}}}
 
 
 @hookimpl
 def pylsp_lint(config, workspace, document):
+    # pylint: disable=too-many-locals
     with workspace.report_progress("lint: pydocstyle"):
         settings = config.plugin_settings('pydocstyle', document_path=document.path)
         log.debug("Got pydocstyle settings: %s", settings)
 
         # Explicitly passing a path to pydocstyle means it doesn't respect the --match flag, so do it ourselves
         filename_match_re = re.compile(settings.get('match', DEFAULT_MATCH_RE) + '$')
         if not filename_match_re.match(os.path.basename(document.path)):
@@ -62,17 +63,27 @@
         conf = pydocstyle.config.ConfigurationParser()
         with _patch_sys_argv(args):
             # TODO(gatesn): We can add more pydocstyle args here from our pylsp config
             conf.parse()
 
         # Will only yield a single filename, the document path
         diags = []
-        for filename, checked_codes, ignore_decorators, property_decorators in conf.get_files_to_check():
+        for (
+            filename,
+            checked_codes,
+            ignore_decorators,
+            property_decorators,
+            ignore_self_only_init,
+        ) in conf.get_files_to_check():
             errors = pydocstyle.checker.ConventionChecker().check_source(
-                document.source, filename, ignore_decorators=ignore_decorators, property_decorators=property_decorators
+                document.source,
+                filename,
+                ignore_decorators=ignore_decorators,
+                property_decorators=property_decorators,
+                ignore_self_only_init=ignore_self_only_init,
             )
 
             try:
                 for error in errors:
                     if error.code not in checked_codes:
                         continue
                     diags.append(_parse_diagnostic(document, error))
```

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/pyflakes_lint.py` & `python-lsp-server-1.7.2/pylsp/plugins/pyflakes_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/pylint_lint.py` & `python-lsp-server-1.7.2/pylsp/plugins/pylint_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/references.py` & `python-lsp-server-1.7.2/pylsp/plugins/references.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 import logging
 from pylsp import hookimpl, uris, _utils
 
 log = logging.getLogger(__name__)
 
 
 @hookimpl
-def pylsp_references(document, workspace, position, exclude_declaration=False):
-    with workspace.report_progress("references"):
-        code_position = _utils.position_to_jedi_linecolumn(document, position)
-        usages = document.jedi_script().get_references(**code_position)
+def pylsp_references(document, position, exclude_declaration=False):
+    code_position = _utils.position_to_jedi_linecolumn(document, position)
+    usages = document.jedi_script().get_references(**code_position)
 
-        if exclude_declaration:
-            # Filter out if the usage is the actual declaration of the thing
-            usages = [d for d in usages if not d.is_definition()]
+    if exclude_declaration:
+        # Filter out if the usage is the actual declaration of the thing
+        usages = [d for d in usages if not d.is_definition()]
 
-        # Filter out builtin modules
-        return [{
-            'uri': uris.uri_with(document.uri, path=str(d.module_path)) if d.module_path else document.uri,
-            'range': {
-                'start': {'line': d.line - 1, 'character': d.column},
-                'end': {'line': d.line - 1, 'character': d.column + len(d.name)}
-            }
-        } for d in usages if not d.in_builtin_module()]
+    # Filter out builtin modules
+    return [{
+        'uri': uris.uri_with(document.uri, path=str(d.module_path)) if d.module_path else document.uri,
+        'range': {
+            'start': {'line': d.line - 1, 'character': d.column},
+            'end': {'line': d.line - 1, 'character': d.column + len(d.name)}
+        }
+    } for d in usages if not d.in_builtin_module()]
```

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/rope_autoimport.py` & `python-lsp-server-1.7.2/pylsp/plugins/rope_autoimport.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/rope_completion.py` & `python-lsp-server-1.7.2/pylsp/plugins/rope_completion.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/rope_rename.py` & `python-lsp-server-1.7.2/pylsp/plugins/rope_rename.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,48 +15,47 @@
 def pylsp_settings():
     # Default rope_rename to disabled
     return {'plugins': {'rope_rename': {'enabled': False}}}
 
 
 @hookimpl
 def pylsp_rename(config, workspace, document, position, new_name):
-    with workspace.report_progress("rename"):
-        rope_config = config.settings(document_path=document.path).get('rope', {})
-        rope_project = workspace._rope_project_builder(rope_config)
-
-        rename = Rename(
-            rope_project,
-            libutils.path_to_resource(rope_project, document.path),
-            document.offset_at_position(position)
-        )
-
-        log.debug("Executing rename of %s to %s", document.word_at_position(position), new_name)
-        changeset = rename.get_changes(new_name, in_hierarchy=True, docs=True)
-        log.debug("Finished rename: %s", changeset.changes)
-        changes = []
-        for change in changeset.changes:
-            uri = uris.from_fs_path(change.resource.path)
-            doc = workspace.get_maybe_document(uri)
-            changes.append({
-                'textDocument': {
-                    'uri': uri,
-                    'version': doc.version if doc else None
-                },
-                'edits': [
-                    {
-                        'range': {
-                            'start': {'line': 0, 'character': 0},
-                            'end': {
-                                'line': _num_lines(change.resource),
-                                'character': 0,
-                            },
+    rope_config = config.settings(document_path=document.path).get('rope', {})
+    rope_project = workspace._rope_project_builder(rope_config)
+
+    rename = Rename(
+        rope_project,
+        libutils.path_to_resource(rope_project, document.path),
+        document.offset_at_position(position)
+    )
+
+    log.debug("Executing rename of %s to %s", document.word_at_position(position), new_name)
+    changeset = rename.get_changes(new_name, in_hierarchy=True, docs=True)
+    log.debug("Finished rename: %s", changeset.changes)
+    changes = []
+    for change in changeset.changes:
+        uri = uris.from_fs_path(change.resource.path)
+        doc = workspace.get_maybe_document(uri)
+        changes.append({
+            'textDocument': {
+                'uri': uri,
+                'version': doc.version if doc else None
+            },
+            'edits': [
+                {
+                    'range': {
+                        'start': {'line': 0, 'character': 0},
+                        'end': {
+                            'line': _num_lines(change.resource),
+                            'character': 0,
                         },
-                        'newText': change.new_contents,
-                    }
-                ]
-            })
-        return {'documentChanges': changes}
+                    },
+                    'newText': change.new_contents,
+                }
+            ]
+        })
+    return {'documentChanges': changes}
 
 
 def _num_lines(resource):
     "Count the number of lines in a `File` resource."
     return len(resource.read().splitlines())
```

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/signature.py` & `python-lsp-server-1.7.2/pylsp/plugins/signature.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/symbols.py` & `python-lsp-server-1.7.2/pylsp/plugins/symbols.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/plugins/yapf_format.py` & `python-lsp-server-1.7.2/pylsp/plugins/yapf_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,31 +19,30 @@
 def pylsp_format_document(workspace, document, options):
     log.info("Formatting document %s with yapf", document)
     with workspace.report_progress("format: yapf"):
         return _format(document, options=options)
 
 
 @hookimpl
-def pylsp_format_range(workspace, document, range, options):  # pylint: disable=redefined-builtin
+def pylsp_format_range(document, range, options):  # pylint: disable=redefined-builtin
     log.info("Formatting document %s in range %s with yapf", document, range)
-    with workspace.report_progress("format_range: yapf"):
-        # First we 'round' the range up/down to full lines only
-        range['start']['character'] = 0
-        range['end']['line'] += 1
-        range['end']['character'] = 0
-
-        # From Yapf docs:
-        # lines: (list of tuples of integers) A list of tuples of lines, [start, end],
-        #   that we want to format. The lines are 1-based indexed. It can be used by
-        #   third-party code (e.g., IDEs) when reformatting a snippet of code rather
-        #   than a whole file.
-
-        # Add 1 for 1-indexing vs LSP's 0-indexing
-        lines = [(range['start']['line'] + 1, range['end']['line'] + 1)]
-        return _format(document, lines=lines, options=options)
+    # First we 'round' the range up/down to full lines only
+    range['start']['character'] = 0
+    range['end']['line'] += 1
+    range['end']['character'] = 0
+
+    # From Yapf docs:
+    # lines: (list of tuples of integers) A list of tuples of lines, [start, end],
+    #   that we want to format. The lines are 1-based indexed. It can be used by
+    #   third-party code (e.g., IDEs) when reformatting a snippet of code rather
+    #   than a whole file.
+
+    # Add 1 for 1-indexing vs LSP's 0-indexing
+    lines = [(range['start']['line'] + 1, range['end']['line'] + 1)]
+    return _format(document, lines=lines, options=options)
 
 
 def get_style_config(document_path, options=None):
     # Exclude file if it follows the patterns for that
     exclude_patterns_from_ignore_file = file_resources.GetExcludePatternsForDir(os.getcwd())
     if file_resources.IsIgnored(document_path, exclude_patterns_from_ignore_file):
         return []
```

### Comparing `python-lsp-server-1.7.1/pylsp/python_lsp.py` & `python-lsp-server-1.7.2/pylsp/python_lsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 class PythonLSPServer(MethodDispatcher):
     """ Implementation of the Microsoft VSCode Language Server Protocol
     https://github.com/Microsoft/language-server-protocol/blob/master/versions/protocol-1-x.md
     """
 
     # pylint: disable=too-many-public-methods,redefined-builtin
 
-    def __init__(self, rx, tx, check_parent_process=False, consumer=None):
+    def __init__(self, rx, tx, check_parent_process=False, consumer=None, *, endpoint_cls=None):
         self.workspace = None
         self.config = None
         self.root_uri = None
         self.watching_thread = None
         self.workspaces = {}
         self.uri_workspace_mapper = {}
 
@@ -168,19 +168,21 @@
             self._jsonrpc_stream_reader = None
 
         if tx is not None:
             self._jsonrpc_stream_writer = JsonRpcStreamWriter(tx)
         else:
             self._jsonrpc_stream_writer = None
 
+        endpoint_cls = endpoint_cls or Endpoint
+
         # if consumer is None, it is assumed that the default streams-based approach is being used
         if consumer is None:
-            self._endpoint = Endpoint(self, self._jsonrpc_stream_writer.write, max_workers=MAX_WORKERS)
+            self._endpoint = endpoint_cls(self, self._jsonrpc_stream_writer.write, max_workers=MAX_WORKERS)
         else:
-            self._endpoint = Endpoint(self, consumer, max_workers=MAX_WORKERS)
+            self._endpoint = endpoint_cls(self, consumer, max_workers=MAX_WORKERS)
 
         self._dispatchers = []
         self._shutdown = False
 
     def start(self):
         """Entry point for the server."""
         self._jsonrpc_stream_reader.listen(self._endpoint.consume)
@@ -354,15 +356,15 @@
     def document_did_save(self, doc_uri):
         return self._hook("pylsp_document_did_save", doc_uri)
 
     def execute_command(self, command, arguments):
         return self._hook('pylsp_execute_command', command=command, arguments=arguments)
 
     def format_document(self, doc_uri, options):
-        return self._hook('pylsp_format_document', doc_uri, options=options)
+        return lambda: self._hook('pylsp_format_document', doc_uri, options=options)
 
     def format_range(self, doc_uri, range, options):
         return self._hook('pylsp_format_range', doc_uri, range=range, options=options)
 
     def highlight(self, doc_uri, position):
         return flatten(self._hook('pylsp_document_highlight', doc_uri, position=position)) or None
```

### Comparing `python-lsp-server-1.7.1/pylsp/text_edit.py` & `python-lsp-server-1.7.2/pylsp/text_edit.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/uris.py` & `python-lsp-server-1.7.2/pylsp/uris.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/pylsp/workspace.py` & `python-lsp-server-1.7.2/pylsp/workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     return wrapper
 
 
 class Workspace:
 
     M_PUBLISH_DIAGNOSTICS = 'textDocument/publishDiagnostics'
     M_PROGRESS = '$/progress'
+    M_INITIALIZE_PROGRESS = 'window/workDoneProgress/create'
     M_APPLY_EDIT = 'workspace/applyEdit'
     M_SHOW_MESSAGE = 'window/showMessage'
 
     def __init__(self, root_uri, endpoint, config=None):
         self._config = config
         self._root_uri = root_uri
         self._endpoint = endpoint
@@ -131,38 +132,69 @@
     @contextmanager
     def report_progress(
         self,
         title: str,
         message: Optional[str] = None,
         percentage: Optional[int] = None,
     ) -> Generator[Callable[[str, Optional[int]], None], None, None]:
-        token = self._progress_begin(title, message, percentage)
+        if self._config:
+            client_supports_progress_reporting = (
+                self._config.capabilities.get("window", {}).get("workDoneProgress", False)
+            )
+        else:
+            client_supports_progress_reporting = False
+
+        if client_supports_progress_reporting:
+            try:
+                token = self._progress_begin(title, message, percentage)
+            except Exception:  # pylint: disable=broad-exception-caught
+                log.warning(
+                    "There was an error while trying to initialize progress reporting."
+                    "Likely progress reporting was used in a synchronous LSP handler, "
+                    "which is not supported by progress reporting yet.",
+                    exc_info=True
+                )
 
-        def progress_message(message: str, percentage: Optional[int] = None) -> None:
-            self._progress_report(token, message, percentage)
+            else:
+                def progress_message(message: str, percentage: Optional[int] = None) -> None:
+                    self._progress_report(token, message, percentage)
+
+                try:
+                    yield progress_message
+                finally:
+                    self._progress_end(token)
+
+                return
+
+        # FALLBACK:
+        # If the client doesn't support progress reporting, or if we failed to
+        # initialize it, we have a dummy method for the caller to use.
+        def dummy_progress_message(message: str, percentage: Optional[int] = None) -> None:
+            # pylint: disable=unused-argument
+            pass
 
-        try:
-            yield progress_message
-        finally:
-            self._progress_end(token)
+        yield dummy_progress_message
 
     def _progress_begin(
         self,
         title: str,
         message: Optional[str] = None,
         percentage: Optional[int] = None,
     ) -> str:
         token = str(uuid.uuid4())
+
+        self._endpoint.request(self.M_INITIALIZE_PROGRESS, {'token': token}).result(timeout=1.0)
+
         value = {
             "kind": "begin",
             "title": title,
         }
-        if message:
+        if message is not None:
             value["message"] = message
-        if percentage:
+        if percentage is not None:
             value["percentage"] = percentage
 
         self._endpoint.notify(
             self.M_PROGRESS,
             params={
                 "token": token,
                 "value": value,
```

### Comparing `python-lsp-server-1.7.1/pyproject.toml` & `python-lsp-server-1.7.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,34 +23,35 @@
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/python-lsp/python-lsp-server"
 
 [project.optional-dependencies]
 all = [
-    "autopep8>=1.6.0,<1.7.0",
+    "autopep8>=1.6.0,<2.1.0",
     "flake8>=5.0.0,<7",
     "mccabe>=0.7.0,<0.8.0",
     "pycodestyle>=2.9.0,<2.11.0",
-    "pydocstyle>=6.2.0,<6.3.0",
+    "pydocstyle>=6.3.0,<6.4.0",
     "pyflakes>=2.5.0,<3.1.0",
     "pylint>=2.5.0,<3",
     "rope>1.2.0",
-    "yapf",
+    "yapf<=0.32.0",
+    "toml",
     "whatthepatch>=1.0.2,<2.0.0"
 ]
-autopep8 = ["autopep8>=1.6.0,<1.7.0"]
+autopep8 = ["autopep8>=1.6.0,<2.1.0"]
 flake8 = ["flake8>=5.0.0,<7"]
 mccabe = ["mccabe>=0.7.0,<0.8.0"]
 pycodestyle = ["pycodestyle>=2.9.0,<2.11.0"]
-pydocstyle = ["pydocstyle>=6.2.0,<6.3.0"]
+pydocstyle = ["pydocstyle>=6.3.0,<6.4.0"]
 pyflakes = ["pyflakes>=2.5.0,<3.1.0"]
 pylint = ["pylint>=2.5.0,<3"]
 rope = ["rope>1.2.0"]
-yapf = ["yapf", "whatthepatch>=1.0.2,<2.0.0"]
+yapf = ["yapf<=0.32.0", "whatthepatch>=1.0.2,<2.0.0", "toml"]
 websockets = ["websockets>=10.3"]
 test = [
     "pylint>=2.5.0,<3",
     "pytest",
     "pytest-cov",
     "coverage",
     "numpy",
```

### Comparing `python-lsp-server-1.7.1/python_lsp_server.egg-info/PKG-INFO` & `python-lsp-server-1.7.2/python_lsp_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-server
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python Language Server for the Language Server Protocol
 Author: Python Language Server Contributors
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-server
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `python-lsp-server-1.7.1/python_lsp_server.egg-info/SOURCES.txt` & `python-lsp-server-1.7.2/python_lsp_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/python_lsp_server.egg-info/entry_points.txt` & `python-lsp-server-1.7.2/python_lsp_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/scripts/jsonschema2md.py` & `python-lsp-server-1.7.2/scripts/jsonschema2md.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_autoimport.py` & `python-lsp-server-1.7.2/test/plugins/test_autoimport.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_autopep8_format.py` & `python-lsp-server-1.7.2/test/plugins/test_autopep8_format.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_completion.py` & `python-lsp-server-1.7.2/test/plugins/test_completion.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_definitions.py` & `python-lsp-server-1.7.2/test/plugins/test_definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,36 +31,36 @@
     # The definition of 'a'
     def_range = {
         'start': {'line': 0, 'character': 4},
         'end': {'line': 0, 'character': 5}
     }
 
     doc = Document(DOC_URI, workspace, DOC)
-    assert [{'uri': DOC_URI, 'range': def_range}] == pylsp_definitions(config, workspace, doc, cursor_pos)
+    assert [{'uri': DOC_URI, 'range': def_range}] == pylsp_definitions(config, doc, cursor_pos)
 
 
 def test_builtin_definition(config, workspace):
     # Over 'i' in dict
     cursor_pos = {'line': 8, 'character': 24}
 
     doc = Document(DOC_URI, workspace, DOC)
     orig_settings = config.settings()
 
     # Check definition for `dict` goes to `builtins.pyi::dict`
     follow_defns_setting = {'follow_builtin_definitions': True}
     settings = {'plugins': {'jedi_definition': follow_defns_setting}}
     config.update(settings)
-    defns = pylsp_definitions(config, workspace, doc, cursor_pos)
+    defns = pylsp_definitions(config, doc, cursor_pos)
     assert len(defns) == 1
     assert defns[0]["uri"].endswith("builtins.pyi")
 
     # Check no definitions for `dict`
     follow_defns_setting['follow_builtin_definitions'] = False
     config.update(settings)
-    defns = pylsp_definitions(config, workspace, doc, cursor_pos)
+    defns = pylsp_definitions(config, doc, cursor_pos)
     assert not defns
 
     config.update(orig_settings)
 
 
 def test_assignment(config, workspace):
     # Over 's' in self.members[id]
@@ -69,15 +69,15 @@
     # The assignment of 'self.members'
     def_range = {
         'start': {'line': 8, 'character': 13},
         'end': {'line': 8, 'character': 20}
     }
 
     doc = Document(DOC_URI, workspace, DOC)
-    assert [{'uri': DOC_URI, 'range': def_range}] == pylsp_definitions(config, workspace, doc, cursor_pos)
+    assert [{'uri': DOC_URI, 'range': def_range}] == pylsp_definitions(config, doc, cursor_pos)
 
 
 def test_document_path_definitions(config, workspace_other_root_path, tmpdir):
     # Create a dummy module out of the workspace's root_path and try to get
     # a definition on it in another file placed next to it.
     module_content = '''
 def foo():
@@ -103,9 +103,9 @@
     cursor_pos = {'line': 0, 'character': 24}
 
     # The uri for mymodule.py
     module_path = str(p)
     module_uri = uris.from_fs_path(module_path)
 
     assert [{"uri": module_uri, "range": def_range}] == pylsp_definitions(
-        config, workspace_other_root_path, doc, cursor_pos
+        config, doc, cursor_pos
     )
```

### Comparing `python-lsp-server-1.7.1/test/plugins/test_flake8_lint.py` & `python-lsp-server-1.7.2/test/plugins/test_flake8_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_folding.py` & `python-lsp-server-1.7.2/test/plugins/test_folding.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_highlight.py` & `python-lsp-server-1.7.2/test/plugins/test_highlight.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_hover.py` & `python-lsp-server-1.7.2/test/plugins/test_hover.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_jedi_rename.py` & `python-lsp-server-1.7.2/test/plugins/test_jedi_rename.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_mccabe_lint.py` & `python-lsp-server-1.7.2/test/plugins/test_mccabe_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_pycodestyle_lint.py` & `python-lsp-server-1.7.2/test/plugins/test_pycodestyle_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_pydocstyle_lint.py` & `python-lsp-server-1.7.2/test/plugins/test_pydocstyle_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_pyflakes_lint.py` & `python-lsp-server-1.7.2/test/plugins/test_pyflakes_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_pylint_lint.py` & `python-lsp-server-1.7.2/test/plugins/test_pylint_lint.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_references.py` & `python-lsp-server-1.7.2/test/plugins/test_references.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 
 def test_references(tmp_workspace):  # pylint: disable=redefined-outer-name
     # Over 'Test1' in class Test1():
     position = {'line': 0, 'character': 8}
     DOC1_URI = uris.from_fs_path(os.path.join(tmp_workspace.root_path, DOC1_NAME))
     doc1 = Document(DOC1_URI, tmp_workspace)
 
-    refs = pylsp_references(doc1, tmp_workspace, position)
+    refs = pylsp_references(doc1, position)
 
     # Definition, the import and the instantiation
     assert len(refs) == 3
 
     # Briefly check excluding the definitions (also excludes imports, only counts uses)
-    no_def_refs = pylsp_references(doc1, tmp_workspace, position, exclude_declaration=True)
+    no_def_refs = pylsp_references(doc1, position, exclude_declaration=True)
     assert len(no_def_refs) == 1
 
     # Make sure our definition is correctly located
     doc1_ref = [u for u in refs if u['uri'] == DOC1_URI][0]
     assert doc1_ref['range']['start'] == {'line': 0, 'character': 6}
     assert doc1_ref['range']['end'] == {'line': 0, 'character': 11}
 
@@ -66,14 +66,14 @@
 
 def test_references_builtin(tmp_workspace):  # pylint: disable=redefined-outer-name
     # Over 'UnicodeError':
     position = {'line': 4, 'character': 7}
     doc2_uri = uris.from_fs_path(os.path.join(str(tmp_workspace.root_path), DOC2_NAME))
     doc2 = Document(doc2_uri, tmp_workspace)
 
-    refs = pylsp_references(doc2, tmp_workspace, position)
+    refs = pylsp_references(doc2, position)
     assert len(refs) >= 1
 
     expected = {'start': {'line': 4, 'character': 7},
                 'end': {'line': 4, 'character': 19}}
     ranges = [r['range'] for r in refs]
     assert expected in ranges
```

### Comparing `python-lsp-server-1.7.1/test/plugins/test_rope_rename.py` & `python-lsp-server-1.7.2/test/plugins/test_rope_rename.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_signature.py` & `python-lsp-server-1.7.2/test/plugins/test_signature.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_symbols.py` & `python-lsp-server-1.7.2/test/plugins/test_symbols.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/plugins/test_yapf_format.py` & `python-lsp-server-1.7.2/test/plugins/test_yapf_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 def test_range_format(workspace):
     doc = Document(DOC_URI, workspace, DOC)
 
     def_range = {
         'start': {'line': 0, 'character': 0},
         'end': {'line': 4, 'character': 10}
     }
-    res = pylsp_format_range(workspace, doc, def_range, None)
+    res = pylsp_format_range(doc, def_range, None)
 
     # Make sure B is still badly formatted
     assert apply_text_edits(doc, res) == "A = ['h', 'w', 'a']\n\nB = ['h',\n\n\n'w']\n"
 
 
 def test_no_change(workspace):
     doc = Document(DOC_URI, workspace, GOOD_DOC)
```

### Comparing `python-lsp-server-1.7.1/test/test_document.py` & `python-lsp-server-1.7.2/test/test_document.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/test_language_server.py` & `python-lsp-server-1.7.2/test/test_language_server.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/test_text_edit.py` & `python-lsp-server-1.7.2/test/test_text_edit.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/test_uris.py` & `python-lsp-server-1.7.2/test/test_uris.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/test_utils.py` & `python-lsp-server-1.7.2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-lsp-server-1.7.1/test/test_workspace.py` & `python-lsp-server-1.7.2/test/test_workspace.py`

 * *Files 24% similar despite different names*

```diff
@@ -291,75 +291,117 @@
 
     # Assert settings are inherited from the server config.
     workspace1_object = pylsp.workspaces[workspace1['uri']]
     workspace1_jedi_settings = workspace1_object._config.plugin_settings('jedi')
     assert workspace1_jedi_settings == server_settings['pylsp']['plugins']['jedi']
 
 
+def test_no_progress_without_capability(workspace, consumer):
+    workspace._config.capabilities['window'] = {"workDoneProgress": False}
+
+    with workspace.report_progress("some_title"):
+        pass
+
+    assert len(consumer.call_args_list) == 0
+
+
 def test_progress_simple(workspace, consumer):
+    workspace._config.capabilities['window'] = {"workDoneProgress": True}
+
     with workspace.report_progress("some_title"):
         pass
 
+    init_call, *progress_calls = consumer.call_args_list
+
+    assert init_call[0][0]['method'] == 'window/workDoneProgress/create'
+
     # same method for all calls
-    assert all(call[0][0]["method"] == "$/progress" for call in consumer.call_args_list)
+    assert all(call[0][0]["method"] == "$/progress" for call in progress_calls), consumer.call_args_list
 
     # same token used in all calls
-    assert len({call[0][0]["params"]["token"] for call in consumer.call_args_list}) == 1
+    assert len({call[0][0]["params"]["token"] for call in progress_calls} | {init_call[0][0]['params']['token']}) == 1
 
-    assert [call[0][0]["params"]["value"] for call in consumer.call_args_list] == [
+    assert [call[0][0]["params"]["value"] for call in progress_calls] == [
         {"kind": "begin", "title": "some_title"},
         {"kind": "end"},
     ]
 
 
+@pytest.mark.parametrize("exc", [Exception("something"), TimeoutError()])
+def test_progress_initialization_fails(workspace, consumer, endpoint, exc):
+    def failing_token_initialization(self, *_args, **_kwargs):
+        raise exc
+    endpoint._dispatcher.m_window__work_done_progress__create = failing_token_initialization
+
+    workspace._config.capabilities['window'] = {"workDoneProgress": True}
+
+    with workspace.report_progress("some_title"):
+        pass
+
+    # we only see the failing token initialization call, no other calls
+    init_call, = consumer.call_args_list
+    assert init_call[0][0]['method'] == 'window/workDoneProgress/create'
+
+
 def test_progress_with_percent(workspace, consumer):
+    workspace._config.capabilities['window'] = {"workDoneProgress": True}
+
     with workspace.report_progress(
         "some_title", "initial message", percentage=1
     ) as progress_message:
         progress_message("ten", 10)
         progress_message("fifty", 50)
         progress_message("ninety", 90)
 
-    # same method for all calls
-    assert all(call[0][0]["method"] == "$/progress" for call in consumer.call_args_list)
+    init_call, *progress_calls = consumer.call_args_list
+
+    assert init_call[0][0]['method'] == 'window/workDoneProgress/create'
+
+    # same method for all progress calls
+    assert all(call[0][0]["method"] == "$/progress" for call in progress_calls)
 
     # same token used in all calls
-    assert len({call[0][0]["params"]["token"] for call in consumer.call_args_list}) == 1
+    assert len({call[0][0]["params"]["token"] for call in progress_calls} | {init_call[0][0]['params']['token']}) == 1
 
-    assert [call[0][0]["params"]["value"] for call in consumer.call_args_list] == [
+    assert [call[0][0]["params"]["value"] for call in progress_calls] == [
         {
             "kind": "begin",
             "message": "initial message",
             "percentage": 1,
             "title": "some_title",
         },
         {"kind": "report", "message": "ten", "percentage": 10},
         {"kind": "report", "message": "fifty", "percentage": 50},
         {"kind": "report", "message": "ninety", "percentage": 90},
         {"kind": "end"},
     ]
 
 
 def test_progress_with_exception(workspace, consumer):
+    workspace._config.capabilities['window'] = {"workDoneProgress": True}
+
     class DummyError(Exception):
         pass
 
     try:
         with workspace.report_progress("some_title"):
             raise DummyError("something")
     except DummyError:
         # we're using a specific exception class here so
         # any other exceptions happening in progress
         # reporting would correctly be raised in the
         # test.
         pass
 
+    init_call, *progress_calls = consumer.call_args_list
+    assert init_call[0][0]['method'] == 'window/workDoneProgress/create'
+
     # same method for all calls
-    assert all(call[0][0]["method"] == "$/progress" for call in consumer.call_args_list)
+    assert all(call[0][0]["method"] == "$/progress" for call in progress_calls)
 
     # same token used in all calls
-    assert len({call[0][0]["params"]["token"] for call in consumer.call_args_list}) == 1
+    assert len({call[0][0]["params"]["token"] for call in progress_calls} | {init_call[0][0]['params']['token']}) == 1
 
-    assert [call[0][0]["params"]["value"] for call in consumer.call_args_list] == [
+    assert [call[0][0]["params"]["value"] for call in progress_calls] == [
         {"kind": "begin", "title": "some_title"},
         {"kind": "end"},
     ]
```

