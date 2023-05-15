# Comparing `tmp/ansible-compat-4.0.3.tar.gz` & `tmp/ansible-compat-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.0.3.tar", last modified: Mon May 15 15:05:25 2023, max compression
+gzip compressed data, was "ansible-compat-4.0.4.tar", last modified: Mon May 15 16:44:56 2023, max compression
```

## Comparing `ansible-compat-4.0.3.tar` & `ansible-compat-4.0.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.486543 ansible-compat-4.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.470543 ansible-compat-4.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.490543 ansible-compat-4.0.3/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.494543 ansible-compat-4.0.3/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.474543 ansible-compat-4.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.498543 ansible-compat-4.0.3/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31373 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.498543 ansible-compat-4.0.3/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 15:05:25.000000 ansible-compat-4.0.3/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.502543 ansible-compat-4.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.474543 ansible-compat-4.0.3/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.474543 ansible-compat-4.0.3/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.474543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/roles/baz/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.506543 ansible-compat-4.0.3/test/collections/acme.goodies/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/collections/acme.goodies/tests/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.482543 ansible-compat-4.0.3/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.478543 ansible-compat-4.0.3/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.482543 ansible-compat-4.0.3/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:05:25.510543 ansible-compat-4.0.3/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    25019 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-15 15:05:08.000000 ansible-compat-4.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.000491 ansible-compat-4.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.988491 ansible-compat-4.0.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.988491 ansible-compat-4.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.012491 ansible-compat-4.0.4/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31718 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.012491 ansible-compat-4.0.4/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.016491 ansible-compat-4.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.016491 ansible-compat-4.0.4/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/tests/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.996491 ansible-compat-4.0.4/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25190 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/tox.ini
```

### Comparing `ansible-compat-4.0.3/.github/dependabot.yml` & `ansible-compat-4.0.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/.github/workflows/release.yml` & `ansible-compat-4.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/.github/workflows/tox.yml` & `ansible-compat-4.0.4/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/.gitignore` & `ansible-compat-4.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/.pre-commit-config.yaml` & `ansible-compat-4.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/.readthedocs.yml` & `ansible-compat-4.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/.vscode/settings.json` & `ansible-compat-4.0.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/LICENSE` & `ansible-compat-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/PKG-INFO` & `ansible-compat-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.3
+Version: 4.0.4
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.3/README.md` & `ansible-compat-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/docs/images/favicon.ico` & `ansible-compat-4.0.4/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/docs/images/logo.png` & `ansible-compat-4.0.4/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/docs/images/logo.svg` & `ansible-compat-4.0.4/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.0.4/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/mkdocs.yml` & `ansible-compat-4.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/pyproject.toml` & `ansible-compat-4.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/requirements.txt` & `ansible-compat-4.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/src/ansible_compat/config.py` & `ansible-compat-4.0.4/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/src/ansible_compat/constants.py` & `ansible-compat-4.0.4/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/src/ansible_compat/errors.py` & `ansible-compat-4.0.4/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/src/ansible_compat/loaders.py` & `ansible-compat-4.0.4/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/src/ansible_compat/prerun.py` & `ansible-compat-4.0.4/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/src/ansible_compat/runtime.py` & `ansible-compat-4.0.4/src/ansible_compat/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from collections import OrderedDict
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import subprocess_tee
 from packaging.version import Version
-from packaging.version import parse as parse_version
 
 from ansible_compat.config import (
     AnsibleConfig,
     ansible_collections_path,
     parse_ansible_version,
 )
 from ansible_compat.constants import MSG_INVALID_FQRL, RC_ANSIBLE_OPTIONS_ERROR
@@ -54,14 +53,26 @@
     """Container for Ansible collection information."""
 
     name: str
     version: str
     path: Path
 
 
