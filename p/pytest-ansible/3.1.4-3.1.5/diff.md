# Comparing `tmp/pytest-ansible-3.1.4.tar.gz` & `tmp/pytest-ansible-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ansible-3.1.4.tar", last modified: Thu May 11 12:37:14 2023, max compression
+gzip compressed data, was "pytest-ansible-3.1.5.tar", last modified: Mon May 15 20:06:18 2023, max compression
```

## Comparing `pytest-ansible-3.1.4.tar` & `pytest-ansible-3.1.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.694323 pytest-ansible-3.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.674323 pytest-ansible-3.1.4/.config/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.678323 pytest-ansible-3.1.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.678323 pytest-ansible-3.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.678323 pytest-ansible-3.1.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-05-11 12:37:14.694323 pytest-ansible-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/inventory
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:37:14.694323 pytest-ansible-3.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.670323 pytest-ansible-3.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.682323 pytest-ansible-3.1.4/src/pytest_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 12:37:14.000000 pytest-ansible-3.1.4/src/pytest_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/has_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.686323 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v29.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.690323 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v29.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/src/pytest_ansible/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.682323 pytest-ansible-3.1.4/src/pytest_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-05-11 12:37:14.000000 pytest-ansible-3.1.4/src/pytest_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-11 12:37:14.000000 pytest-ansible-3.1.4/src/pytest_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:37:14.000000 pytest-ansible-3.1.4/src/pytest_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 12:37:14.000000 pytest-ansible-3.1.4/src/pytest_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-11 12:37:14.000000 pytest-ansible-3.1.4/src/pytest_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 12:37:14.000000 pytest-ansible-3.1.4/src/pytest_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.694323 pytest-ansible-3.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/test_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/test_adhoc_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/test_host_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/test_module_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/test_module_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:37:14.694323 pytest-ansible-3.1.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tests/unit/test_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-11 12:36:58.000000 pytest-ansible-3.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.706703 pytest-ansible-3.1.5/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.706703 pytest-ansible-3.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.706703 pytest-ansible-3.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.706703 pytest-ansible-3.1.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/inventory
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.698703 pytest-ansible-3.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.710703 pytest-ansible-3.1.5/src/pytest_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/has_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.714703 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v29.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.718703 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v29.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.714703 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_adhoc_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_host_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_module_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_module_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/unit/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tox.ini
```

### Comparing `pytest-ansible-3.1.4/.flake8` & `pytest-ansible-3.1.5/.flake8`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/.github/workflows/release.yml` & `pytest-ansible-3.1.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/.github/workflows/tox.yml` & `pytest-ansible-3.1.5/.github/workflows/tox.yml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     outputs:
       matrix: ${{ steps.generate_matrix.outputs.matrix }}
     steps:
       - name: Determine matrix
         id: generate_matrix
         uses: coactions/dynamic-matrix@v1
         with:
-          min_python: "3.8"
+          min_python: "3.7"
           max_python: "3.11"
           other_names: |
             lint
             pkg
             devel
           platforms: linux
```

### Comparing `pytest-ansible-3.1.4/.gitignore` & `pytest-ansible-3.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/.pre-commit-config.yaml` & `pytest-ansible-3.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/HISTORY.md` & `pytest-ansible-3.1.5/HISTORY.md`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/LICENSE` & `pytest-ansible-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/PKG-INFO` & `pytest-ansible-3.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.1.4
+Version: 3.1.5
 Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
@@ -15,19 +15,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lock
 License-File: LICENSE
 
 # pytest-ansible
```

### Comparing `pytest-ansible-3.1.4/README.md` & `pytest-ansible-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/inventory` & `pytest-ansible-3.1.5/inventory`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/pyproject.toml` & `pytest-ansible-3.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "setuptools_scm[toml] >= 7.0.5", # required for "no-local-version" scheme
 
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 # https://peps.python.org/pep-0621/#readme
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 dynamic = ["version", "dependencies", "optional-dependencies"]
 name = "pytest-ansible"
 description = "Plugin for pytest to simplify calling ansible modules from tests or fixtures"
 readme = "README.md"
 authors = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 maintainers = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 license = { text = "MIT" }
@@ -22,14 +22,15 @@
   'License :: OSI Approved :: MIT License',
   'Operating System :: OS Independent',
   'Topic :: Software Development :: Testing',
   'Topic :: Software Development :: Quality Assurance',
   'Topic :: Utilities',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3',
+  'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
 ]
 keywords = ["ansible", "testing", "pytest"]
 
@@ -129,15 +130,15 @@
   "S",
   "SLF",
   "T",
   "TRY",
   "PTH",
   "TCH",
 ]
-target-version = "py38"
+target-version = "py37"
 # Same as Black.
 line-length = 88
 
 [tool.ruff.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
 [tool.ruff.per-file-ignores]
```

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/errors.py` & `pytest-ansible-3.1.5/src/pytest_ansible/errors.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/fixtures.py` & `pytest-ansible-3.1.5/src/pytest_ansible/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/has_version.py` & `pytest-ansible-3.1.5/src/pytest_ansible/has_version.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/host_manager/__init__.py` & `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v1.py` & `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v1.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v2.py` & `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v2.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v212.py` & `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v212.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v213.py` & `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v213.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v24.py` & `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v24.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v28.py` & `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v28.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/host_manager/v29.py` & `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v29.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/__init__.py` & `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v1.py` & `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v1.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v2.py` & `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v2.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v212.py` & `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v212.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v213.py` & `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v213.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v24.py` & `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v24.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v28.py` & `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v28.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/module_dispatcher/v29.py` & `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v29.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/plugin.py` & `pytest-ansible-3.1.5/src/pytest_ansible/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/results.py` & `pytest-ansible-3.1.5/src/pytest_ansible/results.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible/units.py` & `pytest-ansible-3.1.5/src/pytest_ansible/units.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible.egg-info/PKG-INFO` & `pytest-ansible-3.1.5/src/pytest_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.1.4
+Version: 3.1.5
 Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
@@ -15,19 +15,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lock
 License-File: LICENSE
 
 # pytest-ansible
```

### Comparing `pytest-ansible-3.1.4/src/pytest_ansible.egg-info/SOURCES.txt` & `pytest-ansible-3.1.5/src/pytest_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/conftest.py` & `pytest-ansible-3.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/test_adhoc.py` & `pytest-ansible-3.1.5/tests/test_adhoc.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/test_adhoc_result.py` & `pytest-ansible-3.1.5/tests/test_adhoc_result.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/test_fixtures.py` & `pytest-ansible-3.1.5/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/test_host_manager.py` & `pytest-ansible-3.1.5/tests/test_host_manager.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/test_module_dispatcher.py` & `pytest-ansible-3.1.5/tests/test_module_dispatcher.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/test_module_result.py` & `pytest-ansible-3.1.5/tests/test_module_result.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/test_params.py` & `pytest-ansible-3.1.5/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tests/unit/test_unit.py` & `pytest-ansible-3.1.5/tests/unit/test_unit.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.4/tox.ini` & `pytest-ansible-3.1.5/tox.ini`

 * *Files identical despite different names*

