# Comparing `tmp/ansible-compat-4.0.2.tar.gz` & `tmp/ansible-compat-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.0.2.tar", last modified: Thu May  4 15:13:15 2023, max compression
+gzip compressed data, was "ansible-compat-4.0.3.tar", last modified: Mon May 15 15:05:25 2023, max compression
```

## Comparing `ansible-compat-4.0.2.tar` & `ansible-compat-4.0.3.tar`

### file list

```diff
@@ -1,113 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.606701 ansible-compat-4.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.598701 ansible-compat-4.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.610701 ansible-compat-4.0.2/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.598701 ansible-compat-4.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.614701 ansible-compat-4.0.2/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28537 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.614701 ansible-compat-4.0.2/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 15:13:15.000000 ansible-compat-4.0.2/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.618701 ansible-compat-4.0.2/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/collections/acme.goodies/roles/baz/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.602701 ansible-compat-4.0.2/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:15.622701 ansible-compat-4.0.2/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    24524 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-04 15:12:59.000000 ansible-compat-4.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.486543 ansible-compat-4.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.470543 ansible-compat-4.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.494543 ansible-compat-4.0.3/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.474543 ansible-compat-4.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.498543 ansible-compat-4.0.3/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31373 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.498543 ansible-compat-4.0.3/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.502543 ansible-compat-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.474543 ansible-compat-4.0.3/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.474543 ansible-compat-4.0.3/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.474543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/tests/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.482543 ansible-compat-4.0.3/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.482543 ansible-compat-4.0.3/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25019 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/tox.ini
```

### Comparing `ansible-compat-4.0.2/.github/dependabot.yml` & `ansible-compat-4.0.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/.github/workflows/release.yml` & `ansible-compat-4.0.3/.github/workflows/release.yml`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
   release:
     name: release ${{ github.event.ref }}
     needs: before-release
     # unable to use environment with uses/with, basically cannot reuse release pipelines
     environment: release
     runs-on: ubuntu-22.04
+    permissions:
+      id-token: write
 
     env:
       FORCE_COLOR: 1
       PY_COLORS: 1
       TOX_PARALLEL_NO_SPINNER: 1
 
     steps:
@@ -31,9 +33,7 @@
         uses: actions/checkout@v3
         with:
           fetch-depth: 0 # needed by setuptools-scm
       - name: Build dists
         run: python -m tox -e pkg
       - name: Publish to pypi.org
         uses: pypa/gh-action-pypi-publish@unstable/v1
-        with:
-          password: ${{ secrets.pypi_password }}
```

### Comparing `ansible-compat-4.0.2/.github/workflows/tox.yml` & `ansible-compat-4.0.3/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/.gitignore` & `ansible-compat-4.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/.pre-commit-config.yaml` & `ansible-compat-4.0.3/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   python: python3.9
 exclude: |
   (?x)^(
     test/assets/.*
   )$
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.263"
+    rev: "v0.0.267"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
     rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
@@ -61,15 +61,15 @@
         entry: yamllint --strict
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: ["--strict"]
         additional_dependencies:
           - ansible-core
           - cached_property
```

### Comparing `ansible-compat-4.0.2/.readthedocs.yml` & `ansible-compat-4.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/.vscode/settings.json` & `ansible-compat-4.0.3/.vscode/settings.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939903846153846%*

 * *Differences: {"'[python]'": "{'editor.codeActionsOnSave': {'source.organizeImports': False, "*

 * *               "'source.fixAll.ruff': True, 'source.organizeImports.ruff': True}}"}*

```diff
@@ -1,15 +1,17 @@
 {
     "[markdown]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
     "[python]": {
         "editor.codeActionsOnSave": {
             "source.fixAll": true,
-            "source.organizeImports": true
+            "source.fixAll.ruff": true,
+            "source.organizeImports": false,
+            "source.organizeImports.ruff": true
         }
     },
     "editor.formatOnSave": true,
     "evenBetterToml.formatter.alignComments": false,
     "evenBetterToml.formatter.allowedBlankLines": 2,
     "files.exclude": {
         "*.egg-info": true,
```