+class CollectionVersion(Version):
+    """Collection version."""
+
+    def __init__(self, version: str) -> None:
+        """Initialize collection version."""
+        # As packaging Version class does not support wildcard, we convert it
+        # to "0", as this being the smallest version possible.
+        if version == "*":
+            version = "0"
+        super().__init__(version)
+
+
 # pylint: disable=too-many-instance-attributes
 class Runtime:
     """Ansible Runtime manager."""
 
     _version: Optional[Version] = None
     collections: OrderedDict[str, Collection] = OrderedDict()
     cache_dir: Optional[Path] = None
@@ -187,15 +198,15 @@
         with contextlib.suppress(ModuleNotFoundError, ImportError):
             ansible_release_module = importlib.import_module("ansible.release")
 
         if ansible_release_module is None:
             msg = "Unable to find Ansible python module."
             raise RuntimeError(msg)
 
-        ansible_module_version = parse_version(
+        ansible_module_version = Version(
             ansible_release_module.__version__,
         )
         if ansible_module_version != self.version:
             msg = f"Ansible CLI ({self.version}) and python module ({ansible_module_version}) versions do not match. This indicates a broken execution environment."
             raise RuntimeError(msg)
 
         # For ansible 2.15+ we need to initialize the plugin loader
@@ -322,15 +333,15 @@
         if force:
             cmd.append("--force")
 
         # As ansible-galaxy install is not able to automatically determine
         # if the range requires a pre-release, we need to manuall add the --pre
         # flag when needed.
         matches = version_re.search(str(collection))
-        if matches and Version(matches[1]).is_prerelease:
+        if matches and CollectionVersion(matches[1]).is_prerelease:
             cmd.append("--pre")
 
         cpaths: list[str] = self.config.collections_paths
         if destination and str(destination) not in cpaths:
             # we cannot use '-p' because it breaks galaxy ability to ignore already installed collections, so
             # we hack ansible_collections_path instead and inject our own path there.
             # pylint: disable=no-member
@@ -588,18 +599,18 @@
                 if not mpath.exists():
                     msg = f"Found collection at '{collpath}' but missing MANIFEST.json, cannot get info."
                     _logger.fatal(msg)
                     raise InvalidPrerequisiteError(msg)
 
                 with mpath.open(encoding="utf-8") as f:
                     manifest = json.loads(f.read())
-                    found_version = parse_version(
+                    found_version = CollectionVersion(
                         manifest["collection_info"]["version"],
                     )
-                    if version and found_version < parse_version(version):
+                    if version and found_version < CollectionVersion(version):
                         if install:
                             self.install_collection(f"{name}:>={version}")
                             self.require_collection(name, version, install=False)
                         else:
                             msg = f"Found {name} collection {found_version} but {version} or newer is required."
                             _logger.fatal(msg)
                             raise InvalidPrerequisiteError(msg)
```

### Comparing `ansible-compat-4.0.3/src/ansible_compat/schema.py` & `ansible-compat-4.0.4/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/src/ansible_compat/types.py` & `ansible-compat-4.0.4/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.0.4/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.3
+Version: 4.0.4
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.3/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.0.4/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/test/assets/validate0_expected.json` & `ansible-compat-4.0.4/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/test/conftest.py` & `ansible-compat-4.0.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/test/test_config.py` & `ansible-compat-4.0.4/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/test/test_runtime.py` & `ansible-compat-4.0.4/test/test_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,15 +636,19 @@
 
 @pytest.mark.parametrize(
     ("path", "scenario", "expected_collections"),
     (
         pytest.param(
             "test/collections/acme.goodies",
             "default",
-            ["ansible.posix"],
+            [
+                "ansible.posix",  # from tests/requirements.yml
+                "ansible.utils",  # from galaxy.yml
+                "community.molecule",  # from galaxy.yml
+            ],
             id="normal",
         ),
         pytest.param(
             "test/collections/acme.goodies/roles/baz",
             "deep_scenario",
             ["community.molecule"],
             id="deep",
```

### Comparing `ansible-compat-4.0.3/test/test_runtime_example.py` & `ansible-compat-4.0.4/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/test/test_schema.py` & `ansible-compat-4.0.4/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.3/tox.ini` & `ansible-compat-4.0.4/tox.ini`

 * *Files identical despite different names*