### Comparing `ansible-compat-4.0.2/LICENSE` & `ansible-compat-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/PKG-INFO` & `ansible-compat-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.2
+Version: 4.0.3
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.2/README.md` & `ansible-compat-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/docs/images/favicon.ico` & `ansible-compat-4.0.3/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/docs/images/logo.png` & `ansible-compat-4.0.3/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/docs/images/logo.svg` & `ansible-compat-4.0.3/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.0.3/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/mkdocs.yml` & `ansible-compat-4.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/pyproject.toml` & `ansible-compat-4.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -102,44 +102,50 @@
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
   # On purpose disabled as we rely on black
   "line-too-long",
   # local imports do not work well with pre-commit hook
   "import-error",
+  # already covered by ruff which is faster
+  "too-many-arguments", # PLR0913
   # Temporary disable duplicate detection we remove old code from prerun
   "duplicate-code",
 ]
 
 [tool.pytest.ini_options]
 # ensure we treat warnings as error
 filterwarnings = ["error"]
 
 [tool.ruff]
 select = ["ALL"]
 ignore = [
   # Disabled on purpose:
   "ANN101", # Missing type annotation for `self` in method
   "D203", # incompatible with D211
+  "D211",
   "D213", # incompatible with D212
   "E501", # we use black
   "RET504", # Unnecessary variable assignment before `return` statement
   # Temporary disabled during adoption:
   "S607", # Starting a process with a partial executable path
+  "PLR0912", # Bug https://github.com/charliermarsh/ruff/issues/4244
+  "PLR0913", # Bug https://github.com/charliermarsh/ruff/issues/4244
 
 ]
 target-version = "py39"
 
 [tool.ruff.pydocstyle]
 convention = "pep257"
 
 [tool.ruff.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
 [tool.ruff.isort]
 known-first-party = ["ansible_compat"]
+known-third-party = ["packaging"]
 
 [tool.ruff.per-file-ignores]
 "test/**/*.py" = ["SLF001", "S101", "FBT001"]
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `ansible-compat-4.0.2/requirements.txt` & `ansible-compat-4.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/src/ansible_compat/config.py` & `ansible-compat-4.0.3/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/src/ansible_compat/constants.py` & `ansible-compat-4.0.3/src/ansible_compat/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,7 +22,9 @@
 namespace: my_galaxy_namespace  # if absent, author is used instead
 
 Namespace: https://galaxy.ansible.com/docs/contributing/namespaces.html#galaxy-namespace-limitations
 Role: https://galaxy.ansible.com/docs/contributing/creating_role.html#role-names
 
 As an alternative, you can add 'role-name' to either skip_list or warn_list.
 """
+
+RC_ANSIBLE_OPTIONS_ERROR = 5
```

### Comparing `ansible-compat-4.0.2/src/ansible_compat/errors.py` & `ansible-compat-4.0.3/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/src/ansible_compat/loaders.py` & `ansible-compat-4.0.3/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/src/ansible_compat/prerun.py` & `ansible-compat-4.0.3/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/src/ansible_compat/runtime.py` & `ansible-compat-4.0.3/src/ansible_compat/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 import logging
 import os
 import re
 import shutil
 import subprocess
 import tempfile
 import warnings
+from collections import OrderedDict
+from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
-import packaging
 import subprocess_tee
 from packaging.version import Version
+from packaging.version import parse as parse_version
 
 from ansible_compat.config import (
     AnsibleConfig,
     ansible_collections_path,
     parse_ansible_version,
 )
-from ansible_compat.constants import MSG_INVALID_FQRL
+from ansible_compat.constants import MSG_INVALID_FQRL, RC_ANSIBLE_OPTIONS_ERROR
 from ansible_compat.errors import (
     AnsibleCommandError,
     AnsibleCompatError,
     InvalidPrerequisiteError,
     MissingAnsibleError,
 )
 from ansible_compat.loaders import colpath_from_path, yaml_from_file
@@ -43,24 +45,34 @@
 version_re = re.compile(":[>=<]*([^,]*)")
 
 
 class AnsibleWarning(Warning):
     """Warnings related to Ansible runtime."""
 
 
+@dataclass
+class Collection:
+    """Container for Ansible collection information."""
+
+    name: str
+    version: str
+    path: Path
+
+
+# pylint: disable=too-many-instance-attributes
 class Runtime:
     """Ansible Runtime manager."""
 
-    _version: Optional[packaging.version.Version] = None
+    _version: Optional[Version] = None
+    collections: OrderedDict[str, Collection] = OrderedDict()
     cache_dir: Optional[Path] = None
     # Used to track if we have already initialized the Ansible runtime as attempts
     # to do it multiple tilmes will cause runtime warnings from within ansible-core
     initialized: bool = False
 
-    # pylint: disable=too-many-arguments
     def __init__(
         self,
         project_dir: Optional[Path] = None,
         *,
         isolated: bool = False,
         min_required_version: Optional[str] = None,
         require_module: bool = False,
@@ -118,30 +130,72 @@
         def warning(
             self: Display,  # noqa: ARG001
             msg: str,
             *,
             formatted: bool = False,  # noqa: ARG001
         ) -> None:
             """Override ansible.utils.display.Display.warning to avoid printing warnings."""
-            warnings.warn(msg, category=AnsibleWarning, stacklevel=2)
+            warnings.warn(
+                message=msg,
+                category=AnsibleWarning,
+                stacklevel=2,
+                source={"msg": msg},
+            )
 
         # Monkey patch ansible warning in order to use warnings module.
         Display.warning = warning
 
+    def load_collections(self) -> None:
+        """Load collection data."""
+        self.collections = OrderedDict()
+        no_collections_msg = "None of the provided paths were usable"
+
+        # Workaround for https://github.com/ansible/ansible/issues/73127
+        Path("~/.ansible/collections").expanduser().mkdir(exist_ok=True, parents=True)
+
+        proc = self.run(["ansible-galaxy", "collection", "list", "--format=json"])
+        if proc.returncode == RC_ANSIBLE_OPTIONS_ERROR and (
+            no_collections_msg in proc.stdout or no_collections_msg in proc.stderr
+        ):
+            _logger.debug("Ansible reported no installed collections at all.")
+            return
+        if proc.returncode != 0:
+            _logger.error(proc)
+            msg = f"Unable to list collections: {proc}"
+            raise RuntimeError(msg)
+        data = json.loads(proc.stdout)
+        if not isinstance(data, dict):
+            msg = f"Unexpected collection data, {data}"
+            raise TypeError(msg)
+        for path in data:
+            for collection, collection_info in data[path].items():
+                if not isinstance(collection, str):
+                    msg = f"Unexpected collection data, {collection}"
+                    raise TypeError(msg)
+                if not isinstance(collection_info, dict):
+                    msg = f"Unexpected collection data, {collection_info}"
+                    raise TypeError(msg)
+
+                self.collections[collection] = Collection(
+                    name=collection,
+                    version=collection_info["version"],
+                    path=path,
+                )
+
     def _ensure_module_available(self) -> None:
         """Assure that Ansible Python module is installed and matching CLI version."""
         ansible_release_module = None
         with contextlib.suppress(ModuleNotFoundError, ImportError):
             ansible_release_module = importlib.import_module("ansible.release")
 
         if ansible_release_module is None:
             msg = "Unable to find Ansible python module."
             raise RuntimeError(msg)
 
-        ansible_module_version = packaging.version.parse(
+        ansible_module_version = parse_version(
             ansible_release_module.__version__,
         )
         if ansible_module_version != self.version:
             msg = f"Ansible CLI ({self.version}) and python module ({ansible_module_version}) versions do not match. This indicates a broken execution environment."
             raise RuntimeError(msg)
 
         # For ansible 2.15+ we need to initialize the plugin loader
@@ -171,15 +225,15 @@
             Runtime.initialized = True
 
     def clean(self) -> None:
         """Remove content of cache_dir."""
         if self.cache_dir:
             shutil.rmtree(self.cache_dir, ignore_errors=True)
 
-    def run(
+    def run(  # ruff: disable=PLR0913
         self,
         args: Union[str, list[str]],
         *,
         retry: bool = False,
         tee: bool = False,
         env: Optional[dict[str, str]] = None,
         cwd: Optional[Path] = None,
@@ -211,15 +265,15 @@
                 "Retrying execution failure %s of: %s",
                 result.returncode,
                 " ".join(args),
             )
         return result
 
     @property
-    def version(self) -> packaging.version.Version:
+    def version(self) -> Version:
         """Return current Version object for Ansible.
 
         If version is not mentioned, it returns current version as detected.
         When version argument is mentioned, it return converts the version string
         to Version object in order to make it usable in comparisons.
         """
         if self._version:
@@ -238,17 +292,17 @@
         lower: Optional[str] = None,
         upper: Optional[str] = None,
     ) -> bool:
         """Check if Ansible version is inside a required range.
 
         The lower limit is inclusive and the upper one exclusive.
         """
-        if lower and self.version < packaging.version.Version(lower):
+        if lower and self.version < Version(lower):
             return False
-        if upper and self.version >= packaging.version.Version(upper):
+        if upper and self.version >= Version(upper):
             return False
         return True
 
     def install_collection(
         self,
         collection: Union[str, Path],
         *,
@@ -322,15 +376,15 @@
                 self.install_collection(
                     str(Path(tmp_dir) / archive_file),
                     destination=destination,
                     force=True,
                 )
 
     # pylint: disable=too-many-branches
-    def install_requirements(  # noqa: C901,PLR0912
+    def install_requirements(  # noqa: C901
         self,
         requirement: Path,
         *,
         retry: bool = False,
         offline: bool = False,
     ) -> None:
         """Install dependencies from a requirements.yml.
@@ -420,17 +474,34 @@
         # are part of Tower specification
         # https://docs.ansible.com/ansible-tower/latest/html/userguide/projects.html#ansible-galaxy-support
         # https://docs.ansible.com/ansible-tower/latest/html/userguide/projects.html#collections-support
         for req_file in [
             "requirements.yml",
             "roles/requirements.yml",
             "collections/requirements.yml",
+            # These is more of less the official way to store test requirements in collections so far:
+            "tests/requirements.yml",
         ]:
             self.install_requirements(Path(req_file), retry=retry, offline=offline)
 
+        galaxy_path = Path("galaxy.yml")
+        if galaxy_path.exists():
+            data = yaml_from_file(galaxy_path)
+            if isinstance(data, dict) and "dependencies" in data:
+                for name, required_version in data["dependencies"].items():
+                    _logger.info(
+                        "Provisioning collection %s:%s from galaxy.yml",
+                        name,
+                        required_version,
+                    )
+                    self.install_collection(
+                        f"{name}:{required_version}",
+                        destination=destination,
+                    )
+
         if self.cache_dir:
             destination = self.cache_dir / "collections"
         for name, min_version in required_collections.items():
             self.install_collection(
                 f"{name}:>={min_version}",
                 destination=destination,
             )
@@ -470,14 +541,16 @@
         else:
             # no collection, try to recognize and install a standalone role
             self._install_galaxy_role(
                 self.project_dir,
                 role_name_check=role_name_check,
                 ignore_errors=True,
             )
+        # reload collections
+        self.load_collections()
 
     def require_collection(
         self,
         name: str,
         version: Optional[str] = None,
         *,
         install: bool = True,
@@ -515,18 +588,18 @@
                 if not mpath.exists():
                     msg = f"Found collection at '{collpath}' but missing MANIFEST.json, cannot get info."
                     _logger.fatal(msg)
                     raise InvalidPrerequisiteError(msg)
 
                 with mpath.open(encoding="utf-8") as f:
                     manifest = json.loads(f.read())
-                    found_version = packaging.version.parse(
+                    found_version = parse_version(
                         manifest["collection_info"]["version"],
                     )
-                    if version and found_version < packaging.version.parse(version):
+                    if version and found_version < parse_version(version):
                         if install:
                             self.install_collection(f"{name}:>={version}")
                             self.require_collection(name, version, install=False)
                         else:
                             msg = f"Found {name} collection {found_version} but {version} or newer is required."
                             _logger.fatal(msg)
                             raise InvalidPrerequisiteError(msg)
```

### Comparing `ansible-compat-4.0.2/src/ansible_compat/schema.py` & `ansible-compat-4.0.3/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/src/ansible_compat/types.py` & `ansible-compat-4.0.3/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.0.3/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.2
+Version: 4.0.3
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.2/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.0.3/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -64,13 +64,14 @@
 test/collections/acme.broken/galaxy.yml
 test/collections/acme.goodies/galaxy.yml
 test/collections/acme.goodies/molecule/default/converge.yml
 test/collections/acme.goodies/molecule/default/molecule.yml
 test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
 test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
 test/collections/acme.goodies/roles/baz/tasks/main.yml
+test/collections/acme.goodies/tests/requirements.yml
 test/roles/acme.missing_deps/requirements.yml
 test/roles/acme.missing_deps/meta/main.yml
 test/roles/acme.sample2/meta/main.yml
 test/roles/ansible-role-sample/meta/main.yml
 test/roles/sample3/meta/main.yml
 test/roles/sample4/meta/main.yml
```

### Comparing `ansible-compat-4.0.2/test/assets/validate0_expected.json` & `ansible-compat-4.0.3/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/test/conftest.py` & `ansible-compat-4.0.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/test/test_config.py` & `ansible-compat-4.0.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/test/test_runtime.py` & `ansible-compat-4.0.3/test/test_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,22 +631,35 @@
 ) -> None:
     """Validate functioning of version_in_range."""
     runtime = Runtime()
     assert runtime.version_in_range(lower=lower, upper=upper) is expected
 
 
 @pytest.mark.parametrize(
-    ("path", "scenario"),
+    ("path", "scenario", "expected_collections"),
     (
-        ("test/collections/acme.goodies", "default"),
-        ("test/collections/acme.goodies/roles/baz", "deep_scenario"),
+        pytest.param(
+            "test/collections/acme.goodies",
+            "default",
+            ["ansible.posix"],
+            id="normal",
+        ),
+        pytest.param(
+            "test/collections/acme.goodies/roles/baz",
+            "deep_scenario",
+            ["community.molecule"],
+            id="deep",
+        ),
     ),
-    ids=("normal", "deep"),
 )
-def test_install_collection_from_disk(path: str, scenario: str) -> None:
+def test_install_collection_from_disk(
+    path: str,
+    scenario: str,
+    expected_collections: list[str],
+) -> None:
     """Tests ability to install a local collection."""
     # ensure we do not have acme.google installed in user directory as it may
     # produce false positives
     rmtree(
         pathlib.Path(
             "~/.ansible/collections/ansible_collections/acme/goodies",
         ).expanduser(),
@@ -656,14 +669,19 @@
         runtime = Runtime(isolated=True)
         # this should call install_collection_from_disk(".")
         runtime.prepare_environment(install_local=True)
         # that molecule converge playbook can be used without molecule and
         # should validate that the installed collection is available.
         result = runtime.run(["ansible-playbook", f"molecule/{scenario}/converge.yml"])
         assert result.returncode == 0, result.stdout
+        runtime.load_collections()
+        for collection_name in expected_collections:
+            assert (
+                collection_name in runtime.collections
+            ), f"{collection_name} not found in {runtime.collections.keys()}"
         runtime.clean()
 
 
 def test_install_collection_from_disk_fail() -> None:
     """Tests that we fail to install a broken collection."""
     with cwd(Path("test/collections/acme.broken")):
         runtime = Runtime(isolated=True)
```

### Comparing `ansible-compat-4.0.2/test/test_runtime_example.py` & `ansible-compat-4.0.3/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/test/test_schema.py` & `ansible-compat-4.0.3/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.2/tox.ini` & `ansible-compat-4.0.3/tox.ini`

 * *Files identical despite different names*

